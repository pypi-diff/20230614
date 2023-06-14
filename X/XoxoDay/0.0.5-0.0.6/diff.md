# Comparing `tmp/XoxoDay-0.0.5.tar.gz` & `tmp/XoxoDay-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XoxoDay-0.0.5.tar", last modified: Wed Jun 14 20:46:54 2023, max compression
+gzip compressed data, was "XoxoDay-0.0.6.tar", last modified: Wed Jun 14 20:48:50 2023, max compression
```

## Comparing `XoxoDay-0.0.5.tar` & `XoxoDay-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:46:54.619804 XoxoDay-0.0.5/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.5/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1036 2023-06-14 20:46:54.619616 XoxoDay-0.0.5/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      532 2023-06-14 18:07:49.000000 XoxoDay-0.0.5/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:46:54.617535 XoxoDay-0.0.5/XoxoDay/
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:46:54.618535 XoxoDay-0.0.5/XoxoDay/XoxoDay.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1036 2023-06-14 20:46:54.000000 XoxoDay-0.0.5/XoxoDay/XoxoDay.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      424 2023-06-14 20:46:54.000000 XoxoDay-0.0.5/XoxoDay/XoxoDay.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-14 20:46:54.000000 XoxoDay-0.0.5/XoxoDay/XoxoDay.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-14 20:46:54.000000 XoxoDay-0.0.5/XoxoDay/XoxoDay.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       15 2023-06-14 20:46:54.000000 XoxoDay-0.0.5/XoxoDay/XoxoDay.egg-info/top_level.txt
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:46:54.618894 XoxoDay-0.0.5/XoxoDay/helper/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.5/XoxoDay/helper/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      469 2023-06-14 18:27:10.000000 XoxoDay-0.0.5/XoxoDay/helper/sqlite.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      947 2023-06-14 18:27:04.000000 XoxoDay-0.0.5/XoxoDay/helper/token.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:46:54.619382 XoxoDay-0.0.5/XoxoDay/service/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.5/XoxoDay/service/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1121 2023-06-14 18:07:04.000000 XoxoDay-0.0.5/XoxoDay/service/http_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1996 2023-06-14 20:31:24.000000 XoxoDay-0.0.5/XoxoDay/service/token_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1986 2023-06-14 20:33:58.000000 XoxoDay-0.0.5/XoxoDay/service/xoxoday_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-14 20:46:54.619847 XoxoDay-0.0.5/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      935 2023-06-14 20:46:47.000000 XoxoDay-0.0.5/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:48:50.941713 XoxoDay-0.0.6/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.6/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1036 2023-06-14 20:48:50.941599 XoxoDay-0.0.6/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      532 2023-06-14 18:07:49.000000 XoxoDay-0.0.6/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:48:50.939308 XoxoDay-0.0.6/XoxoDay/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      162 2023-06-14 20:34:00.000000 XoxoDay-0.0.6/XoxoDay/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      479 2023-06-14 19:45:14.000000 XoxoDay-0.0.6/XoxoDay/exception.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:48:50.940523 XoxoDay-0.0.6/XoxoDay/helper/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.6/XoxoDay/helper/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      469 2023-06-14 18:27:10.000000 XoxoDay-0.0.6/XoxoDay/helper/sqlite.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      947 2023-06-14 18:27:04.000000 XoxoDay-0.0.6/XoxoDay/helper/token.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.6/XoxoDay/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:48:50.941300 XoxoDay-0.0.6/XoxoDay/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.6/XoxoDay/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1121 2023-06-14 18:07:04.000000 XoxoDay-0.0.6/XoxoDay/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1996 2023-06-14 20:31:24.000000 XoxoDay-0.0.6/XoxoDay/service/token_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1986 2023-06-14 20:33:58.000000 XoxoDay-0.0.6/XoxoDay/service/xoxoday_service.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:48:50.940048 XoxoDay-0.0.6/XoxoDay.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1036 2023-06-14 20:48:50.000000 XoxoDay-0.0.6/XoxoDay.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      447 2023-06-14 20:48:50.000000 XoxoDay-0.0.6/XoxoDay.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-14 20:48:50.000000 XoxoDay-0.0.6/XoxoDay.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-14 20:48:50.000000 XoxoDay-0.0.6/XoxoDay.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-14 20:48:50.000000 XoxoDay-0.0.6/XoxoDay.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-14 20:48:50.941752 XoxoDay-0.0.6/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      909 2023-06-14 20:48:43.000000 XoxoDay-0.0.6/setup.py
```

### Comparing `XoxoDay-0.0.5/LICENSE` & `XoxoDay-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.5/PKG-INFO` & `XoxoDay-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.5
+Version: 0.0.6
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.5/README.md` & `XoxoDay-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.5/XoxoDay/XoxoDay.egg-info/PKG-INFO` & `XoxoDay-0.0.6/XoxoDay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.5
+Version: 0.0.6
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.5/XoxoDay/helper/token.py` & `XoxoDay-0.0.6/XoxoDay/helper/token.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.5/XoxoDay/service/http_service.py` & `XoxoDay-0.0.6/XoxoDay/service/http_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.5/XoxoDay/service/token_service.py` & `XoxoDay-0.0.6/XoxoDay/service/token_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.5/XoxoDay/service/xoxoday_service.py` & `XoxoDay-0.0.6/XoxoDay/service/xoxoday_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.5/setup.py` & `XoxoDay-0.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='XoxoDay',
-    version="0.0.5",
+    version="0.0.6",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='XoxoDay Api Client For Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/XoxoDay.git',
     project_urls={
@@ -18,12 +18,11 @@
     },
     install_requires=['requests', 'python-dotenv'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    packages=setuptools.find_packages(where="XoxoDay"),
-    package_dir={"": "XoxoDay"},
+    packages=['XoxoDay', 'XoxoDay.service', 'XoxoDay.helper'],
     include_package_data=True,
     python_requires=">=3.6",
 )
```

