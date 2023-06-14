# Comparing `tmp/agsi-2.1.tar.gz` & `tmp/agsi-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agsi-2.1.tar", last modified: Wed Jun 14 05:54:23 2023, max compression
+gzip compressed data, was "agsi-2.2.tar", last modified: Wed Jun 14 10:44:42 2023, max compression
```

## Comparing `agsi-2.1.tar` & `agsi-2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-14 05:54:23.200138 agsi-2.1/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-26 04:44:18.000000 agsi-2.1/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-14 05:54:23.200138 agsi-2.1/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      190 2023-05-25 15:22:54.000000 agsi-2.1/README.md
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-14 05:54:23.196138 agsi-2.1/agsi/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-25 15:09:48.000000 agsi-2.1/agsi/__init__.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-14 05:54:23.200138 agsi-2.1/agsi/data/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)    15905 2023-06-14 05:53:34.000000 agsi-2.1/agsi/data/FarmData.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-25 15:09:48.000000 agsi-2.1/agsi/data/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     8933 2023-06-13 03:47:37.000000 agsi-2.1/agsi/data/utils.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)  1079850 2023-06-13 11:40:51.000000 agsi-2.1/agsi/demo_V2.ipynb
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-25 15:09:48.000000 agsi-2.1/agsi/main.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-25 15:09:48.000000 agsi-2.1/agsi/requirements.txt
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-14 05:54:23.200138 agsi-2.1/agsi.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-14 05:54:23.000000 agsi-2.1/agsi.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-06-14 05:54:23.000000 agsi-2.1/agsi.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-06-14 05:54:23.000000 agsi-2.1/agsi.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-06-14 05:54:23.000000 agsi-2.1/agsi.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-06-14 05:54:23.000000 agsi-2.1/agsi.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-06-14 05:54:23.200138 agsi-2.1/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-06-14 05:53:44.000000 agsi-2.1/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-14 10:44:42.476124 agsi-2.2/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-26 04:44:18.000000 agsi-2.2/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-14 10:44:42.476124 agsi-2.2/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      190 2023-05-25 15:22:54.000000 agsi-2.2/README.md
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-14 10:44:42.476124 agsi-2.2/agsi/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-25 15:09:48.000000 agsi-2.2/agsi/__init__.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-14 10:44:42.476124 agsi-2.2/agsi/data/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)    15905 2023-06-14 10:42:50.000000 agsi-2.2/agsi/data/FarmData.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-25 15:09:48.000000 agsi-2.2/agsi/data/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     8979 2023-06-14 10:44:20.000000 agsi-2.2/agsi/data/utils.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)  1079850 2023-06-13 11:40:51.000000 agsi-2.2/agsi/demo_V2.ipynb
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-25 15:09:48.000000 agsi-2.2/agsi/main.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-25 15:09:48.000000 agsi-2.2/agsi/requirements.txt
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-14 10:44:42.476124 agsi-2.2/agsi.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-14 10:44:42.000000 agsi-2.2/agsi.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-06-14 10:44:42.000000 agsi-2.2/agsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-06-14 10:44:42.000000 agsi-2.2/agsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-06-14 10:44:42.000000 agsi-2.2/agsi.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-06-14 10:44:42.000000 agsi-2.2/agsi.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-06-14 10:44:42.476124 agsi-2.2/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-06-14 10:44:36.000000 agsi-2.2/setup.py
```

### Comparing `agsi-2.1/agsi/data/FarmData.py` & `agsi-2.2/agsi/data/FarmData.py`

 * *Files identical despite different names*

### Comparing `agsi-2.1/agsi/data/utils.py` & `agsi-2.2/agsi/data/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,22 +31,22 @@
             file_path (str): The path to the raster image file.
             polygon (shapely.geometry.Polygon): The polygon shape to clip the raster.
 
         Returns:
             numpy.ndarray: The clipped raster image as a NumPy array.
 
     """
-  
     with rasterio.open(file_path) as src:
         out_image, out_transform = rasterio.mask.mask(src,polygon, crop=True)
         out_meta = src.meta
 
     out_meta.update({"driver": "GTiff",
                     "height": out_image.shape[1],
                     "width": out_image.shape[2],
+                    "count": out_image.shape[0],
                     "transform": out_transform})   
 
     clipped_raster=array_to_raster(out_image,out_meta)
 
     return clipped_raster
 
 def array_to_raster(array,meta):
```

### Comparing `agsi-2.1/agsi/demo_V2.ipynb` & `agsi-2.2/agsi/demo_V2.ipynb`

 * *Files identical despite different names*

