# Comparing `tmp/tti_dataset_tools-0.1.5.tar.gz` & `tmp/tti_dataset_tools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tti_dataset_tools-0.1.5.tar", max compression
+gzip compressed data, was "tti_dataset_tools-0.1.6.tar", max compression
```

## Comparing `tti_dataset_tools-0.1.5.tar` & `tti_dataset_tools-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1089 2022-12-16 21:14:46.000000 tti_dataset_tools-0.1.5/LICENSE
--rw-r--r--   0        0        0     1058 2023-06-13 05:03:10.000000 tti_dataset_tools-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       82 2022-12-16 21:14:46.000000 tti_dataset_tools-0.1.5/README.md
--rw-r--r--   0        0        0       42 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.5/src/ind_tools/__init__.py
--rw-r--r--   0        0        0     1471 2023-05-28 23:36:30.000000 tti_dataset_tools-0.1.5/src/ind_tools/IndTransformer.py
--rw-r--r--   0        0        0      303 2023-05-28 23:13:00.000000 tti_dataset_tools-0.1.5/src/tti_dataset_tools/__init__.py
--rw-r--r--   0        0        0     1012 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.5/src/tti_dataset_tools/ColMapper.py
--rw-r--r--   0        0        0     4371 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.5/src/tti_dataset_tools/InfluenceAnalyzer.py
--rw-r--r--   0        0        0        0 2023-05-04 17:45:58.510000 tti_dataset_tools-0.1.5/src/tti_dataset_tools/models/__init__.py
--rw-r--r--   0        0        0     6200 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.5/src/tti_dataset_tools/models/CrosswalkModel.py
--rw-r--r--   0        0        0     1123 2023-05-28 23:07:06.000000 tti_dataset_tools-0.1.5/src/tti_dataset_tools/TrackClass.py
--rw-r--r--   0        0        0      470 2023-05-28 23:03:20.000000 tti_dataset_tools-0.1.5/src/tti_dataset_tools/TrackDirection.py
--rw-r--r--   0        0        0     6615 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.5/src/tti_dataset_tools/TrajectoryCleaner.py
--rw-r--r--   0        0        0     2017 2023-05-28 23:21:04.000000 tti_dataset_tools-0.1.5/src/tti_dataset_tools/TrajectoryMetaBuilder.py
--rw-r--r--   0        0        0     1215 2023-05-28 23:15:48.000000 tti_dataset_tools-0.1.5/src/tti_dataset_tools/TrajectoryProcessor.py
--rw-r--r--   0        0        0    10468 2023-05-28 23:34:46.000000 tti_dataset_tools-0.1.5/src/tti_dataset_tools/TrajectoryTransformer.py
--rw-r--r--   0        0        0    19265 2023-06-13 05:02:44.000000 tti_dataset_tools-0.1.5/src/tti_dataset_tools/TrajectoryUtils.py
--rw-r--r--   0        0        0     2314 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.5/src/tti_dataset_tools/TrajectoryVisualizer.py
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 tti_dataset_tools-0.1.5/setup.py
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 tti_dataset_tools-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1089 2022-12-16 21:14:46.000000 tti_dataset_tools-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1058 2023-06-13 23:54:22.000000 tti_dataset_tools-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       82 2022-12-16 21:14:46.000000 tti_dataset_tools-0.1.6/README.md
+-rw-r--r--   0        0        0       42 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.6/src/ind_tools/__init__.py
+-rw-r--r--   0        0        0     1471 2023-05-28 23:36:30.000000 tti_dataset_tools-0.1.6/src/ind_tools/IndTransformer.py
+-rw-r--r--   0        0        0      303 2023-05-28 23:13:00.000000 tti_dataset_tools-0.1.6/src/tti_dataset_tools/__init__.py
+-rw-r--r--   0        0        0     1012 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.6/src/tti_dataset_tools/ColMapper.py
+-rw-r--r--   0        0        0     4371 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.6/src/tti_dataset_tools/InfluenceAnalyzer.py
+-rw-r--r--   0        0        0        0 2023-05-04 17:45:58.510000 tti_dataset_tools-0.1.6/src/tti_dataset_tools/models/__init__.py
+-rw-r--r--   0        0        0     6200 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.6/src/tti_dataset_tools/models/CrosswalkModel.py
+-rw-r--r--   0        0        0     1123 2023-05-28 23:07:06.000000 tti_dataset_tools-0.1.6/src/tti_dataset_tools/TrackClass.py
+-rw-r--r--   0        0        0      470 2023-05-28 23:03:20.000000 tti_dataset_tools-0.1.6/src/tti_dataset_tools/TrackDirection.py
+-rw-r--r--   0        0        0     6615 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.6/src/tti_dataset_tools/TrajectoryCleaner.py
+-rw-r--r--   0        0        0     2017 2023-05-28 23:21:04.000000 tti_dataset_tools-0.1.6/src/tti_dataset_tools/TrajectoryMetaBuilder.py
+-rw-r--r--   0        0        0     1215 2023-05-28 23:15:48.000000 tti_dataset_tools-0.1.6/src/tti_dataset_tools/TrajectoryProcessor.py
+-rw-r--r--   0        0        0    10468 2023-05-28 23:34:46.000000 tti_dataset_tools-0.1.6/src/tti_dataset_tools/TrajectoryTransformer.py
+-rw-r--r--   0        0        0    19564 2023-06-13 23:48:18.000000 tti_dataset_tools-0.1.6/src/tti_dataset_tools/TrajectoryUtils.py
+-rw-r--r--   0        0        0     2314 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.6/src/tti_dataset_tools/TrajectoryVisualizer.py
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 tti_dataset_tools-0.1.6/setup.py
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 tti_dataset_tools-0.1.6/PKG-INFO
```

### Comparing `tti_dataset_tools-0.1.5/LICENSE` & `tti_dataset_tools-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tti_dataset_tools-0.1.5/pyproject.toml` & `tti_dataset_tools-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tti-dataset-tools"
-version = "0.1.5"
+version = "0.1.6"
 description = "A set of tools for trajectory dataset transformation, clean-up, and augmentation"
 authors = ["Golam Md Muktadir <muktadir@ucsc.edu>"]
 license = "Mozilla Public License Version 2.0"
 include = [
     "MIT License",
 ]
