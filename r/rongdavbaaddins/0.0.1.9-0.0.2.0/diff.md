# Comparing `tmp/rongdavbaaddins-0.0.1.9.tar.gz` & `tmp/rongdavbaaddins-0.0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rongdavbaaddins-0.0.1.9.tar", last modified: Tue Jun 13 01:27:37 2023, max compression
+gzip compressed data, was "rongdavbaaddins-0.0.2.0.tar", last modified: Wed Jun 14 01:33:02 2023, max compression
```

## Comparing `rongdavbaaddins-0.0.1.9.tar` & `rongdavbaaddins-0.0.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 01:27:37.564292 rongdavbaaddins-0.0.1.9/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.1.9/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0      409 2023-06-13 01:27:37.565292 rongdavbaaddins-0.0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 01:27:37.548295 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/
--rw-rw-rw-   0        0        0    15227 2023-06-02 06:14:22.000000 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/Excel.officeUI
-drwxrwxrwx   0        0        0        0 2023-06-13 01:27:37.552291 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/Function/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/Function/__init__.py
--rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/Function/minusFunction.pyd
--rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/Function/minusFunctionpy.py
--rw-rw-rw-   0        0        0   111558 2023-06-13 01:27:20.000000 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/RDaddins.xlam
-drwxrwxrwx   0        0        0        0 2023-06-13 01:27:37.555290 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/Ui/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/Ui/__init__.py
--rw-rw-rw-   0        0        0     3281 2023-06-07 05:42:04.000000 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py
--rw-rw-rw-   0        0        0    54784 2023-05-31 09:26:30.000000 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/Vbalog.pyd
--rw-rw-rw-   0        0        0     1000 2023-06-08 09:19:01.000000 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/Vbalogpy.py
--rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/__init__.py
--rw-rw-rw-   0        0        0    48640 2023-06-08 01:57:00.000000 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/getNumber.pyd
--rw-rw-rw-   0        0        0      448 2023-06-09 06:42:10.000000 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/getNumberpy.py
--rw-rw-rw-   0        0        0    41984 2023-06-08 01:39:24.000000 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/minusFunction.pyd
--rw-rw-rw-   0        0        0   141312 2023-06-13 01:24:29.000000 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/rongdavbaaddins.pyd
--rw-rw-rw-   0        0        0    66560 2023-06-09 03:08:54.000000 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/vbaLogin.pyd
--rw-rw-rw-   0        0        0      289 2023-06-08 07:23:23.000000 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/vbaloginpy.py
--rw-rw-rw-   0        0        0    27954 2023-06-13 01:27:19.000000 rongdavbaaddins-0.0.1.9/rongdaVbaAddins/文件处理类模板.xlsx
-drwxrwxrwx   0        0        0        0 2023-06-13 01:27:37.563292 rongdavbaaddins-0.0.1.9/rongdavbaaddins.egg-info/
--rw-rw-rw-   0        0        0      409 2023-06-13 01:27:37.000000 rongdavbaaddins-0.0.1.9/rongdavbaaddins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      780 2023-06-13 01:27:37.000000 rongdavbaaddins-0.0.1.9/rongdavbaaddins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 01:27:37.000000 rongdavbaaddins-0.0.1.9/rongdavbaaddins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-13 01:27:37.000000 rongdavbaaddins-0.0.1.9/rongdavbaaddins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-06-13 01:27:37.566293 rongdavbaaddins-0.0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1024 2023-06-13 01:23:37.000000 rongdavbaaddins-0.0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:33:02.316204 rongdavbaaddins-0.0.2.0/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      417 2023-06-14 01:33:02.317204 rongdavbaaddins-0.0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 01:33:02.185196 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/
+-rw-rw-rw-   0        0        0    15227 2023-06-02 06:14:22.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Excel.officeUI
+drwxrwxrwx   0        0        0        0 2023-06-14 01:33:02.223196 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Function/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Function/__init__.py
+-rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Function/minusFunction.pyd
+-rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Function/minusFunctionpy.py
+-rw-rw-rw-   0        0        0   111558 2023-06-13 01:27:20.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/RDaddins.xlam
+drwxrwxrwx   0        0        0        0 2023-06-14 01:33:02.244204 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Ui/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Ui/__init__.py
+-rw-rw-rw-   0        0        0     3281 2023-06-07 05:42:04.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py
+-rw-rw-rw-   0        0        0    54784 2023-05-31 09:26:30.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Vbalog.pyd
+-rw-rw-rw-   0        0        0     1000 2023-06-08 09:19:01.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Vbalogpy.py
+-rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/__init__.py
+-rw-rw-rw-   0        0        0    48640 2023-06-08 01:57:00.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/getNumber.pyd
+-rw-rw-rw-   0        0        0      448 2023-06-09 06:42:10.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/getNumberpy.py
+-rw-rw-rw-   0        0        0    41984 2023-06-08 01:39:24.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/minusFunction.pyd
+-rw-rw-rw-   0        0        0   141312 2023-06-14 01:32:05.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/rongdavbaaddins.pyd
+-rw-rw-rw-   0        0        0    66560 2023-06-09 03:08:54.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/vbaLogin.pyd
+-rw-rw-rw-   0        0        0      289 2023-06-08 07:23:23.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/vbaloginpy.py
+-rw-rw-rw-   0        0        0    27954 2023-06-13 01:27:19.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/文件处理类模板.xlsx
+drwxrwxrwx   0        0        0        0 2023-06-14 01:33:02.304206 rongdavbaaddins-0.0.2.0/rongdavbaaddins.egg-info/
+-rw-rw-rw-   0        0        0      417 2023-06-14 01:33:01.000000 rongdavbaaddins-0.0.2.0/rongdavbaaddins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2023-06-14 01:33:01.000000 rongdavbaaddins-0.0.2.0/rongdavbaaddins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 01:33:01.000000 rongdavbaaddins-0.0.2.0/rongdavbaaddins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-14 01:33:01.000000 rongdavbaaddins-0.0.2.0/rongdavbaaddins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-06-14 01:33:02.322204 rongdavbaaddins-0.0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2023-06-14 01:32:33.000000 rongdavbaaddins-0.0.2.0/setup.py
```

### Comparing `rongdavbaaddins-0.0.1.9/LICENSE.txt` & `rongdavbaaddins-0.0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.9/rongdaVbaAddins/Excel.officeUI` & `rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Excel.officeUI`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.9/rongdaVbaAddins/RDaddins.xlam` & `rongdavbaaddins-0.0.2.0/rongdaVbaAddins/RDaddins.xlam`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.9/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py` & `rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.9/rongdaVbaAddins/Vbalogpy.py` & `rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Vbalogpy.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.9/rongdaVbaAddins/文件处理类模板.xlsx` & `rongdavbaaddins-0.0.2.0/rongdaVbaAddins/文件处理类模板.xlsx`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.9/rongdavbaaddins.egg-info/SOURCES.txt` & `rongdavbaaddins-0.0.2.0/rongdavbaaddins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.9/setup.py` & `rongdavbaaddins-0.0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 0
-PATCH = 1
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}.9"
+PATCH = 2
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.0"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "rongdavbaaddins",
     version=VERSION,
-    author="wangweidong",
+    author="qiuxing,wangweidong",
     author_email="17891967090@163.com",
     description='荣大工具箱-Excel插件',
     long_description_content_type="text/markdown",
     url='https://alidocs.dingtalk.com/i/p/4oJRz0VRJyvmLZMydy0mV7WvjQn7MG89',
     long_description=open('README.md', encoding="utf-8").read(),
     python_requires=">=3.8",
     install_requires=get_install_requires(),
```

