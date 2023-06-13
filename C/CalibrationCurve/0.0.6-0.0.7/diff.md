# Comparing `tmp/CalibrationCurve-0.0.6.tar.gz` & `tmp/CalibrationCurve-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CalibrationCurve-0.0.6.tar", last modified: Tue Jun 13 22:39:53 2023, max compression
+gzip compressed data, was "CalibrationCurve-0.0.7.tar", last modified: Tue Jun 13 23:06:37 2023, max compression
```

## Comparing `CalibrationCurve-0.0.6.tar` & `CalibrationCurve-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 22:39:53.014593 CalibrationCurve-0.0.6/
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 22:39:53.014593 CalibrationCurve-0.0.6/CalibrationCurve/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-13 22:39:48.000000 CalibrationCurve-0.0.6/CalibrationCurve/__init__.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     4137 2023-06-13 22:39:48.000000 CalibrationCurve-0.0.6/CalibrationCurve/_modidx.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     3072 2023-06-13 22:39:48.000000 CalibrationCurve-0.0.6/CalibrationCurve/core.py
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 22:39:53.014593 CalibrationCurve-0.0.6/CalibrationCurve.egg-info/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1652 2023-06-13 22:39:52.000000 CalibrationCurve-0.0.6/CalibrationCurve.egg-info/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      414 2023-06-13 22:39:52.000000 CalibrationCurve-0.0.6/CalibrationCurve.egg-info/SOURCES.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-13 22:39:52.000000 CalibrationCurve-0.0.6/CalibrationCurve.egg-info/dependency_links.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       54 2023-06-13 22:39:52.000000 CalibrationCurve-0.0.6/CalibrationCurve.egg-info/entry_points.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-13 00:26:53.000000 CalibrationCurve-0.0.6/CalibrationCurve.egg-info/not-zip-safe
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       67 2023-06-13 22:39:52.000000 CalibrationCurve-0.0.6/CalibrationCurve.egg-info/requires.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       17 2023-06-13 22:39:52.000000 CalibrationCurve-0.0.6/CalibrationCurve.egg-info/top_level.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.6/LICENSE
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.6/MANIFEST.in
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1652 2023-06-13 22:39:53.014593 CalibrationCurve-0.0.6/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      787 2023-06-13 01:59:09.000000 CalibrationCurve-0.0.6/README.md
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1003 2023-06-13 22:39:48.000000 CalibrationCurve-0.0.6/settings.ini
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-13 22:39:53.014593 CalibrationCurve-0.0.6/setup.cfg
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.6/setup.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 23:06:37.319370 CalibrationCurve-0.0.7/
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 23:06:37.309370 CalibrationCurve-0.0.7/CalibrationCurve/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-13 23:06:30.000000 CalibrationCurve-0.0.7/CalibrationCurve/__init__.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     4137 2023-06-13 23:06:30.000000 CalibrationCurve-0.0.7/CalibrationCurve/_modidx.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     3088 2023-06-13 23:06:30.000000 CalibrationCurve-0.0.7/CalibrationCurve/core.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 23:06:37.319370 CalibrationCurve-0.0.7/CalibrationCurve.egg-info/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1652 2023-06-13 23:06:37.000000 CalibrationCurve-0.0.7/CalibrationCurve.egg-info/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      414 2023-06-13 23:06:37.000000 CalibrationCurve-0.0.7/CalibrationCurve.egg-info/SOURCES.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-13 23:06:37.000000 CalibrationCurve-0.0.7/CalibrationCurve.egg-info/dependency_links.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       54 2023-06-13 23:06:37.000000 CalibrationCurve-0.0.7/CalibrationCurve.egg-info/entry_points.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-13 00:26:53.000000 CalibrationCurve-0.0.7/CalibrationCurve.egg-info/not-zip-safe
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       67 2023-06-13 23:06:37.000000 CalibrationCurve-0.0.7/CalibrationCurve.egg-info/requires.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       17 2023-06-13 23:06:37.000000 CalibrationCurve-0.0.7/CalibrationCurve.egg-info/top_level.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.7/LICENSE
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.7/MANIFEST.in
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1652 2023-06-13 23:06:37.319370 CalibrationCurve-0.0.7/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      787 2023-06-13 01:59:09.000000 CalibrationCurve-0.0.7/README.md
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1003 2023-06-13 23:06:25.000000 CalibrationCurve-0.0.7/settings.ini
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-13 23:06:37.319370 CalibrationCurve-0.0.7/setup.cfg
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.7/setup.py
```

### Comparing `CalibrationCurve-0.0.6/CalibrationCurve/_modidx.py` & `CalibrationCurve-0.0.7/CalibrationCurve/_modidx.py`

 * *Files identical despite different names*

### Comparing `CalibrationCurve-0.0.6/CalibrationCurve/core.py` & `CalibrationCurve-0.0.7/CalibrationCurve/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
         else:
             raw_data = data
         return raw_data
 
     def fit_ols(self):
         X = self.raw_data[["concentration"]]
         y = self.raw_data[self.response_variable]
-        self.fit = LinearRegression().fit(X, y)
+        lr = LinearRegression
+        self.fit = lr().fit(X, y)
         self.r2 = self.fit.score(X, y)
         return self.fit
 
     def get_params(self):
         slope = self.fit.coef_[0]
         intercept = self.fit.intercept_
         return slope, intercept
```

### Comparing `CalibrationCurve-0.0.6/CalibrationCurve.egg-info/PKG-INFO` & `CalibrationCurve-0.0.7/CalibrationCurve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalibrationCurve
-Version: 0.0.6
+Version: 0.0.7
 Summary: A collection of functions that streamline the process of creating calibration curves using Python.
 Home-page: https://github.com/Rhys-McAlister/CalibrationCurve
 Author: Rhys McAlister
 Author-email: mcalisterrhys@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CalibrationCurve-0.0.6/LICENSE` & `CalibrationCurve-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `CalibrationCurve-0.0.6/PKG-INFO` & `CalibrationCurve-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalibrationCurve
-Version: 0.0.6
+Version: 0.0.7
 Summary: A collection of functions that streamline the process of creating calibration curves using Python.
 Home-page: https://github.com/Rhys-McAlister/CalibrationCurve
 Author: Rhys McAlister
 Author-email: mcalisterrhys@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CalibrationCurve-0.0.6/README.md` & `CalibrationCurve-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `CalibrationCurve-0.0.6/settings.ini` & `CalibrationCurve-0.0.7/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = CalibrationCurve
 lib_name = CalibrationCurve
-version = 0.0.6
+version = 0.0.7
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = CalibrationCurve
 nbs_path = nbs
 recursive = True
```

### Comparing `CalibrationCurve-0.0.6/setup.py` & `CalibrationCurve-0.0.7/setup.py`

 * *Files identical despite different names*

