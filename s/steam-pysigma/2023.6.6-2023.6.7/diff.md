# Comparing `tmp/steam-pysigma-2023.6.6.tar.gz` & `tmp/steam-pysigma-2023.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-pysigma-2023.6.6.tar", last modified: Wed Jun 14 13:36:59 2023, max compression
+gzip compressed data, was "dist\steam-pysigma-2023.6.7.tar", last modified: Wed Jun 14 14:29:22 2023, max compression
```

## Comparing `steam-pysigma-2023.6.6.tar` & `steam-pysigma-2023.6.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 13:36:59.512051 steam-pysigma-2023.6.6/
--rw-rw-rw-   0        0        0     1030 2023-06-14 13:36:59.511053 steam-pysigma-2023.6.6/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.6.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 13:36:59.512051 steam-pysigma-2023.6.6/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-06-14 13:36:18.000000 steam-pysigma-2023.6.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:36:59.469051 steam-pysigma-2023.6.6/steam_pysigma/
--rw-rw-rw-   0        0        0     2861 2023-05-23 07:10:27.000000 steam-pysigma-2023.6.6/steam_pysigma/MainSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.6.6/steam_pysigma/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:36:59.487052 steam-pysigma-2023.6.6/steam_pysigma/comsol/
--rw-rw-rw-   0        0        0    17446 2023-06-14 06:46:01.000000 steam-pysigma-2023.6.6/steam_pysigma/comsol/BuildComsolModel.py
--rw-rw-rw-   0        0        0    15166 2023-05-24 08:17:29.000000 steam-pysigma-2023.6.6/steam_pysigma/comsol/BuildGlobalVariables.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.6/steam_pysigma/comsol/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:36:59.491051 steam-pysigma-2023.6.6/steam_pysigma/data/
--rw-rw-rw-   0        0        0     8068 2023-05-25 12:15:47.000000 steam-pysigma-2023.6.6/steam_pysigma/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     7220 2023-06-01 09:48:39.000000 steam-pysigma-2023.6.6/steam_pysigma/data/DataSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.6/steam_pysigma/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:36:59.494051 steam-pysigma-2023.6.6/steam_pysigma/domain_generator/
--rw-rw-rw-   0        0        0    17309 2023-06-14 13:36:18.000000 steam-pysigma-2023.6.6/steam_pysigma/domain_generator/GeometryMultipole.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.6/steam_pysigma/domain_generator/__init__.py
--rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.6.6/steam_pysigma/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:36:59.497052 steam-pysigma-2023.6.6/steam_pysigma/parsers/
--rw-rw-rw-   0        0        0     1975 2023-05-25 12:04:31.000000 steam-pysigma-2023.6.6/steam_pysigma/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.6/steam_pysigma/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:36:59.501051 steam-pysigma-2023.6.6/steam_pysigma/plotters/
--rw-rw-rw-   0        0        0    17437 2023-05-08 12:35:29.000000 steam-pysigma-2023.6.6/steam_pysigma/plotters/PlotterPysigma.py
--rw-rw-rw-   0        0        0     8879 2023-05-22 07:52:03.000000 steam-pysigma-2023.6.6/steam_pysigma/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.6/steam_pysigma/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:36:59.504052 steam-pysigma-2023.6.6/steam_pysigma/postprocessing/
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.6/steam_pysigma/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     3077 2023-05-08 12:18:35.000000 steam-pysigma-2023.6.6/steam_pysigma/postprocessing/postprocessing.py
--rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.6.6/steam_pysigma/pysigma.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:36:59.509051 steam-pysigma-2023.6.6/steam_pysigma/utils/
--rw-rw-rw-   0        0        0     1945 2023-05-08 12:45:36.000000 steam-pysigma-2023.6.6/steam_pysigma/utils/Util.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.6/steam_pysigma/utils/__init__.py
--rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-pysigma-2023.6.6/steam_pysigma/utils/make_folder_if_not_existing.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:36:59.482051 steam-pysigma-2023.6.6/steam_pysigma.egg-info/
--rw-rw-rw-   0        0        0     1030 2023-06-14 13:36:55.000000 steam-pysigma-2023.6.6/steam_pysigma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1005 2023-06-14 13:36:55.000000 steam-pysigma-2023.6.6/steam_pysigma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 13:36:55.000000 steam-pysigma-2023.6.6/steam_pysigma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      315 2023-06-14 13:36:55.000000 steam-pysigma-2023.6.6/steam_pysigma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-14 13:36:55.000000 steam-pysigma-2023.6.6/steam_pysigma.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.528104 steam-pysigma-2023.6.7/
+-rw-rw-rw-   0        0        0     1030 2023-06-14 14:29:22.527103 steam-pysigma-2023.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.6.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 14:29:22.528104 steam-pysigma-2023.6.7/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-06-14 14:28:54.000000 steam-pysigma-2023.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.486103 steam-pysigma-2023.6.7/steam_pysigma/
+-rw-rw-rw-   0        0        0     2861 2023-05-23 07:10:27.000000 steam-pysigma-2023.6.7/steam_pysigma/MainSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.6.7/steam_pysigma/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.500103 steam-pysigma-2023.6.7/steam_pysigma/comsol/
+-rw-rw-rw-   0        0        0    17446 2023-06-14 06:46:01.000000 steam-pysigma-2023.6.7/steam_pysigma/comsol/BuildComsolModel.py
+-rw-rw-rw-   0        0        0    15172 2023-06-14 14:28:30.000000 steam-pysigma-2023.6.7/steam_pysigma/comsol/BuildGlobalVariables.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.7/steam_pysigma/comsol/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.506105 steam-pysigma-2023.6.7/steam_pysigma/data/
+-rw-rw-rw-   0        0        0     8068 2023-05-25 12:15:47.000000 steam-pysigma-2023.6.7/steam_pysigma/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     7220 2023-06-01 09:48:39.000000 steam-pysigma-2023.6.7/steam_pysigma/data/DataSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.7/steam_pysigma/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.509103 steam-pysigma-2023.6.7/steam_pysigma/domain_generator/
+-rw-rw-rw-   0        0        0    17309 2023-06-14 13:36:18.000000 steam-pysigma-2023.6.7/steam_pysigma/domain_generator/GeometryMultipole.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.7/steam_pysigma/domain_generator/__init__.py
+-rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.6.7/steam_pysigma/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.512104 steam-pysigma-2023.6.7/steam_pysigma/parsers/
+-rw-rw-rw-   0        0        0     1975 2023-05-25 12:04:31.000000 steam-pysigma-2023.6.7/steam_pysigma/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.7/steam_pysigma/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.517104 steam-pysigma-2023.6.7/steam_pysigma/plotters/
+-rw-rw-rw-   0        0        0    17437 2023-05-08 12:35:29.000000 steam-pysigma-2023.6.7/steam_pysigma/plotters/PlotterPysigma.py
+-rw-rw-rw-   0        0        0     8879 2023-05-22 07:52:03.000000 steam-pysigma-2023.6.7/steam_pysigma/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.7/steam_pysigma/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.520103 steam-pysigma-2023.6.7/steam_pysigma/postprocessing/
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.7/steam_pysigma/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     3077 2023-05-08 12:18:35.000000 steam-pysigma-2023.6.7/steam_pysigma/postprocessing/postprocessing.py
+-rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.6.7/steam_pysigma/pysigma.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.525103 steam-pysigma-2023.6.7/steam_pysigma/utils/
+-rw-rw-rw-   0        0        0     1945 2023-05-08 12:45:36.000000 steam-pysigma-2023.6.7/steam_pysigma/utils/Util.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.7/steam_pysigma/utils/__init__.py
+-rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-pysigma-2023.6.7/steam_pysigma/utils/make_folder_if_not_existing.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.496102 steam-pysigma-2023.6.7/steam_pysigma.egg-info/
+-rw-rw-rw-   0        0        0     1030 2023-06-14 14:29:18.000000 steam-pysigma-2023.6.7/steam_pysigma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1005 2023-06-14 14:29:18.000000 steam-pysigma-2023.6.7/steam_pysigma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 14:29:18.000000 steam-pysigma-2023.6.7/steam_pysigma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      315 2023-06-14 14:29:18.000000 steam-pysigma-2023.6.7/steam_pysigma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-14 14:29:18.000000 steam-pysigma-2023.6.7/steam_pysigma.egg-info/top_level.txt
```

### Comparing `steam-pysigma-2023.6.6/PKG-INFO` & `steam-pysigma-2023.6.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.6.6
+Version: 2023.6.7
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: SIGMA,CERN,STEAM
+Keywords: CERN,STEAM,SIGMA
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.6.6/README.md` & `steam-pysigma-2023.6.7/README.md`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.6/setup.py` & `steam-pysigma-2023.6.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-pysigma',
-    version="2023.6.6",
+    version="2023.6.7",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="This is python wrapper of STEAM SIGMA code",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_pysigma",
     keywords={'STEAM', 'SIGMA', 'CERN'},
```

