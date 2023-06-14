# Comparing `tmp/rowing-0.2.5.tar.gz` & `tmp/rowing-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rowing-0.2.5.tar", last modified: Thu May 26 10:36:35 2022, max compression
+gzip compressed data, was "rowing-0.3.0.tar", last modified: Wed Jun 14 19:09:20 2023, max compression
```

## Comparing `rowing-0.2.5.tar` & `rowing-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-26 10:36:35.398572 rowing-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (116)     1079 2022-05-26 10:36:25.000000 rowing-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     9142 2022-05-26 10:36:35.398572 rowing-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     8710 2022-05-26 10:36:25.000000 rowing-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-26 10:36:35.398572 rowing-0.2.5/rowing/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-05-26 10:36:25.000000 rowing-0.2.5/rowing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5814 2022-05-26 10:36:25.000000 rowing-0.2.5/rowing/_compat.py
--rw-r--r--   0 runner    (1001) docker     (116)     6051 2022-05-26 10:36:25.000000 rowing-0.2.5/rowing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-26 10:36:35.398572 rowing-0.2.5/rowing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     9142 2022-05-26 10:36:34.000000 rowing-0.2.5/rowing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      261 2022-05-26 10:36:35.000000 rowing-0.2.5/rowing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-26 10:36:34.000000 rowing-0.2.5/rowing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      215 2022-05-26 10:36:35.000000 rowing-0.2.5/rowing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      241 2022-05-26 10:36:35.000000 rowing-0.2.5/rowing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2022-05-26 10:36:35.000000 rowing-0.2.5/rowing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-05-26 10:36:35.398572 rowing-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1606 2022-05-26 10:36:25.000000 rowing-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:09:20.852481 rowing-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-14 19:09:11.000000 rowing-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-14 19:09:20.852481 rowing-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-06-14 19:09:11.000000 rowing-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:09:20.852481 rowing-0.3.0/rowing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:09:11.000000 rowing-0.3.0/rowing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-14 19:09:11.000000 rowing-0.3.0/rowing/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-06-14 19:09:11.000000 rowing-0.3.0/rowing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:09:20.852481 rowing-0.3.0/rowing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-14 19:09:20.000000 rowing-0.3.0/rowing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-14 19:09:20.000000 rowing-0.3.0/rowing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:09:20.000000 rowing-0.3.0/rowing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 19:09:20.000000 rowing-0.3.0/rowing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-14 19:09:20.000000 rowing-0.3.0/rowing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 19:09:20.000000 rowing-0.3.0/rowing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 19:09:20.852481 rowing-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-14 19:09:11.000000 rowing-0.3.0/setup.py
```

### Comparing `rowing-0.2.5/LICENSE` & `rowing-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rowing-0.2.5/rowing/_compat.py` & `rowing-0.3.0/rowing/_compat.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -160,8 +160,8 @@
     def __get__(self, obj, cls):
         with self.lock:
             return super(threaded_cached_property_with_ttl, self).__get__(obj, cls)
 
 
 # Alias to make threaded_cached_property_with_ttl easier to use
 threaded_cached_property_ttl = threaded_cached_property_with_ttl
-timed_threaded_cached_property = threaded_cached_property_with_ttl
+timed_threaded_cached_property = threaded_cached_property_with_ttl
```

### Comparing `rowing-0.2.5/setup.py` & `rowing-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,52 +3,52 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='rowing',
-    version='0.2.5',
+    version='0.3.0',
     description='Library for loading and presenting data from the worldrowing.com',
     author='Matthew Griffiths',
     author_email='matthewghgriffiths@gmail.com',
     url='https://github.com/matthewghgriffiths/rowing',
     packages=['rowing'],
     entry_points={
         'console_scripts': [
-            'world_rowing = rowing.world_rowing.cli:run [CLI]', 
-            'rowing_live_tracker = rowing.world_rowing.dashboard:main [CLI]', 
+            'worldrowing = rowing.worldrowing.app:main [WORLDROWING]',
             'garmin = rowing.analysis.garmin:main [GARMIN]',
             'gpx = rowing.analysis.files:main [GPX]',
         ]
     },
-    license='MIT', 
-    long_description=long_description, 
+    license='MIT',
+    long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         'numpy>=1.21.0',
         'scipy>=1.7.0',
         'pandas>=1.3.0',
-        'matplotlib>=3.0.0',
+        'matplotlib>=3.5.1',
         'tqdm>=4.0.0',
     ],
     extras_require={
-        'CLI': ['cmd2>=2.0.0', 'pyqt5>=5.0.0'],
-        'REQ': ['requests>=2.0.0'], # Requests is not required if using pyodide
+        'WORLDROWING': ['streamlit>=1.22.0', 'plotly>=5.14.1'],
+        # Requests is not required if using pyodide
+        'REQ': ['requests>=2.27.1'],
         'GARMIN': [
-            'garminconnect>=0.1.45', 
-            'fitparse>=1.2.0', 
+            'garminconnect>=0.1.45',
+            'fitparse>=1.2.0',
             "openpyxl>=3.0.0",
             "pyarrow>=7.0.0"
         ],
         "GPX": ['gpxpy>=1.5.0', 'fitparse>=1.2.0'],
     },
     python_requires=">=3.8",
     package_data={
         'rowing': [
-            'data/*.csv.gz', 
-            'data/iso_country.json', 
-            'data/flags/*.png', 
+            'data/*.csv.gz',
+            'data/iso_country.json',
+            'data/flags/*.png',
             'data/*.tsv'
         ],
     }
 )
```

