# Comparing `tmp/sports2d-0.2.4.tar.gz` & `tmp/sports2d-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sports2d-0.2.4.tar", last modified: Mon Jun 12 12:28:29 2023, max compression
+gzip compressed data, was "sports2d-0.2.5.tar", last modified: Wed Jun 14 08:16:27 2023, max compression
```

## Comparing `sports2d-0.2.4.tar` & `sports2d-0.2.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:28:29.396700 sports2d-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-12 12:28:17.000000 sports2d-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-06-12 12:28:29.396700 sports2d-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-06-12 12:28:17.000000 sports2d-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:28:29.388700 sports2d-0.2.4/Sports2D/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:28:29.388700 sports2d-0.2.4/Sports2D/Demo/
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Demo/Config_demo.toml
--rw-r--r--   0 runner    (1001) docker     (123)  2539508 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Demo/demo.mp4
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Sports2D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:28:29.392700 sports2d-0.2.4/Sports2D/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Utilities/Blazepose_runsave.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Utilities/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Utilities/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Utilities/skeletons.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Utilities/test_with_blazepose.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21951 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/compute_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)    24282 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/detect_pose.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 12:28:17.000000 sports2d-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-12 12:28:29.396700 sports2d-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-12 12:28:17.000000 sports2d-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:28:29.396700 sports2d-0.2.4/sports2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-06-12 12:28:29.000000 sports2d-0.2.4/sports2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-12 12:28:29.000000 sports2d-0.2.4/sports2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:28:29.000000 sports2d-0.2.4/sports2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:28:29.000000 sports2d-0.2.4/sports2d.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-12 12:28:29.000000 sports2d-0.2.4/sports2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 12:28:29.000000 sports2d-0.2.4/sports2d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:16:27.681594 sports2d-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-14 08:16:15.000000 sports2d-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-06-14 08:16:27.681594 sports2d-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-06-14 08:16:15.000000 sports2d-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:16:27.677594 sports2d-0.2.5/Sports2D/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:16:27.677594 sports2d-0.2.5/Sports2D/Demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-06-14 08:16:15.000000 sports2d-0.2.5/Sports2D/Demo/Config_demo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)  2539508 2023-06-14 08:16:15.000000 sports2d-0.2.5/Sports2D/Demo/demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-14 08:16:15.000000 sports2d-0.2.5/Sports2D/Sports2D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:16:27.681594 sports2d-0.2.5/Sports2D/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-06-14 08:16:15.000000 sports2d-0.2.5/Sports2D/Utilities/Blazepose_runsave.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-14 08:16:15.000000 sports2d-0.2.5/Sports2D/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-14 08:16:15.000000 sports2d-0.2.5/Sports2D/Utilities/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-14 08:16:15.000000 sports2d-0.2.5/Sports2D/Utilities/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-06-14 08:16:15.000000 sports2d-0.2.5/Sports2D/Utilities/skeletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-14 08:16:15.000000 sports2d-0.2.5/Sports2D/Utilities/test_with_blazepose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-14 08:16:15.000000 sports2d-0.2.5/Sports2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21951 2023-06-14 08:16:15.000000 sports2d-0.2.5/Sports2D/compute_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24295 2023-06-14 08:16:15.000000 sports2d-0.2.5/Sports2D/detect_pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-14 08:16:15.000000 sports2d-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-14 08:16:27.681594 sports2d-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-14 08:16:15.000000 sports2d-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:16:27.681594 sports2d-0.2.5/sports2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-06-14 08:16:27.000000 sports2d-0.2.5/sports2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-14 08:16:27.000000 sports2d-0.2.5/sports2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:16:27.000000 sports2d-0.2.5/sports2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:16:27.000000 sports2d-0.2.5/sports2d.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-14 08:16:27.000000 sports2d-0.2.5/sports2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 08:16:27.000000 sports2d-0.2.5/sports2d.egg-info/top_level.txt
```

### Comparing `sports2d-0.2.4/LICENSE` & `sports2d-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.4/PKG-INFO` & `sports2d-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.2.4
+Version: 0.2.5
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
 Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics,sports,sports-analytics
