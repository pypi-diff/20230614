# Comparing `tmp/thefriendlystars-0.1.0.tar.gz` & `tmp/thefriendlystars-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thefriendlystars-0.1.0.tar", last modified: Wed Jun 14 03:20:23 2023, max compression
+gzip compressed data, was "thefriendlystars-0.1.1.tar", last modified: Wed Jun 14 07:41:06 2023, max compression
```

## Comparing `thefriendlystars-0.1.0.tar` & `thefriendlystars-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-14 03:20:23.841244 thefriendlystars-0.1.0/
--rw-r--r--   0 zach       (502) staff       (20)     1076 2023-06-14 03:17:18.000000 thefriendlystars-0.1.0/LICENSE
--rw-r--r--   0 zach       (502) staff       (20)      616 2023-06-14 03:20:23.840994 thefriendlystars-0.1.0/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)     2299 2023-06-14 03:19:01.000000 thefriendlystars-0.1.0/README.md
--rw-r--r--   0 zach       (502) staff       (20)       38 2023-06-14 03:20:23.841312 thefriendlystars-0.1.0/setup.cfg
--rw-r--r--   0 zach       (502) staff       (20)     3882 2023-06-14 03:18:21.000000 thefriendlystars-0.1.0/setup.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-14 03:20:23.839170 thefriendlystars-0.1.0/thefriendlystars/
--rw-r--r--   0 zach       (502) staff       (20)       19 2023-06-14 03:17:18.000000 thefriendlystars-0.1.0/thefriendlystars/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     7860 2023-06-14 03:17:18.000000 thefriendlystars-0.1.0/thefriendlystars/gaia.py
--rw-r--r--   0 zach       (502) staff       (20)      306 2023-06-14 03:17:18.000000 thefriendlystars-0.1.0/thefriendlystars/imports.py
--rwxr-xr-x   0 zach       (502) staff       (20)       62 2023-06-14 03:17:18.000000 thefriendlystars-0.1.0/thefriendlystars/version.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-14 03:20:23.840679 thefriendlystars-0.1.0/thefriendlystars.egg-info/
--rw-r--r--   0 zach       (502) staff       (20)      616 2023-06-14 03:20:23.000000 thefriendlystars-0.1.0/thefriendlystars.egg-info/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)      374 2023-06-14 03:20:23.000000 thefriendlystars-0.1.0/thefriendlystars.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2023-06-14 03:20:23.000000 thefriendlystars-0.1.0/thefriendlystars.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2023-06-14 03:19:56.000000 thefriendlystars-0.1.0/thefriendlystars.egg-info/not-zip-safe
--rw-r--r--   0 zach       (502) staff       (20)      204 2023-06-14 03:20:23.000000 thefriendlystars-0.1.0/thefriendlystars.egg-info/requires.txt
--rw-r--r--   0 zach       (502) staff       (20)       17 2023-06-14 03:20:23.000000 thefriendlystars-0.1.0/thefriendlystars.egg-info/top_level.txt
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-14 07:41:06.271602 thefriendlystars-0.1.1/
+-rw-r--r--   0 zach       (502) staff       (20)     1076 2023-06-14 03:17:18.000000 thefriendlystars-0.1.1/LICENSE
+-rw-r--r--   0 zach       (502) staff       (20)      616 2023-06-14 07:41:06.271455 thefriendlystars-0.1.1/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)     2299 2023-06-14 03:19:01.000000 thefriendlystars-0.1.1/README.md
+-rw-r--r--   0 zach       (502) staff       (20)       38 2023-06-14 07:41:06.271643 thefriendlystars-0.1.1/setup.cfg
+-rw-r--r--   0 zach       (502) staff       (20)     3882 2023-06-14 03:23:24.000000 thefriendlystars-0.1.1/setup.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-14 07:41:06.270265 thefriendlystars-0.1.1/thefriendlystars/
+-rw-r--r--   0 zach       (502) staff       (20)       19 2023-06-14 03:17:18.000000 thefriendlystars-0.1.1/thefriendlystars/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     7917 2023-06-14 03:58:43.000000 thefriendlystars-0.1.1/thefriendlystars/gaia.py
+-rw-r--r--   0 zach       (502) staff       (20)      306 2023-06-14 03:17:18.000000 thefriendlystars-0.1.1/thefriendlystars/imports.py
+-rwxr-xr-x   0 zach       (502) staff       (20)       62 2023-06-14 07:40:53.000000 thefriendlystars-0.1.1/thefriendlystars/version.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-14 07:41:06.271232 thefriendlystars-0.1.1/thefriendlystars.egg-info/
+-rw-r--r--   0 zach       (502) staff       (20)      616 2023-06-14 07:41:06.000000 thefriendlystars-0.1.1/thefriendlystars.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)      374 2023-06-14 07:41:06.000000 thefriendlystars-0.1.1/thefriendlystars.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2023-06-14 07:41:06.000000 thefriendlystars-0.1.1/thefriendlystars.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2023-06-14 03:19:56.000000 thefriendlystars-0.1.1/thefriendlystars.egg-info/not-zip-safe
+-rw-r--r--   0 zach       (502) staff       (20)      204 2023-06-14 07:41:06.000000 thefriendlystars-0.1.1/thefriendlystars.egg-info/requires.txt
+-rw-r--r--   0 zach       (502) staff       (20)       17 2023-06-14 07:41:06.000000 thefriendlystars-0.1.1/thefriendlystars.egg-info/top_level.txt
```

### Comparing `thefriendlystars-0.1.0/LICENSE` & `thefriendlystars-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thefriendlystars-0.1.0/PKG-INFO` & `thefriendlystars-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thefriendlystars
-Version: 0.1.0
+Version: 0.1.1
 Summary:  Python toolkit for making finder charts with catalogs that cover a small patch of the sky.
 Home-page: https://github.com/zkbt/thefriendlystars/
 Author: Zach Berta-Thompson
 Author-email: zach.bertathompson@colorado.edu
 License: MIT
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `thefriendlystars-0.1.0/README.md` & `thefriendlystars-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `thefriendlystars-0.1.0/setup.py` & `thefriendlystars-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `thefriendlystars-0.1.0/thefriendlystars/gaia.py` & `thefriendlystars-0.1.1/thefriendlystars/gaia.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from astropy.table import QTable
 from astropy.visualization import quantity_support
 import warnings 
 
 # set a high row limit to allow lots of stars in crowded fields
 Gaia.ROW_LIMIT = 50000
 Gaia.MAIN_GAIA_TABLE = "gaiaedr3.gaia_source"
+gaia_epoch = 2016.0
 
 # Gaia filter transformations from
 # https://gea.esac.esa.int/archive/documentation/GDR2/Data_processing/chap_cu5pho/sec_cu5pho_calibr/ssec_cu5pho_PhotTransf.html
 terms = {}
 terms["G-r_sloan"] = [-0.12879, 0.24662, -0.027464, -0.049465]
 terms["G-i_sloan"] = [-0.29676, 0.64728, -0.10141]
 terms["G-g_sloan"] = [0.13518, -0.46245, -0.25171, 0.021349]
@@ -145,14 +146,15 @@
 
     # populate with other estimated filter magnitudes
     table = estimate_other_filters(table)
 
     # keep track of center and radius
     table.meta["center"] = center_skycoord
     table.meta["radius"] = radius
+    table.meta['epoch'] = gaia_epoch
 
     # return the table
     return table
 
 
 def plot_gaia(
     table,
```

### Comparing `thefriendlystars-0.1.0/thefriendlystars.egg-info/PKG-INFO` & `thefriendlystars-0.1.1/thefriendlystars.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thefriendlystars
-Version: 0.1.0
+Version: 0.1.1
 Summary:  Python toolkit for making finder charts with catalogs that cover a small patch of the sky.
 Home-page: https://github.com/zkbt/thefriendlystars/
 Author: Zach Berta-Thompson
 Author-email: zach.bertathompson@colorado.edu
 License: MIT
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

