# Comparing `tmp/supervision-0.8.0.tar.gz` & `tmp/supervision-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supervision-0.8.0.tar", last modified: Wed May 17 19:36:51 2023, max compression
+gzip compressed data, was "supervision-0.9.0.tar", last modified: Wed Jun  7 10:58:26 2023, max compression
```

## Comparing `supervision-0.8.0.tar` & `supervision-0.9.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.562546 supervision-0.8.0/
--rw-r--r--   0 skalskip   (501) staff       (20)     1065 2022-12-02 12:52:46.000000 supervision-0.8.0/LICENSE.md
--rw-r--r--   0 skalskip   (501) staff       (20)     6201 2023-05-17 19:36:51.562405 supervision-0.8.0/PKG-INFO
--rw-r--r--   0 skalskip   (501) staff       (20)     4874 2023-05-17 19:02:43.000000 supervision-0.8.0/README.md
--rw-r--r--   0 skalskip   (501) staff       (20)       38 2023-05-17 19:36:51.562599 supervision-0.8.0/setup.cfg
--rw-r--r--   0 skalskip   (501) staff       (20)     2238 2023-05-17 17:05:52.000000 supervision-0.8.0/setup.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.554722 supervision-0.8.0/supervision/
--rw-r--r--   0 skalskip   (501) staff       (20)     1066 2023-05-17 17:05:52.000000 supervision-0.8.0/supervision/__init__.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.555997 supervision-0.8.0/supervision/dataset/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-19 14:17:19.000000 supervision-0.8.0/supervision/dataset/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)    13623 2023-05-17 19:34:46.000000 supervision-0.8.0/supervision/dataset/core.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.556667 supervision-0.8.0/supervision/dataset/formats/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-19 14:17:19.000000 supervision-0.8.0/supervision/dataset/formats/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5396 2023-05-17 17:05:52.000000 supervision-0.8.0/supervision/dataset/formats/pascal_voc.py
--rw-r--r--   0 skalskip   (501) staff       (20)     9267 2023-05-17 17:05:52.000000 supervision-0.8.0/supervision/dataset/formats/yolo.py
--rw-r--r--   0 skalskip   (501) staff       (20)     2357 2023-05-17 18:23:25.000000 supervision-0.8.0/supervision/dataset/ultils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.558026 supervision-0.8.0/supervision/detection/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.8.0/supervision/detection/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     6799 2023-05-09 10:13:33.000000 supervision-0.8.0/supervision/detection/annotate.py
--rw-r--r--   0 skalskip   (501) staff       (20)    20838 2023-05-16 14:15:01.000000 supervision-0.8.0/supervision/detection/core.py
--rw-r--r--   0 skalskip   (501) staff       (20)     7667 2023-05-17 17:05:52.000000 supervision-0.8.0/supervision/detection/line_counter.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.558342 supervision-0.8.0/supervision/detection/tools/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-10 21:52:53.000000 supervision-0.8.0/supervision/detection/tools/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5056 2023-04-19 14:17:19.000000 supervision-0.8.0/supervision/detection/tools/polygon_zone.py
--rw-r--r--   0 skalskip   (501) staff       (20)     9949 2023-05-17 17:05:52.000000 supervision-0.8.0/supervision/detection/utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.558971 supervision-0.8.0/supervision/draw/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.8.0/supervision/draw/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     3675 2023-02-07 18:30:08.000000 supervision-0.8.0/supervision/draw/color.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5147 2023-03-13 13:53:19.000000 supervision-0.8.0/supervision/draw/utils.py
--rw-r--r--   0 skalskip   (501) staff       (20)     2116 2023-05-17 17:05:52.000000 supervision-0.8.0/supervision/file.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.559513 supervision-0.8.0/supervision/geometry/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.8.0/supervision/geometry/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1397 2023-02-07 18:30:08.000000 supervision-0.8.0/supervision/geometry/core.py
--rw-r--r--   0 skalskip   (501) staff       (20)      993 2023-02-07 18:30:08.000000 supervision-0.8.0/supervision/geometry/utils.py
--rw-r--r--   0 skalskip   (501) staff       (20)      421 2023-05-03 22:43:10.000000 supervision-0.8.0/supervision/internal.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.559823 supervision-0.8.0/supervision/notebook/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.8.0/supervision/notebook/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     2839 2023-05-03 22:43:10.000000 supervision-0.8.0/supervision/notebook/utils.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5049 2023-02-07 18:30:08.000000 supervision-0.8.0/supervision/video.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.555583 supervision-0.8.0/supervision.egg-info/
--rw-r--r--   0 skalskip   (501) staff       (20)     6201 2023-05-17 19:36:51.000000 supervision-0.8.0/supervision.egg-info/PKG-INFO
--rw-r--r--   0 skalskip   (501) staff       (20)     1313 2023-05-17 19:36:51.000000 supervision-0.8.0/supervision.egg-info/SOURCES.txt
--rw-r--r--   0 skalskip   (501) staff       (20)        1 2023-05-17 19:36:51.000000 supervision-0.8.0/supervision.egg-info/dependency_links.txt
--rw-r--r--   0 skalskip   (501) staff       (20)      145 2023-05-17 19:36:51.000000 supervision-0.8.0/supervision.egg-info/requires.txt
--rw-r--r--   0 skalskip   (501) staff       (20)       17 2023-05-17 19:36:51.000000 supervision-0.8.0/supervision.egg-info/top_level.txt
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.560095 supervision-0.8.0/test/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.8.0/test/__init__.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.560312 supervision-0.8.0/test/dataset/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-05-10 12:01:26.000000 supervision-0.8.0/test/dataset/__init__.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.560699 supervision-0.8.0/test/dataset/formats/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-05-10 12:01:26.000000 supervision-0.8.0/test/dataset/formats/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     9650 2023-05-17 17:05:52.000000 supervision-0.8.0/test/dataset/formats/test_yolo.py
--rw-r--r--   0 skalskip   (501) staff       (20)     2344 2023-05-17 18:23:25.000000 supervision-0.8.0/test/dataset/test_utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.561378 supervision-0.8.0/test/detection/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.8.0/test/detection/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     6749 2023-05-04 15:46:53.000000 supervision-0.8.0/test/detection/test_core.py
--rw-r--r--   0 skalskip   (501) staff       (20)     8054 2023-04-19 14:17:19.000000 supervision-0.8.0/test/detection/test_utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.561746 supervision-0.8.0/test/draw/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.8.0/test/draw/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1097 2023-02-02 10:53:06.000000 supervision-0.8.0/test/draw/test_color.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.562128 supervision-0.8.0/test/geometry/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.8.0/test/geometry/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1854 2023-02-07 18:30:08.000000 supervision-0.8.0/test/geometry/test_dataclasses.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-06-07 10:58:26.559666 supervision-0.9.0/
+-rw-r--r--   0 skalskip   (501) staff       (20)     1065 2022-12-02 12:52:46.000000 supervision-0.9.0/LICENSE.md
+-rw-r--r--   0 skalskip   (501) staff       (20)    11138 2023-06-07 10:58:26.559440 supervision-0.9.0/PKG-INFO
+-rw-r--r--   0 skalskip   (501) staff       (20)     9760 2023-06-07 09:34:12.000000 supervision-0.9.0/README.md
+-rw-r--r--   0 skalskip   (501) staff       (20)       38 2023-06-07 10:58:26.559716 supervision-0.9.0/setup.cfg
+-rw-r--r--   0 skalskip   (501) staff       (20)     2288 2023-06-07 09:34:12.000000 supervision-0.9.0/setup.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-06-07 10:58:26.552385 supervision-0.9.0/supervision/
+-rw-r--r--   0 skalskip   (501) staff       (20)     1130 2023-06-07 10:20:35.000000 supervision-0.9.0/supervision/__init__.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-06-07 10:58:26.553694 supervision-0.9.0/supervision/dataset/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-19 14:17:19.000000 supervision-0.9.0/supervision/dataset/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)    13629 2023-06-07 09:37:46.000000 supervision-0.9.0/supervision/dataset/core.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-06-07 10:58:26.554133 supervision-0.9.0/supervision/dataset/formats/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-19 14:17:19.000000 supervision-0.9.0/supervision/dataset/formats/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5396 2023-05-17 17:05:52.000000 supervision-0.9.0/supervision/dataset/formats/pascal_voc.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     9290 2023-06-07 09:39:58.000000 supervision-0.9.0/supervision/dataset/formats/yolo.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     2357 2023-05-17 18:23:25.000000 supervision-0.9.0/supervision/dataset/ultils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-06-07 10:58:26.554888 supervision-0.9.0/supervision/detection/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.9.0/supervision/detection/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     6799 2023-05-09 10:13:33.000000 supervision-0.9.0/supervision/detection/annotate.py
+-rw-r--r--   0 skalskip   (501) staff       (20)    21488 2023-06-07 09:37:46.000000 supervision-0.9.0/supervision/detection/core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     7667 2023-05-17 17:05:52.000000 supervision-0.9.0/supervision/detection/line_counter.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-06-07 10:58:26.555155 supervision-0.9.0/supervision/detection/tools/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-10 21:52:53.000000 supervision-0.9.0/supervision/detection/tools/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5133 2023-06-07 10:00:39.000000 supervision-0.9.0/supervision/detection/tools/polygon_zone.py
+-rw-r--r--   0 skalskip   (501) staff       (20)    10969 2023-06-07 09:34:12.000000 supervision-0.9.0/supervision/detection/utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-06-07 10:58:26.555574 supervision-0.9.0/supervision/draw/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.9.0/supervision/draw/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     3675 2023-02-07 18:30:08.000000 supervision-0.9.0/supervision/draw/color.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5147 2023-03-13 13:53:19.000000 supervision-0.9.0/supervision/draw/utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-06-07 10:58:26.556105 supervision-0.9.0/supervision/geometry/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.9.0/supervision/geometry/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1397 2023-02-07 18:30:08.000000 supervision-0.9.0/supervision/geometry/core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)      993 2023-02-07 18:30:08.000000 supervision-0.9.0/supervision/geometry/utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-06-07 10:58:26.556936 supervision-0.9.0/supervision/utils/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-06-07 09:36:50.000000 supervision-0.9.0/supervision/utils/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     2096 2023-06-07 09:45:11.000000 supervision-0.9.0/supervision/utils/file.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     3065 2023-06-07 10:20:35.000000 supervision-0.9.0/supervision/utils/image.py
+-rw-r--r--   0 skalskip   (501) staff       (20)      421 2023-06-04 13:10:07.000000 supervision-0.9.0/supervision/utils/internal.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     2839 2023-05-03 22:43:10.000000 supervision-0.9.0/supervision/utils/notebook.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5299 2023-06-07 09:34:12.000000 supervision-0.9.0/supervision/utils/video.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-06-07 10:58:26.553240 supervision-0.9.0/supervision.egg-info/
+-rw-r--r--   0 skalskip   (501) staff       (20)    11138 2023-06-07 10:58:26.000000 supervision-0.9.0/supervision.egg-info/PKG-INFO
+-rw-r--r--   0 skalskip   (501) staff       (20)     1355 2023-06-07 10:58:26.000000 supervision-0.9.0/supervision.egg-info/SOURCES.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)        1 2023-06-07 10:58:26.000000 supervision-0.9.0/supervision.egg-info/dependency_links.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)      145 2023-06-07 10:58:26.000000 supervision-0.9.0/supervision.egg-info/requires.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)       17 2023-06-07 10:58:26.000000 supervision-0.9.0/supervision.egg-info/top_level.txt
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-06-07 10:58:26.557091 supervision-0.9.0/test/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.9.0/test/__init__.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-06-07 10:58:26.557314 supervision-0.9.0/test/dataset/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-05-10 12:01:26.000000 supervision-0.9.0/test/dataset/__init__.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-06-07 10:58:26.557718 supervision-0.9.0/test/dataset/formats/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-05-10 12:01:26.000000 supervision-0.9.0/test/dataset/formats/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     9650 2023-05-17 17:05:52.000000 supervision-0.9.0/test/dataset/formats/test_yolo.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     2344 2023-05-17 18:23:25.000000 supervision-0.9.0/test/dataset/test_utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-06-07 10:58:26.558337 supervision-0.9.0/test/detection/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.9.0/test/detection/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     9524 2023-06-06 08:54:47.000000 supervision-0.9.0/test/detection/test_core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     8054 2023-04-19 14:17:19.000000 supervision-0.9.0/test/detection/test_utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-06-07 10:58:26.558706 supervision-0.9.0/test/draw/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.9.0/test/draw/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1097 2023-02-02 10:53:06.000000 supervision-0.9.0/test/draw/test_color.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-06-07 10:58:26.559071 supervision-0.9.0/test/geometry/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.9.0/test/geometry/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1854 2023-02-07 18:30:08.000000 supervision-0.9.0/test/geometry/test_dataclasses.py
```

### Comparing `supervision-0.8.0/LICENSE.md` & `supervision-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `supervision-0.8.0/setup.py` & `supervision-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Software Development',
         'Topic :: Scientific/Engineering',
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Scientific/Engineering :: Image Recognition",
         'Typing :: Typed',
         'Operating System :: Microsoft :: Windows',
```

