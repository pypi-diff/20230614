# Comparing `tmp/napatrackmater-3.7.4.tar.gz` & `tmp/napatrackmater-3.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-1x1ogdc2/napatrackmater-3.7.4.tar", last modified: Tue Jun 13 21:46:22 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-72j0zqev/napatrackmater-3.7.5.tar", last modified: Tue Jun 13 23:25:37 2023, max compression
```

## Comparing `napatrackmater-3.7.4.tar` & `napatrackmater-3.7.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-13 21:46:22.518399 napatrackmater-3.7.4/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.7.4/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-13 21:46:22.513579 napatrackmater-3.7.4/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.7.4/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-13 21:46:22.318125 napatrackmater-3.7.4/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.7.4/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.7.4/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   110394 2023-06-11 19:02:37.000000 napatrackmater-3.7.4/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.7.4/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.7.4/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13565 2023-06-13 21:44:31.000000 napatrackmater-3.7.4/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.7.4/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.7.4/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.7.4/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-13 21:46:06.000000 napatrackmater-3.7.4/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-13 21:46:22.486838 napatrackmater-3.7.4/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-13 21:46:21.000000 napatrackmater-3.7.4/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-13 21:46:21.000000 napatrackmater-3.7.4/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-13 21:46:21.000000 napatrackmater-3.7.4/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-13 21:46:21.000000 napatrackmater-3.7.4/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-13 21:46:21.000000 napatrackmater-3.7.4/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-13 21:46:21.000000 napatrackmater-3.7.4/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-13 21:46:22.519400 napatrackmater-3.7.4/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.7.4/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-13 23:25:37.663338 napatrackmater-3.7.5/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.7.5/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-13 23:25:37.659569 napatrackmater-3.7.5/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.7.5/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-13 23:25:37.441091 napatrackmater-3.7.5/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.7.5/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.7.5/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   110394 2023-06-11 19:02:37.000000 napatrackmater-3.7.5/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.7.5/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.7.5/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13887 2023-06-13 23:24:15.000000 napatrackmater-3.7.5/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.7.5/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.7.5/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.7.5/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-13 23:25:12.000000 napatrackmater-3.7.5/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-13 23:25:37.625799 napatrackmater-3.7.5/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-13 23:25:36.000000 napatrackmater-3.7.5/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-13 23:25:37.000000 napatrackmater-3.7.5/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-13 23:25:36.000000 napatrackmater-3.7.5/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-13 23:25:36.000000 napatrackmater-3.7.5/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-13 23:25:36.000000 napatrackmater-3.7.5/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-13 23:25:36.000000 napatrackmater-3.7.5/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-13 23:25:37.665863 napatrackmater-3.7.5/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.7.5/setup.py
```

### Comparing `napatrackmater-3.7.4/LICENSE` & `napatrackmater-3.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.4/PKG-INFO` & `napatrackmater-3.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.7.4
+Version: 3.7.5
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.7.4/README.md` & `napatrackmater-3.7.5/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.4/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.7.5/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.4/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.7.5/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.4/napatrackmater/Trackmate.py` & `napatrackmater-3.7.5/napatrackmater/Trackmate.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.4/napatrackmater/Trackvector.py` & `napatrackmater-3.7.5/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.4/napatrackmater/__init__.py` & `napatrackmater-3.7.5/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.4/napatrackmater/clustering.py` & `napatrackmater-3.7.5/napatrackmater/clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,36 +183,39 @@
                                               valid.append(False)      
                             else:
                                   for j in range(len(binary_image.shape)):
                                               valid.append(True)
                                                     
                             if False not in valid:
                                     #Apply the model prediction for getting clusters
-                                    vertices, faces, normals, values = marching_cubes(binary_image)
-                                    mesh_obj = trimesh.Trimesh(
-                                        vertices=vertices, faces=faces, process=False
-                                    )
-                                   
+                                    try:
+                                            vertices, faces, normals, values = marching_cubes(binary_image)
+                                            mesh_obj = trimesh.Trimesh(
+                                                vertices=vertices, faces=faces, process=False
+                                            )
+                                        
 
-                                    mesh_file = str(label) 
-                                    
-                                    with tempfile.TemporaryDirectory() as mesh_dir:
-                                                save_mesh_file = os.path.join(mesh_dir, mesh_file) + ".off"
-                                                mesh_obj.export(save_mesh_file) 
-                                                data = read_off(save_mesh_file)
-                                    
-                                    points = sample_points(data=data, num=num_points).numpy()
-                                    if ndim == 2:
-                                      cloud = get_panda_cloud_xy(points)
-                                    if ndim == 3:
-                                      cloud = get_panda_cloud_xyz(points)  
-                                    else:
-                                      cloud = get_panda_cloud_xyz(points)    
-                                     
-                                    return  label, centroid, cloud       
+                                            mesh_file = str(label) 
+                                            
+                                            with tempfile.TemporaryDirectory() as mesh_dir:
+                                                        save_mesh_file = os.path.join(mesh_dir, mesh_file) + ".off"
+                                                        mesh_obj.export(save_mesh_file) 
+                                                        data = read_off(save_mesh_file)
+                                            
+                                            points = sample_points(data=data, num=num_points).numpy()
+                                            if ndim == 2:
+                                               cloud = get_panda_cloud_xy(points)
+                                            if ndim == 3:
+                                               cloud = get_panda_cloud_xyz(points)  
+                                            else:
+                                               cloud = get_panda_cloud_xyz(points)    
+                                            
+                                            return  label, centroid, cloud
+                                    except ValueError:
+                                            return None       
        
 
 def get_panda_cloud_xy(points):
         
         cloud = PyntCloud(pd.DataFrame(data=points, columns=["x", "y"]))
 
         return cloud
```

### Comparing `napatrackmater-3.7.4/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.7.5/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.4/napatrackmater/fate_mapping.py` & `napatrackmater-3.7.5/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.4/napatrackmater/pretrained.py` & `napatrackmater-3.7.5/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.4/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.7.5/napatrackmater.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.7.4
+Version: 3.7.5
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.7.4/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.7.5/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.4/setup.py` & `napatrackmater-3.7.5/setup.py`

 * *Files identical despite different names*

