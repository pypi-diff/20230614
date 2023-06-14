# Comparing `tmp/girder-virtual-folders-3.1.9.dev6.tar.gz` & `tmp/girder-virtual-folders-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-virtual-folders-3.1.9.dev6.tar", last modified: Wed Feb 23 16:10:10 2022, max compression
+gzip compressed data, was "dist/girder-virtual-folders-3.1.9.dev8.tar", last modified: Wed Feb 23 17:42:11 2022, max compression
```

## Comparing `girder-virtual-folders-3.1.9.dev6.tar` & `girder-virtual-folders-3.1.9.dev8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:10.000000 girder-virtual-folders-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:10.000000 girder-virtual-folders-3.1.9.dev6/girder_virtual_folders/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8194 2022-02-23 16:09:15.000000 girder-virtual-folders-3.1.9.dev6/girder_virtual_folders/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:10.000000 girder-virtual-folders-3.1.9.dev6/girder_virtual_folders.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      708 2022-02-23 16:10:10.000000 girder-virtual-folders-3.1.9.dev6/girder_virtual_folders.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      441 2022-02-23 16:10:10.000000 girder-virtual-folders-3.1.9.dev6/girder_virtual_folders.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:10:10.000000 girder-virtual-folders-3.1.9.dev6/girder_virtual_folders.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       79 2022-02-23 16:10:10.000000 girder-virtual-folders-3.1.9.dev6/girder_virtual_folders.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:10:10.000000 girder-virtual-folders-3.1.9.dev6/girder_virtual_folders.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 16:10:10.000000 girder-virtual-folders-3.1.9.dev6/girder_virtual_folders.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       23 2022-02-23 16:10:10.000000 girder-virtual-folders-3.1.9.dev6/girder_virtual_folders.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:10.000000 girder-virtual-folders-3.1.9.dev6/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-virtual-folders-3.1.9.dev6/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6178 2022-02-23 16:09:15.000000 girder-virtual-folders-3.1.9.dev6/plugin_tests/virtual_folders_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2022-02-23 16:09:15.000000 girder-virtual-folders-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1764 2022-02-23 16:09:15.000000 girder-virtual-folders-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      708 2022-02-23 16:10:10.000000 girder-virtual-folders-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:10:10.000000 girder-virtual-folders-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:11.000000 girder-virtual-folders-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:11.000000 girder-virtual-folders-3.1.9.dev8/girder_virtual_folders/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8194 2022-02-23 17:41:16.000000 girder-virtual-folders-3.1.9.dev8/girder_virtual_folders/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:11.000000 girder-virtual-folders-3.1.9.dev8/girder_virtual_folders.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      708 2022-02-23 17:42:11.000000 girder-virtual-folders-3.1.9.dev8/girder_virtual_folders.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      441 2022-02-23 17:42:11.000000 girder-virtual-folders-3.1.9.dev8/girder_virtual_folders.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:42:11.000000 girder-virtual-folders-3.1.9.dev8/girder_virtual_folders.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       79 2022-02-23 17:42:11.000000 girder-virtual-folders-3.1.9.dev8/girder_virtual_folders.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:42:11.000000 girder-virtual-folders-3.1.9.dev8/girder_virtual_folders.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 17:42:11.000000 girder-virtual-folders-3.1.9.dev8/girder_virtual_folders.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       23 2022-02-23 17:42:11.000000 girder-virtual-folders-3.1.9.dev8/girder_virtual_folders.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:11.000000 girder-virtual-folders-3.1.9.dev8/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-virtual-folders-3.1.9.dev8/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6178 2022-02-23 17:41:16.000000 girder-virtual-folders-3.1.9.dev8/plugin_tests/virtual_folders_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2022-02-23 17:41:16.000000 girder-virtual-folders-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1764 2022-02-23 17:41:16.000000 girder-virtual-folders-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      708 2022-02-23 17:42:11.000000 girder-virtual-folders-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:42:11.000000 girder-virtual-folders-3.1.9.dev8/setup.cfg
```

### Comparing `girder-virtual-folders-3.1.9.dev6/girder_virtual_folders/__init__.py` & `girder-virtual-folders-3.1.9.dev8/girder_virtual_folders/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-virtual-folders-3.1.9.dev6/girder_virtual_folders.egg-info/PKG-INFO` & `girder-virtual-folders-3.1.9.dev8/girder_virtual_folders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-virtual-folders
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Allows folders to list child items using arbitrary database queries
 Home-page: UNKNOWN
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `girder-virtual-folders-3.1.9.dev6/plugin_tests/virtual_folders_test.py` & `girder-virtual-folders-3.1.9.dev8/plugin_tests/virtual_folders_test.py`

 * *Files identical despite different names*

### Comparing `girder-virtual-folders-3.1.9.dev6/setup.py` & `girder-virtual-folders-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-virtual-folders-3.1.9.dev6/PKG-INFO` & `girder-virtual-folders-3.1.9.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-virtual-folders
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Allows folders to list child items using arbitrary database queries
 Home-page: UNKNOWN
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

