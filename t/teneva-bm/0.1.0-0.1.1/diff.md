# Comparing `tmp/teneva_bm-0.1.0.tar.gz` & `tmp/teneva_bm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teneva_bm-0.1.0.tar", last modified: Wed Apr 26 18:38:41 2023, max compression
+gzip compressed data, was "teneva_bm-0.1.1.tar", last modified: Tue Jun 13 08:14:35 2023, max compression
```

## Comparing `teneva_bm-0.1.0.tar` & `teneva_bm-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-04-26 18:38:41.722859 teneva_bm-0.1.0/
--rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.1.0/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       54 2023-04-26 09:54:29.000000 teneva_bm-0.1.0/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)     3733 2023-04-26 18:38:41.722996 teneva_bm-0.1.0/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     2431 2023-04-26 18:38:14.000000 teneva_bm-0.1.0/README.md
--rw-r--r--   0 andrei     (501) staff       (20)      823 2023-04-26 15:12:44.000000 teneva_bm-0.1.0/demo.py
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-04-26 18:38:41.723481 teneva_bm-0.1.0/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2556 2023-04-26 15:12:02.000000 teneva_bm-0.1.0/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-04-26 18:38:41.720978 teneva_bm-0.1.0/teneva_bm/
--rw-r--r--   0 andrei     (501) staff       (20)      921 2023-04-26 18:38:09.000000 teneva_bm-0.1.0/teneva_bm/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7346 2023-04-26 18:37:08.000000 teneva_bm-0.1.0/teneva_bm/bm.py
--rw-r--r--   0 andrei     (501) staff       (20)     2988 2023-04-26 18:32:42.000000 teneva_bm-0.1.0/teneva_bm/bm_func_ackley.py
--rw-r--r--   0 andrei     (501) staff       (20)     2338 2023-04-26 18:36:21.000000 teneva_bm-0.1.0/teneva_bm/bm_func_alpine.py
--rw-r--r--   0 andrei     (501) staff       (20)     2421 2023-04-26 18:33:04.000000 teneva_bm-0.1.0/teneva_bm/bm_func_dixon.py
--rw-r--r--   0 andrei     (501) staff       (20)     2333 2023-04-26 18:36:30.000000 teneva_bm-0.1.0/teneva_bm/bm_func_exp.py
--rw-r--r--   0 andrei     (501) staff       (20)     2778 2023-04-26 18:36:34.000000 teneva_bm-0.1.0/teneva_bm/bm_func_griewank.py
--rw-r--r--   0 andrei     (501) staff       (20)     3007 2023-04-26 18:36:39.000000 teneva_bm-0.1.0/teneva_bm/bm_func_michalewicz.py
--rw-r--r--   0 andrei     (501) staff       (20)     2462 2023-04-26 17:51:04.000000 teneva_bm-0.1.0/teneva_bm/bm_func_piston.py
--rw-r--r--   0 andrei     (501) staff       (20)     2374 2023-04-26 18:36:44.000000 teneva_bm-0.1.0/teneva_bm/bm_func_qing.py
--rw-r--r--   0 andrei     (501) staff       (20)     2763 2023-04-26 18:36:49.000000 teneva_bm-0.1.0/teneva_bm/bm_func_rastrigin.py
--rw-r--r--   0 andrei     (501) staff       (20)     3077 2023-04-26 18:36:52.000000 teneva_bm-0.1.0/teneva_bm/bm_func_rosenbrock.py
--rw-r--r--   0 andrei     (501) staff       (20)     2192 2023-04-26 18:33:36.000000 teneva_bm-0.1.0/teneva_bm/bm_func_schaffer.py
--rw-r--r--   0 andrei     (501) staff       (20)     2702 2023-04-26 18:36:59.000000 teneva_bm-0.1.0/teneva_bm/bm_func_schwefel.py
--rw-r--r--   0 andrei     (501) staff       (20)     4986 2023-04-26 18:32:24.000000 teneva_bm-0.1.0/teneva_bm/bm_matmul2.py
--rw-r--r--   0 andrei     (501) staff       (20)     3127 2023-04-26 18:18:14.000000 teneva_bm-0.1.0/teneva_bm/bm_oc_simple.py
--rw-r--r--   0 andrei     (501) staff       (20)     1702 2023-04-26 18:18:05.000000 teneva_bm-0.1.0/teneva_bm/bm_oc_simple_constr.py
--rw-r--r--   0 andrei     (501) staff       (20)     2902 2023-04-26 18:33:58.000000 teneva_bm-0.1.0/teneva_bm/bm_qubo_knap_amba.py
--rw-r--r--   0 andrei     (501) staff       (20)     1883 2023-04-26 18:14:29.000000 teneva_bm-0.1.0/teneva_bm/bm_qubo_knap_quad.py
--rw-r--r--   0 andrei     (501) staff       (20)     2578 2023-04-26 18:14:02.000000 teneva_bm-0.1.0/teneva_bm/bm_qubo_maxcut.py
--rw-r--r--   0 andrei     (501) staff       (20)     2584 2023-04-26 18:13:28.000000 teneva_bm-0.1.0/teneva_bm/bm_qubo_mvc.py
--rw-r--r--   0 andrei     (501) staff       (20)    11307 2023-04-26 18:12:04.000000 teneva_bm-0.1.0/teneva_bm/bm_topopt.py
--rw-r--r--   0 andrei     (501) staff       (20)     1699 2023-04-26 18:34:12.000000 teneva_bm-0.1.0/teneva_bm/bm_wall_simple.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-04-26 18:38:41.722596 teneva_bm-0.1.0/teneva_bm.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)     3733 2023-04-26 18:38:41.000000 teneva_bm-0.1.0/teneva_bm.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)      859 2023-04-26 18:38:41.000000 teneva_bm-0.1.0/teneva_bm.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-04-26 18:38:41.000000 teneva_bm-0.1.0/teneva_bm.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)       33 2023-04-26 18:38:41.000000 teneva_bm-0.1.0/teneva_bm.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)       10 2023-04-26 18:38:41.000000 teneva_bm-0.1.0/teneva_bm.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 08:14:35.733312 teneva_bm-0.1.1/
+-rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.1.1/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       54 2023-04-26 09:54:29.000000 teneva_bm-0.1.1/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)     3733 2023-06-13 08:14:35.733522 teneva_bm-0.1.1/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     2431 2023-06-13 08:14:05.000000 teneva_bm-0.1.1/README.md
+-rw-r--r--   0 andrei     (501) staff       (20)      978 2023-06-13 08:10:16.000000 teneva_bm-0.1.1/demo.py
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-06-13 08:14:35.734213 teneva_bm-0.1.1/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2556 2023-04-26 15:12:02.000000 teneva_bm-0.1.1/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 08:14:35.730793 teneva_bm-0.1.1/teneva_bm/
+-rw-r--r--   0 andrei     (501) staff       (20)      919 2023-06-13 08:13:52.000000 teneva_bm-0.1.1/teneva_bm/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7346 2023-04-26 18:37:08.000000 teneva_bm-0.1.1/teneva_bm/bm.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2988 2023-04-26 18:32:42.000000 teneva_bm-0.1.1/teneva_bm/bm_func_ackley.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2338 2023-04-26 18:36:21.000000 teneva_bm-0.1.1/teneva_bm/bm_func_alpine.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2421 2023-04-26 18:33:04.000000 teneva_bm-0.1.1/teneva_bm/bm_func_dixon.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2333 2023-04-26 18:36:30.000000 teneva_bm-0.1.1/teneva_bm/bm_func_exp.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2778 2023-04-26 18:36:34.000000 teneva_bm-0.1.1/teneva_bm/bm_func_griewank.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3007 2023-04-26 18:36:39.000000 teneva_bm-0.1.1/teneva_bm/bm_func_michalewicz.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2462 2023-04-26 17:51:04.000000 teneva_bm-0.1.1/teneva_bm/bm_func_piston.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2374 2023-04-26 18:36:44.000000 teneva_bm-0.1.1/teneva_bm/bm_func_qing.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2763 2023-04-26 18:36:49.000000 teneva_bm-0.1.1/teneva_bm/bm_func_rastrigin.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3077 2023-04-26 18:36:52.000000 teneva_bm-0.1.1/teneva_bm/bm_func_rosenbrock.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2192 2023-04-26 18:33:36.000000 teneva_bm-0.1.1/teneva_bm/bm_func_schaffer.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2702 2023-04-26 18:36:59.000000 teneva_bm-0.1.1/teneva_bm/bm_func_schwefel.py
+-rw-r--r--   0 andrei     (501) staff       (20)     5254 2023-06-13 08:13:02.000000 teneva_bm-0.1.1/teneva_bm/bm_matmul.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3127 2023-04-26 18:18:14.000000 teneva_bm-0.1.1/teneva_bm/bm_oc_simple.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1702 2023-04-26 18:18:05.000000 teneva_bm-0.1.1/teneva_bm/bm_oc_simple_constr.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2902 2023-04-26 18:33:58.000000 teneva_bm-0.1.1/teneva_bm/bm_qubo_knap_amba.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1883 2023-04-26 18:14:29.000000 teneva_bm-0.1.1/teneva_bm/bm_qubo_knap_quad.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2578 2023-04-26 18:14:02.000000 teneva_bm-0.1.1/teneva_bm/bm_qubo_maxcut.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2584 2023-04-26 18:13:28.000000 teneva_bm-0.1.1/teneva_bm/bm_qubo_mvc.py
+-rw-r--r--   0 andrei     (501) staff       (20)    11307 2023-04-26 18:12:04.000000 teneva_bm-0.1.1/teneva_bm/bm_topopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1699 2023-04-26 18:34:12.000000 teneva_bm-0.1.1/teneva_bm/bm_wall_simple.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 08:14:35.732939 teneva_bm-0.1.1/teneva_bm.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)     3733 2023-06-13 08:14:35.000000 teneva_bm-0.1.1/teneva_bm.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)      858 2023-06-13 08:14:35.000000 teneva_bm-0.1.1/teneva_bm.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-06-13 08:14:35.000000 teneva_bm-0.1.1/teneva_bm.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       33 2023-06-13 08:14:35.000000 teneva_bm-0.1.1/teneva_bm.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       10 2023-06-13 08:14:35.000000 teneva_bm-0.1.1/teneva_bm.egg-info/top_level.txt
```

### Comparing `teneva_bm-0.1.0/LICENSE.txt` & `teneva_bm-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/PKG-INFO` & `teneva_bm-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva_bm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Benchmarks library, based on a software product teneva, for tensor based multidimensional approximation and optimization methods
 Home-page: https://github.com/AndreiChertkov/teneva_bm
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
 Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
