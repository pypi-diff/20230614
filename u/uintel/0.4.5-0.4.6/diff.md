# Comparing `tmp/uintel-0.4.5.tar.gz` & `tmp/uintel-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uintel-0.4.5.tar", last modified: Fri Jun  9 03:24:31 2023, max compression
+gzip compressed data, was "uintel-0.4.6.tar", last modified: Tue Jun 13 22:05:57 2023, max compression
```

## Comparing `uintel-0.4.5.tar` & `uintel-0.4.6.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-09 03:24:31.284448 uintel-0.4.5/
--rw-rw-r--   0 sam       (1000) sam       (1000)     1075 2023-04-03 04:47:18.000000 uintel-0.4.5/LICENSE
--rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-06-09 03:24:31.284448 uintel-0.4.5/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)     3274 2023-04-03 04:47:18.000000 uintel-0.4.5/README.md
--rw-rw-r--   0 sam       (1000) sam       (1000)       95 2023-04-03 04:47:18.000000 uintel-0.4.5/pyproject.toml
--rw-rw-r--   0 sam       (1000) sam       (1000)       38 2023-06-09 03:24:31.284448 uintel-0.4.5/setup.cfg
--rw-rw-r--   0 sam       (1000) sam       (1000)     1560 2023-06-09 03:24:20.000000 uintel-0.4.5/setup.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-09 03:24:31.276449 uintel-0.4.5/src/
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-09 03:24:31.280449 uintel-0.4.5/src/uintel/
--rw-rw-r--   0 sam       (1000) sam       (1000)     3030 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     7978 2023-05-05 02:33:43.000000 uintel-0.4.5/src/uintel/aws.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     4657 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/colours.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    10626 2023-05-05 02:33:43.000000 uintel-0.4.5/src/uintel/esri.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-09 03:24:31.284448 uintel-0.4.5/src/uintel/fonts/
--rw-rw-r--   0 sam       (1000) sam       (1000)    94884 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/fonts/Myriad Pro (TrueType).ttf
--rw-rw-r--   0 sam       (1000) sam       (1000)   208636 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/fonts/Rubik (TrueType).ttf
--rw-rw-r--   0 sam       (1000) sam       (1000)   202424 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/fonts/Rubik Italic (TrueType).ttf
--rw-rw-r--   0 sam       (1000) sam       (1000)    20754 2023-06-07 04:00:00.000000 uintel-0.4.5/src/uintel/geometry.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    23184 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/install.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2308 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/ogc.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     3808 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/query.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     7934 2023-05-05 02:33:43.000000 uintel-0.4.5/src/uintel/server.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    13281 2023-05-05 02:33:43.000000 uintel-0.4.5/src/uintel/slack.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     6388 2023-06-09 03:24:12.000000 uintel-0.4.5/src/uintel/sql.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-09 03:24:31.284448 uintel-0.4.5/src/uintel/styles/
--rw-rw-r--   0 sam       (1000) sam       (1000)     1046 2023-04-03 04:47:18.000000 uintel-0.4.5/src/uintel/styles/ui.mplstyle
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-09 03:24:31.284448 uintel-0.4.5/src/uintel.egg-info/
--rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-06-09 03:24:31.000000 uintel-0.4.5/src/uintel.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)      590 2023-06-09 03:24:31.000000 uintel-0.4.5/src/uintel.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-06-09 03:24:31.000000 uintel-0.4.5/src/uintel.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)      158 2023-06-09 03:24:31.000000 uintel-0.4.5/src/uintel.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        7 2023-06-09 03:24:31.000000 uintel-0.4.5/src/uintel.egg-info/top_level.txt
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-13 22:05:57.741646 uintel-0.4.6/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1075 2023-04-03 04:47:18.000000 uintel-0.4.6/LICENSE
+-rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-06-13 22:05:57.741646 uintel-0.4.6/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3274 2023-04-03 04:47:18.000000 uintel-0.4.6/README.md
+-rw-rw-r--   0 sam       (1000) sam       (1000)       95 2023-04-03 04:47:18.000000 uintel-0.4.6/pyproject.toml
+-rw-rw-r--   0 sam       (1000) sam       (1000)       38 2023-06-13 22:05:57.741646 uintel-0.4.6/setup.cfg
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1560 2023-06-13 22:05:41.000000 uintel-0.4.6/setup.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-13 22:05:57.737646 uintel-0.4.6/src/
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-13 22:05:57.741646 uintel-0.4.6/src/uintel/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3048 2023-06-13 21:48:29.000000 uintel-0.4.6/src/uintel/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     7978 2023-05-05 02:33:43.000000 uintel-0.4.6/src/uintel/aws.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     4657 2023-04-03 04:47:18.000000 uintel-0.4.6/src/uintel/colours.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    10626 2023-05-05 02:33:43.000000 uintel-0.4.6/src/uintel/esri.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-13 22:05:57.741646 uintel-0.4.6/src/uintel/fonts/
+-rw-rw-r--   0 sam       (1000) sam       (1000)    94884 2023-04-03 04:47:18.000000 uintel-0.4.6/src/uintel/fonts/Myriad Pro (TrueType).ttf
+-rw-rw-r--   0 sam       (1000) sam       (1000)   208636 2023-04-03 04:47:18.000000 uintel-0.4.6/src/uintel/fonts/Rubik (TrueType).ttf
+-rw-rw-r--   0 sam       (1000) sam       (1000)   202424 2023-04-03 04:47:18.000000 uintel-0.4.6/src/uintel/fonts/Rubik Italic (TrueType).ttf
+-rw-rw-r--   0 sam       (1000) sam       (1000)    20754 2023-06-13 21:23:30.000000 uintel-0.4.6/src/uintel/geometry.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    23184 2023-04-03 04:47:18.000000 uintel-0.4.6/src/uintel/install.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     2308 2023-04-03 04:47:18.000000 uintel-0.4.6/src/uintel/ogc.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3808 2023-04-03 04:47:18.000000 uintel-0.4.6/src/uintel/query.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     9561 2023-06-13 22:02:00.000000 uintel-0.4.6/src/uintel/raster.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     7934 2023-05-05 02:33:43.000000 uintel-0.4.6/src/uintel/server.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    13281 2023-05-05 02:33:43.000000 uintel-0.4.6/src/uintel/slack.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     6388 2023-06-09 03:24:12.000000 uintel-0.4.6/src/uintel/sql.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-13 22:05:57.741646 uintel-0.4.6/src/uintel/styles/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1046 2023-04-03 04:47:18.000000 uintel-0.4.6/src/uintel/styles/ui.mplstyle
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-13 22:05:57.741646 uintel-0.4.6/src/uintel.egg-info/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-06-13 22:05:57.000000 uintel-0.4.6/src/uintel.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)      611 2023-06-13 22:05:57.000000 uintel-0.4.6/src/uintel.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-06-13 22:05:57.000000 uintel-0.4.6/src/uintel.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)      158 2023-06-13 22:05:57.000000 uintel-0.4.6/src/uintel.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        7 2023-06-13 22:05:57.000000 uintel-0.4.6/src/uintel.egg-info/top_level.txt
```

### Comparing `uintel-0.4.5/LICENSE` & `uintel-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `uintel-0.4.5/PKG-INFO` & `uintel-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uintel
-Version: 0.4.5
+Version: 0.4.6
 Summary: Urban Intelligence's unified Python data analysis toolkit
 Home-page: https://uintel.github.io/pyui/
 Author: Sam Archie
 Author-email: sam.archie@urbanintelligence.co.nz
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `uintel-0.4.5/README.md` & `uintel-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `uintel-0.4.5/setup.py` & `uintel-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 setuptools.setup(
     # State the generic information about the package
     name='uintel',
-    version='0.4.5',
+    version='0.4.6',
     author="Sam Archie",
     author_email="sam.archie@urbanintelligence.co.nz",
     description="Urban Intelligence's unified Python data analysis toolkit",
     long_description=open('README.md').read().replace("docs/images/blue_logo.svg", "https://urbanintelligence.co.nz/wp-content/uploads/2022/05/Artboard-1-copy-23.svg"),
     long_description_content_type='text/markdown',
     license="MIT",
     url="https://uintel.github.io/pyui/",
```

