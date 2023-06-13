# Comparing `tmp/CalibrationCurve-0.0.3.tar.gz` & `tmp/CalibrationCurve-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CalibrationCurve-0.0.3.tar", last modified: Tue Jun 13 02:03:05 2023, max compression
+gzip compressed data, was "CalibrationCurve-0.0.4.tar", last modified: Tue Jun 13 22:28:13 2023, max compression
```

## Comparing `CalibrationCurve-0.0.3.tar` & `CalibrationCurve-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 02:03:05.335766 CalibrationCurve-0.0.3/
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 02:03:05.335766 CalibrationCurve-0.0.3/CalibrationCurve/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-13 02:03:01.000000 CalibrationCurve-0.0.3/CalibrationCurve/__init__.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     4386 2023-06-13 02:03:01.000000 CalibrationCurve-0.0.3/CalibrationCurve/_modidx.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     3453 2023-06-13 02:03:01.000000 CalibrationCurve-0.0.3/CalibrationCurve/core.py
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 02:03:05.335766 CalibrationCurve-0.0.3/CalibrationCurve.egg-info/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1652 2023-06-13 02:03:05.000000 CalibrationCurve-0.0.3/CalibrationCurve.egg-info/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      414 2023-06-13 02:03:05.000000 CalibrationCurve-0.0.3/CalibrationCurve.egg-info/SOURCES.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-13 02:03:05.000000 CalibrationCurve-0.0.3/CalibrationCurve.egg-info/dependency_links.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       54 2023-06-13 02:03:05.000000 CalibrationCurve-0.0.3/CalibrationCurve.egg-info/entry_points.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-13 00:26:53.000000 CalibrationCurve-0.0.3/CalibrationCurve.egg-info/not-zip-safe
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       66 2023-06-13 02:03:05.000000 CalibrationCurve-0.0.3/CalibrationCurve.egg-info/requires.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       17 2023-06-13 02:03:05.000000 CalibrationCurve-0.0.3/CalibrationCurve.egg-info/top_level.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.3/LICENSE
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.3/MANIFEST.in
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1652 2023-06-13 02:03:05.335766 CalibrationCurve-0.0.3/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      787 2023-06-13 01:59:09.000000 CalibrationCurve-0.0.3/README.md
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1002 2023-06-13 02:03:01.000000 CalibrationCurve-0.0.3/settings.ini
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-13 02:03:05.335766 CalibrationCurve-0.0.3/setup.cfg
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.3/setup.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 22:28:13.616908 CalibrationCurve-0.0.4/
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 22:28:13.616908 CalibrationCurve-0.0.4/CalibrationCurve/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-13 22:28:06.000000 CalibrationCurve-0.0.4/CalibrationCurve/__init__.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     4137 2023-06-13 22:28:06.000000 CalibrationCurve-0.0.4/CalibrationCurve/_modidx.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     3072 2023-06-13 22:28:06.000000 CalibrationCurve-0.0.4/CalibrationCurve/core.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 22:28:13.616908 CalibrationCurve-0.0.4/CalibrationCurve.egg-info/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1652 2023-06-13 22:28:13.000000 CalibrationCurve-0.0.4/CalibrationCurve.egg-info/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      414 2023-06-13 22:28:13.000000 CalibrationCurve-0.0.4/CalibrationCurve.egg-info/SOURCES.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-13 22:28:13.000000 CalibrationCurve-0.0.4/CalibrationCurve.egg-info/dependency_links.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       54 2023-06-13 22:28:13.000000 CalibrationCurve-0.0.4/CalibrationCurve.egg-info/entry_points.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-13 00:26:53.000000 CalibrationCurve-0.0.4/CalibrationCurve.egg-info/not-zip-safe
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       62 2023-06-13 22:28:13.000000 CalibrationCurve-0.0.4/CalibrationCurve.egg-info/requires.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       17 2023-06-13 22:28:13.000000 CalibrationCurve-0.0.4/CalibrationCurve.egg-info/top_level.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.4/LICENSE
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.4/MANIFEST.in
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1652 2023-06-13 22:28:13.616908 CalibrationCurve-0.0.4/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      787 2023-06-13 01:59:09.000000 CalibrationCurve-0.0.4/README.md
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      998 2023-06-13 22:28:00.000000 CalibrationCurve-0.0.4/settings.ini
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-13 22:28:13.616908 CalibrationCurve-0.0.4/setup.cfg
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.4/setup.py
```

### Comparing `CalibrationCurve-0.0.3/CalibrationCurve/_modidx.py` & `CalibrationCurve-0.0.4/CalibrationCurve/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,11 +28,9 @@
                                                                                                'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.inverse_prediction': ( 'core.html#calibrationmodel.inverse_prediction',
                                                                                                       'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.load_data': ( 'core.html#calibrationmodel.load_data',
                                                                                              'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.plot_fit': ( 'core.html#calibrationmodel.plot_fit',
                                                                                             'CalibrationCurve/core.py'),
-                                       'CalibrationCurve.core.CalibrationModel.summary': ( 'core.html#calibrationmodel.summary',
-                                                                                           'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.tabulate_results': ( 'core.html#calibrationmodel.tabulate_results',
                                                                                                     'CalibrationCurve/core.py')}}}
