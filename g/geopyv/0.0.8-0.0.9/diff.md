# Comparing `tmp/geopyv-0.0.8.tar.gz` & `tmp/geopyv-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geopyv-0.0.8.tar", last modified: Mon Jun  5 12:07:21 2023, max compression
+gzip compressed data, was "geopyv-0.0.9.tar", last modified: Wed Jun  7 15:08:28 2023, max compression
```

## Comparing `geopyv-0.0.8.tar` & `geopyv-0.0.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:07:21.664438 geopyv-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-05 12:07:12.000000 geopyv-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-05 12:07:12.000000 geopyv-0.0.8/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-05 12:07:12.000000 geopyv-0.0.8/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 12:07:12.000000 geopyv-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-05 12:07:21.664438 geopyv-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-05 12:07:12.000000 geopyv-0.0.8/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   167782 2023-06-05 12:07:12.000000 geopyv-0.0.8/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-05 12:07:12.000000 geopyv-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-06-05 12:07:12.000000 geopyv-0.0.8/basictest.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 12:07:12.000000 geopyv-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-05 12:07:21.664438 geopyv-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-05 12:07:12.000000 geopyv-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:07:21.652438 geopyv-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:07:21.660438 geopyv-0.0.8/src/geopyv/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/check.py
--rw-r--r--   0 runner    (1001) docker     (123)    30453 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:07:21.664438 geopyv-0.0.8/src/geopyv/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/geometry/exclusions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/geometry/meshing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/geometry/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:07:21.664438 geopyv-0.0.8/src/geopyv/gui/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:07:21.664438 geopyv-0.0.8/src/geopyv/gui/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/gui/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/gui/selectors/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/gui/selectors/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/gui/selectors/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/gui/selectors/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    71779 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    27589 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    39437 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    49305 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/speckle.py
--rw-r--r--   0 runner    (1001) docker     (123)    22403 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:07:21.664438 geopyv-0.0.8/src/geopyv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-05 12:07:21.000000 geopyv-0.0.8/src/geopyv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-05 12:07:21.000000 geopyv-0.0.8/src/geopyv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:07:21.000000 geopyv-0.0.8/src/geopyv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-05 12:07:21.000000 geopyv-0.0.8/src/geopyv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 12:07:21.000000 geopyv-0.0.8/src/geopyv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:08:28.791661 geopyv-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-07 15:08:16.000000 geopyv-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-07 15:08:16.000000 geopyv-0.0.9/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-07 15:08:16.000000 geopyv-0.0.9/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-07 15:08:16.000000 geopyv-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-07 15:08:28.791661 geopyv-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-07 15:08:16.000000 geopyv-0.0.9/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   167782 2023-06-07 15:08:16.000000 geopyv-0.0.9/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-07 15:08:16.000000 geopyv-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-06-07 15:08:16.000000 geopyv-0.0.9/basictest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-07 15:08:16.000000 geopyv-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 15:08:28.791661 geopyv-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-07 15:08:16.000000 geopyv-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:08:28.783661 geopyv-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:08:28.787661 geopyv-0.0.9/src/geopyv/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31040 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:08:28.791661 geopyv-0.0.9/src/geopyv/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/geometry/meshing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/geometry/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/geometry/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:08:28.791661 geopyv-0.0.9/src/geopyv/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:08:28.791661 geopyv-0.0.9/src/geopyv/gui/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/gui/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/gui/selectors/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/gui/selectors/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/gui/selectors/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/gui/selectors/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72526 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27680 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39437 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44887 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/speckle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22403 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-06-07 15:08:16.000000 geopyv-0.0.9/src/geopyv/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:08:28.787661 geopyv-0.0.9/src/geopyv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-07 15:08:28.000000 geopyv-0.0.9/src/geopyv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-07 15:08:28.000000 geopyv-0.0.9/src/geopyv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:08:28.000000 geopyv-0.0.9/src/geopyv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-07 15:08:28.000000 geopyv-0.0.9/src/geopyv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 15:08:28.000000 geopyv-0.0.9/src/geopyv.egg-info/top_level.txt
```

### Comparing `geopyv-0.0.8/.gitignore` & `geopyv-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/CMakeLists.txt` & `geopyv-0.0.9/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/LICENSE` & `geopyv-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/PKG-INFO` & `geopyv-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geopyv
-Version: 0.0.8
+Version: 0.0.9
 Summary: A PIV/DIC analysis package for Python.
 Author-email: Sam Stanier <sas229@cam.ac.uk>, Jonathan Smith <jdks2@cam.ac.uk>
 Project-URL: Homepage, https://github.com/sas229/geopyv
 Project-URL: Bug Tracker, https://github.com/sas229/geopyv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `geopyv-0.0.8/Pipfile` & `geopyv-0.0.9/Pipfile`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/Pipfile.lock` & `geopyv-0.0.9/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/README.md` & `geopyv-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/basictest.py` & `geopyv-0.0.9/basictest.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 tar = gp.image.Image("./images/T-Bar/IMG_1071.jpg")
 template = gp.templates.Circle(50)
 
 # Subset instantiation.
 subset = gp.subset.Subset(
     f_img=ref, g_img=tar, f_coord=np.asarray([1000, 1000]), template=template
 )
-
 # Subset inspection.
 subset.inspect()
 
 # Subset solving.
 subset.solve()
 
 # Other subset methods.
@@ -30,34 +29,43 @@
 subset = gp.io.load(filename="test")
 
 # Mesh test.
 # Mesh setup.
 ref = gp.image.Image("./images/T-Bar/IMG_1062.jpg")
 tar = gp.image.Image("./images/T-Bar/IMG_1065.jpg")
 template = gp.templates.Circle(50)