### Comparing `uintel-0.4.5/src/uintel/__init__.py` & `uintel-0.4.6/src/uintel/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,9 +85,9 @@
     _install._save_config(config)
 
 
 _install._update_config_file()
 _install._install_styles(force=False, verbose=True)
 _install._install_fonts(force=False, verbose=True)
 
-from . import aws, colours, esri, geometry, server, slack, sql, ogc
-__all__ = ["aws", "colours","esri", "geometry", "server", "slack", "sql", "ogc"]
+from . import aws, colours, esri, geometry, raster, server, slack, sql, ogc
+__all__ = ["aws", "colours","esri", "geometry", "raster", "server", "slack", "sql", "ogc"]
```

### Comparing `uintel-0.4.5/src/uintel/aws.py` & `uintel-0.4.6/src/uintel/aws.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.5/src/uintel/colours.py` & `uintel-0.4.6/src/uintel/colours.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.5/src/uintel/esri.py` & `uintel-0.4.6/src/uintel/esri.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.5/src/uintel/fonts/Myriad Pro (TrueType).ttf` & `uintel-0.4.6/src/uintel/fonts/Myriad Pro (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.4.5/src/uintel/fonts/Rubik (TrueType).ttf` & `uintel-0.4.6/src/uintel/fonts/Rubik (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.4.5/src/uintel/fonts/Rubik Italic (TrueType).ttf` & `uintel-0.4.6/src/uintel/fonts/Rubik Italic (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.4.5/src/uintel/geometry.py` & `uintel-0.4.6/src/uintel/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
     try:
         import osgeo.ogr, osgeo.osr, osgeo.gdal
     except ModuleNotFoundError:
         raise ModuleNotFoundError("GDAL could not be located. Please install GDAL seperately into this Python environment, or run 'pip install uintel[full]'")
     try:
         import rasterio as rio
     except ModuleNotFoundError:
-        raise ModuleNotFoundError("RasterIO could not be located. Please install rasterio seperately into this Python environment, or run 'pip install uintel[full]'")
+        raise ModuleNotFoundError("RasterIO could not be located. Please install RasterIO seperately into this Python environment, or run 'pip install uintel[full]'")
 
     epsg = _check_inputted_datasets(raster_path, vector_path)
 
     # Get GDAL driver
     mem_driver = osgeo.ogr.GetDriverByName("Memory")
     mem_driver_gdal = osgeo.gdal.GetDriverByName("MEM")
```

### Comparing `uintel-0.4.5/src/uintel/install.py` & `uintel-0.4.6/src/uintel/install.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.5/src/uintel/ogc.py` & `uintel-0.4.6/src/uintel/ogc.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.5/src/uintel/query.py` & `uintel-0.4.6/src/uintel/query.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.5/src/uintel/server.py` & `uintel-0.4.6/src/uintel/server.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.5/src/uintel/slack.py` & `uintel-0.4.6/src/uintel/slack.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.5/src/uintel/sql.py` & `uintel-0.4.6/src/uintel/sql.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.5/src/uintel/styles/ui.mplstyle` & `uintel-0.4.6/src/uintel/styles/ui.mplstyle`

 * *Files identical despite different names*

### Comparing `uintel-0.4.5/src/uintel.egg-info/PKG-INFO` & `uintel-0.4.6/src/uintel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uintel
-Version: 0.4.5
+Version: 0.4.6
 Summary: Urban Intelligence's unified Python data analysis toolkit
 Home-page: https://uintel.github.io/pyui/
 Author: Sam Archie
 Author-email: sam.archie@urbanintelligence.co.nz
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `uintel-0.4.5/src/uintel.egg-info/SOURCES.txt` & `uintel-0.4.6/src/uintel.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/uintel/aws.py
 src/uintel/colours.py
 src/uintel/esri.py
 src/uintel/geometry.py
 src/uintel/install.py
 src/uintel/ogc.py
 src/uintel/query.py
+src/uintel/raster.py
 src/uintel/server.py
 src/uintel/slack.py
 src/uintel/sql.py
 src/uintel.egg-info/PKG-INFO
 src/uintel.egg-info/SOURCES.txt
 src/uintel.egg-info/dependency_links.txt
 src/uintel.egg-info/requires.txt
```

