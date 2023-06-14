# Comparing `tmp/qsm_forward-0.2.post1.tar.gz` & `tmp/qsm_forward-0.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsm_forward-0.2.post1.tar", last modified: Mon Jun 12 07:02:25 2023, max compression
+gzip compressed data, was "qsm_forward-0.2.post2.tar", last modified: Wed Jun 14 02:05:05 2023, max compression
```

## Comparing `qsm_forward-0.2.post1.tar` & `qsm_forward-0.2.post2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-12 07:02:25.984252 qsm_forward-0.2.post1/
--rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm_forward-0.2.post1/LICENSE
--rw-r--r--   0 ashley    (1000) ashley    (1000)     1348 2023-06-12 07:02:25.984252 qsm_forward-0.2.post1/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)      571 2023-06-12 04:37:47.000000 qsm_forward-0.2.post1/README.md
--rw-r--r--   0 ashley    (1000) ashley    (1000)      752 2023-06-12 07:02:11.000000 qsm_forward-0.2.post1/pyproject.toml
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-12 07:02:25.984252 qsm_forward-0.2.post1/qsm_forward/
--rw-r--r--   0 ashley    (1000) ashley    (1000)      397 2023-06-12 05:17:28.000000 qsm_forward-0.2.post1/qsm_forward/__init__.py
--rw-r--r--   0 ashley    (1000) ashley    (1000)    11979 2023-06-12 05:17:28.000000 qsm_forward-0.2.post1/qsm_forward/qsm_forward.py
--rw-r--r--   0 ashley    (1000) ashley    (1000)     8139 2023-06-12 05:17:28.000000 qsm_forward-0.2.post1/qsm_forward/visualisation.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-12 07:02:25.984252 qsm_forward-0.2.post1/qsm_forward.egg-info/
--rw-r--r--   0 ashley    (1000) ashley    (1000)     1348 2023-06-12 07:02:25.000000 qsm_forward-0.2.post1/qsm_forward.egg-info/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)      321 2023-06-12 07:02:25.000000 qsm_forward-0.2.post1/qsm_forward.egg-info/SOURCES.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-12 07:02:25.000000 qsm_forward-0.2.post1/qsm_forward.egg-info/dependency_links.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       67 2023-06-12 07:02:25.000000 qsm_forward-0.2.post1/qsm_forward.egg-info/requires.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-12 07:02:25.000000 qsm_forward-0.2.post1/qsm_forward.egg-info/top_level.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-12 07:02:25.984252 qsm_forward-0.2.post1/setup.cfg
--rw-r--r--   0 ashley    (1000) ashley    (1000)      916 2023-06-12 07:02:07.000000 qsm_forward-0.2.post1/setup.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-12 07:02:25.984252 qsm_forward-0.2.post1/tests/
--rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm_forward-0.2.post1/tests/test_qsm_forward.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 02:05:05.004993 qsm_forward-0.2.post2/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm_forward-0.2.post2/LICENSE
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     1348 2023-06-14 02:05:05.004993 qsm_forward-0.2.post2/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      571 2023-06-12 04:37:47.000000 qsm_forward-0.2.post2/README.md
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      752 2023-06-14 02:03:58.000000 qsm_forward-0.2.post2/pyproject.toml
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 02:05:05.001659 qsm_forward-0.2.post2/qsm_forward/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      397 2023-06-12 05:17:28.000000 qsm_forward-0.2.post2/qsm_forward/__init__.py
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    11985 2023-06-14 02:03:24.000000 qsm_forward-0.2.post2/qsm_forward/qsm_forward.py
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     8139 2023-06-12 05:17:28.000000 qsm_forward-0.2.post2/qsm_forward/visualisation.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 02:05:05.004993 qsm_forward-0.2.post2/qsm_forward.egg-info/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     1348 2023-06-14 02:05:04.000000 qsm_forward-0.2.post2/qsm_forward.egg-info/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      321 2023-06-14 02:05:04.000000 qsm_forward-0.2.post2/qsm_forward.egg-info/SOURCES.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-14 02:05:04.000000 qsm_forward-0.2.post2/qsm_forward.egg-info/dependency_links.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       67 2023-06-14 02:05:04.000000 qsm_forward-0.2.post2/qsm_forward.egg-info/requires.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-14 02:05:04.000000 qsm_forward-0.2.post2/qsm_forward.egg-info/top_level.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-14 02:05:05.004993 qsm_forward-0.2.post2/setup.cfg
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      916 2023-06-14 02:04:09.000000 qsm_forward-0.2.post2/setup.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 02:05:05.004993 qsm_forward-0.2.post2/tests/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm_forward-0.2.post2/tests/test_qsm_forward.py
```

### Comparing `qsm_forward-0.2.post1/LICENSE` & `qsm_forward-0.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `qsm_forward-0.2.post1/PKG-INFO` & `qsm_forward-0.2.post2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsm_forward
-Version: 0.2.post1
+Version: 0.2.post2
 Summary: A forward-model simulation for Quantitative Susceptibility Mapping
 Home-page: https://github.com/astewartau/qsm-forward-model
 Author: Ashley Stewart
 Author-email: Ashley Stewart <a.stewart.au@gmail.com>
 Project-URL: Homepage, https://github.com/astewartau/qsm-forward-model
 Project-URL: Bug Tracker, https://github.com/astewartau/qsm-forward-model/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qsm_forward-0.2.post1/README.md` & `qsm_forward-0.2.post2/README.md`

 * *Files identical despite different names*

### Comparing `qsm_forward-0.2.post1/pyproject.toml` & `qsm_forward-0.2.post2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qsm_forward"
-version = "0.2-1"
+version = "0.2-2"
 authors = [
   { name="Ashley Stewart", email="a.stewart.au@gmail.com" },
 ]
 description = "A forward-model simulation for Quantitative Susceptibility Mapping"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
```

### Comparing `qsm_forward-0.2.post1/qsm_forward/qsm_forward.py` & `qsm_forward-0.2.post2/qsm_forward/qsm_forward.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
     -------
     nibabel.nifti1.Nifti1Image
         The resized Nifti image.
 
     """
     
     target_shape = np.array(np.round((np.array(nii.header.get_zooms()) / voxel_size) * np.array(nii.header.get_data_shape())), dtype=int)
-    target_affine = np.diag(voxel_size + [1])
+    target_affine = np.diag(list(voxel_size) + [1])
     
     return resample_img(
         nii,
         target_affine=target_affine,
         target_shape=target_shape,
         interpolation='nearest'
     )
```

### Comparing `qsm_forward-0.2.post1/qsm_forward/visualisation.py` & `qsm_forward-0.2.post2/qsm_forward/visualisation.py`

 * *Files identical despite different names*

### Comparing `qsm_forward-0.2.post1/qsm_forward.egg-info/PKG-INFO` & `qsm_forward-0.2.post2/qsm_forward.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsm-forward
-Version: 0.2.post1
+Version: 0.2.post2
 Summary: A forward-model simulation for Quantitative Susceptibility Mapping
 Home-page: https://github.com/astewartau/qsm-forward-model
 Author: Ashley Stewart
 Author-email: Ashley Stewart <a.stewart.au@gmail.com>
 Project-URL: Homepage, https://github.com/astewartau/qsm-forward-model
 Project-URL: Bug Tracker, https://github.com/astewartau/qsm-forward-model/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qsm_forward-0.2.post1/setup.py` & `qsm_forward-0.2.post2/setup.py`

 * *Files identical despite different names*

