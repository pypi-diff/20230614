# Comparing `tmp/pythonblip-0.2.1.tar.gz` & `tmp/pythonblip-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonblip-0.2.1.tar", last modified: Tue Jun 13 14:55:28 2023, max compression
+gzip compressed data, was "pythonblip-0.3.0.tar", last modified: Wed Jun 14 02:13:11 2023, max compression
```

## Comparing `pythonblip-0.2.1.tar` & `pythonblip-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-13 14:55:28.330933 pythonblip-0.2.1/
--rw-r--r--   0 michael    (501) staff       (20)    10846 2023-06-13 13:55:12.000000 pythonblip-0.2.1/LICENSE
--rw-r--r--   0 michael    (501) staff       (20)     1706 2023-06-13 14:55:28.330743 pythonblip-0.2.1/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      855 2023-06-13 14:54:16.000000 pythonblip-0.2.1/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-13 14:55:28.190397 pythonblip-0.2.1/bin/
--rwxr-xr-x   0 michael    (501) staff       (20)     5490 2023-06-13 14:13:04.000000 pythonblip-0.2.1/bin/blipctl
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-13 14:55:28.232447 pythonblip-0.2.1/pythonblip/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-05 19:03:37.000000 pythonblip-0.2.1/pythonblip/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     3151 2023-06-13 14:13:04.000000 pythonblip-0.2.1/pythonblip/client.py
--rw-r--r--   0 michael    (501) staff       (20)     2435 2023-06-13 14:13:04.000000 pythonblip-0.2.1/pythonblip/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)     9348 2023-06-13 14:13:04.000000 pythonblip-0.2.1/pythonblip/frame.py
--rw-r--r--   0 michael    (501) staff       (20)      723 2023-05-03 18:22:12.000000 pythonblip-0.2.1/pythonblip/headers.py
--rw-r--r--   0 michael    (501) staff       (20)     5419 2023-06-13 14:13:04.000000 pythonblip-0.2.1/pythonblip/output.py
--rw-r--r--   0 michael    (501) staff       (20)     3754 2023-06-13 14:13:04.000000 pythonblip-0.2.1/pythonblip/protocol.py
--rw-r--r--   0 michael    (501) staff       (20)    12382 2023-06-13 14:13:04.000000 pythonblip-0.2.1/pythonblip/replicator.py
--rw-r--r--   0 michael    (501) staff       (20)     2944 2023-05-05 00:55:25.000000 pythonblip-0.2.1/pythonblip/varint.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-13 14:55:28.330406 pythonblip-0.2.1/pythonblip.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1706 2023-06-13 14:55:28.000000 pythonblip-0.2.1/pythonblip.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      408 2023-06-13 14:55:28.000000 pythonblip-0.2.1/pythonblip.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-13 14:55:28.000000 pythonblip-0.2.1/pythonblip.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       58 2023-06-13 14:55:28.000000 pythonblip-0.2.1/pythonblip.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)       11 2023-06-13 14:55:28.000000 pythonblip-0.2.1/pythonblip.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-06-13 14:55:28.330997 pythonblip-0.2.1/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1336 2023-06-13 14:54:57.000000 pythonblip-0.2.1/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-14 02:13:11.022869 pythonblip-0.3.0/
+-rw-r--r--   0 michael    (501) staff       (20)    10846 2023-06-13 13:55:12.000000 pythonblip-0.3.0/LICENSE
+-rw-r--r--   0 michael    (501) staff       (20)     1706 2023-06-14 02:13:11.022679 pythonblip-0.3.0/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      855 2023-06-13 14:54:16.000000 pythonblip-0.3.0/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-14 02:13:10.955421 pythonblip-0.3.0/bin/
+-rwxr-xr-x   0 michael    (501) staff       (20)     5582 2023-06-13 15:57:14.000000 pythonblip-0.3.0/bin/blipctl
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-14 02:13:10.969299 pythonblip-0.3.0/pythonblip/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-05 19:03:37.000000 pythonblip-0.3.0/pythonblip/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     3695 2023-06-13 20:07:27.000000 pythonblip-0.3.0/pythonblip/client.py
+-rw-r--r--   0 michael    (501) staff       (20)     2435 2023-06-13 14:13:04.000000 pythonblip-0.3.0/pythonblip/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)     9348 2023-06-13 14:13:04.000000 pythonblip-0.3.0/pythonblip/frame.py
+-rw-r--r--   0 michael    (501) staff       (20)      723 2023-05-03 18:22:12.000000 pythonblip-0.3.0/pythonblip/headers.py
+-rw-r--r--   0 michael    (501) staff       (20)     5419 2023-06-13 14:13:04.000000 pythonblip-0.3.0/pythonblip/output.py
+-rw-r--r--   0 michael    (501) staff       (20)     3754 2023-06-13 14:13:04.000000 pythonblip-0.3.0/pythonblip/protocol.py
+-rw-r--r--   0 michael    (501) staff       (20)    12702 2023-06-13 16:22:10.000000 pythonblip-0.3.0/pythonblip/replicator.py
+-rw-r--r--   0 michael    (501) staff       (20)     2944 2023-05-05 00:55:25.000000 pythonblip-0.3.0/pythonblip/varint.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-14 02:13:11.022354 pythonblip-0.3.0/pythonblip.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1706 2023-06-14 02:13:10.000000 pythonblip-0.3.0/pythonblip.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      408 2023-06-14 02:13:10.000000 pythonblip-0.3.0/pythonblip.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-14 02:13:10.000000 pythonblip-0.3.0/pythonblip.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       58 2023-06-14 02:13:10.000000 pythonblip-0.3.0/pythonblip.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)       11 2023-06-14 02:13:10.000000 pythonblip-0.3.0/pythonblip.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-06-14 02:13:11.022931 pythonblip-0.3.0/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1336 2023-06-13 16:27:31.000000 pythonblip-0.3.0/setup.py
```

### Comparing `pythonblip-0.2.1/LICENSE` & `pythonblip-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonblip-0.2.1/PKG-INFO` & `pythonblip-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonblip
-Version: 0.2.1
+Version: 0.3.0
 Summary: Couchbase BLIP Protocol Library
 Home-page: https://github.com/mminichino/python-blip
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: Apache License 2.0
 Keywords: couchbase,blip,mobile,syncgateway
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pythonblip-0.2.1/README.md` & `pythonblip-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pythonblip-0.2.1/bin/blipctl` & `pythonblip-0.3.0/bin/blipctl`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 class Parameters(object):
 
     def __init__(self):
         parser = argparse.ArgumentParser()
         parser.add_argument('--ssl', action='store_true', help="Use SSL")
         parser.add_argument('-n', '--host', action='store', help="Hostname or IP address", default="127.0.0.1")
+        parser.add_argument('-P', '--port', action='store', help="Port number", default="4984")
         parser.add_argument('-u', '--user', action='store', help="User Name", default="Administrator")
         parser.add_argument('-p', '--password', action='store', help="User Password", default="password")
         parser.add_argument('-d', '--database', action='store', help="Sync Gateway Database")
         parser.add_argument('-t', '--session', action='store', help="Session Token")
         parser.add_argument('-O', '--screen', action="store_true")
         parser.add_argument('-f', '--file', action="store_true")
         parser.add_argument('-D', '--dir', action="store", help="Output Directory")
@@ -82,32 +83,33 @@
 class RunMain(object):
 
     def __init__(self):
         pass
 
     @staticmethod
     def run(options):
-        connect_string = f"ws://{options.host}:4984"
         directory = options.dir if options.dir else os.environ['HOME']
         scope = options.scope if options.scope else "_default"
         collections = options.collections.split(',') if options.collections else ["_default"]
         logging.basicConfig()
 
         if options.screen:
             output = ScreenOutput()
         elif options.file:
             output = LocalFile(directory)
         else:
             output = LocalDB(directory)
 
         replicator = Replicator(ReplicatorConfiguration.create(
             options.database,
-            connect_string,
+            options.host,
             ReplicatorType.PULL,
             SessionAuth(options.session),
+            options.ssl,
+            options.port,
             scope,
             collections,
             output
         ))
 
         try:
             replicator.start()
```

