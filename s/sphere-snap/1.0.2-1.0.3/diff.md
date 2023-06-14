# Comparing `tmp/sphere_snap-1.0.2-py3-none-any.whl.zip` & `tmp/sphere_snap-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 24419 bytes, number of entries: 13
--rw-r--r--  2.0 unx     3128 b- defN 23-May-06 12:01 sphere_snap/__init__.py
+Zip file size: 24585 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     3128 b- defN 23-Jun-14 14:20 sphere_snap/__init__.py
 -rw-r--r--  2.0 unx     4478 b- defN 23-May-06 10:59 sphere_snap/radial_distortion.py
 -rw-r--r--  2.0 unx     7119 b- defN 23-May-06 10:40 sphere_snap/reprojections.py
 -rw-r--r--  2.0 unx     7348 b- defN 23-May-06 06:04 sphere_snap/snap_config.py
 -rw-r--r--  2.0 unx    12774 b- defN 23-May-03 20:59 sphere_snap/sphere_coor_projections.py
 -rw-r--r--  2.0 unx    22219 b- defN 23-May-06 11:02 sphere_snap/sphere_snap.py
 -rw-r--r--  2.0 unx     7360 b- defN 23-May-05 13:43 sphere_snap/top_view.py
 -rw-r--r--  2.0 unx     7244 b- defN 23-May-06 10:04 sphere_snap/utils.py
--rw-r--r--  2.0 unx     1073 b- defN 23-May-06 12:01 sphere_snap-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     6312 b- defN 23-May-06 12:01 sphere_snap-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-06 12:01 sphere_snap-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-06 12:01 sphere_snap-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1080 b- defN 23-May-06 12:01 sphere_snap-1.0.2.dist-info/RECORD
-13 files, 80239 bytes uncompressed, 22619 bytes compressed:  71.8%
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jun-14 14:23 sphere_snap-1.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6671 b- defN 23-Jun-14 14:23 sphere_snap-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 14:23 sphere_snap-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-14 14:23 sphere_snap-1.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1080 b- defN 23-Jun-14 14:23 sphere_snap-1.0.3.dist-info/RECORD
+13 files, 80598 bytes uncompressed, 22785 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: sphere_snap/top_view.py
 Comment: 
 
 Filename: sphere_snap/utils.py
 Comment: 
 
-Filename: sphere_snap-1.0.2.dist-info/LICENSE
+Filename: sphere_snap-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: sphere_snap-1.0.2.dist-info/METADATA
+Filename: sphere_snap-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: sphere_snap-1.0.2.dist-info/WHEEL
+Filename: sphere_snap-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: sphere_snap-1.0.2.dist-info/top_level.txt
+Filename: sphere_snap-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: sphere_snap-1.0.2.dist-info/RECORD
+Filename: sphere_snap-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `sphere_snap-1.0.2.dist-info/LICENSE` & `sphere_snap-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sphere_snap-1.0.2.dist-info/METADATA` & `sphere_snap-1.0.3.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sphere-snap
-Version: 1.0.2
+Version: 1.0.3
 Summary: A quick and easy to use library for reprojecting various image types
-Home-page: https://androclassic.github.io/SphereSnap/sphere_snap.html
+Home-page: https://github.com/androclassic/SphereSnap
 Author: Andrei Georgescu
 Author-email: andrei.georgescu@yahoo.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -19,32 +19,36 @@
 Requires-Dist: scipy (>=1.5.1)
 Requires-Dist: opencv-python
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: logging
 
 # SphereSnap
-A quick and easy to use library for reprojecting various image types. (inspired by http://paulbourke.net/panorama/sphere2persp/ ) 
+A quick and easy to use library for reprojecting various image types. (inspired by http://paulbourke.net/panorama/sphere2persp/ ).<br />
+The module will use CuPy if detected for accelerating computation. The library can be use simply for reprojecting from one format to another but
+also for more sophisticated usecases of manipulating parts of the image or polygons. 
+
 
 ## Examples and usecases
 ### Reprojecting equirectangular image into pinhole-camera images with customizable FoV and resolution
 <img width="727" alt="image" src="https://user-images.githubusercontent.com/1941529/236621219-457eae8c-ad88-452d-8e89-8b16e4750dd1.jpg">
 <img width="320" alt="image" src="https://user-images.githubusercontent.com/1941529/236621440-5f2fa7f1-b072-4aff-8596-48b236c1d60f.jpg">
 
 ### Create equirectangular image using cubemap faces
 <img width="727" alt="image" src="https://user-images.githubusercontent.com/1941529/236621503-b5cf5e22-6a89-41c1-8765-3c5d23c1df1d.png">
 
 ### Create fisheye images from equirectangular or cubemap images
-<img width="320" alt="image" src="https://user-images.githubusercontent.com/1941529/236621560-cf9f5344-d041-4769-8b86-c52efa2958f6.png">
+<img width="250" alt="image" src="https://user-images.githubusercontent.com/1941529/236621560-cf9f5344-d041-4769-8b86-c52efa2958f6.png">
+<img width="500" alt="image" src="https://user-images.githubusercontent.com/1941529/236662589-e4af0d84-319b-4f10-a118-3a296aa33554.png">
 
 ### Create top view images from equirectangular/fisheye/planar images
-<img width="320" alt="image" src="https://user-images.githubusercontent.com/1941529/236621633-4c6b30b5-0141-4a43-95fd-e93409d56d3e.png">
+<img width="850" alt="image" src="https://user-images.githubusercontent.com/1941529/236662421-3854c164-b856-4b1e-9447-e997db5713d3.png">
 
 ### Correct radially distorted images
-<img width="320" alt="image" src="https://user-images.githubusercontent.com/1941529/236621823-a32b57f9-ec4c-4d8c-b45d-f5cda1dbaecc.png">
+<img width="600" alt="image" src="https://user-images.githubusercontent.com/1941529/236621823-a32b57f9-ec4c-4d8c-b45d-f5cda1dbaecc.png">
 
 
 ## How to use it
 
 Module sphere_snap.reprojections contains easy to use functions for simple situations: 
 - equi2cubemap
 - cubemap2equi
```

