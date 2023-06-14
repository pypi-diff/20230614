# Comparing `tmp/PyPromql-0.0.1.tar.gz` & `tmp/PyPromql-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPromql-0.0.1.tar", last modified: Sat Jun 10 15:17:20 2023, max compression
+gzip compressed data, was "PyPromql-0.0.2.tar", last modified: Wed Jun 14 18:14:41 2023, max compression
```

## Comparing `PyPromql-0.0.1.tar` & `PyPromql-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 15:17:20.105894 PyPromql-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-06-09 16:49:37.000000 PyPromql-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1059 2023-06-10 15:17:20.104911 PyPromql-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-10 15:17:20.090892 PyPromql-0.0.1/PyPromql.egg-info/
--rw-rw-rw-   0        0        0     1059 2023-06-10 15:17:20.000000 PyPromql-0.0.1/PyPromql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      592 2023-06-10 15:17:20.000000 PyPromql-0.0.1/PyPromql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 15:17:20.000000 PyPromql-0.0.1/PyPromql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-10 15:17:20.000000 PyPromql-0.0.1/PyPromql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-10 15:17:20.000000 PyPromql-0.0.1/PyPromql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      185 2023-06-10 14:58:34.000000 PyPromql-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 15:17:20.092893 PyPromql-0.0.1/pypromql/
--rw-rw-rw-   0        0        0      192 2023-06-10 14:45:03.000000 PyPromql-0.0.1/pypromql/__init__.py
--rw-rw-rw-   0        0        0     2281 2023-06-10 14:45:03.000000 PyPromql-0.0.1/pypromql/connection.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:17:20.096896 PyPromql-0.0.1/pypromql/query/
--rw-rw-rw-   0        0        0       74 2023-06-10 12:43:08.000000 PyPromql-0.0.1/pypromql/query/__init__.py
--rw-rw-rw-   0        0        0      885 2023-06-10 12:43:08.000000 PyPromql-0.0.1/pypromql/query/prometheus_label.py
--rw-rw-rw-   0        0        0      557 2023-06-10 12:43:08.000000 PyPromql-0.0.1/pypromql/query/prometheus_query.py
--rw-rw-rw-   0        0        0     2853 2023-06-10 12:43:08.000000 PyPromql-0.0.1/pypromql/query/prometheus_query_builder.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:17:20.099895 PyPromql-0.0.1/pypromql/result/
--rw-rw-rw-   0        0        0      148 2023-06-10 14:45:03.000000 PyPromql-0.0.1/pypromql/result/__init__.py
--rw-rw-rw-   0        0        0      783 2023-06-10 14:45:03.000000 PyPromql-0.0.1/pypromql/result/prometheus_metric.py
--rw-rw-rw-   0        0        0     1505 2023-06-10 14:45:03.000000 PyPromql-0.0.1/pypromql/result/prometheus_result.py
--rw-rw-rw-   0        0        0       42 2023-06-10 15:17:20.106893 PyPromql-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1283 2023-06-10 15:14:39.000000 PyPromql-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:17:20.099895 PyPromql-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-06-10 12:43:08.000000 PyPromql-0.0.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:17:20.101894 PyPromql-0.0.1/tests/query/
--rw-rw-rw-   0        0        0        0 2023-06-10 12:43:08.000000 PyPromql-0.0.1/tests/query/__init__.py
--rw-rw-rw-   0        0        0     2396 2023-06-10 12:43:08.000000 PyPromql-0.0.1/tests/query/test_query.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:17:20.102907 PyPromql-0.0.1/tests/result/
--rw-rw-rw-   0        0        0        0 2023-06-10 14:45:03.000000 PyPromql-0.0.1/tests/result/__init__.py
--rw-rw-rw-   0        0        0     3664 2023-06-10 14:45:03.000000 PyPromql-0.0.1/tests/result/test_result.py
+drwxrwxrwx   0        0        0        0 2023-06-14 18:14:41.944084 PyPromql-0.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-06-09 16:49:37.000000 PyPromql-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3307 2023-06-14 18:14:41.944084 PyPromql-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 18:14:41.919083 PyPromql-0.0.2/PyPromql.egg-info/
+-rw-rw-rw-   0        0        0     3307 2023-06-14 18:14:41.000000 PyPromql-0.0.2/PyPromql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-06-14 18:14:41.000000 PyPromql-0.0.2/PyPromql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 18:14:41.000000 PyPromql-0.0.2/PyPromql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-14 18:14:41.000000 PyPromql-0.0.2/PyPromql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-14 18:14:41.000000 PyPromql-0.0.2/PyPromql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2433 2023-06-14 18:13:15.000000 PyPromql-0.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-14 18:14:41.921085 PyPromql-0.0.2/pypromql/
+-rw-rw-rw-   0        0        0       59 2023-06-14 18:13:15.000000 PyPromql-0.0.2/pypromql/__init__.py
+-rw-rw-rw-   0        0        0     2257 2023-06-14 18:13:15.000000 PyPromql-0.0.2/pypromql/connection.py
+drwxrwxrwx   0        0        0        0 2023-06-14 18:14:41.937084 PyPromql-0.0.2/pypromql/query/
+-rw-rw-rw-   0        0        0      160 2023-06-14 18:13:15.000000 PyPromql-0.0.2/pypromql/query/__init__.py
+-rw-rw-rw-   0        0        0      885 2023-06-10 12:43:08.000000 PyPromql-0.0.2/pypromql/query/prometheus_label.py
+-rw-rw-rw-   0        0        0      557 2023-06-10 12:43:08.000000 PyPromql-0.0.2/pypromql/query/prometheus_query.py
+-rw-rw-rw-   0        0        0     2853 2023-06-10 12:43:08.000000 PyPromql-0.0.2/pypromql/query/prometheus_query_builder.py
+drwxrwxrwx   0        0        0        0 2023-06-14 18:14:41.939084 PyPromql-0.0.2/pypromql/result/
+-rw-rw-rw-   0        0        0      148 2023-06-10 14:45:03.000000 PyPromql-0.0.2/pypromql/result/__init__.py
+-rw-rw-rw-   0        0        0      783 2023-06-10 14:45:03.000000 PyPromql-0.0.2/pypromql/result/prometheus_metric.py
+-rw-rw-rw-   0        0        0     1505 2023-06-10 14:45:03.000000 PyPromql-0.0.2/pypromql/result/prometheus_result.py
+-rw-rw-rw-   0        0        0       42 2023-06-14 18:14:41.944084 PyPromql-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1284 2023-06-14 18:14:39.000000 PyPromql-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 18:14:41.940088 PyPromql-0.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-10 12:43:08.000000 PyPromql-0.0.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 18:14:41.941084 PyPromql-0.0.2/tests/query/
+-rw-rw-rw-   0        0        0        0 2023-06-10 12:43:08.000000 PyPromql-0.0.2/tests/query/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-06-14 18:13:15.000000 PyPromql-0.0.2/tests/query/test_query.py
+drwxrwxrwx   0        0        0        0 2023-06-14 18:14:41.943084 PyPromql-0.0.2/tests/result/
+-rw-rw-rw-   0        0        0        0 2023-06-10 14:45:03.000000 PyPromql-0.0.2/tests/result/__init__.py
+-rw-rw-rw-   0        0        0     3646 2023-06-14 18:13:15.000000 PyPromql-0.0.2/tests/result/test_result.py
```

### Comparing `PyPromql-0.0.1/LICENSE` & `PyPromql-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPromql-0.0.1/PyPromql.egg-info/SOURCES.txt` & `PyPromql-0.0.2/PyPromql.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 LICENSE
-README.md
+README.rst
 setup.py
 PyPromql.egg-info/PKG-INFO
 PyPromql.egg-info/SOURCES.txt
 PyPromql.egg-info/dependency_links.txt
 PyPromql.egg-info/requires.txt
 PyPromql.egg-info/top_level.txt
 pypromql/__init__.py
