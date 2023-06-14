# Comparing `tmp/XoxoDay-0.0.3.tar.gz` & `tmp/XoxoDay-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XoxoDay-0.0.3.tar", last modified: Wed Jun 14 20:40:21 2023, max compression
+gzip compressed data, was "XoxoDay-0.0.4.tar", last modified: Wed Jun 14 20:43:33 2023, max compression
```

## Comparing `XoxoDay-0.0.3.tar` & `XoxoDay-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:40:21.926709 XoxoDay-0.0.3/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.3/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1036 2023-06-14 20:40:21.926580 XoxoDay-0.0.3/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      532 2023-06-14 18:07:49.000000 XoxoDay-0.0.3/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:40:21.924180 XoxoDay-0.0.3/XoxoDay/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      162 2023-06-14 20:34:00.000000 XoxoDay-0.0.3/XoxoDay/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      479 2023-06-14 19:45:14.000000 XoxoDay-0.0.3/XoxoDay/exception.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:40:21.925436 XoxoDay-0.0.3/XoxoDay/helper/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.3/XoxoDay/helper/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      469 2023-06-14 18:27:10.000000 XoxoDay-0.0.3/XoxoDay/helper/sqlite.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      947 2023-06-14 18:27:04.000000 XoxoDay-0.0.3/XoxoDay/helper/token.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.3/XoxoDay/serializer.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:40:21.926263 XoxoDay-0.0.3/XoxoDay/service/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.3/XoxoDay/service/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1121 2023-06-14 18:07:04.000000 XoxoDay-0.0.3/XoxoDay/service/http_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1996 2023-06-14 20:31:24.000000 XoxoDay-0.0.3/XoxoDay/service/token_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1986 2023-06-14 20:33:58.000000 XoxoDay-0.0.3/XoxoDay/service/xoxoday_service.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:40:21.924957 XoxoDay-0.0.3/XoxoDay.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1036 2023-06-14 20:40:21.000000 XoxoDay-0.0.3/XoxoDay.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      447 2023-06-14 20:40:21.000000 XoxoDay-0.0.3/XoxoDay.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-14 20:40:21.000000 XoxoDay-0.0.3/XoxoDay.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-14 20:40:21.000000 XoxoDay-0.0.3/XoxoDay.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-14 20:40:21.000000 XoxoDay-0.0.3/XoxoDay.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-14 20:40:21.926756 XoxoDay-0.0.3/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      942 2023-06-14 20:40:14.000000 XoxoDay-0.0.3/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:43:33.074683 XoxoDay-0.0.4/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.4/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1036 2023-06-14 20:43:33.074507 XoxoDay-0.0.4/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      532 2023-06-14 18:07:49.000000 XoxoDay-0.0.4/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:43:33.070561 XoxoDay-0.0.4/XoxoDay/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      162 2023-06-14 20:34:00.000000 XoxoDay-0.0.4/XoxoDay/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      479 2023-06-14 19:45:14.000000 XoxoDay-0.0.4/XoxoDay/exception.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:43:33.072870 XoxoDay-0.0.4/XoxoDay/helper/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.4/XoxoDay/helper/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      469 2023-06-14 18:27:10.000000 XoxoDay-0.0.4/XoxoDay/helper/sqlite.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      947 2023-06-14 18:27:04.000000 XoxoDay-0.0.4/XoxoDay/helper/token.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.4/XoxoDay/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:43:33.074131 XoxoDay-0.0.4/XoxoDay/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.4/XoxoDay/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1121 2023-06-14 18:07:04.000000 XoxoDay-0.0.4/XoxoDay/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1996 2023-06-14 20:31:24.000000 XoxoDay-0.0.4/XoxoDay/service/token_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      842 2023-06-14 20:32:06.000000 XoxoDay-0.0.4/XoxoDay/service/voucher.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1986 2023-06-14 20:33:58.000000 XoxoDay-0.0.4/XoxoDay/service/xoxoday_service.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:43:33.072253 XoxoDay-0.0.4/XoxoDay.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1036 2023-06-14 20:43:33.000000 XoxoDay-0.0.4/XoxoDay.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      476 2023-06-14 20:43:33.000000 XoxoDay-0.0.4/XoxoDay.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-14 20:43:33.000000 XoxoDay-0.0.4/XoxoDay.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-14 20:43:33.000000 XoxoDay-0.0.4/XoxoDay.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-14 20:43:33.000000 XoxoDay-0.0.4/XoxoDay.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-14 20:43:33.074744 XoxoDay-0.0.4/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      942 2023-06-14 20:43:23.000000 XoxoDay-0.0.4/setup.py
```

### Comparing `XoxoDay-0.0.3/LICENSE` & `XoxoDay-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.3/PKG-INFO` & `XoxoDay-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.3
+Version: 0.0.4
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.3/README.md` & `XoxoDay-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.3/XoxoDay/helper/token.py` & `XoxoDay-0.0.4/XoxoDay/helper/token.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.3/XoxoDay/service/http_service.py` & `XoxoDay-0.0.4/XoxoDay/service/http_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.3/XoxoDay/service/token_service.py` & `XoxoDay-0.0.4/XoxoDay/service/token_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.3/XoxoDay/service/xoxoday_service.py` & `XoxoDay-0.0.4/XoxoDay/service/xoxoday_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.3/XoxoDay.egg-info/PKG-INFO` & `XoxoDay-0.0.4/XoxoDay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.3
+Version: 0.0.4
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.3/setup.py` & `XoxoDay-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='XoxoDay',
-    version="0.0.3",
+    version="0.0.4",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='XoxoDay Api Client For Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/XoxoDay.git',
     project_urls={
@@ -19,10 +19,10 @@
     install_requires=['requests', 'python-dotenv'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=['XoxoDay', 'XoxoDay.service', 'XoxoDay.helper'],
-    package_data={'XoxoDay': ['XoxoDay/service/voucher.json']},
+    data_files=[('voucher', ['XoxoDay/service/voucher.json'])],
     python_requires=">=3.6",
 )
```

