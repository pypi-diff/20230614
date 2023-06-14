# Comparing `tmp/lm_datahandler-0.1.1.tar.gz` & `tmp/lm_datahandler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lm_datahandler-0.1.1.tar", last modified: Wed Jun 14 05:56:25 2023, max compression
+gzip compressed data, was "lm_datahandler-0.1.2.tar", last modified: Wed Jun 14 11:12:24 2023, max compression
```

## Comparing `lm_datahandler-0.1.1.tar` & `lm_datahandler-0.1.2.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 05:56:25.899778 lm_datahandler-0.1.1/
--rw-rw-rw-   0        0        0     1104 2023-06-14 03:54:04.000000 lm_datahandler-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      325 2023-06-14 05:56:25.899616 lm_datahandler-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 05:56:25.866308 lm_datahandler-0.1.1/lm_datahandler/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:11:31.000000 lm_datahandler-0.1.1/lm_datahandler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 05:56:25.891685 lm_datahandler-0.1.1/lm_datahandler/data_load/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:11:51.000000 lm_datahandler-0.1.1/lm_datahandler/data_load/__init__.py
--rw-rw-rw-   0        0        0     1674 2023-06-13 02:30:00.000000 lm_datahandler-0.1.1/lm_datahandler/data_load/data_loader.py
--rw-rw-rw-   0        0        0    10521 2023-06-13 02:44:38.000000 lm_datahandler-0.1.1/lm_datahandler/data_load/loaders.py
--rw-rw-rw-   0        0        0    24343 2023-06-14 03:57:25.000000 lm_datahandler-0.1.1/lm_datahandler/datahandler.py
-drwxrwxrwx   0        0        0        0 2023-06-14 05:56:25.895190 lm_datahandler-0.1.1/lm_datahandler/functions/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:02.000000 lm_datahandler-0.1.1/lm_datahandler/functions/__init__.py
--rw-rw-rw-   0        0        0    31179 2023-06-14 03:24:58.000000 lm_datahandler-0.1.1/lm_datahandler/functions/biomarker.py
--rw-rw-rw-   0        0        0    14569 2023-06-02 03:05:39.000000 lm_datahandler-0.1.1/lm_datahandler/functions/feature_extract.py
--rw-rw-rw-   0        0        0        0 2023-05-31 12:12:04.000000 lm_datahandler-0.1.1/lm_datahandler/functions/os_detect.py
--rw-rw-rw-   0        0        0     1392 2023-06-14 03:25:28.000000 lm_datahandler-0.1.1/lm_datahandler/functions/sleep_staging.py
--rw-rw-rw-   0        0        0     3240 2023-06-14 03:25:28.000000 lm_datahandler-0.1.1/lm_datahandler/functions/sleep_variable_compute.py
--rw-rw-rw-   0        0        0        0 2023-05-31 12:11:57.000000 lm_datahandler-0.1.1/lm_datahandler/functions/spindle_detect.py
-drwxrwxrwx   0        0        0        0 2023-06-14 05:56:25.896252 lm_datahandler-0.1.1/lm_datahandler/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:16.000000 lm_datahandler-0.1.1/lm_datahandler/plots/__init__.py
--rw-rw-rw-   0        0        0      625 2023-06-07 08:43:30.000000 lm_datahandler-0.1.1/lm_datahandler/plots/biomarker_plot.py
--rw-rw-rw-   0        0        0     5653 2023-06-14 05:56:16.000000 lm_datahandler-0.1.1/lm_datahandler/plots/sleep_staging_plot.py
-drwxrwxrwx   0        0        0        0 2023-06-14 05:56:25.896603 lm_datahandler-0.1.1/lm_datahandler/postprocess/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:28.000000 lm_datahandler-0.1.1/lm_datahandler/postprocess/__init__.py
--rw-rw-rw-   0        0        0     2358 2023-06-02 05:40:05.000000 lm_datahandler-0.1.1/lm_datahandler/postprocess/label_smooth.py
-drwxrwxrwx   0        0        0        0 2023-06-14 05:56:25.898194 lm_datahandler-0.1.1/lm_datahandler/preprocess/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:46.000000 lm_datahandler-0.1.1/lm_datahandler/preprocess/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-31 10:45:45.000000 lm_datahandler-0.1.1/lm_datahandler/preprocess/filter.py
--rw-rw-rw-   0        0        0        0 2023-05-31 10:48:56.000000 lm_datahandler-0.1.1/lm_datahandler/preprocess/tailor.py
-drwxrwxrwx   0        0        0        0 2023-06-14 05:56:25.898566 lm_datahandler-0.1.1/lm_datahandler/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:57.000000 lm_datahandler-0.1.1/lm_datahandler/utils/__init__.py
--rw-rw-rw-   0        0        0     1734 2023-04-20 07:01:30.000000 lm_datahandler-0.1.1/lm_datahandler/utils/numba_func.py
-drwxrwxrwx   0        0        0        0 2023-06-14 05:56:25.890910 lm_datahandler-0.1.1/lm_datahandler.egg-info/
--rw-rw-rw-   0        0        0      325 2023-06-14 05:56:25.000000 lm_datahandler-0.1.1/lm_datahandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1043 2023-06-14 05:56:25.000000 lm_datahandler-0.1.1/lm_datahandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 05:56:25.000000 lm_datahandler-0.1.1/lm_datahandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      179 2023-06-14 05:56:25.000000 lm_datahandler-0.1.1/lm_datahandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-14 05:56:25.000000 lm_datahandler-0.1.1/lm_datahandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 05:56:25.900107 lm_datahandler-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      987 2023-06-14 05:56:16.000000 lm_datahandler-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:12:24.725894 lm_datahandler-0.1.2/
+-rw-rw-rw-   0        0        0     1104 2023-06-14 03:54:04.000000 lm_datahandler-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       45 2023-06-14 10:58:27.000000 lm_datahandler-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      325 2023-06-14 11:12:24.724879 lm_datahandler-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 11:12:24.702223 lm_datahandler-0.1.2/lm_datahandler/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:11:31.000000 lm_datahandler-0.1.2/lm_datahandler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:12:24.717499 lm_datahandler-0.1.2/lm_datahandler/data_load/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:11:51.000000 lm_datahandler-0.1.2/lm_datahandler/data_load/__init__.py
+-rw-rw-rw-   0        0        0     1674 2023-06-13 02:30:00.000000 lm_datahandler-0.1.2/lm_datahandler/data_load/data_loader.py
+-rw-rw-rw-   0        0        0    10521 2023-06-13 02:44:38.000000 lm_datahandler-0.1.2/lm_datahandler/data_load/loaders.py
+-rw-rw-rw-   0        0        0    24343 2023-06-14 03:57:25.000000 lm_datahandler-0.1.2/lm_datahandler/datahandler.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:12:24.720114 lm_datahandler-0.1.2/lm_datahandler/functions/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:02.000000 lm_datahandler-0.1.2/lm_datahandler/functions/__init__.py
+-rw-rw-rw-   0        0        0    31179 2023-06-14 03:24:58.000000 lm_datahandler-0.1.2/lm_datahandler/functions/biomarker.py
+-rw-rw-rw-   0        0        0    14569 2023-06-02 03:05:39.000000 lm_datahandler-0.1.2/lm_datahandler/functions/feature_extract.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:12:04.000000 lm_datahandler-0.1.2/lm_datahandler/functions/os_detect.py
+-rw-rw-rw-   0        0        0     1392 2023-06-14 10:53:42.000000 lm_datahandler-0.1.2/lm_datahandler/functions/sleep_staging.py
+-rw-rw-rw-   0        0        0     3240 2023-06-14 03:25:28.000000 lm_datahandler-0.1.2/lm_datahandler/functions/sleep_variable_compute.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:11:57.000000 lm_datahandler-0.1.2/lm_datahandler/functions/spindle_detect.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:12:24.721127 lm_datahandler-0.1.2/lm_datahandler/models/
+-rw-rw-rw-   0        0        0   376172 2023-05-30 01:59:36.000000 lm_datahandler-0.1.2/lm_datahandler/models/wholenight_sleep_staging.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 11:12:24.722157 lm_datahandler-0.1.2/lm_datahandler/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:16.000000 lm_datahandler-0.1.2/lm_datahandler/plots/__init__.py
+-rw-rw-rw-   0        0        0      625 2023-06-07 08:43:30.000000 lm_datahandler-0.1.2/lm_datahandler/plots/biomarker_plot.py
+-rw-rw-rw-   0        0        0     5653 2023-06-14 05:56:16.000000 lm_datahandler-0.1.2/lm_datahandler/plots/sleep_staging_plot.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:12:24.723145 lm_datahandler-0.1.2/lm_datahandler/postprocess/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:28.000000 lm_datahandler-0.1.2/lm_datahandler/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     2358 2023-06-02 05:40:05.000000 lm_datahandler-0.1.2/lm_datahandler/postprocess/label_smooth.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:12:24.724094 lm_datahandler-0.1.2/lm_datahandler/preprocess/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:46.000000 lm_datahandler-0.1.2/lm_datahandler/preprocess/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 10:45:45.000000 lm_datahandler-0.1.2/lm_datahandler/preprocess/filter.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 10:48:56.000000 lm_datahandler-0.1.2/lm_datahandler/preprocess/tailor.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:12:24.724879 lm_datahandler-0.1.2/lm_datahandler/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:57.000000 lm_datahandler-0.1.2/lm_datahandler/utils/__init__.py
+-rw-rw-rw-   0        0        0     1734 2023-04-20 07:01:30.000000 lm_datahandler-0.1.2/lm_datahandler/utils/numba_func.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:12:24.716178 lm_datahandler-0.1.2/lm_datahandler.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-06-14 11:12:24.000000 lm_datahandler-0.1.2/lm_datahandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1106 2023-06-14 11:12:24.000000 lm_datahandler-0.1.2/lm_datahandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 11:12:24.000000 lm_datahandler-0.1.2/lm_datahandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      179 2023-06-14 11:12:24.000000 lm_datahandler-0.1.2/lm_datahandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-14 11:12:24.000000 lm_datahandler-0.1.2/lm_datahandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 11:12:24.725894 lm_datahandler-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-06-14 11:12:14.000000 lm_datahandler-0.1.2/setup.py
```

### Comparing `lm_datahandler-0.1.1/LICENSE` & `lm_datahandler-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.1/lm_datahandler/data_load/data_loader.py` & `lm_datahandler-0.1.2/lm_datahandler/data_load/data_loader.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.1/lm_datahandler/data_load/loaders.py` & `lm_datahandler-0.1.2/lm_datahandler/data_load/loaders.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.1/lm_datahandler/datahandler.py` & `lm_datahandler-0.1.2/lm_datahandler/datahandler.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.1/lm_datahandler/functions/biomarker.py` & `lm_datahandler-0.1.2/lm_datahandler/functions/biomarker.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.1/lm_datahandler/functions/feature_extract.py` & `lm_datahandler-0.1.2/lm_datahandler/functions/feature_extract.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.1/lm_datahandler/functions/sleep_staging.py` & `lm_datahandler-0.1.2/lm_datahandler/functions/sleep_staging.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.1/lm_datahandler/functions/sleep_variable_compute.py` & `lm_datahandler-0.1.2/lm_datahandler/functions/sleep_variable_compute.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.1/lm_datahandler/plots/biomarker_plot.py` & `lm_datahandler-0.1.2/lm_datahandler/plots/biomarker_plot.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.1/lm_datahandler/plots/sleep_staging_plot.py` & `lm_datahandler-0.1.2/lm_datahandler/plots/sleep_staging_plot.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.1/lm_datahandler/postprocess/label_smooth.py` & `lm_datahandler-0.1.2/lm_datahandler/postprocess/label_smooth.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.1/lm_datahandler/utils/numba_func.py` & `lm_datahandler-0.1.2/lm_datahandler/utils/numba_func.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.1/lm_datahandler.egg-info/SOURCES.txt` & `lm_datahandler-0.1.2/lm_datahandler.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 setup.py
 lm_datahandler/__init__.py
 lm_datahandler/datahandler.py
 lm_datahandler.egg-info/PKG-INFO
 lm_datahandler.egg-info/SOURCES.txt
 lm_datahandler.egg-info/dependency_links.txt
 lm_datahandler.egg-info/requires.txt
