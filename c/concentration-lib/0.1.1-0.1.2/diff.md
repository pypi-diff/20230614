# Comparing `tmp/concentration_lib-0.1.1.tar.gz` & `tmp/concentration_lib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/sauxpa/github/concentration_lib/dist/tmp50m_3yls/concentration_lib-0.1.1.tar", last modified: Wed Nov 10 14:58:53 2021, max compression
+gzip compressed data, was "/home/sauxpa/github/concentration_lib/dist/tmpa0raq4zh/concentration_lib-0.1.2.tar", last modified: Mon Nov 15 23:25:38 2021, max compression
```

## Comparing `concentration_lib-0.1.1.tar` & `concentration_lib-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 sauxpa    (1000) sauxpa    (1000)        0 2021-11-10 14:58:53.000000 concentration_lib-0.1.1/
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)    35149 2021-07-20 14:53:20.000000 concentration_lib-0.1.1/LICENSE
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)      885 2021-11-10 14:58:53.000000 concentration_lib-0.1.1/PKG-INFO
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)      546 2021-11-10 14:55:27.000000 concentration_lib-0.1.1/README.md
-drwxrwxr-x   0 sauxpa    (1000) sauxpa    (1000)        0 2021-11-10 14:58:53.000000 concentration_lib-0.1.1/concentration_lib/
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)      196 2021-11-10 14:36:42.000000 concentration_lib-0.1.1/concentration_lib/__init__.py
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)    13576 2021-11-10 13:46:44.000000 concentration_lib-0.1.1/concentration_lib/concentration_bounds.py
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)    14044 2021-11-10 14:13:50.000000 concentration_lib-0.1.1/concentration_lib/concentration_variance_bounds.py
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)    14500 2021-11-10 14:38:43.000000 concentration_lib-0.1.1/concentration_lib/empirical_concentration_bounds.py
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)     9256 2021-10-12 12:50:09.000000 concentration_lib-0.1.1/concentration_lib/helper_ptlm.py
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)    11438 2021-10-13 21:55:30.000000 concentration_lib-0.1.1/concentration_lib/utils.py
-drwxrwxr-x   0 sauxpa    (1000) sauxpa    (1000)        0 2021-11-10 14:58:53.000000 concentration_lib-0.1.1/concentration_lib.egg-info/
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)      885 2021-11-10 14:58:53.000000 concentration_lib-0.1.1/concentration_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)      465 2021-11-10 14:58:53.000000 concentration_lib-0.1.1/concentration_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)        1 2021-11-10 14:58:53.000000 concentration_lib-0.1.1/concentration_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)       12 2021-11-10 14:58:53.000000 concentration_lib-0.1.1/concentration_lib.egg-info/requires.txt
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)       18 2021-11-10 14:58:53.000000 concentration_lib-0.1.1/concentration_lib.egg-info/top_level.txt
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)       38 2021-11-10 14:58:53.000000 concentration_lib-0.1.1/setup.cfg
--rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)      532 2021-11-10 14:56:26.000000 concentration_lib-0.1.1/setup.py
+drwxrwxr-x   0 sauxpa    (1000) sauxpa    (1000)        0 2021-11-15 23:25:38.000000 concentration_lib-0.1.2/
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)    35149 2021-07-20 14:53:20.000000 concentration_lib-0.1.2/LICENSE
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)      885 2021-11-15 23:25:38.000000 concentration_lib-0.1.2/PKG-INFO
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)      546 2021-11-10 14:55:27.000000 concentration_lib-0.1.2/README.md
+drwxrwxr-x   0 sauxpa    (1000) sauxpa    (1000)        0 2021-11-15 23:25:38.000000 concentration_lib-0.1.2/concentration_lib/
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)      196 2021-11-10 14:36:42.000000 concentration_lib-0.1.2/concentration_lib/__init__.py
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)    13576 2021-11-10 13:46:44.000000 concentration_lib-0.1.2/concentration_lib/concentration_bounds.py
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)    14044 2021-11-10 14:13:50.000000 concentration_lib-0.1.2/concentration_lib/concentration_variance_bounds.py
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)    14500 2021-11-10 14:38:43.000000 concentration_lib-0.1.2/concentration_lib/empirical_concentration_bounds.py
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)     9256 2021-10-12 12:50:09.000000 concentration_lib-0.1.2/concentration_lib/helper_ptlm.py
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)    10531 2021-11-15 23:23:18.000000 concentration_lib-0.1.2/concentration_lib/utils.py
+drwxrwxr-x   0 sauxpa    (1000) sauxpa    (1000)        0 2021-11-15 23:25:38.000000 concentration_lib-0.1.2/concentration_lib.egg-info/
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)      885 2021-11-15 23:25:38.000000 concentration_lib-0.1.2/concentration_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)      465 2021-11-15 23:25:38.000000 concentration_lib-0.1.2/concentration_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)        1 2021-11-15 23:25:38.000000 concentration_lib-0.1.2/concentration_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)       12 2021-11-15 23:25:38.000000 concentration_lib-0.1.2/concentration_lib.egg-info/requires.txt
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)       18 2021-11-15 23:25:38.000000 concentration_lib-0.1.2/concentration_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)       38 2021-11-15 23:25:38.000000 concentration_lib-0.1.2/setup.cfg
+-rw-rw-r--   0 sauxpa    (1000) sauxpa    (1000)      532 2021-11-15 23:25:11.000000 concentration_lib-0.1.2/setup.py
```

### Comparing `concentration_lib-0.1.1/LICENSE` & `concentration_lib-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `concentration_lib-0.1.1/PKG-INFO` & `concentration_lib-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concentration_lib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library for concentration bounds
 Home-page: https://github.com/sauxpa/concentration_lib
 Author: Patrick Saux
 Author-email: patrick.saux@ginria.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `concentration_lib-0.1.1/README.md` & `concentration_lib-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `concentration_lib-0.1.1/concentration_lib/concentration_bounds.py` & `concentration_lib-0.1.2/concentration_lib/concentration_bounds.py`

 * *Files identical despite different names*

