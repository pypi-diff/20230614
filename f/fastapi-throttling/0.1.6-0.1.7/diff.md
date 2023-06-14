# Comparing `tmp/fastapi_throttling-0.1.6.tar.gz` & `tmp/fastapi_throttling-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_throttling-0.1.6.tar", max compression
+gzip compressed data, was "fastapi_throttling-0.1.7.tar", max compression
```

## Comparing `fastapi_throttling-0.1.6.tar` & `fastapi_throttling-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    26526 2023-06-13 21:18:26.393691 fastapi_throttling-0.1.6/LICENSE
--rw-r--r--   0        0        0     1347 2023-06-13 21:18:26.393691 fastapi_throttling-0.1.6/README.md
--rw-r--r--   0        0        0     1753 2023-06-13 21:18:26.393691 fastapi_throttling-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       79 2023-06-13 21:18:26.393691 fastapi_throttling-0.1.6/src/fastapi_throttling/__init__.py
--rw-r--r--   0        0        0     2949 2023-06-13 21:18:26.393691 fastapi_throttling-0.1.6/src/fastapi_throttling/throttle.py
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 fastapi_throttling-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-14 17:56:21.981858 fastapi_throttling-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1347 2023-06-14 17:56:21.981858 fastapi_throttling-0.1.7/README.md
+-rw-r--r--   0        0        0     1753 2023-06-14 17:56:21.981858 fastapi_throttling-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-06-14 17:56:21.981858 fastapi_throttling-0.1.7/src/fastapi_throttling/__init__.py
+-rw-r--r--   0        0        0     2949 2023-06-14 17:56:21.981858 fastapi_throttling-0.1.7/src/fastapi_throttling/throttle.py
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 fastapi_throttling-0.1.7/PKG-INFO
```

### Comparing `fastapi_throttling-0.1.6/LICENSE` & `fastapi_throttling-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_throttling-0.1.6/README.md` & `fastapi_throttling-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_throttling-0.1.6/pyproject.toml` & `fastapi_throttling-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "fastapi-throttling"
-version = "0.1.6"
+version = "0.1.7"
 description = "Limit amount of requests to your FastAPI."
 authors = ["wwnbb <wwnbb1@gmail.com>"]
 license = "GPLv2"
 readme = "README.md"
 packages = [{include = "fastapi_throttling", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11.4"
 fastapi = "^0.96.0"
-redis = "^4.5.5"
+redis = "^4.5.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 mypy = "^1.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
```

### Comparing `fastapi_throttling-0.1.6/src/fastapi_throttling/throttle.py` & `fastapi_throttling-0.1.7/src/fastapi_throttling/throttle.py`

 * *Files identical despite different names*

### Comparing `fastapi_throttling-0.1.6/PKG-INFO` & `fastapi_throttling-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fastapi-throttling
-Version: 0.1.6
+Version: 0.1.7
 Summary: Limit amount of requests to your FastAPI.
 License: GPLv2
 Author: wwnbb
 Author-email: wwnbb1@gmail.com
 Requires-Python: >=3.11.4,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: fastapi (>=0.96.0,<0.97.0)
-Requires-Dist: redis (>=4.5.5,<5.0.0)
+Requires-Dist: redis (>=4.5.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 [![Upload Python Package](https://github.com/wwnbb/fastapi-throttling/actions/workflows/publish.yml/badge.svg?branch=master)](https://github.com/wwnbb/fastapi-throttling/actions/workflows/publish.yml)
 
 ## FastAPI Throttling Middleware
 
 FastAPI Throttling Middleware is a rate-limiting middleware for the FastAPI web framework. It uses a Redis server for request tracking and allows you to throttle incoming requests based on IP address and access token.
```