```

### Comparing `PyPromql-0.0.1/pypromql/connection.py` & `PyPromql-0.0.2/pypromql/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import requests
 from requests.adapters import HTTPAdapter
-from requests.packages.urllib3.util.retry import Retry
+from urllib3.util import Retry
 from urllib.parse import quote
 
 __all__ = ['PrometheusConnection']
 
 
 class PrometheusConnection:
     """
```

### Comparing `PyPromql-0.0.1/pypromql/query/prometheus_label.py` & `PyPromql-0.0.2/pypromql/query/prometheus_label.py`

 * *Files identical despite different names*

### Comparing `PyPromql-0.0.1/pypromql/query/prometheus_query.py` & `PyPromql-0.0.2/pypromql/query/prometheus_query.py`

 * *Files identical despite different names*

### Comparing `PyPromql-0.0.1/pypromql/query/prometheus_query_builder.py` & `PyPromql-0.0.2/pypromql/query/prometheus_query_builder.py`

 * *Files identical despite different names*

### Comparing `PyPromql-0.0.1/pypromql/result/prometheus_metric.py` & `PyPromql-0.0.2/pypromql/result/prometheus_metric.py`

 * *Files identical despite different names*

### Comparing `PyPromql-0.0.1/pypromql/result/prometheus_result.py` & `PyPromql-0.0.2/pypromql/result/prometheus_result.py`

 * *Files identical despite different names*

### Comparing `PyPromql-0.0.1/setup.py` & `PyPromql-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 
 def get_readme_file():
-    with open('README.md', 'r') as f:
+    with open('README.rst', 'r') as f:
         return f.read()
 
 
 def get_requirements():
     with open('requirements.txt', 'r') as f:
         return f.read().splitlines()
 
 
 setup(
     name='PyPromql',
-    version='0.0.1',
+    version='0.0.2',
     author='Aviv Levi',
     author_email='60aviv60@gmail.com',
     description='PyPromql is a Python library that simplifies the creation and execution of PromQL queries.',
     long_description=get_readme_file(),
     long_description_content_type='text/markdown',
     url='https://github.com/aviv-levi/pypromql.git',
     packages=find_packages(),
```

### Comparing `PyPromql-0.0.1/tests/query/test_query.py` & `PyPromql-0.0.2/tests/query/test_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pypromql.query.prometheus_query import Query
+from pypromql.query import Query
 from datetime import datetime
 
 
 def test_simple_query():
     # arrange
     metric_name = 'scrape_duration_seconds'
     # act
```

### Comparing `PyPromql-0.0.1/tests/result/test_result.py` & `PyPromql-0.0.2/tests/result/test_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pypromql.result.prometheus_result import PrometheusResult, Metric
+from pypromql.result import PrometheusResult, Metric
 
 
 def test_load_successfully_with_warnings():
     # arrange
     response = {
         'status': 'success',
         'data': {
```

