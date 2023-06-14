# Comparing `tmp/G4EPP-0.0.8.tar.gz` & `tmp/G4EPP-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/G4EPP-0.0.8.tar", last modified: Wed Jun 14 18:05:58 2023, max compression
+gzip compressed data, was "dist/G4EPP-0.0.9.tar", last modified: Wed Jun 14 21:00:31 2023, max compression
```

## Comparing `G4EPP-0.0.8.tar` & `G4EPP-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 18:05:58.000000 G4EPP-0.0.8/
-drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 18:05:58.000000 G4EPP-0.0.8/G4EPP/
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)    11801 2023-06-14 18:04:58.000000 G4EPP-0.0.8/G4EPP/G4EPP.py
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       52 2023-06-14 18:02:10.000000 G4EPP-0.0.8/G4EPP/__init__.py
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)     3960 2023-06-14 18:04:23.000000 G4EPP-0.0.8/G4EPP/utils.py
-drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 18:05:58.000000 G4EPP-0.0.8/G4EPP.egg-info/
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      449 2023-06-14 18:05:58.000000 G4EPP-0.0.8/G4EPP.egg-info/PKG-INFO
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      220 2023-06-14 18:05:58.000000 G4EPP-0.0.8/G4EPP.egg-info/SOURCES.txt
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        1 2023-06-14 18:05:58.000000 G4EPP-0.0.8/G4EPP.egg-info/dependency_links.txt
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       51 2023-06-14 18:05:58.000000 G4EPP-0.0.8/G4EPP.egg-info/requires.txt
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        6 2023-06-14 18:05:58.000000 G4EPP-0.0.8/G4EPP.egg-info/top_level.txt
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      449 2023-06-14 18:05:58.000000 G4EPP-0.0.8/PKG-INFO
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      176 2023-04-10 18:48:29.000000 G4EPP-0.0.8/README.md
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       79 2023-06-14 18:05:58.000000 G4EPP-0.0.8/setup.cfg
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      857 2023-06-14 18:05:55.000000 G4EPP-0.0.8/setup.py
+drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 21:00:31.000000 G4EPP-0.0.9/
+drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 21:00:31.000000 G4EPP-0.0.9/G4EPP/
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)    12041 2023-06-14 20:59:34.000000 G4EPP-0.0.9/G4EPP/G4EPP.py
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       52 2023-06-14 18:02:10.000000 G4EPP-0.0.9/G4EPP/__init__.py
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)     3960 2023-06-14 18:04:23.000000 G4EPP-0.0.9/G4EPP/utils.py
+drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 21:00:31.000000 G4EPP-0.0.9/G4EPP.egg-info/
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      449 2023-06-14 21:00:31.000000 G4EPP-0.0.9/G4EPP.egg-info/PKG-INFO
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      220 2023-06-14 21:00:31.000000 G4EPP-0.0.9/G4EPP.egg-info/SOURCES.txt
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        1 2023-06-14 21:00:31.000000 G4EPP-0.0.9/G4EPP.egg-info/dependency_links.txt
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       51 2023-06-14 21:00:31.000000 G4EPP-0.0.9/G4EPP.egg-info/requires.txt
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        6 2023-06-14 21:00:31.000000 G4EPP-0.0.9/G4EPP.egg-info/top_level.txt
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      449 2023-06-14 21:00:31.000000 G4EPP-0.0.9/PKG-INFO
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      176 2023-04-10 18:48:29.000000 G4EPP-0.0.9/README.md
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       79 2023-06-14 21:00:31.000000 G4EPP-0.0.9/setup.cfg
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      857 2023-06-14 21:00:25.000000 G4EPP-0.0.9/setup.py
```

### Comparing `G4EPP-0.0.8/G4EPP/G4EPP.py` & `G4EPP-0.0.9/G4EPP/G4EPP.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
 from scipy.optimize import curve_fit
 from scipy.optimize import minimize
 from scipy.signal import savgol_filter
 
 import pickle
 
-from utils import FileReader
+from G4EPP.utils import FileReader
 
 # Globals
