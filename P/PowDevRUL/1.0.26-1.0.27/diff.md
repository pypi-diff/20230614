# Comparing `tmp/PowDevRUL-1.0.26.tar.gz` & `tmp/PowDevRUL-1.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PowDevRUL-1.0.26.tar", last modified: Wed Jun 14 12:25:27 2023, max compression
+gzip compressed data, was "PowDevRUL-1.0.27.tar", last modified: Wed Jun 14 13:57:20 2023, max compression
```

## Comparing `PowDevRUL-1.0.26.tar` & `PowDevRUL-1.0.27.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-14 12:25:27.288422 PowDevRUL-1.0.26/
--rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-14 09:57:38.000000 PowDevRUL-1.0.26/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      599 2023-06-14 12:25:27.288422 PowDevRUL-1.0.26/PKG-INFO
--rw-------   0 runner    (1000) runner    (1000)     3277 2023-06-14 12:13:02.000000 PowDevRUL-1.0.26/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      452 2023-06-14 09:54:45.000000 PowDevRUL-1.0.26/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-14 12:25:27.288422 PowDevRUL-1.0.26/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      979 2023-06-14 09:54:48.000000 PowDevRUL-1.0.26/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-14 12:25:27.276422 PowDevRUL-1.0.26/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-14 12:25:27.284422 PowDevRUL-1.0.26/src/PowDevRUL.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      599 2023-06-14 12:25:27.000000 PowDevRUL-1.0.26/src/PowDevRUL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      681 2023-06-14 12:25:27.000000 PowDevRUL-1.0.26/src/PowDevRUL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-14 12:25:27.000000 PowDevRUL-1.0.26/src/PowDevRUL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       92 2023-06-14 12:25:27.000000 PowDevRUL-1.0.26/src/PowDevRUL.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-06-14 12:25:27.000000 PowDevRUL-1.0.26/src/PowDevRUL.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-14 12:25:27.284422 PowDevRUL-1.0.26/src/powdevrul/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-06-14 09:54:13.000000 PowDevRUL-1.0.26/src/powdevrul/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-14 12:25:27.288422 PowDevRUL-1.0.26/src/powdevrul/function/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-06-14 09:54:13.000000 PowDevRUL-1.0.26/src/powdevrul/function/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-14 09:54:13.000000 PowDevRUL-1.0.26/src/powdevrul/function/counters.py
--rw-------   0 runner    (1000) runner    (1000)     2297 2023-06-14 09:54:13.000000 PowDevRUL-1.0.26/src/powdevrul/function/cumul_endommagement.py
--rw-------   0 runner    (1000) runner    (1000)     3279 2023-06-14 09:54:13.000000 PowDevRUL-1.0.26/src/powdevrul/function/graphs.py
--rw-------   0 runner    (1000) runner    (1000)     3175 2023-06-14 09:54:13.000000 PowDevRUL-1.0.26/src/powdevrul/function/losses.py
--rw-------   0 runner    (1000) runner    (1000)      350 2023-06-14 09:54:13.000000 PowDevRUL-1.0.26/src/powdevrul/function/materials.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2782 2023-06-14 09:54:13.000000 PowDevRUL-1.0.26/src/powdevrul/function/matrix.py
--rw-------   0 runner    (1000) runner    (1000)      430 2023-06-14 09:54:13.000000 PowDevRUL-1.0.26/src/powdevrul/function/path_reader.py
--rw-------   0 runner    (1000) runner    (1000)     1115 2023-06-14 09:54:13.000000 PowDevRUL-1.0.26/src/powdevrul/function/poly_somme.py
--rw-------   0 runner    (1000) runner    (1000)     2077 2023-06-14 12:09:29.000000 PowDevRUL-1.0.26/src/powdevrul/function/temperature.py
--rw-------   0 runner    (1000) runner    (1000)     3782 2023-06-14 12:09:28.000000 PowDevRUL-1.0.26/src/powdevrul/function/zth_materials.py
--rw-------   0 runner    (1000) runner    (1000)     3245 2023-06-14 09:54:13.000000 PowDevRUL-1.0.26/src/powdevrul/lifetime.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-14 13:57:20.630552 PowDevRUL-1.0.27/
+-rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-14 09:57:38.000000 PowDevRUL-1.0.27/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      693 2023-06-14 13:57:20.630552 PowDevRUL-1.0.27/PKG-INFO
+-rw-------   0 runner    (1000) runner    (1000)     3277 2023-06-14 12:13:02.000000 PowDevRUL-1.0.27/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      452 2023-06-14 13:57:19.000000 PowDevRUL-1.0.27/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-14 13:57:20.634553 PowDevRUL-1.0.27/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)     1073 2023-06-14 13:57:13.000000 PowDevRUL-1.0.27/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-14 13:57:20.626552 PowDevRUL-1.0.27/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-14 13:57:20.626552 PowDevRUL-1.0.27/src/PowDevRUL.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      693 2023-06-14 13:57:20.000000 PowDevRUL-1.0.27/src/PowDevRUL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      681 2023-06-14 13:57:20.000000 PowDevRUL-1.0.27/src/PowDevRUL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-14 13:57:20.000000 PowDevRUL-1.0.27/src/PowDevRUL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       92 2023-06-14 13:57:20.000000 PowDevRUL-1.0.27/src/PowDevRUL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-06-14 13:57:20.000000 PowDevRUL-1.0.27/src/PowDevRUL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-14 13:57:20.626552 PowDevRUL-1.0.27/src/powdevrul/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-06-14 09:54:13.000000 PowDevRUL-1.0.27/src/powdevrul/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-14 13:57:20.630552 PowDevRUL-1.0.27/src/powdevrul/function/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-06-14 09:54:13.000000 PowDevRUL-1.0.27/src/powdevrul/function/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-14 09:54:13.000000 PowDevRUL-1.0.27/src/powdevrul/function/counters.py
+-rw-------   0 runner    (1000) runner    (1000)     2297 2023-06-14 09:54:13.000000 PowDevRUL-1.0.27/src/powdevrul/function/cumul_endommagement.py
+-rw-------   0 runner    (1000) runner    (1000)     3279 2023-06-14 09:54:13.000000 PowDevRUL-1.0.27/src/powdevrul/function/graphs.py
+-rw-------   0 runner    (1000) runner    (1000)     3175 2023-06-14 09:54:13.000000 PowDevRUL-1.0.27/src/powdevrul/function/losses.py
+-rw-------   0 runner    (1000) runner    (1000)      350 2023-06-14 09:54:13.000000 PowDevRUL-1.0.27/src/powdevrul/function/materials.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2782 2023-06-14 09:54:13.000000 PowDevRUL-1.0.27/src/powdevrul/function/matrix.py
+-rw-------   0 runner    (1000) runner    (1000)      430 2023-06-14 09:54:13.000000 PowDevRUL-1.0.27/src/powdevrul/function/path_reader.py
+-rw-------   0 runner    (1000) runner    (1000)     1115 2023-06-14 09:54:13.000000 PowDevRUL-1.0.27/src/powdevrul/function/poly_somme.py
+-rw-------   0 runner    (1000) runner    (1000)     2077 2023-06-14 12:09:29.000000 PowDevRUL-1.0.27/src/powdevrul/function/temperature.py
+-rw-------   0 runner    (1000) runner    (1000)     3782 2023-06-14 12:09:28.000000 PowDevRUL-1.0.27/src/powdevrul/function/zth_materials.py
+-rw-------   0 runner    (1000) runner    (1000)     3245 2023-06-14 09:54:13.000000 PowDevRUL-1.0.27/src/powdevrul/lifetime.py
```

### Comparing `PowDevRUL-1.0.26/LICENSE` & `PowDevRUL-1.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `PowDevRUL-1.0.26/README.md` & `PowDevRUL-1.0.27/README.md`

 * *Files identical despite different names*

