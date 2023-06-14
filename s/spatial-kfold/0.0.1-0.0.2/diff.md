# Comparing `tmp/spatial-kfold-0.0.1.tar.gz` & `tmp/spatial-kfold-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatial-kfold-0.0.1.tar", last modified: Sun Mar 26 21:24:16 2023, max compression
+gzip compressed data, was "spatial-kfold-0.0.2.tar", last modified: Wed Jun 14 15:06:43 2023, max compression
```

## Comparing `spatial-kfold-0.0.1.tar` & `spatial-kfold-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-03-26 21:24:16.475586 spatial-kfold-0.0.1/
--rwxrwxrwx   0 walido    (1000) walido    (1000)     1427 2023-03-26 21:24:16.474915 spatial-kfold-0.0.1/PKG-INFO
--rwxrwxrwx   0 walido    (1000) walido    (1000)      685 2023-03-20 08:17:17.000000 spatial-kfold-0.0.1/README.md
--rwxrwxrwx   0 walido    (1000) walido    (1000)       38 2023-03-26 21:24:16.475899 spatial-kfold-0.0.1/setup.cfg
--rwxrwxrwx   0 walido    (1000) walido    (1000)     1416 2023-03-26 21:20:47.000000 spatial-kfold-0.0.1/setup.py
-drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-03-26 21:24:16.218032 spatial-kfold-0.0.1/spatial_kfold.egg-info/
--rwxrwxrwx   0 walido    (1000) walido    (1000)     1427 2023-03-26 21:24:16.000000 spatial-kfold-0.0.1/spatial_kfold.egg-info/PKG-INFO
--rwxrwxrwx   0 walido    (1000) walido    (1000)      380 2023-03-26 21:24:16.000000 spatial-kfold-0.0.1/spatial_kfold.egg-info/SOURCES.txt
--rwxrwxrwx   0 walido    (1000) walido    (1000)        1 2023-03-26 21:24:16.000000 spatial-kfold-0.0.1/spatial_kfold.egg-info/dependency_links.txt
--rwxrwxrwx   0 walido    (1000) walido    (1000)       92 2023-03-26 21:24:16.000000 spatial-kfold-0.0.1/spatial_kfold.egg-info/requires.txt
--rwxrwxrwx   0 walido    (1000) walido    (1000)       13 2023-03-26 21:24:16.000000 spatial-kfold-0.0.1/spatial_kfold.egg-info/top_level.txt
-drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-03-26 21:24:16.316723 spatial-kfold-0.0.1/spatialkfold/
--rwxrwxrwx   0 walido    (1000) walido    (1000)      228 2023-03-26 21:16:41.000000 spatial-kfold-0.0.1/spatialkfold/__init__.py
--rwxrwxrwx   0 walido    (1000) walido    (1000)     6267 2023-03-20 09:18:28.000000 spatial-kfold-0.0.1/spatialkfold/blocks.py
--rwxrwxrwx   0 walido    (1000) walido    (1000)     2385 2023-03-20 04:50:52.000000 spatial-kfold-0.0.1/spatialkfold/clusters.py
-drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-03-26 21:24:16.318117 spatial-kfold-0.0.1/spatialkfold/data/
--rwxrwxrwx   0 walido    (1000) walido    (1000)  5186120 2022-12-20 19:07:12.000000 spatial-kfold-0.0.1/spatialkfold/data/ames.geojson
--rwxrwxrwx   0 walido    (1000) walido    (1000)      225 2023-03-26 21:10:21.000000 spatial-kfold-0.0.1/spatialkfold/dataloader.py
--rwxrwxrwx   0 walido    (1000) walido    (1000)     2263 2023-03-26 21:08:31.000000 spatial-kfold-0.0.1/spatialkfold/plotting.py
--rwxrwxrwx   0 walido    (1000) walido    (1000)     1942 2022-12-28 08:16:18.000000 spatial-kfold-0.0.1/spatialkfold/stats.py
+drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 15:06:43.456875 spatial-kfold-0.0.2/
+-rwxrwxrwx   0 walido    (1000) walido    (1000)    35149 2023-06-14 14:55:26.000000 spatial-kfold-0.0.2/LICENSE
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     1557 2023-06-14 15:06:43.456507 spatial-kfold-0.0.2/PKG-INFO
+-rwxrwxrwx   0 walido    (1000) walido    (1000)      687 2023-06-14 15:05:23.000000 spatial-kfold-0.0.2/README.md
+-rwxrwxrwx   0 walido    (1000) walido    (1000)       38 2023-06-14 15:06:43.457033 spatial-kfold-0.0.2/setup.cfg
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     1520 2023-06-14 14:56:02.000000 spatial-kfold-0.0.2/setup.py
+drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 15:06:43.385046 spatial-kfold-0.0.2/spatial_kfold.egg-info/
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     1557 2023-06-14 15:06:43.000000 spatial-kfold-0.0.2/spatial_kfold.egg-info/PKG-INFO
+-rwxrwxrwx   0 walido    (1000) walido    (1000)      386 2023-06-14 15:06:43.000000 spatial-kfold-0.0.2/spatial_kfold.egg-info/SOURCES.txt
+-rwxrwxrwx   0 walido    (1000) walido    (1000)        1 2023-06-14 15:06:43.000000 spatial-kfold-0.0.2/spatial_kfold.egg-info/dependency_links.txt
+-rwxrwxrwx   0 walido    (1000) walido    (1000)       92 2023-06-14 15:06:43.000000 spatial-kfold-0.0.2/spatial_kfold.egg-info/requires.txt
+-rwxrwxrwx   0 walido    (1000) walido    (1000)       13 2023-06-14 15:06:43.000000 spatial-kfold-0.0.2/spatial_kfold.egg-info/top_level.txt
+drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 15:06:43.393673 spatial-kfold-0.0.2/spatialkfold/
+-rwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 13:29:50.000000 spatial-kfold-0.0.2/spatialkfold/__init__.py
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     4990 2023-06-14 09:33:34.000000 spatial-kfold-0.0.2/spatialkfold/blocks.py
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     2384 2023-06-14 13:30:40.000000 spatial-kfold-0.0.2/spatialkfold/clusters.py
+drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 15:06:43.395665 spatial-kfold-0.0.2/spatialkfold/data/
+-rwxrwxrwx   0 walido    (1000) walido    (1000)  5186120 2023-06-14 09:31:33.000000 spatial-kfold-0.0.2/spatialkfold/data/ames.geojson
+-rwxrwxrwx   0 walido    (1000) walido    (1000)      225 2023-06-14 13:25:03.000000 spatial-kfold-0.0.2/spatialkfold/datasets.py
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     2263 2023-06-14 09:31:33.000000 spatial-kfold-0.0.2/spatialkfold/plotting.py
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     1942 2023-06-14 09:31:33.000000 spatial-kfold-0.0.2/spatialkfold/stats.py
```

### Comparing `spatial-kfold-0.0.1/PKG-INFO` & `spatial-kfold-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: spatial-kfold
-Version: 0.0.1
+Version: 0.0.2
 Summary: spatial-kfold: A Python Package for Spatial Resampling Toward More Reliable Cross-Validation in Spatial Studies.
 Home-page: https://github.com/WalidGharianiEAGLE/spatial-kfold
 Author: Walid Ghariani
 Author-email: walid11ghariani@gmail.com