@@ -31,15 +31,15 @@
 ## Description
 
 Benchmarks library, based on a software product [teneva](https://github.com/AndreiChertkov/teneva), for tensor based multidimensional approximation and optimization methods. Benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.1.0".
+> Current version "0.1.1".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.0+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the corresponding python files). Installation of all required libraries for all benchmarks can be done with the following command:
 
@@ -55,15 +55,15 @@
 A typical scenario for working with a benchmark is as follows:
 ```python
 import numpy as np
 from teneva_bm import *
 np.random.seed(42)
 
 # Prepare benchmark and print info:
-bm = BmQuboMaxCut().prep()
+bm = BmQuboMaxcut().prep()
 print(bm.info())
 
 # Get value at multi-index i:
 i = np.ones(bm.d)
 print(bm[i])
 
 # Get values for batch of multi-indices I:
```

### Comparing `teneva_bm-0.1.0/README.md` & `teneva_bm-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## Description
 
 Benchmarks library, based on a software product [teneva](https://github.com/AndreiChertkov/teneva), for tensor based multidimensional approximation and optimization methods. Benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.1.0".
+> Current version "0.1.1".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.0+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the corresponding python files). Installation of all required libraries for all benchmarks can be done with the following command:
 
@@ -28,15 +28,15 @@
 A typical scenario for working with a benchmark is as follows:
 ```python
 import numpy as np
 from teneva_bm import *
 np.random.seed(42)
 
 # Prepare benchmark and print info:
-bm = BmQuboMaxCut().prep()
+bm = BmQuboMaxcut().prep()
 print(bm.info())
 
 # Get value at multi-index i:
 i = np.ones(bm.d)
 print(bm[i])
 
 # Get values for batch of multi-indices I:
```

