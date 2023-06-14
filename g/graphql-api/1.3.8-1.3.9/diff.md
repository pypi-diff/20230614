# Comparing `tmp/graphql-api-1.3.8.tar.gz` & `tmp/graphql-api-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql-api-1.3.8.tar", last modified: Wed May 17 19:27:46 2023, max compression
+gzip compressed data, was "graphql-api-1.3.9.tar", last modified: Sun Jun  4 11:54:46 2023, max compression
```

## Comparing `graphql-api-1.3.8.tar` & `graphql-api-1.3.9.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 19:27:46.313406 graphql-api-1.3.8/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-17 19:27:38.000000 graphql-api-1.3.8/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       73 2023-05-17 19:27:38.000000 graphql-api-1.3.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1946 2023-05-17 19:27:46.313406 graphql-api-1.3.8/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1270 2023-05-17 19:27:38.000000 graphql-api-1.3.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-17 19:27:45.000000 graphql-api-1.3.8/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 19:27:46.310406 graphql-api-1.3.8/graphql_api/
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7527 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/api.py
--rwxrwxrwx   0 root         (0) root         (0)      558 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/context.py
--rwxrwxrwx   0 root         (0) root         (0)     3422 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/dataclass_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/decorators.py
--rwxrwxrwx   0 root         (0) root         (0)      593 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/error.py
--rwxrwxrwx   0 root         (0) root         (0)       52 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/exception.py
--rwxrwxrwx   0 root         (0) root         (0)     5868 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/executor.py
--rwxrwxrwx   0 root         (0) root         (0)    24330 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/mapper.py
--rwxrwxrwx   0 root         (0) root         (0)     3070 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/middleware.py
--rwxrwxrwx   0 root         (0) root         (0)     6756 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/reduce.py
--rwxrwxrwx   0 root         (0) root         (0)     3154 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/relay.py
--rwxrwxrwx   0 root         (0) root         (0)    32869 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/remote.py
--rwxrwxrwx   0 root         (0) root         (0)     4155 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/types.py
--rwxrwxrwx   0 root         (0) root         (0)     5896 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 19:27:46.311406 graphql-api-1.3.8/graphql_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1946 2023-05-17 19:27:46.000000 graphql-api-1.3.8/graphql_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      830 2023-05-17 19:27:46.000000 graphql-api-1.3.8/graphql_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 19:27:46.000000 graphql-api-1.3.8/graphql_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-17 19:27:46.000000 graphql-api-1.3.8/graphql_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-17 19:27:46.000000 graphql-api-1.3.8/graphql_api.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-17 19:27:46.314406 graphql-api-1.3.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1413 2023-05-17 19:27:38.000000 graphql-api-1.3.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 19:27:46.313406 graphql-api-1.3.8/tests/
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5704 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_custom_types.py
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_dataclass.py
--rwxrwxrwx   0 root         (0) root         (0)     6125 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_docstrings.py
--rwxrwxrwx   0 root         (0) root         (0)     3316 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_error.py
--rwxrwxrwx   0 root         (0) root         (0)     6939 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_filtering.py
--rwxrwxrwx   0 root         (0) root         (0)    35981 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_graphql.py
--rwxrwxrwx   0 root         (0) root         (0)     4026 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_relay.py
--rwxrwxrwx   0 root         (0) root         (0)    21648 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_remote.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3543 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:54:46.120524 graphql-api-1.3.9/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-06-04 11:54:38.000000 graphql-api-1.3.9/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       73 2023-06-04 11:54:38.000000 graphql-api-1.3.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-06-04 11:54:46.120524 graphql-api-1.3.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1270 2023-06-04 11:54:38.000000 graphql-api-1.3.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-06-04 11:54:45.000000 graphql-api-1.3.9/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:54:46.117524 graphql-api-1.3.9/graphql_api/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-06-04 11:54:38.000000 graphql-api-1.3.9/graphql_api/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7527 2023-06-04 11:54:38.000000 graphql-api-1.3.9/graphql_api/api.py
+-rwxrwxrwx   0 root         (0) root         (0)      558 2023-06-04 11:54:38.000000 graphql-api-1.3.9/graphql_api/context.py
+-rwxrwxrwx   0 root         (0) root         (0)     3422 2023-06-04 11:54:38.000000 graphql-api-1.3.9/graphql_api/dataclass_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-06-04 11:54:38.000000 graphql-api-1.3.9/graphql_api/decorators.py
+-rwxrwxrwx   0 root         (0) root         (0)      593 2023-06-04 11:54:38.000000 graphql-api-1.3.9/graphql_api/error.py
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-06-04 11:54:38.000000 graphql-api-1.3.9/graphql_api/exception.py
+-rwxrwxrwx   0 root         (0) root         (0)     5951 2023-06-04 11:54:38.000000 graphql-api-1.3.9/graphql_api/executor.py
+-rwxrwxrwx   0 root         (0) root         (0)    24330 2023-06-04 11:54:38.000000 graphql-api-1.3.9/graphql_api/mapper.py
+-rwxrwxrwx   0 root         (0) root         (0)     3302 2023-06-04 11:54:38.000000 graphql-api-1.3.9/graphql_api/middleware.py
+-rwxrwxrwx   0 root         (0) root         (0)     6756 2023-06-04 11:54:38.000000 graphql-api-1.3.9/graphql_api/reduce.py
+-rwxrwxrwx   0 root         (0) root         (0)     3154 2023-06-04 11:54:38.000000 graphql-api-1.3.9/graphql_api/relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    32869 2023-06-04 11:54:38.000000 graphql-api-1.3.9/graphql_api/remote.py
+-rwxrwxrwx   0 root         (0) root         (0)     4155 2023-06-04 11:54:38.000000 graphql-api-1.3.9/graphql_api/types.py
+-rwxrwxrwx   0 root         (0) root         (0)     5896 2023-06-04 11:54:38.000000 graphql-api-1.3.9/graphql_api/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:54:46.118524 graphql-api-1.3.9/graphql_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-06-04 11:54:46.000000 graphql-api-1.3.9/graphql_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      850 2023-06-04 11:54:46.000000 graphql-api-1.3.9/graphql_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 11:54:46.000000 graphql-api-1.3.9/graphql_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-04 11:54:46.000000 graphql-api-1.3.9/graphql_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-04 11:54:46.000000 graphql-api-1.3.9/graphql_api.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-06-04 11:54:46.121524 graphql-api-1.3.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1413 2023-06-04 11:54:38.000000 graphql-api-1.3.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:54:46.120524 graphql-api-1.3.9/tests/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-06-04 11:54:38.000000 graphql-api-1.3.9/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1368 2023-06-04 11:54:38.000000 graphql-api-1.3.9/tests/test_async.py
+-rwxrwxrwx   0 root         (0) root         (0)     5704 2023-06-04 11:54:38.000000 graphql-api-1.3.9/tests/test_custom_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-06-04 11:54:38.000000 graphql-api-1.3.9/tests/test_dataclass.py
+-rwxrwxrwx   0 root         (0) root         (0)     6125 2023-06-04 11:54:38.000000 graphql-api-1.3.9/tests/test_docstrings.py
+-rwxrwxrwx   0 root         (0) root         (0)     3316 2023-06-04 11:54:38.000000 graphql-api-1.3.9/tests/test_error.py
+-rwxrwxrwx   0 root         (0) root         (0)     6939 2023-06-04 11:54:38.000000 graphql-api-1.3.9/tests/test_filtering.py
+-rwxrwxrwx   0 root         (0) root         (0)    35981 2023-06-04 11:54:38.000000 graphql-api-1.3.9/tests/test_graphql.py
+-rwxrwxrwx   0 root         (0) root         (0)     4026 2023-06-04 11:54:38.000000 graphql-api-1.3.9/tests/test_relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    21648 2023-06-04 11:54:38.000000 graphql-api-1.3.9/tests/test_remote.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-06-04 11:54:38.000000 graphql-api-1.3.9/tests/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2023-06-04 11:54:38.000000 graphql-api-1.3.9/tests/test_subscriptions.py
```

### Comparing `graphql-api-1.3.8/LICENSE` & `graphql-api-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/PKG-INFO` & `graphql-api-1.3.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.3.8
+Version: 1.3.9
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.8/graphql-api-v1.3.8.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.9/graphql-api-v1.3.9.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql-api-1.3.8/README.md` & `graphql-api-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/graphql_api/api.py` & `graphql-api-1.3.9/graphql_api/api.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/graphql_api/context.py` & `graphql-api-1.3.9/graphql_api/context.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/graphql_api/dataclass_mapping.py` & `graphql-api-1.3.9/graphql_api/dataclass_mapping.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/graphql_api/error.py` & `graphql-api-1.3.9/graphql_api/error.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/graphql_api/executor.py` & `graphql-api-1.3.9/graphql_api/executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from graphql_api.context import GraphQLContext
 from graphql_api.middleware import (
     middleware_field_context,
     middleware_request_context,
     middleware_local_proxy,
     middleware_adapt_enum,
-    middleware_catch_exception,
+    middleware_catch_exception, middleware_call_coroutine,
 )
 
 
 class GraphQLBaseExecutor:
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.validate()
@@ -87,14 +87,15 @@
             middleware = []
 
         middleware.insert(0, middleware_catch_exception)
         middleware.insert(0, middleware_field_context)
         middleware.insert(0, middleware_request_context)
         middleware.insert(0, middleware_local_proxy)
         middleware.insert(0, middleware_adapt_enum)
