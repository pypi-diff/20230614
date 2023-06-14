# Comparing `tmp/MMEdu-0.1.8.tar.gz` & `tmp/MMEdu-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MMEdu-0.1.8.tar", last modified: Fri Mar 17 03:43:57 2023, max compression
+gzip compressed data, was "MMEdu-0.1.9.tar", last modified: Sun Apr 23 12:15:45 2023, max compression
```

## Comparing `MMEdu-0.1.8.tar` & `MMEdu-0.1.9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.052511 MMEdu-0.1.8/
--rw-rw-r--   0 user      (1001) user      (1001)       84 2023-02-01 08:23:48.000000 MMEdu-0.1.8/MANIFEST.in
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.044512 MMEdu-0.1.8/MMEdu/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.044512 MMEdu-0.1.8/MMEdu/Classification/
--rw-rw-r--   0 user      (1001) user      (1001)    44554 2023-03-16 08:13:55.000000 MMEdu-0.1.8/MMEdu/Classification/Classification_Edu.py
--rw-rw-r--   0 user      (1001) user      (1001)      111 2023-03-16 07:07:37.000000 MMEdu-0.1.8/MMEdu/Classification/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.044512 MMEdu-0.1.8/MMEdu/Classification/models/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Classification/models/LeNet/
--rw-rw-r--   0 user      (1001) user      (1001)     1999 2022-08-17 05:31:59.000000 MMEdu-0.1.8/MMEdu/Classification/models/LeNet/LeNet.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-17 05:31:59.000000 MMEdu-0.1.8/MMEdu/Classification/models/LeNet/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Classification/models/MobileNet/
--rw-rw-r--   0 user      (1001) user      (1001)     2488 2022-08-17 05:31:59.000000 MMEdu-0.1.8/MMEdu/Classification/models/MobileNet/MobileNet.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-17 05:31:59.000000 MMEdu-0.1.8/MMEdu/Classification/models/MobileNet/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Classification/models/RegNet/
--rw-rw-r--   0 user      (1001) user      (1001)     3220 2022-08-17 05:31:59.000000 MMEdu-0.1.8/MMEdu/Classification/models/RegNet/RegNet.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-17 05:31:59.000000 MMEdu-0.1.8/MMEdu/Classification/models/RegNet/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Classification/models/ResNeXt/
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-17 05:31:59.000000 MMEdu-0.1.8/MMEdu/Classification/models/ResNeXt/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Classification/models/ResNet18/
--rw-rw-r--   0 user      (1001) user      (1001)     2467 2022-08-17 05:31:59.000000 MMEdu-0.1.8/MMEdu/Classification/models/ResNet18/ResNet18.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-17 05:31:59.000000 MMEdu-0.1.8/MMEdu/Classification/models/ResNet18/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Classification/models/ResNet50/
--rw-rw-r--   0 user      (1001) user      (1001)     2500 2022-08-17 05:31:59.000000 MMEdu-0.1.8/MMEdu/Classification/models/ResNet50/ResNet50.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-17 05:31:59.000000 MMEdu-0.1.8/MMEdu/Classification/models/ResNet50/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Classification/models/VGG/
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-17 05:31:59.000000 MMEdu-0.1.8/MMEdu/Classification/models/VGG/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)      733 2022-08-17 08:21:03.000000 MMEdu-0.1.8/MMEdu/Classification/models/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Detection/
--rw-rw-r--   0 user      (1001) user      (1001)    29516 2023-03-16 08:14:30.000000 MMEdu-0.1.8/MMEdu/Detection/Detection_Edu.py
--rw-rw-r--   0 user      (1001) user      (1001)       71 2022-08-17 05:34:42.000000 MMEdu-0.1.8/MMEdu/Detection/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Detection/demo/
--rw-rw-r--   0 user      (1001) user      (1001)        0 2023-02-01 08:21:48.000000 MMEdu-0.1.8/MMEdu/Detection/demo/__init__.py
--rw-------   0 user      (1001) user      (1001)   259865 2022-12-21 03:46:20.000000 MMEdu-0.1.8/MMEdu/Detection/demo/demo.jpg
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Detection/models/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Detection/models/FasterRCNN/
--rw-rw-r--   0 user      (1001) user      (1001)     8278 2023-02-01 07:06:09.000000 MMEdu-0.1.8/MMEdu/Detection/models/FasterRCNN/FasterRCNN.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-16 06:25:41.000000 MMEdu-0.1.8/MMEdu/Detection/models/FasterRCNN/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Detection/models/Mask_RCNN/
--rw-rw-r--   0 user      (1001) user      (1001)     8752 2023-02-01 07:07:30.000000 MMEdu-0.1.8/MMEdu/Detection/models/Mask_RCNN/Mask_RCNN.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-16 06:21:35.000000 MMEdu-0.1.8/MMEdu/Detection/models/Mask_RCNN/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Detection/models/SSD_Lite/
--rw-rw-r--   0 user      (1001) user      (1001)     6047 2023-03-03 07:50:38.000000 MMEdu-0.1.8/MMEdu/Detection/models/SSD_Lite/SSD_Lite.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-16 06:22:12.000000 MMEdu-0.1.8/MMEdu/Detection/models/SSD_Lite/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Detection/models/Yolov3/
--rw-rw-r--   0 user      (1001) user      (1001)     5238 2023-03-03 07:53:19.000000 MMEdu-0.1.8/MMEdu/Detection/models/Yolov3/Yolov3.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-16 06:22:28.000000 MMEdu-0.1.8/MMEdu/Detection/models/Yolov3/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)      677 2022-08-17 08:21:08.000000 MMEdu-0.1.8/MMEdu/Detection/models/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-11-04 02:56:31.000000 MMEdu-0.1.8/MMEdu/MMEdu.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Pose/
--rw-rw-r--   0 user      (1001) user      (1001)     8104 2022-09-27 07:20:01.000000 MMEdu-0.1.8/MMEdu/Pose/Pose_Edu.py
--rw-rw-r--   0 user      (1001) user      (1001)       57 2022-09-16 14:16:27.000000 MMEdu-0.1.8/MMEdu/Pose/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Pose/models/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Pose/models/FasterRCNNpose/
--rw-rw-r--   0 user      (1001) user      (1001)     6052 2022-09-16 14:16:27.000000 MMEdu-0.1.8/MMEdu/Pose/models/FasterRCNNpose/FasterRCNN.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-09-21 07:12:52.000000 MMEdu-0.1.8/MMEdu/Pose/models/FasterRCNNpose/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Pose/models/HrNet/
--rw-rw-r--   0 user      (1001) user      (1001)    38596 2022-09-16 14:16:27.000000 MMEdu-0.1.8/MMEdu/Pose/models/HrNet/HrNet.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-09-21 07:12:57.000000 MMEdu-0.1.8/MMEdu/Pose/models/HrNet/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Pose/models/HrNet32/
--rw-rw-r--   0 user      (1001) user      (1001)    10668 2022-09-16 14:16:27.000000 MMEdu-0.1.8/MMEdu/Pose/models/HrNet32/HrNet32.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-09-21 07:13:01.000000 MMEdu-0.1.8/MMEdu/Pose/models/HrNet32/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/Pose/models/SCNet/
--rw-rw-r--   0 user      (1001) user      (1001)     9716 2022-09-16 14:16:27.000000 MMEdu-0.1.8/MMEdu/Pose/models/SCNet/SCNet.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-09-21 07:13:09.000000 MMEdu-0.1.8/MMEdu/Pose/models/SCNet/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)      676 2022-09-21 07:55:20.000000 MMEdu-0.1.8/MMEdu/Pose/models/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)      340 2023-03-16 07:07:00.000000 MMEdu-0.1.8/MMEdu/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.048512 MMEdu-0.1.8/MMEdu/examples/
--rw-rw-r--   0 user      (1001) user      (1001)      138 2022-08-22 02:06:19.000000 MMEdu-0.1.8/MMEdu/examples/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     3972 2023-03-16 06:30:29.000000 MMEdu-0.1.8/MMEdu/examples/cls_demo.py
--rw-rw-r--   0 user      (1001) user      (1001)     3508 2023-03-16 07:51:15.000000 MMEdu-0.1.8/MMEdu/examples/det_demo.py
--rw-rw-r--   0 user      (1001) user      (1001)     1465 2023-03-17 03:43:28.000000 MMEdu-0.1.8/MMEdu/version.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-17 03:43:57.044512 MMEdu-0.1.8/MMEdu.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      380 2023-03-17 03:43:57.000000 MMEdu-0.1.8/MMEdu.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)     1953 2023-03-17 03:43:57.000000 MMEdu-0.1.8/MMEdu.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-03-17 03:43:57.000000 MMEdu-0.1.8/MMEdu.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       46 2023-03-17 03:43:57.000000 MMEdu-0.1.8/MMEdu.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1001) user      (1001)      149 2023-03-17 03:43:57.000000 MMEdu-0.1.8/MMEdu.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        6 2023-03-17 03:43:57.000000 MMEdu-0.1.8/MMEdu.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-04 03:10:21.000000 MMEdu-0.1.8/MMEdu.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)      380 2023-03-17 03:43:57.048512 MMEdu-0.1.8/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      148 2023-02-01 08:19:30.000000 MMEdu-0.1.8/install_requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-03-17 03:43:57.052511 MMEdu-0.1.8/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     6463 2023-03-17 03:43:19.000000 MMEdu-0.1.8/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.853432 MMEdu-0.1.9/
+-rw-rw-r--   0 user      (1001) user      (1001)       84 2023-02-01 08:23:48.000000 MMEdu-0.1.9/MANIFEST.in
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.849432 MMEdu-0.1.9/MMEdu/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.849432 MMEdu-0.1.9/MMEdu/Classification/
+-rw-rw-r--   0 user      (1001) user      (1001)    45730 2023-04-23 12:11:06.000000 MMEdu-0.1.9/MMEdu/Classification/Classification_Edu.py
+-rw-rw-r--   0 user      (1001) user      (1001)      111 2023-03-16 07:07:37.000000 MMEdu-0.1.9/MMEdu/Classification/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.849432 MMEdu-0.1.9/MMEdu/Classification/models/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.849432 MMEdu-0.1.9/MMEdu/Classification/models/LeNet/
+-rw-rw-r--   0 user      (1001) user      (1001)     1999 2022-08-17 05:31:59.000000 MMEdu-0.1.9/MMEdu/Classification/models/LeNet/LeNet.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-17 05:31:59.000000 MMEdu-0.1.9/MMEdu/Classification/models/LeNet/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.849432 MMEdu-0.1.9/MMEdu/Classification/models/MobileNet/
+-rw-rw-r--   0 user      (1001) user      (1001)     2488 2022-08-17 05:31:59.000000 MMEdu-0.1.9/MMEdu/Classification/models/MobileNet/MobileNet.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-17 05:31:59.000000 MMEdu-0.1.9/MMEdu/Classification/models/MobileNet/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.849432 MMEdu-0.1.9/MMEdu/Classification/models/RegNet/
+-rw-rw-r--   0 user      (1001) user      (1001)     3220 2022-08-17 05:31:59.000000 MMEdu-0.1.9/MMEdu/Classification/models/RegNet/RegNet.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-17 05:31:59.000000 MMEdu-0.1.9/MMEdu/Classification/models/RegNet/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.849432 MMEdu-0.1.9/MMEdu/Classification/models/ResNeXt/
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-17 05:31:59.000000 MMEdu-0.1.9/MMEdu/Classification/models/ResNeXt/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.849432 MMEdu-0.1.9/MMEdu/Classification/models/ResNet18/
+-rw-rw-r--   0 user      (1001) user      (1001)     2467 2022-08-17 05:31:59.000000 MMEdu-0.1.9/MMEdu/Classification/models/ResNet18/ResNet18.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-17 05:31:59.000000 MMEdu-0.1.9/MMEdu/Classification/models/ResNet18/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.853432 MMEdu-0.1.9/MMEdu/Classification/models/ResNet50/
+-rw-rw-r--   0 user      (1001) user      (1001)     2500 2022-08-17 05:31:59.000000 MMEdu-0.1.9/MMEdu/Classification/models/ResNet50/ResNet50.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-17 05:31:59.000000 MMEdu-0.1.9/MMEdu/Classification/models/ResNet50/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.853432 MMEdu-0.1.9/MMEdu/Classification/models/VGG/
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-17 05:31:59.000000 MMEdu-0.1.9/MMEdu/Classification/models/VGG/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)      733 2022-08-17 08:21:03.000000 MMEdu-0.1.9/MMEdu/Classification/models/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.853432 MMEdu-0.1.9/MMEdu/Detection/
+-rw-rw-r--   0 user      (1001) user      (1001)    29864 2023-04-23 12:12:53.000000 MMEdu-0.1.9/MMEdu/Detection/Detection_Edu.py
+-rw-rw-r--   0 user      (1001) user      (1001)       71 2022-08-17 05:34:42.000000 MMEdu-0.1.9/MMEdu/Detection/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.853432 MMEdu-0.1.9/MMEdu/Detection/demo/
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2023-02-01 08:21:48.000000 MMEdu-0.1.9/MMEdu/Detection/demo/__init__.py
+-rw-------   0 user      (1001) user      (1001)   259865 2022-12-21 03:46:20.000000 MMEdu-0.1.9/MMEdu/Detection/demo/demo.jpg
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.853432 MMEdu-0.1.9/MMEdu/Detection/models/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.853432 MMEdu-0.1.9/MMEdu/Detection/models/FasterRCNN/
+-rw-rw-r--   0 user      (1001) user      (1001)     8278 2023-02-01 07:06:09.000000 MMEdu-0.1.9/MMEdu/Detection/models/FasterRCNN/FasterRCNN.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-16 06:25:41.000000 MMEdu-0.1.9/MMEdu/Detection/models/FasterRCNN/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.853432 MMEdu-0.1.9/MMEdu/Detection/models/Mask_RCNN/
+-rw-rw-r--   0 user      (1001) user      (1001)     8752 2023-02-01 07:07:30.000000 MMEdu-0.1.9/MMEdu/Detection/models/Mask_RCNN/Mask_RCNN.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-16 06:21:35.000000 MMEdu-0.1.9/MMEdu/Detection/models/Mask_RCNN/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.853432 MMEdu-0.1.9/MMEdu/Detection/models/SSD_Lite/
+-rw-rw-r--   0 user      (1001) user      (1001)     6047 2023-03-03 07:50:38.000000 MMEdu-0.1.9/MMEdu/Detection/models/SSD_Lite/SSD_Lite.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-16 06:22:12.000000 MMEdu-0.1.9/MMEdu/Detection/models/SSD_Lite/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.853432 MMEdu-0.1.9/MMEdu/Detection/models/Yolov3/
+-rw-rw-r--   0 user      (1001) user      (1001)     5238 2023-03-03 07:53:19.000000 MMEdu-0.1.9/MMEdu/Detection/models/Yolov3/Yolov3.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-16 06:22:28.000000 MMEdu-0.1.9/MMEdu/Detection/models/Yolov3/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)      677 2022-08-17 08:21:08.000000 MMEdu-0.1.9/MMEdu/Detection/models/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-11-04 02:56:31.000000 MMEdu-0.1.9/MMEdu/MMEdu.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.853432 MMEdu-0.1.9/MMEdu/Pose/
+-rw-rw-r--   0 user      (1001) user      (1001)     8104 2022-09-27 07:20:01.000000 MMEdu-0.1.9/MMEdu/Pose/Pose_Edu.py
+-rw-rw-r--   0 user      (1001) user      (1001)       57 2022-09-16 14:16:27.000000 MMEdu-0.1.9/MMEdu/Pose/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.853432 MMEdu-0.1.9/MMEdu/Pose/models/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.853432 MMEdu-0.1.9/MMEdu/Pose/models/FasterRCNNpose/
+-rw-rw-r--   0 user      (1001) user      (1001)     6052 2022-09-16 14:16:27.000000 MMEdu-0.1.9/MMEdu/Pose/models/FasterRCNNpose/FasterRCNN.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-09-21 07:12:52.000000 MMEdu-0.1.9/MMEdu/Pose/models/FasterRCNNpose/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.853432 MMEdu-0.1.9/MMEdu/Pose/models/HrNet/
+-rw-rw-r--   0 user      (1001) user      (1001)    38596 2022-09-16 14:16:27.000000 MMEdu-0.1.9/MMEdu/Pose/models/HrNet/HrNet.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-09-21 07:12:57.000000 MMEdu-0.1.9/MMEdu/Pose/models/HrNet/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.853432 MMEdu-0.1.9/MMEdu/Pose/models/HrNet32/
+-rw-rw-r--   0 user      (1001) user      (1001)    10668 2022-09-16 14:16:27.000000 MMEdu-0.1.9/MMEdu/Pose/models/HrNet32/HrNet32.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-09-21 07:13:01.000000 MMEdu-0.1.9/MMEdu/Pose/models/HrNet32/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.853432 MMEdu-0.1.9/MMEdu/Pose/models/SCNet/
+-rw-rw-r--   0 user      (1001) user      (1001)     9716 2022-09-16 14:16:27.000000 MMEdu-0.1.9/MMEdu/Pose/models/SCNet/SCNet.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-09-21 07:13:09.000000 MMEdu-0.1.9/MMEdu/Pose/models/SCNet/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)      676 2022-09-21 07:55:20.000000 MMEdu-0.1.9/MMEdu/Pose/models/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)      340 2023-03-16 07:07:00.000000 MMEdu-0.1.9/MMEdu/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.853432 MMEdu-0.1.9/MMEdu/examples/
+-rw-rw-r--   0 user      (1001) user      (1001)      138 2022-08-22 02:06:19.000000 MMEdu-0.1.9/MMEdu/examples/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     3992 2023-04-21 09:29:01.000000 MMEdu-0.1.9/MMEdu/examples/cls_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)     3508 2023-03-16 07:51:15.000000 MMEdu-0.1.9/MMEdu/examples/det_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1465 2023-04-23 12:15:06.000000 MMEdu-0.1.9/MMEdu/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-23 12:15:45.849432 MMEdu-0.1.9/MMEdu.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      380 2023-04-23 12:15:45.000000 MMEdu-0.1.9/MMEdu.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)     1953 2023-04-23 12:15:45.000000 MMEdu-0.1.9/MMEdu.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-04-23 12:15:45.000000 MMEdu-0.1.9/MMEdu.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       46 2023-04-23 12:15:45.000000 MMEdu-0.1.9/MMEdu.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)      149 2023-04-23 12:15:45.000000 MMEdu-0.1.9/MMEdu.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        6 2023-04-23 12:15:45.000000 MMEdu-0.1.9/MMEdu.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-04 03:10:21.000000 MMEdu-0.1.9/MMEdu.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)      380 2023-04-23 12:15:45.853432 MMEdu-0.1.9/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      148 2023-02-01 08:19:30.000000 MMEdu-0.1.9/install_requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-04-23 12:15:45.853432 MMEdu-0.1.9/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     6463 2023-04-23 12:15:22.000000 MMEdu-0.1.9/setup.py
```

### Comparing `MMEdu-0.1.8/MMEdu/Classification/Classification_Edu.py` & `MMEdu-0.1.9/MMEdu/Classification/Classification_Edu.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from mmcv import Config
 from mmcls.apis import inference_model, init_model, show_result_pyplot, train_model, set_random_seed, single_gpu_test
 from mmcls.models import build_classifier
 from mmcls.datasets import  build_dataloader,build_dataset
 from mmcv.runner import load_checkpoint
 from mmcv.parallel import collate, scatter
 from mmcls.datasets.pipelines import Compose
