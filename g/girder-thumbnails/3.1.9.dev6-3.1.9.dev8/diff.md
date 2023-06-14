# Comparing `tmp/girder-thumbnails-3.1.9.dev6.tar.gz` & `tmp/girder-thumbnails-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-thumbnails-3.1.9.dev6.tar", last modified: Wed Feb 23 16:10:06 2022, max compression
+gzip compressed data, was "dist/girder-thumbnails-3.1.9.dev8.tar", last modified: Wed Feb 23 17:42:07 2022, max compression
```

## Comparing `girder-thumbnails-3.1.9.dev6.tar` & `girder-thumbnails-3.1.9.dev8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      150 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/models/ThumbnailModel.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      496 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/stylesheets/createThumbnailView.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      473 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/stylesheets/flowView.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1510 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/templates/createThumbnailViewTargetDescription.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)       77 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/templates/fileListWidgetCreateButton.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      314 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/templates/flowView.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/templates/itemView.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3910 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/views/CreateThumbnailView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1306 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/views/FileListWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2021 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/views/FlowView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1171 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/views/ItemView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      537 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3104 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2370 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      664 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6350 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails/worker.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      667 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1324 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       65 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       18 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/girder_thumbnails.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/plugin_tests/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/plugin_tests/data/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35946 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/plugin_tests/data/sample_dicom.dcm
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13024 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/plugin_tests/thumbnail_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2205 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/plugin_tests/thumbnailsSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1886 2022-02-23 16:09:15.000000 girder-thumbnails-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      667 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:10:06.000000 girder-thumbnails-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:07.000000 girder-thumbnails-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:07.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:07.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:07.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      150 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/models/ThumbnailModel.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:07.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      496 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/stylesheets/createThumbnailView.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      473 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/stylesheets/flowView.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:07.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1510 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/templates/createThumbnailViewTargetDescription.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       77 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/templates/fileListWidgetCreateButton.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      314 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/templates/flowView.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/templates/itemView.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:07.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3910 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/views/CreateThumbnailView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1306 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/views/FileListWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2021 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/views/FlowView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1171 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/views/ItemView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      537 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3104 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2370 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      664 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6350 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails/worker.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:07.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      667 2022-02-23 17:42:06.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1324 2022-02-23 17:42:06.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:42:06.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       65 2022-02-23 17:42:06.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:42:06.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 17:42:06.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       18 2022-02-23 17:42:06.000000 girder-thumbnails-3.1.9.dev8/girder_thumbnails.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:07.000000 girder-thumbnails-3.1.9.dev8/plugin_tests/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:07.000000 girder-thumbnails-3.1.9.dev8/plugin_tests/data/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35946 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/plugin_tests/data/sample_dicom.dcm
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13024 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/plugin_tests/thumbnail_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2205 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/plugin_tests/thumbnailsSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1886 2022-02-23 17:41:16.000000 girder-thumbnails-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      667 2022-02-23 17:42:07.000000 girder-thumbnails-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:42:07.000000 girder-thumbnails-3.1.9.dev8/setup.cfg
```

### Comparing `girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug` & `girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/views/CreateThumbnailView.js` & `girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/views/CreateThumbnailView.js`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/views/FileListWidget.js` & `girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/views/FileListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/views/FlowView.js` & `girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/views/FlowView.js`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/views/ItemView.js` & `girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/views/ItemView.js`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.1.9.dev6/girder_thumbnails/web_client/package.json` & `girder-thumbnails-3.1.9.dev8/girder_thumbnails/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.1.9.dev6/girder_thumbnails/__init__.py` & `girder-thumbnails-3.1.9.dev8/girder_thumbnails/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.1.9.dev6/girder_thumbnails/rest.py` & `girder-thumbnails-3.1.9.dev8/girder_thumbnails/rest.py`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.1.9.dev6/girder_thumbnails/utils.py` & `girder-thumbnails-3.1.9.dev8/girder_thumbnails/utils.py`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.1.9.dev6/girder_thumbnails/worker.py` & `girder-thumbnails-3.1.9.dev8/girder_thumbnails/worker.py`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.1.9.dev6/girder_thumbnails.egg-info/PKG-INFO` & `girder-thumbnails-3.1.9.dev8/girder_thumbnails.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-thumbnails
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Generate thumbnails from files.
 Home-page: UNKNOWN
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `girder-thumbnails-3.1.9.dev6/girder_thumbnails.egg-info/SOURCES.txt` & `girder-thumbnails-3.1.9.dev8/girder_thumbnails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.1.9.dev6/plugin_tests/data/sample_dicom.dcm` & `girder-thumbnails-3.1.9.dev8/plugin_tests/data/sample_dicom.dcm`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.1.9.dev6/plugin_tests/thumbnail_test.py` & `girder-thumbnails-3.1.9.dev8/plugin_tests/thumbnail_test.py`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.1.9.dev6/plugin_tests/thumbnailsSpec.js` & `girder-thumbnails-3.1.9.dev8/plugin_tests/thumbnailsSpec.js`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.1.9.dev6/setup.py` & `girder-thumbnails-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.1.9.dev6/PKG-INFO` & `girder-thumbnails-3.1.9.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-thumbnails
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Generate thumbnails from files.
 Home-page: UNKNOWN
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

