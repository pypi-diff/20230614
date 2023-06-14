# Comparing `tmp/girder-google-analytics-3.1.9.dev6.tar.gz` & `tmp/girder-google-analytics-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-google-analytics-3.1.9.dev6.tar", last modified: Wed Feb 23 16:09:40 2022, max compression
+gzip compressed data, was "dist/girder-google-analytics-3.1.9.dev8.tar", last modified: Wed Feb 23 17:41:41 2022, max compression
```

## Comparing `girder-google-analytics-3.1.9.dev6.tar` & `girder-google-analytics-3.1.9.dev8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics/web_client/lib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2295 2022-02-23 16:09:15.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics/web_client/lib/backbone.analytics.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      222 2022-02-23 16:09:15.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      526 2022-02-23 16:09:15.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2186 2022-02-23 16:09:15.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1440 2022-02-23 16:09:15.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      597 2022-02-23 16:09:15.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      453 2022-02-23 16:09:15.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      297 2022-02-23 16:09:15.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      679 2022-02-23 16:09:15.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      473 2022-02-23 16:09:15.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      757 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      893 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/girder_google_analytics.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-google-analytics-3.1.9.dev6/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      886 2022-02-23 16:09:15.000000 girder-google-analytics-3.1.9.dev6/plugin_tests/google_analytics_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-02-23 16:09:15.000000 girder-google-analytics-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1835 2022-02-23 16:09:15.000000 girder-google-analytics-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      757 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:09:40.000000 girder-google-analytics-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:41.000000 girder-google-analytics-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:41.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:41.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:41.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics/web_client/lib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2295 2022-02-23 17:41:16.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics/web_client/lib/backbone.analytics.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:41.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      222 2022-02-23 17:41:16.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:41.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      526 2022-02-23 17:41:16.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:41.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2186 2022-02-23 17:41:16.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1440 2022-02-23 17:41:16.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      597 2022-02-23 17:41:16.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      453 2022-02-23 17:41:16.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      297 2022-02-23 17:41:16.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      679 2022-02-23 17:41:16.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics/rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      473 2022-02-23 17:41:16.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:41.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      757 2022-02-23 17:41:40.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      893 2022-02-23 17:41:40.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:40.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2022-02-23 17:41:40.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:40.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 17:41:40.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2022-02-23 17:41:40.000000 girder-google-analytics-3.1.9.dev8/girder_google_analytics.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:41.000000 girder-google-analytics-3.1.9.dev8/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-google-analytics-3.1.9.dev8/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      886 2022-02-23 17:41:16.000000 girder-google-analytics-3.1.9.dev8/plugin_tests/google_analytics_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-02-23 17:41:16.000000 girder-google-analytics-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1835 2022-02-23 17:41:16.000000 girder-google-analytics-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      757 2022-02-23 17:41:41.000000 girder-google-analytics-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:41:41.000000 girder-google-analytics-3.1.9.dev8/setup.cfg
```

### Comparing `girder-google-analytics-3.1.9.dev6/girder_google_analytics/web_client/lib/backbone.analytics.js` & `girder-google-analytics-3.1.9.dev8/girder_google_analytics/web_client/lib/backbone.analytics.js`

 * *Files identical despite different names*

### Comparing `girder-google-analytics-3.1.9.dev6/girder_google_analytics/web_client/templates/configView.pug` & `girder-google-analytics-3.1.9.dev8/girder_google_analytics/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-google-analytics-3.1.9.dev6/girder_google_analytics/web_client/views/ConfigView.js` & `girder-google-analytics-3.1.9.dev8/girder_google_analytics/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-google-analytics-3.1.9.dev6/girder_google_analytics/web_client/main.js` & `girder-google-analytics-3.1.9.dev8/girder_google_analytics/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-google-analytics-3.1.9.dev6/girder_google_analytics/web_client/package.json` & `girder-google-analytics-3.1.9.dev8/girder_google_analytics/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-google-analytics-3.1.9.dev6/girder_google_analytics/rest.py` & `girder-google-analytics-3.1.9.dev8/girder_google_analytics/rest.py`

 * *Files identical despite different names*

### Comparing `girder-google-analytics-3.1.9.dev6/girder_google_analytics.egg-info/PKG-INFO` & `girder-google-analytics-3.1.9.dev8/girder_google_analytics.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-google-analytics
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Allow the tracking of page views via Google Analytics.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#google-analytics
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `girder-google-analytics-3.1.9.dev6/girder_google_analytics.egg-info/SOURCES.txt` & `girder-google-analytics-3.1.9.dev8/girder_google_analytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-google-analytics-3.1.9.dev6/plugin_tests/google_analytics_test.py` & `girder-google-analytics-3.1.9.dev8/plugin_tests/google_analytics_test.py`

 * *Files identical despite different names*

### Comparing `girder-google-analytics-3.1.9.dev6/setup.py` & `girder-google-analytics-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-google-analytics-3.1.9.dev6/PKG-INFO` & `girder-google-analytics-3.1.9.dev8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-google-analytics
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Allow the tracking of page views via Google Analytics.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#google-analytics
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

