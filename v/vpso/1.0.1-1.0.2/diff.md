# Comparing `tmp/vpso-1.0.1.tar.gz` & `tmp/vpso-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vpso-1.0.1.tar", last modified: Mon Jun 12 16:37:50 2023, max compression
+gzip compressed data, was "vpso-1.0.2.tar", last modified: Wed Jun 14 09:06:32 2023, max compression
```

## Comparing `vpso-1.0.1.tar` & `vpso-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 16:37:50.423300 vpso-1.0.1/
--rw-rw-rw-   0        0        0     1093 2023-06-06 07:34:41.000000 vpso-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3573 2023-06-12 16:37:50.421043 vpso-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2872 2023-06-11 14:02:36.000000 vpso-1.0.1/README.md
--rw-rw-rw-   0        0        0      975 2023-06-12 16:09:23.000000 vpso-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 16:37:50.423800 vpso-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-12 16:37:50.334618 vpso-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 16:37:50.383369 vpso-1.0.1/src/vpso/
--rw-rw-rw-   0        0        0       50 2023-06-06 08:52:06.000000 vpso-1.0.1/src/vpso/__init__.py
--rw-rw-rw-   0        0        0     5630 2023-06-12 15:35:37.000000 vpso-1.0.1/src/vpso/adaptation.py
--rw-rw-rw-   0        0        0     5419 2023-06-11 16:30:12.000000 vpso-1.0.1/src/vpso/ask_and_tell.py
--rw-rw-rw-   0        0        0     5099 2023-06-11 17:50:23.000000 vpso-1.0.1/src/vpso/initialization.py
--rw-rw-rw-   0        0        0     3470 2023-06-12 15:29:16.000000 vpso-1.0.1/src/vpso/jit.py
--rw-rw-rw-   0        0        0     4668 2023-06-11 16:30:12.000000 vpso-1.0.1/src/vpso/math.py
--rw-rw-rw-   0        0        0     3748 2023-06-11 16:30:12.000000 vpso-1.0.1/src/vpso/mutation.py
--rw-rw-rw-   0        0        0     3268 2023-06-11 16:30:12.000000 vpso-1.0.1/src/vpso/reparation.py
--rw-rw-rw-   0        0        0     5511 2023-06-12 15:47:43.000000 vpso-1.0.1/src/vpso/termination.py
--rw-rw-rw-   0        0        0      295 2023-06-12 15:05:01.000000 vpso-1.0.1/src/vpso/typing.py
--rw-rw-rw-   0        0        0     7929 2023-06-12 16:32:33.000000 vpso-1.0.1/src/vpso/vpso.py
-drwxrwxrwx   0        0        0        0 2023-06-12 16:37:50.399687 vpso-1.0.1/src/vpso.egg-info/
--rw-rw-rw-   0        0        0     3573 2023-06-12 16:37:50.000000 vpso-1.0.1/src/vpso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      569 2023-06-12 16:37:50.000000 vpso-1.0.1/src/vpso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 16:37:50.000000 vpso-1.0.1/src/vpso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-12 16:37:50.000000 vpso-1.0.1/src/vpso.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-12 16:37:50.000000 vpso-1.0.1/src/vpso.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 16:37:50.417580 vpso-1.0.1/tests/
--rw-rw-rw-   0        0        0     4314 2023-06-12 15:49:15.000000 vpso-1.0.1/tests/test_adaptation.py
--rw-rw-rw-   0        0        0     1201 2023-06-10 15:53:49.000000 vpso-1.0.1/tests/test_initialization.py
--rw-rw-rw-   0        0        0     2893 2023-06-10 15:56:08.000000 vpso-1.0.1/tests/test_math.py
--rw-rw-rw-   0        0        0     3669 2023-06-10 15:56:14.000000 vpso-1.0.1/tests/test_mutation.py
--rw-rw-rw-   0        0        0     2119 2023-06-12 15:53:52.000000 vpso-1.0.1/tests/test_numerical.py
--rw-rw-rw-   0        0        0     3211 2023-06-10 15:56:23.000000 vpso-1.0.1/tests/test_reparation.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:06:32.213582 vpso-1.0.2/
+-rw-rw-rw-   0        0        0     1093 2023-06-06 07:34:41.000000 vpso-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3575 2023-06-14 09:06:32.212581 vpso-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2872 2023-06-11 14:02:36.000000 vpso-1.0.2/README.md
+-rw-rw-rw-   0        0        0      977 2023-06-14 09:02:19.000000 vpso-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 09:06:32.213582 vpso-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 09:06:32.152070 vpso-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 09:06:32.178837 vpso-1.0.2/src/vpso/
+-rw-rw-rw-   0        0        0       50 2023-06-06 08:52:06.000000 vpso-1.0.2/src/vpso/__init__.py
+-rw-rw-rw-   0        0        0     5945 2023-06-13 22:13:58.000000 vpso-1.0.2/src/vpso/adaptation.py
+-rw-rw-rw-   0        0        0     5423 2023-06-13 20:32:15.000000 vpso-1.0.2/src/vpso/ask_and_tell.py
+-rw-rw-rw-   0        0        0     5149 2023-06-13 15:20:00.000000 vpso-1.0.2/src/vpso/initialization.py
+-rw-rw-rw-   0        0        0     4367 2023-06-13 22:06:07.000000 vpso-1.0.2/src/vpso/jit.py
+-rw-rw-rw-   0        0        0     6709 2023-06-13 22:05:05.000000 vpso-1.0.2/src/vpso/math.py
+-rw-rw-rw-   0        0        0     3752 2023-06-13 20:32:15.000000 vpso-1.0.2/src/vpso/mutation.py
+-rw-rw-rw-   0        0        0     3270 2023-06-13 20:32:15.000000 vpso-1.0.2/src/vpso/reparation.py
+-rw-rw-rw-   0        0        0     5513 2023-06-13 20:32:15.000000 vpso-1.0.2/src/vpso/termination.py
+-rw-rw-rw-   0        0        0      295 2023-06-12 15:05:01.000000 vpso-1.0.2/src/vpso/typing.py
+-rw-rw-rw-   0        0        0     7929 2023-06-13 15:19:02.000000 vpso-1.0.2/src/vpso/vpso.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:06:32.190663 vpso-1.0.2/src/vpso.egg-info/
+-rw-rw-rw-   0        0        0     3575 2023-06-14 09:06:32.000000 vpso-1.0.2/src/vpso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2023-06-14 09:06:32.000000 vpso-1.0.2/src/vpso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 09:06:32.000000 vpso-1.0.2/src/vpso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-14 09:06:32.000000 vpso-1.0.2/src/vpso.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-14 09:06:32.000000 vpso-1.0.2/src/vpso.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 09:06:32.210594 vpso-1.0.2/tests/
+-rw-rw-rw-   0        0        0     4314 2023-06-12 15:49:15.000000 vpso-1.0.2/tests/test_adaptation.py
+-rw-rw-rw-   0        0        0     1201 2023-06-10 15:53:49.000000 vpso-1.0.2/tests/test_initialization.py
+-rw-rw-rw-   0        0        0     3467 2023-06-13 22:08:14.000000 vpso-1.0.2/tests/test_math.py
+-rw-rw-rw-   0        0        0     3669 2023-06-10 15:56:14.000000 vpso-1.0.2/tests/test_mutation.py
+-rw-rw-rw-   0        0        0     2119 2023-06-13 20:45:53.000000 vpso-1.0.2/tests/test_numerical.py
+-rw-rw-rw-   0        0        0     3211 2023-06-10 15:56:23.000000 vpso-1.0.2/tests/test_reparation.py
```

### Comparing `vpso-1.0.1/LICENSE` & `vpso-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vpso-1.0.1/PKG-INFO` & `vpso-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vpso
-Version: 1.0.1
-Summary: Multiple Particle Swarm Optimization
+Version: 1.0.2
+Summary: Vectorized Particle Swarm Optimization
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/vectorized-particle-swarm
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/vectorized-particle-swarm/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vpso-1.0.1/README.md` & `vpso-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vpso-1.0.1/pyproject.toml` & `vpso-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vpso"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Filippo Airaldi", email="filippoairaldi@gmail.com" },
 ]
