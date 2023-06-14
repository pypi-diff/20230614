# Comparing `tmp/flet_embed-0.8.0.dev1500.tar.gz` & `tmp/flet_embed-0.8.0.dev1511.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_embed-0.8.0.dev1500.tar", max compression
+gzip compressed data, was "flet_embed-0.8.0.dev1511.tar", max compression
```

## Comparing `flet_embed-0.8.0.dev1500.tar` & `flet_embed-0.8.0.dev1511.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      212 2023-06-12 18:16:06.982696 flet_embed-0.8.0.dev1500/README.md
--rw-r--r--   0        0        0      758 2023-06-12 18:16:37.391111 flet_embed-0.8.0.dev1500/pyproject.toml
--rw-r--r--   0        0        0       27 2023-06-12 18:16:06.982696 flet_embed-0.8.0.dev1500/src/flet/__init__.py
--rw-r--r--   0        0        0       32 2023-06-12 18:16:06.982696 flet_embed-0.8.0.dev1500/src/flet/auth/__init__.py
--rw-r--r--   0        0        0       42 2023-06-12 18:16:06.982696 flet_embed-0.8.0.dev1500/src/flet/auth/providers/__init__.py
--rw-r--r--   0        0        0       31 2023-06-12 18:16:06.982696 flet_embed-0.8.0.dev1500/src/flet/canvas/__init__.py
--rw-r--r--   0        0        0       55 2023-06-12 18:16:06.982696 flet_embed-0.8.0.dev1500/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-06-12 18:16:06.982696 flet_embed-0.8.0.dev1500/src/flet/plotly_chart.py
--rw-r--r--   0        0        0       47 2023-06-12 18:16:06.982696 flet_embed-0.8.0.dev1500/src/flet/utils/__init__.py
--rw-r--r--   0        0        0      103 2023-06-12 18:16:06.982696 flet_embed-0.8.0.dev1500/src/flet/version.py
--rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 flet_embed-0.8.0.dev1500/PKG-INFO
+-rw-r--r--   0        0        0      212 2023-06-14 20:12:35.177499 flet_embed-0.8.0.dev1511/README.md
+-rw-r--r--   0        0        0      758 2023-06-14 20:13:05.466060 flet_embed-0.8.0.dev1511/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-06-14 20:12:35.177499 flet_embed-0.8.0.dev1511/src/flet/__init__.py
+-rw-r--r--   0        0        0       32 2023-06-14 20:12:35.177499 flet_embed-0.8.0.dev1511/src/flet/auth/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-14 20:12:35.177499 flet_embed-0.8.0.dev1511/src/flet/auth/providers/__init__.py
+-rw-r--r--   0        0        0       31 2023-06-14 20:12:35.177499 flet_embed-0.8.0.dev1511/src/flet/canvas/__init__.py
+-rw-r--r--   0        0        0       55 2023-06-14 20:12:35.177499 flet_embed-0.8.0.dev1511/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-06-14 20:12:35.177499 flet_embed-0.8.0.dev1511/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0       44 2023-06-14 20:12:35.177499 flet_embed-0.8.0.dev1511/src/flet/utils/__init__.py
+-rw-r--r--   0        0        0      103 2023-06-14 20:12:35.177499 flet_embed-0.8.0.dev1511/src/flet/version.py
+-rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 flet_embed-0.8.0.dev1511/PKG-INFO
```

### Comparing `flet_embed-0.8.0.dev1500/pyproject.toml` & `flet_embed-0.8.0.dev1511/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-embed"
-version = "0.8.0.dev1500"
+version = "0.8.0.dev1511"
 description = "Flet Embed - embed Python into Flutter apps"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-runtime = "0.8.0.dev1500"
+flet-runtime = "0.8.0.dev1511"
 python = "^3.7"
 typing-extensions = { version = "^4.6.2", python = "<3.8" }
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.6"
 pytest = "^7.2.0"
```

### Comparing `flet_embed-0.8.0.dev1500/PKG-INFO` & `flet_embed-0.8.0.dev1511/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flet-embed
-Version: 0.8.0.dev1500
+Version: 0.8.0.dev1511
 Summary: Flet Embed - embed Python into Flutter apps
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
-Requires-Dist: flet-runtime (==0.8.0.dev1500)
+Requires-Dist: flet-runtime (==0.8.0.dev1511)
 Requires-Dist: typing-extensions (>=4.6.2,<5.0.0) ; python_version < "3.8"
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
 
 # Flet embedded library
```

