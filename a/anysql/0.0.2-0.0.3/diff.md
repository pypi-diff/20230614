# Comparing `tmp/anysql-0.0.2.tar.gz` & `tmp/anysql-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anysql-0.0.2.tar", last modified: Wed Jun 14 07:48:55 2023, max compression
+gzip compressed data, was "anysql-0.0.3.tar", last modified: Wed Jun 14 07:55:30 2023, max compression
```

## Comparing `anysql-0.0.2.tar` & `anysql-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-14 07:48:55.259755 anysql-0.0.2/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-06-14 00:44:55.000000 anysql-0.0.2/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2406 2023-06-14 07:48:55.259755 anysql-0.0.2/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1879 2023-06-14 07:28:25.000000 anysql-0.0.2/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-14 07:48:55.255755 anysql-0.0.2/anysql/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      175 2023-06-13 08:04:12.000000 anysql-0.0.2/anysql/__init__.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-14 07:48:55.259755 anysql-0.0.2/anysql/backends/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      534 2023-06-14 01:42:04.000000 anysql-0.0.2/anysql/backends/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5269 2023-06-14 02:41:35.000000 anysql-0.0.2/anysql/backends/postgres.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5257 2023-06-14 02:41:54.000000 anysql-0.0.2/anysql/backends/pymysql.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     7911 2023-06-14 01:23:29.000000 anysql-0.0.2/anysql/backends/sqlite.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)    11297 2023-06-14 03:20:36.000000 anysql-0.0.2/anysql/core.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     6715 2023-06-14 02:45:10.000000 anysql-0.0.2/anysql/escape.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     3365 2023-06-14 07:43:02.000000 anysql-0.0.2/anysql/interface.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)        0 2023-06-13 09:09:08.000000 anysql-0.0.2/anysql/py.typed
--rw-r--r--   0 andrew    (1000) andrew    (1000)     3412 2023-06-13 04:49:43.000000 anysql-0.0.2/anysql/uri.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-14 07:48:55.255755 anysql-0.0.2/anysql.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2406 2023-06-14 07:48:55.000000 anysql-0.0.2/anysql.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      385 2023-06-14 07:48:55.000000 anysql-0.0.2/anysql.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-06-14 07:48:55.000000 anysql-0.0.2/anysql.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       89 2023-06-14 07:48:55.000000 anysql-0.0.2/anysql.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        7 2023-06-14 07:48:55.000000 anysql-0.0.2/anysql.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-06-14 07:48:55.259755 anysql-0.0.2/setup.cfg
--rw-r--r--   0 andrew    (1000) andrew    (1000)      935 2023-06-14 07:48:36.000000 anysql-0.0.2/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-14 07:55:30.424768 anysql-0.0.3/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-06-14 00:44:55.000000 anysql-0.0.3/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2406 2023-06-14 07:55:30.424768 anysql-0.0.3/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1879 2023-06-14 07:28:25.000000 anysql-0.0.3/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-14 07:55:30.424768 anysql-0.0.3/anysql/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      175 2023-06-13 08:04:12.000000 anysql-0.0.3/anysql/__init__.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-14 07:55:30.424768 anysql-0.0.3/anysql/backends/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      534 2023-06-14 01:42:04.000000 anysql-0.0.3/anysql/backends/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     5269 2023-06-14 02:41:35.000000 anysql-0.0.3/anysql/backends/postgres.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     5257 2023-06-14 02:41:54.000000 anysql-0.0.3/anysql/backends/pymysql.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     7911 2023-06-14 01:23:29.000000 anysql-0.0.3/anysql/backends/sqlite.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)    11297 2023-06-14 03:20:36.000000 anysql-0.0.3/anysql/core.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     6715 2023-06-14 02:45:10.000000 anysql-0.0.3/anysql/escape.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     3365 2023-06-14 07:43:02.000000 anysql-0.0.3/anysql/interface.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)        0 2023-06-13 09:09:08.000000 anysql-0.0.3/anysql/py.typed
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     3412 2023-06-13 04:49:43.000000 anysql-0.0.3/anysql/uri.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-14 07:55:30.424768 anysql-0.0.3/anysql.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2406 2023-06-14 07:55:30.000000 anysql-0.0.3/anysql.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      385 2023-06-14 07:55:30.000000 anysql-0.0.3/anysql.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-06-14 07:55:30.000000 anysql-0.0.3/anysql.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       97 2023-06-14 07:55:30.000000 anysql-0.0.3/anysql.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        7 2023-06-14 07:55:30.000000 anysql-0.0.3/anysql.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-06-14 07:55:30.424768 anysql-0.0.3/setup.cfg
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      954 2023-06-14 07:54:49.000000 anysql-0.0.3/setup.py
```

### Comparing `anysql-0.0.2/LICENSE` & `anysql-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anysql-0.0.2/PKG-INFO` & `anysql-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anysql
-Version: 0.0.2
+Version: 0.0.3
 Summary: Lightweight, Thread-Safe, Version-Agnostic, SQL Client Implementation
 Home-page: https://github.com/imgurbot12/anysql
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `anysql-0.0.2/README.md` & `anysql-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `anysql-0.0.2/anysql/backends/__init__.py` & `anysql-0.0.3/anysql/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `anysql-0.0.2/anysql/backends/postgres.py` & `anysql-0.0.3/anysql/backends/postgres.py`

 * *Files identical despite different names*

### Comparing `anysql-0.0.2/anysql/backends/pymysql.py` & `anysql-0.0.3/anysql/backends/pymysql.py`

 * *Files identical despite different names*

### Comparing `anysql-0.0.2/anysql/backends/sqlite.py` & `anysql-0.0.3/anysql/backends/sqlite.py`

 * *Files identical despite different names*

### Comparing `anysql-0.0.2/anysql/core.py` & `anysql-0.0.3/anysql/core.py`

 * *Files identical despite different names*

### Comparing `anysql-0.0.2/anysql/escape.py` & `anysql-0.0.3/anysql/escape.py`

 * *Files identical despite different names*

### Comparing `anysql-0.0.2/anysql/interface.py` & `anysql-0.0.3/anysql/interface.py`

 * *Files identical despite different names*

### Comparing `anysql-0.0.2/anysql/uri.py` & `anysql-0.0.3/anysql/uri.py`

 * *Files identical despite different names*

### Comparing `anysql-0.0.2/anysql.egg-info/PKG-INFO` & `anysql-0.0.3/anysql.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anysql
-Version: 0.0.2
+Version: 0.0.3
 Summary: Lightweight, Thread-Safe, Version-Agnostic, SQL Client Implementation
 Home-page: https://github.com/imgurbot12/anysql
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `anysql-0.0.2/setup.py` & `anysql-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='anysql',
-    version='0.0.2',
+    version='0.0.3',
     license='MIT',
     packages=find_packages(),
     url='https://github.com/imgurbot12/anysql',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     description='Lightweight, Thread-Safe, Version-Agnostic, SQL Client Implementation',
     python_requires='>=3.7',
     long_description=readme,
     long_description_content_type="text/markdown",
     package_data={"anysql": ["py.typed"]},
     install_requires=[
+        'pypool3',
         'dataclasses',
         'contextvars',
         'typing_extensions',
     ],
     extras_require={
         "mysql":      ["pymysql"],
         "postgresql": ["psycopg2-binary"],
```

