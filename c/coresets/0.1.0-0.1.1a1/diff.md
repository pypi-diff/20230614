# Comparing `tmp/coresets-0.1.0.tar.gz` & `tmp/coresets-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coresets-0.1.0.tar", max compression
+gzip compressed data, was "coresets-0.1.1a1.tar", max compression
```

## Comparing `coresets-0.1.0.tar` & `coresets-0.1.1a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1543 2023-06-13 22:42:31.716106 coresets-0.1.0/LICENSE
--rw-r--r--   0        0        0      412 2023-06-14 03:18:28.353379 coresets-0.1.0/build.py
--rw-r--r--   0        0        0      237 2023-06-14 02:58:13.797126 coresets-0.1.0/coresets/__init__.py
--rw-r--r--   0        0        0      242 2023-06-14 02:59:58.624724 coresets-0.1.0/coresets/algorithms/__init__.py
--rw-r--r--   0        0        0     2744 2023-06-13 22:42:31.716106 coresets-0.1.0/coresets/algorithms/wbgm.py
--rw-r--r--   0        0        0     3030 2023-06-14 03:01:13.560452 coresets-0.1.0/coresets/algorithms/weighted_kmeans.py
--rw-r--r--   0        0        0     1983 2023-06-14 03:10:24.770712 coresets-0.1.0/coresets/algorithms/wgm.py
--rw-r--r--   0        0        0     1641 2023-06-14 02:58:23.057090 coresets-0.1.0/coresets/coreset.py
--rw-r--r--   0        0        0     4518 2023-06-14 03:05:17.211637 coresets-0.1.0/coresets/k_means_coreset.py
--rw-r--r--   0        0        0       49 2023-06-14 03:04:12.215845 coresets-0.1.0/coresets/utils/__init__.py
--rw-r--r--   0        0        0     1925 2023-06-13 22:42:31.720106 coresets-0.1.0/coresets/utils/datagen.py
--rw-r--r--   0        0        0    11467 2023-06-14 02:59:05.744923 coresets-0.1.0/coresets/utils/kmeans_init.py
--rw-r--r--   0        0        0     1488 2023-06-13 22:42:31.720106 coresets-0.1.0/coresets/utils/plotting.py
--rw-r--r--   0        0        0      823 2023-06-14 03:49:20.118951 coresets-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1266 2023-06-14 03:24:21.956449 coresets-0.1.0/readme.md
--rw-r--r--   0        0        0     1491 2023-06-14 03:02:10.768252 coresets-0.1.0/tests/test_k_means_coresets.py
--rw-r--r--   0        0        0      488 2023-06-14 03:02:38.968155 coresets-0.1.0/tests/test_mixtures.py
--rw-r--r--   0        0        0     1440 2023-06-14 03:19:15.257254 coresets-0.1.0/tests/test_sensitivity.py
--rw-r--r--   0        0        0     1141 2023-06-14 03:03:07.948057 coresets-0.1.0/tests/test_weighted_kmeans.py
--rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 coresets-0.1.0/setup.py
--rw-r--r--   0        0        0     2041 1970-01-01 00:00:00.000000 coresets-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1543 2023-06-13 22:42:31.716106 coresets-0.1.1a1/LICENSE
+-rw-r--r--   0        0        0      412 2023-06-14 03:18:28.353379 coresets-0.1.1a1/build.py
+-rw-r--r--   0        0        0      237 2023-06-14 02:58:13.797126 coresets-0.1.1a1/coresets/__init__.py
+-rw-r--r--   0        0        0      242 2023-06-14 02:59:58.624724 coresets-0.1.1a1/coresets/algorithms/__init__.py
+-rw-r--r--   0        0        0     2744 2023-06-13 22:42:31.716106 coresets-0.1.1a1/coresets/algorithms/wbgm.py
+-rw-r--r--   0        0        0     3030 2023-06-14 03:01:13.560452 coresets-0.1.1a1/coresets/algorithms/weighted_kmeans.py
+-rw-r--r--   0        0        0     1983 2023-06-14 03:10:24.770712 coresets-0.1.1a1/coresets/algorithms/wgm.py
+-rw-r--r--   0        0        0     1641 2023-06-14 02:58:23.057090 coresets-0.1.1a1/coresets/coreset.py
+-rw-r--r--   0        0        0     4518 2023-06-14 03:05:17.211637 coresets-0.1.1a1/coresets/k_means_coreset.py
+-rw-r--r--   0        0        0       49 2023-06-14 03:04:12.215845 coresets-0.1.1a1/coresets/utils/__init__.py
+-rw-r--r--   0        0        0     1925 2023-06-13 22:42:31.720106 coresets-0.1.1a1/coresets/utils/datagen.py
+-rw-r--r--   0        0        0    11467 2023-06-14 02:59:05.744923 coresets-0.1.1a1/coresets/utils/kmeans_init.py
+-rw-r--r--   0        0        0     1488 2023-06-13 22:42:31.720106 coresets-0.1.1a1/coresets/utils/plotting.py
+-rw-r--r--   0        0        0      795 2023-06-14 04:03:48.657942 coresets-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0     1266 2023-06-14 03:24:21.956449 coresets-0.1.1a1/readme.md
+-rw-r--r--   0        0        0     2817 2023-06-13 22:42:31.720106 coresets-0.1.1a1/src/sensitivity.cpp
+-rw-r--r--   0        0        0      339 2023-06-13 22:42:31.720106 coresets-0.1.1a1/src/sensitivity.h
+-rw-r--r--   0        0        0     3050 2023-06-13 22:42:31.720106 coresets-0.1.1a1/src/weighted_kmeans.cpp
+-rw-r--r--   0        0        0      504 2023-06-13 22:42:31.720106 coresets-0.1.1a1/src/weighted_kmeans.h
+-rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 coresets-0.1.1a1/setup.py
+-rw-r--r--   0        0        0     2043 1970-01-01 00:00:00.000000 coresets-0.1.1a1/PKG-INFO
```

### Comparing `coresets-0.1.0/LICENSE` & `coresets-0.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `coresets-0.1.0/coresets/algorithms/wbgm.py` & `coresets-0.1.1a1/coresets/algorithms/wbgm.py`

 * *Files identical despite different names*

