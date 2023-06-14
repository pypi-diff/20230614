# Comparing `tmp/backend.ai-plugin-23.3.5.tar.gz` & `tmp/backend.ai-plugin-23.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-plugin-23.3.5.tar", last modified: Tue Jun 13 03:42:17 2023, max compression
+gzip compressed data, was "backend.ai-plugin-23.3.6.tar", last modified: Wed Jun 14 11:13:27 2023, max compression
```

## Comparing `backend.ai-plugin-23.3.5.tar` & `backend.ai-plugin-23.3.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:17.528261 backend.ai-plugin-23.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-13 03:42:17.528261 backend.ai-plugin-23.3.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:17.524261 backend.ai-plugin-23.3.5/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:17.524261 backend.ai-plugin-23.3.5/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:17.528261 backend.ai-plugin-23.3.5/ai/backend/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/ai/backend/plugin/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/ai/backend/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/ai/backend/plugin/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/ai/backend/plugin/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:17.528261 backend.ai-plugin-23.3.5/backend.ai_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/backend.ai_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/backend.ai_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/backend.ai_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/backend.ai_plugin.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/backend.ai_plugin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/backend.ai_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 03:42:17.528261 backend.ai-plugin-23.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:27.061631 backend.ai-plugin-23.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 11:13:26.000000 backend.ai-plugin-23.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-14 11:13:27.061631 backend.ai-plugin-23.3.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:27.061631 backend.ai-plugin-23.3.6/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:27.061631 backend.ai-plugin-23.3.6/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:27.061631 backend.ai-plugin-23.3.6/ai/backend/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 11:13:26.000000 backend.ai-plugin-23.3.6/ai/backend/plugin/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-14 11:13:26.000000 backend.ai-plugin-23.3.6/ai/backend/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-06-14 11:13:26.000000 backend.ai-plugin-23.3.6/ai/backend/plugin/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 11:13:26.000000 backend.ai-plugin-23.3.6/ai/backend/plugin/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:27.061631 backend.ai-plugin-23.3.6/backend.ai_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-14 11:13:27.000000 backend.ai-plugin-23.3.6/backend.ai_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-14 11:13:27.000000 backend.ai-plugin-23.3.6/backend.ai_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:27.000000 backend.ai-plugin-23.3.6/backend.ai_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:27.000000 backend.ai-plugin-23.3.6/backend.ai_plugin.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:27.000000 backend.ai-plugin-23.3.6/backend.ai_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-14 11:13:27.000000 backend.ai-plugin-23.3.6/backend.ai_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-14 11:13:26.000000 backend.ai-plugin-23.3.6/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:13:27.061631 backend.ai-plugin-23.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-14 11:13:26.000000 backend.ai-plugin-23.3.6/setup.py
```

### Comparing `backend.ai-plugin-23.3.5/PKG-INFO` & `backend.ai-plugin-23.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-plugin
-Version: 23.3.5
+Version: 23.3.6
 Summary: Backend.AI Plugin Subsystem
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-plugin-23.3.5/ai/backend/plugin/entrypoint.py` & `backend.ai-plugin-23.3.6/ai/backend/plugin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `backend.ai-plugin-23.3.5/backend.ai_plugin.egg-info/PKG-INFO` & `backend.ai-plugin-23.3.6/backend.ai_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-plugin
-Version: 23.3.5
+Version: 23.3.6
 Summary: Backend.AI Plugin Subsystem
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-plugin-23.3.5/backend_shim.py` & `backend.ai-plugin-23.3.6/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-plugin-23.3.5/setup.py` & `backend.ai-plugin-23.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,11 +46,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.5
+    'version': """23.03.6
 """,
     'zip_safe': False,
 })
```

