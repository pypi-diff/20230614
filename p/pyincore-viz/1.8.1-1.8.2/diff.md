# Comparing `tmp/pyincore_viz-1.8.1.tar.gz` & `tmp/pyincore_viz-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyincore_viz-1.8.1.tar", last modified: Tue Nov 15 21:36:56 2022, max compression
+gzip compressed data, was "pyincore_viz-1.8.2.tar", last modified: Wed Jun 14 17:36:47 2023, max compression
```

## Comparing `pyincore_viz-1.8.1.tar` & `pyincore_viz-1.8.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:36:56.605523 pyincore_viz-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)    16725 2022-11-15 21:35:34.000000 pyincore_viz-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-11-15 21:36:56.601523 pyincore_viz-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1951 2022-11-15 21:35:34.000000 pyincore_viz-1.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:36:56.601523 pyincore_viz-1.8.1/pyincore_viz/
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-11-15 21:35:34.000000 pyincore_viz-1.8.1/pyincore_viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:36:56.601523 pyincore_viz-1.8.1/pyincore_viz/analysis/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-11-15 21:35:34.000000 pyincore_viz-1.8.1/pyincore_viz/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19705 2022-11-15 21:35:34.000000 pyincore_viz-1.8.1/pyincore_viz/analysis/popresultstable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-11-15 21:35:34.000000 pyincore_viz-1.8.1/pyincore_viz/analysisviz.py
--rw-r--r--   0 runner    (1001) docker     (121)    53960 2022-11-15 21:35:34.000000 pyincore_viz-1.8.1/pyincore_viz/geoutil.py
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-11-15 21:35:34.000000 pyincore_viz-1.8.1/pyincore_viz/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:36:56.601523 pyincore_viz-1.8.1/pyincore_viz/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 21:35:34.000000 pyincore_viz-1.8.1/pyincore_viz/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-11-15 21:35:34.000000 pyincore_viz-1.8.1/pyincore_viz/helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-11-15 21:35:34.000000 pyincore_viz-1.8.1/pyincore_viz/logging.ini
--rw-r--r--   0 runner    (1001) docker     (121)    14691 2022-11-15 21:35:34.000000 pyincore_viz-1.8.1/pyincore_viz/plotutil.py
--rw-r--r--   0 runner    (1001) docker     (121)     4778 2022-11-15 21:35:34.000000 pyincore_viz-1.8.1/pyincore_viz/tabledatasetlistmap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:36:56.601523 pyincore_viz-1.8.1/pyincore_viz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-11-15 21:36:56.000000 pyincore_viz-1.8.1/pyincore_viz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-11-15 21:36:56.000000 pyincore_viz-1.8.1/pyincore_viz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 21:36:56.000000 pyincore_viz-1.8.1/pyincore_viz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-15 21:36:56.000000 pyincore_viz-1.8.1/pyincore_viz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-15 21:36:56.000000 pyincore_viz-1.8.1/pyincore_viz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-15 21:36:56.605523 pyincore_viz-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-11-15 21:35:34.000000 pyincore_viz-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:36:47.103342 pyincore_viz-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-14 17:34:56.000000 pyincore_viz-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-14 17:36:47.103342 pyincore_viz-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-14 17:34:56.000000 pyincore_viz-1.8.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:36:47.103342 pyincore_viz-1.8.2/pyincore_viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-14 17:34:56.000000 pyincore_viz-1.8.2/pyincore_viz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:36:47.103342 pyincore_viz-1.8.2/pyincore_viz/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-14 17:34:56.000000 pyincore_viz-1.8.2/pyincore_viz/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19705 2023-06-14 17:34:56.000000 pyincore_viz-1.8.2/pyincore_viz/analysis/popresultstable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-14 17:34:56.000000 pyincore_viz-1.8.2/pyincore_viz/analysisviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53960 2023-06-14 17:34:56.000000 pyincore_viz-1.8.2/pyincore_viz/geoutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-14 17:34:56.000000 pyincore_viz-1.8.2/pyincore_viz/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:36:47.103342 pyincore_viz-1.8.2/pyincore_viz/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:34:56.000000 pyincore_viz-1.8.2/pyincore_viz/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-14 17:34:56.000000 pyincore_viz-1.8.2/pyincore_viz/helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-14 17:34:56.000000 pyincore_viz-1.8.2/pyincore_viz/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    14691 2023-06-14 17:34:56.000000 pyincore_viz-1.8.2/pyincore_viz/plotutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-14 17:34:56.000000 pyincore_viz-1.8.2/pyincore_viz/tabledatasetlistmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:36:47.103342 pyincore_viz-1.8.2/pyincore_viz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-14 17:36:47.000000 pyincore_viz-1.8.2/pyincore_viz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-14 17:36:47.000000 pyincore_viz-1.8.2/pyincore_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 17:36:47.000000 pyincore_viz-1.8.2/pyincore_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-14 17:36:47.000000 pyincore_viz-1.8.2/pyincore_viz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 17:36:47.000000 pyincore_viz-1.8.2/pyincore_viz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 17:36:47.103342 pyincore_viz-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-14 17:34:56.000000 pyincore_viz-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:36:47.103342 pyincore_viz-1.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-14 17:34:56.000000 pyincore_viz-1.8.2/tests/test_format.py
```

### Comparing `pyincore_viz-1.8.1/LICENSE` & `pyincore_viz-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyincore_viz-1.8.1/PKG-INFO` & `pyincore_viz-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyincore_viz
-Version: 1.8.1
+Version: 1.8.2
 Summary: IN-CORE visualization python package
 Home-page: https://incore.ncsa.illinois.edu
 License: Mozilla Public License v2.0
 Project-URL: Bug Reports, https://github.com/IN-CORE/pyincor-vize/issues
 Project-URL: Source, https://github.com/IN-CORE/pyincor-vize
 Keywords: infrastructure,resilience,hazards,data discovery,IN-CORE,earthquake,tsunami,tornado,hurricane,dislocation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyincore_viz-1.8.1/README.rst` & `pyincore_viz-1.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyincore_viz-1.8.1/pyincore_viz/__init__.py` & `pyincore_viz-1.8.2/pyincore_viz/__init__.py`

 * *Files identical despite different names*

### Comparing `pyincore_viz-1.8.1/pyincore_viz/analysis/popresultstable.py` & `pyincore_viz-1.8.2/pyincore_viz/analysis/popresultstable.py`

 * *Files identical despite different names*

### Comparing `pyincore_viz-1.8.1/pyincore_viz/analysisviz.py` & `pyincore_viz-1.8.2/pyincore_viz/analysisviz.py`

 * *Files identical despite different names*

### Comparing `pyincore_viz-1.8.1/pyincore_viz/geoutil.py` & `pyincore_viz-1.8.2/pyincore_viz/geoutil.py`

 * *Files identical despite different names*

### Comparing `pyincore_viz-1.8.1/pyincore_viz/globals.py` & `pyincore_viz-1.8.2/pyincore_viz/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # terms of the Mozilla Public License v2.0 which accompanies this distribution,
 # and is available at https://www.mozilla.org/en-US/MPL/2.0/
 
 import os
 import logging
 from logging import config as logging_config
 
