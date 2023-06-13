# Comparing `tmp/CalibrationCurve-0.0.4.tar.gz` & `tmp/CalibrationCurve-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CalibrationCurve-0.0.4.tar", last modified: Tue Jun 13 22:28:13 2023, max compression
+gzip compressed data, was "CalibrationCurve-0.0.5.tar", last modified: Tue Jun 13 22:33:41 2023, max compression
```

## Comparing `CalibrationCurve-0.0.4.tar` & `CalibrationCurve-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 22:28:13.616908 CalibrationCurve-0.0.4/
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 22:28:13.616908 CalibrationCurve-0.0.4/CalibrationCurve/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-13 22:28:06.000000 CalibrationCurve-0.0.4/CalibrationCurve/__init__.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     4137 2023-06-13 22:28:06.000000 CalibrationCurve-0.0.4/CalibrationCurve/_modidx.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     3072 2023-06-13 22:28:06.000000 CalibrationCurve-0.0.4/CalibrationCurve/core.py
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 22:28:13.616908 CalibrationCurve-0.0.4/CalibrationCurve.egg-info/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1652 2023-06-13 22:28:13.000000 CalibrationCurve-0.0.4/CalibrationCurve.egg-info/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      414 2023-06-13 22:28:13.000000 CalibrationCurve-0.0.4/CalibrationCurve.egg-info/SOURCES.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-13 22:28:13.000000 CalibrationCurve-0.0.4/CalibrationCurve.egg-info/dependency_links.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       54 2023-06-13 22:28:13.000000 CalibrationCurve-0.0.4/CalibrationCurve.egg-info/entry_points.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-13 00:26:53.000000 CalibrationCurve-0.0.4/CalibrationCurve.egg-info/not-zip-safe
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       62 2023-06-13 22:28:13.000000 CalibrationCurve-0.0.4/CalibrationCurve.egg-info/requires.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       17 2023-06-13 22:28:13.000000 CalibrationCurve-0.0.4/CalibrationCurve.egg-info/top_level.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.4/LICENSE
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.4/MANIFEST.in
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1652 2023-06-13 22:28:13.616908 CalibrationCurve-0.0.4/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      787 2023-06-13 01:59:09.000000 CalibrationCurve-0.0.4/README.md
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      998 2023-06-13 22:28:00.000000 CalibrationCurve-0.0.4/settings.ini
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-13 22:28:13.616908 CalibrationCurve-0.0.4/setup.cfg
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.4/setup.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 22:33:41.204588 CalibrationCurve-0.0.5/
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 22:33:41.204588 CalibrationCurve-0.0.5/CalibrationCurve/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-13 22:33:35.000000 CalibrationCurve-0.0.5/CalibrationCurve/__init__.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     4137 2023-06-13 22:33:35.000000 CalibrationCurve-0.0.5/CalibrationCurve/_modidx.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     3072 2023-06-13 22:33:35.000000 CalibrationCurve-0.0.5/CalibrationCurve/core.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 22:33:41.204588 CalibrationCurve-0.0.5/CalibrationCurve.egg-info/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1652 2023-06-13 22:33:41.000000 CalibrationCurve-0.0.5/CalibrationCurve.egg-info/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      414 2023-06-13 22:33:41.000000 CalibrationCurve-0.0.5/CalibrationCurve.egg-info/SOURCES.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-13 22:33:41.000000 CalibrationCurve-0.0.5/CalibrationCurve.egg-info/dependency_links.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       54 2023-06-13 22:33:41.000000 CalibrationCurve-0.0.5/CalibrationCurve.egg-info/entry_points.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-13 00:26:53.000000 CalibrationCurve-0.0.5/CalibrationCurve.egg-info/not-zip-safe
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       67 2023-06-13 22:33:41.000000 CalibrationCurve-0.0.5/CalibrationCurve.egg-info/requires.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       17 2023-06-13 22:33:41.000000 CalibrationCurve-0.0.5/CalibrationCurve.egg-info/top_level.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.5/LICENSE
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.5/MANIFEST.in
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1652 2023-06-13 22:33:41.204588 CalibrationCurve-0.0.5/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      787 2023-06-13 01:59:09.000000 CalibrationCurve-0.0.5/README.md
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1003 2023-06-13 22:33:35.000000 CalibrationCurve-0.0.5/settings.ini
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-13 22:33:41.204588 CalibrationCurve-0.0.5/setup.cfg
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.5/setup.py
```

### Comparing `CalibrationCurve-0.0.4/CalibrationCurve/_modidx.py` & `CalibrationCurve-0.0.5/CalibrationCurve/_modidx.py`

 * *Files identical despite different names*

### Comparing `CalibrationCurve-0.0.4/CalibrationCurve/core.py` & `CalibrationCurve-0.0.5/CalibrationCurve/core.py`

 * *Files identical despite different names*

### Comparing `CalibrationCurve-0.0.4/CalibrationCurve.egg-info/PKG-INFO` & `CalibrationCurve-0.0.5/CalibrationCurve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalibrationCurve
-Version: 0.0.4
+Version: 0.0.5
 Summary: A collection of functions that streamline the process of creating calibration curves using Python.
 Home-page: https://github.com/Rhys-McAlister/CalibrationCurve
 Author: Rhys McAlister
 Author-email: mcalisterrhys@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CalibrationCurve-0.0.4/LICENSE` & `CalibrationCurve-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CalibrationCurve-0.0.4/PKG-INFO` & `CalibrationCurve-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalibrationCurve
-Version: 0.0.4
+Version: 0.0.5
 Summary: A collection of functions that streamline the process of creating calibration curves using Python.
 Home-page: https://github.com/Rhys-McAlister/CalibrationCurve
 Author: Rhys McAlister
 Author-email: mcalisterrhys@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CalibrationCurve-0.0.4/README.md` & `CalibrationCurve-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `CalibrationCurve-0.0.4/settings.ini` & `CalibrationCurve-0.0.5/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = CalibrationCurve
 lib_name = CalibrationCurve
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = CalibrationCurve
 nbs_path = nbs
 recursive = True
@@ -22,15 +22,15 @@
 author_email = mcalisterrhys@gmail.com
 copyright = 2023 onwards, Rhys McAlister
 description = A collection of functions that streamline the process of creating calibration curves using Python.
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = Rhys-McAlister
-requirements = fastcore pandas sklearn matplotlib numpy seaborn scipy
+requirements = fastcore pandas scikit-learn matplotlib numpy seaborn scipy
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
```

### Comparing `CalibrationCurve-0.0.4/setup.py` & `CalibrationCurve-0.0.5/setup.py`

 * *Files identical despite different names*

