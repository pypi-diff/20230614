# Comparing `tmp/xenosite-fragment-0a4.tar.gz` & `tmp/xenosite-fragment-0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenosite-fragment-0a4.tar", last modified: Fri Jun  9 19:06:08 2023, max compression
+gzip compressed data, was "xenosite-fragment-0a5.tar", last modified: Wed Jun 14 16:07:03 2023, max compression
```

## Comparing `xenosite-fragment-0a4.tar` & `xenosite-fragment-0a5.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 swamidass   (501) staff       (20)        0 2023-06-09 19:06:08.558136 xenosite-fragment-0a4/
--rw-r--r--   0 swamidass   (501) staff       (20)     4396 2023-06-09 19:06:08.557584 xenosite-fragment-0a4/PKG-INFO
--rw-r--r--   0 swamidass   (501) staff       (20)     3735 2023-06-09 19:04:17.000000 xenosite-fragment-0a4/README.md
--rw-r--r--   0 swamidass   (501) staff       (20)       76 2022-11-29 00:33:42.000000 xenosite-fragment-0a4/pyproject.toml
--rw-r--r--   0 swamidass   (501) staff       (20)       38 2023-06-09 19:06:08.558363 xenosite-fragment-0a4/setup.cfg
--rw-r--r--   0 swamidass   (501) staff       (20)     1790 2023-06-09 18:47:43.000000 xenosite-fragment-0a4/setup.py
-drwxr-xr-x   0 swamidass   (501) staff       (20)        0 2023-06-09 19:06:08.538501 xenosite-fragment-0a4/test/
--rw-r--r--   0 swamidass   (501) staff       (20)     1460 2023-06-08 21:38:52.000000 xenosite-fragment-0a4/test/test_fragment.py
--rw-r--r--   0 swamidass   (501) staff       (20)      950 2023-05-28 17:37:00.000000 xenosite-fragment-0a4/test/test_morgan.py
--rw-r--r--   0 swamidass   (501) staff       (20)     7779 2023-05-25 21:09:30.000000 xenosite-fragment-0a4/test/test_netx.py
--rw-r--r--   0 swamidass   (501) staff       (20)     1197 2022-12-08 17:59:30.000000 xenosite-fragment-0a4/test/test_remap.py
-drwxr-xr-x   0 swamidass   (501) staff       (20)        0 2023-06-09 19:06:08.533758 xenosite-fragment-0a4/xenosite/
-drwxr-xr-x   0 swamidass   (501) staff       (20)        0 2023-06-09 19:06:08.558735 xenosite-fragment-0a4/xenosite/fragment/
--rw-r--r--   0 swamidass   (501) staff       (20)     3959 2023-06-09 18:45:14.000000 xenosite-fragment-0a4/xenosite/fragment/__init__.py
--rw-r--r--   0 swamidass   (501) staff       (20)     9026 2022-11-28 23:05:55.000000 xenosite-fragment-0a4/xenosite/fragment/__main__.py
--rw-r--r--   0 swamidass   (501) staff       (20)       59 2023-06-09 19:06:08.558907 xenosite-fragment-0a4/xenosite/fragment/_static_version.py
--rw-r--r--   0 swamidass   (501) staff       (20)     5773 2022-11-09 23:54:52.000000 xenosite-fragment-0a4/xenosite/fragment/_version.py
--rw-r--r--   0 swamidass   (501) staff       (20)     7746 2023-06-08 22:02:35.000000 xenosite-fragment-0a4/xenosite/fragment/chem.py
--rw-r--r--   0 swamidass   (501) staff       (20)     6224 2023-06-07 17:13:05.000000 xenosite-fragment-0a4/xenosite/fragment/feature.py
--rw-r--r--   0 swamidass   (501) staff       (20)     4848 2023-06-08 21:33:14.000000 xenosite-fragment-0a4/xenosite/fragment/graph.py
--rw-r--r--   0 swamidass   (501) staff       (20)     1236 2023-06-09 18:52:58.000000 xenosite-fragment-0a4/xenosite/fragment/keras_backend.py
--rw-r--r--   0 swamidass   (501) staff       (20)     3063 2023-06-03 20:49:36.000000 xenosite-fragment-0a4/xenosite/fragment/morgan.py
--rw-r--r--   0 swamidass   (501) staff       (20)       78 2023-05-25 21:12:23.000000 xenosite-fragment-0a4/xenosite/fragment/netx.py
--rw-r--r--   0 swamidass   (501) staff       (20)     3180 2022-12-08 17:59:30.000000 xenosite-fragment-0a4/xenosite/fragment/remap.py
--rw-r--r--   0 swamidass   (501) staff       (20)     5640 2023-06-07 18:01:31.000000 xenosite-fragment-0a4/xenosite/fragment/serialize.py
--rw-r--r--   0 swamidass   (501) staff       (20)     3650 2023-05-27 20:39:10.000000 xenosite-fragment-0a4/xenosite/fragment/stats.py
-drwxr-xr-x   0 swamidass   (501) staff       (20)        0 2023-06-09 19:06:08.556635 xenosite-fragment-0a4/xenosite_fragment.egg-info/
--rw-r--r--   0 swamidass   (501) staff       (20)     4396 2023-06-09 19:06:08.000000 xenosite-fragment-0a4/xenosite_fragment.egg-info/PKG-INFO
--rw-r--r--   0 swamidass   (501) staff       (20)      743 2023-06-09 19:06:08.000000 xenosite-fragment-0a4/xenosite_fragment.egg-info/SOURCES.txt
--rw-r--r--   0 swamidass   (501) staff       (20)        1 2023-06-09 19:06:08.000000 xenosite-fragment-0a4/xenosite_fragment.egg-info/dependency_links.txt
--rw-r--r--   0 swamidass   (501) staff       (20)      131 2023-06-09 19:06:08.000000 xenosite-fragment-0a4/xenosite_fragment.egg-info/entry_points.txt
--rw-r--r--   0 swamidass   (501) staff       (20)       45 2023-06-09 19:06:08.000000 xenosite-fragment-0a4/xenosite_fragment.egg-info/requires.txt
--rw-r--r--   0 swamidass   (501) staff       (20)       18 2023-06-09 19:06:08.000000 xenosite-fragment-0a4/xenosite_fragment.egg-info/top_level.txt
+drwxr-xr-x   0 swamidass   (501) staff       (20)        0 2023-06-14 16:07:03.392874 xenosite-fragment-0a5/
+-rw-r--r--   0 swamidass   (501) staff       (20)     4396 2023-06-14 16:07:03.392266 xenosite-fragment-0a5/PKG-INFO
+-rw-r--r--   0 swamidass   (501) staff       (20)     3735 2023-06-09 19:04:17.000000 xenosite-fragment-0a5/README.md
+-rw-r--r--   0 swamidass   (501) staff       (20)       76 2022-11-29 00:33:42.000000 xenosite-fragment-0a5/pyproject.toml
+-rw-r--r--   0 swamidass   (501) staff       (20)       38 2023-06-14 16:07:03.393129 xenosite-fragment-0a5/setup.cfg
+-rw-r--r--   0 swamidass   (501) staff       (20)     1790 2023-06-09 18:47:43.000000 xenosite-fragment-0a5/setup.py
+drwxr-xr-x   0 swamidass   (501) staff       (20)        0 2023-06-14 16:07:03.380389 xenosite-fragment-0a5/test/
+-rw-r--r--   0 swamidass   (501) staff       (20)     1460 2023-06-08 21:38:52.000000 xenosite-fragment-0a5/test/test_fragment.py
+-rw-r--r--   0 swamidass   (501) staff       (20)      950 2023-05-28 17:37:00.000000 xenosite-fragment-0a5/test/test_morgan.py
+-rw-r--r--   0 swamidass   (501) staff       (20)     7779 2023-05-25 21:09:30.000000 xenosite-fragment-0a5/test/test_netx.py
+-rw-r--r--   0 swamidass   (501) staff       (20)     1197 2022-12-08 17:59:30.000000 xenosite-fragment-0a5/test/test_remap.py
+-rw-r--r--   0 swamidass   (501) staff       (20)     1106 2023-06-14 15:20:24.000000 xenosite-fragment-0a5/test/test_tanimoto.py
+drwxr-xr-x   0 swamidass   (501) staff       (20)        0 2023-06-14 16:07:03.376796 xenosite-fragment-0a5/xenosite/
+drwxr-xr-x   0 swamidass   (501) staff       (20)        0 2023-06-14 16:07:03.393497 xenosite-fragment-0a5/xenosite/fragment/
+-rw-r--r--   0 swamidass   (501) staff       (20)     3976 2023-06-14 15:09:35.000000 xenosite-fragment-0a5/xenosite/fragment/__init__.py
+-rw-r--r--   0 swamidass   (501) staff       (20)     9026 2022-11-28 23:05:55.000000 xenosite-fragment-0a5/xenosite/fragment/__main__.py
+-rw-r--r--   0 swamidass   (501) staff       (20)       59 2023-06-14 16:07:03.393642 xenosite-fragment-0a5/xenosite/fragment/_static_version.py
+-rw-r--r--   0 swamidass   (501) staff       (20)     5773 2022-11-09 23:54:52.000000 xenosite-fragment-0a5/xenosite/fragment/_version.py
+-rw-r--r--   0 swamidass   (501) staff       (20)    12807 2023-06-14 15:22:00.000000 xenosite-fragment-0a5/xenosite/fragment/chem.py
+-rw-r--r--   0 swamidass   (501) staff       (20)     6224 2023-06-07 17:13:05.000000 xenosite-fragment-0a5/xenosite/fragment/feature.py
+-rw-r--r--   0 swamidass   (501) staff       (20)     4848 2023-06-08 21:33:14.000000 xenosite-fragment-0a5/xenosite/fragment/graph.py
+-rw-r--r--   0 swamidass   (501) staff       (20)     1236 2023-06-14 16:06:47.000000 xenosite-fragment-0a5/xenosite/fragment/keras_backend.py
+-rw-r--r--   0 swamidass   (501) staff       (20)     3063 2023-06-03 20:49:36.000000 xenosite-fragment-0a5/xenosite/fragment/morgan.py
+-rw-r--r--   0 swamidass   (501) staff       (20)       78 2023-05-25 21:12:23.000000 xenosite-fragment-0a5/xenosite/fragment/netx.py
+-rw-r--r--   0 swamidass   (501) staff       (20)     3180 2022-12-08 17:59:30.000000 xenosite-fragment-0a5/xenosite/fragment/remap.py
+-rw-r--r--   0 swamidass   (501) staff       (20)     5640 2023-06-07 18:01:31.000000 xenosite-fragment-0a5/xenosite/fragment/serialize.py
+-rw-r--r--   0 swamidass   (501) staff       (20)     3650 2023-05-27 20:39:10.000000 xenosite-fragment-0a5/xenosite/fragment/stats.py
+drwxr-xr-x   0 swamidass   (501) staff       (20)        0 2023-06-14 16:07:03.391438 xenosite-fragment-0a5/xenosite_fragment.egg-info/
+-rw-r--r--   0 swamidass   (501) staff       (20)     4396 2023-06-14 16:07:03.000000 xenosite-fragment-0a5/xenosite_fragment.egg-info/PKG-INFO
+-rw-r--r--   0 swamidass   (501) staff       (20)      765 2023-06-14 16:07:03.000000 xenosite-fragment-0a5/xenosite_fragment.egg-info/SOURCES.txt
+-rw-r--r--   0 swamidass   (501) staff       (20)        1 2023-06-14 16:07:03.000000 xenosite-fragment-0a5/xenosite_fragment.egg-info/dependency_links.txt
+-rw-r--r--   0 swamidass   (501) staff       (20)      131 2023-06-14 16:07:03.000000 xenosite-fragment-0a5/xenosite_fragment.egg-info/entry_points.txt
+-rw-r--r--   0 swamidass   (501) staff       (20)       45 2023-06-14 16:07:03.000000 xenosite-fragment-0a5/xenosite_fragment.egg-info/requires.txt
+-rw-r--r--   0 swamidass   (501) staff       (20)       18 2023-06-14 16:07:03.000000 xenosite-fragment-0a5/xenosite_fragment.egg-info/top_level.txt
```

### Comparing `xenosite-fragment-0a4/PKG-INFO` & `xenosite-fragment-0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xenosite-fragment
-Version: 0a4
+Version: 0a5
 Summary: Library for molecule fragment operations.
 Author: S. Joshua Swamidass
 Author-email: swamidass@wustl.edu
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
```

### Comparing `xenosite-fragment-0a4/README.md` & `xenosite-fragment-0a5/README.md`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a4/setup.py` & `xenosite-fragment-0a5/setup.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a4/test/test_fragment.py` & `xenosite-fragment-0a5/test/test_fragment.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a4/test/test_morgan.py` & `xenosite-fragment-0a5/test/test_morgan.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a4/test/test_netx.py` & `xenosite-fragment-0a5/test/test_netx.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a4/test/test_remap.py` & `xenosite-fragment-0a5/test/test_remap.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a4/xenosite/fragment/__init__.py` & `xenosite-fragment-0a5/xenosite/fragment/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 >>> fragments["size"].to_numpy()
 array([5, 1, 4])
 
 """
 
 
 from .graph import Graph
-from .chem import Fragment, MolToSmartsGraph
+from .chem import Fragment, MolToSmartsGraph, smarts_tanimoto
 from .net import (
     SubGraphFragmentNetwork as FragmentNetworkX,
     RingFragmentNetwork as RingFragmentNetworkX,
 )
 from ._version import __version__
```

