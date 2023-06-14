# Comparing `tmp/logging-gelf-0.0.8.tar.gz` & `tmp/logging-gelf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/logging-gelf-0.0.8.tar", last modified: Tue Oct 24 10:15:54 2017, max compression
+gzip compressed data, was "dist/logging-gelf-0.0.9.tar", last modified: Wed Mar 14 16:50:33 2018, max compression
```

## Comparing `logging-gelf-0.0.8.tar` & `logging-gelf-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-10-24 10:15:54.000000 logging-gelf-0.0.8/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-10-24 10:15:54.000000 logging-gelf-0.0.8/src/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-10-24 10:15:54.000000 logging-gelf-0.0.8/src/logging_gelf/
--rw-r--r--   0 travis    (2000) travis    (2000)      896 2017-10-24 10:15:30.000000 logging-gelf-0.0.8/src/logging_gelf/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1858 2017-10-24 10:15:30.000000 logging-gelf-0.0.8/src/logging_gelf/formatters.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1470 2017-10-24 10:15:30.000000 logging-gelf-0.0.8/src/logging_gelf/handlers.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2334 2017-10-24 10:15:30.000000 logging-gelf-0.0.8/src/logging_gelf/schemas.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-10-24 10:15:54.000000 logging-gelf-0.0.8/src/logging_gelf.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     2503 2017-10-24 10:15:54.000000 logging-gelf-0.0.8/src/logging_gelf.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      407 2017-10-24 10:15:54.000000 logging-gelf-0.0.8/src/logging_gelf.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2017-10-24 10:15:54.000000 logging-gelf-0.0.8/src/logging_gelf.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       12 2017-10-24 10:15:54.000000 logging-gelf-0.0.8/src/logging_gelf.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       13 2017-10-24 10:15:54.000000 logging-gelf-0.0.8/src/logging_gelf.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2017-10-24 10:15:54.000000 logging-gelf-0.0.8/src/logging_gelf.egg-info/zip-safe
--rw-r--r--   0 travis    (2000) travis    (2000)       56 2017-10-24 10:15:30.000000 logging-gelf-0.0.8/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)     1684 2017-10-24 10:15:30.000000 logging-gelf-0.0.8/README.rst
--rw-r--r--   0 travis    (2000) travis    (2000)        6 2017-10-24 10:15:30.000000 logging-gelf-0.0.8/VERSION
--rw-r--r--   0 travis    (2000) travis    (2000)       11 2017-10-24 10:15:30.000000 logging-gelf-0.0.8/requirements.txt
--rwxr-xr-x   0 travis    (2000) travis    (2000)      792 2017-10-24 10:15:30.000000 logging-gelf-0.0.8/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2503 2017-10-24 10:15:54.000000 logging-gelf-0.0.8/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)       38 2017-10-24 10:15:54.000000 logging-gelf-0.0.8/setup.cfg
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-03-14 16:50:33.000000 logging-gelf-0.0.9/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-03-14 16:50:33.000000 logging-gelf-0.0.9/src/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-03-14 16:50:33.000000 logging-gelf-0.0.9/src/logging_gelf/
+-rw-r--r--   0 travis    (2000) travis    (2000)      896 2018-03-14 16:50:10.000000 logging-gelf-0.0.9/src/logging_gelf/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1853 2018-03-14 16:50:10.000000 logging-gelf-0.0.9/src/logging_gelf/formatters.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1470 2018-03-14 16:50:10.000000 logging-gelf-0.0.9/src/logging_gelf/handlers.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2334 2018-03-14 16:50:10.000000 logging-gelf-0.0.9/src/logging_gelf/schemas.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-03-14 16:50:33.000000 logging-gelf-0.0.9/src/logging_gelf.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     2537 2018-03-14 16:50:33.000000 logging-gelf-0.0.9/src/logging_gelf.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)      407 2018-03-14 16:50:33.000000 logging-gelf-0.0.9/src/logging_gelf.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-03-14 16:50:33.000000 logging-gelf-0.0.9/src/logging_gelf.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       21 2018-03-14 16:50:33.000000 logging-gelf-0.0.9/src/logging_gelf.egg-info/requires.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       13 2018-03-14 16:50:33.000000 logging-gelf-0.0.9/src/logging_gelf.egg-info/top_level.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-03-14 16:50:33.000000 logging-gelf-0.0.9/src/logging_gelf.egg-info/zip-safe
+-rw-r--r--   0 travis    (2000) travis    (2000)       56 2018-03-14 16:50:10.000000 logging-gelf-0.0.9/MANIFEST.in
+-rw-r--r--   0 travis    (2000) travis    (2000)     1684 2018-03-14 16:50:10.000000 logging-gelf-0.0.9/README.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)        6 2018-03-14 16:50:10.000000 logging-gelf-0.0.9/VERSION
+-rw-r--r--   0 travis    (2000) travis    (2000)       20 2018-03-14 16:50:10.000000 logging-gelf-0.0.9/requirements.txt
+-rwxr-xr-x   0 travis    (2000) travis    (2000)      792 2018-03-14 16:50:10.000000 logging-gelf-0.0.9/setup.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2537 2018-03-14 16:50:33.000000 logging-gelf-0.0.9/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)       38 2018-03-14 16:50:33.000000 logging-gelf-0.0.9/setup.cfg
```

### Comparing `logging-gelf-0.0.8/src/logging_gelf/__init__.py` & `logging-gelf-0.0.9/src/logging_gelf/__init__.py`

 * *Files identical despite different names*

### Comparing `logging-gelf-0.0.8/src/logging_gelf/formatters.py` & `logging-gelf-0.0.9/src/logging_gelf/formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,11 +47,11 @@
         inherit from :class:`logging_gelf.schemas.GelfSchema`.
 
         :param logging.LogRecord record: Contains all the information pertinent
         to the event being logged.
         :return: A JSON dump of the record.
         :rtype: str
         """
-        out = json.dumps(self.schema().dump(record).data, cls=self._encoder_cls)
+        out = json.dumps(self.schema().dump(record), cls=self._encoder_cls)
         if self.null_character is True:
             out += '\0'
         return out
```

### Comparing `logging-gelf-0.0.8/src/logging_gelf/handlers.py` & `logging-gelf-0.0.9/src/logging_gelf/handlers.py`

 * *Files identical despite different names*

### Comparing `logging-gelf-0.0.8/src/logging_gelf/schemas.py` & `logging-gelf-0.0.9/src/logging_gelf/schemas.py`

 * *Files identical despite different names*

### Comparing `logging-gelf-0.0.8/src/logging_gelf.egg-info/PKG-INFO` & `logging-gelf-0.0.9/src/logging_gelf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: logging-gelf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Logging bundle to send logs using GELF
 Home-page: https://github.com/cdumay/logging-gelf
 Author: Cedric DUMAY
 Author-email: cedric.dumay@gmail.com
 License: Apache License 2.0
+Description-Content-Type: UNKNOWN
 Description: ************
         Logging GELF
         ************
         
         .. image:: https://img.shields.io/pypi/v/logging-gelf.svg
            :target: https://pypi.python.org/pypi/logging-gelf/
            :alt: Latest Version
```

### Comparing `logging-gelf-0.0.8/README.rst` & `logging-gelf-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `logging-gelf-0.0.8/setup.py` & `logging-gelf-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `logging-gelf-0.0.8/PKG-INFO` & `logging-gelf-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: logging-gelf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Logging bundle to send logs using GELF
 Home-page: https://github.com/cdumay/logging-gelf
 Author: Cedric DUMAY
 Author-email: cedric.dumay@gmail.com
 License: Apache License 2.0
+Description-Content-Type: UNKNOWN
 Description: ************
         Logging GELF
         ************
         
         .. image:: https://img.shields.io/pypi/v/logging-gelf.svg
            :target: https://pypi.python.org/pypi/logging-gelf/
            :alt: Latest Version
```