+        middleware.insert(0, middleware_call_coroutine)
 
         self.meta = meta
         self.schema = schema
         self.middleware = middleware
         self.root_value = root_value
         self.middleware_on_introspection = middleware_on_introspection
         self.execution_context_class = (
```

### Comparing `graphql-api-1.3.8/graphql_api/mapper.py` & `graphql-api-1.3.9/graphql_api/mapper.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/graphql_api/middleware.py` & `graphql-api-1.3.9/graphql_api/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import enum
+import inspect
+
+import asyncio
 import sys
 import traceback
 
 from graphql import GraphQLObjectType, GraphQLNonNull, GraphQLResolveInfo
 
 from graphql_api.mapper import GraphQLMetaKey
 
@@ -49,14 +52,25 @@
 
     if isinstance(value, Exception):
         raise value
 
     return value
 
 
+def middleware_call_coroutine(next):
+    """
+    GraphQL middleware, call coroutine
+    """
+    value = next()
+    if inspect.iscoroutine(value):
+        value = asyncio.run(value)
+
+    return value
+
+
 def middleware_adapt_enum(next):
     """
     GraphQL middleware, by default enums return the value
     """
     value = next()
     if isinstance(value, enum.Enum):
         value = value.value
```

### Comparing `graphql-api-1.3.8/graphql_api/reduce.py` & `graphql-api-1.3.9/graphql_api/reduce.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/graphql_api/relay.py` & `graphql-api-1.3.9/graphql_api/relay.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/graphql_api/remote.py` & `graphql-api-1.3.9/graphql_api/remote.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/graphql_api/types.py` & `graphql-api-1.3.9/graphql_api/types.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/graphql_api/utils.py` & `graphql-api-1.3.9/graphql_api/utils.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/graphql_api.egg-info/PKG-INFO` & `graphql-api-1.3.9/graphql_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.3.8
+Version: 1.3.9
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.8/graphql-api-v1.3.8.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.9/graphql-api-v1.3.9.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql-api-1.3.8/graphql_api.egg-info/SOURCES.txt` & `graphql-api-1.3.9/graphql_api.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 graphql_api/utils.py
 graphql_api.egg-info/PKG-INFO
 graphql_api.egg-info/SOURCES.txt
 graphql_api.egg-info/dependency_links.txt
 graphql_api.egg-info/requires.txt
 graphql_api.egg-info/top_level.txt
 tests/__init__.py
+tests/test_async.py
 tests/test_custom_types.py
 tests/test_dataclass.py
 tests/test_docstrings.py
 tests/test_error.py
 tests/test_filtering.py
 tests/test_graphql.py
 tests/test_relay.py
```

### Comparing `graphql-api-1.3.8/setup.py` & `graphql-api-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/tests/test_custom_types.py` & `graphql-api-1.3.9/tests/test_custom_types.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/tests/test_dataclass.py` & `graphql-api-1.3.9/tests/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/tests/test_docstrings.py` & `graphql-api-1.3.9/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/tests/test_error.py` & `graphql-api-1.3.9/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/tests/test_filtering.py` & `graphql-api-1.3.9/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/tests/test_graphql.py` & `graphql-api-1.3.9/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/tests/test_relay.py` & `graphql-api-1.3.9/tests/test_relay.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/tests/test_remote.py` & `graphql-api-1.3.9/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/tests/test_schema.py` & `graphql-api-1.3.9/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.8/tests/test_subscriptions.py` & `graphql-api-1.3.9/tests/test_subscriptions.py`

 * *Files identical despite different names*