+import onnx
+from onnx import load_model
 
 def pth_info(checkpoint):
     import torch
     ckpt = torch.load(checkpoint,map_location='cpu')
     meta = ckpt['meta']
     m = list(meta.keys())
     if 'device' in m:
@@ -200,35 +202,43 @@
         self.cfg.gpu_ids = range(1)
 
         self.cfg.seed = random_seed
         self.cfg.device = device
         if batch_size is not None:
             self.cfg.data.samples_per_gpu = batch_size
 
+        import sys
+        sys.path.append("..")
+        from version import __version__
         meta_info = {
-            'tool':'MMEdu', 
+            'tool':'MMEdu'+__version__, 
             'task':'Classification',
             'backbone':self.backbone, 
             'device':device,
             'dataset_size':len(datasets[0]),
             'learning_rate':lr
         }
-
-
+        t = time.strftime('%Y%m%d_%H%M%S', time.localtime())
         train_model(
             model,
             datasets,
             self.cfg,
             distributed=distributed,
             validate=validate,
-            timestamp=time.strftime('%Y%m%d_%H%M%S', time.localtime()),
+            timestamp=t,
             device=device,
             meta=meta_info
         )
-            
+        file = open(os.path.join(self.save_fold ,str(t)+".log.json"), 'r') 
+        log = []
+        import ast 
+        for i in file.readlines():
+            d = ast.literal_eval(i.rstrip('\n'))
+            log.append(d)
+        return log
 
     def print_result(self, res=None):
         if self.is_sample == True:
             print("示例分类结果如下：")
             sample_result = r"[{'标签': 2, '置信度': 1.0, '预测结果': 'scissors'}]"
             print(sample_result)
         else:
