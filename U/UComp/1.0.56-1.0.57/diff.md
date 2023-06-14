# Comparing `tmp/UComp-1.0.56.tar.gz` & `tmp/UComp-1.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.56.tar", last modified: Wed Jun 14 11:03:15 2023, max compression
+gzip compressed data, was "UComp-1.0.57.tar", last modified: Wed Jun 14 11:20:49 2023, max compression
```

## Comparing `UComp-1.0.56.tar` & `UComp-1.0.57.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 11:03:15.796759 UComp-1.0.56/
--rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.56/MANIFEST.in
--rw-rw-rw-   0        0        0      343 2023-06-14 11:03:15.797757 UComp-1.0.56/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.56/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 11:03:15.760818 UComp-1.0.56/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.56/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.56/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0    10981 2023-06-14 11:02:03.000000 UComp-1.0.56/UComp/ETSmodule.py
--rw-rw-rw-   0        0        0    11794 2023-06-14 07:44:36.000000 UComp-1.0.56/UComp/PTSmodule.py
--rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.56/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.56/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    24546 2023-06-14 07:48:55.000000 UComp-1.0.56/UComp/UCmodule.py
--rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.56/UComp/__init__.py
--rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.56/UComp/airpas.bin
--rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.56/UComp/gdp.bin
--rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.56/UComp/ipi.bin
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.56/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    29759 2023-06-14 08:05:48.000000 UComp-1.0.56/UComp/tools.py
--rw-rw-rw-   0        0        0      570 2023-06-09 15:36:47.000000 UComp-1.0.56/UComp/tsfile.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:03:15.793766 UComp-1.0.56/UComp.egg-info/
--rw-rw-rw-   0        0        0      343 2023-06-14 11:03:15.000000 UComp-1.0.56/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-14 11:03:15.000000 UComp-1.0.56/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 11:03:15.000000 UComp-1.0.56/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-14 11:03:15.000000 UComp-1.0.56/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 11:03:15.000000 UComp-1.0.56/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 11:03:15.800756 UComp-1.0.56/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-14 11:02:27.000000 UComp-1.0.56/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:20:49.322283 UComp-1.0.57/
+-rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.57/MANIFEST.in
+-rw-rw-rw-   0        0        0      343 2023-06-14 11:20:49.323323 UComp-1.0.57/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.57/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 11:20:49.268372 UComp-1.0.57/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.57/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.57/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0    11122 2023-06-14 11:14:57.000000 UComp-1.0.57/UComp/ETSmodule.py
+-rw-rw-rw-   0        0        0    11794 2023-06-14 07:44:36.000000 UComp-1.0.57/UComp/PTSmodule.py
+-rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.57/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.57/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    24546 2023-06-14 07:48:55.000000 UComp-1.0.57/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.57/UComp/__init__.py
+-rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.57/UComp/airpas.bin
+-rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.57/UComp/gdp.bin
+-rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.57/UComp/ipi.bin
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.57/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    29782 2023-06-14 11:19:12.000000 UComp-1.0.57/UComp/tools.py
+-rw-rw-rw-   0        0        0      570 2023-06-09 15:36:47.000000 UComp-1.0.57/UComp/tsfile.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:20:49.320331 UComp-1.0.57/UComp.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-06-14 11:20:48.000000 UComp-1.0.57/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-14 11:20:48.000000 UComp-1.0.57/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 11:20:48.000000 UComp-1.0.57/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-14 11:20:48.000000 UComp-1.0.57/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 11:20:48.000000 UComp-1.0.57/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 11:20:49.326330 UComp-1.0.57/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-14 11:20:43.000000 UComp-1.0.57/setup.py
```

### Comparing `UComp-1.0.56/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.57/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.56/UComp/ETSmodule.py` & `UComp-1.0.57/UComp/ETSmodule.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,17 +142,17 @@
                 rowu, colu = u.shape
             if rowu > colu:
                 u = np.transpose(u)
                 rowu, colu = u.shape
         m1 = ETSc.ETSfunC("components", self.y, u.flatten(), rowu, colu, self.model, self.s, self.h, False,
                           self.criterion, self.identAll, self.alphaL, self.betaL, self.gammaL, self.phiL,
                           "standard", False, False, 0, np.array([0, 0]), self.armaIdent, self.p0, self.lambdaBoxCox)
