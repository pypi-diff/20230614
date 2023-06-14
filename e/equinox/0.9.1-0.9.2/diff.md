# Comparing `tmp/equinox-0.9.1.tar.gz` & `tmp/equinox-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equinox-0.9.1.tar", last modified: Tue Nov 15 05:28:59 2022, max compression
+gzip compressed data, was "equinox-0.9.2.tar", last modified: Thu Nov 17 05:41:18 2022, max compression
```

## Comparing `equinox-0.9.1.tar` & `equinox-0.9.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 05:28:59.334461 equinox-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-15 05:28:54.000000 equinox-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-15 05:28:54.000000 equinox-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4442 2022-11-15 05:28:59.334461 equinox-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-11-15 05:28:54.000000 equinox-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 05:28:59.330461 equinox-0.9.1/equinox/
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/callback.py
--rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/compile_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/eval_shape.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 05:28:59.330461 equinox-0.9.1/equinox/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6929 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/experimental/batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (121)     6072 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/experimental/spectral_norm.py
--rw-r--r--   0 runner    (1001) docker     (121)    24461 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/experimental/stateful.py
--rw-r--r--   0 runner    (1001) docker     (121)     5818 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)    19475 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/grad.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 05:28:59.334461 equinox-0.9.1/equinox/internal/
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4460 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/internal/ad.py
--rw-r--r--   0 runner    (1001) docker     (121)     4437 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/internal/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)     3455 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/internal/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/internal/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/internal/nextafter.py
--rw-r--r--   0 runner    (1001) docker     (121)    15614 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/internal/noinline.py
--rw-r--r--   0 runner    (1001) docker     (121)     7100 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/internal/omega.py
--rw-r--r--   0 runner    (1001) docker     (121)    12906 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/internal/primitive.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/internal/str2jax.py
--rw-r--r--   0 runner    (1001) docker     (121)     2731 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/internal/unvmap.py
--rw-r--r--   0 runner    (1001) docker     (121)     9388 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/jit.py
--rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/make_jaxpr.py
--rw-r--r--   0 runner    (1001) docker     (121)     9332 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 05:28:59.334461 equinox-0.9.1/equinox/nn/
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10674 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/nn/attention.py
--rw-r--r--   0 runner    (1001) docker     (121)     5432 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/nn/composed.py
--rw-r--r--   0 runner    (1001) docker     (121)    20546 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/nn/conv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2820 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/nn/dropout.py
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/nn/embedding.py
--rw-r--r--   0 runner    (1001) docker     (121)     3000 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/nn/linear.py
--rw-r--r--   0 runner    (1001) docker     (121)     6431 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/nn/normalisation.py
--rw-r--r--   0 runner    (1001) docker     (121)    20342 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/nn/pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     6638 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/nn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (121)     7106 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/pretty_print.py
--rw-r--r--   0 runner    (1001) docker     (121)    10362 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/serialisation.py
--rw-r--r--   0 runner    (1001) docker     (121)    11165 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/tree.py
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/update.py
--rw-r--r--   0 runner    (1001) docker     (121)    22488 2022-11-15 05:28:54.000000 equinox-0.9.1/equinox/vmap_pmap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 05:28:59.330461 equinox-0.9.1/equinox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4442 2022-11-15 05:28:59.000000 equinox-0.9.1/equinox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-11-15 05:28:59.000000 equinox-0.9.1/equinox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 05:28:59.000000 equinox-0.9.1/equinox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 05:28:59.000000 equinox-0.9.1/equinox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-15 05:28:59.000000 equinox-0.9.1/equinox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-15 05:28:59.000000 equinox-0.9.1/equinox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-15 05:28:59.334461 equinox-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-11-15 05:28:54.000000 equinox-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 05:41:18.737711 equinox-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-17 05:41:14.000000 equinox-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-17 05:41:14.000000 equinox-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4442 2022-11-17 05:41:18.737711 equinox-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-11-17 05:41:14.000000 equinox-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 05:41:18.729710 equinox-0.9.2/equinox/
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/callback.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/compile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      824 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/doc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      889 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/eval_shape.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 05:41:18.733711 equinox-0.9.2/equinox/experimental/
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6929 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/experimental/batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6072 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/experimental/spectral_norm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22389 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/experimental/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5818 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/filters.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19552 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/grad.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 05:41:18.733711 equinox-0.9.2/equinox/internal/
+-rw-r--r--   0 runner    (1001) docker     (121)      760 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4460 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/internal/ad.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4437 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/internal/debug.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3455 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/internal/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/internal/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      884 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/internal/nextafter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15614 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/internal/noinline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7100 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/internal/omega.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12906 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/internal/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/internal/str2jax.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2731 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/internal/unvmap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9388 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/jit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2126 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/make_jaxpr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9332 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/module.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 05:41:18.737711 equinox-0.9.2/equinox/nn/
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10674 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/nn/attention.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5432 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/nn/composed.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20546 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/nn/conv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2820 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/nn/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/nn/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3000 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/nn/linear.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6431 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/nn/normalisation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20342 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/nn/pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6638 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/nn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7106 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/pretty_print.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10958 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11165 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)      866 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/update.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22488 2022-11-17 05:41:14.000000 equinox-0.9.2/equinox/vmap_pmap.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 05:41:18.733711 equinox-0.9.2/equinox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4442 2022-11-17 05:41:18.000000 equinox-0.9.2/equinox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-11-17 05:41:18.000000 equinox-0.9.2/equinox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 05:41:18.000000 equinox-0.9.2/equinox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 05:41:18.000000 equinox-0.9.2/equinox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-17 05:41:18.000000 equinox-0.9.2/equinox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-17 05:41:18.000000 equinox-0.9.2/equinox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-17 05:41:18.737711 equinox-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-11-17 05:41:14.000000 equinox-0.9.2/setup.py
```

### Comparing `equinox-0.9.1/LICENSE` & `equinox-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/PKG-INFO` & `equinox-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equinox
-Version: 0.9.1
+Version: 0.9.2
 Summary: PyTorch-like neural networks in JAX
 Home-page: https://github.com/patrick-kidger/equinox
 Author: Patrick Kidger
 Author-email: contact@kidger.site
 Maintainer: Patrick Kidger
 Maintainer-email: contact@kidger.site
 License: Apache-2.0
