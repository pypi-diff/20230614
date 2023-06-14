# Comparing `tmp/segment-lidar-0.1.4.tar.gz` & `tmp/segment-lidar-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\segment-lidar-0.1.4.tar", last modified: Fri Jun  9 21:11:49 2023, max compression
+gzip compressed data, was "segment-lidar-0.1.5.tar", last modified: Tue Jun 13 23:59:52 2023, max compression
```

## Comparing `segment-lidar-0.1.4.tar` & `segment-lidar-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 21:11:49.054980 segment-lidar-0.1.4/
--rw-rw-rw-   0        0        0     1246 2023-06-09 11:49:11.000000 segment-lidar-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     6986 2023-06-09 21:11:49.053978 segment-lidar-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     6442 2023-06-09 20:03:51.000000 segment-lidar-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 21:11:49.017983 segment-lidar-0.1.4/segment_lidar/
--rw-rw-rw-   0        0        0        0 2023-06-06 11:35:39.000000 segment-lidar-0.1.4/segment_lidar/__init__.py
--rw-rw-rw-   0        0        0    11013 2023-06-09 21:10:01.000000 segment-lidar-0.1.4/segment_lidar/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:11:49.052979 segment-lidar-0.1.4/segment_lidar.egg-info/
--rw-rw-rw-   0        0        0     6986 2023-06-09 21:11:48.000000 segment-lidar-0.1.4/segment_lidar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-06-09 21:11:48.000000 segment-lidar-0.1.4/segment_lidar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 21:11:48.000000 segment-lidar-0.1.4/segment_lidar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-09 21:11:48.000000 segment-lidar-0.1.4/segment_lidar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      156 2023-06-09 21:11:48.000000 segment-lidar-0.1.4/segment_lidar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-09 21:11:48.000000 segment-lidar-0.1.4/segment_lidar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 21:11:49.055977 segment-lidar-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      944 2023-06-09 21:10:50.000000 segment-lidar-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 23:59:52.776556 segment-lidar-0.1.5/
+-rw-rw-rw-   0        0        0     1246 2023-06-09 11:49:11.000000 segment-lidar-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     4885 2023-06-13 23:59:52.774556 segment-lidar-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4341 2023-06-13 23:53:42.000000 segment-lidar-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 23:59:52.724613 segment-lidar-0.1.5/segment_lidar/
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:35:39.000000 segment-lidar-0.1.5/segment_lidar/__init__.py
+-rw-rw-rw-   0        0        0    19008 2023-06-13 23:44:39.000000 segment-lidar-0.1.5/segment_lidar/samlidar.py
+drwxrwxrwx   0        0        0        0 2023-06-13 23:59:52.772608 segment-lidar-0.1.5/segment_lidar.egg-info/
+-rw-rw-rw-   0        0        0     4885 2023-06-13 23:59:52.000000 segment-lidar-0.1.5/segment_lidar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-06-13 23:59:52.000000 segment-lidar-0.1.5/segment_lidar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 23:59:52.000000 segment-lidar-0.1.5/segment_lidar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      170 2023-06-13 23:59:52.000000 segment-lidar-0.1.5/segment_lidar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-13 23:59:52.000000 segment-lidar-0.1.5/segment_lidar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 23:59:52.776556 segment-lidar-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2023-06-13 23:17:14.000000 segment-lidar-0.1.5/setup.py
```

### Comparing `segment-lidar-0.1.4/LICENSE` & `segment-lidar-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-lidar-0.1.4/PKG-INFO` & `segment-lidar-0.1.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-lidar
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.
 Home-page: https://github.com/Yarroudh/segment-lidar
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: BSD 3-Clause "New" or "Revised" License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -14,24 +14,24 @@
 
 <img src="https://user-images.githubusercontent.com/72500344/210864557-4078754f-86c1-4e7c-b291-73223bdf4e4d.png" alt="logo" width="200"/>
 
 # segment-lidar
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/Yarroudh/ZRect3D/blob/main/LICENSE)
 [![Geomatics Unit of ULiege - Development](https://img.shields.io/badge/Geomatics_Unit_of_ULiege-Development-2ea44f)](http://geomatics.ulg.ac.be/)
 
-*Python CLI for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta Research.*
+*Python package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta Research.*
 
 This package is specifically designed for **unsupervised instance segmentation** of **aerial LiDAR data**. It brings together the power of the **Segment-Anything Model (SAM)** developed by [Meta Research](https://github.com/facebookresearch) and the **segment-geospatial** package from [Open Geospatial Solutions](https://github.com/opengeos). Whether you're a researcher, developer, or a geospatial enthusiast, segment-lidar opens up new possibilities for automatic processing of aerial LiDAR data and enables further applications. We encourage you to explore our code, contribute to its development and leverage its capabilities for your segmentation tasks.
 
 ![results](https://github.com/Yarroudh/segment-lidar/assets/72500344/1ed9c405-a305-46ff-827b-a70275733371)
 
 
 ## Installation
 
-We recommand using `python==3.9`. First, you need to install `PyTorch`. Please follow the instructions [here](https://pytorch.org/).
+We recommand using `Python 3.9`. First, you need to install `PyTorch`. Please follow the instructions [here](https://pytorch.org/).
 
 Then, you can easily install `segment-lidar` from [PyPI](https://pypi.org/project/segment-lidar/):
 
 ```bash
 pip install segment-lidar
 ```
 
@@ -39,116 +39,53 @@
 
 ```bash
 git clone https://github.com/Yarroudh/segment-lidar
 cd segment-lidar
 python setup.py install
 ```
 
-## Usage of the package
+Please, note that the actual version is a pre-release and it's under tests. If you find any issues or bugs, please report them in [issues](https://github.com/Yarroudh/segment-lidar/issues) section. The second version will have more advanced features and fonctionalities.
 
-After installation, you have a small program called <code>segment-lidar</code>. Use <code>segment-lidar --help</code> to see the detailed help:
 
-```
-Usage: segment-lidar [OPTIONS] COMMAND [ARGS]...
-
-  A package for segmenting LiDAR data using Segment-Anything from Meta AI
-  Research.
-
-Options:
-  --help  Show this message and exit.
-
-Commands:
-  create-config  Create a configuration YAML file.
-  segment        Segment LiDAR data.
-```
-
-The package reads `.las` or `.laz` file, then perform instance segmentation using [segment-geospatial](https://github.com/opengeos/segment-geospatial) or/and [segment-anything](https://github.com/facebookresearch/segment-anything) algorithms. The user should first create the **configuration** file by running:
+## Documentation
 
-```bash
-segment-lidar create-config -o config.yaml
-```
+If you are using `segment-lidar`, we highly recommend that you take the time to read the [documentation](segment-lidar.readthedocs.io). The documentation is an essential resource that will help you understand the features and functionality of our software, as well as provide guidance on how to use it effectively.
 
-This will create a configuration file as follow:
+## Basic tutorial
 
-```yaml
-algorithm: segment-geospatial
-classification: null
-csf_filter: true
-csf_params:
-  class_threshold: 0.5
-  cloth_resolution: 0.2
-  interations: 500
-  slope_smooth: false
-device: cuda:0
-image_path: raster.tif
-input_path: pointcloud.las
-model_path: sam_vit_h_4b8939.pth
-model_type: vit_h
-output_path: classified.las
-resolution: 0.15
-sam_geo:
-  automatic: true
-  box_threshold: 0.24
-  erosion_kernel_size: 3
-  sam_kwargs: true
-  text_prompt: null
-  text_threshold: 0.3
-sam_kwargs:
-  crop_n_layers: 1
-  crop_n_points_downscale_factor: 1
-  min_mask_region_area: 1000
-  points_per_side: 32
-  pred_iou_thresh: 0.95
-  stability_score_thresh: 0.92
-```
+A basic tutorial is available [here]().
+You can also refer to API for more information about different parameters.
 
-The second step is to run the segmentation:
+```python
+from segment_lidar import samlidar
 
-```bash
-segment-lidar segment --config config.yaml
+model = samlidar.SamLidar(ckpt_path="sam_vit_h_4b8939.pth")
+points = model.read("pointcloud.las")
+cloud, non_ground, ground = model.csf(points)
+labels, *_ = instance.segment(points=cloud, image_path="raster.tif", labels_path="labeled.tif")
+model.write(points=points, non_ground=non_ground, ground=ground, segment_ids=labels, save_path="segmented.las")
 ```
 
-The resulted point cloud contains a new scalar field called `segment_id`. For visualization and further processing, we recommand using [CloudCompare](https://www.danielgm.net/cc/).
-
-## Testing data
+## Sample data
 
 For testing purposes, you can download a sample here: [pointcloud.las](https://drive.google.com/file/d/16EF2aRSvo8u0pXvwtaQ6sjhP5h0sWw3o/view?usp=sharing).
 
 This data was retrieved from **AHN-4**. For more data, please visit [AHN-Viewer](https://ahn.arcgisonline.nl/ahnviewer/)
 
-## Configuration
-
-- `algorithm`: algorithm to use for instance segmentation [segment-geospatial/segment-anything].
-- `model_path`: path of the model checkpoints. See **segment-anything** repository for models.
-- `model_type`: SAM model version [**vit_h/vit_l/vit_b**].
-- `device`: if **cpu** the prediction will use the CPU, if you have cuda, use **cuda:0** instead for GPU.
-- `input_path`: path to your input **.las/.laz** file.
-- `output_path`: path to your output .las/.laz file. The results will be saved in this file.
-- `image_path`: path to the resulted image. The segmentation results of SAM or segment-geospatial will be saved in this file.
-- `classification`: specify the class number you want to segment. This will limit instance segmentation to specified **class**.
-- `csf_filter`: apply ground filtering using cloth simulation filter.
-- `csf_params`: refer to [Cloth Simulation Filer](http://ramm.bnu.edu.cn/projects/CSF) for additional information.
-- `resolution`: resolution of the image created from the point cloud.
-- `sam_kwargs`: refer to **segment-anything** for additional information.
-- `sam_geo`: refer to **segment-geospatial** for additional information.
-
-Please note that the actual version is a pre-release and it's under tests. If you find any issues or bugs, please report them in [issues](https://github.com/Yarroudh/segment-lidar/issues) section. The second version will have more advanced features and fonctionalities.
 
 ## Related repositories
 
 We would like to express our acknowledgments to the creators of:
 
 - [segment-anything](https://github.com/facebookresearch/segment-anything)
 - [segment-geospatial](https://github.com/opengeos/segment-geospatial)
 
-## Documentation
-
-Coming soon.
+Please, visit these repositories for more information about image automatic segmentation using SAM from Meta AI.
 
 ## License
 
 This software is under the BSD 3-Clause "New" or "Revised" license which is a permissive license that allows you almost unlimited freedom with the software so long as you include the BSD copyright and license notice in it. Please refer to the [LICENSE](https://github.com/Yarroudh/segment-lidar/blob/main/LICENSE) file for more detailed information.
 
 ## Author
 
-This software was developped by [Anass Yarroudh](https://www.linkedin.com/in/anass-yarroudh/), a Research Engineer in the [Geomatics Unit of the University of Liege](http://geomatics.ulg.ac.be/fr/home.php).
+This software was developped by [Anass Yarroudh](https://www.linkedin.com/in/anass-yarroudh/), a Research Engineer in the [Geomatics Unit of University of Liege](http://geomatics.ulg.ac.be/fr/home.php).
 For more detailed information please contact us via <ayarroudh@uliege.be>, we are pleased to send you the necessary information.
```

### Comparing `segment-lidar-0.1.4/README.md` & `segment-lidar-0.1.5/segment_lidar.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,37 @@
+Metadata-Version: 2.1
+Name: segment-lidar
+Version: 0.1.5
+Summary: A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.
+Home-page: https://github.com/Yarroudh/segment-lidar
+Author: Anass Yarroudh
+Author-email: ayarroudh@uliege.be
+License: BSD 3-Clause "New" or "Revised" License
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <img src="https://user-images.githubusercontent.com/72500344/210864557-4078754f-86c1-4e7c-b291-73223bdf4e4d.png" alt="logo" width="200"/>
 
 # segment-lidar
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/Yarroudh/ZRect3D/blob/main/LICENSE)
 [![Geomatics Unit of ULiege - Development](https://img.shields.io/badge/Geomatics_Unit_of_ULiege-Development-2ea44f)](http://geomatics.ulg.ac.be/)
 
-*Python CLI for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta Research.*
+*Python package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta Research.*
 
 This package is specifically designed for **unsupervised instance segmentation** of **aerial LiDAR data**. It brings together the power of the **Segment-Anything Model (SAM)** developed by [Meta Research](https://github.com/facebookresearch) and the **segment-geospatial** package from [Open Geospatial Solutions](https://github.com/opengeos). Whether you're a researcher, developer, or a geospatial enthusiast, segment-lidar opens up new possibilities for automatic processing of aerial LiDAR data and enables further applications. We encourage you to explore our code, contribute to its development and leverage its capabilities for your segmentation tasks.
 
 ![results](https://github.com/Yarroudh/segment-lidar/assets/72500344/1ed9c405-a305-46ff-827b-a70275733371)
 
 
 ## Installation
 
-We recommand using `python==3.9`. First, you need to install `PyTorch`. Please follow the instructions [here](https://pytorch.org/).
+We recommand using `Python 3.9`. First, you need to install `PyTorch`. Please follow the instructions [here](https://pytorch.org/).
 
 Then, you can easily install `segment-lidar` from [PyPI](https://pypi.org/project/segment-lidar/):
 
 ```bash
 pip install segment-lidar
 ```
 
@@ -25,116 +39,53 @@
 
 ```bash
 git clone https://github.com/Yarroudh/segment-lidar
 cd segment-lidar
 python setup.py install
 ```
 
-## Usage of the package
+Please, note that the actual version is a pre-release and it's under tests. If you find any issues or bugs, please report them in [issues](https://github.com/Yarroudh/segment-lidar/issues) section. The second version will have more advanced features and fonctionalities.
 
-After installation, you have a small program called <code>segment-lidar</code>. Use <code>segment-lidar --help</code> to see the detailed help:
 
-```
-Usage: segment-lidar [OPTIONS] COMMAND [ARGS]...
+## Documentation
 
-  A package for segmenting LiDAR data using Segment-Anything from Meta AI
-  Research.
+If you are using `segment-lidar`, we highly recommend that you take the time to read the [documentation](segment-lidar.readthedocs.io). The documentation is an essential resource that will help you understand the features and functionality of our software, as well as provide guidance on how to use it effectively.
 
-Options:
-  --help  Show this message and exit.
+## Basic tutorial
 
-Commands:
-  create-config  Create a configuration YAML file.
-  segment        Segment LiDAR data.
-```
+A basic tutorial is available [here]().
+You can also refer to API for more information about different parameters.
 
-The package reads `.las` or `.laz` file, then perform instance segmentation using [segment-geospatial](https://github.com/opengeos/segment-geospatial) or/and [segment-anything](https://github.com/facebookresearch/segment-anything) algorithms. The user should first create the **configuration** file by running:
+```python
+from segment_lidar import samlidar
 
-```bash
-segment-lidar create-config -o config.yaml
+model = samlidar.SamLidar(ckpt_path="sam_vit_h_4b8939.pth")
+points = model.read("pointcloud.las")
+cloud, non_ground, ground = model.csf(points)
+labels, *_ = instance.segment(points=cloud, image_path="raster.tif", labels_path="labeled.tif")
+model.write(points=points, non_ground=non_ground, ground=ground, segment_ids=labels, save_path="segmented.las")
 ```
 
-This will create a configuration file as follow:
-
-```yaml
-algorithm: segment-geospatial
-classification: null
-csf_filter: true
-csf_params:
-  class_threshold: 0.5
-  cloth_resolution: 0.2
-  interations: 500
-  slope_smooth: false
-device: cuda:0
-image_path: raster.tif
-input_path: pointcloud.las
-model_path: sam_vit_h_4b8939.pth
-model_type: vit_h
-output_path: classified.las
-resolution: 0.15
-sam_geo:
-  automatic: true
-  box_threshold: 0.24
-  erosion_kernel_size: 3
-  sam_kwargs: true
-  text_prompt: null
-  text_threshold: 0.3
-sam_kwargs:
-  crop_n_layers: 1
-  crop_n_points_downscale_factor: 1
-  min_mask_region_area: 1000
-  points_per_side: 32
-  pred_iou_thresh: 0.95
-  stability_score_thresh: 0.92
-```
-
-The second step is to run the segmentation:
-
-```bash
-segment-lidar segment --config config.yaml
-```
-
-The resulted point cloud contains a new scalar field called `segment_id`. For visualization and further processing, we recommand using [CloudCompare](https://www.danielgm.net/cc/).
-
-## Testing data
+## Sample data
 
 For testing purposes, you can download a sample here: [pointcloud.las](https://drive.google.com/file/d/16EF2aRSvo8u0pXvwtaQ6sjhP5h0sWw3o/view?usp=sharing).
 
 This data was retrieved from **AHN-4**. For more data, please visit [AHN-Viewer](https://ahn.arcgisonline.nl/ahnviewer/)
 
-## Configuration
-
-- `algorithm`: algorithm to use for instance segmentation [segment-geospatial/segment-anything].
-- `model_path`: path of the model checkpoints. See **segment-anything** repository for models.
-- `model_type`: SAM model version [**vit_h/vit_l/vit_b**].
-- `device`: if **cpu** the prediction will use the CPU, if you have cuda, use **cuda:0** instead for GPU.
-- `input_path`: path to your input **.las/.laz** file.
-- `output_path`: path to your output .las/.laz file. The results will be saved in this file.
-- `image_path`: path to the resulted image. The segmentation results of SAM or segment-geospatial will be saved in this file.
-- `classification`: specify the class number you want to segment. This will limit instance segmentation to specified **class**.
-- `csf_filter`: apply ground filtering using cloth simulation filter.
-- `csf_params`: refer to [Cloth Simulation Filer](http://ramm.bnu.edu.cn/projects/CSF) for additional information.
-- `resolution`: resolution of the image created from the point cloud.
-- `sam_kwargs`: refer to **segment-anything** for additional information.
-- `sam_geo`: refer to **segment-geospatial** for additional information.
-
-Please note that the actual version is a pre-release and it's under tests. If you find any issues or bugs, please report them in [issues](https://github.com/Yarroudh/segment-lidar/issues) section. The second version will have more advanced features and fonctionalities.
 
 ## Related repositories
 
 We would like to express our acknowledgments to the creators of:
 
 - [segment-anything](https://github.com/facebookresearch/segment-anything)
 - [segment-geospatial](https://github.com/opengeos/segment-geospatial)
 
-## Documentation
-
-Coming soon.
+Please, visit these repositories for more information about image automatic segmentation using SAM from Meta AI.
 
 ## License
 
 This software is under the BSD 3-Clause "New" or "Revised" license which is a permissive license that allows you almost unlimited freedom with the software so long as you include the BSD copyright and license notice in it. Please refer to the [LICENSE](https://github.com/Yarroudh/segment-lidar/blob/main/LICENSE) file for more detailed information.
 
 ## Author
 
-This software was developped by [Anass Yarroudh](https://www.linkedin.com/in/anass-yarroudh/), a Research Engineer in the [Geomatics Unit of the University of Liege](http://geomatics.ulg.ac.be/fr/home.php).
-For more detailed information please contact us via <ayarroudh@uliege.be>, we are pleased to send you the necessary information.
+This software was developped by [Anass Yarroudh](https://www.linkedin.com/in/anass-yarroudh/), a Research Engineer in the [Geomatics Unit of University of Liege](http://geomatics.ulg.ac.be/fr/home.php).
+For more detailed information please contact us via <ayarroudh@uliege.be>, we are pleased to send you the necessary information.
```