## Comparing `sphere_snap-1.0.2.dist-info/RECORD` & `sphere_snap-1.0.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 sphere_snap/radial_distortion.py,sha256=WmN9nJggfSEgI7q3ouPnPTTXcQmKPixdj_172pE9hTk,4478
 sphere_snap/reprojections.py,sha256=OIaG_z7VmJXEitAMIehm5M-OUlhaV7XPIrwGYY6Ag4c,7119
 sphere_snap/snap_config.py,sha256=_MgDpGefyI3cCOpUCkDyJ7VizMwrHU8KG8diGunezP4,7348
 sphere_snap/sphere_coor_projections.py,sha256=bBcHT-pkCXVwxuYE6vYMbf8lbyOHJ2zrVg4p24Sbgu4,12774
 sphere_snap/sphere_snap.py,sha256=5bElb1kS1JQaVccIOAg53gBh0duGSDB83hx2jX01R7E,22219
 sphere_snap/top_view.py,sha256=s4M0MaqRMd237VoIEPqgGWdlTXX83RpTkRc7WJ6vosU,7360
 sphere_snap/utils.py,sha256=uIVvJgaDbHnmfk8z1X1VZvFa3UpE0-2sSTW5pCsZfdI,7244
-sphere_snap-1.0.2.dist-info/LICENSE,sha256=HQNXCkSWMaajqkPgo5zBC8aIMlMoYtL55T5BmutAHkg,1073
-sphere_snap-1.0.2.dist-info/METADATA,sha256=hX933eYT15SHVh8PE3SlDEl5eG8BcaJrk7rc6NR0Uu0,6312
-sphere_snap-1.0.2.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sphere_snap-1.0.2.dist-info/top_level.txt,sha256=06UAvfkOXmuJahsoPhi4MwozdWVascHcxeObJ8isH2c,12
-sphere_snap-1.0.2.dist-info/RECORD,,
+sphere_snap-1.0.3.dist-info/LICENSE,sha256=HQNXCkSWMaajqkPgo5zBC8aIMlMoYtL55T5BmutAHkg,1073
+sphere_snap-1.0.3.dist-info/METADATA,sha256=EoTJ93uLtm9bKjKqfDHMpSjtdL2SAP0Xvzozn-_rzeM,6671
+sphere_snap-1.0.3.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sphere_snap-1.0.3.dist-info/top_level.txt,sha256=06UAvfkOXmuJahsoPhi4MwozdWVascHcxeObJ8isH2c,12
+sphere_snap-1.0.3.dist-info/RECORD,,
```

