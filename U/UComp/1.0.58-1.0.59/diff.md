# Comparing `tmp/UComp-1.0.58.tar.gz` & `tmp/UComp-1.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.58.tar", last modified: Wed Jun 14 11:29:54 2023, max compression
+gzip compressed data, was "UComp-1.0.59.tar", last modified: Wed Jun 14 14:52:37 2023, max compression
```

## Comparing `UComp-1.0.58.tar` & `UComp-1.0.59.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 11:29:54.335226 UComp-1.0.58/
--rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.58/MANIFEST.in
--rw-rw-rw-   0        0        0      343 2023-06-14 11:29:54.335226 UComp-1.0.58/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.58/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 11:29:54.306284 UComp-1.0.58/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.58/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.58/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0    11285 2023-06-14 11:29:03.000000 UComp-1.0.58/UComp/ETSmodule.py
--rw-rw-rw-   0        0        0    11794 2023-06-14 07:44:36.000000 UComp-1.0.58/UComp/PTSmodule.py
--rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.58/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.58/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    24546 2023-06-14 07:48:55.000000 UComp-1.0.58/UComp/UCmodule.py
--rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.58/UComp/__init__.py
--rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.58/UComp/airpas.bin
--rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.58/UComp/gdp.bin
--rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.58/UComp/ipi.bin
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.58/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    29782 2023-06-14 11:19:12.000000 UComp-1.0.58/UComp/tools.py
--rw-rw-rw-   0        0        0      570 2023-06-09 15:36:47.000000 UComp-1.0.58/UComp/tsfile.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:29:54.333227 UComp-1.0.58/UComp.egg-info/
--rw-rw-rw-   0        0        0      343 2023-06-14 11:29:53.000000 UComp-1.0.58/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-14 11:29:53.000000 UComp-1.0.58/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 11:29:53.000000 UComp-1.0.58/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-14 11:29:53.000000 UComp-1.0.58/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 11:29:53.000000 UComp-1.0.58/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 11:29:54.338179 UComp-1.0.58/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-14 11:29:17.000000 UComp-1.0.58/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:52:37.002962 UComp-1.0.59/
+-rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.59/MANIFEST.in
+-rw-rw-rw-   0        0        0      304 2023-06-14 14:52:37.002962 UComp-1.0.59/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.59/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 14:52:36.971714 UComp-1.0.59/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.59/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.59/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0    11274 2023-06-14 14:49:10.000000 UComp-1.0.59/UComp/ETSmodule.py
+-rw-rw-rw-   0        0        0    11790 2023-06-14 14:49:10.000000 UComp-1.0.59/UComp/PTSmodule.py
+-rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.59/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.59/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    24515 2023-06-14 14:47:37.000000 UComp-1.0.59/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.59/UComp/__init__.py
+-rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.59/UComp/airpas.bin
+-rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.59/UComp/gdp.bin
+-rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.59/UComp/ipi.bin
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.59/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    29855 2023-06-14 14:47:37.000000 UComp-1.0.59/UComp/tools.py
+-rw-rw-rw-   0        0        0      570 2023-06-09 15:36:47.000000 UComp-1.0.59/UComp/tsfile.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:52:37.002962 UComp-1.0.59/UComp.egg-info/
+-rw-rw-rw-   0        0        0      304 2023-06-14 14:52:35.000000 UComp-1.0.59/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-14 14:52:35.000000 UComp-1.0.59/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 14:52:35.000000 UComp-1.0.59/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-14 14:52:35.000000 UComp-1.0.59/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 14:52:35.000000 UComp-1.0.59/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 14:52:37.002962 UComp-1.0.59/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-14 14:51:11.000000 UComp-1.0.59/setup.py
```

### Comparing `UComp-1.0.58/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.59/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.58/UComp/ETSmodule.py` & `UComp-1.0.59/UComp/ETSmodule.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 # c++ -O3 -Wall -shared -std=c++11 -undefined dynamic_lookup -I/Library/Frameworks/Python.framework/Headers
 # -I"/Users/diego.pedregal/Google Drive/C++/armadillo-10.8.2/include" -llapack -lblas $(python3 -m
 # pybind11 --includes) pythonBSM.cpp -o BSMc$(python3-config --extension-suffix)
 import numpy as np
 import pandas as pd
 
 
