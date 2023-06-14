# Comparing `tmp/zhousf-lib-0.6.9.tar.gz` & `tmp/zhousf-lib-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhousf-lib-0.6.9.tar", last modified: Mon Jun 12 06:52:43 2023, max compression
+gzip compressed data, was "zhousf-lib-0.7.0.tar", last modified: Wed Jun 14 07:16:10 2023, max compression
```

## Comparing `zhousf-lib-0.6.9.tar` & `zhousf-lib-0.7.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 06:52:43.544239 zhousf-lib-0.6.9/
--rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.6.9/LICENSE
--rw-rw-rw-   0        0        0     2073 2023-06-12 06:52:43.543272 zhousf-lib-0.6.9/PKG-INFO
--rw-rw-rw-   0        0        0     1179 2023-06-09 06:54:16.000000 zhousf-lib-0.6.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 06:52:43.544239 zhousf-lib-0.6.9/setup.cfg
--rw-rw-rw-   0        0        0     4289 2023-06-12 06:52:37.000000 zhousf-lib-0.6.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:52:43.097118 zhousf-lib-0.6.9/zhousf_lib.egg-info/
--rw-rw-rw-   0        0        0     2073 2023-06-12 06:52:42.000000 zhousf-lib-0.6.9/zhousf_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1929 2023-06-12 06:52:42.000000 zhousf-lib-0.6.9/zhousf_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 06:52:42.000000 zhousf-lib-0.6.9/zhousf_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-12 06:52:42.000000 zhousf-lib-0.6.9/zhousf_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 06:52:43.098127 zhousf-lib-0.6.9/zhousflib/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.6.9/zhousflib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:52:43.100117 zhousf-lib-0.6.9/zhousflib/datasets/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.6.9/zhousflib/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:52:43.102090 zhousf-lib-0.6.9/zhousflib/datasets/classification/
--rw-rw-rw-   0        0        0       73 2023-06-07 01:45:12.000000 zhousf-lib-0.6.9/zhousflib/datasets/classification/__init__.py
--rw-rw-rw-   0        0        0     2937 2023-06-09 06:13:45.000000 zhousf-lib-0.6.9/zhousflib/datasets/classification/classification_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:52:43.169090 zhousf-lib-0.6.9/zhousflib/datasets/coco/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.9/zhousflib/datasets/coco/__init__.py
--rw-rw-rw-   0        0        0     8251 2023-06-07 07:58:31.000000 zhousf-lib-0.6.9/zhousflib/datasets/coco/coco_bbox_extract.py
--rw-rw-rw-   0        0        0     5484 2023-06-12 06:00:08.000000 zhousf-lib-0.6.9/zhousflib/datasets/coco/coco_bbox_update.py
--rw-rw-rw-   0        0        0     6637 2023-06-08 02:33:01.000000 zhousf-lib-0.6.9/zhousflib/datasets/coco/coco_bbox_vis.py
--rw-rw-rw-   0        0        0     2896 2023-06-07 07:55:47.000000 zhousf-lib-0.6.9/zhousflib/datasets/coco/coco_dataset_merge.py
--rw-rw-rw-   0        0        0     6278 2023-06-09 06:13:45.000000 zhousf-lib-0.6.9/zhousflib/datasets/coco/coco_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:52:43.212108 zhousf-lib-0.6.9/zhousflib/datasets/labelme/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.9/zhousflib/datasets/labelme/__init__.py
--rw-rw-rw-   0        0        0     3825 2023-06-07 01:45:12.000000 zhousf-lib-0.6.9/zhousflib/datasets/labelme/labelme_clip.py
--rw-rw-rw-   0        0        0     8090 2023-06-07 01:45:12.000000 zhousf-lib-0.6.9/zhousflib/datasets/labelme/labelme_convert_coco.py
--rw-rw-rw-   0        0        0     9622 2023-06-06 09:07:37.000000 zhousf-lib-0.6.9/zhousflib/datasets/labelme/labelme_convert_seg.py
--rw-rw-rw-   0        0        0     3827 2023-06-07 01:45:12.000000 zhousf-lib-0.6.9/zhousflib/datasets/labelme/labelme_dataset_clip.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:52:43.214091 zhousf-lib-0.6.9/zhousflib/datasets/segmentation/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.9/zhousflib/datasets/segmentation/__init__.py
--rw-rw-rw-   0        0        0     2871 2023-06-06 09:07:37.000000 zhousf-lib-0.6.9/zhousflib/datasets/segmentation/seg_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:52:43.223090 zhousf-lib-0.6.9/zhousflib/db/
--rw-rw-rw-   0        0        0       62 2023-06-08 02:33:01.000000 zhousf-lib-0.6.9/zhousflib/db/__init__.py
--rw-rw-rw-   0        0        0     2345 2023-06-09 06:00:56.000000 zhousf-lib-0.6.9/zhousflib/db/lmdb_master.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:52:43.227089 zhousf-lib-0.6.9/zhousflib/decorator/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.9/zhousflib/decorator/__init__.py
--rw-rw-rw-   0        0        0      466 2023-06-07 01:49:12.000000 zhousf-lib-0.6.9/zhousflib/decorator/except_util.py
--rw-rw-rw-   0        0        0     1094 2023-06-07 01:49:12.000000 zhousf-lib-0.6.9/zhousflib/decorator/interceptor_util.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:52:43.362118 zhousf-lib-0.6.9/zhousflib/font/
--rw-rw-rw-   0        0        0 15320040 2023-03-31 01:19:09.000000 zhousf-lib-0.6.9/zhousflib/font/SimSun.ttf
--rw-rw-rw-   0        0        0  2152796 2023-03-31 01:19:09.000000 zhousf-lib-0.6.9/zhousflib/font/Symbola.ttf
--rw-rw-rw-   0        0        0      763 2023-06-09 05:53:49.000000 zhousf-lib-0.6.9/zhousflib/font/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:52:43.373119 zhousf-lib-0.6.9/zhousflib/locust/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.9/zhousflib/locust/__init__.py
--rw-rw-rw-   0        0        0     1544 2023-06-09 06:20:55.000000 zhousf-lib-0.6.9/zhousflib/locust/locust_demo.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:52:43.376119 zhousf-lib-0.6.9/zhousflib/pandas/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.6.9/zhousflib/pandas/__init__.py
--rw-rw-rw-   0        0        0     3279 2023-06-12 06:52:37.000000 zhousf-lib-0.6.9/zhousflib/pandas/openpyxl_util.py
--rw-rw-rw-   0        0        0     5889 2023-06-12 06:22:28.000000 zhousf-lib-0.6.9/zhousflib/pandas/pandas_util.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:52:43.388120 zhousf-lib-0.6.9/zhousflib/pdf/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.9/zhousflib/pdf/__init__.py
--rw-rw-rw-   0        0        0     1845 2023-06-07 01:49:12.000000 zhousf-lib-0.6.9/zhousflib/pdf/export_image.py
--rw-rw-rw-   0        0        0     1467 2023-06-08 02:34:30.000000 zhousf-lib-0.6.9/zhousflib/pdf/pdfplumber_util.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:52:43.490616 zhousf-lib-0.6.9/zhousflib/util/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.9/zhousflib/util/__init__.py
--rw-rw-rw-   0        0        0     2770 2023-06-07 01:49:13.000000 zhousf-lib-0.6.9/zhousflib/util/calculater_util.py
--rw-rw-rw-   0        0        0      635 2023-06-07 01:49:12.000000 zhousf-lib-0.6.9/zhousflib/util/cv_util.py
--rw-rw-rw-   0        0        0     2193 2023-06-07 01:49:13.000000 zhousf-lib-0.6.9/zhousflib/util/encrypt_util.py
--rw-rw-rw-   0        0        0     1336 2023-06-07 01:49:12.000000 zhousf-lib-0.6.9/zhousflib/util/img_util.py
--rw-rw-rw-   0        0        0    12930 2023-06-07 01:49:12.000000 zhousf-lib-0.6.9/zhousflib/util/iou_util.py
--rw-rw-rw-   0        0        0     3373 2023-06-07 01:49:12.000000 zhousf-lib-0.6.9/zhousflib/util/json_util.py
--rw-rw-rw-   0        0        0      472 2023-06-07 01:49:13.000000 zhousf-lib-0.6.9/zhousflib/util/list_util.py
--rw-rw-rw-   0        0        0     1358 2023-06-07 01:49:12.000000 zhousf-lib-0.6.9/zhousflib/util/permission_util.py
--rw-rw-rw-   0        0        0     3524 2023-06-07 01:49:11.000000 zhousf-lib-0.6.9/zhousflib/util/poly_util.py
--rw-rw-rw-   0        0        0      633 2023-06-07 01:49:12.000000 zhousf-lib-0.6.9/zhousflib/util/re_util.py
--rw-rw-rw-   0        0        0      520 2023-06-07 01:49:12.000000 zhousf-lib-0.6.9/zhousflib/util/singleton.py
--rw-rw-rw-   0        0        0     4246 2023-06-09 06:46:55.000000 zhousf-lib-0.6.9/zhousflib/util/string_util.py
--rw-rw-rw-   0        0        0     4663 2023-06-07 01:49:11.000000 zhousf-lib-0.6.9/zhousflib/util/time_util.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:52:43.539267 zhousf-lib-0.6.9/zhousflib/web/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.9/zhousflib/web/__init__.py
--rw-rw-rw-   0        0        0     4355 2023-06-07 01:49:13.000000 zhousf-lib-0.6.9/zhousflib/web/config.py
--rw-rw-rw-   0        0        0     3105 2023-06-07 01:49:12.000000 zhousf-lib-0.6.9/zhousflib/web/log_util.py
--rw-rw-rw-   0        0        0     2860 2023-06-07 01:49:13.000000 zhousf-lib-0.6.9/zhousflib/web/logger.py
--rw-rw-rw-   0        0        0     1340 2023-06-07 01:49:13.000000 zhousf-lib-0.6.9/zhousflib/web/response.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:10.216587 zhousf-lib-0.7.0/
+-rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0     2073 2023-06-14 07:16:10.216587 zhousf-lib-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1179 2023-06-09 06:54:16.000000 zhousf-lib-0.7.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 07:16:10.216587 zhousf-lib-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     4289 2023-06-14 07:16:03.000000 zhousf-lib-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:09.737328 zhousf-lib-0.7.0/zhousf_lib.egg-info/
+-rw-rw-rw-   0        0        0     2073 2023-06-14 07:16:09.000000 zhousf-lib-0.7.0/zhousf_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1929 2023-06-14 07:16:09.000000 zhousf-lib-0.7.0/zhousf_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 07:16:09.000000 zhousf-lib-0.7.0/zhousf_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-14 07:16:09.000000 zhousf-lib-0.7.0/zhousf_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:09.737328 zhousf-lib-0.7.0/zhousflib/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.7.0/zhousflib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:09.739287 zhousf-lib-0.7.0/zhousflib/datasets/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.7.0/zhousflib/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:09.741259 zhousf-lib-0.7.0/zhousflib/datasets/classification/
+-rw-rw-rw-   0        0        0       73 2023-06-07 01:45:12.000000 zhousf-lib-0.7.0/zhousflib/datasets/classification/__init__.py
+-rw-rw-rw-   0        0        0     4895 2023-06-13 08:58:42.000000 zhousf-lib-0.7.0/zhousflib/datasets/classification/classification_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:09.805258 zhousf-lib-0.7.0/zhousflib/datasets/coco/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.7.0/zhousflib/datasets/coco/__init__.py
+-rw-rw-rw-   0        0        0     8251 2023-06-07 07:58:31.000000 zhousf-lib-0.7.0/zhousflib/datasets/coco/coco_bbox_extract.py
+-rw-rw-rw-   0        0        0     5484 2023-06-12 06:00:08.000000 zhousf-lib-0.7.0/zhousflib/datasets/coco/coco_bbox_update.py
+-rw-rw-rw-   0        0        0     6637 2023-06-08 02:33:01.000000 zhousf-lib-0.7.0/zhousflib/datasets/coco/coco_bbox_vis.py
+-rw-rw-rw-   0        0        0     2896 2023-06-07 07:55:47.000000 zhousf-lib-0.7.0/zhousflib/datasets/coco/coco_dataset_merge.py
+-rw-rw-rw-   0        0        0     6278 2023-06-09 06:13:45.000000 zhousf-lib-0.7.0/zhousflib/datasets/coco/coco_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:09.873863 zhousf-lib-0.7.0/zhousflib/datasets/labelme/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.7.0/zhousflib/datasets/labelme/__init__.py
+-rw-rw-rw-   0        0        0     3825 2023-06-07 01:45:12.000000 zhousf-lib-0.7.0/zhousflib/datasets/labelme/labelme_clip.py
+-rw-rw-rw-   0        0        0     8090 2023-06-07 01:45:12.000000 zhousf-lib-0.7.0/zhousflib/datasets/labelme/labelme_convert_coco.py
+-rw-rw-rw-   0        0        0     9622 2023-06-06 09:07:37.000000 zhousf-lib-0.7.0/zhousflib/datasets/labelme/labelme_convert_seg.py
+-rw-rw-rw-   0        0        0     3827 2023-06-07 01:45:12.000000 zhousf-lib-0.7.0/zhousflib/datasets/labelme/labelme_dataset_clip.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:09.875862 zhousf-lib-0.7.0/zhousflib/datasets/segmentation/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.7.0/zhousflib/datasets/segmentation/__init__.py
+-rw-rw-rw-   0        0        0     2871 2023-06-06 09:07:37.000000 zhousf-lib-0.7.0/zhousflib/datasets/segmentation/seg_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:09.883863 zhousf-lib-0.7.0/zhousflib/db/
+-rw-rw-rw-   0        0        0       62 2023-06-08 02:33:01.000000 zhousf-lib-0.7.0/zhousflib/db/__init__.py
+-rw-rw-rw-   0        0        0     2345 2023-06-09 06:00:56.000000 zhousf-lib-0.7.0/zhousflib/db/lmdb_master.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:09.887864 zhousf-lib-0.7.0/zhousflib/decorator/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.7.0/zhousflib/decorator/__init__.py
+-rw-rw-rw-   0        0        0      466 2023-06-07 01:49:12.000000 zhousf-lib-0.7.0/zhousflib/decorator/except_util.py
+-rw-rw-rw-   0        0        0     1094 2023-06-07 01:49:12.000000 zhousf-lib-0.7.0/zhousflib/decorator/interceptor_util.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:10.012838 zhousf-lib-0.7.0/zhousflib/font/
+-rw-rw-rw-   0        0        0 15320040 2023-03-31 01:19:09.000000 zhousf-lib-0.7.0/zhousflib/font/SimSun.ttf
+-rw-rw-rw-   0        0        0  2152796 2023-03-31 01:19:09.000000 zhousf-lib-0.7.0/zhousflib/font/Symbola.ttf
+-rw-rw-rw-   0        0        0      763 2023-06-09 05:53:49.000000 zhousf-lib-0.7.0/zhousflib/font/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:10.023837 zhousf-lib-0.7.0/zhousflib/locust/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.7.0/zhousflib/locust/__init__.py
+-rw-rw-rw-   0        0        0     1544 2023-06-09 06:20:55.000000 zhousf-lib-0.7.0/zhousflib/locust/locust_demo.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:10.026838 zhousf-lib-0.7.0/zhousflib/pandas/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.7.0/zhousflib/pandas/__init__.py
+-rw-rw-rw-   0        0        0     3556 2023-06-14 07:15:37.000000 zhousf-lib-0.7.0/zhousflib/pandas/openpyxl_util.py
+-rw-rw-rw-   0        0        0     5737 2023-06-14 07:15:37.000000 zhousf-lib-0.7.0/zhousflib/pandas/pandas_util.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:10.038838 zhousf-lib-0.7.0/zhousflib/pdf/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.7.0/zhousflib/pdf/__init__.py
+-rw-rw-rw-   0        0        0     1845 2023-06-07 01:49:12.000000 zhousf-lib-0.7.0/zhousflib/pdf/export_image.py
+-rw-rw-rw-   0        0        0     1467 2023-06-08 02:34:30.000000 zhousf-lib-0.7.0/zhousflib/pdf/pdfplumber_util.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:10.163869 zhousf-lib-0.7.0/zhousflib/util/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.7.0/zhousflib/util/__init__.py
+-rw-rw-rw-   0        0        0     2770 2023-06-07 01:49:13.000000 zhousf-lib-0.7.0/zhousflib/util/calculater_util.py
+-rw-rw-rw-   0        0        0      635 2023-06-07 01:49:12.000000 zhousf-lib-0.7.0/zhousflib/util/cv_util.py
+-rw-rw-rw-   0        0        0     2193 2023-06-07 01:49:13.000000 zhousf-lib-0.7.0/zhousflib/util/encrypt_util.py
+-rw-rw-rw-   0        0        0     1592 2023-06-14 06:14:27.000000 zhousf-lib-0.7.0/zhousflib/util/img_util.py
+-rw-rw-rw-   0        0        0    12930 2023-06-07 01:49:12.000000 zhousf-lib-0.7.0/zhousflib/util/iou_util.py
+-rw-rw-rw-   0        0        0     3373 2023-06-07 01:49:12.000000 zhousf-lib-0.7.0/zhousflib/util/json_util.py
+-rw-rw-rw-   0        0        0      749 2023-06-13 08:44:02.000000 zhousf-lib-0.7.0/zhousflib/util/list_util.py
+-rw-rw-rw-   0        0        0     1358 2023-06-07 01:49:12.000000 zhousf-lib-0.7.0/zhousflib/util/permission_util.py
+-rw-rw-rw-   0        0        0     3524 2023-06-07 01:49:11.000000 zhousf-lib-0.7.0/zhousflib/util/poly_util.py
+-rw-rw-rw-   0        0        0      633 2023-06-07 01:49:12.000000 zhousf-lib-0.7.0/zhousflib/util/re_util.py
+-rw-rw-rw-   0        0        0      520 2023-06-07 01:49:12.000000 zhousf-lib-0.7.0/zhousflib/util/singleton.py
+-rw-rw-rw-   0        0        0     4246 2023-06-09 06:46:55.000000 zhousf-lib-0.7.0/zhousflib/util/string_util.py
+-rw-rw-rw-   0        0        0     4663 2023-06-07 01:49:11.000000 zhousf-lib-0.7.0/zhousflib/util/time_util.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:16:10.212425 zhousf-lib-0.7.0/zhousflib/web/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.7.0/zhousflib/web/__init__.py
+-rw-rw-rw-   0        0        0     4355 2023-06-07 01:49:13.000000 zhousf-lib-0.7.0/zhousflib/web/config.py
+-rw-rw-rw-   0        0        0     3105 2023-06-07 01:49:12.000000 zhousf-lib-0.7.0/zhousflib/web/log_util.py
+-rw-rw-rw-   0        0        0     2860 2023-06-07 01:49:13.000000 zhousf-lib-0.7.0/zhousflib/web/logger.py
+-rw-rw-rw-   0        0        0     1340 2023-06-07 01:49:13.000000 zhousf-lib-0.7.0/zhousflib/web/response.py
```

### Comparing `zhousf-lib-0.6.9/LICENSE` & `zhousf-lib-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/PKG-INFO` & `zhousf-lib-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 0.6.9
+Version: 0.7.0
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-0.6.9/README.md` & `zhousf-lib-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/setup.py` & `zhousf-lib-0.7.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # 打包：python setup.py upload
 NAME = 'zhousf-lib'
 DESCRIPTION = 'a python library of zhousf'
 URL = 'https://github.com/MrZhousf/ZhousfLib'
 EMAIL = '442553199@qq.com'
 AUTHOR = 'zhousf'
 REQUIRES_PYTHON = '>=3.6.13'
