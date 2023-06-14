# Comparing `tmp/XoxoDay-0.0.8.tar.gz` & `tmp/XoxoDay-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XoxoDay-0.0.8.tar", last modified: Wed Jun 14 20:52:42 2023, max compression
+gzip compressed data, was "XoxoDay-0.0.9.tar", last modified: Wed Jun 14 21:13:27 2023, max compression
```

## Comparing `XoxoDay-0.0.8.tar` & `XoxoDay-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:52:42.290470 XoxoDay-0.0.8/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.8/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1036 2023-06-14 20:52:42.290335 XoxoDay-0.0.8/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      532 2023-06-14 18:07:49.000000 XoxoDay-0.0.8/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:52:42.287495 XoxoDay-0.0.8/XoxoDay/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      162 2023-06-14 20:34:00.000000 XoxoDay-0.0.8/XoxoDay/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      479 2023-06-14 19:45:14.000000 XoxoDay-0.0.8/XoxoDay/exception.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:52:42.288819 XoxoDay-0.0.8/XoxoDay/helper/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.8/XoxoDay/helper/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      469 2023-06-14 18:27:10.000000 XoxoDay-0.0.8/XoxoDay/helper/sqlite.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      947 2023-06-14 18:27:04.000000 XoxoDay-0.0.8/XoxoDay/helper/token.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.8/XoxoDay/serializer.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:52:42.289998 XoxoDay-0.0.8/XoxoDay/service/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.8/XoxoDay/service/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1121 2023-06-14 18:07:04.000000 XoxoDay-0.0.8/XoxoDay/service/http_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1996 2023-06-14 20:31:24.000000 XoxoDay-0.0.8/XoxoDay/service/token_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      842 2023-06-14 20:32:06.000000 XoxoDay-0.0.8/XoxoDay/service/voucher.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1986 2023-06-14 20:33:58.000000 XoxoDay-0.0.8/XoxoDay/service/xoxoday_service.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 20:52:42.288267 XoxoDay-0.0.8/XoxoDay.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1036 2023-06-14 20:52:42.000000 XoxoDay-0.0.8/XoxoDay.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      476 2023-06-14 20:52:42.000000 XoxoDay-0.0.8/XoxoDay.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-14 20:52:42.000000 XoxoDay-0.0.8/XoxoDay.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-14 20:52:42.000000 XoxoDay-0.0.8/XoxoDay.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-14 20:52:42.000000 XoxoDay-0.0.8/XoxoDay.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-14 20:52:42.290517 XoxoDay-0.0.8/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      944 2023-06-14 20:52:21.000000 XoxoDay-0.0.8/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 21:13:27.688422 XoxoDay-0.0.9/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.9/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1036 2023-06-14 21:13:27.688263 XoxoDay-0.0.9/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      532 2023-06-14 18:07:49.000000 XoxoDay-0.0.9/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 21:13:27.684661 XoxoDay-0.0.9/XoxoDay/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      162 2023-06-14 20:34:00.000000 XoxoDay-0.0.9/XoxoDay/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      479 2023-06-14 19:45:14.000000 XoxoDay-0.0.9/XoxoDay/exception.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 21:13:27.686371 XoxoDay-0.0.9/XoxoDay/helper/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.9/XoxoDay/helper/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      469 2023-06-14 18:27:10.000000 XoxoDay-0.0.9/XoxoDay/helper/sqlite.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      947 2023-06-14 18:27:04.000000 XoxoDay-0.0.9/XoxoDay/helper/token.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.9/XoxoDay/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 21:13:27.687859 XoxoDay-0.0.9/XoxoDay/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.9/XoxoDay/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1121 2023-06-14 18:07:04.000000 XoxoDay-0.0.9/XoxoDay/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1996 2023-06-14 20:31:24.000000 XoxoDay-0.0.9/XoxoDay/service/token_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.9/XoxoDay/service/voucher.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2677 2023-06-14 21:13:11.000000 XoxoDay-0.0.9/XoxoDay/service/xoxoday_service.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 21:13:27.685734 XoxoDay-0.0.9/XoxoDay.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1036 2023-06-14 21:13:27.000000 XoxoDay-0.0.9/XoxoDay.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      476 2023-06-14 21:13:27.000000 XoxoDay-0.0.9/XoxoDay.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-14 21:13:27.000000 XoxoDay-0.0.9/XoxoDay.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-14 21:13:27.000000 XoxoDay-0.0.9/XoxoDay.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-14 21:13:27.000000 XoxoDay-0.0.9/XoxoDay.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-14 21:13:27.688473 XoxoDay-0.0.9/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      944 2023-06-14 21:13:19.000000 XoxoDay-0.0.9/setup.py
```

### Comparing `XoxoDay-0.0.8/LICENSE` & `XoxoDay-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.8/PKG-INFO` & `XoxoDay-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.8
+Version: 0.0.9
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.8/README.md` & `XoxoDay-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.8/XoxoDay/helper/token.py` & `XoxoDay-0.0.9/XoxoDay/helper/token.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.8/XoxoDay/service/http_service.py` & `XoxoDay-0.0.9/XoxoDay/service/http_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.8/XoxoDay/service/token_service.py` & `XoxoDay-0.0.9/XoxoDay/service/token_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.8/XoxoDay.egg-info/PKG-INFO` & `XoxoDay-0.0.9/XoxoDay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.8
+Version: 0.0.9
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

