# Comparing `tmp/common_tool-0.0.7.tar.gz` & `tmp/common_tool-0.0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_tool-0.0.7.tar", last modified: Fri Jun  9 09:05:05 2023, max compression
+gzip compressed data, was "common_tool-0.0.7.1.tar", last modified: Tue Jun 13 07:49:00 2023, max compression
```

## Comparing `common_tool-0.0.7.tar` & `common_tool-0.0.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-09 09:05:05.844561 common_tool-0.0.7/
--rw-r--r--   0 donghao    (501) staff       (20)     1065 2022-07-13 09:33:27.000000 common_tool-0.0.7/LICENSE
--rw-r--r--   0 donghao    (501) staff       (20)      601 2023-06-09 09:05:05.844432 common_tool-0.0.7/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)      317 2022-07-13 10:19:33.000000 common_tool-0.0.7/README.md
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-09 09:05:05.843498 common_tool-0.0.7/common_tool/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2022-07-13 09:32:57.000000 common_tool-0.0.7/common_tool/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)      877 2023-06-09 09:04:39.000000 common_tool-0.0.7/common_tool/datetime.py
--rw-r--r--   0 donghao    (501) staff       (20)     3653 2023-06-05 09:13:08.000000 common_tool-0.0.7/common_tool/enum.py
--rw-r--r--   0 donghao    (501) staff       (20)     1464 2023-06-05 01:21:44.000000 common_tool-0.0.7/common_tool/http.py
--rw-r--r--   0 donghao    (501) staff       (20)      246 2023-05-19 06:58:46.000000 common_tool-0.0.7/common_tool/loggers.py
--rw-r--r--   0 donghao    (501) staff       (20)      476 2022-07-13 09:32:57.000000 common_tool-0.0.7/common_tool/math.py
--rw-r--r--   0 donghao    (501) staff       (20)     1162 2022-07-13 09:32:57.000000 common_tool-0.0.7/common_tool/random.py
--rw-r--r--   0 donghao    (501) staff       (20)      402 2022-07-13 09:32:57.000000 common_tool-0.0.7/common_tool/token.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-09 09:05:05.844016 common_tool-0.0.7/common_tool.egg-info/
--rw-r--r--   0 donghao    (501) staff       (20)      601 2023-06-09 09:05:05.000000 common_tool-0.0.7/common_tool.egg-info/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)      391 2023-06-09 09:05:05.000000 common_tool-0.0.7/common_tool.egg-info/SOURCES.txt
--rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-09 09:05:05.000000 common_tool-0.0.7/common_tool.egg-info/dependency_links.txt
--rw-r--r--   0 donghao    (501) staff       (20)       12 2023-06-09 09:05:05.000000 common_tool-0.0.7/common_tool.egg-info/requires.txt
--rw-r--r--   0 donghao    (501) staff       (20)       17 2023-06-09 09:05:05.000000 common_tool-0.0.7/common_tool.egg-info/top_level.txt
--rw-r--r--   0 donghao    (501) staff       (20)       38 2023-06-09 09:05:05.844601 common_tool-0.0.7/setup.cfg
--rw-r--r--   0 donghao    (501) staff       (20)      714 2023-06-09 09:04:39.000000 common_tool-0.0.7/setup.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-09 09:05:05.844111 common_tool-0.0.7/test/
--rw-r--r--   0 donghao    (501) staff       (20)       97 2022-07-13 10:03:42.000000 common_tool-0.0.7/test/__init__.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-13 07:49:00.451354 common_tool-0.0.7.1/
+-rw-r--r--   0 donghao    (501) staff       (20)     1065 2022-07-13 09:33:27.000000 common_tool-0.0.7.1/LICENSE
+-rw-r--r--   0 donghao    (501) staff       (20)      603 2023-06-13 07:49:00.451197 common_tool-0.0.7.1/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)      317 2022-07-13 10:19:33.000000 common_tool-0.0.7.1/README.md
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-13 07:49:00.449535 common_tool-0.0.7.1/common_tool/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2022-07-13 09:32:57.000000 common_tool-0.0.7.1/common_tool/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)      998 2023-06-13 07:48:46.000000 common_tool-0.0.7.1/common_tool/datetime.py
+-rw-r--r--   0 donghao    (501) staff       (20)     3653 2023-06-05 09:13:08.000000 common_tool-0.0.7.1/common_tool/enum.py
+-rw-r--r--   0 donghao    (501) staff       (20)     1464 2023-06-05 01:21:44.000000 common_tool-0.0.7.1/common_tool/http.py
+-rw-r--r--   0 donghao    (501) staff       (20)      246 2023-05-19 06:58:46.000000 common_tool-0.0.7.1/common_tool/loggers.py
+-rw-r--r--   0 donghao    (501) staff       (20)      476 2022-07-13 09:32:57.000000 common_tool-0.0.7.1/common_tool/math.py
+-rw-r--r--   0 donghao    (501) staff       (20)     1162 2022-07-13 09:32:57.000000 common_tool-0.0.7.1/common_tool/random.py
+-rw-r--r--   0 donghao    (501) staff       (20)      402 2022-07-13 09:32:57.000000 common_tool-0.0.7.1/common_tool/token.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-13 07:49:00.450581 common_tool-0.0.7.1/common_tool.egg-info/
+-rw-r--r--   0 donghao    (501) staff       (20)      603 2023-06-13 07:49:00.000000 common_tool-0.0.7.1/common_tool.egg-info/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)      391 2023-06-13 07:49:00.000000 common_tool-0.0.7.1/common_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-13 07:49:00.000000 common_tool-0.0.7.1/common_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       12 2023-06-13 07:49:00.000000 common_tool-0.0.7.1/common_tool.egg-info/requires.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       17 2023-06-13 07:49:00.000000 common_tool-0.0.7.1/common_tool.egg-info/top_level.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       38 2023-06-13 07:49:00.451401 common_tool-0.0.7.1/setup.cfg
+-rw-r--r--   0 donghao    (501) staff       (20)      716 2023-06-13 07:48:46.000000 common_tool-0.0.7.1/setup.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-13 07:49:00.450751 common_tool-0.0.7.1/test/
+-rw-r--r--   0 donghao    (501) staff       (20)       97 2022-07-13 10:03:42.000000 common_tool-0.0.7.1/test/__init__.py
```

### Comparing `common_tool-0.0.7/LICENSE` & `common_tool-0.0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `common_tool-0.0.7/PKG-INFO` & `common_tool-0.0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common_tool
-Version: 0.0.7
+Version: 0.0.7.1
 Summary: Basic toolkit packaging
 Home-page: https://github.com/RelaxedDong/dh_common
 Author: donghao
 Author-email: is_simple@163.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `common_tool-0.0.7/common_tool/datetime.py` & `common_tool-0.0.7.1/common_tool/datetime.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 import datetime
 
