# Comparing `tmp/pcleaner-1.7.3.tar.gz` & `tmp/pcleaner-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcleaner-1.7.3.tar", last modified: Mon May  8 16:51:44 2023, max compression
+gzip compressed data, was "pcleaner-1.7.4.tar", last modified: Wed Jun 14 00:44:09 2023, max compression
```

## Comparing `pcleaner-1.7.3.tar` & `pcleaner-1.7.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:51:44.734479 pcleaner-1.7.3/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.7.3/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)    12273 2023-05-08 16:51:44.734479 pcleaner-1.7.3/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11599 2023-05-04 21:07:46.000000 pcleaner-1.7.3/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:51:44.727812 pcleaner-1.7.3/pcleaner/
--rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2023-05-08 16:51:12.000000 pcleaner-1.7.3/pcleaner/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    19402 2023-05-04 21:08:14.000000 pcleaner-1.7.3/pcleaner/analytics.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6380 2023-05-04 21:08:14.000000 pcleaner-1.7.3/pcleaner/cli_utils.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:51:44.727812 pcleaner-1.7.3/pcleaner/comic_text_detector/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/basemodel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/inference.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:51:44.727812 pcleaner-1.7.3/pcleaner/comic_text_detector/models/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/models/__init__.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:51:44.727812 pcleaner-1.7.3/pcleaner/comic_text_detector/models/yolov5/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/models/yolov5/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/models/yolov5/common.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/models/yolov5/yolo.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:51:44.731146 pcleaner-1.7.3/pcleaner/comic_text_detector/utils/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/utils/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/utils/db_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/utils/export.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/utils/general.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/utils/imgproc_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/utils/io_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/utils/loss.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/utils/textblock.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/utils/textmask.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/utils/weight_init.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.7.3/pcleaner/comic_text_detector/utils/yolov5_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    45878 2023-05-08 00:59:00.000000 pcleaner-1.7.3/pcleaner/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6237 2023-05-08 16:47:38.000000 pcleaner-1.7.3/pcleaner/ctd_interface.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:51:44.731146 pcleaner-1.7.3/pcleaner/data/
--rw-r--r--   0 corbin    (1000) corbin    (1001)   410712 2021-09-30 18:43:41.000000 pcleaner-1.7.3/pcleaner/data/LiberationSans-Regular.ttf
--rw-r--r--   0 corbin    (1000) corbin    (1001)   107848 2018-04-08 15:54:09.000000 pcleaner-1.7.3/pcleaner/data/NotoMono-Regular.ttf
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner-1.7.3/pcleaner/data/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5573 2023-04-14 12:31:20.000000 pcleaner-1.7.3/pcleaner/denoiser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:51:44.731146 pcleaner-1.7.3/pcleaner/gui/
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:51:44.731146 pcleaner-1.7.3/pcleaner/gui/CustomQ/
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2600 2023-05-05 16:04:17.000000 pcleaner-1.7.3/pcleaner/gui/CustomQ/CColorButton.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3651 2023-05-08 16:20:55.000000 pcleaner-1.7.3/pcleaner/gui/CustomQ/CComboBox.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3234 2023-04-21 15:08:36.000000 pcleaner-1.7.3/pcleaner/gui/CustomQ/CTableWidget.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-1.7.3/pcleaner/gui/CustomQ/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-1.7.3/pcleaner/gui/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    21094 2023-05-05 16:04:17.000000 pcleaner-1.7.3/pcleaner/gui/file_table.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1094 2023-05-05 20:27:29.000000 pcleaner-1.7.3/pcleaner/gui/gui_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1958 2023-04-22 17:01:16.000000 pcleaner-1.7.3/pcleaner/gui/launcher.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    48840 2023-05-08 16:25:13.000000 pcleaner-1.7.3/pcleaner/gui/mainwindow_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4457 2023-05-05 16:04:17.000000 pcleaner-1.7.3/pcleaner/gui/new_profile_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    16366 2023-05-08 02:27:17.000000 pcleaner-1.7.3/pcleaner/gui/profile_parser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:51:44.731146 pcleaner-1.7.3/pcleaner/gui/rc_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-1.7.3/pcleaner/gui/rc_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10008 2023-04-22 16:59:47.000000 pcleaner-1.7.3/pcleaner/gui/rc_generated_files/icons_rc.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    84179 2023-05-08 16:50:50.000000 pcleaner-1.7.3/pcleaner/gui/rc_generated_files/theme_icons_rc.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:51:44.734479 pcleaner-1.7.3/pcleaner/gui/ui_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 00:09:43.000000 pcleaner-1.7.3/pcleaner/gui/ui_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6310 2023-04-17 00:10:07.000000 pcleaner-1.7.3/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    30265 2023-05-08 02:51:16.000000 pcleaner-1.7.3/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7464 2023-05-05 16:04:17.000000 pcleaner-1.7.3/pcleaner/gui/ui_generated_files/ui_NewProfile.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3233 2023-05-05 16:04:17.000000 pcleaner-1.7.3/pcleaner/gui/worker_thread.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1828 2023-04-21 20:13:16.000000 pcleaner-1.7.3/pcleaner/helpers.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    23467 2023-05-05 14:10:21.000000 pcleaner-1.7.3/pcleaner/image_ops.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27106 2023-05-08 01:47:32.000000 pcleaner-1.7.3/pcleaner/main.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8762 2023-05-06 17:47:48.000000 pcleaner-1.7.3/pcleaner/masker.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4845 2023-04-14 12:51:27.000000 pcleaner-1.7.3/pcleaner/model_downloader.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8817 2023-05-06 17:51:16.000000 pcleaner-1.7.3/pcleaner/pre_processor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7989 2023-05-08 02:36:30.000000 pcleaner-1.7.3/pcleaner/profile_cli.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14109 2023-05-06 17:51:42.000000 pcleaner-1.7.3/pcleaner/structures.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-08 16:51:44.727812 pcleaner-1.7.3/pcleaner.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    12273 2023-05-08 16:51:44.000000 pcleaner-1.7.3/pcleaner.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2218 2023-05-08 16:51:44.000000 pcleaner-1.7.3/pcleaner.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-05-08 16:51:44.000000 pcleaner-1.7.3/pcleaner.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-05-08 16:51:44.000000 pcleaner-1.7.3/pcleaner.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      188 2023-05-08 16:51:44.000000 pcleaner-1.7.3/pcleaner.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-05-08 16:51:44.000000 pcleaner-1.7.3/pcleaner.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.7.3/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1138 2023-05-08 16:51:44.734479 pcleaner-1.7.3/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.7.3/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-06-14 00:44:09.663677 pcleaner-1.7.4/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.7.4/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    12273 2023-06-14 00:44:09.663677 pcleaner-1.7.4/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11599 2023-05-04 21:07:46.000000 pcleaner-1.7.4/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-06-14 00:44:09.660344 pcleaner-1.7.4/pcleaner/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2023-06-14 00:44:05.000000 pcleaner-1.7.4/pcleaner/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    19402 2023-05-04 21:08:14.000000 pcleaner-1.7.4/pcleaner/analytics.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6380 2023-05-04 21:08:14.000000 pcleaner-1.7.4/pcleaner/cli_utils.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-06-14 00:44:09.660344 pcleaner-1.7.4/pcleaner/comic_text_detector/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/basemodel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/inference.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-06-14 00:44:09.660344 pcleaner-1.7.4/pcleaner/comic_text_detector/models/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/models/__init__.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-06-14 00:44:09.660344 pcleaner-1.7.4/pcleaner/comic_text_detector/models/yolov5/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/models/yolov5/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/models/yolov5/common.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/models/yolov5/yolo.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-06-14 00:44:09.663677 pcleaner-1.7.4/pcleaner/comic_text_detector/utils/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/utils/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/utils/db_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/utils/export.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/utils/general.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/utils/imgproc_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/utils/io_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/utils/loss.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/utils/textblock.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/utils/textmask.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/utils/weight_init.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.7.4/pcleaner/comic_text_detector/utils/yolov5_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    45991 2023-05-11 14:15:02.000000 pcleaner-1.7.4/pcleaner/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6237 2023-05-08 16:47:38.000000 pcleaner-1.7.4/pcleaner/ctd_interface.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-06-14 00:44:09.663677 pcleaner-1.7.4/pcleaner/data/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   410712 2021-09-30 18:43:41.000000 pcleaner-1.7.4/pcleaner/data/LiberationSans-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   107848 2018-04-08 15:54:09.000000 pcleaner-1.7.4/pcleaner/data/NotoMono-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner-1.7.4/pcleaner/data/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5573 2023-04-14 12:31:20.000000 pcleaner-1.7.4/pcleaner/denoiser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-06-14 00:44:09.663677 pcleaner-1.7.4/pcleaner/gui/
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-06-14 00:44:09.663677 pcleaner-1.7.4/pcleaner/gui/CustomQ/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2600 2023-05-05 16:04:17.000000 pcleaner-1.7.4/pcleaner/gui/CustomQ/CColorButton.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3651 2023-05-08 16:20:55.000000 pcleaner-1.7.4/pcleaner/gui/CustomQ/CComboBox.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3234 2023-04-21 15:08:36.000000 pcleaner-1.7.4/pcleaner/gui/CustomQ/CTableWidget.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-1.7.4/pcleaner/gui/CustomQ/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-1.7.4/pcleaner/gui/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    21094 2023-05-05 16:04:17.000000 pcleaner-1.7.4/pcleaner/gui/file_table.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1094 2023-05-05 20:27:29.000000 pcleaner-1.7.4/pcleaner/gui/gui_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1958 2023-04-22 17:01:16.000000 pcleaner-1.7.4/pcleaner/gui/launcher.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    48840 2023-05-08 16:25:13.000000 pcleaner-1.7.4/pcleaner/gui/mainwindow_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4457 2023-05-05 16:04:17.000000 pcleaner-1.7.4/pcleaner/gui/new_profile_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    16366 2023-05-08 02:27:17.000000 pcleaner-1.7.4/pcleaner/gui/profile_parser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-06-14 00:44:09.663677 pcleaner-1.7.4/pcleaner/gui/rc_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-1.7.4/pcleaner/gui/rc_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10008 2023-04-22 16:59:47.000000 pcleaner-1.7.4/pcleaner/gui/rc_generated_files/icons_rc.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    84179 2023-05-08 16:50:50.000000 pcleaner-1.7.4/pcleaner/gui/rc_generated_files/theme_icons_rc.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-06-14 00:44:09.663677 pcleaner-1.7.4/pcleaner/gui/ui_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 00:09:43.000000 pcleaner-1.7.4/pcleaner/gui/ui_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6310 2023-04-17 00:10:07.000000 pcleaner-1.7.4/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    30265 2023-05-08 02:51:16.000000 pcleaner-1.7.4/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7464 2023-05-05 16:04:17.000000 pcleaner-1.7.4/pcleaner/gui/ui_generated_files/ui_NewProfile.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3233 2023-05-05 16:04:17.000000 pcleaner-1.7.4/pcleaner/gui/worker_thread.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1828 2023-04-21 20:13:16.000000 pcleaner-1.7.4/pcleaner/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    23683 2023-05-11 17:47:34.000000 pcleaner-1.7.4/pcleaner/image_ops.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27094 2023-06-14 00:36:17.000000 pcleaner-1.7.4/pcleaner/main.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8762 2023-05-06 17:47:48.000000 pcleaner-1.7.4/pcleaner/masker.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4845 2023-04-14 12:51:27.000000 pcleaner-1.7.4/pcleaner/model_downloader.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8773 2023-05-11 14:11:11.000000 pcleaner-1.7.4/pcleaner/pre_processor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7989 2023-05-08 02:36:30.000000 pcleaner-1.7.4/pcleaner/profile_cli.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14109 2023-05-06 17:51:42.000000 pcleaner-1.7.4/pcleaner/structures.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-06-14 00:44:09.660344 pcleaner-1.7.4/pcleaner.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    12273 2023-06-14 00:44:09.000000 pcleaner-1.7.4/pcleaner.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2218 2023-06-14 00:44:09.000000 pcleaner-1.7.4/pcleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-06-14 00:44:09.000000 pcleaner-1.7.4/pcleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-06-14 00:44:09.000000 pcleaner-1.7.4/pcleaner.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      188 2023-06-14 00:44:09.000000 pcleaner-1.7.4/pcleaner.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-06-14 00:44:09.000000 pcleaner-1.7.4/pcleaner.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.7.4/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1138 2023-06-14 00:44:09.663677 pcleaner-1.7.4/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.7.4/setup.py
```

### Comparing `pcleaner-1.7.3/LICENSE` & `pcleaner-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/PKG-INFO` & `pcleaner-1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.7.3
+Version: 1.7.4
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pcleaner-1.7.3/README.md` & `pcleaner-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/analytics.py` & `pcleaner-1.7.4/pcleaner/analytics.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/cli_utils.py` & `pcleaner-1.7.4/pcleaner/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/comic_text_detector/basemodel.py` & `pcleaner-1.7.4/pcleaner/comic_text_detector/basemodel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/comic_text_detector/inference.py` & `pcleaner-1.7.4/pcleaner/comic_text_detector/inference.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/comic_text_detector/models/yolov5/common.py` & `pcleaner-1.7.4/pcleaner/comic_text_detector/models/yolov5/common.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/comic_text_detector/models/yolov5/yolo.py` & `pcleaner-1.7.4/pcleaner/comic_text_detector/models/yolov5/yolo.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/comic_text_detector/utils/db_utils.py` & `pcleaner-1.7.4/pcleaner/comic_text_detector/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/comic_text_detector/utils/export.py` & `pcleaner-1.7.4/pcleaner/comic_text_detector/utils/export.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/comic_text_detector/utils/general.py` & `pcleaner-1.7.4/pcleaner/comic_text_detector/utils/general.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/comic_text_detector/utils/imgproc_utils.py` & `pcleaner-1.7.4/pcleaner/comic_text_detector/utils/imgproc_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/comic_text_detector/utils/io_utils.py` & `pcleaner-1.7.4/pcleaner/comic_text_detector/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/comic_text_detector/utils/loss.py` & `pcleaner-1.7.4/pcleaner/comic_text_detector/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/comic_text_detector/utils/textblock.py` & `pcleaner-1.7.4/pcleaner/comic_text_detector/utils/textblock.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/comic_text_detector/utils/textmask.py` & `pcleaner-1.7.4/pcleaner/comic_text_detector/utils/textmask.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/comic_text_detector/utils/weight_init.py` & `pcleaner-1.7.4/pcleaner/comic_text_detector/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/comic_text_detector/utils/yolov5_utils.py` & `pcleaner-1.7.4/pcleaner/comic_text_detector/utils/yolov5_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/config.py` & `pcleaner-1.7.4/pcleaner/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,14 +352,15 @@
         # When true, the mask selection algorith will pick the first perfect mask, if one is found early.
         # This is faster, but may not find the best mask, if a slightly bigger one would have been better.
         mask_selection_fast = {self.mask_selection_fast}
         
         # The maximum standard deviation of a mask to consider.
         # A high value here means a higher tolerance for the mask intersecting text or other objects,
         # which isn't a good mask, as it will require inpainting anyway.