### Comparing `teneva_bm-0.1.0/demo.py` & `teneva_bm-0.1.1/demo.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import subprocess
+import sys
 
 
-def demo():
+def demo(bm_use=None):
     # Extract the file names of all benchmarks from the "__init__.py" file:
     with open('teneva_bm/__init__.py', encoding='utf-8') as f:
         lines = f.readlines()
     bms = []
     for l in lines:
         if 'import' in l and l[0] != '#':
             bm = l.split('from .')[1].split(' import')[0]
@@ -14,16 +15,21 @@
 
     print(f'Full list of benchmark files (total: {len(bms)}):')
     print('>>>>', '; '.join(bms))
     print('\n\n')
 
     # Run the benchmark python file as the direct console call:
     for bm in bms:
+        if bm_use and bm_use != bm:
+            continue
+            
         out = subprocess.getoutput(f'python teneva_bm/{bm}.py')
         print(out + '\n\n\n')
         if 'Traceback' in out:
             '\n\n<----- ERROR !!! Break.\n\n'
             return
 
 
 if __name__ == '__main__':
-    demo()
+    bm_use = sys.argv[1] if len(sys.argv) > 1 else None
+
+    demo(bm_use)
```

### Comparing `teneva_bm-0.1.0/setup.py` & `teneva_bm-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/__init__.py` & `teneva_bm-0.1.1/teneva_bm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 
 from .bm import Bm
 from .bm_func_ackley import BmFuncAckley
 from .bm_func_alpine import BmFuncAlpine
 from .bm_func_dixon import BmFuncDixon
 from .bm_func_exp import BmFuncExp
