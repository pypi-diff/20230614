# Comparing `tmp/moosez-2.0.8.tar.gz` & `tmp/moosez-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.0.8.tar", last modified: Mon Jun 12 16:31:45 2023, max compression
+gzip compressed data, was "moosez-2.0.9.tar", last modified: Mon Jun 12 16:44:33 2023, max compression
```

## Comparing `moosez-2.0.8.tar` & `moosez-2.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:31:45.050985 moosez-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 16:31:26.000000 moosez-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-12 16:31:45.050985 moosez-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19071 2023-06-12 16:31:26.000000 moosez-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:31:45.050985 moosez-2.0.8/moosez/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-12 16:31:26.000000 moosez-2.0.8/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-12 16:31:26.000000 moosez-2.0.8/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-12 16:31:26.000000 moosez-2.0.8/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-12 16:31:26.000000 moosez-2.0.8/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-12 16:31:26.000000 moosez-2.0.8/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-06-12 16:31:26.000000 moosez-2.0.8/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-12 16:31:26.000000 moosez-2.0.8/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-12 16:31:26.000000 moosez-2.0.8/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-06-12 16:31:26.000000 moosez-2.0.8/moosez/moosez.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-06-12 16:31:26.000000 moosez-2.0.8/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-12 16:31:26.000000 moosez-2.0.8/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:31:45.050985 moosez-2.0.8/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-12 16:31:45.000000 moosez-2.0.8/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-12 16:31:45.000000 moosez-2.0.8/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:31:45.000000 moosez-2.0.8/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 16:31:45.000000 moosez-2.0.8/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-12 16:31:45.000000 moosez-2.0.8/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 16:31:45.000000 moosez-2.0.8/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:31:45.050985 moosez-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-12 16:31:26.000000 moosez-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:44:33.884248 moosez-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 16:44:21.000000 moosez-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-12 16:44:33.884248 moosez-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19071 2023-06-12 16:44:21.000000 moosez-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:44:33.884248 moosez-2.0.9/moosez/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/moosez.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-12 16:44:21.000000 moosez-2.0.9/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:44:33.884248 moosez-2.0.9/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-12 16:44:33.000000 moosez-2.0.9/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-12 16:44:33.000000 moosez-2.0.9/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:44:33.000000 moosez-2.0.9/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 16:44:33.000000 moosez-2.0.9/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-12 16:44:33.000000 moosez-2.0.9/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 16:44:33.000000 moosez-2.0.9/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:44:33.884248 moosez-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-12 16:44:21.000000 moosez-2.0.9/setup.py
```

### Comparing `moosez-2.0.8/LICENSE` & `moosez-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.0.8/PKG-INFO` & `moosez-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.0.8
+Version: 2.0.9
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.0.8/README.md` & `moosez-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `moosez-2.0.8/moosez/constants.py` & `moosez-2.0.9/moosez/constants.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.8/moosez/display.py` & `moosez-2.0.9/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.8/moosez/download.py` & `moosez-2.0.9/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.8/moosez/file_utilities.py` & `moosez-2.0.9/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.8/moosez/image_conversion.py` & `moosez-2.0.9/moosez/image_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 from halo import Halo
 import SimpleITK
 import pydicom
 from moosez import constants
 from multiprocessing import Pool
 from typing import List
 from tqdm import tqdm
+from rich.progress import Progress
+
 
 
 def read_dicom_folder(folder_path: str) -> SimpleITK.Image:
     """
     Reads a folder of DICOM files and returns the image
 
     :param folder_path: str, Directory to get DICOM files from
@@ -73,36 +75,34 @@
 
     if output_directory is None:
         output_directory = os.path.dirname(input_path)
     output_image_path = os.path.join(output_directory, output_image_basename)
     SimpleITK.WriteImage(output_image, output_image_path)
 
 
-from rich.progress import Progress
-
 def standardize_to_nifti(parent_dir: str):
     """
     Converts all images in a parent directory to NIFTI
     """
     # go through the subdirectories
     subjects = os.listdir(parent_dir)
     # get only the directories
     subjects = [subject for subject in subjects if os.path.isdir(os.path.join(parent_dir, subject))]
 
     with Progress() as progress:
         task = progress.add_task("[cyan] Processing subjects...", total=len(subjects))
         for subject in subjects:
             subject_path = os.path.join(parent_dir, subject)
             if os.path.isdir(subject_path):
-                progress.console.print(f" Processing {subject}", highlight=False)
                 images = os.listdir(subject_path)
                 for image in images:
                     if os.path.isdir(os.path.join(subject_path, image)):
                         image_path = os.path.join(subject_path, image)
                         non_nifti_to_nifti(image_path)
                     elif os.path.isfile(os.path.join(subject_path, image)):
                         image_path = os.path.join(subject_path, image)
                         non_nifti_to_nifti(image_path)
             else:
                 continue
-            progress.update(task, advance=1)
+            progress.update(task, advance=1, description=f"[cyan]Processing {subject}...")
+
```

### Comparing `moosez-2.0.8/moosez/image_processing.py` & `moosez-2.0.9/moosez/image_processing.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.8/moosez/input_validation.py` & `moosez-2.0.9/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.8/moosez/moosez.py` & `moosez-2.0.9/moosez/moosez.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.8/moosez/predict.py` & `moosez-2.0.9/moosez/predict.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.8/moosez/resources.py` & `moosez-2.0.9/moosez/resources.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.8/moosez.egg-info/PKG-INFO` & `moosez-2.0.9/moosez.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.0.8
+Version: 2.0.9
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.0.8/setup.py` & `moosez-2.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='moosez',
-    version='2.0.8',
+    version='2.0.9',
     author='Lalith Kumar Shiyam Sundar',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.9',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
```