-VERSION = '0.6.9'
+VERSION = '0.7.0'
 PACKAGE_DATA = {'': ['*.yaml', '*.ttf', '*.txt', '*.md']}
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 # What packages are required for this module to be executed?
```

### Comparing `zhousf-lib-0.6.9/zhousf_lib.egg-info/PKG-INFO` & `zhousf-lib-0.7.0/zhousf_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 0.6.9
+Version: 0.7.0
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-0.6.9/zhousf_lib.egg-info/SOURCES.txt` & `zhousf-lib-0.7.0/zhousf_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/datasets/coco/coco_bbox_extract.py` & `zhousf-lib-0.7.0/zhousflib/datasets/coco/coco_bbox_extract.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/datasets/coco/coco_bbox_update.py` & `zhousf-lib-0.7.0/zhousflib/datasets/coco/coco_bbox_update.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/datasets/coco/coco_bbox_vis.py` & `zhousf-lib-0.7.0/zhousflib/datasets/coco/coco_bbox_vis.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/datasets/coco/coco_dataset_merge.py` & `zhousf-lib-0.7.0/zhousflib/datasets/coco/coco_dataset_merge.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/datasets/coco/coco_dataset_split.py` & `zhousf-lib-0.7.0/zhousflib/datasets/coco/coco_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/datasets/labelme/labelme_clip.py` & `zhousf-lib-0.7.0/zhousflib/datasets/labelme/labelme_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/datasets/labelme/labelme_convert_coco.py` & `zhousf-lib-0.7.0/zhousflib/datasets/labelme/labelme_convert_coco.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/datasets/labelme/labelme_convert_seg.py` & `zhousf-lib-0.7.0/zhousflib/datasets/labelme/labelme_convert_seg.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/datasets/labelme/labelme_dataset_clip.py` & `zhousf-lib-0.7.0/zhousflib/datasets/labelme/labelme_dataset_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/datasets/segmentation/seg_dataset_split.py` & `zhousf-lib-0.7.0/zhousflib/datasets/segmentation/seg_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/db/lmdb_master.py` & `zhousf-lib-0.7.0/zhousflib/db/lmdb_master.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/decorator/interceptor_util.py` & `zhousf-lib-0.7.0/zhousflib/decorator/interceptor_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/font/SimSun.ttf` & `zhousf-lib-0.7.0/zhousflib/font/SimSun.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/font/Symbola.ttf` & `zhousf-lib-0.7.0/zhousflib/font/Symbola.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/font/__init__.py` & `zhousf-lib-0.7.0/zhousflib/font/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/locust/locust_demo.py` & `zhousf-lib-0.7.0/zhousflib/locust/locust_demo.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/pandas/openpyxl_util.py` & `zhousf-lib-0.7.0/zhousflib/pandas/openpyxl_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,15 +67,20 @@
                         if cell.value and not next_cell.value:
                             next_cell.value = cell.value
         """
         拆分合并单元格后会有重复的两条，这里去重一下
         """
         if delete_duplicates:
             for fill in need_fill:
