# Comparing `tmp/chasha-0.0.1.tar.gz` & `tmp/chasha-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chasha-0.0.1.tar", last modified: Wed Jun 14 19:14:22 2023, max compression
+gzip compressed data, was "chasha-0.0.2.tar", last modified: Wed Jun 14 19:55:06 2023, max compression
```

## Comparing `chasha-0.0.1.tar` & `chasha-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:14:22.733098 chasha-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-14 19:14:12.000000 chasha-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-06-14 19:14:22.733098 chasha-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-14 19:14:12.000000 chasha-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:14:22.729098 chasha-0.0.1/chasha/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-14 19:14:12.000000 chasha-0.0.1/chasha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:14:22.729098 chasha-0.0.1/chasha/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:14:12.000000 chasha-0.0.1/chasha/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:14:22.729098 chasha-0.0.1/chasha/contrib/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:14:12.000000 chasha-0.0.1/chasha/contrib/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-14 19:14:12.000000 chasha-0.0.1/chasha/contrib/adapters/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-14 19:14:12.000000 chasha-0.0.1/chasha/contrib/adapters/yandex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-14 19:14:12.000000 chasha-0.0.1/chasha/contrib/client_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    22034 2023-06-14 19:14:12.000000 chasha-0.0.1/chasha/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:14:22.729098 chasha-0.0.1/chasha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-06-14 19:14:22.000000 chasha-0.0.1/chasha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-14 19:14:22.000000 chasha-0.0.1/chasha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:14:22.000000 chasha-0.0.1/chasha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 19:14:22.000000 chasha-0.0.1/chasha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-14 19:14:12.000000 chasha-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 19:14:22.733098 chasha-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:14:22.733098 chasha-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-14 19:14:12.000000 chasha-0.0.1/tests/test_di.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-14 19:14:12.000000 chasha-0.0.1/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-14 19:14:12.000000 chasha-0.0.1/tests/test_query_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-14 19:14:12.000000 chasha-0.0.1/tests/test_router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:06.443842 chasha-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-14 19:54:55.000000 chasha-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-06-14 19:55:06.443842 chasha-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-14 19:54:55.000000 chasha-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:06.439842 chasha-0.0.2/chasha/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-14 19:54:55.000000 chasha-0.0.2/chasha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:06.443842 chasha-0.0.2/chasha/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:54:55.000000 chasha-0.0.2/chasha/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:06.443842 chasha-0.0.2/chasha/contrib/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:54:55.000000 chasha-0.0.2/chasha/contrib/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-14 19:54:55.000000 chasha-0.0.2/chasha/contrib/adapters/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-14 19:54:55.000000 chasha-0.0.2/chasha/contrib/adapters/yandex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-14 19:54:55.000000 chasha-0.0.2/chasha/contrib/client_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22034 2023-06-14 19:54:55.000000 chasha-0.0.2/chasha/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:06.439842 chasha-0.0.2/chasha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-06-14 19:55:06.000000 chasha-0.0.2/chasha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-14 19:55:06.000000 chasha-0.0.2/chasha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:55:06.000000 chasha-0.0.2/chasha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 19:55:06.000000 chasha-0.0.2/chasha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-14 19:54:55.000000 chasha-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 19:55:06.443842 chasha-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:06.443842 chasha-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-14 19:54:55.000000 chasha-0.0.2/tests/test_di.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-14 19:54:55.000000 chasha-0.0.2/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-14 19:54:55.000000 chasha-0.0.2/tests/test_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-14 19:54:55.000000 chasha-0.0.2/tests/test_router.py
```

### Comparing `chasha-0.0.1/LICENSE.txt` & `chasha-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chasha-0.0.1/PKG-INFO` & `chasha-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chasha
-Version: 0.0.1
+Version: 0.0.2
 Summary: Microframework for serverless functions
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 Chasha
 ---
```

### Comparing `chasha-0.0.1/README.md` & `chasha-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `chasha-0.0.1/chasha/__init__.py` & `chasha-0.0.2/chasha/__init__.py`

 * *Files identical despite different names*

### Comparing `chasha-0.0.1/chasha/contrib/adapters/wsgi.py` & `chasha-0.0.2/chasha/contrib/adapters/wsgi.py`

 * *Files identical despite different names*

### Comparing `chasha-0.0.1/chasha/contrib/adapters/yandex.py` & `chasha-0.0.2/chasha/contrib/adapters/yandex.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import base64
 from urllib.parse import urlparse
 from chasha import Chasha, Request
 
 
 class YandexCloudAdapter:
     """
     Adapter for Yandex Cloud Functions
@@ -20,20 +21,24 @@
     @staticmethod
     def _get_path(url: str):
         result = urlparse(url)
         return result.path
 
     @classmethod
     def adapt_request(cls, event):
+        body = event.get('body', '')
+        if body and event.get('isBase64Encoded'):
+            body = base64.b64decode(body).decode('utf-8')
+
         request = Request(
             method=event['httpMethod'],
             query=cls._denormalize_multi_value(event.get('multiValueQueryStringParameters', {})),
             headers=event.get('headers', {}),
             path=cls._get_path(event['url']),
-            body=event.get('body', ''),
+            body=body,
             raw=event
         )
         return request
 
     @classmethod
     def adapt_response(cls, response):
         headers = {}
```

### Comparing `chasha-0.0.1/chasha/contrib/client_session.py` & `chasha-0.0.2/chasha/contrib/client_session.py`

 * *Files identical despite different names*

### Comparing `chasha-0.0.1/chasha/core.py` & `chasha-0.0.2/chasha/core.py`

 * *Files identical despite different names*

### Comparing `chasha-0.0.1/chasha.egg-info/PKG-INFO` & `chasha-0.0.2/chasha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chasha
-Version: 0.0.1
+Version: 0.0.2
 Summary: Microframework for serverless functions
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 Chasha
 ---
```

### Comparing `chasha-0.0.1/tests/test_di.py` & `chasha-0.0.2/tests/test_di.py`

 * *Files identical despite different names*

### Comparing `chasha-0.0.1/tests/test_http.py` & `chasha-0.0.2/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `chasha-0.0.1/tests/test_query_params.py` & `chasha-0.0.2/tests/test_query_params.py`

 * *Files identical despite different names*

### Comparing `chasha-0.0.1/tests/test_router.py` & `chasha-0.0.2/tests/test_router.py`

 * *Files identical despite different names*