@@ -10,15 +10,15 @@
 from .bm_func_michalewicz import BmFuncMichalewicz
 from .bm_func_piston import BmFuncPiston
 from .bm_func_qing import BmFuncQing
 from .bm_func_rastrigin import BmFuncRastrigin
 from .bm_func_rosenbrock import BmFuncRosenbrock
 from .bm_func_schaffer import BmFuncSchaffer
 from .bm_func_schwefel import BmFuncSchwefel
-from .bm_matmul2 import BmMatmul2
+from .bm_matmul import BmMatmul
 from .bm_oc_simple import BmOcSimple
 from .bm_oc_simple_constr import BmOcSimpleConstr
 from .bm_qubo_knap_amba import BmQuboKnapAmba
 from .bm_qubo_knap_quad import BmQuboKnapQuad
 from .bm_qubo_maxcut import BmQuboMaxcut
 from .bm_qubo_mvc import BmQuboMvc
 from .bm_topopt import BmTopopt
```

### Comparing `teneva_bm-0.1.0/teneva_bm/bm.py` & `teneva_bm-0.1.1/teneva_bm/bm.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_func_ackley.py` & `teneva_bm-0.1.1/teneva_bm/bm_func_ackley.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_func_alpine.py` & `teneva_bm-0.1.1/teneva_bm/bm_func_alpine.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_func_dixon.py` & `teneva_bm-0.1.1/teneva_bm/bm_func_dixon.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_func_exp.py` & `teneva_bm-0.1.1/teneva_bm/bm_func_exp.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_func_griewank.py` & `teneva_bm-0.1.1/teneva_bm/bm_func_griewank.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_func_michalewicz.py` & `teneva_bm-0.1.1/teneva_bm/bm_func_michalewicz.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_func_piston.py` & `teneva_bm-0.1.1/teneva_bm/bm_func_piston.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_func_qing.py` & `teneva_bm-0.1.1/teneva_bm/bm_func_qing.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_func_rastrigin.py` & `teneva_bm-0.1.1/teneva_bm/bm_func_rastrigin.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_func_rosenbrock.py` & `teneva_bm-0.1.1/teneva_bm/bm_func_rosenbrock.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_func_schaffer.py` & `teneva_bm-0.1.1/teneva_bm/bm_func_schaffer.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_func_schwefel.py` & `teneva_bm-0.1.1/teneva_bm/bm_func_schwefel.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_matmul2.py` & `teneva_bm-0.1.1/teneva_bm/bm_matmul.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,48 +2,49 @@
 import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Problem for fast 2x2 matrix multiplication (like Strassen algorithm)
