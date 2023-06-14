# Comparing `tmp/yplib-1.0.4.tar.gz` & `tmp/yplib-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.0.4.tar", last modified: Tue Jun 13 07:01:57 2023, max compression
+gzip compressed data, was "dist\yplib-1.0.5.tar", last modified: Tue Jun 13 23:59:35 2023, max compression
```

## Comparing `yplib-1.0.4.tar` & `yplib-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 07:01:57.007032 yplib-1.0.4/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-13 07:01:57.006531 yplib-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 07:01:57.007032 yplib-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-13 07:01:39.000000 yplib-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:01:57.003615 yplib-1.0.4/yplib/
--rw-rw-rw-   0        0        0       87 2023-06-13 06:23:51.000000 yplib-1.0.4/yplib/__init__.py
--rw-rw-rw-   0        0        0     2815 2023-06-13 06:37:43.000000 yplib-1.0.4/yplib/file.py
--rw-rw-rw-   0        0        0    12648 2023-06-13 07:01:18.000000 yplib-1.0.4/yplib/index.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-1.0.4/yplib/line_stack_temp.py
--rw-rw-rw-   0        0        0     3362 2023-06-13 07:00:43.000000 yplib-1.0.4/yplib/test_my_fun.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:01:57.005924 yplib-1.0.4/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-13 07:01:56.000000 yplib-1.0.4/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-13 07:01:56.000000 yplib-1.0.4/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 07:01:56.000000 yplib-1.0.4/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 07:01:56.000000 yplib-1.0.4/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 23:59:35.819677 yplib-1.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-13 23:59:35.819228 yplib-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 23:59:35.819677 yplib-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-13 23:58:35.000000 yplib-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 23:59:35.806773 yplib-1.0.5/yplib/
+-rw-rw-rw-   0        0        0       75 2023-06-13 23:58:21.000000 yplib-1.0.5/yplib/__init__.py
+-rw-rw-rw-   0        0        0     2815 2023-06-13 06:37:43.000000 yplib-1.0.5/yplib/file.py
+-rw-rw-rw-   0        0        0    12648 2023-06-13 07:01:18.000000 yplib-1.0.5/yplib/index.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-1.0.5/yplib/line_stack_temp.py
+-rw-rw-rw-   0        0        0     3362 2023-06-13 07:05:02.000000 yplib-1.0.5/yplib/test_my_fun.py
+drwxrwxrwx   0        0        0        0 2023-06-13 23:59:35.818599 yplib-1.0.5/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-13 23:59:35.000000 yplib-1.0.5/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-13 23:59:35.000000 yplib-1.0.5/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 23:59:35.000000 yplib-1.0.5/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 23:59:35.000000 yplib-1.0.5/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.0.4/LICENSE` & `yplib-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.0.4/PKG-INFO` & `yplib-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 1.0.4
+Version: 1.0.5
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-1.0.4/setup.py` & `yplib-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.0.4",
+  version="1.0.5",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-1.0.4/yplib/file.py` & `yplib-1.0.5/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.0.4/yplib/index.py` & `yplib-1.0.5/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-1.0.4/yplib/line_stack_temp.py` & `yplib-1.0.5/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-1.0.4/yplib/test_my_fun.py` & `yplib-1.0.5/yplib/test_my_fun.py`

 * *Files identical despite different names*

### Comparing `yplib-1.0.4/yplib.egg-info/PKG-INFO` & `yplib-1.0.5/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 1.0.4
+Version: 1.0.5
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

