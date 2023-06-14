# Comparing `tmp/eparse-0.3.0.tar.gz` & `tmp/eparse-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eparse-0.3.0.tar", last modified: Wed Jun 14 15:56:47 2023, max compression
+gzip compressed data, was "eparse-0.4.1.tar", last modified: Wed Jun 14 17:30:20 2023, max compression
```

## Comparing `eparse-0.3.0.tar` & `eparse-0.4.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 15:56:47.130245 eparse-0.3.0/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-08 00:46:57.000000 eparse-0.3.0/AUTHORS.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-08 00:46:57.000000 eparse-0.3.0/CONTRIBUTING.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      323 2023-06-13 20:47:22.000000 eparse-0.3.0/HISTORY.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-08 00:46:57.000000 eparse-0.3.0/LICENSE
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-08 00:46:57.000000 eparse-0.3.0/MANIFEST.in
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    10455 2023-06-14 15:56:47.130245 eparse-0.3.0/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9442 2023-06-14 15:19:41.000000 eparse-0.3.0/README.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 15:56:47.130245 eparse-0.3.0/docs/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/Makefile
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/authors.rst
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/conf.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/contributing.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/history.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/index.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/installation.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/make.bat
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/readme.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-08 00:46:57.000000 eparse-0.3.0/docs/usage.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 15:56:47.130245 eparse-0.3.0/eparse/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      126 2023-06-14 00:08:57.000000 eparse-0.3.0/eparse/__init__.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    10172 2023-06-14 15:53:36.000000 eparse-0.3.0/eparse/cli.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     4736 2023-06-14 15:27:35.000000 eparse-0.3.0/eparse/core.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     5572 2023-06-14 15:53:50.000000 eparse-0.3.0/eparse/interfaces.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1554 2023-06-12 23:01:06.000000 eparse-0.3.0/eparse/migrations.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 15:56:47.130245 eparse-0.3.0/eparse.egg-info/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    10455 2023-06-14 15:56:47.000000 eparse-0.3.0/eparse.egg-info/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      701 2023-06-14 15:56:47.000000 eparse-0.3.0/eparse.egg-info/SOURCES.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-14 15:56:47.000000 eparse-0.3.0/eparse.egg-info/dependency_links.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-06-14 15:56:47.000000 eparse-0.3.0/eparse.egg-info/entry_points.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-14 15:56:47.000000 eparse-0.3.0/eparse.egg-info/not-zip-safe
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-06-14 15:56:47.000000 eparse-0.3.0/eparse.egg-info/requires.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-06-14 15:56:47.000000 eparse-0.3.0/eparse.egg-info/top_level.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      427 2023-06-14 15:56:47.130245 eparse-0.3.0/setup.cfg
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1513 2023-06-14 00:08:48.000000 eparse-0.3.0/setup.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 15:56:47.130245 eparse-0.3.0/tests/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-08 00:46:57.000000 eparse-0.3.0/tests/__init__.py
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-08 00:46:57.000000 eparse-0.3.0/tests/eparse_unit_test_data.xlsx
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      893 2023-06-14 14:09:23.000000 eparse-0.3.0/tests/fixtures.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)   237568 2023-06-14 14:02:00.000000 eparse-0.3.0/tests/test.db
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1950 2023-06-14 15:53:16.000000 eparse-0.3.0/tests/test_cli.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1085 2023-06-13 20:47:22.000000 eparse-0.3.0/tests/test_core.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2609 2023-06-14 13:42:33.000000 eparse-0.3.0/tests/test_interfaces.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 17:30:20.804639 eparse-0.4.1/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-08 00:46:57.000000 eparse-0.4.1/AUTHORS.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-08 00:46:57.000000 eparse-0.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      323 2023-06-13 20:47:22.000000 eparse-0.4.1/HISTORY.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-08 00:46:57.000000 eparse-0.4.1/LICENSE
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-08 00:46:57.000000 eparse-0.4.1/MANIFEST.in
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    12067 2023-06-14 17:30:20.804639 eparse-0.4.1/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    10996 2023-06-14 17:19:22.000000 eparse-0.4.1/README.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 17:30:20.804639 eparse-0.4.1/docs/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/Makefile
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/authors.rst
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/conf.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/contributing.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/history.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/index.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/installation.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/make.bat
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/readme.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-08 00:46:57.000000 eparse-0.4.1/docs/usage.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 17:30:20.804639 eparse-0.4.1/eparse/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      126 2023-06-14 17:29:53.000000 eparse-0.4.1/eparse/__init__.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    10172 2023-06-14 15:53:36.000000 eparse-0.4.1/eparse/cli.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     4736 2023-06-14 15:27:35.000000 eparse-0.4.1/eparse/core.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     6280 2023-06-14 16:48:23.000000 eparse-0.4.1/eparse/interfaces.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1554 2023-06-12 23:01:06.000000 eparse-0.4.1/eparse/migrations.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 17:30:20.804639 eparse-0.4.1/eparse.egg-info/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    12067 2023-06-14 17:30:20.000000 eparse-0.4.1/eparse.egg-info/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      701 2023-06-14 17:30:20.000000 eparse-0.4.1/eparse.egg-info/SOURCES.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-14 17:30:20.000000 eparse-0.4.1/eparse.egg-info/dependency_links.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-06-14 17:30:20.000000 eparse-0.4.1/eparse.egg-info/entry_points.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-14 17:30:20.000000 eparse-0.4.1/eparse.egg-info/not-zip-safe
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-06-14 17:30:20.000000 eparse-0.4.1/eparse.egg-info/requires.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-06-14 17:30:20.000000 eparse-0.4.1/eparse.egg-info/top_level.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      427 2023-06-14 17:30:20.814639 eparse-0.4.1/setup.cfg
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1570 2023-06-14 17:29:38.000000 eparse-0.4.1/setup.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 17:30:20.804639 eparse-0.4.1/tests/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-08 00:46:57.000000 eparse-0.4.1/tests/__init__.py
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-08 00:46:57.000000 eparse-0.4.1/tests/eparse_unit_test_data.xlsx
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      893 2023-06-14 14:09:23.000000 eparse-0.4.1/tests/fixtures.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)   237568 2023-06-14 14:02:00.000000 eparse-0.4.1/tests/test.db
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1950 2023-06-14 15:53:16.000000 eparse-0.4.1/tests/test_cli.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1085 2023-06-13 20:47:22.000000 eparse-0.4.1/tests/test_core.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2609 2023-06-14 13:42:33.000000 eparse-0.4.1/tests/test_interfaces.py
```

### Comparing `eparse-0.3.0/CONTRIBUTING.rst` & `eparse-0.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.3.0/LICENSE` & `eparse-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eparse-0.3.0/PKG-INFO` & `eparse-0.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: eparse
-Version: 0.3.0
-Summary: Excel spreadsheet crawler and table parser for data extraction and querying
+Version: 0.4.1
+Summary: Excel spreadsheet crawler and table parser for data discovery, extraction, and querying
 Home-page: https://github.com/ChrisPappalardo/eparse
 Author: Chris Pappalardo
 Author-email: cpappala@gmail.com
 License: MIT license
 Keywords: eparse
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 License-File: LICENSE
@@ -58,14 +59,34 @@
 
 .. code-block:: bash
 
    $ git clone https://github.com/ChrisPappalardo/eparse.git
    $ cd eparse
    $ pip install .
 
