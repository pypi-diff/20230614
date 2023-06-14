# Comparing `tmp/asyncudp-0.8.0.tar.gz` & `tmp/asyncudp-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncudp-0.8.0.tar", last modified: Mon Feb 20 17:46:31 2023, max compression
+gzip compressed data, was "asyncudp-0.9.0.tar", last modified: Mon Feb 20 18:08:30 2023, max compression
```

## Comparing `asyncudp-0.8.0.tar` & `asyncudp-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-20 17:46:31.970383 asyncudp-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-02-20 17:46:21.000000 asyncudp-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-02-20 17:46:21.000000 asyncudp-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      692 2023-02-20 17:46:31.966383 asyncudp-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-02-20 17:46:21.000000 asyncudp-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-20 17:46:31.966383 asyncudp-0.8.0/asyncudp/
--rw-r--r--   0 runner    (1001) docker     (122)     2684 2023-02-20 17:46:21.000000 asyncudp-0.8.0/asyncudp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-02-20 17:46:21.000000 asyncudp-0.8.0/asyncudp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-20 17:46:31.966383 asyncudp-0.8.0/asyncudp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      692 2023-02-20 17:46:31.000000 asyncudp-0.8.0/asyncudp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-02-20 17:46:31.000000 asyncudp-0.8.0/asyncudp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-20 17:46:31.000000 asyncudp-0.8.0/asyncudp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-02-20 17:46:31.000000 asyncudp-0.8.0/asyncudp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-20 17:46:31.970383 asyncudp-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      793 2023-02-20 17:46:21.000000 asyncudp-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-20 17:46:31.966383 asyncudp-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-20 17:46:21.000000 asyncudp-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3565 2023-02-20 17:46:21.000000 asyncudp-0.8.0/tests/test_asyncudp.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-20 18:08:30.369321 asyncudp-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-02-20 18:08:21.000000 asyncudp-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-02-20 18:08:21.000000 asyncudp-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      692 2023-02-20 18:08:30.369321 asyncudp-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-02-20 18:08:21.000000 asyncudp-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-20 18:08:30.365321 asyncudp-0.9.0/asyncudp/
+-rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-02-20 18:08:21.000000 asyncudp-0.9.0/asyncudp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-02-20 18:08:21.000000 asyncudp-0.9.0/asyncudp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-20 18:08:30.369321 asyncudp-0.9.0/asyncudp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      692 2023-02-20 18:08:30.000000 asyncudp-0.9.0/asyncudp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-02-20 18:08:30.000000 asyncudp-0.9.0/asyncudp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-20 18:08:30.000000 asyncudp-0.9.0/asyncudp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-02-20 18:08:30.000000 asyncudp-0.9.0/asyncudp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-20 18:08:30.369321 asyncudp-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      793 2023-02-20 18:08:21.000000 asyncudp-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-20 18:08:30.369321 asyncudp-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-20 18:08:21.000000 asyncudp-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4420 2023-02-20 18:08:21.000000 asyncudp-0.9.0/tests/test_asyncudp.py
```

### Comparing `asyncudp-0.8.0/LICENSE` & `asyncudp-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncudp-0.8.0/PKG-INFO` & `asyncudp-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncudp
-Version: 0.8.0
+Version: 0.9.0
 Summary: Asyncio high level UDP sockets.
 Home-page: https://github.com/eerimoq/asyncudp
 Author: Erik Moqvist
 Author-email: erik.moqvist@gmail.com
 License: MIT
 Keywords: asyncio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `asyncudp-0.8.0/asyncudp/__init__.py` & `asyncudp-0.9.0/asyncudp/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import asyncio
+
 from .version import __version__
 
 
 class ClosedError(Exception):
     pass
 
 
 class _SocketProtocol:
 
-    def __init__(self):
+    def __init__(self, packets_queue_max_size):
         self._error = None
-        self._packets = asyncio.Queue()
+        self._packets = asyncio.Queue(packets_queue_max_size)
 
     def connection_made(self, transport):
         pass
 
     def connection_lost(self, transport):
         self._packets.put_nowait(None)
 
@@ -100,21 +101,21 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, *exc_info):
         self.close()
 
 
-async def create_socket(local_addr=None, remote_addr=None):
+async def create_socket(local_addr=None, remote_addr=None, packets_queue_max_size=0):
     """Create a UDP socket with given local and remote addresses.
 
     >>> sock = await asyncudp.create_socket(local_addr=('127.0.0.1', 9999))
 
     """
 
     loop = asyncio.get_running_loop()
     transport, protocol = await loop.create_datagram_endpoint(
-        _SocketProtocol,
+        lambda: _SocketProtocol(packets_queue_max_size),
         local_addr=local_addr,
         remote_addr=remote_addr)
 
     return Socket(transport, protocol)
```

### Comparing `asyncudp-0.8.0/asyncudp.egg-info/PKG-INFO` & `asyncudp-0.9.0/asyncudp.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncudp
-Version: 0.8.0
+Version: 0.9.0
 Summary: Asyncio high level UDP sockets.
 Home-page: https://github.com/eerimoq/asyncudp
 Author: Erik Moqvist
 Author-email: erik.moqvist@gmail.com
 License: MIT
 Keywords: asyncio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `asyncudp-0.8.0/setup.py` & `asyncudp-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `asyncudp-0.8.0/tests/test_asyncudp.py` & `asyncudp-0.9.0/tests/test_asyncudp.py`

 * *Files 14% similar despite different names*

```diff
@@ -105,7 +105,29 @@
             self.assertEqual(addr, server_addr)
 
             self.assertEqual(server._transport.is_closing(), False)
             self.assertEqual(client._transport.is_closing(), False)
 
         self.assertEqual(server._transport.is_closing(), True)
         self.assertEqual(client._transport.is_closing(), True)
+
+    def test_packets_queue_max_size(self):
+        asyncio.run(self.packets_queue_max_size())
+
+    async def packets_queue_max_size(self):
+        server = await asyncudp.create_socket(local_addr=('127.0.0.1', 0),
+                                              packets_queue_max_size=1)
+        server_addr = server.getsockname()
+        client = await asyncudp.create_socket(remote_addr=server_addr)
+
+        client.sendto(b'local_addresses to server 1')
+        client.sendto(b'local_addresses to server 2')
+        await asyncio.sleep(1.0)
+        data, _ = await server.recvfrom()
+        self.assertEqual(data, b'local_addresses to server 1')
+
+        client.sendto(b'local_addresses to server 3')
+        data, _ = await server.recvfrom()
+        self.assertEqual(data, b'local_addresses to server 3')
+
+        server.close()
+        client.close()
```

