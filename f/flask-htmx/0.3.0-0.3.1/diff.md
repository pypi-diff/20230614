# Comparing `tmp/flask_htmx-0.3.0.tar.gz` & `tmp/flask_htmx-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_htmx-0.3.0.tar", max compression
+gzip compressed data, was "flask_htmx-0.3.1.tar", max compression
```

## Comparing `flask_htmx-0.3.0.tar` & `flask_htmx-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2023-04-18 10:24:38.347851 flask_htmx-0.3.0/LICENSE
--rw-r--r--   0        0        0     4648 2023-04-18 10:24:38.347851 flask_htmx-0.3.0/README.rst
--rw-r--r--   0        0        0      108 2023-04-18 10:24:38.347851 flask_htmx-0.3.0/flask_htmx/__init__.py
--rw-r--r--   0        0        0      466 2023-04-18 10:24:38.347851 flask_htmx-0.3.0/flask_htmx/constants.py
--rw-r--r--   0        0        0     2680 2023-04-18 10:24:38.347851 flask_htmx-0.3.0/flask_htmx/htmx.py
--rw-r--r--   0        0        0     4767 2023-04-18 10:24:38.347851 flask_htmx-0.3.0/flask_htmx/responses.py
--rw-r--r--   0        0        0     1430 2023-04-18 10:25:16.752200 flask_htmx-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5851 1970-01-01 00:00:00.000000 flask_htmx-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-14 12:09:32.769885 flask_htmx-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4648 2023-06-14 12:09:32.769885 flask_htmx-0.3.1/README.rst
+-rw-r--r--   0        0        0      108 2023-06-14 12:09:32.769885 flask_htmx-0.3.1/flask_htmx/__init__.py
+-rw-r--r--   0        0        0      471 2023-06-14 12:09:32.769885 flask_htmx-0.3.1/flask_htmx/constants.py
+-rw-r--r--   0        0        0     2680 2023-06-14 12:09:32.769885 flask_htmx-0.3.1/flask_htmx/htmx.py
+-rw-r--r--   0        0        0     4767 2023-06-14 12:09:32.769885 flask_htmx-0.3.1/flask_htmx/responses.py
+-rw-r--r--   0        0        0     1430 2023-06-14 12:10:09.429842 flask_htmx-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5851 1970-01-01 00:00:00.000000 flask_htmx-0.3.1/PKG-INFO
```

### Comparing `flask_htmx-0.3.0/LICENSE` & `flask_htmx-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_htmx-0.3.0/README.rst` & `flask_htmx-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `flask_htmx-0.3.0/flask_htmx/htmx.py` & `flask_htmx-0.3.1/flask_htmx/htmx.py`

 * *Files identical despite different names*

### Comparing `flask_htmx-0.3.0/flask_htmx/responses.py` & `flask_htmx-0.3.1/flask_htmx/responses.py`

 * *Files identical despite different names*

### Comparing `flask_htmx-0.3.0/pyproject.toml` & `flask_htmx-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask-htmx"
-version = "0.3.0"
+version = "0.3.1"
 description = "A Flask extension to work with HTMX."
 authors = ["Edmond Chuc <edmond.chuc@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/edmondchuc/flask-htmx"
 repository = "https://github.com/edmondchuc/flask-htmx"
 documentation = "https://flask-htmx.readthedocs.io"
```

### Comparing `flask_htmx-0.3.0/PKG-INFO` & `flask_htmx-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-htmx
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Flask extension to work with HTMX.
 Home-page: https://github.com/edmondchuc/flask-htmx
 License: MIT
 Keywords: Flask,HTMX,Python,Web
 Author: Edmond Chuc
 Author-email: edmond.chuc@gmail.com
 Requires-Python: >=3.8,<4.0
```

