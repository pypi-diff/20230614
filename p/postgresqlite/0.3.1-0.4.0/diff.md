# Comparing `tmp/postgresqlite-0.3.1.tar.gz` & `tmp/postgresqlite-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgresqlite-0.3.1.tar", max compression
+gzip compressed data, was "postgresqlite-0.4.0.tar", max compression
```

## Comparing `postgresqlite-0.3.1.tar` & `postgresqlite-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    15193 2022-10-11 12:02:33.616396 postgresqlite-0.3.1/README.md
--rw-r--r--   0        0        0    18214 2022-10-12 06:57:39.467241 postgresqlite-0.3.1/postgresqlite/__init__.py
--rw-r--r--   0        0        0       27 2022-10-11 14:59:26.513207 postgresqlite-0.3.1/postgresqlite/__main__.py
--rw-r--r--   0        0        0      822 2022-10-12 06:58:12.043422 postgresqlite-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    16475 1970-01-01 00:00:00.000000 postgresqlite-0.3.1/setup.py
--rw-r--r--   0        0        0    16183 1970-01-01 00:00:00.000000 postgresqlite-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    15321 2023-06-14 10:26:48.369503 postgresqlite-0.4.0/README.md
+-rw-r--r--   0        0        0    19589 2023-06-14 12:09:40.681821 postgresqlite-0.4.0/postgresqlite/__init__.py
+-rw-r--r--   0        0        0       27 2022-10-12 06:58:47.552893 postgresqlite-0.4.0/postgresqlite/__main__.py
+-rw-r--r--   0        0        0      822 2023-06-14 10:25:07.819763 postgresqlite-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    16362 1970-01-01 00:00:00.000000 postgresqlite-0.4.0/PKG-INFO
```

### Comparing `postgresqlite-0.3.1/README.md` & `postgresqlite-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,15 @@
 ### The `FriendlyConnection` object
 
 By default the `postgresqlite.connect` method will return a `FriendlyConnection`, which is a DB-API compatible `Connection` object, but with a few programmer-friendly differences:
 
 - Row objects can be indexed using column names as well as column indexes. For example `row['name']` instead of `row[0]`. In addition, attribute syntax can be used, like `row.name`.
 - Autocommit mode is enabled by default.
 - Query parameters are in `:named` style.
+- Exceptions are instances of `SQLError` and contain easy to read error messages, highlighting the offending part of the query.
 
 Besides, those changes, the `FriendlyConnection` object offers a couple of additional methods:
 
 #### execute(sql: str, params: dict = {})
 
 Create a new `Cursor`, execute the given `sql` with the given `params` dictionary on that cursor, and return the `Cursor`. Example:
```

### Comparing `postgresqlite-0.3.1/postgresqlite/__init__.py` & `postgresqlite-0.4.0/postgresqlite/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, string, random, json, sys, subprocess, fcntl, time, traceback, socket, urllib.request, urllib.error, tarfile, pg8000, pg8000.dbapi, glob
+import os, string, random, json, sys, subprocess, fcntl, time, traceback, socket, urllib.request, urllib.error, tarfile, pg8000, pg8000.dbapi, glob, re
 
 
 class FriendlyConnection(pg8000.dbapi.Connection):
     def cursor(self):
         return FriendlyCursor(self)
 
     def execute(self, *args, **kwargs):
@@ -31,23 +31,57 @@
     def query_column(self, sql, **kwparams):
         cursor = self.cursor()
         result = cursor.query_column(sql, **kwparams)
         cursor.close()
         return result
 
 
+mark_start = "\u001b[31m"
+mark_end = "\u001b[0m"
+
+def get_exception_message(query, args, org_exception):
+    msg = str(org_exception)
+    
+    match_m = re.search("'M': '((\\\\.|[^'])+)'", msg) # message
+    if match_m:
+        match_h = re.search("'H': '((\\\\.|[^'])+)'", msg) # hint
+        match_p = re.search("'P': '((\\\\.|[^'])+)'", msg) # position
+        msg = match_m.group(1)
+        msg = msg[0].upper() + msg[1:] + "."
+        if match_h:
+            msg += f"\nHint: {match_h.group(1)}"
+        if match_p and match_p.group(1).isdigit():
+            # Make the error position in the query red
+            start_pos = int(match_p.group(1))-1
+            match_word = re.search('^[a-zA-Z_.]+|[^a-zA-Z_.]+', query[start_pos:])
+            if match_word and match_word.group(0).strip():
+                end_pos = start_pos + len(match_word.group(0))
+            else:
+                query = query[:start_pos] + "⚠" + query[start_pos:]
+                end_pos = start_pos + 1
+            query = query[0:start_pos] + self.mark_start  + query[start_pos:end_pos] + self.mark_end + query[end_pos:]
+
+    msg = f"{msg}\nFor query:\n\t" + query.replace("\n","\n\t")
+    if args:
+        msg += f"\nWith arguments: {args}"
+    return msg
+
+
 class FriendlyCursor(pg8000.dbapi.Cursor):