-License: MIT
+License: GPL-3.0
 Keywords: cross-validation,machine-learning,GIS,spatial
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
+License-File: LICENSE
 
 # spatial-kfold
+
 spatial resampling for more robust cross validation in spatial studies
 
-spatial-kfold is a python library for performing spatial resampling to ensure more robust cross-validation in spatial studies. It offers spatial clustering and block resampling technique with  user-friendly parameters to customize the resampling. It enables users to conduct a "Leave Region Out" cross-validation, which can be useful for evaluating the model's generalization to new locations as well as improving the reliability of [feature selection](https://doi.org/10.1016/j.ecolmodel.2019.108815) and [hyperparameter tuning](https://doi.org/10.1016/j.ecolmodel.2019.06.002) in spatial studies
+spatial-kfold is a python library for performing spatial resampling to ensure more robust cross-validation in spatial studies. It offers spatial clustering and block resampling technique with  user-friendly parameters to customize the resampling. It enables users to conduct a "Leave Region Out" cross-validation, which can be useful for evaluating the model's generalization to new locations as well as improving the reliability of [feature selection](https://doi.org/10.1016/j.ecolmodel.2019.108815) and [hyperparameter tuning](https://doi.org/10.1016/j.ecolmodel.2019.06.002) in spatial studies.
```

### Comparing `spatial-kfold-0.0.1/README.md` & `spatial-kfold-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,4 +1,5 @@
 # spatial-kfold
