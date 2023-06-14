# Comparing `tmp/async-executor-0.1.0.tar.gz` & `tmp/async-executor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-executor-0.1.0.tar", last modified: Fri Dec  9 18:59:32 2022, max compression
+gzip compressed data, was "async-executor-0.1.1.tar", last modified: Wed Jun 14 17:27:11 2023, max compression
```

## Comparing `async-executor-0.1.0.tar` & `async-executor-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 ar        (1000) ar        (1000)        0 2022-12-09 18:59:32.589995 async-executor-0.1.0/
--rw-r--r--   0 ar        (1000) ar        (1000)     1070 2022-12-09 18:57:57.000000 async-executor-0.1.0/LICENSE
--rw-r--r--   0 ar        (1000) ar        (1000)      698 2022-12-09 18:59:32.589995 async-executor-0.1.0/PKG-INFO
--rw-r--r--   0 ar        (1000) ar        (1000)      436 2022-12-09 18:57:46.000000 async-executor-0.1.0/README.md
-drwxr-xr-x   0 ar        (1000) ar        (1000)        0 2022-12-09 18:59:32.589995 async-executor-0.1.0/async_executor.egg-info/
--rw-r--r--   0 ar        (1000) ar        (1000)      698 2022-12-09 18:59:32.000000 async-executor-0.1.0/async_executor.egg-info/PKG-INFO
--rw-r--r--   0 ar        (1000) ar        (1000)      206 2022-12-09 18:59:32.000000 async-executor-0.1.0/async_executor.egg-info/SOURCES.txt
--rw-r--r--   0 ar        (1000) ar        (1000)        1 2022-12-09 18:59:32.000000 async-executor-0.1.0/async_executor.egg-info/dependency_links.txt
--rw-r--r--   0 ar        (1000) ar        (1000)       15 2022-12-09 18:59:32.000000 async-executor-0.1.0/async_executor.egg-info/top_level.txt
--rw-r--r--   0 ar        (1000) ar        (1000)     1361 2022-12-09 18:54:15.000000 async-executor-0.1.0/async_executor.py
--rw-r--r--   0 ar        (1000) ar        (1000)      351 2022-12-09 18:59:32.589995 async-executor-0.1.0/setup.cfg
--rw-r--r--   0 ar        (1000) ar        (1000)       37 2022-12-09 18:56:28.000000 async-executor-0.1.0/setup.py
+drwxr-xr-x   0 ar        (1000) ar        (1000)        0 2023-06-14 17:27:11.517401 async-executor-0.1.1/
+-rw-r--r--   0 ar        (1000) ar        (1000)       38 2022-12-09 19:10:41.000000 async-executor-0.1.1/.gitignore
+-rw-r--r--   0 ar        (1000) ar        (1000)     1070 2022-12-09 19:10:41.000000 async-executor-0.1.1/LICENSE
+-rw-r--r--   0 ar        (1000) ar        (1000)     1651 2023-06-14 17:27:11.517401 async-executor-0.1.1/PKG-INFO
+-rw-r--r--   0 ar        (1000) ar        (1000)     1389 2022-12-09 19:28:05.000000 async-executor-0.1.1/README.md
+drwxr-xr-x   0 ar        (1000) ar        (1000)        0 2023-06-14 17:27:11.517401 async-executor-0.1.1/async_executor.egg-info/
+-rw-r--r--   0 ar        (1000) ar        (1000)     1651 2023-06-14 17:27:11.000000 async-executor-0.1.1/async_executor.egg-info/PKG-INFO
+-rw-r--r--   0 ar        (1000) ar        (1000)      239 2023-06-14 17:27:11.000000 async-executor-0.1.1/async_executor.egg-info/SOURCES.txt
+-rw-r--r--   0 ar        (1000) ar        (1000)        1 2023-06-14 17:27:11.000000 async-executor-0.1.1/async_executor.egg-info/dependency_links.txt
+-rw-r--r--   0 ar        (1000) ar        (1000)       15 2023-06-14 17:27:11.000000 async-executor-0.1.1/async_executor.egg-info/top_level.txt
+-rw-r--r--   0 ar        (1000) ar        (1000)     1567 2023-06-14 17:25:02.000000 async-executor-0.1.1/async_executor.py
+drwxr-xr-x   0 ar        (1000) ar        (1000)        0 2023-06-14 17:27:11.517401 async-executor-0.1.1/examples/
+-rw-r--r--   0 ar        (1000) ar        (1000)      580 2022-12-09 19:22:08.000000 async-executor-0.1.1/examples/example_1.py
+-rw-r--r--   0 ar        (1000) ar        (1000)      351 2023-06-14 17:27:11.517401 async-executor-0.1.1/setup.cfg
+-rw-r--r--   0 ar        (1000) ar        (1000)       37 2022-12-09 19:10:41.000000 async-executor-0.1.1/setup.py
```

### Comparing `async-executor-0.1.0/LICENSE` & `async-executor-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async-executor-0.1.0/async_executor.py` & `async-executor-0.1.1/async_executor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import asyncio
 import os
 
 
 class AsyncExecutor:
     def __init__(self, max_concurrent=None):
-        self._max_concurrent = \
-            os.cpu_count() if max_concurrent is None else max_concurrent
+        if max_concurrent and not isinstance(max_concurrent, int):
+            raise ValueError('max_concurrent must type int')
+        if max_concurrent and max_concurrent < 0:
+            raise ValueError('max_concurrent must be greater than 0')
+        self._max_concurrent = max_concurrent or os.cpu_count()
         self._queued = []
         self._pending = set()
         self._completed = set()
 
     def submit(self, func, *args, **kwargs):
         event = asyncio.Event()
         task = asyncio.create_task(self._wrap(event, func, args, kwargs))
```

