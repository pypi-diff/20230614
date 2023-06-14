# Comparing `tmp/PyPromql-0.0.2.tar.gz` & `tmp/PyPromql-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPromql-0.0.2.tar", last modified: Wed Jun 14 18:14:41 2023, max compression
+gzip compressed data, was "PyPromql-0.0.3.tar", last modified: Wed Jun 14 20:38:00 2023, max compression
```

## Comparing `PyPromql-0.0.2.tar` & `PyPromql-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 18:14:41.944084 PyPromql-0.0.2/
--rw-rw-rw-   0        0        0     1087 2023-06-09 16:49:37.000000 PyPromql-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3307 2023-06-14 18:14:41.944084 PyPromql-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 18:14:41.919083 PyPromql-0.0.2/PyPromql.egg-info/
--rw-rw-rw-   0        0        0     3307 2023-06-14 18:14:41.000000 PyPromql-0.0.2/PyPromql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      593 2023-06-14 18:14:41.000000 PyPromql-0.0.2/PyPromql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 18:14:41.000000 PyPromql-0.0.2/PyPromql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-14 18:14:41.000000 PyPromql-0.0.2/PyPromql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-14 18:14:41.000000 PyPromql-0.0.2/PyPromql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2433 2023-06-14 18:13:15.000000 PyPromql-0.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-14 18:14:41.921085 PyPromql-0.0.2/pypromql/
--rw-rw-rw-   0        0        0       59 2023-06-14 18:13:15.000000 PyPromql-0.0.2/pypromql/__init__.py
--rw-rw-rw-   0        0        0     2257 2023-06-14 18:13:15.000000 PyPromql-0.0.2/pypromql/connection.py
-drwxrwxrwx   0        0        0        0 2023-06-14 18:14:41.937084 PyPromql-0.0.2/pypromql/query/
--rw-rw-rw-   0        0        0      160 2023-06-14 18:13:15.000000 PyPromql-0.0.2/pypromql/query/__init__.py
--rw-rw-rw-   0        0        0      885 2023-06-10 12:43:08.000000 PyPromql-0.0.2/pypromql/query/prometheus_label.py
--rw-rw-rw-   0        0        0      557 2023-06-10 12:43:08.000000 PyPromql-0.0.2/pypromql/query/prometheus_query.py
--rw-rw-rw-   0        0        0     2853 2023-06-10 12:43:08.000000 PyPromql-0.0.2/pypromql/query/prometheus_query_builder.py
-drwxrwxrwx   0        0        0        0 2023-06-14 18:14:41.939084 PyPromql-0.0.2/pypromql/result/
--rw-rw-rw-   0        0        0      148 2023-06-10 14:45:03.000000 PyPromql-0.0.2/pypromql/result/__init__.py
--rw-rw-rw-   0        0        0      783 2023-06-10 14:45:03.000000 PyPromql-0.0.2/pypromql/result/prometheus_metric.py
--rw-rw-rw-   0        0        0     1505 2023-06-10 14:45:03.000000 PyPromql-0.0.2/pypromql/result/prometheus_result.py
--rw-rw-rw-   0        0        0       42 2023-06-14 18:14:41.944084 PyPromql-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1284 2023-06-14 18:14:39.000000 PyPromql-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 18:14:41.940088 PyPromql-0.0.2/tests/
--rw-rw-rw-   0        0        0        0 2023-06-10 12:43:08.000000 PyPromql-0.0.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 18:14:41.941084 PyPromql-0.0.2/tests/query/
--rw-rw-rw-   0        0        0        0 2023-06-10 12:43:08.000000 PyPromql-0.0.2/tests/query/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-06-14 18:13:15.000000 PyPromql-0.0.2/tests/query/test_query.py
-drwxrwxrwx   0        0        0        0 2023-06-14 18:14:41.943084 PyPromql-0.0.2/tests/result/
--rw-rw-rw-   0        0        0        0 2023-06-10 14:45:03.000000 PyPromql-0.0.2/tests/result/__init__.py
--rw-rw-rw-   0        0        0     3646 2023-06-14 18:13:15.000000 PyPromql-0.0.2/tests/result/test_result.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:38:00.353052 PyPromql-0.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-06-09 16:49:37.000000 PyPromql-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2509 2023-06-14 20:38:00.351013 PyPromql-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 20:38:00.336012 PyPromql-0.0.3/PyPromql.egg-info/
+-rw-rw-rw-   0        0        0     2509 2023-06-14 20:38:00.000000 PyPromql-0.0.3/PyPromql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2023-06-14 20:38:00.000000 PyPromql-0.0.3/PyPromql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 20:38:00.000000 PyPromql-0.0.3/PyPromql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-14 20:38:00.000000 PyPromql-0.0.3/PyPromql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-14 20:38:00.000000 PyPromql-0.0.3/PyPromql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1633 2023-06-14 20:36:43.000000 PyPromql-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 20:38:00.338011 PyPromql-0.0.3/pypromql/
+-rw-rw-rw-   0        0        0       59 2023-06-14 18:13:15.000000 PyPromql-0.0.3/pypromql/__init__.py
+-rw-rw-rw-   0        0        0     2257 2023-06-14 18:13:15.000000 PyPromql-0.0.3/pypromql/connection.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:38:00.342013 PyPromql-0.0.3/pypromql/query/
+-rw-rw-rw-   0        0        0      160 2023-06-14 18:13:15.000000 PyPromql-0.0.3/pypromql/query/__init__.py
+-rw-rw-rw-   0        0        0      885 2023-06-10 12:43:08.000000 PyPromql-0.0.3/pypromql/query/prometheus_label.py
+-rw-rw-rw-   0        0        0      557 2023-06-10 12:43:08.000000 PyPromql-0.0.3/pypromql/query/prometheus_query.py
+-rw-rw-rw-   0        0        0     2853 2023-06-10 12:43:08.000000 PyPromql-0.0.3/pypromql/query/prometheus_query_builder.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:38:00.346013 PyPromql-0.0.3/pypromql/result/
+-rw-rw-rw-   0        0        0      148 2023-06-10 14:45:03.000000 PyPromql-0.0.3/pypromql/result/__init__.py
+-rw-rw-rw-   0        0        0      783 2023-06-10 14:45:03.000000 PyPromql-0.0.3/pypromql/result/prometheus_metric.py
+-rw-rw-rw-   0        0        0     1505 2023-06-10 14:45:03.000000 PyPromql-0.0.3/pypromql/result/prometheus_result.py
+-rw-rw-rw-   0        0        0       42 2023-06-14 20:38:00.353052 PyPromql-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1283 2023-06-14 20:36:43.000000 PyPromql-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:38:00.347014 PyPromql-0.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-10 12:43:08.000000 PyPromql-0.0.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:38:00.348012 PyPromql-0.0.3/tests/query/
+-rw-rw-rw-   0        0        0        0 2023-06-10 12:43:08.000000 PyPromql-0.0.3/tests/query/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-06-14 18:13:15.000000 PyPromql-0.0.3/tests/query/test_query.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:38:00.350013 PyPromql-0.0.3/tests/result/
+-rw-rw-rw-   0        0        0        0 2023-06-10 14:45:03.000000 PyPromql-0.0.3/tests/result/__init__.py
+-rw-rw-rw-   0        0        0     3646 2023-06-14 18:13:15.000000 PyPromql-0.0.3/tests/result/test_result.py
```

### Comparing `PyPromql-0.0.2/LICENSE` & `PyPromql-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPromql-0.0.2/PyPromql.egg-info/SOURCES.txt` & `PyPromql-0.0.3/PyPromql.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 LICENSE
-README.rst
+README.md
 setup.py
 PyPromql.egg-info/PKG-INFO
 PyPromql.egg-info/SOURCES.txt
 PyPromql.egg-info/dependency_links.txt
 PyPromql.egg-info/requires.txt
 PyPromql.egg-info/top_level.txt
 pypromql/__init__.py
