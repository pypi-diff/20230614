# Comparing `tmp/st_line_plotter-0.0.1.tar.gz` & `tmp/st_line_plotter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_line_plotter-0.0.1.tar", last modified: Tue Jun 13 16:07:49 2023, max compression
+gzip compressed data, was "st_line_plotter-0.0.2.tar", last modified: Wed Jun 14 07:39:19 2023, max compression
```

## Comparing `st_line_plotter-0.0.1.tar` & `st_line_plotter-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,31 @@
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-13 16:07:49.271979 st_line_plotter-0.0.1/
--rw-r--r--   0 elliotglas   (501) staff       (20)     2340 2023-06-08 13:50:21.000000 st_line_plotter-0.0.1/LICENSE
--rw-r--r--   0 elliotglas   (501) staff       (20)       43 2023-06-08 13:50:21.000000 st_line_plotter-0.0.1/MANIFEST.in
--rw-r--r--   0 elliotglas   (501) staff       (20)      298 2023-06-13 16:07:49.271807 st_line_plotter-0.0.1/PKG-INFO
--rw-r--r--   0 elliotglas   (501) staff       (20)       38 2023-06-13 16:07:49.272036 st_line_plotter-0.0.1/setup.cfg
--rw-r--r--   0 elliotglas   (501) staff       (20)      671 2023-06-13 16:07:23.000000 st_line_plotter-0.0.1/setup.py
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-13 16:07:49.270743 st_line_plotter-0.0.1/st_line_plotter/
--rw-r--r--   0 elliotglas   (501) staff       (20)     2070 2023-06-13 16:02:18.000000 st_line_plotter-0.0.1/st_line_plotter/__init__.py
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-13 16:07:49.271575 st_line_plotter-0.0.1/st_line_plotter.egg-info/
--rw-r--r--   0 elliotglas   (501) staff       (20)      298 2023-06-13 16:07:49.000000 st_line_plotter-0.0.1/st_line_plotter.egg-info/PKG-INFO
--rw-r--r--   0 elliotglas   (501) staff       (20)      250 2023-06-13 16:07:49.000000 st_line_plotter-0.0.1/st_line_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)        1 2023-06-13 16:07:49.000000 st_line_plotter-0.0.1/st_line_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-06-13 16:07:49.000000 st_line_plotter-0.0.1/st_line_plotter.egg-info/requires.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-06-13 16:07:49.000000 st_line_plotter-0.0.1/st_line_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-14 07:39:19.274049 st_line_plotter-0.0.2/
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2340 2023-06-08 13:50:21.000000 st_line_plotter-0.0.2/LICENSE
+-rw-r--r--   0 elliotglas   (501) staff       (20)       51 2023-06-14 07:33:03.000000 st_line_plotter-0.0.2/MANIFEST.in
+-rw-r--r--   0 elliotglas   (501) staff       (20)      298 2023-06-14 07:39:19.273869 st_line_plotter-0.0.2/PKG-INFO
+-rw-r--r--   0 elliotglas   (501) staff       (20)       38 2023-06-14 07:39:19.274115 st_line_plotter-0.0.2/setup.cfg
+-rw-r--r--   0 elliotglas   (501) staff       (20)      671 2023-06-14 07:33:40.000000 st_line_plotter-0.0.2/setup.py
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-14 07:39:19.266085 st_line_plotter-0.0.2/st_line_plotter/
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2070 2023-06-13 16:02:18.000000 st_line_plotter-0.0.2/st_line_plotter/__init__.py
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-14 07:39:19.264699 st_line_plotter-0.0.2/st_line_plotter/frontend/
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-14 07:39:19.268352 st_line_plotter-0.0.2/st_line_plotter/frontend/build/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      928 2023-06-13 13:38:23.000000 st_line_plotter-0.0.2/st_line_plotter/frontend/build/asset-manifest.json
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2119 2023-06-13 13:38:23.000000 st_line_plotter-0.0.2/st_line_plotter/frontend/build/index.html
+-rw-r--r--   0 elliotglas   (501) staff       (20)      673 2023-06-13 13:38:23.000000 st_line_plotter-0.0.2/st_line_plotter/frontend/build/precache-manifest.2789ed6399de93230535e104691ce67f.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)     1183 2023-06-13 13:38:23.000000 st_line_plotter-0.0.2/st_line_plotter/frontend/build/service-worker.js
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-14 07:39:19.265162 st_line_plotter-0.0.2/st_line_plotter/frontend/build/static/
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-14 07:39:19.273125 st_line_plotter-0.0.2/st_line_plotter/frontend/build/static/js/
+-rw-r--r--   0 elliotglas   (501) staff       (20)   459440 2023-06-13 13:38:23.000000 st_line_plotter-0.0.2/st_line_plotter/frontend/build/static/js/2.51f30e44.chunk.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)     1909 2023-06-13 13:38:23.000000 st_line_plotter-0.0.2/st_line_plotter/frontend/build/static/js/2.51f30e44.chunk.js.LICENSE.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)  1700606 2023-06-13 13:38:23.000000 st_line_plotter-0.0.2/st_line_plotter/frontend/build/static/js/2.51f30e44.chunk.js.map
+-rw-r--r--   0 elliotglas   (501) staff       (20)     7864 2023-06-13 13:38:23.000000 st_line_plotter-0.0.2/st_line_plotter/frontend/build/static/js/main.e8acecfa.chunk.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)    26390 2023-06-13 13:38:23.000000 st_line_plotter-0.0.2/st_line_plotter/frontend/build/static/js/main.e8acecfa.chunk.js.map
+-rw-r--r--   0 elliotglas   (501) staff       (20)     1598 2023-06-13 13:38:23.000000 st_line_plotter-0.0.2/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)     8317 2023-06-13 13:38:23.000000 st_line_plotter-0.0.2/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js.map
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-14 07:39:19.273394 st_line_plotter-0.0.2/st_line_plotter/frontend/build/static/media/
+-rw-r--r--   0 elliotglas   (501) staff       (20)   149674 2023-06-13 13:38:23.000000 st_line_plotter-0.0.2/st_line_plotter/frontend/build/static/media/ground.0d5856bc.png
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-14 07:39:19.267185 st_line_plotter-0.0.2/st_line_plotter.egg-info/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      298 2023-06-14 07:39:19.000000 st_line_plotter-0.0.2/st_line_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 elliotglas   (501) staff       (20)     1008 2023-06-14 07:39:19.000000 st_line_plotter-0.0.2/st_line_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)        1 2023-06-14 07:39:19.000000 st_line_plotter-0.0.2/st_line_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-06-14 07:39:19.000000 st_line_plotter-0.0.2/st_line_plotter.egg-info/requires.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-06-14 07:39:19.000000 st_line_plotter-0.0.2/st_line_plotter.egg-info/top_level.txt
```

### Comparing `st_line_plotter-0.0.1/LICENSE` & `st_line_plotter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.1/setup.py` & `st_line_plotter-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_line_plotter",
-    version="0.0.1",
+    version="0.0.2",
     author="Elliot Glas",
     author_email="elliot.glas@hotmail.se",
     description="A tool to place lines on an image and get back the coordinates for those lines",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_line_plotter-0.0.1/st_line_plotter/__init__.py` & `st_line_plotter-0.0.2/st_line_plotter/__init__.py`

 * *Files identical despite different names*