@@ -675,111 +685,126 @@
             results_tmp.extend(result)
 
             batch_size = data['img'].size(0)
             for _ in range(batch_size):
                 prog_bar.update()
         return results_tmp
     
-    def convert(self, checkpoint=None, backend="ONNX", out_file="convert_model.onnx"):
+def convert(self, checkpoint=None, backend="ONNX", out_file="convert_model.onnx"):
         if not (backend == "ONNX" or backend == 'onnx'):
             print("Sorry, we only suport ONNX up to now.")
-            return 
+            return
         state_dict = torch.load(checkpoint, map_location=torch.device('cpu'))
         classes_list = state_dict['meta']['CLASSES']
         self.num_classes = len(classes_list)
         if self.backbone == 'LeNet':
             from mmcls.models.backbones import LeNet5
             from collections import OrderedDict
             model = LeNet5(num_classes=self.num_classes)
-            
+
             class LeNet5_SoftMax(LeNet5):
                 def forward(self, x):
                     x = self.features(x)
                     if self.num_classes > 0:
                         x = self.classifier(x.squeeze())
                         x = torch.softmax(x, dim=0)
-                    return (x, )
+                    return (x,)
 
-            model = LeNet5_SoftMax(num_classes=self.num_classes)    
+            model = LeNet5_SoftMax(num_classes=self.num_classes)
             new_state_dict = OrderedDict()
             for key in state_dict['state_dict']:
                 new_state_dict[key[9:]] = state_dict['state_dict'][key]
             model.load_state_dict(new_state_dict)
             dummy_input = torch.randn(1, 1, 32, 32)
             try:
                 torch.onnx.export(model, dummy_input, out_file)
                 print(f'Successfully exported ONNX model: {out_file}')
             except:
                 print('Please use the checkpoint train by MMEdu')
         else:
