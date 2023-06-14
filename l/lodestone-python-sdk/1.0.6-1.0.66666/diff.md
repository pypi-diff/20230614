# Comparing `tmp/lodestone-python-sdk-1.0.6.tar.gz` & `tmp/lodestone-python-sdk-1.0.66666.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lodestone-python-sdk-1.0.6.tar", last modified: Wed Jun 14 09:32:08 2023, max compression
+gzip compressed data, was "lodestone-python-sdk-1.0.66666.tar", last modified: Wed Jun 14 09:31:00 2023, max compression
```

## Comparing `lodestone-python-sdk-1.0.6.tar` & `lodestone-python-sdk-1.0.66666.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-14 09:32:08.091626 lodestone-python-sdk-1.0.6/
--rw-r--r--   0 bocai      (501) staff       (20)      518 2023-06-14 09:32:08.091511 lodestone-python-sdk-1.0.6/PKG-INFO
--rw-r--r--   0 bocai      (501) staff       (20)      248 2023-06-13 08:22:58.000000 lodestone-python-sdk-1.0.6/README.md
-drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-14 09:32:08.090752 lodestone-python-sdk-1.0.6/lodestone_python_sdk/
--rw-r--r--   0 bocai      (501) staff       (20)        0 2023-06-13 09:41:00.000000 lodestone-python-sdk-1.0.6/lodestone_python_sdk/__init__.py
--rw-r--r--   0 bocai      (501) staff       (20)      697 2023-06-13 09:41:00.000000 lodestone-python-sdk-1.0.6/lodestone_python_sdk/auth_client.py
--rw-r--r--   0 bocai      (501) staff       (20)       42 2023-06-13 09:41:00.000000 lodestone-python-sdk-1.0.6/lodestone_python_sdk/exceptions.py
-drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-14 09:32:08.091357 lodestone-python-sdk-1.0.6/lodestone_python_sdk.egg-info/
--rw-r--r--   0 bocai      (501) staff       (20)      518 2023-06-14 09:32:08.000000 lodestone-python-sdk-1.0.6/lodestone_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 bocai      (501) staff       (20)      341 2023-06-14 09:32:08.000000 lodestone-python-sdk-1.0.6/lodestone_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 bocai      (501) staff       (20)        1 2023-06-14 09:32:08.000000 lodestone-python-sdk-1.0.6/lodestone_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 bocai      (501) staff       (20)       21 2023-06-14 09:32:08.000000 lodestone-python-sdk-1.0.6/lodestone_python_sdk.egg-info/requires.txt
--rw-r--r--   0 bocai      (501) staff       (20)       21 2023-06-14 09:32:08.000000 lodestone-python-sdk-1.0.6/lodestone_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 bocai      (501) staff       (20)       38 2023-06-14 09:32:08.091671 lodestone-python-sdk-1.0.6/setup.cfg
--rw-r--r--   0 bocai      (501) staff       (20)      502 2023-06-14 09:31:58.000000 lodestone-python-sdk-1.0.6/setup.py
+drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-14 09:31:00.506024 lodestone-python-sdk-1.0.66666/
+-rw-r--r--   0 bocai      (501) staff       (20)      522 2023-06-14 09:31:00.505886 lodestone-python-sdk-1.0.66666/PKG-INFO
+-rw-r--r--   0 bocai      (501) staff       (20)      248 2023-06-13 08:22:58.000000 lodestone-python-sdk-1.0.66666/README.md
+drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-14 09:31:00.505118 lodestone-python-sdk-1.0.66666/lodestone_python_sdk/
+-rw-r--r--   0 bocai      (501) staff       (20)        0 2023-06-13 09:41:00.000000 lodestone-python-sdk-1.0.66666/lodestone_python_sdk/__init__.py
+-rw-r--r--   0 bocai      (501) staff       (20)      697 2023-06-13 09:41:00.000000 lodestone-python-sdk-1.0.66666/lodestone_python_sdk/auth_client.py
+-rw-r--r--   0 bocai      (501) staff       (20)       42 2023-06-13 09:41:00.000000 lodestone-python-sdk-1.0.66666/lodestone_python_sdk/exceptions.py
+drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-14 09:31:00.505667 lodestone-python-sdk-1.0.66666/lodestone_python_sdk.egg-info/
+-rw-r--r--   0 bocai      (501) staff       (20)      522 2023-06-14 09:31:00.000000 lodestone-python-sdk-1.0.66666/lodestone_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 bocai      (501) staff       (20)      341 2023-06-14 09:31:00.000000 lodestone-python-sdk-1.0.66666/lodestone_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 bocai      (501) staff       (20)        1 2023-06-14 09:31:00.000000 lodestone-python-sdk-1.0.66666/lodestone_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 bocai      (501) staff       (20)       21 2023-06-14 09:31:00.000000 lodestone-python-sdk-1.0.66666/lodestone_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 bocai      (501) staff       (20)       21 2023-06-14 09:31:00.000000 lodestone-python-sdk-1.0.66666/lodestone_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 bocai      (501) staff       (20)       38 2023-06-14 09:31:00.506075 lodestone-python-sdk-1.0.66666/setup.cfg
+-rw-r--r--   0 bocai      (501) staff       (20)      506 2023-06-14 09:30:30.000000 lodestone-python-sdk-1.0.66666/setup.py
```

### Comparing `lodestone-python-sdk-1.0.6/PKG-INFO` & `lodestone-python-sdk-1.0.66666/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lodestone-python-sdk
-Version: 1.0.6
+Version: 1.0.66666
 Summary: Auth to tuyoo's Lodestone
 Home-page: UNKNOWN
 Author: bocai
 Author-email: peijianbo@tuyoogame.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >3.2
```

### Comparing `lodestone-python-sdk-1.0.6/lodestone_python_sdk/auth_client.py` & `lodestone-python-sdk-1.0.66666/lodestone_python_sdk/auth_client.py`

 * *Files identical despite different names*

### Comparing `lodestone-python-sdk-1.0.6/lodestone_python_sdk.egg-info/PKG-INFO` & `lodestone-python-sdk-1.0.66666/lodestone_python_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lodestone-python-sdk
-Version: 1.0.6
+Version: 1.0.66666
 Summary: Auth to tuyoo's Lodestone
 Home-page: UNKNOWN
 Author: bocai
 Author-email: peijianbo@tuyoogame.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >3.2
```

