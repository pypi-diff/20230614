# Comparing `tmp/commonMethods_zhaozl_green-2.3.tar.gz` & `tmp/commonMethods_zhaozl_green-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonMethods_zhaozl_green-2.3.tar", last modified: Thu Jun  8 03:38:03 2023, max compression
+gzip compressed data, was "commonMethods_zhaozl_green-2.4.tar", last modified: Wed Jun 14 12:10:46 2023, max compression
```

## Comparing `commonMethods_zhaozl_green-2.3.tar` & `commonMethods_zhaozl_green-2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-06-08 03:38:03.815474 commonMethods_zhaozl_green-2.3/
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)     1027 2023-06-08 03:38:03.815325 commonMethods_zhaozl_green-2.3/PKG-INFO
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      359 2023-06-08 03:36:49.000000 commonMethods_zhaozl_green-2.3/README.md
-drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-06-08 03:38:03.810873 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     2605 2023-06-08 03:32:18.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/__init__.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      353 2021-03-20 02:19:04.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/__version__.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     8061 2023-05-31 12:11:20.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/core.py
-drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-06-08 03:38:03.814958 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5919 2021-04-21 06:17:46.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    10898 2021-04-16 08:39:53.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     6639 2021-04-20 02:05:23.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5354 2021-09-12 12:24:17.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     8260 2023-05-31 12:08:15.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_processBar.py
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)     2084 2023-06-08 03:30:17.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_shuffle.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     1821 2023-05-31 01:17:47.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    15542 2021-04-21 06:44:27.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     2113 2023-06-08 03:31:57.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/__init__.py
-drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-06-08 03:38:03.812195 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green.egg-info/
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)     1027 2023-06-08 03:38:03.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green.egg-info/PKG-INFO
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)      894 2023-06-08 03:38:03.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green.egg-info/SOURCES.txt
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)        1 2023-06-08 03:38:03.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green.egg-info/dependency_links.txt
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)       97 2023-06-08 03:38:03.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green.egg-info/requires.txt
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)       27 2023-06-08 03:38:03.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green.egg-info/top_level.txt
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)       38 2023-06-08 03:38:03.815528 commonMethods_zhaozl_green-2.3/setup.cfg
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     4066 2023-06-08 03:36:29.000000 commonMethods_zhaozl_green-2.3/setup.py
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-06-14 12:10:46.437094 commonMethods_zhaozl_green-2.4/
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)     1067 2023-06-14 12:10:46.436970 commonMethods_zhaozl_green-2.4/PKG-INFO
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      401 2023-06-14 12:10:13.000000 commonMethods_zhaozl_green-2.4/README.md
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-06-14 12:10:46.433918 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     2605 2023-06-08 03:32:18.000000 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/__init__.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      353 2021-03-20 02:19:04.000000 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/__version__.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     8061 2023-05-31 12:11:20.000000 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/core.py
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-06-14 12:10:46.436710 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5919 2021-04-21 06:17:46.000000 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    10898 2021-04-16 08:39:53.000000 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     6639 2021-04-20 02:05:23.000000 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5354 2021-09-12 12:24:17.000000 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     8260 2023-05-31 12:08:15.000000 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/Method_processBar.py
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)     2084 2023-06-08 03:30:17.000000 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/Method_shuffle.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     1821 2023-05-31 01:17:47.000000 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    15542 2021-04-21 06:44:27.000000 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     2113 2023-06-08 03:31:57.000000 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/__init__.py
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-06-14 12:10:46.434702 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green.egg-info/
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)     1067 2023-06-14 12:10:46.000000 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green.egg-info/PKG-INFO
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)      894 2023-06-14 12:10:46.000000 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)        1 2023-06-14 12:10:46.000000 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)       97 2023-06-14 12:10:46.000000 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green.egg-info/requires.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)       27 2023-06-14 12:10:46.000000 commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green.egg-info/top_level.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)       38 2023-06-14 12:10:46.437138 commonMethods_zhaozl_green-2.4/setup.cfg
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     4066 2023-06-14 12:09:46.000000 commonMethods_zhaozl_green-2.4/setup.py
```

### Comparing `commonMethods_zhaozl_green-2.3/PKG-INFO` & `commonMethods_zhaozl_green-2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: commonMethods_zhaozl_green
-Version: 2.3
+Version: 2.4
 Summary: timeTrans code2Name mysqlOperator printWithColor comtradeParse processBar trendAnalyzer bounceAnalyzer evennessDetermine……
 Home-page: 
 Author: zhaozl1123
 Author-email: 545362989@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 
 
 ## 版本记录
 
 v1.0 从commonMethods_zhaozl==v3.13版本中，删除bpNetWork的内容
 
@@ -25,7 +25,9 @@
 v1.2 修正了冗余代码
 
 v2.0 简化并优化了脚本，适应Python3.8
 
 v2.2 增加了几种进度条
 
 v2.3 toolbox中增加了Shuffle
+
+v2.4 降级了环境要求，Python3.7
```

### Comparing `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/__init__.py` & `commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/__init__.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/core.py` & `commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/core.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py` & `commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py` & `commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py` & `commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py` & `commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_processBar.py` & `commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/Method_processBar.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_shuffle.py` & `commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/Method_shuffle.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py` & `commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py` & `commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/__init__.py` & `commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green/toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green.egg-info/SOURCES.txt` & `commonMethods_zhaozl_green-2.4/commonMethods_zhaozl_green.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.3/setup.py` & `commonMethods_zhaozl_green-2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 
 # Package meta-data.
 NAME = 'commonMethods_zhaozl_green'
 DESCRIPTION = 'timeTrans code2Name mysqlOperator printWithColor comtradeParse processBar trendAnalyzer bounceAnalyzer evennessDetermine……'
 URL = ''
 EMAIL = '545362989@qq.com'
 AUTHOR = 'zhaozl1123'
-REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '2.3'
+REQUIRES_PYTHON = '>=3.7.0'
+VERSION = '2.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    'numpy==1.24.3', 'joblib>=0.16.0', 'pandas==1.5.3', 'matplotlib>=3.3.0', 'scikit-learn>=1.2.2', 'PyMySQL>=0.10.0'
+    'numpy>=1.19.5', 'joblib>=0.16.0', 'pandas>=1.1.5', 'matplotlib>=3.3.0', 'scikit-learn>=1.0.2', 'PyMySQL>=0.10.0'
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

