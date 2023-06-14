# Comparing `tmp/large-image-source-tifffile-1.22.4.dev3.tar.gz` & `tmp/large-image-source-tifffile-1.22.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-tifffile-1.22.4.dev3.tar", last modified: Mon Jun 12 21:40:12 2023, max compression
+gzip compressed data, was "large-image-source-tifffile-1.22.5.dev2.tar", last modified: Wed Jun 14 21:14:36 2023, max compression
```

## Comparing `large-image-source-tifffile-1.22.4.dev3.tar` & `large-image-source-tifffile-1.22.5.dev2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 21:40:12.063052 large-image-source-tifffile-1.22.4.dev3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-12 21:40:11.000000 large-image-source-tifffile-1.22.4.dev3/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-06-12 21:40:12.063052 large-image-source-tifffile-1.22.4.dev3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-12 21:40:11.000000 large-image-source-tifffile-1.22.4.dev3/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 21:40:12.063052 large-image-source-tifffile-1.22.4.dev3/large_image_source_tifffile/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20974 2023-06-12 21:38:20.000000 large-image-source-tifffile-1.22.4.dev3/large_image_source_tifffile/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2023-06-12 21:38:20.000000 large-image-source-tifffile-1.22.4.dev3/large_image_source_tifffile/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 21:40:12.063052 large-image-source-tifffile-1.22.4.dev3/large_image_source_tifffile.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-06-12 21:40:11.000000 large-image-source-tifffile-1.22.4.dev3/large_image_source_tifffile.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-06-12 21:40:12.000000 large-image-source-tifffile-1.22.4.dev3/large_image_source_tifffile.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-12 21:40:11.000000 large-image-source-tifffile-1.22.4.dev3/large_image_source_tifffile.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-06-12 21:40:11.000000 large-image-source-tifffile-1.22.4.dev3/large_image_source_tifffile.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2023-06-12 21:40:11.000000 large-image-source-tifffile-1.22.4.dev3/large_image_source_tifffile.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-06-12 21:40:11.000000 large-image-source-tifffile-1.22.4.dev3/large_image_source_tifffile.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-12 21:40:12.063052 large-image-source-tifffile-1.22.4.dev3/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2694 2023-06-12 21:38:20.000000 large-image-source-tifffile-1.22.4.dev3/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:14:36.697084 large-image-source-tifffile-1.22.5.dev2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-14 21:14:36.000000 large-image-source-tifffile-1.22.5.dev2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-06-14 21:14:36.697084 large-image-source-tifffile-1.22.5.dev2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-14 21:14:36.000000 large-image-source-tifffile-1.22.5.dev2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:14:36.697084 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20974 2023-06-14 21:12:44.000000 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2023-06-14 21:12:44.000000 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:14:36.697084 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-06-14 21:14:36.000000 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-06-14 21:14:36.000000 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-14 21:14:36.000000 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-06-14 21:14:36.000000 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2023-06-14 21:14:36.000000 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-06-14 21:14:36.000000 large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-14 21:14:36.697084 large-image-source-tifffile-1.22.5.dev2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2694 2023-06-14 21:12:44.000000 large-image-source-tifffile-1.22.5.dev2/setup.py
```

### Comparing `large-image-source-tifffile-1.22.4.dev3/LICENSE` & `large-image-source-tifffile-1.22.5.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.22.4.dev3/PKG-INFO` & `large-image-source-tifffile-1.22.5.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.22.4.dev3
+Version: 1.22.5.dev2
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-tifffile-1.22.4.dev3/README.rst` & `large-image-source-tifffile-1.22.5.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.22.4.dev3/large_image_source_tifffile/__init__.py` & `large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.22.4.dev3/large_image_source_tifffile/girder_source.py` & `large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.22.4.dev3/large_image_source_tifffile.egg-info/PKG-INFO` & `large-image-source-tifffile-1.22.5.dev2/large_image_source_tifffile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.22.4.dev3
+Version: 1.22.5.dev2
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-tifffile-1.22.4.dev3/setup.py` & `large-image-source-tifffile-1.22.5.dev2/setup.py`

 * *Files identical despite different names*