```

### Comparing `equinox-0.9.1/README.md` & `equinox-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/__init__.py` & `equinox-0.9.2/equinox/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     tree_serialise_leaves,
 )
 from .tree import tree_at, tree_equal, tree_inference
 from .update import apply_updates
 from .vmap_pmap import filter_pmap, filter_vmap
 
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
```

### Comparing `equinox-0.9.1/equinox/callback.py` & `equinox-0.9.2/equinox/callback.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,22 @@
     callback, *args, result_shape_dtypes, vectorized=False, **kwargs
 ):
     """Calls a Python function inside a JIT region. As `jax.pure_callback` but accepts
     arbitrary Python objects as inputs and outputs. (Not just JAXable types.)
 
     **Arguments:**
 
-        - `callback`: The Python function to call.
-        - `args`, `kwargs`: The function will be called as `callback(*args, **kwargs)`.
-            These may be arbitrary Python objects.
-        - `result_shape_dtypes`: A PyTree specifying the output of `callback`. It should
-            have a `jax.ShapeDtypeStruct` in place of any JAX arrays.
-        - `vectorized`: If `True` then `callback` is batched(when transformed by `vmap`)
-            by calling it directly on the batched arrays. If `False` then `callback` is
-            called on each batch element individually.
+    - `callback`: The Python function to call.
+    - `args`, `kwargs`: The function will be called as `callback(*args, **kwargs)`.
+        These may be arbitrary Python objects.
+    - `result_shape_dtypes`: A PyTree specifying the output of `callback`. It should
+        have a `jax.ShapeDtypeStruct` in place of any JAX arrays.
+    - `vectorized`: If `True` then `callback` is batched(when transformed by `vmap`)
+        by calling it directly on the batched arrays. If `False` then `callback` is
+        called on each batch element individually.
 
     **Returns:**
 
     The result of `callback(*args, **kwargs)`, valid for use under JIT.
     """
     dynamic, static = partition((args, kwargs), is_array)
     dynamic_struct, static_struct = partition(result_shape_dtypes, _is_struct)
