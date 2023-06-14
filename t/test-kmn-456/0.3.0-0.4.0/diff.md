# Comparing `tmp/test_kmn_456-0.3.0.tar.gz` & `tmp/test_kmn_456-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_kmn_456-0.3.0.tar", last modified: Wed Jun 14 20:46:28 2023, max compression
+gzip compressed data, was "test_kmn_456-0.4.0.tar", last modified: Wed Jun 14 20:59:52 2023, max compression
```

## Comparing `test_kmn_456-0.3.0.tar` & `test_kmn_456-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:46:28.477002 test_kmn_456-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 20:46:10.000000 test_kmn_456-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-14 20:46:28.477002 test_kmn_456-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-14 20:46:10.000000 test_kmn_456-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-14 20:46:10.000000 test_kmn_456-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 20:46:28.477002 test_kmn_456-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:46:28.473001 test_kmn_456-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:46:28.477002 test_kmn_456-0.3.0/src/test_kmn_456/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:46:10.000000 test_kmn_456-0.3.0/src/test_kmn_456/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-14 20:46:10.000000 test_kmn_456-0.3.0/src/test_kmn_456/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:46:28.477002 test_kmn_456-0.3.0/src/test_kmn_456.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-14 20:46:28.000000 test_kmn_456-0.3.0/src/test_kmn_456.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-14 20:46:28.000000 test_kmn_456-0.3.0/src/test_kmn_456.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:46:28.000000 test_kmn_456-0.3.0/src/test_kmn_456.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 20:46:28.000000 test_kmn_456-0.3.0/src/test_kmn_456.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:59:52.868019 test_kmn_456-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 20:59:36.000000 test_kmn_456-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-14 20:59:52.868019 test_kmn_456-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-14 20:59:36.000000 test_kmn_456-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-14 20:59:36.000000 test_kmn_456-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 20:59:52.868019 test_kmn_456-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:59:52.864019 test_kmn_456-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:59:52.864019 test_kmn_456-0.4.0/src/test_kmn_456/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:59:36.000000 test_kmn_456-0.4.0/src/test_kmn_456/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-14 20:59:36.000000 test_kmn_456-0.4.0/src/test_kmn_456/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:59:52.868019 test_kmn_456-0.4.0/src/test_kmn_456.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-14 20:59:52.000000 test_kmn_456-0.4.0/src/test_kmn_456.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-14 20:59:52.000000 test_kmn_456-0.4.0/src/test_kmn_456.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:59:52.000000 test_kmn_456-0.4.0/src/test_kmn_456.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 20:59:52.000000 test_kmn_456-0.4.0/src/test_kmn_456.egg-info/top_level.txt
```

### Comparing `test_kmn_456-0.3.0/LICENSE` & `test_kmn_456-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `test_kmn_456-0.3.0/PKG-INFO` & `test_kmn_456-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_kmn_456
-Version: 0.3.0
+Version: 0.4.0
 Summary: A small test example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `test_kmn_456-0.3.0/README.md` & `test_kmn_456-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `test_kmn_456-0.3.0/pyproject.toml` & `test_kmn_456-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "test_kmn_456"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small test example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `test_kmn_456-0.3.0/src/test_kmn_456.egg-info/PKG-INFO` & `test_kmn_456-0.4.0/src/test_kmn_456.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-kmn-456
-Version: 0.3.0
+Version: 0.4.0
 Summary: A small test example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