-description = "Multiple Particle Swarm Optimization"
+description = "Vectorized Particle Swarm Optimization"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "MIT" }
 classifiers = [
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
```

### Comparing `vpso-1.0.1/src/vpso/adaptation.py` & `vpso-1.0.2/src/vpso/adaptation.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 """
 
 import logging
 
 import numpy as np
 
 from vpso.jit import _int, jit
-from vpso.math import batch_cdist, batch_pdist, batch_squareform
+from vpso.math import batch_cdist_and_pdist
 from vpso.typing import Array1d, Array2d, Array3d
 
 
-@jit
+@jit()
 def adaptation_strategy(f: Array1d) -> Array2d:
     """Picks the adaptation strategy for each problem based on the ratio of average
     distances between particles and to the best particle.
 
     Parameters
     ----------
     f : 1d array
@@ -44,21 +44,25 @@
 
     deltas = np.where(f <= 23 / 30, [(1.0, -1.0)], deltas)  # S1
     deltas = np.where(f < 0.5, [(0.5, -0.5)], deltas)  # S2
     deltas = np.where(f < 7 / 30, [(0.5, 0.5)], deltas)  # S3
     return deltas
 
 
-@jit
+@jit()
 def perform_adaptation(
+    px: Array3d,
+    sx: Array3d,
     nvec: int,
+    swarmsize: int,
+    lb: Array3d,
+    ub: Array3d,
     w: Array3d,
     c1: Array3d,
     c2: Array3d,
-    stage: Array1d,
     np_random: np.random.Generator,
 ) -> tuple[Array3d, Array3d, Array3d]:
     """Performs the adaptation of the parameters `w`, `c1` and `c2` based on the
     stage of the algorithm.
 
     Parameters
     ----------
@@ -80,14 +84,26 @@
         Random number generator.
 
     Returns
     -------
     tuple of 3d arrays
         The newly adapted parameters `w`, `c1` and `c2`.
     """
+    domain = ub - lb
+    px_norm = px / domain
+    sx_norm = sx / domain
+    G_, D_ = batch_cdist_and_pdist(px_norm, sx_norm, "euclidean")
+    G = G_[:, :, 0].sum(1) / swarmsize
+    D = D_.sum(2) / (swarmsize - 1)
+    # NOTE: cannot run Dmin = D.min(1) and Dmax = D.max(1) in numba, so we use
+    # https://stackoverflow.com/a/71214489/19648688
+    Dmin = np.take_along_axis(D, D.argmin(1)[:, np.newaxis], 1)[:, 0]
+    Dmax = np.take_along_axis(D, D.argmax(1)[:, np.newaxis], 1)[:, 0]
+    stage = (G - Dmin) / (Dmax - Dmin + 1e-32)
+
     # adapt w
     w = (1 / (1 + 1.5 * np.exp(-2.6 * stage)))[:, np.newaxis, np.newaxis]
 
     # adapt c1 and c2
     deltas = adaptation_strategy(stage) * np_random.uniform(
         0.05, 0.1, size=(nvec, _int(1))
     )
@@ -144,23 +160,17 @@
         Logger object.
 
     Returns
     -------
     tuple of 3d arrays
         The newly adapted parameters `w`, `c1` and `c2`.
     """
-    domain = ub - lb
-    px_normalized = px / domain
-    sx_normalized = sx / domain
-    D = batch_squareform(batch_pdist(px_normalized)).sum(2) / (swarmsize - 1)
-    Dmin = D.min(1)
-    Dmax = D.max(1)
-    G = batch_cdist(px_normalized, sx_normalized).mean((1, 2))
-    stage = (G - Dmin) / (Dmax - Dmin + 1e-32)
-    w_new, c1_new, c2_new = perform_adaptation(nvec, w, c1, c2, stage, np_random)
+    w_new, c1_new, c2_new = perform_adaptation(
+        px, sx, nvec, swarmsize, lb, ub, w, c1, c2, np_random
+    )
 
     if logger.level <= logging.DEBUG:
         logger.debug(
             "adaptation: w ∈ [%e, %e], c1 ∈ [%e, %e], c2 ∈ [%e, %e]",
             w_new.min(),
             w_new.max(),
             c1_new.min(),
```

### Comparing `vpso-1.0.1/src/vpso/ask_and_tell.py` & `vpso-1.0.2/src/vpso/ask_and_tell.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from vpso.jit import jit
 from vpso.math import pso_equation
 from vpso.mutation import mutate
 from vpso.reparation import repair_out_of_bounds
 from vpso.typing import Array1d, Array2d, Array3d
 
 
-@jit
+@jit()
 def generate_offsprings(
     x: Array3d,
     px: Array3d,
     pf: Array2d,
     sx: Array3d,
     v: Array3d,
     v_max: Array3d,
@@ -83,15 +83,15 @@
         x, x_new, v_new, px, sx, v, v_max, lb, ub, w, c1, c2, repair_iters, np_random
     )
     if perturb_best:
         mutate(x_new, px, pf, lb, ub, nvec, dim, mutation_prob, np_random)
     return x_new, v_new
 
 
-@jit
+@jit()
 def advance_population(
     x: Array3d, f: Array2d, px: Array3d, pf: Array2d
 ) -> tuple[Array3d, Array2d]:
     """Advances the population by replacing the particles with better positions.
 
     Parameters
     ----------
```

### Comparing `vpso-1.0.1/src/vpso/initialization.py` & `vpso-1.0.2/src/vpso/initialization.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,16 +73,16 @@
 
     Returns
     -------
     tuple of 3d and 1d arrays
         Returns the `lb`, `ub`, `nvec`, `dim`, `max_velocity_rate`, `w`, `c1`, `c2`,
         `ftol`, `xtol`, and `patience`.
     """
-    lb = np.expand_dims(lb, 1)  # add swarm dimension
-    ub = np.expand_dims(ub, 1)  # add swarm dimension
+    lb = np.expand_dims(lb, 1).astype(float, copy=True)  # add swarm dimension
+    ub = np.expand_dims(ub, 1).astype(float, copy=True)  # add swarm dimension
     nvec, _, dim = lb.shape
     return (
         lb,
         ub,
         nvec,
         dim,
         _asarray(max_velocity_rate, nvec, float, 3),
```

### Comparing `vpso-1.0.1/src/vpso/math.py` & `vpso-1.0.2/src/vpso/math.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,77 @@
+from typing import Literal
+
 import numpy as np
-from scipy.spatial.distance import (
-    _copy_array_if_base_present,
-    _distance_pybind,
-    _distance_wrap,
-)
+from numba import prange
 
 from vpso.jit import jit
 from vpso.typing import Array2d, Array3d
 
 
+@jit()
+def cdist_func(
+    x: Array2d, y: Array2d, type: Literal["euclidean", "sqeuclidean"]
+) -> Array2d:
+    """Computes the distance matrix for 2D arrays `x` and `y`.
+
+    Parameters
+    ----------
+    x : 2d array
+        A 2D array of shape `(N, d)`.
+    y : 2d array
+        A 2D array of shape `(M, d)`.
+    type : {"euclidean", "sqeuclidean"}
+        Type of distance to compute.
+
+    Returns
+    -------
+    2d array
+        Distance matrix of shape `(N, M)` between each pair of entries in `x` and `y`.
+    """
+    x2_sum = np.square(x).sum(axis=1)
+    y2_sum = np.square(y).sum(axis=1)
+    xy_dot = np.dot(x, y.T)
+    D = np.maximum(x2_sum[:, np.newaxis] + y2_sum - 2 * xy_dot, 0.0)
+    if type == "euclidean":
+        return np.sqrt(D)
+    if type == "sqeuclidean":
+        return D
+    raise ValueError(f"unknown cdist type: {type}")
+
+
+@jit()
+def pdist_func(x: Array2d, type: Literal["euclidean", "sqeuclidean"]) -> Array2d:
+    """Computes the pairwise distance matrix of the elements in the 2D array `x`.
+
+    Parameters
+    ----------
+    x : 2d array
+        A 2D array of shape `(N, d)`.
+    type : {"euclidean", "sqeuclidean"}
+        Type of distance to compute.
+
+    Returns
+    -------
+    2d array
+        Symmetric distance matrix of shape `(N, N)` between each pair of entries in `x`.
+    """
+    x2_sum = np.square(x).sum(axis=1)
+    xx_dot = np.dot(x, x.T)
+    D = np.maximum(x2_sum[:, np.newaxis] + x2_sum - 2 * xx_dot, 0.0)
+    np.fill_diagonal(D, 0.0)
+    if type == "euclidean":
+        return np.sqrt(D)
+    if type == "sqeuclidean":
+        return D
+    raise ValueError(f"unknown pdist type: {type}")
+
+
+@jit(parallel=True)
 def batch_cdist(
-    X: Array3d, Y: Array3d, dist_func=_distance_pybind.cdist_euclidean
+    X: Array3d, Y: Array3d, type: Literal["euclidean", "sqeuclidean"]
 ) -> Array3d:
     """Computes the distance matrices for 3D arrays.
 
     Parameters
     ----------
     X : 3d array
         An array of shape `(N, M, d)`.
@@ -27,70 +84,80 @@
     Returns
     -------
     3d array
         Distance matrices between each of the `(M, d)` and `(K, d)` matrices, where `d`
         is assumed to be the axis over which the distance is computed. The output has
         thus shape (N, M, K).
     """
-    N = X.shape[0]
-    out = np.empty((N, X.shape[1], Y.shape[1]), dtype=X.dtype)
-    for i in range(N):
-        dist_func(X[i], Y[i], out=out[i])
+    B, N, _ = X.shape
+    out = np.empty((B, N, Y.shape[1]), dtype=X.dtype)
+    for i in prange(B):
+        out[i] = cdist_func(X[i], Y[i], type)
     return out
 
 
-def batch_pdist(X: Array3d, dist_func=_distance_pybind.pdist_euclidean) -> Array2d:
+@jit(parallel=True)
+def batch_pdist(X: Array3d, type: Literal["euclidean", "sqeuclidean"]) -> Array3d:
     """Computes the pairwise distance matrices for the entries of a 3D array.
 
     Parameters
     ----------
     X : 3d array
         An array of shape `(N, M, d)`.
     dist_func : callable, optional
         Distance function to use. By default, `scipy.spatial.distance.pdist_euclidean`
         is used. It must support the `out` argument.
 
     Returns
     -------
-    2d array
-        Distance matrix of shape `(N, M * (M - 1) / 2)` between each pair of entries of
+    3d array
+        Distance matrix of shape `(N, M, M)` between each pair of entries of
         the `(M, d)` matrices, where `d` is assumed to be the axis over which the
         distance is computed.
     """
-    N, M = X.shape[:2]
-    out = np.empty((N, (M - 1) * M // 2), dtype=X.dtype)
-    for i in range(N):
-        dist_func(X[i], out=out[i])
+    B, N, _ = X.shape
+    out = np.empty((B, N, N), dtype=X.dtype)
+    for i in prange(B):
+        out[i] = pdist_func(X[i], type)
     return out
 
 
-def batch_squareform(D: Array2d) -> Array2d:
-    """Converts a batch of pairwise distance matrices to distance matrices.
+@jit(parallel=True)
+def batch_cdist_and_pdist(
+    X: Array3d, Y: Array3d, type: Literal["euclidean", "sqeuclidean"]
+) -> tuple[Array3d, Array3d]:
+    """Computes the distance matrices between the 3D arrays `X` and `Y`, as well as the
+    pairwise distance matrices for the entries of `X`.
 
     Parameters
     ----------
-    D : 2d array
-        Pairwise distance matrices of shape `(N, M * (M - 1) / 2)`, i.e., as returned by
-        `batch_pdist` and not in square form.
+    X : 3d array
+        An array of shape `(N, M, d)`.
+    Y : 3d array
+        An array of shape `(N, K, d)`.
+    dist_func : callable, optional
+        Distance function to use. By default, `scipy.spatial.distance.cdist_euclidean`
+        is used. It must support the `out` argument.
 
     Returns
     -------
-    3d array
-        The same distance matrices but in square form, i.e., of shape `(N, M, M)`.
+    tuple of 3d arrays
+        Returns both distance matrices between `X` and `Y` and `X` itself. See
+        `batch_cdist` and `batch_pdist` for more details.
     """
-    D = _copy_array_if_base_present(D)
-    N, M = D.shape
-    d = int(0.5 * (np.sqrt(8 * M + 1) + 1))
-    out = np.zeros((N, d, d), dtype=D.dtype)
-    for i in range(N):
-        _distance_wrap.to_squareform_from_vector_wrap(out[i], D[i])
-    return out
+    B, N, _ = X.shape
+    out_c = np.empty((B, N, Y.shape[1]), dtype=X.dtype)
+    out_p = np.empty((B, N, N), dtype=X.dtype)
+    for i in prange(B):
+        out_c[i] = cdist_func(X[i], Y[i], type)
+        out_p[i] = pdist_func(X[i], type)
+    return out_c, out_p
 
 
-@jit
+@jit()
 def pso_equation(
     x: Array3d,
     px: Array3d,
     sx: Array3d,
     v: Array3d,
     v_max: Array3d,
     w: Array3d,
```

### Comparing `vpso-1.0.1/src/vpso/mutation.py` & `vpso-1.0.2/src/vpso/mutation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 
 from vpso.jit import _int, jit
 from vpso.typing import Array2d, Array3d
 
 
-@jit
+@jit()
 def polynomial_mutation(
     x_best: Array2d,
     mutation_mask: Array2d,
     lb: Array2d,
     ub: Array2d,
     nvec: int,
     dim: int,
@@ -48,15 +48,15 @@
     val1 = np.power(2.0 * R + (1.0 - 2.0 * R) * xy1, mut_pow)
     val2 = np.power(2.0 * (1.0 - R) + 2.0 * (R - 0.5) * xy2, mut_pow)
     deltaq = np.where(R <= 0.5, val1 - 1.0, 1.0 - val2)
 
     return np.where(mutation_mask, x_best + deltaq * domain, x_best).clip(lb, ub)
 
 
-@jit
+@jit()
 def mutate(
     x: Array3d,
     px: Array3d,
     pf: Array2d,
     lb: Array3d,
     ub: Array3d,
     nvec: int,
```

### Comparing `vpso-1.0.1/src/vpso/reparation.py` & `vpso-1.0.2/src/vpso/reparation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
 from vpso.jit import jit
 from vpso.math import pso_equation
 from vpso.typing import Array3d
 
 
-@jit
+@jit()
 def repair_out_of_bounds(
     x: Array3d,
     x_new: Array3d,
     v_new: Array3d,
     px: Array3d,
     sx: Array3d,
     v: Array3d,
```

### Comparing `vpso-1.0.1/src/vpso/termination.py` & `vpso-1.0.2/src/vpso/termination.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 
 from vpso.jit import jit
 from vpso.typing import Array1d, Array1i, Array2i, Array3d
 
 
-@jit
+@jit()
 def update_patience(
     sx: Array3d,
     sf: Array1d,
     sx_new: Array3d,
     sf_new: Array1d,
     lb: Array3d,
     ub: Array3d,
```

### Comparing `vpso-1.0.1/src/vpso/vpso.py` & `vpso-1.0.2/src/vpso/vpso.py`

 * *Files identical despite different names*

### Comparing `vpso-1.0.1/src/vpso.egg-info/PKG-INFO` & `vpso-1.0.2/src/vpso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vpso
-Version: 1.0.1
-Summary: Multiple Particle Swarm Optimization
+Version: 1.0.2
+Summary: Vectorized Particle Swarm Optimization
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/vectorized-particle-swarm
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/vectorized-particle-swarm/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vpso-1.0.1/src/vpso.egg-info/SOURCES.txt` & `vpso-1.0.2/src/vpso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vpso-1.0.1/tests/test_adaptation.py` & `vpso-1.0.2/tests/test_adaptation.py`

 * *Files identical despite different names*

### Comparing `vpso-1.0.1/tests/test_initialization.py` & `vpso-1.0.2/tests/test_initialization.py`

 * *Files identical despite different names*

### Comparing `vpso-1.0.1/tests/test_math.py` & `vpso-1.0.2/tests/test_math.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 import unittest
 
 import numpy as np
+from parameterized import parameterized
 from scipy.spatial.distance import cdist, pdist, squareform
 
-from vpso.math import batch_cdist, batch_pdist, batch_squareform, pso_equation
+from vpso.math import batch_cdist, batch_cdist_and_pdist, batch_pdist, pso_equation
 
 
 class TestMath(unittest.TestCase):
-    def test_batch_cdist(self):
+    @parameterized.expand((("euclidean",), ("sqeuclidean",)))
+    def test_batch_cdist(self, dist_type: str):
         N, M1, M2, d = np.random.randint(10, 50, size=4)
         X = np.random.randn(N, M1, d)
         Y = np.random.randn(N, M2, d)
-        actual = batch_cdist(X, Y)
-        expected = np.asarray([cdist(x, y) for x, y in zip(X, Y)])
+        actual = batch_cdist(X, Y, dist_type)
+        expected = np.asarray([cdist(x, y, dist_type) for x, y in zip(X, Y)])
         np.testing.assert_allclose(actual, expected)
 
-    def test_batch_pdist(self):
+    @parameterized.expand((("euclidean",), ("sqeuclidean",)))
+    def test_batch_pdist(self, dist_type: str):
         N, M, d = np.random.randint(10, 50, size=3)
         X = np.random.randn(N, M, d)
-        actual = batch_pdist(X)
-        expected = np.asarray([pdist(x) for x in X])
+        actual = batch_pdist(X, dist_type)
+        expected = np.asarray([squareform(pdist(x, dist_type)) for x in X])
         np.testing.assert_allclose(actual, expected)
 
-    def test_batch_squareform(self):
-        N, d = np.random.randint(10, 50, size=2)
-        X = np.random.randn(N, d * (d - 1) // 2)
-        actual = batch_squareform(X)
-        expected = np.asarray([squareform(x) for x in X])
-        np.testing.assert_allclose(actual, expected)
+    @parameterized.expand((("euclidean",), ("sqeuclidean",)))
+    def test_batch_cdist_and_pdist(self, dist_type: str):
+        N, M1, M2, d = np.random.randint(10, 50, size=4)
+        X = np.random.randn(N, M1, d)
+        Y = np.random.randn(N, M2, d)
+        actual_c, actual_p = batch_cdist_and_pdist(X, Y, dist_type)
+        expected_c = np.asarray([cdist(x, y, dist_type) for x, y in zip(X, Y)])
+        expected_p = np.asarray([squareform(pdist(x, dist_type)) for x in X])
+        np.testing.assert_allclose(actual_c, expected_c)
+        np.testing.assert_allclose(actual_p, expected_p)
 
     def test_pso_equation(self):
         seed = np.random.randint(0, 1000)
         nvec, dim = np.random.randint(3, 10, size=2)
         swarmsize = np.random.randint(1000, 2000)
         np_random = np.random.Generator(np.random.PCG64(seed))
         r1 = np_random.uniform(size=(nvec, swarmsize, dim))
```

### Comparing `vpso-1.0.1/tests/test_mutation.py` & `vpso-1.0.2/tests/test_mutation.py`

 * *Files identical despite different names*

### Comparing `vpso-1.0.1/tests/test_numerical.py` & `vpso-1.0.2/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `vpso-1.0.1/tests/test_reparation.py` & `vpso-1.0.2/tests/test_reparation.py`

 * *Files identical despite different names*

