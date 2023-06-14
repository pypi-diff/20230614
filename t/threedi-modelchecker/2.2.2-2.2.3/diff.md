# Comparing `tmp/threedi-modelchecker-2.2.2.tar.gz` & `tmp/threedi-modelchecker-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi-modelchecker-2.2.2.tar", last modified: Wed May 17 09:27:55 2023, max compression
+gzip compressed data, was "threedi-modelchecker-2.2.3.tar", last modified: Wed Jun 14 09:05:35 2023, max compression
```

## Comparing `threedi-modelchecker-2.2.2.tar` & `threedi-modelchecker-2.2.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:55.778960 threedi-modelchecker-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    20124 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-17 09:27:55.778960 threedi-modelchecker-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-17 09:27:55.778960 threedi-modelchecker-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:55.770960 threedi-modelchecker-2.2.2/threedi_modelchecker/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:55.774960 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/cross_section_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/geo_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    32998 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/other.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    94471 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/exporters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:55.774960 threedi-modelchecker-2.2.2/threedi_modelchecker/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/interfaces/raster_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/interfaces/raster_interface_gdal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/interfaces/raster_interface_rasterio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/model_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:55.778960 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:55.778960 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/data/empty_v4.sqlite
--rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    27178 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15823 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_cross_section_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    22881 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_other.py
--rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_model_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:55.770960 threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-17 09:27:55.000000 threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-17 09:27:55.000000 threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:27:55.000000 threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 09:27:55.000000 threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:27:55.000000 threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-17 09:27:55.000000 threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 09:27:55.000000 threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:35.454912 threedi-modelchecker-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    20385 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-14 09:05:35.454912 threedi-modelchecker-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-14 09:05:35.454912 threedi-modelchecker-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:35.442912 threedi-modelchecker-2.2.3/threedi_modelchecker/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:35.450912 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/cross_section_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/geo_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32998 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94957 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/exporters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:35.450912 threedi-modelchecker-2.2.3/threedi_modelchecker/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/interfaces/raster_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/interfaces/raster_interface_gdal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/interfaces/raster_interface_rasterio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/model_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:35.454912 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:35.454912 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/data/empty_v4.sqlite
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27178 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15823 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_cross_section_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22881 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_other.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14685 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_model_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:35.446912 threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-14 09:05:35.000000 threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-14 09:05:35.000000 threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:05:35.000000 threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 09:05:35.000000 threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:05:35.000000 threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-14 09:05:35.000000 threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 09:05:35.000000 threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/top_level.txt
```

### Comparing `threedi-modelchecker-2.2.2/CHANGES.rst` & `threedi-modelchecker-2.2.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Changelog of threedi-modelchecker
 =================================
 
 
+2.2.3 (2023-06-14)
+------------------
+
+- Ignore tiny floating-point deviations in RasterGridSizeCheck (check 798).
+
+- Add check 327 to make sure vegetation drag is only used if the friction type is Chezy.
+
+- Change log level of check 63 from ERROR to WARNING
+
+
 2.2.2 (2023-05-17)
 ------------------
 
 - Rewrite release workflow to use a supported github action for github release.
-- Build the release with the build package instead of setuptools.
 
+- Build the release with the build package instead of setuptools.
 
 
 2.2.1 (2023-05-16)
 ------------------
 
 - Fixed incorrect units in pumpstation check 66.
