# Comparing `tmp/purpleair_data_logger-1.2.1.tar.gz` & `tmp/purpleair_data_logger-1.2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "purpleair_data_logger-1.2.1.tar", last modified: Wed Jun 14 04:24:31 2023, max compression
+gzip compressed data, was "purpleair_data_logger-1.2.1a1.tar", last modified: Thu May 18 04:50:42 2023, max compression
```

## Comparing `purpleair_data_logger-1.2.1.tar` & `purpleair_data_logger-1.2.1a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:24:31.469754 purpleair_data_logger-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-14 04:24:20.000000 purpleair_data_logger-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17094 2023-06-14 04:24:31.469754 purpleair_data_logger-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-06-14 04:24:20.000000 purpleair_data_logger-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:24:31.465754 purpleair_data_logger-1.2.1/purpleair_data_logger/
--rw-r--r--   0 runner    (1001) docker     (123)    20652 2023-06-14 04:24:20.000000 purpleair_data_logger-1.2.1/purpleair_data_logger/PurpleAirCSVDataLogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-14 04:24:20.000000 purpleair_data_logger-1.2.1/purpleair_data_logger/PurpleAirCSVDataLoggerConstants.py
--rw-r--r--   0 runner    (1001) docker     (123)    23354 2023-06-14 04:24:20.000000 purpleair_data_logger-1.2.1/purpleair_data_logger/PurpleAirDataLogger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23174 2023-06-14 04:24:20.000000 purpleair_data_logger-1.2.1/purpleair_data_logger/PurpleAirPSQLDataLogger.py
--rw-r--r--   0 runner    (1001) docker     (123)    19714 2023-06-14 04:24:20.000000 purpleair_data_logger-1.2.1/purpleair_data_logger/PurpleAirPSQLQueryStatements.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-14 04:24:20.000000 purpleair_data_logger-1.2.1/purpleair_data_logger/PurpleAirSQLiteDataLogger.py
--rw-r--r--   0 runner    (1001) docker     (123)    14086 2023-06-14 04:24:20.000000 purpleair_data_logger-1.2.1/purpleair_data_logger/PurpleAirSQLiteQueryStatements.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:24:20.000000 purpleair_data_logger-1.2.1/purpleair_data_logger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:24:31.469754 purpleair_data_logger-1.2.1/purpleair_data_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17094 2023-06-14 04:24:31.000000 purpleair_data_logger-1.2.1/purpleair_data_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-14 04:24:31.000000 purpleair_data_logger-1.2.1/purpleair_data_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:24:31.000000 purpleair_data_logger-1.2.1/purpleair_data_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 04:24:31.000000 purpleair_data_logger-1.2.1/purpleair_data_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 04:24:31.000000 purpleair_data_logger-1.2.1/purpleair_data_logger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-14 04:24:31.469754 purpleair_data_logger-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-14 04:24:20.000000 purpleair_data_logger-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:50:42.591796 purpleair_data_logger-1.2.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17096 2023-05-18 04:50:42.591796 purpleair_data_logger-1.2.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:50:42.591796 purpleair_data_logger-1.2.1a1/purpleair_data_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)    20652 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirCSVDataLogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirCSVDataLoggerConstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23354 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirDataLogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23174 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirPSQLDataLogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19714 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirPSQLQueryStatements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirSQLiteDataLogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14086 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirSQLiteQueryStatements.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:50:42.591796 purpleair_data_logger-1.2.1a1/purpleair_data_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17096 2023-05-18 04:50:42.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-18 04:50:42.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 04:50:42.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-18 04:50:42.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 04:50:42.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-18 04:50:42.591796 purpleair_data_logger-1.2.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/setup.py
```

### Comparing `purpleair_data_logger-1.2.1/LICENSE` & `purpleair_data_logger-1.2.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `purpleair_data_logger-1.2.1/PKG-INFO` & `purpleair_data_logger-1.2.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purpleair_data_logger
-Version: 1.2.1
+Version: 1.2.1a1
 Home-page: https://github.com/carlkidcrypto/purpleair_data_logger
 Author: Carlos Santos
 Author-email: dose.lucky.sake@cloak.id
 License: MIT
 Keywords: purpleair_data_logger,purple air,purple air data logger,PurpleAirPSQLDataLogger,PurpleAirCSVDataLogger,purple air api,PurpleAirSQLiteDataLogger
 Platform: Windows 32/64
 Platform: Linux 32/64
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: purpleair_data_logger Version: 1.2.1 Home-page:
+Metadata-Version: 2.1 Name: purpleair_data_logger Version: 1.2.1a1 Home-page:
 https://github.com/carlkidcrypto/purpleair_data_logger Author: Carlos Santos
 Author-email: dose.lucky.sake@cloak.id License: MIT Keywords:
 purpleair_data_logger,purple air,purple air data
 logger,PurpleAirPSQLDataLogger,PurpleAirCSVDataLogger,purple air
 api,PurpleAirSQLiteDataLogger Platform: Windows 32/64 Platform: Linux 32/64
 Platform: MacOS 32/64 Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE # Purple Air Data Logger(s) (PADLs) A set of
```

