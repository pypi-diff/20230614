# Comparing `tmp/filter_stations-0.3.8.tar.gz` & `tmp/filter_stations-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filter_stations-0.3.8.tar", last modified: Tue Jun 13 06:51:36 2023, max compression
+gzip compressed data, was "filter_stations-0.3.9.tar", last modified: Tue Jun 13 07:04:13 2023, max compression
```

## Comparing `filter_stations-0.3.8.tar` & `filter_stations-0.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 06:51:36.652294 filter_stations-0.3.8/
--rw-rw-rw-   0        0        0      361 2023-06-13 06:51:36.651285 filter_stations-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-05-04 10:44:45.000000 filter_stations-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 06:51:36.616643 filter_stations-0.3.8/filter_stations/
--rw-rw-rw-   0        0        0    47221 2023-06-13 06:51:22.000000 filter_stations-0.3.8/filter_stations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 06:51:36.649653 filter_stations-0.3.8/filter_stations.egg-info/
--rw-rw-rw-   0        0        0      361 2023-06-13 06:51:36.000000 filter_stations-0.3.8/filter_stations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-06-13 06:51:36.000000 filter_stations-0.3.8/filter_stations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 06:51:36.000000 filter_stations-0.3.8/filter_stations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-13 06:51:36.000000 filter_stations-0.3.8/filter_stations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-06-13 06:51:36.000000 filter_stations-0.3.8/filter_stations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-13 06:51:36.000000 filter_stations-0.3.8/filter_stations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 06:51:36.652294 filter_stations-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-06-13 06:51:29.000000 filter_stations-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:04:13.886512 filter_stations-0.3.9/
+-rw-rw-rw-   0        0        0      361 2023-06-13 07:04:13.886002 filter_stations-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-05-04 10:44:45.000000 filter_stations-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 07:04:13.863167 filter_stations-0.3.9/filter_stations/
+-rw-rw-rw-   0        0        0    47224 2023-06-13 06:53:14.000000 filter_stations-0.3.9/filter_stations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:04:13.884249 filter_stations-0.3.9/filter_stations.egg-info/
+-rw-rw-rw-   0        0        0      361 2023-06-13 07:04:13.000000 filter_stations-0.3.9/filter_stations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-06-13 07:04:13.000000 filter_stations-0.3.9/filter_stations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 07:04:13.000000 filter_stations-0.3.9/filter_stations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-13 07:04:13.000000 filter_stations-0.3.9/filter_stations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-06-13 07:04:13.000000 filter_stations-0.3.9/filter_stations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-13 07:04:13.000000 filter_stations-0.3.9/filter_stations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 07:04:13.887097 filter_stations-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-06-13 07:04:05.000000 filter_stations-0.3.9/setup.py
```

### Comparing `filter_stations-0.3.8/filter_stations/__init__.py` & `filter_stations-0.3.9/filter_stations/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import datetime
 import gc
 from math import ceil
 
 
 # Constants
 API_BASE_URL = 'https://datahub.tahmo.org'
-API_MAX_PERIOD = 'Y'
+API_MAX_PERIOD = '365D'
 
 endpoints = {'VARIABLES': 'services/assets/v2/variables', # 28 different variables
              'STATION_INFO': 'services/assets/v2/stations',
              'WEATHER_DATA': 'services/measurements/v2/stations', # Configured before requesting
              'DATA_COMPLETE': 'custom/sensordx/latestmeasurements',
              'STATION_STATUS': 'custom/stations/status'}
```

### Comparing `filter_stations-0.3.8/setup.py` & `filter_stations-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='filter_stations',
-    version='0.3.8',
+    version='0.3.9',
     packages=find_packages(),
     include_package_data=True,
     description='Making it easier to navigate and clean station data',
     author='Austin Kaburia',
     author_email='kaburiaaustin1@gmail.com',
     url='https://github.com/kaburia/Packaging/tree/main/filter_stations',
     install_requires=[
```

