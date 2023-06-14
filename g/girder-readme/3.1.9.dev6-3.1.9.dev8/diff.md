# Comparing `tmp/girder-readme-3.1.9.dev6.tar.gz` & `tmp/girder-readme-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-readme-3.1.9.dev6.tar", last modified: Wed Feb 23 16:10:00 2022, max compression
+gzip compressed data, was "dist/girder-readme-3.1.9.dev8.tar", last modified: Wed Feb 23 17:42:00 2022, max compression
```

## Comparing `girder-readme-3.1.9.dev6.tar` & `girder-readme-3.1.9.dev8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:00.000000 girder-readme-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:00.000000 girder-readme-3.1.9.dev6/girder_readme/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:00.000000 girder-readme-3.1.9.dev6/girder_readme/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:00.000000 girder-readme-3.1.9.dev6/girder_readme/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      283 2022-02-23 16:09:15.000000 girder-readme-3.1.9.dev6/girder_readme/web_client/stylesheets/readmeWidget.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:00.000000 girder-readme-3.1.9.dev6/girder_readme/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      101 2022-02-23 16:09:15.000000 girder-readme-3.1.9.dev6/girder_readme/web_client/templates/readmeWidget.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:00.000000 girder-readme-3.1.9.dev6/girder_readme/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      997 2022-02-23 16:09:15.000000 girder-readme-3.1.9.dev6/girder_readme/web_client/views/HierarchyWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       63 2022-02-23 16:09:15.000000 girder-readme-3.1.9.dev6/girder_readme/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      470 2022-02-23 16:09:15.000000 girder-readme-3.1.9.dev6/girder_readme/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      308 2022-02-23 16:09:15.000000 girder-readme-3.1.9.dev6/girder_readme/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1015 2022-02-23 16:09:15.000000 girder-readme-3.1.9.dev6/girder_readme/rest.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:00.000000 girder-readme-3.1.9.dev6/girder_readme.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      667 2022-02-23 16:09:59.000000 girder-readme-3.1.9.dev6/girder_readme.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      612 2022-02-23 16:10:00.000000 girder-readme-3.1.9.dev6/girder_readme.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:59.000000 girder-readme-3.1.9.dev6/girder_readme.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2022-02-23 16:09:59.000000 girder-readme-3.1.9.dev6/girder_readme.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:59.000000 girder-readme-3.1.9.dev6/girder_readme.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 16:09:59.000000 girder-readme-3.1.9.dev6/girder_readme.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2022-02-23 16:09:59.000000 girder-readme-3.1.9.dev6/girder_readme.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:00.000000 girder-readme-3.1.9.dev6/plugin_tests/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:00.000000 girder-readme-3.1.9.dev6/plugin_tests/data/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      272 2022-02-23 16:09:15.000000 girder-readme-3.1.9.dev6/plugin_tests/data/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1626 2022-02-23 16:09:15.000000 girder-readme-3.1.9.dev6/plugin_tests/readmeSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       51 2022-02-23 16:09:15.000000 girder-readme-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1662 2022-02-23 16:09:15.000000 girder-readme-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      667 2022-02-23 16:10:00.000000 girder-readme-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:10:00.000000 girder-readme-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:00.000000 girder-readme-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:00.000000 girder-readme-3.1.9.dev8/girder_readme/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:00.000000 girder-readme-3.1.9.dev8/girder_readme/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:00.000000 girder-readme-3.1.9.dev8/girder_readme/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      283 2022-02-23 17:41:16.000000 girder-readme-3.1.9.dev8/girder_readme/web_client/stylesheets/readmeWidget.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:00.000000 girder-readme-3.1.9.dev8/girder_readme/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      101 2022-02-23 17:41:16.000000 girder-readme-3.1.9.dev8/girder_readme/web_client/templates/readmeWidget.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:00.000000 girder-readme-3.1.9.dev8/girder_readme/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      997 2022-02-23 17:41:16.000000 girder-readme-3.1.9.dev8/girder_readme/web_client/views/HierarchyWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       63 2022-02-23 17:41:16.000000 girder-readme-3.1.9.dev8/girder_readme/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      470 2022-02-23 17:41:16.000000 girder-readme-3.1.9.dev8/girder_readme/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      308 2022-02-23 17:41:16.000000 girder-readme-3.1.9.dev8/girder_readme/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1015 2022-02-23 17:41:16.000000 girder-readme-3.1.9.dev8/girder_readme/rest.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:00.000000 girder-readme-3.1.9.dev8/girder_readme.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      667 2022-02-23 17:41:59.000000 girder-readme-3.1.9.dev8/girder_readme.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      612 2022-02-23 17:41:59.000000 girder-readme-3.1.9.dev8/girder_readme.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:59.000000 girder-readme-3.1.9.dev8/girder_readme.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2022-02-23 17:41:59.000000 girder-readme-3.1.9.dev8/girder_readme.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:59.000000 girder-readme-3.1.9.dev8/girder_readme.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 17:41:59.000000 girder-readme-3.1.9.dev8/girder_readme.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2022-02-23 17:41:59.000000 girder-readme-3.1.9.dev8/girder_readme.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:00.000000 girder-readme-3.1.9.dev8/plugin_tests/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:00.000000 girder-readme-3.1.9.dev8/plugin_tests/data/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      272 2022-02-23 17:41:16.000000 girder-readme-3.1.9.dev8/plugin_tests/data/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1626 2022-02-23 17:41:16.000000 girder-readme-3.1.9.dev8/plugin_tests/readmeSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       51 2022-02-23 17:41:16.000000 girder-readme-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1662 2022-02-23 17:41:16.000000 girder-readme-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      667 2022-02-23 17:42:00.000000 girder-readme-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:42:00.000000 girder-readme-3.1.9.dev8/setup.cfg
```

### Comparing `girder-readme-3.1.9.dev6/girder_readme/web_client/views/HierarchyWidget.js` & `girder-readme-3.1.9.dev8/girder_readme/web_client/views/HierarchyWidget.js`

 * *Files identical despite different names*

### Comparing `girder-readme-3.1.9.dev6/girder_readme/rest.py` & `girder-readme-3.1.9.dev8/girder_readme/rest.py`

 * *Files identical despite different names*

### Comparing `girder-readme-3.1.9.dev6/girder_readme.egg-info/PKG-INFO` & `girder-readme-3.1.9.dev8/girder_readme.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-readme
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Render READMEs from the folder view
 Home-page: UNKNOWN
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `girder-readme-3.1.9.dev6/girder_readme.egg-info/SOURCES.txt` & `girder-readme-3.1.9.dev8/girder_readme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-readme-3.1.9.dev6/plugin_tests/readmeSpec.js` & `girder-readme-3.1.9.dev8/plugin_tests/readmeSpec.js`

 * *Files identical despite different names*

### Comparing `girder-readme-3.1.9.dev6/setup.py` & `girder-readme-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-readme-3.1.9.dev6/PKG-INFO` & `girder-readme-3.1.9.dev8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-readme
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Render READMEs from the folder view
 Home-page: UNKNOWN
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

