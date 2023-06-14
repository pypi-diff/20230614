# Comparing `tmp/girder-download-statistics-3.1.9.dev6.tar.gz` & `tmp/girder-download-statistics-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-download-statistics-3.1.9.dev6.tar", last modified: Wed Feb 23 16:09:38 2022, max compression
+gzip compressed data, was "dist/girder-download-statistics-3.1.9.dev8.tar", last modified: Wed Feb 23 17:41:38 2022, max compression
```

## Comparing `girder-download-statistics-3.1.9.dev6.tar` & `girder-download-statistics-3.1.9.dev8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:38.000000 girder-download-statistics-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:38.000000 girder-download-statistics-3.1.9.dev6/girder_download_statistics/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1171 2022-02-23 16:09:15.000000 girder-download-statistics-3.1.9.dev6/girder_download_statistics/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:38.000000 girder-download-statistics-3.1.9.dev6/girder_download_statistics.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      676 2022-02-23 16:09:37.000000 girder-download-statistics-3.1.9.dev6/girder_download_statistics.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      533 2022-02-23 16:09:38.000000 girder-download-statistics-3.1.9.dev6/girder_download_statistics.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:37.000000 girder-download-statistics-3.1.9.dev6/girder_download_statistics.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       91 2022-02-23 16:09:37.000000 girder-download-statistics-3.1.9.dev6/girder_download_statistics.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:37.000000 girder-download-statistics-3.1.9.dev6/girder_download_statistics.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 16:09:37.000000 girder-download-statistics-3.1.9.dev6/girder_download_statistics.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2022-02-23 16:09:37.000000 girder-download-statistics-3.1.9.dev6/girder_download_statistics.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:38.000000 girder-download-statistics-3.1.9.dev6/plugin_tests/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:38.000000 girder-download-statistics-3.1.9.dev6/plugin_tests/files/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2022-02-23 16:09:15.000000 girder-download-statistics-3.1.9.dev6/plugin_tests/files/txt1.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2022-02-23 16:09:15.000000 girder-download-statistics-3.1.9.dev6/plugin_tests/files/txt2.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-download-statistics-3.1.9.dev6/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6527 2022-02-23 16:09:15.000000 girder-download-statistics-3.1.9.dev6/plugin_tests/download_statistics_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       64 2022-02-23 16:09:15.000000 girder-download-statistics-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1744 2022-02-23 16:09:15.000000 girder-download-statistics-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      676 2022-02-23 16:09:38.000000 girder-download-statistics-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:09:38.000000 girder-download-statistics-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:38.000000 girder-download-statistics-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:38.000000 girder-download-statistics-3.1.9.dev8/girder_download_statistics/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1171 2022-02-23 17:41:16.000000 girder-download-statistics-3.1.9.dev8/girder_download_statistics/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:38.000000 girder-download-statistics-3.1.9.dev8/girder_download_statistics.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      676 2022-02-23 17:41:38.000000 girder-download-statistics-3.1.9.dev8/girder_download_statistics.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      533 2022-02-23 17:41:38.000000 girder-download-statistics-3.1.9.dev8/girder_download_statistics.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:38.000000 girder-download-statistics-3.1.9.dev8/girder_download_statistics.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       91 2022-02-23 17:41:38.000000 girder-download-statistics-3.1.9.dev8/girder_download_statistics.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:38.000000 girder-download-statistics-3.1.9.dev8/girder_download_statistics.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 17:41:38.000000 girder-download-statistics-3.1.9.dev8/girder_download_statistics.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2022-02-23 17:41:38.000000 girder-download-statistics-3.1.9.dev8/girder_download_statistics.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:38.000000 girder-download-statistics-3.1.9.dev8/plugin_tests/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:38.000000 girder-download-statistics-3.1.9.dev8/plugin_tests/files/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2022-02-23 17:41:16.000000 girder-download-statistics-3.1.9.dev8/plugin_tests/files/txt1.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2022-02-23 17:41:16.000000 girder-download-statistics-3.1.9.dev8/plugin_tests/files/txt2.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-download-statistics-3.1.9.dev8/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6527 2022-02-23 17:41:16.000000 girder-download-statistics-3.1.9.dev8/plugin_tests/download_statistics_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       64 2022-02-23 17:41:16.000000 girder-download-statistics-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1744 2022-02-23 17:41:16.000000 girder-download-statistics-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      676 2022-02-23 17:41:38.000000 girder-download-statistics-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:41:38.000000 girder-download-statistics-3.1.9.dev8/setup.cfg
```

### Comparing `girder-download-statistics-3.1.9.dev6/girder_download_statistics/__init__.py` & `girder-download-statistics-3.1.9.dev8/girder_download_statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-download-statistics-3.1.9.dev6/girder_download_statistics.egg-info/PKG-INFO` & `girder-download-statistics-3.1.9.dev8/girder_download_statistics.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-download-statistics
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Record file download statistics
 Home-page: UNKNOWN
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `girder-download-statistics-3.1.9.dev6/girder_download_statistics.egg-info/SOURCES.txt` & `girder-download-statistics-3.1.9.dev8/girder_download_statistics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-download-statistics-3.1.9.dev6/plugin_tests/download_statistics_test.py` & `girder-download-statistics-3.1.9.dev8/plugin_tests/download_statistics_test.py`

 * *Files identical despite different names*

### Comparing `girder-download-statistics-3.1.9.dev6/setup.py` & `girder-download-statistics-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-download-statistics-3.1.9.dev6/PKG-INFO` & `girder-download-statistics-3.1.9.dev8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-download-statistics
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Record file download statistics
 Home-page: UNKNOWN
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

