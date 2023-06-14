# Comparing `tmp/mjwt-0.0.3.tar.gz` & `tmp/mjwt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mjwt-0.0.3.tar", last modified: Wed Jun 14 13:56:02 2023, max compression
+gzip compressed data, was "mjwt-0.0.4.tar", last modified: Wed Jun 14 14:22:32 2023, max compression
```

## Comparing `mjwt-0.0.3.tar` & `mjwt-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 13:56:02.201905 mjwt-0.0.3/
--rw-r--r--   0 jovyan    (1000) users      (100)     1072 2023-06-09 12:33:50.000000 mjwt-0.0.3/LICENSE
--rw-rw-r--   0 jovyan    (1000) users      (100)      111 2023-04-27 10:12:58.000000 mjwt-0.0.3/MANIFEST.in
--rw-r--r--   0 jovyan    (1000) users      (100)     1365 2023-06-14 13:56:02.196897 mjwt-0.0.3/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)      546 2023-06-14 13:51:17.000000 mjwt-0.0.3/README.md
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 13:56:02.080057 mjwt-0.0.3/mjwt/
--rw-r--r--   0 jovyan    (1000) users      (100)       22 2023-06-14 13:51:10.000000 mjwt-0.0.3/mjwt/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)     3140 2023-06-14 13:51:10.000000 mjwt-0.0.3/mjwt/_modidx.py
--rw-r--r--   0 jovyan    (1000) users      (100)    10861 2023-06-14 13:51:10.000000 mjwt-0.0.3/mjwt/utils.py
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 13:56:02.182476 mjwt-0.0.3/mjwt.egg-info/
--rw-r--r--   0 jovyan    (1000) users      (100)     1365 2023-06-14 13:56:01.000000 mjwt-0.0.3/mjwt.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)      295 2023-06-14 13:56:01.000000 mjwt-0.0.3/mjwt.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-06-14 13:56:01.000000 mjwt-0.0.3/mjwt.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       93 2023-06-14 13:56:01.000000 mjwt-0.0.3/mjwt.egg-info/entry_points.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-06-09 14:25:28.000000 mjwt-0.0.3/mjwt.egg-info/not-zip-safe
--rw-r--r--   0 jovyan    (1000) users      (100)       37 2023-06-14 13:56:01.000000 mjwt-0.0.3/mjwt.egg-info/requires.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        5 2023-06-14 13:56:01.000000 mjwt-0.0.3/mjwt.egg-info/top_level.txt
--rw-r--r--   0 jovyan    (1000) users      (100)      940 2023-06-14 13:47:35.000000 mjwt-0.0.3/settings.ini
--rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-06-14 13:56:02.203886 mjwt-0.0.3/setup.cfg
--rw-rw-r--   0 jovyan    (1000) users      (100)     2596 2023-04-27 10:12:58.000000 mjwt-0.0.3/setup.py
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 14:22:32.206904 mjwt-0.0.4/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1072 2023-06-09 12:33:50.000000 mjwt-0.0.4/LICENSE
+-rw-rw-r--   0 jovyan    (1000) users      (100)      111 2023-04-27 10:12:58.000000 mjwt-0.0.4/MANIFEST.in
+-rw-r--r--   0 jovyan    (1000) users      (100)     1365 2023-06-14 14:22:32.203125 mjwt-0.0.4/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)      546 2023-06-14 13:51:17.000000 mjwt-0.0.4/README.md
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 14:22:32.104359 mjwt-0.0.4/mjwt/
+-rw-r--r--   0 jovyan    (1000) users      (100)       22 2023-06-14 14:22:30.000000 mjwt-0.0.4/mjwt/__init__.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     3140 2023-06-14 14:22:30.000000 mjwt-0.0.4/mjwt/_modidx.py
+-rw-r--r--   0 jovyan    (1000) users      (100)    10861 2023-06-14 14:22:30.000000 mjwt-0.0.4/mjwt/utils.py
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 14:22:32.192804 mjwt-0.0.4/mjwt.egg-info/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1365 2023-06-14 14:22:31.000000 mjwt-0.0.4/mjwt.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)      295 2023-06-14 14:22:31.000000 mjwt-0.0.4/mjwt.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-06-14 14:22:31.000000 mjwt-0.0.4/mjwt.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)       82 2023-06-14 14:22:31.000000 mjwt-0.0.4/mjwt.egg-info/entry_points.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-06-09 14:25:28.000000 mjwt-0.0.4/mjwt.egg-info/not-zip-safe
+-rw-r--r--   0 jovyan    (1000) users      (100)       45 2023-06-14 14:22:31.000000 mjwt-0.0.4/mjwt.egg-info/requires.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        5 2023-06-14 14:22:31.000000 mjwt-0.0.4/mjwt.egg-info/top_level.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)      937 2023-06-14 14:22:30.000000 mjwt-0.0.4/settings.ini
+-rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-06-14 14:22:32.208333 mjwt-0.0.4/setup.cfg
+-rw-rw-r--   0 jovyan    (1000) users      (100)     2596 2023-04-27 10:12:58.000000 mjwt-0.0.4/setup.py
```

### Comparing `mjwt-0.0.3/LICENSE` & `mjwt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mjwt-0.0.3/PKG-INFO` & `mjwt-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mjwt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package with coding tools, code snippets and notes from Menno Witteveen
 Home-page: https://github.com/mennowitteveen/mjwt
 Author: Menno Witteveen
 Author-email: menno102@hotmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mjwt-0.0.3/README.md` & `mjwt-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mjwt-0.0.3/mjwt/_modidx.py` & `mjwt-0.0.4/mjwt/_modidx.py`

 * *Files identical despite different names*

### Comparing `mjwt-0.0.3/mjwt/utils.py` & `mjwt-0.0.4/mjwt/utils.py`

 * *Files identical despite different names*

### Comparing `mjwt-0.0.3/mjwt.egg-info/PKG-INFO` & `mjwt-0.0.4/mjwt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mjwt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package with coding tools, code snippets and notes from Menno Witteveen
 Home-page: https://github.com/mennowitteveen/mjwt
 Author: Menno Witteveen
 Author-email: menno102@hotmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mjwt-0.0.3/settings.ini` & `mjwt-0.0.4/settings.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = mjwt
 lib_name = mjwt
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = mjwt
 nbs_path = nbs
 recursive = True
@@ -28,10 +28,10 @@
 user = mennowitteveen
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
-requirements = pandas numpy scipy matplotlib
-console_scripts = mjwt_magic=mjwt.utils.printfun:mjwt_magic
+requirements = pandas numpy scipy matplotlib ipython
+console_scripts = mjwt_magic=mjwt.utils:printfun
```

### Comparing `mjwt-0.0.3/setup.py` & `mjwt-0.0.4/setup.py`

 * *Files identical despite different names*

