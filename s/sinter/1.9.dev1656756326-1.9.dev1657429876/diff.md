# Comparing `tmp/sinter-1.9.dev1656756326.tar.gz` & `tmp/sinter-1.9.dev1657429876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinter-1.9.dev1656756326.tar", last modified: Sat Jul  2 10:29:35 2022, max compression
+gzip compressed data, was "sinter-1.9.dev1657429876.tar", last modified: Sun Jul 10 05:33:54 2022, max compression
```

## Comparing `sinter-1.9.dev1656756326.tar` & `sinter-1.9.dev1657429876.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:35.662133 sinter-1.9.dev1656756326/
--rw-r--r--   0 runner     (501) staff       (20)    14154 2022-07-02 10:29:35.661648 sinter-1.9.dev1656756326/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    13845 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/README.md
--rw-r--r--   0 runner     (501) staff       (20)    91472 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/readme_example_plot.png
--rw-r--r--   0 runner     (501) staff       (20)      112 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/requirements.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2022-07-02 10:29:35.662250 sinter-1.9.dev1656756326/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1460 2022-07-02 10:07:06.000000 sinter-1.9.dev1656756326/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:35.637873 sinter-1.9.dev1656756326/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:35.657774 sinter-1.9.dev1656756326/src/sinter/
--rw-r--r--   0 runner     (501) staff       (20)      860 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      975 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/anon_task_stats.py
--rw-r--r--   0 runner     (501) staff       (20)    12098 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/collection.py
--rw-r--r--   0 runner     (501) staff       (20)     3426 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/collection_options.py
--rw-r--r--   0 runner     (501) staff       (20)     4177 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/collection_test.py
--rw-r--r--   0 runner     (501) staff       (20)     7879 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/collection_tracker_for_single_task.py
--rw-r--r--   0 runner     (501) staff       (20)     8983 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/collection_work_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1820 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/csv_out.py
--rw-r--r--   0 runner     (501) staff       (20)     8522 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/decoding.py
--rw-r--r--   0 runner     (501) staff       (20)     1155 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/decoding_internal.py
--rw-r--r--   0 runner     (501) staff       (20)     6573 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/decoding_pymatching.py
--rw-r--r--   0 runner     (501) staff       (20)     5693 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/decoding_test.py
--rw-r--r--   0 runner     (501) staff       (20)     2718 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/existing_data.py
--rw-r--r--   0 runner     (501) staff       (20)      117 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/json_type.py
--rw-r--r--   0 runner     (501) staff       (20)     1311 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/main.py
--rw-r--r--   0 runner     (501) staff       (20)     8819 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/main_collect.py
--rw-r--r--   0 runner     (501) staff       (20)      475 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/main_combine.py
--rw-r--r--   0 runner     (501) staff       (20)    10726 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/main_plot.py
--rw-r--r--   0 runner     (501) staff       (20)     3314 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/main_predict.py
--rw-r--r--   0 runner     (501) staff       (20)     8043 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/main_test.py
--rw-r--r--   0 runner     (501) staff       (20)     9953 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/plotting.py
--rw-r--r--   0 runner     (501) staff       (20)     2612 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/plotting_test.py
--rw-r--r--   0 runner     (501) staff       (20)    10399 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/predict.py
--rw-r--r--   0 runner     (501) staff       (20)     3918 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/predict_test.py
--rw-r--r--   0 runner     (501) staff       (20)     1921 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/printer.py
--rw-r--r--   0 runner     (501) staff       (20)    13781 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/probability_util.py
--rw-r--r--   0 runner     (501) staff       (20)     7729 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/probability_util_test.py
--rw-r--r--   0 runner     (501) staff       (20)     6956 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/task.py
--rw-r--r--   0 runner     (501) staff       (20)     1545 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/task_stats.py
--rw-r--r--   0 runner     (501) staff       (20)     4148 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/worker.py
--rw-r--r--   0 runner     (501) staff       (20)     2254 2022-07-02 10:07:05.000000 sinter-1.9.dev1656756326/src/sinter/worker_test.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:35.661036 sinter-1.9.dev1656756326/src/sinter.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)    14154 2022-07-02 10:29:35.000000 sinter-1.9.dev1656756326/src/sinter.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1112 2022-07-02 10:29:35.000000 sinter-1.9.dev1656756326/src/sinter.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-07-02 10:29:35.000000 sinter-1.9.dev1656756326/src/sinter.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       45 2022-07-02 10:29:35.000000 sinter-1.9.dev1656756326/src/sinter.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)       56 2022-07-02 10:29:35.000000 sinter-1.9.dev1656756326/src/sinter.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        7 2022-07-02 10:29:35.000000 sinter-1.9.dev1656756326/src/sinter.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:54.856423 sinter-1.9.dev1657429876/
+-rw-r--r--   0 runner     (501) staff       (20)    14154 2022-07-10 05:33:54.855917 sinter-1.9.dev1657429876/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    13845 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/README.md
+-rw-r--r--   0 runner     (501) staff       (20)    91472 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/readme_example_plot.png
+-rw-r--r--   0 runner     (501) staff       (20)      112 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/requirements.txt
+-rw-r--r--   0 runner     (501) staff       (20)       38 2022-07-10 05:33:54.856537 sinter-1.9.dev1657429876/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1460 2022-07-10 05:11:44.000000 sinter-1.9.dev1657429876/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:54.787124 sinter-1.9.dev1657429876/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:54.852228 sinter-1.9.dev1657429876/src/sinter/
+-rw-r--r--   0 runner     (501) staff       (20)      860 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      975 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/anon_task_stats.py
+-rw-r--r--   0 runner     (501) staff       (20)    12098 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/collection.py
+-rw-r--r--   0 runner     (501) staff       (20)     3426 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/collection_options.py
+-rw-r--r--   0 runner     (501) staff       (20)     4177 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/collection_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     7879 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/collection_tracker_for_single_task.py
+-rw-r--r--   0 runner     (501) staff       (20)     8983 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/collection_work_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1820 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/csv_out.py
+-rw-r--r--   0 runner     (501) staff       (20)     8522 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/decoding.py
+-rw-r--r--   0 runner     (501) staff       (20)     1155 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/decoding_internal.py
+-rw-r--r--   0 runner     (501) staff       (20)     6573 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/decoding_pymatching.py
+-rw-r--r--   0 runner     (501) staff       (20)     5693 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/decoding_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     2718 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/existing_data.py
+-rw-r--r--   0 runner     (501) staff       (20)      117 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/json_type.py
+-rw-r--r--   0 runner     (501) staff       (20)     1311 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/main.py
+-rw-r--r--   0 runner     (501) staff       (20)     8819 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/main_collect.py
+-rw-r--r--   0 runner     (501) staff       (20)      475 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/main_combine.py
+-rw-r--r--   0 runner     (501) staff       (20)    10726 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/main_plot.py
+-rw-r--r--   0 runner     (501) staff       (20)     3314 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/main_predict.py
+-rw-r--r--   0 runner     (501) staff       (20)     8043 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/main_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     9979 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/plotting.py
+-rw-r--r--   0 runner     (501) staff       (20)     2612 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/plotting_test.py
+-rw-r--r--   0 runner     (501) staff       (20)    10399 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/predict.py
+-rw-r--r--   0 runner     (501) staff       (20)     3918 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/predict_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     1921 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/printer.py
+-rw-r--r--   0 runner     (501) staff       (20)    13781 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/probability_util.py
+-rw-r--r--   0 runner     (501) staff       (20)     7729 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/probability_util_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     6956 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/task.py
+-rw-r--r--   0 runner     (501) staff       (20)     1545 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/task_stats.py
+-rw-r--r--   0 runner     (501) staff       (20)     4148 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     2254 2022-07-10 05:11:43.000000 sinter-1.9.dev1657429876/src/sinter/worker_test.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:54.855286 sinter-1.9.dev1657429876/src/sinter.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    14154 2022-07-10 05:33:54.000000 sinter-1.9.dev1657429876/src/sinter.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1112 2022-07-10 05:33:54.000000 sinter-1.9.dev1657429876/src/sinter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-07-10 05:33:54.000000 sinter-1.9.dev1657429876/src/sinter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       45 2022-07-10 05:33:54.000000 sinter-1.9.dev1657429876/src/sinter.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)       56 2022-07-10 05:33:54.000000 sinter-1.9.dev1657429876/src/sinter.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        7 2022-07-10 05:33:54.000000 sinter-1.9.dev1657429876/src/sinter.egg-info/top_level.txt
```

### Comparing `sinter-1.9.dev1656756326/PKG-INFO` & `sinter-1.9.dev1657429876/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinter
-Version: 1.9.dev1656756326
+Version: 1.9.dev1657429876
 Summary: Samples stim circuits and decodes them using pymatching.
 Home-page: UNKNOWN
 Author: Craig Gidney
 Author-email: craig.gidney@gmail.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.7.0
