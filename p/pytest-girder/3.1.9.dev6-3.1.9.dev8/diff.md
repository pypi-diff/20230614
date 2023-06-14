# Comparing `tmp/pytest-girder-3.1.9.dev6.tar.gz` & `tmp/pytest-girder-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-girder-3.1.9.dev6.tar", last modified: Wed Feb 23 16:10:12 2022, max compression
+gzip compressed data, was "dist/pytest-girder-3.1.9.dev8.tar", last modified: Wed Feb 23 17:42:14 2022, max compression
```

## Comparing `pytest-girder-3.1.9.dev6.tar` & `pytest-girder-3.1.9.dev8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:12.000000 pytest-girder-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:12.000000 pytest-girder-3.1.9.dev6/pytest_girder/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 pytest-girder-3.1.9.dev6/pytest_girder/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1022 2022-02-23 16:09:15.000000 pytest-girder-3.1.9.dev6/pytest_girder/assertions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6446 2022-02-23 16:09:15.000000 pytest-girder-3.1.9.dev6/pytest_girder/fixtures.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1772 2022-02-23 16:09:15.000000 pytest-girder-3.1.9.dev6/pytest_girder/plugin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2671 2022-02-23 16:09:15.000000 pytest-girder-3.1.9.dev6/pytest_girder/plugin_registry.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11116 2022-02-23 16:09:15.000000 pytest-girder-3.1.9.dev6/pytest_girder/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5970 2022-02-23 16:09:15.000000 pytest-girder-3.1.9.dev6/pytest_girder/web_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:12.000000 pytest-girder-3.1.9.dev6/pytest_girder.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      306 2022-02-23 16:10:12.000000 pytest-girder-3.1.9.dev6/pytest_girder.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      440 2022-02-23 16:10:12.000000 pytest-girder-3.1.9.dev6/pytest_girder.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:10:12.000000 pytest-girder-3.1.9.dev6/pytest_girder.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       42 2022-02-23 16:10:12.000000 pytest-girder-3.1.9.dev6/pytest_girder.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       51 2022-02-23 16:10:12.000000 pytest-girder-3.1.9.dev6/pytest_girder.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2022-02-23 16:10:12.000000 pytest-girder-3.1.9.dev6/pytest_girder.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2022-02-23 16:09:15.000000 pytest-girder-3.1.9.dev6/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2022-02-23 16:09:15.000000 pytest-girder-3.1.9.dev6/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1266 2022-02-23 16:09:15.000000 pytest-girder-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      306 2022-02-23 16:10:12.000000 pytest-girder-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:10:12.000000 pytest-girder-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:14.000000 pytest-girder-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:14.000000 pytest-girder-3.1.9.dev8/pytest_girder/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 pytest-girder-3.1.9.dev8/pytest_girder/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1022 2022-02-23 17:41:16.000000 pytest-girder-3.1.9.dev8/pytest_girder/assertions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6446 2022-02-23 17:41:16.000000 pytest-girder-3.1.9.dev8/pytest_girder/fixtures.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1772 2022-02-23 17:41:16.000000 pytest-girder-3.1.9.dev8/pytest_girder/plugin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2671 2022-02-23 17:41:16.000000 pytest-girder-3.1.9.dev8/pytest_girder/plugin_registry.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11116 2022-02-23 17:41:16.000000 pytest-girder-3.1.9.dev8/pytest_girder/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5970 2022-02-23 17:41:16.000000 pytest-girder-3.1.9.dev8/pytest_girder/web_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:14.000000 pytest-girder-3.1.9.dev8/pytest_girder.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      306 2022-02-23 17:42:14.000000 pytest-girder-3.1.9.dev8/pytest_girder.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      440 2022-02-23 17:42:14.000000 pytest-girder-3.1.9.dev8/pytest_girder.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:42:14.000000 pytest-girder-3.1.9.dev8/pytest_girder.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       42 2022-02-23 17:42:14.000000 pytest-girder-3.1.9.dev8/pytest_girder.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       51 2022-02-23 17:42:14.000000 pytest-girder-3.1.9.dev8/pytest_girder.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2022-02-23 17:42:14.000000 pytest-girder-3.1.9.dev8/pytest_girder.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2022-02-23 17:41:16.000000 pytest-girder-3.1.9.dev8/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2022-02-23 17:41:16.000000 pytest-girder-3.1.9.dev8/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1266 2022-02-23 17:41:16.000000 pytest-girder-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      306 2022-02-23 17:42:14.000000 pytest-girder-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:42:14.000000 pytest-girder-3.1.9.dev8/setup.cfg
```

### Comparing `pytest-girder-3.1.9.dev6/pytest_girder/assertions.py` & `pytest-girder-3.1.9.dev8/pytest_girder/assertions.py`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.1.9.dev6/pytest_girder/fixtures.py` & `pytest-girder-3.1.9.dev8/pytest_girder/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.1.9.dev6/pytest_girder/plugin.py` & `pytest-girder-3.1.9.dev8/pytest_girder/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.1.9.dev6/pytest_girder/plugin_registry.py` & `pytest-girder-3.1.9.dev8/pytest_girder/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.1.9.dev6/pytest_girder/utils.py` & `pytest-girder-3.1.9.dev8/pytest_girder/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.1.9.dev6/pytest_girder/web_client.py` & `pytest-girder-3.1.9.dev8/pytest_girder/web_client.py`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.1.9.dev6/LICENSE` & `pytest-girder-3.1.9.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.1.9.dev6/setup.py` & `pytest-girder-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

