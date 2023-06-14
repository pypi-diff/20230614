# Comparing `tmp/gpjax-0.6.5.tar.gz` & `tmp/gpjax-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpjax-0.6.5.tar", max compression
+gzip compressed data, was "gpjax-0.6.6.tar", max compression
```

## Comparing `gpjax-0.6.5.tar` & `gpjax-0.6.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    11357 2023-05-30 19:04:23.359578 gpjax-0.6.5/LICENSE
--rw-r--r--   0        0        0     7471 2023-06-07 20:24:44.026934 gpjax-0.6.5/README.md
--rw-r--r--   0        0        0     3030 2023-06-14 19:58:51.907494 gpjax-0.6.5/gpjax/__init__.py
--rw-r--r--   0        0        0     1068 2023-05-30 19:04:23.413913 gpjax-0.6.5/gpjax/base/__init__.py
--rw-r--r--   0        0        0    12487 2023-06-07 14:15:07.164032 gpjax-0.6.5/gpjax/base/module.py
--rw-r--r--   0        0        0     2271 2023-05-30 19:04:23.414167 gpjax-0.6.5/gpjax/base/param.py
--rw-r--r--   0        0        0     5078 2023-06-13 18:44:31.911756 gpjax-0.6.5/gpjax/citation.py
--rw-r--r--   0        0        0     3452 2023-05-30 19:04:23.414269 gpjax-0.6.5/gpjax/dataset.py
--rw-r--r--   0        0        0     8216 2023-06-07 20:24:44.031018 gpjax-0.6.5/gpjax/fit.py
--rw-r--r--   0        0        0     9121 2023-05-30 19:04:23.414517 gpjax-0.6.5/gpjax/gaussian_distribution.py
--rw-r--r--   0        0        0    29097 2023-06-07 20:24:44.031235 gpjax-0.6.5/gpjax/gps.py
--rw-r--r--   0        0        0     5701 2023-06-07 20:24:44.031598 gpjax-0.6.5/gpjax/integrators.py
--rw-r--r--   0        0        0     1815 2023-05-30 19:04:23.414985 gpjax-0.6.5/gpjax/kernels/__init__.py
--rw-r--r--   0        0        0       68 2023-05-30 19:04:23.415113 gpjax-0.6.5/gpjax/kernels/approximations/__init__.py
--rw-r--r--   0        0        0     3183 2023-05-30 19:04:23.415213 gpjax-0.6.5/gpjax/kernels/approximations/rff.py
--rw-r--r--   0        0        0     6680 2023-05-30 19:04:23.415334 gpjax-0.6.5/gpjax/kernels/base.py
--rw-r--r--   0        0        0     1379 2023-05-30 19:04:23.415474 gpjax-0.6.5/gpjax/kernels/computations/__init__.py
--rw-r--r--   0        0        0     2585 2023-05-30 19:04:23.415588 gpjax-0.6.5/gpjax/kernels/computations/base.py
--rw-r--r--   0        0        0     2478 2023-05-30 19:04:23.415673 gpjax-0.6.5/gpjax/kernels/computations/basis_functions.py
--rw-r--r--   0        0        0     2830 2023-05-30 19:04:23.415758 gpjax-0.6.5/gpjax/kernels/computations/constant_diagonal.py
--rw-r--r--   0        0        0     1661 2023-05-30 19:04:23.415841 gpjax-0.6.5/gpjax/kernels/computations/dense.py
--rw-r--r--   0        0        0     2383 2023-05-30 19:04:23.415926 gpjax-0.6.5/gpjax/kernels/computations/diagonal.py
--rw-r--r--   0        0        0     2165 2023-05-30 19:04:23.416024 gpjax-0.6.5/gpjax/kernels/computations/eigen.py
--rw-r--r--   0        0        0      790 2023-05-30 19:04:23.416154 gpjax-0.6.5/gpjax/kernels/non_euclidean/__init__.py
--rw-r--r--   0        0        0     3511 2023-05-30 19:04:23.416256 gpjax-0.6.5/gpjax/kernels/non_euclidean/graph.py
--rw-r--r--   0        0        0     1620 2023-05-30 19:04:23.416342 gpjax-0.6.5/gpjax/kernels/non_euclidean/utils.py
--rw-r--r--   0        0        0      930 2023-05-30 19:04:23.416456 gpjax-0.6.5/gpjax/kernels/nonstationary/__init__.py
--rw-r--r--   0        0        0     4078 2023-05-30 19:04:23.416567 gpjax-0.6.5/gpjax/kernels/nonstationary/arccosine.py
--rw-r--r--   0        0        0     2016 2023-05-30 19:04:23.416675 gpjax-0.6.5/gpjax/kernels/nonstationary/linear.py
--rw-r--r--   0        0        0     2384 2023-05-30 19:04:23.416805 gpjax-0.6.5/gpjax/kernels/nonstationary/polynomial.py
--rw-r--r--   0        0        0     1323 2023-05-30 19:04:23.416936 gpjax-0.6.5/gpjax/kernels/stationary/__init__.py
--rw-r--r--   0        0        0     2521 2023-05-30 19:04:23.417037 gpjax-0.6.5/gpjax/kernels/stationary/matern12.py
--rw-r--r--   0        0        0     2723 2023-05-30 19:04:23.417110 gpjax-0.6.5/gpjax/kernels/stationary/matern32.py
--rw-r--r--   0        0        0     2792 2023-05-30 19:04:23.417181 gpjax-0.6.5/gpjax/kernels/stationary/matern52.py
--rw-r--r--   0        0        0     2420 2023-05-30 19:04:23.417272 gpjax-0.6.5/gpjax/kernels/stationary/periodic.py
--rw-r--r--   0        0        0     2674 2023-06-07 20:24:44.031983 gpjax-0.6.5/gpjax/kernels/stationary/powered_exponential.py
--rw-r--r--   0        0        0     2389 2023-05-30 19:04:23.417470 gpjax-0.6.5/gpjax/kernels/stationary/rational_quadratic.py
--rw-r--r--   0        0        0     2440 2023-05-30 19:04:23.417547 gpjax-0.6.5/gpjax/kernels/stationary/rbf.py
--rw-r--r--   0        0        0     2226 2023-05-30 19:04:23.417639 gpjax-0.6.5/gpjax/kernels/stationary/utils.py
--rw-r--r--   0        0        0     2072 2023-05-30 19:04:23.417729 gpjax-0.6.5/gpjax/kernels/stationary/white.py
--rw-r--r--   0        0        0     8015 2023-06-09 06:53:24.626957 gpjax-0.6.5/gpjax/likelihoods.py
--rw-r--r--   0        0        0     1609 2023-05-30 19:04:23.417969 gpjax-0.6.5/gpjax/linops/__init__.py
--rw-r--r--   0        0        0     6259 2023-05-30 19:04:23.418078 gpjax-0.6.5/gpjax/linops/constant_diagonal_linear_operator.py
--rw-r--r--   0        0        0     6201 2023-05-30 19:04:23.418223 gpjax-0.6.5/gpjax/linops/dense_linear_operator.py
--rw-r--r--   0        0        0     7179 2023-05-30 19:04:23.418329 gpjax-0.6.5/gpjax/linops/diagonal_linear_operator.py
--rw-r--r--   0        0        0     3607 2023-05-30 19:04:23.418426 gpjax-0.6.5/gpjax/linops/identity_linear_operator.py
--rw-r--r--   0        0        0     7131 2023-05-30 19:04:23.418534 gpjax-0.6.5/gpjax/linops/linear_operator.py
--rw-r--r--   0        0        0     3187 2023-05-30 19:04:23.418674 gpjax-0.6.5/gpjax/linops/triangular_linear_operator.py
--rw-r--r--   0        0        0     3443 2023-05-30 19:04:23.418772 gpjax-0.6.5/gpjax/linops/utils.py
--rw-r--r--   0        0        0     5939 2023-05-30 19:04:23.418880 gpjax-0.6.5/gpjax/linops/zero_linear_operator.py
--rw-r--r--   0        0        0     6081 2023-05-30 19:04:23.418977 gpjax-0.6.5/gpjax/mean_functions.py
--rw-r--r--   0        0        0    14868 2023-06-07 20:24:44.032504 gpjax-0.6.5/gpjax/objectives.py
--rw-r--r--   0        0        0     4407 2023-05-30 19:04:23.419266 gpjax-0.6.5/gpjax/progress_bar.py
--rw-r--r--   0        0        0     5506 2023-05-30 19:04:23.419458 gpjax-0.6.5/gpjax/scan.py
--rw-r--r--   0        0        0     1694 2023-05-30 19:04:23.419555 gpjax-0.6.5/gpjax/typing.py
--rw-r--r--   0        0        0    26453 2023-05-30 19:04:23.419787 gpjax-0.6.5/gpjax/variational_families.py
--rw-r--r--   0        0        0     5113 2023-06-14 19:59:22.063865 gpjax-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     8805 1970-01-01 00:00:00.000000 gpjax-0.6.5/setup.py
--rw-r--r--   0        0        0     8692 1970-01-01 00:00:00.000000 gpjax-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 19:04:23.359578 gpjax-0.6.6/LICENSE
+-rw-r--r--   0        0        0     7471 2023-06-07 20:24:44.026934 gpjax-0.6.6/README.md
+-rw-r--r--   0        0        0     3030 2023-06-14 20:05:19.097929 gpjax-0.6.6/gpjax/__init__.py
+-rw-r--r--   0        0        0     1068 2023-05-30 19:04:23.413913 gpjax-0.6.6/gpjax/base/__init__.py
+-rw-r--r--   0        0        0    12487 2023-06-07 14:15:07.164032 gpjax-0.6.6/gpjax/base/module.py
+-rw-r--r--   0        0        0     2271 2023-05-30 19:04:23.414167 gpjax-0.6.6/gpjax/base/param.py
+-rw-r--r--   0        0        0     5078 2023-06-13 18:44:31.911756 gpjax-0.6.6/gpjax/citation.py
+-rw-r--r--   0        0        0     3452 2023-05-30 19:04:23.414269 gpjax-0.6.6/gpjax/dataset.py
+-rw-r--r--   0        0        0     8216 2023-06-07 20:24:44.031018 gpjax-0.6.6/gpjax/fit.py
+-rw-r--r--   0        0        0     9121 2023-05-30 19:04:23.414517 gpjax-0.6.6/gpjax/gaussian_distribution.py
+-rw-r--r--   0        0        0    29097 2023-06-07 20:24:44.031235 gpjax-0.6.6/gpjax/gps.py
+-rw-r--r--   0        0        0     5701 2023-06-07 20:24:44.031598 gpjax-0.6.6/gpjax/integrators.py
+-rw-r--r--   0        0        0     1815 2023-05-30 19:04:23.414985 gpjax-0.6.6/gpjax/kernels/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-30 19:04:23.415113 gpjax-0.6.6/gpjax/kernels/approximations/__init__.py
+-rw-r--r--   0        0        0     3183 2023-05-30 19:04:23.415213 gpjax-0.6.6/gpjax/kernels/approximations/rff.py
+-rw-r--r--   0        0        0     6680 2023-05-30 19:04:23.415334 gpjax-0.6.6/gpjax/kernels/base.py
+-rw-r--r--   0        0        0     1379 2023-05-30 19:04:23.415474 gpjax-0.6.6/gpjax/kernels/computations/__init__.py
+-rw-r--r--   0        0        0     2585 2023-05-30 19:04:23.415588 gpjax-0.6.6/gpjax/kernels/computations/base.py
+-rw-r--r--   0        0        0     2478 2023-05-30 19:04:23.415673 gpjax-0.6.6/gpjax/kernels/computations/basis_functions.py
+-rw-r--r--   0        0        0     2830 2023-05-30 19:04:23.415758 gpjax-0.6.6/gpjax/kernels/computations/constant_diagonal.py
+-rw-r--r--   0        0        0     1661 2023-05-30 19:04:23.415841 gpjax-0.6.6/gpjax/kernels/computations/dense.py
+-rw-r--r--   0        0        0     2383 2023-05-30 19:04:23.415926 gpjax-0.6.6/gpjax/kernels/computations/diagonal.py
+-rw-r--r--   0        0        0     2165 2023-05-30 19:04:23.416024 gpjax-0.6.6/gpjax/kernels/computations/eigen.py
+-rw-r--r--   0        0        0      790 2023-05-30 19:04:23.416154 gpjax-0.6.6/gpjax/kernels/non_euclidean/__init__.py
+-rw-r--r--   0        0        0     3511 2023-05-30 19:04:23.416256 gpjax-0.6.6/gpjax/kernels/non_euclidean/graph.py
+-rw-r--r--   0        0        0     1620 2023-05-30 19:04:23.416342 gpjax-0.6.6/gpjax/kernels/non_euclidean/utils.py
+-rw-r--r--   0        0        0      930 2023-05-30 19:04:23.416456 gpjax-0.6.6/gpjax/kernels/nonstationary/__init__.py
+-rw-r--r--   0        0        0     4078 2023-05-30 19:04:23.416567 gpjax-0.6.6/gpjax/kernels/nonstationary/arccosine.py
+-rw-r--r--   0        0        0     2016 2023-05-30 19:04:23.416675 gpjax-0.6.6/gpjax/kernels/nonstationary/linear.py
+-rw-r--r--   0        0        0     2384 2023-05-30 19:04:23.416805 gpjax-0.6.6/gpjax/kernels/nonstationary/polynomial.py
+-rw-r--r--   0        0        0     1323 2023-05-30 19:04:23.416936 gpjax-0.6.6/gpjax/kernels/stationary/__init__.py
+-rw-r--r--   0        0        0     2521 2023-05-30 19:04:23.417037 gpjax-0.6.6/gpjax/kernels/stationary/matern12.py
+-rw-r--r--   0        0        0     2723 2023-05-30 19:04:23.417110 gpjax-0.6.6/gpjax/kernels/stationary/matern32.py
+-rw-r--r--   0        0        0     2792 2023-05-30 19:04:23.417181 gpjax-0.6.6/gpjax/kernels/stationary/matern52.py
+-rw-r--r--   0        0        0     2420 2023-05-30 19:04:23.417272 gpjax-0.6.6/gpjax/kernels/stationary/periodic.py
+-rw-r--r--   0        0        0     2674 2023-06-07 20:24:44.031983 gpjax-0.6.6/gpjax/kernels/stationary/powered_exponential.py
+-rw-r--r--   0        0        0     2389 2023-05-30 19:04:23.417470 gpjax-0.6.6/gpjax/kernels/stationary/rational_quadratic.py
+-rw-r--r--   0        0        0     2440 2023-05-30 19:04:23.417547 gpjax-0.6.6/gpjax/kernels/stationary/rbf.py
+-rw-r--r--   0        0        0     2226 2023-05-30 19:04:23.417639 gpjax-0.6.6/gpjax/kernels/stationary/utils.py
+-rw-r--r--   0        0        0     2072 2023-05-30 19:04:23.417729 gpjax-0.6.6/gpjax/kernels/stationary/white.py
+-rw-r--r--   0        0        0     8015 2023-06-09 06:53:24.626957 gpjax-0.6.6/gpjax/likelihoods.py
+-rw-r--r--   0        0        0     1609 2023-05-30 19:04:23.417969 gpjax-0.6.6/gpjax/linops/__init__.py
+-rw-r--r--   0        0        0     6259 2023-05-30 19:04:23.418078 gpjax-0.6.6/gpjax/linops/constant_diagonal_linear_operator.py
+-rw-r--r--   0        0        0     6201 2023-05-30 19:04:23.418223 gpjax-0.6.6/gpjax/linops/dense_linear_operator.py
+-rw-r--r--   0        0        0     7179 2023-05-30 19:04:23.418329 gpjax-0.6.6/gpjax/linops/diagonal_linear_operator.py
+-rw-r--r--   0        0        0     3607 2023-05-30 19:04:23.418426 gpjax-0.6.6/gpjax/linops/identity_linear_operator.py
+-rw-r--r--   0        0        0     7131 2023-05-30 19:04:23.418534 gpjax-0.6.6/gpjax/linops/linear_operator.py
+-rw-r--r--   0        0        0     3187 2023-05-30 19:04:23.418674 gpjax-0.6.6/gpjax/linops/triangular_linear_operator.py
+-rw-r--r--   0        0        0     3443 2023-05-30 19:04:23.418772 gpjax-0.6.6/gpjax/linops/utils.py
+-rw-r--r--   0        0        0     5939 2023-05-30 19:04:23.418880 gpjax-0.6.6/gpjax/linops/zero_linear_operator.py
+-rw-r--r--   0        0        0     6081 2023-05-30 19:04:23.418977 gpjax-0.6.6/gpjax/mean_functions.py
+-rw-r--r--   0        0        0    14868 2023-06-07 20:24:44.032504 gpjax-0.6.6/gpjax/objectives.py
+-rw-r--r--   0        0        0     4407 2023-05-30 19:04:23.419266 gpjax-0.6.6/gpjax/progress_bar.py
+-rw-r--r--   0        0        0     5506 2023-05-30 19:04:23.419458 gpjax-0.6.6/gpjax/scan.py
+-rw-r--r--   0        0        0     1694 2023-05-30 19:04:23.419555 gpjax-0.6.6/gpjax/typing.py
+-rw-r--r--   0        0        0    26453 2023-05-30 19:04:23.419787 gpjax-0.6.6/gpjax/variational_families.py
+-rw-r--r--   0        0        0     5113 2023-06-14 20:05:19.096551 gpjax-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     8805 1970-01-01 00:00:00.000000 gpjax-0.6.6/setup.py
+-rw-r--r--   0        0        0     8692 1970-01-01 00:00:00.000000 gpjax-0.6.6/PKG-INFO
```

### Comparing `gpjax-0.6.5/LICENSE` & `gpjax-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/README.md` & `gpjax-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/__init__.py` & `gpjax-0.6.6/gpjax/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     WhitenedVariationalGaussian,
 )
 
 __license__ = "MIT"
 __description__ = "Didactic Gaussian processes in JAX"
 __url__ = "https://github.com/JaxGaussianProcesses/GPJax"
 __contributors__ = "https://github.com/JaxGaussianProcesses/GPJax/graphs/contributors"
