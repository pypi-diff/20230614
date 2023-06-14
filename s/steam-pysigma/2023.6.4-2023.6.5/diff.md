# Comparing `tmp/steam-pysigma-2023.6.4.tar.gz` & `tmp/steam-pysigma-2023.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-pysigma-2023.6.4.tar", last modified: Fri Jun  9 08:42:11 2023, max compression
+gzip compressed data, was "dist\steam-pysigma-2023.6.5.tar", last modified: Wed Jun 14 07:46:19 2023, max compression
```

## Comparing `steam-pysigma-2023.6.4.tar` & `steam-pysigma-2023.6.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.635981 steam-pysigma-2023.6.4/
--rw-rw-rw-   0        0        0     1030 2023-06-09 08:42:11.634982 steam-pysigma-2023.6.4/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.6.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 08:42:11.635981 steam-pysigma-2023.6.4/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-06-09 08:38:29.000000 steam-pysigma-2023.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.592982 steam-pysigma-2023.6.4/steam_pysigma/
--rw-rw-rw-   0        0        0     2861 2023-05-23 07:10:27.000000 steam-pysigma-2023.6.4/steam_pysigma/MainSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.6.4/steam_pysigma/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.605982 steam-pysigma-2023.6.4/steam_pysigma/comsol/
--rw-rw-rw-   0        0        0    17425 2023-06-09 08:39:51.000000 steam-pysigma-2023.6.4/steam_pysigma/comsol/BuildComsolModel.py
--rw-rw-rw-   0        0        0    15166 2023-05-24 08:17:29.000000 steam-pysigma-2023.6.4/steam_pysigma/comsol/BuildGlobalVariables.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.4/steam_pysigma/comsol/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.610982 steam-pysigma-2023.6.4/steam_pysigma/data/
--rw-rw-rw-   0        0        0     8068 2023-05-25 12:15:47.000000 steam-pysigma-2023.6.4/steam_pysigma/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     7220 2023-06-01 09:48:39.000000 steam-pysigma-2023.6.4/steam_pysigma/data/DataSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.4/steam_pysigma/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.613984 steam-pysigma-2023.6.4/steam_pysigma/domain_generator/
--rw-rw-rw-   0        0        0    17563 2023-06-09 08:16:54.000000 steam-pysigma-2023.6.4/steam_pysigma/domain_generator/GeometryMultipole.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.4/steam_pysigma/domain_generator/__init__.py
--rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.6.4/steam_pysigma/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.617982 steam-pysigma-2023.6.4/steam_pysigma/parsers/
--rw-rw-rw-   0        0        0     1975 2023-05-25 12:04:31.000000 steam-pysigma-2023.6.4/steam_pysigma/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.4/steam_pysigma/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.623982 steam-pysigma-2023.6.4/steam_pysigma/plotters/
--rw-rw-rw-   0        0        0    17437 2023-05-08 12:35:29.000000 steam-pysigma-2023.6.4/steam_pysigma/plotters/PlotterPysigma.py
--rw-rw-rw-   0        0        0     8879 2023-05-22 07:52:03.000000 steam-pysigma-2023.6.4/steam_pysigma/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.4/steam_pysigma/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.626990 steam-pysigma-2023.6.4/steam_pysigma/postprocessing/
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.4/steam_pysigma/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     3077 2023-05-08 12:18:35.000000 steam-pysigma-2023.6.4/steam_pysigma/postprocessing/postprocessing.py
--rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.6.4/steam_pysigma/pysigma.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.631981 steam-pysigma-2023.6.4/steam_pysigma/utils/
--rw-rw-rw-   0        0        0     1945 2023-05-08 12:45:36.000000 steam-pysigma-2023.6.4/steam_pysigma/utils/Util.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.4/steam_pysigma/utils/__init__.py
--rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-pysigma-2023.6.4/steam_pysigma/utils/make_folder_if_not_existing.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.600982 steam-pysigma-2023.6.4/steam_pysigma.egg-info/
--rw-rw-rw-   0        0        0     1030 2023-06-09 08:42:07.000000 steam-pysigma-2023.6.4/steam_pysigma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1005 2023-06-09 08:42:07.000000 steam-pysigma-2023.6.4/steam_pysigma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 08:42:07.000000 steam-pysigma-2023.6.4/steam_pysigma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      315 2023-06-09 08:42:07.000000 steam-pysigma-2023.6.4/steam_pysigma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-09 08:42:07.000000 steam-pysigma-2023.6.4/steam_pysigma.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 07:46:19.493874 steam-pysigma-2023.6.5/
+-rw-rw-rw-   0        0        0     1030 2023-06-14 07:46:19.492873 steam-pysigma-2023.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.6.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 07:46:19.493874 steam-pysigma-2023.6.5/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-06-14 07:42:13.000000 steam-pysigma-2023.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:46:19.449874 steam-pysigma-2023.6.5/steam_pysigma/
+-rw-rw-rw-   0        0        0     2861 2023-05-23 07:10:27.000000 steam-pysigma-2023.6.5/steam_pysigma/MainSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.6.5/steam_pysigma/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:46:19.465874 steam-pysigma-2023.6.5/steam_pysigma/comsol/
+-rw-rw-rw-   0        0        0    17446 2023-06-14 06:46:01.000000 steam-pysigma-2023.6.5/steam_pysigma/comsol/BuildComsolModel.py
+-rw-rw-rw-   0        0        0    15166 2023-05-24 08:17:29.000000 steam-pysigma-2023.6.5/steam_pysigma/comsol/BuildGlobalVariables.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.5/steam_pysigma/comsol/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:46:19.470873 steam-pysigma-2023.6.5/steam_pysigma/data/
+-rw-rw-rw-   0        0        0     8068 2023-05-25 12:15:47.000000 steam-pysigma-2023.6.5/steam_pysigma/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     7220 2023-06-01 09:48:39.000000 steam-pysigma-2023.6.5/steam_pysigma/data/DataSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.5/steam_pysigma/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:46:19.473874 steam-pysigma-2023.6.5/steam_pysigma/domain_generator/
+-rw-rw-rw-   0        0        0    17639 2023-06-14 06:46:01.000000 steam-pysigma-2023.6.5/steam_pysigma/domain_generator/GeometryMultipole.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.5/steam_pysigma/domain_generator/__init__.py
+-rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.6.5/steam_pysigma/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:46:19.476873 steam-pysigma-2023.6.5/steam_pysigma/parsers/
+-rw-rw-rw-   0        0        0     1975 2023-05-25 12:04:31.000000 steam-pysigma-2023.6.5/steam_pysigma/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.5/steam_pysigma/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:46:19.483874 steam-pysigma-2023.6.5/steam_pysigma/plotters/
+-rw-rw-rw-   0        0        0    17437 2023-05-08 12:35:29.000000 steam-pysigma-2023.6.5/steam_pysigma/plotters/PlotterPysigma.py
+-rw-rw-rw-   0        0        0     8879 2023-05-22 07:52:03.000000 steam-pysigma-2023.6.5/steam_pysigma/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.5/steam_pysigma/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:46:19.485874 steam-pysigma-2023.6.5/steam_pysigma/postprocessing/
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.5/steam_pysigma/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     3077 2023-05-08 12:18:35.000000 steam-pysigma-2023.6.5/steam_pysigma/postprocessing/postprocessing.py
+-rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.6.5/steam_pysigma/pysigma.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:46:19.490873 steam-pysigma-2023.6.5/steam_pysigma/utils/
+-rw-rw-rw-   0        0        0     1945 2023-05-08 12:45:36.000000 steam-pysigma-2023.6.5/steam_pysigma/utils/Util.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.5/steam_pysigma/utils/__init__.py
+-rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-pysigma-2023.6.5/steam_pysigma/utils/make_folder_if_not_existing.py
+drwxrwxrwx   0        0        0        0 2023-06-14 07:46:19.459874 steam-pysigma-2023.6.5/steam_pysigma.egg-info/
+-rw-rw-rw-   0        0        0     1030 2023-06-14 07:46:15.000000 steam-pysigma-2023.6.5/steam_pysigma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1005 2023-06-14 07:46:15.000000 steam-pysigma-2023.6.5/steam_pysigma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 07:46:15.000000 steam-pysigma-2023.6.5/steam_pysigma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      315 2023-06-14 07:46:15.000000 steam-pysigma-2023.6.5/steam_pysigma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-14 07:46:15.000000 steam-pysigma-2023.6.5/steam_pysigma.egg-info/top_level.txt
```

### Comparing `steam-pysigma-2023.6.4/PKG-INFO` & `steam-pysigma-2023.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.6.4
+Version: 2023.6.5
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,SIGMA,STEAM
+Keywords: CERN,STEAM,SIGMA
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.6.4/README.md` & `steam-pysigma-2023.6.5/README.md`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.4/setup.py` & `steam-pysigma-2023.6.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-pysigma',
-    version="2023.6.4",
+    version="2023.6.5",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="This is python wrapper of STEAM SIGMA code",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_pysigma",
     keywords={'STEAM', 'SIGMA', 'CERN'},
```

