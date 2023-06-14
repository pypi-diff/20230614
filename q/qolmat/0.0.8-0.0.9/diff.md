# Comparing `tmp/qolmat-0.0.8.tar.gz` & `tmp/qolmat-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qolmat-0.0.8.tar", last modified: Wed Mar  8 11:46:39 2023, max compression
+gzip compressed data, was "qolmat-0.0.9.tar", last modified: Wed Mar  8 12:02:03 2023, max compression
```

## Comparing `qolmat-0.0.8.tar` & `qolmat-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 11:46:39.515900 qolmat-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-03-08 11:46:39.515900 qolmat-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-03-08 11:46:31.000000 qolmat-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 11:46:39.515900 qolmat-0.0.8/qolmat/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-08 11:46:31.000000 qolmat-0.0.8/qolmat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-08 11:46:31.000000 qolmat-0.0.8/qolmat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 11:46:39.515900 qolmat-0.0.8/qolmat/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 11:46:31.000000 qolmat-0.0.8/qolmat/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-03-08 11:46:31.000000 qolmat-0.0.8/qolmat/tests/test_benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-03-08 11:46:31.000000 qolmat-0.0.8/qolmat/tests/test_em_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-03-08 11:46:31.000000 qolmat-0.0.8/qolmat/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-03-08 11:46:31.000000 qolmat-0.0.8/qolmat/tests/test_rpca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-03-08 11:46:31.000000 qolmat-0.0.8/qolmat/tests/test_rpca_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 11:46:39.515900 qolmat-0.0.8/qolmat/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 11:46:31.000000 qolmat-0.0.8/qolmat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-03-08 11:46:31.000000 qolmat-0.0.8/qolmat/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-03-08 11:46:31.000000 qolmat-0.0.8/qolmat/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-03-08 11:46:31.000000 qolmat-0.0.8/qolmat/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 11:46:39.515900 qolmat-0.0.8/qolmat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-03-08 11:46:39.000000 qolmat-0.0.8/qolmat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-08 11:46:39.000000 qolmat-0.0.8/qolmat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 11:46:39.000000 qolmat-0.0.8/qolmat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 11:46:39.000000 qolmat-0.0.8/qolmat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-08 11:46:39.000000 qolmat-0.0.8/qolmat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-08 11:46:39.000000 qolmat-0.0.8/qolmat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 11:46:39.515900 qolmat-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-03-08 11:46:31.000000 qolmat-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:02:03.080152 qolmat-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-03-08 12:02:03.080152 qolmat-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-03-08 12:01:54.000000 qolmat-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:02:03.080152 qolmat-0.0.9/qolmat/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-08 12:01:54.000000 qolmat-0.0.9/qolmat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-08 12:01:54.000000 qolmat-0.0.9/qolmat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:02:03.080152 qolmat-0.0.9/qolmat/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 12:01:54.000000 qolmat-0.0.9/qolmat/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-03-08 12:01:54.000000 qolmat-0.0.9/qolmat/tests/test_benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-03-08 12:01:54.000000 qolmat-0.0.9/qolmat/tests/test_em_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-03-08 12:01:54.000000 qolmat-0.0.9/qolmat/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-03-08 12:01:54.000000 qolmat-0.0.9/qolmat/tests/test_rpca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-03-08 12:01:54.000000 qolmat-0.0.9/qolmat/tests/test_rpca_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:02:03.080152 qolmat-0.0.9/qolmat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 12:01:54.000000 qolmat-0.0.9/qolmat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-03-08 12:01:54.000000 qolmat-0.0.9/qolmat/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-03-08 12:01:54.000000 qolmat-0.0.9/qolmat/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-03-08 12:01:54.000000 qolmat-0.0.9/qolmat/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:02:03.080152 qolmat-0.0.9/qolmat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-03-08 12:02:03.000000 qolmat-0.0.9/qolmat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-08 12:02:03.000000 qolmat-0.0.9/qolmat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 12:02:03.000000 qolmat-0.0.9/qolmat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 12:02:03.000000 qolmat-0.0.9/qolmat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-08 12:02:03.000000 qolmat-0.0.9/qolmat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-08 12:02:03.000000 qolmat-0.0.9/qolmat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 12:02:03.080152 qolmat-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-03-08 12:01:54.000000 qolmat-0.0.9/setup.py
```

### Comparing `qolmat-0.0.8/PKG-INFO` & `qolmat-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qolmat
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools to impute
 Author: Hong-Lan Botterman, Julien Roussel, Thomas Morzadec, Rima Hajou, Firas Dakhli
 Author-email: 
 hlbotterman@quantmetry.com,
 jroussel@quantmetry.com,
 tmorzadec@quantmetry.com,
 rhajou@quantmetry.com,
```

### Comparing `qolmat-0.0.8/README.rst` & `qolmat-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `qolmat-0.0.8/qolmat/tests/test_benchmark_utils.py` & `qolmat-0.0.9/qolmat/tests/test_benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `qolmat-0.0.8/qolmat/tests/test_em_sampler.py` & `qolmat-0.0.9/qolmat/tests/test_em_sampler.py`

 * *Files identical despite different names*

### Comparing `qolmat-0.0.8/qolmat/tests/test_models.py` & `qolmat-0.0.9/qolmat/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `qolmat-0.0.8/qolmat/tests/test_rpca.py` & `qolmat-0.0.9/qolmat/tests/test_rpca.py`

 * *Files identical despite different names*

### Comparing `qolmat-0.0.8/qolmat/tests/test_rpca_utils.py` & `qolmat-0.0.9/qolmat/tests/test_rpca_utils.py`

 * *Files identical despite different names*

### Comparing `qolmat-0.0.8/qolmat/utils/data.py` & `qolmat-0.0.9/qolmat/utils/data.py`

 * *Files identical despite different names*

### Comparing `qolmat-0.0.8/qolmat/utils/plot.py` & `qolmat-0.0.9/qolmat/utils/plot.py`

 * *Files identical despite different names*

### Comparing `qolmat-0.0.8/qolmat/utils/utils.py` & `qolmat-0.0.9/qolmat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qolmat-0.0.8/qolmat.egg-info/PKG-INFO` & `qolmat-0.0.9/qolmat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qolmat
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools to impute
 Author: Hong-Lan Botterman, Julien Roussel, Thomas Morzadec, Rima Hajou, Firas Dakhli
 Author-email: 
 hlbotterman@quantmetry.com,
 jroussel@quantmetry.com,
 tmorzadec@quantmetry.com,
 rhajou@quantmetry.com,
```

### Comparing `qolmat-0.0.8/setup.py` & `qolmat-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import codecs
 
 from setuptools import find_packages, setup
 
 DISTNAME = "qolmat"
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 DESCRIPTION = "Tools to impute"
 LONG_DESCRIPTION_CONTENT_TYPE = "text/x-rst"
 with codecs.open("README.rst", encoding="utf-8-sig") as f:
     LONG_DESCRIPTION = f.read()
 
 # """
 # Here we should add the correct
```

