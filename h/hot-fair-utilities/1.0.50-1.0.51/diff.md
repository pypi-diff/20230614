# Comparing `tmp/hot-fair-utilities-1.0.50.tar.gz` & `tmp/hot-fair-utilities-1.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hot-fair-utilities-1.0.50.tar", last modified: Mon Jun 12 13:19:02 2023, max compression
+gzip compressed data, was "hot-fair-utilities-1.0.51.tar", last modified: Wed Jun 14 09:13:45 2023, max compression
```

## Comparing `hot-fair-utilities-1.0.50.tar` & `hot-fair-utilities-1.0.51.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-06-12 13:19:02.821496 hot-fair-utilities-1.0.50/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)    34523 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/LICENSE
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       91 2023-01-30 11:58:06.000000 hot-fair-utilities-1.0.50/MANIFEST.in
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)    43175 2023-06-12 13:19:02.821496 hot-fair-utilities-1.0.50/PKG-INFO
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2801 2022-12-28 10:39:39.000000 hot-fair-utilities-1.0.50/README.md
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-06-12 13:19:02.811496 hot-fair-utilities-1.0.50/hot_fair_utilities/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)      188 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/__init__.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1720 2023-01-04 15:35:16.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/georeferencing.py
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-06-12 13:19:02.811496 hot-fair-utilities-1.0.50/hot_fair_utilities/inference/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       29 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/inference/__init__.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2648 2023-06-12 06:44:41.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/inference/predict.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)      775 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/inference/utils.py
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-06-12 13:19:02.821496 hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       68 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/__init__.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2715 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/building_footprint.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)      991 2023-06-12 06:44:41.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/get_polygons.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2470 2023-06-12 06:44:41.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/merge_polygons.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1640 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/polygonize.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     8440 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/utils.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2452 2023-06-12 13:16:01.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/vectorize.py
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-06-12 13:19:02.821496 hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       35 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/__init__.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     4532 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/clip_labels.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1248 2023-06-12 06:44:41.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/fix_labels.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2917 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/preprocess.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)      629 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/reproject_labels.py
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-06-12 13:19:02.821496 hot-fair-utilities-1.0.50/hot_fair_utilities/training/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       25 2023-06-12 13:16:01.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/training/__init__.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1967 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/training/cleanup.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     3629 2023-06-12 13:16:01.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/training/prepare_data.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     4105 2023-06-12 13:16:01.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/training/ramp_config_base.json
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)    11507 2023-06-12 13:16:01.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/training/run_training.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2269 2023-06-12 13:16:01.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/training/train.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2255 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/utils.py
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-06-12 13:19:02.811496 hot-fair-utilities-1.0.50/hot_fair_utilities.egg-info/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)    43175 2023-06-12 13:19:02.000000 hot-fair-utilities-1.0.50/hot_fair_utilities.egg-info/PKG-INFO
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1313 2023-06-12 13:19:02.000000 hot-fair-utilities-1.0.50/hot_fair_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)        1 2023-06-12 13:19:02.000000 hot-fair-utilities-1.0.50/hot_fair_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)      207 2023-06-12 13:19:02.000000 hot-fair-utilities-1.0.50/hot_fair_utilities.egg-info/requires.txt
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       19 2023-06-12 13:19:02.000000 hot-fair-utilities-1.0.50/hot_fair_utilities.egg-info/top_level.txt
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1595 2023-06-12 13:18:10.000000 hot-fair-utilities-1.0.50/pyproject.toml
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       38 2023-06-12 13:19:02.821496 hot-fair-utilities-1.0.50/setup.cfg
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       38 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:45.565979 hot-fair-utilities-1.0.51/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    43175 2023-06-14 09:13:45.565979 hot-fair-utilities-1.0.51/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:45.561979 hot-fair-utilities-1.0.51/hot_fair_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/georeferencing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:45.561979 hot-fair-utilities-1.0.51/hot_fair_utilities/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/inference/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/inference/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:45.561979 hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/building_footprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/get_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/merge_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/polygonize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/vectorize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:45.561979 hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/clip_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/fix_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/reproject_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:45.565979 hot-fair-utilities-1.0.51/hot_fair_utilities/training/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/training/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/training/prepare_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/training/ramp_config_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/training/run_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/training/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:45.561979 hot-fair-utilities-1.0.51/hot_fair_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43175 2023-06-14 09:13:45.000000 hot-fair-utilities-1.0.51/hot_fair_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-14 09:13:45.000000 hot-fair-utilities-1.0.51/hot_fair_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:13:45.000000 hot-fair-utilities-1.0.51/hot_fair_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-14 09:13:45.000000 hot-fair-utilities-1.0.51/hot_fair_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-14 09:13:45.000000 hot-fair-utilities-1.0.51/hot_fair_utilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:13:45.565979 hot-fair-utilities-1.0.51/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/setup.py
```

### Comparing `hot-fair-utilities-1.0.50/LICENSE` & `hot-fair-utilities-1.0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.50/PKG-INFO` & `hot-fair-utilities-1.0.51/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hot-fair-utilities
-Version: 1.0.50
+Version: 1.0.51
 Summary: Utilities for AI - Assisted Mapping fAIr
 Author-email: Omdena <project@omdena.com>, Hot Tech Team <sysadmin@hotosm.org>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hot-fair-utilities-1.0.50/README.md` & `hot-fair-utilities-1.0.51/README.md`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/georeferencing.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/georeferencing.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/inference/predict.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/inference/predict.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/inference/utils.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/inference/utils.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/building_footprint.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/building_footprint.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/get_polygons.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/get_polygons.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/merge_polygons.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/merge_polygons.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/polygonize.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/polygonize.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/utils.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/vectorize.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/vectorize.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from rasterio.merge import merge
 from shapely.geometry import Polygon, shape
 from tqdm import tqdm
 
 TOLERANCE = 0.5
 AREA_THRESHOLD = 0.1
 MAX_RATIO = 10
+MIN_AREA = 3  # sqm
 
 
 def vectorize(input_path: str, output_path: str) -> None:
     """Polygonize raster tiles from the input path.
 
     Note that as input, we are expecting GeoTIF images with EPSG:3857 as
     CRS here. CRS of the resulting GeoJSON file will be EPSG:4326.
@@ -49,15 +50,15 @@
     areas = [poly.area for poly in polygons]
     max_area, median_area = np.max(areas), np.median(areas)
     polygons = [
         Polygon(poly.exterior.coords)
         for poly in polygons
         if poly.area != max_area
         and poly.area / median_area > AREA_THRESHOLD
-        and poly.area > 3
+        and poly.area > MIN_AREA
     ]
 
     gs = gpd.GeoSeries(polygons, crs=kwargs["crs"]).simplify(TOLERANCE)
     gs = remove_overlapping_polygons(gs)
     if gs.empty:
         raise ValueError("No Features Found")
     gs.to_crs("EPSG:4326").to_file(output_path)
```

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/clip_labels.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/clip_labels.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/fix_labels.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/fix_labels.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/preprocess.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/reproject_labels.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/reproject_labels.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/training/cleanup.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/training/cleanup.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/training/prepare_data.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/training/prepare_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -54,18 +54,18 @@
                 "-pfx",
                 f"{dst_path}/fair_split",
                 "-trn",
                 "0.85",
                 "-val",
                 "0.15",
             ],
