# Comparing `tmp/napatrackmater-3.7.6.tar.gz` & `tmp/napatrackmater-3.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-y6wd6ylf/napatrackmater-3.7.6.tar", last modified: Wed Jun 14 05:04:29 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-i54lffzu/napatrackmater-3.7.7.tar", last modified: Wed Jun 14 08:19:56 2023, max compression
```

## Comparing `napatrackmater-3.7.6.tar` & `napatrackmater-3.7.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-14 05:04:29.867462 napatrackmater-3.7.6/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.7.6/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-14 05:04:29.864200 napatrackmater-3.7.6/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.7.6/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-14 05:04:29.708628 napatrackmater-3.7.6/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.7.6/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.7.6/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   110394 2023-06-11 19:02:37.000000 napatrackmater-3.7.6/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.7.6/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.7.6/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    14147 2023-06-14 05:03:33.000000 napatrackmater-3.7.6/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.7.6/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.7.6/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.7.6/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-14 05:03:54.000000 napatrackmater-3.7.6/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-14 05:04:29.833882 napatrackmater-3.7.6/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-14 05:04:29.000000 napatrackmater-3.7.6/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-14 05:04:29.000000 napatrackmater-3.7.6/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-14 05:04:29.000000 napatrackmater-3.7.6/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-14 05:04:29.000000 napatrackmater-3.7.6/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-14 05:04:29.000000 napatrackmater-3.7.6/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-14 05:04:29.000000 napatrackmater-3.7.6/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-14 05:04:29.868462 napatrackmater-3.7.6/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.7.6/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-14 08:19:56.681998 napatrackmater-3.7.7/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.7.7/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-14 08:19:56.675925 napatrackmater-3.7.7/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.7.7/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-14 08:19:56.462034 napatrackmater-3.7.7/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.7.7/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.7.7/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   110394 2023-06-11 19:02:37.000000 napatrackmater-3.7.7/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.7.7/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.7.7/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    14305 2023-06-14 08:19:13.000000 napatrackmater-3.7.7/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.7.7/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.7.7/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.7.7/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-14 08:19:32.000000 napatrackmater-3.7.7/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-14 08:19:56.644260 napatrackmater-3.7.7/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-14 08:19:55.000000 napatrackmater-3.7.7/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-14 08:19:56.000000 napatrackmater-3.7.7/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-14 08:19:55.000000 napatrackmater-3.7.7/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-14 08:19:55.000000 napatrackmater-3.7.7/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-14 08:19:55.000000 napatrackmater-3.7.7/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-14 08:19:55.000000 napatrackmater-3.7.7/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-14 08:19:56.684005 napatrackmater-3.7.7/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.7.7/setup.py
```

### Comparing `napatrackmater-3.7.6/LICENSE` & `napatrackmater-3.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.6/PKG-INFO` & `napatrackmater-3.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.7.6
+Version: 3.7.7
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.7.6/README.md` & `napatrackmater-3.7.7/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.6/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.7.7/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.6/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.7.7/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.6/napatrackmater/Trackmate.py` & `napatrackmater-3.7.7/napatrackmater/Trackmate.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.6/napatrackmater/Trackvector.py` & `napatrackmater-3.7.7/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.6/napatrackmater/__init__.py` & `napatrackmater-3.7.7/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.6/napatrackmater/clustering.py` & `napatrackmater-3.7.7/napatrackmater/clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,24 +200,25 @@
 
                                             mesh_file = str(label) 
                                             
                                             with tempfile.TemporaryDirectory() as mesh_dir:
                                                         save_mesh_file = os.path.join(mesh_dir, mesh_file) + ".off"
                                                         mesh_obj.export(save_mesh_file) 
                                                         data = read_off(save_mesh_file)
-                                            
-                                            points = sample_points(data=data, num=num_points).numpy()
-                                            if ndim == 2:
-                                               cloud = get_panda_cloud_xy(points)
-                                            if ndim == 3:
-                                               cloud = get_panda_cloud_xyz(points)  
-                                            else:
-                                               cloud = get_panda_cloud_xyz(points)    
-                                            
-                                            return  label, centroid, cloud
+                                            pos, face = data["pos"], data["face"]
+                                            if pos.size(1) == 3 and face.size(0) == 3:
+                                                points = sample_points(data=data, num=num_points).numpy()
+                                                if ndim == 2:
+                                                  cloud = get_panda_cloud_xy(points)
+                                                if ndim == 3:
+                                                  cloud = get_panda_cloud_xyz(points)  
+                                                else:
+                                                  cloud = get_panda_cloud_xyz(points)    
+                                                
+                                                return  label, centroid, cloud
                                     
                                                 
        
 
 def get_panda_cloud_xy(points):
         
         cloud = PyntCloud(pd.DataFrame(data=points, columns=["x", "y"]))
```

### Comparing `napatrackmater-3.7.6/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.7.7/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.6/napatrackmater/fate_mapping.py` & `napatrackmater-3.7.7/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.6/napatrackmater/pretrained.py` & `napatrackmater-3.7.7/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.6/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.7.7/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.7.6
+Version: 3.7.7
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.7.6/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.7.7/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.6/setup.py` & `napatrackmater-3.7.7/setup.py`

 * *Files identical despite different names*

