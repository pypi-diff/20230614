# Comparing `tmp/G4EPP-0.0.7.tar.gz` & `tmp/G4EPP-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/G4EPP-0.0.7.tar", last modified: Wed Jun 14 16:53:25 2023, max compression
+gzip compressed data, was "dist/G4EPP-0.0.8.tar", last modified: Wed Jun 14 18:05:58 2023, max compression
```

## Comparing `G4EPP-0.0.7.tar` & `G4EPP-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 16:53:25.000000 G4EPP-0.0.7/
-drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 16:53:25.000000 G4EPP-0.0.7/G4EPP/
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)    11720 2023-06-14 16:34:53.000000 G4EPP-0.0.7/G4EPP/G4EPP.py
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       81 2023-06-14 16:49:40.000000 G4EPP-0.0.7/G4EPP/__init__.py
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)     3934 2023-06-14 16:33:46.000000 G4EPP-0.0.7/G4EPP/utils.py
-drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 16:53:25.000000 G4EPP-0.0.7/G4EPP.egg-info/
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      449 2023-06-14 16:53:25.000000 G4EPP-0.0.7/G4EPP.egg-info/PKG-INFO
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      220 2023-06-14 16:53:25.000000 G4EPP-0.0.7/G4EPP.egg-info/SOURCES.txt
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        1 2023-06-14 16:53:25.000000 G4EPP-0.0.7/G4EPP.egg-info/dependency_links.txt
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       51 2023-06-14 16:53:25.000000 G4EPP-0.0.7/G4EPP.egg-info/requires.txt
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        6 2023-06-14 16:53:25.000000 G4EPP-0.0.7/G4EPP.egg-info/top_level.txt
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      449 2023-06-14 16:53:25.000000 G4EPP-0.0.7/PKG-INFO
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      176 2023-04-10 18:48:29.000000 G4EPP-0.0.7/README.md
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       79 2023-06-14 16:53:25.000000 G4EPP-0.0.7/setup.cfg
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      857 2023-06-14 16:50:07.000000 G4EPP-0.0.7/setup.py
+drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 18:05:58.000000 G4EPP-0.0.8/
+drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 18:05:58.000000 G4EPP-0.0.8/G4EPP/
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)    11801 2023-06-14 18:04:58.000000 G4EPP-0.0.8/G4EPP/G4EPP.py
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       52 2023-06-14 18:02:10.000000 G4EPP-0.0.8/G4EPP/__init__.py
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)     3960 2023-06-14 18:04:23.000000 G4EPP-0.0.8/G4EPP/utils.py
+drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 18:05:58.000000 G4EPP-0.0.8/G4EPP.egg-info/
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      449 2023-06-14 18:05:58.000000 G4EPP-0.0.8/G4EPP.egg-info/PKG-INFO
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      220 2023-06-14 18:05:58.000000 G4EPP-0.0.8/G4EPP.egg-info/SOURCES.txt
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        1 2023-06-14 18:05:58.000000 G4EPP-0.0.8/G4EPP.egg-info/dependency_links.txt
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       51 2023-06-14 18:05:58.000000 G4EPP-0.0.8/G4EPP.egg-info/requires.txt
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        6 2023-06-14 18:05:58.000000 G4EPP-0.0.8/G4EPP.egg-info/top_level.txt
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      449 2023-06-14 18:05:58.000000 G4EPP-0.0.8/PKG-INFO
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      176 2023-04-10 18:48:29.000000 G4EPP-0.0.8/README.md
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       79 2023-06-14 18:05:58.000000 G4EPP-0.0.8/setup.cfg
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      857 2023-06-14 18:05:55.000000 G4EPP-0.0.8/setup.py
```

### Comparing `G4EPP-0.0.7/G4EPP/G4EPP.py` & `G4EPP-0.0.8/G4EPP/G4EPP.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 
 from scipy.optimize import curve_fit
 from scipy.optimize import minimize
 from scipy.signal import savgol_filter
 
 import pickle
 
+from utils import FileReader
 
 # Globals
+# TODO: make these direct imports instead of globals
 Earray  = np.round(np.logspace(np.log10(0.250), np.log10(10000), 100), 2)
 
 h       = np.arange(0, 500);
 
 runList = np.array([10, 14, 20, 32, 50, 71, 100, 141, 200, 316, 500, 
                     707, 1000, 1414, 2000, 3162, 5000, 7071, 10000])
 
@@ -79,15 +81,15 @@
         Internal function to download 
         """
         import wget
         
         url = "https://zenodo.org/record/8034275/files/G4data_mono_discretePAD_0degLat.pkl?download=1"
 
         try:
-            wget.download(url, out='./data')
+            wget.download(url, out=dirname)
             print("Data downloaded!")
         except:
             print("Couldn't download data :( contact Grant.Berland@colorado.edu and I'll email it to you")
 
     def plot_spectral_profile(self, energyDistribution, 
                                     pitchAngleDistribution, 
                                     flux,
```

### Comparing `G4EPP-0.0.7/G4EPP/utils.py` & `G4EPP-0.0.8/G4EPP/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
             raise EPP_Exception(energy, "Error: %.1f not in %s" % (energy, self.runList))
 
 
 class FileReader(EPP_Exception_Handler):
     def __init__(self, Earray, runList, PAlist):
 
-        self.data_path = "../data/"
+        self.data_path = os.path.dirname(__file__) + "/data/"
 
         super().__init__(runList)
 
         # Load in pkl data table 
         self.D = pickle.load(open(self.data_path + "G4data_mono_discretePAD_0degLat.pkl", "rb"))
 
         self.runList        = runList
```

### Comparing `G4EPP-0.0.7/setup.py` & `G4EPP-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7' 
+VERSION = '0.0.8' 
 DESCRIPTION = 'GEANT4 EPP Simulation wrapper'
 LONG_DESCRIPTION = 'Python wrapper to process and plot GEANT4 EPP simulation outputs'
 
 setup(
         name="G4EPP", 
         version=VERSION,
         author="Grant Berland",
```

