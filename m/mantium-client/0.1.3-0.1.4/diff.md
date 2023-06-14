# Comparing `tmp/mantium_client-0.1.3.tar.gz` & `tmp/mantium_client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mantium_client-0.1.3.tar", max compression
+gzip compressed data, was "mantium_client-0.1.4.tar", max compression
```

## Comparing `mantium_client-0.1.3.tar` & `mantium_client-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-06-13 19:47:52.127222 mantium_client-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     1338 2023-06-13 19:47:52.127222 mantium_client-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-13 19:47:52.127222 mantium_client-0.1.3/mantium_client/__init__.py
--rw-r--r--   0        0        0     4179 2023-06-13 19:47:52.127222 mantium_client-0.1.3/mantium_client/api_client.py
--rw-r--r--   0        0        0      894 2023-06-13 19:47:52.127222 mantium_client-0.1.3/mantium_client/invoke_tasks/__init__.py
--rw-r--r--   0        0        0     1447 2023-06-13 19:47:52.127222 mantium_client-0.1.3/mantium_client/invoke_tasks/build.py
--rw-r--r--   0        0        0      176 2023-06-13 19:47:52.127222 mantium_client-0.1.3/mantium_client/invoke_tasks/test.py
--rw-r--r--   0        0        0     1324 2023-06-13 19:47:52.127222 mantium_client-0.1.3/mantium_client/invoke_tasks/utils.py
--rw-r--r--   0        0        0       22 2023-06-13 19:47:52.127222 mantium_client-0.1.3/mantium_client/version.py
--rw-r--r--   0        0        0     1775 2023-06-13 19:47:52.127222 mantium_client-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 mantium_client-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-14 17:59:22.245009 mantium_client-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     1338 2023-06-14 17:59:22.245009 mantium_client-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 17:59:22.245009 mantium_client-0.1.4/mantium_client/__init__.py
+-rw-r--r--   0        0        0     4179 2023-06-14 17:59:22.245009 mantium_client-0.1.4/mantium_client/api_client.py
+-rw-r--r--   0        0        0      894 2023-06-14 17:59:22.245009 mantium_client-0.1.4/mantium_client/invoke_tasks/__init__.py
+-rw-r--r--   0        0        0     1447 2023-06-14 17:59:22.245009 mantium_client-0.1.4/mantium_client/invoke_tasks/build.py
+-rw-r--r--   0        0        0      176 2023-06-14 17:59:22.245009 mantium_client-0.1.4/mantium_client/invoke_tasks/test.py
+-rw-r--r--   0        0        0     1324 2023-06-14 17:59:22.245009 mantium_client-0.1.4/mantium_client/invoke_tasks/utils.py
+-rw-r--r--   0        0        0       22 2023-06-14 17:59:22.245009 mantium_client-0.1.4/mantium_client/version.py
+-rw-r--r--   0        0        0     1775 2023-06-14 17:59:22.245009 mantium_client-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 mantium_client-0.1.4/PKG-INFO
```

### Comparing `mantium_client-0.1.3/LICENSE.txt` & `mantium_client-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mantium_client-0.1.3/README.md` & `mantium_client-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mantium_client-0.1.3/mantium_client/api_client.py` & `mantium_client-0.1.4/mantium_client/api_client.py`

 * *Files identical despite different names*

### Comparing `mantium_client-0.1.3/mantium_client/invoke_tasks/__init__.py` & `mantium_client-0.1.4/mantium_client/invoke_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `mantium_client-0.1.3/mantium_client/invoke_tasks/build.py` & `mantium_client-0.1.4/mantium_client/invoke_tasks/build.py`

 * *Files identical despite different names*

### Comparing `mantium_client-0.1.3/mantium_client/invoke_tasks/utils.py` & `mantium_client-0.1.4/mantium_client/invoke_tasks/utils.py`

 * *Files identical despite different names*

### Comparing `mantium_client-0.1.3/pyproject.toml` & `mantium_client-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mantium-client"
-version = "0.1.3"
+version = "0.1.4"
 license = "Apache-2.0"
 description = "Python client for the Mantium API"
 authors = ["Mantium <support@mantiumai.com>"]
 readme = "README.md"
 repository = "https://github.com/mantiumai/mantium-client-py"
 homepage = "https://github.com/mantiumai/mantium-client-py"
 classifiers = [
```

### Comparing `mantium_client-0.1.3/PKG-INFO` & `mantium_client-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mantium-client
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python client for the Mantium API
 Home-page: https://github.com/mantiumai/mantium-client-py
 License: Apache-2.0
 Keywords: mantium,ChatGPT,AI
 Author: Mantium
 Author-email: support@mantiumai.com
 Requires-Python: >=3.10,<4.0
```

