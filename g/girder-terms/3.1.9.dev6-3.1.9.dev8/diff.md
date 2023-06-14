# Comparing `tmp/girder-terms-3.1.9.dev6.tar.gz` & `tmp/girder-terms-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-terms-3.1.9.dev6.tar", last modified: Wed Feb 23 16:10:04 2022, max compression
+gzip compressed data, was "dist/girder-terms-3.1.9.dev8.tar", last modified: Wed Feb 23 17:42:04 2022, max compression
```

## Comparing `girder-terms-3.1.9.dev6.tar` & `girder-terms-3.1.9.dev8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/girder_terms/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3270 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/models/CollectionModel.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      118 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/stylesheets/collectionInfoWidget.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)       67 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/stylesheets/editCollectionTermsWidget.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      103 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/stylesheets/termsAcceptance.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      106 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/templates/collectionInfoWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      291 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/templates/editCollectionTermsWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      266 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/templates/termsAcceptance.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      717 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/views/CollectionInfoWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2413 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/views/EditCollectionWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1495 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/views/TermsAcceptanceView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      132 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      655 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3087 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/girder_terms/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3408 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/girder_terms/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/girder_terms.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      770 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/girder_terms.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1054 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/girder_terms.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/girder_terms.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       50 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/girder_terms.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/girder_terms.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/girder_terms.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       13 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/girder_terms.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14763 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/plugin_tests/termsSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6115 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/plugin_tests/terms_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       50 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1823 2022-02-23 16:09:15.000000 girder-terms-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      770 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:10:04.000000 girder-terms-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/girder_terms/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3270 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/models/CollectionModel.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      118 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/stylesheets/collectionInfoWidget.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       67 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/stylesheets/editCollectionTermsWidget.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      103 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/stylesheets/termsAcceptance.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      106 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/templates/collectionInfoWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      291 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/templates/editCollectionTermsWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      266 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/templates/termsAcceptance.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      717 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/views/CollectionInfoWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2413 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/views/EditCollectionWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1495 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/views/TermsAcceptanceView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      132 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      655 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3087 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/girder_terms/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3408 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/girder_terms/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/girder_terms.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      770 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/girder_terms.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1054 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/girder_terms.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/girder_terms.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       50 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/girder_terms.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/girder_terms.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/girder_terms.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       13 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/girder_terms.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14763 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/plugin_tests/termsSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6115 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/plugin_tests/terms_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       50 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1823 2022-02-23 17:41:16.000000 girder-terms-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      770 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:42:04.000000 girder-terms-3.1.9.dev8/setup.cfg
```

### Comparing `girder-terms-3.1.9.dev6/girder_terms/web_client/models/CollectionModel.js` & `girder-terms-3.1.9.dev8/girder_terms/web_client/models/CollectionModel.js`

 * *Files identical despite different names*

### Comparing `girder-terms-3.1.9.dev6/girder_terms/web_client/views/CollectionInfoWidget.js` & `girder-terms-3.1.9.dev8/girder_terms/web_client/views/CollectionInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-terms-3.1.9.dev6/girder_terms/web_client/views/EditCollectionWidget.js` & `girder-terms-3.1.9.dev8/girder_terms/web_client/views/EditCollectionWidget.js`

 * *Files identical despite different names*

### Comparing `girder-terms-3.1.9.dev6/girder_terms/web_client/views/TermsAcceptanceView.js` & `girder-terms-3.1.9.dev8/girder_terms/web_client/views/TermsAcceptanceView.js`

 * *Files identical despite different names*

### Comparing `girder-terms-3.1.9.dev6/girder_terms/web_client/package.json` & `girder-terms-3.1.9.dev8/girder_terms/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-terms-3.1.9.dev6/girder_terms/web_client/routes.js` & `girder-terms-3.1.9.dev8/girder_terms/web_client/routes.js`

 * *Files identical despite different names*

### Comparing `girder-terms-3.1.9.dev6/girder_terms/__init__.py` & `girder-terms-3.1.9.dev8/girder_terms/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-terms-3.1.9.dev6/girder_terms.egg-info/PKG-INFO` & `girder-terms-3.1.9.dev8/girder_terms.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-terms
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Allows Girder collections to require users to accept terms of use before browsing.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#terms-of-use
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `girder-terms-3.1.9.dev6/girder_terms.egg-info/SOURCES.txt` & `girder-terms-3.1.9.dev8/girder_terms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-terms-3.1.9.dev6/plugin_tests/termsSpec.js` & `girder-terms-3.1.9.dev8/plugin_tests/termsSpec.js`

 * *Files identical despite different names*

### Comparing `girder-terms-3.1.9.dev6/plugin_tests/terms_test.py` & `girder-terms-3.1.9.dev8/plugin_tests/terms_test.py`

 * *Files identical despite different names*

### Comparing `girder-terms-3.1.9.dev6/setup.py` & `girder-terms-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-terms-3.1.9.dev6/PKG-INFO` & `girder-terms-3.1.9.dev8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-terms
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Allows Girder collections to require users to accept terms of use before browsing.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#terms-of-use
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