-            ashape = [224,224]
+            ashape = [224, 224]
             if len(ashape) == 1:
                 input_shape = (1, 3, ashape[0], ashape[0])
             elif len(ashape) == 2:
                 input_shape = (
-                    1,
-                    3,
-                ) + tuple(ashape)
+                                  1,
+                                  3,
+                              ) + tuple(ashape)
             else:
                 raise ValueError('invalid input shape')
             self.cfg.model.pretrained = None
 
             self.cfg.model.head.num_classes = self.num_classes
             # build the model and load checkpoint
             classifier = build_classifier(self.cfg.model)
 
             if checkpoint:
                 load_checkpoint(classifier, checkpoint, map_location='cpu')
             else:
                 load_checkpoint(classifier, self.checkpoint, map_location='cpu')
 
             pytorch2onnx(
-                classifier, # 模型，此处是分类器
-                input_shape, 
+                classifier,  # 模型，此处是分类器
+                input_shape,
                 output_file=out_file,
-                do_simplify = False,
-                verify =False)
+                do_simplify=False,
+                verify=False)
+
+        onnx_model = load_model(out_file)
+        unicode_string = '|'.join([name for name in classes_list])
+        class_name_metadata = onnx.StringStringEntryProto(key='CLASSES', value=unicode_string)
+        onnx_model.metadata_props.append(class_name_metadata)
+        inputs = onnx_model.graph.input
+        name_to_input = {}
+        for input in inputs:
+            name_to_input[input.name] = input
+
+        for initializer in onnx_model.graph.initializer:
+            if initializer.name in name_to_input:
+                inputs.remove(name_to_input[initializer.name])
 