+If you plan to use the postgres interface, you also need to install
+the postgres package ``psycopg2``. Instructions can be found
+`here <https://www.psycopg.org/docs/install.html#quick-install>`_.
+This package is optional, and you can use the other interfaces
+such as the ``SQLite3`` interface without having to install
+``psycopg2``.
+
+The easiest way to install the ``psycopg2`` package for your
+particular environment may be to install the pre-compiled
+binary driver as follows:
+
+.. code-block:: bash
+
+   $ pip install psycopg2-binary
+
+If you see an error while trying to use a postgres endpoint such
+as ``postgres://user:pass@host:port/my_db`` that mentions the
+postgres driver is missing, then you know you haven't properly
+installed (and compiled)  ``psycopg2``.
+
 
 Usage
 =====
 eparse is intended to be used from the command-line.  You can view
 supported commands and usage with ``--help`` as follows:
 
 .. code-block:: bash
@@ -196,14 +217,34 @@
 You can also specify a path and filename of your choosing, like so:
 
 .. code-block:: bash
 
     $ mkdir .files
     $ eparse -f <path_to_files> -o sqlite3:///path/filename.db parse -z
 
+postgres
+^^^^^^^^
+eparse also supports `postgresql` integrations. As mentioned above,
+you will need ``psycopg2`` installed for `postgresql` integrations
+to work. The eparse ``BaseDatabaseInterface`` abstracts the
+implementation details, so you would use this interface the same
+way you use the others, with the exception of the endpoint.
+
+To use a ``postgresql`` database as the source and/or destination
+of your data, you would supply an ``--input`` and/or ``--output``
+endpoint to the tool as follows:
+
+.. code-block:: bash
+
+    $ eparse -o postgres://user:password@host:port/db_name ...
+
+Where details like ``user``, ``host``, ``port`` are provided to
+you by your db administrator. eparse will create the necessary
+table(s) and indexes for you when inserting data into the database.
+
 
 Query
 -----
 Once you have stored parsed data, you can begin to query it using the
 ``peewee`` ORM.  This can be done with the tool or directly with
 the database.
