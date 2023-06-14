# Comparing `tmp/qsm-forward-0.2.post4.tar.gz` & `tmp/qsm-forward-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsm-forward-0.2.post4.tar", last modified: Wed Jun 14 04:17:30 2023, max compression
+gzip compressed data, was "qsm-forward-0.3.tar", last modified: Wed Jun 14 05:04:17 2023, max compression
```

## Comparing `qsm-forward-0.2.post4.tar` & `qsm-forward-0.3.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 04:17:30.781465 qsm-forward-0.2.post4/
--rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm-forward-0.2.post4/LICENSE
--rw-r--r--   0 ashley    (1000) ashley    (1000)     1348 2023-06-14 04:17:30.781465 qsm-forward-0.2.post4/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)      571 2023-06-12 04:37:47.000000 qsm-forward-0.2.post4/README.md
--rw-r--r--   0 ashley    (1000) ashley    (1000)      752 2023-06-14 04:17:11.000000 qsm-forward-0.2.post4/pyproject.toml
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 04:17:30.781465 qsm-forward-0.2.post4/qsm_forward/
--rw-r--r--   0 ashley    (1000) ashley    (1000)      425 2023-06-14 04:06:28.000000 qsm-forward-0.2.post4/qsm_forward/__init__.py
--rw-r--r--   0 ashley    (1000) ashley    (1000)    12026 2023-06-14 04:16:41.000000 qsm-forward-0.2.post4/qsm_forward/qsm_forward.py
--rw-r--r--   0 ashley    (1000) ashley    (1000)     8139 2023-06-12 05:17:28.000000 qsm-forward-0.2.post4/qsm_forward/visualisation.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 04:17:30.781465 qsm-forward-0.2.post4/qsm_forward.egg-info/
--rw-r--r--   0 ashley    (1000) ashley    (1000)     1348 2023-06-14 04:17:30.000000 qsm-forward-0.2.post4/qsm_forward.egg-info/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)      321 2023-06-14 04:17:30.000000 qsm-forward-0.2.post4/qsm_forward.egg-info/SOURCES.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-14 04:17:30.000000 qsm-forward-0.2.post4/qsm_forward.egg-info/dependency_links.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       19 2023-06-14 04:17:30.000000 qsm-forward-0.2.post4/qsm_forward.egg-info/requires.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-14 04:17:30.000000 qsm-forward-0.2.post4/qsm_forward.egg-info/top_level.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-14 04:17:30.781465 qsm-forward-0.2.post4/setup.cfg
--rw-r--r--   0 ashley    (1000) ashley    (1000)      814 2023-06-14 04:17:07.000000 qsm-forward-0.2.post4/setup.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 04:17:30.781465 qsm-forward-0.2.post4/tests/
--rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm-forward-0.2.post4/tests/test_qsm_forward.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 05:04:17.058063 qsm-forward-0.3/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm-forward-0.3/LICENSE
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     1342 2023-06-14 05:04:17.058063 qsm-forward-0.3/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      571 2023-06-12 04:37:47.000000 qsm-forward-0.3/README.md
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      750 2023-06-14 05:03:17.000000 qsm-forward-0.3/pyproject.toml
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 05:04:17.054729 qsm-forward-0.3/qsm_forward/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      339 2023-06-14 04:21:57.000000 qsm-forward-0.3/qsm_forward/__init__.py
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    12190 2023-06-14 04:59:40.000000 qsm-forward-0.3/qsm_forward/qsm_forward.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 05:04:17.054729 qsm-forward-0.3/qsm_forward.egg-info/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     1342 2023-06-14 05:04:17.000000 qsm-forward-0.3/qsm_forward.egg-info/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      292 2023-06-14 05:04:17.000000 qsm-forward-0.3/qsm_forward.egg-info/SOURCES.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-14 05:04:17.000000 qsm-forward-0.3/qsm_forward.egg-info/dependency_links.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       19 2023-06-14 05:04:17.000000 qsm-forward-0.3/qsm_forward.egg-info/requires.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-14 05:04:17.000000 qsm-forward-0.3/qsm_forward.egg-info/top_level.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-14 05:04:17.058063 qsm-forward-0.3/setup.cfg
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      812 2023-06-14 05:03:22.000000 qsm-forward-0.3/setup.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 05:04:17.054729 qsm-forward-0.3/tests/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm-forward-0.3/tests/test_qsm_forward.py
```

### Comparing `qsm-forward-0.2.post4/LICENSE` & `qsm-forward-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qsm-forward-0.2.post4/PKG-INFO` & `qsm-forward-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsm-forward
-Version: 0.2.post4
+Version: 0.3
 Summary: A forward-model simulation for Quantitative Susceptibility Mapping
 Home-page: https://github.com/astewartau/qsm-forward-model
 Author: Ashley Stewart
 Author-email: Ashley Stewart <a.stewart.au@gmail.com>
 Project-URL: Homepage, https://github.com/astewartau/qsm-forward-model
 Project-URL: Bug Tracker, https://github.com/astewartau/qsm-forward-model/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qsm-forward-0.2.post4/README.md` & `qsm-forward-0.3/README.md`

 * *Files identical despite different names*

