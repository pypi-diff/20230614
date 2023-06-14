# Comparing `tmp/swampyer-3.0.20230108.tar.gz` & `tmp/swampyer-3.0.20230614.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swampyer-3.0.20230108.tar", last modified: Sun Jan  8 22:06:33 2023, max compression
+gzip compressed data, was "swampyer-3.0.20230614.tar", max compression
```

## Comparing `swampyer-3.0.20230108.tar` & `swampyer-3.0.20230614.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      689 2023-01-08 22:06:20.794701 swampyer-3.0.20230108/pyproject.toml
--rw-r--r--   0        0        0      168 2022-08-16 23:40:19.004711 swampyer-3.0.20230108/swampyer/__init__.py
--rw-r--r--   0        0        0    39009 2022-11-23 22:29:42.674475 swampyer-3.0.20230108/swampyer/client.py
--rw-r--r--   0        0        0     1098 2022-09-26 22:26:31.459187 swampyer-3.0.20230108/swampyer/common.py
--rw-r--r--   0        0        0      658 2022-08-16 23:40:19.004711 swampyer-3.0.20230108/swampyer/exceptions.py
--rw-r--r--   0        0        0     1014 2022-09-09 18:53:53.522720 swampyer-3.0.20230108/swampyer/fields.py
--rw-r--r--   0        0        0     7101 2022-11-23 22:28:58.618298 swampyer-3.0.20230108/swampyer/messages.py
--rw-r--r--   0        0        0    11295 2022-08-16 23:40:19.004711 swampyer-3.0.20230108/swampyer/queues.py
--rw-r--r--   0        0        0     4560 2022-11-23 15:19:59.503717 swampyer-3.0.20230108/swampyer/serializers.py
--rw-r--r--   0        0        0    17194 2022-11-22 20:12:28.152904 swampyer-3.0.20230108/swampyer/transport.py
--rw-r--r--   0        0        0       57 2022-08-16 23:40:19.004711 swampyer-3.0.20230108/swampyer/utils.py
--rw-r--r--   0        0        0      875 2023-01-08 22:06:33.566724 swampyer-3.0.20230108/setup.py
--rw-r--r--   0        0        0      780 2023-01-08 22:06:33.566998 swampyer-3.0.20230108/PKG-INFO
+-rw-r--r--   0        0        0      689 2023-06-14 18:01:18.094832 swampyer-3.0.20230614/pyproject.toml
+-rw-r--r--   0        0        0      168 2022-08-16 23:40:19.004711 swampyer-3.0.20230614/swampyer/__init__.py
+-rw-r--r--   0        0        0    39009 2023-01-27 23:39:43.540898 swampyer-3.0.20230614/swampyer/client.py
+-rw-r--r--   0        0        0     1098 2022-09-26 22:26:31.459187 swampyer-3.0.20230614/swampyer/common.py
+-rw-r--r--   0        0        0      658 2022-08-16 23:40:19.004711 swampyer-3.0.20230614/swampyer/exceptions.py
+-rw-r--r--   0        0        0     1014 2022-09-09 18:53:53.522720 swampyer-3.0.20230614/swampyer/fields.py
+-rw-r--r--   0        0        0     7101 2022-11-23 22:28:58.618298 swampyer-3.0.20230614/swampyer/messages.py
+-rw-r--r--   0        0        0    11295 2022-08-16 23:40:19.004711 swampyer-3.0.20230614/swampyer/queues.py
+-rw-r--r--   0        0        0     4696 2023-06-14 18:00:00.758370 swampyer-3.0.20230614/swampyer/serializers.py
+-rw-r--r--   0        0        0    17194 2022-11-22 20:12:28.152904 swampyer-3.0.20230614/swampyer/transport.py
+-rw-r--r--   0        0        0       57 2022-08-16 23:40:19.004711 swampyer-3.0.20230614/swampyer/utils.py
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 swampyer-3.0.20230614/setup.py
+-rw-r--r--   0        0        0      834 1970-01-01 00:00:00.000000 swampyer-3.0.20230614/PKG-INFO
```

### Comparing `swampyer-3.0.20230108/pyproject.toml` & `swampyer-3.0.20230614/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "swampyer"
 description = "Simple WAMP library with minimal external dependencies"