+        os.remove(out_file)
+        onnx.save(onnx_model, out_file)
         with open(out_file.replace(".onnx", ".py"), "w+") as f:
 
             gen0 = """
-import onnxruntime as rt
-from BaseDT.data_image import ImageData
-import numpy as np
 import cv2
-
-class_names = 
-"""
-
-            gen1 = """
-sess = rt.InferenceSession('
+import numpy as np
+import onnxruntime as rt
+from BaseDT.data import ImageData, ModelData
+model_path = '
 """
-            gen2 = """', None)
-input_name = sess.get_inputs()[0].name
-out_name = sess.get_outputs()[0].name
-
+            gen1 = """'
 cap = cv2.VideoCapture(0)
-ret_flag,Vshow = cap.read()
-dt = ImageData(Vshow, backbone="
+sess = rt.InferenceSession(model_path, None)
+input_name = sess.get_inputs()[0].name
+output_name = sess.get_outputs()[0].name
+ret,img = cap.read()
+cap.release()
+dt = ImageData(img, backbone='
 """
-
-            gen3 = """")
-input_data = dt.to_tensor()
-
-pred_onx = sess.run([out_name], {input_name: input_data})
+            gen2 = """')
+pred_onx = sess.run([output_name], {input_name: dt.to_tensor()})
+class_names = ModelData(model_path).get_labels()
 ort_output = pred_onx[0]
 idx = np.argmax(ort_output, axis=1)[0]
-print('result:' + tag[idx])
-cap.release()
-""" 
-            # if class_path != None:
-            gen = gen0.strip("\n") + str(classes_list)+ "\n" + gen1.strip("\n")+out_file+ gen2.strip("\n") + str(self.backbone) + gen3
-            # else:
-            #     gen = gen0.strip("tag = \n") + "\n\n" + gen1.strip("\n")+out_file+ gen2.strip("\n") + str(self.backbone) + gen3.replace("tag[idx]", "idx")
+print('label:{}, acc:{}'.format(class_names[idx], ort_output[0][idx]))
+            """
+
+            gen3 = """')
+pred_onx = sess.run([output_name], {input_name: dt.to_tensor()})
+class_names = ModelData(model_path).get_labels()
+idx = np.argmax(pred_onx, axis=1)[0]
+print('label:{}, acc:{}'.format(class_names[idx], pred_onx[0][idx]))
+            """
+
+            gen = gen0.strip('\n') + out_file + gen1.strip('\n') + str(self.backbone) + (
+                gen2 if str(self.backbone) != 'LeNet' else gen3)
             f.write(gen)
+
     
 # 模型部署
 def _demo_mm_inputs(input_shape, num_classes):
     """Create a superset of inputs needed to run test or train batches.
     Args:
         input_shape (tuple):
             input batch dimensions
```

### Comparing `MMEdu-0.1.8/MMEdu/Classification/models/LeNet/LeNet.py` & `MMEdu-0.1.9/MMEdu/Classification/models/LeNet/LeNet.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/Classification/models/MobileNet/MobileNet.py` & `MMEdu-0.1.9/MMEdu/Classification/models/MobileNet/MobileNet.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/Classification/models/RegNet/RegNet.py` & `MMEdu-0.1.9/MMEdu/Classification/models/RegNet/RegNet.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/Classification/models/ResNet18/ResNet18.py` & `MMEdu-0.1.9/MMEdu/Classification/models/ResNet18/ResNet18.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/Classification/models/ResNet50/ResNet50.py` & `MMEdu-0.1.9/MMEdu/Classification/models/ResNet50/ResNet50.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/Classification/models/__init__.py` & `MMEdu-0.1.9/MMEdu/Classification/models/__init__.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/Detection/Detection_Edu.py` & `MMEdu-0.1.9/MMEdu/Detection/Detection_Edu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os
 import json
 import mmcv
 import time
+import onnx
+from onnx import load_model
 from mmcv import Config
 from mmdet.apis import inference_detector, init_detector, show_result_pyplot, train_detector
 from mmdet.models import build_detector
 from mmdet.datasets import build_dataset
 from mmcv.runner import load_checkpoint
 from tqdm import tqdm
 import warnings
@@ -148,34 +150,43 @@
         # 设置每 5 个训练批次输出一次日志
         # self.cfg.log_config.interval = 1
         self.cfg.gpu_ids = range(1)
 
         self.cfg.seed = random_seed
         if batch_size is not None:
             self.cfg.data.samples_per_gpu = batch_size
-
+        import sys
+        sys.path.append("..")
+        from version import __version__
         meta_info = {
-            'tool':'MMEdu', 
+            'tool':'MMEdu'+__version__,
             'task':'Detection',
-            'backbone':self.backbone, 
+            'backbone':self.backbone,
             'device':device,
             'dataset_size':len(datasets[0]),
             'learning_rate':lr
         }
-
+        t = time.strftime('%Y%m%d_%H%M%S', time.localtime())
         train_detector(
             model,
             datasets,
             self.cfg,
             distributed=distributed,
             validate=validate,
-            timestamp=time.strftime('%Y%m%d_%H%M%S', time.localtime()),
+            timestamp=t,
             meta=meta_info
         )
-
+        file = open(os.path.join(self.save_fold ,str(t)+".log.json"), 'r') 
+        log = []
+        import ast 
+        for i in file.readlines():
+            d = ast.literal_eval(i.rstrip('\n'))
+            log.append(d)
+        return log
+    
     def print_result(self, res=None):
         if self.is_sample == True:
             print("示例检测结果如下：")
             sample_result = r"[{'类别标签': 0, '置信度': 1.0, '坐标': {'x': 26, 'y': 81, 'w': 497, 'h': 414}},{'类别标签': 1, '置信度': 1.0, '坐标': {'x1': 250, 'y1': 103, 'x2': 494, 'y2': 341}}]"
             print(sample_result)
         else:
             print("检测结果如下：")
@@ -454,62 +465,60 @@
                 show=False,
                 output_file=out_file,
                 verify=False,
                 test_img=None,
                 do_simplify=False)
         else:
             print("Sorry, we only suport ONNX up to now.")
+
+        classes_list = torch.load(checkpoint, map_location=torch.device('cpu'))['meta']['CLASSES']
+        onnx_model = load_model(out_file)
+        unicode_string = '|'.join([name for name in classes_list])
+        class_name_metadata = onnx.StringStringEntryProto(key='CLASSES', value=unicode_string)
+        onnx_model.metadata_props.append(class_name_metadata)
+        inputs = onnx_model.graph.input
+        name_to_input = {}
+        for input in inputs:
+            name_to_input[input.name] = input
+
+        for initializer in onnx_model.graph.initializer:
+            if initializer.name in name_to_input:
+                inputs.remove(name_to_input[initializer.name])
+
+        os.remove(out_file)
+        onnx.save(onnx_model, out_file)
+
         with open(out_file.replace(".onnx", ".py"), "w+") as f:
             tp = str(self.cfg.test_pipeline).replace("},", "},\n\t")
-            # if class_path != None:
-            #     classes_list = self.get_class(class_path)
-            classes_list = torch.load(checkpoint, map_location=torch.device('cpu'))['meta']['CLASSES']
 
             gen0 = """
-import onnxruntime as rt
 import cv2
-from BaseDT.data_image import ImageData
+import onnxruntime as rt
+from BaseDT.data import ImageData, ModelData
 from BaseDT.plot import imshow_det_bboxes
-
-cap = cv2.VideoCapture(0)
-ret_flag,image = cap.read()
-cap.release()
-"""
-            gen_sz = """
-class_names = 
-"""
-            gen1 = """
-sess = rt.InferenceSession('
+model_path = '
 """
-            gen2 = """', None)
+            gen1 = """'
+cap = cv2.VideoCapture(0)
+sess = rt.InferenceSession(model_path, None)
 input_name = sess.get_inputs()[0].name
 output_names = [o.name for o in sess.get_outputs()]
-dt = ImageData(image, backbone="
+ret,img = cap.read()
+cap.release()
+dt = ImageData(img, backbone='
 """
-
-            gen3 = """")
-input_data = dt.to_tensor()
-pred_onx = sess.run(output_names, {input_name: input_data})
-boxes = pred_onx[0][0]
+            gen2 = """')
+pred_onx = sess.run(output_names, {input_name: dt.to_tensor()})
+class_names = ModelData(model_path).get_labels()
+boxes = dt.map_orig_coords(pred_onx[0][0])
 labels = pred_onx[1][0]
-
-imshow_det_bboxes(img, bboxes = boxes,labels = labels, class_names = class_names, score_thr = 0.8) #根据需求修改阈值score_thr
-
+img = imshow_det_bboxes(img, bboxes=boxes, labels=labels, class_names=class_names, score_thr=0.8)
 """
-            ashape = self.cfg.test_pipeline[1].img_scale
-            # if class_path != None:
-            gen = gen0.strip("\n") + '\n' + gen_sz.replace('sz_h', str(ashape[0])).replace('sz_w',
-                                                                                           str(ashape[1])).strip(
-                '\n') + str(classes_list) + "\n" + gen1.strip("\n") + out_file + gen2.strip("\n") + str(
-                self.backbone) + gen3
-            # else:
-            #     gen = gen0.strip("tag = \n") + "\n\n" + gen1.strip("\n")+out_file+ gen2.strip("\n") + str(self.backbone) + gen3.replace("tag[labels[idx]]", "labels[idx]")
+            gen = gen0.strip('\n') + out_file + gen1.strip('\n') + str(self.backbone) + gen2
             f.write(gen)
-
-
 def parse_normalize_cfg(test_pipeline):
     transforms = None
     for pipeline in test_pipeline:
         if 'transforms' in pipeline:
             transforms = pipeline['transforms']
             break
     assert transforms is not None, 'Failed to find `transforms`'
```

### Comparing `MMEdu-0.1.8/MMEdu/Detection/demo/demo.jpg` & `MMEdu-0.1.9/MMEdu/Detection/demo/demo.jpg`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/Detection/models/FasterRCNN/FasterRCNN.py` & `MMEdu-0.1.9/MMEdu/Detection/models/FasterRCNN/FasterRCNN.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/Detection/models/Mask_RCNN/Mask_RCNN.py` & `MMEdu-0.1.9/MMEdu/Detection/models/Mask_RCNN/Mask_RCNN.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/Detection/models/SSD_Lite/SSD_Lite.py` & `MMEdu-0.1.9/MMEdu/Detection/models/SSD_Lite/SSD_Lite.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/Detection/models/Yolov3/Yolov3.py` & `MMEdu-0.1.9/MMEdu/Detection/models/Yolov3/Yolov3.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/Detection/models/__init__.py` & `MMEdu-0.1.9/MMEdu/Detection/models/__init__.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/Pose/Pose_Edu.py` & `MMEdu-0.1.9/MMEdu/Pose/Pose_Edu.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/Pose/models/FasterRCNNpose/FasterRCNN.py` & `MMEdu-0.1.9/MMEdu/Pose/models/FasterRCNNpose/FasterRCNN.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/Pose/models/HrNet/HrNet.py` & `MMEdu-0.1.9/MMEdu/Pose/models/HrNet/HrNet.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/Pose/models/HrNet32/HrNet32.py` & `MMEdu-0.1.9/MMEdu/Pose/models/HrNet32/HrNet32.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/Pose/models/SCNet/SCNet.py` & `MMEdu-0.1.9/MMEdu/Pose/models/SCNet/SCNet.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/Pose/models/__init__.py` & `MMEdu-0.1.9/MMEdu/Pose/models/__init__.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/examples/cls_demo.py` & `MMEdu-0.1.9/MMEdu/examples/cls_demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,17 @@
 	# 指定数据集的路径
 	model.load_dataset(path='../../dataset/cls/hand_gray_q')
 	# 指定保存模型配置文件和权重文件的路径
 	model.save_fold = '../checkpoints/cls_model/h1'
 	# 开始训练，轮次为10，“validate=True”表示每轮训练后，在验证集上测试一次准确率
 	import time
 	a = time.time()
-	model.train(epochs=1, validate=False, optimizer='Adagrad', device='cuda', batch_size=16)
+	log = model.train(epochs=1, validate=False, optimizer='Adagrad', device='cuda', batch_size=16)
 	print("执行时间：",time.time() - a)
+	print(log)
 	# 训练结束后，可以用“model.inference”进行推理，看看效果。
 
 def fast_infer_demo():
 	# 指定一张图片
 	# img='car_plate.png'
 	img = '/home/user/桌面/pip测试4/dataset/cls/hand_gray/test_set/scissors/testscissors02-09.png'
 	# img = 'testrock01-02.png'
@@ -85,9 +86,9 @@
 if __name__ == "__main__":
 	# 请按照次序逐一调用函数，训练模型要耗费较长时间。MMEdu的文档，可以获得更多帮助。
 	# only_infer_demo()
 	# continue_train_demo()
 	normal_train_demo()
 	# fast_infer_demo()
 	# convert_demo()
-	pth_info( '../checkpoints/cls_model/h1/latest.pth')
+	# pth_info( '../checkpoints/cls_model/h1/latest.pth')
```

### Comparing `MMEdu-0.1.8/MMEdu/examples/det_demo.py` & `MMEdu-0.1.9/MMEdu/examples/det_demo.py`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/MMEdu/version.py` & `MMEdu-0.1.9/MMEdu/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-__version__='0.1.8'
+__version__='0.1.9'
 __path__=os.path.abspath(os.getcwd())
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split('.'):
         if x.isdigit():
             version_info.append(int(x))
```

### Comparing `MMEdu-0.1.8/MMEdu.egg-info/SOURCES.txt` & `MMEdu-0.1.9/MMEdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MMEdu-0.1.8/setup.py` & `MMEdu-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 #     install_requires.append('torch @ https://download.pytorch.org/whl/cu101/torch-1.8.1%2Bcu101-cp36-cp36-linux_x86_64.whl')
 #     install_requires.append('torchvision @ https://download.pytorch.org/whl/cu101/torchvision-0.9.1%2Bcu101-cp36-cp36-linux_x86_64.whl')
 
 # print(install_requires)
 setup(
     name='MMEdu',
     # version='0.0.1rc2',
-    version='0.1.8',
+    version='0.1.9',
     # version='0.0.1rc1',
     description='MMEdu originates from the domestic artificial intelligence visual algorithm integration framework OpenMMLab, and is a "out of the box" deep learning development tool.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
```

