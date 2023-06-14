# Comparing `tmp/sinyi_datateam_utils-0.1.5.tar.gz` & `tmp/sinyi_datateam_utils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinyi_datateam_utils-0.1.5.tar", last modified: Wed May 31 06:17:07 2023, max compression
+gzip compressed data, was "sinyi_datateam_utils-0.1.6.tar", last modified: Wed Jun 14 02:49:00 2023, max compression
```

## Comparing `sinyi_datateam_utils-0.1.5.tar` & `sinyi_datateam_utils-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-05-31 06:17:07.516218 sinyi_datateam_utils-0.1.5/
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2406 2023-05-31 06:17:07.516218 sinyi_datateam_utils-0.1.5/PKG-INFO
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2180 2022-12-16 02:49:49.000000 sinyi_datateam_utils-0.1.5/README.md
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       38 2023-05-31 06:17:07.516218 sinyi_datateam_utils-0.1.5/setup.cfg
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)      646 2023-05-31 06:16:49.000000 sinyi_datateam_utils-0.1.5/setup.py
-drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-05-31 06:17:07.512218 sinyi_datateam_utils-0.1.5/sinyi_datateam_utils.egg-info/
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2406 2023-05-31 06:17:07.000000 sinyi_datateam_utils-0.1.5/sinyi_datateam_utils.egg-info/PKG-INFO
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)      316 2023-05-31 06:17:07.000000 sinyi_datateam_utils-0.1.5/sinyi_datateam_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        1 2023-05-31 06:17:07.000000 sinyi_datateam_utils-0.1.5/sinyi_datateam_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       83 2023-05-31 06:17:07.000000 sinyi_datateam_utils-0.1.5/sinyi_datateam_utils.egg-info/requires.txt
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       12 2023-05-31 06:17:07.000000 sinyi_datateam_utils-0.1.5/sinyi_datateam_utils.egg-info/top_level.txt
-drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-05-31 06:17:07.516218 sinyi_datateam_utils-0.1.5/sinyi_utils/
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2022-12-06 02:44:18.000000 sinyi_datateam_utils-0.1.5/sinyi_utils/__init__.py
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2634 2022-12-16 02:49:49.000000 sinyi_datateam_utils-0.1.5/sinyi_utils/db_connector.py
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     3906 2023-05-31 06:15:07.000000 sinyi_datateam_utils-0.1.5/sinyi_utils/format_tool.py
+drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-06-14 02:49:00.841084 sinyi_datateam_utils-0.1.6/
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2406 2023-06-14 02:49:00.841084 sinyi_datateam_utils-0.1.6/PKG-INFO
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2180 2022-12-16 02:49:49.000000 sinyi_datateam_utils-0.1.6/README.md
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       38 2023-06-14 02:49:00.841084 sinyi_datateam_utils-0.1.6/setup.cfg
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)      646 2023-06-14 02:48:39.000000 sinyi_datateam_utils-0.1.6/setup.py
+drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-06-14 02:49:00.837084 sinyi_datateam_utils-0.1.6/sinyi_datateam_utils.egg-info/
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2406 2023-06-14 02:49:00.000000 sinyi_datateam_utils-0.1.6/sinyi_datateam_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)      316 2023-06-14 02:49:00.000000 sinyi_datateam_utils-0.1.6/sinyi_datateam_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        1 2023-06-14 02:49:00.000000 sinyi_datateam_utils-0.1.6/sinyi_datateam_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       83 2023-06-14 02:49:00.000000 sinyi_datateam_utils-0.1.6/sinyi_datateam_utils.egg-info/requires.txt
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       12 2023-06-14 02:49:00.000000 sinyi_datateam_utils-0.1.6/sinyi_datateam_utils.egg-info/top_level.txt
+drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-06-14 02:49:00.841084 sinyi_datateam_utils-0.1.6/sinyi_utils/
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2022-12-06 02:44:18.000000 sinyi_datateam_utils-0.1.6/sinyi_utils/__init__.py
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2634 2022-12-16 02:49:49.000000 sinyi_datateam_utils-0.1.6/sinyi_utils/db_connector.py
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     3732 2023-06-14 02:48:39.000000 sinyi_datateam_utils-0.1.6/sinyi_utils/format_tool.py
```

### Comparing `sinyi_datateam_utils-0.1.5/PKG-INFO` & `sinyi_datateam_utils-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinyi_datateam_utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: Utilities for data analysis
 Home-page: https://SinyiDataTeam@dev.azure.com/SinyiDataTeam/Label360/_git/sinyi_utils
 Author: sinyidatateam
 Author-email: me30@sinyi.com.tw
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `sinyi_datateam_utils-0.1.5/README.md` & `sinyi_datateam_utils-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `sinyi_datateam_utils-0.1.5/setup.py` & `sinyi_datateam_utils-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
   
 with open("README.md", "r") as fh:
     description = fh.read()
   
 setuptools.setup(
     name="sinyi_datateam_utils",
-    version="0.1.5",
+    version="0.1.6",
     author="sinyidatateam",
     author_email="me30@sinyi.com.tw",
     packages=["sinyi_utils"],
     description="Utilities for data analysis",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://SinyiDataTeam@dev.azure.com/SinyiDataTeam/Label360/_git/sinyi_utils",
```

### Comparing `sinyi_datateam_utils-0.1.5/sinyi_datateam_utils.egg-info/PKG-INFO` & `sinyi_datateam_utils-0.1.6/sinyi_datateam_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinyi-datateam-utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: Utilities for data analysis
 Home-page: https://SinyiDataTeam@dev.azure.com/SinyiDataTeam/Label360/_git/sinyi_utils
 Author: sinyidatateam
 Author-email: me30@sinyi.com.tw
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `sinyi_datateam_utils-0.1.5/sinyi_utils/db_connector.py` & `sinyi_datateam_utils-0.1.6/sinyi_utils/db_connector.py`

 * *Files identical despite different names*

### Comparing `sinyi_datateam_utils-0.1.5/sinyi_utils/format_tool.py` & `sinyi_datateam_utils-0.1.6/sinyi_utils/format_tool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 import os
-from azure.keyvault.secrets import SecretClient
-from azure.identity import EnvironmentCredential
 from pathlib import Path
 import sqlalchemy
 from sqlalchemy.engine import URL
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad
 import base64
 import requests
 
 
-# Databricks environment
-vault_url = os.environ['AZURE_VAULT_URL']
-credential = EnvironmentCredential()
-client = SecretClient(vault_url,credential=credential)
-
-
 def roc_era_to_ad(roc_era):
     roc_era = roc_era.replace('-',"").replace(" ","").replace('_',"")
     if roc_era: 
         if len(roc_era) == 6 or len(roc_era) == 7 :
             year = roc_era[:-4]
             year = str(int(year)+1911)
             return year+roc_era[-4:]
         else:
             return None
 
 class AESCrypto:
     def __init__(self):
-        self.key = client.get_secret('AESCrypto-key').value.encode("utf8")
-        self.iv =  client.get_secret('AESCrypto-iv').value.encode("utf8")
-
+        self.key = dbutils.secrets.get(scope = "label360-kv-dev", key = "AESCrypto-key")
+        self.iv =  dbutils.secrets.get(scope = "label360-kv-dev", key = "AESCrypto-iv")
     def decrypt(self, text:str)-> str:
         # decrypt text
         if text:
             cipher = AES.new(self.key, AES.MODE_CBC, self.iv)
 
             decryptByts = base64.b64decode(text)
             msg = cipher.decrypt(decryptByts)
@@ -50,18 +41,17 @@
         text = pad(text.encode('utf-8'), AES.block_size)
 
         msg = cipher.encrypt(text)
         msg = base64.b64encode(msg)
 
         return msg.decode('utf8')
 
-
 class Road8:
-    road8_api_key = client.get_secret('road8-api-key').value
-    url = client.get_secret('road8-host').value
+    road8_api_key = dbutils.secrets.get(scope = "label360-kv-dev", key = "road8-api-key")
+    url = dbutils.secrets.get(scope = "label360-kv-dev", key = "road8-host")
 
     @classmethod
     def normalize(cls, address = None):
         address = address.replace('\u3000','')
         normalize_url = cls.url + '/Api/Normalization'
         params = {'key': cls.road8_api_key, 
                 'zip': 'zip33',
```

