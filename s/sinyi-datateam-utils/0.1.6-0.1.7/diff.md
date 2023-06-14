# Comparing `tmp/sinyi_datateam_utils-0.1.6.tar.gz` & `tmp/sinyi_datateam_utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinyi_datateam_utils-0.1.6.tar", last modified: Wed Jun 14 02:49:00 2023, max compression
+gzip compressed data, was "sinyi_datateam_utils-0.1.7.tar", last modified: Wed Jun 14 03:04:43 2023, max compression
```

## Comparing `sinyi_datateam_utils-0.1.6.tar` & `sinyi_datateam_utils-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-06-14 02:49:00.841084 sinyi_datateam_utils-0.1.6/
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2406 2023-06-14 02:49:00.841084 sinyi_datateam_utils-0.1.6/PKG-INFO
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2180 2022-12-16 02:49:49.000000 sinyi_datateam_utils-0.1.6/README.md
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       38 2023-06-14 02:49:00.841084 sinyi_datateam_utils-0.1.6/setup.cfg
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)      646 2023-06-14 02:48:39.000000 sinyi_datateam_utils-0.1.6/setup.py
-drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-06-14 02:49:00.837084 sinyi_datateam_utils-0.1.6/sinyi_datateam_utils.egg-info/
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2406 2023-06-14 02:49:00.000000 sinyi_datateam_utils-0.1.6/sinyi_datateam_utils.egg-info/PKG-INFO
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)      316 2023-06-14 02:49:00.000000 sinyi_datateam_utils-0.1.6/sinyi_datateam_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        1 2023-06-14 02:49:00.000000 sinyi_datateam_utils-0.1.6/sinyi_datateam_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       83 2023-06-14 02:49:00.000000 sinyi_datateam_utils-0.1.6/sinyi_datateam_utils.egg-info/requires.txt
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       12 2023-06-14 02:49:00.000000 sinyi_datateam_utils-0.1.6/sinyi_datateam_utils.egg-info/top_level.txt
-drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-06-14 02:49:00.841084 sinyi_datateam_utils-0.1.6/sinyi_utils/
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2022-12-06 02:44:18.000000 sinyi_datateam_utils-0.1.6/sinyi_utils/__init__.py
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2634 2022-12-16 02:49:49.000000 sinyi_datateam_utils-0.1.6/sinyi_utils/db_connector.py
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     3732 2023-06-14 02:48:39.000000 sinyi_datateam_utils-0.1.6/sinyi_utils/format_tool.py
+drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-06-14 03:04:43.316691 sinyi_datateam_utils-0.1.7/
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2406 2023-06-14 03:04:43.316691 sinyi_datateam_utils-0.1.7/PKG-INFO
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2180 2022-12-16 02:49:49.000000 sinyi_datateam_utils-0.1.7/README.md
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       38 2023-06-14 03:04:43.316691 sinyi_datateam_utils-0.1.7/setup.cfg
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)      646 2023-06-14 03:04:12.000000 sinyi_datateam_utils-0.1.7/setup.py
+drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-06-14 03:04:43.312691 sinyi_datateam_utils-0.1.7/sinyi_datateam_utils.egg-info/
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2406 2023-06-14 03:04:43.000000 sinyi_datateam_utils-0.1.7/sinyi_datateam_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)      316 2023-06-14 03:04:43.000000 sinyi_datateam_utils-0.1.7/sinyi_datateam_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        1 2023-06-14 03:04:43.000000 sinyi_datateam_utils-0.1.7/sinyi_datateam_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       83 2023-06-14 03:04:43.000000 sinyi_datateam_utils-0.1.7/sinyi_datateam_utils.egg-info/requires.txt
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       12 2023-06-14 03:04:43.000000 sinyi_datateam_utils-0.1.7/sinyi_datateam_utils.egg-info/top_level.txt
+drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-06-14 03:04:43.316691 sinyi_datateam_utils-0.1.7/sinyi_utils/
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2022-12-06 02:44:18.000000 sinyi_datateam_utils-0.1.7/sinyi_utils/__init__.py
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2634 2022-12-16 02:49:49.000000 sinyi_datateam_utils-0.1.7/sinyi_utils/db_connector.py
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     3769 2023-06-14 03:02:54.000000 sinyi_datateam_utils-0.1.7/sinyi_utils/format_tool.py
```

### Comparing `sinyi_datateam_utils-0.1.6/PKG-INFO` & `sinyi_datateam_utils-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinyi_datateam_utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: Utilities for data analysis
 Home-page: https://SinyiDataTeam@dev.azure.com/SinyiDataTeam/Label360/_git/sinyi_utils
 Author: sinyidatateam
 Author-email: me30@sinyi.com.tw
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `sinyi_datateam_utils-0.1.6/README.md` & `sinyi_datateam_utils-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `sinyi_datateam_utils-0.1.6/setup.py` & `sinyi_datateam_utils-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
   
 with open("README.md", "r") as fh:
     description = fh.read()
   
 setuptools.setup(
     name="sinyi_datateam_utils",
-    version="0.1.6",
+    version="0.1.7",
     author="sinyidatateam",
     author_email="me30@sinyi.com.tw",
     packages=["sinyi_utils"],
     description="Utilities for data analysis",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://SinyiDataTeam@dev.azure.com/SinyiDataTeam/Label360/_git/sinyi_utils",
```

### Comparing `sinyi_datateam_utils-0.1.6/sinyi_datateam_utils.egg-info/PKG-INFO` & `sinyi_datateam_utils-0.1.7/sinyi_datateam_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinyi-datateam-utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: Utilities for data analysis
 Home-page: https://SinyiDataTeam@dev.azure.com/SinyiDataTeam/Label360/_git/sinyi_utils
 Author: sinyidatateam
 Author-email: me30@sinyi.com.tw
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `sinyi_datateam_utils-0.1.6/sinyi_utils/db_connector.py` & `sinyi_datateam_utils-0.1.7/sinyi_utils/db_connector.py`

 * *Files identical despite different names*

### Comparing `sinyi_datateam_utils-0.1.6/sinyi_utils/format_tool.py` & `sinyi_datateam_utils-0.1.7/sinyi_utils/format_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from pathlib import Path
+from databricks.sdk.runtime import *
 import sqlalchemy
 from sqlalchemy.engine import URL
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad
 import base64
 import requests
```

