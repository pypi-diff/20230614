# Comparing `tmp/mjwt-0.0.2.tar.gz` & `tmp/mjwt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mjwt-0.0.2.tar", last modified: Wed Jun 14 10:32:29 2023, max compression
+gzip compressed data, was "mjwt-0.0.3.tar", last modified: Wed Jun 14 13:56:02 2023, max compression
```

## Comparing `mjwt-0.0.2.tar` & `mjwt-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 10:32:29.387441 mjwt-0.0.2/
--rw-r--r--   0 jovyan    (1000) users      (100)     1072 2023-06-09 12:33:50.000000 mjwt-0.0.2/LICENSE
--rw-rw-r--   0 jovyan    (1000) users      (100)      111 2023-04-27 10:12:58.000000 mjwt-0.0.2/MANIFEST.in
--rw-r--r--   0 jovyan    (1000) users      (100)     1323 2023-06-14 10:32:29.384119 mjwt-0.0.2/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)      504 2023-06-14 10:00:25.000000 mjwt-0.0.2/README.md
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 10:32:29.231873 mjwt-0.0.2/mjwt/
--rw-r--r--   0 jovyan    (1000) users      (100)       22 2023-06-14 10:32:11.000000 mjwt-0.0.2/mjwt/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)      369 2023-06-14 10:32:11.000000 mjwt-0.0.2/mjwt/_modidx.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1664 2023-06-14 10:32:11.000000 mjwt-0.0.2/mjwt/utils.py
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 10:32:29.372298 mjwt-0.0.2/mjwt.egg-info/
--rw-r--r--   0 jovyan    (1000) users      (100)     1323 2023-06-14 10:32:28.000000 mjwt-0.0.2/mjwt.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)      295 2023-06-14 10:32:28.000000 mjwt-0.0.2/mjwt.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-06-14 10:32:28.000000 mjwt-0.0.2/mjwt.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       30 2023-06-14 10:32:28.000000 mjwt-0.0.2/mjwt.egg-info/entry_points.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-06-09 14:25:28.000000 mjwt-0.0.2/mjwt.egg-info/not-zip-safe
--rw-r--r--   0 jovyan    (1000) users      (100)        7 2023-06-14 10:32:28.000000 mjwt-0.0.2/mjwt.egg-info/requires.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        5 2023-06-14 10:32:28.000000 mjwt-0.0.2/mjwt.egg-info/top_level.txt
--rw-r--r--   0 jovyan    (1000) users      (100)      835 2023-06-14 10:32:11.000000 mjwt-0.0.2/settings.ini
--rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-06-14 10:32:29.388613 mjwt-0.0.2/setup.cfg
--rw-rw-r--   0 jovyan    (1000) users      (100)     2596 2023-04-27 10:12:58.000000 mjwt-0.0.2/setup.py
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 13:56:02.201905 mjwt-0.0.3/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1072 2023-06-09 12:33:50.000000 mjwt-0.0.3/LICENSE
+-rw-rw-r--   0 jovyan    (1000) users      (100)      111 2023-04-27 10:12:58.000000 mjwt-0.0.3/MANIFEST.in
+-rw-r--r--   0 jovyan    (1000) users      (100)     1365 2023-06-14 13:56:02.196897 mjwt-0.0.3/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)      546 2023-06-14 13:51:17.000000 mjwt-0.0.3/README.md
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 13:56:02.080057 mjwt-0.0.3/mjwt/
+-rw-r--r--   0 jovyan    (1000) users      (100)       22 2023-06-14 13:51:10.000000 mjwt-0.0.3/mjwt/__init__.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     3140 2023-06-14 13:51:10.000000 mjwt-0.0.3/mjwt/_modidx.py
+-rw-r--r--   0 jovyan    (1000) users      (100)    10861 2023-06-14 13:51:10.000000 mjwt-0.0.3/mjwt/utils.py
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 13:56:02.182476 mjwt-0.0.3/mjwt.egg-info/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1365 2023-06-14 13:56:01.000000 mjwt-0.0.3/mjwt.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)      295 2023-06-14 13:56:01.000000 mjwt-0.0.3/mjwt.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-06-14 13:56:01.000000 mjwt-0.0.3/mjwt.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)       93 2023-06-14 13:56:01.000000 mjwt-0.0.3/mjwt.egg-info/entry_points.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-06-09 14:25:28.000000 mjwt-0.0.3/mjwt.egg-info/not-zip-safe
+-rw-r--r--   0 jovyan    (1000) users      (100)       37 2023-06-14 13:56:01.000000 mjwt-0.0.3/mjwt.egg-info/requires.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        5 2023-06-14 13:56:01.000000 mjwt-0.0.3/mjwt.egg-info/top_level.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)      940 2023-06-14 13:47:35.000000 mjwt-0.0.3/settings.ini
+-rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-06-14 13:56:02.203886 mjwt-0.0.3/setup.cfg
+-rw-rw-r--   0 jovyan    (1000) users      (100)     2596 2023-04-27 10:12:58.000000 mjwt-0.0.3/setup.py
```

### Comparing `mjwt-0.0.2/LICENSE` & `mjwt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mjwt-0.0.2/PKG-INFO` & `mjwt-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mjwt
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package with coding tools, code snippets and notes from Menno Witteveen
 Home-page: https://github.com/mennowitteveen/mjwt
 Author: Menno Witteveen
 Author-email: menno102@hotmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -21,16 +21,17 @@
 License-File: LICENSE
 
 mjwt
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-Hurr durr, this will become my readme it says. is this now mjws readmoi?
-This is new text 14-6 thunderbird
+Construction newest readme. JUne14-15:51. Hurr durr, this will become my
+readme it says. is this now mjws readmoi? This is new text 14-6
+thunderbird
 
 ## Install
 
 ``` sh
 pip install mjwt
 ```
```

### Comparing `mjwt-0.0.2/mjwt.egg-info/PKG-INFO` & `mjwt-0.0.3/mjwt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mjwt
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package with coding tools, code snippets and notes from Menno Witteveen
 Home-page: https://github.com/mennowitteveen/mjwt
 Author: Menno Witteveen
 Author-email: menno102@hotmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -21,16 +21,17 @@
 License-File: LICENSE
 
 mjwt
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-Hurr durr, this will become my readme it says. is this now mjws readmoi?
-This is new text 14-6 thunderbird
+Construction newest readme. JUne14-15:51. Hurr durr, this will become my
+readme it says. is this now mjws readmoi? This is new text 14-6
+thunderbird
 
 ## Install
 
 ``` sh
 pip install mjwt
 ```
```

### Comparing `mjwt-0.0.2/settings.ini` & `mjwt-0.0.3/settings.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = mjwt
 lib_name = mjwt
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = mjwt
 nbs_path = nbs
 recursive = True
@@ -28,8 +28,10 @@
 user = mennowitteveen
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
+requirements = pandas numpy scipy matplotlib
+console_scripts = mjwt_magic=mjwt.utils.printfun:mjwt_magic
```

### Comparing `mjwt-0.0.2/setup.py` & `mjwt-0.0.3/setup.py`

 * *Files identical despite different names*

