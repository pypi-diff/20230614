# Comparing `tmp/flet_runtime-0.8.0.dev1500.tar.gz` & `tmp/flet_runtime-0.8.0.dev1511.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_runtime-0.8.0.dev1500.tar", max compression
+gzip compressed data, was "flet_runtime-0.8.0.dev1511.tar", max compression
```

## Comparing `flet_runtime-0.8.0.dev1500.tar` & `flet_runtime-0.8.0.dev1511.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      204 2023-06-12 18:16:06.982696 flet_runtime-0.8.0.dev1500/README.md
--rw-r--r--   0        0        0      747 2023-06-12 18:16:37.563113 flet_runtime-0.8.0.dev1500/pyproject.toml
--rw-r--r--   0        0        0      107 2023-06-12 18:16:06.982696 flet_runtime-0.8.0.dev1500/src/flet_runtime/__init__.py
--rw-r--r--   0        0        0    23064 2023-06-12 18:16:06.982696 flet_runtime-0.8.0.dev1500/src/flet_runtime/app.py
--rw-r--r--   0        0        0     6309 2023-06-12 18:16:06.982696 flet_runtime-0.8.0.dev1500/src/flet_runtime/async_local_socket_connection.py
--rw-r--r--   0        0        0      252 2023-06-12 18:16:06.982696 flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/__init__.py
--rw-r--r--   0        0        0     9107 2023-06-12 18:16:06.982696 flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/authorization.py
--rw-r--r--   0        0        0      128 2023-06-12 18:16:06.982696 flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/group.py
--rw-r--r--   0        0        0     1515 2023-06-12 18:16:06.982696 flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/oauth_provider.py
--rw-r--r--   0        0        0      847 2023-06-12 18:16:06.982696 flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/oauth_token.py
--rw-r--r--   0        0        0      324 2023-06-12 18:16:06.982696 flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/providers/__init__.py
--rw-r--r--   0        0        0      743 2023-06-12 18:16:06.982696 flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/providers/auth0_oauth_provider.py
--rw-r--r--   0        0        0      848 2023-06-12 18:16:06.982696 flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/providers/azure_oauth_provider.py
--rw-r--r--   0        0        0     3683 2023-06-12 18:16:06.982696 flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/providers/github_oauth_provider.py
--rw-r--r--   0        0        0      807 2023-06-12 18:16:06.982696 flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/providers/google_oauth_provider.py
--rw-r--r--   0        0        0      146 2023-06-12 18:16:06.982696 flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/user.py
--rw-r--r--   0        0        0    10255 2023-06-12 18:16:06.986697 flet_runtime-0.8.0.dev1500/src/flet_runtime/pubsub.py
--rw-r--r--   0        0        0     6934 2023-06-12 18:16:06.986697 flet_runtime-0.8.0.dev1500/src/flet_runtime/sync_local_socket_connection.py
--rw-r--r--   0        0        0     7334 2023-06-12 18:16:06.986697 flet_runtime-0.8.0.dev1500/src/flet_runtime/utils.py
--rw-r--r--   0        0        0      103 2023-06-12 18:16:06.986697 flet_runtime-0.8.0.dev1500/src/flet_runtime/version.py
--rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 flet_runtime-0.8.0.dev1500/PKG-INFO
+-rw-r--r--   0        0        0      204 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/README.md
+-rw-r--r--   0        0        0      747 2023-06-14 20:13:05.642069 flet_runtime-0.8.0.dev1511/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/__init__.py
+-rw-r--r--   0        0        0    23064 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/app.py
+-rw-r--r--   0        0        0     6309 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/async_local_socket_connection.py
+-rw-r--r--   0        0        0      252 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/__init__.py
+-rw-r--r--   0        0        0     9107 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/authorization.py
+-rw-r--r--   0        0        0      128 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/group.py
+-rw-r--r--   0        0        0     1515 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/oauth_provider.py
+-rw-r--r--   0        0        0      847 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/oauth_token.py
+-rw-r--r--   0        0        0      324 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/providers/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/providers/auth0_oauth_provider.py
+-rw-r--r--   0        0        0      848 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/providers/azure_oauth_provider.py
+-rw-r--r--   0        0        0     3683 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/providers/github_oauth_provider.py
+-rw-r--r--   0        0        0      807 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/providers/google_oauth_provider.py
+-rw-r--r--   0        0        0      146 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/user.py
+-rw-r--r--   0        0        0    10255 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/pubsub.py
+-rw-r--r--   0        0        0     6934 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/sync_local_socket_connection.py
+-rw-r--r--   0        0        0     3593 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/utils.py
+-rw-r--r--   0        0        0      103 2023-06-14 20:12:35.177499 flet_runtime-0.8.0.dev1511/src/flet_runtime/version.py
+-rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 flet_runtime-0.8.0.dev1511/PKG-INFO
```

### Comparing `flet_runtime-0.8.0.dev1500/pyproject.toml` & `flet_runtime-0.8.0.dev1511/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-runtime"
-version = "0.8.0.dev1500"
+version = "0.8.0.dev1511"
 description = "Flet Runtime - a base package for Flet desktop and Flet mobile."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet_runtime", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-core = "0.8.0.dev1500"
+flet-core = "0.8.0.dev1511"
 python = "^3.7"
 oauthlib = "^3.2.2"
 httpx = "^0.24.1"
 typing-extensions = { version = "^4.6.2", python = "<3.8" }
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `flet_runtime-0.8.0.dev1500/src/flet_runtime/app.py` & `flet_runtime-0.8.0.dev1511/src/flet_runtime/app.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1500/src/flet_runtime/async_local_socket_connection.py` & `flet_runtime-0.8.0.dev1511/src/flet_runtime/async_local_socket_connection.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/authorization.py` & `flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/authorization.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/oauth_provider.py` & `flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/oauth_token.py` & `flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/oauth_token.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/providers/auth0_oauth_provider.py` & `flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/providers/auth0_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/providers/azure_oauth_provider.py` & `flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/providers/azure_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/providers/github_oauth_provider.py` & `flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/providers/github_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1500/src/flet_runtime/auth/providers/google_oauth_provider.py` & `flet_runtime-0.8.0.dev1511/src/flet_runtime/auth/providers/google_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1500/src/flet_runtime/pubsub.py` & `flet_runtime-0.8.0.dev1511/src/flet_runtime/pubsub.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1500/src/flet_runtime/sync_local_socket_connection.py` & `flet_runtime-0.8.0.dev1511/src/flet_runtime/sync_local_socket_connection.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1500/PKG-INFO` & `flet_runtime-0.8.0.dev1511/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flet-runtime
-Version: 0.8.0.dev1500
+Version: 0.8.0.dev1511
 Summary: Flet Runtime - a base package for Flet desktop and Flet mobile.
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-core (==0.8.0.dev1500)
+Requires-Dist: flet-core (==0.8.0.dev1511)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
 Requires-Dist: typing-extensions (>=4.6.2,<5.0.0) ; python_version < "3.8"
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
```

