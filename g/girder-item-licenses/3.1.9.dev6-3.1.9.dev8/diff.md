# Comparing `tmp/girder-item-licenses-3.1.9.dev6.tar.gz` & `tmp/girder-item-licenses-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-item-licenses-3.1.9.dev6.tar", last modified: Wed Feb 23 16:09:50 2022, max compression
+gzip compressed data, was "dist/girder-item-licenses-3.1.9.dev8.tar", last modified: Wed Feb 23 17:41:50 2022, max compression
```

## Comparing `girder-item-licenses-3.1.9.dev6.tar` & `girder-item-licenses-3.1.9.dev8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:50.000000 girder-item-licenses-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:50.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:50.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:50.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:50.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      504 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      175 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/templates/itemLicenseWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      406 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/templates/selectLicenseWidget.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:50.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2499 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1480 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/views/EditItemWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/views/HierarchyWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      471 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/views/ItemLicenseWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1047 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/views/ItemView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      610 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/views/SelectLicenseWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1576 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/views/UploadWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      174 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      478 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      441 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2855 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      677 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4514 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:50.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      668 2022-02-23 16:09:49.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1281 2022-02-23 16:09:49.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:49.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       73 2022-02-23 16:09:49.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:49.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 16:09:49.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2022-02-23 16:09:49.000000 girder-item-licenses-3.1.9.dev6/girder_item_licenses.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:50.000000 girder-item-licenses-3.1.9.dev6/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15913 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/plugin_tests/itemLicensesSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12372 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/plugin_tests/item_licenses_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       58 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1718 2022-02-23 16:09:15.000000 girder-item-licenses-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      668 2022-02-23 16:09:50.000000 girder-item-licenses-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:09:50.000000 girder-item-licenses-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:50.000000 girder-item-licenses-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:50.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:50.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:50.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:50.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      504 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/templates/configView.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      175 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/templates/itemLicenseWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      406 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/templates/selectLicenseWidget.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:50.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2499 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1480 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/views/EditItemWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/views/HierarchyWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      471 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/views/ItemLicenseWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1047 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/views/ItemView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      610 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/views/SelectLicenseWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1576 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/views/UploadWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      174 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      478 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      441 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2855 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      677 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4514 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:50.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      668 2022-02-23 17:41:50.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1281 2022-02-23 17:41:50.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:50.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       73 2022-02-23 17:41:50.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:50.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 17:41:50.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2022-02-23 17:41:50.000000 girder-item-licenses-3.1.9.dev8/girder_item_licenses.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:50.000000 girder-item-licenses-3.1.9.dev8/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15913 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/plugin_tests/itemLicensesSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12372 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/plugin_tests/item_licenses_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       58 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1718 2022-02-23 17:41:16.000000 girder-item-licenses-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      668 2022-02-23 17:41:50.000000 girder-item-licenses-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:41:50.000000 girder-item-licenses-3.1.9.dev8/setup.cfg
```

### Comparing `girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/views/ConfigView.js` & `girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/views/EditItemWidget.js` & `girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/views/EditItemWidget.js`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/views/HierarchyWidget.js` & `girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/views/HierarchyWidget.js`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/views/ItemView.js` & `girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/views/ItemView.js`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/views/SelectLicenseWidget.js` & `girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/views/SelectLicenseWidget.js`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.1.9.dev6/girder_item_licenses/web_client/views/UploadWidget.js` & `girder-item-licenses-3.1.9.dev8/girder_item_licenses/web_client/views/UploadWidget.js`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.1.9.dev6/girder_item_licenses/__init__.py` & `girder-item-licenses-3.1.9.dev8/girder_item_licenses/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.1.9.dev6/girder_item_licenses/rest.py` & `girder-item-licenses-3.1.9.dev8/girder_item_licenses/rest.py`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.1.9.dev6/girder_item_licenses/settings.py` & `girder-item-licenses-3.1.9.dev8/girder_item_licenses/settings.py`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.1.9.dev6/girder_item_licenses.egg-info/PKG-INFO` & `girder-item-licenses-3.1.9.dev8/girder_item_licenses.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-item-licenses
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Add a license field to items.
 Home-page: UNKNOWN
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `girder-item-licenses-3.1.9.dev6/girder_item_licenses.egg-info/SOURCES.txt` & `girder-item-licenses-3.1.9.dev8/girder_item_licenses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.1.9.dev6/plugin_tests/itemLicensesSpec.js` & `girder-item-licenses-3.1.9.dev8/plugin_tests/itemLicensesSpec.js`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.1.9.dev6/plugin_tests/item_licenses_test.py` & `girder-item-licenses-3.1.9.dev8/plugin_tests/item_licenses_test.py`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.1.9.dev6/setup.py` & `girder-item-licenses-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.1.9.dev6/PKG-INFO` & `girder-item-licenses-3.1.9.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-item-licenses
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Add a license field to items.
 Home-page: UNKNOWN
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

