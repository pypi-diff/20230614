# Comparing `tmp/spatial-moto-0.0.5.tar.gz` & `tmp/spatial-moto-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatial-moto-0.0.5.tar", last modified: Wed Jun 14 13:16:52 2023, max compression
+gzip compressed data, was "spatial-moto-0.0.6.tar", last modified: Wed Jun 14 13:21:31 2023, max compression
```

## Comparing `spatial-moto-0.0.5.tar` & `spatial-moto-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 13:16:52.266220 spatial-moto-0.0.5/
--rwxrwxrwx   0 walido    (1000) walido    (1000)     1071 2023-06-14 09:31:33.000000 spatial-moto-0.0.5/LICENSE
--rwxrwxrwx   0 walido    (1000) walido    (1000)     1849 2023-06-14 13:16:52.265857 spatial-moto-0.0.5/PKG-INFO
--rwxrwxrwx   0 walido    (1000) walido    (1000)     1115 2023-06-14 13:13:02.000000 spatial-moto-0.0.5/README.md
--rwxrwxrwx   0 walido    (1000) walido    (1000)       38 2023-06-14 13:16:52.266485 spatial-moto-0.0.5/setup.cfg
--rwxrwxrwx   0 walido    (1000) walido    (1000)     1384 2023-06-14 13:15:54.000000 spatial-moto-0.0.5/setup.py
-drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 13:16:52.193664 spatial-moto-0.0.5/spatial_moto.egg-info/
--rwxrwxrwx   0 walido    (1000) walido    (1000)     1849 2023-06-14 13:16:52.000000 spatial-moto-0.0.5/spatial_moto.egg-info/PKG-INFO
--rwxrwxrwx   0 walido    (1000) walido    (1000)      374 2023-06-14 13:16:52.000000 spatial-moto-0.0.5/spatial_moto.egg-info/SOURCES.txt
--rwxrwxrwx   0 walido    (1000) walido    (1000)        1 2023-06-14 13:16:52.000000 spatial-moto-0.0.5/spatial_moto.egg-info/dependency_links.txt
--rwxrwxrwx   0 walido    (1000) walido    (1000)       92 2023-06-14 13:16:52.000000 spatial-moto-0.0.5/spatial_moto.egg-info/requires.txt
--rwxrwxrwx   0 walido    (1000) walido    (1000)       12 2023-06-14 13:16:52.000000 spatial-moto-0.0.5/spatial_moto.egg-info/top_level.txt
-drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 13:16:52.203031 spatial-moto-0.0.5/spatialmoto/
--rwxrwxrwx   0 walido    (1000) walido    (1000)      211 2023-06-14 09:48:03.000000 spatial-moto-0.0.5/spatialmoto/__init__.py
--rwxrwxrwx   0 walido    (1000) walido    (1000)     4990 2023-06-14 09:33:34.000000 spatial-moto-0.0.5/spatialmoto/blocks.py
--rwxrwxrwx   0 walido    (1000) walido    (1000)     2385 2023-06-14 09:31:33.000000 spatial-moto-0.0.5/spatialmoto/clusters.py
-drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 13:16:52.205377 spatial-moto-0.0.5/spatialmoto/data/
--rwxrwxrwx   0 walido    (1000) walido    (1000)  5186120 2023-06-14 09:31:33.000000 spatial-moto-0.0.5/spatialmoto/data/ames.geojson
--rwxrwxrwx   0 walido    (1000) walido    (1000)      225 2023-06-14 10:54:39.000000 spatial-moto-0.0.5/spatialmoto/datasets.py
--rwxrwxrwx   0 walido    (1000) walido    (1000)     2263 2023-06-14 09:31:33.000000 spatial-moto-0.0.5/spatialmoto/plotting.py
--rwxrwxrwx   0 walido    (1000) walido    (1000)     1942 2023-06-14 09:31:33.000000 spatial-moto-0.0.5/spatialmoto/stats.py
+drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 13:21:31.600491 spatial-moto-0.0.6/
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     1071 2023-06-14 09:31:33.000000 spatial-moto-0.0.6/LICENSE
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     1379 2023-06-14 13:21:31.600143 spatial-moto-0.0.6/PKG-INFO
+-rwxrwxrwx   0 walido    (1000) walido    (1000)      686 2023-06-14 13:20:35.000000 spatial-moto-0.0.6/README.md
+-rwxrwxrwx   0 walido    (1000) walido    (1000)       38 2023-06-14 13:21:31.600664 spatial-moto-0.0.6/setup.cfg
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     1385 2023-06-14 13:19:06.000000 spatial-moto-0.0.6/setup.py
+drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 13:21:31.527939 spatial-moto-0.0.6/spatial_moto.egg-info/
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     1379 2023-06-14 13:21:31.000000 spatial-moto-0.0.6/spatial_moto.egg-info/PKG-INFO
+-rwxrwxrwx   0 walido    (1000) walido    (1000)      374 2023-06-14 13:21:31.000000 spatial-moto-0.0.6/spatial_moto.egg-info/SOURCES.txt
+-rwxrwxrwx   0 walido    (1000) walido    (1000)        1 2023-06-14 13:21:31.000000 spatial-moto-0.0.6/spatial_moto.egg-info/dependency_links.txt
+-rwxrwxrwx   0 walido    (1000) walido    (1000)       92 2023-06-14 13:21:31.000000 spatial-moto-0.0.6/spatial_moto.egg-info/requires.txt
+-rwxrwxrwx   0 walido    (1000) walido    (1000)       12 2023-06-14 13:21:31.000000 spatial-moto-0.0.6/spatial_moto.egg-info/top_level.txt
+drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 13:21:31.539508 spatial-moto-0.0.6/spatialmoto/
+-rwxrwxrwx   0 walido    (1000) walido    (1000)      211 2023-06-14 09:48:03.000000 spatial-moto-0.0.6/spatialmoto/__init__.py
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     4990 2023-06-14 09:33:34.000000 spatial-moto-0.0.6/spatialmoto/blocks.py
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     2385 2023-06-14 09:31:33.000000 spatial-moto-0.0.6/spatialmoto/clusters.py
+drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 13:21:31.541689 spatial-moto-0.0.6/spatialmoto/data/
+-rwxrwxrwx   0 walido    (1000) walido    (1000)  5186120 2023-06-14 09:31:33.000000 spatial-moto-0.0.6/spatialmoto/data/ames.geojson
+-rwxrwxrwx   0 walido    (1000) walido    (1000)      225 2023-06-14 10:54:39.000000 spatial-moto-0.0.6/spatialmoto/datasets.py
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     2263 2023-06-14 09:31:33.000000 spatial-moto-0.0.6/spatialmoto/plotting.py
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     1942 2023-06-14 09:31:33.000000 spatial-moto-0.0.6/spatialmoto/stats.py
```

### Comparing `spatial-moto-0.0.5/LICENSE` & `spatial-moto-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spatial-moto-0.0.5/PKG-INFO` & `spatial-moto-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatial-moto
-Version: 0.0.5
+Version: 0.0.6
 Summary: spatial-moto: test 1
 Home-page: https://github.com/WalidGharianiEAGLE/spatial-moto
 Author: Walid Ghariani
 License: MIT
 Keywords: spatial
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -12,34 +12,13 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # spatial-kfold
 spatial resampling for more robust cross validation in spatial studies
 
 spatial-kfold is a python library for performing spatial resampling to ensure more robust cross-validation in spatial studies. It offers spatial clustering and block resampling technique with  user-friendly parameters to customize the resampling. It enables users to conduct a "Leave Region Out" cross-validation, which can be useful for evaluating the model's generalization to new locations as well as improving the reliability of [feature selection](https://doi.org/10.1016/j.ecolmodel.2019.108815) and [hyperparameter tuning](https://doi.org/10.1016/j.ecolmodel.2019.06.002) in spatial studies