### Comparing `steam-pysigma-2023.6.4/steam_pysigma/MainSIGMA.py` & `steam-pysigma-2023.6.5/steam_pysigma/MainSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.4/steam_pysigma/comsol/BuildComsolModel.py` & `steam-pysigma-2023.6.5/steam_pysigma/comsol/BuildComsolModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         bgv.validate_sigma_model_data()
         self.cfg = self.setup_config_sigma()
         self.srv = self.g.TxtSigmaServer(self.cfg.getOutputModelPath(), self.cfg.getComsolBatchPath(),
                                          self.cfg.getComsolCompilePath())
 
 
         geom_multipole = GeometryMultipole(self.g, self.roxie_data, model_data, self.bh_curve_database, self.input_conductor_params,
-                                           self.settings_dict)
+                                           self.settings_dict, self.COMSOL_version)
 
         self.domains = geom_multipole.build_magnet()
         self.wedge_areas = geom_multipole.wedge_areas
         #self.plot_magnet()
         self.connect_create_MPH_model(self.domains)
         self.save_files_java()
         self.save_compile_and_open_bat()
```

### Comparing `steam-pysigma-2023.6.4/steam_pysigma/comsol/BuildGlobalVariables.py` & `steam-pysigma-2023.6.5/steam_pysigma/comsol/BuildGlobalVariables.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.4/steam_pysigma/data/DataRoxieParser.py` & `steam-pysigma-2023.6.5/steam_pysigma/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.4/steam_pysigma/data/DataSIGMA.py` & `steam-pysigma-2023.6.5/steam_pysigma/data/DataSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.4/steam_pysigma/domain_generator/GeometryMultipole.py` & `steam-pysigma-2023.6.5/steam_pysigma/domain_generator/GeometryMultipole.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,30 +8,31 @@
 class GeometryMultipole:
     """
     Class creates SIGMA domain objects
     IMPROVMENTS:
     No dependency on config sigma
     """
 
