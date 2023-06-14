# Comparing `tmp/UComp-1.0.51.tar.gz` & `tmp/UComp-1.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.51.tar", last modified: Fri Jun  9 15:50:51 2023, max compression
+gzip compressed data, was "UComp-1.0.54.tar", last modified: Wed Jun 14 08:07:12 2023, max compression
```

## Comparing `UComp-1.0.51.tar` & `UComp-1.0.54.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 15:50:51.655257 UComp-1.0.51/
--rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.51/MANIFEST.in
--rw-rw-rw-   0        0        0      304 2023-06-09 15:50:51.655257 UComp-1.0.51/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.51/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 15:50:51.617483 UComp-1.0.51/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.51/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.51/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0    10871 2023-06-09 15:48:14.000000 UComp-1.0.51/UComp/ETSmodule.py
--rw-rw-rw-   0        0        0    11596 2023-06-09 12:22:16.000000 UComp-1.0.51/UComp/PTSmodule.py
--rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.51/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.51/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    24348 2023-06-09 15:47:19.000000 UComp-1.0.51/UComp/UCmodule.py
--rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.51/UComp/__init__.py
--rw-rw-rw-   0        0        0    16507 2023-06-09 15:01:03.000000 UComp-1.0.51/UComp/airpas.bin
--rw-rw-rw-   0        0        0     3645 2023-06-09 15:01:03.000000 UComp-1.0.51/UComp/gdp.bin
--rw-rw-rw-   0        0        0    14731 2023-06-09 15:01:03.000000 UComp-1.0.51/UComp/ipi.bin
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.51/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    29523 2023-06-09 15:49:34.000000 UComp-1.0.51/UComp/tools.py
--rw-rw-rw-   0        0        0      570 2023-06-09 15:36:47.000000 UComp-1.0.51/UComp/tsfile.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:50:51.655257 UComp-1.0.51/UComp.egg-info/
--rw-rw-rw-   0        0        0      304 2023-06-09 15:50:51.000000 UComp-1.0.51/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-09 15:50:51.000000 UComp-1.0.51/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 15:50:51.000000 UComp-1.0.51/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-09 15:50:51.000000 UComp-1.0.51/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 15:50:51.000000 UComp-1.0.51/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 15:50:51.655257 UComp-1.0.51/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-09 15:50:37.000000 UComp-1.0.51/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:07:12.053126 UComp-1.0.54/
+-rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.54/MANIFEST.in
+-rw-rw-rw-   0        0        0      343 2023-06-14 08:07:12.053126 UComp-1.0.54/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.54/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 08:07:12.021887 UComp-1.0.54/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.54/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.54/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0    11069 2023-06-14 07:44:36.000000 UComp-1.0.54/UComp/ETSmodule.py
+-rw-rw-rw-   0        0        0    11794 2023-06-14 07:44:36.000000 UComp-1.0.54/UComp/PTSmodule.py
+-rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.54/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.54/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    24546 2023-06-14 07:48:55.000000 UComp-1.0.54/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.54/UComp/__init__.py
+-rw-rw-rw-   0        0        0    16507 2023-06-09 15:01:03.000000 UComp-1.0.54/UComp/airpas.bin
+-rw-rw-rw-   0        0        0     3645 2023-06-09 15:01:03.000000 UComp-1.0.54/UComp/gdp.bin
+-rw-rw-rw-   0        0        0    14731 2023-06-09 15:01:03.000000 UComp-1.0.54/UComp/ipi.bin
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.54/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    29759 2023-06-14 08:05:48.000000 UComp-1.0.54/UComp/tools.py
+-rw-rw-rw-   0        0        0      570 2023-06-09 15:36:47.000000 UComp-1.0.54/UComp/tsfile.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:07:12.053126 UComp-1.0.54/UComp.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-06-14 08:07:11.000000 UComp-1.0.54/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-14 08:07:11.000000 UComp-1.0.54/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 08:07:11.000000 UComp-1.0.54/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-14 08:07:11.000000 UComp-1.0.54/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 08:07:11.000000 UComp-1.0.54/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 08:07:12.053126 UComp-1.0.54/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-14 08:06:02.000000 UComp-1.0.54/setup.py
```

### Comparing `UComp-1.0.51/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.54/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.51/UComp/ETSmodule.py` & `UComp-1.0.54/UComp/ETSmodule.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,20 @@
         if not isinstance(self.y, np.ndarray):
             self.comp = tsfile.ts(self.comp, self.y.index[0], self.y.index.freq)
         self.table = ' '.join([str(i) for i in m1.table])
         if show:
             print(self.table)
 
 
+    def plot(self):
+        if any(self.comp.shape) == 0:
+            self.components(self)
+        self.comp.plot(subplots=True, layout=(len(self.comp.columns), 1), figsize=(10, 6), sharex=True)
+
+
 def ETS(y: np.array, s: int = np.nan, u: np.array = np.array([]), model: str = "???",
         h: int = 24, criterion: str = "aicc",
         armaIdent: bool = False, identAll: bool = False, forIntervals: bool = False,
         bootstrap: bool = False, nSimul: int = 5000, verbose: bool = False,
         alphaL: np.array = np.array([0, 1]), betaL: np.array = np.array([0, 1]),
         gammaL: np.array = np.array([0, 1]), phiL: np.array = np.array([0.8, 0.98]),
         p0: np.array = np.array([-99999]), lambdaBoxCox: np.array = np.array(1.0)):