-# TODO: make these direct imports instead of globals
 Earray  = np.round(np.logspace(np.log10(0.250), np.log10(10000), 100), 2)
 
 h       = np.arange(0, 500);
 
 runList = np.array([10, 14, 20, 32, 50, 71, 100, 141, 200, 316, 500, 
                     707, 1000, 1414, 2000, 3162, 5000, 7071, 10000])
 
@@ -43,56 +42,61 @@
         self.dE = np.hstack([np.diff(self.Earray), np.diff(self.Earray)[-1]])
 
         self.EbinCenters = self.Earray + self.dE
 
         self.runList        = runList
         self.PAlist         = PAlist
 
+        self.dirname = os.path.dirname(__file__)
+        
+        # Check if look up table downloaded
+        if self._check_if_data_present() is False:
 
-        try:
-            super().__init__(self.Earray, self.runList, self.PAlist)
-
-        except(FileNotFoundError):
+            print("Lookup table data missing, downloading now...")
+            
+            # If not, download from Zenodo
+            self._download_data()
 
-            # Check if look up table downloaded
-            if self._check_if_data_present() is False:
+        super().__init__(self.Earray, self.runList, self.PAlist)
 
-                print("Lookup table data missing, downloading now...")
-            
-                # If not, download from Zenodo
-                self._download_data()
 
 
         self.X_energy, self.Y_altitude = np.meshgrid(self.Earray, self.h)
 
         
 
     def _check_if_data_present(self):
         """
         Internal function to check if look up table is present
         """
-        dirname = os.path.dirname(__file__)
 
-        total_path = dirname + '/data/G4data_mono_discretePAD_0degLat.pkl'
+        total_path = self.dirname + '/data/G4data_mono_discretePAD_0degLat.pkl'
 
         return os.path.isfile(total_path)
 
     def _download_data(self):
         """
         Internal function to download 
         """
-        import wget
-        
+        import wget, sys
+
+        os.mkdir(self.dirname + '/data')
+
         url = "https://zenodo.org/record/8034275/files/G4data_mono_discretePAD_0degLat.pkl?download=1"
+        def bar_progress(current, total, width=80):
+            progress_message = "Downloading: %d%% [%d / %d] kB" % (current / total * 100, int(1e-3 * current), int(1e-3 * total))
+            sys.stdout.write("\r" + progress_message)
+            sys.stdout.flush()
+
 
-        try:
-            wget.download(url, out=dirname)
-            print("Data downloaded!")
-        except:
-            print("Couldn't download data :( contact Grant.Berland@colorado.edu and I'll email it to you")
+        #try:
+        wget.download(url, out=self.dirname + '/data', bar=bar_progress)
+        print("Data downloaded!")
+        #except:
+            #print("Couldn't download data :( contact Grant.Berland@colorado.edu and I'll email it to you")
 
     def plot_spectral_profile(self, energyDistribution, 
                                     pitchAngleDistribution, 
                                     flux, 
                                     particle=None):
 
         result, norm = self._formGreensFunctionSpectrum(energyDistribution, 
@@ -187,15 +191,15 @@
     def get_energy_array(self):
         return self.Earray
 
     def get_bin_width(self):
         return self.binWidth
 
     def get_run_list(self):
-        return self.runList
+        return 1e3 * self.runList
 
     def get_PA_list(self):
         return self.PAlist
 
 
 class XrayAnalysis(FileReader):
     def __init__(self):
```

### Comparing `G4EPP-0.0.8/G4EPP/utils.py` & `G4EPP-0.0.9/G4EPP/utils.py`

 * *Files identical despite different names*

### Comparing `G4EPP-0.0.8/setup.py` & `G4EPP-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8' 
+VERSION = '0.0.9' 
 DESCRIPTION = 'GEANT4 EPP Simulation wrapper'
 LONG_DESCRIPTION = 'Python wrapper to process and plot GEANT4 EPP simulation outputs'
 
 setup(
         name="G4EPP", 
         version=VERSION,
         author="Grant Berland",
```

