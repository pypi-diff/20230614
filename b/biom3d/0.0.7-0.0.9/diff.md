# Comparing `tmp/biom3d-0.0.7.tar.gz` & `tmp/biom3d-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biom3d-0.0.7.tar", last modified: Fri Jan 13 11:41:10 2023, max compression
+gzip compressed data, was "biom3d-0.0.9.tar", last modified: Thu Jan 26 11:31:56 2023, max compression
```

## Comparing `biom3d-0.0.7.tar` & `biom3d-0.0.9.tar`

### file list

```diff
@@ -1,52 +1,43 @@
-drwxrwxr-x   0 gumougeot  (1000) gumougeot  (1000)        0 2023-01-13 11:41:10.540032 biom3d-0.0.7/
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    35146 2022-12-19 10:03:50.000000 biom3d-0.0.7/LICENSE
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    13877 2023-01-13 11:41:10.540032 biom3d-0.0.7/PKG-INFO
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    13190 2022-11-23 16:54:44.000000 biom3d-0.0.7/README.md
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     1310 2023-01-13 11:40:54.000000 biom3d-0.0.7/pyproject.toml
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)       38 2023-01-13 11:41:10.540032 biom3d-0.0.7/setup.cfg
-drwxrwxr-x   0 gumougeot  (1000) gumougeot  (1000)        0 2023-01-13 11:41:10.532031 biom3d-0.0.7/src/
-drwxrwxr-x   0 gumougeot  (1000) gumougeot  (1000)        0 2023-01-13 11:41:10.536031 biom3d-0.0.7/src/biom3d/
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)        0 2022-11-24 13:42:31.000000 biom3d-0.0.7/src/biom3d/__init__.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     4542 2022-11-24 16:45:30.000000 biom3d-0.0.7/src/biom3d/auto_config.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    25903 2022-11-24 16:45:30.000000 biom3d-0.0.7/src/biom3d/builder.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    21111 2022-11-24 16:45:30.000000 biom3d-0.0.7/src/biom3d/callbacks.py
-drwxrwxr-x   0 gumougeot  (1000) gumougeot  (1000)        0 2023-01-13 11:41:10.536031 biom3d-0.0.7/src/biom3d/configs/
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)        0 2022-11-24 13:42:49.000000 biom3d-0.0.7/src/biom3d/configs/__init__.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     9314 2022-09-14 09:22:34.000000 biom3d-0.0.7/src/biom3d/configs/unet_chromo.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     6936 2022-11-24 16:31:11.000000 biom3d-0.0.7/src/biom3d/configs/unet_default.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     9470 2022-09-14 09:22:34.000000 biom3d-0.0.7/src/biom3d/configs/unet_lung.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     9422 2023-01-13 11:40:47.000000 biom3d-0.0.7/src/biom3d/configs/unet_pancreas.py
-drwxrwxr-x   0 gumougeot  (1000) gumougeot  (1000)        0 2023-01-13 11:41:10.536031 biom3d-0.0.7/src/biom3d/datasets/
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)        0 2022-11-24 13:42:47.000000 biom3d-0.0.7/src/biom3d/datasets/__init__.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    10553 2022-11-24 16:44:48.000000 biom3d-0.0.7/src/biom3d/datasets/arcface.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     9916 2022-11-24 16:44:49.000000 biom3d-0.0.7/src/biom3d/datasets/dino.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    16195 2022-11-24 16:44:49.000000 biom3d-0.0.7/src/biom3d/datasets/semseg_patch_fast.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    10826 2022-11-24 16:44:49.000000 biom3d-0.0.7/src/biom3d/datasets/triplet.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    56634 2022-12-20 11:05:20.000000 biom3d-0.0.7/src/biom3d/gui.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    44077 2022-11-24 17:08:39.000000 biom3d-0.0.7/src/biom3d/metrics.py
-drwxrwxr-x   0 gumougeot  (1000) gumougeot  (1000)        0 2023-01-13 11:41:10.540032 biom3d-0.0.7/src/biom3d/models/
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)        0 2022-11-24 13:42:46.000000 biom3d-0.0.7/src/biom3d/models/__init__.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     6569 2022-11-24 16:45:01.000000 biom3d-0.0.7/src/biom3d/models/decoder_vgg_deep.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    22852 2022-11-24 16:45:01.000000 biom3d-0.0.7/src/biom3d/models/encoder_efficientnet3d.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     7515 2023-01-13 11:40:47.000000 biom3d-0.0.7/src/biom3d/models/encoder_vgg.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    10248 2022-11-24 17:05:01.000000 biom3d-0.0.7/src/biom3d/models/head.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    30454 2022-11-24 16:45:01.000000 biom3d-0.0.7/src/biom3d/models/hrnet.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    36681 2022-11-24 16:45:01.000000 biom3d-0.0.7/src/biom3d/models/hrnet_2.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     7491 2022-11-24 16:45:02.000000 biom3d-0.0.7/src/biom3d/models/unet3d_eff_2.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     7377 2022-11-24 16:45:02.000000 biom3d-0.0.7/src/biom3d/models/unet3d_eff_3.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    10348 2022-11-24 17:00:14.000000 biom3d-0.0.7/src/biom3d/models/unet3d_vgg_deep.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     4512 2022-11-24 16:45:31.000000 biom3d-0.0.7/src/biom3d/omero_downloader.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     2708 2022-11-24 16:45:31.000000 biom3d-0.0.7/src/biom3d/omero_pred.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     5320 2022-11-24 16:45:31.000000 biom3d-0.0.7/src/biom3d/pred.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    10323 2022-12-20 08:38:38.000000 biom3d-0.0.7/src/biom3d/predictors.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    10095 2022-11-30 12:05:43.000000 biom3d-0.0.7/src/biom3d/preprocess.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     6952 2023-01-13 11:40:47.000000 biom3d-0.0.7/src/biom3d/register.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    11282 2023-01-13 11:40:47.000000 biom3d-0.0.7/src/biom3d/train.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    23018 2022-11-24 16:45:31.000000 biom3d-0.0.7/src/biom3d/trainers.py
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    32270 2022-11-24 16:45:31.000000 biom3d-0.0.7/src/biom3d/utils.py
-drwxrwxr-x   0 gumougeot  (1000) gumougeot  (1000)        0 2023-01-13 11:41:10.536031 biom3d-0.0.7/src/biom3d.egg-info/
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    13877 2023-01-13 11:41:10.000000 biom3d-0.0.7/src/biom3d.egg-info/PKG-INFO
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     1210 2023-01-13 11:41:10.000000 biom3d-0.0.7/src/biom3d.egg-info/SOURCES.txt
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)        1 2023-01-13 11:41:10.000000 biom3d-0.0.7/src/biom3d.egg-info/dependency_links.txt
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)      327 2023-01-13 11:41:10.000000 biom3d-0.0.7/src/biom3d.egg-info/requires.txt
--rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)        7 2023-01-13 11:41:10.000000 biom3d-0.0.7/src/biom3d.egg-info/top_level.txt
+drwxrwxr-x   0 gumougeot  (1000) gumougeot  (1000)        0 2023-01-26 11:31:56.407461 biom3d-0.0.9/
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    35146 2022-12-19 10:03:50.000000 biom3d-0.0.9/LICENSE
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    13142 2023-01-26 11:31:56.407461 biom3d-0.0.9/PKG-INFO
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    12455 2023-01-23 15:21:00.000000 biom3d-0.0.9/README.md
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     1310 2023-01-26 11:31:06.000000 biom3d-0.0.9/pyproject.toml
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)       38 2023-01-26 11:31:56.407461 biom3d-0.0.9/setup.cfg
+drwxrwxr-x   0 gumougeot  (1000) gumougeot  (1000)        0 2023-01-26 11:31:56.407461 biom3d-0.0.9/src/
+drwxrwxr-x   0 gumougeot  (1000) gumougeot  (1000)        0 2023-01-26 11:31:56.407461 biom3d-0.0.9/src/biom3d/
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)        0 2022-11-24 13:42:31.000000 biom3d-0.0.9/src/biom3d/__init__.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     4542 2022-11-24 16:45:30.000000 biom3d-0.0.9/src/biom3d/auto_config.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    25084 2023-01-23 15:21:00.000000 biom3d-0.0.9/src/biom3d/builder.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    21111 2022-11-24 16:45:30.000000 biom3d-0.0.9/src/biom3d/callbacks.py
+drwxrwxr-x   0 gumougeot  (1000) gumougeot  (1000)        0 2023-01-26 11:31:56.407461 biom3d-0.0.9/src/biom3d/configs/
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)        0 2022-11-24 13:42:49.000000 biom3d-0.0.9/src/biom3d/configs/__init__.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     9314 2022-09-14 09:22:34.000000 biom3d-0.0.9/src/biom3d/configs/unet_chromo.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     6937 2023-01-26 11:28:30.000000 biom3d-0.0.9/src/biom3d/configs/unet_default.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     9470 2022-09-14 09:22:34.000000 biom3d-0.0.9/src/biom3d/configs/unet_lung.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     9419 2023-01-26 11:28:01.000000 biom3d-0.0.9/src/biom3d/configs/unet_pancreas.py
+drwxrwxr-x   0 gumougeot  (1000) gumougeot  (1000)        0 2023-01-26 11:31:56.407461 biom3d-0.0.9/src/biom3d/datasets/
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)        0 2022-11-24 13:42:47.000000 biom3d-0.0.9/src/biom3d/datasets/__init__.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    16347 2023-01-18 14:24:15.000000 biom3d-0.0.9/src/biom3d/datasets/semseg_patch_fast.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    56629 2023-01-18 17:52:55.000000 biom3d-0.0.9/src/biom3d/gui.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    14769 2023-01-26 11:28:01.000000 biom3d-0.0.9/src/biom3d/metrics.py
+drwxrwxr-x   0 gumougeot  (1000) gumougeot  (1000)        0 2023-01-26 11:31:56.407461 biom3d-0.0.9/src/biom3d/models/
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)        0 2022-11-24 13:42:46.000000 biom3d-0.0.9/src/biom3d/models/__init__.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     6544 2023-01-18 14:23:06.000000 biom3d-0.0.9/src/biom3d/models/decoder_vgg_deep.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     7515 2023-01-26 11:28:01.000000 biom3d-0.0.9/src/biom3d/models/encoder_vgg.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     3545 2023-01-26 11:28:01.000000 biom3d-0.0.9/src/biom3d/models/unet3d_vgg_deep.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     4512 2022-11-24 16:45:31.000000 biom3d-0.0.9/src/biom3d/omero_downloader.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     2708 2022-11-24 16:45:31.000000 biom3d-0.0.9/src/biom3d/omero_pred.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     5320 2022-11-24 16:45:31.000000 biom3d-0.0.9/src/biom3d/pred.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     8756 2023-01-23 15:21:00.000000 biom3d-0.0.9/src/biom3d/predictors.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    10095 2022-11-30 12:05:43.000000 biom3d-0.0.9/src/biom3d/preprocess.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     2542 2023-01-26 11:28:01.000000 biom3d-0.0.9/src/biom3d/register.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    11282 2023-01-26 11:28:01.000000 biom3d-0.0.9/src/biom3d/train.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)     6768 2023-01-26 11:28:01.000000 biom3d-0.0.9/src/biom3d/trainers.py
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    31925 2023-01-23 15:21:00.000000 biom3d-0.0.9/src/biom3d/utils.py
+drwxrwxr-x   0 gumougeot  (1000) gumougeot  (1000)        0 2023-01-26 11:31:56.407461 biom3d-0.0.9/src/biom3d.egg-info/
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)    13142 2023-01-26 11:31:56.000000 biom3d-0.0.9/src/biom3d.egg-info/PKG-INFO
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)      926 2023-01-26 11:31:56.000000 biom3d-0.0.9/src/biom3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)        1 2023-01-26 11:31:56.000000 biom3d-0.0.9/src/biom3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)      327 2023-01-26 11:31:56.000000 biom3d-0.0.9/src/biom3d.egg-info/requires.txt
+-rw-rw-r--   0 gumougeot  (1000) gumougeot  (1000)        7 2023-01-26 11:31:56.000000 biom3d-0.0.9/src/biom3d.egg-info/top_level.txt
```

### Comparing `biom3d-0.0.7/LICENSE` & `biom3d-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `biom3d-0.0.7/PKG-INFO` & `biom3d-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biom3d
-Version: 0.0.7
+Version: 0.0.9
 Summary: Biom3d. Framework for easy-to-use biomedical image segmentation.
 Author-email: Guillaume Mougeot <guillaume.mougeot@laposte.net>
 Project-URL: Homepage, https://github.com/GuillaumeMougeot/biom3d
 Project-URL: Bug Tracker, https://github.com/GuillaumeMougeot/biom3d/issues
 Keywords: deep learning,image segmentation,medical image analysis,medical image segmentation,biological image segmentation,bio-imaging
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -12,67 +12,49 @@
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: gui
 License-File: LICENSE
 
 # :microscope: Biom3d 
 
-[**Documentation!**](https://biom3d.readthedocs.io/)
+[**Documentation**](https://biom3d.readthedocs.io/)
 
 **Warning! This repository is still a work in progress.**
 
 An easy-to-use and unofficial implementation of [nnUNet](https://github.com/MIC-DKFZ/nnUNet).
 
+Biom3d modules             |  nnUNet modules
+:-------------------------:|:-------------------------:
+![](images/biom3d_train.png)  |  ![](images/nnunet_run_run_training.png)
+
+*Illustrations generated with `pydeps` module*
+
 The goal of Biom3d (and of the original nnUNet) is to automatically configured the training of a U-Net deep learning model for 3D semantic segmentation.
 
 Biom3d is yet more flexible for developers than the original nnUNet implementation: easier to read/understand and easier to edit. Biom3d has also been made easy-to-use for community users.
 
-Biom3d does not include ensemble learning and the possibility to use 2D U-Net or 3D-Cascade U-Net yet. However, these options could easily be adapted if needed.
+Biom3d does not include ensemble learning, the possibility to use 2D U-Net or 3D-Cascade U-Net or Pytorch parallel computing yet. However, these options could easily be adapted if needed.
 
-There two main types of users of Biom3d:
+There are two main types of users of Biom3d:
 
 * Community users, who are interested in using the basic features of Biom3d: GUI, predictions with ready-to-use models or basic training.
-* Deep-learning developers, who are insterested in more advanced features: configuration of module parameters, writing of new Biom3d modules, Biom3d core editing etc.
+* Deep-learning developers, who are interested in more advanced features: configuration of module parameters, writing of new Biom3d modules, Biom3d core editing etc.
 
 In the following documentation, we marked the advanced features with :rocket: symbol.
 
 For Windows users, the paths are here written in "linux-like format". You will have to change '/' symbols to '\\' symbols in the command lines. 
 
 ## :hammer: Installation
 
-Requirements:
-* A NVidia GPUs (at least a Geforce GTX 1080)
-* Windows 10 or Ubuntu 18.04 (other OS have not been tested)
-* Python 3.8 or 3.9 or 3.10 (newer or older version have not been tested)
-* CUDA & CuDNN (cf [Nvidia doc](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html))
-* (optional but recommended) Use Conda or Pip-env. The later is recommended: use `python3 -m venv env` to create a virtual environment and `source env/bin/activate` to activate it. 
-* pytorch==1.12.1 (please be sure that you have access to your NVidia GPU)
-
-Once pytorch installed, the installation can be completed with the following command:
-
-```
-pip3 install -r requirements.txt
-```
-
-Or with the following:
-
-```
-pip3 install SimpleITK==2.1.1 pandas==1.4.0 scikit-image==0.19.0 tensorboard==2.8.0 tqdm==4.62.3 numpy==1.21.2 matplotlib==3.5.3 PyYAML==6.0 torchio==0.18.83 protobuf==3.19.3
-```
-
-Optional: If planning to use omero_dowloader to download datasets/projects from omero, please install omero-py with the following command:
-
-```
-pip3 install omero-py
-```
-
-For Windows users, careful with the previous package: you might need to install [Visual Studio C++ 14.0](https://stackoverflow.com/questions/29846087/error-microsoft-visual-c-14-0-is-required-unable-to-find-vcvarsall-bat) to install `zeroc` dependency.
+**Please check our documentation for the installation details:** [**Documentation-Installation**](https://biom3d.readthedocs.io/en/latest/installation.html)
 
 ## :hand: Usage
 
+**For Graphical User Interface users, check our new documentation!** [**Documentation-GUI**](https://biom3d.readthedocs.io/en/latest/quick_run_gui.html)
+
 Two options:
 * If you have a trained model (you can use one of the publicly available one), you can do [predictions](#prediction) directly.
 * If you do not have a trained model, you must train one and, to do so, you must preprocess your data and create a configuration file. 
 
 Three steps to train a new model:
 * [data preprocessing to tif format (both images and ground truth masks)](#preprocessing)
 * [configuration file definition](#configuration-file-definition)
@@ -92,19 +74,19 @@
     │   ├── image_02.tif
     │   └── ...
     └── masks
         ├── image_01.tif
         ├── image_01.tif
         └── ...
 
-About the naming, the only constraint is that the images and masks have the exact same name. All the folders can have any name and the folder structure does not matter.
+About the naming, the only constraint is that the images and masks have the exact same name. All the folders can have any name **with no space in it** and the parent folder structure does not matter.
 
 #### Image format
 
-To help formating the images to the correct format, we have written a preprocessing script (preprocess.py). More details are available in [the next section](#helper-function).
+To help formatting the images to the correct format, we have written a preprocessing script (preprocess.py). More details are available in [the next section](#helper-function).
 
 Constraints:
 - The images and masks must be .tif files. 
 - The images and masks must all have 4 dimensions: (channel, height, width, depth).
 - Each dimension of each image must be identical to each dimension of the corresponding mask, expect for the channel dimension.
 - Images must be stored in float32 format (numpy.float32).
 - Masks must be stored in byte format (numpy.byte) or int64 format (numpy.int64 or python int type).
```