```

### Comparing `eparse-0.3.0/README.rst` & `eparse-0.4.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -38,14 +38,34 @@
 
 .. code-block:: bash
 
    $ git clone https://github.com/ChrisPappalardo/eparse.git
    $ cd eparse
    $ pip install .
 
+If you plan to use the postgres interface, you also need to install
+the postgres package ``psycopg2``. Instructions can be found
+`here <https://www.psycopg.org/docs/install.html#quick-install>`_.
+This package is optional, and you can use the other interfaces
+such as the ``SQLite3`` interface without having to install
+``psycopg2``.
+
+The easiest way to install the ``psycopg2`` package for your
+particular environment may be to install the pre-compiled
+binary driver as follows:
+
+.. code-block:: bash
+
+   $ pip install psycopg2-binary
+
+If you see an error while trying to use a postgres endpoint such
+as ``postgres://user:pass@host:port/my_db`` that mentions the
+postgres driver is missing, then you know you haven't properly
+installed (and compiled)  ``psycopg2``.
+
 
 Usage
 =====
 eparse is intended to be used from the command-line.  You can view
 supported commands and usage with ``--help`` as follows:
 
 .. code-block:: bash
@@ -176,14 +196,34 @@
 You can also specify a path and filename of your choosing, like so:
 
 .. code-block:: bash
 
     $ mkdir .files
     $ eparse -f <path_to_files> -o sqlite3:///path/filename.db parse -z
 
+postgres
+^^^^^^^^
+eparse also supports `postgresql` integrations. As mentioned above,
+you will need ``psycopg2`` installed for `postgresql` integrations
+to work. The eparse ``BaseDatabaseInterface`` abstracts the
+implementation details, so you would use this interface the same
+way you use the others, with the exception of the endpoint.
+
+To use a ``postgresql`` database as the source and/or destination
+of your data, you would supply an ``--input`` and/or ``--output``
+endpoint to the tool as follows:
+
+.. code-block:: bash
+
+    $ eparse -o postgres://user:password@host:port/db_name ...
+
+Where details like ``user``, ``host``, ``port`` are provided to
+you by your db administrator. eparse will create the necessary
+table(s) and indexes for you when inserting data into the database.
+
 
 Query
 -----
 Once you have stored parsed data, you can begin to query it using the
 ``peewee`` ORM.  This can be done with the tool or directly with
 the database.
```

### Comparing `eparse-0.3.0/docs/Makefile` & `eparse-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eparse-0.3.0/docs/conf.py` & `eparse-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eparse-0.3.0/docs/installation.rst` & `eparse-0.4.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.3.0/docs/make.bat` & `eparse-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eparse-0.3.0/eparse/cli.py` & `eparse-0.4.1/eparse/cli.py`

 * *Files identical despite different names*

### Comparing `eparse-0.3.0/eparse/core.py` & `eparse-0.4.1/eparse/core.py`

 * *Files identical despite different names*

### Comparing `eparse-0.3.0/eparse/interfaces.py` & `eparse-0.4.1/eparse/interfaces.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     AutoField,
     CharField,
     DatabaseProxy,
     DateTimeField,
     fn,
     IntegerField,
     Model,
