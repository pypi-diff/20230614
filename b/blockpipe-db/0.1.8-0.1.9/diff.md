# Comparing `tmp/blockpipe_db-0.1.8.tar.gz` & `tmp/blockpipe_db-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockpipe_db-0.1.8.tar", max compression
+gzip compressed data, was "blockpipe_db-0.1.9.tar", max compression
```

## Comparing `blockpipe_db-0.1.8.tar` & `blockpipe_db-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       28 2023-05-28 13:20:46.955674 blockpipe_db-0.1.8/README.md
--rw-r--r--   0        0        0       27 2023-05-28 13:31:46.448380 blockpipe_db-0.1.8/blockpipe_db/__init__.py
--rw-r--r--   0        0        0     2258 2023-05-30 10:32:23.074881 blockpipe_db-0.1.8/blockpipe_db/client.py
--rw-r--r--   0        0        0      595 2023-05-30 09:20:34.775341 blockpipe_db-0.1.8/blockpipe_db/msg.py
--rw-r--r--   0        0        0      393 2023-05-30 10:32:42.773700 blockpipe_db-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 blockpipe_db-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       28 2023-05-28 13:20:46.955674 blockpipe_db-0.1.9/README.md
+-rw-r--r--   0        0        0       27 2023-05-28 13:31:46.448380 blockpipe_db-0.1.9/blockpipe_db/__init__.py
+-rw-r--r--   0        0        0     2290 2023-06-14 10:05:03.191180 blockpipe_db-0.1.9/blockpipe_db/client.py
+-rw-r--r--   0        0        0      595 2023-05-30 09:20:34.775341 blockpipe_db-0.1.9/blockpipe_db/msg.py
+-rw-r--r--   0        0        0      393 2023-06-14 10:05:17.879271 blockpipe_db-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 blockpipe_db-0.1.9/PKG-INFO
```

### Comparing `blockpipe_db-0.1.8/blockpipe_db/client.py` & `blockpipe_db-0.1.9/blockpipe_db/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import msgpack
 import pandas as pd
 from hexbytes import HexBytes
 
 from .msg import GetLogs1Request
 
 
-_DEFAULT_HOST = 'blockpipe_db_host'
+# _DEFAULT_HOST = 'blockpipe_db_host'
+_DEFAULT_HOST = '10.148.0.43'
 _DEFAULT_PORT = 5555
 
 
 class BufferedSocket:
     def __init__(self, sock):
         self.sock = sock
         self.buffer = b''
```

### Comparing `blockpipe_db-0.1.8/blockpipe_db/msg.py` & `blockpipe_db-0.1.9/blockpipe_db/msg.py`

 * *Files identical despite different names*

### Comparing `blockpipe_db-0.1.8/PKG-INFO` & `blockpipe_db-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockpipe-db
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Sorawit Suriyakarn
 Author-email: thepsint@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

