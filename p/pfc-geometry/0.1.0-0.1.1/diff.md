# Comparing `tmp/pfc_geometry-0.1.0.tar.gz` & `tmp/pfc_geometry-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfc_geometry-0.1.0.tar", last modified: Tue Feb 28 15:18:06 2023, max compression
+gzip compressed data, was "pfc_geometry-0.1.1.tar", last modified: Tue Feb 28 17:58:02 2023, max compression
```

## Comparing `pfc_geometry-0.1.0.tar` & `pfc_geometry-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-02-28 15:18:06.045318 pfc_geometry-0.1.0/
--rw-r--r--   0 tom       (1000) tom       (1000)    35129 2022-12-20 14:21:13.000000 pfc_geometry-0.1.0/COPYING
--rw-r--r--   0 tom       (1000) tom       (1000)      321 2023-02-28 15:18:06.045318 pfc_geometry-0.1.0/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      112 2022-12-20 14:21:13.000000 pfc_geometry-0.1.0/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-02-28 15:18:06.045318 pfc_geometry-0.1.0/geometry/
--rw-r--r--   0 tom       (1000) tom       (1000)     1179 2022-12-20 14:21:13.000000 pfc_geometry-0.1.0/geometry/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8619 2022-12-20 14:21:13.000000 pfc_geometry-0.1.0/geometry/base.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1126 2022-12-20 14:21:13.000000 pfc_geometry-0.1.0/geometry/circle.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2956 2023-02-28 15:08:16.000000 pfc_geometry-0.1.0/geometry/coordinate_frame.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3573 2022-12-20 14:21:13.000000 pfc_geometry-0.1.0/geometry/gps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1271 2022-12-20 14:21:13.000000 pfc_geometry-0.1.0/geometry/mass.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5150 2022-12-20 14:21:13.000000 pfc_geometry-0.1.0/geometry/point.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8238 2022-12-31 14:16:51.000000 pfc_geometry-0.1.0/geometry/quaternion.py
--rw-r--r--   0 tom       (1000) tom       (1000)      375 2022-12-20 14:21:13.000000 pfc_geometry-0.1.0/geometry/testing.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3870 2022-12-20 14:21:13.000000 pfc_geometry-0.1.0/geometry/transformation.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-02-28 15:18:06.045318 pfc_geometry-0.1.0/pfc_geometry.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)      321 2023-02-28 15:18:06.000000 pfc_geometry-0.1.0/pfc_geometry.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      387 2023-02-28 15:18:06.000000 pfc_geometry-0.1.0/pfc_geometry.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-02-28 15:18:06.000000 pfc_geometry-0.1.0/pfc_geometry.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        9 2023-02-28 15:18:06.000000 pfc_geometry-0.1.0/pfc_geometry.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       79 2023-02-28 15:18:06.045318 pfc_geometry-0.1.0/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)     1016 2023-02-28 14:51:17.000000 pfc_geometry-0.1.0/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-02-28 17:58:02.455318 pfc_geometry-0.1.1/
+-rw-r--r--   0 tom       (1000) tom       (1000)    35129 2022-12-20 14:21:13.000000 pfc_geometry-0.1.1/COPYING
+-rw-r--r--   0 tom       (1000) tom       (1000)     7632 2023-02-28 16:22:05.000000 pfc_geometry-0.1.1/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)      432 2023-02-28 17:58:02.455318 pfc_geometry-0.1.1/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      114 2023-02-28 16:05:35.000000 pfc_geometry-0.1.1/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-02-28 17:58:02.455318 pfc_geometry-0.1.1/geometry/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1179 2022-12-20 14:21:13.000000 pfc_geometry-0.1.1/geometry/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8619 2022-12-20 14:21:13.000000 pfc_geometry-0.1.1/geometry/base.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1126 2022-12-20 14:21:13.000000 pfc_geometry-0.1.1/geometry/circle.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2956 2023-02-28 15:08:16.000000 pfc_geometry-0.1.1/geometry/coordinate_frame.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3573 2022-12-20 14:21:13.000000 pfc_geometry-0.1.1/geometry/gps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1271 2022-12-20 14:21:13.000000 pfc_geometry-0.1.1/geometry/mass.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5150 2022-12-20 14:21:13.000000 pfc_geometry-0.1.1/geometry/point.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8238 2022-12-31 14:16:51.000000 pfc_geometry-0.1.1/geometry/quaternion.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      375 2022-12-20 14:21:13.000000 pfc_geometry-0.1.1/geometry/testing.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3870 2022-12-20 14:21:13.000000 pfc_geometry-0.1.1/geometry/transformation.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-02-28 17:58:02.455318 pfc_geometry-0.1.1/pfc_geometry.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)      432 2023-02-28 17:58:02.000000 pfc_geometry-0.1.1/pfc_geometry.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      430 2023-02-28 17:58:02.000000 pfc_geometry-0.1.1/pfc_geometry.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-02-28 17:58:02.000000 pfc_geometry-0.1.1/pfc_geometry.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       24 2023-02-28 17:58:02.000000 pfc_geometry-0.1.1/pfc_geometry.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        9 2023-02-28 17:58:02.000000 pfc_geometry-0.1.1/pfc_geometry.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)      426 2023-02-28 17:58:02.455318 pfc_geometry-0.1.1/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)      699 2023-02-28 15:48:55.000000 pfc_geometry-0.1.1/setup.py
```

### Comparing `pfc_geometry-0.1.0/COPYING` & `pfc_geometry-0.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.0/geometry/__init__.py` & `pfc_geometry-0.1.1/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.0/geometry/base.py` & `pfc_geometry-0.1.1/geometry/base.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.0/geometry/circle.py` & `pfc_geometry-0.1.1/geometry/circle.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.0/geometry/coordinate_frame.py` & `pfc_geometry-0.1.1/geometry/coordinate_frame.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.0/geometry/gps.py` & `pfc_geometry-0.1.1/geometry/gps.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.0/geometry/mass.py` & `pfc_geometry-0.1.1/geometry/mass.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.0/geometry/point.py` & `pfc_geometry-0.1.1/geometry/point.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.0/geometry/quaternion.py` & `pfc_geometry-0.1.1/geometry/quaternion.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.0/geometry/transformation.py` & `pfc_geometry-0.1.1/geometry/transformation.py`

 * *Files identical despite different names*