```

### Comparing `equinox-0.9.1/equinox/compile_utils.py` & `equinox-0.9.2/equinox/compile_utils.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/doc_utils.py` & `equinox-0.9.2/equinox/doc_utils.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/eval_shape.py` & `equinox-0.9.2/equinox/eval_shape.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/experimental/batch_norm.py` & `equinox-0.9.2/equinox/experimental/batch_norm.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/experimental/spectral_norm.py` & `equinox-0.9.2/equinox/experimental/spectral_norm.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/experimental/stateful.py` & `equinox-0.9.2/equinox/experimental/stateful.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import jax.lax as lax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 from jaxtyping import Array, PyTree
 
 from ..filters import is_array
 from ..module import Module, static_field
-from ..tree import tree_at
 
 
 # So the use of a weak dictionary is a bit of wishful thinking here, really.
 # In practice JAX will cache the _IndexObj when it is passed across the hcb.call
 # boundary.
 # Which at least in part is what we want! We want the cached state to persist for
 # as long as the XLA graph it's part of.
@@ -231,56 +230,19 @@
 
 
 def _monkey_patch():
     global _have_monkey_patched
     if not _have_monkey_patched:
         _have_monkey_patched = True
 
-        _old_outside_call_impl = hcb.outside_call_p.impl
-        _old_outside_call_translation_rule = xla._translations[hcb.outside_call_p]
         _old_outside_call_batching_rule = batching.primitive_batchers[
             hcb.outside_call_p
         ]
 
         #
-        # Overwrite impl and abstract_eval:
-        # Make `get_state` not actually pass `like` into the
-        # callback. This means we don't need to wait for `like` to be computed at
-        # runtime.
-        #
-
-        def _outside_call_impl(*arg_flat, arg_treedef, **params):
-            leaves = [None] * arg_treedef.num_leaves
-            call_type = type(jtu.tree_unflatten(arg_treedef, leaves))
-            # Not using isinstance for speed. (Questionable choice?)
-            if call_type is _GetStateArg:
-                arg = jtu.tree_unflatten(arg_treedef, arg_flat)
-                assert arg.index._state is None
-                token_like = jtu.tree_map(lambda _: jax.core.token, arg.like)
-                arg = tree_at(lambda a: a.like, arg, token_like)
-                arg_flat = jtu.tree_leaves(arg)
-            return _old_outside_call_impl(*arg_flat, arg_treedef=arg_treedef, **params)
-
-        def _outside_call_translation_rule(ctx, avals_in, *args, arg_treedef, **kwargs):
-            leaves = [None] * arg_treedef.num_leaves
-            call_type = type(jtu.tree_unflatten(arg_treedef, leaves))
-            if call_type is _GetStateArg:
-                arg_flat = avals_in[:-2]
-                extra_tokens = avals_in[-2:]
-                arg = jtu.tree_unflatten(arg_treedef, arg_flat)
-                assert arg.index._state is None
-                token_like = jtu.tree_map(lambda _: jax.core.abstract_token, arg.like)
-                arg = tree_at(lambda a: a.like, arg, token_like)
-                arg_flat = jtu.tree_leaves(arg)
-                avals_in = arg_flat + extra_tokens
-            return _old_outside_call_translation_rule(
-                ctx, avals_in, *args, arg_treedef=arg_treedef, **kwargs
-            )
-
-        #
         # Overwrite batching:
         # Allows us to use get_state and set_state inside vmap.
         # (Not implemented for general `host_callback.call`s.)
         #
 
         def _target_batch_axes(batch_axes_flat, arg_treedef, target):
             batch_axes_leaves_flat = [_Leaf(b) for b in batch_axes_flat]
@@ -320,17 +282,15 @@
                     arg_flat,
                     batch_axes_flat,
                     arg_treedef=arg_treedef,
                     result_treedef=result_treedef,
                     **params,
                 )
 