### Comparing `concentration_lib-0.1.1/concentration_lib/concentration_variance_bounds.py` & `concentration_lib-0.1.2/concentration_lib/concentration_variance_bounds.py`

 * *Files identical despite different names*

### Comparing `concentration_lib-0.1.1/concentration_lib/empirical_concentration_bounds.py` & `concentration_lib-0.1.2/concentration_lib/empirical_concentration_bounds.py`

 * *Files identical despite different names*

### Comparing `concentration_lib-0.1.1/concentration_lib/helper_ptlm.py` & `concentration_lib-0.1.2/concentration_lib/helper_ptlm.py`

 * *Files identical despite different names*

### Comparing `concentration_lib-0.1.1/concentration_lib/utils.py` & `concentration_lib-0.1.2/concentration_lib/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Utility function to help handle various modes (concentration of sum or mean,
 one or two sided bounds...)
 """
 
 # Author: Patrick Saux <patrick.saux@inria.fr>
 
 import numpy as np
-import pandas as pd
 from typing import Callable, List, Union
 from scipy.optimize import root_scalar as root_scalar_scipy
 from scipy.optimize.zeros import RootResults
 
 
 def check_mode(mode: str):
     assert mode in {'sum', 'mean'}, 'Unknown mode {:s}'.format(mode)
@@ -348,33 +347,7 @@
             bound_mean = np.nan
     else:
         bound_mean = np.nan
 
     return return_bound(
         n, bound_mean, side, 'mean', mode
         )
-
-
-def intersection_uniform_bound(bounds: List[float], side='lower'):
-    """Compute the running intersection of time-uniform confidence intervals.
-
-    bounds: List
-    Dimensions are assumed to be (N,) or (N, M) if side == 'lower' or
-    side == 'upper' and (2, N,) or (2, N, M) is side == 'both',
-    where N is the number of observations and M the number of replicates
-    (in case of MC simulations).
-    """
-    check_side(side)
-
-    if side == 'lower':
-        return pd.DataFrame(bounds).cummax(axis=0).values
-    elif side == 'upper':
-        return pd.DataFrame(bounds).cummin(axis=0).values
-    else:
-        N, M = bounds.shape[1:]
-        return np.concatenate(
-            [
-                pd.Series(bounds[0]).cummax(axis=0).values.reshape(1, N, M),
-                pd.Series(bounds[1]).cummin(axis=0).values.reshape(1, N, M),
-            ],
-            axis=0,
-        )
```

### Comparing `concentration_lib-0.1.1/concentration_lib.egg-info/PKG-INFO` & `concentration_lib-0.1.2/concentration_lib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concentration-lib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library for concentration bounds
 Home-page: https://github.com/sauxpa/concentration_lib
 Author: Patrick Saux
 Author-email: patrick.saux@ginria.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `concentration_lib-0.1.1/setup.py` & `concentration_lib-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='concentration_lib',
     packages=['concentration_lib'],
-    version='0.1.1',
+    version='0.1.2',
     author="Patrick Saux",
     author_email="patrick.saux@ginria.fr",
     description="Library for concentration bounds",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sauxpa/concentration_lib",
     install_requires=['numpy', 'scipy'],
```

