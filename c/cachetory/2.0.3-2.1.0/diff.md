# Comparing `tmp/cachetory-2.0.3.tar.gz` & `tmp/cachetory-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachetory-2.0.3.tar", max compression
+gzip compressed data, was "cachetory-2.1.0.tar", max compression
```

## Comparing `cachetory-2.0.3.tar` & `cachetory-2.1.0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0    11355 2023-04-24 20:01:45.657741 cachetory-2.0.3/LICENSE
--rw-r--r--   0        0        0    12891 2023-04-24 20:01:45.657741 cachetory-2.0.3/README.md
--rw-r--r--   0        0        0        0 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/__init__.py
--rw-r--r--   0        0        0       43 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/__init__.py
--rw-r--r--   0        0        0      999 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/async_/__init__.py
--rw-r--r--   0        0        0     1539 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/async_/dummy.py
--rw-r--r--   0        0        0     1727 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/async_/memory.py
--rw-r--r--   0        0        0     2502 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/async_/redis.py
--rw-r--r--   0        0        0      993 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/sync/__init__.py
--rw-r--r--   0        0        0     1427 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/sync/dummy.py
--rw-r--r--   0        0        0     2361 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/sync/memory.py
--rw-r--r--   0        0        0     2197 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/sync/redis.py
--rw-r--r--   0        0        0       47 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/caches/__init__.py
--rw-r--r--   0        0        0     3631 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/caches/async_.py
--rw-r--r--   0        0        0      122 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/caches/private.py
--rw-r--r--   0        0        0     2978 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/caches/sync.py
--rw-r--r--   0        0        0        0 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/decorators/__init__.py
--rw-r--r--   0        0        0     2041 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/decorators/async_.py
--rw-r--r--   0        0        0      990 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/decorators/shared.py
--rw-r--r--   0        0        0     1953 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/decorators/sync.py
--rw-r--r--   0        0        0       41 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/interfaces/backends/__init__.py
--rw-r--r--   0        0        0     3644 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/interfaces/backends/async_.py
--rw-r--r--   0        0        0     1183 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/interfaces/backends/private.py
--rw-r--r--   0        0        0     3478 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/interfaces/backends/sync.py
--rw-r--r--   0        0        0     1598 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/interfaces/serializers.py
--rw-r--r--   0        0        0       67 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/private/__init__.py
--rw-r--r--   0        0        0      307 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/private/asyncio.py
--rw-r--r--   0        0        0      255 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/private/datetime.py
--rw-r--r--   0        0        0      205 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/private/typing.py
--rw-r--r--   0        0        0        0 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/py.typed
--rw-r--r--   0        0        0      402 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/serializers/__init__.py
--rw-r--r--   0        0        0     2170 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/serializers/chained.py
--rw-r--r--   0        0        0      326 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/serializers/compressors/__init__.py
--rw-r--r--   0        0        0     1026 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/serializers/compressors/zlib.py
--rw-r--r--   0        0        0     1248 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/serializers/compressors/zstd.py
--rw-r--r--   0        0        0      538 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/serializers/noop.py
--rw-r--r--   0        0        0     1106 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/serializers/pickle.py
--rw-r--r--   0        0        0     3087 2023-04-24 20:01:59.890282 cachetory-2.0.3/pyproject.toml
--rw-r--r--   0        0        0    14563 1970-01-01 00:00:00.000000 cachetory-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-06-02 11:11:26.305038 cachetory-2.1.0/LICENSE
+-rw-r--r--   0        0        0    13566 2023-06-02 11:11:26.305038 cachetory-2.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/__init__.py
+-rw-r--r--   0        0        0       43 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/backends/__init__.py
+-rw-r--r--   0        0        0      999 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/backends/async_/__init__.py
+-rw-r--r--   0        0        0     1539 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/backends/async_/dummy.py
+-rw-r--r--   0        0        0     1727 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/backends/async_/memory.py
+-rw-r--r--   0        0        0     2502 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/backends/async_/redis.py
+-rw-r--r--   0        0        0      993 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/backends/sync/__init__.py
+-rw-r--r--   0        0        0     1427 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/backends/sync/dummy.py
+-rw-r--r--   0        0        0     2361 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/backends/sync/memory.py
+-rw-r--r--   0        0        0     2197 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/backends/sync/redis.py
+-rw-r--r--   0        0        0       47 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/caches/__init__.py
+-rw-r--r--   0        0        0     3631 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/caches/async_.py
+-rw-r--r--   0        0        0      122 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/caches/private.py
+-rw-r--r--   0        0        0     2978 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/caches/sync.py
+-rw-r--r--   0        0        0        0 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/decorators/__init__.py
+-rw-r--r--   0        0        0     2041 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/decorators/async_.py
+-rw-r--r--   0        0        0      990 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/decorators/shared.py
+-rw-r--r--   0        0        0     1953 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/decorators/sync.py
+-rw-r--r--   0        0        0       41 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/interfaces/backends/__init__.py
+-rw-r--r--   0        0        0     3644 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/interfaces/backends/async_.py
+-rw-r--r--   0        0        0     1183 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/interfaces/backends/private.py
+-rw-r--r--   0        0        0     3478 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/interfaces/backends/sync.py
+-rw-r--r--   0        0        0     1598 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/interfaces/serializers.py
+-rw-r--r--   0        0        0       67 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/private/__init__.py
+-rw-r--r--   0        0        0      307 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/private/asyncio.py
+-rw-r--r--   0        0        0      255 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/private/datetime.py
+-rw-r--r--   0        0        0      205 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/private/typing.py
+-rw-r--r--   0        0        0        0 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/py.typed
+-rw-r--r--   0        0        0      402 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/serializers/__init__.py
+-rw-r--r--   0        0        0     2718 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/serializers/chained.py
+-rw-r--r--   0        0        0      326 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/serializers/compressors/__init__.py
+-rw-r--r--   0        0        0     1026 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/serializers/compressors/zlib.py
+-rw-r--r--   0        0        0     1248 2023-06-02 11:11:26.305038 cachetory-2.1.0/cachetory/serializers/compressors/zstd.py
+-rw-r--r--   0        0        0      544 2023-06-02 11:11:26.309038 cachetory-2.1.0/cachetory/serializers/json.py
+-rw-r--r--   0        0        0      608 2023-06-02 11:11:26.309038 cachetory-2.1.0/cachetory/serializers/msgpack.py
+-rw-r--r--   0        0        0      538 2023-06-02 11:11:26.309038 cachetory-2.1.0/cachetory/serializers/noop.py
+-rw-r--r--   0        0        0     1106 2023-06-02 11:11:26.309038 cachetory-2.1.0/cachetory/serializers/pickle.py
+-rw-r--r--   0        0        0     3220 2023-06-02 11:11:40.021011 cachetory-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    15081 1970-01-01 00:00:00.000000 cachetory-2.1.0/PKG-INFO
```

### Comparing `cachetory-2.0.3/LICENSE` & `cachetory-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/README.md` & `cachetory-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -209,14 +209,36 @@
 |:-----------------------------------------|
 | `cachetory.serializers.PickleSerializer` |
 
 | URL parameter     |                                                                                                  |
 |:------------------|--------------------------------------------------------------------------------------------------|
 | `pickle-protocol` | Version of [`pickle` protocol](https://docs.python.org/3/library/pickle.html#data-stream-format) |
 
+### Json
+
+![scheme: json](https://img.shields.io/badge/scheme-json://-important)
+
+Serializes using the standard [`json`](https://docs.python.org/3/library/json.html) module.
+
+| Class                                  |
+|:---------------------------------------|
+| `cachetory.serializers.JsonSerializer` |
+
+### MessagePack
+
+![scheme: msgpack](https://img.shields.io/badge/scheme-msgpack://-important)
+
+Serializes using the non-standard [`msgpack`](https://github.com/aviramha/ormsgpack) module.
+
+| Class                                     |
+|:------------------------------------------|
+| `cachetory.serializers.MsgPackSerializer` |
+
+This serializer is not available on PyPy
+
 ### No-operation
 
 ![scheme: noop](https://img.shields.io/badge/scheme-noop://-important)
 ![scheme: null](https://img.shields.io/badge/scheme-null://-important)
 
 | Class                                   |
 |:----------------------------------------|
```

### Comparing `cachetory-2.0.3/cachetory/backends/async_/__init__.py` & `cachetory-2.1.0/cachetory/backends/async_/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/backends/async_/dummy.py` & `cachetory-2.1.0/cachetory/backends/async_/dummy.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/backends/async_/memory.py` & `cachetory-2.1.0/cachetory/backends/async_/memory.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/backends/async_/redis.py` & `cachetory-2.1.0/cachetory/backends/async_/redis.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/backends/sync/__init__.py` & `cachetory-2.1.0/cachetory/backends/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/backends/sync/dummy.py` & `cachetory-2.1.0/cachetory/backends/sync/dummy.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/backends/sync/memory.py` & `cachetory-2.1.0/cachetory/backends/sync/memory.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/backends/sync/redis.py` & `cachetory-2.1.0/cachetory/backends/sync/redis.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/caches/async_.py` & `cachetory-2.1.0/cachetory/caches/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/caches/sync.py` & `cachetory-2.1.0/cachetory/caches/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/decorators/async_.py` & `cachetory-2.1.0/cachetory/decorators/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/decorators/shared.py` & `cachetory-2.1.0/cachetory/decorators/shared.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/decorators/sync.py` & `cachetory-2.1.0/cachetory/decorators/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/interfaces/backends/async_.py` & `cachetory-2.1.0/cachetory/interfaces/backends/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/interfaces/backends/private.py` & `cachetory-2.1.0/cachetory/interfaces/backends/private.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/interfaces/backends/sync.py` & `cachetory-2.1.0/cachetory/interfaces/backends/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/interfaces/serializers.py` & `cachetory-2.1.0/cachetory/interfaces/serializers.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/serializers/chained.py` & `cachetory-2.1.0/cachetory/serializers/chained.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,25 +2,34 @@
 
 from typing import Any, Generic, Iterable, cast
 from urllib.parse import urlparse
 
 from cachetory.interfaces.backends.private import WireT
 from cachetory.interfaces.serializers import Serializer, ValueT
 from cachetory.serializers.compressors.zlib import ZlibCompressor
+from cachetory.serializers.json import JsonSerializer
 from cachetory.serializers.noop import NoopSerializer
 from cachetory.serializers.pickle import PickleSerializer
 
 try:
     # noinspection PyUnresolvedReferences
     from cachetory.serializers.compressors import ZstdCompressor
 except ImportError:
     _is_zstd_available = False
 else:
     _is_zstd_available = True
 
+try:
+    # noinspection PyUnresolvedReferences
+    from cachetory.serializers.msgpack import MsgPackSerializer
+except ImportError:
+    _is_msgpack_available = False
+else:
+    _is_msgpack_available = True
+
 
 class ChainedSerializer(Serializer[ValueT, WireT], Generic[ValueT, WireT]):
     """Sequentially applies the chain of serializers. Allows defining multiple steps of serialization."""
 
     __slots__ = ("_layers",)
 
     @classmethod
@@ -42,14 +51,20 @@
         value = cast(Any, data)
         for layer in self._layers[::-1]:
             value = layer.deserialize(value)
         return cast(ValueT, value)
 
     @classmethod
     def _make_layer(cls, scheme: str, url: str) -> Serializer:
+        if scheme == "json":
+            return JsonSerializer.from_url(url)
+        if scheme == "msgpack":
+            if not _is_msgpack_available:
+                raise ValueError(f"`{scheme}://` requires `cachetory[msgpack]` extra")
+            return MsgPackSerializer.from_url(url)
         if scheme == "pickle":
             return PickleSerializer.from_url(url)
         if scheme in ("noop", "null"):
             return NoopSerializer.from_url(url)
         if scheme in ("zstd", "zstandard"):
             if not _is_zstd_available:
                 raise ValueError(f"`{scheme}://` requires `cachetory[zstd]` extra")
```

### Comparing `cachetory-2.0.3/cachetory/serializers/compressors/zlib.py` & `cachetory-2.1.0/cachetory/serializers/compressors/zlib.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/serializers/compressors/zstd.py` & `cachetory-2.1.0/cachetory/serializers/compressors/zstd.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/serializers/noop.py` & `cachetory-2.1.0/cachetory/serializers/noop.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/cachetory/serializers/pickle.py` & `cachetory-2.1.0/cachetory/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.3/pyproject.toml` & `cachetory-2.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ]
 description = "Caching library with support for multiple cache backends"
 keywords = ["cache"]
 license = "Apache-2.0"
 name = "cachetory"
 readme = "README.md"
 repository = "https://github.com/kpn/cachetory"
-version = "2.0.3"
+version = "2.1.0"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -32,18 +32,20 @@
 
 [tool.poetry.dependencies]
 python = "^3.7.0"
 pydantic = "^1.10.4"
 typing-extensions = "^4.4.0"
 redis = {version = "^4.4.2", optional = true}
 zstd = {version = "^1.5.2.6", optional = true}
+ormsgpack = {version = "^1.2.6", optional = true, markers = "platform_python_implementation == 'CPython'"}
 
 [tool.poetry.extras]
 redis = ["redis"]
 zstd = ["zstd"]
+ormsgpack = ["ormsgpack"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^0.991"
 black = "^23.1.0"
```

### Comparing `cachetory-2.0.3/PKG-INFO` & `cachetory-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachetory
-Version: 2.0.3
+Version: 2.1.0
 Summary: Caching library with support for multiple cache backends
 Home-page: https://github.com/kpn/cachetory
 License: Apache-2.0
 Keywords: cache
 Author: Pavel Perestoronin
 Author-email: pavel.perestoronin@kpn.com
 Requires-Python: >=3.7.0,<4.0.0
@@ -16,25 +16,21 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Typing :: Typed
+Provides-Extra: ormsgpack
 Provides-Extra: redis
 Provides-Extra: zstd
+Requires-Dist: ormsgpack (>=1.2.6,<2.0.0) ; (platform_python_implementation == "CPython") and (extra == "ormsgpack")
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Requires-Dist: redis (>=4.4.2,<5.0.0) ; extra == "redis"
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Requires-Dist: zstd (>=1.5.2.6,<2.0.0.0) ; extra == "zstd"
 Project-URL: Repository, https://github.com/kpn/cachetory
 Description-Content-Type: text/markdown
 
@@ -249,14 +245,36 @@
 |:-----------------------------------------|
 | `cachetory.serializers.PickleSerializer` |
 
 | URL parameter     |                                                                                                  |
 |:------------------|--------------------------------------------------------------------------------------------------|
 | `pickle-protocol` | Version of [`pickle` protocol](https://docs.python.org/3/library/pickle.html#data-stream-format) |
 
+### Json
+
+![scheme: json](https://img.shields.io/badge/scheme-json://-important)
+
+Serializes using the standard [`json`](https://docs.python.org/3/library/json.html) module.
+
+| Class                                  |
+|:---------------------------------------|
+| `cachetory.serializers.JsonSerializer` |
+
+### MessagePack
+
+![scheme: msgpack](https://img.shields.io/badge/scheme-msgpack://-important)
+
+Serializes using the non-standard [`msgpack`](https://github.com/aviramha/ormsgpack) module.
+
+| Class                                     |
+|:------------------------------------------|
+| `cachetory.serializers.MsgPackSerializer` |
+
+This serializer is not available on PyPy
+
 ### No-operation
 
 ![scheme: noop](https://img.shields.io/badge/scheme-noop://-important)
 ![scheme: null](https://img.shields.io/badge/scheme-null://-important)
 
 | Class                                   |
 |:----------------------------------------|
```

