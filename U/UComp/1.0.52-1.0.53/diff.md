# Comparing `tmp/UComp-1.0.52.tar.gz` & `tmp/UComp-1.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.52.tar", last modified: Wed Jun 14 07:57:58 2023, max compression
+gzip compressed data, was "UComp-1.0.53.tar", last modified: Wed Jun 14 08:04:06 2023, max compression
```

## Comparing `UComp-1.0.52.tar` & `UComp-1.0.53.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 07:57:58.459736 UComp-1.0.52/
--rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.52/MANIFEST.in
--rw-rw-rw-   0        0        0      343 2023-06-14 07:57:58.459736 UComp-1.0.52/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.52/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 07:57:58.428494 UComp-1.0.52/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.52/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.52/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0    11069 2023-06-14 07:44:36.000000 UComp-1.0.52/UComp/ETSmodule.py
--rw-rw-rw-   0        0        0    11794 2023-06-14 07:44:36.000000 UComp-1.0.52/UComp/PTSmodule.py
--rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.52/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.52/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    24546 2023-06-14 07:48:55.000000 UComp-1.0.52/UComp/UCmodule.py
--rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.52/UComp/__init__.py
--rw-rw-rw-   0        0        0    16507 2023-06-09 15:01:03.000000 UComp-1.0.52/UComp/airpas.bin
--rw-rw-rw-   0        0        0     3645 2023-06-09 15:01:03.000000 UComp-1.0.52/UComp/gdp.bin
--rw-rw-rw-   0        0        0    14731 2023-06-09 15:01:03.000000 UComp-1.0.52/UComp/ipi.bin
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.52/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    29679 2023-06-14 07:52:36.000000 UComp-1.0.52/UComp/tools.py
--rw-rw-rw-   0        0        0      570 2023-06-09 15:36:47.000000 UComp-1.0.52/UComp/tsfile.py
-drwxrwxrwx   0        0        0        0 2023-06-14 07:57:58.459736 UComp-1.0.52/UComp.egg-info/
--rw-rw-rw-   0        0        0      343 2023-06-14 07:57:57.000000 UComp-1.0.52/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-14 07:57:57.000000 UComp-1.0.52/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 07:57:57.000000 UComp-1.0.52/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-14 07:57:57.000000 UComp-1.0.52/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 07:57:57.000000 UComp-1.0.52/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 07:57:58.475360 UComp-1.0.52/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-14 07:57:04.000000 UComp-1.0.52/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:04:06.859877 UComp-1.0.53/
+-rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.53/MANIFEST.in
+-rw-rw-rw-   0        0        0      343 2023-06-14 08:04:06.859877 UComp-1.0.53/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.53/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 08:04:06.822036 UComp-1.0.53/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.53/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.53/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0    11069 2023-06-14 07:44:36.000000 UComp-1.0.53/UComp/ETSmodule.py
+-rw-rw-rw-   0        0        0    11794 2023-06-14 07:44:36.000000 UComp-1.0.53/UComp/PTSmodule.py
+-rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.53/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.53/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    24546 2023-06-14 07:48:55.000000 UComp-1.0.53/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.53/UComp/__init__.py
+-rw-rw-rw-   0        0        0    16507 2023-06-09 15:01:03.000000 UComp-1.0.53/UComp/airpas.bin
+-rw-rw-rw-   0        0        0     3645 2023-06-09 15:01:03.000000 UComp-1.0.53/UComp/gdp.bin
+-rw-rw-rw-   0        0        0    14731 2023-06-09 15:01:03.000000 UComp-1.0.53/UComp/ipi.bin
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.53/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    29768 2023-06-14 08:02:34.000000 UComp-1.0.53/UComp/tools.py
+-rw-rw-rw-   0        0        0      570 2023-06-09 15:36:47.000000 UComp-1.0.53/UComp/tsfile.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:04:06.859877 UComp-1.0.53/UComp.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-06-14 08:04:06.000000 UComp-1.0.53/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-14 08:04:06.000000 UComp-1.0.53/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 08:04:06.000000 UComp-1.0.53/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-14 08:04:06.000000 UComp-1.0.53/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 08:04:06.000000 UComp-1.0.53/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 08:04:06.875459 UComp-1.0.53/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-14 08:03:52.000000 UComp-1.0.53/setup.py
```

### Comparing `UComp-1.0.52/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.53/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.52/UComp/ETSmodule.py` & `UComp-1.0.53/UComp/ETSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.52/UComp/PTSmodule.py` & `UComp-1.0.53/UComp/PTSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.52/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.53/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.52/UComp/UCmodule.py` & `UComp-1.0.53/UComp/UCmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.52/UComp/airpas.bin` & `UComp-1.0.53/UComp/airpas.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.52/UComp/gdp.bin` & `UComp-1.0.53/UComp/gdp.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.52/UComp/ipi.bin` & `UComp-1.0.53/UComp/ipi.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.52/UComp/libopenblas.dll` & `UComp-1.0.53/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.52/UComp/tools.py` & `UComp-1.0.53/UComp/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,21 @@
 
 
 ipi = pd.read_pickle("ipi.bin")
 gdp = pd.read_pickle("gdp.bin")
 airpas = pd.read_pickle("airpas.bin")
 
 
-def window(y, start=y.index[0], end=y.index[-1]):
-   suby = y.loc[pd.to_datetime(start) : pd.to_datetime(end)]
-   return(suby)
+def window(y, start='', end=y.index[-1]):
+    if start == '':
+        start = y.index[0]
+    if end == '':
+        end = y.index[-1]
+    suby = y.loc[pd.to_datetime(start) : pd.to_datetime(end)]
+    return(suby)
 
 
 def obj2array(y):
     if isinstance(y, uc.UCmodel):
         x = y.v.values
     elif isinstance(y, ets.ETSmodel):
         x = y.comp[:, 0].values
```

### Comparing `UComp-1.0.52/UComp/tsfile.py` & `UComp-1.0.53/UComp/tsfile.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.52/setup.py` & `UComp-1.0.53/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.52',
+    version='1.0.53',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

