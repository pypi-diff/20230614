# Comparing `tmp/segment-geospatial-0.8.0.tar.gz` & `tmp/segment-geospatial-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-geospatial-0.8.0.tar", last modified: Wed May 24 04:08:45 2023, max compression
+gzip compressed data, was "segment-geospatial-0.8.1.tar", last modified: Thu May 25 01:13:33 2023, max compression
```

## Comparing `segment-geospatial-0.8.0.tar` & `segment-geospatial-0.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 04:08:45.937092 segment-geospatial-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-05-24 04:08:45.937092 segment-geospatial-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 04:08:45.937092 segment-geospatial-0.8.0/samgeo/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/samgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    82805 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/samgeo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    29816 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/samgeo/samgeo.py
--rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/samgeo/text_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 04:08:45.937092 segment-geospatial-0.8.0/segment_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-05-24 04:08:45.000000 segment-geospatial-0.8.0/segment_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-24 04:08:45.000000 segment-geospatial-0.8.0/segment_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-24 04:08:45.000000 segment-geospatial-0.8.0/segment_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 04:08:45.000000 segment-geospatial-0.8.0/segment_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-24 04:08:45.000000 segment-geospatial-0.8.0/segment_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 04:08:45.000000 segment-geospatial-0.8.0/segment_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-24 04:08:45.937092 segment-geospatial-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-24 04:08:36.000000 segment-geospatial-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:13:33.887836 segment-geospatial-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-25 01:13:20.000000 segment-geospatial-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 01:13:20.000000 segment-geospatial-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-25 01:13:33.887836 segment-geospatial-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-25 01:13:20.000000 segment-geospatial-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 01:13:20.000000 segment-geospatial-0.8.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:13:33.887836 segment-geospatial-0.8.1/samgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-25 01:13:20.000000 segment-geospatial-0.8.1/samgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82805 2023-05-25 01:13:20.000000 segment-geospatial-0.8.1/samgeo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29816 2023-05-25 01:13:20.000000 segment-geospatial-0.8.1/samgeo/samgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16755 2023-05-25 01:13:20.000000 segment-geospatial-0.8.1/samgeo/text_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:13:33.887836 segment-geospatial-0.8.1/segment_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-25 01:13:33.000000 segment-geospatial-0.8.1/segment_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-25 01:13:33.000000 segment-geospatial-0.8.1/segment_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 01:13:33.000000 segment-geospatial-0.8.1/segment_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 01:13:33.000000 segment-geospatial-0.8.1/segment_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-25 01:13:33.000000 segment-geospatial-0.8.1/segment_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 01:13:33.000000 segment-geospatial-0.8.1/segment_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-25 01:13:33.887836 segment-geospatial-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-25 01:13:20.000000 segment-geospatial-0.8.1/setup.py
```

### Comparing `segment-geospatial-0.8.0/LICENSE` & `segment-geospatial-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.8.0/PKG-INFO` & `segment-geospatial-0.8.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.8.0
+Version: 0.8.1
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -26,22 +26,29 @@
 [![image](https://img.shields.io/badge/Open-Planetary%20Computer-black?style=flat&logo=microsoft)](https://pccompute.westeurope.cloudapp.azure.com/compute/hub/user-redirect/git-pull?repo=https://github.com/opengeos/segment-geospatial&urlpath=lab/tree/segment-geospatial/docs/examples/satellite.ipynb&branch=main)
 [![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
 [![image](https://img.shields.io/pypi/v/segment-geospatial.svg)](https://pypi.python.org/pypi/segment-geospatial)
 [![image](https://img.shields.io/conda/vn/conda-forge/segment-geospatial.svg)](https://anaconda.org/conda-forge/segment-geospatial)
 [![Docker Pulls](https://badgen.net/docker/pulls/giswqs/segment-geospatial?icon=docker&label=pulls)](https://hub.docker.com/r/giswqs/segment-geospatial)
 [![PyPI Downloads](https://static.pepy.tech/badge/segment-geospatial)](https://pepy.tech/project/segment-geospatial)
 [![Conda Downloads](https://anaconda.org/conda-forge/segment-geospatial/badges/downloads.svg)](https://anaconda.org/conda-forge/segment-geospatial)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7966658.svg)](https://doi.org/10.5281/zenodo.7966658)
 
 **A Python package for segmenting geospatial data with the Segment Anything Model (SAM)**
 
+## Introduction
+
 The **segment-geospatial** package draws its inspiration from [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository authored by [Aliaksandr Hancharenka](https://github.com/aliaksandr960). To facilitate the use of the Segment Anything Model (SAM) for geospatial data, I have developed the [segment-anything-py](https://github.com/opengeos/segment-anything) and [segment-geospatial](https://github.com/opengeos/segment-geospatial) Python packages, which are now available on PyPI and conda-forge. My primary objective is to simplify the process of leveraging SAM for geospatial data analysis by enabling users to achieve this with minimal coding effort. I have adapted the source code of segment-geospatial from the [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository, and credit for its original version goes to Aliaksandr Hancharenka.
 
 -   Free software: MIT license
 -   Documentation: <https://samgeo.gishub.org>
 
+## Citations
+
+-   Qiusheng Wu, & Lucas Osco. (2023). samgeo: A Python package for segmenting geospatial data with the Segment Anything Model (SAM). Zenodo. <https://doi.org/10.5281/zenodo.7966658>
+
 ## Features
 
 -   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
 -   Segment GeoTIFF files using the Segment Anything Model (SAM)
 -   Segment remote sensing imagery with text prompts
 -   Create foreground and background markers interactively
 -   Load existing markers from vector datasets
@@ -67,26 +74,34 @@
 
 ![](https://i.imgur.com/2Nyg9uW.gif)
 
 -   Input prompts from existing files
 
 ![](https://i.imgur.com/Cb4ZaKY.gif)
 
+-   Interactive segmentation with text prompts
+
+![](https://i.imgur.com/wydt5Xt.gif)
+
 ## Tutorials
 
 Video tutorials are available on my [YouTube Channel](https://youtube.com/@giswqs).
 
 -   Automatic mask generation
 
 [![Alt text](https://img.youtube.com/vi/YHA_-QMB8_U/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
 
 -   Using SAM with ArcGIS Pro
 
 [![Alt text](https://img.youtube.com/vi/VvyInoQ6N8Q/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
 
+-   Interactive segmentation with text prompts
+
+[![Alt text](https://img.youtube.com/vi/cSDvuv1zRos/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
+
 ## Using SAM with Desktop GIS
 
 -   **QGIS**: Check out the [Geometric Attributes plugin for QGIS](https://github.com/BjornNyberg/Geometric-Attributes-Toolbox/wiki/User-Guide#segment-anything-model). Credit goes to [Bjorn Nyberg](https://github.com/BjornNyberg).
 -   **ArcGIS**: Check out the [Segment Anything Model (SAM) Toolbox for ArcGIS](https://www.arcgis.com/home/item.html?id=9b67b441f29f4ce6810979f5f0667ebe). Credit goes to [Esri](https://www.esri.com).
 
 ## Computing Resources
```

### Comparing `segment-geospatial-0.8.0/README.md` & `segment-geospatial-0.8.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,29 @@
 [![image](https://img.shields.io/badge/Open-Planetary%20Computer-black?style=flat&logo=microsoft)](https://pccompute.westeurope.cloudapp.azure.com/compute/hub/user-redirect/git-pull?repo=https://github.com/opengeos/segment-geospatial&urlpath=lab/tree/segment-geospatial/docs/examples/satellite.ipynb&branch=main)
 [![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
 [![image](https://img.shields.io/pypi/v/segment-geospatial.svg)](https://pypi.python.org/pypi/segment-geospatial)
 [![image](https://img.shields.io/conda/vn/conda-forge/segment-geospatial.svg)](https://anaconda.org/conda-forge/segment-geospatial)
 [![Docker Pulls](https://badgen.net/docker/pulls/giswqs/segment-geospatial?icon=docker&label=pulls)](https://hub.docker.com/r/giswqs/segment-geospatial)
 [![PyPI Downloads](https://static.pepy.tech/badge/segment-geospatial)](https://pepy.tech/project/segment-geospatial)
 [![Conda Downloads](https://anaconda.org/conda-forge/segment-geospatial/badges/downloads.svg)](https://anaconda.org/conda-forge/segment-geospatial)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7966658.svg)](https://doi.org/10.5281/zenodo.7966658)
 
 **A Python package for segmenting geospatial data with the Segment Anything Model (SAM)**
 
+## Introduction
+
 The **segment-geospatial** package draws its inspiration from [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository authored by [Aliaksandr Hancharenka](https://github.com/aliaksandr960). To facilitate the use of the Segment Anything Model (SAM) for geospatial data, I have developed the [segment-anything-py](https://github.com/opengeos/segment-anything) and [segment-geospatial](https://github.com/opengeos/segment-geospatial) Python packages, which are now available on PyPI and conda-forge. My primary objective is to simplify the process of leveraging SAM for geospatial data analysis by enabling users to achieve this with minimal coding effort. I have adapted the source code of segment-geospatial from the [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository, and credit for its original version goes to Aliaksandr Hancharenka.
 
 -   Free software: MIT license
 -   Documentation: <https://samgeo.gishub.org>
 
+## Citations
+
+-   Qiusheng Wu, & Lucas Osco. (2023). samgeo: A Python package for segmenting geospatial data with the Segment Anything Model (SAM). Zenodo. <https://doi.org/10.5281/zenodo.7966658>
+
 ## Features
 
 -   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
 -   Segment GeoTIFF files using the Segment Anything Model (SAM)
 -   Segment remote sensing imagery with text prompts
 -   Create foreground and background markers interactively
 -   Load existing markers from vector datasets
@@ -45,26 +52,34 @@
 
 ![](https://i.imgur.com/2Nyg9uW.gif)
 
 -   Input prompts from existing files
 
 ![](https://i.imgur.com/Cb4ZaKY.gif)
 
+-   Interactive segmentation with text prompts
+
+![](https://i.imgur.com/wydt5Xt.gif)
+
 ## Tutorials
 
 Video tutorials are available on my [YouTube Channel](https://youtube.com/@giswqs).
 
 -   Automatic mask generation
 
 [![Alt text](https://img.youtube.com/vi/YHA_-QMB8_U/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
 
 -   Using SAM with ArcGIS Pro
 
 [![Alt text](https://img.youtube.com/vi/VvyInoQ6N8Q/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
 
+-   Interactive segmentation with text prompts
+
+[![Alt text](https://img.youtube.com/vi/cSDvuv1zRos/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
+
 ## Using SAM with Desktop GIS
 
 -   **QGIS**: Check out the [Geometric Attributes plugin for QGIS](https://github.com/BjornNyberg/Geometric-Attributes-Toolbox/wiki/User-Guide#segment-anything-model). Credit goes to [Bjorn Nyberg](https://github.com/BjornNyberg).
 -   **ArcGIS**: Check out the [Segment Anything Model (SAM) Toolbox for ArcGIS](https://www.arcgis.com/home/item.html?id=9b67b441f29f4ce6810979f5f0667ebe). Credit goes to [Esri](https://www.esri.com).
 
 ## Computing Resources
```

### Comparing `segment-geospatial-0.8.0/samgeo/common.py` & `segment-geospatial-0.8.1/samgeo/common.py`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.8.0/samgeo/samgeo.py` & `segment-geospatial-0.8.1/samgeo/samgeo.py`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.8.0/samgeo/text_sam.py` & `segment-geospatial-0.8.1/samgeo/text_sam.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import warnings
 import argparse
 import numpy as np
 import torch
 from PIL import Image
 from segment_anything import sam_model_registry
 from segment_anything import SamPredictor
+from huggingface_hub import hf_hub_download
 from .common import *
 
 try:
     import rasterio
 except ImportError:
     print("Installing rasterio...")
     install_package("rasterio")
@@ -25,15 +26,15 @@
 try:
     import groundingdino.datasets.transforms as T
     from groundingdino.models import build_model
     from groundingdino.util import box_ops
     from groundingdino.util.inference import predict
     from groundingdino.util.slconfig import SLConfig
     from groundingdino.util.utils import clean_state_dict
-    from huggingface_hub import hf_hub_download
+
 except ImportError:
     print("Installing GroundingDINO...")
     install_package("groundingdino-py")
     print("Please restart the kernel and run the notebook again.")
 
 # Mode checkpoints
 SAM_MODELS = {
```

### Comparing `segment-geospatial-0.8.0/segment_geospatial.egg-info/PKG-INFO` & `segment-geospatial-0.8.1/segment_geospatial.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.8.0
+Version: 0.8.1
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -26,22 +26,29 @@
 [![image](https://img.shields.io/badge/Open-Planetary%20Computer-black?style=flat&logo=microsoft)](https://pccompute.westeurope.cloudapp.azure.com/compute/hub/user-redirect/git-pull?repo=https://github.com/opengeos/segment-geospatial&urlpath=lab/tree/segment-geospatial/docs/examples/satellite.ipynb&branch=main)
 [![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
 [![image](https://img.shields.io/pypi/v/segment-geospatial.svg)](https://pypi.python.org/pypi/segment-geospatial)
 [![image](https://img.shields.io/conda/vn/conda-forge/segment-geospatial.svg)](https://anaconda.org/conda-forge/segment-geospatial)
 [![Docker Pulls](https://badgen.net/docker/pulls/giswqs/segment-geospatial?icon=docker&label=pulls)](https://hub.docker.com/r/giswqs/segment-geospatial)
 [![PyPI Downloads](https://static.pepy.tech/badge/segment-geospatial)](https://pepy.tech/project/segment-geospatial)
 [![Conda Downloads](https://anaconda.org/conda-forge/segment-geospatial/badges/downloads.svg)](https://anaconda.org/conda-forge/segment-geospatial)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7966658.svg)](https://doi.org/10.5281/zenodo.7966658)
 
 **A Python package for segmenting geospatial data with the Segment Anything Model (SAM)**
 
+## Introduction
+
 The **segment-geospatial** package draws its inspiration from [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository authored by [Aliaksandr Hancharenka](https://github.com/aliaksandr960). To facilitate the use of the Segment Anything Model (SAM) for geospatial data, I have developed the [segment-anything-py](https://github.com/opengeos/segment-anything) and [segment-geospatial](https://github.com/opengeos/segment-geospatial) Python packages, which are now available on PyPI and conda-forge. My primary objective is to simplify the process of leveraging SAM for geospatial data analysis by enabling users to achieve this with minimal coding effort. I have adapted the source code of segment-geospatial from the [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository, and credit for its original version goes to Aliaksandr Hancharenka.
 
 -   Free software: MIT license
 -   Documentation: <https://samgeo.gishub.org>
 
+## Citations
+
+-   Qiusheng Wu, & Lucas Osco. (2023). samgeo: A Python package for segmenting geospatial data with the Segment Anything Model (SAM). Zenodo. <https://doi.org/10.5281/zenodo.7966658>
+
 ## Features
 
 -   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
 -   Segment GeoTIFF files using the Segment Anything Model (SAM)
 -   Segment remote sensing imagery with text prompts
 -   Create foreground and background markers interactively
 -   Load existing markers from vector datasets
@@ -67,26 +74,34 @@
 
 ![](https://i.imgur.com/2Nyg9uW.gif)
 
 -   Input prompts from existing files
 
 ![](https://i.imgur.com/Cb4ZaKY.gif)
 
+-   Interactive segmentation with text prompts
+
+![](https://i.imgur.com/wydt5Xt.gif)
+
 ## Tutorials
 
 Video tutorials are available on my [YouTube Channel](https://youtube.com/@giswqs).
 
 -   Automatic mask generation
 
 [![Alt text](https://img.youtube.com/vi/YHA_-QMB8_U/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
 
 -   Using SAM with ArcGIS Pro
 
 [![Alt text](https://img.youtube.com/vi/VvyInoQ6N8Q/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
 
+-   Interactive segmentation with text prompts
+
+[![Alt text](https://img.youtube.com/vi/cSDvuv1zRos/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
+
 ## Using SAM with Desktop GIS
 
 -   **QGIS**: Check out the [Geometric Attributes plugin for QGIS](https://github.com/BjornNyberg/Geometric-Attributes-Toolbox/wiki/User-Guide#segment-anything-model). Credit goes to [Bjorn Nyberg](https://github.com/BjornNyberg).
 -   **ArcGIS**: Check out the [Segment Anything Model (SAM) Toolbox for ArcGIS](https://www.arcgis.com/home/item.html?id=9b67b441f29f4ce6810979f5f0667ebe). Credit goes to [Esri](https://www.esri.com).
 
 ## Computing Resources
```

### Comparing `segment-geospatial-0.8.0/setup.py` & `segment-geospatial-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     keywords="samgeo",
     name="segment-geospatial",
     packages=find_packages(include=["samgeo", "samgeo.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/opengeos/segment-geospatial",
-    version='0.8.0',
+    version='0.8.1',
     zip_safe=False,
 )
```