@@ -39,15 +39,15 @@
 [![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
 [![status](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26/status.svg)](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26)
 -->
 
 
 # Sports2D
 
-**`Sports2D` lets you compute 2D joint positions, as well as joint and segment angles from a video.**
+**`Sports2D` automatically computes 2D joint positions, as well as joint and segment angles from a video.**
 
 </br>
 
 **`Announcement:` \
 User-friendly Colab version released!\
 Works on any smartphone!**\
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://bit.ly/Sports2D_Colab)
@@ -77,15 +77,19 @@
 
 
 ## Installation and Demonstration
 
 ### Installation
 
 - OPTION 0: **Use Colab** \
-  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://bit.ly/Sports2D_Colab)
+  User-friendly (but full) version, also works on a phone or a tablet.\
+  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://bit.ly/Sports2D_Colab)\
+  YouTube tutorial:\
+  <a href = "https://www.youtube.com/watch?v=Er5RpcJ8o1Y"><img src="Content/Video_tuto_Sports2D_Colab.png" width="380"></a>
+  
 
 
 - OPTION 1: **Quick install** \
     Open a terminal. Type `python -V` to make sure python '>=3.7 <=3.10' is installed, and then:
     ```
     pip install sports2d
     ```
```

### Comparing `sports2d-0.2.4/README.md` & `sports2d-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
 [![status](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26/status.svg)](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26)
 -->
 
 
 # Sports2D
 
-**`Sports2D` lets you compute 2D joint positions, as well as joint and segment angles from a video.**
+**`Sports2D` automatically computes 2D joint positions, as well as joint and segment angles from a video.**
 
 </br>
 
 **`Announcement:` \
 User-friendly Colab version released!\
 Works on any smartphone!**\
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://bit.ly/Sports2D_Colab)
@@ -50,15 +50,19 @@
 
 
 ## Installation and Demonstration
 
 ### Installation
 
 - OPTION 0: **Use Colab** \
-  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://bit.ly/Sports2D_Colab)
+  User-friendly (but full) version, also works on a phone or a tablet.\
+  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://bit.ly/Sports2D_Colab)\
+  YouTube tutorial:\
+  <a href = "https://www.youtube.com/watch?v=Er5RpcJ8o1Y"><img src="Content/Video_tuto_Sports2D_Colab.png" width="380"></a>
+  
 
 
 - OPTION 1: **Quick install** \
     Open a terminal. Type `python -V` to make sure python '>=3.7 <=3.10' is installed, and then:
     ```
     pip install sports2d
     ```
```

### Comparing `sports2d-0.2.4/Sports2D/Demo/Config_demo.toml` & `sports2d-0.2.5/Sports2D/Demo/Config_demo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
    	
 	
 
 # ADVANCED CONFIGURATION
 	
 [pose_advanced] # only for OPENPOSE
-load_pose = true # If true, don't run openpose again if json pose files are found. If false, run it and overwrite pose files. 
+overwrite_pose = false # If false, don't run openpose again if json pose files are found. 
 save_vid = true
 save_img = true
 interp_gap_smaller_than = 5 # do not interpolate bigger gaps
 filter = true
 show_plots = false
 filter_type = 'butterworth' # butterworth, gaussian, LOESS, median
    [pose_advanced.butterworth]
```

### Comparing `sports2d-0.2.4/Sports2D/Demo/demo.mp4` & `sports2d-0.2.5/Sports2D/Demo/demo.mp4`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.4/Sports2D/Sports2D.py` & `sports2d-0.2.5/Sports2D/Sports2D.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.4/Sports2D/Utilities/Blazepose_runsave.py` & `sports2d-0.2.5/Sports2D/Utilities/Blazepose_runsave.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.4/Sports2D/Utilities/common.py` & `sports2d-0.2.5/Sports2D/Utilities/common.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.4/Sports2D/Utilities/filter.py` & `sports2d-0.2.5/Sports2D/Utilities/filter.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.4/Sports2D/Utilities/skeletons.py` & `sports2d-0.2.5/Sports2D/Utilities/skeletons.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.4/Sports2D/compute_angles.py` & `sports2d-0.2.5/Sports2D/compute_angles.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.4/Sports2D/detect_pose.py` & `sports2d-0.2.5/Sports2D/detect_pose.py`

 * *Files 1% similar despite different names*

```diff
@@ -544,15 +544,15 @@
     '''
     
     # Retrieve parameters
     root_dir = os.getcwd()
     video_dir, video_file, result_dir, frame_rate = base_params(config_dict)
     pose_algo = config_dict.get('pose').get('pose_algo')
     
-    load_pose = config_dict.get('pose_advanced').get('load_pose')
+    load_pose = not config_dict.get('pose_advanced').get('overwrite_pose')
     save_vid = config_dict.get('pose_advanced').get('save_vid')
     save_img = config_dict.get('pose_advanced').get('save_img')
     interp_gap_smaller_than = config_dict.get('pose_advanced').get('interp_gap_smaller_than')
     
     show_plots = config_dict.get('pose_advanced').get('show_plots')
     do_filter = config_dict.get('pose_advanced').get('filter')
     filter_type = config_dict.get('pose_advanced').get('filter_type')
@@ -569,15 +569,15 @@
 
     if pose_algo == 'OPENPOSE':
         pose_model = config_dict.get('pose').get('OPENPOSE').get('openpose_model')
         json_path = result_dir / '_'.join((video_file_stem,pose_model,'json'))
 
         # Pose detection skipped if load existing json files
         if load_pose and len(list(json_path.glob('*')))>0:
-            logging.info(f'2D joint positions have already been detected. To run the analysis over again from the beginning, set "load_pose" to false in Advanced pose settings.')
+            logging.info(f'2D joint positions have already been detected. To run the analysis over again from the beginning, set "overwrite_pose" to true in Advanced pose settings.')
             pass
         else:
             logging.info(f'Detecting 2D joint positions with OpenPose model {pose_model}, for {video_file}.')
             json_path.mkdir(parents=True, exist_ok=True)
             openpose_path = config_dict.get('pose').get('OPENPOSE').get('openpose_path')
             os.chdir(openpose_path)
             if platform =="win32":
```

### Comparing `sports2d-0.2.4/setup.cfg` & `sports2d-0.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sports2d
-version = 0.2.4
+version = 0.2.5
 author = David Pagnon
 author_email = contact@david-pagnon.com
 description = Detect pose and compute 2D joint angles from a video.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/davidpagnon/Sports2D
 keywords = markerless, kinematics, OpenPose, BlazePose, joint angles, 2D, biomechanics, sports, sports-analytics
```

### Comparing `sports2d-0.2.4/sports2d.egg-info/PKG-INFO` & `sports2d-0.2.5/sports2d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.2.4
+Version: 0.2.5
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
 Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics,sports,sports-analytics
@@ -39,15 +39,15 @@
 [![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
 [![status](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26/status.svg)](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26)
 -->
 
 
 # Sports2D
 
-**`Sports2D` lets you compute 2D joint positions, as well as joint and segment angles from a video.**
+**`Sports2D` automatically computes 2D joint positions, as well as joint and segment angles from a video.**
 
 </br>
 
 **`Announcement:` \
 User-friendly Colab version released!\
 Works on any smartphone!**\
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://bit.ly/Sports2D_Colab)
@@ -77,15 +77,19 @@
 
 
 ## Installation and Demonstration
 
 ### Installation
 
 - OPTION 0: **Use Colab** \
-  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://bit.ly/Sports2D_Colab)
+  User-friendly (but full) version, also works on a phone or a tablet.\
+  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://bit.ly/Sports2D_Colab)\
+  YouTube tutorial:\
+  <a href = "https://www.youtube.com/watch?v=Er5RpcJ8o1Y"><img src="Content/Video_tuto_Sports2D_Colab.png" width="380"></a>
+  
 
 
 - OPTION 1: **Quick install** \
     Open a terminal. Type `python -V` to make sure python '>=3.7 <=3.10' is installed, and then:
     ```
     pip install sports2d
     ```
```

### Comparing `sports2d-0.2.4/sports2d.egg-info/SOURCES.txt` & `sports2d-0.2.5/sports2d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

