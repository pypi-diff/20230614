# Comparing `tmp/test_graphql_sdk-0.1.0.tar.gz` & `tmp/test_graphql_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_graphql_sdk-0.1.0.tar", last modified: Tue Jun  6 10:10:29 2023, max compression
+gzip compressed data, was "test_graphql_sdk-0.1.1.tar", last modified: Wed Jun 14 07:58:02 2023, max compression
```

## Comparing `test_graphql_sdk-0.1.0.tar` & `test_graphql_sdk-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-06 10:10:29.729888 test_graphql_sdk-0.1.0/
--rw-r--r--   0 sarvesh    (501) staff       (20)     3133 2023-06-06 10:10:29.729944 test_graphql_sdk-0.1.0/PKG-INFO
--rw-r--r--   0 sarvesh    (501) staff       (20)     2621 2023-06-06 09:14:13.000000 test_graphql_sdk-0.1.0/README.md
--rw-r--r--   0 sarvesh    (501) staff       (20)       85 2023-05-31 07:35:04.000000 test_graphql_sdk-0.1.0/pyproject.toml
--rw-r--r--   0 sarvesh    (501) staff       (20)      716 2023-06-06 10:10:29.730181 test_graphql_sdk-0.1.0/setup.cfg
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-06 10:10:29.728013 test_graphql_sdk-0.1.0/src/
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-06 10:10:29.729097 test_graphql_sdk-0.1.0/src/airstack/
--rw-r--r--   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:53:03.000000 test_graphql_sdk-0.1.0/src/airstack/__init__.py
--rw-r--r--   0 sarvesh    (501) staff       (20)      308 2023-06-06 08:53:37.000000 test_graphql_sdk-0.1.0/src/airstack/constant.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     6370 2023-06-06 09:32:09.000000 test_graphql_sdk-0.1.0/src/airstack/execute_query.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     5805 2023-06-06 08:57:11.000000 test_graphql_sdk-0.1.0/src/airstack/generic.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     1816 2023-06-06 08:57:31.000000 test_graphql_sdk-0.1.0/src/airstack/send_request.py
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-06 10:10:29.729761 test_graphql_sdk-0.1.0/src/test_graphql_sdk.egg-info/
--rw-r--r--   0 sarvesh    (501) staff       (20)     3133 2023-06-06 10:10:29.000000 test_graphql_sdk-0.1.0/src/test_graphql_sdk.egg-info/PKG-INFO
--rw-r--r--   0 sarvesh    (501) staff       (20)      386 2023-06-06 10:10:29.000000 test_graphql_sdk-0.1.0/src/test_graphql_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-06 10:10:29.000000 test_graphql_sdk-0.1.0/src/test_graphql_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)       35 2023-06-06 10:10:29.000000 test_graphql_sdk-0.1.0/src/test_graphql_sdk.egg-info/requires.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)        9 2023-06-06 10:10:29.000000 test_graphql_sdk-0.1.0/src/test_graphql_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-14 07:58:02.876209 test_graphql_sdk-0.1.1/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3163 2023-06-14 07:58:02.876278 test_graphql_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)     2651 2023-06-09 12:45:46.000000 test_graphql_sdk-0.1.1/README.md
+-rw-r--r--   0 sarvesh    (501) staff       (20)       85 2023-06-09 12:45:46.000000 test_graphql_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0 sarvesh    (501) staff       (20)      716 2023-06-14 07:58:02.876551 test_graphql_sdk-0.1.1/setup.cfg
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-14 07:58:02.873484 test_graphql_sdk-0.1.1/src/
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-14 07:58:02.875106 test_graphql_sdk-0.1.1/src/airstack/
+-rw-r--r--   0 sarvesh    (501) staff       (20)        0 2023-06-09 12:45:46.000000 test_graphql_sdk-0.1.1/src/airstack/__init__.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)      308 2023-06-09 12:45:46.000000 test_graphql_sdk-0.1.1/src/airstack/constant.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     6374 2023-06-14 07:39:08.000000 test_graphql_sdk-0.1.1/src/airstack/execute_query.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     5805 2023-06-09 12:45:46.000000 test_graphql_sdk-0.1.1/src/airstack/generic.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     1811 2023-06-09 12:45:46.000000 test_graphql_sdk-0.1.1/src/airstack/send_request.py
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-14 07:58:02.876028 test_graphql_sdk-0.1.1/src/test_graphql_sdk.egg-info/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3163 2023-06-14 07:58:02.000000 test_graphql_sdk-0.1.1/src/test_graphql_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)      386 2023-06-14 07:58:02.000000 test_graphql_sdk-0.1.1/src/test_graphql_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-14 07:58:02.000000 test_graphql_sdk-0.1.1/src/test_graphql_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)       35 2023-06-14 07:58:02.000000 test_graphql_sdk-0.1.1/src/test_graphql_sdk.egg-info/requires.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        9 2023-06-14 07:58:02.000000 test_graphql_sdk-0.1.1/src/test_graphql_sdk.egg-info/top_level.txt
```

### Comparing `test_graphql_sdk-0.1.0/PKG-INFO` & `test_graphql_sdk-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_graphql_sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Sarvesh
 Author-email: sarveshsingh.03@gmail.com
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -63,14 +63,14 @@
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
 
 query_response = await api_client.execute_paginated_query(query=query, variables=variables)
 
 if query_response.has_next_page:
-    next_page_response = await get_next_page()
+    next_page_response = await query_response.get_next_page()
 
 if next_page_response.has_prev_page:
-    prev_page_response = await get_prev_page()
+    prev_page_response = await query_response.get_prev_page()
 ```
```

### Comparing `test_graphql_sdk-0.1.0/README.md` & `test_graphql_sdk-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,14 @@
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
 
 query_response = await api_client.execute_paginated_query(query=query, variables=variables)
 
 if query_response.has_next_page:
-    next_page_response = await get_next_page()
+    next_page_response = await query_response.get_next_page()
 
 if next_page_response.has_prev_page:
-    prev_page_response = await get_prev_page()
+    prev_page_response = await query_response.get_prev_page()
 ```
```

### Comparing `test_graphql_sdk-0.1.0/setup.cfg` & `test_graphql_sdk-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = test_graphql_sdk
-version = 0.1.0
+version = 0.1.1
 author = Sarvesh
 author_email = sarveshsingh.03@gmail.com
 description = Python sdk for airstack apis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Airstack-xyz/airstack-python-sdk
 project_urls =
```

### Comparing `test_graphql_sdk-0.1.0/src/airstack/execute_query.py` & `test_graphql_sdk-0.1.1/src/airstack/execute_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         Returns:
             Tuple: GraphQL response data or None, GraphQL response status code,
             error message or None
         """
         headers = {
             'Content-Type': 'application/json',
-            'x-api-key': self.api_key
+            'Authorization': self.api_key
         }
         payload = {
             'query': query,
             'variables': variables
         }
 
         response, status_code, error = await SendRequest.send_post_request(
```

### Comparing `test_graphql_sdk-0.1.0/src/airstack/generic.py` & `test_graphql_sdk-0.1.1/src/airstack/generic.py`

 * *Files identical despite different names*

### Comparing `test_graphql_sdk-0.1.0/src/airstack/send_request.py` & `test_graphql_sdk-0.1.1/src/airstack/send_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,9 +40,9 @@
                             return None, response.status, response.reason
                         return None, response.status, nt["error"]
 
                     if "errors" in nt:
                         return nt, response.status, nt["errors"]
 
                     return nt["data"], response.status, None
-            except Exception:
-                return None, response.status, "Unable to fetch data"
+            except Exception as exec:
+                return None, response.status, str(exec)
```

### Comparing `test_graphql_sdk-0.1.0/src/test_graphql_sdk.egg-info/PKG-INFO` & `test_graphql_sdk-0.1.1/src/test_graphql_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-graphql-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Sarvesh
 Author-email: sarveshsingh.03@gmail.com
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -63,14 +63,14 @@
 from airstack.execute_query import AirstackClient
 
 api_client = AirstackClient(api_key='api-key')
 
 query_response = await api_client.execute_paginated_query(query=query, variables=variables)
 
 if query_response.has_next_page:
-    next_page_response = await get_next_page()
+    next_page_response = await query_response.get_next_page()
 
 if next_page_response.has_prev_page:
-    prev_page_response = await get_prev_page()
+    prev_page_response = await query_response.get_prev_page()
 ```
```