### Comparing `PowDevRUL-1.0.26/setup.py` & `PowDevRUL-1.0.27/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='PowDevRUL',
-    version='1.0.26',
-    description ='The project aims to assess the lifetime and efficiency of electronic components by using thermal and electrical calculations based on data from an Excel file.',
+    version='1.0.27',
+    description ='The project aims to assess the lifetime and efficiency of electronic components by using thermal and electrical calculations based on data from an Excel file. Authors: Paul Garnier (paul.garnier@ens-rennes.fr), Briac Baudais (briac.baudais@ens-rennes.fr)',
     readme='README.md',
     license='MIT',
-    author='Garnier Paul , Baudais Briac',
-    author_email='paul.garnier@ens-rennes.fr , briac.baudais@ens-rennes.fr',
+    author='Garnier Paul, Baudais Briac',
+    author_email='paul.garnier@ens-rennes.fr, briac.baudais@ens-rennes.fr',
     url='https://github.com/PGarn/LifeTime',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     include_package_data=True,
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

### Comparing `PowDevRUL-1.0.26/src/PowDevRUL.egg-info/SOURCES.txt` & `PowDevRUL-1.0.27/src/PowDevRUL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PowDevRUL-1.0.26/src/powdevrul/function/counters.py` & `PowDevRUL-1.0.27/src/powdevrul/function/counters.py`

 * *Files identical despite different names*

### Comparing `PowDevRUL-1.0.26/src/powdevrul/function/cumul_endommagement.py` & `PowDevRUL-1.0.27/src/powdevrul/function/cumul_endommagement.py`

 * *Files identical despite different names*

### Comparing `PowDevRUL-1.0.26/src/powdevrul/function/graphs.py` & `PowDevRUL-1.0.27/src/powdevrul/function/graphs.py`

 * *Files identical despite different names*

### Comparing `PowDevRUL-1.0.26/src/powdevrul/function/losses.py` & `PowDevRUL-1.0.27/src/powdevrul/function/losses.py`

 * *Files identical despite different names*

### Comparing `PowDevRUL-1.0.26/src/powdevrul/function/matrix.py` & `PowDevRUL-1.0.27/src/powdevrul/function/matrix.py`

 * *Files identical despite different names*

### Comparing `PowDevRUL-1.0.26/src/powdevrul/function/poly_somme.py` & `PowDevRUL-1.0.27/src/powdevrul/function/poly_somme.py`

 * *Files identical despite different names*

### Comparing `PowDevRUL-1.0.26/src/powdevrul/function/temperature.py` & `PowDevRUL-1.0.27/src/powdevrul/function/temperature.py`

 * *Files identical despite different names*

### Comparing `PowDevRUL-1.0.26/src/powdevrul/function/zth_materials.py` & `PowDevRUL-1.0.27/src/powdevrul/function/zth_materials.py`

 * *Files identical despite different names*

### Comparing `PowDevRUL-1.0.26/src/powdevrul/lifetime.py` & `PowDevRUL-1.0.27/src/powdevrul/lifetime.py`

 * *Files identical despite different names*

