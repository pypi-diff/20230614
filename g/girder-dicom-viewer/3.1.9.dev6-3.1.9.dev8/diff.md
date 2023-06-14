# Comparing `tmp/girder-dicom-viewer-3.1.9.dev6.tar.gz` & `tmp/girder-dicom-viewer-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-dicom-viewer-3.1.9.dev6.tar", last modified: Wed Feb 23 16:09:35 2022, max compression
+gzip compressed data, was "dist/girder-dicom-viewer-3.1.9.dev8.tar", last modified: Wed Feb 23 17:41:36 2022, max compression
```

## Comparing `girder-dicom-viewer-3.1.9.dev6.tar` & `girder-dicom-viewer-3.1.9.dev8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      487 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/stylesheets/dicomItem.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/stylesheets/dicomSliceMetadata.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1286 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/templates/dicomItem.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      165 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/templates/dicomSliceMetadata.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/templates/parseDicomItem.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13597 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/views/DicomView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2264 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      719 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      686 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/webpack.helper.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9458 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1023 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/event_helper.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      727 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       70 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      102 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/plugin_tests/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/plugin_tests/data/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/plugin_tests/data/000000.dcm.sha512
--rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/plugin_tests/data/000001.dcm.sha512
--rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/plugin_tests/data/000002.dcm.sha512
--rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/plugin_tests/data/000003.dcm.sha512
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11231 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/plugin_tests/dicom_viewer_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      279 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1910 2022-02-23 16:09:15.000000 girder-dicom-viewer-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      727 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:09:35.000000 girder-dicom-viewer-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:36.000000 girder-dicom-viewer-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:36.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:36.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:36.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      487 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/stylesheets/dicomItem.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/stylesheets/dicomSliceMetadata.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:36.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1286 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/templates/dicomItem.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      165 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/templates/dicomSliceMetadata.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/templates/parseDicomItem.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:36.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13597 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/views/DicomView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2264 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      719 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      686 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/webpack.helper.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9458 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1023 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/event_helper.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:36.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      727 2022-02-23 17:41:35.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2022-02-23 17:41:36.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:35.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       70 2022-02-23 17:41:35.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:35.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      102 2022-02-23 17:41:35.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2022-02-23 17:41:35.000000 girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:36.000000 girder-dicom-viewer-3.1.9.dev8/plugin_tests/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:36.000000 girder-dicom-viewer-3.1.9.dev8/plugin_tests/data/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/plugin_tests/data/000000.dcm.sha512
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/plugin_tests/data/000001.dcm.sha512
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/plugin_tests/data/000002.dcm.sha512
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/plugin_tests/data/000003.dcm.sha512
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11231 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/plugin_tests/dicom_viewer_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      279 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1910 2022-02-23 17:41:16.000000 girder-dicom-viewer-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      727 2022-02-23 17:41:36.000000 girder-dicom-viewer-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:41:36.000000 girder-dicom-viewer-3.1.9.dev8/setup.cfg
```

### Comparing `girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/templates/dicomItem.pug` & `girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/templates/dicomItem.pug`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/views/DicomView.js` & `girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/views/DicomView.js`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/main.js` & `girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/package.json` & `girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/web_client/webpack.helper.js` & `girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/web_client/webpack.helper.js`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/__init__.py` & `girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer/event_helper.py` & `girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer/event_helper.py`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer.egg-info/PKG-INFO` & `girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-dicom-viewer
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: View DICOM images in the browser
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#dicom-viewer
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `girder-dicom-viewer-3.1.9.dev6/girder_dicom_viewer.egg-info/SOURCES.txt` & `girder-dicom-viewer-3.1.9.dev8/girder_dicom_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.1.9.dev6/plugin_tests/dicom_viewer_test.py` & `girder-dicom-viewer-3.1.9.dev8/plugin_tests/dicom_viewer_test.py`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.1.9.dev6/setup.py` & `girder-dicom-viewer-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.1.9.dev6/PKG-INFO` & `girder-dicom-viewer-3.1.9.dev8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-dicom-viewer
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: View DICOM images in the browser
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#dicom-viewer
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

