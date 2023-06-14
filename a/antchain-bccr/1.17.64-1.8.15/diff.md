# Comparing `tmp/antchain_bccr-1.17.64.tar.gz` & `tmp/antchain_bccr-1.8.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_bccr-1.17.64.tar", last modified: Wed Jun 14 09:28:54 2023, max compression
+gzip compressed data, was "dist/antchain_bccr-1.8.15.tar", last modified: Tue Mar 30 13:32:25 2021, max compression
```

## Comparing `antchain_bccr-1.17.64.tar` & `antchain_bccr-1.8.15.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:28:54.000000 antchain_bccr-1.17.64/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-14 09:28:53.000000 antchain_bccr-1.17.64/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-14 09:28:53.000000 antchain_bccr-1.17.64/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2170 2023-06-14 09:28:54.000000 antchain_bccr-1.17.64/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-06-14 09:28:53.000000 antchain_bccr-1.17.64/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-14 09:28:53.000000 antchain_bccr-1.17.64/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:28:54.000000 antchain_bccr-1.17.64/antchain_bccr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2170 2023-06-14 09:28:54.000000 antchain_bccr-1.17.64/antchain_bccr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-06-14 09:28:54.000000 antchain_bccr-1.17.64/antchain_bccr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 09:28:54.000000 antchain_bccr-1.17.64/antchain_bccr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-14 09:28:54.000000 antchain_bccr-1.17.64/antchain_bccr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-14 09:28:54.000000 antchain_bccr-1.17.64/antchain_bccr.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:28:54.000000 antchain_bccr-1.17.64/antchain_sdk_bccr/
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-14 09:28:53.000000 antchain_bccr-1.17.64/antchain_sdk_bccr/__init__.py
--rw-r--r--   0 root         (0) root         (0)   145389 2023-06-14 09:28:53.000000 antchain_bccr-1.17.64/antchain_sdk_bccr/client.py
--rw-r--r--   0 root         (0) root         (0)   503395 2023-06-14 09:28:53.000000 antchain_bccr-1.17.64/antchain_sdk_bccr/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-14 09:28:54.000000 antchain_bccr-1.17.64/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2023-06-14 09:28:53.000000 antchain_bccr-1.17.64/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-30 13:32:25.000000 antchain_bccr-1.8.15/
+-rw-r--r--   0 root         (0) root         (0)      600 2021-03-30 13:32:24.000000 antchain_bccr-1.8.15/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2021-03-30 13:32:24.000000 antchain_bccr-1.8.15/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2177 2021-03-30 13:32:25.000000 antchain_bccr-1.8.15/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      815 2021-03-30 13:32:24.000000 antchain_bccr-1.8.15/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1001 2021-03-30 13:32:24.000000 antchain_bccr-1.8.15/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-30 13:32:25.000000 antchain_bccr-1.8.15/antchain_bccr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2177 2021-03-30 13:32:24.000000 antchain_bccr-1.8.15/antchain_bccr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2021-03-30 13:32:24.000000 antchain_bccr-1.8.15/antchain_bccr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-03-30 13:32:24.000000 antchain_bccr-1.8.15/antchain_bccr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2021-03-30 13:32:24.000000 antchain_bccr-1.8.15/antchain_bccr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2021-03-30 13:32:24.000000 antchain_bccr-1.8.15/antchain_bccr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-30 13:32:25.000000 antchain_bccr-1.8.15/antchain_sdk_bccr/
+-rw-r--r--   0 root         (0) root         (0)       22 2021-03-30 13:32:24.000000 antchain_bccr-1.8.15/antchain_sdk_bccr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54981 2021-03-30 13:32:24.000000 antchain_bccr-1.8.15/antchain_sdk_bccr/client.py
+-rw-r--r--   0 root         (0) root         (0)   147122 2021-03-30 13:32:24.000000 antchain_bccr-1.8.15/antchain_sdk_bccr/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2021-03-30 13:32:25.000000 antchain_bccr-1.8.15/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2493 2021-03-30 13:32:24.000000 antchain_bccr-1.8.15/setup.py
```

### Comparing `antchain_bccr-1.17.64/LICENSE` & `antchain_bccr-1.8.15/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_bccr-1.17.64/PKG-INFO` & `antchain_bccr-1.8.15/antchain_bccr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_bccr
-Version: 1.17.64
+Name: antchain-bccr
+Version: 1.8.15
 Summary: Ant Chain BCCR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain-bccr
-        pip install antchain-bccr
+        # Install the antchain_sdk_bccr
+        pip install antchain_sdk_bccr
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_bccr-1.17.64/README-CN.md` & `antchain_bccr-1.8.15/README-CN.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## 安装
 
 - **使用 pip 安装(推荐)**
 
 如未安装 `pip`, 请先至pip官网 [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") 安装pip .
 
 ```bash
-# 安装 antchain-bccr
-pip install antchain-bccr
+# 安装 antchain_sdk_bccr
+pip install antchain_sdk_bccr
 ```
 
 ## 问题
 
 [提交 Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new)，不符合指南的问题可能会立即关闭。
 
 ## 使用说明
```

### Comparing `antchain_bccr-1.17.64/README.md` & `antchain_bccr-1.8.15/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## Installation
 
 - **Install with pip**
 
 Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
 
 ```bash
-# Install the antchain-bccr
-pip install antchain-bccr
+# Install the antchain_sdk_bccr
+pip install antchain_sdk_bccr
 ```
 
 ## Issues
 
 [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
 
 ## Usage
```

### Comparing `antchain_bccr-1.17.64/antchain_bccr.egg-info/PKG-INFO` & `antchain_bccr-1.8.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-bccr
-Version: 1.17.64
+Name: antchain_bccr
+Version: 1.8.15
 Summary: Ant Chain BCCR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain-bccr
-        pip install antchain-bccr
+        # Install the antchain_sdk_bccr
+        pip install antchain_sdk_bccr
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_bccr-1.17.64/setup.py` & `antchain_bccr-1.8.15/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_bccr.
 
-Created on 14/06/2023
+Created on 30/03/2021
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_bccr"
 NAME = "antchain_bccr" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain BCCR SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
-    "alibabacloud_rpc_util>=0.0.4, <1.0.0"
+    "antchain_alipay_util>=1.0.0, <2.0.0",
+    "alibabacloud_tea_util>=0.3.3, <1.0.0",
+    "alibabacloud_rpc_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