### Comparing `qsm-forward-0.2.post4/pyproject.toml` & `qsm-forward-0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qsm-forward"
-version = "0.2-4"
+version = "0.3"
 authors = [
   { name="Ashley Stewart", email="a.stewart.au@gmail.com" },
 ]
 description = "A forward-model simulation for Quantitative Susceptibility Mapping"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
```

### Comparing `qsm-forward-0.2.post4/qsm_forward/qsm_forward.py` & `qsm-forward-0.3/qsm_forward/qsm_forward.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,24 +183,26 @@
     """
 
     noise = np.random.randn(*sig.shape) + 1j * np.random.randn(*sig.shape)
     sig_noisy = sig + (noise * np.max(np.abs(sig))) / peak_snr
     return sig_noisy
 
 
-def resize(nii, voxel_size):
+def resize(nii, voxel_size, interpolation='continuous'):
     """
     Resize a Nifti image to a voxel size.
 
     Parameters
     ----------
     nii : nibabel.nifti1.Nifti1Image
         The input Nifti image.
     voxel_size : list of float
         The desired voxel size after resizing.
+    interpolation : str
+        Can be 'continuous', 'linear', or 'nearest'. Indicates the resample method. Default='continuous'.
 
     Returns
     -------
     nibabel.nifti1.Nifti1Image
         The resized Nifti image.
 
     """
@@ -208,15 +210,15 @@
     target_shape = np.array(np.round((np.array(nii.header.get_zooms()) / voxel_size) * np.array(nii.header.get_data_shape())), dtype=int)
     target_affine = np.diag(list(voxel_size) + [1])
     
     return resample_img(
         nii,
         target_affine=target_affine,
         target_shape=target_shape,
-        interpolation='nearest'
+        interpolation=interpolation
     )
 
 
 def crop_imagespace(x, shape):
     """
     Crop a nD matrix around its center.
```

### Comparing `qsm-forward-0.2.post4/qsm_forward.egg-info/PKG-INFO` & `qsm-forward-0.3/qsm_forward.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsm-forward
-Version: 0.2.post4
+Version: 0.3
 Summary: A forward-model simulation for Quantitative Susceptibility Mapping
 Home-page: https://github.com/astewartau/qsm-forward-model
 Author: Ashley Stewart
 Author-email: Ashley Stewart <a.stewart.au@gmail.com>
 Project-URL: Homepage, https://github.com/astewartau/qsm-forward-model
 Project-URL: Bug Tracker, https://github.com/astewartau/qsm-forward-model/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qsm-forward-0.2.post4/setup.py` & `qsm-forward-0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='qsm-forward',
-    version='0.2-4',
+    version='0.3',
     packages=find_packages(),
     url='https://github.com/astewartau/qsm-forward-model',
     author='Ashley Stewart',
     author_email='a.stewart.au@gmail.com',
     description='A forward-model simulation for Quantitative Susceptibility Mapping',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