### Comparing `pythonblip-0.2.1/pythonblip/client.py` & `pythonblip-0.3.0/pythonblip/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##
 ##
-
+import ssl
 import time
 import logging
 import asyncio
 import websockets
 from websockets.legacy.client import WebSocketClientProtocol
 from websockets.exceptions import InvalidStatusCode, ConnectionClosed
 import multiprocessing
@@ -15,31 +15,44 @@
 logger = logging.getLogger('pythonblip.client')
 logger.addHandler(logging.NullHandler())
 sent_counter = MPAtomicIncrement()
 
 
 class BLIPClient(object):
 
-    def __init__(self, uri: str, headers: dict):
+    def __init__(self, target: str, headers: dict, tls: bool = False):
         lock = Lock()
-        self.uri = uri
         self.headers = headers
         self.run_loop = True
         self.websocket = WebSocketClientProtocol()
         self.loop = asyncio.get_event_loop()
         self.read_queue = multiprocessing.Queue()
         self.write_queue = multiprocessing.Queue()
         self.run_status = multiprocessing.Value('i', 0)
         self.run_message = multiprocessing.Array('c', 256, lock=lock)
 
+        if not tls:
+            self.ssl_context = None
+        else:
+            self.ssl_context = ssl.SSLContext()
+            self.ssl_context.check_hostname = False
+            self.ssl_context.verify_mode = ssl.CERT_NONE
+            self.ssl_context.options |= ssl.OP_NO_TLSv1
+            self.ssl_context.options |= ssl.OP_NO_TLSv1_1
+            self.ssl_context.load_default_certs()
+
+        self.uri = target
+
     async def connect(self):
         tasks = []