-    in terms of the tensor based formulation (the search for the rank-7 CP
-    decomposition is performed).
-    The dimension and mode size are determined automatically.
+    Problem for fast size x size matrix multiplication (like Strassen
+    algorithm in the case size = 2) in terms of the tensor based
+    formulation (the search for the rank-7 CP decomposition is performed).
+    The dimension and mode size are determined automatically, but the rank
+    argument should be set manually in the case if size > 2 (e.g., for the
+    size = 3, the best known rank is 23).
 """
 
 
-class BmMatmul2(Bm):
-    def __init__(self, name='Matmul2', desc=DESC, only2=False):
-        size = 2
-        rank = 7
+class BmMatmul(Bm):
+    def __init__(self, name='Matmul', size=2, rank=7, desc=DESC, only2=False):
         E = [-1, 0, 1] # Possible items of the factor matrices
         T = _tensor_generate(size, size, size)
         d = (2 if only2 else 3) * T.shape[0] * rank
         n = len(E)
 
         super().__init__(d, n, name, desc)
 
-        self.set_min(i=np.array([
-            2, 1, 2, 1, 2, 0, 1,
-            1, 1, 1, 1, 2, 1, 2,
-            1, 2, 1, 1, 1, 2, 1,
-            2, 2, 1, 2, 1, 1, 0,
-
-            2, 2, 1, 0, 1, 2, 1,
-            1, 1, 2, 1, 1, 2, 1,
-            1, 1, 1, 2, 1, 1, 2,
-            2, 1, 0, 1, 2, 1, 2,
-
-            2, 1, 1, 2, 0, 1, 2,
-            1, 1, 2, 1, 2, 1, 1,
-            1, 2, 1, 2, 1, 1, 1,
-            2, 0, 2, 1, 1, 2, 1], dtype=int),
-            y=0.)
+        if size == 2:
+            self.set_min(i=np.array([
+                2, 1, 2, 1, 2, 0, 1,
+                1, 1, 1, 1, 2, 1, 2,
+                1, 2, 1, 1, 1, 2, 1,
+                2, 2, 1, 2, 1, 1, 0,
+
+                2, 2, 1, 0, 1, 2, 1,
+                1, 1, 2, 1, 1, 2, 1,
+                1, 1, 1, 2, 1, 1, 2,
+                2, 1, 0, 1, 2, 1, 2,
+
+                2, 1, 1, 2, 0, 1, 2,
+                1, 1, 2, 1, 2, 1, 1,
+                1, 2, 1, 2, 1, 1, 1,
+                2, 0, 2, 1, 1, 2, 1], dtype=int),
+                y=0.)
 
         self.T = T
         self.E = E
         self.size = size
         self.rank = rank
         self.only2 = only2
 
@@ -151,15 +152,15 @@
                 T[i * b + j][j * c + k][k + i * c] = 1
     return T
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmMatmul2().prep()
+    bm = BmMatmul(size=2, rank=7).prep()
     print(bm.info())
 
     text = 'Range of y for 10K random samples : '
     bm.build_trn(1.E+4)
     text += f'[{np.min(bm.y_trn):-10.3e},'
     text += f' {np.max(bm.y_trn):-10.3e}] '
     text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
@@ -176,12 +177,14 @@
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    text = 'Value at minimum (real vs calc)   :  '
-    y_real = bm.y_min_real
-    y_calc = bm[bm.i_min_real]
-    text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
+    if bm.size == 2:
+        text = 'Value at minimum (real vs calc)   :  '
+        y_real = bm.y_min_real
+        y_calc = bm[bm.i_min_real]
+        text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
+
     print(text)
```

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_oc_simple.py` & `teneva_bm-0.1.1/teneva_bm/bm_oc_simple.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_oc_simple_constr.py` & `teneva_bm-0.1.1/teneva_bm/bm_oc_simple_constr.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_qubo_knap_amba.py` & `teneva_bm-0.1.1/teneva_bm/bm_qubo_knap_amba.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_qubo_knap_quad.py` & `teneva_bm-0.1.1/teneva_bm/bm_qubo_knap_quad.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_qubo_maxcut.py` & `teneva_bm-0.1.1/teneva_bm/bm_qubo_maxcut.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_qubo_mvc.py` & `teneva_bm-0.1.1/teneva_bm/bm_qubo_mvc.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_topopt.py` & `teneva_bm-0.1.1/teneva_bm/bm_topopt.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm/bm_wall_simple.py` & `teneva_bm-0.1.1/teneva_bm/bm_wall_simple.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.1.0/teneva_bm.egg-info/PKG-INFO` & `teneva_bm-0.1.1/teneva_bm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva-bm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Benchmarks library, based on a software product teneva, for tensor based multidimensional approximation and optimization methods
 Home-page: https://github.com/AndreiChertkov/teneva_bm
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
 Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
@@ -31,15 +31,15 @@
 ## Description
 
 Benchmarks library, based on a software product [teneva](https://github.com/AndreiChertkov/teneva), for tensor based multidimensional approximation and optimization methods. Benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.1.0".
+> Current version "0.1.1".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.0+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the corresponding python files). Installation of all required libraries for all benchmarks can be done with the following command:
 
@@ -55,15 +55,15 @@
 A typical scenario for working with a benchmark is as follows:
 ```python
 import numpy as np
 from teneva_bm import *
 np.random.seed(42)
 
 # Prepare benchmark and print info:
-bm = BmQuboMaxCut().prep()
+bm = BmQuboMaxcut().prep()
 print(bm.info())
 
 # Get value at multi-index i:
 i = np.ones(bm.d)
 print(bm[i])
 
 # Get values for batch of multi-indices I:
```

### Comparing `teneva_bm-0.1.0/teneva_bm.egg-info/SOURCES.txt` & `teneva_bm-0.1.1/teneva_bm.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 teneva_bm/bm_func_michalewicz.py
 teneva_bm/bm_func_piston.py
 teneva_bm/bm_func_qing.py
 teneva_bm/bm_func_rastrigin.py
 teneva_bm/bm_func_rosenbrock.py
 teneva_bm/bm_func_schaffer.py
 teneva_bm/bm_func_schwefel.py
-teneva_bm/bm_matmul2.py
+teneva_bm/bm_matmul.py
 teneva_bm/bm_oc_simple.py
 teneva_bm/bm_oc_simple_constr.py
 teneva_bm/bm_qubo_knap_amba.py
 teneva_bm/bm_qubo_knap_quad.py
 teneva_bm/bm_qubo_maxcut.py
 teneva_bm/bm_qubo_mvc.py
 teneva_bm/bm_topopt.py
```

