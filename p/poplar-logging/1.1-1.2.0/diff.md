# Comparing `tmp/poplar_logging-1.1.tar.gz` & `tmp/poplar_logging-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poplar_logging-1.1.tar", last modified: Mon Jun 12 05:13:30 2023, max compression
+gzip compressed data, was "poplar_logging-1.2.0.tar", last modified: Wed Jun 14 19:53:53 2023, max compression
```

## Comparing `poplar_logging-1.1.tar` & `poplar_logging-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-12 05:13:30.123028 poplar_logging-1.1/
--rw-r--r--   0 odai       (501) staff       (20)     1070 2023-06-12 04:45:07.000000 poplar_logging-1.1/LICENSE
--rw-r--r--   0 odai       (501) staff       (20)      863 2023-06-12 05:13:30.122900 poplar_logging-1.1/PKG-INFO
--rw-r--r--   0 odai       (501) staff       (20)      431 2023-06-12 04:56:46.000000 poplar_logging-1.1/README.md
--rw-r--r--   0 odai       (501) staff       (20)      425 2023-06-12 05:03:31.000000 poplar_logging-1.1/pyproject.toml
--rw-r--r--   0 odai       (501) staff       (20)       38 2023-06-12 05:13:30.123068 poplar_logging-1.1/setup.cfg
-drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-12 05:13:30.121452 poplar_logging-1.1/src/
-drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-12 05:13:30.122362 poplar_logging-1.1/src/poplar_logging.egg-info/
--rw-r--r--   0 odai       (501) staff       (20)      863 2023-06-12 05:13:30.000000 poplar_logging-1.1/src/poplar_logging.egg-info/PKG-INFO
--rw-r--r--   0 odai       (501) staff       (20)      276 2023-06-12 05:13:30.000000 poplar_logging-1.1/src/poplar_logging.egg-info/SOURCES.txt
--rw-r--r--   0 odai       (501) staff       (20)        1 2023-06-12 05:13:30.000000 poplar_logging-1.1/src/poplar_logging.egg-info/dependency_links.txt
--rw-r--r--   0 odai       (501) staff       (20)       23 2023-06-12 05:13:30.000000 poplar_logging-1.1/src/poplar_logging.egg-info/top_level.txt
-drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-12 05:13:30.122544 poplar_logging-1.1/src/poplar_logging_heyodai/
--rw-r--r--   0 odai       (501) staff       (20)        0 2023-06-12 04:48:03.000000 poplar_logging-1.1/src/poplar_logging_heyodai/__init__.py
--rw-r--r--   0 odai       (501) staff       (20)     1507 2023-06-12 04:52:54.000000 poplar_logging-1.1/src/poplar_logging_heyodai/poplar.py
+drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-14 19:53:53.759179 poplar_logging-1.2.0/
+-rw-r--r--   0 odai       (501) staff       (20)     1070 2023-06-12 04:45:07.000000 poplar_logging-1.2.0/LICENSE
+-rw-r--r--   0 odai       (501) staff       (20)      865 2023-06-14 19:53:53.759058 poplar_logging-1.2.0/PKG-INFO
+-rw-r--r--   0 odai       (501) staff       (20)      431 2023-06-12 04:56:46.000000 poplar_logging-1.2.0/README.md
+-rw-r--r--   0 odai       (501) staff       (20)      427 2023-06-14 19:51:52.000000 poplar_logging-1.2.0/pyproject.toml
+-rw-r--r--   0 odai       (501) staff       (20)       38 2023-06-14 19:53:53.759217 poplar_logging-1.2.0/setup.cfg
+drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-14 19:53:53.757315 poplar_logging-1.2.0/src/
+drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-14 19:53:53.758220 poplar_logging-1.2.0/src/poplar_logging/
+-rw-r--r--   0 odai       (501) staff       (20)        0 2023-06-12 04:48:03.000000 poplar_logging-1.2.0/src/poplar_logging/__init__.py
+-rw-r--r--   0 odai       (501) staff       (20)     1529 2023-06-14 19:48:34.000000 poplar_logging-1.2.0/src/poplar_logging/main.py
+drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-14 19:53:53.758917 poplar_logging-1.2.0/src/poplar_logging.egg-info/
+-rw-r--r--   0 odai       (501) staff       (20)      865 2023-06-14 19:53:53.000000 poplar_logging-1.2.0/src/poplar_logging.egg-info/PKG-INFO
+-rw-r--r--   0 odai       (501) staff       (20)      258 2023-06-14 19:53:53.000000 poplar_logging-1.2.0/src/poplar_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 odai       (501) staff       (20)        1 2023-06-14 19:53:53.000000 poplar_logging-1.2.0/src/poplar_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 odai       (501) staff       (20)       15 2023-06-14 19:53:53.000000 poplar_logging-1.2.0/src/poplar_logging.egg-info/top_level.txt
```

### Comparing `poplar_logging-1.1/LICENSE` & `poplar_logging-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poplar_logging-1.1/PKG-INFO` & `poplar_logging-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poplar_logging
-Version: 1.1
+Version: 1.2.0
 Summary: Simple Python logging library
 Author-email: Odai Athamneh <heyodai@gmail.com>
 Project-URL: Homepage, https://github.com/heyodai/poplar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `poplar_logging-1.1/src/poplar_logging.egg-info/PKG-INFO` & `poplar_logging-1.2.0/src/poplar_logging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poplar-logging
-Version: 1.1
+Version: 1.2.0
 Summary: Simple Python logging library
 Author-email: Odai Athamneh <heyodai@gmail.com>
 Project-URL: Homepage, https://github.com/heyodai/poplar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `poplar_logging-1.1/src/poplar_logging_heyodai/poplar.py` & `poplar_logging-1.2.0/src/poplar_logging/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 import os
 from datetime import datetime
 
+__all__ = ['poplar']
+
 class PoplarLogger:
     def __init__(self):
         self.log_directory = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'logs')
         os.makedirs(self.log_directory, exist_ok=True)
 
         self.logger = logging.getLogger()
         self.logger.setLevel(logging.INFO)
```