-FORMAT_DATETIME = u'%Y-%m-%d %H:%M:%S'
-FORMAT_DATE = u'%Y-%m-%d'
+FORMAT_TIME = '%H:%M:%S'
+FORMAT_DATETIME = '%Y-%m-%d %H:%M:%S'
+
+FORMAT_DATE = '%Y-%m-%d'
+FORMAT_SLASH_DATE = '%Y/%m/%d'
+FORMAT_NO_YEAR_DATE = '%m-%d'
+FORMAT_SLASH_NO_YEAR_DATE = '%m/%d'
 
 
 def datetime_to_str(date, date_format=FORMAT_DATETIME, process_none=False):
     """
     convert {@see datetime} into date string ('2011-01-12')
     """
     if process_none and date is None:
```

### Comparing `common_tool-0.0.7/common_tool/enum.py` & `common_tool-0.0.7.1/common_tool/enum.py`

 * *Files identical despite different names*

### Comparing `common_tool-0.0.7/common_tool/http.py` & `common_tool-0.0.7.1/common_tool/http.py`

 * *Files identical despite different names*

### Comparing `common_tool-0.0.7/common_tool/random.py` & `common_tool-0.0.7.1/common_tool/random.py`

 * *Files identical despite different names*

### Comparing `common_tool-0.0.7/common_tool.egg-info/PKG-INFO` & `common_tool-0.0.7.1/common_tool.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-tool
-Version: 0.0.7
+Version: 0.0.7.1
 Summary: Basic toolkit packaging
 Home-page: https://github.com/RelaxedDong/dh_common
 Author: donghao
 Author-email: is_simple@163.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `common_tool-0.0.7/setup.py` & `common_tool-0.0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = "0.0.7"
+VERSION = "0.0.7.1"
 AUTHOR = "donghao"
 AUTHOR_EMAIL = "is_simple@163.com"
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
```