-        self.v = np.array(m1.v)
         self.comp = np.array(m1.comp)
         self.comp = np.reshape(self.comp, (np.floor_divide(self.comp.size, m1.rowcomp), m1.rowcomp))
+        self.v = self.comp[:, 0]
         if m1.compNames[-1] == "/":
             names = m1.compNames[:-1]
         else:
             names = m1.compNames
         names = names.split("/")
         if not isinstance(self.y, np.ndarray):
             self.v = tsfile.ts(np.array(m1.v), self.y.index[0], self.y.index.freq)
@@ -177,15 +177,17 @@
                 rowu, colu = u.shape
             if rowu > colu:
                 u = np.transpose(u)
                 rowu, colu = u.shape
         m1 = ETSc.ETSfunC("validate", self.y, u.flatten(), rowu, colu, self.model, self.s, self.h, False,
                           self.criterion, self.identAll, self.alphaL, self.betaL, self.gammaL, self.phiL,
                           "standard", False, False, 0, np.array([0, 0]), self.armaIdent, self.p0, self.lambdaBoxCox)
-        self.v = np.array(m1.v)
+        self.comp = np.array(m1.comp)
+        self.comp = np.reshape(self.comp, (np.floor_divide(self.comp.size, m1.rowcomp), m1.rowcomp))
+        self.v = self.comp[:, 0]
         self.table = ' '.join([str(i) for i in m1.table])
         if show:
             print(self.table)
 
 
     def plot(self):
         if any(self.comp.shape) == 0:
```

### Comparing `UComp-1.0.56/UComp/PTSmodule.py` & `UComp-1.0.57/UComp/PTSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.56/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.57/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.56/UComp/UCmodule.py` & `UComp-1.0.57/UComp/UCmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.56/UComp/airpas.bin` & `UComp-1.0.57/UComp/airpas.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.56/UComp/gdp.bin` & `UComp-1.0.57/UComp/gdp.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.56/UComp/ipi.bin` & `UComp-1.0.57/UComp/ipi.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.56/UComp/libopenblas.dll` & `UComp-1.0.57/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.56/UComp/tools.py` & `UComp-1.0.57/UComp/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import seaborn as sns
 import scipy.stats as stats
 if False:
     import UCmodule as uc
 else:
     from UComp import UCmodule as uc
     from UComp import ETSmodule as ets
+    from UComp import PTSmodule as pts
     from UComp import tsfile
 
 
 ipi = pd.read_pickle("ipi.bin")
 gdp = pd.read_pickle("gdp.bin")
 airpas = pd.read_pickle("airpas.bin")
 
@@ -23,18 +24,16 @@
     if end == '':
         end = y.index[-1]
     suby = y.loc[pd.to_datetime(start) : pd.to_datetime(end)]
     return(suby)
 
 
 def obj2array(y):
-    if isinstance(y, uc.UCmodel):
-        x = y.v.values
-    elif isinstance(y, ets.ETSmodel):
-        x = y.comp[:, 0].values
+    if isinstance(y, uc.UCmodel) or isinstance(y, ets.ETSmodel) or isinstance(y, pts.PTSmodel):
+        x = y.v
     elif isinstance(y, pd.Series) or isinstance(y, pd.DataFrame):
         x = y.values
     elif isinstance(y, np.ndarray):
         x = y
     return x
```

### Comparing `UComp-1.0.56/UComp/tsfile.py` & `UComp-1.0.57/UComp/tsfile.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.56/setup.py` & `UComp-1.0.57/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.56',
+    version='1.0.57',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