@@ -13,14 +14,15 @@
 lm_datahandler/functions/__init__.py
 lm_datahandler/functions/biomarker.py
 lm_datahandler/functions/feature_extract.py
 lm_datahandler/functions/os_detect.py
 lm_datahandler/functions/sleep_staging.py
 lm_datahandler/functions/sleep_variable_compute.py
 lm_datahandler/functions/spindle_detect.py
+lm_datahandler/models/wholenight_sleep_staging.txt
 lm_datahandler/plots/__init__.py
 lm_datahandler/plots/biomarker_plot.py
 lm_datahandler/plots/sleep_staging_plot.py
 lm_datahandler/postprocess/__init__.py
 lm_datahandler/postprocess/label_smooth.py
 lm_datahandler/preprocess/__init__.py
 lm_datahandler/preprocess/filter.py
```

### Comparing `lm_datahandler-0.1.1/setup.py` & `lm_datahandler-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'lm_datahandler',
-    version = '0.1.1',
+    version = '0.1.2',
     keywords='eeg sleep staging analysis',
     description = 'a python analyse tool for LM Data Recorder data',
     license = 'MIT License',
     url = 'https://github.com/zx950618/lm_datahandler',
     author = 'Eric Zheng',
     author_email = '1248471980@qq.com',
     packages = find_packages(),
```