-        hcb.outside_call_p.def_impl(_outside_call_impl)
         batching.primitive_batchers[hcb.outside_call_p] = _outside_call_batching_rule
-        xla.register_translation(hcb.outside_call_p, _outside_call_translation_rule)
 
 
 def _batchify_impl(*flat, treedef, like_batch_axes, current_batch_axes):
     if current_batch_axes != like_batch_axes:
         raise RuntimeError("`like` and the saved state have different batch axes")
     state, like = jtu.tree_unflatten(treedef, flat)
     return jtu.tree_leaves(state)
```

### Comparing `equinox-0.9.1/equinox/filters.py` & `equinox-0.9.2/equinox/filters.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/grad.py` & `equinox-0.9.2/equinox/grad.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 import jax.tree_util as jtu
 from jaxtyping import Array, PyTree
 
 from .custom_types import BoolAxisSpec, sentinel
 from .doc_utils import doc_strip_annotations
 from .filters import (
     combine,
+    filter,
     is_array,
     is_inexact_array,
     is_inexact_array_like,
     partition,
 )
 from .make_jaxpr import filter_make_jaxpr
-from .module import Module, module_update_wrapper, Static
+from .module import Module, module_update_wrapper, Static, static_field
 
 
 class _ValueAndGradWrapper(Module):
     _fun: Callable
     _arg: PyTree[BoolAxisSpec]
     _gradkwargs: Dict[str, Any]
 
@@ -255,18 +256,18 @@
     if has_aux:
         return out, vjp_fn, aux
     else:
         return out, vjp_fn
 
 
 class _ClosureConvert(Module):
-    jaxpr: jax.core.Jaxpr
+    jaxpr: jax.core.Jaxpr = static_field()
     consts: PyTree[Array]  # Captured in the PyTree structure of _ClosureConvert
