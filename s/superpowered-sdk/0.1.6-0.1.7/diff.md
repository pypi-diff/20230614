# Comparing `tmp/superpowered-sdk-0.1.6.tar.gz` & `tmp/superpowered-sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpowered-sdk-0.1.6.tar", last modified: Tue Jun  6 07:26:12 2023, max compression
+gzip compressed data, was "superpowered-sdk-0.1.7.tar", last modified: Wed Jun 14 01:27:32 2023, max compression
```

## Comparing `superpowered-sdk-0.1.6.tar` & `superpowered-sdk-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:26:12.983679 superpowered-sdk-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-06 07:26:12.983679 superpowered-sdk-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-06 07:25:55.000000 superpowered-sdk-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 07:26:12.983679 superpowered-sdk-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-06 07:25:55.000000 superpowered-sdk-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:26:12.979679 superpowered-sdk-0.1.6/superpowered/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-06 07:25:55.000000 superpowered-sdk-0.1.6/superpowered/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-06 07:25:55.000000 superpowered-sdk-0.1.6/superpowered/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-06-06 07:25:55.000000 superpowered-sdk-0.1.6/superpowered/superpowered.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:26:12.983679 superpowered-sdk-0.1.6/superpowered_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-06 07:26:12.000000 superpowered-sdk-0.1.6/superpowered_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-06 07:26:12.000000 superpowered-sdk-0.1.6/superpowered_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 07:26:12.000000 superpowered-sdk-0.1.6/superpowered_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 07:26:12.000000 superpowered-sdk-0.1.6/superpowered_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 07:26:12.000000 superpowered-sdk-0.1.6/superpowered_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:32.086274 superpowered-sdk-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-14 01:27:32.086274 superpowered-sdk-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-14 01:27:21.000000 superpowered-sdk-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 01:27:32.086274 superpowered-sdk-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-14 01:27:21.000000 superpowered-sdk-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:32.086274 superpowered-sdk-0.1.7/superpowered/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-14 01:27:21.000000 superpowered-sdk-0.1.7/superpowered/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-14 01:27:21.000000 superpowered-sdk-0.1.7/superpowered/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-06-14 01:27:21.000000 superpowered-sdk-0.1.7/superpowered/superpowered.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:32.086274 superpowered-sdk-0.1.7/superpowered_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-14 01:27:31.000000 superpowered-sdk-0.1.7/superpowered_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-14 01:27:32.000000 superpowered-sdk-0.1.7/superpowered_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:27:31.000000 superpowered-sdk-0.1.7/superpowered_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 01:27:31.000000 superpowered-sdk-0.1.7/superpowered_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 01:27:31.000000 superpowered-sdk-0.1.7/superpowered_sdk.egg-info/top_level.txt
```

### Comparing `superpowered-sdk-0.1.6/PKG-INFO` & `superpowered-sdk-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpowered-sdk
-Version: 0.1.6
+Version: 0.1.7
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
-Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.7 Summary:
 Superpowered AI SDK Home-page: https://superpowered.ai Author: superpowered
 Author-email: justin@superpowered.ai License: Proprietary License Project-URL:
 Homepage, https://superpowered.ai Project-URL: Documentation, https://
 superpowered.ai/docs Project-URL: Contact, https://superpowered.ai/contact/
 Project-URL: End-User License Agreement, https://superpowered.ai/api-user-
 agreement/ Description: # This is the official Superpowered AI Python SDK ##
 Installation `pip install superpowered-sdk` _Note_: To create API keys, please
```

### Comparing `superpowered-sdk-0.1.6/README.md` & `superpowered-sdk-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.6/setup.py` & `superpowered-sdk-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.6/superpowered/__init__.py` & `superpowered-sdk-0.1.7/superpowered/__init__.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.6/superpowered/exceptions.py` & `superpowered-sdk-0.1.7/superpowered/exceptions.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.6/superpowered/superpowered.py` & `superpowered-sdk-0.1.7/superpowered/superpowered.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,18 +226,18 @@
         'Content-MD5': encoded_md5,
     }
     args = {
         'url': resp['temporary_url'],
         'data': file_content,
         'headers': headers,
     }
-    with requests.put(**args) as resp:
+    with requests.put(**args) as r:
         pass
 
-    return {'message': 'Successfully uploaded file. Vectorization process will begin shortly.'}
+    return resp['document']
 
 
 def download_file(knowledge_base_id: str, file_name: str, destination_path: str = None) -> bytes:
     """
     POST /knowledge_bases/{knowledge_base_id}/documents/request_signed_file_url
     +
     GET response['temporary_url']
```

### Comparing `superpowered-sdk-0.1.6/superpowered_sdk.egg-info/PKG-INFO` & `superpowered-sdk-0.1.7/superpowered_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpowered-sdk
-Version: 0.1.6
+Version: 0.1.7
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
-Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.7 Summary:
 Superpowered AI SDK Home-page: https://superpowered.ai Author: superpowered
 Author-email: justin@superpowered.ai License: Proprietary License Project-URL:
 Homepage, https://superpowered.ai Project-URL: Documentation, https://
 superpowered.ai/docs Project-URL: Contact, https://superpowered.ai/contact/
 Project-URL: End-User License Agreement, https://superpowered.ai/api-user-
 agreement/ Description: # This is the official Superpowered AI Python SDK ##
 Installation `pip install superpowered-sdk` _Note_: To create API keys, please
```