-__version__ = "0.0.0"
+__version__ = "0.6.6"
 
 __all__ = [
     "Module",
     "param_field",
     "cite",
     "kernels",
     "fit",
```

### Comparing `gpjax-0.6.5/gpjax/base/__init__.py` & `gpjax-0.6.6/gpjax/base/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/base/module.py` & `gpjax-0.6.6/gpjax/base/module.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/base/param.py` & `gpjax-0.6.6/gpjax/base/param.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/citation.py` & `gpjax-0.6.6/gpjax/citation.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/dataset.py` & `gpjax-0.6.6/gpjax/dataset.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/fit.py` & `gpjax-0.6.6/gpjax/fit.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/gaussian_distribution.py` & `gpjax-0.6.6/gpjax/gaussian_distribution.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/gps.py` & `gpjax-0.6.6/gpjax/gps.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/integrators.py` & `gpjax-0.6.6/gpjax/integrators.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/__init__.py` & `gpjax-0.6.6/gpjax/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/approximations/rff.py` & `gpjax-0.6.6/gpjax/kernels/approximations/rff.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/base.py` & `gpjax-0.6.6/gpjax/kernels/base.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/computations/__init__.py` & `gpjax-0.6.6/gpjax/kernels/computations/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/computations/base.py` & `gpjax-0.6.6/gpjax/kernels/computations/base.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/computations/basis_functions.py` & `gpjax-0.6.6/gpjax/kernels/computations/basis_functions.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/computations/constant_diagonal.py` & `gpjax-0.6.6/gpjax/kernels/computations/constant_diagonal.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/computations/dense.py` & `gpjax-0.6.6/gpjax/kernels/computations/dense.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/computations/diagonal.py` & `gpjax-0.6.6/gpjax/kernels/computations/diagonal.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/computations/eigen.py` & `gpjax-0.6.6/gpjax/kernels/computations/eigen.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/non_euclidean/__init__.py` & `gpjax-0.6.6/gpjax/kernels/non_euclidean/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/non_euclidean/graph.py` & `gpjax-0.6.6/gpjax/kernels/non_euclidean/graph.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/non_euclidean/utils.py` & `gpjax-0.6.6/gpjax/kernels/non_euclidean/utils.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/nonstationary/__init__.py` & `gpjax-0.6.6/gpjax/kernels/nonstationary/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/nonstationary/arccosine.py` & `gpjax-0.6.6/gpjax/kernels/nonstationary/arccosine.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/nonstationary/linear.py` & `gpjax-0.6.6/gpjax/kernels/nonstationary/linear.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/nonstationary/polynomial.py` & `gpjax-0.6.6/gpjax/kernels/nonstationary/polynomial.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/stationary/__init__.py` & `gpjax-0.6.6/gpjax/kernels/stationary/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/stationary/matern12.py` & `gpjax-0.6.6/gpjax/kernels/stationary/matern12.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/stationary/matern32.py` & `gpjax-0.6.6/gpjax/kernels/stationary/matern32.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/stationary/matern52.py` & `gpjax-0.6.6/gpjax/kernels/stationary/matern52.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/stationary/periodic.py` & `gpjax-0.6.6/gpjax/kernels/stationary/periodic.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/stationary/powered_exponential.py` & `gpjax-0.6.6/gpjax/kernels/stationary/powered_exponential.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/stationary/rational_quadratic.py` & `gpjax-0.6.6/gpjax/kernels/stationary/rational_quadratic.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/stationary/rbf.py` & `gpjax-0.6.6/gpjax/kernels/stationary/rbf.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/stationary/utils.py` & `gpjax-0.6.6/gpjax/kernels/stationary/utils.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/kernels/stationary/white.py` & `gpjax-0.6.6/gpjax/kernels/stationary/white.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/likelihoods.py` & `gpjax-0.6.6/gpjax/likelihoods.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/linops/__init__.py` & `gpjax-0.6.6/gpjax/linops/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/linops/constant_diagonal_linear_operator.py` & `gpjax-0.6.6/gpjax/linops/constant_diagonal_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/linops/dense_linear_operator.py` & `gpjax-0.6.6/gpjax/linops/dense_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/linops/diagonal_linear_operator.py` & `gpjax-0.6.6/gpjax/linops/diagonal_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/linops/identity_linear_operator.py` & `gpjax-0.6.6/gpjax/linops/identity_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/linops/linear_operator.py` & `gpjax-0.6.6/gpjax/linops/linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/linops/triangular_linear_operator.py` & `gpjax-0.6.6/gpjax/linops/triangular_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/linops/utils.py` & `gpjax-0.6.6/gpjax/linops/utils.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/linops/zero_linear_operator.py` & `gpjax-0.6.6/gpjax/linops/zero_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/mean_functions.py` & `gpjax-0.6.6/gpjax/mean_functions.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/objectives.py` & `gpjax-0.6.6/gpjax/objectives.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/progress_bar.py` & `gpjax-0.6.6/gpjax/progress_bar.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/scan.py` & `gpjax-0.6.6/gpjax/scan.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/typing.py` & `gpjax-0.6.6/gpjax/typing.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/gpjax/variational_families.py` & `gpjax-0.6.6/gpjax/variational_families.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.5/pyproject.toml` & `gpjax-0.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpjax"
-version = "0.6.5" # Merely a placeholder, will be replaced by the dynamic versioning plugin
+version = "0.6.6" # Merely a placeholder, will be replaced by the dynamic versioning plugin
 description = "Gaussian processes in JAX."
 authors = ["Thomas Pinder <tompinder@live.co.uk>", "Daniel Dodd <daniel_dodd@icloud.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/JaxGaussianProcesses/GPJax"
 repository = "https://github.com/JaxGaussianProcesses/GPJax"
 include = [
@@ -191,11 +191,11 @@
 output = "reports/coverage.xml"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 
 [tool.poetry-dynamic-versioning.substitution]
-files = ["dowhy/__init__.py"]
+files = ["gpjax/__init__.py"]
 
 [tool.codespell]
 ignore-words-list = "fro" # Frobenius
```

### Comparing `gpjax-0.6.5/setup.py` & `gpjax-0.6.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'plum-dispatch>=2.1.0,<3.0.0',
  'simple-pytree>=0.1.7,<0.2.0',
  'tensorflow-probability>=0.19.0,<0.20.0',
  'tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'gpjax',
-    'version': '0.6.5',
+    'version': '0.6.6',
     'description': 'Gaussian processes in JAX.',
     'long_description': '<!-- <h1 align=\'center\'>GPJax</h1>\n<h2 align=\'center\'>Gaussian processes in Jax.</h2> -->\n<p align="center">\n<img width="700" height="300" src="https://raw.githubusercontent.com/JaxGaussianProcesses/GPJax/main/docs/_static/gpjax_logo.svg" alt="GPJax\'s logo">\n</p>\n\n[![codecov](https://codecov.io/gh/JaxGaussianProcesses/GPJax/branch/master/graph/badge.svg?token=DM1DRDASU2)](https://codecov.io/gh/JaxGaussianProcesses/GPJax)\n[![CodeFactor](https://www.codefactor.io/repository/github/jaxgaussianprocesses/gpjax/badge)](https://www.codefactor.io/repository/github/jaxgaussianprocesses/gpjax)\n[![Netlify Status](https://api.netlify.com/api/v1/badges/d3950e6f-321f-4508-9e52-426b5dae2715/deploy-status)](https://app.netlify.com/sites/endearing-crepe-c2d5fe/deploys)\n[![PyPI version](https://badge.fury.io/py/GPJax.svg)](https://badge.fury.io/py/GPJax)\n[![DOI](https://joss.theoj.org/papers/10.21105/joss.04455/status.svg)](https://doi.org/10.21105/joss.04455)\n[![Downloads](https://pepy.tech/badge/gpjax)](https://pepy.tech/project/gpjax)\n[![Slack Invite](https://img.shields.io/badge/Slack_Invite--blue?style=social&logo=slack)](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)\n\n[**Quickstart**](#simple-example)\n| [**Install guide**](#installation)\n| [**Documentation**](https://docs.jaxgaussianprocesses.com/)\n| [**Slack Community**](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)\n\nGPJax aims to provide a low-level interface to Gaussian process (GP) models in\n[Jax](https://github.com/google/jax), structured to give researchers maximum\nflexibility in extending the code to suit their own needs. The idea is that the\ncode should be as close as possible to the maths we write on paper when working\nwith GP models.\n\n# Package support\n\nGPJax was founded by [Thomas Pinder](https://github.com/thomaspinder). Today,\nthe maintenance of GPJax is undertaken by [Thomas\nPinder](https://github.com/thomaspinder) and [Daniel\nDodd](https://github.com/Daniel-Dodd).\n\nWe would be delighted to receive contributions from interested individuals and\ngroups. To learn how you can get involved, please read our [guide for\ncontributing](https://github.com/JaxGaussianProcesses/GPJax/blob/master/CONTRIBUTING.md).\nIf you have any questions, we encourage you to [open an\nissue](https://github.com/JaxGaussianProcesses/GPJax/issues/new/choose). For\nbroader conversations, such as best GP fitting practices or questions about the\nmathematics of GPs, we invite you to [open a\ndiscussion](https://github.com/JaxGaussianProcesses/GPJax/discussions).\n\nFeel free to join our [Slack\nChannel](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw),\nwhere we can discuss the development of GPJax and broader support for Gaussian\nprocess modelling.\n\n# Supported methods and interfaces\n\n## Notebook examples\n\n> - [**Conjugate Inference**](https://docs.jaxgaussianprocesses.com/examples/regression/)\n> - [**Classification with MCMC**](https://docs.jaxgaussianprocesses.com/examples/classification/)\n> - [**Sparse Variational Inference**](https://docs.jaxgaussianprocesses.com/examples/collapsed_vi/)\n> - [**Stochastic Variational Inference**](https://docs.jaxgaussianprocesses.com/examples/uncollapsed_vi/)\n> - [**BlackJax Integration**](https://docs.jaxgaussianprocesses.com/examples/classification/#mcmc-inference)\n> - [**Laplace Approximation**](https://docs.jaxgaussianprocesses.com/examples/classification/#laplace-approximation)\n> - [**Inference on Non-Euclidean Spaces**](https://docs.jaxgaussianprocesses.com/examples/kernels/#custom-kernel)\n> - [**Inference on Graphs**](https://docs.jaxgaussianprocesses.com/examples/graph_kernels/)\n> - [**Pathwise Sampling**](https://docs.jaxgaussianprocesses.com/examples/spatial/)\n> - [**Learning Gaussian Process Barycentres**](https://docs.jaxgaussianprocesses.com/examples/barycentres/)\n> - [**Deep Kernel Regression**](https://docs.jaxgaussianprocesses.com/examples/deep_kernels/)\n> - [**Poisson Regression**](https://docs.jaxgaussianprocesses.com/examples/poisson/)\n\n## Guides for customisation\n>\n> - [**Custom kernels**](https://docs.jaxgaussianprocesses.com/examples/kernels/#custom-kernel)\n> - [**UCI regression**](https://docs.jaxgaussianprocesses.com/examples/yacht/)\n\n## Conversion between `.ipynb` and `.py`\nAbove examples are stored in [examples](examples) directory in the double\npercent (`py:percent`) format. Checkout [jupytext\nusing-cli](https://jupytext.readthedocs.io/en/latest/using-cli.html) for more\ninfo.\n\n* To convert `example.py` to `example.ipynb`, run:\n\n```bash\njupytext --to notebook example.py\n```\n\n* To convert `example.ipynb` to `example.py`, run:\n\n```bash\njupytext --to py:percent example.ipynb\n```\n\n# Simple example\n\nLet us import some dependencies and simulate a toy dataset $\\mathcal{D}$.\n\n```python\nimport gpjax as gpx\nfrom jax import grad, jit\nimport jax.numpy as jnp\nimport jax.random as jr\nimport optax as ox\n\nkey = jr.PRNGKey(123)\n\nf = lambda x: 10 * jnp.sin(x)\n\nn = 50\nx = jr.uniform(key=key, minval=-3.0, maxval=3.0, shape=(n,1)).sort()\ny = f(x) + jr.normal(key, shape=(n,1))\nD = gpx.Dataset(X=x, y=y)\n\n# Construct the prior\nmeanf = gpx.mean_functions.Zero()\nkernel = gpx.kernels.RBF()\nprior = gpx.Prior(mean_function=meanf, kernel = kernel)\n\n# Define a likelihood\nlikelihood = gpx.Gaussian(num_datapoints = n)\n\n# Construct the posterior\nposterior = prior * likelihood\n\n# Define an optimiser\noptimiser = ox.adam(learning_rate=1e-2)\n\n# Define the marginal log-likelihood\nnegative_mll = jit(gpx.objectives.ConjugateMLL(negative=True))\n\n# Obtain Type 2 MLEs of the hyperparameters\nopt_posterior, history = gpx.fit(\n    model=posterior,\n    objective=negative_mll,\n    train_data=D,\n    optim=optimiser,\n    num_iters=500,\n    safe=True,\n    key=key,\n)\n\n# Infer the predictive posterior distribution\nxtest = jnp.linspace(-3., 3., 100).reshape(-1, 1)\nlatent_dist = opt_posterior(xtest, D)\npredictive_dist = opt_posterior.likelihood(latent_dist)\n\n# Obtain the predictive mean and standard deviation\npred_mean = predictive_dist.mean()\npred_std = predictive_dist.stddev()\n```\n\n# Installation\n\n## Stable version\n\nThe latest stable version of GPJax can be installed via\npip:\n\n```bash\npip install gpjax\n```\n\n> **Note**\n>\n> We recommend you check your installation version:\n> ```python\n> python -c \'import gpjax; print(gpjax.__version__)\'\n> ```\n\n\n\n## Development version\n> **Warning**\n>\n> This version is possibly unstable and may contain bugs.\n\n> **Note**\n>\n> We advise you create virtual environment before installing:\n> ```\n> conda create -n gpjax_experimental python=3.10.0\n> conda activate gpjax_experimental\n>  ```\n\n\nClone a copy of the repository to your local machine and run the setup\nconfiguration in development mode.\n```bash\ngit clone https://github.com/JaxGaussianProcesses/GPJax.git\ncd GPJax\npoetry install\n```\n\n> We recommend you check your installation passes the supplied unit tests:\n>\n> ```python\n> poetry run pytest\n> ```\n\n# Citing GPJax\n\nIf you use GPJax in your research, please cite our [JOSS paper](https://joss.theoj.org/papers/10.21105/joss.04455#).\n\n```\n@article{Pinder2022,\n  doi = {10.21105/joss.04455},\n  url = {https://doi.org/10.21105/joss.04455},\n  year = {2022},\n  publisher = {The Open Journal},\n  volume = {7},\n  number = {75},\n  pages = {4455},\n  author = {Thomas Pinder and Daniel Dodd},\n  title = {GPJax: A Gaussian Process Framework in JAX},\n  journal = {Journal of Open Source Software}\n}\n```\n',
     'author': 'Thomas Pinder',
     'author_email': 'tompinder@live.co.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/JaxGaussianProcesses/GPJax',
```

### Comparing `gpjax-0.6.5/PKG-INFO` & `gpjax-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpjax
-Version: 0.6.5
+Version: 0.6.6
 Summary: Gaussian processes in JAX.
 Home-page: https://github.com/JaxGaussianProcesses/GPJax
 License: Apache-2.0
 Keywords: gaussian-processes jax machine-learning bayesian
 Author: Thomas Pinder
 Author-email: tompinder@live.co.uk
 Requires-Python: >=3.8,<3.12
```