-boundary = np.asarray(
-    [[200.0, 200.0], [200.0, 2700.0], [3900.0, 2700.0], [3900.0, 200.0]]
+boundary = gp.geometry.region.Path(
+    boundary=np.asarray(
+        [[200.0, 200.0], [200.0, 2700.0], [3900.0, 2700.0], [3900.0, 200.0]]
+    ),
+    rigid=False,
+    hard=False,
+    track=True,
 )
 exclusions = []
 exclusions.append(
-    gp.geometry.exclusions.circular_exclusion(
-        np.asarray([1925, 1470]), radius=430, size=100
+    gp.geometry.region.Circle(
+        coord=np.asarray([1925, 1470]),
+        radius=430.0,
+        size=100.0,
+        rigid=True,
+        hard=True,
+        track=True,
     )
 )
 seed = np.asarray([400, 400.0])
 alpha = 0.2
 
 # Mesh instantiation.
 mesh = gp.mesh.Mesh(
     f_img=ref,
     g_img=tar,
     target_nodes=1000,
     boundary=boundary,
     exclusions=exclusions,
-    hard_boundary=False,
     subset_size_compensation=True,
     mesh_order=1,
 )
 
 # Mesh inspection.
 # mesh.inspect(subset_index=5000)
 
@@ -69,14 +77,15 @@
     seed_coord=seed,
     template=template,
     adaptive_iterations=3,
     method="ICGN",
     alpha=alpha,
     tolerance=0.7,
 )
+
 # Mesh saving.
 gp.io.save(object=mesh, filename="mesh")
 del mesh
 
 # Mesh loading.
 mesh = gp.io.load(filename="mesh")
 
@@ -119,21 +128,31 @@
 
 # If you supply a subset index that is out of range you get a ValueError.
 # mesh.convergence(subset_index=4000)
 
 # Sequence test.
 # Sequence setup.
 template = gp.templates.Circle(50)
-boundary = np.asarray(
-    [[200.0, 200.0], [200.0, 2700.0], [3900.0, 2700.0], [3900.0, 200.0]]
+boundary = gp.geometry.region.Path(
+    boundary=np.asarray(
+        [[200.0, 200.0], [200.0, 2700.0], [3900.0, 2700.0], [3900.0, 200.0]]
+    ),
+    rigid=False,
+    hard=False,
+    track=True,
 )
 exclusions = []
 exclusions.append(
-    gp.geometry.exclusions.circular_exclusion(
-        np.asarray([1925, 1470]), radius=430, size=100
+    gp.geometry.region.Circle(
+        coord=np.asarray([1925, 1470]),
+        radius=430.0,
+        size=100.0,
+        rigid=True,
+        hard=True,
+        track=True,
     )
 )
 seed = np.asarray([400, 400.0])
 alpha = 0.2
 
 # Sequence instantiation.
 sequence = gp.sequence.Sequence(
@@ -143,15 +162,14 @@
     exclusions=exclusions,
     save_by_reference=True,
     mesh_dir="images/T-Bar/meshes/",
 )
 
 # Sequence solving.
 sequence.solve(
-    track=True,
     seed_coord=seed,
     template=template,
     adaptive_iterations=0,
     method="ICGN",
     alpha=alpha,
     tolerance=0.7,
 )
@@ -213,25 +231,27 @@
 field.inspect()
 
 # Extracting data.
 component = 0
 particle_index = 4
 
 # Coordinates.
-coordinates = field.data["particles"][particle_index]["coordinates"]
+coordinates = field.data["particles"][particle_index]["results"]["coordinates"]
 print(coordinates)
 
 # Warps.
 # Full.
-warps = field.data["particles"][particle_index]["warps"]  # warp components :
+warps = field.data["particles"][particle_index]["results"]["warps"]  # warp components :
 # [u, v, dudx, dudy, dvdx, dvdy, d2udx2, d2udxdy, d2udy2, d2vdx2, d2vdxdy, d2vdy2]
 print(warps)
-warps = field.data["particles"][particle_index]["warps"][
+warps = field.data["particles"][particle_index]["results"]["warps"][
     2:5, :2
 ]  # Time steps 2-5 for components 0 and 1 i.e. displacements.
 print(warps)
 
 # e.g. to extract volume progression. Note, area is in pixels.
-volume_array = field.data["particles"][particle_index]["volumes"]
+volume_array = field.data["particles"][particle_index]["results"]["volumes"]
 print(volume_array)
-volume = field.data["particles"][particle_index]["volumes"][3]  # At time step 3.
+volume = field.data["particles"][particle_index]["results"]["volumes"][
+    3
+]  # At time step 3.
 print(volume)
```

### Comparing `geopyv-0.0.8/pyproject.toml` & `geopyv-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "cmake",
     "ninja"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geopyv"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Sam Stanier", email="sas229@cam.ac.uk" },
   { name="Jonathan Smith", email="jdks2@cam.ac.uk" },
 ]
 description = "A PIV/DIC analysis package for Python."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `geopyv-0.0.8/src/geopyv/__init__.py` & `geopyv-0.0.9/src/geopyv/__init__.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/src/geopyv/calibration.py` & `geopyv-0.0.9/src/geopyv/calibration.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/src/geopyv/check.py` & `geopyv-0.0.9/src/geopyv/check.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/src/geopyv/field.py` & `geopyv-0.0.9/src/geopyv/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -586,21 +586,31 @@
                 self._exclusions = mesh_0["exclusions"]
             self._size_lower_bound = mesh_0["size_lower_bound"]
             self._size_upper_bound = mesh_0["size_upper_bound"]
 
             self._size_upper_bound = min(
                 self._size_upper_bound,
                 np.max(
-                    np.sqrt(np.sum(np.square(np.diff(self._boundary, axis=0)), axis=1))
+                    np.sqrt(
+                        np.sum(
+                            np.square(
+                                np.diff(self._boundary.data["boundaries"][0], axis=0)
+                            ),
+                            axis=1,
+                        )
+                    )
                 ),
             )
 
             # Define region of interest.
+            self._boundary._boundary = self._boundary.data["boundaries"][0]
+            for exclusion in self._exclusions:
+                exclusion._boundary = exclusion.data["boundaries"][0]
             (
-                self._boundary,
+                self._borders,
                 self._segments,
                 self._curves,
                 _,
             ) = gp.geometry.meshing._define_RoI(
                 gp.image.Image(self._image_0),
                 self._boundary,
                 self._exclusions,
@@ -651,15 +661,15 @@
         approximately the desired number of elements.
 
         """
 
         def f(size):
             return self._uniform_remesh(
                 size,
-                self._boundary,
+                self._borders,
                 self._segments,
                 self._curves,
                 self._target_particles,
                 self._size_lower_bound,
                 self._size_upper_bound,
             )
 
@@ -746,21 +756,27 @@
 
         self.data.update({"particles": self._particles, "volumes": self._vol_totals})
         self.solved = True
         self.data["solved"] = self.solved
         return self.solved
 
     def _stress_state(self, stresses):
+        """
+        Private method to define the initial stress state.
+        """
         if np.shape(stresses)[0] == np.shape(self._coordinates)[0]:
             self._stresses = stresses
         elif np.shape(stresses)[0] == 2:
             self._stresses = stresses[0] + (stresses[1] - stresses[0]) * (
                 (
-                    (self._coordinates[:, 1] - np.min(self._boundary[:, 1]))
-                    / (np.max(self._boundary[:, 1]) - np.min(self._boundary[:, 1]))
+                    (self._coordinates[:, 1] - np.min(self._boundary._boundary[:, 1]))
+                    / (
+                        np.max(self._boundary._boundary[:, 1])
+                        - np.min(self._boundary._boundary[:, 1])
+                    )
                 )[:, np.newaxis]
             )
         else:
             self._stresses = np.tile(stresses, (np.shape(self._coordinates)[0], 1))
 
     @staticmethod
     def _uniform_remesh(
```

### Comparing `geopyv-0.0.8/src/geopyv/geometry/meshing.py` & `geopyv-0.0.9/src/geopyv/geometry/meshing.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,63 +19,80 @@
 #         "Generating mesh using gmsh with approximately {n} nodes.".format(
 #             n=self._target_nodes
 #         )
 #     )
 #     _initial_mesh()
 
 
-def _define_RoI(_f_img, _boundary, _exclusions):
+def _define_RoI(f_img, boundary, exclusions):
     """
 
     Private method to define the RoI.
 
     """
 
     # Create binary mask RoI.
     binary_img = ImagePIL.new(
         "L",
-        (np.shape(_f_img.image_gs)[1], np.shape(_f_img.image_gs)[0]),
+        (np.shape(f_img.image_gs)[1], np.shape(f_img.image_gs)[0]),
         0,
     )
-    ImageDrawPIL.Draw(binary_img).polygon(
-        _boundary.flatten().tolist(), outline=1, fill=1
-    )
+    if boundary._hard:
+        ImageDrawPIL.Draw(binary_img).polygon(
+            boundary._boundary.flatten().tolist(), outline=1, fill=1
+        )
+    else:
+        image_edge = np.asarray(
+            [
+                [0.0, 0.0],
+                [0.0, np.shape(f_img.image_gs)[0]],
+                [
+                    np.shape(f_img.image_gs)[1],
+                    np.shape(f_img.image_gs)[0],
+                ],
+                [np.shape(f_img.image_gs)[1], 0.0],
+            ]
+        )
+        ImageDrawPIL.Draw(binary_img).polygon(
+            image_edge.flatten().tolist(), outline=1, fill=1
+        )
 
     # Create objects for mesh generation.
-    _segments = np.empty(
-        (np.shape(_boundary)[0], 2), dtype=np.int32
+    segments = np.empty(
+        (np.shape(boundary._boundary)[0], 2), dtype=np.int32
     )  # Initiate segment array.
-    _segments[:, 0] = np.arange(
-        np.shape(_boundary)[0], dtype=np.int32
+    segments[:, 0] = np.arange(
+        np.shape(boundary._boundary)[0], dtype=np.int32
     )  # Fill segment array.
-    _segments[:, 1] = np.roll(_segments[:, 0], -1)  # Fill segment array.
-    _curves = [list(_segments[:, 0])]  # Create curve list.
+    segments[:, 1] = np.roll(segments[:, 0], -1)  # Fill segment array.
+    curves = [list(segments[:, 0])]  # Create curve list.
 
     # Add exclusions.
-    for exclusion in _exclusions:
+    borders = boundary._boundary
+    for exclusion in exclusions:
         ImageDrawPIL.Draw(binary_img).polygon(
-            exclusion.flatten().tolist(), outline=1, fill=0
+            exclusion._boundary.flatten().tolist(), outline=1, fill=0
         )  # Add exclusion to binary mask.
-        cur_max_idx = np.amax(_segments)  # Highest index used by current segments.
+        cur_max_idx = np.amax(segments)  # Highest index used by current segments.
         exclusion_segment = np.empty(
-            np.shape(exclusion)
+            np.shape(exclusion._boundary)
         )  # Initiate exclusion segment array.
         exclusion_segment[:, 0] = np.arange(
-            cur_max_idx + 1, cur_max_idx + 1 + np.shape(exclusion)[0]
+            cur_max_idx + 1, cur_max_idx + 1 + np.shape(exclusion._boundary)[0]
         )  # Fill exclusion segment array.
         exclusion_segment[:, 1] = np.roll(
             exclusion_segment[:, 0], -1
         )  # Fill exclusion segment array.
-        _boundary = np.append(
-            _boundary, exclusion, axis=0
+        borders = np.append(
+            borders, exclusion._boundary, axis=0
         )  # Append exclusion to boundary array.
-        _segments = np.append(_segments, exclusion_segment, axis=0).astype(
+        segments = np.append(segments, exclusion_segment, axis=0).astype(
             "int32"
         )  # Append exclusion segments to segment array.
-        _curves.append(
+        curves.append(
             list(exclusion_segment[:, 0].astype("int32"))
         )  # Append exclusion curve to curve list.
 
     # Finalise mask.
-    _mask = np.array(binary_img)
+    mask = np.array(binary_img)
 
-    return _boundary, _segments, _curves, _mask
+    return borders, segments, curves, mask
```

### Comparing `geopyv-0.0.8/src/geopyv/geometry/utilities.py` & `geopyv-0.0.9/src/geopyv/geometry/utilities.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/src/geopyv/gui/selectors/coordinate.py` & `geopyv-0.0.9/src/geopyv/gui/selectors/coordinate.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/src/geopyv/gui/selectors/file.py` & `geopyv-0.0.9/src/geopyv/gui/selectors/file.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/src/geopyv/gui/selectors/folder.py` & `geopyv-0.0.9/src/geopyv/gui/selectors/folder.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/src/geopyv/gui/selectors/image.py` & `geopyv-0.0.9/src/geopyv/gui/selectors/image.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/src/geopyv/image.py` & `geopyv-0.0.9/src/geopyv/image.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/src/geopyv/io.py` & `geopyv-0.0.9/src/geopyv/io.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """
 
 IO module for geopyv.
 
 """
 import importlib
 import logging
-import json
 import pickle
 import os
-import numpy as np
 import geopyv as gp
 from alive_progress import alive_bar
 
 log = logging.getLogger(__name__)
 
 
 def load(*, filename=None, directory=None, old_format=False, verbose=True):
@@ -59,42 +57,29 @@
         with open(filepath, "rb") as infile:
             if verbose:
                 message = "Loading geopyv object"
                 with alive_bar(dual_line=True, bar=None, title=message) as bar:
                     bar.text = "-> Loading object from {filepath}...".format(
                         filepath=filepath
                     )
-                    if old_format:
-                        log.warning(
-                            "json file storage deprecated. "
-                            "Load and save objects to convert to new format."
-                        )
-                        data = json.load(infile)
-                        data = _convert_list_to_ndarray(data)
-                    else:
-                        data = pickle.load(infile)
+                    data = pickle.load(infile)
                     bar()
             else:
-                if old_format:
-                    log.warning(
-                        "json file storage deprecated. "
-                        "Load and save objects to convert to new format."
-                    )
-                    data = json.load(infile)
-                    data = _convert_list_to_ndarray(data)
-                else:
-                    data = pickle.load(infile)
+                data = pickle.load(infile)
             object_type = data["type"]
             if verbose:
                 log.info(
                     "Loaded {object_type} object from {filepath}.".format(
                         object_type=object_type, filepath=filepath
                     )
                 )
-            class_name = data["type"] + "Results"
+            if "." in data["type"]:
+                class_name = data["type"].split(".")[-1] + "Results"
+            else:
+                class_name = data["type"] + "Results"
             module = importlib.import_module("geopyv." + object_type.lower())
             results_instance = getattr(module, class_name)
             return results_instance(data)
     except Exception:
         log.error(
             "File does not exist at the path supplied:\n{filepath}".format(
                 filepath=filepath
@@ -156,59 +141,14 @@
             log.warn("Object not solved therefore no data to save.")
             return False
     else:
         log.error("Nothing saved. Object supplied not a valid geopyv type.")
         return False
 
 
-def _convert_list_to_ndarray(data):
-    """
-
-    Recursive function to convert lists back to numpy ndarray.
-
-
-    Parameters
-    ----------
-    data : dict
-        Data dictionary containing lists to be parsed into `numpy.ndarray`.
-
-
-    Returns
-    -------
-    data : dict
-        Data dictionary containing `numpy.ndarray` after conversion from lists.
-
-
-    """
-    for key, value in data.items():
-        if key == "meshes":
-            try:
-                for subset in value:
-                    _convert_list_to_ndarray(subset)
-            except Exception:
-                data[key] = list(value)
-        # If not a list of subsets, convert to numpy ndarray.
-        elif (
-            type(value) == list
-            and key != "subsets"
-            and key != "mesh"
-            and key != "particles"
-            and key != "field"
-        ):
-            data[key] = np.asarray(value)
-        # If a dict convert recursively.
-        elif type(value) == dict:
-            _convert_list_to_ndarray(data[key])
-        # If a list of subsets convert recursively.
-        elif key == "subsets" or key == "mesh" or key == "particles" or key == "field":
-            for subset in value:
-                _convert_list_to_ndarray(subset)
-    return data
-
-
 def _load_img(message):
     """
 
     Private method to open a file dialog and select an image.
 
     """
     directory = os.getcwd()
```

### Comparing `geopyv-0.0.8/src/geopyv/log.py` & `geopyv-0.0.9/src/geopyv/log.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/src/geopyv/mesh.py` & `geopyv-0.0.9/src/geopyv/mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from copy import deepcopy
 from scipy.optimize import minimize_scalar
 import PIL.Image as ImagePIL
 import PIL.ImageDraw as ImageDrawPIL
 from alive_progress import alive_bar
 import traceback
 
+
 log = logging.getLogger(__name__)
 
 
 class MeshBase(Object):
     """
 
     Mesh base class to be used as a mixin. Contains plot functionality.
@@ -577,15 +578,14 @@
         g_img=None,
         target_nodes=1000,
         boundary=None,
         exclusions=[],
         size_lower_bound=1.0,
         size_upper_bound=1000.0,
         mesh_order=2,
-        hard_boundary=True,
         subset_size_compensation=False,
     ):
         """
 
         Initialisation of geopyv mesh object.
 
         Parameters
@@ -604,18 +604,14 @@
             List of `numpy.ndarray` to define the mesh exclusions.
         size_lower_bound : float, optional
             Lower bound on element size. Defaults to a value of 1.0.
         size_upper_bound : float, optional
             Lower bound on element size. Defaults to a value of 1000.0.
         mesh_order : int, optional
             Mesh element order. Options are 1 and 2. Defaults to 2.
-        hard_boundary : bool, optional
-            Boolean to control whether the boundary is included in the
-            binary mask. True -included, False - not included.
-            Defaults to True.
         subset_size_compensation: bool, optional
             Boolean to control whether masked subsets are enlarged to
             maintain area (and thus better correlation).
             Defaults to False.
 
         Attributes
         ----------
@@ -646,50 +642,40 @@
                     gp.check._conversion(target_nodes, "target_nodes", int), "Warning"
                 )
             except Exception:
                 self._report(check, "TypeError")
         self._report(
             gp.check._check_range(target_nodes, "target_nodes", 1), "ValueError"
         )
-        check = gp.check._check_type(boundary, "boundary", [np.ndarray])
-        if check:
-            try:
-                boundary = np.asarray(boundary)
-                self._report(
-                    gp.check._conversion(boundary, "boundary", np.ndarray, False),
-                    "Warning",
-                )
-            except Exception:
-                self._report(check, "TypeError")
-        self._report(gp.check._check_dim(boundary, "boundary", 2), "ValueError")
-        self._report(gp.check._check_axis(boundary, "boundary", 1, [2]), "ValueError")
+        self._report(
+            gp.check._check_type(
+                boundary,
+                "boundary",
+                [gp.geometry.region.Circle, gp.geometry.region.Path],
+            ),
+            "TypeError",
+        )
         check = gp.check._check_type(exclusions, "exclusions", [list])
         if check:
             try:
                 exclusions = list(exclusions)
                 self._report(
                     gp.check._conversion(exclusions, "exclusions", list, False),
                     "Warning",
                 )
             except Exception:
                 self._report(check, "TypeError")
         for exclusion in exclusions:
-            check = gp.check._check_type(exclusion, "exclusion", [np.ndarray])
-            if check:
-                try:
-                    exclusion = np.asarray(exclusion)
-                    self._report(
-                        gp.check._conversion(exclusion, "exclusion", np.ndarray, False),
-                        "Warning",
-                    )
-                except Exception:
-                    self._report(check, "TypeError")
-            self._report(gp.check._check_dim(exclusion, "exclusion", 2), "ValueError")
             self._report(
-                gp.check._check_axis(exclusion, "exclusion", 1, [2]), "ValueError"
+                gp.check._check_type(
+                    exclusion,
+                    "exclusion",
+                    [gp.geometry.region.Circle, gp.geometry.region.Path],
+                ),
+                "TypeError",
             )
         self._report(
             gp.check._check_type(size_lower_bound, "size_lower_bound", [int, float]),
             "TypeError",
         )
         self._report(
             gp.check._check_type(size_upper_bound, "size_upper_bound", [int, float]),
@@ -701,50 +687,58 @@
                 "size_lower_bound",
                 size_upper_bound,
                 "size_upper_bound",
             ),
             "ValueError",
         )
         self._report(
-            gp.check._check_type(hard_boundary, "hard_boundary", [bool]), "TypeError"
-        )
-        self._report(
             gp.check._check_type(
                 subset_size_compensation, "subset_size_compensation", [bool]
             ),
             "TypeError",
         )
 
         # Pre-processing.
         size_upper_bound = min(
             size_upper_bound,
-            np.max(np.sqrt(np.sum(np.square(np.diff(boundary, axis=0)), axis=1))),
+            np.max(
+                np.sqrt(np.sum(np.square(np.diff(boundary._boundary, axis=0)), axis=1))
+            ),
         )
-        minimum_nodes = np.shape(boundary)[0]
+        minimum_nodes = np.shape(boundary._boundary)[0]
         for exclusion in exclusions:
-            minimum_nodes += np.shape(exclusion)[0]
+            minimum_nodes += np.shape(exclusion._boundary)[0]
         target_nodes = max(target_nodes, minimum_nodes)
 
         # Store.
         self._initialised = False
         self._f_img = f_img
         self._g_img = g_img
         self._target_nodes = target_nodes
         self._boundary = boundary
+        self._boundary._rigid = False
         self._exclusions = exclusions
         self._size_lower_bound = size_lower_bound
         self._size_upper_bound = size_upper_bound
         self._mesh_order = mesh_order
-        self._hard_boundary = hard_boundary
+        self._hard_boundary = boundary._hard
         self._subset_size_compensation = subset_size_compensation
         self.solved = False
         self._unsolvable = False
 
         # Define region of interest.
-        self._define_RoI()
+        (
+            self._borders,
+            self._segments,
+            self._curves,
+            self._mask,
+        ) = gp.geometry.meshing._define_RoI(
+            self._f_img, self._boundary, self._exclusions
+        )
+        # self._define_RoI()
 
         # Initialize gmsh if not already initialized.
         if gmsh.isInitialized() == 0:
             gmsh.initialize()
         gmsh.option.setNumber("General.Verbosity", 2)
         # 0: silent except for fatal errors, 1: +errors, 2: +warnings,
         # 3: +direct, 4: +information, 5: +status, 99: +debug.
@@ -1102,14 +1096,19 @@
                         "Minimum correlation coefficient: "
                         "{min_C:.2f}; tolerance: {tolerance:.2f}.".format(
                             min_C=np.amin(self._C_ZNCC[np.where(self._C_ZNCC > 0.0)]),
                             tolerance=self._tolerance,
                         )
                     )
                     return self.solved
+            self._region_tracing()
+            if self._unsolvable:
+                log.error("Rigid exclusion tracking failure.")
+                return self.solved
+
             log.info(
                 "Solved mesh. Minimum correlation coefficient: {min_C:.2f}; "
                 "maximum correlation coefficient: {max_C:.2f}.".format(
                     min_C=np.amin(self._C_ZNCC),
                     max_C=np.amax(self._C_ZNCC),
                 )
             )
@@ -1155,14 +1154,46 @@
             print(traceback.format_exc())
             self._update = True
             self.solved = False
             self._unsolvable = True
         gmsh.finalize()
         return self.solved
 
+    def _region_tracing(self):
+        exclusion_warp = []
+        for i in range(np.shape(self._exclusions)[0]):
+            if self._exclusions[i]._rigid:
+                subset = gp.subset.Subset(
+                    f_img=self._f_img,
+                    g_img=self._g_img,
+                    f_coord=self._exclusions[i]._coord,
+                    template=gp.templates.Circle(
+                        int(self._exclusions[i]._specifics["radius"])
+                    ),
+                )
+                subset.solve(
+                    tolerance=0.9,
+                )
+                if subset.data["solved"] is not True:
+                    self._update = True
+                    self.solved = False
+                    self._unsolvable = True
+                    del subset
+                    return False
+                else:
+                    exclusion_warp.append(subset._p.flatten())
+                    del subset
+            else:
+                exclusion_warp.append(self._displacements[self._exclusions_tags[i]])
+        self._boundary._update(
+            self.data["images"]["f_img"], self._displacements[self._boundary_tags]
+        )
+        for i in range(np.shape(self._exclusions)[0]):
+            self._exclusions[i]._update(self.data["images"]["f_img"], exclusion_warp[i])
+
     def _update_mesh(self):
         """
 
         Private method to update the mesh variables.
 
         """
         (
@@ -1201,19 +1232,17 @@
             "L",
             (
                 np.shape(self._f_img.image_gs)[1],
                 np.shape(self._f_img.image_gs)[0],
             ),
             0,
         )
-        # plt.imshow(np.asarray(binary_img))
-        # plt.show()
         if self._hard_boundary:
             ImageDrawPIL.Draw(binary_img).polygon(
-                self._boundary.flatten().tolist(), outline=1, fill=1
+                self._boundary._boundary.flatten().tolist(), outline=1, fill=1
             )
         else:
             image_edge = np.asarray(
                 [
                     [0.0, 0.0],
                     [0.0, np.shape(self._f_img.image_gs)[0]],
                     [
@@ -1225,43 +1254,43 @@
             )
             ImageDrawPIL.Draw(binary_img).polygon(
                 image_edge.flatten().tolist(), outline=1, fill=1
             )
 
         # Create objects for mesh generation.
         self._segments = np.empty(
-            (np.shape(self._boundary)[0], 2), dtype=np.int32
+            (np.shape(self._boundary._boundary)[0], 2), dtype=np.int32
         )  # Initiate segment array.
         self._segments[:, 0] = np.arange(
-            np.shape(self._boundary)[0], dtype=np.int32
+            np.shape(self._boundary._boundary)[0], dtype=np.int32
         )  # Fill segment array.
         self._segments[:, 1] = np.roll(self._segments[:, 0], -1)  # Fill segment array.
         self._curves = [list(self._segments[:, 0])]  # Create curve list.
 
         # Add exclusions.
-        self._borders = self._boundary
+        self._borders = self._boundary._boundary
         for exclusion in self._exclusions:
             ImageDrawPIL.Draw(binary_img).polygon(
-                exclusion.flatten().tolist(), outline=1, fill=0
+                exclusion._boundary.flatten().tolist(), outline=1, fill=0
             )  # Add exclusion to binary mask.
             cur_max_idx = np.amax(
                 self._segments
             )  # Highest index used by current segments.
             exclusion_segment = np.empty(
-                np.shape(exclusion)
+                np.shape(exclusion._boundary)
             )  # Initiate exclusion segment array.
             exclusion_segment[:, 0] = np.arange(
                 cur_max_idx + 1,
-                cur_max_idx + 1 + np.shape(exclusion)[0],
+                cur_max_idx + 1 + np.shape(exclusion._boundary)[0],
             )  # Fill exclusion segment array.
             exclusion_segment[:, 1] = np.roll(
                 exclusion_segment[:, 0], -1
             )  # Fill exclusion segment array.
             self._borders = np.append(
-                self._borders, exclusion, axis=0
+                self._borders, exclusion._boundary, axis=0
             )  # Append exclusion to boundary array.
             self._segments = np.append(
                 self._segments, exclusion_segment, axis=0
             ).astype(
                 "int32"
             )  # Append exclusion segments to segment array.
             self._curves.append(
```

### Comparing `geopyv-0.0.8/src/geopyv/particle.py` & `geopyv-0.0.9/src/geopyv/particle.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 import numpy as np
 import geopyv as gp
 from geopyv.object import Object
 import re
 import shapely
 from alive_progress import alive_bar
 import math
-
-try:
-    import models
-except Exception:
-    pass
+from build.models import LinearElastic, MCC, SMCC
 
 log = logging.getLogger(__name__)
 
 
 class ParticleBase(Object):
     """
     Particle base class to be used as a mixin. Contains plot functionality.
@@ -707,29 +703,32 @@
             )
         self._strain_def()
         return True
 
     def _stress_path(self, model, state, parameters):
         if model == "LinearElastic":
             # Put input checks here!
-            model = models.LinearElastic(
+            # model = models.LinearElastic(
+            model = LinearElastic(
                 parameters=parameters,
                 state=state,
                 # log_severity = "verbose"
             )
         if model == "MCC":
             # Put input checks here!
-            model = models.MCC(
+            # model = models.MCC(
+            model = MCC(
                 parameters=parameters,
                 state=state,
                 # log_severity = "verbose"
             )
         elif model == "SMCC":
             # Put input checks here!
-            model = models.SMCC(
+            # model = models.SMCC(
+            model = SMCC(
                 parameters=parameters,
                 state=state,
                 # log_severity = "verbose"
             )
         strain_incs = np.diff(self._strains, axis=0)
         ps = []
         qs = []
```

### Comparing `geopyv-0.0.8/src/geopyv/plots.py` & `geopyv-0.0.9/src/geopyv/plots.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/src/geopyv/sequence.py` & `geopyv-0.0.9/src/geopyv/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -702,50 +702,40 @@
                     gp.check._conversion(target_nodes, "target_nodes", int), "Warning"
                 )
             except Exception:
                 self._report(check, "TypeError")
         self._report(
             gp.check._check_range(target_nodes, "target_nodes", 1), "ValueError"
         )
-        check = gp.check._check_type(boundary, "boundary", [np.ndarray])
-        if check:
-            try:
-                boundary = np.asarray(boundary)
-                self._report(
-                    gp.check._conversion(boundary, "boundary", np.ndarray, False),
-                    "Warning",
-                )
-            except Exception:
-                self._report(check, "TypeError")
-        self._report(gp.check._check_dim(boundary, "boundary", 2), "ValueError")
-        self._report(gp.check._check_axis(boundary, "boundary", 1, [2]), "ValueError")
+        self._report(
+            gp.check._check_type(
+                boundary,
+                "boundary",
+                [gp.geometry.region.Circle, gp.geometry.region.Path],
+            ),
+            "TypeError",
+        )
         check = gp.check._check_type(exclusions, "exclusions", [list])
         if check:
             try:
                 exclusions = list(exclusions)
                 self._report(
                     gp.check._conversion(exclusions, "exclusions", list, False),
                     "Warning",
                 )
             except Exception:
                 self._report(check, "TypeError")
         for exclusion in exclusions:
-            check = gp.check._check_type(exclusion, "exclusion", [np.ndarray])
-            if check:
-                try:
-                    exclusion = np.asarray(exclusion)
-                    self._report(
-                        gp.check._conversion(exclusion, "exclusion", np.ndarray, False),
-                        "Warning",
-                    )
-                except Exception:
-                    self._report(check, "TypeError")
-            self._report(gp.check._check_dim(exclusion, "exclusion", 2), "ValueError")
             self._report(
-                gp.check._check_axis(exclusion, "exclusion", 1, [2]), "ValueError"
+                gp.check._check_type(
+                    exclusion,
+                    "exclusion",
+                    [gp.geometry.region.Circle, gp.geometry.region.Path],
+                ),
+                "TypeError",
             )
         self._report(
             gp.check._check_type(size_lower_bound, "size_lower_bound", [int, float]),
             "TypeError",
         )
         self._report(
             gp.check._check_type(size_upper_bound, "size_upper_bound", [int, float]),
@@ -854,17 +844,14 @@
         corrective_iterations=0,
         method="ICGN",
         mesh_order=2,
         subset_order=1,
         tolerance=0.75,
         seed_tolerance=0.9,
         alpha=0.5,
-        track=False,
-        hard_boundary=True,
-        rigid=False,
         subset_size_compensation=False,
         guide=False,
         sequential=False,
     ):
         """
         Method to solve for the sequence.
 
@@ -895,22 +882,14 @@
             Default is ICGN since it is faster.
         adaptive_iterations : int, optional
             Number of mesh adaptivity iterations to perform.
             Defaults to a value of 0.
         alpha : float, optional
             Mesh adaptivity control parameter.
             Defaults to a value of 0.5.
-        track : bool, optional
-            Mesh boundary tracking at reference image updates. Options are:
-            False - no movement,
-            True - movement of initially defined boundary points tracked.
-        hard_boundary : bool, optional
-            Boolean to control whether the boundary is included in the
-            binary mask. True -included, False - not included.
-            Defaults to True.
         subset_size_compensation: bool, optional
             Boolean to control whether masked subsets are enlarged to
             maintain area (and thus better correlation).
             Defaults to False.
 
         Returns
         -------
@@ -1044,19 +1023,14 @@
         if check:
             try:
                 alpha = float(alpha)
                 self._report(gp.check._conversion(alpha, "alpha", float), "Warning")
             except Exception:
                 self._report(check, "TypeError")
         self._report(gp.check._check_range(alpha, "alpha", 0.0, 1.0), "ValueError")
-        self._report(gp.check._check_type(track, "track", [bool]), "TypeError")
-        self._report(gp.check._check_type(rigid, "rigid", [bool]), "TypeError")
-        self._report(
-            gp.check._check_type(hard_boundary, "hard_boundary", [bool]), "TypeError"
-        )
         self._report(
             gp.check._check_type(
                 subset_size_compensation, "subset_size_compensation", [bool]
             ),
             "TypeError",
         )
         if seed_warp is not None:
@@ -1087,17 +1061,14 @@
         self._corrective_iterations = corrective_iterations
         self._method = method
         self._subset_order = subset_order
         self._mesh_order = mesh_order
         self._tolerance = tolerance
         self._seed_tolerance = seed_tolerance
         self._alpha = alpha
-        self._track = track
-        self._hard_boundary = hard_boundary
-        self._rigid = rigid
         self._guide = guide
         self._sequential = sequential
         self._subset_size_compensation = subset_size_compensation
         self._seed_warp = np.zeros(6 * self._subset_order)
 
         # Solve.
         _f_index = 0
@@ -1116,15 +1087,14 @@
                 g_img=_g_img,
                 target_nodes=self._target_nodes,
                 boundary=self._boundary,
                 exclusions=self._exclusions,
                 size_lower_bound=self._size_lower_bound,
                 size_upper_bound=self._size_upper_bound,
                 mesh_order=self._mesh_order,
-                hard_boundary=self._hard_boundary,
                 subset_size_compensation=self._subset_size_compensation,
             )  # Initialise mesh object.
             mesh.solve(
                 seed_coord=self._seed_coord,
                 seed_warp=self._seed_warp,
                 template=self._template,
                 max_iterations=self._max_iterations,
@@ -1151,17 +1121,14 @@
                         "mesh_"
                         + str(self._image_indices[_f_index])
                         + "_"
                         + str(self._image_indices[_g_index])
                     )
                 else:
                     self.data["meshes"][_g_index - 1] = mesh.data
-                if self._track:
-                    self._boundary_tags = mesh._boundary_tags
-                    self._exclusions_tags = mesh._exclusions_tags
                 if self._guide:
                     seed = gp.particle.Particle(
                         series=mesh, coordinate_0=self._seed_coord
                     )
                     seed.solve()
                     self._seed_warp[
                         : 6 * min(self._mesh_order, self._subset_order)
@@ -1176,16 +1143,14 @@
                     self.solved = True
                 if self._sequential:
                     _f_index = _g_index - 1
                     del _f_img
                     _f_img = gp.image.Image(self._image_dir + self._images[_f_index])
             elif _f_index + 1 < _g_index:
                 _f_index = _g_index - 1
-                if self._track:
-                    self._tracking(_f_index)
                 del _f_img
                 _f_img = gp.image.Image(self._image_dir + self._images[_f_index])
             else:
                 log.error(
                     "Mesh for consecutive image pair {a}-{b} is unsolvable. "
                     "Sequence curtailed.".format(
                         a=self._image_indices[_f_index],
@@ -1201,74 +1166,14 @@
 
         # Pack data.
         self.data["solved"] = self.solved
         self.data["unsolvable"] = self._unsolvable
         self.data["meshes"] = np.asarray(self.data["meshes"])
         return self.solved
 
-    def _tracking(self, _f_index):
-        """
-        Private method for tracking the movement of the mesh boundary
-        and exclusions upon reference image updates.
-        """
-
-        log.info("Tracing boundary and exclusion displacements.")
-        if self._save_by_reference:
-            previous_mesh = gp.io.load(
-                filename=self._mesh_dir + self.data["meshes"][_f_index - 1]
-            ).data
-        else:
-            previous_mesh = self.data["meshes"][_f_index - 1]
-        self._boundary = (
-            previous_mesh["nodes"][self._boundary_tags]
-            + previous_mesh["results"]["displacements"][self._boundary_tags]
-        )
-        _exclusions = []
-        if self._rigid:
-            for i in range(np.shape(self._exclusions)[0]):
-                centre = np.mean(self._exclusions[i], axis=0)
-                local_coordinates = self._exclusions[i] - centre
-                f_img = gp.image.Image(
-                    filepath=previous_mesh["images"]["f_img"],
-                )
-                g_img = gp.image.Image(
-                    filepath=previous_mesh["images"]["g_img"],
-                )
-                subset = gp.subset.Subset(
-                    f_img=f_img,
-                    g_img=g_img,
-                    f_coord=centre,
-                    template=gp.templates.Circle(50),
-                )
-                subset.solve(
-                    subset.solve(warp_0=self._exclusions[i][0].data["results"]["p"])
-                )
-                if subset.data["solved"] is not True:
-                    subset.solve()
-                    if subset.data["solved"] is not True:
-                        log.error("Could not track rigid exclusion.")
-                        raise ValueError("Could not track rigid exclusion.")
-                subset.solve()
-                warp = subset.data["results"]["p"].flatten()
-                theta = (warp[3] - warp[4]) / 2
-                rot = np.asarray(
-                    [[np.cos(theta), np.sin(theta)], [-np.sin(theta), np.cos(theta)]]
-                )
-                centre += warp[:2]
-                _exclusions.append(centre + local_coordinates @ rot)
-        else:
-            for i in range(np.shape(self._exclusions)[0]):
-                _exclusions.append(
-                    previous_mesh["nodes"][self._exclusions_tags[i]]
-                    + previous_mesh["results"]["displacements"][
-                        self._exclusions_tags[i]
-                    ]
-                )
-        self._exclusions = _exclusions
-
     def load(self):
         try:
             _meshes = glob.glob("*.pyv", root_dir=self._mesh_dir)
             _mesh_tars = [int(re.findall(r"\d+", x)[-1]) for x in _meshes]
             _mesh_indices_arguments = np.argsort(_mesh_tars)
             self._meshes = np.asarray(
                 [_meshes[index] for index in _mesh_indices_arguments], dtype=object
```

### Comparing `geopyv-0.0.8/src/geopyv/speckle.py` & `geopyv-0.0.9/src/geopyv/speckle.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/src/geopyv/subset.py` & `geopyv-0.0.9/src/geopyv/subset.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/src/geopyv/templates.py` & `geopyv-0.0.9/src/geopyv/templates.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/src/geopyv/validation.py` & `geopyv-0.0.9/src/geopyv/validation.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.8/src/geopyv.egg-info/PKG-INFO` & `geopyv-0.0.9/src/geopyv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geopyv
-Version: 0.0.8
+Version: 0.0.9
 Summary: A PIV/DIC analysis package for Python.
 Author-email: Sam Stanier <sas229@cam.ac.uk>, Jonathan Smith <jdks2@cam.ac.uk>
 Project-URL: Homepage, https://github.com/sas229/geopyv
 Project-URL: Bug Tracker, https://github.com/sas229/geopyv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `geopyv-0.0.8/src/geopyv.egg-info/SOURCES.txt` & `geopyv-0.0.9/src/geopyv.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 src/geopyv/validation.py
 src/geopyv.egg-info/PKG-INFO
 src/geopyv.egg-info/SOURCES.txt
 src/geopyv.egg-info/dependency_links.txt
 src/geopyv.egg-info/requires.txt
 src/geopyv.egg-info/top_level.txt
 src/geopyv/geometry/__init__.py
-src/geopyv/geometry/exclusions.py
 src/geopyv/geometry/meshing.py
+src/geopyv/geometry/region.py
 src/geopyv/geometry/utilities.py
 src/geopyv/gui/__init__.py
 src/geopyv/gui/selectors/__init__.py
 src/geopyv/gui/selectors/coordinate.py
 src/geopyv/gui/selectors/file.py
 src/geopyv/gui/selectors/folder.py
 src/geopyv/gui/selectors/image.py
```

