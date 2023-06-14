# Comparing `tmp/XoxoDay-0.0.1.tar.gz` & `tmp/XoxoDay-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XoxoDay-0.0.1.tar", last modified: Wed Jun 14 18:09:45 2023, max compression
+gzip compressed data, was "XoxoDay-0.0.2.tar", last modified: Wed Jun 14 20:34:09 2023, max compression
```

## Comparing `XoxoDay-0.0.1.tar` & `XoxoDay-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:09:45.480816 XoxoDay-0.0.1/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.1/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1036 2023-06-14 18:09:45.480672 XoxoDay-0.0.1/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      532 2023-06-14 18:07:49.000000 XoxoDay-0.0.1/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:09:45.477965 XoxoDay-0.0.1/XoxoDay/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      146 2023-06-14 18:09:38.000000 XoxoDay-0.0.1/XoxoDay/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      430 2023-06-14 18:07:04.000000 XoxoDay-0.0.1/XoxoDay/exception.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:09:45.479340 XoxoDay-0.0.1/XoxoDay/helper/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.1/XoxoDay/helper/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      459 2023-06-14 18:07:04.000000 XoxoDay-0.0.1/XoxoDay/helper/sqlite.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      937 2023-06-14 18:07:04.000000 XoxoDay-0.0.1/XoxoDay/helper/token.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.1/XoxoDay/serializer.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:09:45.480377 XoxoDay-0.0.1/XoxoDay/service/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      122 2023-06-14 18:07:04.000000 XoxoDay-0.0.1/XoxoDay/service/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1121 2023-06-14 18:07:04.000000 XoxoDay-0.0.1/XoxoDay/service/http_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1141 2023-06-14 18:07:04.000000 XoxoDay-0.0.1/XoxoDay/service/token_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1627 2023-06-14 18:07:04.000000 XoxoDay-0.0.1/XoxoDay/service/xoxoday_service.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:09:45.478832 XoxoDay-0.0.1/XoxoDay.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1036 2023-06-14 18:09:45.000000 XoxoDay-0.0.1/XoxoDay.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      447 2023-06-14 18:09:45.000000 XoxoDay-0.0.1/XoxoDay.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-14 18:09:45.000000 XoxoDay-0.0.1/XoxoDay.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-14 18:09:45.000000 XoxoDay-0.0.1/XoxoDay.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-14 18:09:45.000000 XoxoDay-0.0.1/XoxoDay.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-14 18:09:45.480862 XoxoDay-0.0.1/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      878 2023-06-14 18:08:18.000000 XoxoDay-0.0.1/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:34:09.746560 XoxoDay-0.0.2/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.2/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1036 2023-06-14 20:34:09.746402 XoxoDay-0.0.2/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      532 2023-06-14 18:07:49.000000 XoxoDay-0.0.2/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:34:09.743973 XoxoDay-0.0.2/XoxoDay/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      162 2023-06-14 20:34:00.000000 XoxoDay-0.0.2/XoxoDay/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      479 2023-06-14 19:45:14.000000 XoxoDay-0.0.2/XoxoDay/exception.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:34:09.745247 XoxoDay-0.0.2/XoxoDay/helper/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.2/XoxoDay/helper/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      469 2023-06-14 18:27:10.000000 XoxoDay-0.0.2/XoxoDay/helper/sqlite.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      947 2023-06-14 18:27:04.000000 XoxoDay-0.0.2/XoxoDay/helper/token.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.2/XoxoDay/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:34:09.746029 XoxoDay-0.0.2/XoxoDay/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.2/XoxoDay/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1121 2023-06-14 18:07:04.000000 XoxoDay-0.0.2/XoxoDay/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1996 2023-06-14 20:31:24.000000 XoxoDay-0.0.2/XoxoDay/service/token_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1986 2023-06-14 20:33:58.000000 XoxoDay-0.0.2/XoxoDay/service/xoxoday_service.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:34:09.744771 XoxoDay-0.0.2/XoxoDay.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1036 2023-06-14 20:34:09.000000 XoxoDay-0.0.2/XoxoDay.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      447 2023-06-14 20:34:09.000000 XoxoDay-0.0.2/XoxoDay.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-14 20:34:09.000000 XoxoDay-0.0.2/XoxoDay.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-14 20:34:09.000000 XoxoDay-0.0.2/XoxoDay.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-14 20:34:09.000000 XoxoDay-0.0.2/XoxoDay.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-14 20:34:09.746613 XoxoDay-0.0.2/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      878 2023-06-14 20:33:58.000000 XoxoDay-0.0.2/setup.py
```

### Comparing `XoxoDay-0.0.1/LICENSE` & `XoxoDay-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.1/PKG-INFO` & `XoxoDay-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.1
+Version: 0.0.2
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.1/README.md` & `XoxoDay-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.1/XoxoDay/helper/token.py` & `XoxoDay-0.0.2/XoxoDay/helper/token.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import sqlite3 as lite
 
-from XoxoDay import XoxoDayException
+from XoxoDay.exception import XoxoDayException
 from XoxoDay.serializer import Serializer
 
 sql_path = f'{os.path.dirname(os.path.abspath(__file__))}/logo_rest.sqlite'
 
 
 def get_token():
     try:
```

### Comparing `XoxoDay-0.0.1/XoxoDay/service/http_service.py` & `XoxoDay-0.0.2/XoxoDay/service/http_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.1/XoxoDay.egg-info/PKG-INFO` & `XoxoDay-0.0.2/XoxoDay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.1
+Version: 0.0.2
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.1/setup.py` & `XoxoDay-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='XoxoDay',
-    version="0.0.1",
+    version="0.0.2",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='XoxoDay Api Client For Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/XoxoDay.git',
     project_urls={
```