### Comparing `purpleair_data_logger-1.2.1/README.md` & `purpleair_data_logger-1.2.1a1/README.md`

 * *Files identical despite different names*

### Comparing `purpleair_data_logger-1.2.1/purpleair_data_logger/PurpleAirCSVDataLogger.py` & `purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirCSVDataLogger.py`

 * *Files identical despite different names*

### Comparing `purpleair_data_logger-1.2.1/purpleair_data_logger/PurpleAirCSVDataLoggerConstants.py` & `purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirCSVDataLoggerConstants.py`

 * *Files identical despite different names*

### Comparing `purpleair_data_logger-1.2.1/purpleair_data_logger/PurpleAirDataLogger.py` & `purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirDataLogger.py`

 * *Files identical despite different names*

### Comparing `purpleair_data_logger-1.2.1/purpleair_data_logger/PurpleAirPSQLDataLogger.py` & `purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirPSQLDataLogger.py`

 * *Files identical despite different names*

### Comparing `purpleair_data_logger-1.2.1/purpleair_data_logger/PurpleAirPSQLQueryStatements.py` & `purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirPSQLQueryStatements.py`

 * *Files identical despite different names*

### Comparing `purpleair_data_logger-1.2.1/purpleair_data_logger/PurpleAirSQLiteDataLogger.py` & `purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirSQLiteDataLogger.py`

 * *Files identical despite different names*

### Comparing `purpleair_data_logger-1.2.1/purpleair_data_logger/PurpleAirSQLiteQueryStatements.py` & `purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirSQLiteQueryStatements.py`

 * *Files identical despite different names*

### Comparing `purpleair_data_logger-1.2.1/purpleair_data_logger.egg-info/PKG-INFO` & `purpleair_data_logger-1.2.1a1/purpleair_data_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purpleair-data-logger
-Version: 1.2.1
+Version: 1.2.1a1
 Home-page: https://github.com/carlkidcrypto/purpleair_data_logger
 Author: Carlos Santos
 Author-email: dose.lucky.sake@cloak.id
 License: MIT
 Keywords: purpleair_data_logger,purple air,purple air data logger,PurpleAirPSQLDataLogger,PurpleAirCSVDataLogger,purple air api,PurpleAirSQLiteDataLogger
 Platform: Windows 32/64
 Platform: Linux 32/64
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: purpleair-data-logger Version: 1.2.1 Home-page:
+Metadata-Version: 2.1 Name: purpleair-data-logger Version: 1.2.1a1 Home-page:
 https://github.com/carlkidcrypto/purpleair_data_logger Author: Carlos Santos
 Author-email: dose.lucky.sake@cloak.id License: MIT Keywords:
 purpleair_data_logger,purple air,purple air data
 logger,PurpleAirPSQLDataLogger,PurpleAirCSVDataLogger,purple air
 api,PurpleAirSQLiteDataLogger Platform: Windows 32/64 Platform: Linux 32/64
 Platform: MacOS 32/64 Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE # Purple Air Data Logger(s) (PADLs) A set of
```

### Comparing `purpleair_data_logger-1.2.1/purpleair_data_logger.egg-info/SOURCES.txt` & `purpleair_data_logger-1.2.1a1/purpleair_data_logger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `purpleair_data_logger-1.2.1/setup.py` & `purpleair_data_logger-1.2.1a1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         os.path.join(os.path.dirname(__file__), filename), encoding="utf-8"
     ) as file:
         return file.read()
 
 
 setup(
     name="purpleair_data_logger",
-    version="1.2.1",
+    version="1.2.1a1",
     license="MIT",
     author="Carlos Santos",
     author_email="dose.lucky.sake@cloak.id",
     long_description=read_file("README.md"),
     long_description_content_type="text/markdown",
     packages=["purpleair_data_logger"],
     url="https://github.com/carlkidcrypto/purpleair_data_logger",
@@ -25,10 +25,10 @@
         "purple air",
         "purple air data logger",
         "PurpleAirPSQLDataLogger",
         "PurpleAirCSVDataLogger",
         "purple air api",
         "PurpleAirSQLiteDataLogger",
     ],
-    install_requires=["pg8000==1.29.6", "requests", "purpleair_api==1.0.2"],
+    install_requires=["pg8000==1.29.5", "requests", "purpleair_api==1.0.2a1"],
     platforms=["Windows 32/64", "Linux 32/64", "MacOS 32/64"],
 )
```