```

### Comparing `UComp-1.0.51/UComp/PTSmodule.py` & `UComp-1.0.54/UComp/PTSmodule.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,14 +236,20 @@
         #     if m['comp'].shape[1] == 3:
         #         m['comp'].iloc[:, 1] = m['comp'].iloc[:, 2]
         #     else:
         #         m['comp'].iloc[:, 1] = m['comp'].iloc[:, 3:].sum(axis=1)
         #     self.comp.columns = ["Error", "Fit"] + list(names[ind])
 
 
+    def plot(self):
+        if any(self.comp.shape) == 0:
+            self.components(self)
+        self.comp.plot(subplots=True, layout=(len(self.comp.columns), 1), figsize=(10, 6), sharex=True)
+
+
 def PTS(y: pd.DataFrame, s: int = np.nan, u: np.array = np.array([]), model: str = "???",
                  h: int = 9999, criterion: str="aicc", lambdaBoxCox: np.array = np.array(1.0), armaIdent: bool=False,
                  verbose: bool = False):
     """
     Run PTS general univariate MSOE models
 
     Inputs:
```

### Comparing `UComp-1.0.51/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.54/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.51/UComp/UCmodule.py` & `UComp-1.0.54/UComp/UCmodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,14 +338,20 @@
         else:
             self.v = tsfile.ts(np.array(m1.v), self.y.index[0], self.y.index.freq)
         if show:
             print(self.table)
         return self
 
 
+    def plot(self):
+        if any(self.comp.shape) == 0:
+            self.components(self)
+        self.comp.plot(subplots=True, layout=(len(self.comp.columns), 1), figsize=(10, 6), sharex=True)
+
+
     def filter_(self, smooth: str):
         u = self.u
         if u.size == 0:
             u = np.array([-99999])
             rowu = 0
             colu = 0
         else:
```

### Comparing `UComp-1.0.51/UComp/airpas.bin` & `UComp-1.0.54/UComp/airpas.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.51/UComp/gdp.bin` & `UComp-1.0.54/UComp/gdp.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.51/UComp/ipi.bin` & `UComp-1.0.54/UComp/ipi.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.51/UComp/libopenblas.dll` & `UComp-1.0.54/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.51/UComp/tools.py` & `UComp-1.0.54/UComp/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,23 @@
 
 
 ipi = pd.read_pickle("ipi.bin")
 gdp = pd.read_pickle("gdp.bin")
 airpas = pd.read_pickle("airpas.bin")
 
 
+def window(y, start='', end=''):
+    if start == '':
+        start = y.index[0]
+    if end == '':
+        end = y.index[-1]
+    suby = y.loc[pd.to_datetime(start) : pd.to_datetime(end)]
+    return(suby)
+
+
 def obj2array(y):
     if isinstance(y, uc.UCmodel):
         x = y.v.values
     elif isinstance(y, ets.ETSmodel):
         x = y.comp[:, 0].values
     elif isinstance(y, pd.Series) or isinstance(y, pd.DataFrame):
         x = y.values
@@ -845,37 +854,38 @@
     ax2 = fig.add_subplot(2, 2, 3)
     ax3 = fig.add_subplot(2, 2, 4)
     out = ident(y, nCoef, nPar, True)
     plotAcfPacf(np.array(out["SACF"]), np.array(out["SPACF"]), s, len(y), [ax2, ax3])
     plt.show(block=False)
 
 
-def tests(x, parts=1/3, nCoef=None, nPar=0, avoid=16):
+def tests(y, parts=1/3, nCoef=None, nPar=0, avoid=16):
     """
     Tests on a time series
 
     y: a vector, ts or tsibble object
     parts: proportion of sample to include in ratio of variances test
     nCoef: number of autocorrelation coefficients to estimate
     nPar: number of parameters in a model if y is a residual
     s: seasonal period, number of observations per year
     avoid: number of observations to avoid at beginning of sample to eliminate initial effects
 
     Author: Diego J. Pedregal
     """
-    if isinstance(x, pd.Series) or isinstance(x, pd.DataFrame):
-        s = x.resample('Y').count()[1]
+    if isinstance(y, pd.Series) or isinstance(y, pd.DataFrame):
+        s = y.resample('Y').count()[1]
     else:
         s = 1
+    x = obj2array(y)
     print("Summary statistics:")
     print("===================")
     print(sumStats(x))
     print("Autocorrelation tests:")
     print("=====================")
-    nCoef = min(25, len(x) / 4)
+    nCoef = min(37, len(x) / 4)
     # Plot figure
     fig = plt.figure(figsize=(8, 6))
     ax1 = fig.add_subplot(4, 1, 1)
     ax1.plot(x)
     ax1.set_xlabel('Time')
     ax1.set_ylabel('Value')
     ax2 = fig.add_subplot(4, 2, 3)
```

### Comparing `UComp-1.0.51/UComp/tsfile.py` & `UComp-1.0.54/UComp/tsfile.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.51/setup.py` & `UComp-1.0.54/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.51',
+    version='1.0.54',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