### Comparing `supervision-0.8.0/supervision/__init__.py` & `supervision-0.9.0/supervision/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 from supervision.dataset.core import BaseDataset, DetectionDataset
 from supervision.detection.annotate import BoxAnnotator, MaskAnnotator
 from supervision.detection.core import Detections
 from supervision.detection.line_counter import LineZone, LineZoneAnnotator
 from supervision.detection.tools.polygon_zone import PolygonZone, PolygonZoneAnnotator
 from supervision.detection.utils import (
@@ -12,17 +12,18 @@
     mask_to_xyxy,
     non_max_suppression,
     polygon_to_mask,
     polygon_to_xyxy,
 )
 from supervision.draw.color import Color, ColorPalette
 from supervision.draw.utils import draw_filled_rectangle, draw_polygon, draw_text
-from supervision.file import list_files_with_extensions
 from supervision.geometry.core import Point, Position, Rect
 from supervision.geometry.utils import get_polygon_center
-from supervision.notebook.utils import plot_image, plot_images_grid
-from supervision.video import (
+from supervision.utils.file import list_files_with_extensions
+from supervision.utils.image import ImageSink, crop
+from supervision.utils.notebook import plot_image, plot_images_grid
+from supervision.utils.video import (
     VideoInfo,
     VideoSink,
     get_video_frames_generator,
     process_video,
 )
```

### Comparing `supervision-0.8.0/supervision/dataset/core.py` & `supervision-0.9.0/supervision/dataset/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from supervision.dataset.formats.yolo import (
     load_yolo_annotations,
     save_data_yaml,
     save_yolo_annotations,
 )
 from supervision.dataset.ultils import save_dataset_images, train_test_split
 from supervision.detection.core import Detections
-from supervision.file import list_files_with_extensions
+from supervision.utils.file import list_files_with_extensions
 
 
 @dataclass
 class BaseDataset(ABC):
     @abstractmethod
     def __len__(self) -> int:
         pass
```

### Comparing `supervision-0.8.0/supervision/dataset/formats/pascal_voc.py` & `supervision-0.9.0/supervision/dataset/formats/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `supervision-0.8.0/supervision/dataset/formats/yolo.py` & `supervision-0.9.0/supervision/dataset/formats/yolo.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 import cv2
 import numpy as np
 import yaml
 
 from supervision.dataset.ultils import approximate_mask_with_polygons
 from supervision.detection.core import Detections
 from supervision.detection.utils import polygon_to_mask, polygon_to_xyxy
-from supervision.file import list_files_with_extensions, read_txt_file, save_text_file
+from supervision.utils.file import (
+    list_files_with_extensions,
+    read_txt_file,
+    save_text_file,
+)
 
 
 def _parse_box(values: List[str]) -> np.ndarray:
     x_center, y_center, width, height = values
     return np.array(
         [
             float(x_center) - float(width) / 2,
```

### Comparing `supervision-0.8.0/supervision/dataset/ultils.py` & `supervision-0.9.0/supervision/dataset/ultils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.8.0/supervision/detection/annotate.py` & `supervision-0.9.0/supervision/detection/annotate.py`

 * *Files identical despite different names*

### Comparing `supervision-0.8.0/supervision/detection/core.py` & `supervision-0.9.0/supervision/detection/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from __future__ import annotations
 
 from dataclasses import astuple, dataclass
-from typing import Any, Iterator, List, Optional, Tuple
+from typing import Any, Iterator, List, Optional, Tuple, Union
 
+import cv2
 import numpy as np
 
-from supervision.detection.utils import non_max_suppression, xywh_to_xyxy
+from supervision.detection.utils import (
+    extract_yolov8_masks,
+    non_max_suppression,
+    xywh_to_xyxy,
+)
 from supervision.geometry.core import Position
-from supervision.internal import deprecated
+from supervision.utils.internal import deprecated
 
 
 def _validate_xyxy(xyxy: Any, n: int) -> None:
     is_valid = isinstance(xyxy, np.ndarray) and xyxy.shape == (n, 4)
     if not is_valid:
         raise ValueError("xyxy must be 2d np.ndarray with (n, 4) shape")
 
@@ -187,14 +192,15 @@
             >>> detections = sv.Detections.from_yolov8(result)
             ```
         """
         return cls(
             xyxy=yolov8_results.boxes.xyxy.cpu().numpy(),
             confidence=yolov8_results.boxes.conf.cpu().numpy(),
             class_id=yolov8_results.boxes.cls.cpu().numpy().astype(int),
+            mask=extract_yolov8_masks(yolov8_results),
         )
 
     @classmethod
     def from_yolo_nas(cls, yolo_nas_results) -> Detections:
         """
         Creates a Detections instance from a [YOLO-NAS](https://github.com/Deci-AI/super-gradients/blob/master/YOLONAS.md) inference result.
 
@@ -465,31 +471,51 @@
         elif anchor == Position.BOTTOM_CENTER:
             return np.array(
                 [(self.xyxy[:, 0] + self.xyxy[:, 2]) / 2, self.xyxy[:, 3]]
             ).transpose()
 
         raise ValueError(f"{anchor} is not supported.")
 
-    def __getitem__(self, index: np.ndarray) -> Detections:
-        if isinstance(index, np.ndarray) and (
-            index.dtype == bool or index.dtype == int
-        ):
-            return Detections(
-                xyxy=self.xyxy[index],
-                mask=self.mask[index] if self.mask is not None else None,
-                confidence=self.confidence[index]
-                if self.confidence is not None
-                else None,
-                class_id=self.class_id[index] if self.class_id is not None else None,
-                tracker_id=self.tracker_id[index]
-                if self.tracker_id is not None
-                else None,
-            )
-        raise TypeError(
-            f"Detections.__getitem__ not supported for index of type {type(index)}."
+    def __getitem__(
+        self, index: Union[int, slice, List[int], np.ndarray]
+    ) -> Detections:
+        """
+        Get a subset of the Detections object.
+
+        Args:
+            index (Union[int, slice, List[int], np.ndarray]): The index or indices of the subset of the Detections
+
+        Returns:
+            (Detections): A subset of the Detections object.
+
+        Example:
+            ```python
+            >>> import supervision as sv
+
+            >>> detections = sv.Detections(...)
+
+            >>> first_detection = detections[0]
+
+            >>> first_10_detections = detections[0:10]
+
+            >>> some_detections = detections[[0, 2, 4]]
+
+            >>> class_0_detections = detections[detections.class_id == 0]
+
+            >>> high_confidence_detections = detections[detections.confidence > 0.5]
+            ```
+        """
+        if isinstance(index, int):
+            index = [index]
+        return Detections(
+            xyxy=self.xyxy[index],
+            mask=self.mask[index] if self.mask is not None else None,
+            confidence=self.confidence[index] if self.confidence is not None else None,
+            class_id=self.class_id[index] if self.class_id is not None else None,
+            tracker_id=self.tracker_id[index] if self.tracker_id is not None else None,
         )
 
     @property
     def area(self) -> np.ndarray:
         """
         Calculate the area of each detection in the set of object detections. If masks field is defined property
         returns are of each mask. If only box is given property return area of each box.
```

### Comparing `supervision-0.8.0/supervision/detection/line_counter.py` & `supervision-0.9.0/supervision/detection/line_counter.py`

 * *Files identical despite different names*

### Comparing `supervision-0.8.0/supervision/detection/tools/polygon_zone.py` & `supervision-0.9.0/supervision/detection/tools/polygon_zone.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 
 
 class PolygonZone:
     """
     A class for defining a polygon-shaped zone within a frame for detecting objects.
 
     Attributes:
-        polygon (np.ndarray): A numpy array defining the polygon vertices
+        polygon (np.ndarray): A polygon represented by a numpy array of shape `(N, 2)`, containing the `x`, `y` coordinates of the points.
         frame_resolution_wh (Tuple[int, int]): The frame resolution (width, height)
         triggering_position (Position): The position within the bounding box that triggers the zone (default: Position.BOTTOM_CENTER)
         current_count (int): The current count of detected objects within the zone
         mask (np.ndarray): The 2D bool mask for the polygon zone
     """
 
     def __init__(
         self,
         polygon: np.ndarray,
         frame_resolution_wh: Tuple[int, int],
         triggering_position: Position = Position.BOTTOM_CENTER,
     ):
-        self.polygon = polygon
+        self.polygon = polygon.astype(int)
         self.frame_resolution_wh = frame_resolution_wh
         self.triggering_position = triggering_position
         self.current_count = 0
 
         width, height = frame_resolution_wh
         self.mask = polygon_to_mask(
             polygon=polygon, resolution_wh=(width + 1, height + 1)
```

### Comparing `supervision-0.8.0/supervision/detection/utils.py` & `supervision-0.9.0/supervision/detection/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -254,7 +254,41 @@
         new_approximated_points = cv2.approxPolyDP(polygon, epsilon, closed=True)
         if len(new_approximated_points) > target_points:
             approximated_points = new_approximated_points
         else:
             break
 
     return np.squeeze(approximated_points, axis=1)
+
+
+def extract_yolov8_masks(yolov8_results) -> Optional[np.ndarray]:
+    if not yolov8_results.masks:
+        return None
+
+    orig_shape = yolov8_results.orig_shape
+    inference_shape = tuple(yolov8_results.masks.data.shape[1:])
+
+    gain = 0
+    pad = (0, 0)
+
+    if inference_shape != orig_shape:
+        gain = min(
+            inference_shape[0] / orig_shape[0],
+            inference_shape[1] / orig_shape[1],
+        )
+        pad = (
+            (inference_shape[1] - orig_shape[1] * gain) / 2,
+            (inference_shape[0] - orig_shape[0] * gain) / 2,
+        )
+
+    top, left = int(pad[1]), int(pad[0])
+    bottom, right = int(inference_shape[0] - pad[1]), int(inference_shape[1] - pad[0])
+
+    mask_maps = []
+    masks = yolov8_results.masks.data.cpu().numpy()
+    for i in range(masks.shape[0]):
+        mask = masks[i]
+        mask = mask[top:bottom, left:right]
+        mask = cv2.resize(mask, (orig_shape[1], orig_shape[0]))
+        mask_maps.append(mask)
+
+    return np.asarray(mask_maps, dtype=bool)
```

### Comparing `supervision-0.8.0/supervision/draw/color.py` & `supervision-0.9.0/supervision/draw/color.py`

 * *Files identical despite different names*

### Comparing `supervision-0.8.0/supervision/draw/utils.py` & `supervision-0.9.0/supervision/draw/utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.8.0/supervision/file.py` & `supervision-0.9.0/supervision/utils/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
         extensions (Optional[List[str]]): A list of file extensions to filter. Default is None, which lists all files.
 
     Returns:
         (List[Path]): A list of Path objects for the matching files.
 
     Examples:
         ```python
-        >>> from supervision import list_files_with_extensions
+        >>> import supervision as sv
 
         >>> # List all files in the directory
-        >>> files = list_files_with_extensions(directory='my_directory')
+        >>> files = sv.list_files_with_extensions(directory='my_directory')
 
         >>> # List only files with '.txt' and '.md' extensions
-        >>> files = list_files_with_extensions(directory='my_directory', extensions=['txt', 'md'])
+        >>> files = sv.list_files_with_extensions(directory='my_directory', extensions=['txt', 'md'])
         ```
     """
     directory = Path(directory)
     files_with_extensions = []
 
     if extensions is not None:
         for ext in extensions:
```

### Comparing `supervision-0.8.0/supervision/geometry/core.py` & `supervision-0.9.0/supervision/geometry/core.py`

 * *Files identical despite different names*

### Comparing `supervision-0.8.0/supervision/geometry/utils.py` & `supervision-0.9.0/supervision/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.8.0/supervision/notebook/utils.py` & `supervision-0.9.0/supervision/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `supervision-0.8.0/supervision/video.py` & `supervision-0.9.0/supervision/utils/video.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,17 +16,17 @@
         width (int): width of the video in pixels
         height (int): height of the video in pixels
         fps (int): frames per second of the video
         total_frames (int, optional): total number of frames in the video, default is None
 
     Examples:
         ```python
-        >>> from supervision import VideoInfo
+        >>> import supervision as sv
 
-        >>> video_info = VideoInfo.from_video_path(video_path='video.mp4')
+        >>> video_info = sv.VideoInfo.from_video_path(video_path='video.mp4')
 
         >>> video_info
         VideoInfo(width=3840, height=2160, fps=25, total_frames=538)
 
         >>> video_info.resolution_wh
         (3840, 2160)
         ```
@@ -59,23 +59,23 @@
     """
     Context manager that saves video frames to a file using OpenCV.
 
     Attributes:
         target_path (str): The path to the output file where the video will be saved.
         video_info (VideoInfo): Information about the video resolution, fps, and total frame count.
 
-    Examples:
+    Example:
         ```python
-        >>> from supervision import VideoInfo, VideoSink
+        >>> import supervision as sv
 
-        >>> video_info = VideoInfo.from_video_path(video_path='source_video.mp4')
+        >>> video_info = sv.VideoInfo.from_video_path(video_path='source_video.mp4')
 
-        >>> with VideoSink(target_path='target_video.mp4', video_info=video_info) as s:
-        ...     frame = ...
-        ...     s.write_frame(frame=frame)
+        >>> with sv.VideoSink(target_path='target_video.mp4', video_info=video_info) as sink:
+        ...     for frame in get_video_frames_generator(source_path='source_video.mp4', stride=2):
+        ...         sink.write_frame(frame=frame)
         ```
     """
 
     def __init__(self, target_path: str, video_info: VideoInfo):
         self.target_path = target_path
         self.video_info = video_info
         self.__fourcc = cv2.VideoWriter_fourcc(*"mp4v")
@@ -89,43 +89,51 @@
             self.video_info.resolution_wh,
         )
         return self
 
     def write_frame(self, frame: np.ndarray):
         self.__writer.write(frame)
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
+    def __exit__(self, exc_type, exc_value, exc_traceback):
         self.__writer.release()
 
 
-def get_video_frames_generator(source_path: str) -> Generator[np.ndarray, None, None]:
+def get_video_frames_generator(
+    source_path: str, stride: int = 1
+) -> Generator[np.ndarray, None, None]:
     """
     Get a generator that yields the frames of the video.
 
     Args:
         source_path (str): The path of the video file.
+        stride (int): The number of frames to skip before returning the next one.
 
     Returns:
         (Generator[np.ndarray, None, None]): A generator that yields the frames of the video.
 
     Examples:
         ```python
-        >>> from supervision import get_video_frames_generator
+        >>> import supervision as sv
 
-        >>> for frame in get_video_frames_generator(source_path='source_video.mp4'):
+        >>> for frame in sv.get_video_frames_generator(source_path='source_video.mp4', stride=2):
         ...     ...
         ```
     """
     video = cv2.VideoCapture(source_path)
     if not video.isOpened():
         raise Exception(f"Could not open video at {source_path}")
+
+    frame_count = 0
     success, frame = video.read()
     while success:
-        yield frame
+        if frame_count % stride == 0:
+            yield frame
         success, frame = video.read()
+        frame_count += 1
+
     video.release()
 
 
 def process_video(
     source_path: str,
     target_path: str,
     callback: Callable[[np.ndarray, int], np.ndarray],
```

### Comparing `supervision-0.8.0/supervision.egg-info/SOURCES.txt` & `supervision-0.9.0/supervision.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 LICENSE.md
 README.md
 setup.py
 supervision/__init__.py
-supervision/file.py
-supervision/internal.py
-supervision/video.py
 supervision.egg-info/PKG-INFO
 supervision.egg-info/SOURCES.txt
 supervision.egg-info/dependency_links.txt
 supervision.egg-info/requires.txt
 supervision.egg-info/top_level.txt
 supervision/dataset/__init__.py
 supervision/dataset/core.py
@@ -25,16 +22,20 @@
 supervision/detection/tools/polygon_zone.py
 supervision/draw/__init__.py
 supervision/draw/color.py
 supervision/draw/utils.py
 supervision/geometry/__init__.py
 supervision/geometry/core.py
 supervision/geometry/utils.py
-supervision/notebook/__init__.py
-supervision/notebook/utils.py
+supervision/utils/__init__.py
+supervision/utils/file.py
+supervision/utils/image.py
+supervision/utils/internal.py
+supervision/utils/notebook.py
+supervision/utils/video.py
 test/__init__.py
 test/dataset/__init__.py
 test/dataset/test_utils.py
 test/dataset/formats/__init__.py
 test/dataset/formats/test_yolo.py
 test/detection/__init__.py
 test/detection/test_core.py
```

### Comparing `supervision-0.8.0/test/dataset/formats/test_yolo.py` & `supervision-0.9.0/test/dataset/formats/test_yolo.py`

 * *Files identical despite different names*

### Comparing `supervision-0.8.0/test/dataset/test_utils.py` & `supervision-0.9.0/test/dataset/test_utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.8.0/test/detection/test_utils.py` & `supervision-0.9.0/test/detection/test_utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.8.0/test/draw/test_color.py` & `supervision-0.9.0/test/draw/test_color.py`

 * *Files identical despite different names*

### Comparing `supervision-0.8.0/test/geometry/test_dataclasses.py` & `supervision-0.9.0/test/geometry/test_dataclasses.py`

 * *Files identical despite different names*

