# Comparing `tmp/girder-ldap-3.1.9.dev6.tar.gz` & `tmp/girder-ldap-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-ldap-3.1.9.dev6.tar", last modified: Wed Feb 23 16:09:55 2022, max compression
+gzip compressed data, was "dist/girder-ldap-3.1.9.dev8.tar", last modified: Wed Feb 23 17:41:55 2022, max compression
```

## Comparing `girder-ldap-3.1.9.dev6.tar` & `girder-ldap-3.1.9.dev8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:55.000000 girder-ldap-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:55.000000 girder-ldap-3.1.9.dev6/girder_ldap/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:55.000000 girder-ldap-3.1.9.dev6/girder_ldap/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:55.000000 girder-ldap-3.1.9.dev6/girder_ldap/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      272 2022-02-23 16:09:15.000000 girder-ldap-3.1.9.dev6/girder_ldap/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:55.000000 girder-ldap-3.1.9.dev6/girder_ldap/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      899 2022-02-23 16:09:15.000000 girder-ldap-3.1.9.dev6/girder_ldap/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2592 2022-02-23 16:09:15.000000 girder-ldap-3.1.9.dev6/girder_ldap/web_client/templates/editServerMixin.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-02-23 16:09:15.000000 girder-ldap-3.1.9.dev6/girder_ldap/web_client/templates/newServerTemplate.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:55.000000 girder-ldap-3.1.9.dev6/girder_ldap/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4413 2022-02-23 16:09:15.000000 girder-ldap-3.1.9.dev6/girder_ldap/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2022-02-23 16:09:15.000000 girder-ldap-3.1.9.dev6/girder_ldap/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      561 2022-02-23 16:09:15.000000 girder-ldap-3.1.9.dev6/girder_ldap/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      406 2022-02-23 16:09:15.000000 girder-ldap-3.1.9.dev6/girder_ldap/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5384 2022-02-23 16:09:15.000000 girder-ldap-3.1.9.dev6/girder_ldap/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1363 2022-02-23 16:09:15.000000 girder-ldap-3.1.9.dev6/girder_ldap/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:55.000000 girder-ldap-3.1.9.dev6/girder_ldap.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2022-02-23 16:09:55.000000 girder-ldap-3.1.9.dev6/girder_ldap.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      716 2022-02-23 16:09:55.000000 girder-ldap-3.1.9.dev6/girder_ldap.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:55.000000 girder-ldap-3.1.9.dev6/girder_ldap.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       47 2022-02-23 16:09:55.000000 girder-ldap-3.1.9.dev6/girder_ldap.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:55.000000 girder-ldap-3.1.9.dev6/girder_ldap.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       17 2022-02-23 16:09:55.000000 girder-ldap-3.1.9.dev6/girder_ldap.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-02-23 16:09:55.000000 girder-ldap-3.1.9.dev6/girder_ldap.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:55.000000 girder-ldap-3.1.9.dev6/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-ldap-3.1.9.dev6/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7614 2022-02-23 16:09:15.000000 girder-ldap-3.1.9.dev6/plugin_tests/ldap_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       49 2022-02-23 16:09:15.000000 girder-ldap-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1734 2022-02-23 16:09:15.000000 girder-ldap-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2022-02-23 16:09:55.000000 girder-ldap-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:09:55.000000 girder-ldap-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:55.000000 girder-ldap-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:55.000000 girder-ldap-3.1.9.dev8/girder_ldap/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:55.000000 girder-ldap-3.1.9.dev8/girder_ldap/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:55.000000 girder-ldap-3.1.9.dev8/girder_ldap/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      272 2022-02-23 17:41:16.000000 girder-ldap-3.1.9.dev8/girder_ldap/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:55.000000 girder-ldap-3.1.9.dev8/girder_ldap/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      899 2022-02-23 17:41:16.000000 girder-ldap-3.1.9.dev8/girder_ldap/web_client/templates/configView.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2592 2022-02-23 17:41:16.000000 girder-ldap-3.1.9.dev8/girder_ldap/web_client/templates/editServerMixin.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-02-23 17:41:16.000000 girder-ldap-3.1.9.dev8/girder_ldap/web_client/templates/newServerTemplate.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:55.000000 girder-ldap-3.1.9.dev8/girder_ldap/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4413 2022-02-23 17:41:16.000000 girder-ldap-3.1.9.dev8/girder_ldap/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2022-02-23 17:41:16.000000 girder-ldap-3.1.9.dev8/girder_ldap/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      561 2022-02-23 17:41:16.000000 girder-ldap-3.1.9.dev8/girder_ldap/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      406 2022-02-23 17:41:16.000000 girder-ldap-3.1.9.dev8/girder_ldap/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5384 2022-02-23 17:41:16.000000 girder-ldap-3.1.9.dev8/girder_ldap/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1363 2022-02-23 17:41:16.000000 girder-ldap-3.1.9.dev8/girder_ldap/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:55.000000 girder-ldap-3.1.9.dev8/girder_ldap.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2022-02-23 17:41:54.000000 girder-ldap-3.1.9.dev8/girder_ldap.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      716 2022-02-23 17:41:55.000000 girder-ldap-3.1.9.dev8/girder_ldap.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:54.000000 girder-ldap-3.1.9.dev8/girder_ldap.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       47 2022-02-23 17:41:54.000000 girder-ldap-3.1.9.dev8/girder_ldap.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:54.000000 girder-ldap-3.1.9.dev8/girder_ldap.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       17 2022-02-23 17:41:54.000000 girder-ldap-3.1.9.dev8/girder_ldap.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-02-23 17:41:54.000000 girder-ldap-3.1.9.dev8/girder_ldap.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:55.000000 girder-ldap-3.1.9.dev8/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-ldap-3.1.9.dev8/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7614 2022-02-23 17:41:16.000000 girder-ldap-3.1.9.dev8/plugin_tests/ldap_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       49 2022-02-23 17:41:16.000000 girder-ldap-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1734 2022-02-23 17:41:16.000000 girder-ldap-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2022-02-23 17:41:55.000000 girder-ldap-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:41:55.000000 girder-ldap-3.1.9.dev8/setup.cfg
```

### Comparing `girder-ldap-3.1.9.dev6/girder_ldap/web_client/templates/configView.pug` & `girder-ldap-3.1.9.dev8/girder_ldap/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.1.9.dev6/girder_ldap/web_client/templates/editServerMixin.pug` & `girder-ldap-3.1.9.dev8/girder_ldap/web_client/templates/editServerMixin.pug`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.1.9.dev6/girder_ldap/web_client/views/ConfigView.js` & `girder-ldap-3.1.9.dev8/girder_ldap/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.1.9.dev6/girder_ldap/web_client/package.json` & `girder-ldap-3.1.9.dev8/girder_ldap/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.1.9.dev6/girder_ldap/__init__.py` & `girder-ldap-3.1.9.dev8/girder_ldap/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.1.9.dev6/girder_ldap/settings.py` & `girder-ldap-3.1.9.dev8/girder_ldap/settings.py`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.1.9.dev6/girder_ldap.egg-info/PKG-INFO` & `girder-ldap-3.1.9.dev8/girder_ldap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-ldap
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Authenticate user credentials against LDAP or Active Directory servers.
 Home-page: UNKNOWN
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `girder-ldap-3.1.9.dev6/girder_ldap.egg-info/SOURCES.txt` & `girder-ldap-3.1.9.dev8/girder_ldap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.1.9.dev6/plugin_tests/ldap_test.py` & `girder-ldap-3.1.9.dev8/plugin_tests/ldap_test.py`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.1.9.dev6/setup.py` & `girder-ldap-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.1.9.dev6/PKG-INFO` & `girder-ldap-3.1.9.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-ldap
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Authenticate user credentials against LDAP or Active Directory servers.
 Home-page: UNKNOWN
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