+        logger.debug(f"Connecting to {self.uri}")
 
         try:
             connection = websockets.connect(self.uri,
+                                            ssl=self.ssl_context,
                                             extra_headers=self.headers,
                                             subprotocols=['BLIP_3+CBMobile_3'],
                                             logger=logger)
             async with connection as self.websocket:
                 while self.websocket.open:
                     tasks.append(self.loop.create_task(self.reader()))
                     tasks.append(self.loop.create_task(self.writer()))
```

### Comparing `pythonblip-0.2.1/pythonblip/exceptions.py` & `pythonblip-0.3.0/pythonblip/exceptions.py`

 * *Files identical despite different names*

### Comparing `pythonblip-0.2.1/pythonblip/frame.py` & `pythonblip-0.3.0/pythonblip/frame.py`

 * *Files identical despite different names*

### Comparing `pythonblip-0.2.1/pythonblip/headers.py` & `pythonblip-0.3.0/pythonblip/headers.py`

 * *Files identical despite different names*

### Comparing `pythonblip-0.2.1/pythonblip/output.py` & `pythonblip-0.3.0/pythonblip/output.py`

 * *Files identical despite different names*

### Comparing `pythonblip-0.2.1/pythonblip/protocol.py` & `pythonblip-0.3.0/pythonblip/protocol.py`

 * *Files identical despite different names*

### Comparing `pythonblip-0.2.1/pythonblip/replicator.py` & `pythonblip-0.3.0/pythonblip/replicator.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,37 +27,47 @@
 
 @attr.s
 class ReplicatorConfiguration(object):
     database = attr.ib(validator=instance_of(str))
     target = attr.ib(validator=instance_of(str))
     type = attr.ib(validator=instance_of(ReplicatorType))
     authenticator = attr.ib(validator=instance_of((SessionAuth, BasicAuth)))
+    tls = attr.ib(validator=instance_of(bool))
+    port = attr.ib(validator=instance_of(str))
     scope = attr.ib(validator=instance_of(str))
     collections = attr.ib(validator=instance_of(list))
     datastore = attr.ib(validator=instance_of((LocalDB, LocalFile, ScreenOutput)))
     continuous = attr.ib(validator=instance_of(bool))
     checkpoint = attr.ib(validator=instance_of(bool))
 
     @classmethod
     def create(cls, database: str,
-               target: str,
+               hostname: str,
                r_type: ReplicatorType,
                authenticator: Union[SessionAuth, BasicAuth],
+               tls: bool = False,
+               port: str = "4984",
                scope: str = "_default",
                collections: list[str] = None,
                output: Union[LocalDB, LocalFile, ScreenOutput] = None,
                continuous: bool = False,
                checkpoint: bool = True):
         if not collections:
             collections = ["_default"]
+        if tls:
+            prefix = "wss"
+        else:
+            prefix = "ws"
         return cls(
             database,
-            f"{target}/{database}/_blipsync",
+            f"{prefix}://{hostname}:{port}/{database}/_blipsync",
             r_type,
             authenticator,
+            tls,
+            port,
             scope,
             collections,
             output.database(database, collections),
             continuous,
             checkpoint
         )
 
@@ -117,15 +127,15 @@
         self.collection_rev_list = []
         if self.collections[0] != "_default":
             for collection in self.collections:
                 _target = f"{self.config.scope}.{collection}"
                 _hash = self.get_id_hash(self.config.scope, collection)
                 self.collection_list.append(_target)
                 self.hash_list.append(_hash)
-        self.blip = BLIPProtocol(self.config.target, self.config.authenticator.header())
+        self.blip = BLIPProtocol(self.config.target, self.config.authenticator.header(), self.config.tls)
         logger.info(f"Replicator active for client {self.client}")
 
     def get_id_hash(self, scope: str = None, collection: str = None) -> str:
         if not collection and not scope:
             id_hash = sha1()
         else:
             id_hash = sha256()
```

### Comparing `pythonblip-0.2.1/pythonblip/varint.py` & `pythonblip-0.3.0/pythonblip/varint.py`

 * *Files identical despite different names*

### Comparing `pythonblip-0.2.1/pythonblip.egg-info/PKG-INFO` & `pythonblip-0.3.0/pythonblip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonblip
-Version: 0.2.1
+Version: 0.3.0
 Summary: Couchbase BLIP Protocol Library
 Home-page: https://github.com/mminichino/python-blip
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: Apache License 2.0
 Keywords: couchbase,blip,mobile,syncgateway
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pythonblip-0.2.1/setup.py` & `pythonblip-0.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pythonblip',
-    version='0.2.1',
+    version='0.3.0',
     packages=['pythonblip'],
     url='https://github.com/mminichino/python-blip',
     license='Apache License 2.0',
     author='Michael Minichino',
     python_requires='>=3.9',
     scripts=['bin/blipctl'],
     install_requires=[
```

