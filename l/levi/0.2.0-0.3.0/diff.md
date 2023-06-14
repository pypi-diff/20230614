# Comparing `tmp/levi-0.2.0.tar.gz` & `tmp/levi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "levi-0.2.0.tar", max compression
+gzip compressed data, was "levi-0.3.0.tar", max compression
```

## Comparing `levi-0.2.0.tar` & `levi-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1070 2023-03-06 15:12:43.834601 levi-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     1909 2023-05-17 11:56:45.930406 levi-0.2.0/README.md
--rw-r--r--   0        0        0     3213 2023-05-17 11:56:45.930577 levi-0.2.0/levi/__init__.py
--rw-r--r--   0        0        0      422 2023-05-17 11:56:45.930946 levi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2379 1970-01-01 00:00:00.000000 levi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-06 15:12:43.834601 levi-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     1909 2023-05-17 11:56:45.930406 levi-0.3.0/README.md
+-rw-r--r--   0        0        0     3213 2023-05-17 11:56:45.930577 levi-0.3.0/levi/__init__.py
+-rw-r--r--   0        0        0      420 2023-06-14 17:46:31.289245 levi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2375 1970-01-01 00:00:00.000000 levi-0.3.0/PKG-INFO
```

### Comparing `levi-0.2.0/LICENSE.md` & `levi-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `levi-0.2.0/README.md` & `levi-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `levi-0.2.0/levi/__init__.py` & `levi-0.3.0/levi/__init__.py`

 * *Files identical despite different names*

### Comparing `levi-0.2.0/PKG-INFO` & `levi-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: levi
-Version: 0.2.0
+Version: 0.3.0
 Summary: Delta Lake helper methods
 Author: Matthew Powers
 Author-email: matthewkevinpowers@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: deltalake[pandas] (>=0.9.0,<0.10.0)
+Requires-Dist: deltalake[pandas] (>=0.9,<0.10)
 Description-Content-Type: text/markdown
 
 # Levi
 
 Delta Lake helper methods.  No Spark dependency.
 
 ## Installation
```