+
 spatial resampling for more robust cross validation in spatial studies
 
-spatial-kfold is a python library for performing spatial resampling to ensure more robust cross-validation in spatial studies. It offers spatial clustering and block resampling technique with  user-friendly parameters to customize the resampling. It enables users to conduct a "Leave Region Out" cross-validation, which can be useful for evaluating the model's generalization to new locations as well as improving the reliability of [feature selection](https://doi.org/10.1016/j.ecolmodel.2019.108815) and [hyperparameter tuning](https://doi.org/10.1016/j.ecolmodel.2019.06.002) in spatial studies
+spatial-kfold is a python library for performing spatial resampling to ensure more robust cross-validation in spatial studies. It offers spatial clustering and block resampling technique with  user-friendly parameters to customize the resampling. It enables users to conduct a "Leave Region Out" cross-validation, which can be useful for evaluating the model's generalization to new locations as well as improving the reliability of [feature selection](https://doi.org/10.1016/j.ecolmodel.2019.108815) and [hyperparameter tuning](https://doi.org/10.1016/j.ecolmodel.2019.06.002) in spatial studies.
```

### Comparing `spatial-kfold-0.0.1/setup.py` & `spatial-kfold-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 # Dependencies
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 setup(
     name='spatial-kfold',
-    version="0.0.01",
+    version="0.0.02",
     packages=["spatialkfold"],
     author="Walid Ghariani",
     author_email="walid11ghariani@gmail.com",
     description=("spatial-kfold: A Python Package for Spatial Resampling Toward More Reliable Cross-Validation in Spatial Studies."),
     long_description=README,
-    license="MIT",
+    license="GPL-3.0",
     keywords="cross-validation, machine-learning, GIS, spatial",
     url="https://github.com/WalidGharianiEAGLE/spatial-kfold",
 
     #packages=find_packages(),
     package_data={'spatialkfold': ['./data/*.geojson']},
     include_package_data=True,
 
@@ -36,13 +36,15 @@
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 
     # testing
     setup_requires=['pytest-runner'],
     tests_require=['pytest']
 )
```

### Comparing `spatial-kfold-0.0.1/spatial_kfold.egg-info/PKG-INFO` & `spatial-kfold-0.0.2/spatial_kfold.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: spatial-kfold
-Version: 0.0.1
+Version: 0.0.2
 Summary: spatial-kfold: A Python Package for Spatial Resampling Toward More Reliable Cross-Validation in Spatial Studies.
 Home-page: https://github.com/WalidGharianiEAGLE/spatial-kfold
 Author: Walid Ghariani
 Author-email: walid11ghariani@gmail.com
-License: MIT
+License: GPL-3.0
 Keywords: cross-validation,machine-learning,GIS,spatial
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
+License-File: LICENSE
 
 # spatial-kfold
+
 spatial resampling for more robust cross validation in spatial studies
 
