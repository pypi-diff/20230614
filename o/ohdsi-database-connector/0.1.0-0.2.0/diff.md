# Comparing `tmp/ohdsi-database-connector-0.1.0.tar.gz` & `tmp/ohdsi-database-connector-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohdsi-database-connector-0.1.0.tar", last modified: Tue Jun 13 14:53:58 2023, max compression
+gzip compressed data, was "ohdsi-database-connector-0.2.0.tar", last modified: Wed Jun 14 08:26:51 2023, max compression
```

## Comparing `ohdsi-database-connector-0.1.0.tar` & `ohdsi-database-connector-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:58.309216 ohdsi-database-connector-0.1.0/
--rw-rw-rw-   0        0        0      953 2023-06-13 14:53:58.309216 ohdsi-database-connector-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:58.290863 ohdsi-database-connector-0.1.0/ohdsi/
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:58.293578 ohdsi-database-connector-0.1.0/ohdsi/database_connector/
--rw-rw-rw-   0        0        0     4594 2023-06-13 12:55:22.000000 ohdsi-database-connector-0.1.0/ohdsi/database_connector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:58.293578 ohdsi-database-connector-0.1.0/ohdsi/database_connector/java/
--rw-rw-rw-   0        0        0  1004719 2023-03-28 14:10:27.000000 ohdsi-database-connector-0.1.0/ohdsi/database_connector/java/postgresql-42.2.18.jar
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:58.309216 ohdsi-database-connector-0.1.0/ohdsi_database_connector.egg-info/
--rw-rw-rw-   0        0        0      953 2023-06-13 14:53:58.000000 ohdsi-database-connector-0.1.0/ohdsi_database_connector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-06-13 14:53:58.000000 ohdsi-database-connector-0.1.0/ohdsi_database_connector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 14:53:58.000000 ohdsi-database-connector-0.1.0/ohdsi_database_connector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-13 14:53:58.000000 ohdsi-database-connector-0.1.0/ohdsi_database_connector.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 14:53:58.000000 ohdsi-database-connector-0.1.0/ohdsi_database_connector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 14:53:58.309216 ohdsi-database-connector-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1077 2023-06-13 12:02:47.000000 ohdsi-database-connector-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.505507 ohdsi-database-connector-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-14 08:26:51.505507 ohdsi-database-connector-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.501507 ohdsi-database-connector-0.2.0/ohdsi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.505507 ohdsi-database-connector-0.2.0/ohdsi/database_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-06-14 08:26:29.000000 ohdsi-database-connector-0.2.0/ohdsi/database_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.505507 ohdsi-database-connector-0.2.0/ohdsi/database_connector/java/
+-rw-r--r--   0 runner    (1001) docker     (123)  1004719 2023-06-14 08:26:29.000000 ohdsi-database-connector-0.2.0/ohdsi/database_connector/java/postgresql-42.2.18.jar
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.505507 ohdsi-database-connector-0.2.0/ohdsi_database_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-14 08:26:51.000000 ohdsi-database-connector-0.2.0/ohdsi_database_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-14 08:26:51.000000 ohdsi-database-connector-0.2.0/ohdsi_database_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:26:51.000000 ohdsi-database-connector-0.2.0/ohdsi_database_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 08:26:51.000000 ohdsi-database-connector-0.2.0/ohdsi_database_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 08:26:51.000000 ohdsi-database-connector-0.2.0/ohdsi_database_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:26:51.505507 ohdsi-database-connector-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-14 08:26:29.000000 ohdsi-database-connector-0.2.0/setup.py
```

### Comparing `ohdsi-database-connector-0.1.0/PKG-INFO` & `ohdsi-database-connector-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1
-Name: ohdsi-database-connector
-Version: 0.1.0
-Summary: Python wrapper for the OHDSI R packages
-Home-page: https://github.com/vantage6/python-ohdsi
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
-# python-ohdsi
-Python wrappers for (some) OHDSI tools. This project has been initiated for supporting
-OMOP data sources in vantage6.
-
-# TODO
-Packages to be wrapped:
-- [ ] [Capr](https://github.com/OHDSI/Capr)
-- [X] [CirceR](https://github.com/OHDSI/CirceR)
-- [X] [CohortGenerator](https://github.com/OHDSI/cohortgenerator)
-- [X] [SqlRender](https://github.com/OHDSI/SqlRender)
-- [X] [DatabaseConnector](https://github.com/OHDSI/DatabaseConnector)
-- [ ] [FeatureExtraction](https://github.com/OHDSI/FeatureExtraction)
-
-Release packages: `ohdsi-circe`, `ohdsi-capr`, `ohdsi-cohortgenerator`, `ohdsi-sqlrender`, `ohdsi-databaseconnector`, `ohdsi-featureextraction`
+Metadata-Version: 2.1
+Name: ohdsi-database-connector
+Version: 0.2.0
+Summary: Python wrapper for the OHDSI R packages
+Home-page: https://github.com/vantage6/python-ohdsi
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
+# python-ohdsi
+Python wrappers for (some) OHDSI tools. This project has been initiated for supporting
+OMOP data sources in vantage6.
+
+# TODO
+Packages to be wrapped:
+- [ ] [Capr](https://github.com/OHDSI/Capr)
+- [X] [CirceR](https://github.com/OHDSI/CirceR)
+- [X] [CohortGenerator](https://github.com/OHDSI/cohortgenerator)
+- [X] [SqlRender](https://github.com/OHDSI/SqlRender)
+- [X] [DatabaseConnector](https://github.com/OHDSI/DatabaseConnector)
+- [ ] [FeatureExtraction](https://github.com/OHDSI/FeatureExtraction)
+
+Release packages: `ohdsi-circe`, `ohdsi-capr`, `ohdsi-cohortgenerator`, `ohdsi-sqlrender`, `ohdsi-databaseconnector`, `ohdsi-featureextraction`
```

### Comparing `ohdsi-database-connector-0.1.0/ohdsi/database_connector/__init__.py` & `ohdsi-database-connector-0.2.0/ohdsi/database_connector/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-from importlib.resources import files
-
-from rpy2.robjects.packages import importr
-from rpy2.robjects.vectors import ListVector
-from rpy2.robjects.methods import RS4
-
-
-database_connector_r = importr('DatabaseConnector')
-
-
-class Connect:
-
-    @staticmethod
-    def create_connection_details(
-        dbms: str, user: str | None = None, password: str | None = None,
-        server: str | None = None, port: int | None = None,
-        extra_settings: str | None = None, oracle_driver: str = "thin",
-        connection_string: str | None = None,
-        path_to_driver: str | None = None
-    ) -> ListVector:
-        """
-        Create Connection Details.
-
-        Creates a list containing all details needed to connect to a database.
-        There are three ways to call this function:
-
-        - ``create_connection_details(dbms, user, password, server, port,
-                                      extraSettings, oracleDriver,
-                                      pathToDriver)``
-        - ``create_connection_details(dbms, connectionString, pathToDriver)``
-        - ``create_connection_details(dbms, connectionString, user, password,
-                                      pathToDriver)``
-
-        Parameters
-        ----------
-        dbms : str
-            The DBMS type.
-        user : str | None, optional
-            The database user name. Required if ``connection_string`` is not
-            provided.
-        password : str | None, optional
-            The database password. Required if ``connection_string`` is not
-            provided.
-        server : str | None, optional
-            The database server name. Required if ``connection_string`` is not
-            provided.
-        port : int | None, optional
-            The database server port. Required if ``connection_string`` is not
-            provided.
-        extra_settings : str | None, optional
-            Additional database connection settings.
-        oracle_driver : str, optional
-            The Oracle driver to use. Defaults to ``thin``.
-        connection_string : str | None, optional
-            The database connection string. ``user``, ``password``, ``server``,
-            and ``port`` are ignored if this is provided.
-        path_to_driver : str | None, optional
-            The path to the database driver jar file.
-
-        Returns
-        -------
-        ListVector
-            The connection details.
-
-        Examples
-        --------
-        >>> Connect.create_connection_details(
-        ...     dbms="postgresql", user="user", password="password",
-        ...     server="localhost/postgres", port=5432
-        ... )
-        """
-        # The jar required is shipped with the package
-        if not path_to_driver:
-            jar = files('ohdsi.database_connector.java')
-            # Hack to get the path to the folder of driver jar file,
-            # as the files method returns a MultiPlexPath object which
-            # does not allow simple conversion to string.
-            path_to_driver = str(jar.joinpath(''))
-
-        input_args = {
-            "dbms": dbms, "user": user, "password": password,
-            "server": server, "port": port, "extraSettings": extra_settings,
-            "oracleDriver": oracle_driver,
-            "connectionString": connection_string,
-            "pathToDriver": path_to_driver
-        }
-        # Remove None values
-        input_args = {k: v for k, v in input_args.items() if v is not None}
-        return database_connector_r.createConnectionDetails(**input_args)
-
-    @staticmethod
-    def connect(connection_details: ListVector) -> RS4:
-        """
-        Connect to a OMOP CDM database.
-
-        Connects to a database using the provided connection details,
-        created by ``create_connection_details``.
-
-        Parameters
-        ----------
-        connection_details : ListVector
-            The connection details.
-
-        Returns
-        -------
-        RS4
-            The database connection.
-
-        Examples
-        --------
-        >>> Connect.connect(connection_details)
-        """
-        return database_connector_r.connect(connection_details)
-
-    @staticmethod
-    def disconnect(connection: RS4) -> None:
-        """
-        Disconnect from a database.
-
-        Parameters
-        ----------
-        connection : RS4
-            The database connection.
-
-        Examples
-        --------
-        >>> Connect.disconnect(connection)
-        """
+from importlib.resources import files
+
+from rpy2.robjects.packages import importr
+from rpy2.robjects.vectors import ListVector
+from rpy2.robjects.methods import RS4
+
+
+database_connector_r = importr('DatabaseConnector')
+
+
+class Connect:
+
+    @staticmethod
+    def create_connection_details(
+        dbms: str, user: str | None = None, password: str | None = None,
+        server: str | None = None, port: int | None = None,
+        extra_settings: str | None = None, oracle_driver: str = "thin",
+        connection_string: str | None = None,
+        path_to_driver: str | None = None
+    ) -> ListVector:
+        """
+        Create Connection Details.
+
+        Creates a list containing all details needed to connect to a database.
+        There are three ways to call this function:
+
+        - ``create_connection_details(dbms, user, password, server, port,
+                                      extraSettings, oracleDriver,
+                                      pathToDriver)``
+        - ``create_connection_details(dbms, connectionString, pathToDriver)``
+        - ``create_connection_details(dbms, connectionString, user, password,
+                                      pathToDriver)``
+
+        Parameters
+        ----------
+        dbms : str
+            The DBMS type.
+        user : str | None, optional
+            The database user name. Required if ``connection_string`` is not
+            provided.
+        password : str | None, optional
+            The database password. Required if ``connection_string`` is not
+            provided.
+        server : str | None, optional
+            The database server name. Required if ``connection_string`` is not
+            provided.
+        port : int | None, optional
+            The database server port. Required if ``connection_string`` is not
+            provided.
+        extra_settings : str | None, optional
+            Additional database connection settings.
+        oracle_driver : str, optional
+            The Oracle driver to use. Defaults to ``thin``.
+        connection_string : str | None, optional
+            The database connection string. ``user``, ``password``, ``server``,
+            and ``port`` are ignored if this is provided.
+        path_to_driver : str | None, optional
+            The path to the database driver jar file.
+
+        Returns
+        -------
+        ListVector
+            The connection details.
+
+        Examples
+        --------
+        >>> Connect.create_connection_details(
+        ...     dbms="postgresql", user="user", password="password",
+        ...     server="localhost/postgres", port=5432
+        ... )
+        """
+        # The jar required is shipped with the package
+        if not path_to_driver:
+            jar = files('ohdsi.database_connector.java')
+            # Hack to get the path to the folder of driver jar file,
+            # as the files method returns a MultiPlexPath object which
+            # does not allow simple conversion to string.
+            path_to_driver = str(jar.joinpath(''))
+
+        input_args = {
+            "dbms": dbms, "user": user, "password": password,
+            "server": server, "port": port, "extraSettings": extra_settings,
+            "oracleDriver": oracle_driver,
+            "connectionString": connection_string,
+            "pathToDriver": path_to_driver
+        }
+        # Remove None values
+        input_args = {k: v for k, v in input_args.items() if v is not None}
+        return database_connector_r.createConnectionDetails(**input_args)
+
+    @staticmethod
+    def connect(connection_details: ListVector) -> RS4:
+        """
+        Connect to a OMOP CDM database.
+
+        Connects to a database using the provided connection details,
+        created by ``create_connection_details``.
+
+        Parameters
+        ----------
+        connection_details : ListVector
+            The connection details.
+
+        Returns
+        -------
+        RS4
+            The database connection.
+
+        Examples
+        --------
+        >>> Connect.connect(connection_details)
+        """
+        return database_connector_r.connect(connection_details)
+
+    @staticmethod
+    def disconnect(connection: RS4) -> None:
+        """
+        Disconnect from a database.
+
+        Parameters
+        ----------
+        connection : RS4
+            The database connection.
+
+        Examples
+        --------
+        >>> Connect.disconnect(connection)
+        """
         database_connector_r.disconnect(connection)
```

### Comparing `ohdsi-database-connector-0.1.0/ohdsi/database_connector/java/postgresql-42.2.18.jar` & `ohdsi-database-connector-0.2.0/ohdsi/database_connector/java/postgresql-42.2.18.jar`

 * *Files identical despite different names*

### Comparing `ohdsi-database-connector-0.1.0/ohdsi_database_connector.egg-info/PKG-INFO` & `ohdsi-database-connector-0.2.0/ohdsi_database_connector.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1
-Name: ohdsi-database-connector
-Version: 0.1.0
-Summary: Python wrapper for the OHDSI R packages
-Home-page: https://github.com/vantage6/python-ohdsi
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
-# python-ohdsi
-Python wrappers for (some) OHDSI tools. This project has been initiated for supporting
-OMOP data sources in vantage6.
-
-# TODO
-Packages to be wrapped:
-- [ ] [Capr](https://github.com/OHDSI/Capr)
-- [X] [CirceR](https://github.com/OHDSI/CirceR)
-- [X] [CohortGenerator](https://github.com/OHDSI/cohortgenerator)
-- [X] [SqlRender](https://github.com/OHDSI/SqlRender)
-- [X] [DatabaseConnector](https://github.com/OHDSI/DatabaseConnector)
-- [ ] [FeatureExtraction](https://github.com/OHDSI/FeatureExtraction)
-
-Release packages: `ohdsi-circe`, `ohdsi-capr`, `ohdsi-cohortgenerator`, `ohdsi-sqlrender`, `ohdsi-databaseconnector`, `ohdsi-featureextraction`
+Metadata-Version: 2.1
+Name: ohdsi-database-connector
+Version: 0.2.0
+Summary: Python wrapper for the OHDSI R packages
+Home-page: https://github.com/vantage6/python-ohdsi
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
+# python-ohdsi
+Python wrappers for (some) OHDSI tools. This project has been initiated for supporting
+OMOP data sources in vantage6.
+
+# TODO
+Packages to be wrapped:
+- [ ] [Capr](https://github.com/OHDSI/Capr)
+- [X] [CirceR](https://github.com/OHDSI/CirceR)
+- [X] [CohortGenerator](https://github.com/OHDSI/cohortgenerator)
+- [X] [SqlRender](https://github.com/OHDSI/SqlRender)
+- [X] [DatabaseConnector](https://github.com/OHDSI/DatabaseConnector)
+- [ ] [FeatureExtraction](https://github.com/OHDSI/FeatureExtraction)
+
+Release packages: `ohdsi-circe`, `ohdsi-capr`, `ohdsi-cohortgenerator`, `ohdsi-sqlrender`, `ohdsi-databaseconnector`, `ohdsi-featureextraction`
```

### Comparing `ohdsi-database-connector-0.1.0/setup.py` & `ohdsi-database-connector-0.2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,42 @@
-import codecs
-
-from setuptools import setup, find_namespace_packages
-from pathlib import Path
-
-# get current directory
-here = Path(__file__).parent.absolute()
-parent_dir = here.parent.absolute()
-
-# get the long description from the README file
-with codecs.open(parent_dir / 'README.md', encoding='utf-8') as f:
-    long_description = f.read()
-
-# setup the package
-setup(
-    name='ohdsi-database-connector',
-    version='0.1.0',
-    description='Python wrapper for the OHDSI R packages',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/vantage6/python-ohdsi',
-    packages=find_namespace_packages(include=['ohdsi.*']),
-    python_requires='>=3.10',
-    install_requires=[
-        'rpy2==3.5.12',
-    ],
-    extras_require={
-        'dev': []
-    },
-    package_data={
-        'ohdsi.database_connector.java': ['*.jar'],
-    },
-    # entry_points={
-    #     'console_scripts': [
-    #         'vserver-local=vantage6.server.cli.server:cli_server'
-    #     ]
-    # }
-)
+import codecs
+
+from setuptools import setup, find_namespace_packages
+from pathlib import Path
+
+# get current directory
+here = Path(__file__).parent.absolute()
+parent_dir = here.parent.absolute()
+
+# get the long description from the README file
+with codecs.open(parent_dir / 'README.md', encoding='utf-8') as f:
+    long_description = f.read()
+
+# get the version from the parent dir
+with open(parent_dir / 'VERSION') as f:
+    version = f.read().strip()
+
+# setup the package
+setup(
+    name='ohdsi-database-connector',
+    version=version,
+    description='Python wrapper for the OHDSI R packages',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://github.com/vantage6/python-ohdsi',
+    packages=find_namespace_packages(include=['ohdsi.*']),
+    python_requires='>=3.10',
+    install_requires=[
+        'rpy2==3.5.12',
+    ],
+    extras_require={
+        'dev': []
+    },
+    package_data={
+        'ohdsi.database_connector.java': ['*.jar'],
+    },
+    # entry_points={
+    #     'console_scripts': [
+    #         'vserver-local=vantage6.server.cli.server:cli_server'
+    #     ]
+    # }
+)
```

