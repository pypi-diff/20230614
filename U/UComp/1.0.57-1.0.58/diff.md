# Comparing `tmp/UComp-1.0.57.tar.gz` & `tmp/UComp-1.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.57.tar", last modified: Wed Jun 14 11:20:49 2023, max compression
+gzip compressed data, was "UComp-1.0.58.tar", last modified: Wed Jun 14 11:29:54 2023, max compression
```

## Comparing `UComp-1.0.57.tar` & `UComp-1.0.58.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 11:20:49.322283 UComp-1.0.57/
--rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.57/MANIFEST.in
--rw-rw-rw-   0        0        0      343 2023-06-14 11:20:49.323323 UComp-1.0.57/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.57/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 11:20:49.268372 UComp-1.0.57/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.57/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.57/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0    11122 2023-06-14 11:14:57.000000 UComp-1.0.57/UComp/ETSmodule.py
--rw-rw-rw-   0        0        0    11794 2023-06-14 07:44:36.000000 UComp-1.0.57/UComp/PTSmodule.py
--rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.57/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.57/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    24546 2023-06-14 07:48:55.000000 UComp-1.0.57/UComp/UCmodule.py
--rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.57/UComp/__init__.py
--rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.57/UComp/airpas.bin
--rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.57/UComp/gdp.bin
--rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.57/UComp/ipi.bin
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.57/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    29782 2023-06-14 11:19:12.000000 UComp-1.0.57/UComp/tools.py
--rw-rw-rw-   0        0        0      570 2023-06-09 15:36:47.000000 UComp-1.0.57/UComp/tsfile.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:20:49.320331 UComp-1.0.57/UComp.egg-info/
--rw-rw-rw-   0        0        0      343 2023-06-14 11:20:48.000000 UComp-1.0.57/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-14 11:20:48.000000 UComp-1.0.57/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 11:20:48.000000 UComp-1.0.57/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-14 11:20:48.000000 UComp-1.0.57/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 11:20:48.000000 UComp-1.0.57/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 11:20:49.326330 UComp-1.0.57/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-14 11:20:43.000000 UComp-1.0.57/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:29:54.335226 UComp-1.0.58/
+-rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.58/MANIFEST.in
+-rw-rw-rw-   0        0        0      343 2023-06-14 11:29:54.335226 UComp-1.0.58/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.58/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 11:29:54.306284 UComp-1.0.58/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.58/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.58/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0    11285 2023-06-14 11:29:03.000000 UComp-1.0.58/UComp/ETSmodule.py
+-rw-rw-rw-   0        0        0    11794 2023-06-14 07:44:36.000000 UComp-1.0.58/UComp/PTSmodule.py
+-rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.58/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.58/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    24546 2023-06-14 07:48:55.000000 UComp-1.0.58/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.58/UComp/__init__.py
+-rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.58/UComp/airpas.bin
+-rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.58/UComp/gdp.bin
+-rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.58/UComp/ipi.bin
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.58/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    29782 2023-06-14 11:19:12.000000 UComp-1.0.58/UComp/tools.py
+-rw-rw-rw-   0        0        0      570 2023-06-09 15:36:47.000000 UComp-1.0.58/UComp/tsfile.py
+drwxrwxrwx   0        0        0        0 2023-06-14 11:29:54.333227 UComp-1.0.58/UComp.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-06-14 11:29:53.000000 UComp-1.0.58/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-14 11:29:53.000000 UComp-1.0.58/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 11:29:53.000000 UComp-1.0.58/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-14 11:29:53.000000 UComp-1.0.58/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 11:29:53.000000 UComp-1.0.58/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 11:29:54.338179 UComp-1.0.58/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-14 11:29:17.000000 UComp-1.0.58/setup.py
```

### Comparing `UComp-1.0.57/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.58/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.57/UComp/ETSmodule.py` & `UComp-1.0.58/UComp/ETSmodule.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,23 +143,21 @@
             if rowu > colu:
                 u = np.transpose(u)
                 rowu, colu = u.shape
         m1 = ETSc.ETSfunC("components", self.y, u.flatten(), rowu, colu, self.model, self.s, self.h, False,
                           self.criterion, self.identAll, self.alphaL, self.betaL, self.gammaL, self.phiL,
                           "standard", False, False, 0, np.array([0, 0]), self.armaIdent, self.p0, self.lambdaBoxCox)
         self.comp = np.array(m1.comp)
-        self.comp = np.reshape(self.comp, (np.floor_divide(self.comp.size, m1.rowcomp), m1.rowcomp))
         self.v = self.comp[:, 0]
         if m1.compNames[-1] == "/":
             names = m1.compNames[:-1]
         else:
             names = m1.compNames
         names = names.split("/")
         if not isinstance(self.y, np.ndarray):
-            self.v = tsfile.ts(np.array(m1.v), self.y.index[0], self.y.index.freq)
             self.comp = tsfile.ts(self.comp, self.y.index[0], self.y.index.freq)
             self.comp.columns = names
         else:
             dt = [(nombre, self.comp.dtype) for nombre in names]
             self.comp = self.comp.view(dtype=dt)
 
 
@@ -178,16 +176,26 @@
             if rowu > colu:
                 u = np.transpose(u)
                 rowu, colu = u.shape
         m1 = ETSc.ETSfunC("validate", self.y, u.flatten(), rowu, colu, self.model, self.s, self.h, False,
                           self.criterion, self.identAll, self.alphaL, self.betaL, self.gammaL, self.phiL,
                           "standard", False, False, 0, np.array([0, 0]), self.armaIdent, self.p0, self.lambdaBoxCox)
         self.comp = np.array(m1.comp)
-        self.comp = np.reshape(self.comp, (np.floor_divide(self.comp.size, m1.rowcomp), m1.rowcomp))
         self.v = self.comp[:, 0]
+        if m1.compNames[-1] == "/":
+            names = m1.compNames[:-1]
+        else:
+            names = m1.compNames
+        names = names.split("/")
+        if not isinstance(self.y, np.ndarray):
+            self.comp = tsfile.ts(self.comp, self.y.index[0], self.y.index.freq)
+            self.comp.columns = names
+        else:
+            dt = [(nombre, self.comp.dtype) for nombre in names]
+            self.comp = self.comp.view(dtype=dt)
         self.table = ' '.join([str(i) for i in m1.table])
         if show:
             print(self.table)
 
 
     def plot(self):
         if any(self.comp.shape) == 0:
```

### Comparing `UComp-1.0.57/UComp/PTSmodule.py` & `UComp-1.0.58/UComp/PTSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.57/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.58/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.57/UComp/UCmodule.py` & `UComp-1.0.58/UComp/UCmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.57/UComp/airpas.bin` & `UComp-1.0.58/UComp/airpas.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.57/UComp/gdp.bin` & `UComp-1.0.58/UComp/gdp.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.57/UComp/ipi.bin` & `UComp-1.0.58/UComp/ipi.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.57/UComp/libopenblas.dll` & `UComp-1.0.58/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.57/UComp/tools.py` & `UComp-1.0.58/UComp/tools.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.57/UComp/tsfile.py` & `UComp-1.0.58/UComp/tsfile.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.57/setup.py` & `UComp-1.0.58/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.57',
+    version='1.0.58',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

