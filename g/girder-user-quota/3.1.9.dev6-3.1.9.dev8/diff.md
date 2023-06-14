# Comparing `tmp/girder-user-quota-3.1.9.dev6.tar.gz` & `tmp/girder-user-quota-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-user-quota-3.1.9.dev6.tar", last modified: Wed Feb 23 16:10:08 2022, max compression
+gzip compressed data, was "dist/girder-user-quota-3.1.9.dev8.tar", last modified: Wed Feb 23 17:42:09 2022, max compression
```

## Comparing `girder-user-quota-3.1.9.dev6.tar` & `girder-user-quota-3.1.9.dev8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      154 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/models/CollectionModel.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/models/UserModel.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3788 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/models/extendModel.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      395 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/stylesheets/userQuota.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      240 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/templates/collectionViewPoliciesMenu.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1337 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3480 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      228 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/templates/userViewPoliciesMenu.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/utilities/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2168 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/utilities/Conversions.js
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      283 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/views/CollectionView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3357 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6817 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/views/QuotaPoliciesWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      677 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/views/UploadWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      241 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/views/UserView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1609 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/views/extendView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      295 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      559 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      429 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      898 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16560 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/quota.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      735 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/girder_user_quota/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/girder_user_quota.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      765 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/girder_user_quota.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1424 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/girder_user_quota.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/girder_user_quota.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       64 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/girder_user_quota.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/girder_user_quota.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/girder_user_quota.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       18 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/girder_user_quota.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16489 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/plugin_tests/userQuotaSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21166 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/plugin_tests/user_quota_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1813 2022-02-23 16:09:15.000000 girder-user-quota-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      765 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:10:08.000000 girder-user-quota-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:09.000000 girder-user-quota-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:09.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:09.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:09.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      154 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/models/CollectionModel.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      130 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/models/UserModel.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3788 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/models/extendModel.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:09.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      395 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/stylesheets/userQuota.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:09.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      240 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/templates/collectionViewPoliciesMenu.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1337 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/templates/configView.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3480 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      228 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/templates/userViewPoliciesMenu.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:09.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/utilities/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2168 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/utilities/Conversions.js
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:09.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      283 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/views/CollectionView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3357 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6817 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/views/QuotaPoliciesWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      677 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/views/UploadWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      241 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/views/UserView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1609 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/views/extendView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      295 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      559 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      429 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/routes.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      898 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16560 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/quota.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      735 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/girder_user_quota/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:09.000000 girder-user-quota-3.1.9.dev8/girder_user_quota.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      765 2022-02-23 17:42:08.000000 girder-user-quota-3.1.9.dev8/girder_user_quota.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1424 2022-02-23 17:42:09.000000 girder-user-quota-3.1.9.dev8/girder_user_quota.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:42:08.000000 girder-user-quota-3.1.9.dev8/girder_user_quota.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       64 2022-02-23 17:42:08.000000 girder-user-quota-3.1.9.dev8/girder_user_quota.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:42:08.000000 girder-user-quota-3.1.9.dev8/girder_user_quota.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 17:42:08.000000 girder-user-quota-3.1.9.dev8/girder_user_quota.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       18 2022-02-23 17:42:08.000000 girder-user-quota-3.1.9.dev8/girder_user_quota.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:42:09.000000 girder-user-quota-3.1.9.dev8/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16489 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/plugin_tests/userQuotaSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21166 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/plugin_tests/user_quota_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1813 2022-02-23 17:41:16.000000 girder-user-quota-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      765 2022-02-23 17:42:09.000000 girder-user-quota-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:42:09.000000 girder-user-quota-3.1.9.dev8/setup.cfg
```

### Comparing `girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/models/extendModel.js` & `girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/models/extendModel.js`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/templates/configView.pug` & `girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug` & `girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/utilities/Conversions.js` & `girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/utilities/Conversions.js`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/views/ConfigView.js` & `girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/views/QuotaPoliciesWidget.js` & `girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/views/QuotaPoliciesWidget.js`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/views/UploadWidget.js` & `girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/views/UploadWidget.js`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/views/extendView.js` & `girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/views/extendView.js`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.1.9.dev6/girder_user_quota/web_client/package.json` & `girder-user-quota-3.1.9.dev8/girder_user_quota/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.1.9.dev6/girder_user_quota/__init__.py` & `girder-user-quota-3.1.9.dev8/girder_user_quota/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.1.9.dev6/girder_user_quota/quota.py` & `girder-user-quota-3.1.9.dev8/girder_user_quota/quota.py`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.1.9.dev6/girder_user_quota/settings.py` & `girder-user-quota-3.1.9.dev8/girder_user_quota/settings.py`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.1.9.dev6/girder_user_quota.egg-info/PKG-INFO` & `girder-user-quota-3.1.9.dev8/girder_user_quota.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-user-quota
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Limits total file size stored for individual users and collections and can direct all files to a specific assetstore
 Home-page: UNKNOWN
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `girder-user-quota-3.1.9.dev6/girder_user_quota.egg-info/SOURCES.txt` & `girder-user-quota-3.1.9.dev8/girder_user_quota.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.1.9.dev6/plugin_tests/userQuotaSpec.js` & `girder-user-quota-3.1.9.dev8/plugin_tests/userQuotaSpec.js`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.1.9.dev6/plugin_tests/user_quota_test.py` & `girder-user-quota-3.1.9.dev8/plugin_tests/user_quota_test.py`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.1.9.dev6/setup.py` & `girder-user-quota-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.1.9.dev6/PKG-INFO` & `girder-user-quota-3.1.9.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-user-quota
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Limits total file size stored for individual users and collections and can direct all files to a specific assetstore
 Home-page: UNKNOWN
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