+    PostgresqlDatabase,
     SqliteDatabase,
 )
 
 
 DATABASE = DatabaseProxy()
 
 
@@ -90,14 +91,15 @@
     endpoint = ''
     user = ''
     password = ''
     host = ''
     port = 0
     name = ''
 
+    Database = None
     Model = None
 
     def __init__(self, uri: str, Model: Optional[Model] = None):
         for k, v in self.parse_uri(uri).items():
             setattr(self, k, v)
         self.Model = Model
 
@@ -161,35 +163,37 @@
     def output(self, data, *args, **kwargs):
         PrettyPrinter().pprint(data)
 
     def migrate(self, *args, **kwargs):
         pass
 
 
-class Sqlite3Interface(BaseInterface):
+class BaseDatabaseInterface(BaseInterface):
     '''
-    sqlite3 interface
+    base database interface
     '''
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    @abstractmethod
+    def initialize(self, *args, **kwargs):
+        '''
+        override with db-specific initialization
+        '''
 
-        if not self.name:
-            self.name = f'.files/{uuid4()}.db'
+        pass
 
     def input(self, method, **kwargs):
         m = getattr(self.Model, method, None)
 
         # if no explicit method is available, try get_column
         if m is None:
             m = self.Model.get_column
             patt = r'^(?:get_)?(?P<column>.*)$'
             kwargs['column'] = re.match(patt, method).group('column')
 
-        DATABASE.initialize(SqliteDatabase(self.name))
+        self.initialize(DATABASE)
         DATABASE.connect()
 
         return m(**kwargs)
 
     def output(self, data, obj):
         # skip empty data
         if hasattr(data, 'empty') and data.empty:
@@ -200,15 +204,15 @@
         # check that data is serialized
         try:
             assert isinstance(data, Iterable)
             assert isinstance(data[0], Mapping)
         except Exception:
             raise ValueError('bad data - did you serialize it first?')
 
-        DATABASE.initialize(SqliteDatabase(self.name))
+        self.initialize(DATABASE)
         DATABASE.connect()
         DATABASE.create_tables([self.Model])
 
         # insert data into Model
         for d in data:
             self.Model.create(**d)
 
@@ -218,25 +222,57 @@
         try:
             m = importlib.import_module('eparse.migrations')
             migration_fcn = getattr(m, migration)
         except AttributeError:
             msg = f'migration error - there is no {migration}'
             raise AttributeError(msg)
 
-        DATABASE.initialize(SqliteDatabase(self.name))
+        self.initialize(DATABASE)
         DATABASE.connect()
         migration_fcn(self.Model)
 
 
+class Sqlite3Interface(BaseDatabaseInterface):
+    '''
+    sqlite3 interface
+    '''
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        if not self.name:
+            self.name = f'.files/{uuid4()}.db'
+
+    def initialize(self, db):
+        db.initialize(SqliteDatabase(self.name))
+
+
+class PostgresInterface(BaseDatabaseInterface):
+    '''
+    postgres interface
+    '''
+
+    def initialize(self, db):
+        db.initialize(PostgresqlDatabase(
+            self.name,
+            user=self.user,
+            password=self.password,
+            host=self.host,
+            port=self.port,
+        ))
+
+
 def i_factory(uri, Model=None):
     '''
     return interface object based on uri
     '''
 
     if uri.startswith('null'):
         return NullInterface(uri)
     elif uri.startswith('stdout'):
         return StdoutInterface(uri)
     elif uri.startswith('sqlite3'):
         return Sqlite3Interface(uri, Model)
+    elif uri.startswith('postgres'):
+        return PostgresInterface(uri, Model)
 
     raise ValueError(f'{uri} is not a recognized endpoint')
```

### Comparing `eparse-0.3.0/eparse/migrations.py` & `eparse-0.4.1/eparse/migrations.py`

 * *Files identical despite different names*

### Comparing `eparse-0.3.0/eparse.egg-info/PKG-INFO` & `eparse-0.4.1/eparse.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: eparse
-Version: 0.3.0
-Summary: Excel spreadsheet crawler and table parser for data extraction and querying
+Version: 0.4.1
+Summary: Excel spreadsheet crawler and table parser for data discovery, extraction, and querying
 Home-page: https://github.com/ChrisPappalardo/eparse
 Author: Chris Pappalardo
 Author-email: cpappala@gmail.com
 License: MIT license
 Keywords: eparse
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 License-File: LICENSE
@@ -58,14 +59,34 @@
 
 .. code-block:: bash
 
    $ git clone https://github.com/ChrisPappalardo/eparse.git
    $ cd eparse
    $ pip install .
 
