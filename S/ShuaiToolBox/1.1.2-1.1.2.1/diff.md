# Comparing `tmp/ShuaiToolBox-1.1.2.tar.gz` & `tmp/ShuaiToolBox-1.1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ShuaiToolBox-1.1.2.tar", last modified: Wed Jun 14 01:59:53 2023, max compression
+gzip compressed data, was "dist\ShuaiToolBox-1.1.2.1.tar", last modified: Wed Jun 14 02:20:28 2023, max compression
```

## Comparing `ShuaiToolBox-1.1.2.tar` & `ShuaiToolBox-1.1.2.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/
--rw-rw-rw-   0        0        0      199 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-13 06:20:27.000000 ShuaiToolBox-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/
--rw-rw-rw-   0        0        0    12679 2023-06-13 09:51:02.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/EORmodule.py
--rw-rw-rw-   0        0        0     2526 2023-06-13 08:11:37.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/FindContours.py
--rw-rw-rw-   0        0        0    13782 2023-06-13 08:11:14.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/VideoPro.py
--rw-rw-rw-   0        0        0     8658 2023-06-14 01:55:09.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/VideoProList.py
--rw-rw-rw-   0        0        0      187 2023-06-13 09:22:13.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/__init__.py
--rw-rw-rw-   0        0        0     1026 2023-06-13 08:21:34.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/cv_plugin.py
--rw-rw-rw-   0        0        0     2119 2023-06-13 08:06:47.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/cv_vdopro.py
--rw-rw-rw-   0        0        0     8687 2023-06-14 01:59:16.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/opencv_Functions.py
--rw-rw-rw-   0        0        0     1635 2023-06-13 07:56:00.000000 ShuaiToolBox-1.1.2/ShuaiToolBox/py_plugin.py
-drwxrwxrwx   0        0        0        0 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/ShuaiToolBox.egg-info/
--rw-rw-rw-   0        0        0      199 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/ShuaiToolBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/ShuaiToolBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/ShuaiToolBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/ShuaiToolBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 01:59:53.000000 ShuaiToolBox-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      240 2023-06-13 07:56:32.000000 ShuaiToolBox-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:20:28.000000 ShuaiToolBox-1.1.2.1/
+-rw-rw-rw-   0        0        0      223 2023-06-14 02:20:28.000000 ShuaiToolBox-1.1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-13 06:20:27.000000 ShuaiToolBox-1.1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 02:20:28.000000 ShuaiToolBox-1.1.2.1/ShuaiToolBox/
+-rw-rw-rw-   0        0        0    12679 2023-06-13 09:51:02.000000 ShuaiToolBox-1.1.2.1/ShuaiToolBox/EORmodule.py
+-rw-rw-rw-   0        0        0     2526 2023-06-13 08:11:37.000000 ShuaiToolBox-1.1.2.1/ShuaiToolBox/FindContours.py
+-rw-rw-rw-   0        0        0    13782 2023-06-13 08:11:14.000000 ShuaiToolBox-1.1.2.1/ShuaiToolBox/VideoPro.py
+-rw-rw-rw-   0        0        0     8658 2023-06-14 01:55:09.000000 ShuaiToolBox-1.1.2.1/ShuaiToolBox/VideoProList.py
+-rw-rw-rw-   0        0        0      187 2023-06-13 09:22:13.000000 ShuaiToolBox-1.1.2.1/ShuaiToolBox/__init__.py
+-rw-rw-rw-   0        0        0     1026 2023-06-13 08:21:34.000000 ShuaiToolBox-1.1.2.1/ShuaiToolBox/cv_plugin.py
+-rw-rw-rw-   0        0        0     2119 2023-06-13 08:06:47.000000 ShuaiToolBox-1.1.2.1/ShuaiToolBox/cv_vdopro.py
+-rw-rw-rw-   0        0        0     8687 2023-06-14 01:59:16.000000 ShuaiToolBox-1.1.2.1/ShuaiToolBox/opencv_Functions.py
+-rw-rw-rw-   0        0        0     1635 2023-06-13 07:56:00.000000 ShuaiToolBox-1.1.2.1/ShuaiToolBox/py_plugin.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:20:28.000000 ShuaiToolBox-1.1.2.1/ShuaiToolBox.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-06-14 02:20:28.000000 ShuaiToolBox-1.1.2.1/ShuaiToolBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-06-14 02:20:28.000000 ShuaiToolBox-1.1.2.1/ShuaiToolBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 02:20:28.000000 ShuaiToolBox-1.1.2.1/ShuaiToolBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-14 02:20:28.000000 ShuaiToolBox-1.1.2.1/ShuaiToolBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:20:28.000000 ShuaiToolBox-1.1.2.1/ShuaiToolBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 02:20:28.000000 ShuaiToolBox-1.1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      413 2023-06-14 02:20:12.000000 ShuaiToolBox-1.1.2.1/setup.py
```

### Comparing `ShuaiToolBox-1.1.2/ShuaiToolBox/EORmodule.py` & `ShuaiToolBox-1.1.2.1/ShuaiToolBox/EORmodule.py`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2/ShuaiToolBox/FindContours.py` & `ShuaiToolBox-1.1.2.1/ShuaiToolBox/FindContours.py`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2/ShuaiToolBox/VideoPro.py` & `ShuaiToolBox-1.1.2.1/ShuaiToolBox/VideoPro.py`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2/ShuaiToolBox/VideoProList.py` & `ShuaiToolBox-1.1.2.1/ShuaiToolBox/VideoProList.py`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2/ShuaiToolBox/cv_plugin.py` & `ShuaiToolBox-1.1.2.1/ShuaiToolBox/cv_plugin.py`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2/ShuaiToolBox/cv_vdopro.py` & `ShuaiToolBox-1.1.2.1/ShuaiToolBox/cv_vdopro.py`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2/ShuaiToolBox/opencv_Functions.py` & `ShuaiToolBox-1.1.2.1/ShuaiToolBox/opencv_Functions.py`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.1.2/ShuaiToolBox/py_plugin.py` & `ShuaiToolBox-1.1.2.1/ShuaiToolBox/py_plugin.py`

 * *Files identical despite different names*

