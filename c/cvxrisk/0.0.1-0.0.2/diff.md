# Comparing `tmp/cvxrisk-0.0.1.tar.gz` & `tmp/cvxrisk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxrisk-0.0.1.tar", max compression
+gzip compressed data, was "cvxrisk-0.0.2.tar", max compression
```

## Comparing `cvxrisk-0.0.1.tar` & `cvxrisk-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11375 2023-06-09 13:36:45.699415 cvxrisk-0.0.1/LICENSE
--rw-r--r--   0        0        0      869 2023-06-09 13:36:45.699415 cvxrisk-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-09 13:36:45.703415 cvxrisk-0.0.1/cvx/risk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 13:36:45.703415 cvxrisk-0.0.1/cvx/risk/cvar/__init__.py
--rw-r--r--   0        0        0      705 2023-06-09 13:36:45.703415 cvxrisk-0.0.1/cvx/risk/cvar/cvar.py
--rw-r--r--   0        0        0        0 2023-06-09 13:36:45.703415 cvxrisk-0.0.1/cvx/risk/factor/__init__.py
--rw-r--r--   0        0        0      755 2023-06-09 13:36:45.703415 cvxrisk-0.0.1/cvx/risk/factor/_model.py
--rw-r--r--   0        0        0      498 2023-06-09 13:36:45.703415 cvxrisk-0.0.1/cvx/risk/factor/fundamental.py
--rw-r--r--   0        0        0        0 2023-06-09 13:36:45.703415 cvxrisk-0.0.1/cvx/risk/factor/linalg/__init__.py
--rw-r--r--   0        0        0      820 2023-06-09 13:36:45.703415 cvxrisk-0.0.1/cvx/risk/factor/linalg/pca.py
--rw-r--r--   0        0        0     1655 2023-06-09 13:36:45.703415 cvxrisk-0.0.1/cvx/risk/factor/timeseries.py
--rw-r--r--   0        0        0        0 2023-06-09 13:36:45.703415 cvxrisk-0.0.1/cvx/risk/factor/util/__init__.py
--rw-r--r--   0        0        0      343 2023-06-09 13:36:45.703415 cvxrisk-0.0.1/cvx/risk/model.py
--rw-r--r--   0        0        0        0 2023-06-09 13:36:45.703415 cvxrisk-0.0.1/cvx/risk/sample/__init__.py
--rw-r--r--   0        0        0      914 2023-06-09 13:36:45.703415 cvxrisk-0.0.1/cvx/risk/sample/sample.py
--rw-r--r--   0        0        0      602 2023-06-09 13:37:09.347934 cvxrisk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 cvxrisk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-06-14 05:23:32.191506 cvxrisk-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4855 2023-06-14 05:23:32.191506 cvxrisk-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/cvar/__init__.py
+-rw-r--r--   0        0        0      705 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/cvar/cvar.py
+-rw-r--r--   0        0        0      162 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/factor/__init__.py
+-rw-r--r--   0        0        0      755 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/factor/_model.py
+-rw-r--r--   0        0        0      498 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/factor/fundamental.py
+-rw-r--r--   0        0        0        0 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/factor/linalg/__init__.py
+-rw-r--r--   0        0        0      820 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/factor/linalg/pca.py
+-rw-r--r--   0        0        0     1655 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/factor/timeseries.py
+-rw-r--r--   0        0        0        0 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/factor/util/__init__.py
+-rw-r--r--   0        0        0      343 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/model.py
+-rw-r--r--   0        0        0      142 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/sample/__init__.py
+-rw-r--r--   0        0        0      914 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/sample/sample.py
+-rw-r--r--   0        0        0      581 2023-06-14 05:24:06.360278 cvxrisk-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5463 1970-01-01 00:00:00.000000 cvxrisk-0.0.2/PKG-INFO
```

### Comparing `cvxrisk-0.0.1/LICENSE` & `cvxrisk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.1/cvx/risk/cvar/cvar.py` & `cvxrisk-0.0.2/cvx/risk/cvar/cvar.py`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.1/cvx/risk/factor/_model.py` & `cvxrisk-0.0.2/cvx/risk/factor/_model.py`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.1/cvx/risk/factor/linalg/pca.py` & `cvxrisk-0.0.2/cvx/risk/factor/linalg/pca.py`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.1/cvx/risk/factor/timeseries.py` & `cvxrisk-0.0.2/cvx/risk/factor/timeseries.py`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.1/cvx/risk/sample/sample.py` & `cvxrisk-0.0.2/cvx/risk/sample/sample.py`

 * *Files identical despite different names*