-    def __init__(self, g, input_roxie_data, input_model_data, bh_curve_database, input_conductor_params, settings_dict, flag_build=True,
+    def __init__(self, g, input_roxie_data, input_model_data, bh_curve_database, input_conductor_params, settings_dict, COMSOL_VERSION, flag_build=True,
                  verbose=False):
 
         self.model_data = input_model_data
         self.roxie_data = input_roxie_data
         self.input_conductor_params = input_conductor_params
         self.bh_curve_database = bh_curve_database
         self.settings_dict: dict = settings_dict
+        self.COMSOL_version = COMSOL_VERSION
         self.verbose = verbose
         if (not self.model_data or not self.roxie_data) and flag_build:
             raise Exception('Cannot build model without providing DataModelMagnet and RoxieData')
         elif flag_build:
             self.g = g
             self.a = ps.ArraysSIGMA
             self.cfg = self.g.ConfigSigma()
-            self.cfg.setComsolVersion("53a")
+            self.cfg.setComsolVersion(self.COMSOL_version)
             self.max_r: float = 0.1
             self.conductor_name = str
             self.cableParameters = {'cable': {}, 'strand': {}, 'Jc_fit': {}}  # dM.Conductor #self.cablesParameters
             # self.wedge_elements =
             # self.model =
             self.coil = []
             self.elements = {}
```

### Comparing `steam-pysigma-2023.6.4/steam_pysigma/helpers.py` & `steam-pysigma-2023.6.5/steam_pysigma/helpers.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.4/steam_pysigma/parsers/ParserRoxie.py` & `steam-pysigma-2023.6.5/steam_pysigma/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.4/steam_pysigma/plotters/PlotterPysigma.py` & `steam-pysigma-2023.6.5/steam_pysigma/plotters/PlotterPysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.4/steam_pysigma/plotters/PlotterRoxie.py` & `steam-pysigma-2023.6.5/steam_pysigma/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.4/steam_pysigma/postprocessing/postprocessing.py` & `steam-pysigma-2023.6.5/steam_pysigma/postprocessing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.4/steam_pysigma/pysigma.py` & `steam-pysigma-2023.6.5/steam_pysigma/pysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.4/steam_pysigma/utils/Util.py` & `steam-pysigma-2023.6.5/steam_pysigma/utils/Util.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.4/steam_pysigma.egg-info/PKG-INFO` & `steam-pysigma-2023.6.5/steam_pysigma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.6.4
+Version: 2023.6.5
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,SIGMA,STEAM
+Keywords: CERN,STEAM,SIGMA
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.6.4/steam_pysigma.egg-info/SOURCES.txt` & `steam-pysigma-2023.6.5/steam_pysigma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

