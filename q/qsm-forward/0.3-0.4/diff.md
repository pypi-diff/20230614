# Comparing `tmp/qsm-forward-0.3.tar.gz` & `tmp/qsm-forward-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsm-forward-0.3.tar", last modified: Wed Jun 14 05:04:17 2023, max compression
+gzip compressed data, was "qsm-forward-0.4.tar", last modified: Wed Jun 14 05:55:46 2023, max compression
```

## Comparing `qsm-forward-0.3.tar` & `qsm-forward-0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 05:04:17.058063 qsm-forward-0.3/
--rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm-forward-0.3/LICENSE
--rw-r--r--   0 ashley    (1000) ashley    (1000)     1342 2023-06-14 05:04:17.058063 qsm-forward-0.3/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)      571 2023-06-12 04:37:47.000000 qsm-forward-0.3/README.md
--rw-r--r--   0 ashley    (1000) ashley    (1000)      750 2023-06-14 05:03:17.000000 qsm-forward-0.3/pyproject.toml
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 05:04:17.054729 qsm-forward-0.3/qsm_forward/
--rw-r--r--   0 ashley    (1000) ashley    (1000)      339 2023-06-14 04:21:57.000000 qsm-forward-0.3/qsm_forward/__init__.py
--rw-r--r--   0 ashley    (1000) ashley    (1000)    12190 2023-06-14 04:59:40.000000 qsm-forward-0.3/qsm_forward/qsm_forward.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 05:04:17.054729 qsm-forward-0.3/qsm_forward.egg-info/
--rw-r--r--   0 ashley    (1000) ashley    (1000)     1342 2023-06-14 05:04:17.000000 qsm-forward-0.3/qsm_forward.egg-info/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)      292 2023-06-14 05:04:17.000000 qsm-forward-0.3/qsm_forward.egg-info/SOURCES.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-14 05:04:17.000000 qsm-forward-0.3/qsm_forward.egg-info/dependency_links.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       19 2023-06-14 05:04:17.000000 qsm-forward-0.3/qsm_forward.egg-info/requires.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-14 05:04:17.000000 qsm-forward-0.3/qsm_forward.egg-info/top_level.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-14 05:04:17.058063 qsm-forward-0.3/setup.cfg
--rw-r--r--   0 ashley    (1000) ashley    (1000)      812 2023-06-14 05:03:22.000000 qsm-forward-0.3/setup.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 05:04:17.054729 qsm-forward-0.3/tests/
--rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm-forward-0.3/tests/test_qsm_forward.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 05:55:46.437987 qsm-forward-0.4/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm-forward-0.4/LICENSE
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     1342 2023-06-14 05:55:46.437987 qsm-forward-0.4/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      571 2023-06-12 04:37:47.000000 qsm-forward-0.4/README.md
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      750 2023-06-14 05:55:09.000000 qsm-forward-0.4/pyproject.toml
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 05:55:46.437987 qsm-forward-0.4/qsm_forward/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      465 2023-06-14 05:36:03.000000 qsm-forward-0.4/qsm_forward/__init__.py
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    19256 2023-06-14 05:34:06.000000 qsm-forward-0.4/qsm_forward/qsm_forward.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 05:55:46.437987 qsm-forward-0.4/qsm_forward.egg-info/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     1342 2023-06-14 05:55:46.000000 qsm-forward-0.4/qsm_forward.egg-info/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      292 2023-06-14 05:55:46.000000 qsm-forward-0.4/qsm_forward.egg-info/SOURCES.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-14 05:55:46.000000 qsm-forward-0.4/qsm_forward.egg-info/dependency_links.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       19 2023-06-14 05:55:46.000000 qsm-forward-0.4/qsm_forward.egg-info/requires.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-14 05:55:46.000000 qsm-forward-0.4/qsm_forward.egg-info/top_level.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-14 05:55:46.437987 qsm-forward-0.4/setup.cfg
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      812 2023-06-14 05:36:21.000000 qsm-forward-0.4/setup.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 05:55:46.437987 qsm-forward-0.4/tests/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm-forward-0.4/tests/test_qsm_forward.py
```

### Comparing `qsm-forward-0.3/LICENSE` & `qsm-forward-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qsm-forward-0.3/PKG-INFO` & `qsm-forward-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsm-forward
-Version: 0.3
+Version: 0.4
 Summary: A forward-model simulation for Quantitative Susceptibility Mapping
 Home-page: https://github.com/astewartau/qsm-forward-model
 Author: Ashley Stewart
 Author-email: Ashley Stewart <a.stewart.au@gmail.com>
 Project-URL: Homepage, https://github.com/astewartau/qsm-forward-model
 Project-URL: Bug Tracker, https://github.com/astewartau/qsm-forward-model/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qsm-forward-0.3/README.md` & `qsm-forward-0.4/README.md`

 * *Files identical despite different names*

### Comparing `qsm-forward-0.3/pyproject.toml` & `qsm-forward-0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qsm-forward"
-version = "0.3"
+version = "0.4"
 authors = [
   { name="Ashley Stewart", email="a.stewart.au@gmail.com" },
 ]
 description = "A forward-model simulation for Quantitative Susceptibility Mapping"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
```

### Comparing `qsm-forward-0.3/qsm_forward.egg-info/PKG-INFO` & `qsm-forward-0.4/qsm_forward.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsm-forward
-Version: 0.3
+Version: 0.4
 Summary: A forward-model simulation for Quantitative Susceptibility Mapping
 Home-page: https://github.com/astewartau/qsm-forward-model
 Author: Ashley Stewart
 Author-email: Ashley Stewart <a.stewart.au@gmail.com>
 Project-URL: Homepage, https://github.com/astewartau/qsm-forward-model
 Project-URL: Bug Tracker, https://github.com/astewartau/qsm-forward-model/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qsm-forward-0.3/setup.py` & `qsm-forward-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='qsm-forward',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     url='https://github.com/astewartau/qsm-forward-model',
     author='Ashley Stewart',
     author_email='a.stewart.au@gmail.com',
     description='A forward-model simulation for Quantitative Susceptibility Mapping',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

