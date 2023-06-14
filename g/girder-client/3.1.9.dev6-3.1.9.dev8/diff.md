# Comparing `tmp/girder-client-3.1.9.dev6.tar.gz` & `tmp/girder-client-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-client-3.1.9.dev6.tar", last modified: Wed Feb 23 16:10:16 2022, max compression
+gzip compressed data, was "dist/girder-client-3.1.9.dev8.tar", last modified: Wed Feb 23 17:42:17 2022, max compression
```

## Comparing `girder-client-3.1.9.dev6.tar` & `girder-client-3.1.9.dev8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:16.000000 girder-client-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:16.000000 girder-client-3.1.9.dev6/girder_client/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    68237 2022-02-23 16:09:15.000000 girder-client-3.1.9.dev6/girder_client/__init__.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    13559 2022-02-23 16:09:15.000000 girder-client-3.1.9.dev6/girder_client/cli.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:16.000000 girder-client-3.1.9.dev6/girder_client.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      834 2022-02-23 16:10:15.000000 girder-client-3.1.9.dev6/girder_client.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      326 2022-02-23 16:10:16.000000 girder-client-3.1.9.dev6/girder_client.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:10:15.000000 girder-client-3.1.9.dev6/girder_client.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       94 2022-02-23 16:10:15.000000 girder-client-3.1.9.dev6/girder_client.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:10:15.000000 girder-client-3.1.9.dev6/girder_client.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2022-02-23 16:10:15.000000 girder-client-3.1.9.dev6/girder_client.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2022-02-23 16:10:15.000000 girder-client-3.1.9.dev6/girder_client.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      309 2022-02-23 16:09:15.000000 girder-client-3.1.9.dev6/README.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1778 2022-02-23 16:09:15.000000 girder-client-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      834 2022-02-23 16:10:16.000000 girder-client-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:10:16.000000 girder-client-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:17.000000 girder-client-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:17.000000 girder-client-3.1.9.dev8/girder_client/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    68237 2022-02-23 17:41:16.000000 girder-client-3.1.9.dev8/girder_client/__init__.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    13559 2022-02-23 17:41:16.000000 girder-client-3.1.9.dev8/girder_client/cli.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:17.000000 girder-client-3.1.9.dev8/girder_client.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      834 2022-02-23 17:42:16.000000 girder-client-3.1.9.dev8/girder_client.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      326 2022-02-23 17:42:17.000000 girder-client-3.1.9.dev8/girder_client.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:42:16.000000 girder-client-3.1.9.dev8/girder_client.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       94 2022-02-23 17:42:16.000000 girder-client-3.1.9.dev8/girder_client.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:42:16.000000 girder-client-3.1.9.dev8/girder_client.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2022-02-23 17:42:16.000000 girder-client-3.1.9.dev8/girder_client.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2022-02-23 17:42:16.000000 girder-client-3.1.9.dev8/girder_client.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      309 2022-02-23 17:41:16.000000 girder-client-3.1.9.dev8/README.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1778 2022-02-23 17:41:16.000000 girder-client-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      834 2022-02-23 17:42:17.000000 girder-client-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:42:17.000000 girder-client-3.1.9.dev8/setup.cfg
```

### Comparing `girder-client-3.1.9.dev6/girder_client/__init__.py` & `girder-client-3.1.9.dev8/girder_client/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-client-3.1.9.dev6/girder_client/cli.py` & `girder-client-3.1.9.dev8/girder_client/cli.py`

 * *Files identical despite different names*

### Comparing `girder-client-3.1.9.dev6/girder_client.egg-info/PKG-INFO` & `girder-client-3.1.9.dev8/girder_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-client
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Python client for interacting with Girder servers
 Home-page: http://girder.readthedocs.org/en/latest/python-client.html
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `girder-client-3.1.9.dev6/setup.py` & `girder-client-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-client-3.1.9.dev6/PKG-INFO` & `girder-client-3.1.9.dev8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-client
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Python client for interacting with Girder servers
 Home-page: http://girder.readthedocs.org/en/latest/python-client.html
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