+        # Setting this to 0 will only allow perfect masks, which is recommended for very high resolution images.
         mask_max_standard_deviation = {self.mask_max_standard_deviation}
         
         # Color to use for the debug mask. [CLI: This is a tuple of RGBA values.]
         debug_mask_color = {','.join(map(str, self.debug_mask_color))}
         
         """
         masker_conf = cu.ConfigUpdater()
```

### Comparing `pcleaner-1.7.3/pcleaner/ctd_interface.py` & `pcleaner-1.7.4/pcleaner/ctd_interface.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/data/LiberationSans-Regular.ttf` & `pcleaner-1.7.4/pcleaner/data/LiberationSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/data/NotoMono-Regular.ttf` & `pcleaner-1.7.4/pcleaner/data/NotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/denoiser.py` & `pcleaner-1.7.4/pcleaner/denoiser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/gui/CustomQ/CColorButton.py` & `pcleaner-1.7.4/pcleaner/gui/CustomQ/CColorButton.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/gui/CustomQ/CComboBox.py` & `pcleaner-1.7.4/pcleaner/gui/CustomQ/CComboBox.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/gui/CustomQ/CTableWidget.py` & `pcleaner-1.7.4/pcleaner/gui/CustomQ/CTableWidget.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/gui/file_table.py` & `pcleaner-1.7.4/pcleaner/gui/file_table.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/gui/gui_utils.py` & `pcleaner-1.7.4/pcleaner/gui/gui_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/gui/launcher.py` & `pcleaner-1.7.4/pcleaner/gui/launcher.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/gui/mainwindow_driver.py` & `pcleaner-1.7.4/pcleaner/gui/mainwindow_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/gui/new_profile_driver.py` & `pcleaner-1.7.4/pcleaner/gui/new_profile_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/gui/profile_parser.py` & `pcleaner-1.7.4/pcleaner/gui/profile_parser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/gui/rc_generated_files/icons_rc.py` & `pcleaner-1.7.4/pcleaner/gui/rc_generated_files/icons_rc.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/gui/rc_generated_files/theme_icons_rc.py` & `pcleaner-1.7.4/pcleaner/gui/rc_generated_files/theme_icons_rc.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/gui/ui_generated_files/ui_ImageDetails.py` & `pcleaner-1.7.4/pcleaner/gui/ui_generated_files/ui_ImageDetails.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/gui/ui_generated_files/ui_Mainwindow.py` & `pcleaner-1.7.4/pcleaner/gui/ui_generated_files/ui_Mainwindow.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/gui/ui_generated_files/ui_NewProfile.py` & `pcleaner-1.7.4/pcleaner/gui/ui_generated_files/ui_NewProfile.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/gui/worker_thread.py` & `pcleaner-1.7.4/pcleaner/gui/worker_thread.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/helpers.py` & `pcleaner-1.7.4/pcleaner/helpers.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/image_ops.py` & `pcleaner-1.7.4/pcleaner/image_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,28 +305,32 @@
     # but it could not exceed the image dimensions.
     # These relative coords are used to paste the mask onto the base image.
     x_offset = masking_box[0] - reference_box[0]
     y_offset = masking_box[1] - reference_box[1]
 
     # Replace all given images with their corresponding cutouts.
     base = cut_out_box(base, reference_box)
-    precise_mask = cut_out_mask(precise_mask, masking_box, base.size, x_offset, y_offset)
+    precise_mask_cut = cut_out_mask(precise_mask, masking_box, base.size, x_offset, y_offset)
 
     # Check that the precise mask is not blank.
-    if precise_mask.getbbox() is None:
+    if precise_mask_cut.getbbox() is None:
         # This means the box was probably just noise, so abort picking a mask.
-        logger.warning("Found an empty mask, this is likely due to name collisions.")
+        logger.warning(
+            "Found an empty mask, the Text Detector didn't find anything but still recorded text present.\n"
+            f"Image: {analytics_page_path.name} Masking box: {masking_box}, x offset: {x_offset}, y offset: {y_offset}."
+            f" Skipping."
+        )
         return None
 
     box_mask = cut_out_mask(box_mask, masking_box, base.size, x_offset, y_offset)
 
     # Generate masks of various sizes for the precise mask, then add the box mask to the list.
     # The generated masks are in ascending size order.
     mask_gen = make_mask_steps_convolution(
-        precise_mask,
+        precise_mask_cut,
         hp.scale_length_rounded(masker_conf.mask_growth_step_pixels, scale),
         masker_conf.mask_growth_steps,
     )
 
     # When using the fast mask selection, make a new generator with the box mask as the first mask,
     # followed by the generated masks.
     def generator_with_first(generator, first):
```

### Comparing `pcleaner-1.7.3/pcleaner/main.py` & `pcleaner-1.7.4/pcleaner/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 import time
 from multiprocessing import Pool
 from pathlib import Path
 import itertools
 from PIL import Image
 
 from manga_ocr import MangaOcr
-from docopt import magic_docopt
+from docopt import docopt
 from logzero import logger, loglevel, DEBUG, INFO
 from tqdm import tqdm
 from natsort import natsorted
 import torch
 import tifffile
 
 from pcleaner import __version__
@@ -135,15 +135,15 @@
 
 # Allow loading of large images.
 Image.MAX_IMAGE_PIXELS = 2**32
 
 
 def main():
 
-    args = magic_docopt(__doc__, version=f"Panel Cleaner {__version__}")
+    args = docopt(__doc__, version=f"Panel Cleaner {__version__}")
     # Loglevel is info by default.
     if args.debug:
         loglevel(DEBUG)
     else:
         loglevel(INFO)
 
     logger.debug(args)
```

### Comparing `pcleaner-1.7.3/pcleaner/masker.py` & `pcleaner-1.7.4/pcleaner/masker.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/model_downloader.py` & `pcleaner-1.7.4/pcleaner/model_downloader.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/pre_processor.py` & `pcleaner-1.7.4/pcleaner/pre_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,18 +63,16 @@
     :param mocr: [Optional] Manga ocr object.
     :param cache_masks_ocr: [Optional] Whether to cache the masks early for ocr.
     :return: Analytics data if the manga ocr object is given, None otherwise.
     """
     logger.debug(f"Processing json file: {json_file_path}")
 
     # Check if the file was already processed.
