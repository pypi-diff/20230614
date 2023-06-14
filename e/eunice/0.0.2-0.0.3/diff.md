# Comparing `tmp/eunice-0.0.2.tar.gz` & `tmp/eunice-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eunice-0.0.2.tar", last modified: Wed Jun 14 11:56:39 2023, max compression
+gzip compressed data, was "eunice-0.0.3.tar", last modified: Wed Jun 14 12:13:25 2023, max compression
```

## Comparing `eunice-0.0.2.tar` & `eunice-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2023-06-14 11:56:39.929982 eunice-0.0.2/
--rw-r--r--   0 rob        (501) staff       (20)     1059 2023-06-13 19:41:25.000000 eunice-0.0.2/LICENCE
--rw-r--r--   0 rob        (501) staff       (20)      785 2023-06-14 11:56:39.929799 eunice-0.0.2/PKG-INFO
--rw-r--r--   0 rob        (501) staff       (20)      188 2023-06-13 18:24:10.000000 eunice-0.0.2/README.md
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2023-06-14 11:56:39.928712 eunice-0.0.2/eunice/
--rw-r--r--   0 rob        (501) staff       (20)        0 2023-06-13 16:21:12.000000 eunice-0.0.2/eunice/__init__.py
--rw-r--r--   0 rob        (501) staff       (20)      292 2023-06-13 20:15:39.000000 eunice-0.0.2/eunice/__main__.py
--rw-r--r--   0 rob        (501) staff       (20)      353 2023-06-13 17:14:12.000000 eunice-0.0.2/eunice/args.py
--rw-r--r--   0 rob        (501) staff       (20)      252 2023-06-13 20:15:39.000000 eunice-0.0.2/eunice/cmdline.py
--rw-r--r--   0 rob        (501) staff       (20)      283 2023-06-13 16:57:48.000000 eunice-0.0.2/eunice/definitions.py
--rw-r--r--   0 rob        (501) staff       (20)      680 2023-06-13 17:16:17.000000 eunice-0.0.2/eunice/eunice_logging.py
--rw-r--r--   0 rob        (501) staff       (20)     1116 2023-06-13 17:29:52.000000 eunice-0.0.2/eunice/models.py
--rw-r--r--   0 rob        (501) staff       (20)     1980 2023-06-14 11:50:59.000000 eunice-0.0.2/eunice/run.py
--rw-r--r--   0 rob        (501) staff       (20)      325 2023-06-13 17:21:32.000000 eunice-0.0.2/eunice/utils.py
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2023-06-14 11:56:39.929618 eunice-0.0.2/eunice.egg-info/
--rw-r--r--   0 rob        (501) staff       (20)      785 2023-06-14 11:56:39.000000 eunice-0.0.2/eunice.egg-info/PKG-INFO
--rw-r--r--   0 rob        (501) staff       (20)      402 2023-06-14 11:56:39.000000 eunice-0.0.2/eunice.egg-info/SOURCES.txt
--rw-r--r--   0 rob        (501) staff       (20)        1 2023-06-14 11:56:39.000000 eunice-0.0.2/eunice.egg-info/dependency_links.txt
--rw-r--r--   0 rob        (501) staff       (20)       47 2023-06-14 11:56:39.000000 eunice-0.0.2/eunice.egg-info/entry_points.txt
--rw-r--r--   0 rob        (501) staff       (20)        1 2023-06-13 18:19:23.000000 eunice-0.0.2/eunice.egg-info/not-zip-safe
--rw-r--r--   0 rob        (501) staff       (20)       13 2023-06-14 11:56:39.000000 eunice-0.0.2/eunice.egg-info/requires.txt
--rw-r--r--   0 rob        (501) staff       (20)        7 2023-06-14 11:56:39.000000 eunice-0.0.2/eunice.egg-info/top_level.txt
--rw-r--r--   0 rob        (501) staff       (20)       38 2023-06-14 11:56:39.930043 eunice-0.0.2/setup.cfg
--rw-r--r--   0 rob        (501) staff       (20)      971 2023-06-14 11:52:03.000000 eunice-0.0.2/setup.py
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2023-06-14 12:13:25.438298 eunice-0.0.3/
+-rw-r--r--   0 rob        (501) staff       (20)     1059 2023-06-13 19:41:25.000000 eunice-0.0.3/LICENCE
+-rw-r--r--   0 rob        (501) staff       (20)      785 2023-06-14 12:13:25.438177 eunice-0.0.3/PKG-INFO
+-rw-r--r--   0 rob        (501) staff       (20)      188 2023-06-13 18:24:10.000000 eunice-0.0.3/README.md
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2023-06-14 12:13:25.437071 eunice-0.0.3/eunice/
+-rw-r--r--   0 rob        (501) staff       (20)        0 2023-06-13 16:21:12.000000 eunice-0.0.3/eunice/__init__.py
+-rw-r--r--   0 rob        (501) staff       (20)      292 2023-06-13 20:15:39.000000 eunice-0.0.3/eunice/__main__.py
+-rw-r--r--   0 rob        (501) staff       (20)      353 2023-06-13 17:14:12.000000 eunice-0.0.3/eunice/args.py
+-rw-r--r--   0 rob        (501) staff       (20)      252 2023-06-13 20:15:39.000000 eunice-0.0.3/eunice/cmdline.py
+-rw-r--r--   0 rob        (501) staff       (20)      283 2023-06-13 16:57:48.000000 eunice-0.0.3/eunice/definitions.py
+-rw-r--r--   0 rob        (501) staff       (20)      680 2023-06-13 17:16:17.000000 eunice-0.0.3/eunice/eunice_logging.py
+-rw-r--r--   0 rob        (501) staff       (20)     1116 2023-06-13 17:29:52.000000 eunice-0.0.3/eunice/models.py
+-rw-r--r--   0 rob        (501) staff       (20)     2893 2023-06-14 12:11:43.000000 eunice-0.0.3/eunice/run.py
+-rw-r--r--   0 rob        (501) staff       (20)      325 2023-06-13 17:21:32.000000 eunice-0.0.3/eunice/utils.py
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2023-06-14 12:13:25.438006 eunice-0.0.3/eunice.egg-info/
+-rw-r--r--   0 rob        (501) staff       (20)      785 2023-06-14 12:13:25.000000 eunice-0.0.3/eunice.egg-info/PKG-INFO
+-rw-r--r--   0 rob        (501) staff       (20)      402 2023-06-14 12:13:25.000000 eunice-0.0.3/eunice.egg-info/SOURCES.txt
+-rw-r--r--   0 rob        (501) staff       (20)        1 2023-06-14 12:13:25.000000 eunice-0.0.3/eunice.egg-info/dependency_links.txt
+-rw-r--r--   0 rob        (501) staff       (20)       47 2023-06-14 12:13:25.000000 eunice-0.0.3/eunice.egg-info/entry_points.txt
+-rw-r--r--   0 rob        (501) staff       (20)        1 2023-06-13 18:19:23.000000 eunice-0.0.3/eunice.egg-info/not-zip-safe
+-rw-r--r--   0 rob        (501) staff       (20)       13 2023-06-14 12:13:25.000000 eunice-0.0.3/eunice.egg-info/requires.txt
+-rw-r--r--   0 rob        (501) staff       (20)        7 2023-06-14 12:13:25.000000 eunice-0.0.3/eunice.egg-info/top_level.txt
+-rw-r--r--   0 rob        (501) staff       (20)       38 2023-06-14 12:13:25.438331 eunice-0.0.3/setup.cfg
+-rw-r--r--   0 rob        (501) staff       (20)      971 2023-06-14 12:12:36.000000 eunice-0.0.3/setup.py
```

### Comparing `eunice-0.0.2/LICENCE` & `eunice-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `eunice-0.0.2/PKG-INFO` & `eunice-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eunice
-Version: 0.0.2
+Version: 0.0.3
 Summary: eunice - a simple chatgpt cli wrapper
 Home-page: http://github.com/rob-parker-what/eunice
 Author: rob-parker-what
 Author-email: robparkerwhat.dev@gmail.com
 License: MIT
 Keywords: chatgpt,ai,openai
 Classifier: Intended Audience :: Developers
```

### Comparing `eunice-0.0.2/eunice/eunice_logging.py` & `eunice-0.0.3/eunice/eunice_logging.py`

 * *Files identical despite different names*

### Comparing `eunice-0.0.2/eunice/models.py` & `eunice-0.0.3/eunice/models.py`

 * *Files identical despite different names*

### Comparing `eunice-0.0.2/eunice.egg-info/PKG-INFO` & `eunice-0.0.3/eunice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eunice
-Version: 0.0.2
+Version: 0.0.3
 Summary: eunice - a simple chatgpt cli wrapper
 Home-page: http://github.com/rob-parker-what/eunice
 Author: rob-parker-what
 Author-email: robparkerwhat.dev@gmail.com
 License: MIT
 Keywords: chatgpt,ai,openai
 Classifier: Intended Audience :: Developers
```

### Comparing `eunice-0.0.2/setup.py` & `eunice-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 
 with open("README.md") as f:
     readme = f.read()
 
 
 setup(
```

