# Comparing `tmp/xython-1.1.0.tar.gz` & `tmp/xython-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xython-1.1.0.tar", last modified: Wed Jun 14 13:11:45 2023, max compression
+gzip compressed data, was "xython-1.2.0.tar", last modified: Wed Jun 14 13:35:12 2023, max compression
```

## Comparing `xython-1.1.0.tar` & `xython-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 13:11:45.753354 xython-1.1.0/
--rw-rw-rw-   0        0        0      388 2023-06-05 14:30:55.000000 xython-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     9251 2023-06-14 13:11:45.754353 xython-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     8722 2023-06-05 14:30:55.000000 xython-1.1.0/README.md
--rw-rw-rw-   0        0        0        0 2021-06-11 06:00:16.000000 xython-1.1.0/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-06-14 13:11:45.757353 xython-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      898 2023-06-14 13:10:09.000000 xython-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:11:45.677337 xython-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-14 13:11:45.727146 xython-1.1.0/src/xython/
--rw-rw-rw-   0        0        0      472 2023-06-14 13:06:35.000000 xython-1.1.0/src/xython/__init__.py
--rw-rw-rw-   0        0        0    23159 2023-05-14 09:19:38.000000 xython-1.1.0/src/xython/anydb.py
--rw-rw-rw-   0        0        0    80419 2023-06-03 06:07:50.000000 xython-1.1.0/src/xython/basic_data.py
--rw-rw-rw-   0        0        0    24552 2023-05-23 21:32:30.000000 xython-1.1.0/src/xython/ganada.py
--rw-rw-rw-   0        0        0    19604 2023-05-22 13:41:17.000000 xython-1.1.0/src/xython/jfinder.py
--rw-rw-rw-   0        0        0    24532 2023-05-23 21:32:30.000000 xython-1.1.0/src/xython/mailmail.py
--rw-rw-rw-   0        0        0   141238 2023-06-04 07:04:32.000000 xython-1.1.0/src/xython/pcell.py
--rw-rw-rw-   0        0        0     5736 2023-04-08 04:25:55.000000 xython-1.1.0/src/xython/pcell_event.py
--rw-rw-rw-   0        0        0    11415 2023-05-22 13:34:23.000000 xython-1.1.0/src/xython/pyclick.py
--rw-rw-rw-   0        0        0    36331 2023-05-23 20:51:47.000000 xython-1.1.0/src/xython/pynal.py
--rw-rw-rw-   0        0        0    34869 2023-05-29 02:11:51.000000 xython-1.1.0/src/xython/scolor.py
--rw-rw-rw-   0        0        0    52683 2023-06-04 07:06:03.000000 xython-1.1.0/src/xython/youtil.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:11:45.751360 xython-1.1.0/src/xython.egg-info/
--rw-rw-rw-   0        0        0     9251 2023-06-14 13:11:45.000000 xython-1.1.0/src/xython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-06-14 13:11:45.000000 xython-1.1.0/src/xython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 13:11:45.000000 xython-1.1.0/src/xython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-05 14:32:10.000000 xython-1.1.0/src/xython.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-14 13:11:45.000000 xython-1.1.0/src/xython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 13:35:12.245499 xython-1.2.0/
+-rw-rw-rw-   0        0        0      388 2023-06-05 14:30:55.000000 xython-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9251 2023-06-14 13:35:12.245499 xython-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8722 2023-06-05 14:30:55.000000 xython-1.2.0/README.md
+-rw-rw-rw-   0        0        0        0 2021-06-11 06:00:16.000000 xython-1.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-06-14 13:35:12.247299 xython-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      898 2023-06-14 13:33:39.000000 xython-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:35:12.177517 xython-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 13:35:12.223301 xython-1.2.0/src/xython/
+-rw-rw-rw-   0        0        0      467 2023-06-14 13:32:51.000000 xython-1.2.0/src/xython/__init__.py
+-rw-rw-rw-   0        0        0    23159 2023-05-14 09:19:38.000000 xython-1.2.0/src/xython/anydb.py
+-rw-rw-rw-   0        0        0    80419 2023-06-03 06:07:50.000000 xython-1.2.0/src/xython/basic_data.py
+-rw-rw-rw-   0        0        0    24552 2023-05-23 21:32:30.000000 xython-1.2.0/src/xython/ganada.py
+-rw-rw-rw-   0        0        0    19604 2023-05-22 13:41:17.000000 xython-1.2.0/src/xython/jfinder.py
+-rw-rw-rw-   0        0        0    24532 2023-05-23 21:32:30.000000 xython-1.2.0/src/xython/mailmail.py
+-rw-rw-rw-   0        0        0   141238 2023-06-04 07:04:32.000000 xython-1.2.0/src/xython/pcell.py
+-rw-rw-rw-   0        0        0     5736 2023-04-08 04:25:55.000000 xython-1.2.0/src/xython/pcell_event.py
+-rw-rw-rw-   0        0        0    11415 2023-05-22 13:34:23.000000 xython-1.2.0/src/xython/pyclick.py
+-rw-rw-rw-   0        0        0    36331 2023-05-23 20:51:47.000000 xython-1.2.0/src/xython/pynal.py
+-rw-rw-rw-   0        0        0    34869 2023-05-29 02:11:51.000000 xython-1.2.0/src/xython/scolor.py
+-rw-rw-rw-   0        0        0    52683 2023-06-04 07:06:03.000000 xython-1.2.0/src/xython/youtil.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:35:12.243302 xython-1.2.0/src/xython.egg-info/
+-rw-rw-rw-   0        0        0     9251 2023-06-14 13:35:11.000000 xython-1.2.0/src/xython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-06-14 13:35:12.000000 xython-1.2.0/src/xython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 13:35:12.000000 xython-1.2.0/src/xython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-05 14:32:10.000000 xython-1.2.0/src/xython.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-14 13:35:12.000000 xython-1.2.0/src/xython.egg-info/top_level.txt
```

### Comparing `xython-1.1.0/PKG-INFO` & `xython-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: xython
-Version: 1.1.0
+Version: 1.2.0
 Summary: Easy Read / Write for Excel, Word, Color, Etc using Python
 Home-page: https://github.com/sjpark/xython