### Comparing `xenosite-fragment-0a4/xenosite/fragment/__main__.py` & `xenosite-fragment-0a5/xenosite/fragment/__main__.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a4/xenosite/fragment/_version.py` & `xenosite-fragment-0a5/xenosite/fragment/_version.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a4/xenosite/fragment/feature.py` & `xenosite-fragment-0a5/xenosite/fragment/feature.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a4/xenosite/fragment/graph.py` & `xenosite-fragment-0a5/xenosite/fragment/graph.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a4/xenosite/fragment/keras_backend.py` & `xenosite-fragment-0a5/xenosite/fragment/keras_backend.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a4/xenosite/fragment/morgan.py` & `xenosite-fragment-0a5/xenosite/fragment/morgan.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a4/xenosite/fragment/remap.py` & `xenosite-fragment-0a5/xenosite/fragment/remap.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a4/xenosite/fragment/serialize.py` & `xenosite-fragment-0a5/xenosite/fragment/serialize.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a4/xenosite/fragment/stats.py` & `xenosite-fragment-0a5/xenosite/fragment/stats.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a4/xenosite_fragment.egg-info/PKG-INFO` & `xenosite-fragment-0a5/xenosite_fragment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xenosite-fragment
-Version: 0a4
+Version: 0a5
 Summary: Library for molecule fragment operations.
 Author: S. Joshua Swamidass
 Author-email: swamidass@wustl.edu
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
```

### Comparing `xenosite-fragment-0a4/xenosite_fragment.egg-info/SOURCES.txt` & `xenosite-fragment-0a5/xenosite_fragment.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.md
 pyproject.toml
 setup.py
 test/test_fragment.py
 test/test_morgan.py
 test/test_netx.py
 test/test_remap.py
+test/test_tanimoto.py
 xenosite/fragment/__init__.py
 xenosite/fragment/__main__.py
 xenosite/fragment/_static_version.py
 xenosite/fragment/_version.py
 xenosite/fragment/chem.py
 xenosite/fragment/feature.py
 xenosite/fragment/graph.py
```