-if False:           # To run locally
-    import ETSc
-else:              # To run from package in PyPI
+RunningFromPackage = True
+if RunningFromPackage:
     from UComp import ETSc
     from UComp import tsfile
+else:
+    import ETSc
+    import tsfile
 
 
 class ETSmodel:
     """
     ETSmodel
     Estimates and forecasts a general ETS model
 
@@ -143,26 +145,27 @@
             if rowu > colu:
                 u = np.transpose(u)
                 rowu, colu = u.shape
         m1 = ETSc.ETSfunC("components", self.y, u.flatten(), rowu, colu, self.model, self.s, self.h, False,
                           self.criterion, self.identAll, self.alphaL, self.betaL, self.gammaL, self.phiL,
                           "standard", False, False, 0, np.array([0, 0]), self.armaIdent, self.p0, self.lambdaBoxCox)
         self.comp = np.array(m1.comp)
+        nrows = int(self.comp.shape[0] / self.y.shape[0])
+        self.comp = np.transpose(np.reshape(self.comp, (nrows, np.floor_divide(self.comp.size, nrows))))
         self.v = self.comp[:, 0]
         if m1.compNames[-1] == "/":
             names = m1.compNames[:-1]
         else:
             names = m1.compNames
         names = names.split("/")
         if not isinstance(self.y, np.ndarray):
             self.comp = tsfile.ts(self.comp, self.y.index[0], self.y.index.freq)
-            self.comp.columns = names
         else:
-            dt = [(nombre, self.comp.dtype) for nombre in names]
-            self.comp = self.comp.view(dtype=dt)
+            self.comp = pd.DataFrame(self.comp, index=range(self.comp.shape[0]))
+        self.comp.columns = names
 
 
     def validate(self, show=True):
         u = self.u
         if u.size == 0:
             u = np.array([-99999])
             rowu = 0
@@ -175,36 +178,31 @@
                 rowu, colu = u.shape
             if rowu > colu:
                 u = np.transpose(u)
                 rowu, colu = u.shape
         m1 = ETSc.ETSfunC("validate", self.y, u.flatten(), rowu, colu, self.model, self.s, self.h, False,
                           self.criterion, self.identAll, self.alphaL, self.betaL, self.gammaL, self.phiL,
                           "standard", False, False, 0, np.array([0, 0]), self.armaIdent, self.p0, self.lambdaBoxCox)
-        self.comp = np.array(m1.comp)
-        self.v = self.comp[:, 0]
-        if m1.compNames[-1] == "/":
-            names = m1.compNames[:-1]
-        else:
-            names = m1.compNames
-        names = names.split("/")
-        if not isinstance(self.y, np.ndarray):
-            self.comp = tsfile.ts(self.comp, self.y.index[0], self.y.index.freq)
-            self.comp.columns = names
-        else:
-            dt = [(nombre, self.comp.dtype) for nombre in names]
-            self.comp = self.comp.view(dtype=dt)
+        comp = np.array(m1.comp)
+        nrows = int(comp.shape[0] / self.y.shape[0])
+        comp = np.transpose(np.reshape(comp, (nrows, np.floor_divide(comp.size, nrows))))
+        self.v = comp[:, 0]
         self.table = ' '.join([str(i) for i in m1.table])
         if show:
             print(self.table)
 
 
     def plot(self):
         if any(self.comp.shape) == 0:
-            self.components(self)
-        self.comp.plot(subplots=True, layout=(len(self.comp.columns), 1), figsize=(10, 6), sharex=True)
+            self.components()
+        if isinstance(self.comp, pd.Series) or isinstance(self.comp, pd.DataFrame):
+            toplot = self.comp
+        else:
+            toplot = pd.DataFrame(self.comp, range(self.comp.shape[0]))
+        toplot.plot(subplots=True, layout=(len(toplot.columns), 1), figsize=(10, 6), sharex=True)
 
 
 def ETS(y: np.array, s: int = np.nan, u: np.array = np.array([]), model: str = "???",
         h: int = 24, criterion: str = "aicc",
         armaIdent: bool = False, identAll: bool = False, forIntervals: bool = False,
         bootstrap: bool = False, nSimul: int = 5000, verbose: bool = False,
         alphaL: np.array = np.array([0, 1]), betaL: np.array = np.array([0, 1]),
```

### Comparing `UComp-1.0.58/UComp/PTSmodule.py` & `UComp-1.0.59/UComp/PTSmodule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Compile with:
 # c++ -O3 -Wall -shared -std=c++11 -undefined dynamic_lookup -I/Library/Frameworks/Python.framework/Headers
 # -I"/Users/diego.pedregal/Google Drive/C++/armadillo-10.8.2/include" -llapack -lblas $(python3 -m
 # pybind11 --includes) pythonBSM.cpp -o BSMc$(python3-config --extension-suffix)
 import numpy as np
 import pandas as pd
 
-if False:           # To run locally
-    import UCmodule as uc
-else:              # To run from package in PyPI
+RunningFromPackage = True
+if RunningFromPackage:
     from UComp import UCmodule as uc
+else:           # To run locally
+    import UCmodule as uc
 
 
 def modelUC2arma(model):
     # ARMA model orders
     ar = 0
     ma = 0
     posi = model.find("arma")
```

### Comparing `UComp-1.0.58/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.59/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.58/UComp/UCmodule.py` & `UComp-1.0.59/UComp/UCmodule.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 # c++ -O3 -Wall -shared -std=c++11 -undefined dynamic_lookup -I/Library/Frameworks/Python.framework/Headers
 # -I"/Users/diego.pedregal/Google Drive/C++/armadillo-10.8.2/include" -llapack -lblas $(python3 -m
 # pybind11 --includes) pythonBSM.cpp -o BSMc$(python3-config --extension-suffix)
 import numpy as np
 import pandas as pd
 
 
-if False:           # To run locally
-    import UCc
-else:              # To run from package in PyPI
+RunningFromPackage = True
+if RunningFromPackage:
     from UComp import UCc
     from UComp import tsfile
+else:
+    import UCc
 
 
 class UCmodel:
     """
     UCmodel
     Estimates and forecasts UC general time series models
```

### Comparing `UComp-1.0.58/UComp/airpas.bin` & `UComp-1.0.59/UComp/airpas.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.58/UComp/gdp.bin` & `UComp-1.0.59/UComp/gdp.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.58/UComp/ipi.bin` & `UComp-1.0.59/UComp/ipi.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.58/UComp/libopenblas.dll` & `UComp-1.0.59/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.58/UComp/tools.py` & `UComp-1.0.59/UComp/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import multiprocessing as mp
 import seaborn as sns
 import scipy.stats as stats
-if False:
-    import UCmodule as uc
-else:
+
+
+RunningFromPackage = True
+if RunningFromPackage:
     from UComp import UCmodule as uc
     from UComp import ETSmodule as ets
     from UComp import PTSmodule as pts
     from UComp import tsfile
+else:
+    import UCmodule as uc
+    import ETSmodule as ets
 
 
 ipi = pd.read_pickle("ipi.bin")
 gdp = pd.read_pickle("gdp.bin")
 airpas = pd.read_pickle("airpas.bin")
```

### Comparing `UComp-1.0.58/UComp/tsfile.py` & `UComp-1.0.59/UComp/tsfile.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.58/setup.py` & `UComp-1.0.59/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.58',
+    version='1.0.59',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

