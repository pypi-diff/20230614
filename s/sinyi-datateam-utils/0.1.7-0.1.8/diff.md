# Comparing `tmp/sinyi_datateam_utils-0.1.7.tar.gz` & `tmp/sinyi_datateam_utils-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinyi_datateam_utils-0.1.7.tar", last modified: Wed Jun 14 03:04:43 2023, max compression
+gzip compressed data, was "sinyi_datateam_utils-0.1.8.tar", last modified: Wed Jun 14 03:37:09 2023, max compression
```

## Comparing `sinyi_datateam_utils-0.1.7.tar` & `sinyi_datateam_utils-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-06-14 03:04:43.316691 sinyi_datateam_utils-0.1.7/
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2406 2023-06-14 03:04:43.316691 sinyi_datateam_utils-0.1.7/PKG-INFO
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2180 2022-12-16 02:49:49.000000 sinyi_datateam_utils-0.1.7/README.md
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       38 2023-06-14 03:04:43.316691 sinyi_datateam_utils-0.1.7/setup.cfg
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)      646 2023-06-14 03:04:12.000000 sinyi_datateam_utils-0.1.7/setup.py
-drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-06-14 03:04:43.312691 sinyi_datateam_utils-0.1.7/sinyi_datateam_utils.egg-info/
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2406 2023-06-14 03:04:43.000000 sinyi_datateam_utils-0.1.7/sinyi_datateam_utils.egg-info/PKG-INFO
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)      316 2023-06-14 03:04:43.000000 sinyi_datateam_utils-0.1.7/sinyi_datateam_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        1 2023-06-14 03:04:43.000000 sinyi_datateam_utils-0.1.7/sinyi_datateam_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       83 2023-06-14 03:04:43.000000 sinyi_datateam_utils-0.1.7/sinyi_datateam_utils.egg-info/requires.txt
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       12 2023-06-14 03:04:43.000000 sinyi_datateam_utils-0.1.7/sinyi_datateam_utils.egg-info/top_level.txt
-drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-06-14 03:04:43.316691 sinyi_datateam_utils-0.1.7/sinyi_utils/
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2022-12-06 02:44:18.000000 sinyi_datateam_utils-0.1.7/sinyi_utils/__init__.py
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2634 2022-12-16 02:49:49.000000 sinyi_datateam_utils-0.1.7/sinyi_utils/db_connector.py
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     3769 2023-06-14 03:02:54.000000 sinyi_datateam_utils-0.1.7/sinyi_utils/format_tool.py
+drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-06-14 03:37:09.056800 sinyi_datateam_utils-0.1.8/
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2406 2023-06-14 03:37:09.056800 sinyi_datateam_utils-0.1.8/PKG-INFO
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2180 2022-12-16 02:49:49.000000 sinyi_datateam_utils-0.1.8/README.md
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       38 2023-06-14 03:37:09.056800 sinyi_datateam_utils-0.1.8/setup.cfg
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)      646 2023-06-14 03:36:50.000000 sinyi_datateam_utils-0.1.8/setup.py
+drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-06-14 03:37:09.056800 sinyi_datateam_utils-0.1.8/sinyi_datateam_utils.egg-info/
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2406 2023-06-14 03:37:09.000000 sinyi_datateam_utils-0.1.8/sinyi_datateam_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)      316 2023-06-14 03:37:09.000000 sinyi_datateam_utils-0.1.8/sinyi_datateam_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        1 2023-06-14 03:37:09.000000 sinyi_datateam_utils-0.1.8/sinyi_datateam_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       83 2023-06-14 03:37:09.000000 sinyi_datateam_utils-0.1.8/sinyi_datateam_utils.egg-info/requires.txt
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       12 2023-06-14 03:37:09.000000 sinyi_datateam_utils-0.1.8/sinyi_datateam_utils.egg-info/top_level.txt
+drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-06-14 03:37:09.056800 sinyi_datateam_utils-0.1.8/sinyi_utils/
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2022-12-06 02:44:18.000000 sinyi_datateam_utils-0.1.8/sinyi_utils/__init__.py
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2634 2022-12-16 02:49:49.000000 sinyi_datateam_utils-0.1.8/sinyi_utils/db_connector.py
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     3561 2023-06-14 03:36:50.000000 sinyi_datateam_utils-0.1.8/sinyi_utils/format_tool.py
```

### Comparing `sinyi_datateam_utils-0.1.7/PKG-INFO` & `sinyi_datateam_utils-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinyi_datateam_utils
-Version: 0.1.7
+Version: 0.1.8
 Summary: Utilities for data analysis
 Home-page: https://SinyiDataTeam@dev.azure.com/SinyiDataTeam/Label360/_git/sinyi_utils
 Author: sinyidatateam
 Author-email: me30@sinyi.com.tw
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `sinyi_datateam_utils-0.1.7/README.md` & `sinyi_datateam_utils-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `sinyi_datateam_utils-0.1.7/setup.py` & `sinyi_datateam_utils-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
   
 with open("README.md", "r") as fh:
     description = fh.read()
   
 setuptools.setup(
     name="sinyi_datateam_utils",
-    version="0.1.7",
+    version="0.1.8",
     author="sinyidatateam",
     author_email="me30@sinyi.com.tw",
     packages=["sinyi_utils"],
     description="Utilities for data analysis",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://SinyiDataTeam@dev.azure.com/SinyiDataTeam/Label360/_git/sinyi_utils",
```

### Comparing `sinyi_datateam_utils-0.1.7/sinyi_datateam_utils.egg-info/PKG-INFO` & `sinyi_datateam_utils-0.1.8/sinyi_datateam_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinyi-datateam-utils
-Version: 0.1.7
+Version: 0.1.8
 Summary: Utilities for data analysis
 Home-page: https://SinyiDataTeam@dev.azure.com/SinyiDataTeam/Label360/_git/sinyi_utils
 Author: sinyidatateam
 Author-email: me30@sinyi.com.tw
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `sinyi_datateam_utils-0.1.7/sinyi_utils/db_connector.py` & `sinyi_datateam_utils-0.1.8/sinyi_utils/db_connector.py`

 * *Files identical despite different names*

### Comparing `sinyi_datateam_utils-0.1.7/sinyi_utils/format_tool.py` & `sinyi_datateam_utils-0.1.8/sinyi_utils/format_tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 from pathlib import Path
-from databricks.sdk.runtime import *
 import sqlalchemy
 from sqlalchemy.engine import URL
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad
 import base64
 import requests
 
@@ -16,17 +15,17 @@
             year = roc_era[:-4]
             year = str(int(year)+1911)
             return year+roc_era[-4:]
         else:
             return None
 
 class AESCrypto:
-    def __init__(self):
-        self.key = dbutils.secrets.get(scope = "label360-kv-dev", key = "AESCrypto-key")
-        self.iv =  dbutils.secrets.get(scope = "label360-kv-dev", key = "AESCrypto-iv")
+    def __init__(self, secrect_key, secrect_iv):
+        self.key = secrect_key
+        self.iv =  secrect_iv
     def decrypt(self, text:str)-> str:
         # decrypt text
         if text:
             cipher = AES.new(self.key, AES.MODE_CBC, self.iv)
 
             decryptByts = base64.b64decode(text)
             msg = cipher.decrypt(decryptByts)
@@ -43,22 +42,22 @@
 
         msg = cipher.encrypt(text)
         msg = base64.b64encode(msg)
 
         return msg.decode('utf8')
 
 class Road8:
-    road8_api_key = dbutils.secrets.get(scope = "label360-kv-dev", key = "road8-api-key")
-    url = dbutils.secrets.get(scope = "label360-kv-dev", key = "road8-host")
+    def __init__(self, api_key, host):
+        self.road8_api_key = api_key
+        self.url =  host
 
-    @classmethod
-    def normalize(cls, address = None):
+    def normalize(self, address = None):
         address = address.replace('\u3000','')
-        normalize_url = cls.url + '/Api/Normalization'
-        params = {'key': cls.road8_api_key, 
+        normalize_url = self.url + '/Api/Normalization'
+        params = {'key': self.road8_api_key, 
                 'zip': 'zip33', 
                 'update': 0,
                 'exist': 1,
                 'locate':1,
                 'addr' : address}
         error_json={
              'source_address': address,
```

