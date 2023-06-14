# Comparing `tmp/xflow-net-0.0.6.tar.gz` & `tmp/xflow-net-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xflow-net-0.0.6.tar", last modified: Wed Jun 14 16:15:40 2023, max compression
+gzip compressed data, was "xflow-net-0.0.7.tar", last modified: Wed Jun 14 16:21:04 2023, max compression
```

## Comparing `xflow-net-0.0.6.tar` & `xflow-net-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:15:40.734794 xflow-net-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-14 16:15:22.000000 xflow-net-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-14 16:15:40.734794 xflow-net-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-14 16:15:22.000000 xflow-net-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-14 16:15:22.000000 xflow-net-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-14 16:15:40.734794 xflow-net-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-14 16:15:22.000000 xflow-net-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:15:40.730794 xflow-net-0.0.6/xflow/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 16:15:22.000000 xflow-net-0.0.6/xflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:15:40.734794 xflow-net-0.0.6/xflow/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-14 16:15:22.000000 xflow-net-0.0.6/xflow/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-14 16:15:22.000000 xflow-net-0.0.6/xflow/dataset/nx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-14 16:15:22.000000 xflow-net-0.0.6/xflow/dataset/pyg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:15:40.734794 xflow-net-0.0.6/xflow/method/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:15:22.000000 xflow-net-0.0.6/xflow/method/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-14 16:15:22.000000 xflow-net-0.0.6/xflow/method/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-06-14 16:15:22.000000 xflow-net-0.0.6/xflow/method/im.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-14 16:15:22.000000 xflow-net-0.0.6/xflow/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-14 16:15:22.000000 xflow-net-0.0.6/xflow/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:15:40.734794 xflow-net-0.0.6/xflow_net.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-14 16:15:40.000000 xflow-net-0.0.6/xflow_net.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-14 16:15:40.000000 xflow-net-0.0.6/xflow_net.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:15:40.000000 xflow-net-0.0.6/xflow_net.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-14 16:15:40.000000 xflow-net-0.0.6/xflow_net.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 16:15:40.000000 xflow-net-0.0.6/xflow_net.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:21:04.670457 xflow-net-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-14 16:20:40.000000 xflow-net-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-14 16:21:04.670457 xflow-net-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-14 16:20:40.000000 xflow-net-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-14 16:20:40.000000 xflow-net-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-14 16:21:04.670457 xflow-net-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-14 16:20:40.000000 xflow-net-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:21:04.662457 xflow-net-0.0.7/xflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 16:20:40.000000 xflow-net-0.0.7/xflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:21:04.662457 xflow-net-0.0.7/xflow/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-14 16:20:40.000000 xflow-net-0.0.7/xflow/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-14 16:20:40.000000 xflow-net-0.0.7/xflow/dataset/nx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-14 16:20:40.000000 xflow-net-0.0.7/xflow/dataset/pyg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:21:04.666457 xflow-net-0.0.7/xflow/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-14 16:20:40.000000 xflow-net-0.0.7/xflow/diffusion/IC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-14 16:20:40.000000 xflow-net-0.0.7/xflow/diffusion/LT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-14 16:20:40.000000 xflow-net-0.0.7/xflow/diffusion/SI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:20:40.000000 xflow-net-0.0.7/xflow/diffusion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:21:04.670457 xflow-net-0.0.7/xflow/method/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:20:40.000000 xflow-net-0.0.7/xflow/method/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-14 16:20:40.000000 xflow-net-0.0.7/xflow/method/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-06-14 16:20:40.000000 xflow-net-0.0.7/xflow/method/im.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-14 16:20:40.000000 xflow-net-0.0.7/xflow/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-14 16:20:40.000000 xflow-net-0.0.7/xflow/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:21:04.670457 xflow-net-0.0.7/xflow_net.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-14 16:21:04.000000 xflow-net-0.0.7/xflow_net.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-14 16:21:04.000000 xflow-net-0.0.7/xflow_net.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:21:04.000000 xflow-net-0.0.7/xflow_net.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-14 16:21:04.000000 xflow-net-0.0.7/xflow_net.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 16:21:04.000000 xflow-net-0.0.7/xflow_net.egg-info/top_level.txt
```

### Comparing `xflow-net-0.0.6/LICENSE` & `xflow-net-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.6/PKG-INFO` & `xflow-net-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xflow-net
-Version: 0.0.6
+Version: 0.0.7
 Summary: a python library for graph flow
 Home-page: https://xflow.network/
 Author: XGraphing
 Author-email: zchen@cse.msstate.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xflow-net-0.0.6/README.md` & `xflow-net-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.6/setup.py` & `xflow-net-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Package meta-data.
 NAME = 'xflow-net'
 DESCRIPTION = 'a python library for graph flow'
 URL = 'https://xflow.network/'
 EMAIL = 'zchen@cse.msstate.edu'
 AUTHOR = 'XGraphing'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
    'networkx', 'ndlib'
 ]
 
 # What packages are optional?
```

### Comparing `xflow-net-0.0.6/xflow/dataset/nx.py` & `xflow-net-0.0.7/xflow/dataset/nx.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.6/xflow/dataset/pyg.py` & `xflow-net-0.0.7/xflow/dataset/pyg.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.6/xflow/method/ibm.py` & `xflow-net-0.0.7/xflow/method/ibm.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.6/xflow/method/im.py` & `xflow-net-0.0.7/xflow/method/im.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.6/xflow/visualization.py` & `xflow-net-0.0.7/xflow/visualization.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.6/xflow_net.egg-info/PKG-INFO` & `xflow-net-0.0.7/xflow_net.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xflow-net
-Version: 0.0.6
+Version: 0.0.7
 Summary: a python library for graph flow
 Home-page: https://xflow.network/
 Author: XGraphing
 Author-email: zchen@cse.msstate.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

