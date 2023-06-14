# Comparing `tmp/LambertProblem-0.6.tar.gz` & `tmp/LambertProblem-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LambertProblem-0.6.tar", last modified: Tue Jun 13 16:02:10 2023, max compression
+gzip compressed data, was "LambertProblem-0.7.tar", last modified: Wed Jun 14 02:22:01 2023, max compression
```

## Comparing `LambertProblem-0.6.tar` & `LambertProblem-0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-13 16:02:10.496192 LambertProblem-0.6/
--rw-r--r--   0 juanita   (1000) juanita   (1000)     1134 2023-05-16 14:58:24.000000 LambertProblem-0.6/LICENSE
-drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-13 16:02:10.496192 LambertProblem-0.6/LambertProblem/
--rw-r--r--   0 juanita   (1000) juanita   (1000)     7345 2023-06-13 15:43:44.000000 LambertProblem-0.6/LambertProblem/__init__.py
-drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-13 16:02:10.496192 LambertProblem-0.6/LambertProblem.egg-info/
--rw-rw-r--   0 juanita   (1000) juanita   (1000)     2191 2023-06-13 16:02:10.000000 LambertProblem-0.6/LambertProblem.egg-info/PKG-INFO
--rw-rw-r--   0 juanita   (1000) juanita   (1000)      300 2023-06-13 16:02:10.000000 LambertProblem-0.6/LambertProblem.egg-info/SOURCES.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)        1 2023-06-13 16:02:10.000000 LambertProblem-0.6/LambertProblem.egg-info/dependency_links.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       51 2023-06-13 16:02:10.000000 LambertProblem-0.6/LambertProblem.egg-info/entry_points.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       12 2023-06-13 16:02:10.000000 LambertProblem-0.6/LambertProblem.egg-info/requires.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       15 2023-06-13 16:02:10.000000 LambertProblem-0.6/LambertProblem.egg-info/top_level.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)     2191 2023-06-13 16:02:10.496192 LambertProblem-0.6/PKG-INFO
--rw-r--r--   0 juanita   (1000) juanita   (1000)     1675 2023-05-16 14:58:20.000000 LambertProblem-0.6/README.md
--rw-r--r--   0 juanita   (1000) juanita   (1000)      110 2023-06-13 16:01:48.000000 LambertProblem-0.6/pyproject.toml
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       38 2023-06-13 16:02:10.496192 LambertProblem-0.6/setup.cfg
--rw-r--r--   0 juanita   (1000) juanita   (1000)     2233 2023-06-13 16:01:34.000000 LambertProblem-0.6/setup.py
+drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-14 02:22:01.268388 LambertProblem-0.7/
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     1134 2023-05-16 14:58:24.000000 LambertProblem-0.7/LICENSE
+drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-14 02:22:01.264388 LambertProblem-0.7/LambertProblem/
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     7345 2023-06-13 15:43:44.000000 LambertProblem-0.7/LambertProblem/__init__.py
+drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-14 02:22:01.264388 LambertProblem-0.7/LambertProblem.egg-info/
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)     2698 2023-06-14 02:22:01.000000 LambertProblem-0.7/LambertProblem.egg-info/PKG-INFO
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)      300 2023-06-14 02:22:01.000000 LambertProblem-0.7/LambertProblem.egg-info/SOURCES.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)        1 2023-06-14 02:22:01.000000 LambertProblem-0.7/LambertProblem.egg-info/dependency_links.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       51 2023-06-14 02:22:01.000000 LambertProblem-0.7/LambertProblem.egg-info/entry_points.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       12 2023-06-14 02:22:01.000000 LambertProblem-0.7/LambertProblem.egg-info/requires.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       15 2023-06-14 02:22:01.000000 LambertProblem-0.7/LambertProblem.egg-info/top_level.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)     2698 2023-06-14 02:22:01.264388 LambertProblem-0.7/PKG-INFO
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     2182 2023-06-14 02:19:40.000000 LambertProblem-0.7/README.md
+-rw-r--r--   0 juanita   (1000) juanita   (1000)      110 2023-06-13 16:01:48.000000 LambertProblem-0.7/pyproject.toml
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       38 2023-06-14 02:22:01.268388 LambertProblem-0.7/setup.cfg
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     2233 2023-06-14 02:20:14.000000 LambertProblem-0.7/setup.py
```

### Comparing `LambertProblem-0.6/LICENSE` & `LambertProblem-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `LambertProblem-0.6/LambertProblem/__init__.py` & `LambertProblem-0.7/LambertProblem/__init__.py`

 * *Files identical despite different names*

### Comparing `LambertProblem-0.6/setup.py` & `LambertProblem-0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         ],
-    version='0.6',
+    version='0.7',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
```