```

### Comparing `CalibrationCurve-0.0.3/CalibrationCurve/core.py` & `CalibrationCurve-0.0.4/CalibrationCurve/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,96 +1,85 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
 __all__ = ['CalibrationModel']
 
 # %% ../nbs/00_core.ipynb 5
 class CalibrationModel:
-
-# TODO: think about adding replicates and no. of calibration points here or read it automatically from data
-
     def __init__(self, data, response_variable, test_replicates):
         self.raw_data = self.load_data(data)
         self.response_variable = response_variable
         self.fit = None
         self.test_replicates = test_replicates
         self.cal_line_points = self.raw_data.shape[0]
-        self.r2 = None 
+        self.r2 = None
 
     def load_data(self, data):
         if ".csv" in data:
             raw_data = pd.read_csv(data)
         else:
             raw_data = data
-
         return raw_data
 
-
-    
-
     def fit_ols(self):
-        self.fit = smf.ols(f"{self.response_variable} ~ concentration", data=self.raw_data).fit()
-        self.r2 = self.fit.rsquared
-        # print(self.fit.summary())
-        return self.fit 
-    
+        X = self.raw_data[["concentration"]]
+        y = self.raw_data[self.response_variable]
+        self.fit = LinearRegression().fit(X, y)
+        self.r2 = self.fit.score(X, y)
+        return self.fit
+
     def get_params(self):
-        slope = self.fit.params[1]
-        intercept = self.fit.params[0]
+        slope = self.fit.coef_[0]
+        intercept = self.fit.intercept_
         return slope, intercept
-    
+
     def get_r2(self):
-        return self.fit.rsquared
-    
+        return self.r2
+
     def inverse_prediction(self, unknown: float):
-        """Returns the concentration given the provided response variable."""
         slope, intercept = self.get_params()
-        return (unknown - intercept)/slope
-    
+        return (unknown - intercept) / slope
+
     def calculate_sse(self):
-        return np.sum((self.fit.fittedvalues - self.raw_data[self.response_variable]) **2)
-    
+        y_pred = self.fit.predict(self.raw_data[["concentration"]])
+        return np.sum((y_pred - self.raw_data[self.response_variable]) ** 2)
+
     def calculate_syx(self):
-        return np.sqrt((self.calculate_sse())/(len(self.raw_data)-2))
+        return np.sqrt((self.calculate_sse()) / (len(self.raw_data) - 2))
 
-    
-    def get_t_value(self,alpha):
-        return t.ppf(1 - alpha/2, self.fit.df_resid)
+    def get_t_value(self, alpha):
+        return t.ppf(1 - alpha / 2, len(self.raw_data) - 2)
 
     def calculate_uncertainty(self):
         return self.calculate_sxhat() * self.get_t_value(0.05)
-    
+
     def calculate_sxhat(self):
