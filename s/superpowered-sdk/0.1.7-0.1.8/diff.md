# Comparing `tmp/superpowered-sdk-0.1.7.tar.gz` & `tmp/superpowered-sdk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpowered-sdk-0.1.7.tar", last modified: Wed Jun 14 01:27:32 2023, max compression
+gzip compressed data, was "superpowered-sdk-0.1.8.tar", last modified: Wed Jun 14 21:54:24 2023, max compression
```

## Comparing `superpowered-sdk-0.1.7.tar` & `superpowered-sdk-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:32.086274 superpowered-sdk-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-14 01:27:32.086274 superpowered-sdk-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-14 01:27:21.000000 superpowered-sdk-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 01:27:32.086274 superpowered-sdk-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-14 01:27:21.000000 superpowered-sdk-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:32.086274 superpowered-sdk-0.1.7/superpowered/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-14 01:27:21.000000 superpowered-sdk-0.1.7/superpowered/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-14 01:27:21.000000 superpowered-sdk-0.1.7/superpowered/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-06-14 01:27:21.000000 superpowered-sdk-0.1.7/superpowered/superpowered.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:32.086274 superpowered-sdk-0.1.7/superpowered_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-14 01:27:31.000000 superpowered-sdk-0.1.7/superpowered_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-14 01:27:32.000000 superpowered-sdk-0.1.7/superpowered_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:27:31.000000 superpowered-sdk-0.1.7/superpowered_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 01:27:31.000000 superpowered-sdk-0.1.7/superpowered_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 01:27:31.000000 superpowered-sdk-0.1.7/superpowered_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:54:24.579136 superpowered-sdk-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-14 21:54:24.579136 superpowered-sdk-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-14 21:54:11.000000 superpowered-sdk-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:54:24.579136 superpowered-sdk-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-14 21:54:11.000000 superpowered-sdk-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:54:24.575136 superpowered-sdk-0.1.8/superpowered/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-14 21:54:11.000000 superpowered-sdk-0.1.8/superpowered/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-14 21:54:11.000000 superpowered-sdk-0.1.8/superpowered/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-06-14 21:54:11.000000 superpowered-sdk-0.1.8/superpowered/superpowered.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:54:24.575136 superpowered-sdk-0.1.8/superpowered_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-14 21:54:24.000000 superpowered-sdk-0.1.8/superpowered_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-14 21:54:24.000000 superpowered-sdk-0.1.8/superpowered_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:54:24.000000 superpowered-sdk-0.1.8/superpowered_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 21:54:24.000000 superpowered-sdk-0.1.8/superpowered_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 21:54:24.000000 superpowered-sdk-0.1.8/superpowered_sdk.egg-info/top_level.txt
```

### Comparing `superpowered-sdk-0.1.7/PKG-INFO` & `superpowered-sdk-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpowered-sdk
-Version: 0.1.7
+Version: 0.1.8
 Summary: Superpowered AI SDK
 Home-page: https://superpowered.ai
 Author: superpowered
 Author-email: justin@superpowered.ai
 License: Proprietary License
 Project-URL: Homepage, https://superpowered.ai
 Project-URL: Documentation, https://superpowered.ai/docs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.8 Summary:
 Superpowered AI SDK Home-page: https://superpowered.ai Author: superpowered
 Author-email: justin@superpowered.ai License: Proprietary License Project-URL:
 Homepage, https://superpowered.ai Project-URL: Documentation, https://
 superpowered.ai/docs Project-URL: Contact, https://superpowered.ai/contact/
 Project-URL: End-User License Agreement, https://superpowered.ai/api-user-
 agreement/ Description: # This is the official Superpowered AI Python SDK ##
 Installation `pip install superpowered-sdk` _Note_: To create API keys, please
```

### Comparing `superpowered-sdk-0.1.7/README.md` & `superpowered-sdk-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.7/setup.py` & `superpowered-sdk-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.7/superpowered/__init__.py` & `superpowered-sdk-0.1.8/superpowered/__init__.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.7/superpowered/exceptions.py` & `superpowered-sdk-0.1.8/superpowered/exceptions.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.7/superpowered/superpowered.py` & `superpowered-sdk-0.1.8/superpowered/superpowered.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,22 +295,26 @@
         args['params']['next_page_token'] = resp['next_page_token']
         resp = make_api_call(args)
         documents.extend(resp.get('documents', []))
 
     return documents
 
 
-def get_document(knowledge_base_id: str, document_id: str) -> dict:
+def get_document(knowledge_base_id: str, document_id: str, include_content: bool = True) -> dict:
     """
     GET /knowledge_bases/{knowledge_base_id}/documents/{document_id}
     """
+    params = {
+        'include_content': include_content,
+    }
     args = {
         'method': 'GET',
         'url': f'{get_base_url()}/knowledge_bases/{knowledge_base_id}/documents/{document_id}',
         'auth': auth(),
+        'params': params,
     }
     return make_api_call(args)
 
 
 def update_document(knowledge_base_id: str, document_id: str, title: str = None, description: str = None, supp_id: str = None) -> dict:
     """
     PATCH /knowledge_bases/{knowledge_base_id}/documents/{document_id}
```

### Comparing `superpowered-sdk-0.1.7/superpowered_sdk.egg-info/PKG-INFO` & `superpowered-sdk-0.1.8/superpowered_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpowered-sdk
-Version: 0.1.7
+Version: 0.1.8
 Summary: Superpowered AI SDK
 Home-page: https://superpowered.ai
 Author: superpowered
 Author-email: justin@superpowered.ai
 License: Proprietary License
 Project-URL: Homepage, https://superpowered.ai
 Project-URL: Documentation, https://superpowered.ai/docs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.8 Summary:
 Superpowered AI SDK Home-page: https://superpowered.ai Author: superpowered
 Author-email: justin@superpowered.ai License: Proprietary License Project-URL:
 Homepage, https://superpowered.ai Project-URL: Documentation, https://
 superpowered.ai/docs Project-URL: Contact, https://superpowered.ai/contact/
 Project-URL: End-User License Agreement, https://superpowered.ai/api-user-
 agreement/ Description: # This is the official Superpowered AI Python SDK ##
 Installation `pip install superpowered-sdk` _Note_: To create API keys, please
```

