# Comparing `tmp/resend-0.3.0.tar.gz` & `tmp/resend-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/resend-0.3.0.tar", last modified: Tue May  2 21:42:06 2023, max compression
+gzip compressed data, was "dist/resend-0.4.0.tar", last modified: Sat May 20 18:44:07 2023, max compression
```

## Comparing `resend-0.3.0.tar` & `resend-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-05-02 21:42:06.000000 resend-0.3.0/
--rw-r--r--   0 derich     (501) staff       (20)     2653 2023-05-02 21:42:06.000000 resend-0.3.0/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)     1444 2023-05-02 00:53:58.000000 resend-0.3.0/README.md
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-05-02 21:42:06.000000 resend-0.3.0/resend/
--rw-r--r--   0 derich     (501) staff       (20)      334 2023-05-02 21:36:30.000000 resend-0.3.0/resend/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)     1019 2023-05-02 00:53:58.000000 resend-0.3.0/resend/api.py
--rw-r--r--   0 derich     (501) staff       (20)      796 2023-05-02 00:53:58.000000 resend-0.3.0/resend/api_keys.py
--rw-r--r--   0 derich     (501) staff       (20)     1033 2023-05-02 21:36:30.000000 resend-0.3.0/resend/domains.py
--rw-r--r--   0 derich     (501) staff       (20)      588 2023-05-02 00:53:58.000000 resend-0.3.0/resend/emails.py
--rw-r--r--   0 derich     (501) staff       (20)     4152 2023-05-02 21:36:30.000000 resend-0.3.0/resend/exceptions.py
--rw-r--r--   0 derich     (501) staff       (20)     1694 2023-05-02 21:36:30.000000 resend-0.3.0/resend/request.py
--rw-r--r--   0 derich     (501) staff       (20)      163 2023-05-02 21:36:45.000000 resend-0.3.0/resend/version.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-05-02 21:42:06.000000 resend-0.3.0/resend.egg-info/
--rw-r--r--   0 derich     (501) staff       (20)     2653 2023-05-02 21:42:05.000000 resend-0.3.0/resend.egg-info/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)      350 2023-05-02 21:42:06.000000 resend-0.3.0/resend.egg-info/SOURCES.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2023-05-02 21:42:05.000000 resend-0.3.0/resend.egg-info/dependency_links.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2023-05-02 21:42:05.000000 resend-0.3.0/resend.egg-info/not-zip-safe
--rw-r--r--   0 derich     (501) staff       (20)       17 2023-05-02 21:42:05.000000 resend-0.3.0/resend.egg-info/requires.txt
--rw-r--r--   0 derich     (501) staff       (20)        7 2023-05-02 21:42:05.000000 resend-0.3.0/resend.egg-info/top_level.txt
--rw-r--r--   0 derich     (501) staff       (20)       67 2023-05-02 21:42:06.000000 resend-0.3.0/setup.cfg
--rw-r--r--   0 derich     (501) staff       (20)     1112 2023-05-02 21:37:28.000000 resend-0.3.0/setup.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-05-20 18:44:07.000000 resend-0.4.0/
+-rw-r--r--   0 derich     (501) staff       (20)     2641 2023-05-20 18:44:07.000000 resend-0.4.0/PKG-INFO
+-rw-r--r--   0 derich     (501) staff       (20)     1448 2023-05-10 21:41:17.000000 resend-0.4.0/README.md
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-05-20 18:44:07.000000 resend-0.4.0/resend/
+-rw-r--r--   0 derich     (501) staff       (20)      373 2023-05-10 21:41:17.000000 resend-0.4.0/resend/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)     1059 2023-05-10 21:41:17.000000 resend-0.4.0/resend/api.py
+-rw-r--r--   0 derich     (501) staff       (20)      796 2023-05-02 00:53:58.000000 resend-0.4.0/resend/api_keys.py
+-rw-r--r--   0 derich     (501) staff       (20)     1268 2023-05-20 18:42:47.000000 resend-0.4.0/resend/domains.py
+-rw-r--r--   0 derich     (501) staff       (20)      588 2023-05-02 00:53:58.000000 resend-0.4.0/resend/emails.py
+-rw-r--r--   0 derich     (501) staff       (20)     4152 2023-05-02 21:36:30.000000 resend-0.4.0/resend/exceptions.py
+-rw-r--r--   0 derich     (501) staff       (20)     1694 2023-05-10 22:06:57.000000 resend-0.4.0/resend/request.py
+-rw-r--r--   0 derich     (501) staff       (20)      163 2023-05-20 18:42:52.000000 resend-0.4.0/resend/version.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-05-20 18:44:07.000000 resend-0.4.0/resend.egg-info/
+-rw-r--r--   0 derich     (501) staff       (20)     2641 2023-05-20 18:44:07.000000 resend-0.4.0/resend.egg-info/PKG-INFO
+-rw-r--r--   0 derich     (501) staff       (20)      350 2023-05-20 18:44:07.000000 resend-0.4.0/resend.egg-info/SOURCES.txt
+-rw-r--r--   0 derich     (501) staff       (20)        1 2023-05-20 18:44:07.000000 resend-0.4.0/resend.egg-info/dependency_links.txt
+-rw-r--r--   0 derich     (501) staff       (20)        1 2023-05-20 18:44:07.000000 resend-0.4.0/resend.egg-info/not-zip-safe
+-rw-r--r--   0 derich     (501) staff       (20)       17 2023-05-20 18:44:07.000000 resend-0.4.0/resend.egg-info/requires.txt
+-rw-r--r--   0 derich     (501) staff       (20)        7 2023-05-20 18:44:07.000000 resend-0.4.0/resend.egg-info/top_level.txt
+-rw-r--r--   0 derich     (501) staff       (20)       67 2023-05-20 18:44:07.000000 resend-0.4.0/setup.cfg
+-rw-r--r--   0 derich     (501) staff       (20)     1112 2023-05-02 21:37:28.000000 resend-0.4.0/setup.py
```

### Comparing `resend-0.3.0/PKG-INFO` & `resend-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 0.3.0
+Version: 0.4.0
 Summary: Resend Python SDK
 Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 License: UNKNOWN
 Description: # Resend Python SDK
         
