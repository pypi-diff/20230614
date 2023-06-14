# Comparing `tmp/pandas_selectable-1.1.1.tar.gz` & `tmp/pandas_selectable-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_selectable-1.1.1.tar", last modified: Thu Nov 11 16:50:38 2021, max compression
+gzip compressed data, was "pandas_selectable-1.2.0.tar", last modified: Wed Jun 14 21:43:11 2023, max compression
```

## Comparing `pandas_selectable-1.1.1.tar` & `pandas_selectable-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:38.660240 pandas_selectable-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2021-11-11 16:50:29.000000 pandas_selectable-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2395 2021-11-11 16:50:38.660240 pandas_selectable-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2021-11-11 16:50:29.000000 pandas_selectable-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:38.656240 pandas_selectable-1.1.1/pandas_selectable/
--rw-r--r--   0 runner    (1001) docker     (121)     8035 2021-11-11 16:50:29.000000 pandas_selectable-1.1.1/pandas_selectable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:38.660240 pandas_selectable-1.1.1/pandas_selectable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2395 2021-11-11 16:50:38.000000 pandas_selectable-1.1.1/pandas_selectable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-11-11 16:50:38.000000 pandas_selectable-1.1.1/pandas_selectable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-11 16:50:38.000000 pandas_selectable-1.1.1/pandas_selectable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-11-11 16:50:38.000000 pandas_selectable-1.1.1/pandas_selectable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      306 2021-11-11 16:50:29.000000 pandas_selectable-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-11 16:50:38.660240 pandas_selectable-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      569 2021-11-11 16:50:29.000000 pandas_selectable-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:11.025844 pandas_selectable-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-14 21:43:00.000000 pandas_selectable-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-14 21:43:11.025844 pandas_selectable-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-14 21:43:00.000000 pandas_selectable-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:11.025844 pandas_selectable-1.2.0/pandas_selectable/
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-06-14 21:43:00.000000 pandas_selectable-1.2.0/pandas_selectable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:11.025844 pandas_selectable-1.2.0/pandas_selectable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-14 21:43:10.000000 pandas_selectable-1.2.0/pandas_selectable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-14 21:43:11.000000 pandas_selectable-1.2.0/pandas_selectable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:43:10.000000 pandas_selectable-1.2.0/pandas_selectable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 21:43:10.000000 pandas_selectable-1.2.0/pandas_selectable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-14 21:43:00.000000 pandas_selectable-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:43:11.025844 pandas_selectable-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-14 21:43:00.000000 pandas_selectable-1.2.0/setup.py
```

### Comparing `pandas_selectable-1.1.1/LICENSE` & `pandas_selectable-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_selectable-1.1.1/PKG-INFO` & `pandas_selectable-1.2.0/pandas_selectable.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
-Name: pandas_selectable
-Version: 1.1.1
+Name: pandas-selectable
+Version: 1.2.0
 Summary: Add a select accessor to pandas
 Home-page: https://github.com/jseabold/pandas-selectable
 Author: Skipper Seabold
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pandas-selectable
@@ -116,9 +114,7 @@
 [pandas](https://pandas.pydata.org/) >= 1.1
 
 ## Installation
 
 ```bash
 pip install pandas-selectable
 ```
-
-
```

### Comparing `pandas_selectable-1.1.1/README.md` & `pandas_selectable-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pandas_selectable-1.1.1/pandas_selectable/__init__.py` & `pandas_selectable-1.2.0/pandas_selectable/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import inspect
 import operator
 from functools import wraps
 
-import numpy as np
 import pandas as pd
 from pandas.core.accessor import CachedAccessor
 from pandas.core.indexes.accessors import (
     CombinedDatetimelikeProperties,
     DatetimeProperties,
     PeriodProperties,
 )
-from pandas.core.strings import StringMethods
+
+try:
+    from pandas.core.strings import StringMethods
+except ImportError:  # moved in pandas 2
+    from pandas.core.strings.accessor import StringMethods
 from pandas.util._decorators import doc
 
 _str_boolean_methods = set(
     [
         'contains',
         'endswith',
         'isalnum',
```

### Comparing `pandas_selectable-1.1.1/pandas_selectable.egg-info/PKG-INFO` & `pandas_selectable-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
-Name: pandas-selectable
-Version: 1.1.1
+Name: pandas_selectable
+Version: 1.2.0
 Summary: Add a select accessor to pandas
 Home-page: https://github.com/jseabold/pandas-selectable
 Author: Skipper Seabold
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pandas-selectable
@@ -116,9 +114,7 @@
 [pandas](https://pandas.pydata.org/) >= 1.1
 
 ## Installation
 
 ```bash
 pip install pandas-selectable
 ```
-
-
```

### Comparing `pandas_selectable-1.1.1/setup.py` & `pandas_selectable-1.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md") as readme:
     description = readme.read()
 
 
 setup(
     name='pandas_selectable',
-    version='1.1.1',
+    version='1.2.0',
     description='Add a select accessor to pandas',
     packages=['pandas_selectable'],
     long_description=description,
     long_description_content_type="text/markdown",
     author="Skipper Seabold",
     url="https://github.com/jseabold/pandas-selectable",
     classifiers=[
```

