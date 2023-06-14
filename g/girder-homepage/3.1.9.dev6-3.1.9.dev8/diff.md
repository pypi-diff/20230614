# Comparing `tmp/girder-homepage-3.1.9.dev6.tar.gz` & `tmp/girder-homepage-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-homepage-3.1.9.dev6.tar", last modified: Wed Feb 23 16:09:47 2022, max compression
+gzip compressed data, was "dist/girder-homepage-3.1.9.dev8.tar", last modified: Wed Feb 23 17:41:48 2022, max compression
```

## Comparing `girder-homepage-3.1.9.dev6.tar` & `girder-homepage-3.1.9.dev8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:47.000000 girder-homepage-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:47.000000 girder-homepage-3.1.9.dev6/girder_homepage/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:47.000000 girder-homepage-3.1.9.dev6/girder_homepage/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:47.000000 girder-homepage-3.1.9.dev6/girder_homepage/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      912 2022-02-23 16:09:15.000000 girder-homepage-3.1.9.dev6/girder_homepage/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:47.000000 girder-homepage-3.1.9.dev6/girder_homepage/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1472 2022-02-23 16:09:15.000000 girder-homepage-3.1.9.dev6/girder_homepage/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:47.000000 girder-homepage-3.1.9.dev6/girder_homepage/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6270 2022-02-23 16:09:15.000000 girder-homepage-3.1.9.dev6/girder_homepage/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1267 2022-02-23 16:09:15.000000 girder-homepage-3.1.9.dev6/girder_homepage/web_client/views/FrontPageView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2022-02-23 16:09:15.000000 girder-homepage-3.1.9.dev6/girder_homepage/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      557 2022-02-23 16:09:15.000000 girder-homepage-3.1.9.dev6/girder_homepage/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      422 2022-02-23 16:09:15.000000 girder-homepage-3.1.9.dev6/girder_homepage/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      267 2022-02-23 16:09:15.000000 girder-homepage-3.1.9.dev6/girder_homepage/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2022-02-23 16:09:15.000000 girder-homepage-3.1.9.dev6/girder_homepage/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2432 2022-02-23 16:09:15.000000 girder-homepage-3.1.9.dev6/girder_homepage/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1695 2022-02-23 16:09:15.000000 girder-homepage-3.1.9.dev6/girder_homepage/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:47.000000 girder-homepage-3.1.9.dev6/girder_homepage.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      738 2022-02-23 16:09:47.000000 girder-homepage-3.1.9.dev6/girder_homepage.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      804 2022-02-23 16:09:47.000000 girder-homepage-3.1.9.dev6/girder_homepage.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:47.000000 girder-homepage-3.1.9.dev6/girder_homepage.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       59 2022-02-23 16:09:47.000000 girder-homepage-3.1.9.dev6/girder_homepage.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:47.000000 girder-homepage-3.1.9.dev6/girder_homepage.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 16:09:47.000000 girder-homepage-3.1.9.dev6/girder_homepage.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2022-02-23 16:09:47.000000 girder-homepage-3.1.9.dev6/girder_homepage.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:47.000000 girder-homepage-3.1.9.dev6/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-homepage-3.1.9.dev6/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6120 2022-02-23 16:09:15.000000 girder-homepage-3.1.9.dev6/plugin_tests/homepageSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      724 2022-02-23 16:09:15.000000 girder-homepage-3.1.9.dev6/plugin_tests/homepage_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2022-02-23 16:09:15.000000 girder-homepage-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1793 2022-02-23 16:09:15.000000 girder-homepage-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      738 2022-02-23 16:09:47.000000 girder-homepage-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:09:47.000000 girder-homepage-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:48.000000 girder-homepage-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:48.000000 girder-homepage-3.1.9.dev8/girder_homepage/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:48.000000 girder-homepage-3.1.9.dev8/girder_homepage/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:48.000000 girder-homepage-3.1.9.dev8/girder_homepage/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      912 2022-02-23 17:41:16.000000 girder-homepage-3.1.9.dev8/girder_homepage/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:48.000000 girder-homepage-3.1.9.dev8/girder_homepage/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1472 2022-02-23 17:41:16.000000 girder-homepage-3.1.9.dev8/girder_homepage/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:48.000000 girder-homepage-3.1.9.dev8/girder_homepage/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6270 2022-02-23 17:41:16.000000 girder-homepage-3.1.9.dev8/girder_homepage/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1267 2022-02-23 17:41:16.000000 girder-homepage-3.1.9.dev8/girder_homepage/web_client/views/FrontPageView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2022-02-23 17:41:16.000000 girder-homepage-3.1.9.dev8/girder_homepage/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      557 2022-02-23 17:41:16.000000 girder-homepage-3.1.9.dev8/girder_homepage/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      422 2022-02-23 17:41:16.000000 girder-homepage-3.1.9.dev8/girder_homepage/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      267 2022-02-23 17:41:16.000000 girder-homepage-3.1.9.dev8/girder_homepage/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2022-02-23 17:41:16.000000 girder-homepage-3.1.9.dev8/girder_homepage/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2432 2022-02-23 17:41:16.000000 girder-homepage-3.1.9.dev8/girder_homepage/rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1695 2022-02-23 17:41:16.000000 girder-homepage-3.1.9.dev8/girder_homepage/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:48.000000 girder-homepage-3.1.9.dev8/girder_homepage.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      738 2022-02-23 17:41:47.000000 girder-homepage-3.1.9.dev8/girder_homepage.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      804 2022-02-23 17:41:48.000000 girder-homepage-3.1.9.dev8/girder_homepage.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:47.000000 girder-homepage-3.1.9.dev8/girder_homepage.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       59 2022-02-23 17:41:47.000000 girder-homepage-3.1.9.dev8/girder_homepage.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:47.000000 girder-homepage-3.1.9.dev8/girder_homepage.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 17:41:47.000000 girder-homepage-3.1.9.dev8/girder_homepage.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2022-02-23 17:41:47.000000 girder-homepage-3.1.9.dev8/girder_homepage.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:48.000000 girder-homepage-3.1.9.dev8/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-homepage-3.1.9.dev8/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6120 2022-02-23 17:41:16.000000 girder-homepage-3.1.9.dev8/plugin_tests/homepageSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      724 2022-02-23 17:41:16.000000 girder-homepage-3.1.9.dev8/plugin_tests/homepage_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2022-02-23 17:41:16.000000 girder-homepage-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1793 2022-02-23 17:41:16.000000 girder-homepage-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      738 2022-02-23 17:41:48.000000 girder-homepage-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:41:48.000000 girder-homepage-3.1.9.dev8/setup.cfg
```

### Comparing `girder-homepage-3.1.9.dev6/girder_homepage/web_client/stylesheets/configView.styl` & `girder-homepage-3.1.9.dev8/girder_homepage/web_client/stylesheets/configView.styl`

 * *Files identical despite different names*

### Comparing `girder-homepage-3.1.9.dev6/girder_homepage/web_client/templates/configView.pug` & `girder-homepage-3.1.9.dev8/girder_homepage/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-homepage-3.1.9.dev6/girder_homepage/web_client/views/ConfigView.js` & `girder-homepage-3.1.9.dev8/girder_homepage/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-homepage-3.1.9.dev6/girder_homepage/web_client/views/FrontPageView.js` & `girder-homepage-3.1.9.dev8/girder_homepage/web_client/views/FrontPageView.js`

 * *Files identical despite different names*

### Comparing `girder-homepage-3.1.9.dev6/girder_homepage/web_client/package.json` & `girder-homepage-3.1.9.dev8/girder_homepage/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-homepage-3.1.9.dev6/girder_homepage/rest.py` & `girder-homepage-3.1.9.dev8/girder_homepage/rest.py`

 * *Files identical despite different names*

### Comparing `girder-homepage-3.1.9.dev6/girder_homepage/settings.py` & `girder-homepage-3.1.9.dev8/girder_homepage/settings.py`

 * *Files identical despite different names*

### Comparing `girder-homepage-3.1.9.dev6/girder_homepage.egg-info/PKG-INFO` & `girder-homepage-3.1.9.dev8/girder_homepage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-homepage
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Customize the homepage using Markdown.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#homepage
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `girder-homepage-3.1.9.dev6/girder_homepage.egg-info/SOURCES.txt` & `girder-homepage-3.1.9.dev8/girder_homepage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-homepage-3.1.9.dev6/plugin_tests/homepageSpec.js` & `girder-homepage-3.1.9.dev8/plugin_tests/homepageSpec.js`

 * *Files identical despite different names*

### Comparing `girder-homepage-3.1.9.dev6/plugin_tests/homepage_test.py` & `girder-homepage-3.1.9.dev8/plugin_tests/homepage_test.py`

 * *Files identical despite different names*

### Comparing `girder-homepage-3.1.9.dev6/setup.py` & `girder-homepage-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-homepage-3.1.9.dev6/PKG-INFO` & `girder-homepage-3.1.9.dev8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-homepage
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Customize the homepage using Markdown.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#homepage
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

