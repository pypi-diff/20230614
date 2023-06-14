# Comparing `tmp/girder-oauth-3.1.9.dev6.tar.gz` & `tmp/girder-oauth-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-oauth-3.1.9.dev6.tar", last modified: Wed Feb 23 16:09:57 2022, max compression
+gzip compressed data, was "dist/girder-oauth-3.1.9.dev8.tar", last modified: Wed Feb 23 17:41:57 2022, max compression
```

## Comparing `girder-oauth-3.1.9.dev6.tar` & `girder-oauth-3.1.9.dev8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/girder_oauth/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/girder_oauth/providers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      448 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/providers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9107 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/providers/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3550 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/providers/bitbucket.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2527 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/providers/box.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3277 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/providers/github.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2770 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/providers/globus.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2959 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/providers/google.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2975 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/providers/linkedin.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/girder_oauth/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/girder_oauth/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      458 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/web_client/stylesheets/configView.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2398 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/web_client/stylesheets/oauthLoginView.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/girder_oauth/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2303 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      392 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/web_client/templates/oauthLoginView.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/girder_oauth/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6930 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      416 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/web_client/views/LoginView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2661 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/web_client/views/OAuthLoginView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      607 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/web_client/views/RegisterView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      108 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      568 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      410 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1773 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5015 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2706 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/girder_oauth/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/girder_oauth.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      752 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/girder_oauth.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1157 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/girder_oauth.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/girder_oauth.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       50 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/girder_oauth.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/girder_oauth.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       18 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/girder_oauth.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       13 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/girder_oauth.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    63218 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/plugin_tests/oauth_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       50 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1832 2022-02-23 16:09:15.000000 girder-oauth-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      752 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:09:57.000000 girder-oauth-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/girder_oauth/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/girder_oauth/providers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      448 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/providers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9107 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/providers/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3550 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/providers/bitbucket.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2527 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/providers/box.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3277 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/providers/github.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2770 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/providers/globus.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2959 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/providers/google.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2975 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/providers/linkedin.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/girder_oauth/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/girder_oauth/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      458 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/web_client/stylesheets/configView.styl
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2398 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/web_client/stylesheets/oauthLoginView.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/girder_oauth/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2303 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/web_client/templates/configView.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      392 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/web_client/templates/oauthLoginView.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/girder_oauth/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6930 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      416 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/web_client/views/LoginView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2661 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/web_client/views/OAuthLoginView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      607 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/web_client/views/RegisterView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      108 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      568 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      410 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1773 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5015 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2706 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/girder_oauth/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/girder_oauth.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      752 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/girder_oauth.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1157 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/girder_oauth.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/girder_oauth.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       50 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/girder_oauth.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/girder_oauth.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       18 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/girder_oauth.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       13 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/girder_oauth.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    63218 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/plugin_tests/oauth_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       50 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1832 2022-02-23 17:41:16.000000 girder-oauth-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      752 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:41:57.000000 girder-oauth-3.1.9.dev8/setup.cfg
```

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth/providers/base.py` & `girder-oauth-3.1.9.dev8/girder_oauth/providers/base.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth/providers/bitbucket.py` & `girder-oauth-3.1.9.dev8/girder_oauth/providers/bitbucket.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth/providers/box.py` & `girder-oauth-3.1.9.dev8/girder_oauth/providers/box.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth/providers/github.py` & `girder-oauth-3.1.9.dev8/girder_oauth/providers/github.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth/providers/globus.py` & `girder-oauth-3.1.9.dev8/girder_oauth/providers/globus.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth/providers/google.py` & `girder-oauth-3.1.9.dev8/girder_oauth/providers/google.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth/providers/linkedin.py` & `girder-oauth-3.1.9.dev8/girder_oauth/providers/linkedin.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth/web_client/stylesheets/oauthLoginView.styl` & `girder-oauth-3.1.9.dev8/girder_oauth/web_client/stylesheets/oauthLoginView.styl`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth/web_client/templates/configView.pug` & `girder-oauth-3.1.9.dev8/girder_oauth/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth/web_client/views/ConfigView.js` & `girder-oauth-3.1.9.dev8/girder_oauth/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth/web_client/views/OAuthLoginView.js` & `girder-oauth-3.1.9.dev8/girder_oauth/web_client/views/OAuthLoginView.js`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth/web_client/views/RegisterView.js` & `girder-oauth-3.1.9.dev8/girder_oauth/web_client/views/RegisterView.js`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth/web_client/package.json` & `girder-oauth-3.1.9.dev8/girder_oauth/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth/__init__.py` & `girder-oauth-3.1.9.dev8/girder_oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth/rest.py` & `girder-oauth-3.1.9.dev8/girder_oauth/rest.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth/settings.py` & `girder-oauth-3.1.9.dev8/girder_oauth/settings.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth.egg-info/PKG-INFO` & `girder-oauth-3.1.9.dev8/girder_oauth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-oauth
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Allow users to login via supported OAuth2 providers.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#oauth-login
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `girder-oauth-3.1.9.dev6/girder_oauth.egg-info/SOURCES.txt` & `girder-oauth-3.1.9.dev8/girder_oauth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/plugin_tests/oauth_test.py` & `girder-oauth-3.1.9.dev8/plugin_tests/oauth_test.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/setup.py` & `girder-oauth-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.1.9.dev6/PKG-INFO` & `girder-oauth-3.1.9.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-oauth
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Allow users to login via supported OAuth2 providers.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#oauth-login
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