-Download-URL: https://github.com/sjpark/xython/archive/v1.1.0.tar.gz
+Download-URL: https://github.com/sjpark/xython/archive/v1.2.0.tar.gz
 Author: sjpark
 Author-email: sjpkorea@yahoo.com
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 ## xython 모듈에 대하여
```

### Comparing `xython-1.1.0/README.md` & `xython-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `xython-1.1.0/setup.py` & `xython-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 #with open("README.md", "rt", encoding='UTF8') as fh:
 #    long_description = fh.read()
 setup(
     name='xython',
-    version='1.1.0',
+    version='1.2.0',
     url='https://github.com/sjpark/xython',
-    download_url='https://github.com/sjpark/xython/archive/v1.1.0.tar.gz',
+    download_url='https://github.com/sjpark/xython/archive/v1.2.0.tar.gz',
     author='sjpark',
     author_email='sjpkorea@yahoo.com',
     description='Easy Read / Write for Excel, Word, Color, Etc using Python',
     packages=find_packages("src"),
     package_dir={"": "src"},
     include_package_data=True,
     package_data={
```

### Comparing `xython-1.1.0/src/xython/anydb.py` & `xython-1.2.0/src/xython/anydb.py`

 * *Files identical despite different names*

### Comparing `xython-1.1.0/src/xython/basic_data.py` & `xython-1.2.0/src/xython/basic_data.py`

 * *Files identical despite different names*

### Comparing `xython-1.1.0/src/xython/ganada.py` & `xython-1.2.0/src/xython/ganada.py`

 * *Files identical despite different names*

### Comparing `xython-1.1.0/src/xython/jfinder.py` & `xython-1.2.0/src/xython/jfinder.py`

 * *Files identical despite different names*

### Comparing `xython-1.1.0/src/xython/mailmail.py` & `xython-1.2.0/src/xython/mailmail.py`

 * *Files identical despite different names*

### Comparing `xython-1.1.0/src/xython/pcell.py` & `xython-1.2.0/src/xython/pcell.py`

 * *Files identical despite different names*

### Comparing `xython-1.1.0/src/xython/pcell_event.py` & `xython-1.2.0/src/xython/pcell_event.py`

 * *Files identical despite different names*

### Comparing `xython-1.1.0/src/xython/pyclick.py` & `xython-1.2.0/src/xython/pyclick.py`

 * *Files identical despite different names*

### Comparing `xython-1.1.0/src/xython/pynal.py` & `xython-1.2.0/src/xython/pynal.py`

 * *Files identical despite different names*

### Comparing `xython-1.1.0/src/xython/scolor.py` & `xython-1.2.0/src/xython/scolor.py`

 * *Files identical despite different names*

### Comparing `xython-1.1.0/src/xython/youtil.py` & `xython-1.2.0/src/xython/youtil.py`

 * *Files identical despite different names*

### Comparing `xython-1.1.0/src/xython.egg-info/PKG-INFO` & `xython-1.2.0/src/xython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: xython
-Version: 1.1.0
+Version: 1.2.0
 Summary: Easy Read / Write for Excel, Word, Color, Etc using Python
 Home-page: https://github.com/sjpark/xython
-Download-URL: https://github.com/sjpark/xython/archive/v1.1.0.tar.gz
+Download-URL: https://github.com/sjpark/xython/archive/v1.2.0.tar.gz
 Author: sjpark
 Author-email: sjpkorea@yahoo.com
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 ## xython 모듈에 대하여
```

