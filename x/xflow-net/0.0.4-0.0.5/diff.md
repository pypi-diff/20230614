# Comparing `tmp/xflow-net-0.0.4.tar.gz` & `tmp/xflow-net-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xflow-net-0.0.4.tar", last modified: Tue Jun 13 16:47:06 2023, max compression
+gzip compressed data, was "xflow-net-0.0.5.tar", last modified: Tue Jun 13 17:07:41 2023, max compression
```

## Comparing `xflow-net-0.0.4.tar` & `xflow-net-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:47:06.340326 xflow-net-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-13 16:46:53.000000 xflow-net-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-13 16:47:06.340326 xflow-net-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-13 16:46:53.000000 xflow-net-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-13 16:46:53.000000 xflow-net-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-13 16:47:06.340326 xflow-net-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-13 16:46:53.000000 xflow-net-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:47:06.340326 xflow-net-0.0.4/xflow/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-13 16:46:53.000000 xflow-net-0.0.4/xflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-13 16:46:53.000000 xflow-net-0.0.4/xflow/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-13 16:46:53.000000 xflow-net-0.0.4/xflow/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:47:06.340326 xflow-net-0.0.4/xflow_net.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-13 16:47:06.000000 xflow-net-0.0.4/xflow_net.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-13 16:47:06.000000 xflow-net-0.0.4/xflow_net.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:47:06.000000 xflow-net-0.0.4/xflow_net.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 16:47:06.000000 xflow-net-0.0.4/xflow_net.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 16:47:06.000000 xflow-net-0.0.4/xflow_net.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:07:41.454141 xflow-net-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-13 17:07:30.000000 xflow-net-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-13 17:07:41.454141 xflow-net-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-13 17:07:30.000000 xflow-net-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-13 17:07:30.000000 xflow-net-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-13 17:07:41.454141 xflow-net-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-13 17:07:30.000000 xflow-net-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:07:41.454141 xflow-net-0.0.5/xflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-13 17:07:30.000000 xflow-net-0.0.5/xflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:07:41.454141 xflow-net-0.0.5/xflow/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-13 17:07:30.000000 xflow-net-0.0.5/xflow/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-13 17:07:30.000000 xflow-net-0.0.5/xflow/dataset/nx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-13 17:07:30.000000 xflow-net-0.0.5/xflow/dataset/pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-13 17:07:30.000000 xflow-net-0.0.5/xflow/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-13 17:07:30.000000 xflow-net-0.0.5/xflow/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:07:41.454141 xflow-net-0.0.5/xflow_net.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-13 17:07:41.000000 xflow-net-0.0.5/xflow_net.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 17:07:41.000000 xflow-net-0.0.5/xflow_net.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:07:41.000000 xflow-net-0.0.5/xflow_net.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 17:07:41.000000 xflow-net-0.0.5/xflow_net.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 17:07:41.000000 xflow-net-0.0.5/xflow_net.egg-info/top_level.txt
```

### Comparing `xflow-net-0.0.4/LICENSE` & `xflow-net-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.4/PKG-INFO` & `xflow-net-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xflow-net
-Version: 0.0.4
+Version: 0.0.5
 Summary: a python library for graph flow
 Home-page: https://xflow.network/
 Author: XGraphing
 Author-email: zchen@cse.msstate.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xflow-net-0.0.4/README.md` & `xflow-net-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.4/setup.py` & `xflow-net-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Package meta-data.
 NAME = 'xflow-net'
 DESCRIPTION = 'a python library for graph flow'
 URL = 'https://xflow.network/'
 EMAIL = 'zchen@cse.msstate.edu'
 AUTHOR = 'XGraphing'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
    'networkx', 'ndlib'
 ]
 
 # What packages are optional?
```

### Comparing `xflow-net-0.0.4/xflow/visualization.py` & `xflow-net-0.0.5/xflow/visualization.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.4/xflow_net.egg-info/PKG-INFO` & `xflow-net-0.0.5/xflow_net.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xflow-net
-Version: 0.0.4
+Version: 0.0.5
 Summary: a python library for graph flow
 Home-page: https://xflow.network/
 Author: XGraphing
 Author-email: zchen@cse.msstate.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