-        return (self.calculate_syx() / self.fit.params[1]) * np.sqrt(1/ self.test_replicates + self.cal_line_points) 
-    
+        return (self.calculate_syx() / self.fit.coef_[0]) * np.sqrt(1 / self.test_replicates + self.cal_line_points)
+
     def fit_model(self):
         self.fit_ols()
-        # self.plot_fit()
         self.get_params()
         self.get_r2()
         self.calculate_uncertainty()
         self.tabulate_results()
 
-    
     def plot_fit(self):
         sns.regplot(x="concentration", y=self.response_variable, data=self.raw_data)
         sns.despine()
         sns.set_context("paper")
         plt.title(f"Calibration curve of concentration versus {self.response_variable}")
-        plt.xlabel("Concentration") 
-        plt.ylabel('Peak Value')
-        plt.annotate(f"R-squared = {self.get_r2():.3f}", xy=(0.3, 0.8), xycoords='axes fraction', fontsize=9, ha='center', va='center')
-        plt.annotate(f"Regression formula: y = {self.get_params()[0]:.3f} * x + {self.get_params()[1]:.3f}", xy=(0.3, 0.7), xycoords='axes fraction', fontsize=9, ha='center', va='center')
-        plt.show()    
-
-    def summary(self):
-        """Provides a summary of the fitted model by plotting the data alongside the regression fit and printing the summary of the fit."""
-        self.plot_fit()
-        return self.fit.summary()
-    
+        plt.xlabel("Concentration")
+        plt.ylabel("Peak Value")
+        plt.annotate(f"R-squared = {self.get_r2():.3f}", xy=(0.3, 0.8), xycoords="axes fraction", fontsize=9,
+                     ha="center", va="center")
+        plt.annotate(f"Regression formula: y = {self.get_params()[0]:.3f} * x + {self.get_params()[1]:.3f}",
+                     xy=(0.3, 0.7), xycoords="axes fraction", fontsize=9, ha="center", va="center")
+        plt.show()
+
+
 
     def tabulate_results(self):
         print(f"Calibration curve of {self.response_variable} versus concentration")
         print(f"R2 = {self.r2}")
         print(f"Slope = {self.get_params()[0]}")
         print(f"Intercept = {self.get_params()[1]}")
         print(f"Uncertainity = {self.calculate_uncertainty()}")
```

### Comparing `CalibrationCurve-0.0.3/CalibrationCurve.egg-info/PKG-INFO` & `CalibrationCurve-0.0.4/CalibrationCurve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalibrationCurve
-Version: 0.0.3
+Version: 0.0.4
 Summary: A collection of functions that streamline the process of creating calibration curves using Python.
 Home-page: https://github.com/Rhys-McAlister/CalibrationCurve
 Author: Rhys McAlister
 Author-email: mcalisterrhys@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CalibrationCurve-0.0.3/LICENSE` & `CalibrationCurve-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CalibrationCurve-0.0.3/PKG-INFO` & `CalibrationCurve-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalibrationCurve
-Version: 0.0.3
+Version: 0.0.4
 Summary: A collection of functions that streamline the process of creating calibration curves using Python.
 Home-page: https://github.com/Rhys-McAlister/CalibrationCurve
 Author: Rhys McAlister
 Author-email: mcalisterrhys@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CalibrationCurve-0.0.3/README.md` & `CalibrationCurve-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `CalibrationCurve-0.0.3/settings.ini` & `CalibrationCurve-0.0.4/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = CalibrationCurve
 lib_name = CalibrationCurve
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = CalibrationCurve
 nbs_path = nbs
 recursive = True
@@ -22,15 +22,15 @@
 author_email = mcalisterrhys@gmail.com
 copyright = 2023 onwards, Rhys McAlister
 description = A collection of functions that streamline the process of creating calibration curves using Python.
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = Rhys-McAlister
-requirements = fastcore pandas statsmodels matplotlib numpy seaborn scipy
+requirements = fastcore pandas sklearn matplotlib numpy seaborn scipy
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
```

### Comparing `CalibrationCurve-0.0.3/setup.py` & `CalibrationCurve-0.0.4/setup.py`

 * *Files identical despite different names*

