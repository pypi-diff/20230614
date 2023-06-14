# Comparing `tmp/girder-gravatar-3.1.9.dev6.tar.gz` & `tmp/girder-gravatar-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-gravatar-3.1.9.dev6.tar", last modified: Wed Feb 23 16:09:42 2022, max compression
+gzip compressed data, was "dist/girder-gravatar-3.1.9.dev8.tar", last modified: Wed Feb 23 17:41:43 2022, max compression
```

## Comparing `girder-gravatar-3.1.9.dev6.tar` & `girder-gravatar-3.1.9.dev8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:42.000000 girder-gravatar-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:42.000000 girder-gravatar-3.1.9.dev6/girder_gravatar/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:42.000000 girder-gravatar-3.1.9.dev6/girder_gravatar/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:42.000000 girder-gravatar-3.1.9.dev6/girder_gravatar/web_client/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      367 2022-02-23 16:09:15.000000 girder-gravatar-3.1.9.dev6/girder_gravatar/web_client/models/UserModel.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:42.000000 girder-gravatar-3.1.9.dev6/girder_gravatar/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      554 2022-02-23 16:09:15.000000 girder-gravatar-3.1.9.dev6/girder_gravatar/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:42.000000 girder-gravatar-3.1.9.dev6/girder_gravatar/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2103 2022-02-23 16:09:15.000000 girder-gravatar-3.1.9.dev6/girder_gravatar/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       78 2022-02-23 16:09:15.000000 girder-gravatar-3.1.9.dev6/girder_gravatar/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      558 2022-02-23 16:09:15.000000 girder-gravatar-3.1.9.dev6/girder_gravatar/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      422 2022-02-23 16:09:15.000000 girder-gravatar-3.1.9.dev6/girder_gravatar/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1946 2022-02-23 16:09:15.000000 girder-gravatar-3.1.9.dev6/girder_gravatar/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      403 2022-02-23 16:09:15.000000 girder-gravatar-3.1.9.dev6/girder_gravatar/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:42.000000 girder-gravatar-3.1.9.dev6/girder_gravatar.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      739 2022-02-23 16:09:42.000000 girder-gravatar-3.1.9.dev6/girder_gravatar.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      664 2022-02-23 16:09:42.000000 girder-gravatar-3.1.9.dev6/girder_gravatar.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:42.000000 girder-gravatar-3.1.9.dev6/girder_gravatar.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       59 2022-02-23 16:09:42.000000 girder-gravatar-3.1.9.dev6/girder_gravatar.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:42.000000 girder-gravatar-3.1.9.dev6/girder_gravatar.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 16:09:42.000000 girder-gravatar-3.1.9.dev6/girder_gravatar.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2022-02-23 16:09:42.000000 girder-gravatar-3.1.9.dev6/girder_gravatar.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:42.000000 girder-gravatar-3.1.9.dev6/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-gravatar-3.1.9.dev6/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3130 2022-02-23 16:09:15.000000 girder-gravatar-3.1.9.dev6/plugin_tests/gravatar_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2022-02-23 16:09:15.000000 girder-gravatar-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1794 2022-02-23 16:09:15.000000 girder-gravatar-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      739 2022-02-23 16:09:42.000000 girder-gravatar-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:09:42.000000 girder-gravatar-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:43.000000 girder-gravatar-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:43.000000 girder-gravatar-3.1.9.dev8/girder_gravatar/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:43.000000 girder-gravatar-3.1.9.dev8/girder_gravatar/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:43.000000 girder-gravatar-3.1.9.dev8/girder_gravatar/web_client/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      367 2022-02-23 17:41:16.000000 girder-gravatar-3.1.9.dev8/girder_gravatar/web_client/models/UserModel.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:43.000000 girder-gravatar-3.1.9.dev8/girder_gravatar/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      554 2022-02-23 17:41:16.000000 girder-gravatar-3.1.9.dev8/girder_gravatar/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:43.000000 girder-gravatar-3.1.9.dev8/girder_gravatar/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2103 2022-02-23 17:41:16.000000 girder-gravatar-3.1.9.dev8/girder_gravatar/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       78 2022-02-23 17:41:16.000000 girder-gravatar-3.1.9.dev8/girder_gravatar/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      558 2022-02-23 17:41:16.000000 girder-gravatar-3.1.9.dev8/girder_gravatar/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      422 2022-02-23 17:41:16.000000 girder-gravatar-3.1.9.dev8/girder_gravatar/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1946 2022-02-23 17:41:16.000000 girder-gravatar-3.1.9.dev8/girder_gravatar/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      403 2022-02-23 17:41:16.000000 girder-gravatar-3.1.9.dev8/girder_gravatar/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:43.000000 girder-gravatar-3.1.9.dev8/girder_gravatar.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      739 2022-02-23 17:41:43.000000 girder-gravatar-3.1.9.dev8/girder_gravatar.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      664 2022-02-23 17:41:43.000000 girder-gravatar-3.1.9.dev8/girder_gravatar.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:43.000000 girder-gravatar-3.1.9.dev8/girder_gravatar.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       59 2022-02-23 17:41:43.000000 girder-gravatar-3.1.9.dev8/girder_gravatar.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:43.000000 girder-gravatar-3.1.9.dev8/girder_gravatar.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 17:41:43.000000 girder-gravatar-3.1.9.dev8/girder_gravatar.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2022-02-23 17:41:43.000000 girder-gravatar-3.1.9.dev8/girder_gravatar.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:43.000000 girder-gravatar-3.1.9.dev8/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-gravatar-3.1.9.dev8/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3130 2022-02-23 17:41:16.000000 girder-gravatar-3.1.9.dev8/plugin_tests/gravatar_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2022-02-23 17:41:16.000000 girder-gravatar-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1794 2022-02-23 17:41:16.000000 girder-gravatar-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      739 2022-02-23 17:41:43.000000 girder-gravatar-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:41:43.000000 girder-gravatar-3.1.9.dev8/setup.cfg
```

### Comparing `girder-gravatar-3.1.9.dev6/girder_gravatar/web_client/templates/configView.pug` & `girder-gravatar-3.1.9.dev8/girder_gravatar/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-gravatar-3.1.9.dev6/girder_gravatar/web_client/views/ConfigView.js` & `girder-gravatar-3.1.9.dev8/girder_gravatar/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-gravatar-3.1.9.dev6/girder_gravatar/web_client/package.json` & `girder-gravatar-3.1.9.dev8/girder_gravatar/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-gravatar-3.1.9.dev6/girder_gravatar/__init__.py` & `girder-gravatar-3.1.9.dev8/girder_gravatar/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-gravatar-3.1.9.dev6/girder_gravatar.egg-info/PKG-INFO` & `girder-gravatar-3.1.9.dev8/girder_gravatar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-gravatar
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Adds Gravatar URLs for users.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#gravatar-portraits
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `girder-gravatar-3.1.9.dev6/girder_gravatar.egg-info/SOURCES.txt` & `girder-gravatar-3.1.9.dev8/girder_gravatar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-gravatar-3.1.9.dev6/plugin_tests/gravatar_test.py` & `girder-gravatar-3.1.9.dev8/plugin_tests/gravatar_test.py`

 * *Files identical despite different names*

### Comparing `girder-gravatar-3.1.9.dev6/setup.py` & `girder-gravatar-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-gravatar-3.1.9.dev6/PKG-INFO` & `girder-gravatar-3.1.9.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-gravatar
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Adds Gravatar URLs for users.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#gravatar-portraits
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

