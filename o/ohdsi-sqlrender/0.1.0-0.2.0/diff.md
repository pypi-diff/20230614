# Comparing `tmp/ohdsi-sqlrender-0.1.0.tar.gz` & `tmp/ohdsi-sqlrender-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohdsi-sqlrender-0.1.0.tar", last modified: Tue Jun 13 14:53:58 2023, max compression
+gzip compressed data, was "ohdsi-sqlrender-0.2.0.tar", last modified: Wed Jun 14 08:26:52 2023, max compression
```

## Comparing `ohdsi-sqlrender-0.1.0.tar` & `ohdsi-sqlrender-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:58.842019 ohdsi-sqlrender-0.1.0/
--rw-rw-rw-   0        0        0      944 2023-06-13 14:53:58.842019 ohdsi-sqlrender-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:58.826394 ohdsi-sqlrender-0.1.0/ohdsi/
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:58.826394 ohdsi-sqlrender-0.1.0/ohdsi/sqlrender/
--rw-rw-rw-   0        0        0    12504 2023-06-08 13:22:08.000000 ohdsi-sqlrender-0.1.0/ohdsi/sqlrender/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:58.842019 ohdsi-sqlrender-0.1.0/ohdsi_sqlrender.egg-info/
--rw-rw-rw-   0        0        0      944 2023-06-13 14:53:58.000000 ohdsi-sqlrender-0.1.0/ohdsi_sqlrender.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-06-13 14:53:58.000000 ohdsi-sqlrender-0.1.0/ohdsi_sqlrender.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 14:53:58.000000 ohdsi-sqlrender-0.1.0/ohdsi_sqlrender.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-13 14:53:58.000000 ohdsi-sqlrender-0.1.0/ohdsi_sqlrender.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 14:53:58.000000 ohdsi-sqlrender-0.1.0/ohdsi_sqlrender.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 14:53:58.842019 ohdsi-sqlrender-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1060 2023-06-08 13:17:51.000000 ohdsi-sqlrender-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:52.025513 ohdsi-sqlrender-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-14 08:26:52.025513 ohdsi-sqlrender-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:52.025513 ohdsi-sqlrender-0.2.0/ohdsi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:52.025513 ohdsi-sqlrender-0.2.0/ohdsi/sqlrender/
+-rw-r--r--   0 runner    (1001) docker     (123)    12125 2023-06-14 08:26:29.000000 ohdsi-sqlrender-0.2.0/ohdsi/sqlrender/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:52.025513 ohdsi-sqlrender-0.2.0/ohdsi_sqlrender.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-14 08:26:51.000000 ohdsi-sqlrender-0.2.0/ohdsi_sqlrender.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 08:26:51.000000 ohdsi-sqlrender-0.2.0/ohdsi_sqlrender.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:26:51.000000 ohdsi-sqlrender-0.2.0/ohdsi_sqlrender.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 08:26:51.000000 ohdsi-sqlrender-0.2.0/ohdsi_sqlrender.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 08:26:51.000000 ohdsi-sqlrender-0.2.0/ohdsi_sqlrender.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:26:52.025513 ohdsi-sqlrender-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-14 08:26:29.000000 ohdsi-sqlrender-0.2.0/setup.py
```

### Comparing `ohdsi-sqlrender-0.1.0/PKG-INFO` & `ohdsi-sqlrender-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1
-Name: ohdsi-sqlrender
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
+Name: ohdsi-sqlrender
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

### Comparing `ohdsi-sqlrender-0.1.0/ohdsi_sqlrender.egg-info/PKG-INFO` & `ohdsi-sqlrender-0.2.0/ohdsi_sqlrender.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1
-Name: ohdsi-sqlrender
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
+Name: ohdsi-sqlrender
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

### Comparing `ohdsi-sqlrender-0.1.0/setup.py` & `ohdsi-sqlrender-0.2.0/setup.py`

 * *Files 27% similar despite different names*

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
-    name='ohdsi-sqlrender',
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
-        'ohdsi.sqlrender.data': ['*.json'],
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
+    name='ohdsi-sqlrender',
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
+        'ohdsi.sqlrender.data': ['*.json'],
+    },
+    # entry_points={
+    #     'console_scripts': [
+    #         'vserver-local=vantage6.server.cli.server:cli_server'
+    #     ]
+    # }
+)
```

