# Comparing `tmp/hierts-0.4.tar.gz` & `tmp/hierts-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hierts-0.4.tar", last modified: Tue Jun 13 15:30:06 2023, max compression
+gzip compressed data, was "hierts-0.5.tar", last modified: Wed Jun 14 09:36:37 2023, max compression
```

## Comparing `hierts-0.4.tar` & `hierts-0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 15:30:06.516034 hierts-0.4/
--rw-rw-rw-   0        0        0    10983 2022-07-06 12:50:59.000000 hierts-0.4/LICENSE
--rw-rw-rw-   0        0        0    14643 2023-06-13 15:30:06.515034 hierts-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1589 2022-08-12 07:31:52.000000 hierts-0.4/README.md
--rw-rw-rw-   0        0        0      793 2023-06-13 15:25:44.000000 hierts-0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 15:30:06.516034 hierts-0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 15:30:06.487837 hierts-0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 15:30:06.493836 hierts-0.4/src/hierts/
--rw-rw-rw-   0        0        0      153 2022-07-06 07:17:40.000000 hierts-0.4/src/hierts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:30:06.514033 hierts-0.4/src/hierts/_old/
--rw-rw-rw-   0        0        0    17256 2022-07-11 17:10:06.000000 hierts-0.4/src/hierts/_old/reconciliation.py
--rw-rw-rw-   0        0        0    20363 2023-06-13 15:24:05.000000 hierts-0.4/src/hierts/reconciliation.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:30:06.513033 hierts-0.4/src/hierts.egg-info/
--rw-rw-rw-   0        0        0    14643 2023-06-13 15:30:06.000000 hierts-0.4/src/hierts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-13 15:30:06.000000 hierts-0.4/src/hierts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 15:30:06.000000 hierts-0.4/src/hierts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-13 15:30:06.000000 hierts-0.4/src/hierts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-13 15:30:06.000000 hierts-0.4/src/hierts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 09:36:37.900236 hierts-0.5/
+-rw-rw-rw-   0        0        0    10983 2022-07-06 12:50:59.000000 hierts-0.5/LICENSE
+-rw-rw-rw-   0        0        0    14643 2023-06-14 09:36:37.899237 hierts-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1589 2022-08-12 07:31:52.000000 hierts-0.5/README.md
+-rw-rw-rw-   0        0        0      793 2023-06-14 09:35:48.000000 hierts-0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 09:36:37.900236 hierts-0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 09:36:37.853236 hierts-0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 09:36:37.871234 hierts-0.5/src/hierts/
+-rw-rw-rw-   0        0        0      153 2022-07-06 07:17:40.000000 hierts-0.5/src/hierts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:36:37.898237 hierts-0.5/src/hierts/_old/
+-rw-rw-rw-   0        0        0    17256 2022-07-11 17:10:06.000000 hierts-0.5/src/hierts/_old/reconciliation.py
+-rw-rw-rw-   0        0        0    20363 2023-06-14 09:34:14.000000 hierts-0.5/src/hierts/reconciliation.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:36:37.897240 hierts-0.5/src/hierts.egg-info/
+-rw-rw-rw-   0        0        0    14643 2023-06-14 09:36:37.000000 hierts-0.5/src/hierts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-14 09:36:37.000000 hierts-0.5/src/hierts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 09:36:37.000000 hierts-0.5/src/hierts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-14 09:36:37.000000 hierts-0.5/src/hierts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-14 09:36:37.000000 hierts-0.5/src/hierts.egg-info/top_level.txt
```

### Comparing `hierts-0.4/LICENSE` & `hierts-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hierts-0.4/PKG-INFO` & `hierts-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hierts
-Version: 0.4
+Version: 0.5
 Summary: Hierarchical time series reconciliation
 Author-email: Olivier Sprangers <o.r.sprangers@uva.nl>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `hierts-0.4/README.md` & `hierts-0.5/README.md`

 * *Files identical despite different names*

### Comparing `hierts-0.4/pyproject.toml` & `hierts-0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hierts"
-version = "0.4"
+version = "0.5"
 authors = [
   { name="Olivier Sprangers", email="o.r.sprangers@uva.nl" },
 ]
 description = "Hierarchical time series reconciliation"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `hierts-0.4/src/hierts/_old/reconciliation.py` & `hierts-0.5/src/hierts/_old/reconciliation.py`

 * *Files identical despite different names*

### Comparing `hierts-0.4/src/hierts/reconciliation.py` & `hierts-0.5/src/hierts/reconciliation.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,20 +152,20 @@
     # the empirical correlation matrix and the off-diagonal sum of the squared 
     # empirical correlation matrix.
     emp_cov = np.zeros((n_timeseries, n_timeseries), dtype=np.float32)
     sum_var_emp_corr = np.float32(0)
     sum_sq_emp_corr = np.float32(-n_timeseries)
     factor_emp_corr = n_samples / (n_samples - 1)
     factor_var_emp_cor = n_samples / (n_samples - 1)**3
-    for i in range(n_timeseries):
+    for i in prange(n_timeseries):
         # Calculate standardized residuals
         X_i = (residuals[i] - residuals_mean[i]) 
         Xs_i = X_i / residuals_std[i]
         Xs_i_mean = np.mean(Xs_i)
-        for j in prange(n_timeseries):
+        for j in range(n_timeseries):
             # Calculate standardized residuals
             X_j = (residuals[j] - residuals_mean[j]) 
             Xs_j = X_j / residuals_std[j]
             Xs_j_mean = np.mean(Xs_j)
             # Empirical covariance
             emp_cov[i, j] = factor_emp_corr * np.mean(X_i * X_j)
             # Sum off-diagonal variance of empirical correlation
```

### Comparing `hierts-0.4/src/hierts.egg-info/PKG-INFO` & `hierts-0.5/src/hierts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hierts
-Version: 0.4
+Version: 0.5
 Summary: Hierarchical time series reconciliation
 Author-email: Olivier Sprangers <o.r.sprangers@uva.nl>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