@@ -53,17 +53,15 @@
             "cc": ["to@gmail.com"],
             "tags": [
                 {"name": "tag1", "value": "tagvalue1"},
                 {"name": "tag2", "value": "tagvalue2"},
             ],
         }
         
-        r = resend.Emails.send(
-        
-        )
+        r = resend.Emails.send(params)
         print(r)
         ```
         
 Keywords: email,email platform
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `resend-0.3.0/README.md` & `resend-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,12 +45,10 @@
     "cc": ["to@gmail.com"],
     "tags": [
         {"name": "tag1", "value": "tagvalue1"},
         {"name": "tag2", "value": "tagvalue2"},
     ],
 }
 
-r = resend.Emails.send(
-
-)
+r = resend.Emails.send(params)
 print(r)
 ```
```

### Comparing `resend-0.3.0/resend/api.py` & `resend-0.4.0/resend/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from warnings import warn
 from typing import Dict, List
 
 import resend
 
 
 class Resend:
     def __init__(self, api_key: str):
@@ -18,17 +19,17 @@
         cc=None,
         reply_to=None,
         html: str = None,
         text: str = None,
         attachments: List[Dict] = None,
         tags: List[Dict] = None,
     ):
-        print(
-            "[DEPRECATION]: method `send_email` is deprecated. Use resend.Emails.send() instead"  # noqa
-        )
+        warn(
+            "[DEPRECATION]: method `send_email` is deprecated. Use resend.Emails.send() instead",
+            DeprecationWarning)
         return resend.Emails.send(
             {
                 "from": sender,
                 "to": to,
                 "subject": subject,
                 "bcc": bcc,
                 "cc": cc,
```

### Comparing `resend-0.3.0/resend/api_keys.py` & `resend-0.4.0/resend/api_keys.py`

 * *Files identical despite different names*

### Comparing `resend-0.3.0/resend/domains.py` & `resend-0.4.0/resend/domains.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,20 @@
     @classmethod
     # https://resend.com/docs/api-reference/domains/create-domain
     def create(cls, params={}) -> Dict:
         path = "/domains"
         return request.Request(path=path, params=params, verb="post").perform()
 
     @classmethod
+    # https://resend.com/docs/api-reference/domains/get-domain
+    def get(cls, domain_id="") -> Dict:
+        path = f"/domains/{domain_id}"
+        return request.Request(path=path, params={}, verb="get").perform()
+
+    @classmethod
     # https://resend.com/docs/api-reference/domains/list-domains
     def list(cls) -> Dict:
         path = "/domains"
         return request.Request(path=path, params={}, verb="get").perform()
 
     @classmethod
     # https://resend.com/docs/api-reference/domains/delete-domain
```

### Comparing `resend-0.3.0/resend/emails.py` & `resend-0.4.0/resend/emails.py`

 * *Files identical despite different names*

### Comparing `resend-0.3.0/resend/exceptions.py` & `resend-0.4.0/resend/exceptions.py`

 * *Files identical despite different names*

### Comparing `resend-0.3.0/resend/request.py` & `resend-0.4.0/resend/request.py`

 * *Files identical despite different names*

### Comparing `resend-0.3.0/resend.egg-info/PKG-INFO` & `resend-0.4.0/resend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 0.3.0
+Version: 0.4.0
 Summary: Resend Python SDK
 Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 License: UNKNOWN
 Description: # Resend Python SDK
         
@@ -53,17 +53,15 @@
             "cc": ["to@gmail.com"],
             "tags": [
                 {"name": "tag1", "value": "tagvalue1"},
                 {"name": "tag2", "value": "tagvalue2"},
             ],
         }
         
-        r = resend.Emails.send(
-        
-        )
+        r = resend.Emails.send(params)
         print(r)
         ```
         
 Keywords: email,email platform
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `resend-0.3.0/setup.py` & `resend-0.4.0/setup.py`

 * *Files identical despite different names*