### Comparing `biom3d-0.0.7/README.md` & `biom3d-0.0.9/src/biom3d.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,60 @@
+Metadata-Version: 2.1
+Name: biom3d
+Version: 0.0.9
+Summary: Biom3d. Framework for easy-to-use biomedical image segmentation.
+Author-email: Guillaume Mougeot <guillaume.mougeot@laposte.net>
+Project-URL: Homepage, https://github.com/GuillaumeMougeot/biom3d
+Project-URL: Bug Tracker, https://github.com/GuillaumeMougeot/biom3d/issues
+Keywords: deep learning,image segmentation,medical image analysis,medical image segmentation,biological image segmentation,bio-imaging
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: gui
+License-File: LICENSE
+
 # :microscope: Biom3d 
 
-[**Documentation!**](https://biom3d.readthedocs.io/)
+[**Documentation**](https://biom3d.readthedocs.io/)
 
 **Warning! This repository is still a work in progress.**
 
 An easy-to-use and unofficial implementation of [nnUNet](https://github.com/MIC-DKFZ/nnUNet).
 
+Biom3d modules             |  nnUNet modules
+:-------------------------:|:-------------------------:
+![](images/biom3d_train.png)  |  ![](images/nnunet_run_run_training.png)
+
+*Illustrations generated with `pydeps` module*
+
 The goal of Biom3d (and of the original nnUNet) is to automatically configured the training of a U-Net deep learning model for 3D semantic segmentation.
 
 Biom3d is yet more flexible for developers than the original nnUNet implementation: easier to read/understand and easier to edit. Biom3d has also been made easy-to-use for community users.
 
-Biom3d does not include ensemble learning and the possibility to use 2D U-Net or 3D-Cascade U-Net yet. However, these options could easily be adapted if needed.
+Biom3d does not include ensemble learning, the possibility to use 2D U-Net or 3D-Cascade U-Net or Pytorch parallel computing yet. However, these options could easily be adapted if needed.
 
-There two main types of users of Biom3d:
+There are two main types of users of Biom3d:
 
 * Community users, who are interested in using the basic features of Biom3d: GUI, predictions with ready-to-use models or basic training.
-* Deep-learning developers, who are insterested in more advanced features: configuration of module parameters, writing of new Biom3d modules, Biom3d core editing etc.
+* Deep-learning developers, who are interested in more advanced features: configuration of module parameters, writing of new Biom3d modules, Biom3d core editing etc.
 
 In the following documentation, we marked the advanced features with :rocket: symbol.
 
 For Windows users, the paths are here written in "linux-like format". You will have to change '/' symbols to '\\' symbols in the command lines. 
 
 ## :hammer: Installation
 
-Requirements:
-* A NVidia GPUs (at least a Geforce GTX 1080)
-* Windows 10 or Ubuntu 18.04 (other OS have not been tested)
-* Python 3.8 or 3.9 or 3.10 (newer or older version have not been tested)
-* CUDA & CuDNN (cf [Nvidia doc](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html))
-* (optional but recommended) Use Conda or Pip-env. The later is recommended: use `python3 -m venv env` to create a virtual environment and `source env/bin/activate` to activate it. 
-* pytorch==1.12.1 (please be sure that you have access to your NVidia GPU)
-
-Once pytorch installed, the installation can be completed with the following command:
-
-```
-pip3 install -r requirements.txt
-```
-
-Or with the following:
-
-```
-pip3 install SimpleITK==2.1.1 pandas==1.4.0 scikit-image==0.19.0 tensorboard==2.8.0 tqdm==4.62.3 numpy==1.21.2 matplotlib==3.5.3 PyYAML==6.0 torchio==0.18.83 protobuf==3.19.3
-```
-
-Optional: If planning to use omero_dowloader to download datasets/projects from omero, please install omero-py with the following command:
-
-```
-pip3 install omero-py
-```
-
-For Windows users, careful with the previous package: you might need to install [Visual Studio C++ 14.0](https://stackoverflow.com/questions/29846087/error-microsoft-visual-c-14-0-is-required-unable-to-find-vcvarsall-bat) to install `zeroc` dependency.
+**Please check our documentation for the installation details:** [**Documentation-Installation**](https://biom3d.readthedocs.io/en/latest/installation.html)
 
 ## :hand: Usage
 
+**For Graphical User Interface users, check our new documentation!** [**Documentation-GUI**](https://biom3d.readthedocs.io/en/latest/quick_run_gui.html)
+
 Two options:
 * If you have a trained model (you can use one of the publicly available one), you can do [predictions](#prediction) directly.
 * If you do not have a trained model, you must train one and, to do so, you must preprocess your data and create a configuration file. 
 
 Three steps to train a new model:
 * [data preprocessing to tif format (both images and ground truth masks)](#preprocessing)
 * [configuration file definition](#configuration-file-definition)
@@ -76,19 +74,19 @@
     │   ├── image_02.tif
     │   └── ...
     └── masks
         ├── image_01.tif
         ├── image_01.tif
         └── ...
 
-About the naming, the only constraint is that the images and masks have the exact same name. All the folders can have any name and the folder structure does not matter.
+About the naming, the only constraint is that the images and masks have the exact same name. All the folders can have any name **with no space in it** and the parent folder structure does not matter.
 
 #### Image format
 
-To help formating the images to the correct format, we have written a preprocessing script (preprocess.py). More details are available in [the next section](#helper-function).
+To help formatting the images to the correct format, we have written a preprocessing script (preprocess.py). More details are available in [the next section](#helper-function).
 
 Constraints:
 - The images and masks must be .tif files. 
 - The images and masks must all have 4 dimensions: (channel, height, width, depth).
 - Each dimension of each image must be identical to each dimension of the corresponding mask, expect for the channel dimension.
 - Images must be stored in float32 format (numpy.float32).
 - Masks must be stored in byte format (numpy.byte) or int64 format (numpy.int64 or python int type).
```

### Comparing `biom3d-0.0.7/pyproject.toml` & `biom3d-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [license]
 file = "LICENSE"
 
 [project]
 name = "biom3d"
-version = "0.0.7"
+version = "0.0.9"
 authors = [
   {name="Guillaume Mougeot", email="guillaume.mougeot@laposte.net"},
 ]
 description = "Biom3d. Framework for easy-to-use biomedical image segmentation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `biom3d-0.0.7/src/biom3d/auto_config.py` & `biom3d-0.0.9/src/biom3d/auto_config.py`

 * *Files identical despite different names*

### Comparing `biom3d-0.0.7/src/biom3d/builder.py` & `biom3d-0.0.9/src/biom3d/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,32 +151,24 @@
     def build_dataset(self):
         """
         build the dataset.
         """
         if 'TRAIN_DATASET' in self.config.keys():
             self.train_dataset = read_config(self.config.TRAIN_DATASET, register.datasets)
         if 'TRAIN_DATALOADER' in self.config.keys():
-            # [DEPRECATED] imread is a special argument of the train_dataloader
-            # imread values should be replaced by corresponding function indicated in the register
-            # if 'imread' in self.config.TRAIN_DATALOADER.kwargs.keys():
-            #     self.config.TRAIN_DATALOADER.kwargs['imread']=read_config(self.config.TRAIN_DATALOADER.kwargs['imread'], register.imread)
             self.train_dataloader = read_config(self.config.TRAIN_DATALOADER, register.datasets)
         else:
             self.train_dataloader = DataLoader(self.train_dataset,**self.config.TRAIN_DATALOADER_KWARGS)
-            # self.train_dataloader = ThreadDataLoader(self.train_dataset,**self.config.TRAIN_DATALOADER_KWARGS)
 
         if 'VAL_DATASET' in self.config.keys():
             self.val_dataset = read_config(self.config.VAL_DATASET, register.datasets)
         if 'VAL_DATALOADER' in self.config.keys():
-            # if 'imread' in self.config.VAL_DATALOADER.kwargs.keys():
-            #     self.config.VAL_DATALOADER.kwargs['imread']=read_config(self.config.VAL_DATALOADER.kwargs['imread'], register.imread)
             self.val_dataloader = read_config(self.config.VAL_DATALOADER, register.datasets)
         elif 'VAL_DATALOADER_KWARGS' in self.config.keys():
             self.val_dataloader = DataLoader(self.val_dataset,**self.config.VAL_DATALOADER_KWARGS)
-            # self.val_dataloader = ThreadDataLoader(self.val_dataset,**self.config.VAL_DATALOADER_KWARGS)
 
 
     def build_model(self, training=True):
         """
         build the model, the losses and the metrics.
         """
```

### Comparing `biom3d-0.0.7/src/biom3d/callbacks.py` & `biom3d-0.0.9/src/biom3d/callbacks.py`

 * *Files identical despite different names*

### Comparing `biom3d-0.0.7/src/biom3d/configs/unet_chromo.py` & `biom3d-0.0.9/src/biom3d/configs/unet_chromo.py`

 * *Files identical despite different names*

### Comparing `biom3d-0.0.7/src/biom3d/configs/unet_default.py` & `biom3d-0.0.9/src/biom3d/configs/unet_default.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,15 +212,15 @@
 )
 
 #---------------------------------------------------------------------------
 # predictors configs
 
 PREDICTOR = Dict(
     fct="SegPatch",
-    kwargs=Dict(patch_size=PATCH_SIZE, tta=True, median_spacing=MEDIAN_SPACING, use_softmax=USE_SOFTMAX, keep_biggest_only=True),
+    kwargs=Dict(patch_size=PATCH_SIZE, tta=True, median_spacing=MEDIAN_SPACING, use_softmax=USE_SOFTMAX, keep_biggest_only=False),
 )
 
 ############################################################################
 # end of config file
 # do not write anything in or below this field
 
 CONFIG = Dict(**globals().copy()) # stores all variables in one Dict
```

### Comparing `biom3d-0.0.7/src/biom3d/configs/unet_lung.py` & `biom3d-0.0.9/src/biom3d/configs/unet_lung.py`

 * *Files identical despite different names*

### Comparing `biom3d-0.0.7/src/biom3d/configs/unet_pancreas.py` & `biom3d-0.0.9/src/biom3d/configs/unet_pancreas.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 # MSK_DIR = 'data/nucleus/masks_resampled_sophie'
 # MSK_DIR = 'data/nucleus/masks_resampled'
 # MSK_DIR = 'data/nucleus/masks_manual'
 
 # PT_PATH = 'data/pancreas/data_pancreas.pt'
 LOG_DIR = 'logs/'
 
-DESC = 'unet_mine-pancreas_21'
+DESC = 'unet_mine-pancreas'
 # DESC = 'unet_mine-chromo_21'
 
 #---------------------------------------------------------------------------
 # training configs
 
 SAVE_BEST = True # whether we save also the best model
```

### Comparing `biom3d-0.0.7/src/biom3d/datasets/semseg_patch_fast.py` & `biom3d-0.0.9/src/biom3d/datasets/semseg_patch_fast.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,14 +264,18 @@
         self.train = train
         print("current fold: {}\n \
         length of the training set: {}\n \
         length of the validation set: {}\n \
         length of the testing set: {}\n \
         is training mode active?: {}".format(fold, len(self.train_imgs), len(self.val_imgs), len(testset), self.train))
 
+        # print train and validation image names
+        print("Training images:", self.train_imgs)
+        print("Validation images:", self.val_imgs)
+
         self.use_aug = use_aug
 
         if self.use_aug:
             ps = np.array(self.patch_size)
 
             # [aug] flipping probabilities
             flip_prop=ps.min()/ps
```

### Comparing `biom3d-0.0.7/src/biom3d/gui.py` & `biom3d-0.0.9/src/biom3d/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 from biom3d.configs.unet_default import CONFIG
 from biom3d.preprocess import preprocess
 from biom3d.auto_config import auto_config
 
 # the packages below are only needed for the local version of the GUI
 # WARNING! the lines below must be commented when deploying the remote version,
 # and uncommented when installing the local version.
-# from biom3d.pred import pred
-# from biom3d.builder import Builder
+from biom3d.pred import pred
+from biom3d.builder import Builder
 # import omero_pred
 
 #----------------------------------------------------------------------------
 # Constants 
 # remote or local
 
 REMOTE = False
@@ -1298,15 +1298,15 @@
         self.train_tab_frame = TrainTab(master=self.train_tab, preprocess_tab=self.preprocess_tab_frame)
         self.train_tab_frame.grid(column=0, row=0, sticky=(N,W,E), pady=24, padx=12)
         self.train_tab.columnconfigure(0, weight=1)
         self.train_tab.rowconfigure(0, weight=1)
 
 if __name__=='__main__':
     parser = argparse.ArgumentParser(description="Graphical User Interface of Biom3d")
-    parser.add_argument("-L", "--local", default=False,  action='store_true', dest='local',
+    parser.add_argument("-L", "--local", default=True,  action='store_true', dest='local',
         help="Start the GUI with the local version (the remote version is the default version).") 
     args = parser.parse_args()
 
     LOCAL = args.local
 
     root = Root()
```

### Comparing `biom3d-0.0.7/src/biom3d/models/decoder_vgg_deep.py` & `biom3d-0.0.9/src/biom3d/models/decoder_vgg_deep.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #---------------------------------------------------------------------------
 # 3D VGG decoder
 # with deep supervision: meaning that each decoder level has an output
 #---------------------------------------------------------------------------
 
-from curses import panel
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.nn.init as init
 import numpy as np
 
 from biom3d.models.encoder_vgg import EncoderBlock
```

### Comparing `biom3d-0.0.7/src/biom3d/models/encoder_vgg.py` & `biom3d-0.0.9/src/biom3d/models/encoder_vgg.py`

 * *Files identical despite different names*

### Comparing `biom3d-0.0.7/src/biom3d/omero_downloader.py` & `biom3d-0.0.9/src/biom3d/omero_downloader.py`

 * *Files identical despite different names*

### Comparing `biom3d-0.0.7/src/biom3d/omero_pred.py` & `biom3d-0.0.9/src/biom3d/omero_pred.py`

 * *Files identical despite different names*

### Comparing `biom3d-0.0.7/src/biom3d/pred.py` & `biom3d-0.0.9/src/biom3d/pred.py`

 * *Files identical despite different names*

### Comparing `biom3d-0.0.7/src/biom3d/predictors.py` & `biom3d-0.0.9/src/biom3d/predictors.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,26 +7,24 @@
 import torch 
 import torchio as tio
 import numpy as np
 from skimage.io import imread
 from tqdm import tqdm
 # from scipy.ndimage.filters import gaussian_filter
 
-from biom3d.utils import keep_biggest_volume_centered, sitk_imread
+from biom3d.utils import keep_biggest_volume_centered, adaptive_imread
 
 #---------------------------------------------------------------------------
 # model predictor for segmentation
 
 def load_img_seg(fname):
     img = imread(fname)
-    # img = utils.sitk_imread()(fname)
 
     # normalize
     img = (img - img.min()) / (img.max() - img.min())
-    # img = (img-img.mean())/img.std()
     
     # to tensor
     img = torch.tensor(img, dtype=torch.float)
 
     # expand dim
     img = torch.unsqueeze(img, dim=0)
     img = torch.unsqueeze(img, dim=0)
@@ -83,16 +81,15 @@
         self.patch_size = np.array(patch_size)
         self.median_spacing = np.array(median_spacing)
         self.clipping_bounds = clipping_bounds
         self.intensity_moments = intensity_moments
         
         # prepare image
         # load the image
-        # img = imread(fname)
-        img,self.spacing = sitk_imread(self.fname)
+        img,self.spacing = adaptive_imread(self.fname)
 
         # store img shape (for post processing)
         self.img_shape = img.shape
         print("image shape: ",self.img_shape)
         
         # expand dims
         img = np.expand_dims(img, 0)
@@ -156,38 +153,14 @@
             if not np.array_equal(sub.img.shape[1:], self.img_shape):
                 sub = tio.Resize(self.img_shape)(sub)
                 img = sub.img.tensor
             return img
         else:
             return logit
 
-def load_img_seg_patch(fname, patch_size=(64,64,32)):
-    """
-    Prepare image for model prediction
-    """
-    # load the image
-    # img = imread(fname)
-    img,_ = sitk_imread(fname)
-
-    # normalize the image
-    # bits = lambda x: ((np.log2(x)>8).astype(int)+(np.log2(x)>16).astype(int)*2+1)*8
-    # img = img / (2**bits(np.max(img)) - 1)
-    img = (img-img.mean())/img.std()
-    img = np.expand_dims(img, 0)
-    img = torch.from_numpy(img).float()
-
-    # define the grid sampler 
-    sub = tio.Subject(img=tio.ScalarImage(tensor=img))
-    patch_size = np.array(patch_size)
-    sampler= tio.data.GridSampler(subject=sub, 
-                            patch_size=patch_size, 
-                            patch_overlap=patch_size//2,
-                            padding_mode='constant')
-    return sampler
-
 def seg_predict_patch(
     img_path,
     model,
     return_logit=False,
     patch_size=None,
     tta=False,          # test time augmentation 
     median_spacing=[],
@@ -202,15 +175,14 @@
     for one image path, load the image, compute the model prediction, return the prediction
     """
 
     device = 'cuda' if torch.cuda.is_available() else 'cpu'
     enable_autocast = torch.cuda.is_available() and enable_autocast # tmp, autocast seems to work only with gpu for now... 
     print('AMP {}'.format('enable' if enable_autocast else 'disable'))
 
-    # img = load_img_seg_patch(img_path, patch_size)
     img_loader = LoadImgPatch(
         img_path,
         patch_size,
         median_spacing,
         clipping_bounds,
         intensity_moments,
     )
@@ -230,76 +202,69 @@
 
         for patch in tqdm(patch_loader):
             X = patch['img'][tio.DATA]
             if torch.cuda.is_available():
                 X = X.cuda()
             
             if tta: # test time augmentation: flip around each axis
-                # Xs = [X] + [torch.flip(X,dims=[i]) for i in range(2,5)]
-                # with torch.cuda.amp.autocast():
-                #     preds = [model(x).cpu() for x in Xs]
-                # preds = [preds[0]]+[torch.flip(preds[i], dims=[i+1]) for i in range(1,4)]
-                # pred = torch.mean(torch.stack(preds), dim=0)
-
                 with torch.autocast(device, enabled=enable_autocast):
                     pred=model(X).cpu()
-                    # pred+=torch.flip(pred, dims=[1]).cpu()
                 
                 # flipping tta
-                # dims = [[1],[2],[3],[1,2],[1,3],[2,3],[1,2,3]]
                 dims = [[2],[3],[4]]
-                # dims = [[2]]
                 for i in range(len(dims)):
                     X_flip = torch.flip(X,dims=dims[i])
 
-                    # with torch.cuda.amp.autocast():
                     with torch.autocast(device, enabled=enable_autocast):
                         pred_flip = model(X_flip)
                         pred += torch.flip(pred_flip, dims=dims[i]).cpu()
                     
                     del X_flip, pred_flip
-                    # torch.cuda.empty_cache()
                 
                 pred = pred/(len(dims)+1)
-                # pred = pred/3
                 del X
-                # torch.cuda.empty_cache()
             else:
-                # with torch.cuda.amp.autocast():
                 with torch.autocast(device, enabled=enable_autocast):
                     pred=model(X).cpu()
                     del X
-                    # torch.cuda.empty_cache()
+
             pred_aggr.add_batch(pred, patch[tio.LOCATION])
         
+        print("Prediction done!")
+
+        print("Aggregation...")
         logit = pred_aggr.get_output_tensor().float()
+        print("Aggregation done!")
     
     if torch.cuda.is_available():
         torch.cuda.empty_cache()
 
     # post-processing:
+    print("Post-processing...")
     logit = img_loader.post_process(logit)
 
-    if return_logit: return logit.numpy()
+    if return_logit: 
+        print("Post-processing done!")
+        return logit.numpy()
 
     if use_softmax:
-        # out = (logit.softmax(dim=0)>0.5).int()[1:]
         out = (logit.softmax(dim=0).argmax(dim=0)).int()
     else:
         out = (logit.sigmoid()>0.5).int()
     out = out.numpy()
 
+    # TODO: the function below is too slow
     if keep_biggest_only:
-        # out = utils.keep_center_only(out)
         if len(out.shape)==3:
             out = keep_biggest_volume_centered(out)
         elif len(out.shape)==4:
             tmp = []
             for i in range(out.shape[0]):
                 tmp += [keep_biggest_volume_centered(out[i])]
             out = np.array(tmp)
 
     out = out.astype(np.byte) 
-    print("output shape",out.shape)
+    print("Post-processing done!")
+    print("Output shape:",out.shape)
     return out
 
 #---------------------------------------------------------------------------
```

### Comparing `biom3d-0.0.7/src/biom3d/preprocess.py` & `biom3d-0.0.9/src/biom3d/preprocess.py`

 * *Files identical despite different names*

### Comparing `biom3d-0.0.7/src/biom3d/train.py` & `biom3d-0.0.9/src/biom3d/train.py`

 * *Files identical despite different names*

### Comparing `biom3d-0.0.7/src/biom3d/utils.py` & `biom3d-0.0.9/src/biom3d/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,28 +137,15 @@
 
 class skimage_imread:
     """
     image reader for .tif files
     """
     def __call__(self, img_path):
         return io.imread(img_path)
-# def skimage_imread(img_path):
-#     """
-#     image reader for .tif files
-#     """
-#     return io.imread(img_path)
 
-# class sitk_imread:
-#     """
-#     image reader for nii.gz files
-#     """
-#     def __call__(self, img_path): 
-#         img = sitk.ReadImage(img_path)
-#         img_np = sitk.GetArrayFromImage(img)
-#         return img_np
 def sitk_imread(img_path):
     """
     image reader for nii.gz files
     """
     img = sitk.ReadImage(img_path)
     img_np = sitk.GetArrayFromImage(img)
     return img_np, np.array(img.GetSpacing())
```

### Comparing `biom3d-0.0.7/src/biom3d.egg-info/PKG-INFO` & `biom3d-0.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,44 @@
-Metadata-Version: 2.1
-Name: biom3d
-Version: 0.0.7
-Summary: Biom3d. Framework for easy-to-use biomedical image segmentation.
-Author-email: Guillaume Mougeot <guillaume.mougeot@laposte.net>
-Project-URL: Homepage, https://github.com/GuillaumeMougeot/biom3d
-Project-URL: Bug Tracker, https://github.com/GuillaumeMougeot/biom3d/issues
-Keywords: deep learning,image segmentation,medical image analysis,medical image segmentation,biological image segmentation,bio-imaging
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: gui
-License-File: LICENSE
-
 # :microscope: Biom3d 
 
-[**Documentation!**](https://biom3d.readthedocs.io/)
+[**Documentation**](https://biom3d.readthedocs.io/)
 
 **Warning! This repository is still a work in progress.**
 
 An easy-to-use and unofficial implementation of [nnUNet](https://github.com/MIC-DKFZ/nnUNet).
 
+Biom3d modules             |  nnUNet modules
+:-------------------------:|:-------------------------:
+![](images/biom3d_train.png)  |  ![](images/nnunet_run_run_training.png)
+
+*Illustrations generated with `pydeps` module*
+
 The goal of Biom3d (and of the original nnUNet) is to automatically configured the training of a U-Net deep learning model for 3D semantic segmentation.
 
 Biom3d is yet more flexible for developers than the original nnUNet implementation: easier to read/understand and easier to edit. Biom3d has also been made easy-to-use for community users.
 
-Biom3d does not include ensemble learning and the possibility to use 2D U-Net or 3D-Cascade U-Net yet. However, these options could easily be adapted if needed.
+Biom3d does not include ensemble learning, the possibility to use 2D U-Net or 3D-Cascade U-Net or Pytorch parallel computing yet. However, these options could easily be adapted if needed.
 
-There two main types of users of Biom3d:
+There are two main types of users of Biom3d:
 
 * Community users, who are interested in using the basic features of Biom3d: GUI, predictions with ready-to-use models or basic training.
-* Deep-learning developers, who are insterested in more advanced features: configuration of module parameters, writing of new Biom3d modules, Biom3d core editing etc.
+* Deep-learning developers, who are interested in more advanced features: configuration of module parameters, writing of new Biom3d modules, Biom3d core editing etc.
 
 In the following documentation, we marked the advanced features with :rocket: symbol.
 
 For Windows users, the paths are here written in "linux-like format". You will have to change '/' symbols to '\\' symbols in the command lines. 
 
 ## :hammer: Installation
 
-Requirements:
-* A NVidia GPUs (at least a Geforce GTX 1080)
-* Windows 10 or Ubuntu 18.04 (other OS have not been tested)
-* Python 3.8 or 3.9 or 3.10 (newer or older version have not been tested)
-* CUDA & CuDNN (cf [Nvidia doc](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html))
-* (optional but recommended) Use Conda or Pip-env. The later is recommended: use `python3 -m venv env` to create a virtual environment and `source env/bin/activate` to activate it. 
-* pytorch==1.12.1 (please be sure that you have access to your NVidia GPU)
-
-Once pytorch installed, the installation can be completed with the following command:
-
-```
-pip3 install -r requirements.txt
-```
-
-Or with the following:
-
-```
-pip3 install SimpleITK==2.1.1 pandas==1.4.0 scikit-image==0.19.0 tensorboard==2.8.0 tqdm==4.62.3 numpy==1.21.2 matplotlib==3.5.3 PyYAML==6.0 torchio==0.18.83 protobuf==3.19.3
-```
-
-Optional: If planning to use omero_dowloader to download datasets/projects from omero, please install omero-py with the following command:
-
-```
-pip3 install omero-py
-```
-
-For Windows users, careful with the previous package: you might need to install [Visual Studio C++ 14.0](https://stackoverflow.com/questions/29846087/error-microsoft-visual-c-14-0-is-required-unable-to-find-vcvarsall-bat) to install `zeroc` dependency.
+**Please check our documentation for the installation details:** [**Documentation-Installation**](https://biom3d.readthedocs.io/en/latest/installation.html)
 
 ## :hand: Usage
 
+**For Graphical User Interface users, check our new documentation!** [**Documentation-GUI**](https://biom3d.readthedocs.io/en/latest/quick_run_gui.html)
+
 Two options:
 * If you have a trained model (you can use one of the publicly available one), you can do [predictions](#prediction) directly.
 * If you do not have a trained model, you must train one and, to do so, you must preprocess your data and create a configuration file. 
 
 Three steps to train a new model:
 * [data preprocessing to tif format (both images and ground truth masks)](#preprocessing)
 * [configuration file definition](#configuration-file-definition)
@@ -92,19 +58,19 @@
     │   ├── image_02.tif
     │   └── ...
     └── masks
         ├── image_01.tif
         ├── image_01.tif
         └── ...
 
-About the naming, the only constraint is that the images and masks have the exact same name. All the folders can have any name and the folder structure does not matter.
+About the naming, the only constraint is that the images and masks have the exact same name. All the folders can have any name **with no space in it** and the parent folder structure does not matter.
 
 #### Image format
 
-To help formating the images to the correct format, we have written a preprocessing script (preprocess.py). More details are available in [the next section](#helper-function).
+To help formatting the images to the correct format, we have written a preprocessing script (preprocess.py). More details are available in [the next section](#helper-function).
 
 Constraints:
 - The images and masks must be .tif files. 
 - The images and masks must all have 4 dimensions: (channel, height, width, depth).
 - Each dimension of each image must be identical to each dimension of the corresponding mask, expect for the channel dimension.
 - Images must be stored in float32 format (numpy.float32).
 - Masks must be stored in byte format (numpy.byte) or int64 format (numpy.int64 or python int type).
```

### Comparing `biom3d-0.0.7/src/biom3d.egg-info/SOURCES.txt` & `biom3d-0.0.9/src/biom3d.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -23,21 +23,12 @@
 src/biom3d.egg-info/top_level.txt
 src/biom3d/configs/__init__.py
 src/biom3d/configs/unet_chromo.py
 src/biom3d/configs/unet_default.py
 src/biom3d/configs/unet_lung.py
 src/biom3d/configs/unet_pancreas.py
 src/biom3d/datasets/__init__.py
-src/biom3d/datasets/arcface.py
-src/biom3d/datasets/dino.py
 src/biom3d/datasets/semseg_patch_fast.py
-src/biom3d/datasets/triplet.py
 src/biom3d/models/__init__.py
 src/biom3d/models/decoder_vgg_deep.py
-src/biom3d/models/encoder_efficientnet3d.py
 src/biom3d/models/encoder_vgg.py
-src/biom3d/models/head.py
-src/biom3d/models/hrnet.py
-src/biom3d/models/hrnet_2.py
-src/biom3d/models/unet3d_eff_2.py
-src/biom3d/models/unet3d_eff_3.py
 src/biom3d/models/unet3d_vgg_deep.py
```