-spatial-kfold is a python library for performing spatial resampling to ensure more robust cross-validation in spatial studies. It offers spatial clustering and block resampling technique with  user-friendly parameters to customize the resampling. It enables users to conduct a "Leave Region Out" cross-validation, which can be useful for evaluating the model's generalization to new locations as well as improving the reliability of [feature selection](https://doi.org/10.1016/j.ecolmodel.2019.108815) and [hyperparameter tuning](https://doi.org/10.1016/j.ecolmodel.2019.06.002) in spatial studies
+spatial-kfold is a python library for performing spatial resampling to ensure more robust cross-validation in spatial studies. It offers spatial clustering and block resampling technique with  user-friendly parameters to customize the resampling. It enables users to conduct a "Leave Region Out" cross-validation, which can be useful for evaluating the model's generalization to new locations as well as improving the reliability of [feature selection](https://doi.org/10.1016/j.ecolmodel.2019.108815) and [hyperparameter tuning](https://doi.org/10.1016/j.ecolmodel.2019.06.002) in spatial studies.
```

### Comparing `spatial-kfold-0.0.1/spatialkfold/blocks.py` & `spatial-kfold-0.0.2/spatialkfold/blocks.py`

 * *Files 18% similar despite different names*

```diff
@@ -118,47 +118,8 @@
     for i, arr in enumerate(split_blocks):
         arr['folds'] = i +1
         blocks_list.append(arr)
     
     # Set as Create a geodataframe
     blocks_folds_gdf = gpd.GeoDataFrame(pd.concat(blocks_list))
     
-    return blocks_folds_gdf
-
-def spatial_kfold_blocks (gdf, gdf_blocks):
-    
-    """
-    Return a GeoDataFrame with folds by intersecting the spatial blocks wih the spatial points.
-    
-    Parameters
-    ----------
-    gdf : GeoDataFrame
-        The base GeoDataFrame to intersect with `gdf_blocks`.
-    gdf_blocks : GeoDataFrame
-        The GeoDataFrame to intersect with `gdf` to create folds.
-        
-    Returns
-    -------
-    GeoDataFrame
-        A GeoDataFrame with folds created by intersecting `gdf` and `gdf_blocks`.
-    
-    Raises
-    ------
-    TypeError
-        If either `gdf` or `gdf_blocks` is not a GeoDataFrame.
-    AttributeError
-        If `gdf` and `gdf_blocks` have different CRS.
-    """
-        
-    # Check that the input is a GeoDataFrame
-    if not isinstance(gdf, gpd.GeoDataFrame):
-        raise TypeError('Input must be a GeoDataFrame')
-    if not isinstance(gdf_blocks, gpd.GeoDataFrame):
-        raise TypeError('Input must be a GeoDataFrame')
-
-    # Check the crs of the GeoDataFrame
-    if (gdf.crs != gdf_blocks.crs):
-        raise AttributeError('The passed GeoDataFrames have different CRS. Use `to_crs()` to reproject one of the input geometries.')
-        
-    gdf_kfold_blocks = gpd.overlay(gdf, gdf_blocks, how="intersection")
-    
-    return gdf_kfold_blocks
+    return blocks_folds_gdf
```

### Comparing `spatial-kfold-0.0.1/spatialkfold/clusters.py` & `spatial-kfold-0.0.2/spatialkfold/clusters.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -54,8 +54,8 @@
     lon_lat[name] = gdf_sp[name]
     
     lon_lat_valid = lon_lat[[name, 'folds']]
     
     # assign the folds-clusters to the original gdf 
     gdf_kfold_clusters = gdf.merge(lon_lat_valid, on= name, how='left')
     
-    return gdf_kfold_clusters
+    return gdf_kfold_clusters
```

### Comparing `spatial-kfold-0.0.1/spatialkfold/data/ames.geojson` & `spatial-kfold-0.0.2/spatialkfold/data/ames.geojson`

 * *Files identical despite different names*

### Comparing `spatial-kfold-0.0.1/spatialkfold/plotting.py` & `spatial-kfold-0.0.2/spatialkfold/plotting.py`

 * *Files identical despite different names*

### Comparing `spatial-kfold-0.0.1/spatialkfold/stats.py` & `spatial-kfold-0.0.2/spatialkfold/stats.py`

 * *Files identical despite different names*