-                worksheet.delete_rows(idx=fill[1])
+                data = []
+                for row_cells in worksheet.iter_rows(min_row=min(fill), max_row=max(fill)):
+                    data.append([cell.value for cell in row_cells])
+                if len(data) == 2:
+                    if data[0] == data[1]:
+                        worksheet.delete_rows(idx=fill[1])
     if tmp_excel:
         wb.save(str(tmp_excel))
         wb.close()
         return tmp_excel
     else:
         if contain_merge_cells:
             wb.save(str(excel_file))
```

### Comparing `zhousf-lib-0.6.9/zhousflib/pandas/pandas_util.py` & `zhousf-lib-0.7.0/zhousflib/pandas/pandas_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,11 +160,8 @@
     """
     with open(csv_path, "w") as file:
         writer = csv.writer(file)
         writer.writerows(data)
 
 
 if __name__ == "__main__":
-    df = read_excel_merge_cell(file_path=Path(r"C:\Users\zhousf-a\Desktop\1_ocr_data.xlsx"))
-    for index, row in df.iterrows():
-        print(row)
     pass
```

### Comparing `zhousf-lib-0.6.9/zhousflib/pdf/export_image.py` & `zhousf-lib-0.7.0/zhousflib/pdf/export_image.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/pdf/pdfplumber_util.py` & `zhousf-lib-0.7.0/zhousflib/pdf/pdfplumber_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/util/calculater_util.py` & `zhousf-lib-0.7.0/zhousflib/util/calculater_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/util/cv_util.py` & `zhousf-lib-0.7.0/zhousflib/util/cv_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/util/encrypt_util.py` & `zhousf-lib-0.7.0/zhousflib/util/encrypt_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/util/img_util.py` & `zhousf-lib-0.7.0/zhousflib/util/img_util.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,18 +3,28 @@
 # Description:
 import imghdr
 import base64
 import hashlib
 from pathlib import Path
 
 
-def get_file_base64(file_file: Path):
-    with file_file.open('rb') as infile:
+def get_file_base64(file_path: Path, contain_file_name=True, split_char=","):
+    """
+    图片转base64
+    :param file_path: 图片路径
+    :param contain_file_name: 是否包含文件名称
+    :param split_char: 分隔符
+    :return: 'a.jpg,iVBORw0KGgoAAAANSUhEUgAABNcAAANtCAYAAACzHZ25AAA.....'
+    """
+    with file_path.open('rb') as infile:
         s = infile.read()
-    return base64.b64encode(s).decode("utf-8")
+    base64_str = base64.b64encode(s).decode("utf-8")
+    if contain_file_name:
+        base64_str = file_path.name + split_char + base64_str
+    return base64_str
 
 
 def md5(file_path: Path):
     with file_path.open('rb') as f:
         return hashlib.md5(f.read()).hexdigest()
 
 
@@ -30,16 +40,16 @@
         count += 1
         new_name = md5(file)
         new_name += file.suffix
         print(new_name)
         if dst_dir.joinpath(new_name).exists():
             repeat += 1
             continue
-        file.rename(dst_dir.joinpath(new_name))
+        if not dst_dir.joinpath(file.parent.name).exists():
+            dst_dir.joinpath(file.parent.name).mkdir(parents=True)
+        file.rename(dst_dir.joinpath(file.parent.name).joinpath(new_name))
     print("count=", count)
     print("repeat=", repeat)
 
 
 if __name__ == "__main__":
-    src_dir_ = Path("/Users/zhousf/Desktop/工作空间/土建排布图/标注数据/目标检测/第3批/第三批已筛选图纸-3.24交付")
-    dst_dir_ = Path("/Users/zhousf/Desktop/工作空间/土建排布图/标注数据/目标检测/第3批/原图1")
-    rename_image_with_md5(src_dir_, dst_dir_)
+    pass
```

### Comparing `zhousf-lib-0.6.9/zhousflib/util/iou_util.py` & `zhousf-lib-0.7.0/zhousflib/util/iou_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/util/json_util.py` & `zhousf-lib-0.7.0/zhousflib/util/json_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/util/permission_util.py` & `zhousf-lib-0.7.0/zhousflib/util/permission_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/util/poly_util.py` & `zhousf-lib-0.7.0/zhousflib/util/poly_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/util/re_util.py` & `zhousf-lib-0.7.0/zhousflib/util/re_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/util/singleton.py` & `zhousf-lib-0.7.0/zhousflib/util/singleton.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/util/string_util.py` & `zhousf-lib-0.7.0/zhousflib/util/string_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/util/time_util.py` & `zhousf-lib-0.7.0/zhousflib/util/time_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/web/config.py` & `zhousf-lib-0.7.0/zhousflib/web/config.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/web/log_util.py` & `zhousf-lib-0.7.0/zhousflib/web/log_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/web/logger.py` & `zhousf-lib-0.7.0/zhousflib/web/logger.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.9/zhousflib/web/response.py` & `zhousf-lib-0.7.0/zhousflib/web/response.py`

 * *Files identical despite different names*

