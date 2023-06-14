# Comparing `tmp/girder-autojoin-3.1.9.dev6.tar.gz` & `tmp/girder-autojoin-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-autojoin-3.1.9.dev6.tar", last modified: Wed Feb 23 16:09:33 2022, max compression
+gzip compressed data, was "dist/girder-autojoin-3.1.9.dev8.tar", last modified: Wed Feb 23 17:41:33 2022, max compression
```

## Comparing `girder-autojoin-3.1.9.dev6.tar` & `girder-autojoin-3.1.9.dev8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:33.000000 girder-autojoin-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:33.000000 girder-autojoin-3.1.9.dev6/girder_autojoin/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:33.000000 girder-autojoin-3.1.9.dev6/girder_autojoin/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:33.000000 girder-autojoin-3.1.9.dev6/girder_autojoin/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       92 2022-02-23 16:09:15.000000 girder-autojoin-3.1.9.dev6/girder_autojoin/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:33.000000 girder-autojoin-3.1.9.dev6/girder_autojoin/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1805 2022-02-23 16:09:15.000000 girder-autojoin-3.1.9.dev6/girder_autojoin/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:33.000000 girder-autojoin-3.1.9.dev6/girder_autojoin/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3781 2022-02-23 16:09:15.000000 girder-autojoin-3.1.9.dev6/girder_autojoin/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2022-02-23 16:09:15.000000 girder-autojoin-3.1.9.dev6/girder_autojoin/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      588 2022-02-23 16:09:15.000000 girder-autojoin-3.1.9.dev6/girder_autojoin/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      422 2022-02-23 16:09:15.000000 girder-autojoin-3.1.9.dev6/girder_autojoin/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      905 2022-02-23 16:09:15.000000 girder-autojoin-3.1.9.dev6/girder_autojoin/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1022 2022-02-23 16:09:15.000000 girder-autojoin-3.1.9.dev6/girder_autojoin/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:33.000000 girder-autojoin-3.1.9.dev6/girder_autojoin.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      756 2022-02-23 16:09:32.000000 girder-autojoin-3.1.9.dev6/girder_autojoin.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2022-02-23 16:09:32.000000 girder-autojoin-3.1.9.dev6/girder_autojoin.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:32.000000 girder-autojoin-3.1.9.dev6/girder_autojoin.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       59 2022-02-23 16:09:32.000000 girder-autojoin-3.1.9.dev6/girder_autojoin.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:32.000000 girder-autojoin-3.1.9.dev6/girder_autojoin.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 16:09:32.000000 girder-autojoin-3.1.9.dev6/girder_autojoin.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2022-02-23 16:09:32.000000 girder-autojoin-3.1.9.dev6/girder_autojoin.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:33.000000 girder-autojoin-3.1.9.dev6/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-autojoin-3.1.9.dev6/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3790 2022-02-23 16:09:15.000000 girder-autojoin-3.1.9.dev6/plugin_tests/autojoinSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2418 2022-02-23 16:09:15.000000 girder-autojoin-3.1.9.dev6/plugin_tests/autojoin_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2022-02-23 16:09:15.000000 girder-autojoin-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1811 2022-02-23 16:09:15.000000 girder-autojoin-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      756 2022-02-23 16:09:33.000000 girder-autojoin-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:09:33.000000 girder-autojoin-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:33.000000 girder-autojoin-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:33.000000 girder-autojoin-3.1.9.dev8/girder_autojoin/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:33.000000 girder-autojoin-3.1.9.dev8/girder_autojoin/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:33.000000 girder-autojoin-3.1.9.dev8/girder_autojoin/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       92 2022-02-23 17:41:16.000000 girder-autojoin-3.1.9.dev8/girder_autojoin/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:33.000000 girder-autojoin-3.1.9.dev8/girder_autojoin/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1805 2022-02-23 17:41:16.000000 girder-autojoin-3.1.9.dev8/girder_autojoin/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:33.000000 girder-autojoin-3.1.9.dev8/girder_autojoin/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3781 2022-02-23 17:41:16.000000 girder-autojoin-3.1.9.dev8/girder_autojoin/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2022-02-23 17:41:16.000000 girder-autojoin-3.1.9.dev8/girder_autojoin/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      588 2022-02-23 17:41:16.000000 girder-autojoin-3.1.9.dev8/girder_autojoin/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      422 2022-02-23 17:41:16.000000 girder-autojoin-3.1.9.dev8/girder_autojoin/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      905 2022-02-23 17:41:16.000000 girder-autojoin-3.1.9.dev8/girder_autojoin/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1022 2022-02-23 17:41:16.000000 girder-autojoin-3.1.9.dev8/girder_autojoin/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:33.000000 girder-autojoin-3.1.9.dev8/girder_autojoin.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      756 2022-02-23 17:41:33.000000 girder-autojoin-3.1.9.dev8/girder_autojoin.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2022-02-23 17:41:33.000000 girder-autojoin-3.1.9.dev8/girder_autojoin.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:33.000000 girder-autojoin-3.1.9.dev8/girder_autojoin.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       59 2022-02-23 17:41:33.000000 girder-autojoin-3.1.9.dev8/girder_autojoin.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:33.000000 girder-autojoin-3.1.9.dev8/girder_autojoin.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 17:41:33.000000 girder-autojoin-3.1.9.dev8/girder_autojoin.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2022-02-23 17:41:33.000000 girder-autojoin-3.1.9.dev8/girder_autojoin.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:33.000000 girder-autojoin-3.1.9.dev8/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-autojoin-3.1.9.dev8/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3790 2022-02-23 17:41:16.000000 girder-autojoin-3.1.9.dev8/plugin_tests/autojoinSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2418 2022-02-23 17:41:16.000000 girder-autojoin-3.1.9.dev8/plugin_tests/autojoin_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2022-02-23 17:41:16.000000 girder-autojoin-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1811 2022-02-23 17:41:16.000000 girder-autojoin-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      756 2022-02-23 17:41:33.000000 girder-autojoin-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:41:33.000000 girder-autojoin-3.1.9.dev8/setup.cfg
```

### Comparing `girder-autojoin-3.1.9.dev6/girder_autojoin/web_client/templates/configView.pug` & `girder-autojoin-3.1.9.dev8/girder_autojoin/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.1.9.dev6/girder_autojoin/web_client/views/ConfigView.js` & `girder-autojoin-3.1.9.dev8/girder_autojoin/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.1.9.dev6/girder_autojoin/web_client/package.json` & `girder-autojoin-3.1.9.dev8/girder_autojoin/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.1.9.dev6/girder_autojoin/__init__.py` & `girder-autojoin-3.1.9.dev8/girder_autojoin/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.1.9.dev6/girder_autojoin/settings.py` & `girder-autojoin-3.1.9.dev8/girder_autojoin/settings.py`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.1.9.dev6/girder_autojoin.egg-info/PKG-INFO` & `girder-autojoin-3.1.9.dev8/girder_autojoin.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-autojoin
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Automatically assign new users to groups based on their email domain
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#auto-join
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `girder-autojoin-3.1.9.dev6/girder_autojoin.egg-info/SOURCES.txt` & `girder-autojoin-3.1.9.dev8/girder_autojoin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.1.9.dev6/plugin_tests/autojoinSpec.js` & `girder-autojoin-3.1.9.dev8/plugin_tests/autojoinSpec.js`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.1.9.dev6/plugin_tests/autojoin_test.py` & `girder-autojoin-3.1.9.dev8/plugin_tests/autojoin_test.py`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.1.9.dev6/setup.py` & `girder-autojoin-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.1.9.dev6/PKG-INFO` & `girder-autojoin-3.1.9.dev8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-autojoin
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Automatically assign new users to groups based on their email domain
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#auto-join
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