### Comparing `steam-pysigma-2023.6.6/steam_pysigma/MainSIGMA.py` & `steam-pysigma-2023.6.7/steam_pysigma/MainSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.6/steam_pysigma/comsol/BuildComsolModel.py` & `steam-pysigma-2023.6.7/steam_pysigma/comsol/BuildComsolModel.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.6/steam_pysigma/comsol/BuildGlobalVariables.py` & `steam-pysigma-2023.6.7/steam_pysigma/comsol/BuildGlobalVariables.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                 if key == "time":
                     # Check number of values
                     if len(value) != len(options_sigma.postprocessing.out_1D_vs_times.variables):
                         raise ValueError("Number of time vectors must be the same as number of variables.")
                     else:
                         for i in range(len(value)):
                             if len(value[i]) == 3:
-                                if value[0] > value[2]:
+                                if value[i][0] > value[i][2]:
                                     raise ValueError(
                                         f"options_sigma.postprocessing.out_1D_vs_times.time has invalid data for value {value}. Start value can not be larger than end value.")
                             else:
                                 raise ValueError(
                                     "options_sigma.postprocessing.out_1D_vs_times.time has invalid data. Three elements needed.")
 
         # options_sigma.quench_heaters
```

### Comparing `steam-pysigma-2023.6.6/steam_pysigma/data/DataRoxieParser.py` & `steam-pysigma-2023.6.7/steam_pysigma/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.6/steam_pysigma/data/DataSIGMA.py` & `steam-pysigma-2023.6.7/steam_pysigma/data/DataSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.6/steam_pysigma/domain_generator/GeometryMultipole.py` & `steam-pysigma-2023.6.7/steam_pysigma/domain_generator/GeometryMultipole.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.6/steam_pysigma/helpers.py` & `steam-pysigma-2023.6.7/steam_pysigma/helpers.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.6/steam_pysigma/parsers/ParserRoxie.py` & `steam-pysigma-2023.6.7/steam_pysigma/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.6/steam_pysigma/plotters/PlotterPysigma.py` & `steam-pysigma-2023.6.7/steam_pysigma/plotters/PlotterPysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.6/steam_pysigma/plotters/PlotterRoxie.py` & `steam-pysigma-2023.6.7/steam_pysigma/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.6/steam_pysigma/postprocessing/postprocessing.py` & `steam-pysigma-2023.6.7/steam_pysigma/postprocessing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.6/steam_pysigma/pysigma.py` & `steam-pysigma-2023.6.7/steam_pysigma/pysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.6/steam_pysigma/utils/Util.py` & `steam-pysigma-2023.6.7/steam_pysigma/utils/Util.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.6/steam_pysigma.egg-info/PKG-INFO` & `steam-pysigma-2023.6.7/steam_pysigma.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.6.6
+Version: 2023.6.7
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: SIGMA,CERN,STEAM
+Keywords: CERN,STEAM,SIGMA
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.6.6/steam_pysigma.egg-info/SOURCES.txt` & `steam-pysigma-2023.6.7/steam_pysigma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

