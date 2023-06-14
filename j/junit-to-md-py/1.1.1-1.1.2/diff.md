# Comparing `tmp/junit-to-md-py-1.1.1.tar.gz` & `tmp/junit-to-md-py-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junit-to-md-py-1.1.1.tar", last modified: Tue Jun 13 12:43:16 2023, max compression
+gzip compressed data, was "junit-to-md-py-1.1.2.tar", last modified: Wed Jun 14 09:45:49 2023, max compression
```

## Comparing `junit-to-md-py-1.1.1.tar` & `junit-to-md-py-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 12:43:16.726388 junit-to-md-py-1.1.1/
--rw-rw-rw-   0        0        0      554 2023-06-13 12:43:16.725388 junit-to-md-py-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-06-09 11:48:23.000000 junit-to-md-py-1.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-13 12:43:16.716406 junit-to-md-py-1.1.1/junit_to_md_py.egg-info/
--rw-rw-rw-   0        0        0      554 2023-06-13 12:43:16.000000 junit-to-md-py-1.1.1/junit_to_md_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-06-13 12:43:16.000000 junit-to-md-py-1.1.1/junit_to_md_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 12:43:16.000000 junit-to-md-py-1.1.1/junit_to_md_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-13 12:43:16.000000 junit-to-md-py-1.1.1/junit_to_md_py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2023-06-13 12:43:16.000000 junit-to-md-py-1.1.1/junit_to_md_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-13 12:43:16.000000 junit-to-md-py-1.1.1/junit_to_md_py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 12:43:16.722389 junit-to-md-py-1.1.1/script/
--rw-rw-rw-   0        0        0        0 2023-06-09 11:39:01.000000 junit-to-md-py-1.1.1/script/__init__.py
--rw-rw-rw-   0        0        0     1267 2023-06-09 11:45:28.000000 junit-to-md-py-1.1.1/script/junit_to_md.py
--rw-rw-rw-   0        0        0       42 2023-06-13 12:43:16.726388 junit-to-md-py-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      642 2023-06-13 12:42:48.000000 junit-to-md-py-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:45:49.168610 junit-to-md-py-1.1.2/
+-rw-rw-rw-   0        0        0      554 2023-06-14 09:45:49.167611 junit-to-md-py-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-06-09 11:48:23.000000 junit-to-md-py-1.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-14 09:45:49.158608 junit-to-md-py-1.1.2/junit_to_md_py.egg-info/
+-rw-rw-rw-   0        0        0      554 2023-06-14 09:45:48.000000 junit-to-md-py-1.1.2/junit_to_md_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-06-14 09:45:48.000000 junit-to-md-py-1.1.2/junit_to_md_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 09:45:48.000000 junit-to-md-py-1.1.2/junit_to_md_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-14 09:45:48.000000 junit-to-md-py-1.1.2/junit_to_md_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2023-06-14 09:45:48.000000 junit-to-md-py-1.1.2/junit_to_md_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-14 09:45:48.000000 junit-to-md-py-1.1.2/junit_to_md_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 09:45:49.164610 junit-to-md-py-1.1.2/script/
+-rw-rw-rw-   0        0        0        0 2023-06-09 11:39:01.000000 junit-to-md-py-1.1.2/script/__init__.py
+-rw-rw-rw-   0        0        0     1871 2023-06-14 09:45:17.000000 junit-to-md-py-1.1.2/script/junit_to_md.py
+-rw-rw-rw-   0        0        0       42 2023-06-14 09:45:49.169610 junit-to-md-py-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      642 2023-06-14 09:45:32.000000 junit-to-md-py-1.1.2/setup.py
```

### Comparing `junit-to-md-py-1.1.1/PKG-INFO` & `junit-to-md-py-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junit-to-md-py
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python script which converts junit xml file/text into the markdown representation
 Home-page: https://github.com/catalogicsoftware/dpx-utils-junit-to-md
 Author: srydz_catalogicsoftware
 Author-email: srydz@catalogicsoftware.com
 License: MIT
 
 Python script which converts junit xml file/text into the markdown representation
```

### Comparing `junit-to-md-py-1.1.1/junit_to_md_py.egg-info/PKG-INFO` & `junit-to-md-py-1.1.2/junit_to_md_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junit-to-md-py
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python script which converts junit xml file/text into the markdown representation
 Home-page: https://github.com/catalogicsoftware/dpx-utils-junit-to-md
 Author: srydz_catalogicsoftware
 Author-email: srydz@catalogicsoftware.com
 License: MIT
 
 Python script which converts junit xml file/text into the markdown representation
```

### Comparing `junit-to-md-py-1.1.1/setup.py` & `junit-to-md-py-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="junit-to-md-py",
-    version="1.1.1",
+    version="1.1.2",
     author="srydz_catalogicsoftware",
     author_email="srydz@catalogicsoftware.com",
     description="Python script which converts junit xml file/text into the markdown representation",
     long_description=open("README.rst", encoding="utf-8").read(),
     url="https://github.com/catalogicsoftware/dpx-utils-junit-to-md",
     license="MIT",
     packages=["script"],
```