-    out_dynamic_struct: PyTree[jax.ShapeDtypeStruct]
-    out_static: PyTree[Any]
+    out_dynamic_struct: PyTree[jax.ShapeDtypeStruct] = static_field()
+    out_static: PyTree[Any] = static_field()
 
     def __call__(self, *args, **kwargs):
         dynamic = filter((args, kwargs), is_array)
         dynamic_flat = jtu.tree_leaves(dynamic)
         out_dynamic_flat = jax.core.eval_jaxpr(self.jaxpr, self.consts, *dynamic_flat)
         out_dynamic_struct_flat, out_dynamic_treedef = jtu.tree_flatten(
             self.out_dynamic_struct
@@ -278,15 +279,15 @@
         out = jtu.tree_unflatten(out_dynamic_treedef, out_dynamic_flat)
         out = combine(out, self.out_static)
         return out
 
 
 def filter_closure_convert(fn, *args, **kwargs):
     """As `jax.closure_convert`, but works on functions accepting and returning
-    arbtirary PyTree objects. In addition, all JAX arrays are hoisted into constants
+    arbitrary PyTree objects. In addition, all JAX arrays are hoisted into constants
     (not just floating point arrays).
 
     This is useful for explicitly capturing any closed-over JAX tracers
     before crossing an API boundary, such as `jax.grad`, `jax.custom_vjp`, or the
     rule of a custom primitive.
 
     **Arguments:**
```

### Comparing `equinox-0.9.1/equinox/internal/__init__.py` & `equinox-0.9.2/equinox/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/internal/ad.py` & `equinox-0.9.2/equinox/internal/ad.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/internal/debug.py` & `equinox-0.9.2/equinox/internal/debug.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/internal/errors.py` & `equinox-0.9.2/equinox/internal/errors.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/internal/misc.py` & `equinox-0.9.2/equinox/internal/misc.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/internal/nextafter.py` & `equinox-0.9.2/equinox/internal/nextafter.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/internal/noinline.py` & `equinox-0.9.2/equinox/internal/noinline.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/internal/omega.py` & `equinox-0.9.2/equinox/internal/omega.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/internal/primitive.py` & `equinox-0.9.2/equinox/internal/primitive.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/internal/unvmap.py` & `equinox-0.9.2/equinox/internal/unvmap.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/jit.py` & `equinox-0.9.2/equinox/jit.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/make_jaxpr.py` & `equinox-0.9.2/equinox/make_jaxpr.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,18 +39,20 @@
     - `fun`: The function `fun(*arg, **kwargs)` whose jaxpr is to be computed. Its
         positional and keyword arguments may be anything, as can its return value.
 
     **Returns:**
 
     A wrapped version of `fun`, that when applied to example arguments
     `*args, **kwargs`, will return a 3-tuple of:
+
     - A `ClosedJaxpr` representing the evaluation of that function on those arguments.
     - A `PyTree[jax.ShapeDtypeStruct]` representing the output shape and dtype of the
         result.
     - A `PyTree[Any]` representing any non-array outputs from `fun`.
 
-    The example arguments may be either JAX/NumPy arrays, or anything with `.shape` and
-    `.dtype` fields (typically `jax.ShapeDtypeStruct`s). Python builtins (`int`,
-    `float`, `bool`, `complex`) are treated as static inputs; wrap them in JAX/NumPy
+    The example arguments to be traced may be anything with `.shape` and `.dtype`
+    fields (typically JAX arrays, NumPy arrays, of `jax.ShapeDtypeStruct`s). All
+    other argments are treated statically. In particular, Python builtins (`bool`,
+    `int`, `float`, `complex`) are treated as static inputs; wrap them in JAX/NumPy
     arrays if you would like them to be traced.
     """
     return _MakeJaxpr(fun)
```

### Comparing `equinox-0.9.1/equinox/module.py` & `equinox-0.9.2/equinox/module.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/nn/__init__.py` & `equinox-0.9.2/equinox/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/nn/attention.py` & `equinox-0.9.2/equinox/nn/attention.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/nn/composed.py` & `equinox-0.9.2/equinox/nn/composed.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/nn/conv.py` & `equinox-0.9.2/equinox/nn/conv.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/nn/dropout.py` & `equinox-0.9.2/equinox/nn/dropout.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/nn/embedding.py` & `equinox-0.9.2/equinox/nn/embedding.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/nn/linear.py` & `equinox-0.9.2/equinox/nn/linear.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/nn/normalisation.py` & `equinox-0.9.2/equinox/nn/normalisation.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/nn/pool.py` & `equinox-0.9.2/equinox/nn/pool.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/nn/rnn.py` & `equinox-0.9.2/equinox/nn/rnn.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/pretty_print.py` & `equinox-0.9.2/equinox/pretty_print.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/serialisation.py` & `equinox-0.9.2/equinox/serialisation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pathlib
+from contextlib import contextmanager
 from typing import Any, BinaryIO, Callable, Optional, Union
 
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy as np
 from jaxtyping import PyTree
 
@@ -159,14 +160,28 @@
     path = pathlib.Path(path)
     if path.suffix == "":
         return path.with_suffix(".eqx")
     else:
         return path
 
 
+@contextmanager
+def _maybe_open(path_or_file: Union[str, pathlib.Path, BinaryIO], mode: str):
+    """A function that unifies handling of file objects and path-like objects
+    by opening the latter."""
+    if isinstance(path_or_file, (str, pathlib.Path)):
+        file = open(_with_suffix(path_or_file), mode)
+        try:
+            yield file
+        finally:
+            file.close()
+    else:  # file-like object
+        yield path_or_file
+
+
 def _assert_same(new, old):
     if type(new) is not type(old):
         raise RuntimeError(
             f"Deserialised leaf has changed type from {type(old)} in `like` to {type(new)} on disk."
         )
     if isinstance(new, (np.ndarray, jnp.ndarray)):
         if new.shape != old.shape:
@@ -180,24 +195,24 @@
 
 
 def _is_index(x):
     return isinstance(x, experimental.StateIndex)
 
 
 def tree_serialise_leaves(
-    path: Union[str, pathlib.Path],
+    path_or_file: Union[str, pathlib.Path, BinaryIO],
     pytree: PyTree,
     filter_spec=default_serialise_filter_spec,
     is_leaf: Callable[[Any], bool] = _is_index,
 ) -> None:
     """Save the leaves of a PyTree to file.
 
     **Arguments:**
 
-    - `path`: The file location to save values to.
+    - `path_or_file`: The file location to save values to or a binary file-like object.
     - `pytree`: The PyTree whose leaves will be saved.
     - `filter_spec`: Specifies how to save each kind of leaf. By default all JAX
         arrays, NumPy arrays, Python bool/int/float/complexes are saved,
         [`equinox.experimental.StateIndex`][] instances have their value looked up
         and saved, and all other leaf types are ignored. (See
         [`equinox.default_serialise_filter_spec`][].)
     - `is_leaf`: Called on every node of `pytree`; if `True` then this node will be
@@ -226,36 +241,36 @@
         does nothing.
 
         It can also be a PyTree of such functions, in which case the PyTree structure
         should be a prefix of `pytree`, and each function will be mapped over the
         corresponding sub-PyTree of `pytree`.
     """
 
-    with open(_with_suffix(path), "wb") as f:
+    with _maybe_open(path_or_file, "wb") as f:
 
         def _serialise(spec, x):
             def __serialise(y):
                 spec(f, y)
 
             _ordered_tree_map(__serialise, x, is_leaf=is_leaf)
 
         _ordered_tree_map(_serialise, filter_spec, pytree)
 
 
 def tree_deserialise_leaves(
-    path: Union[str, pathlib.Path],
+    path_or_file: Union[str, pathlib.Path, BinaryIO],
     like: PyTree,
     filter_spec=default_deserialise_filter_spec,
     is_leaf: Callable[[Any], bool] = _is_index,
 ) -> PyTree:
     """Load the leaves of a PyTree from a file.
 
     **Arguments:**
 
-    - `path`: The file location to load values from.
+    - `path_or_file`: The file location to load values from or a binary file-like object.
     - `like`: A PyTree of same structure, and with leaves of the same type, as the
         PyTree being loaded. Those leaves which are loaded will replace the
         corresponding leaves of `like`.
     - `filter_spec`: Specifies how to load each kind of leaf. By default all JAX
         arrays, NumPy arrays, Python bool/int/float/complexes are loaded, and
         [`equinox.experimental.StateIndex`][] instances have their value looked up
         and stored, and all other leaf types are not loaded, and will retain their
@@ -289,16 +304,15 @@
         a file handle and a leaf from `like`, and either returns the corresponding
         loaded leaf, or retuns the leaf from `like` unchanged.
 
         It can also be a PyTree of such functions, in which case the PyTree structure
         should be a prefix of `pytree`, and each function will be mapped over the
         corresponding sub-PyTree of `pytree`.
     """
-
-    with open(_with_suffix(path), "rb") as f:
+    with _maybe_open(path_or_file, "rb") as f:
 
         def _deserialise(spec, x):
             def __deserialise(y):
                 return spec(f, y)
 
             return _ordered_tree_map(__deserialise, x, is_leaf=is_leaf)
```

### Comparing `equinox-0.9.1/equinox/tree.py` & `equinox-0.9.2/equinox/tree.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/update.py` & `equinox-0.9.2/equinox/update.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox/vmap_pmap.py` & `equinox-0.9.2/equinox/vmap_pmap.py`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/equinox.egg-info/PKG-INFO` & `equinox-0.9.2/equinox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equinox
-Version: 0.9.1
+Version: 0.9.2
 Summary: PyTorch-like neural networks in JAX
 Home-page: https://github.com/patrick-kidger/equinox
 Author: Patrick Kidger
 Author-email: contact@kidger.site
 Maintainer: Patrick Kidger
 Maintainer-email: contact@kidger.site
 License: Apache-2.0
```

### Comparing `equinox-0.9.1/equinox.egg-info/SOURCES.txt` & `equinox-0.9.2/equinox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equinox-0.9.1/setup.py` & `equinox-0.9.2/setup.py`

 * *Files identical despite different names*