```

### Comparing `PyPromql-0.0.2/pypromql/connection.py` & `PyPromql-0.0.3/pypromql/connection.py`

 * *Files identical despite different names*

### Comparing `PyPromql-0.0.2/pypromql/query/prometheus_label.py` & `PyPromql-0.0.3/pypromql/query/prometheus_label.py`

 * *Files identical despite different names*

### Comparing `PyPromql-0.0.2/pypromql/query/prometheus_query.py` & `PyPromql-0.0.3/pypromql/query/prometheus_query.py`

 * *Files identical despite different names*

### Comparing `PyPromql-0.0.2/pypromql/query/prometheus_query_builder.py` & `PyPromql-0.0.3/pypromql/query/prometheus_query_builder.py`

 * *Files identical despite different names*

### Comparing `PyPromql-0.0.2/pypromql/result/prometheus_metric.py` & `PyPromql-0.0.3/pypromql/result/prometheus_metric.py`

 * *Files identical despite different names*

### Comparing `PyPromql-0.0.2/pypromql/result/prometheus_result.py` & `PyPromql-0.0.3/pypromql/result/prometheus_result.py`

 * *Files identical despite different names*

### Comparing `PyPromql-0.0.2/setup.py` & `PyPromql-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 
 def get_readme_file():
-    with open('README.rst', 'r') as f:
+    with open('README.md', 'r') as f:
         return f.read()
 
 
 def get_requirements():
     with open('requirements.txt', 'r') as f:
         return f.read().splitlines()
 
 
 setup(
     name='PyPromql',
-    version='0.0.2',
+    version='0.0.3',
     author='Aviv Levi',
     author_email='60aviv60@gmail.com',
     description='PyPromql is a Python library that simplifies the creation and execution of PromQL queries.',
     long_description=get_readme_file(),
     long_description_content_type='text/markdown',
     url='https://github.com/aviv-levi/pypromql.git',
     packages=find_packages(),
```

### Comparing `PyPromql-0.0.2/tests/query/test_query.py` & `PyPromql-0.0.3/tests/query/test_query.py`

 * *Files identical despite different names*

### Comparing `PyPromql-0.0.2/tests/result/test_result.py` & `PyPromql-0.0.3/tests/result/test_result.py`

 * *Files identical despite different names*

