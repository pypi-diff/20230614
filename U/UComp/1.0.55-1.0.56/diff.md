# Comparing `tmp/UComp-1.0.55.tar.gz` & `tmp/UComp-1.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.55.tar", last modified: Wed Jun 14 08:44:10 2023, max compression
+gzip compressed data, was "UComp-1.0.56.tar", last modified: Wed Jun 14 11:03:15 2023, max compression
```

## Comparing `UComp-1.0.55.tar` & `UComp-1.0.56.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:44:10.051337 UComp-1.0.55/
--rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.55/MANIFEST.in
--rw-rw-rw-   0        0        0      343 2023-06-14 08:44:10.051337 UComp-1.0.55/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.55/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 08:44:10.020098 UComp-1.0.55/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.55/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.55/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0    11069 2023-06-14 07:44:36.000000 UComp-1.0.55/UComp/ETSmodule.py
--rw-rw-rw-   0        0        0    11794 2023-06-14 07:44:36.000000 UComp-1.0.55/UComp/PTSmodule.py
--rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.55/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.55/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    24546 2023-06-14 07:48:55.000000 UComp-1.0.55/UComp/UCmodule.py
--rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.55/UComp/__init__.py
--rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.55/UComp/airpas.bin
--rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.55/UComp/gdp.bin
--rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.55/UComp/ipi.bin
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.55/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    29759 2023-06-14 08:05:48.000000 UComp-1.0.55/UComp/tools.py
--rw-rw-rw-   0        0        0      570 2023-06-09 15:36:47.000000 UComp-1.0.55/UComp/tsfile.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:44:10.051337 UComp-1.0.55/UComp.egg-info/
--rw-rw-rw-   0        0        0      343 2023-06-14 08:44:09.000000 UComp-1.0.55/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-14 08:44:09.000000 UComp-1.0.55/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:44:09.000000 UComp-1.0.55/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-14 08:44:09.000000 UComp-1.0.55/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 08:44:09.000000 UComp-1.0.55/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 08:44:10.051337 UComp-1.0.55/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-14 08:44:00.000000 UComp-1.0.55/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:03:15.796759 UComp-1.0.56/
+-rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.56/MANIFEST.in
+-rw-rw-rw-   0        0        0      343 2023-06-14 11:03:15.797757 UComp-1.0.56/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.56/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 11:03:15.760818 UComp-1.0.56/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.56/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.56/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0    10981 2023-06-14 11:02:03.000000 UComp-1.0.56/UComp/ETSmodule.py
+-rw-rw-rw-   0        0        0    11794 2023-06-14 07:44:36.000000 UComp-1.0.56/UComp/PTSmodule.py
+-rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.56/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.56/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    24546 2023-06-14 07:48:55.000000 UComp-1.0.56/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.56/UComp/__init__.py
+-rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.56/UComp/airpas.bin
+-rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.56/UComp/gdp.bin
+-rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.56/UComp/ipi.bin
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.56/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    29759 2023-06-14 08:05:48.000000 UComp-1.0.56/UComp/tools.py
+-rw-rw-rw-   0        0        0      570 2023-06-09 15:36:47.000000 UComp-1.0.56/UComp/tsfile.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:03:15.793766 UComp-1.0.56/UComp.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-06-14 11:03:15.000000 UComp-1.0.56/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-14 11:03:15.000000 UComp-1.0.56/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 11:03:15.000000 UComp-1.0.56/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-14 11:03:15.000000 UComp-1.0.56/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 11:03:15.000000 UComp-1.0.56/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 11:03:15.800756 UComp-1.0.56/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-14 11:02:27.000000 UComp-1.0.56/setup.py
```

### Comparing `UComp-1.0.55/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.56/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.55/UComp/ETSmodule.py` & `UComp-1.0.56/UComp/ETSmodule.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,21 +142,29 @@
                 rowu, colu = u.shape
             if rowu > colu:
                 u = np.transpose(u)
                 rowu, colu = u.shape
         m1 = ETSc.ETSfunC("components", self.y, u.flatten(), rowu, colu, self.model, self.s, self.h, False,
                           self.criterion, self.identAll, self.alphaL, self.betaL, self.gammaL, self.phiL,
                           "standard", False, False, 0, np.array([0, 0]), self.armaIdent, self.p0, self.lambdaBoxCox)
-        self.compNames = m1.compNames
-        nComp = m1.compNames.count('/') + 1
+        self.v = np.array(m1.v)
         self.comp = np.array(m1.comp)
-        self.comp = np.transpose(self.comp.reshape((nComp, len(self.comp) // nComp)))
-        self.comp = tsfile.ts(self.comp, self.y.index[0], self.y.index.freq)
+        self.comp = np.reshape(self.comp, (np.floor_divide(self.comp.size, m1.rowcomp), m1.rowcomp))
+        if m1.compNames[-1] == "/":
+            names = m1.compNames[:-1]
+        else:
+            names = m1.compNames
+        names = names.split("/")
         if not isinstance(self.y, np.ndarray):
+            self.v = tsfile.ts(np.array(m1.v), self.y.index[0], self.y.index.freq)
             self.comp = tsfile.ts(self.comp, self.y.index[0], self.y.index.freq)
+            self.comp.columns = names
+        else:
+            dt = [(nombre, self.comp.dtype) for nombre in names]
+            self.comp = self.comp.view(dtype=dt)
 
 
     def validate(self, show=True):
         u = self.u
         if u.size == 0:
             u = np.array([-99999])
             rowu = 0
@@ -169,21 +177,15 @@
                 rowu, colu = u.shape
             if rowu > colu:
                 u = np.transpose(u)
                 rowu, colu = u.shape
         m1 = ETSc.ETSfunC("validate", self.y, u.flatten(), rowu, colu, self.model, self.s, self.h, False,
                           self.criterion, self.identAll, self.alphaL, self.betaL, self.gammaL, self.phiL,
                           "standard", False, False, 0, np.array([0, 0]), self.armaIdent, self.p0, self.lambdaBoxCox)
-        self.compNames = m1.compNames
-        nComp = m1.compNames.count('/') + 1
-        self.comp = np.array(m1.comp)
-        self.comp = np.transpose(self.comp.reshape((nComp, len(self.comp) // nComp)))
-        self.comp = tsfile.ts(self.comp, self.y.index[0], self.y.index.freq)
-        if not isinstance(self.y, np.ndarray):
-            self.comp = tsfile.ts(self.comp, self.y.index[0], self.y.index.freq)
+        self.v = np.array(m1.v)
         self.table = ' '.join([str(i) for i in m1.table])
         if show:
             print(self.table)
 
 
     def plot(self):
         if any(self.comp.shape) == 0:
```

### Comparing `UComp-1.0.55/UComp/PTSmodule.py` & `UComp-1.0.56/UComp/PTSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.55/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.56/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.55/UComp/UCmodule.py` & `UComp-1.0.56/UComp/UCmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.55/UComp/airpas.bin` & `UComp-1.0.56/UComp/airpas.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.55/UComp/gdp.bin` & `UComp-1.0.56/UComp/gdp.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.55/UComp/ipi.bin` & `UComp-1.0.56/UComp/ipi.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.55/UComp/libopenblas.dll` & `UComp-1.0.56/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.55/UComp/tools.py` & `UComp-1.0.56/UComp/tools.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.55/UComp/tsfile.py` & `UComp-1.0.56/UComp/tsfile.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.55/setup.py` & `UComp-1.0.56/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.55',
+    version='1.0.56',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