### Comparing `coresets-0.1.0/coresets/algorithms/weighted_kmeans.py` & `coresets-0.1.1a1/coresets/algorithms/weighted_kmeans.py`

 * *Files identical despite different names*

### Comparing `coresets-0.1.0/coresets/algorithms/wgm.py` & `coresets-0.1.1a1/coresets/algorithms/wgm.py`

 * *Files identical despite different names*

### Comparing `coresets-0.1.0/coresets/coreset.py` & `coresets-0.1.1a1/coresets/coreset.py`

 * *Files identical despite different names*

### Comparing `coresets-0.1.0/coresets/k_means_coreset.py` & `coresets-0.1.1a1/coresets/k_means_coreset.py`

 * *Files identical despite different names*

### Comparing `coresets-0.1.0/coresets/utils/datagen.py` & `coresets-0.1.1a1/coresets/utils/datagen.py`

 * *Files identical despite different names*

### Comparing `coresets-0.1.0/coresets/utils/kmeans_init.py` & `coresets-0.1.1a1/coresets/utils/kmeans_init.py`

 * *Files identical despite different names*

### Comparing `coresets-0.1.0/coresets/utils/plotting.py` & `coresets-0.1.1a1/coresets/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `coresets-0.1.0/pyproject.toml` & `coresets-0.1.1a1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "coresets"
-version = "0.1.0"
+version = "0.1.1-alpha.1"
 description = "Coreset generation for k-Means and (Bayesian) Gaussian mixture models"
 authors = [
     "Zalán Borsos <zalan.borsos@inf.ethz.ch>",
     "Alexander Shtuchkin <ashtuchkin@gmail.com>"
 ]
 repository = "https://github.com/ashtuchkin/coresets"
 license = "BSD-3-Clause"
 readme = "readme.md"
-packages = [
-    { include = "coresets" },
-    { include = "tests", format = "sdist" },
+include = [
+    { path = "src", format = "sdist" },
 ]
 
 [tool.poetry.build]
 script = "build.py"
 generate-setup-file = true
 
 [tool.poetry.dependencies]
```

### Comparing `coresets-0.1.0/readme.md` & `coresets-0.1.1a1/readme.md`

 * *Files identical despite different names*

### Comparing `coresets-0.1.0/setup.py` & `coresets-0.1.1a1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['coresets', 'coresets.algorithms', 'coresets.utils', 'tests']
+['coresets', 'coresets.algorithms', 'coresets.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.14,<2.0', 'scikit-learn>=1.0,<2.0']
 
 setup_kwargs = {
     'name': 'coresets',
-    'version': '0.1.0',
+    'version': '0.1.1a1',
     'description': 'Coreset generation for k-Means and (Bayesian) Gaussian mixture models',
     'long_description': 'Coresets\n--------\nThis library contains the implementation coreset generation for k-Means and (Bayesian) Gaussian mixture models.\nIt also offers the extended versions of the corresponding algorithms that support weighted data sets.\n\nTo get started, take a look at:\n>examples/intro.ipynb\n\n(this is a fork of https://github.com/zalanborsos/coresets, intended to fix installation issues + publish to pypi)\n\nSetup\n-------\n1. Install [poetry](https://python-poetry.org/docs/).\n2.\n```shell\npoetry build\npoetry install\n```\n\nRunning tests\n-------------\nIn project root run:\n```shell\npoetry run pytest\n```\n\n\nReferences\n---------\nThe implementation of the library is based on the following works:\n>Bachem, O., Lucic, M., & Krause, A. (2017). Practical coreset constructions for machine learning. arXiv preprint arXiv:1703.06476.\n\n> Bachem, O., Lucic, M., & Krause, A. (2017). Scalable and distributed clustering via lightweight coresets. arXiv preprint arXiv:1702.08248.\n\n>Lucic, M., Faulkner, M., Krause, A., & Feldman, D. (2018). Training Gaussian Mixture Models at Scale via Coresets. Journal of Machine Learning Research, 18, Art-No.\n\n> Borsos, Z., Bachem, O., & Krause, A. Variational Inference for DPGMM with Coresets. (2017). Advances in Approximate Bayesian Inference\n',
     'author': 'Zalán Borsos',
     'author_email': 'zalan.borsos@inf.ethz.ch',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ashtuchkin/coresets',
```

### Comparing `coresets-0.1.0/PKG-INFO` & `coresets-0.1.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coresets
-Version: 0.1.0
+Version: 0.1.1a1
 Summary: Coreset generation for k-Means and (Bayesian) Gaussian mixture models
 Home-page: https://github.com/ashtuchkin/coresets
 License: BSD-3-Clause
 Author: Zalán Borsos
 Author-email: zalan.borsos@inf.ethz.ch
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