-    def execute(self, *args, **kwargs):
+    def execute(self, sql, kwparams):
         self._lookup = None
         org_paramstyle = pg8000.dbapi.paramstyle
         pg8000.dbapi.paramstyle = self._c._paramstyle
         try:
-            super().execute(*args, **kwargs)
+            super().execute(sql, kwparams)
             if self.description:
                 self._lookup = {info[0]: index for index, info in enumerate(self.description)}
+        except Exception as e:
+            msg = get_exception_message(sql, kwparams, e)
+            raise type(e)(msg) from None
         finally:
             pg8000.dbapi.paramstyle = org_paramstyle
 
     def __next__(self):
         data = super().__next__()
         return FriendlyRow(data, self._lookup)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `postgresqlite-0.3.1/pyproject.toml` & `postgresqlite-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "postgresqlite"
-version = "0.3.1"
+version = "0.4.0"
 description = "Python package that gives you the power of a PostgreSQL server, with the convenience of the sqlite3 package."
 authors = ["Frank van Viegen <pp@vanviegen.net>"]
 readme = "README.md"
 repository = "https://github.com/vanviegen/postgresqlite"
 documentation = "https://github.com/vanviegen/postgresqlite/blob/master/README.md#Documentation"
 classifiers = [
     'Development Status :: 4 - Beta',
```

### Comparing `postgresqlite-0.3.1/setup.py` & `postgresqlite-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,339 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: postgresqlite
+Version: 0.4.0
+Summary: Python package that gives you the power of a PostgreSQL server, with the convenience of the sqlite3 package.
+Home-page: https://github.com/vanviegen/postgresqlite
+Author: Frank van Viegen
+Author-email: pp@vanviegen.net
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Database
+Requires-Dist: pg8000 (>=1.24.1,<2.0.0)
+Project-URL: Documentation, https://github.com/vanviegen/postgresqlite/blob/master/README.md#Documentation
+Project-URL: Repository, https://github.com/vanviegen/postgresqlite
+Description-Content-Type: text/markdown
 
-packages = \
-['postgresqlite']
+# PostgreSQLite
 
-package_data = \
-{'': ['*']}
+Python module that gives you the power of a PostgreSQL server, with the convenience of the `sqlite3` module.
 
