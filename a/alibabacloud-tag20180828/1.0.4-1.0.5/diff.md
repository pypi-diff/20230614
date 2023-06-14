# Comparing `tmp/alibabacloud_tag20180828-1.0.4.tar.gz` & `tmp/alibabacloud_tag20180828-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_tag20180828-1.0.4.tar", last modified: Wed Jul  6 07:03:27 2022, max compression
+gzip compressed data, was "dist/alibabacloud_tag20180828-1.0.5.tar", last modified: Wed Jun 14 02:36:38 2023, max compression
```

## Comparing `alibabacloud_tag20180828-1.0.4.tar` & `alibabacloud_tag20180828-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-06 07:03:27.000000 alibabacloud_tag20180828-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      259 2022-07-06 07:03:26.000000 alibabacloud_tag20180828-1.0.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-07-06 07:03:26.000000 alibabacloud_tag20180828-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-07-06 07:03:26.000000 alibabacloud_tag20180828-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2328 2022-07-06 07:03:27.000000 alibabacloud_tag20180828-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2022-07-06 07:03:26.000000 alibabacloud_tag20180828-1.0.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2022-07-06 07:03:26.000000 alibabacloud_tag20180828-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-06 07:03:27.000000 alibabacloud_tag20180828-1.0.4/alibabacloud_tag20180828/
--rw-r--r--   0 root         (0) root         (0)       21 2022-07-06 07:03:26.000000 alibabacloud_tag20180828-1.0.4/alibabacloud_tag20180828/__init__.py
--rw-r--r--   0 root         (0) root         (0)   109416 2022-07-06 07:03:26.000000 alibabacloud_tag20180828-1.0.4/alibabacloud_tag20180828/client.py
--rw-r--r--   0 root         (0) root         (0)   158930 2022-07-06 07:03:26.000000 alibabacloud_tag20180828-1.0.4/alibabacloud_tag20180828/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-06 07:03:27.000000 alibabacloud_tag20180828-1.0.4/alibabacloud_tag20180828.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2328 2022-07-06 07:03:26.000000 alibabacloud_tag20180828-1.0.4/alibabacloud_tag20180828.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2022-07-06 07:03:26.000000 alibabacloud_tag20180828-1.0.4/alibabacloud_tag20180828.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-06 07:03:26.000000 alibabacloud_tag20180828-1.0.4/alibabacloud_tag20180828.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-07-06 07:03:26.000000 alibabacloud_tag20180828-1.0.4/alibabacloud_tag20180828.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-07-06 07:03:26.000000 alibabacloud_tag20180828-1.0.4/alibabacloud_tag20180828.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-07-06 07:03:27.000000 alibabacloud_tag20180828-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2610 2022-07-06 07:03:26.000000 alibabacloud_tag20180828-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:36:38.000000 alibabacloud_tag20180828-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      311 2023-06-14 02:36:37.000000 alibabacloud_tag20180828-1.0.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-14 02:36:37.000000 alibabacloud_tag20180828-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-14 02:36:37.000000 alibabacloud_tag20180828-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-06-14 02:36:38.000000 alibabacloud_tag20180828-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-06-14 02:36:37.000000 alibabacloud_tag20180828-1.0.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-06-14 02:36:37.000000 alibabacloud_tag20180828-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:36:38.000000 alibabacloud_tag20180828-1.0.5/alibabacloud_tag20180828/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-14 02:36:37.000000 alibabacloud_tag20180828-1.0.5/alibabacloud_tag20180828/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   176408 2023-06-14 02:36:37.000000 alibabacloud_tag20180828-1.0.5/alibabacloud_tag20180828/client.py
+-rw-r--r--   0 root         (0) root         (0)   204022 2023-06-14 02:36:37.000000 alibabacloud_tag20180828-1.0.5/alibabacloud_tag20180828/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:36:38.000000 alibabacloud_tag20180828-1.0.5/alibabacloud_tag20180828.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-06-14 02:36:37.000000 alibabacloud_tag20180828-1.0.5/alibabacloud_tag20180828.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-14 02:36:38.000000 alibabacloud_tag20180828-1.0.5/alibabacloud_tag20180828.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 02:36:37.000000 alibabacloud_tag20180828-1.0.5/alibabacloud_tag20180828.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-14 02:36:37.000000 alibabacloud_tag20180828-1.0.5/alibabacloud_tag20180828.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-14 02:36:37.000000 alibabacloud_tag20180828-1.0.5/alibabacloud_tag20180828.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-14 02:36:38.000000 alibabacloud_tag20180828-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2610 2023-06-14 02:36:37.000000 alibabacloud_tag20180828-1.0.5/setup.py
```

### Comparing `alibabacloud_tag20180828-1.0.4/LICENSE` & `alibabacloud_tag20180828-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_tag20180828-1.0.4/PKG-INFO` & `alibabacloud_tag20180828-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_tag20180828
-Version: 1.0.4
+Version: 1.0.5
 Summary: Alibaba Cloud Tag (20180828) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_tag20180828-1.0.4/README-CN.md` & `alibabacloud_tag20180828-1.0.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_tag20180828-1.0.4/README.md` & `alibabacloud_tag20180828-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_tag20180828-1.0.4/alibabacloud_tag20180828.egg-info/PKG-INFO` & `alibabacloud_tag20180828-1.0.5/alibabacloud_tag20180828.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-tag20180828
-Version: 1.0.4
+Version: 1.0.5
 Summary: Alibaba Cloud Tag (20180828) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_tag20180828-1.0.4/setup.py` & `alibabacloud_tag20180828-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_tag20180828.
 
-Created on 06/07/2022
+Created on 14/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_tag20180828"
 NAME = "alibabacloud_tag20180828" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Tag (20180828) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