-            stderr=subprocess.PIPE,
+            env=os.environ,
         )
     except subprocess.CalledProcessError as ex:
-        raise RaiseError(ex.stderr.decode())
+        raise ex
 
     # move all the VALIDATION chips, labels and masks to their new locations
     try:
         subprocess.check_output(
             [
                 python_exec,
                 f"{RAMP_HOME}/ramp-code/scripts/move_chips_from_csv.py",
@@ -73,47 +73,47 @@
                 f"{dst_path}/chips",
                 "-td",
                 f"{dst_path}/val-chips",
                 "-csv",
                 f"{dst_path}/fair_split_val.csv",
                 "-mv",
             ],
-            stderr=subprocess.PIPE,
+            env=os.environ,
         )
     except subprocess.CalledProcessError as ex:
-        raise RaiseError(ex.stderr.decode())
+        raise ex
 
     try:
         subprocess.check_output(
             [
                 python_exec,
                 f"{RAMP_HOME}/ramp-code/scripts/move_chips_from_csv.py",
                 "-sd",
                 f"{dst_path}/labels",
                 "-td",
                 f"{dst_path}/val-labels",
                 "-csv",
                 f"{dst_path}/fair_split_val.csv",
                 "-mv",
             ],
-            stderr=subprocess.PIPE,
+            env=os.environ,
         )
     except subprocess.CalledProcessError as ex:
-        raise RaiseError(ex.stderr.decode())
+        raise ex
 
     try:
         subprocess.check_output(
             [
                 python_exec,
                 f"{RAMP_HOME}/ramp-code/scripts/move_chips_from_csv.py",
                 "-sd",
                 f"{dst_path}/binarymasks",
                 "-td",
                 f"{dst_path}/val-binarymasks",
                 "-csv",
                 f"{dst_path}/fair_split_val.csv",
                 "-mv",
             ],
-            stderr=subprocess.PIPE,
+            env=os.environ,
         )
     except subprocess.CalledProcessError as ex:
-        raise RaiseError(ex.stderr.decode())
+        raise ex
```

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/training/ramp_config_base.json` & `hot-fair-utilities-1.0.51/hot_fair_utilities/training/ramp_config_base.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'feedback'": "OrderedDict([('freeze_layers', False)])"}*

```diff
@@ -50,14 +50,17 @@
             "patience": 50,
             "restore_best_weights": false,
             "verbose": 0
         },
         "use_early_stopping": true
     },
     "experiment_name": "HOT-OSM Efficient-Unet Finetune model_set1_batch20_epoch20_imgAug",
+    "feedback": {
+        "freeze_layers": false
+    },
     "input_img_shape": [
         256,
         256
     ],
     "logging": {
         "experiment_log_path": "ramp-data/TRAIN/fAIr-experiments.csv",
         "experiment_notes": "Binary Mask model, batchsize 20, 20 epochs on HOT-OSM dataset 1 Multizoom, finetuning from RAMP saved model",
```

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/training/run_training.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/training/run_training.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,16 +56,32 @@
 sm.set_framework("tf.keras")
 
 
 # this variable must be defined. It is the parent of the 'ramp-code' directory.
 working_ramp_home = os.environ["RAMP_HOME"]
 
 
-def manage_fine_tuning_config(output_path, num_epochs, batch_size):
+def apply_feedback(
+    pretrained_model_path, output_path, num_epochs, batch_size, freeze_layers
+):
+    if not os.path.exists(output_path):
+        os.makedirs(output_path)
 
+    # Update the fine-tuning configuration
+    fine_tuning_cfg = manage_fine_tuning_config(output_path, num_epochs, batch_size)
+
+    # Set the path of the pre-trained model in the configuration
+    fine_tuning_cfg["saved_model"]["saved_model_path"] = pretrained_model_path
+    fine_tuning_cfg["saved_model"]["use_saved_model"] = True
+    fine_tuning_cfg["freeze_layers"] = freeze_layers
+
+    run_main_train_code(fine_tuning_cfg)
+
+
+def manage_fine_tuning_config(output_path, num_epochs, batch_size, freeze_layers):
     # Define the paths to the source and destination JSON files
     working_dir = os.path.realpath(os.path.dirname(__file__))
     config_base_path = os.path.join(working_dir, "ramp_config_base.json")
     dst_path = os.path.join(output_path, "ramp_fair_config_finetune.json")
 
     # Read the content of the source JSON file
     with open(config_base_path, "r") as f:
@@ -76,14 +92,15 @@
     data["datasets"]["train_mask_dir"] = f"{output_path}/binarymasks"
     data["datasets"]["val_img_dir"] = f"{output_path}/val-chips"
     data["datasets"]["val_mask_dir"] = f"{output_path}/val-binarymasks"
 
     # epoch batchconfig
     data["num_epochs"] = num_epochs
     data["batch_size"] = batch_size
+    data["freeze_layers"] = freeze_layers
 
     # clr plot
     data["cyclic_learning_scheduler"]["clr_plot_dir"] = f"{output_path}/plots"
     # logs
     data["tensorboard"]["tb_logs_dir"] = f"{output_path}/logs"
     # output images
     data["graph_location"] = f"{output_path}/graphs"
@@ -110,15 +127,14 @@
     get_loss_fn = getattr(loss_constructors, get_loss_fn_name)
 
     # Construct the loss function
     loss_fn = get_loss_fn(cfg)
 
     the_metrics = []
     if cfg["metrics"]["use_metrics"]:
-
         get_metrics_fn_names = cfg["metrics"]["get_metrics_fn_names"]
         get_metrics_fn_parms = cfg["metrics"]["metrics_fn_parms"]
 
         for get_mf_name, mf_parms in zip(get_metrics_fn_names, get_metrics_fn_parms):
             get_metric_fn = getattr(metric_constructors, get_mf_name)
             print(f"Metric constructor function: {get_metric_fn.__name__}")
             metric_fn = get_metric_fn(mf_parms)
@@ -130,23 +146,27 @@
     get_optimizer_fn = getattr(optimizer_constructors, get_optimizer_fn_name)
 
     optimizer = get_optimizer_fn(cfg)
 
     the_model = None
 
     if cfg["saved_model"]["use_saved_model"]:
-
         # load (construct) the model
         model_path = Path(working_ramp_home) / cfg["saved_model"]["saved_model_path"]
         print(f"Model: importing saved model {str(model_path)}")
         the_model = tf.keras.models.load_model(model_path)
         assert (
             the_model is not None
         ), f"the saved model was not constructed: {model_path}"
 
+        if cfg["freeze_layers"]:
+            for layer in the_model.layers:
+                layer.trainable = False  # freeze previous layers only update new layers
+                # print("Setting previous model layers traininable : False")
+
         if not cfg["saved_model"]["save_optimizer_state"]:
             # If you don't want to save the original state of training, recompile the model.
             the_model.compile(optimizer=optimizer, loss=loss_fn, metrics=[the_metrics])
 
             # the_model.compile(optimizer = optimizer,
             #    loss=loss_fn,
             #    metrics = [get_iou_coef_fn])
@@ -178,14 +198,17 @@
     input_img_shape = cfg["input_img_shape"]
     output_img_shape = cfg["output_img_shape"]
 
     n_training = get_num_files(train_img_dir, "*.tif")
     n_val = get_num_files(val_img_dir, "*.tif")
     steps_per_epoch = n_training // batch_size
     validation_steps = n_val // batch_size
+    # Testing step , not recommended
+    if validation_steps <= 0:
+        validation_steps = 1
 
     # add these back to the config
     # in case they are needed by callbacks
     cfg["runtime"] = {}
     cfg["runtime"]["n_training"] = n_training
     cfg["runtime"]["n_val"] = n_val
     cfg["runtime"]["steps_per_epoch"] = steps_per_epoch
@@ -215,15 +238,14 @@
 
     assert val_batches is not None, "validation batches were not constructed"
 
     ## Callbacks ##
     callbacks_list = []
 
     if not discard_experiment:
-
         # get model checkpoint callback
         if cfg["model_checkpts"]["use_model_checkpts"]:
             get_model_checkpt_callback_fn_name = cfg["model_checkpts"][
                 "get_model_checkpt_callback_fn_name"
             ]
             get_model_checkpt_callback_fn = getattr(
                 callback_constructors, get_model_checkpt_callback_fn_name
@@ -249,15 +271,14 @@
             )
             callbacks_list.append(get_prediction_logging_fn(the_model, cfg))
 
     # free up RAM
     keras.backend.clear_session()
 
     if cfg["early_stopping"]["use_early_stopping"]:
-
         callbacks_list.append(callback_constructors.get_early_stopping_callback_fn(cfg))
 
         # get cyclic learning scheduler callback
     if cfg["cyclic_learning_scheduler"]["use_clr"]:
         assert not cfg["early_stopping"][
             "use_early_stopping"
         ], "cannot use early_stopping with cycling_learning_scheduler"
@@ -270,15 +291,15 @@
     ## Main training block ##
     n_epochs = cfg["num_epochs"]
     print(
         f"Starting Training with {n_epochs} epochs , {batch_size} batch size , {steps_per_epoch} steps per epoch , {validation_steps} validation steps......"
     )
     if validation_steps <= 0:
         raise RaiseError(
-            "Not enough data for training, Increase image or Try reducing batchsize/ephochs"
+            "Not enough data for training, Increase image or Try reducing batchsize/epochs"
         )
     # FIXME : Make checkpoint
     start = perf_counter()
     history = the_model.fit(
         train_batches,
         epochs=n_epochs,
         steps_per_epoch=steps_per_epoch,
@@ -294,27 +315,24 @@
     if not os.path.exists(cfg["graph_location"]):
         os.mkdir(cfg["graph_location"])
 
     loss = history.history["loss"]
     # val_loss = history.history["val_loss"]
     epochs = range(1, len(loss) + 1)
 
-    # plt.plot(epochs, loss, "y", label="Training loss")
-    # plt.plot(epochs, val_loss, "r", label="Validation loss")
-    # plt.title("Training and validation loss")
-    # plt.xlabel("Epochs")
-    # plt.ylabel("Loss")
-    # plt.legend()
-    # plt.savefig(f"{cfg['graph_location']}/training_validation_loss.png")
-
     acc = history.history["sparse_categorical_accuracy"]
     val_acc = history.history["val_sparse_categorical_accuracy"]
-    plt.plot(epochs, acc, "y", label="Training acc")
-    plt.plot(epochs, val_acc, "r", label="Validation sparse categorical acc")
-    plt.title("Training and validation sparse categorical accuracy")
+
+    # Plot training and validation accuracy
+    plt.plot(epochs, acc, "y", label="Training Accuracy")
+    plt.plot(epochs, val_acc, "r", label="Validation Accuracy")
+
+    # Set labels and title
     plt.xlabel("Epochs")
-    plt.ylabel("Sparse Categorical Accuracy")
+    plt.ylabel("Accuracy")
+    plt.title("Training and Validation Accuracy")
+
     plt.legend()
     plt.savefig(
         f"{cfg['graph_location']}/training_validation_sparse_categorical_accuracy.png"
     )
     print(f"Graph generated at : {cfg['graph_location']}")
```

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/training/train.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/training/train.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Standard library imports
 import os
 
 from .cleanup import extract_highest_accuracy_model
 from .prepare_data import split_training_2_validation
-from .run_training import manage_fine_tuning_config, run_main_train_code
+from .run_training import apply_feedback, manage_fine_tuning_config, run_main_train_code
 
 
 def train(
     input_path: str,
     output_path: str,
     epoch_size: int,
     batch_size: int,
     model: str,
     model_home: str,
+    freeze_layers: bool = False,
 ):
     """Trains the input image with base model
 
 
     Args:
         input_path: Path of the directory output by preprocess
         output_path: Path of the working dir for training
@@ -47,13 +48,39 @@
     os.environ.update(os.environ)
     if model.lower() == "ramp":
         # Add a new environment variable to the operating system
         os.environ["RAMP_HOME"] = model_home
         # Print the environment variables to verify that the new variable was added
         print("Starting to prepare data for training")
         split_training_2_validation(input_path, output_path)
-        cfg = manage_fine_tuning_config(output_path, epoch_size, batch_size)
+        cfg = manage_fine_tuning_config(
+            output_path, epoch_size, batch_size, freeze_layers
+        )
         print("Data is ready for training")
         run_main_train_code(cfg)
         print("extracting highest accuracy model")
         final_accuracy, final_model_path = extract_highest_accuracy_model(output_path)
         return (final_accuracy, final_model_path)
+
+
+def run_feedback(
+    input_path,
+    output_path,
+    feedback_base_model,
+    model_home: str,
+    epoch_size: int,
+    batch_size: int,
+    freeze_layers: bool = False,
+):
+    assert os.path.exists(input_path), "Input Feedback Path Doesn't Exist"
+    assert os.path.exists(feedback_base_model), "Feedback base Model Doesn't Exist"
+    os.environ.update(os.environ)
+    os.environ["RAMP_HOME"] = model_home
+    print("Starting to prepare data for training")
+    split_training_2_validation(input_path, output_path)
+    print("Data is ready for training")
+
+    apply_feedback(
+        feedback_base_model, output_path, epoch_size, batch_size, freeze_layers
+    )
+    final_accuracy, final_model_path = extract_highest_accuracy_model(output_path)
+    return (final_accuracy, final_model_path)
```

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities/utils.py` & `hot-fair-utilities-1.0.51/hot_fair_utilities/utils.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities.egg-info/PKG-INFO` & `hot-fair-utilities-1.0.51/hot_fair_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hot-fair-utilities
-Version: 1.0.50
+Version: 1.0.51
 Summary: Utilities for AI - Assisted Mapping fAIr
 Author-email: Omdena <project@omdena.com>, Hot Tech Team <sysadmin@hotosm.org>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hot-fair-utilities-1.0.50/hot_fair_utilities.egg-info/SOURCES.txt` & `hot-fair-utilities-1.0.51/hot_fair_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.50/pyproject.toml` & `hot-fair-utilities-1.0.51/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hot-fair-utilities"
-version = "1.0.50"
+version = "1.0.51"
 description = "Utilities for AI - Assisted Mapping fAIr"
 readme = "README.md"
 authors = [{ name = "Omdena", email = "project@omdena.com" },{ name = "Hot Tech Team", email = "sysadmin@hotosm.org" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
@@ -29,15 +29,15 @@
     build = ["build", "twine"]
     dev   = ["black", "bumpver", "isort"]
 
     [project.urls]
     repository    = "https://github.com/hotosm/fAIr-utilities"
 
 [tool.bumpver]
-current_version = "1.0.44"
+current_version = "1.0.51"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
     [tool.bumpver.file_patterns]
```