-install_requires = \
-['pg8000>=1.24.1,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['postgresqlite = postgresqlite:main']}
-
-setup_kwargs = {
-    'name': 'postgresqlite',
-    'version': '0.3.1',
-    'description': 'Python package that gives you the power of a PostgreSQL server, with the convenience of the sqlite3 package.',
-    'long_description': '# PostgreSQLite\n\nPython module that gives you the power of a PostgreSQL server, with the convenience of the `sqlite3` module.\n\n## Features\n\n- Using just a `postgresqlite.connect()` call, the library will automatically...\n    - Download and install PostgreSQL into the user\'s `~/.cache` directory. (Linux and macOS EM64T only, for now.)\n    - Create a new database (`initdb`) within the project directory with a random password.\n    - Start the PostgreSQL server.\n    - Set up a DB-API connection to the server (using the `pg8000` driver).\n    - Shut down the server when it\'s no longer in use.\n- It also adds a couple of conveniences on top of DB-API, making it more similar to the `sqlite3` module:\n    - Calling `execute` on the connection will create a new cursor.\n    - Calls to `fetchall` and `fetchone` return objects that can address fields both by number (as is standard for DB-API) as well as by name (as `sqlite3` offers when you configure `connection.row_factory = sqlite3.Row`).\n    - Autocommit mode is enabled by default.\n    - Parameterized queries use `?` as a placeholder. (`paramstyle = \'qmark\'`)\n- It can open `psql` and other PostgreSQL clients passing in connection details, while making sure the database is running.\n- For use in production, the configuration file can be modified to point your application at a (non-auto-starting) PostgreSQL server.\n\n\n## Examples\n\n### Using DB-API directly\n\n```sh\npip install postgresqlite\n```\n\n```python\nimport postgresqlite\n\ndb = postgresqlite.connect(mode=\'dbapi\')\n\ncursor = db.cursor()\ncursor.execute(\'create table if not exists tests(id serial, info text not null, created_at timestamp not null default current_timestamp)\')\ncursor.execute("insert into tests(info) values(\'Hi mom!\'),(\'This is great!\')")\ndb.commit()\n\ncursor.execute("select id, info, created_at from tests where id=%s", [1])\nfor row in cursor:\n    print("row:", row, "id:", row[0], "created_at:", row[2])\n\ncursor.execute("select count(*) from tests")\nprint("count:", cursor.fetchone()[0])\n\ncursor.execute("select * from tests order by id desc limit 1")\nprint("row:", cursor.fetchone())\n```\n\n### Using the `FriendlyConnection` API\n\n```sh\npip install postgresqlite\n```\n\n```python\nimport postgresqlite\n\ndb = postgresqlite.connect()\n\ndb.query(\'create table if not exists tests(id serial, info text not null, created_at timestamp not null default current_timestamp)\')\ndb.query("insert into tests(info) values(\'Hi mom!\'),(\'This is great!\')")\n\nrows = db.query("select * from tests where id=:id", id=1)\nfor row in rows:\n    print("row:", row, "id:", row.id, "created_at:", row.created_at)\n\nprint("count:", db.query_value("select count(*) from tests"))\n\nprint("last row:", db.query_row("select * from tests order by id desc limit 1"))\n```\n\n### Using Flask-SQLAlchemy\n\n```sh\npip install postgresqlite flask_sqlalchemy\n```\n\n```python\nimport postgresqlite, flask, flask_sqlalchemy, datetime\n\napp = flask.Flask(__name__)\napp.config[\'SQLALCHEMY_DATABASE_URI\'] = postgresqlite.get_uri()\napp.config[\'SQLALCHEMY_TRACK_MODIFICATIONS\'] = False\n\ndb = flask_sqlalchemy.SQLAlchemy(app)\n\nclass Car(db.Model):\n    id = db.Column(db.Integer, primary_key=True)\n    brand = db.Column(db.String)\n    model = db.Column(db.String, nullable=False)\n    day_rate = db.Column(db.Integer)\n    rentals = db.relationship(\'Rental\', backref=\'car\')\n\n    def to_dict(self):\n        return {\'id\': self.id, \'brand\': self.brand, \'model\': self.model, \'day_rate\': self.day_rate, \'rentals\': [rental.to_dict() for rental in self.rentals]}\n    \nclass Rental(db.Model):\n    id = db.Column(db.Integer, primary_key=True)\n    car_id = db.Column(db.Integer, db.ForeignKey(\'car.id\'), nullable=False)\n\n    customer_name = db.Column(db.String, nullable=False)\n    start_time = db.Column(db.DateTime, default=datetime.datetime.now)\n    end_time = db.Column(db.DateTime)\n\n    def to_dict(self):\n        return {\'id\': self.id, \'car_id\': self.car_id, \'customer_name\': self.customer_name, \'start_time\': self.start_time, \'end_time\': self.end_time}\n\n@app.route(\'/cars\')\ndef show_all():\n   return flask.jsonify([car.to_dict() for car in Car.query.all()])\n\n@app.route(\'/cars\', methods = [\'POST\'])\ndef new_car():\n    car = Car(**flask.request.get_json())\n    db.session.add(car)\n    db.session.commit()\n    return flask.jsonify(car.to_dict())\n\n@app.route(\'/rentals\', methods = [\'POST\'])\ndef new_rental():\n    rental = Rental(**flask.request.get_json())\n    db.session.add(rental)\n    db.session.commit()\n    return flask.jsonify(rental.to_dict())\n\n# Create tables based on the Model classes above.\nwith app.app_context():\n    db.create_all()\n\nif __name__ == \'__main__\':\n    app.run(debug = True)\n```\n\nRunning this should expose a REST API. If you have [httpie](https://httpie.io/) installed, it can be tested from the command like this:\n\n```sh\nhttp http://127.0.0.1:5000/cars brand=Volvo model=S60\nhttp http://127.0.0.1:5000/rentals car_id=1 customer_name=Frank\nhttp http://127.0.0.1:5000/cars\n```\n\n\n\n## Documentation\n\n### API functions\n\n#### `postgresqlite.connect(dirname=\'data/postgresqlite\', mode=\'friendly\', config=None)`\n\nStart a server (if needed), wait for it, and return a DB-API compatible object.\n\nArguments:\n- `dirname` (str): The dir where the configuration file (`postgresqlite.json`)\n    will be read or created, and where database files will be stored. If the\n    path does not exist, it will be created.\n- `mode` (\'easy\', \'sqlite\', \'dbapi\'): \n  - When set to `friendly` (the default), a `FriendlyConnection` object is returned. It\'s a DB-API compatible Connection, but with a few additions to make it more programmer-friendly, as documented in the [The FriendlyConnection object](#the-friendlyconnection-object)-section.\n  - When set to \'dbapi\', the created connection will be a plain PG8000 DB-API Connection.\n  - When set to \'sqlite3\', a few (superficial) additions are added on top of the DB-API to make it resemble the Python `sqlite3` API more closely:\n    - `Connection` objects have an `execute` method that creates a new cursor and \n        runs the given query on it.\n    - Row objects can be indexed using numeric indexes as well as column names,\n        just like (like with `connection.row_factory = sqlite3.Row` for `sqlite3`).\n    - Autocommit mode is enabled by default.\n    - Parameterized queries use `?` as a placeholder. (`paramstyle = \'qmark\'`)\n- `config` (Config | None): An object obtained through `get_config()` can be given to configure the connection. This causes `dirname` to be ignored.\n\nArguments:\n- dirname (str, defaults to `data/postgresqlite`): The directory where the configuration file (`postgresqlite.json`) will be read or created, and where database files will be stored. If the path does not exist, it will be created.\n- sqlite_compatible (bool, defaults to `True`): When set, a few (superficial) changes are made to the exposed DB-API to make it resemble the Python `sqlite3` API more closely, as described in the *Features* section.\n- config (`Config` object, defaults to `None`): This can be an object returned by `get_config`. When `None`, the `connect` method will create a default configuration.\n\nReturns a [DB-API compatible connection object](https://peps.python.org/pep-0249/#connection-objects).\n\n#### `postgresqlite.get_config(dirname=\'data/postgresqlite\')`\n\nStart a server (if needed), wait for it, and return the config object. If the PostgreSQL server is in autostart mode (which is the default), it will be kept running until some time after the calling process (and any other processes that depend on this server) have terminated.\n \nArguments:\n- dirname (str): The directory where the configuration file (`postgresqlite.json`) will be read or created, and where database files will be stored. If the path does not exist, it will be created.\n\nReturns a `Config` object, that includes (among others) the following attributes:\n- `user` (string): Database user name.\n- `password` (string): Database password. (Can be `None`.)\n- `port` (int): Database TCP port. (Can be `None`.)\n- `host` (string): Database host name. (Can be `None`.)\n- `database` (string): Database name.\n- `socket` (string): Database UNIX domain socket. (Can be `None`.)\n- `env` (dict): A dictionary containing `PGHOST`, `PGPORT`, `PGDATABASE`, `PGSOCKET`, `PGUSER`, `PGPASSWORD` and `PGURI` keys with their appropriate values.\n\n#### `postgresqlite.get_uri(dirname=\'data/postgresqlite\', driver=\'pg8000\')`\nStart a server (if needed), wait for it, and return a connection URL.\n\nArguments:\n- dirname (str): The directory where the configuration file (`postgresqlite.json`) will be read or created, and where database files will be stored. If the path does not exist, it will be created.\n- driver (str): The URI may include a driver part (`postgresql+DRIVER://user:pwd@host/db`), which we\'ll set to `pg8000` by default. This parameter allows you to specify a different direct, or leave it out (by providing `None`).\n\n### The `FriendlyConnection` object\n\nBy default the `postgresqlite.connect` method will return a `FriendlyConnection`, which is a DB-API compatible `Connection` object, but with a few programmer-friendly differences:\n\n- Row objects can be indexed using column names as well as column indexes. For example `row[\'name\']` instead of `row[0]`. In addition, attribute syntax can be used, like `row.name`.\n- Autocommit mode is enabled by default.\n- Query parameters are in `:named` style.\n\nBesides, those changes, the `FriendlyConnection` object offers a couple of additional methods:\n\n#### execute(sql: str, params: dict = {})\n\nCreate a new `Cursor`, execute the given `sql` with the given `params` dictionary on that cursor, and return the `Cursor`. Example:\n\n```python\nrow = db.execute(\'select * from test where id=:id\', {\'id\': 123})).fetchone()`\n```\n\n#### query(sql, param1=.., param2=..)\n\nExecute the `sql` with the given parameters, returning a list of `FriendlyRow` objects. Example:\n\n```python\nrows = db.query(\'select id, name from test where name=:name\', name=\'Ivo\')\nprint(len(rows), rows[0].id) # 3 123\n```\n\n#### query_row(sql, param1=.., param2=..)\n\nExecute the `sql` with the given parameters, returning a single `FriendlyRow` object or `None` (if no rows were returned). If the query results in more than one row, an exception is thrown. Example:\n\n```python\nrow = db.query_row(\'select id, name from test where id=:id\', id=123)\nprint(row.id, row.name) # 123 Ivo\n```\n\n#### query_column(sql, param1=.., param2=..)\n\nExecute the `sql` with the given parameters, returning a list of values. If the query results in more than one column, an exception is thrown. Example:\n\n```python\ntest_ids = db.query_column(\'select id from test where name=:name\', name=\'Ivo\')\nprint(test_ids) # [123, 456, 789]\n```\n\n#### query_value(sql, param1=.., param2=..)\n\nExecute the `sql` with the given parameters, returning a single value. If the query results in more than one column or more than one row, an exception is thrown. Example:\n\n```python\ntest_id = db.query_value(\'select id from test where name=:name limit 1\', name=\'Ivo\')\nprint(test_id) # 123\n```\n\n\n### CLI interface\n\nIn order to easily access the database your application is using, PostgreSQLite can open a client application (such as *psql* or [Beekeeper Studio](https://www.beekeeperstudio.io/)) for you, making sure the database is started (and doesn\'t shutdown) while the application is open, and passing in connection details.\n\nThe connection details are provided in environment variables called `PGHOST`, `PGPORT`, `PGDATABASE`, `PGSOCKET`, `PGUSER`, `PGPASSWORD` and `PGURI`. \n\nAn application can be started by running the `postgresqlite` package with `-m`, providing the executable and its arguments as arguments.\n- When no arguments are passed: `psql`, the default PostgreSQL client, is run. So opening your database in `psql` can be done like this:\n  ```sh\n  python -mpostgresqlite\n  ```\n  The `psql` client uses the environment variables to set up a connection.\n- When exactly one argument is passed and it contains the string `$PG`, it will be executed as a shell command. So in order to pass the URI as the argument to an application, one could use:\n  ```sh\n  python -mpostgresqlite \'xdg-open $PGURI\'\n  ```\n  As Beekeeper Studio registers as an opener for the `postgresql://` protocol, the above command can be used to open your database with it.\n- Otherwise, the arguments are used to launch the application as-is. It can use the environment variables to set up a connection.\n  ```sh\n  python -mpostgresqlite my-client connect --extra-fancy\n  ```\n\nOptionally, the directory where the configuration file (`postgresqlite.json`) will be read or created, and where database files will be stored, can be specified by prefixing the command with `-c` `<dirname>`. For example:\n\n```sh\npython -mpostgresqlite -d mydbdir \'xdg-open $PGURI\'\n```\n\n\n### The config file\n\nWhen PostgreSQLite is first started (for a certain directory), a configuration file called `postgresqlite.json` is created. After initial creation, the file is all yours to modify. It contains the following values:\n\n- `autostart` (bool): When true, PostgreSQLite will automatically start/stop a PostgreSQL server. Otherwise, it will just connect to an existing database given the credentials in this file.\n- `host` (str): Connection host name.\n- `port` (int): Connection TCP port.\n- `socket` (str): Connection UNIX domain socket (optional).\n- `database` (int): Database name.\n- `user` (str): Connection user name.\n- `password` (str): Connection password name (optional).\n- `socket_id` (str): A (random) string that distinguishes this instance of PostgreSQLite, for creating the PostgreSQL unix socket file in `/tmp`.\n\nThese fields are only relevant when `autostart` is true:\n- `expire_seconds` (int): The time in seconds after which a server is shutdown when there are no active clients anymore.\n- `pg_cache_dir` (str): The directory into which PostgreSQL will be installed and from which it will be ran.\n- `postgresql_version` (str): The version of PostgreSQL to use. Currently only `"14.3"` is supported.\n\n\n### The autostart mechanism\n\nPostgreSQLite uses a series of lock files (stored in `locks/` in the configuration directory) to coordinate different application instances that may want to use the database. When such a process starts and no database is running, it forks a daemon that will start and eventually stop the PostgreSQL server. Stopping happens when there have been no more database applications running for `expire_seconds`, based on the lock files created by each application.\n\nIn case you want to force the server to stop immediately, you can do so by deleting the `locks/daemon.lock` file within the configuration directory. Starting the application again will cause the server to start anew.\n\n\n### Standalone PostgreSQL\n\nThe autostart feature installs PostgreSQL from a tarball stored as a [GitHub release](https://github.com/vanviegen/postgresqlite/releases/tag/libs). This tarball is created using the `Dockerfile` and `run.sh` script provided in the `create-standalone-postgresql/` directory.\n\nIt works by copying the PostgreSQL binaries and depend files (including any `.so` files being used) from an Arch linux installation to a `.tar.gz` file. \n',
-    'author': 'Frank van Viegen',
-    'author_email': 'pp@vanviegen.net',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/vanviegen/postgresqlite',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+## Features
 
+- Using just a `postgresqlite.connect()` call, the library will automatically...
+    - Download and install PostgreSQL into the user's `~/.cache` directory. (Linux and macOS EM64T only, for now.)
+    - Create a new database (`initdb`) within the project directory with a random password.
+    - Start the PostgreSQL server.
+    - Set up a DB-API connection to the server (using the `pg8000` driver).
+    - Shut down the server when it's no longer in use.
+- It also adds a couple of conveniences on top of DB-API, making it more similar to the `sqlite3` module:
+    - Calling `execute` on the connection will create a new cursor.
+    - Calls to `fetchall` and `fetchone` return objects that can address fields both by number (as is standard for DB-API) as well as by name (as `sqlite3` offers when you configure `connection.row_factory = sqlite3.Row`).
+    - Autocommit mode is enabled by default.
+    - Parameterized queries use `?` as a placeholder. (`paramstyle = 'qmark'`)
+- It can open `psql` and other PostgreSQL clients passing in connection details, while making sure the database is running.
+- For use in production, the configuration file can be modified to point your application at a (non-auto-starting) PostgreSQL server.
+
+
+## Examples
+
+### Using DB-API directly
+
+```sh
+pip install postgresqlite
+```
+
+```python
+import postgresqlite
+
+db = postgresqlite.connect(mode='dbapi')
+
+cursor = db.cursor()
+cursor.execute('create table if not exists tests(id serial, info text not null, created_at timestamp not null default current_timestamp)')
+cursor.execute("insert into tests(info) values('Hi mom!'),('This is great!')")
+db.commit()
+
+cursor.execute("select id, info, created_at from tests where id=%s", [1])
+for row in cursor:
+    print("row:", row, "id:", row[0], "created_at:", row[2])
+
+cursor.execute("select count(*) from tests")
+print("count:", cursor.fetchone()[0])
+
+cursor.execute("select * from tests order by id desc limit 1")
+print("row:", cursor.fetchone())
+```
+
+### Using the `FriendlyConnection` API
+
+```sh
+pip install postgresqlite
+```
+
+```python
+import postgresqlite
+
+db = postgresqlite.connect()
+
+db.query('create table if not exists tests(id serial, info text not null, created_at timestamp not null default current_timestamp)')
+db.query("insert into tests(info) values('Hi mom!'),('This is great!')")
+
+rows = db.query("select * from tests where id=:id", id=1)
+for row in rows:
+    print("row:", row, "id:", row.id, "created_at:", row.created_at)
+
+print("count:", db.query_value("select count(*) from tests"))
+
+print("last row:", db.query_row("select * from tests order by id desc limit 1"))
+```
+
+### Using Flask-SQLAlchemy
+
+```sh
+pip install postgresqlite flask_sqlalchemy
+```
+
+```python
+import postgresqlite, flask, flask_sqlalchemy, datetime
+
+app = flask.Flask(__name__)
+app.config['SQLALCHEMY_DATABASE_URI'] = postgresqlite.get_uri()
+app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
+
+db = flask_sqlalchemy.SQLAlchemy(app)
+
+class Car(db.Model):
+    id = db.Column(db.Integer, primary_key=True)
+    brand = db.Column(db.String)
+    model = db.Column(db.String, nullable=False)
+    day_rate = db.Column(db.Integer)
+    rentals = db.relationship('Rental', backref='car')
+
+    def to_dict(self):
+        return {'id': self.id, 'brand': self.brand, 'model': self.model, 'day_rate': self.day_rate, 'rentals': [rental.to_dict() for rental in self.rentals]}
+    
+class Rental(db.Model):
+    id = db.Column(db.Integer, primary_key=True)
+    car_id = db.Column(db.Integer, db.ForeignKey('car.id'), nullable=False)
+
+    customer_name = db.Column(db.String, nullable=False)
+    start_time = db.Column(db.DateTime, default=datetime.datetime.now)
+    end_time = db.Column(db.DateTime)
+
+    def to_dict(self):
+        return {'id': self.id, 'car_id': self.car_id, 'customer_name': self.customer_name, 'start_time': self.start_time, 'end_time': self.end_time}
+
+@app.route('/cars')
+def show_all():
+   return flask.jsonify([car.to_dict() for car in Car.query.all()])
+
+@app.route('/cars', methods = ['POST'])
+def new_car():
+    car = Car(**flask.request.get_json())
+    db.session.add(car)
+    db.session.commit()
+    return flask.jsonify(car.to_dict())
+
+@app.route('/rentals', methods = ['POST'])
+def new_rental():
+    rental = Rental(**flask.request.get_json())
+    db.session.add(rental)
+    db.session.commit()
+    return flask.jsonify(rental.to_dict())
+
+# Create tables based on the Model classes above.
+with app.app_context():
+    db.create_all()
+
+if __name__ == '__main__':
+    app.run(debug = True)
+```
+
+Running this should expose a REST API. If you have [httpie](https://httpie.io/) installed, it can be tested from the command like this:
+
+```sh
+http http://127.0.0.1:5000/cars brand=Volvo model=S60
+http http://127.0.0.1:5000/rentals car_id=1 customer_name=Frank
+http http://127.0.0.1:5000/cars
+```
+
+
+
+## Documentation
+
+### API functions
+
+#### `postgresqlite.connect(dirname='data/postgresqlite', mode='friendly', config=None)`
+
+Start a server (if needed), wait for it, and return a DB-API compatible object.
+
+Arguments:
+- `dirname` (str): The dir where the configuration file (`postgresqlite.json`)
+    will be read or created, and where database files will be stored. If the
+    path does not exist, it will be created.
+- `mode` ('easy', 'sqlite', 'dbapi'): 
+  - When set to `friendly` (the default), a `FriendlyConnection` object is returned. It's a DB-API compatible Connection, but with a few additions to make it more programmer-friendly, as documented in the [The FriendlyConnection object](#the-friendlyconnection-object)-section.
+  - When set to 'dbapi', the created connection will be a plain PG8000 DB-API Connection.
+  - When set to 'sqlite3', a few (superficial) additions are added on top of the DB-API to make it resemble the Python `sqlite3` API more closely:
+    - `Connection` objects have an `execute` method that creates a new cursor and 
+        runs the given query on it.
+    - Row objects can be indexed using numeric indexes as well as column names,
+        just like (like with `connection.row_factory = sqlite3.Row` for `sqlite3`).
+    - Autocommit mode is enabled by default.
+    - Parameterized queries use `?` as a placeholder. (`paramstyle = 'qmark'`)
+- `config` (Config | None): An object obtained through `get_config()` can be given to configure the connection. This causes `dirname` to be ignored.
+
+Arguments:
+- dirname (str, defaults to `data/postgresqlite`): The directory where the configuration file (`postgresqlite.json`) will be read or created, and where database files will be stored. If the path does not exist, it will be created.
+- sqlite_compatible (bool, defaults to `True`): When set, a few (superficial) changes are made to the exposed DB-API to make it resemble the Python `sqlite3` API more closely, as described in the *Features* section.
+- config (`Config` object, defaults to `None`): This can be an object returned by `get_config`. When `None`, the `connect` method will create a default configuration.
+
+Returns a [DB-API compatible connection object](https://peps.python.org/pep-0249/#connection-objects).
+
+#### `postgresqlite.get_config(dirname='data/postgresqlite')`
+
+Start a server (if needed), wait for it, and return the config object. If the PostgreSQL server is in autostart mode (which is the default), it will be kept running until some time after the calling process (and any other processes that depend on this server) have terminated.
+ 
+Arguments:
+- dirname (str): The directory where the configuration file (`postgresqlite.json`) will be read or created, and where database files will be stored. If the path does not exist, it will be created.
+
+Returns a `Config` object, that includes (among others) the following attributes:
+- `user` (string): Database user name.
+- `password` (string): Database password. (Can be `None`.)
+- `port` (int): Database TCP port. (Can be `None`.)
+- `host` (string): Database host name. (Can be `None`.)
+- `database` (string): Database name.
+- `socket` (string): Database UNIX domain socket. (Can be `None`.)
+- `env` (dict): A dictionary containing `PGHOST`, `PGPORT`, `PGDATABASE`, `PGSOCKET`, `PGUSER`, `PGPASSWORD` and `PGURI` keys with their appropriate values.
+
+#### `postgresqlite.get_uri(dirname='data/postgresqlite', driver='pg8000')`
+Start a server (if needed), wait for it, and return a connection URL.
+
+Arguments:
+- dirname (str): The directory where the configuration file (`postgresqlite.json`) will be read or created, and where database files will be stored. If the path does not exist, it will be created.
+- driver (str): The URI may include a driver part (`postgresql+DRIVER://user:pwd@host/db`), which we'll set to `pg8000` by default. This parameter allows you to specify a different direct, or leave it out (by providing `None`).
+
+### The `FriendlyConnection` object
+
+By default the `postgresqlite.connect` method will return a `FriendlyConnection`, which is a DB-API compatible `Connection` object, but with a few programmer-friendly differences:
+
+- Row objects can be indexed using column names as well as column indexes. For example `row['name']` instead of `row[0]`. In addition, attribute syntax can be used, like `row.name`.
+- Autocommit mode is enabled by default.
+- Query parameters are in `:named` style.
+- Exceptions are instances of `SQLError` and contain easy to read error messages, highlighting the offending part of the query.
+
+Besides, those changes, the `FriendlyConnection` object offers a couple of additional methods:
+
+#### execute(sql: str, params: dict = {})
+
+Create a new `Cursor`, execute the given `sql` with the given `params` dictionary on that cursor, and return the `Cursor`. Example:
+
+```python
+row = db.execute('select * from test where id=:id', {'id': 123})).fetchone()`
+```
+
+#### query(sql, param1=.., param2=..)
+
+Execute the `sql` with the given parameters, returning a list of `FriendlyRow` objects. Example:
+
+```python
+rows = db.query('select id, name from test where name=:name', name='Ivo')
+print(len(rows), rows[0].id) # 3 123
+```
+
+#### query_row(sql, param1=.., param2=..)
+
+Execute the `sql` with the given parameters, returning a single `FriendlyRow` object or `None` (if no rows were returned). If the query results in more than one row, an exception is thrown. Example:
+
+```python
+row = db.query_row('select id, name from test where id=:id', id=123)
+print(row.id, row.name) # 123 Ivo
+```
+
+#### query_column(sql, param1=.., param2=..)
+
+Execute the `sql` with the given parameters, returning a list of values. If the query results in more than one column, an exception is thrown. Example:
+
+```python
+test_ids = db.query_column('select id from test where name=:name', name='Ivo')
+print(test_ids) # [123, 456, 789]
+```
+
+#### query_value(sql, param1=.., param2=..)
+
+Execute the `sql` with the given parameters, returning a single value. If the query results in more than one column or more than one row, an exception is thrown. Example:
+
+```python
+test_id = db.query_value('select id from test where name=:name limit 1', name='Ivo')
+print(test_id) # 123
+```
+
+
+### CLI interface
+
+In order to easily access the database your application is using, PostgreSQLite can open a client application (such as *psql* or [Beekeeper Studio](https://www.beekeeperstudio.io/)) for you, making sure the database is started (and doesn't shutdown) while the application is open, and passing in connection details.
+
+The connection details are provided in environment variables called `PGHOST`, `PGPORT`, `PGDATABASE`, `PGSOCKET`, `PGUSER`, `PGPASSWORD` and `PGURI`. 
+
+An application can be started by running the `postgresqlite` package with `-m`, providing the executable and its arguments as arguments.
+- When no arguments are passed: `psql`, the default PostgreSQL client, is run. So opening your database in `psql` can be done like this:
+  ```sh
+  python -mpostgresqlite
+  ```
+  The `psql` client uses the environment variables to set up a connection.
+- When exactly one argument is passed and it contains the string `$PG`, it will be executed as a shell command. So in order to pass the URI as the argument to an application, one could use:
+  ```sh
+  python -mpostgresqlite 'xdg-open $PGURI'
+  ```
+  As Beekeeper Studio registers as an opener for the `postgresql://` protocol, the above command can be used to open your database with it.
+- Otherwise, the arguments are used to launch the application as-is. It can use the environment variables to set up a connection.
+  ```sh
+  python -mpostgresqlite my-client connect --extra-fancy
+  ```
+
+Optionally, the directory where the configuration file (`postgresqlite.json`) will be read or created, and where database files will be stored, can be specified by prefixing the command with `-c` `<dirname>`. For example:
+
+```sh
+python -mpostgresqlite -d mydbdir 'xdg-open $PGURI'
+```
+
+
+### The config file
+
+When PostgreSQLite is first started (for a certain directory), a configuration file called `postgresqlite.json` is created. After initial creation, the file is all yours to modify. It contains the following values:
+
+- `autostart` (bool): When true, PostgreSQLite will automatically start/stop a PostgreSQL server. Otherwise, it will just connect to an existing database given the credentials in this file.
+- `host` (str): Connection host name.
+- `port` (int): Connection TCP port.
+- `socket` (str): Connection UNIX domain socket (optional).
+- `database` (int): Database name.
+- `user` (str): Connection user name.
+- `password` (str): Connection password name (optional).
+- `socket_id` (str): A (random) string that distinguishes this instance of PostgreSQLite, for creating the PostgreSQL unix socket file in `/tmp`.
+
+These fields are only relevant when `autostart` is true:
+- `expire_seconds` (int): The time in seconds after which a server is shutdown when there are no active clients anymore.
+- `pg_cache_dir` (str): The directory into which PostgreSQL will be installed and from which it will be ran.
+- `postgresql_version` (str): The version of PostgreSQL to use. Currently only `"14.3"` is supported.
+
+
+### The autostart mechanism
+
+PostgreSQLite uses a series of lock files (stored in `locks/` in the configuration directory) to coordinate different application instances that may want to use the database. When such a process starts and no database is running, it forks a daemon that will start and eventually stop the PostgreSQL server. Stopping happens when there have been no more database applications running for `expire_seconds`, based on the lock files created by each application.
+
+In case you want to force the server to stop immediately, you can do so by deleting the `locks/daemon.lock` file within the configuration directory. Starting the application again will cause the server to start anew.
+
+
+### Standalone PostgreSQL
+
+The autostart feature installs PostgreSQL from a tarball stored as a [GitHub release](https://github.com/vanviegen/postgresqlite/releases/tag/libs). This tarball is created using the `Dockerfile` and `run.sh` script provided in the `create-standalone-postgresql/` directory.
+
+It works by copying the PostgreSQL binaries and depend files (including any `.so` files being used) from an Arch linux installation to a `.tar.gz` file. 
 
-setup(**setup_kwargs)
```

