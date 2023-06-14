# Comparing `tmp/cvxreg-0.1.4.tar.gz` & `tmp/cvxreg-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxreg-0.1.4.tar", last modified: Tue Jun 13 15:52:13 2023, max compression
+gzip compressed data, was "cvxreg-0.1.5.tar", last modified: Tue Jun 13 16:45:39 2023, max compression
```

## Comparing `cvxreg-0.1.4.tar` & `cvxreg-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:52:13.187606 cvxreg-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-13 15:52:01.000000 cvxreg-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-13 15:52:13.187606 cvxreg-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-13 15:52:01.000000 cvxreg-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:52:13.183606 cvxreg-0.1.4/cvxreg/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 15:52:01.000000 cvxreg-0.1.4/cvxreg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-13 15:52:01.000000 cvxreg-0.1.4/cvxreg/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-13 15:52:01.000000 cvxreg-0.1.4/cvxreg/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:52:13.187606 cvxreg-0.1.4/cvxreg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-13 15:52:01.000000 cvxreg-0.1.4/cvxreg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-13 15:52:01.000000 cvxreg-0.1.4/cvxreg/models/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-13 15:52:01.000000 cvxreg-0.1.4/cvxreg/models/_penalized.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:52:13.187606 cvxreg-0.1.4/cvxreg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-13 15:52:01.000000 cvxreg-0.1.4/cvxreg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-06-13 15:52:01.000000 cvxreg-0.1.4/cvxreg/utils/_param_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-13 15:52:01.000000 cvxreg-0.1.4/cvxreg/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-13 15:52:01.000000 cvxreg-0.1.4/cvxreg/utils/extmath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:52:13.183606 cvxreg-0.1.4/cvxreg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-13 15:52:13.000000 cvxreg-0.1.4/cvxreg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-13 15:52:13.000000 cvxreg-0.1.4/cvxreg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:52:13.000000 cvxreg-0.1.4/cvxreg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:52:12.000000 cvxreg-0.1.4/cvxreg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 15:52:13.000000 cvxreg-0.1.4/cvxreg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 15:52:13.000000 cvxreg-0.1.4/cvxreg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 15:52:13.187606 cvxreg-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-13 15:52:01.000000 cvxreg-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:45:39.842438 cvxreg-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-13 16:45:29.000000 cvxreg-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-13 16:45:39.842438 cvxreg-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-13 16:45:29.000000 cvxreg-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:45:39.838438 cvxreg-0.1.5/cvxreg/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-13 16:45:29.000000 cvxreg-0.1.5/cvxreg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-13 16:45:29.000000 cvxreg-0.1.5/cvxreg/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-13 16:45:29.000000 cvxreg-0.1.5/cvxreg/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:45:39.842438 cvxreg-0.1.5/cvxreg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-13 16:45:29.000000 cvxreg-0.1.5/cvxreg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-13 16:45:29.000000 cvxreg-0.1.5/cvxreg/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-13 16:45:29.000000 cvxreg-0.1.5/cvxreg/models/_cvxpy_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-13 16:45:29.000000 cvxreg-0.1.5/cvxreg/models/_penalized.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:45:39.842438 cvxreg-0.1.5/cvxreg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-13 16:45:29.000000 cvxreg-0.1.5/cvxreg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-06-13 16:45:29.000000 cvxreg-0.1.5/cvxreg/utils/_param_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-13 16:45:29.000000 cvxreg-0.1.5/cvxreg/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-13 16:45:29.000000 cvxreg-0.1.5/cvxreg/utils/extmath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:45:39.842438 cvxreg-0.1.5/cvxreg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-13 16:45:39.000000 cvxreg-0.1.5/cvxreg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-13 16:45:39.000000 cvxreg-0.1.5/cvxreg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:45:39.000000 cvxreg-0.1.5/cvxreg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:45:39.000000 cvxreg-0.1.5/cvxreg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 16:45:39.000000 cvxreg-0.1.5/cvxreg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 16:45:39.000000 cvxreg-0.1.5/cvxreg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:45:39.842438 cvxreg-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-13 16:45:29.000000 cvxreg-0.1.5/setup.py
```

### Comparing `cvxreg-0.1.4/LICENSE` & `cvxreg-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.4/PKG-INFO` & `cvxreg-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxreg
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python Package for Convex Regression
 Home-page: https://github.com/ConvexRegression/cvxreg
 Download-URL: https://pypi.org/project/cvxreg/
 Author: Zhiqiang Liao
 Author-email: zhiqiang.liao@aalto.fi
 License: MIT
 Keywords: ML,Prediction,Regression
```

### Comparing `cvxreg-0.1.4/README.md` & `cvxreg-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.4/cvxreg/base.py` & `cvxreg-0.1.5/cvxreg/base.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.4/cvxreg/models/_base.py` & `cvxreg-0.1.5/cvxreg/models/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # Author: Zhiqiang Liao @ Aalto University <zhiqiang.liao@aalto.fi>
 # License: MIT
 
 from abc import ABCMeta, abstractmethod
 import numpy as np
 from cvxpy import Variable, sum_squares
 
+from ._cvxpy_opt import solve_model
 from ..base import BaseEstimator
-from ..opt.cvxpy_opt import solve_model
 from ..constant import convex, concave
 from ..utils.extmath import yhat
 from ..utils._param_check import StrOptions
 from ..utils.check import check_ndarray
 
 def _calculate_matrix_A(n):
     res = np.zeros((n*(n-1), n))
```

### Comparing `cvxreg-0.1.4/cvxreg/models/_penalized.py` & `cvxreg-0.1.5/cvxreg/models/_penalized.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 # License: MIT
 
 from numbers import Real
 import numpy as np
 from cvxpy import Variable, sum_squares
 
 from ._base import CRModel, _calculate_matrix_A, _calculate_matrix_B, _shape_constraint
+from ._cvxpy_opt import solve_model
 from ..constant import convex, concave
-from ..opt.cvxpy_opt import solve_model
 from ..utils._param_check import Interval, StrOptions
 
 
 class PCR(CRModel):
     """
     Penalized Convex Regression (PCR) model.
```

### Comparing `cvxreg-0.1.4/cvxreg/utils/_param_check.py` & `cvxreg-0.1.5/cvxreg/utils/_param_check.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.4/cvxreg/utils/check.py` & `cvxreg-0.1.5/cvxreg/utils/check.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.4/cvxreg/utils/extmath.py` & `cvxreg-0.1.5/cvxreg/utils/extmath.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.4/cvxreg.egg-info/PKG-INFO` & `cvxreg-0.1.5/cvxreg.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxreg
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python Package for Convex Regression
 Home-page: https://github.com/ConvexRegression/cvxreg
 Download-URL: https://pypi.org/project/cvxreg/
 Author: Zhiqiang Liao
 Author-email: zhiqiang.liao@aalto.fi
 License: MIT
 Keywords: ML,Prediction,Regression
```

### Comparing `cvxreg-0.1.4/setup.py` & `cvxreg-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='cvxreg',
-    version='0.1.4',
+    version='0.1.5',
     description='A Python Package for Convex Regression',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Zhiqiang Liao',
     author_email='zhiqiang.liao@aalto.fi',
```

