# Comparing `tmp/filtro-0.1.0.tar.gz` & `tmp/filtro-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filtro-0.1.0.tar", max compression
+gzip compressed data, was "filtro-0.1.1.tar", max compression
```

## Comparing `filtro-0.1.0.tar` & `filtro-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1264 2023-06-14 07:34:49.810751 filtro-0.1.0/README.md
--rw-r--r--   0        0        0       35 2023-06-13 23:04:54.215294 filtro-0.1.0/filtro/__init__.py
--rw-r--r--   0        0        0      652 2023-06-14 07:20:21.528966 filtro-0.1.0/filtro/api_client.py
--rw-r--r--   0        0        0      340 2023-06-14 07:35:32.469218 filtro-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1665 1970-01-01 00:00:00.000000 filtro-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1264 2023-06-14 07:34:49.810751 filtro-0.1.1/README.md
+-rw-r--r--   0        0        0       35 2023-06-13 23:04:54.215294 filtro-0.1.1/filtro/__init__.py
+-rw-r--r--   0        0        0      652 2023-06-14 07:20:21.528966 filtro-0.1.1/filtro/api_client.py
+-rw-r--r--   0        0        0      339 2023-06-14 07:45:06.400431 filtro-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1765 1970-01-01 00:00:00.000000 filtro-0.1.1/PKG-INFO
```

### Comparing `filtro-0.1.0/README.md` & `filtro-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `filtro-0.1.0/filtro/api_client.py` & `filtro-0.1.1/filtro/api_client.py`

 * *Files identical despite different names*

### Comparing `filtro-0.1.0/PKG-INFO` & `filtro-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: filtro
-Version: 0.1.0
+Version: 0.1.1
 Summary: The official filtro python package.
 Author: Andrea Pinto
 Author-email: andrea@filtro.ai
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # filtro-python
```