+If you plan to use the postgres interface, you also need to install
+the postgres package ``psycopg2``. Instructions can be found
+`here <https://www.psycopg.org/docs/install.html#quick-install>`_.
+This package is optional, and you can use the other interfaces
+such as the ``SQLite3`` interface without having to install
+``psycopg2``.
+
+The easiest way to install the ``psycopg2`` package for your
+particular environment may be to install the pre-compiled
+binary driver as follows:
+
+.. code-block:: bash
+
+   $ pip install psycopg2-binary
+
+If you see an error while trying to use a postgres endpoint such
+as ``postgres://user:pass@host:port/my_db`` that mentions the
+postgres driver is missing, then you know you haven't properly
+installed (and compiled)  ``psycopg2``.
+
 
 Usage
 =====
 eparse is intended to be used from the command-line.  You can view
 supported commands and usage with ``--help`` as follows:
 
 .. code-block:: bash
@@ -196,14 +217,34 @@
 You can also specify a path and filename of your choosing, like so:
 
 .. code-block:: bash
 
     $ mkdir .files
     $ eparse -f <path_to_files> -o sqlite3:///path/filename.db parse -z
 
+postgres
+^^^^^^^^
+eparse also supports `postgresql` integrations. As mentioned above,
+you will need ``psycopg2`` installed for `postgresql` integrations
+to work. The eparse ``BaseDatabaseInterface`` abstracts the
+implementation details, so you would use this interface the same
+way you use the others, with the exception of the endpoint.
+
+To use a ``postgresql`` database as the source and/or destination
+of your data, you would supply an ``--input`` and/or ``--output``
+endpoint to the tool as follows:
+
+.. code-block:: bash
+
+    $ eparse -o postgres://user:password@host:port/db_name ...
+
+Where details like ``user``, ``host``, ``port`` are provided to
+you by your db administrator. eparse will create the necessary
+table(s) and indexes for you when inserting data into the database.
+
 
 Query
 -----
 Once you have stored parsed data, you can begin to query it using the
 ``peewee`` ORM.  This can be done with the tool or directly with
 the database.
```

### Comparing `eparse-0.3.0/eparse.egg-info/SOURCES.txt` & `eparse-0.4.1/eparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eparse-0.3.0/setup.py` & `eparse-0.4.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,24 +28,25 @@
 ]
 
 setup(
     author='Chris Pappalardo',
     author_email='cpappala@gmail.com',
     python_requires='>=3.9',
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
+        'Intended Audience :: End Users/Desktop',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     description='''
-    Excel spreadsheet crawler and table parser for data extraction and querying
+    Excel spreadsheet crawler and table parser for data discovery, extraction, and querying
     ''',
     entry_points={
         'console_scripts': [
             'eparse=eparse.cli:entry_point',
         ],
     },
     install_requires=requirements,
@@ -54,10 +55,10 @@
     include_package_data=True,
     keywords='eparse',
     name='eparse',
     packages=find_packages(include=['eparse', 'eparse.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ChrisPappalardo/eparse',
-    version='0.3.0',
+    version='0.4.1',
     zip_safe=False,
 )
```

### Comparing `eparse-0.3.0/tests/eparse_unit_test_data.xlsx` & `eparse-0.4.1/tests/eparse_unit_test_data.xlsx`

 * *Files identical despite different names*

### Comparing `eparse-0.3.0/tests/fixtures.py` & `eparse-0.4.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `eparse-0.3.0/tests/test.db` & `eparse-0.4.1/tests/test.db`

 * *Files identical despite different names*

### Comparing `eparse-0.3.0/tests/test_cli.py` & `eparse-0.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `eparse-0.3.0/tests/test_core.py` & `eparse-0.4.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `eparse-0.3.0/tests/test_interfaces.py` & `eparse-0.4.1/tests/test_interfaces.py`

 * *Files identical despite different names*