```

### Comparing `threedi-modelchecker-2.2.2/LICENSE` & `threedi-modelchecker-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/PKG-INFO` & `threedi-modelchecker-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-modelchecker
-Version: 2.2.2
+Version: 2.2.3
 Summary: Checks validity of a 3Di schematisation
 Home-page: https://github.com/nens/threedi-modelchecker
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `threedi-modelchecker-2.2.2/README.rst` & `threedi-modelchecker-2.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/setup.py` & `threedi-modelchecker-2.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/checks/base.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/checks/base.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/checks/cross_section_definitions.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/checks/cross_section_definitions.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/checks/factories.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/checks/factories.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/checks/geo_query.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/checks/geo_query.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/checks/other.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/checks/other.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/checks/raster.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/checks/raster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import dataclass
+from math import isclose
 from pathlib import Path
 from typing import Optional, Set, Type
 
 from threedi_schema import models
 
 from threedi_modelchecker.interfaces import GDALRasterInterface, RasterInterface
 
@@ -203,17 +204,19 @@
         return super().get_invalid(session)
 
     def is_valid(self, path: str, interface_cls: Type[RasterInterface]):
         with interface_cls(path) as raster:
             if not raster.is_valid_geotiff:
                 return True
             # the x pixel size is used here,but it is equal to the y pixel size
-            return ((self.grid_space / raster.pixel_size[0]) % 2 == 0) and (
-                self.grid_space >= (2 * raster.pixel_size[0])
-            )
+            return (
+                isclose(
+                    a=((self.grid_space / raster.pixel_size[0]) % 2), b=0, rel_tol=1e-09
+                )
+            ) and (self.grid_space >= (2 * raster.pixel_size[0]))
 
     def description(self):
         return "v2_global_settings.grid_space is not a positive even multiple of the raster cell size."
 
 
 class RasterRangeCheck(BaseRasterCheck):
     """Check whether a raster has values outside of provided range.
```

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/checks/timeseries.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/checks/timeseries.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/config.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,15 +358,15 @@
         invalid=Query(models.Pumpstation).filter(
             models.Pumpstation.lower_stop_level >= models.Pumpstation.start_level,
         ),
         message="v2_pumpstation.lower_stop_level should be less than v2_pumpstation.start_level",
     ),
     QueryCheck(
         error_code=63,
-        level=CheckLevel.ERROR,
+        level=CheckLevel.WARNING,
         column=models.ConnectionNode.storage_area,
         invalid=Query(models.ConnectionNode)
         .join(
             models.Pumpstation,
             models.Pumpstation.connection_node_end_id == models.ConnectionNode.id,
         )
         .filter(models.ConnectionNode.storage_area != None)
@@ -1254,14 +1254,27 @@
         (models.NumericalSettings, models.GlobalSetting.numerical_settings_id),
         (models.ControlGroup, models.GlobalSetting.control_group_id),
         (models.VegetationDrag, models.GlobalSetting.vegetation_drag_settings_id),
     )
 ]
 
 CHECKS += [
+    QueryCheck(
+        error_code=327,
+        column=models.GlobalSetting.vegetation_drag_settings_id,
+        invalid=Query(models.GlobalSetting).filter(
+            first_setting_filter,
+            ~is_none_or_empty(models.GlobalSetting.vegetation_drag_settings_id),
+            models.GlobalSetting.frict_type != constants.FrictionType.CHEZY.value,
+        ),
+        message="Vegetation drag can only be used in combination with friction type 1 (Chézy)",
+    )
+]
+
+CHECKS += [
     AllEqualCheck(error_code=330 + i, column=column, level=CheckLevel.WARNING)
     for i, column in enumerate(
         [
             models.GlobalSetting.use_2d_flow,
             models.GlobalSetting.use_1d_flow,
             models.GlobalSetting.grid_space,
             models.GlobalSetting.dist_calc_points,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/exporters.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/exporters.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/interfaces/raster_interface.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/interfaces/raster_interface.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/interfaces/raster_interface_gdal.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/interfaces/raster_interface_gdal.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/interfaces/raster_interface_rasterio.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/interfaces/raster_interface_rasterio.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/model_checks.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/model_checks.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/scripts.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/scripts.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/conftest.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/factories.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/factories.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_base.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_base.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_cross_section_definitions.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_cross_section_definitions.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_factories.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_factories.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_other.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_other.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_raster.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_raster.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,14 +335,15 @@
     "raster_pixel_size, sqlite_grid_space, validity",
     [
         (2, 7, False),
         (2, 4, True),
         (2, 3, False),
         (2, 0, False),
         (2, -4, False),
+        (2, 7.9999999999999999, True),
     ],
 )
 def test_raster_grid_size(
     tmp_path, interface_cls, raster_pixel_size, sqlite_grid_space, validity
 ):
     path = create_geotiff(
         tmp_path / "raster.tiff", dx=raster_pixel_size, dy=raster_pixel_size
```

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_timeseries.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_timeseries.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_exporters.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_model_checks.py` & `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_model_checks.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/PKG-INFO` & `threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-modelchecker
-Version: 2.2.2
+Version: 2.2.3
 Summary: Checks validity of a 3Di schematisation
 Home-page: https://github.com/nens/threedi-modelchecker
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/SOURCES.txt` & `threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