-
-
-# Main Features
-
-spatial-kfold allow to conduct "Leave Region Out" using two spatial resampling techniques:
-
-* 1. Spatial clustering with kmeans
-* 2. Spatial blocks
-    * Random blocks
-    * Continuous blocks 
-        * tb-lr : top-bottom, left-right
-        * bt-rl : bottom-top, right-left
-
-# Installation
-
-spatial-kfold can be installed from [PyPI](https://pypi.org/project/spatial-kfold/)
-
-```
-pip install spatial-kfold
-```
```

### Comparing `spatial-moto-0.0.5/README.md` & `spatial-moto-0.0.6/spatial_moto.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
+Metadata-Version: 2.1
+Name: spatial-moto
+Version: 0.0.6
+Summary: spatial-moto: test 1
+Home-page: https://github.com/WalidGharianiEAGLE/spatial-moto
+Author: Walid Ghariani
+License: MIT
+Keywords: spatial
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+License-File: LICENSE
+
 # spatial-kfold
 spatial resampling for more robust cross validation in spatial studies
 
 spatial-kfold is a python library for performing spatial resampling to ensure more robust cross-validation in spatial studies. It offers spatial clustering and block resampling technique with  user-friendly parameters to customize the resampling. It enables users to conduct a "Leave Region Out" cross-validation, which can be useful for evaluating the model's generalization to new locations as well as improving the reliability of [feature selection](https://doi.org/10.1016/j.ecolmodel.2019.108815) and [hyperparameter tuning](https://doi.org/10.1016/j.ecolmodel.2019.06.002) in spatial studies
-
-
-# Main Features
-
-spatial-kfold allow to conduct "Leave Region Out" using two spatial resampling techniques:
-
-* 1. Spatial clustering with kmeans
-* 2. Spatial blocks
-    * Random blocks
-    * Continuous blocks 
-        * tb-lr : top-bottom, left-right
-        * bt-rl : bottom-top, right-left
-
-# Installation
-
-spatial-kfold can be installed from [PyPI](https://pypi.org/project/spatial-kfold/)
-
-```
-pip install spatial-kfold
-```
```

### Comparing `spatial-moto-0.0.5/setup.py` & `spatial-moto-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 
 # Dependencies
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 setup(
     name='spatial-moto',
-    version="0.0.05",
+    version="0.0.06",
     packages=["spatialmoto"],
     author="Walid Ghariani",
     description=("spatial-moto: test 1"),
     long_description=README,
-    long_description_content_type="text/markdown",
+    #long_description_content_type="text/markdown",
     license="MIT",
     keywords="spatial",
     url="https://github.com/WalidGharianiEAGLE/spatial-moto",
 
     #packages=find_packages(),
     package_data={'spatialmoto': ['./data/*.geojson']},
     include_package_data=True,
```

### Comparing `spatial-moto-0.0.5/spatialmoto/blocks.py` & `spatial-moto-0.0.6/spatialmoto/blocks.py`

 * *Files identical despite different names*

### Comparing `spatial-moto-0.0.5/spatialmoto/clusters.py` & `spatial-moto-0.0.6/spatialmoto/clusters.py`

 * *Files identical despite different names*

### Comparing `spatial-moto-0.0.5/spatialmoto/data/ames.geojson` & `spatial-moto-0.0.6/spatialmoto/data/ames.geojson`

 * *Files identical despite different names*

### Comparing `spatial-moto-0.0.5/spatialmoto/plotting.py` & `spatial-moto-0.0.6/spatialmoto/plotting.py`

 * *Files identical despite different names*

### Comparing `spatial-moto-0.0.5/spatialmoto/stats.py` & `spatial-moto-0.0.6/spatialmoto/stats.py`

 * *Files identical despite different names*