-    if json_file_path.name.endswith("#clean.json"):
-        return
-    if json_file_path.name.endswith("#mask_data.json"):
-        return
+    if not json_file_path.name.endswith("#raw.json"):
+        return None
 
     json_data = json.loads(json_file_path.read_text())
 
     image_path = json_data["image_path"]
     mask_path = json_data["mask_path"]
     original_path = json_data["original_path"]
     scale = json_data["scale"]
@@ -138,15 +136,15 @@
     # Copy the merged extended boxes to the reference boxes and grow them once again.
     page_data.reference_boxes = page_data.merged_extended_boxes.copy()
     page_data.grow_boxes(
         scale_len(pre_processor_conf.box_reference_padding), st.BoxType.REFERENCE_BOX
     )
 
     # Write the json file with the cleaned data.
-    json_out_path = json_file_path.parent / f"{json_file_path.stem}#clean.json"
+    json_out_path = json_file_path.parent / f"{json_file_path.stem.replace('#raw', '')}#clean.json"
     # Remove the _image_size attribute, because it's a cached value that may be unset.
     page_data_dict = asdict(page_data)
     del page_data_dict["_image_size"]
     json_out_path.write_text(json.dumps(page_data_dict, indent=4))
 
     # Draw the boxes on the image and save it.
     if cache_masks and not cache_masks_ocr:
```

### Comparing `pcleaner-1.7.3/pcleaner/profile_cli.py` & `pcleaner-1.7.4/pcleaner/profile_cli.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner/structures.py` & `pcleaner-1.7.4/pcleaner/structures.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/pcleaner.egg-info/PKG-INFO` & `pcleaner-1.7.4/pcleaner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.7.3
+Version: 1.7.4
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pcleaner-1.7.3/pcleaner.egg-info/SOURCES.txt` & `pcleaner-1.7.4/pcleaner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.3/setup.cfg` & `pcleaner-1.7.4/setup.cfg`

 * *Files identical despite different names*

