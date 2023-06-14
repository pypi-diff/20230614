# Comparing `tmp/aacommpy-0.1.8.tar.gz` & `tmp/aacommpy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aacommpy-0.1.8.tar", last modified: Mon Apr 24 13:36:17 2023, max compression
+gzip compressed data, was "aacommpy-0.1.9.tar", last modified: Mon May  1 09:53:01 2023, max compression
```

## Comparing `aacommpy-0.1.8.tar` & `aacommpy-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 13:36:17.349441 aacommpy-0.1.8/
--rw-rw-rw-   0        0        0      533 2023-04-24 13:36:17.349441 aacommpy-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       50 2023-04-24 12:46:06.000000 aacommpy-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 13:36:17.330531 aacommpy-0.1.8/aacommpy/
--rw-rw-rw-   0        0        0       95 2023-04-24 11:51:36.000000 aacommpy-0.1.8/aacommpy/__init__.py
--rw-rw-rw-   0        0        0      263 2023-04-24 13:36:09.000000 aacommpy-0.1.8/aacommpy/__version__.py
--rw-rw-rw-   0        0        0    10361 2023-04-23 17:15:24.000000 aacommpy-0.1.8/aacommpy/curves.py
--rw-rw-rw-   0        0        0     2289 2023-04-24 13:35:49.000000 aacommpy-0.1.8/aacommpy/entry_points.py
--rw-rw-rw-   0        0        0      104 2023-04-24 13:18:38.000000 aacommpy-0.1.8/aacommpy/nugetmanagement.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:36:17.348445 aacommpy-0.1.8/aacommpy.egg-info/
--rw-rw-rw-   0        0        0      533 2023-04-24 13:36:17.000000 aacommpy-0.1.8/aacommpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-24 13:36:17.000000 aacommpy-0.1.8/aacommpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 13:36:17.000000 aacommpy-0.1.8/aacommpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-24 13:36:17.000000 aacommpy-0.1.8/aacommpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 12:09:32.000000 aacommpy-0.1.8/aacommpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-04-24 13:36:17.000000 aacommpy-0.1.8/aacommpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 13:36:17.000000 aacommpy-0.1.8/aacommpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 13:36:17.349441 aacommpy-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1359 2023-04-24 13:36:13.000000 aacommpy-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:53:01.844637 aacommpy-0.1.9/
+-rw-rw-rw-   0        0        0     4295 2023-05-01 09:53:01.844637 aacommpy-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3784 2023-04-30 11:16:57.000000 aacommpy-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 09:53:01.812516 aacommpy-0.1.9/aacommpy/
+-rw-rw-rw-   0        0        0       95 2023-04-24 11:51:36.000000 aacommpy-0.1.9/aacommpy/__init__.py
+-rw-rw-rw-   0        0        0      263 2023-05-01 08:18:12.000000 aacommpy-0.1.9/aacommpy/__version__.py
+-rw-rw-rw-   0        0        0      876 2023-04-30 10:33:14.000000 aacommpy-0.1.9/aacommpy/aacommpy.py
+-rw-rw-rw-   0        0        0     6885 2023-04-24 16:38:20.000000 aacommpy-0.1.9/aacommpy/curves.py
+-rw-rw-rw-   0        0        0     1861 2023-05-01 09:51:58.000000 aacommpy-0.1.9/aacommpy/entry_points.py
+-rw-rw-rw-   0        0        0     2272 2023-05-01 09:35:50.000000 aacommpy-0.1.9/aacommpy/nugetmanagement.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:53:01.843640 aacommpy-0.1.9/aacommpy.egg-info/
+-rw-rw-rw-   0        0        0     4295 2023-05-01 09:53:01.000000 aacommpy-0.1.9/aacommpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-05-01 09:53:01.000000 aacommpy-0.1.9/aacommpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 09:53:01.000000 aacommpy-0.1.9/aacommpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-01 09:53:01.000000 aacommpy-0.1.9/aacommpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 12:09:32.000000 aacommpy-0.1.9/aacommpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2023-05-01 09:53:01.000000 aacommpy-0.1.9/aacommpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-01 09:53:01.000000 aacommpy-0.1.9/aacommpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 09:53:01.845633 aacommpy-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1359 2023-05-01 08:18:22.000000 aacommpy-0.1.9/setup.py
```

### Comparing `aacommpy-0.1.8/setup.py` & `aacommpy-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 from setuptools import setup
 
 about = {
     'name': 'aacommpy',
     'description': 'A Python package for wrapping aacomm nuget package',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'author': 'HIEU',
     'author_email': 'trunghieupcs@gmail.com',
     'url': 'https://github.com/hieu/aacommpy',
     'license': 'MIT',
 }
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, 'aacommpy', '__version__.py')) as f:
```

