# Comparing `tmp/girder-sentry-3.1.9.dev6.tar.gz` & `tmp/girder-sentry-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-sentry-3.1.9.dev6.tar", last modified: Wed Feb 23 16:10:02 2022, max compression
+gzip compressed data, was "dist/girder-sentry-3.1.9.dev8.tar", last modified: Wed Feb 23 17:42:02 2022, max compression
```

## Comparing `girder-sentry-3.1.9.dev6.tar` & `girder-sentry-3.1.9.dev8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:02.000000 girder-sentry-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:02.000000 girder-sentry-3.1.9.dev6/girder_sentry/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:02.000000 girder-sentry-3.1.9.dev6/girder_sentry/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:02.000000 girder-sentry-3.1.9.dev6/girder_sentry/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      202 2022-02-23 16:09:15.000000 girder-sentry-3.1.9.dev6/girder_sentry/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:02.000000 girder-sentry-3.1.9.dev6/girder_sentry/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      809 2022-02-23 16:09:15.000000 girder-sentry-3.1.9.dev6/girder_sentry/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:02.000000 girder-sentry-3.1.9.dev6/girder_sentry/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2728 2022-02-23 16:09:15.000000 girder-sentry-3.1.9.dev6/girder_sentry/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      403 2022-02-23 16:09:15.000000 girder-sentry-3.1.9.dev6/girder_sentry/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      592 2022-02-23 16:09:15.000000 girder-sentry-3.1.9.dev6/girder_sentry/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      414 2022-02-23 16:09:15.000000 girder-sentry-3.1.9.dev6/girder_sentry/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      428 2022-02-23 16:09:15.000000 girder-sentry-3.1.9.dev6/girder_sentry/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      625 2022-02-23 16:09:15.000000 girder-sentry-3.1.9.dev6/girder_sentry/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      579 2022-02-23 16:09:15.000000 girder-sentry-3.1.9.dev6/girder_sentry/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:02.000000 girder-sentry-3.1.9.dev6/girder_sentry.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      692 2022-02-23 16:10:01.000000 girder-sentry-3.1.9.dev6/girder_sentry.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      609 2022-02-23 16:10:02.000000 girder-sentry-3.1.9.dev6/girder_sentry.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:10:01.000000 girder-sentry-3.1.9.dev6/girder_sentry.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2022-02-23 16:10:01.000000 girder-sentry-3.1.9.dev6/girder_sentry.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:10:01.000000 girder-sentry-3.1.9.dev6/girder_sentry.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2022-02-23 16:10:01.000000 girder-sentry-3.1.9.dev6/girder_sentry.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2022-02-23 16:10:01.000000 girder-sentry-3.1.9.dev6/girder_sentry.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       51 2022-02-23 16:09:15.000000 girder-sentry-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1758 2022-02-23 16:09:15.000000 girder-sentry-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      692 2022-02-23 16:10:02.000000 girder-sentry-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:10:02.000000 girder-sentry-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:02.000000 girder-sentry-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:02.000000 girder-sentry-3.1.9.dev8/girder_sentry/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:02.000000 girder-sentry-3.1.9.dev8/girder_sentry/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:02.000000 girder-sentry-3.1.9.dev8/girder_sentry/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      202 2022-02-23 17:41:16.000000 girder-sentry-3.1.9.dev8/girder_sentry/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:02.000000 girder-sentry-3.1.9.dev8/girder_sentry/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      809 2022-02-23 17:41:16.000000 girder-sentry-3.1.9.dev8/girder_sentry/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:02.000000 girder-sentry-3.1.9.dev8/girder_sentry/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2728 2022-02-23 17:41:16.000000 girder-sentry-3.1.9.dev8/girder_sentry/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      403 2022-02-23 17:41:16.000000 girder-sentry-3.1.9.dev8/girder_sentry/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      592 2022-02-23 17:41:16.000000 girder-sentry-3.1.9.dev8/girder_sentry/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      414 2022-02-23 17:41:16.000000 girder-sentry-3.1.9.dev8/girder_sentry/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      428 2022-02-23 17:41:16.000000 girder-sentry-3.1.9.dev8/girder_sentry/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      625 2022-02-23 17:41:16.000000 girder-sentry-3.1.9.dev8/girder_sentry/rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      579 2022-02-23 17:41:16.000000 girder-sentry-3.1.9.dev8/girder_sentry/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:02.000000 girder-sentry-3.1.9.dev8/girder_sentry.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      692 2022-02-23 17:42:02.000000 girder-sentry-3.1.9.dev8/girder_sentry.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      609 2022-02-23 17:42:02.000000 girder-sentry-3.1.9.dev8/girder_sentry.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:42:02.000000 girder-sentry-3.1.9.dev8/girder_sentry.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2022-02-23 17:42:02.000000 girder-sentry-3.1.9.dev8/girder_sentry.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:42:02.000000 girder-sentry-3.1.9.dev8/girder_sentry.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2022-02-23 17:42:02.000000 girder-sentry-3.1.9.dev8/girder_sentry.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2022-02-23 17:42:02.000000 girder-sentry-3.1.9.dev8/girder_sentry.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       51 2022-02-23 17:41:16.000000 girder-sentry-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1758 2022-02-23 17:41:16.000000 girder-sentry-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      692 2022-02-23 17:42:02.000000 girder-sentry-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:42:02.000000 girder-sentry-3.1.9.dev8/setup.cfg
```

### Comparing `girder-sentry-3.1.9.dev6/girder_sentry/web_client/templates/configView.pug` & `girder-sentry-3.1.9.dev8/girder_sentry/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-sentry-3.1.9.dev6/girder_sentry/web_client/views/ConfigView.js` & `girder-sentry-3.1.9.dev8/girder_sentry/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-sentry-3.1.9.dev6/girder_sentry/web_client/package.json` & `girder-sentry-3.1.9.dev8/girder_sentry/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-sentry-3.1.9.dev6/girder_sentry/rest.py` & `girder-sentry-3.1.9.dev8/girder_sentry/rest.py`

 * *Files identical despite different names*

### Comparing `girder-sentry-3.1.9.dev6/girder_sentry/settings.py` & `girder-sentry-3.1.9.dev8/girder_sentry/settings.py`

 * *Files identical despite different names*

### Comparing `girder-sentry-3.1.9.dev6/girder_sentry.egg-info/PKG-INFO` & `girder-sentry-3.1.9.dev8/girder_sentry.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-sentry
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Allow the automatic tracking of issues using Sentry.
 Home-page: UNKNOWN
 Maintainer: Kitware, Inc.
 Maintainer-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `girder-sentry-3.1.9.dev6/girder_sentry.egg-info/SOURCES.txt` & `girder-sentry-3.1.9.dev8/girder_sentry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-sentry-3.1.9.dev6/setup.py` & `girder-sentry-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-sentry-3.1.9.dev6/PKG-INFO` & `girder-sentry-3.1.9.dev8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-sentry
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Allow the automatic tracking of issues using Sentry.
 Home-page: UNKNOWN
 Maintainer: Kitware, Inc.
 Maintainer-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

