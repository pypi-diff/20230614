# Comparing `tmp/visualize-algos-0.0.1.tar.gz` & `tmp/visualize-algos-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visualize-algos-0.0.1.tar", last modified: Mon Jun 12 17:49:11 2023, max compression
+gzip compressed data, was "visualize-algos-0.0.3.tar", last modified: Wed Jun 14 03:17:50 2023, max compression
```

## Comparing `visualize-algos-0.0.1.tar` & `visualize-algos-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 dhvanik   (1001) dhvanik   (1002)        0 2023-06-12 17:49:11.503783 visualize-algos-0.0.1/
--rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)      523 2023-06-12 17:49:11.499782 visualize-algos-0.0.1/PKG-INFO
--rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)       38 2023-06-12 17:49:11.503783 visualize-algos-0.0.1/setup.cfg
--rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)      678 2023-06-12 17:48:57.000000 visualize-algos-0.0.1/setup.py
-drwxrwxr-x   0 dhvanik   (1001) dhvanik   (1002)        0 2023-06-12 17:49:11.495781 visualize-algos-0.0.1/visualize_algos/
--rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)       28 2023-06-12 16:31:17.000000 visualize-algos-0.0.1/visualize_algos/__init__.py
--rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)     5785 2023-06-12 16:35:55.000000 visualize-algos-0.0.1/visualize_algos/path_finding_algos.py
--rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)     3615 2023-06-12 16:37:10.000000 visualize-algos-0.0.1/visualize_algos/ui_based_path_search.py
-drwxrwxr-x   0 dhvanik   (1001) dhvanik   (1002)        0 2023-06-12 17:49:11.499782 visualize-algos-0.0.1/visualize_algos.egg-info/
--rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)      523 2023-06-12 17:49:11.000000 visualize-algos-0.0.1/visualize_algos.egg-info/PKG-INFO
--rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)      270 2023-06-12 17:49:11.000000 visualize-algos-0.0.1/visualize_algos.egg-info/SOURCES.txt
--rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)        1 2023-06-12 17:49:11.000000 visualize-algos-0.0.1/visualize_algos.egg-info/dependency_links.txt
--rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)       16 2023-06-12 17:49:11.000000 visualize-algos-0.0.1/visualize_algos.egg-info/top_level.txt
+drwxrwxr-x   0 dhvanik   (1001) dhvanik   (1002)        0 2023-06-14 03:17:50.180742 visualize-algos-0.0.3/
+-rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)      608 2023-06-14 03:17:50.180742 visualize-algos-0.0.3/PKG-INFO
+-rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)       38 2023-06-14 03:17:50.180742 visualize-algos-0.0.3/setup.cfg
+-rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)      763 2023-06-14 03:17:43.000000 visualize-algos-0.0.3/setup.py
+drwxrwxr-x   0 dhvanik   (1001) dhvanik   (1002)        0 2023-06-14 03:17:50.176742 visualize-algos-0.0.3/visualize_algos/
+-rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)       36 2023-06-14 03:12:35.000000 visualize-algos-0.0.3/visualize_algos/__init__.py
+-rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)     5785 2023-06-12 16:35:55.000000 visualize-algos-0.0.3/visualize_algos/path_finding_algos.py
+-rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)     3615 2023-06-12 16:37:10.000000 visualize-algos-0.0.3/visualize_algos/ui_based_path_search.py
+drwxrwxr-x   0 dhvanik   (1001) dhvanik   (1002)        0 2023-06-14 03:17:50.176742 visualize-algos-0.0.3/visualize_algos.egg-info/
+-rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)      608 2023-06-14 03:17:50.000000 visualize-algos-0.0.3/visualize_algos.egg-info/PKG-INFO
+-rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)      270 2023-06-14 03:17:50.000000 visualize-algos-0.0.3/visualize_algos.egg-info/SOURCES.txt
+-rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)        1 2023-06-14 03:17:50.000000 visualize-algos-0.0.3/visualize_algos.egg-info/dependency_links.txt
+-rw-rw-r--   0 dhvanik   (1001) dhvanik   (1002)       16 2023-06-14 03:17:50.000000 visualize-algos-0.0.3/visualize_algos.egg-info/top_level.txt
```

### Comparing `visualize-algos-0.0.1/PKG-INFO` & `visualize-algos-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: visualize-algos
-Version: 0.0.1
+Version: 0.0.3
 Summary: Visualize path finding algorithms simultaneously for the same condition in UI.
+Home-page: https://github.com/Dhvanik-Viradiya/Path-finding-algorithm-visuallization
 Author: Dhvanik Viradiya
 Author-email: viradiyadhvanik@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `visualize-algos-0.0.1/setup.py` & `visualize-algos-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import setuptools
 
 setuptools.setup(
     name="visualize-algos",
-    version="0.0.1",
+    version="0.0.3",
     author="Dhvanik Viradiya",
     author_email="viradiyadhvanik@gmail.com",
     description="Visualize path finding algorithms simultaneously for the same condition in UI.",
     long_description="There are only limited algorithms implemented. In follow up versions more algorithms will be added and will be used to visualize the algorithms easily.",
     long_description_content_type="text/markdown",
+    url="https://github.com/Dhvanik-Viradiya/Path-finding-algorithm-visuallization",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
     python_requires=">=3.6",
 )
```

### Comparing `visualize-algos-0.0.1/visualize_algos/path_finding_algos.py` & `visualize-algos-0.0.3/visualize_algos/path_finding_algos.py`

 * *Files identical despite different names*

### Comparing `visualize-algos-0.0.1/visualize_algos/ui_based_path_search.py` & `visualize-algos-0.0.3/visualize_algos/ui_based_path_search.py`

 * *Files identical despite different names*

### Comparing `visualize-algos-0.0.1/visualize_algos.egg-info/PKG-INFO` & `visualize-algos-0.0.3/visualize_algos.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: visualize-algos
-Version: 0.0.1
+Version: 0.0.3
 Summary: Visualize path finding algorithms simultaneously for the same condition in UI.
+Home-page: https://github.com/Dhvanik-Viradiya/Path-finding-algorithm-visuallization
 Author: Dhvanik Viradiya
 Author-email: viradiyadhvanik@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

