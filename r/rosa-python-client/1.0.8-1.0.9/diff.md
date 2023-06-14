# Comparing `tmp/rosa_python_client-1.0.8.tar.gz` & `tmp/rosa_python_client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosa_python_client-1.0.8.tar", max compression
+gzip compressed data, was "rosa_python_client-1.0.9.tar", max compression
```

## Comparing `rosa_python_client-1.0.8.tar` & `rosa_python_client-1.0.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      511 2023-06-08 08:13:24.162913 rosa_python_client-1.0.8/README.md
--rw-r--r--   0        0        0      353 2023-06-08 08:13:24.162913 rosa_python_client-1.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 08:13:24.162913 rosa_python_client-1.0.8/rosa/__init__.py
--rw-r--r--   0        0        0     6338 2023-06-08 08:13:24.162913 rosa_python_client-1.0.8/rosa/cli.py
--rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 rosa_python_client-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      511 2023-06-14 13:03:12.785023 rosa_python_client-1.0.9/README.md
+-rw-r--r--   0        0        0      353 2023-06-14 13:03:12.785023 rosa_python_client-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-14 13:03:12.785023 rosa_python_client-1.0.9/rosa/__init__.py
+-rw-r--r--   0        0        0     8586 2023-06-14 13:03:12.785023 rosa_python_client-1.0.9/rosa/cli.py
+-rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 rosa_python_client-1.0.9/PKG-INFO
```

### Comparing `rosa_python_client-1.0.8/PKG-INFO` & `rosa_python_client-1.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosa-python-client
-Version: 1.0.8
+Version: 1.0.9
 Summary: Wrapper for rosa cli
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