```

### Comparing `sinter-1.9.dev1656756326/README.md` & `sinter-1.9.dev1657429876/README.md`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/readme_example_plot.png` & `sinter-1.9.dev1657429876/readme_example_plot.png`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/setup.py` & `sinter-1.9.dev1657429876/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup
 
 with open('README.md', encoding='UTF-8') as f:
     long_description = f.read()
 with open('requirements.txt', encoding='UTF-8') as f:
     requirements = [line.split()[0] for line in f.read().splitlines()]
 
-version = '1.9.dev1656756326'
+version = '1.9.dev1657429876'
 
 setup(
     name='sinter',
     version=version,
     author='Craig Gidney',
     author_email='craig.gidney@gmail.com',
     license='Apache 2',
```

### Comparing `sinter-1.9.dev1656756326/src/sinter/__init__.py` & `sinter-1.9.dev1657429876/src/sinter/__init__.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/anon_task_stats.py` & `sinter-1.9.dev1657429876/src/sinter/anon_task_stats.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/collection.py` & `sinter-1.9.dev1657429876/src/sinter/collection.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/collection_options.py` & `sinter-1.9.dev1657429876/src/sinter/collection_options.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/collection_test.py` & `sinter-1.9.dev1657429876/src/sinter/collection_test.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/collection_tracker_for_single_task.py` & `sinter-1.9.dev1657429876/src/sinter/collection_tracker_for_single_task.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/collection_work_manager.py` & `sinter-1.9.dev1657429876/src/sinter/collection_work_manager.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/csv_out.py` & `sinter-1.9.dev1657429876/src/sinter/csv_out.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/decoding.py` & `sinter-1.9.dev1657429876/src/sinter/decoding.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/decoding_internal.py` & `sinter-1.9.dev1657429876/src/sinter/decoding_internal.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/decoding_pymatching.py` & `sinter-1.9.dev1657429876/src/sinter/decoding_pymatching.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/decoding_test.py` & `sinter-1.9.dev1657429876/src/sinter/decoding_test.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/existing_data.py` & `sinter-1.9.dev1657429876/src/sinter/existing_data.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/main.py` & `sinter-1.9.dev1657429876/src/sinter/main.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/main_collect.py` & `sinter-1.9.dev1657429876/src/sinter/main_collect.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/main_plot.py` & `sinter-1.9.dev1657429876/src/sinter/main_plot.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/main_predict.py` & `sinter-1.9.dev1657429876/src/sinter/main_predict.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/main_test.py` & `sinter-1.9.dev1657429876/src/sinter/main_test.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/plotting.py` & `sinter-1.9.dev1657429876/src/sinter/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         key: Items that produce the same value from this function get grouped together.
 
     Returns:
         A dictionary mapping outputs that were produced by the grouping function to
         the list of items that produced that output.
 
     Examples:
+        >>> import sinter
         >>> sinter.group_by([1, 2, 3], key=lambda i: i == 2)
         {False: [1, 3], True: [2]}
 
         >>> sinter.group_by(range(10), key=lambda i: i % 3)
         {0: [0, 3, 6, 9], 1: [1, 4, 7], 2: [2, 5, 8]}
     """
```

### Comparing `sinter-1.9.dev1656756326/src/sinter/plotting_test.py` & `sinter-1.9.dev1657429876/src/sinter/plotting_test.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/predict.py` & `sinter-1.9.dev1657429876/src/sinter/predict.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/predict_test.py` & `sinter-1.9.dev1657429876/src/sinter/predict_test.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/printer.py` & `sinter-1.9.dev1657429876/src/sinter/printer.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/probability_util.py` & `sinter-1.9.dev1657429876/src/sinter/probability_util.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/probability_util_test.py` & `sinter-1.9.dev1657429876/src/sinter/probability_util_test.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/task.py` & `sinter-1.9.dev1657429876/src/sinter/task.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/task_stats.py` & `sinter-1.9.dev1657429876/src/sinter/task_stats.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/worker.py` & `sinter-1.9.dev1657429876/src/sinter/worker.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter/worker_test.py` & `sinter-1.9.dev1657429876/src/sinter/worker_test.py`

 * *Files identical despite different names*

### Comparing `sinter-1.9.dev1656756326/src/sinter.egg-info/PKG-INFO` & `sinter-1.9.dev1657429876/src/sinter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinter
-Version: 1.9.dev1656756326
+Version: 1.9.dev1657429876
 Summary: Samples stim circuits and decodes them using pymatching.
 Home-page: UNKNOWN
 Author: Craig Gidney
 Author-email: craig.gidney@gmail.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.7.0
```

### Comparing `sinter-1.9.dev1656756326/src/sinter.egg-info/SOURCES.txt` & `sinter-1.9.dev1657429876/src/sinter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