-PACKAGE_VERSION = "1.8.1"
+PACKAGE_VERSION = "1.8.2"
 
 INCORE_GEOSERVER_WMS_URL = "https://incore.ncsa.illinois.edu/geoserver/incore/wms"
 INCORE_GEOSERVER_DEV_WMS_URL = "https://incore-dev.ncsa.illinois.edu/geoserver/incore/wms"
 
 PYINCORE_VIZ_ROOT_FOLDER = os.path.dirname(os.path.dirname(__file__))
 
 LOGGING_CONFIG = os.path.abspath(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'logging.ini'))
```

### Comparing `pyincore_viz-1.8.1/pyincore_viz/helpers/common.py` & `pyincore_viz-1.8.2/pyincore_viz/helpers/common.py`

 * *Files identical despite different names*

### Comparing `pyincore_viz-1.8.1/pyincore_viz/logging.ini` & `pyincore_viz-1.8.2/pyincore_viz/logging.ini`

 * *Files identical despite different names*

### Comparing `pyincore_viz-1.8.1/pyincore_viz/plotutil.py` & `pyincore_viz-1.8.2/pyincore_viz/plotutil.py`

 * *Files identical despite different names*

### Comparing `pyincore_viz-1.8.1/pyincore_viz/tabledatasetlistmap.py` & `pyincore_viz-1.8.2/pyincore_viz/tabledatasetlistmap.py`

 * *Files identical despite different names*

### Comparing `pyincore_viz-1.8.1/pyincore_viz.egg-info/PKG-INFO` & `pyincore_viz-1.8.2/pyincore_viz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyincore-viz
-Version: 1.8.1
+Version: 1.8.2
 Summary: IN-CORE visualization python package
 Home-page: https://incore.ncsa.illinois.edu
 License: Mozilla Public License v2.0
 Project-URL: Bug Reports, https://github.com/IN-CORE/pyincor-vize/issues
 Project-URL: Source, https://github.com/IN-CORE/pyincor-vize
 Keywords: infrastructure,resilience,hazards,data discovery,IN-CORE,earthquake,tsunami,tornado,hurricane,dislocation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyincore_viz-1.8.1/pyincore_viz.egg-info/SOURCES.txt` & `pyincore_viz-1.8.2/pyincore_viz.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 pyincore_viz.egg-info/SOURCES.txt
 pyincore_viz.egg-info/dependency_links.txt
 pyincore_viz.egg-info/requires.txt
 pyincore_viz.egg-info/top_level.txt
 pyincore_viz/analysis/__init__.py
 pyincore_viz/analysis/popresultstable.py
 pyincore_viz/helpers/__init__.py
-pyincore_viz/helpers/common.py
+pyincore_viz/helpers/common.py
+tests/test_format.py
```

### Comparing `pyincore_viz-1.8.1/setup.py` & `pyincore_viz-1.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This program and the accompanying materials are made available under the
 # terms of the Mozilla Public License v2.0 which accompanies this distribution,
 # and is available at https://www.mozilla.org/en-US/MPL/2.0/
 
 from setuptools import setup, find_packages
 
 # version number of pyincore
-version = '1.8.1'
+version = '1.8.2'
 
 with open("README.rst", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name='pyincore_viz',
     version=version,
```

