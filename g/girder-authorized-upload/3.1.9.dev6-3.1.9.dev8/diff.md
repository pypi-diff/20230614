# Comparing `tmp/girder-authorized-upload-3.1.9.dev6.tar.gz` & `tmp/girder-authorized-upload-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-authorized-upload-3.1.9.dev6.tar", last modified: Wed Feb 23 16:09:30 2022, max compression
+gzip compressed data, was "dist/girder-authorized-upload-3.1.9.dev8.tar", last modified: Wed Feb 23 17:41:31 2022, max compression
```

## Comparing `girder-authorized-upload-3.1.9.dev6.tar` & `girder-authorized-upload-3.1.9.dev8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/mail_templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      281 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/mail_templates/authorized_upload.uploadFinished.mako
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       35 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/stylesheets/authorizeUpload.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)      966 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      827 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/templates/authorizeUpload.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      766 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/templates/authorizedUpload.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      137 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/templates/folderActions.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1064 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/views/AuthorizeUploadView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1544 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/views/AuthorizedUploadView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      707 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      664 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      905 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4629 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1736 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/rest.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      797 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1240 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       85 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       25 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/girder_authorized_upload.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3124 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/plugin_tests/authorizedUploadSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4624 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/plugin_tests/upload_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       62 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1885 2022-02-23 16:09:15.000000 girder-authorized-upload-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      797 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:09:30.000000 girder-authorized-upload-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/mail_templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      281 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/mail_templates/authorized_upload.uploadFinished.mako
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       35 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/stylesheets/authorizeUpload.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      966 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      827 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/templates/authorizeUpload.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      766 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/templates/authorizedUpload.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      137 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/templates/folderActions.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1064 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/views/AuthorizeUploadView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1544 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/views/AuthorizedUploadView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      707 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      664 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      905 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4629 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1736 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/rest.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      797 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1240 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       85 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       25 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/girder_authorized_upload.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3124 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/plugin_tests/authorizedUploadSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4624 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/plugin_tests/upload_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       62 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1885 2022-02-23 17:41:16.000000 girder-authorized-upload-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      797 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:41:31.000000 girder-authorized-upload-3.1.9.dev8/setup.cfg
```

### Comparing `girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl` & `girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/templates/authorizeUpload.pug` & `girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/templates/authorizeUpload.pug`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/templates/authorizedUpload.pug` & `girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/templates/authorizedUpload.pug`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/views/AuthorizeUploadView.js` & `girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/views/AuthorizeUploadView.js`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/views/AuthorizedUploadView.js` & `girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/views/AuthorizedUploadView.js`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/main.js` & `girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/package.json` & `girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/web_client/routes.js` & `girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/web_client/routes.js`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/__init__.py` & `girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.1.9.dev6/girder_authorized_upload/rest.py` & `girder-authorized-upload-3.1.9.dev8/girder_authorized_upload/rest.py`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.1.9.dev6/girder_authorized_upload.egg-info/PKG-INFO` & `girder-authorized-upload-3.1.9.dev8/girder_authorized_upload.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-authorized-upload
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Allows registered users to authorize file uploads on their behalf via a secure one-use URL.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#authorized-uploads
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `girder-authorized-upload-3.1.9.dev6/girder_authorized_upload.egg-info/SOURCES.txt` & `girder-authorized-upload-3.1.9.dev8/girder_authorized_upload.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.1.9.dev6/plugin_tests/authorizedUploadSpec.js` & `girder-authorized-upload-3.1.9.dev8/plugin_tests/authorizedUploadSpec.js`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.1.9.dev6/plugin_tests/upload_test.py` & `girder-authorized-upload-3.1.9.dev8/plugin_tests/upload_test.py`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.1.9.dev6/setup.py` & `girder-authorized-upload-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.1.9.dev6/PKG-INFO` & `girder-authorized-upload-3.1.9.dev8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-authorized-upload
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Allows registered users to authorize file uploads on their behalf via a secure one-use URL.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#authorized-uploads
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

