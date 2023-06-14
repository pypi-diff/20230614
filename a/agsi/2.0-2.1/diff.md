# Comparing `tmp/agsi-2.0.tar.gz` & `tmp/agsi-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agsi-2.0.tar", last modified: Tue Jun 13 03:48:47 2023, max compression
+gzip compressed data, was "agsi-2.1.tar", last modified: Wed Jun 14 05:54:23 2023, max compression
```

## Comparing `agsi-2.0.tar` & `agsi-2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-13 03:48:47.972014 agsi-2.0/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-26 04:44:18.000000 agsi-2.0/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-13 03:48:47.972014 agsi-2.0/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      190 2023-05-25 15:22:54.000000 agsi-2.0/README.md
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-13 03:48:47.972014 agsi-2.0/agsi/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-25 15:09:48.000000 agsi-2.0/agsi/__init__.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-13 03:48:47.972014 agsi-2.0/agsi/data/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)    15761 2023-06-12 10:27:05.000000 agsi-2.0/agsi/data/FarmData.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-25 15:09:48.000000 agsi-2.0/agsi/data/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     8933 2023-06-13 03:47:37.000000 agsi-2.0/agsi/data/utils.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)  1079849 2023-06-12 10:26:58.000000 agsi-2.0/agsi/demo_V2.ipynb
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-25 15:09:48.000000 agsi-2.0/agsi/main.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-25 15:09:48.000000 agsi-2.0/agsi/requirements.txt
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-13 03:48:47.972014 agsi-2.0/agsi.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-13 03:48:47.000000 agsi-2.0/agsi.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-06-13 03:48:47.000000 agsi-2.0/agsi.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-06-13 03:48:47.000000 agsi-2.0/agsi.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-06-13 03:48:47.000000 agsi-2.0/agsi.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-06-13 03:48:47.000000 agsi-2.0/agsi.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-06-13 03:48:47.972014 agsi-2.0/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-06-13 03:48:40.000000 agsi-2.0/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-14 05:54:23.200138 agsi-2.1/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-26 04:44:18.000000 agsi-2.1/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-14 05:54:23.200138 agsi-2.1/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      190 2023-05-25 15:22:54.000000 agsi-2.1/README.md
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-14 05:54:23.196138 agsi-2.1/agsi/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-25 15:09:48.000000 agsi-2.1/agsi/__init__.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-14 05:54:23.200138 agsi-2.1/agsi/data/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)    15905 2023-06-14 05:53:34.000000 agsi-2.1/agsi/data/FarmData.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-25 15:09:48.000000 agsi-2.1/agsi/data/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     8933 2023-06-13 03:47:37.000000 agsi-2.1/agsi/data/utils.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)  1079850 2023-06-13 11:40:51.000000 agsi-2.1/agsi/demo_V2.ipynb
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-25 15:09:48.000000 agsi-2.1/agsi/main.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-25 15:09:48.000000 agsi-2.1/agsi/requirements.txt
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-14 05:54:23.200138 agsi-2.1/agsi.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-14 05:54:23.000000 agsi-2.1/agsi.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-06-14 05:54:23.000000 agsi-2.1/agsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-06-14 05:54:23.000000 agsi-2.1/agsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-06-14 05:54:23.000000 agsi-2.1/agsi.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-06-14 05:54:23.000000 agsi-2.1/agsi.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-06-14 05:54:23.200138 agsi-2.1/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-06-14 05:53:44.000000 agsi-2.1/setup.py
```

### Comparing `agsi-2.0/agsi/data/FarmData.py` & `agsi-2.1/agsi/data/FarmData.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,17 @@
       if self.info['data_path'][timestamp][modality_type]!="":
          if shp_clip:            
             shp_file=self.info['shp']
             block_image_path=self.info['data_path'][timestamp][modality_type]
             if modality_type.startswith("drone_"):
               crs="epsg:32644"
             else:
-              crs="epsg:3857"
+              crs_x=str(open_tiff(block_image_path).profile['crs']).lower()
+              crs=crs_x.split("epsg:")[1].lstrip("(").rstrip(")")
+              crs=f"epsg:{crs}"
             block_polygon=open_shp(shp_file,crs)['geometry'].values[0]
             clipped_chip=get_clipped_chip(block_image_path,[block_polygon])
             return clipped_chip
          else:
             image_path=self.info['data_path'][timestamp][modality_type]
             return open_tiff(image_path)        
       else:
```

### Comparing `agsi-2.0/agsi/data/utils.py` & `agsi-2.1/agsi/data/utils.py`

 * *Files identical despite different names*

### Comparing `agsi-2.0/agsi/demo_V2.ipynb` & `agsi-2.1/agsi/demo_V2.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993965517241379%*

 * *Differences: {"'cells'": "{0: {'execution_count': 11, 'source': {insert: [(2, 'from agsi import FarmData\\n'), "*

 * *            "(3, '#from data.FarmData import FarmData\\n')], delete: [3, 2]}}}"}*

```diff
@@ -1,19 +1,19 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
                 "import os, sys\n",
-                "#from agsi import FarmData\n",
-                "from data.FarmData import FarmData\n",
+                "from agsi import FarmData\n",
+                "#from data.FarmData import FarmData\n",
                 "from rasterio.plot import show\n",
                 "import rasterio\n",
                 "from data.utils import convert_path\n",
                 "from pprint import pprint"
             ]
         },
         {
```