```

### Comparing `tti_dataset_tools-0.1.5/src/ind_tools/IndTransformer.py` & `tti_dataset_tools-0.1.6/src/ind_tools/IndTransformer.py`

 * *Files identical despite different names*

### Comparing `tti_dataset_tools-0.1.5/src/tti_dataset_tools/ColMapper.py` & `tti_dataset_tools-0.1.6/src/tti_dataset_tools/ColMapper.py`

 * *Files identical despite different names*

### Comparing `tti_dataset_tools-0.1.5/src/tti_dataset_tools/InfluenceAnalyzer.py` & `tti_dataset_tools-0.1.6/src/tti_dataset_tools/InfluenceAnalyzer.py`

 * *Files identical despite different names*

### Comparing `tti_dataset_tools-0.1.5/src/tti_dataset_tools/models/CrosswalkModel.py` & `tti_dataset_tools-0.1.6/src/tti_dataset_tools/models/CrosswalkModel.py`

 * *Files identical despite different names*

### Comparing `tti_dataset_tools-0.1.5/src/tti_dataset_tools/TrackClass.py` & `tti_dataset_tools-0.1.6/src/tti_dataset_tools/TrackClass.py`

 * *Files identical despite different names*

### Comparing `tti_dataset_tools-0.1.5/src/tti_dataset_tools/TrajectoryCleaner.py` & `tti_dataset_tools-0.1.6/src/tti_dataset_tools/TrajectoryCleaner.py`

 * *Files identical despite different names*

### Comparing `tti_dataset_tools-0.1.5/src/tti_dataset_tools/TrajectoryMetaBuilder.py` & `tti_dataset_tools-0.1.6/src/tti_dataset_tools/TrajectoryMetaBuilder.py`

 * *Files identical despite different names*

### Comparing `tti_dataset_tools-0.1.5/src/tti_dataset_tools/TrajectoryProcessor.py` & `tti_dataset_tools-0.1.6/src/tti_dataset_tools/TrajectoryProcessor.py`

 * *Files identical despite different names*

### Comparing `tti_dataset_tools-0.1.5/src/tti_dataset_tools/TrajectoryTransformer.py` & `tti_dataset_tools-0.1.6/src/tti_dataset_tools/TrajectoryTransformer.py`

 * *Files identical despite different names*

### Comparing `tti_dataset_tools-0.1.5/src/tti_dataset_tools/TrajectoryUtils.py` & `tti_dataset_tools-0.1.6/src/tti_dataset_tools/TrajectoryUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -496,8 +496,15 @@
         return Point(x, y)
 
 
     @staticmethod
     def headingX(a, b) -> float:
         direction = (b[0] - a[0], b[1] - a[1])
         angleX = math.degrees(math.atan2(direction[1], direction[0]))
-        return angleX
+        return angleX
+    
+    @staticmethod
+    def shift(points: List[Tuple[float, float]], shift: Tuple[float, float]) -> List[Tuple[float, float]]:
+        shiftedPoints = []
+        for point in points:
+            shiftedPoints.append((point[0] + shift[0], point[1] + shift[1]))
+        return shiftedPoints
```

### Comparing `tti_dataset_tools-0.1.5/src/tti_dataset_tools/TrajectoryVisualizer.py` & `tti_dataset_tools-0.1.6/src/tti_dataset_tools/TrajectoryVisualizer.py`

 * *Files identical despite different names*

### Comparing `tti_dataset_tools-0.1.5/setup.py` & `tti_dataset_tools-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'seaborn>=0.12.1,<0.13.0',
  'shapely>=1.7.1,<1.8.0',
  'tqdm>=4.65.0,<5.0.0',
  'vg>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'tti-dataset-tools',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'A set of tools for trajectory dataset transformation, clean-up, and augmentation',
     'long_description': '# A set of tools for trajectory dataset transformation, clean-up, and augmentation',
     'author': 'Golam Md Muktadir',
     'author_email': 'muktadir@ucsc.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/adhocmaster/TTI-dataset-tools',
```

### Comparing `tti_dataset_tools-0.1.5/PKG-INFO` & `tti_dataset_tools-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tti-dataset-tools
-Version: 0.1.5
+Version: 0.1.6
 Summary: A set of tools for trajectory dataset transformation, clean-up, and augmentation
 Home-page: https://github.com/adhocmaster/TTI-dataset-tools
 License: Mozilla Public License Version 2.0
 Keywords: Trajectory Dataset,Trajectory Analysis,Trajectory Transformation,Trajectory Augmentation
 Author: Golam Md Muktadir
 Author-email: muktadir@ucsc.edu
 Requires-Python: >=3.8.0,<4.0.0
```