-version = '3.0.20230108'
+version = '3.0.20230614'
 authors = ["Aki Mimoto <aki@zaber.com>"]
 packages = [
   { include = "swampyer" }
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.6.0,<4.0"
+python = ">=3.7.0,<4.0"
 websocket-client = ">=0.59.0"
 certifi = ">=2020.12.5"
 six = "^1.16.0"
 cbor = { version = "^1.0.0", optional = true }
 msgpack = { version = "^1.0.2", optional = true }
 
 [tool.poetry.dev-dependencies]
```

### Comparing `swampyer-3.0.20230108/swampyer/client.py` & `swampyer-3.0.20230614/swampyer/client.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20230108/swampyer/common.py` & `swampyer-3.0.20230614/swampyer/common.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20230108/swampyer/exceptions.py` & `swampyer-3.0.20230614/swampyer/exceptions.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20230108/swampyer/fields.py` & `swampyer-3.0.20230614/swampyer/fields.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20230108/swampyer/messages.py` & `swampyer-3.0.20230614/swampyer/messages.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20230108/swampyer/queues.py` & `swampyer-3.0.20230614/swampyer/queues.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20230108/swampyer/serializers.py` & `swampyer-3.0.20230614/swampyer/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import struct
 import decimal
 
 import socket
 import websocket
 import traceback
 
+from datetime import date, datetime
+
 from .common import *
 from .utils import logger
 from .exceptions import *
 
 def register_serializer(code):
     def register(klass):
         global SERIALIZER_REGISTRY
@@ -46,14 +48,16 @@
                 without making nasty customizations to WAMP JSON
             """
             def default(self, obj):
                 if isinstance(obj, decimal.Decimal):
                     return float(obj)
                 elif isinstance(obj, memoryview):
                     return self.default(bytes(obj))
+                elif isinstance(obj, (datetime, date)):
+                    return obj.isoformat()
                 elif isinstance(obj, bytes):
                     try:
                         return obj.decode()
                     except UnicodeDecodeError as ex:
                         # Only show the entire data if we're below 200bytes
                         # FIXME: we'll probably want to allow for
                         # configuration or even interception later
```

### Comparing `swampyer-3.0.20230108/swampyer/transport.py` & `swampyer-3.0.20230614/swampyer/transport.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20230108/setup.py` & `swampyer-3.0.20230614/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 extras_require = \
 {'all': ['cbor>=1.0.0,<2.0.0', 'msgpack>=1.0.2,<2.0.0'],
  'cbor': ['cbor>=1.0.0,<2.0.0'],
  'msgpack': ['msgpack>=1.0.2,<2.0.0']}
 
 setup_kwargs = {
     'name': 'swampyer',
-    'version': '3.0.20230108',
+    'version': '3.0.20230614',
     'description': 'Simple WAMP library with minimal external dependencies',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Aki Mimoto',
     'author_email': 'aki@zaber.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.6.0,<4.0',
+    'python_requires': '>=3.7.0,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `swampyer-3.0.20230108/PKG-INFO` & `swampyer-3.0.20230614/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: swampyer
-Version: 3.0.20230108
+Version: 3.0.20230614
 Summary: Simple WAMP library with minimal external dependencies
 Author: Aki Mimoto
 Author-email: aki@zaber.com
-Requires-Python: >=3.6.0,<4.0
+Requires-Python: >=3.7.0,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: cbor
 Provides-Extra: msgpack
-Requires-Dist: cbor (>=1.0.0,<2.0.0); extra == "cbor" or extra == "all"
+Requires-Dist: cbor (>=1.0.0,<2.0.0) ; extra == "cbor" or extra == "all"
 Requires-Dist: certifi (>=2020.12.5)
-Requires-Dist: msgpack (>=1.0.2,<2.0.0); extra == "msgpack" or extra == "all"
+Requires-Dist: msgpack (>=1.0.2,<2.0.0) ; extra == "msgpack" or extra == "all"
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Requires-Dist: websocket-client (>=0.59.0)
```

