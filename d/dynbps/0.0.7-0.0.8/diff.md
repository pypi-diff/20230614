# Comparing `tmp/dynbps-0.0.7.tar.gz` & `tmp/dynbps-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dynbps-0.0.7.tar", last modified: Mon May 22 19:23:59 2023, max compression
+gzip compressed data, was "dist/dynbps-0.0.8.tar", last modified: Mon May 22 22:17:46 2023, max compression
```

## Comparing `dynbps-0.0.7.tar` & `dynbps-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-22 19:23:59.562447 dynbps-0.0.7/
--rw-r--r--   0 josephrilling   (501) staff       (20)    11357 2023-05-16 21:26:28.000000 dynbps-0.0.7/LICENSE
--rw-rw-r--   0 josephrilling   (501) staff       (20)      111 2023-04-27 10:12:58.000000 dynbps-0.0.7/MANIFEST.in
--rw-r--r--   0 josephrilling   (501) staff       (20)     1051 2023-05-22 19:23:59.561791 dynbps-0.0.7/PKG-INFO
--rw-r--r--   0 josephrilling   (501) staff       (20)      284 2023-05-22 19:10:12.000000 dynbps-0.0.7/README.md
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-22 19:23:59.551951 dynbps-0.0.7/dynbps/
--rw-r--r--   0 josephrilling   (501) staff       (20)     8905 2023-05-22 19:23:47.000000 dynbps-0.0.7/dynbps/BPS.py
--rw-r--r--   0 josephrilling   (501) staff       (20)       22 2023-05-22 19:23:47.000000 dynbps-0.0.7/dynbps/__init__.py
--rw-r--r--   0 josephrilling   (501) staff       (20)      763 2023-05-22 19:23:47.000000 dynbps-0.0.7/dynbps/_modidx.py
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-22 19:23:59.559712 dynbps-0.0.7/dynbps/datasets/
--rw-r--r--   0 josephrilling   (501) staff       (20)    41999 2023-05-17 22:21:27.000000 dynbps-0.0.7/dynbps/datasets/data.xlsx
--rw-r--r--   0 josephrilling   (501) staff       (20)      747 2023-05-22 19:23:47.000000 dynbps-0.0.7/dynbps/loadData.py
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-22 19:23:59.558803 dynbps-0.0.7/dynbps.egg-info/
--rw-r--r--   0 josephrilling   (501) staff       (20)     1051 2023-05-22 19:23:59.000000 dynbps-0.0.7/dynbps.egg-info/PKG-INFO
--rw-r--r--   0 josephrilling   (501) staff       (20)      358 2023-05-22 19:23:59.000000 dynbps-0.0.7/dynbps.egg-info/SOURCES.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-22 19:23:59.000000 dynbps-0.0.7/dynbps.egg-info/dependency_links.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)       34 2023-05-22 19:23:59.000000 dynbps-0.0.7/dynbps.egg-info/entry_points.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 21:36:56.000000 dynbps-0.0.7/dynbps.egg-info/not-zip-safe
--rw-r--r--   0 josephrilling   (501) staff       (20)       35 2023-05-22 19:23:59.000000 dynbps-0.0.7/dynbps.egg-info/requires.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        7 2023-05-22 19:23:59.000000 dynbps-0.0.7/dynbps.egg-info/top_level.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)      830 2023-05-22 19:23:47.000000 dynbps-0.0.7/settings.ini
--rw-r--r--   0 josephrilling   (501) staff       (20)       38 2023-05-22 19:23:59.562617 dynbps-0.0.7/setup.cfg
--rw-rw-r--   0 josephrilling   (501) staff       (20)     2640 2023-05-17 22:24:08.000000 dynbps-0.0.7/setup.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-22 22:17:46.353302 dynbps-0.0.8/
+-rw-r--r--   0 josephrilling   (501) staff       (20)    11357 2023-05-16 21:26:28.000000 dynbps-0.0.8/LICENSE
+-rw-rw-r--   0 josephrilling   (501) staff       (20)      111 2023-04-27 10:12:58.000000 dynbps-0.0.8/MANIFEST.in
+-rw-r--r--   0 josephrilling   (501) staff       (20)     7337 2023-05-22 22:17:46.351531 dynbps-0.0.8/PKG-INFO
+-rw-r--r--   0 josephrilling   (501) staff       (20)     6570 2023-05-22 22:10:05.000000 dynbps-0.0.8/README.md
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-22 22:17:46.332153 dynbps-0.0.8/dynbps/
+-rw-r--r--   0 josephrilling   (501) staff       (20)     8905 2023-05-22 22:17:36.000000 dynbps-0.0.8/dynbps/BPS.py
+-rw-r--r--   0 josephrilling   (501) staff       (20)       22 2023-05-22 22:17:36.000000 dynbps-0.0.8/dynbps/__init__.py
+-rw-r--r--   0 josephrilling   (501) staff       (20)      763 2023-05-22 22:17:36.000000 dynbps-0.0.8/dynbps/_modidx.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-22 22:17:46.348316 dynbps-0.0.8/dynbps/datasets/
+-rw-r--r--   0 josephrilling   (501) staff       (20)    41999 2023-05-17 22:21:27.000000 dynbps-0.0.8/dynbps/datasets/data.xlsx
+-rw-r--r--   0 josephrilling   (501) staff       (20)      747 2023-05-22 22:17:36.000000 dynbps-0.0.8/dynbps/loadData.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-22 22:17:46.347249 dynbps-0.0.8/dynbps.egg-info/
+-rw-r--r--   0 josephrilling   (501) staff       (20)     7337 2023-05-22 22:17:46.000000 dynbps-0.0.8/dynbps.egg-info/PKG-INFO
+-rw-r--r--   0 josephrilling   (501) staff       (20)      358 2023-05-22 22:17:46.000000 dynbps-0.0.8/dynbps.egg-info/SOURCES.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-22 22:17:46.000000 dynbps-0.0.8/dynbps.egg-info/dependency_links.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)       34 2023-05-22 22:17:46.000000 dynbps-0.0.8/dynbps.egg-info/entry_points.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 21:36:56.000000 dynbps-0.0.8/dynbps.egg-info/not-zip-safe
+-rw-r--r--   0 josephrilling   (501) staff       (20)       44 2023-05-22 22:17:46.000000 dynbps-0.0.8/dynbps.egg-info/requires.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        7 2023-05-22 22:17:46.000000 dynbps-0.0.8/dynbps.egg-info/top_level.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)      839 2023-05-22 22:17:36.000000 dynbps-0.0.8/settings.ini
+-rw-r--r--   0 josephrilling   (501) staff       (20)       38 2023-05-22 22:17:46.353588 dynbps-0.0.8/setup.cfg
+-rw-rw-r--   0 josephrilling   (501) staff       (20)     2640 2023-05-17 22:24:08.000000 dynbps-0.0.8/setup.py
```

### Comparing `dynbps-0.0.7/LICENSE` & `dynbps-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.7/dynbps/BPS.py` & `dynbps-0.0.8/dynbps/BPS.py`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.7/dynbps/_modidx.py` & `dynbps-0.0.8/dynbps/_modidx.py`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.7/dynbps/datasets/data.xlsx` & `dynbps-0.0.8/dynbps/datasets/data.xlsx`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.7/dynbps/loadData.py` & `dynbps-0.0.8/dynbps/loadData.py`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.7/settings.ini` & `dynbps-0.0.8/settings.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dynbps
 lib_name = dynbps
-version = 0.0.7
+version = 0.0.8
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dynbps
 nbs_path = nbs
 recursive = True
@@ -22,15 +22,15 @@
 author_email = tun52698@gmail.com
 copyright = 2023 onwards, josephrilling
 description = Python code for Dynamic BPS
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = josephrilling
-requirements = fastcore pandas numpy scipy
+requirements = fastcore pandas numpy scipy openpyxl
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
```

### Comparing `dynbps-0.0.7/setup.py` & `dynbps-0.0.8/setup.py`

 * *Files identical despite different names*

