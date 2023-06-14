# Comparing `tmp/dimod-0.9.8.tar.gz` & `tmp/dimod-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "./dist/dimod-0.9.8.tar", last modified: Fri Sep 25 17:02:50 2020, max compression
+gzip compressed data, was "./dist/dimod-0.9.9.tar", last modified: Tue Oct  6 01:40:38 2020, max compression
```

## Comparing `dimod-0.9.8.tar` & `dimod-0.9.9.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.288527 dimod-0.9.8/
--rw-r--r--   0 root         (0) root         (0)      168 2020-09-25 16:56:35.000000 dimod-0.9.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3772 2020-09-25 17:02:50.288527 dimod-0.9.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2292 2020-09-25 16:56:35.000000 dimod-0.9.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.260526 dimod-0.9.8/dimod/
--rw-r--r--   0 root         (0) root         (0)      717 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/__init__.pxd
--rw-r--r--   0 root         (0) root         (0)     1860 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15582 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/binary_quadratic_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.272526 dimod-0.9.8/dimod/bqm/
--rw-r--r--   0 root         (0) root         (0)      980 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/bqm/__init__.pxd
--rw-r--r--   0 root         (0) root         (0)      914 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/bqm/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1584641 2020-09-25 17:02:42.000000 dimod-0.9.8/dimod/bqm/adjarraybqm.cpp
--rw-r--r--   0 root         (0) root         (0)     4531 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/bqm/adjarraybqm.pxd
--rw-r--r--   0 root         (0) root         (0)    23754 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/bqm/adjarraybqm.pyx
--rw-r--r--   0 root         (0) root         (0)    20598 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/bqm/adjdictbqm.py
--rw-r--r--   0 root         (0) root         (0)  1703440 2020-09-25 17:02:44.000000 dimod-0.9.8/dimod/bqm/adjmapbqm.cpp
--rw-r--r--   0 root         (0) root         (0)     4444 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/bqm/adjmapbqm.pxd
--rw-r--r--   0 root         (0) root         (0)    32208 2020-09-25 16:58:13.000000 dimod-0.9.8/dimod/bqm/adjmapbqm.pyx
--rw-r--r--   0 root         (0) root         (0)  1710056 2020-09-25 17:02:45.000000 dimod-0.9.8/dimod/bqm/adjvectorbqm.cpp
--rw-r--r--   0 root         (0) root         (0)     4559 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/bqm/adjvectorbqm.pxd
--rw-r--r--   0 root         (0) root         (0)    32238 2020-09-25 16:58:13.000000 dimod-0.9.8/dimod/bqm/adjvectorbqm.pyx
--rw-r--r--   0 root         (0) root         (0)   283502 2020-09-25 17:02:45.000000 dimod-0.9.8/dimod/bqm/common.cpp
--rw-r--r--   0 root         (0) root         (0)     1161 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/bqm/common.pxd
--rw-r--r--   0 root         (0) root         (0)     1007 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/bqm/common.pyx
--rw-r--r--   0 root         (0) root         (0)     4215 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/bqm/construction.py
--rw-r--r--   0 root         (0) root         (0)     9520 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/bqm/cppbqm.pxd
--rw-r--r--   0 root         (0) root         (0)     2427 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/bqm/make.py
--rw-r--r--   0 root         (0) root         (0)    32183 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/bqm/shapeablebqm.pyx.src
--rw-r--r--   0 root         (0) root         (0)  2042528 2020-09-25 17:02:47.000000 dimod-0.9.8/dimod/bqm/utils.cpp
--rw-r--r--   0 root         (0) root         (0)      824 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/bqm/utils.pxd
--rw-r--r--   0 root         (0) root         (0)    13316 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/bqm/utils.pyx
--rw-r--r--   0 root         (0) root         (0)     1204 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/compatibility23.py
--rw-r--r--   0 root         (0) root         (0)     3951 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/converters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.272526 dimod-0.9.8/dimod/core/
--rw-r--r--   0 root         (0) root         (0)      971 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50072 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/core/bqm.py
--rw-r--r--   0 root         (0) root         (0)     4065 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/core/composite.py
--rw-r--r--   0 root         (0) root         (0)     8288 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/core/initialized.py
--rw-r--r--   0 root         (0) root         (0)     5053 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/core/polysampler.py
--rw-r--r--   0 root         (0) root         (0)     8336 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/core/sampler.py
--rw-r--r--   0 root         (0) root         (0)     5072 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/core/structured.py
--rw-r--r--   0 root         (0) root         (0)    15093 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.276527 dimod-0.9.8/dimod/discrete/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/discrete/__init__.pxd
--rw-r--r--   0 root         (0) root         (0)      665 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/discrete/__init__.py
--rw-r--r--   0 root         (0) root         (0)  2110670 2020-09-25 17:02:50.000000 dimod-0.9.8/dimod/discrete/cydiscrete_quadratic_model.cpp
--rw-r--r--   0 root         (0) root         (0)     2442 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/discrete/cydiscrete_quadratic_model.pxd
--rw-r--r--   0 root         (0) root         (0)    20257 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/discrete/cydiscrete_quadratic_model.pyx
--rw-r--r--   0 root         (0) root         (0)    27981 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/discrete/discrete_quadratic_model.py
--rw-r--r--   0 root         (0) root         (0)     1541 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.276527 dimod-0.9.8/dimod/generators/
--rw-r--r--   0 root         (0) root         (0)     1004 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/generators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3108 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/generators/anti_crossing.py
--rw-r--r--   0 root         (0) root         (0)     4454 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/generators/chimera.py
--rw-r--r--   0 root         (0) root         (0)     3527 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/generators/constraints.py
--rw-r--r--   0 root         (0) root         (0)     6425 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/generators/fcl.py
--rw-r--r--   0 root         (0) root         (0)     8515 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/generators/random.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.276527 dimod-0.9.8/dimod/higherorder/
--rw-r--r--   0 root         (0) root         (0)      829 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/higherorder/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15710 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/higherorder/polynomial.py
--rw-r--r--   0 root         (0) root         (0)     9722 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/higherorder/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.256526 dimod-0.9.8/dimod/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.280526 dimod-0.9.8/dimod/include/dimod/
--rw-r--r--   0 root         (0) root         (0)     6828 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/include/dimod/adjarraybqm.h
--rw-r--r--   0 root         (0) root         (0)     6248 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/include/dimod/adjmapbqm.h
--rw-r--r--   0 root         (0) root         (0)    11380 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/include/dimod/adjvectorbqm.h
--rw-r--r--   0 root         (0) root         (0)      950 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/include/dimod/utils.h
--rw-r--r--   0 root         (0) root         (0)     2173 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/meta.py
--rw-r--r--   0 root         (0) root         (0)      882 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/package_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.280526 dimod-0.9.8/dimod/reference/
--rw-r--r--   0 root         (0) root         (0)      792 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.280526 dimod-0.9.8/dimod/reference/composites/
--rw-r--r--   0 root         (0) root         (0)     1381 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/composites/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3896 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/composites/clipcomposite.py
--rw-r--r--   0 root         (0) root         (0)     4552 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/composites/connectedcomponent.py
--rw-r--r--   0 root         (0) root         (0)     3920 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/composites/fixedvariable.py
--rw-r--r--   0 root         (0) root         (0)    20009 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/composites/higherordercomposites.py
--rw-r--r--   0 root         (0) root         (0)     3017 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/composites/roofduality.py
--rw-r--r--   0 root         (0) root         (0)     5374 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/composites/scalecomposite.py
--rw-r--r--   0 root         (0) root         (0)     5040 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/composites/spin_transform.py
--rw-r--r--   0 root         (0) root         (0)     4097 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/composites/structure.py
--rw-r--r--   0 root         (0) root         (0)     7357 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/composites/tracking.py
--rw-r--r--   0 root         (0) root         (0)     3114 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/composites/truncatecomposite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.280526 dimod-0.9.8/dimod/reference/samplers/
--rw-r--r--   0 root         (0) root         (0)      985 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/samplers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5544 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/samplers/exact_solver.py
--rw-r--r--   0 root         (0) root         (0)     3999 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/samplers/identity_sampler.py
--rw-r--r--   0 root         (0) root         (0)     2921 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/samplers/null_sampler.py
--rw-r--r--   0 root         (0) root         (0)     2558 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/samplers/random_sampler.py
--rw-r--r--   0 root         (0) root         (0)     9719 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/reference/samplers/simulated_annealing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.284527 dimod-0.9.8/dimod/roof_duality/
--rw-r--r--   0 root         (0) root         (0)      758 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/roof_duality/__init__.py
--rw-r--r--   0 root         (0) root         (0)   252345 2020-09-25 17:02:45.000000 dimod-0.9.8/dimod/roof_duality/_fix_variables.cpp
--rw-r--r--   0 root         (0) root         (0)     2005 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/roof_duality/_fix_variables.pyx
--rw-r--r--   0 root         (0) root         (0)     4354 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/roof_duality/fix_variables.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.284527 dimod-0.9.8/dimod/roof_duality/src/
--rw-r--r--   0 root         (0) root         (0)    18661 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/roof_duality/src/compressed_matrix.hpp
--rw-r--r--   0 root         (0) root         (0)    39235 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/roof_duality/src/fix_variables.cpp
--rw-r--r--   0 root         (0) root         (0)     1354 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/roof_duality/src/fix_variables.hpp
--rw-r--r--   0 root         (0) root         (0)    60264 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/sampleset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.284527 dimod-0.9.8/dimod/serialization/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/serialization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5084 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/serialization/coo.py
--rw-r--r--   0 root         (0) root         (0)    22790 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/serialization/fileview.py
--rw-r--r--   0 root         (0) root         (0)    14181 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/serialization/format.py
--rw-r--r--   0 root         (0) root         (0)     3393 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/serialization/json.py
--rw-r--r--   0 root         (0) root         (0)     4542 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/serialization/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.284527 dimod-0.9.8/dimod/testing/
--rw-r--r--   0 root         (0) root         (0)     1001 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/testing/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12199 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/testing/asserts.py
--rw-r--r--   0 root         (0) root         (0)     7871 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/testing/sampler.py
--rw-r--r--   0 root         (0) root         (0)     3841 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/traversal.py
--rw-r--r--   0 root         (0) root         (0)    15878 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/utilities.py
--rw-r--r--   0 root         (0) root         (0)     4513 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/variables.py
--rw-r--r--   0 root         (0) root         (0)     4678 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/vartypes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.288527 dimod-0.9.8/dimod/views/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4607 2020-09-25 16:56:35.000000 dimod-0.9.8/dimod/views/samples.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 17:02:50.260526 dimod-0.9.8/dimod.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3772 2020-09-25 17:02:50.000000 dimod-0.9.8/dimod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3149 2020-09-25 17:02:50.000000 dimod-0.9.8/dimod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-09-25 17:02:50.000000 dimod-0.9.8/dimod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-09-25 16:58:25.000000 dimod-0.9.8/dimod.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       92 2020-09-25 17:02:50.000000 dimod-0.9.8/dimod.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2020-09-25 17:02:50.000000 dimod-0.9.8/dimod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       80 2020-09-25 17:02:50.288527 dimod-0.9.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5619 2020-09-25 16:56:35.000000 dimod-0.9.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.568371 dimod-0.9.9/
+-rw-r--r--   0 root         (0) root         (0)      168 2020-10-06 01:35:23.000000 dimod-0.9.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3772 2020-10-06 01:40:38.568371 dimod-0.9.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2292 2020-10-06 01:35:23.000000 dimod-0.9.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.540370 dimod-0.9.9/dimod/
+-rw-r--r--   0 root         (0) root         (0)      717 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/__init__.pxd
+-rw-r--r--   0 root         (0) root         (0)     1860 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15582 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/binary_quadratic_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.552371 dimod-0.9.9/dimod/bqm/
+-rw-r--r--   0 root         (0) root         (0)      980 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/bqm/__init__.pxd
+-rw-r--r--   0 root         (0) root         (0)      914 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/bqm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1584641 2020-10-06 01:40:31.000000 dimod-0.9.9/dimod/bqm/adjarraybqm.cpp
+-rw-r--r--   0 root         (0) root         (0)     4531 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/bqm/adjarraybqm.pxd
+-rw-r--r--   0 root         (0) root         (0)    23754 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/bqm/adjarraybqm.pyx
+-rw-r--r--   0 root         (0) root         (0)    20598 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/bqm/adjdictbqm.py
+-rw-r--r--   0 root         (0) root         (0)  1703440 2020-10-06 01:40:33.000000 dimod-0.9.9/dimod/bqm/adjmapbqm.cpp
+-rw-r--r--   0 root         (0) root         (0)     4444 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/bqm/adjmapbqm.pxd
+-rw-r--r--   0 root         (0) root         (0)    32208 2020-10-06 01:36:43.000000 dimod-0.9.9/dimod/bqm/adjmapbqm.pyx
+-rw-r--r--   0 root         (0) root         (0)  1710056 2020-10-06 01:40:34.000000 dimod-0.9.9/dimod/bqm/adjvectorbqm.cpp
+-rw-r--r--   0 root         (0) root         (0)     4559 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/bqm/adjvectorbqm.pxd
+-rw-r--r--   0 root         (0) root         (0)    32238 2020-10-06 01:36:43.000000 dimod-0.9.9/dimod/bqm/adjvectorbqm.pyx
+-rw-r--r--   0 root         (0) root         (0)   283502 2020-10-06 01:40:34.000000 dimod-0.9.9/dimod/bqm/common.cpp
+-rw-r--r--   0 root         (0) root         (0)     1161 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/bqm/common.pxd
+-rw-r--r--   0 root         (0) root         (0)     1007 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/bqm/common.pyx
+-rw-r--r--   0 root         (0) root         (0)     4215 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/bqm/construction.py
+-rw-r--r--   0 root         (0) root         (0)     9520 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/bqm/cppbqm.pxd
+-rw-r--r--   0 root         (0) root         (0)     2427 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/bqm/make.py
+-rw-r--r--   0 root         (0) root         (0)    32183 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/bqm/shapeablebqm.pyx.src
+-rw-r--r--   0 root         (0) root         (0)  2042528 2020-10-06 01:40:36.000000 dimod-0.9.9/dimod/bqm/utils.cpp
+-rw-r--r--   0 root         (0) root         (0)      824 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/bqm/utils.pxd
+-rw-r--r--   0 root         (0) root         (0)    13316 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/bqm/utils.pyx
+-rw-r--r--   0 root         (0) root         (0)     1204 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/compatibility23.py
+-rw-r--r--   0 root         (0) root         (0)     3951 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/converters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.552371 dimod-0.9.9/dimod/core/
+-rw-r--r--   0 root         (0) root         (0)      971 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50072 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/core/bqm.py
+-rw-r--r--   0 root         (0) root         (0)     4065 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/core/composite.py
+-rw-r--r--   0 root         (0) root         (0)     8288 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/core/initialized.py
+-rw-r--r--   0 root         (0) root         (0)     5053 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/core/polysampler.py
+-rw-r--r--   0 root         (0) root         (0)     8336 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/core/sampler.py
+-rw-r--r--   0 root         (0) root         (0)     5072 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/core/structured.py
+-rw-r--r--   0 root         (0) root         (0)    15093 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.556371 dimod-0.9.9/dimod/discrete/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/discrete/__init__.pxd
+-rw-r--r--   0 root         (0) root         (0)      665 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/discrete/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  2150912 2020-10-06 01:40:38.000000 dimod-0.9.9/dimod/discrete/cydiscrete_quadratic_model.cpp
+-rw-r--r--   0 root         (0) root         (0)     2442 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/discrete/cydiscrete_quadratic_model.pxd
+-rw-r--r--   0 root         (0) root         (0)    20674 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/discrete/cydiscrete_quadratic_model.pyx
+-rw-r--r--   0 root         (0) root         (0)    29294 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/discrete/discrete_quadratic_model.py
+-rw-r--r--   0 root         (0) root         (0)     1541 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.556371 dimod-0.9.9/dimod/generators/
+-rw-r--r--   0 root         (0) root         (0)     1004 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/generators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/generators/anti_crossing.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/generators/chimera.py
+-rw-r--r--   0 root         (0) root         (0)     3527 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/generators/constraints.py
+-rw-r--r--   0 root         (0) root         (0)     6425 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/generators/fcl.py
+-rw-r--r--   0 root         (0) root         (0)     8515 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/generators/random.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.560371 dimod-0.9.9/dimod/higherorder/
+-rw-r--r--   0 root         (0) root         (0)      829 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/higherorder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15710 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/higherorder/polynomial.py
+-rw-r--r--   0 root         (0) root         (0)     9722 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/higherorder/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.536370 dimod-0.9.9/dimod/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.560371 dimod-0.9.9/dimod/include/dimod/
+-rw-r--r--   0 root         (0) root         (0)     6828 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/include/dimod/adjarraybqm.h
+-rw-r--r--   0 root         (0) root         (0)    10254 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/include/dimod/adjmapbqm.h
+-rw-r--r--   0 root         (0) root         (0)    11380 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/include/dimod/adjvectorbqm.h
+-rw-r--r--   0 root         (0) root         (0)      950 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/include/dimod/utils.h
+-rw-r--r--   0 root         (0) root         (0)     2173 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/meta.py
+-rw-r--r--   0 root         (0) root         (0)      882 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/package_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.560371 dimod-0.9.9/dimod/reference/
+-rw-r--r--   0 root         (0) root         (0)      792 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.560371 dimod-0.9.9/dimod/reference/composites/
+-rw-r--r--   0 root         (0) root         (0)     1381 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/composites/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3896 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/composites/clipcomposite.py
+-rw-r--r--   0 root         (0) root         (0)     4552 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/composites/connectedcomponent.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/composites/fixedvariable.py
+-rw-r--r--   0 root         (0) root         (0)    20009 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/composites/higherordercomposites.py
+-rw-r--r--   0 root         (0) root         (0)     3017 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/composites/roofduality.py
+-rw-r--r--   0 root         (0) root         (0)     5374 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/composites/scalecomposite.py
+-rw-r--r--   0 root         (0) root         (0)     5040 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/composites/spin_transform.py
+-rw-r--r--   0 root         (0) root         (0)     4097 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/composites/structure.py
+-rw-r--r--   0 root         (0) root         (0)     7357 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/composites/tracking.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/composites/truncatecomposite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.564371 dimod-0.9.9/dimod/reference/samplers/
+-rw-r--r--   0 root         (0) root         (0)      985 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/samplers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5544 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/samplers/exact_solver.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/samplers/identity_sampler.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/samplers/null_sampler.py
+-rw-r--r--   0 root         (0) root         (0)     2558 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/samplers/random_sampler.py
+-rw-r--r--   0 root         (0) root         (0)     9719 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/reference/samplers/simulated_annealing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.564371 dimod-0.9.9/dimod/roof_duality/
+-rw-r--r--   0 root         (0) root         (0)      758 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/roof_duality/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   252345 2020-10-06 01:40:31.000000 dimod-0.9.9/dimod/roof_duality/_fix_variables.cpp
+-rw-r--r--   0 root         (0) root         (0)     2005 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/roof_duality/_fix_variables.pyx
+-rw-r--r--   0 root         (0) root         (0)     4354 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/roof_duality/fix_variables.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.564371 dimod-0.9.9/dimod/roof_duality/src/
+-rw-r--r--   0 root         (0) root         (0)    18661 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/roof_duality/src/compressed_matrix.hpp
+-rw-r--r--   0 root         (0) root         (0)    39235 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/roof_duality/src/fix_variables.cpp
+-rw-r--r--   0 root         (0) root         (0)     1354 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/roof_duality/src/fix_variables.hpp
+-rw-r--r--   0 root         (0) root         (0)    60264 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/sampleset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.568371 dimod-0.9.9/dimod/serialization/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/serialization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5084 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/serialization/coo.py
+-rw-r--r--   0 root         (0) root         (0)    22794 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/serialization/fileview.py
+-rw-r--r--   0 root         (0) root         (0)    14181 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/serialization/format.py
+-rw-r--r--   0 root         (0) root         (0)     3393 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/serialization/json.py
+-rw-r--r--   0 root         (0) root         (0)     4542 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/serialization/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.568371 dimod-0.9.9/dimod/testing/
+-rw-r--r--   0 root         (0) root         (0)     1001 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12199 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/testing/asserts.py
+-rw-r--r--   0 root         (0) root         (0)     7871 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/testing/sampler.py
+-rw-r--r--   0 root         (0) root         (0)     3841 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/traversal.py
+-rw-r--r--   0 root         (0) root         (0)    15878 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     4513 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/variables.py
+-rw-r--r--   0 root         (0) root         (0)     4678 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/vartypes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.568371 dimod-0.9.9/dimod/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4607 2020-10-06 01:35:23.000000 dimod-0.9.9/dimod/views/samples.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-06 01:40:38.544370 dimod-0.9.9/dimod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3772 2020-10-06 01:40:38.000000 dimod-0.9.9/dimod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3149 2020-10-06 01:40:38.000000 dimod-0.9.9/dimod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-10-06 01:40:38.000000 dimod-0.9.9/dimod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-10-06 01:36:52.000000 dimod-0.9.9/dimod.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       92 2020-10-06 01:40:38.000000 dimod-0.9.9/dimod.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2020-10-06 01:40:38.000000 dimod-0.9.9/dimod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2020-10-06 01:40:38.568371 dimod-0.9.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     5619 2020-10-06 01:35:24.000000 dimod-0.9.9/setup.py
```

### Comparing `dimod-0.9.8/PKG-INFO` & `dimod-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimod
-Version: 0.9.8
+Version: 0.9.9
 Summary: A shared API for binary quadratic model samplers.
 Home-page: https://github.com/dwavesystems/dimod
 Author: D-Wave Systems Inc.
 Author-email: acondello@dwavesys.com
 License: Apache 2.0
 Download-URL: https://github.com/dwavesystems/dimod/releases
 Description: .. image:: https://img.shields.io/pypi/v/dimod.svg
```

### Comparing `dimod-0.9.8/README.rst` & `dimod-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/__init__.pxd` & `dimod-0.9.9/dimod/__init__.pxd`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/__init__.py` & `dimod-0.9.9/dimod/__init__.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/binary_quadratic_model.py` & `dimod-0.9.9/dimod/binary_quadratic_model.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/__init__.pxd` & `dimod-0.9.9/dimod/bqm/__init__.pxd`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/__init__.py` & `dimod-0.9.9/dimod/bqm/__init__.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/adjarraybqm.cpp` & `dimod-0.9.9/dimod/bqm/adjarraybqm.cpp`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/adjarraybqm.pxd` & `dimod-0.9.9/dimod/bqm/adjarraybqm.pxd`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/adjarraybqm.pyx` & `dimod-0.9.9/dimod/bqm/adjarraybqm.pyx`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/adjdictbqm.py` & `dimod-0.9.9/dimod/bqm/adjdictbqm.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/adjmapbqm.cpp` & `dimod-0.9.9/dimod/bqm/adjmapbqm.cpp`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/adjmapbqm.pxd` & `dimod-0.9.9/dimod/bqm/adjmapbqm.pxd`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/adjmapbqm.pyx` & `dimod-0.9.9/dimod/bqm/adjmapbqm.pyx`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/adjvectorbqm.cpp` & `dimod-0.9.9/dimod/bqm/adjvectorbqm.cpp`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/adjvectorbqm.pxd` & `dimod-0.9.9/dimod/bqm/adjvectorbqm.pxd`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/adjvectorbqm.pyx` & `dimod-0.9.9/dimod/bqm/adjvectorbqm.pyx`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/common.cpp` & `dimod-0.9.9/dimod/bqm/common.cpp`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/common.pxd` & `dimod-0.9.9/dimod/bqm/common.pxd`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/common.pyx` & `dimod-0.9.9/dimod/bqm/common.pyx`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/construction.py` & `dimod-0.9.9/dimod/bqm/construction.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/cppbqm.pxd` & `dimod-0.9.9/dimod/bqm/cppbqm.pxd`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/make.py` & `dimod-0.9.9/dimod/bqm/make.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/shapeablebqm.pyx.src` & `dimod-0.9.9/dimod/bqm/shapeablebqm.pyx.src`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/utils.cpp` & `dimod-0.9.9/dimod/bqm/utils.cpp`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/utils.pxd` & `dimod-0.9.9/dimod/bqm/utils.pxd`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/bqm/utils.pyx` & `dimod-0.9.9/dimod/bqm/utils.pyx`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/compatibility23.py` & `dimod-0.9.9/dimod/compatibility23.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/converters.py` & `dimod-0.9.9/dimod/converters.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/core/__init__.py` & `dimod-0.9.9/dimod/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/core/bqm.py` & `dimod-0.9.9/dimod/core/bqm.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/core/composite.py` & `dimod-0.9.9/dimod/core/composite.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/core/initialized.py` & `dimod-0.9.9/dimod/core/initialized.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/core/polysampler.py` & `dimod-0.9.9/dimod/core/polysampler.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/core/sampler.py` & `dimod-0.9.9/dimod/core/sampler.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/core/structured.py` & `dimod-0.9.9/dimod/core/structured.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/decorators.py` & `dimod-0.9.9/dimod/decorators.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/discrete/__init__.py` & `dimod-0.9.9/dimod/discrete/__init__.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/discrete/cydiscrete_quadratic_model.cpp` & `dimod-0.9.9/dimod/discrete/cydiscrete_quadratic_model.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -4392,31 +4392,38 @@
   Py_ssize_t __pyx_v_u;
   Py_ssize_t __pyx_v_v;
   Py_ssize_t __pyx_v_ci;
   Py_ssize_t __pyx_v_cj;
   Py_ssize_t __pyx_v_nc;
   int __pyx_v_is_sorted;
   Py_ssize_t __pyx_v_qi;
+  __Pyx_memviewslice __pyx_v_degrees = { 0, 0, { 0 }, { 0 }, { 0 } };
   std::vector<std::unordered_set<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> >  __pyx_v_adjset;
   std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_v_span;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   Py_ssize_t __pyx_t_8;
   int __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_11;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_12;
-  std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_t_13;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_14;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_13 = NULL;
+  __Pyx_memviewslice __pyx_t_14 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  size_t __pyx_t_15;
+  Py_ssize_t __pyx_t_16;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_17;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_18;
+  std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_t_19;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_20;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_0_from_numpy_vectors", 0);
 
   /* "dimod/discrete/cydiscrete_quadratic_model.pyx":125
  * 
@@ -4728,391 +4735,488 @@
       __pyx_v_is_sorted = 0;
 
       /* "dimod/discrete/cydiscrete_quadratic_model.pyx":163
  *             if irow[qi] == irow[qi + 1] and icol[qi] >= icol[qi+1]:
  *                 is_sorted = False
  *                 break             # <<<<<<<<<<<<<<
  * 
- *         if is_sorted:
+ * 
  */
       goto __pyx_L12_break;
 
       /* "dimod/discrete/cydiscrete_quadratic_model.pyx":161
  *                 break
  * 
  *             if irow[qi] == irow[qi + 1] and icol[qi] >= icol[qi+1]:             # <<<<<<<<<<<<<<
  *                 is_sorted = False
  *                 break
  */
     }
   }
   __pyx_L12_break:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":165
- *                 break
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":168
+ *         # reserve the memory for the vectors, this helps use less memory
+ *         # and speeds things up
+ *         cdef np.uint64_t[:] degrees = np.zeros(num_cases, dtype=np.uint64)             # <<<<<<<<<<<<<<
+ * 
+ *         for qi in range(num_interactions):
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_zeros); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_num_cases); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_11 = PyTuple_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_GIVEREF(__pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_7);
+  __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_12);
+  __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_uint64); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_13) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_11, __pyx_t_7); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_14 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_t_13, PyBUF_WRITABLE); if (unlikely(!__pyx_t_14.memview)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_v_degrees = __pyx_t_14;
+  __pyx_t_14.memview = NULL;
+  __pyx_t_14.data = NULL;
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":170
+ *         cdef np.uint64_t[:] degrees = np.zeros(num_cases, dtype=np.uint64)
+ * 
+ *         for qi in range(num_interactions):             # <<<<<<<<<<<<<<
+ *             degrees[irow[qi]] += 1
+ *             degrees[icol[qi]] += 1
+ */
+  __pyx_t_1 = __pyx_v_num_interactions;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_qi = __pyx_t_3;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":171
+ * 
+ *         for qi in range(num_interactions):
+ *             degrees[irow[qi]] += 1             # <<<<<<<<<<<<<<
+ *             degrees[icol[qi]] += 1
+ * 
+ */
+    __pyx_t_4 = __pyx_v_qi;
+    __pyx_t_15 = (*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )));
+    *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_15 * __pyx_v_degrees.strides[0]) )) += 1;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":172
+ *         for qi in range(num_interactions):
+ *             degrees[irow[qi]] += 1
+ *             degrees[icol[qi]] += 1             # <<<<<<<<<<<<<<
+ * 
+ *         for ci in range(num_cases):
+ */
+    __pyx_t_4 = __pyx_v_qi;
+    __pyx_t_15 = (*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )));
+    *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_15 * __pyx_v_degrees.strides[0]) )) += 1;
+  }
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+ *             degrees[icol[qi]] += 1
+ * 
+ *         for ci in range(num_cases):             # <<<<<<<<<<<<<<
+ *             self.bqm_.adj[ci].first.reserve(degrees[ci])
+ * 
+ */
+  __pyx_t_1 = __pyx_v_num_cases;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_ci = __pyx_t_3;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":175
  * 
+ *         for ci in range(num_cases):
+ *             self.bqm_.adj[ci].first.reserve(degrees[ci])             # <<<<<<<<<<<<<<
+ * 
+ *         # set the quadratic
+ */
+    __pyx_t_4 = __pyx_v_ci;
+    (__pyx_v_self->bqm_.adj[__pyx_v_ci]).first.reserve((*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_4 * __pyx_v_degrees.strides[0]) ))));
+  }
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":178
+ * 
+ *         # set the quadratic
  *         if is_sorted:             # <<<<<<<<<<<<<<
  *             for qi in range(num_interactions):
  *                 # cython really has a hard time with push_back so we do this
  */
   __pyx_t_9 = (__pyx_v_is_sorted != 0);
   if (__pyx_t_9) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":166
- * 
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":179
+ *         # set the quadratic
  *         if is_sorted:
  *             for qi in range(num_interactions):             # <<<<<<<<<<<<<<
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  */
     __pyx_t_1 = __pyx_v_num_interactions;
     __pyx_t_2 = __pyx_t_1;
     for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
       __pyx_v_qi = __pyx_t_3;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":169
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  */
       __pyx_t_4 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":170
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":183
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  */
       __pyx_t_5 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":169
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  */
       try {
         (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )))]).first.resize(((__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_5 * __pyx_v_irow.strides[0]) )))]).first.size() + 1));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 169, __pyx_L1_error)
+        __PYX_ERR(0, 182, __pyx_L1_error)
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":171
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":184
  *                 self.bqm_.adj[irow[qi]].first.resize(
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  */
       __pyx_t_5 = __pyx_v_qi;
       __pyx_t_4 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )))]).first.back().first = (*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":172
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":185
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]             # <<<<<<<<<<<<<<
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_5 * __pyx_v_irow.strides[0]) )))]).first.back().second = (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_4 * __pyx_v_qdata.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":187
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  */
       __pyx_t_5 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":175
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":188
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]
  */
       __pyx_t_4 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":187
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  */
       try {
         (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )))]).first.resize(((__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )))]).first.size() + 1));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 174, __pyx_L1_error)
+        __PYX_ERR(0, 187, __pyx_L1_error)
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":176
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":189
  *                 self.bqm_.adj[icol[qi]].first.resize(
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]
  * 
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )))]).first.back().first = (*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":177
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":190
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]             # <<<<<<<<<<<<<<
  * 
  *         else:
  */
       __pyx_t_5 = __pyx_v_qi;
       __pyx_t_4 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )))]).first.back().second = (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_5 * __pyx_v_qdata.strides[0]) )));
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":165
- *                 break
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":178
  * 
+ *         # set the quadratic
  *         if is_sorted:             # <<<<<<<<<<<<<<
  *             for qi in range(num_interactions):
  *                 # cython really has a hard time with push_back so we do this
  */
-    goto __pyx_L17;
+    goto __pyx_L21;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":195
  *             # this is *much* slower, an alternative would be to make a copy
  *             # and then sort but for now let's stick with the simple thing
  *             for qi in range(num_interactions):             # <<<<<<<<<<<<<<
  *                 self.bqm_.set_quadratic(irow[qi], icol[qi], qdata[qi])
  * 
  */
   /*else*/ {
     __pyx_t_1 = __pyx_v_num_interactions;
     __pyx_t_2 = __pyx_t_1;
     for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
       __pyx_v_qi = __pyx_t_3;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":183
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":196
  *             # and then sort but for now let's stick with the simple thing
  *             for qi in range(num_interactions):
  *                 self.bqm_.set_quadratic(irow[qi], icol[qi], qdata[qi])             # <<<<<<<<<<<<<<
  * 
  *         # build the adj. This is not really the memory bottleneck so
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
-      __pyx_t_10 = __pyx_v_qi;
+      __pyx_t_16 = __pyx_v_qi;
       try {
-        __pyx_v_self->bqm_.set_quadratic((*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) ))), (*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) ))), (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_10 * __pyx_v_qdata.strides[0]) ))));
+        __pyx_v_self->bqm_.set_quadratic((*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) ))), (*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) ))), (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_16 * __pyx_v_qdata.strides[0]) ))));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 183, __pyx_L1_error)
+        __PYX_ERR(0, 196, __pyx_L1_error)
       }
     }
   }
-  __pyx_L17:;
+  __pyx_L21:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":188
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":201
  *         # we can build an intermediate (unordered) set version
  *         cdef vector[unordered_set[VarIndex]] adjset
  *         adjset.resize(num_variables)             # <<<<<<<<<<<<<<
  *         u = 0
  *         for ci in range(self.bqm_.num_variables()):
  */
   try {
     __pyx_v_adjset.resize(__pyx_v_num_variables);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 188, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":189
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":202
  *         cdef vector[unordered_set[VarIndex]] adjset
  *         adjset.resize(num_variables)
  *         u = 0             # <<<<<<<<<<<<<<
  *         for ci in range(self.bqm_.num_variables()):
  * 
  */
   __pyx_v_u = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":190
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":203
  *         adjset.resize(num_variables)
  *         u = 0
  *         for ci in range(self.bqm_.num_variables()):             # <<<<<<<<<<<<<<
  * 
  *             # we've been careful so don't need ui < case_starts.size() - 1
  */
   try {
-    __pyx_t_11 = __pyx_v_self->bqm_.num_variables();
+    __pyx_t_17 = __pyx_v_self->bqm_.num_variables();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 190, __pyx_L1_error)
+    __PYX_ERR(0, 203, __pyx_L1_error)
   }
-  __pyx_t_12 = __pyx_t_11;
-  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_12; __pyx_t_1+=1) {
+  __pyx_t_18 = __pyx_t_17;
+  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_18; __pyx_t_1+=1) {
     __pyx_v_ci = __pyx_t_1;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":193
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":206
  * 
  *             # we've been careful so don't need ui < case_starts.size() - 1
  *             while ci >= self.case_starts_[u+1]:             # <<<<<<<<<<<<<<
  *                 u += 1
  * 
  */
     while (1) {
       __pyx_t_9 = ((__pyx_v_ci >= (__pyx_v_self->case_starts_[(__pyx_v_u + 1)])) != 0);
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":194
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":207
  *             # we've been careful so don't need ui < case_starts.size() - 1
  *             while ci >= self.case_starts_[u+1]:
  *                 u += 1             # <<<<<<<<<<<<<<
  * 
  *             span = self.bqm_.neighborhood(ci)
  */
       __pyx_v_u = (__pyx_v_u + 1);
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":196
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":209
  *                 u += 1
  * 
  *             span = self.bqm_.neighborhood(ci)             # <<<<<<<<<<<<<<
  * 
  *             v = 0
  */
     try {
-      __pyx_t_13 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
+      __pyx_t_19 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 196, __pyx_L1_error)
+      __PYX_ERR(0, 209, __pyx_L1_error)
     }
-    __pyx_v_span = __pyx_t_13;
+    __pyx_v_span = __pyx_t_19;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":198
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":211
  *             span = self.bqm_.neighborhood(ci)
  * 
  *             v = 0             # <<<<<<<<<<<<<<
  *             while span.first != span.second:
  *                 cj = deref(span.first).first
  */
     __pyx_v_v = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":199
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":212
  * 
  *             v = 0
  *             while span.first != span.second:             # <<<<<<<<<<<<<<
  *                 cj = deref(span.first).first
  * 
  */
     while (1) {
       __pyx_t_9 = ((__pyx_v_span.first != __pyx_v_span.second) != 0);
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":200
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":213
  *             v = 0
  *             while span.first != span.second:
  *                 cj = deref(span.first).first             # <<<<<<<<<<<<<<
  * 
  *                 # see above note
  */
-      __pyx_t_14 = (*__pyx_v_span.first).first;
-      __pyx_v_cj = __pyx_t_14;
+      __pyx_t_20 = (*__pyx_v_span.first).first;
+      __pyx_v_cj = __pyx_t_20;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":203
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":216
  * 
  *                 # see above note
  *                 while cj >= self.case_starts_[v+1]:             # <<<<<<<<<<<<<<
  *                     v += 1
  * 
  */
       while (1) {
         __pyx_t_9 = ((__pyx_v_cj >= (__pyx_v_self->case_starts_[(__pyx_v_v + 1)])) != 0);
         if (!__pyx_t_9) break;
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":204
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":217
  *                 # see above note
  *                 while cj >= self.case_starts_[v+1]:
  *                     v += 1             # <<<<<<<<<<<<<<
  * 
  *                 adjset[u].insert(v)
  */
         __pyx_v_v = (__pyx_v_v + 1);
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":206
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":219
  *                     v += 1
  * 
  *                 adjset[u].insert(v)             # <<<<<<<<<<<<<<
  * 
  *                 inc(span.first)
  */
       (void)((__pyx_v_adjset[__pyx_v_u]).insert(__pyx_v_v));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":208
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":221
  *                 adjset[u].insert(v)
  * 
  *                 inc(span.first)             # <<<<<<<<<<<<<<
  * 
  *         # now put adjset into adj
  */
       (void)((++__pyx_v_span.first));
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":211
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":224
  * 
  *         # now put adjset into adj
  *         self.adj_.resize(num_variables)             # <<<<<<<<<<<<<<
  *         for v in range(num_variables):
  *             self.adj_[v].insert(self.adj_[v].begin(),
  */
   try {
     __pyx_v_self->adj_.resize(__pyx_v_num_variables);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 211, __pyx_L1_error)
+    __PYX_ERR(0, 224, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":212
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":225
  *         # now put adjset into adj
  *         self.adj_.resize(num_variables)
  *         for v in range(num_variables):             # <<<<<<<<<<<<<<
  *             self.adj_[v].insert(self.adj_[v].begin(),
  *                                 adjset[v].begin(), adjset[v].end())
  */
   __pyx_t_1 = __pyx_v_num_variables;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_v = __pyx_t_3;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":213
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":226
  *         self.adj_.resize(num_variables)
  *         for v in range(num_variables):
  *             self.adj_[v].insert(self.adj_[v].begin(),             # <<<<<<<<<<<<<<
  *                                 adjset[v].begin(), adjset[v].end())
  *             sort(self.adj_[v].begin(), self.adj_[v].end())
  */
     try {
       (__pyx_v_self->adj_[__pyx_v_v]).insert((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_adjset[__pyx_v_v]).begin(), (__pyx_v_adjset[__pyx_v_v]).end());
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 213, __pyx_L1_error)
+      __PYX_ERR(0, 226, __pyx_L1_error)
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":215
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":228
  *             self.adj_[v].insert(self.adj_[v].begin(),
  *                                 adjset[v].begin(), adjset[v].end())
  *             sort(self.adj_[v].begin(), self.adj_[v].end())             # <<<<<<<<<<<<<<
  * 
  *     @classmethod
  */
     std::sort<std::vector<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> ::iterator>((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_self->adj_[__pyx_v_v]).end());
@@ -5126,47 +5230,60 @@
  *                                   Bias[:] qdata) except *:
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_13);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_14, 1);
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel._from_numpy_vectors", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
+  __PYX_XDEC_MEMVIEW(&__pyx_v_degrees, 1);
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_1__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel__from_numpy_vectors(struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *__pyx_v_self, __Pyx_memviewslice __pyx_v_starts, __Pyx_memviewslice __pyx_v_ldata, __Pyx_memviewslice __pyx_v_irow, __Pyx_memviewslice __pyx_v_icol, __Pyx_memviewslice __pyx_v_qdata) {
   Py_ssize_t __pyx_v_num_variables;
   Py_ssize_t __pyx_v_num_cases;
   Py_ssize_t __pyx_v_num_interactions;
   Py_ssize_t __pyx_v_u;
   Py_ssize_t __pyx_v_v;
   Py_ssize_t __pyx_v_ci;
   Py_ssize_t __pyx_v_cj;
   Py_ssize_t __pyx_v_nc;
   int __pyx_v_is_sorted;
   Py_ssize_t __pyx_v_qi;
+  __Pyx_memviewslice __pyx_v_degrees = { 0, 0, { 0 }, { 0 }, { 0 } };
   std::vector<std::unordered_set<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> >  __pyx_v_adjset;
   std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_v_span;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   Py_ssize_t __pyx_t_8;
   int __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_11;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_12;
-  std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_t_13;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_14;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_13 = NULL;
+  __Pyx_memviewslice __pyx_t_14 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  size_t __pyx_t_15;
+  Py_ssize_t __pyx_t_16;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_17;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_18;
+  std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_t_19;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_20;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_1_from_numpy_vectors", 0);
 
   /* "dimod/discrete/cydiscrete_quadratic_model.pyx":125
  * 
@@ -5478,391 +5595,488 @@
       __pyx_v_is_sorted = 0;
 
       /* "dimod/discrete/cydiscrete_quadratic_model.pyx":163
  *             if irow[qi] == irow[qi + 1] and icol[qi] >= icol[qi+1]:
  *                 is_sorted = False
  *                 break             # <<<<<<<<<<<<<<
  * 
- *         if is_sorted:
+ * 
  */
       goto __pyx_L12_break;
 
       /* "dimod/discrete/cydiscrete_quadratic_model.pyx":161
  *                 break
  * 
  *             if irow[qi] == irow[qi + 1] and icol[qi] >= icol[qi+1]:             # <<<<<<<<<<<<<<
  *                 is_sorted = False
  *                 break
  */
     }
   }
   __pyx_L12_break:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":165
- *                 break
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":168
+ *         # reserve the memory for the vectors, this helps use less memory
+ *         # and speeds things up
+ *         cdef np.uint64_t[:] degrees = np.zeros(num_cases, dtype=np.uint64)             # <<<<<<<<<<<<<<
+ * 
+ *         for qi in range(num_interactions):
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_zeros); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_num_cases); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_11 = PyTuple_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_GIVEREF(__pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_7);
+  __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_12);
+  __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_uint64); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_13) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_11, __pyx_t_7); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_14 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_t_13, PyBUF_WRITABLE); if (unlikely(!__pyx_t_14.memview)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_v_degrees = __pyx_t_14;
+  __pyx_t_14.memview = NULL;
+  __pyx_t_14.data = NULL;
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":170
+ *         cdef np.uint64_t[:] degrees = np.zeros(num_cases, dtype=np.uint64)
+ * 
+ *         for qi in range(num_interactions):             # <<<<<<<<<<<<<<
+ *             degrees[irow[qi]] += 1
+ *             degrees[icol[qi]] += 1
+ */
+  __pyx_t_1 = __pyx_v_num_interactions;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_qi = __pyx_t_3;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":171
+ * 
+ *         for qi in range(num_interactions):
+ *             degrees[irow[qi]] += 1             # <<<<<<<<<<<<<<
+ *             degrees[icol[qi]] += 1
+ * 
+ */
+    __pyx_t_4 = __pyx_v_qi;
+    __pyx_t_15 = (*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )));
+    *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_15 * __pyx_v_degrees.strides[0]) )) += 1;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":172
+ *         for qi in range(num_interactions):
+ *             degrees[irow[qi]] += 1
+ *             degrees[icol[qi]] += 1             # <<<<<<<<<<<<<<
+ * 
+ *         for ci in range(num_cases):
+ */
+    __pyx_t_4 = __pyx_v_qi;
+    __pyx_t_15 = (*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )));
+    *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_15 * __pyx_v_degrees.strides[0]) )) += 1;
+  }
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+ *             degrees[icol[qi]] += 1
+ * 
+ *         for ci in range(num_cases):             # <<<<<<<<<<<<<<
+ *             self.bqm_.adj[ci].first.reserve(degrees[ci])
+ * 
+ */
+  __pyx_t_1 = __pyx_v_num_cases;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_ci = __pyx_t_3;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":175
  * 
+ *         for ci in range(num_cases):
+ *             self.bqm_.adj[ci].first.reserve(degrees[ci])             # <<<<<<<<<<<<<<
+ * 
+ *         # set the quadratic
+ */
+    __pyx_t_4 = __pyx_v_ci;
+    (__pyx_v_self->bqm_.adj[__pyx_v_ci]).first.reserve((*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_4 * __pyx_v_degrees.strides[0]) ))));
+  }
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":178
+ * 
+ *         # set the quadratic
  *         if is_sorted:             # <<<<<<<<<<<<<<
  *             for qi in range(num_interactions):
  *                 # cython really has a hard time with push_back so we do this
  */
   __pyx_t_9 = (__pyx_v_is_sorted != 0);
   if (__pyx_t_9) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":166
- * 
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":179
+ *         # set the quadratic
  *         if is_sorted:
  *             for qi in range(num_interactions):             # <<<<<<<<<<<<<<
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  */
     __pyx_t_1 = __pyx_v_num_interactions;
     __pyx_t_2 = __pyx_t_1;
     for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
       __pyx_v_qi = __pyx_t_3;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":169
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  */
       __pyx_t_4 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":170
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":183
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  */
       __pyx_t_5 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":169
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  */
       try {
         (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )))]).first.resize(((__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_5 * __pyx_v_irow.strides[0]) )))]).first.size() + 1));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 169, __pyx_L1_error)
+        __PYX_ERR(0, 182, __pyx_L1_error)
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":171
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":184
  *                 self.bqm_.adj[irow[qi]].first.resize(
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  */
       __pyx_t_5 = __pyx_v_qi;
       __pyx_t_4 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )))]).first.back().first = (*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":172
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":185
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]             # <<<<<<<<<<<<<<
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_5 * __pyx_v_irow.strides[0]) )))]).first.back().second = (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_4 * __pyx_v_qdata.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":187
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  */
       __pyx_t_5 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":175
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":188
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]
  */
       __pyx_t_4 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":187
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  */
       try {
         (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )))]).first.resize(((__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )))]).first.size() + 1));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 174, __pyx_L1_error)
+        __PYX_ERR(0, 187, __pyx_L1_error)
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":176
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":189
  *                 self.bqm_.adj[icol[qi]].first.resize(
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]
  * 
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )))]).first.back().first = (*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":177
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":190
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]             # <<<<<<<<<<<<<<
  * 
  *         else:
  */
       __pyx_t_5 = __pyx_v_qi;
       __pyx_t_4 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )))]).first.back().second = (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_5 * __pyx_v_qdata.strides[0]) )));
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":165
- *                 break
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":178
  * 
+ *         # set the quadratic
  *         if is_sorted:             # <<<<<<<<<<<<<<
  *             for qi in range(num_interactions):
  *                 # cython really has a hard time with push_back so we do this
  */
-    goto __pyx_L17;
+    goto __pyx_L21;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":195
  *             # this is *much* slower, an alternative would be to make a copy
  *             # and then sort but for now let's stick with the simple thing
  *             for qi in range(num_interactions):             # <<<<<<<<<<<<<<
  *                 self.bqm_.set_quadratic(irow[qi], icol[qi], qdata[qi])
  * 
  */
   /*else*/ {
     __pyx_t_1 = __pyx_v_num_interactions;
     __pyx_t_2 = __pyx_t_1;
     for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
       __pyx_v_qi = __pyx_t_3;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":183
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":196
  *             # and then sort but for now let's stick with the simple thing
  *             for qi in range(num_interactions):
  *                 self.bqm_.set_quadratic(irow[qi], icol[qi], qdata[qi])             # <<<<<<<<<<<<<<
  * 
  *         # build the adj. This is not really the memory bottleneck so
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
-      __pyx_t_10 = __pyx_v_qi;
+      __pyx_t_16 = __pyx_v_qi;
       try {
-        __pyx_v_self->bqm_.set_quadratic((*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) ))), (*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) ))), (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_10 * __pyx_v_qdata.strides[0]) ))));
+        __pyx_v_self->bqm_.set_quadratic((*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) ))), (*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) ))), (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_16 * __pyx_v_qdata.strides[0]) ))));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 183, __pyx_L1_error)
+        __PYX_ERR(0, 196, __pyx_L1_error)
       }
     }
   }
-  __pyx_L17:;
+  __pyx_L21:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":188
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":201
  *         # we can build an intermediate (unordered) set version
  *         cdef vector[unordered_set[VarIndex]] adjset
  *         adjset.resize(num_variables)             # <<<<<<<<<<<<<<
  *         u = 0
  *         for ci in range(self.bqm_.num_variables()):
  */
   try {
     __pyx_v_adjset.resize(__pyx_v_num_variables);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 188, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":189
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":202
  *         cdef vector[unordered_set[VarIndex]] adjset
  *         adjset.resize(num_variables)
  *         u = 0             # <<<<<<<<<<<<<<
  *         for ci in range(self.bqm_.num_variables()):
  * 
  */
   __pyx_v_u = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":190
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":203
  *         adjset.resize(num_variables)
  *         u = 0
  *         for ci in range(self.bqm_.num_variables()):             # <<<<<<<<<<<<<<
  * 
  *             # we've been careful so don't need ui < case_starts.size() - 1
  */
   try {
-    __pyx_t_11 = __pyx_v_self->bqm_.num_variables();
+    __pyx_t_17 = __pyx_v_self->bqm_.num_variables();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 190, __pyx_L1_error)
+    __PYX_ERR(0, 203, __pyx_L1_error)
   }
-  __pyx_t_12 = __pyx_t_11;
-  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_12; __pyx_t_1+=1) {
+  __pyx_t_18 = __pyx_t_17;
+  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_18; __pyx_t_1+=1) {
     __pyx_v_ci = __pyx_t_1;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":193
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":206
  * 
  *             # we've been careful so don't need ui < case_starts.size() - 1
  *             while ci >= self.case_starts_[u+1]:             # <<<<<<<<<<<<<<
  *                 u += 1
  * 
  */
     while (1) {
       __pyx_t_9 = ((__pyx_v_ci >= (__pyx_v_self->case_starts_[(__pyx_v_u + 1)])) != 0);
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":194
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":207
  *             # we've been careful so don't need ui < case_starts.size() - 1
  *             while ci >= self.case_starts_[u+1]:
  *                 u += 1             # <<<<<<<<<<<<<<
  * 
  *             span = self.bqm_.neighborhood(ci)
  */
       __pyx_v_u = (__pyx_v_u + 1);
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":196
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":209
  *                 u += 1
  * 
  *             span = self.bqm_.neighborhood(ci)             # <<<<<<<<<<<<<<
  * 
  *             v = 0
  */
     try {
-      __pyx_t_13 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
+      __pyx_t_19 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 196, __pyx_L1_error)
+      __PYX_ERR(0, 209, __pyx_L1_error)
     }
-    __pyx_v_span = __pyx_t_13;
+    __pyx_v_span = __pyx_t_19;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":198
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":211
  *             span = self.bqm_.neighborhood(ci)
  * 
  *             v = 0             # <<<<<<<<<<<<<<
  *             while span.first != span.second:
  *                 cj = deref(span.first).first
  */
     __pyx_v_v = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":199
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":212
  * 
  *             v = 0
  *             while span.first != span.second:             # <<<<<<<<<<<<<<
  *                 cj = deref(span.first).first
  * 
  */
     while (1) {
       __pyx_t_9 = ((__pyx_v_span.first != __pyx_v_span.second) != 0);
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":200
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":213
  *             v = 0
  *             while span.first != span.second:
  *                 cj = deref(span.first).first             # <<<<<<<<<<<<<<
  * 
  *                 # see above note
  */
-      __pyx_t_14 = (*__pyx_v_span.first).first;
-      __pyx_v_cj = __pyx_t_14;
+      __pyx_t_20 = (*__pyx_v_span.first).first;
+      __pyx_v_cj = __pyx_t_20;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":203
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":216
  * 
  *                 # see above note
  *                 while cj >= self.case_starts_[v+1]:             # <<<<<<<<<<<<<<
  *                     v += 1
  * 
  */
       while (1) {
         __pyx_t_9 = ((__pyx_v_cj >= (__pyx_v_self->case_starts_[(__pyx_v_v + 1)])) != 0);
         if (!__pyx_t_9) break;
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":204
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":217
  *                 # see above note
  *                 while cj >= self.case_starts_[v+1]:
  *                     v += 1             # <<<<<<<<<<<<<<
  * 
  *                 adjset[u].insert(v)
  */
         __pyx_v_v = (__pyx_v_v + 1);
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":206
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":219
  *                     v += 1
  * 
  *                 adjset[u].insert(v)             # <<<<<<<<<<<<<<
  * 
  *                 inc(span.first)
  */
       (void)((__pyx_v_adjset[__pyx_v_u]).insert(__pyx_v_v));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":208
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":221
  *                 adjset[u].insert(v)
  * 
  *                 inc(span.first)             # <<<<<<<<<<<<<<
  * 
  *         # now put adjset into adj
  */
       (void)((++__pyx_v_span.first));
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":211
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":224
  * 
  *         # now put adjset into adj
  *         self.adj_.resize(num_variables)             # <<<<<<<<<<<<<<
  *         for v in range(num_variables):
  *             self.adj_[v].insert(self.adj_[v].begin(),
  */
   try {
     __pyx_v_self->adj_.resize(__pyx_v_num_variables);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 211, __pyx_L1_error)
+    __PYX_ERR(0, 224, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":212
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":225
  *         # now put adjset into adj
  *         self.adj_.resize(num_variables)
  *         for v in range(num_variables):             # <<<<<<<<<<<<<<
  *             self.adj_[v].insert(self.adj_[v].begin(),
  *                                 adjset[v].begin(), adjset[v].end())
  */
   __pyx_t_1 = __pyx_v_num_variables;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_v = __pyx_t_3;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":213
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":226
  *         self.adj_.resize(num_variables)
  *         for v in range(num_variables):
  *             self.adj_[v].insert(self.adj_[v].begin(),             # <<<<<<<<<<<<<<
  *                                 adjset[v].begin(), adjset[v].end())
  *             sort(self.adj_[v].begin(), self.adj_[v].end())
  */
     try {
       (__pyx_v_self->adj_[__pyx_v_v]).insert((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_adjset[__pyx_v_v]).begin(), (__pyx_v_adjset[__pyx_v_v]).end());
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 213, __pyx_L1_error)
+      __PYX_ERR(0, 226, __pyx_L1_error)
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":215
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":228
  *             self.adj_[v].insert(self.adj_[v].begin(),
  *                                 adjset[v].begin(), adjset[v].end())
  *             sort(self.adj_[v].begin(), self.adj_[v].end())             # <<<<<<<<<<<<<<
  * 
  *     @classmethod
  */
     std::sort<std::vector<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> ::iterator>((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_self->adj_[__pyx_v_v]).end());
@@ -5876,47 +6090,60 @@
  *                                   Bias[:] qdata) except *:
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_13);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_14, 1);
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel._from_numpy_vectors", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
+  __PYX_XDEC_MEMVIEW(&__pyx_v_degrees, 1);
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_2__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel__from_numpy_vectors(struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *__pyx_v_self, __Pyx_memviewslice __pyx_v_starts, __Pyx_memviewslice __pyx_v_ldata, __Pyx_memviewslice __pyx_v_irow, __Pyx_memviewslice __pyx_v_icol, __Pyx_memviewslice __pyx_v_qdata) {
   Py_ssize_t __pyx_v_num_variables;
   Py_ssize_t __pyx_v_num_cases;
   Py_ssize_t __pyx_v_num_interactions;
   Py_ssize_t __pyx_v_u;
   Py_ssize_t __pyx_v_v;
   Py_ssize_t __pyx_v_ci;
   Py_ssize_t __pyx_v_cj;
   Py_ssize_t __pyx_v_nc;
   int __pyx_v_is_sorted;
   Py_ssize_t __pyx_v_qi;
+  __Pyx_memviewslice __pyx_v_degrees = { 0, 0, { 0 }, { 0 }, { 0 } };
   std::vector<std::unordered_set<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> >  __pyx_v_adjset;
   std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_v_span;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   Py_ssize_t __pyx_t_8;
   int __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_11;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_12;
-  std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_t_13;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_14;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_13 = NULL;
+  __Pyx_memviewslice __pyx_t_14 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  size_t __pyx_t_15;
+  Py_ssize_t __pyx_t_16;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_17;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_18;
+  std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_t_19;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_20;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_2_from_numpy_vectors", 0);
 
   /* "dimod/discrete/cydiscrete_quadratic_model.pyx":125
  * 
@@ -6228,391 +6455,488 @@
       __pyx_v_is_sorted = 0;
 
       /* "dimod/discrete/cydiscrete_quadratic_model.pyx":163
  *             if irow[qi] == irow[qi + 1] and icol[qi] >= icol[qi+1]:
  *                 is_sorted = False
  *                 break             # <<<<<<<<<<<<<<
  * 
- *         if is_sorted:
+ * 
  */
       goto __pyx_L12_break;
 
       /* "dimod/discrete/cydiscrete_quadratic_model.pyx":161
  *                 break
  * 
  *             if irow[qi] == irow[qi + 1] and icol[qi] >= icol[qi+1]:             # <<<<<<<<<<<<<<
  *                 is_sorted = False
  *                 break
  */
     }
   }
   __pyx_L12_break:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":165
- *                 break
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":168
+ *         # reserve the memory for the vectors, this helps use less memory
+ *         # and speeds things up
+ *         cdef np.uint64_t[:] degrees = np.zeros(num_cases, dtype=np.uint64)             # <<<<<<<<<<<<<<
+ * 
+ *         for qi in range(num_interactions):
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_zeros); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_num_cases); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_11 = PyTuple_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_GIVEREF(__pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_7);
+  __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_12);
+  __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_uint64); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_13) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_11, __pyx_t_7); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_14 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_t_13, PyBUF_WRITABLE); if (unlikely(!__pyx_t_14.memview)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_v_degrees = __pyx_t_14;
+  __pyx_t_14.memview = NULL;
+  __pyx_t_14.data = NULL;
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":170
+ *         cdef np.uint64_t[:] degrees = np.zeros(num_cases, dtype=np.uint64)
+ * 
+ *         for qi in range(num_interactions):             # <<<<<<<<<<<<<<
+ *             degrees[irow[qi]] += 1
+ *             degrees[icol[qi]] += 1
+ */
+  __pyx_t_1 = __pyx_v_num_interactions;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_qi = __pyx_t_3;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":171
+ * 
+ *         for qi in range(num_interactions):
+ *             degrees[irow[qi]] += 1             # <<<<<<<<<<<<<<
+ *             degrees[icol[qi]] += 1
+ * 
+ */
+    __pyx_t_4 = __pyx_v_qi;
+    __pyx_t_15 = (*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )));
+    *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_15 * __pyx_v_degrees.strides[0]) )) += 1;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":172
+ *         for qi in range(num_interactions):
+ *             degrees[irow[qi]] += 1
+ *             degrees[icol[qi]] += 1             # <<<<<<<<<<<<<<
+ * 
+ *         for ci in range(num_cases):
+ */
+    __pyx_t_4 = __pyx_v_qi;
+    __pyx_t_15 = (*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )));
+    *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_15 * __pyx_v_degrees.strides[0]) )) += 1;
+  }
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+ *             degrees[icol[qi]] += 1
+ * 
+ *         for ci in range(num_cases):             # <<<<<<<<<<<<<<
+ *             self.bqm_.adj[ci].first.reserve(degrees[ci])
  * 
+ */
+  __pyx_t_1 = __pyx_v_num_cases;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_ci = __pyx_t_3;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":175
+ * 
+ *         for ci in range(num_cases):
+ *             self.bqm_.adj[ci].first.reserve(degrees[ci])             # <<<<<<<<<<<<<<
+ * 
+ *         # set the quadratic
+ */
+    __pyx_t_4 = __pyx_v_ci;
+    (__pyx_v_self->bqm_.adj[__pyx_v_ci]).first.reserve((*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_4 * __pyx_v_degrees.strides[0]) ))));
+  }
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":178
+ * 
+ *         # set the quadratic
  *         if is_sorted:             # <<<<<<<<<<<<<<
  *             for qi in range(num_interactions):
  *                 # cython really has a hard time with push_back so we do this
  */
   __pyx_t_9 = (__pyx_v_is_sorted != 0);
   if (__pyx_t_9) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":166
- * 
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":179
+ *         # set the quadratic
  *         if is_sorted:
  *             for qi in range(num_interactions):             # <<<<<<<<<<<<<<
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  */
     __pyx_t_1 = __pyx_v_num_interactions;
     __pyx_t_2 = __pyx_t_1;
     for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
       __pyx_v_qi = __pyx_t_3;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":169
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  */
       __pyx_t_4 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":170
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":183
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  */
       __pyx_t_5 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":169
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  */
       try {
         (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )))]).first.resize(((__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_5 * __pyx_v_irow.strides[0]) )))]).first.size() + 1));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 169, __pyx_L1_error)
+        __PYX_ERR(0, 182, __pyx_L1_error)
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":171
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":184
  *                 self.bqm_.adj[irow[qi]].first.resize(
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  */
       __pyx_t_5 = __pyx_v_qi;
       __pyx_t_4 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )))]).first.back().first = (*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":172
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":185
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]             # <<<<<<<<<<<<<<
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_5 * __pyx_v_irow.strides[0]) )))]).first.back().second = (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_4 * __pyx_v_qdata.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":187
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  */
       __pyx_t_5 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":175
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":188
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]
  */
       __pyx_t_4 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":187
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  */
       try {
         (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )))]).first.resize(((__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )))]).first.size() + 1));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 174, __pyx_L1_error)
+        __PYX_ERR(0, 187, __pyx_L1_error)
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":176
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":189
  *                 self.bqm_.adj[icol[qi]].first.resize(
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]
  * 
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )))]).first.back().first = (*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":177
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":190
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]             # <<<<<<<<<<<<<<
  * 
  *         else:
  */
       __pyx_t_5 = __pyx_v_qi;
       __pyx_t_4 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )))]).first.back().second = (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_5 * __pyx_v_qdata.strides[0]) )));
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":165
- *                 break
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":178
  * 
+ *         # set the quadratic
  *         if is_sorted:             # <<<<<<<<<<<<<<
  *             for qi in range(num_interactions):
  *                 # cython really has a hard time with push_back so we do this
  */
-    goto __pyx_L17;
+    goto __pyx_L21;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":195
  *             # this is *much* slower, an alternative would be to make a copy
  *             # and then sort but for now let's stick with the simple thing
  *             for qi in range(num_interactions):             # <<<<<<<<<<<<<<
  *                 self.bqm_.set_quadratic(irow[qi], icol[qi], qdata[qi])
  * 
  */
   /*else*/ {
     __pyx_t_1 = __pyx_v_num_interactions;
     __pyx_t_2 = __pyx_t_1;
     for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
       __pyx_v_qi = __pyx_t_3;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":183
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":196
  *             # and then sort but for now let's stick with the simple thing
  *             for qi in range(num_interactions):
  *                 self.bqm_.set_quadratic(irow[qi], icol[qi], qdata[qi])             # <<<<<<<<<<<<<<
  * 
  *         # build the adj. This is not really the memory bottleneck so
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
-      __pyx_t_10 = __pyx_v_qi;
+      __pyx_t_16 = __pyx_v_qi;
       try {
-        __pyx_v_self->bqm_.set_quadratic((*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) ))), (*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) ))), (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_10 * __pyx_v_qdata.strides[0]) ))));
+        __pyx_v_self->bqm_.set_quadratic((*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) ))), (*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) ))), (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_16 * __pyx_v_qdata.strides[0]) ))));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 183, __pyx_L1_error)
+        __PYX_ERR(0, 196, __pyx_L1_error)
       }
     }
   }
-  __pyx_L17:;
+  __pyx_L21:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":188
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":201
  *         # we can build an intermediate (unordered) set version
  *         cdef vector[unordered_set[VarIndex]] adjset
  *         adjset.resize(num_variables)             # <<<<<<<<<<<<<<
  *         u = 0
  *         for ci in range(self.bqm_.num_variables()):
  */
   try {
     __pyx_v_adjset.resize(__pyx_v_num_variables);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 188, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":189
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":202
  *         cdef vector[unordered_set[VarIndex]] adjset
  *         adjset.resize(num_variables)
  *         u = 0             # <<<<<<<<<<<<<<
  *         for ci in range(self.bqm_.num_variables()):
  * 
  */
   __pyx_v_u = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":190
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":203
  *         adjset.resize(num_variables)
  *         u = 0
  *         for ci in range(self.bqm_.num_variables()):             # <<<<<<<<<<<<<<
  * 
  *             # we've been careful so don't need ui < case_starts.size() - 1
  */
   try {
-    __pyx_t_11 = __pyx_v_self->bqm_.num_variables();
+    __pyx_t_17 = __pyx_v_self->bqm_.num_variables();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 190, __pyx_L1_error)
+    __PYX_ERR(0, 203, __pyx_L1_error)
   }
-  __pyx_t_12 = __pyx_t_11;
-  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_12; __pyx_t_1+=1) {
+  __pyx_t_18 = __pyx_t_17;
+  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_18; __pyx_t_1+=1) {
     __pyx_v_ci = __pyx_t_1;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":193
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":206
  * 
  *             # we've been careful so don't need ui < case_starts.size() - 1
  *             while ci >= self.case_starts_[u+1]:             # <<<<<<<<<<<<<<
  *                 u += 1
  * 
  */
     while (1) {
       __pyx_t_9 = ((__pyx_v_ci >= (__pyx_v_self->case_starts_[(__pyx_v_u + 1)])) != 0);
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":194
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":207
  *             # we've been careful so don't need ui < case_starts.size() - 1
  *             while ci >= self.case_starts_[u+1]:
  *                 u += 1             # <<<<<<<<<<<<<<
  * 
  *             span = self.bqm_.neighborhood(ci)
  */
       __pyx_v_u = (__pyx_v_u + 1);
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":196
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":209
  *                 u += 1
  * 
  *             span = self.bqm_.neighborhood(ci)             # <<<<<<<<<<<<<<
  * 
  *             v = 0
  */
     try {
-      __pyx_t_13 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
+      __pyx_t_19 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 196, __pyx_L1_error)
+      __PYX_ERR(0, 209, __pyx_L1_error)
     }
-    __pyx_v_span = __pyx_t_13;
+    __pyx_v_span = __pyx_t_19;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":198
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":211
  *             span = self.bqm_.neighborhood(ci)
  * 
  *             v = 0             # <<<<<<<<<<<<<<
  *             while span.first != span.second:
  *                 cj = deref(span.first).first
  */
     __pyx_v_v = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":199
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":212
  * 
  *             v = 0
  *             while span.first != span.second:             # <<<<<<<<<<<<<<
  *                 cj = deref(span.first).first
  * 
  */
     while (1) {
       __pyx_t_9 = ((__pyx_v_span.first != __pyx_v_span.second) != 0);
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":200
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":213
  *             v = 0
  *             while span.first != span.second:
  *                 cj = deref(span.first).first             # <<<<<<<<<<<<<<
  * 
  *                 # see above note
  */
-      __pyx_t_14 = (*__pyx_v_span.first).first;
-      __pyx_v_cj = __pyx_t_14;
+      __pyx_t_20 = (*__pyx_v_span.first).first;
+      __pyx_v_cj = __pyx_t_20;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":203
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":216
  * 
  *                 # see above note
  *                 while cj >= self.case_starts_[v+1]:             # <<<<<<<<<<<<<<
  *                     v += 1
  * 
  */
       while (1) {
         __pyx_t_9 = ((__pyx_v_cj >= (__pyx_v_self->case_starts_[(__pyx_v_v + 1)])) != 0);
         if (!__pyx_t_9) break;
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":204
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":217
  *                 # see above note
  *                 while cj >= self.case_starts_[v+1]:
  *                     v += 1             # <<<<<<<<<<<<<<
  * 
  *                 adjset[u].insert(v)
  */
         __pyx_v_v = (__pyx_v_v + 1);
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":206
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":219
  *                     v += 1
  * 
  *                 adjset[u].insert(v)             # <<<<<<<<<<<<<<
  * 
  *                 inc(span.first)
  */
       (void)((__pyx_v_adjset[__pyx_v_u]).insert(__pyx_v_v));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":208
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":221
  *                 adjset[u].insert(v)
  * 
  *                 inc(span.first)             # <<<<<<<<<<<<<<
  * 
  *         # now put adjset into adj
  */
       (void)((++__pyx_v_span.first));
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":211
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":224
  * 
  *         # now put adjset into adj
  *         self.adj_.resize(num_variables)             # <<<<<<<<<<<<<<
  *         for v in range(num_variables):
  *             self.adj_[v].insert(self.adj_[v].begin(),
  */
   try {
     __pyx_v_self->adj_.resize(__pyx_v_num_variables);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 211, __pyx_L1_error)
+    __PYX_ERR(0, 224, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":212
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":225
  *         # now put adjset into adj
  *         self.adj_.resize(num_variables)
  *         for v in range(num_variables):             # <<<<<<<<<<<<<<
  *             self.adj_[v].insert(self.adj_[v].begin(),
  *                                 adjset[v].begin(), adjset[v].end())
  */
   __pyx_t_1 = __pyx_v_num_variables;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_v = __pyx_t_3;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":213
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":226
  *         self.adj_.resize(num_variables)
  *         for v in range(num_variables):
  *             self.adj_[v].insert(self.adj_[v].begin(),             # <<<<<<<<<<<<<<
  *                                 adjset[v].begin(), adjset[v].end())
  *             sort(self.adj_[v].begin(), self.adj_[v].end())
  */
     try {
       (__pyx_v_self->adj_[__pyx_v_v]).insert((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_adjset[__pyx_v_v]).begin(), (__pyx_v_adjset[__pyx_v_v]).end());
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 213, __pyx_L1_error)
+      __PYX_ERR(0, 226, __pyx_L1_error)
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":215
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":228
  *             self.adj_[v].insert(self.adj_[v].begin(),
  *                                 adjset[v].begin(), adjset[v].end())
  *             sort(self.adj_[v].begin(), self.adj_[v].end())             # <<<<<<<<<<<<<<
  * 
  *     @classmethod
  */
     std::sort<std::vector<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> ::iterator>((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_self->adj_[__pyx_v_v]).end());
@@ -6626,47 +6950,60 @@
  *                                   Bias[:] qdata) except *:
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_13);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_14, 1);
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel._from_numpy_vectors", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
+  __PYX_XDEC_MEMVIEW(&__pyx_v_degrees, 1);
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_3__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel__from_numpy_vectors(struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *__pyx_v_self, __Pyx_memviewslice __pyx_v_starts, __Pyx_memviewslice __pyx_v_ldata, __Pyx_memviewslice __pyx_v_irow, __Pyx_memviewslice __pyx_v_icol, __Pyx_memviewslice __pyx_v_qdata) {
   Py_ssize_t __pyx_v_num_variables;
   Py_ssize_t __pyx_v_num_cases;
   Py_ssize_t __pyx_v_num_interactions;
   Py_ssize_t __pyx_v_u;
   Py_ssize_t __pyx_v_v;
   Py_ssize_t __pyx_v_ci;
   Py_ssize_t __pyx_v_cj;
   Py_ssize_t __pyx_v_nc;
   int __pyx_v_is_sorted;
   Py_ssize_t __pyx_v_qi;
+  __Pyx_memviewslice __pyx_v_degrees = { 0, 0, { 0 }, { 0 }, { 0 } };
   std::vector<std::unordered_set<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> >  __pyx_v_adjset;
   std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_v_span;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   Py_ssize_t __pyx_t_8;
   int __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_11;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_12;
-  std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_t_13;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_14;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_13 = NULL;
+  __Pyx_memviewslice __pyx_t_14 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __pyx_t_5numpy_uint64_t __pyx_t_15;
+  Py_ssize_t __pyx_t_16;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_17;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_18;
+  std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_t_19;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_20;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_3_from_numpy_vectors", 0);
 
   /* "dimod/discrete/cydiscrete_quadratic_model.pyx":125
  * 
@@ -6978,391 +7315,488 @@
       __pyx_v_is_sorted = 0;
 
       /* "dimod/discrete/cydiscrete_quadratic_model.pyx":163
  *             if irow[qi] == irow[qi + 1] and icol[qi] >= icol[qi+1]:
  *                 is_sorted = False
  *                 break             # <<<<<<<<<<<<<<
  * 
- *         if is_sorted:
+ * 
  */
       goto __pyx_L12_break;
 
       /* "dimod/discrete/cydiscrete_quadratic_model.pyx":161
  *                 break
  * 
  *             if irow[qi] == irow[qi + 1] and icol[qi] >= icol[qi+1]:             # <<<<<<<<<<<<<<
  *                 is_sorted = False
  *                 break
  */
     }
   }
   __pyx_L12_break:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":165
- *                 break
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":168
+ *         # reserve the memory for the vectors, this helps use less memory
+ *         # and speeds things up
+ *         cdef np.uint64_t[:] degrees = np.zeros(num_cases, dtype=np.uint64)             # <<<<<<<<<<<<<<
+ * 
+ *         for qi in range(num_interactions):
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_zeros); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_num_cases); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_11 = PyTuple_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_GIVEREF(__pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_7);
+  __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_12);
+  __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_uint64); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_13) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_11, __pyx_t_7); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_14 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_t_13, PyBUF_WRITABLE); if (unlikely(!__pyx_t_14.memview)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_v_degrees = __pyx_t_14;
+  __pyx_t_14.memview = NULL;
+  __pyx_t_14.data = NULL;
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":170
+ *         cdef np.uint64_t[:] degrees = np.zeros(num_cases, dtype=np.uint64)
+ * 
+ *         for qi in range(num_interactions):             # <<<<<<<<<<<<<<
+ *             degrees[irow[qi]] += 1
+ *             degrees[icol[qi]] += 1
+ */
+  __pyx_t_1 = __pyx_v_num_interactions;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_qi = __pyx_t_3;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":171
+ * 
+ *         for qi in range(num_interactions):
+ *             degrees[irow[qi]] += 1             # <<<<<<<<<<<<<<
+ *             degrees[icol[qi]] += 1
+ * 
+ */
+    __pyx_t_4 = __pyx_v_qi;
+    __pyx_t_15 = (*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )));
+    *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_15 * __pyx_v_degrees.strides[0]) )) += 1;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":172
+ *         for qi in range(num_interactions):
+ *             degrees[irow[qi]] += 1
+ *             degrees[icol[qi]] += 1             # <<<<<<<<<<<<<<
+ * 
+ *         for ci in range(num_cases):
+ */
+    __pyx_t_4 = __pyx_v_qi;
+    __pyx_t_15 = (*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )));
+    *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_15 * __pyx_v_degrees.strides[0]) )) += 1;
+  }
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+ *             degrees[icol[qi]] += 1
+ * 
+ *         for ci in range(num_cases):             # <<<<<<<<<<<<<<
+ *             self.bqm_.adj[ci].first.reserve(degrees[ci])
  * 
+ */
+  __pyx_t_1 = __pyx_v_num_cases;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_ci = __pyx_t_3;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":175
+ * 
+ *         for ci in range(num_cases):
+ *             self.bqm_.adj[ci].first.reserve(degrees[ci])             # <<<<<<<<<<<<<<
+ * 
+ *         # set the quadratic
+ */
+    __pyx_t_4 = __pyx_v_ci;
+    (__pyx_v_self->bqm_.adj[__pyx_v_ci]).first.reserve((*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_4 * __pyx_v_degrees.strides[0]) ))));
+  }
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":178
+ * 
+ *         # set the quadratic
  *         if is_sorted:             # <<<<<<<<<<<<<<
  *             for qi in range(num_interactions):
  *                 # cython really has a hard time with push_back so we do this
  */
   __pyx_t_9 = (__pyx_v_is_sorted != 0);
   if (__pyx_t_9) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":166
- * 
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":179
+ *         # set the quadratic
  *         if is_sorted:
  *             for qi in range(num_interactions):             # <<<<<<<<<<<<<<
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  */
     __pyx_t_1 = __pyx_v_num_interactions;
     __pyx_t_2 = __pyx_t_1;
     for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
       __pyx_v_qi = __pyx_t_3;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":169
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  */
       __pyx_t_4 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":170
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":183
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  */
       __pyx_t_5 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":169
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  */
       try {
         (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )))]).first.resize(((__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_5 * __pyx_v_irow.strides[0]) )))]).first.size() + 1));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 169, __pyx_L1_error)
+        __PYX_ERR(0, 182, __pyx_L1_error)
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":171
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":184
  *                 self.bqm_.adj[irow[qi]].first.resize(
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  */
       __pyx_t_5 = __pyx_v_qi;
       __pyx_t_4 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )))]).first.back().first = (*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":172
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":185
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]             # <<<<<<<<<<<<<<
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_5 * __pyx_v_irow.strides[0]) )))]).first.back().second = (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_4 * __pyx_v_qdata.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":187
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  */
       __pyx_t_5 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":175
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":188
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]
  */
       __pyx_t_4 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":187
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  */
       try {
         (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )))]).first.resize(((__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )))]).first.size() + 1));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 174, __pyx_L1_error)
+        __PYX_ERR(0, 187, __pyx_L1_error)
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":176
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":189
  *                 self.bqm_.adj[icol[qi]].first.resize(
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]
  * 
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )))]).first.back().first = (*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":177
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":190
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]             # <<<<<<<<<<<<<<
  * 
  *         else:
  */
       __pyx_t_5 = __pyx_v_qi;
       __pyx_t_4 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )))]).first.back().second = (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_5 * __pyx_v_qdata.strides[0]) )));
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":165
- *                 break
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":178
  * 
+ *         # set the quadratic
  *         if is_sorted:             # <<<<<<<<<<<<<<
  *             for qi in range(num_interactions):
  *                 # cython really has a hard time with push_back so we do this
  */
-    goto __pyx_L17;
+    goto __pyx_L21;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":195
  *             # this is *much* slower, an alternative would be to make a copy
  *             # and then sort but for now let's stick with the simple thing
  *             for qi in range(num_interactions):             # <<<<<<<<<<<<<<
  *                 self.bqm_.set_quadratic(irow[qi], icol[qi], qdata[qi])
  * 
  */
   /*else*/ {
     __pyx_t_1 = __pyx_v_num_interactions;
     __pyx_t_2 = __pyx_t_1;
     for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
       __pyx_v_qi = __pyx_t_3;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":183
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":196
  *             # and then sort but for now let's stick with the simple thing
  *             for qi in range(num_interactions):
  *                 self.bqm_.set_quadratic(irow[qi], icol[qi], qdata[qi])             # <<<<<<<<<<<<<<
  * 
  *         # build the adj. This is not really the memory bottleneck so
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
-      __pyx_t_10 = __pyx_v_qi;
+      __pyx_t_16 = __pyx_v_qi;
       try {
-        __pyx_v_self->bqm_.set_quadratic((*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) ))), (*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) ))), (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_10 * __pyx_v_qdata.strides[0]) ))));
+        __pyx_v_self->bqm_.set_quadratic((*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) ))), (*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) ))), (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_16 * __pyx_v_qdata.strides[0]) ))));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 183, __pyx_L1_error)
+        __PYX_ERR(0, 196, __pyx_L1_error)
       }
     }
   }
-  __pyx_L17:;
+  __pyx_L21:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":188
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":201
  *         # we can build an intermediate (unordered) set version
  *         cdef vector[unordered_set[VarIndex]] adjset
  *         adjset.resize(num_variables)             # <<<<<<<<<<<<<<
  *         u = 0
  *         for ci in range(self.bqm_.num_variables()):
  */
   try {
     __pyx_v_adjset.resize(__pyx_v_num_variables);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 188, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":189
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":202
  *         cdef vector[unordered_set[VarIndex]] adjset
  *         adjset.resize(num_variables)
  *         u = 0             # <<<<<<<<<<<<<<
  *         for ci in range(self.bqm_.num_variables()):
  * 
  */
   __pyx_v_u = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":190
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":203
  *         adjset.resize(num_variables)
  *         u = 0
  *         for ci in range(self.bqm_.num_variables()):             # <<<<<<<<<<<<<<
  * 
  *             # we've been careful so don't need ui < case_starts.size() - 1
  */
   try {
-    __pyx_t_11 = __pyx_v_self->bqm_.num_variables();
+    __pyx_t_17 = __pyx_v_self->bqm_.num_variables();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 190, __pyx_L1_error)
+    __PYX_ERR(0, 203, __pyx_L1_error)
   }
-  __pyx_t_12 = __pyx_t_11;
-  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_12; __pyx_t_1+=1) {
+  __pyx_t_18 = __pyx_t_17;
+  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_18; __pyx_t_1+=1) {
     __pyx_v_ci = __pyx_t_1;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":193
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":206
  * 
  *             # we've been careful so don't need ui < case_starts.size() - 1
  *             while ci >= self.case_starts_[u+1]:             # <<<<<<<<<<<<<<
  *                 u += 1
  * 
  */
     while (1) {
       __pyx_t_9 = ((__pyx_v_ci >= (__pyx_v_self->case_starts_[(__pyx_v_u + 1)])) != 0);
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":194
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":207
  *             # we've been careful so don't need ui < case_starts.size() - 1
  *             while ci >= self.case_starts_[u+1]:
  *                 u += 1             # <<<<<<<<<<<<<<
  * 
  *             span = self.bqm_.neighborhood(ci)
  */
       __pyx_v_u = (__pyx_v_u + 1);
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":196
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":209
  *                 u += 1
  * 
  *             span = self.bqm_.neighborhood(ci)             # <<<<<<<<<<<<<<
  * 
  *             v = 0
  */
     try {
-      __pyx_t_13 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
+      __pyx_t_19 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 196, __pyx_L1_error)
+      __PYX_ERR(0, 209, __pyx_L1_error)
     }
-    __pyx_v_span = __pyx_t_13;
+    __pyx_v_span = __pyx_t_19;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":198
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":211
  *             span = self.bqm_.neighborhood(ci)
  * 
  *             v = 0             # <<<<<<<<<<<<<<
  *             while span.first != span.second:
  *                 cj = deref(span.first).first
  */
     __pyx_v_v = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":199
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":212
  * 
  *             v = 0
  *             while span.first != span.second:             # <<<<<<<<<<<<<<
  *                 cj = deref(span.first).first
  * 
  */
     while (1) {
       __pyx_t_9 = ((__pyx_v_span.first != __pyx_v_span.second) != 0);
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":200
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":213
  *             v = 0
  *             while span.first != span.second:
  *                 cj = deref(span.first).first             # <<<<<<<<<<<<<<
  * 
  *                 # see above note
  */
-      __pyx_t_14 = (*__pyx_v_span.first).first;
-      __pyx_v_cj = __pyx_t_14;
+      __pyx_t_20 = (*__pyx_v_span.first).first;
+      __pyx_v_cj = __pyx_t_20;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":203
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":216
  * 
  *                 # see above note
  *                 while cj >= self.case_starts_[v+1]:             # <<<<<<<<<<<<<<
  *                     v += 1
  * 
  */
       while (1) {
         __pyx_t_9 = ((__pyx_v_cj >= (__pyx_v_self->case_starts_[(__pyx_v_v + 1)])) != 0);
         if (!__pyx_t_9) break;
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":204
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":217
  *                 # see above note
  *                 while cj >= self.case_starts_[v+1]:
  *                     v += 1             # <<<<<<<<<<<<<<
  * 
  *                 adjset[u].insert(v)
  */
         __pyx_v_v = (__pyx_v_v + 1);
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":206
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":219
  *                     v += 1
  * 
  *                 adjset[u].insert(v)             # <<<<<<<<<<<<<<
  * 
  *                 inc(span.first)
  */
       (void)((__pyx_v_adjset[__pyx_v_u]).insert(__pyx_v_v));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":208
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":221
  *                 adjset[u].insert(v)
  * 
  *                 inc(span.first)             # <<<<<<<<<<<<<<
  * 
  *         # now put adjset into adj
  */
       (void)((++__pyx_v_span.first));
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":211
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":224
  * 
  *         # now put adjset into adj
  *         self.adj_.resize(num_variables)             # <<<<<<<<<<<<<<
  *         for v in range(num_variables):
  *             self.adj_[v].insert(self.adj_[v].begin(),
  */
   try {
     __pyx_v_self->adj_.resize(__pyx_v_num_variables);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 211, __pyx_L1_error)
+    __PYX_ERR(0, 224, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":212
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":225
  *         # now put adjset into adj
  *         self.adj_.resize(num_variables)
  *         for v in range(num_variables):             # <<<<<<<<<<<<<<
  *             self.adj_[v].insert(self.adj_[v].begin(),
  *                                 adjset[v].begin(), adjset[v].end())
  */
   __pyx_t_1 = __pyx_v_num_variables;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_v = __pyx_t_3;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":213
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":226
  *         self.adj_.resize(num_variables)
  *         for v in range(num_variables):
  *             self.adj_[v].insert(self.adj_[v].begin(),             # <<<<<<<<<<<<<<
  *                                 adjset[v].begin(), adjset[v].end())
  *             sort(self.adj_[v].begin(), self.adj_[v].end())
  */
     try {
       (__pyx_v_self->adj_[__pyx_v_v]).insert((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_adjset[__pyx_v_v]).begin(), (__pyx_v_adjset[__pyx_v_v]).end());
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 213, __pyx_L1_error)
+      __PYX_ERR(0, 226, __pyx_L1_error)
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":215
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":228
  *             self.adj_[v].insert(self.adj_[v].begin(),
  *                                 adjset[v].begin(), adjset[v].end())
  *             sort(self.adj_[v].begin(), self.adj_[v].end())             # <<<<<<<<<<<<<<
  * 
  *     @classmethod
  */
     std::sort<std::vector<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> ::iterator>((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_self->adj_[__pyx_v_v]).end());
@@ -7376,47 +7810,59 @@
  *                                   Bias[:] qdata) except *:
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_13);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_14, 1);
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel._from_numpy_vectors", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
+  __PYX_XDEC_MEMVIEW(&__pyx_v_degrees, 1);
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_4__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel__from_numpy_vectors(struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *__pyx_v_self, __Pyx_memviewslice __pyx_v_starts, __Pyx_memviewslice __pyx_v_ldata, __Pyx_memviewslice __pyx_v_irow, __Pyx_memviewslice __pyx_v_icol, __Pyx_memviewslice __pyx_v_qdata) {
   Py_ssize_t __pyx_v_num_variables;
   Py_ssize_t __pyx_v_num_cases;
   Py_ssize_t __pyx_v_num_interactions;
   Py_ssize_t __pyx_v_u;
   Py_ssize_t __pyx_v_v;
   Py_ssize_t __pyx_v_ci;
   Py_ssize_t __pyx_v_cj;
   Py_ssize_t __pyx_v_nc;
   int __pyx_v_is_sorted;
   Py_ssize_t __pyx_v_qi;
+  __Pyx_memviewslice __pyx_v_degrees = { 0, 0, { 0 }, { 0 }, { 0 } };
   std::vector<std::unordered_set<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> >  __pyx_v_adjset;
   std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_v_span;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   Py_ssize_t __pyx_t_8;
   int __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_11;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_12;
-  std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_t_13;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_14;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_13 = NULL;
+  __Pyx_memviewslice __pyx_t_14 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  Py_ssize_t __pyx_t_15;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_16;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_17;
+  std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_t_18;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_19;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_4_from_numpy_vectors", 0);
 
   /* "dimod/discrete/cydiscrete_quadratic_model.pyx":125
  * 
@@ -7728,391 +8174,488 @@
       __pyx_v_is_sorted = 0;
 
       /* "dimod/discrete/cydiscrete_quadratic_model.pyx":163
  *             if irow[qi] == irow[qi + 1] and icol[qi] >= icol[qi+1]:
  *                 is_sorted = False
  *                 break             # <<<<<<<<<<<<<<
  * 
- *         if is_sorted:
+ * 
  */
       goto __pyx_L12_break;
 
       /* "dimod/discrete/cydiscrete_quadratic_model.pyx":161
  *                 break
  * 
  *             if irow[qi] == irow[qi + 1] and icol[qi] >= icol[qi+1]:             # <<<<<<<<<<<<<<
  *                 is_sorted = False
  *                 break
  */
     }
   }
   __pyx_L12_break:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":165
- *                 break
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":168
+ *         # reserve the memory for the vectors, this helps use less memory
+ *         # and speeds things up
+ *         cdef np.uint64_t[:] degrees = np.zeros(num_cases, dtype=np.uint64)             # <<<<<<<<<<<<<<
+ * 
+ *         for qi in range(num_interactions):
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_zeros); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_num_cases); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_11 = PyTuple_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_GIVEREF(__pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_7);
+  __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_12);
+  __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_uint64); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_13) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_11, __pyx_t_7); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_14 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_t_13, PyBUF_WRITABLE); if (unlikely(!__pyx_t_14.memview)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_v_degrees = __pyx_t_14;
+  __pyx_t_14.memview = NULL;
+  __pyx_t_14.data = NULL;
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":170
+ *         cdef np.uint64_t[:] degrees = np.zeros(num_cases, dtype=np.uint64)
+ * 
+ *         for qi in range(num_interactions):             # <<<<<<<<<<<<<<
+ *             degrees[irow[qi]] += 1
+ *             degrees[icol[qi]] += 1
+ */
+  __pyx_t_1 = __pyx_v_num_interactions;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_qi = __pyx_t_3;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":171
+ * 
+ *         for qi in range(num_interactions):
+ *             degrees[irow[qi]] += 1             # <<<<<<<<<<<<<<
+ *             degrees[icol[qi]] += 1
+ * 
+ */
+    __pyx_t_4 = __pyx_v_qi;
+    __pyx_t_5 = (*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )));
+    *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_5 * __pyx_v_degrees.strides[0]) )) += 1;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":172
+ *         for qi in range(num_interactions):
+ *             degrees[irow[qi]] += 1
+ *             degrees[icol[qi]] += 1             # <<<<<<<<<<<<<<
+ * 
+ *         for ci in range(num_cases):
+ */
+    __pyx_t_4 = __pyx_v_qi;
+    __pyx_t_5 = (*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )));
+    *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_5 * __pyx_v_degrees.strides[0]) )) += 1;
+  }
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+ *             degrees[icol[qi]] += 1
  * 
+ *         for ci in range(num_cases):             # <<<<<<<<<<<<<<
+ *             self.bqm_.adj[ci].first.reserve(degrees[ci])
+ * 
+ */
+  __pyx_t_1 = __pyx_v_num_cases;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_ci = __pyx_t_3;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":175
+ * 
+ *         for ci in range(num_cases):
+ *             self.bqm_.adj[ci].first.reserve(degrees[ci])             # <<<<<<<<<<<<<<
+ * 
+ *         # set the quadratic
+ */
+    __pyx_t_4 = __pyx_v_ci;
+    (__pyx_v_self->bqm_.adj[__pyx_v_ci]).first.reserve((*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_4 * __pyx_v_degrees.strides[0]) ))));
+  }
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":178
+ * 
+ *         # set the quadratic
  *         if is_sorted:             # <<<<<<<<<<<<<<
  *             for qi in range(num_interactions):
  *                 # cython really has a hard time with push_back so we do this
  */
   __pyx_t_9 = (__pyx_v_is_sorted != 0);
   if (__pyx_t_9) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":166
- * 
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":179
+ *         # set the quadratic
  *         if is_sorted:
  *             for qi in range(num_interactions):             # <<<<<<<<<<<<<<
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  */
     __pyx_t_1 = __pyx_v_num_interactions;
     __pyx_t_2 = __pyx_t_1;
     for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
       __pyx_v_qi = __pyx_t_3;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":169
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  */
       __pyx_t_4 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":170
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":183
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  */
       __pyx_t_5 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":169
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  */
       try {
         (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )))]).first.resize(((__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_5 * __pyx_v_irow.strides[0]) )))]).first.size() + 1));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 169, __pyx_L1_error)
+        __PYX_ERR(0, 182, __pyx_L1_error)
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":171
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":184
  *                 self.bqm_.adj[irow[qi]].first.resize(
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  */
       __pyx_t_5 = __pyx_v_qi;
       __pyx_t_4 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )))]).first.back().first = (*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":172
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":185
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]             # <<<<<<<<<<<<<<
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_5 * __pyx_v_irow.strides[0]) )))]).first.back().second = (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_4 * __pyx_v_qdata.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":187
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  */
       __pyx_t_5 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":175
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":188
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]
  */
       __pyx_t_4 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":187
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  */
       try {
         (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )))]).first.resize(((__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )))]).first.size() + 1));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 174, __pyx_L1_error)
+        __PYX_ERR(0, 187, __pyx_L1_error)
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":176
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":189
  *                 self.bqm_.adj[icol[qi]].first.resize(
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]
  * 
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )))]).first.back().first = (*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":177
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":190
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]             # <<<<<<<<<<<<<<
  * 
  *         else:
  */
       __pyx_t_5 = __pyx_v_qi;
       __pyx_t_4 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )))]).first.back().second = (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_5 * __pyx_v_qdata.strides[0]) )));
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":165
- *                 break
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":178
  * 
+ *         # set the quadratic
  *         if is_sorted:             # <<<<<<<<<<<<<<
  *             for qi in range(num_interactions):
  *                 # cython really has a hard time with push_back so we do this
  */
-    goto __pyx_L17;
+    goto __pyx_L21;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":195
  *             # this is *much* slower, an alternative would be to make a copy
  *             # and then sort but for now let's stick with the simple thing
  *             for qi in range(num_interactions):             # <<<<<<<<<<<<<<
  *                 self.bqm_.set_quadratic(irow[qi], icol[qi], qdata[qi])
  * 
  */
   /*else*/ {
     __pyx_t_1 = __pyx_v_num_interactions;
     __pyx_t_2 = __pyx_t_1;
     for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
       __pyx_v_qi = __pyx_t_3;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":183
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":196
  *             # and then sort but for now let's stick with the simple thing
  *             for qi in range(num_interactions):
  *                 self.bqm_.set_quadratic(irow[qi], icol[qi], qdata[qi])             # <<<<<<<<<<<<<<
  * 
  *         # build the adj. This is not really the memory bottleneck so
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
-      __pyx_t_10 = __pyx_v_qi;
+      __pyx_t_15 = __pyx_v_qi;
       try {
-        __pyx_v_self->bqm_.set_quadratic((*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) ))), (*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) ))), (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_10 * __pyx_v_qdata.strides[0]) ))));
+        __pyx_v_self->bqm_.set_quadratic((*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) ))), (*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) ))), (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_15 * __pyx_v_qdata.strides[0]) ))));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 183, __pyx_L1_error)
+        __PYX_ERR(0, 196, __pyx_L1_error)
       }
     }
   }
-  __pyx_L17:;
+  __pyx_L21:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":188
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":201
  *         # we can build an intermediate (unordered) set version
  *         cdef vector[unordered_set[VarIndex]] adjset
  *         adjset.resize(num_variables)             # <<<<<<<<<<<<<<
  *         u = 0
  *         for ci in range(self.bqm_.num_variables()):
  */
   try {
     __pyx_v_adjset.resize(__pyx_v_num_variables);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 188, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":189
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":202
  *         cdef vector[unordered_set[VarIndex]] adjset
  *         adjset.resize(num_variables)
  *         u = 0             # <<<<<<<<<<<<<<
  *         for ci in range(self.bqm_.num_variables()):
  * 
  */
   __pyx_v_u = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":190
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":203
  *         adjset.resize(num_variables)
  *         u = 0
  *         for ci in range(self.bqm_.num_variables()):             # <<<<<<<<<<<<<<
  * 
  *             # we've been careful so don't need ui < case_starts.size() - 1
  */
   try {
-    __pyx_t_11 = __pyx_v_self->bqm_.num_variables();
+    __pyx_t_16 = __pyx_v_self->bqm_.num_variables();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 190, __pyx_L1_error)
+    __PYX_ERR(0, 203, __pyx_L1_error)
   }
-  __pyx_t_12 = __pyx_t_11;
-  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_12; __pyx_t_1+=1) {
+  __pyx_t_17 = __pyx_t_16;
+  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_17; __pyx_t_1+=1) {
     __pyx_v_ci = __pyx_t_1;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":193
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":206
  * 
  *             # we've been careful so don't need ui < case_starts.size() - 1
  *             while ci >= self.case_starts_[u+1]:             # <<<<<<<<<<<<<<
  *                 u += 1
  * 
  */
     while (1) {
       __pyx_t_9 = ((__pyx_v_ci >= (__pyx_v_self->case_starts_[(__pyx_v_u + 1)])) != 0);
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":194
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":207
  *             # we've been careful so don't need ui < case_starts.size() - 1
  *             while ci >= self.case_starts_[u+1]:
  *                 u += 1             # <<<<<<<<<<<<<<
  * 
  *             span = self.bqm_.neighborhood(ci)
  */
       __pyx_v_u = (__pyx_v_u + 1);
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":196
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":209
  *                 u += 1
  * 
  *             span = self.bqm_.neighborhood(ci)             # <<<<<<<<<<<<<<
  * 
  *             v = 0
  */
     try {
-      __pyx_t_13 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
+      __pyx_t_18 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 196, __pyx_L1_error)
+      __PYX_ERR(0, 209, __pyx_L1_error)
     }
-    __pyx_v_span = __pyx_t_13;
+    __pyx_v_span = __pyx_t_18;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":198
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":211
  *             span = self.bqm_.neighborhood(ci)
  * 
  *             v = 0             # <<<<<<<<<<<<<<
  *             while span.first != span.second:
  *                 cj = deref(span.first).first
  */
     __pyx_v_v = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":199
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":212
  * 
  *             v = 0
  *             while span.first != span.second:             # <<<<<<<<<<<<<<
  *                 cj = deref(span.first).first
  * 
  */
     while (1) {
       __pyx_t_9 = ((__pyx_v_span.first != __pyx_v_span.second) != 0);
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":200
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":213
  *             v = 0
  *             while span.first != span.second:
  *                 cj = deref(span.first).first             # <<<<<<<<<<<<<<
  * 
  *                 # see above note
  */
-      __pyx_t_14 = (*__pyx_v_span.first).first;
-      __pyx_v_cj = __pyx_t_14;
+      __pyx_t_19 = (*__pyx_v_span.first).first;
+      __pyx_v_cj = __pyx_t_19;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":203
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":216
  * 
  *                 # see above note
  *                 while cj >= self.case_starts_[v+1]:             # <<<<<<<<<<<<<<
  *                     v += 1
  * 
  */
       while (1) {
         __pyx_t_9 = ((__pyx_v_cj >= (__pyx_v_self->case_starts_[(__pyx_v_v + 1)])) != 0);
         if (!__pyx_t_9) break;
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":204
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":217
  *                 # see above note
  *                 while cj >= self.case_starts_[v+1]:
  *                     v += 1             # <<<<<<<<<<<<<<
  * 
  *                 adjset[u].insert(v)
  */
         __pyx_v_v = (__pyx_v_v + 1);
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":206
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":219
  *                     v += 1
  * 
  *                 adjset[u].insert(v)             # <<<<<<<<<<<<<<
  * 
  *                 inc(span.first)
  */
       (void)((__pyx_v_adjset[__pyx_v_u]).insert(__pyx_v_v));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":208
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":221
  *                 adjset[u].insert(v)
  * 
  *                 inc(span.first)             # <<<<<<<<<<<<<<
  * 
  *         # now put adjset into adj
  */
       (void)((++__pyx_v_span.first));
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":211
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":224
  * 
  *         # now put adjset into adj
  *         self.adj_.resize(num_variables)             # <<<<<<<<<<<<<<
  *         for v in range(num_variables):
  *             self.adj_[v].insert(self.adj_[v].begin(),
  */
   try {
     __pyx_v_self->adj_.resize(__pyx_v_num_variables);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 211, __pyx_L1_error)
+    __PYX_ERR(0, 224, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":212
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":225
  *         # now put adjset into adj
  *         self.adj_.resize(num_variables)
  *         for v in range(num_variables):             # <<<<<<<<<<<<<<
  *             self.adj_[v].insert(self.adj_[v].begin(),
  *                                 adjset[v].begin(), adjset[v].end())
  */
   __pyx_t_1 = __pyx_v_num_variables;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_v = __pyx_t_3;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":213
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":226
  *         self.adj_.resize(num_variables)
  *         for v in range(num_variables):
  *             self.adj_[v].insert(self.adj_[v].begin(),             # <<<<<<<<<<<<<<
  *                                 adjset[v].begin(), adjset[v].end())
  *             sort(self.adj_[v].begin(), self.adj_[v].end())
  */
     try {
       (__pyx_v_self->adj_[__pyx_v_v]).insert((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_adjset[__pyx_v_v]).begin(), (__pyx_v_adjset[__pyx_v_v]).end());
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 213, __pyx_L1_error)
+      __PYX_ERR(0, 226, __pyx_L1_error)
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":215
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":228
  *             self.adj_[v].insert(self.adj_[v].begin(),
  *                                 adjset[v].begin(), adjset[v].end())
  *             sort(self.adj_[v].begin(), self.adj_[v].end())             # <<<<<<<<<<<<<<
  * 
  *     @classmethod
  */
     std::sort<std::vector<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> ::iterator>((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_self->adj_[__pyx_v_v]).end());
@@ -8126,47 +8669,59 @@
  *                                   Bias[:] qdata) except *:
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_13);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_14, 1);
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel._from_numpy_vectors", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
+  __PYX_XDEC_MEMVIEW(&__pyx_v_degrees, 1);
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_5__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel__from_numpy_vectors(struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *__pyx_v_self, __Pyx_memviewslice __pyx_v_starts, __Pyx_memviewslice __pyx_v_ldata, __Pyx_memviewslice __pyx_v_irow, __Pyx_memviewslice __pyx_v_icol, __Pyx_memviewslice __pyx_v_qdata) {
   Py_ssize_t __pyx_v_num_variables;
   Py_ssize_t __pyx_v_num_cases;
   Py_ssize_t __pyx_v_num_interactions;
   Py_ssize_t __pyx_v_u;
   Py_ssize_t __pyx_v_v;
   Py_ssize_t __pyx_v_ci;
   Py_ssize_t __pyx_v_cj;
   Py_ssize_t __pyx_v_nc;
   int __pyx_v_is_sorted;
   Py_ssize_t __pyx_v_qi;
+  __Pyx_memviewslice __pyx_v_degrees = { 0, 0, { 0 }, { 0 }, { 0 } };
   std::vector<std::unordered_set<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> >  __pyx_v_adjset;
   std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_v_span;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   Py_ssize_t __pyx_t_8;
   int __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_11;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_12;
-  std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_t_13;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_14;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_13 = NULL;
+  __Pyx_memviewslice __pyx_t_14 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  Py_ssize_t __pyx_t_15;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_16;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_17;
+  std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_t_18;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_19;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_5_from_numpy_vectors", 0);
 
   /* "dimod/discrete/cydiscrete_quadratic_model.pyx":125
  * 
@@ -8478,391 +9033,488 @@
       __pyx_v_is_sorted = 0;
 
       /* "dimod/discrete/cydiscrete_quadratic_model.pyx":163
  *             if irow[qi] == irow[qi + 1] and icol[qi] >= icol[qi+1]:
  *                 is_sorted = False
  *                 break             # <<<<<<<<<<<<<<
  * 
- *         if is_sorted:
+ * 
  */
       goto __pyx_L12_break;
 
       /* "dimod/discrete/cydiscrete_quadratic_model.pyx":161
  *                 break
  * 
  *             if irow[qi] == irow[qi + 1] and icol[qi] >= icol[qi+1]:             # <<<<<<<<<<<<<<
  *                 is_sorted = False
  *                 break
  */
     }
   }
   __pyx_L12_break:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":165
- *                 break
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":168
+ *         # reserve the memory for the vectors, this helps use less memory
+ *         # and speeds things up
+ *         cdef np.uint64_t[:] degrees = np.zeros(num_cases, dtype=np.uint64)             # <<<<<<<<<<<<<<
+ * 
+ *         for qi in range(num_interactions):
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_zeros); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_num_cases); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_11 = PyTuple_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_GIVEREF(__pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_7);
+  __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_12);
+  __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_uint64); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_13) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_11, __pyx_t_7); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_14 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_t_13, PyBUF_WRITABLE); if (unlikely(!__pyx_t_14.memview)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_v_degrees = __pyx_t_14;
+  __pyx_t_14.memview = NULL;
+  __pyx_t_14.data = NULL;
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":170
+ *         cdef np.uint64_t[:] degrees = np.zeros(num_cases, dtype=np.uint64)
+ * 
+ *         for qi in range(num_interactions):             # <<<<<<<<<<<<<<
+ *             degrees[irow[qi]] += 1
+ *             degrees[icol[qi]] += 1
+ */
+  __pyx_t_1 = __pyx_v_num_interactions;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_qi = __pyx_t_3;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":171
+ * 
+ *         for qi in range(num_interactions):
+ *             degrees[irow[qi]] += 1             # <<<<<<<<<<<<<<
+ *             degrees[icol[qi]] += 1
+ * 
+ */
+    __pyx_t_4 = __pyx_v_qi;
+    __pyx_t_5 = (*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )));
+    *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_5 * __pyx_v_degrees.strides[0]) )) += 1;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":172
+ *         for qi in range(num_interactions):
+ *             degrees[irow[qi]] += 1
+ *             degrees[icol[qi]] += 1             # <<<<<<<<<<<<<<
+ * 
+ *         for ci in range(num_cases):
+ */
+    __pyx_t_4 = __pyx_v_qi;
+    __pyx_t_5 = (*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )));
+    *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_5 * __pyx_v_degrees.strides[0]) )) += 1;
+  }
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+ *             degrees[icol[qi]] += 1
+ * 
+ *         for ci in range(num_cases):             # <<<<<<<<<<<<<<
+ *             self.bqm_.adj[ci].first.reserve(degrees[ci])
+ * 
+ */
+  __pyx_t_1 = __pyx_v_num_cases;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_ci = __pyx_t_3;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":175
  * 
+ *         for ci in range(num_cases):
+ *             self.bqm_.adj[ci].first.reserve(degrees[ci])             # <<<<<<<<<<<<<<
+ * 
+ *         # set the quadratic
+ */
+    __pyx_t_4 = __pyx_v_ci;
+    (__pyx_v_self->bqm_.adj[__pyx_v_ci]).first.reserve((*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_4 * __pyx_v_degrees.strides[0]) ))));
+  }
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":178
+ * 
+ *         # set the quadratic
  *         if is_sorted:             # <<<<<<<<<<<<<<
  *             for qi in range(num_interactions):
  *                 # cython really has a hard time with push_back so we do this
  */
   __pyx_t_9 = (__pyx_v_is_sorted != 0);
   if (__pyx_t_9) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":166
- * 
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":179
+ *         # set the quadratic
  *         if is_sorted:
  *             for qi in range(num_interactions):             # <<<<<<<<<<<<<<
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  */
     __pyx_t_1 = __pyx_v_num_interactions;
     __pyx_t_2 = __pyx_t_1;
     for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
       __pyx_v_qi = __pyx_t_3;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":169
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  */
       __pyx_t_4 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":170
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":183
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  */
       __pyx_t_5 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":169
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  */
       try {
         (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )))]).first.resize(((__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_5 * __pyx_v_irow.strides[0]) )))]).first.size() + 1));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 169, __pyx_L1_error)
+        __PYX_ERR(0, 182, __pyx_L1_error)
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":171
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":184
  *                 self.bqm_.adj[irow[qi]].first.resize(
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  */
       __pyx_t_5 = __pyx_v_qi;
       __pyx_t_4 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )))]).first.back().first = (*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":172
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":185
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]             # <<<<<<<<<<<<<<
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_5 * __pyx_v_irow.strides[0]) )))]).first.back().second = (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_4 * __pyx_v_qdata.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":187
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  */
       __pyx_t_5 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":175
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":188
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]
  */
       __pyx_t_4 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":187
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  */
       try {
         (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )))]).first.resize(((__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )))]).first.size() + 1));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 174, __pyx_L1_error)
+        __PYX_ERR(0, 187, __pyx_L1_error)
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":176
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":189
  *                 self.bqm_.adj[icol[qi]].first.resize(
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]
  * 
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )))]).first.back().first = (*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":177
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":190
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]             # <<<<<<<<<<<<<<
  * 
  *         else:
  */
       __pyx_t_5 = __pyx_v_qi;
       __pyx_t_4 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )))]).first.back().second = (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_5 * __pyx_v_qdata.strides[0]) )));
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":165
- *                 break
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":178
  * 
+ *         # set the quadratic
  *         if is_sorted:             # <<<<<<<<<<<<<<
  *             for qi in range(num_interactions):
  *                 # cython really has a hard time with push_back so we do this
  */
-    goto __pyx_L17;
+    goto __pyx_L21;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":195
  *             # this is *much* slower, an alternative would be to make a copy
  *             # and then sort but for now let's stick with the simple thing
  *             for qi in range(num_interactions):             # <<<<<<<<<<<<<<
  *                 self.bqm_.set_quadratic(irow[qi], icol[qi], qdata[qi])
  * 
  */
   /*else*/ {
     __pyx_t_1 = __pyx_v_num_interactions;
     __pyx_t_2 = __pyx_t_1;
     for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
       __pyx_v_qi = __pyx_t_3;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":183
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":196
  *             # and then sort but for now let's stick with the simple thing
  *             for qi in range(num_interactions):
  *                 self.bqm_.set_quadratic(irow[qi], icol[qi], qdata[qi])             # <<<<<<<<<<<<<<
  * 
  *         # build the adj. This is not really the memory bottleneck so
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
-      __pyx_t_10 = __pyx_v_qi;
+      __pyx_t_15 = __pyx_v_qi;
       try {
-        __pyx_v_self->bqm_.set_quadratic((*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) ))), (*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) ))), (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_10 * __pyx_v_qdata.strides[0]) ))));
+        __pyx_v_self->bqm_.set_quadratic((*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) ))), (*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) ))), (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_15 * __pyx_v_qdata.strides[0]) ))));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 183, __pyx_L1_error)
+        __PYX_ERR(0, 196, __pyx_L1_error)
       }
     }
   }
-  __pyx_L17:;
+  __pyx_L21:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":188
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":201
  *         # we can build an intermediate (unordered) set version
  *         cdef vector[unordered_set[VarIndex]] adjset
  *         adjset.resize(num_variables)             # <<<<<<<<<<<<<<
  *         u = 0
  *         for ci in range(self.bqm_.num_variables()):
  */
   try {
     __pyx_v_adjset.resize(__pyx_v_num_variables);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 188, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":189
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":202
  *         cdef vector[unordered_set[VarIndex]] adjset
  *         adjset.resize(num_variables)
  *         u = 0             # <<<<<<<<<<<<<<
  *         for ci in range(self.bqm_.num_variables()):
  * 
  */
   __pyx_v_u = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":190
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":203
  *         adjset.resize(num_variables)
  *         u = 0
  *         for ci in range(self.bqm_.num_variables()):             # <<<<<<<<<<<<<<
  * 
  *             # we've been careful so don't need ui < case_starts.size() - 1
  */
   try {
-    __pyx_t_11 = __pyx_v_self->bqm_.num_variables();
+    __pyx_t_16 = __pyx_v_self->bqm_.num_variables();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 190, __pyx_L1_error)
+    __PYX_ERR(0, 203, __pyx_L1_error)
   }
-  __pyx_t_12 = __pyx_t_11;
-  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_12; __pyx_t_1+=1) {
+  __pyx_t_17 = __pyx_t_16;
+  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_17; __pyx_t_1+=1) {
     __pyx_v_ci = __pyx_t_1;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":193
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":206
  * 
  *             # we've been careful so don't need ui < case_starts.size() - 1
  *             while ci >= self.case_starts_[u+1]:             # <<<<<<<<<<<<<<
  *                 u += 1
  * 
  */
     while (1) {
       __pyx_t_9 = ((__pyx_v_ci >= (__pyx_v_self->case_starts_[(__pyx_v_u + 1)])) != 0);
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":194
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":207
  *             # we've been careful so don't need ui < case_starts.size() - 1
  *             while ci >= self.case_starts_[u+1]:
  *                 u += 1             # <<<<<<<<<<<<<<
  * 
  *             span = self.bqm_.neighborhood(ci)
  */
       __pyx_v_u = (__pyx_v_u + 1);
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":196
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":209
  *                 u += 1
  * 
  *             span = self.bqm_.neighborhood(ci)             # <<<<<<<<<<<<<<
  * 
  *             v = 0
  */
     try {
-      __pyx_t_13 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
+      __pyx_t_18 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 196, __pyx_L1_error)
+      __PYX_ERR(0, 209, __pyx_L1_error)
     }
-    __pyx_v_span = __pyx_t_13;
+    __pyx_v_span = __pyx_t_18;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":198
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":211
  *             span = self.bqm_.neighborhood(ci)
  * 
  *             v = 0             # <<<<<<<<<<<<<<
  *             while span.first != span.second:
  *                 cj = deref(span.first).first
  */
     __pyx_v_v = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":199
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":212
  * 
  *             v = 0
  *             while span.first != span.second:             # <<<<<<<<<<<<<<
  *                 cj = deref(span.first).first
  * 
  */
     while (1) {
       __pyx_t_9 = ((__pyx_v_span.first != __pyx_v_span.second) != 0);
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":200
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":213
  *             v = 0
  *             while span.first != span.second:
  *                 cj = deref(span.first).first             # <<<<<<<<<<<<<<
  * 
  *                 # see above note
  */
-      __pyx_t_14 = (*__pyx_v_span.first).first;
-      __pyx_v_cj = __pyx_t_14;
+      __pyx_t_19 = (*__pyx_v_span.first).first;
+      __pyx_v_cj = __pyx_t_19;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":203
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":216
  * 
  *                 # see above note
  *                 while cj >= self.case_starts_[v+1]:             # <<<<<<<<<<<<<<
  *                     v += 1
  * 
  */
       while (1) {
         __pyx_t_9 = ((__pyx_v_cj >= (__pyx_v_self->case_starts_[(__pyx_v_v + 1)])) != 0);
         if (!__pyx_t_9) break;
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":204
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":217
  *                 # see above note
  *                 while cj >= self.case_starts_[v+1]:
  *                     v += 1             # <<<<<<<<<<<<<<
  * 
  *                 adjset[u].insert(v)
  */
         __pyx_v_v = (__pyx_v_v + 1);
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":206
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":219
  *                     v += 1
  * 
  *                 adjset[u].insert(v)             # <<<<<<<<<<<<<<
  * 
  *                 inc(span.first)
  */
       (void)((__pyx_v_adjset[__pyx_v_u]).insert(__pyx_v_v));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":208
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":221
  *                 adjset[u].insert(v)
  * 
  *                 inc(span.first)             # <<<<<<<<<<<<<<
  * 
  *         # now put adjset into adj
  */
       (void)((++__pyx_v_span.first));
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":211
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":224
  * 
  *         # now put adjset into adj
  *         self.adj_.resize(num_variables)             # <<<<<<<<<<<<<<
  *         for v in range(num_variables):
  *             self.adj_[v].insert(self.adj_[v].begin(),
  */
   try {
     __pyx_v_self->adj_.resize(__pyx_v_num_variables);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 211, __pyx_L1_error)
+    __PYX_ERR(0, 224, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":212
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":225
  *         # now put adjset into adj
  *         self.adj_.resize(num_variables)
  *         for v in range(num_variables):             # <<<<<<<<<<<<<<
  *             self.adj_[v].insert(self.adj_[v].begin(),
  *                                 adjset[v].begin(), adjset[v].end())
  */
   __pyx_t_1 = __pyx_v_num_variables;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_v = __pyx_t_3;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":213
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":226
  *         self.adj_.resize(num_variables)
  *         for v in range(num_variables):
  *             self.adj_[v].insert(self.adj_[v].begin(),             # <<<<<<<<<<<<<<
  *                                 adjset[v].begin(), adjset[v].end())
  *             sort(self.adj_[v].begin(), self.adj_[v].end())
  */
     try {
       (__pyx_v_self->adj_[__pyx_v_v]).insert((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_adjset[__pyx_v_v]).begin(), (__pyx_v_adjset[__pyx_v_v]).end());
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 213, __pyx_L1_error)
+      __PYX_ERR(0, 226, __pyx_L1_error)
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":215
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":228
  *             self.adj_[v].insert(self.adj_[v].begin(),
  *                                 adjset[v].begin(), adjset[v].end())
  *             sort(self.adj_[v].begin(), self.adj_[v].end())             # <<<<<<<<<<<<<<
  * 
  *     @classmethod
  */
     std::sort<std::vector<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> ::iterator>((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_self->adj_[__pyx_v_v]).end());
@@ -8876,47 +9528,59 @@
  *                                   Bias[:] qdata) except *:
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_13);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_14, 1);
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel._from_numpy_vectors", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
+  __PYX_XDEC_MEMVIEW(&__pyx_v_degrees, 1);
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_6__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel__from_numpy_vectors(struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *__pyx_v_self, __Pyx_memviewslice __pyx_v_starts, __Pyx_memviewslice __pyx_v_ldata, __Pyx_memviewslice __pyx_v_irow, __Pyx_memviewslice __pyx_v_icol, __Pyx_memviewslice __pyx_v_qdata) {
   Py_ssize_t __pyx_v_num_variables;
   Py_ssize_t __pyx_v_num_cases;
   Py_ssize_t __pyx_v_num_interactions;
   Py_ssize_t __pyx_v_u;
   Py_ssize_t __pyx_v_v;
   Py_ssize_t __pyx_v_ci;
   Py_ssize_t __pyx_v_cj;
   Py_ssize_t __pyx_v_nc;
   int __pyx_v_is_sorted;
   Py_ssize_t __pyx_v_qi;
+  __Pyx_memviewslice __pyx_v_degrees = { 0, 0, { 0 }, { 0 }, { 0 } };
   std::vector<std::unordered_set<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> >  __pyx_v_adjset;
   std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_v_span;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   Py_ssize_t __pyx_t_8;
   int __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_11;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_12;
-  std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_t_13;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_14;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_13 = NULL;
+  __Pyx_memviewslice __pyx_t_14 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  Py_ssize_t __pyx_t_15;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_16;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_17;
+  std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_t_18;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_19;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_6_from_numpy_vectors", 0);
 
   /* "dimod/discrete/cydiscrete_quadratic_model.pyx":125
  * 
@@ -9228,391 +9892,488 @@
       __pyx_v_is_sorted = 0;
 
       /* "dimod/discrete/cydiscrete_quadratic_model.pyx":163
  *             if irow[qi] == irow[qi + 1] and icol[qi] >= icol[qi+1]:
  *                 is_sorted = False
  *                 break             # <<<<<<<<<<<<<<
  * 
- *         if is_sorted:
+ * 
  */
       goto __pyx_L12_break;
 
       /* "dimod/discrete/cydiscrete_quadratic_model.pyx":161
  *                 break
  * 
  *             if irow[qi] == irow[qi + 1] and icol[qi] >= icol[qi+1]:             # <<<<<<<<<<<<<<
  *                 is_sorted = False
  *                 break
  */
     }
   }
   __pyx_L12_break:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":165
- *                 break
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":168
+ *         # reserve the memory for the vectors, this helps use less memory
+ *         # and speeds things up
+ *         cdef np.uint64_t[:] degrees = np.zeros(num_cases, dtype=np.uint64)             # <<<<<<<<<<<<<<
+ * 
+ *         for qi in range(num_interactions):
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_zeros); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_num_cases); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_11 = PyTuple_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_GIVEREF(__pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_7);
+  __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_12);
+  __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_uint64); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_13) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_11, __pyx_t_7); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_14 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_t_13, PyBUF_WRITABLE); if (unlikely(!__pyx_t_14.memview)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_v_degrees = __pyx_t_14;
+  __pyx_t_14.memview = NULL;
+  __pyx_t_14.data = NULL;
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":170
+ *         cdef np.uint64_t[:] degrees = np.zeros(num_cases, dtype=np.uint64)
+ * 
+ *         for qi in range(num_interactions):             # <<<<<<<<<<<<<<
+ *             degrees[irow[qi]] += 1
+ *             degrees[icol[qi]] += 1
+ */
+  __pyx_t_1 = __pyx_v_num_interactions;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_qi = __pyx_t_3;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":171
+ * 
+ *         for qi in range(num_interactions):
+ *             degrees[irow[qi]] += 1             # <<<<<<<<<<<<<<
+ *             degrees[icol[qi]] += 1
+ * 
+ */
+    __pyx_t_4 = __pyx_v_qi;
+    __pyx_t_5 = (*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )));
+    *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_5 * __pyx_v_degrees.strides[0]) )) += 1;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":172
+ *         for qi in range(num_interactions):
+ *             degrees[irow[qi]] += 1
+ *             degrees[icol[qi]] += 1             # <<<<<<<<<<<<<<
+ * 
+ *         for ci in range(num_cases):
+ */
+    __pyx_t_4 = __pyx_v_qi;
+    __pyx_t_5 = (*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )));
+    *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_5 * __pyx_v_degrees.strides[0]) )) += 1;
+  }
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+ *             degrees[icol[qi]] += 1
  * 
+ *         for ci in range(num_cases):             # <<<<<<<<<<<<<<
+ *             self.bqm_.adj[ci].first.reserve(degrees[ci])
+ * 
+ */
+  __pyx_t_1 = __pyx_v_num_cases;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_ci = __pyx_t_3;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":175
+ * 
+ *         for ci in range(num_cases):
+ *             self.bqm_.adj[ci].first.reserve(degrees[ci])             # <<<<<<<<<<<<<<
+ * 
+ *         # set the quadratic
+ */
+    __pyx_t_4 = __pyx_v_ci;
+    (__pyx_v_self->bqm_.adj[__pyx_v_ci]).first.reserve((*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_4 * __pyx_v_degrees.strides[0]) ))));
+  }
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":178
+ * 
+ *         # set the quadratic
  *         if is_sorted:             # <<<<<<<<<<<<<<
  *             for qi in range(num_interactions):
  *                 # cython really has a hard time with push_back so we do this
  */
   __pyx_t_9 = (__pyx_v_is_sorted != 0);
   if (__pyx_t_9) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":166
- * 
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":179
+ *         # set the quadratic
  *         if is_sorted:
  *             for qi in range(num_interactions):             # <<<<<<<<<<<<<<
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  */
     __pyx_t_1 = __pyx_v_num_interactions;
     __pyx_t_2 = __pyx_t_1;
     for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
       __pyx_v_qi = __pyx_t_3;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":169
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  */
       __pyx_t_4 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":170
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":183
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  */
       __pyx_t_5 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":169
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  */
       try {
         (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )))]).first.resize(((__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_5 * __pyx_v_irow.strides[0]) )))]).first.size() + 1));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 169, __pyx_L1_error)
+        __PYX_ERR(0, 182, __pyx_L1_error)
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":171
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":184
  *                 self.bqm_.adj[irow[qi]].first.resize(
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  */
       __pyx_t_5 = __pyx_v_qi;
       __pyx_t_4 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )))]).first.back().first = (*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":172
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":185
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]             # <<<<<<<<<<<<<<
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_5 * __pyx_v_irow.strides[0]) )))]).first.back().second = (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_4 * __pyx_v_qdata.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":187
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  */
       __pyx_t_5 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":175
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":188
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]
  */
       __pyx_t_4 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":187
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  */
       try {
         (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )))]).first.resize(((__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )))]).first.size() + 1));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 174, __pyx_L1_error)
+        __PYX_ERR(0, 187, __pyx_L1_error)
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":176
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":189
  *                 self.bqm_.adj[icol[qi]].first.resize(
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]
  * 
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )))]).first.back().first = (*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":177
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":190
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]             # <<<<<<<<<<<<<<
  * 
  *         else:
  */
       __pyx_t_5 = __pyx_v_qi;
       __pyx_t_4 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )))]).first.back().second = (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_5 * __pyx_v_qdata.strides[0]) )));
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":165
- *                 break
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":178
  * 
+ *         # set the quadratic
  *         if is_sorted:             # <<<<<<<<<<<<<<
  *             for qi in range(num_interactions):
  *                 # cython really has a hard time with push_back so we do this
  */
-    goto __pyx_L17;
+    goto __pyx_L21;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":195
  *             # this is *much* slower, an alternative would be to make a copy
  *             # and then sort but for now let's stick with the simple thing
  *             for qi in range(num_interactions):             # <<<<<<<<<<<<<<
  *                 self.bqm_.set_quadratic(irow[qi], icol[qi], qdata[qi])
  * 
  */
   /*else*/ {
     __pyx_t_1 = __pyx_v_num_interactions;
     __pyx_t_2 = __pyx_t_1;
     for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
       __pyx_v_qi = __pyx_t_3;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":183
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":196
  *             # and then sort but for now let's stick with the simple thing
  *             for qi in range(num_interactions):
  *                 self.bqm_.set_quadratic(irow[qi], icol[qi], qdata[qi])             # <<<<<<<<<<<<<<
  * 
  *         # build the adj. This is not really the memory bottleneck so
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
-      __pyx_t_10 = __pyx_v_qi;
+      __pyx_t_15 = __pyx_v_qi;
       try {
-        __pyx_v_self->bqm_.set_quadratic((*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) ))), (*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) ))), (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_10 * __pyx_v_qdata.strides[0]) ))));
+        __pyx_v_self->bqm_.set_quadratic((*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) ))), (*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) ))), (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_15 * __pyx_v_qdata.strides[0]) ))));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 183, __pyx_L1_error)
+        __PYX_ERR(0, 196, __pyx_L1_error)
       }
     }
   }
-  __pyx_L17:;
+  __pyx_L21:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":188
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":201
  *         # we can build an intermediate (unordered) set version
  *         cdef vector[unordered_set[VarIndex]] adjset
  *         adjset.resize(num_variables)             # <<<<<<<<<<<<<<
  *         u = 0
  *         for ci in range(self.bqm_.num_variables()):
  */
   try {
     __pyx_v_adjset.resize(__pyx_v_num_variables);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 188, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":189
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":202
  *         cdef vector[unordered_set[VarIndex]] adjset
  *         adjset.resize(num_variables)
  *         u = 0             # <<<<<<<<<<<<<<
  *         for ci in range(self.bqm_.num_variables()):
  * 
  */
   __pyx_v_u = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":190
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":203
  *         adjset.resize(num_variables)
  *         u = 0
  *         for ci in range(self.bqm_.num_variables()):             # <<<<<<<<<<<<<<
  * 
  *             # we've been careful so don't need ui < case_starts.size() - 1
  */
   try {
-    __pyx_t_11 = __pyx_v_self->bqm_.num_variables();
+    __pyx_t_16 = __pyx_v_self->bqm_.num_variables();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 190, __pyx_L1_error)
+    __PYX_ERR(0, 203, __pyx_L1_error)
   }
-  __pyx_t_12 = __pyx_t_11;
-  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_12; __pyx_t_1+=1) {
+  __pyx_t_17 = __pyx_t_16;
+  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_17; __pyx_t_1+=1) {
     __pyx_v_ci = __pyx_t_1;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":193
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":206
  * 
  *             # we've been careful so don't need ui < case_starts.size() - 1
  *             while ci >= self.case_starts_[u+1]:             # <<<<<<<<<<<<<<
  *                 u += 1
  * 
  */
     while (1) {
       __pyx_t_9 = ((__pyx_v_ci >= (__pyx_v_self->case_starts_[(__pyx_v_u + 1)])) != 0);
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":194
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":207
  *             # we've been careful so don't need ui < case_starts.size() - 1
  *             while ci >= self.case_starts_[u+1]:
  *                 u += 1             # <<<<<<<<<<<<<<
  * 
  *             span = self.bqm_.neighborhood(ci)
  */
       __pyx_v_u = (__pyx_v_u + 1);
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":196
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":209
  *                 u += 1
  * 
  *             span = self.bqm_.neighborhood(ci)             # <<<<<<<<<<<<<<
  * 
  *             v = 0
  */
     try {
-      __pyx_t_13 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
+      __pyx_t_18 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 196, __pyx_L1_error)
+      __PYX_ERR(0, 209, __pyx_L1_error)
     }
-    __pyx_v_span = __pyx_t_13;
+    __pyx_v_span = __pyx_t_18;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":198
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":211
  *             span = self.bqm_.neighborhood(ci)
  * 
  *             v = 0             # <<<<<<<<<<<<<<
  *             while span.first != span.second:
  *                 cj = deref(span.first).first
  */
     __pyx_v_v = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":199
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":212
  * 
  *             v = 0
  *             while span.first != span.second:             # <<<<<<<<<<<<<<
  *                 cj = deref(span.first).first
  * 
  */
     while (1) {
       __pyx_t_9 = ((__pyx_v_span.first != __pyx_v_span.second) != 0);
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":200
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":213
  *             v = 0
  *             while span.first != span.second:
  *                 cj = deref(span.first).first             # <<<<<<<<<<<<<<
  * 
  *                 # see above note
  */
-      __pyx_t_14 = (*__pyx_v_span.first).first;
-      __pyx_v_cj = __pyx_t_14;
+      __pyx_t_19 = (*__pyx_v_span.first).first;
+      __pyx_v_cj = __pyx_t_19;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":203
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":216
  * 
  *                 # see above note
  *                 while cj >= self.case_starts_[v+1]:             # <<<<<<<<<<<<<<
  *                     v += 1
  * 
  */
       while (1) {
         __pyx_t_9 = ((__pyx_v_cj >= (__pyx_v_self->case_starts_[(__pyx_v_v + 1)])) != 0);
         if (!__pyx_t_9) break;
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":204
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":217
  *                 # see above note
  *                 while cj >= self.case_starts_[v+1]:
  *                     v += 1             # <<<<<<<<<<<<<<
  * 
  *                 adjset[u].insert(v)
  */
         __pyx_v_v = (__pyx_v_v + 1);
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":206
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":219
  *                     v += 1
  * 
  *                 adjset[u].insert(v)             # <<<<<<<<<<<<<<
  * 
  *                 inc(span.first)
  */
       (void)((__pyx_v_adjset[__pyx_v_u]).insert(__pyx_v_v));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":208
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":221
  *                 adjset[u].insert(v)
  * 
  *                 inc(span.first)             # <<<<<<<<<<<<<<
  * 
  *         # now put adjset into adj
  */
       (void)((++__pyx_v_span.first));
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":211
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":224
  * 
  *         # now put adjset into adj
  *         self.adj_.resize(num_variables)             # <<<<<<<<<<<<<<
  *         for v in range(num_variables):
  *             self.adj_[v].insert(self.adj_[v].begin(),
  */
   try {
     __pyx_v_self->adj_.resize(__pyx_v_num_variables);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 211, __pyx_L1_error)
+    __PYX_ERR(0, 224, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":212
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":225
  *         # now put adjset into adj
  *         self.adj_.resize(num_variables)
  *         for v in range(num_variables):             # <<<<<<<<<<<<<<
  *             self.adj_[v].insert(self.adj_[v].begin(),
  *                                 adjset[v].begin(), adjset[v].end())
  */
   __pyx_t_1 = __pyx_v_num_variables;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_v = __pyx_t_3;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":213
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":226
  *         self.adj_.resize(num_variables)
  *         for v in range(num_variables):
  *             self.adj_[v].insert(self.adj_[v].begin(),             # <<<<<<<<<<<<<<
  *                                 adjset[v].begin(), adjset[v].end())
  *             sort(self.adj_[v].begin(), self.adj_[v].end())
  */
     try {
       (__pyx_v_self->adj_[__pyx_v_v]).insert((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_adjset[__pyx_v_v]).begin(), (__pyx_v_adjset[__pyx_v_v]).end());
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 213, __pyx_L1_error)
+      __PYX_ERR(0, 226, __pyx_L1_error)
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":215
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":228
  *             self.adj_[v].insert(self.adj_[v].begin(),
  *                                 adjset[v].begin(), adjset[v].end())
  *             sort(self.adj_[v].begin(), self.adj_[v].end())             # <<<<<<<<<<<<<<
  * 
  *     @classmethod
  */
     std::sort<std::vector<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> ::iterator>((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_self->adj_[__pyx_v_v]).end());
@@ -9626,47 +10387,60 @@
  *                                   Bias[:] qdata) except *:
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_13);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_14, 1);
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel._from_numpy_vectors", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
+  __PYX_XDEC_MEMVIEW(&__pyx_v_degrees, 1);
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_7__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel__from_numpy_vectors(struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *__pyx_v_self, __Pyx_memviewslice __pyx_v_starts, __Pyx_memviewslice __pyx_v_ldata, __Pyx_memviewslice __pyx_v_irow, __Pyx_memviewslice __pyx_v_icol, __Pyx_memviewslice __pyx_v_qdata) {
   Py_ssize_t __pyx_v_num_variables;
   Py_ssize_t __pyx_v_num_cases;
   Py_ssize_t __pyx_v_num_interactions;
   Py_ssize_t __pyx_v_u;
   Py_ssize_t __pyx_v_v;
   Py_ssize_t __pyx_v_ci;
   Py_ssize_t __pyx_v_cj;
   Py_ssize_t __pyx_v_nc;
   int __pyx_v_is_sorted;
   Py_ssize_t __pyx_v_qi;
+  __Pyx_memviewslice __pyx_v_degrees = { 0, 0, { 0 }, { 0 }, { 0 } };
   std::vector<std::unordered_set<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> >  __pyx_v_adjset;
   std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_v_span;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   Py_ssize_t __pyx_t_8;
   int __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_11;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_12;
-  std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_t_13;
-  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_14;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_13 = NULL;
+  __Pyx_memviewslice __pyx_t_14 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __pyx_t_5numpy_int64_t __pyx_t_15;
+  Py_ssize_t __pyx_t_16;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_17;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::size_type __pyx_t_18;
+  std::pair<dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator,dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::outvars_iterator>  __pyx_t_19;
+  dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_20;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_7_from_numpy_vectors", 0);
 
   /* "dimod/discrete/cydiscrete_quadratic_model.pyx":125
  * 
@@ -9978,391 +10752,488 @@
       __pyx_v_is_sorted = 0;
 
       /* "dimod/discrete/cydiscrete_quadratic_model.pyx":163
  *             if irow[qi] == irow[qi + 1] and icol[qi] >= icol[qi+1]:
  *                 is_sorted = False
  *                 break             # <<<<<<<<<<<<<<
  * 
- *         if is_sorted:
+ * 
  */
       goto __pyx_L12_break;
 
       /* "dimod/discrete/cydiscrete_quadratic_model.pyx":161
  *                 break
  * 
  *             if irow[qi] == irow[qi + 1] and icol[qi] >= icol[qi+1]:             # <<<<<<<<<<<<<<
  *                 is_sorted = False
  *                 break
  */
     }
   }
   __pyx_L12_break:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":165
- *                 break
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":168
+ *         # reserve the memory for the vectors, this helps use less memory
+ *         # and speeds things up
+ *         cdef np.uint64_t[:] degrees = np.zeros(num_cases, dtype=np.uint64)             # <<<<<<<<<<<<<<
+ * 
+ *         for qi in range(num_interactions):
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_zeros); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_num_cases); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_11 = PyTuple_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_GIVEREF(__pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_7);
+  __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_12);
+  __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_uint64); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_13) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_11, __pyx_t_7); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_14 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_t_13, PyBUF_WRITABLE); if (unlikely(!__pyx_t_14.memview)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_v_degrees = __pyx_t_14;
+  __pyx_t_14.memview = NULL;
+  __pyx_t_14.data = NULL;
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":170
+ *         cdef np.uint64_t[:] degrees = np.zeros(num_cases, dtype=np.uint64)
+ * 
+ *         for qi in range(num_interactions):             # <<<<<<<<<<<<<<
+ *             degrees[irow[qi]] += 1
+ *             degrees[icol[qi]] += 1
+ */
+  __pyx_t_1 = __pyx_v_num_interactions;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_qi = __pyx_t_3;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":171
+ * 
+ *         for qi in range(num_interactions):
+ *             degrees[irow[qi]] += 1             # <<<<<<<<<<<<<<
+ *             degrees[icol[qi]] += 1
+ * 
+ */
+    __pyx_t_4 = __pyx_v_qi;
+    __pyx_t_15 = (*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )));
+    *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_15 * __pyx_v_degrees.strides[0]) )) += 1;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":172
+ *         for qi in range(num_interactions):
+ *             degrees[irow[qi]] += 1
+ *             degrees[icol[qi]] += 1             # <<<<<<<<<<<<<<
+ * 
+ *         for ci in range(num_cases):
+ */
+    __pyx_t_4 = __pyx_v_qi;
+    __pyx_t_15 = (*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )));
+    *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_15 * __pyx_v_degrees.strides[0]) )) += 1;
+  }
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+ *             degrees[icol[qi]] += 1
+ * 
+ *         for ci in range(num_cases):             # <<<<<<<<<<<<<<
+ *             self.bqm_.adj[ci].first.reserve(degrees[ci])
  * 
+ */
+  __pyx_t_1 = __pyx_v_num_cases;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_ci = __pyx_t_3;
+
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":175
+ * 
+ *         for ci in range(num_cases):
+ *             self.bqm_.adj[ci].first.reserve(degrees[ci])             # <<<<<<<<<<<<<<
+ * 
+ *         # set the quadratic
+ */
+    __pyx_t_4 = __pyx_v_ci;
+    (__pyx_v_self->bqm_.adj[__pyx_v_ci]).first.reserve((*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_degrees.data + __pyx_t_4 * __pyx_v_degrees.strides[0]) ))));
+  }
+
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":178
+ * 
+ *         # set the quadratic
  *         if is_sorted:             # <<<<<<<<<<<<<<
  *             for qi in range(num_interactions):
  *                 # cython really has a hard time with push_back so we do this
  */
   __pyx_t_9 = (__pyx_v_is_sorted != 0);
   if (__pyx_t_9) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":166
- * 
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":179
+ *         # set the quadratic
  *         if is_sorted:
  *             for qi in range(num_interactions):             # <<<<<<<<<<<<<<
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  */
     __pyx_t_1 = __pyx_v_num_interactions;
     __pyx_t_2 = __pyx_t_1;
     for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
       __pyx_v_qi = __pyx_t_3;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":169
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  */
       __pyx_t_4 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":170
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":183
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  */
       __pyx_t_5 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":169
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
  *                 # cython really has a hard time with push_back so we do this
  *                 # workaround
  *                 self.bqm_.adj[irow[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  */
       try {
         (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )))]).first.resize(((__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_5 * __pyx_v_irow.strides[0]) )))]).first.size() + 1));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 169, __pyx_L1_error)
+        __PYX_ERR(0, 182, __pyx_L1_error)
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":171
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":184
  *                 self.bqm_.adj[irow[qi]].first.resize(
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  */
       __pyx_t_5 = __pyx_v_qi;
       __pyx_t_4 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )))]).first.back().first = (*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":172
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":185
  *                     self.bqm_.adj[irow[qi]].first.size() + 1)
  *                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]             # <<<<<<<<<<<<<<
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_5 * __pyx_v_irow.strides[0]) )))]).first.back().second = (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_4 * __pyx_v_qdata.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":187
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  */
       __pyx_t_5 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":175
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":188
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]
  */
       __pyx_t_4 = __pyx_v_qi;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":174
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":187
  *                 self.bqm_.adj[irow[qi]].first.back().second = qdata[qi]
  * 
  *                 self.bqm_.adj[icol[qi]].first.resize(             # <<<<<<<<<<<<<<
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  */
       try {
         (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )))]).first.resize(((__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )))]).first.size() + 1));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 174, __pyx_L1_error)
+        __PYX_ERR(0, 187, __pyx_L1_error)
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":176
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":189
  *                 self.bqm_.adj[icol[qi]].first.resize(
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]             # <<<<<<<<<<<<<<
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]
  * 
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) )))]).first.back().first = (*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":177
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":190
  *                     self.bqm_.adj[icol[qi]].first.size() + 1)
  *                 self.bqm_.adj[icol[qi]].first.back().first = irow[qi]
  *                 self.bqm_.adj[icol[qi]].first.back().second = qdata[qi]             # <<<<<<<<<<<<<<
  * 
  *         else:
  */
       __pyx_t_5 = __pyx_v_qi;
       __pyx_t_4 = __pyx_v_qi;
       (__pyx_v_self->bqm_.adj[(*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )))]).first.back().second = (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_5 * __pyx_v_qdata.strides[0]) )));
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":165
- *                 break
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":178
  * 
+ *         # set the quadratic
  *         if is_sorted:             # <<<<<<<<<<<<<<
  *             for qi in range(num_interactions):
  *                 # cython really has a hard time with push_back so we do this
  */
-    goto __pyx_L17;
+    goto __pyx_L21;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":182
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":195
  *             # this is *much* slower, an alternative would be to make a copy
  *             # and then sort but for now let's stick with the simple thing
  *             for qi in range(num_interactions):             # <<<<<<<<<<<<<<
  *                 self.bqm_.set_quadratic(irow[qi], icol[qi], qdata[qi])
  * 
  */
   /*else*/ {
     __pyx_t_1 = __pyx_v_num_interactions;
     __pyx_t_2 = __pyx_t_1;
     for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
       __pyx_v_qi = __pyx_t_3;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":183
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":196
  *             # and then sort but for now let's stick with the simple thing
  *             for qi in range(num_interactions):
  *                 self.bqm_.set_quadratic(irow[qi], icol[qi], qdata[qi])             # <<<<<<<<<<<<<<
  * 
  *         # build the adj. This is not really the memory bottleneck so
  */
       __pyx_t_4 = __pyx_v_qi;
       __pyx_t_5 = __pyx_v_qi;
-      __pyx_t_10 = __pyx_v_qi;
+      __pyx_t_16 = __pyx_v_qi;
       try {
-        __pyx_v_self->bqm_.set_quadratic((*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) ))), (*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) ))), (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_10 * __pyx_v_qdata.strides[0]) ))));
+        __pyx_v_self->bqm_.set_quadratic((*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) ))), (*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_5 * __pyx_v_icol.strides[0]) ))), (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_16 * __pyx_v_qdata.strides[0]) ))));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 183, __pyx_L1_error)
+        __PYX_ERR(0, 196, __pyx_L1_error)
       }
     }
   }
-  __pyx_L17:;
+  __pyx_L21:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":188
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":201
  *         # we can build an intermediate (unordered) set version
  *         cdef vector[unordered_set[VarIndex]] adjset
  *         adjset.resize(num_variables)             # <<<<<<<<<<<<<<
  *         u = 0
  *         for ci in range(self.bqm_.num_variables()):
  */
   try {
     __pyx_v_adjset.resize(__pyx_v_num_variables);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 188, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":189
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":202
  *         cdef vector[unordered_set[VarIndex]] adjset
  *         adjset.resize(num_variables)
  *         u = 0             # <<<<<<<<<<<<<<
  *         for ci in range(self.bqm_.num_variables()):
  * 
  */
   __pyx_v_u = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":190
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":203
  *         adjset.resize(num_variables)
  *         u = 0
  *         for ci in range(self.bqm_.num_variables()):             # <<<<<<<<<<<<<<
  * 
  *             # we've been careful so don't need ui < case_starts.size() - 1
  */
   try {
-    __pyx_t_11 = __pyx_v_self->bqm_.num_variables();
+    __pyx_t_17 = __pyx_v_self->bqm_.num_variables();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 190, __pyx_L1_error)
+    __PYX_ERR(0, 203, __pyx_L1_error)
   }
-  __pyx_t_12 = __pyx_t_11;
-  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_12; __pyx_t_1+=1) {
+  __pyx_t_18 = __pyx_t_17;
+  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_18; __pyx_t_1+=1) {
     __pyx_v_ci = __pyx_t_1;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":193
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":206
  * 
  *             # we've been careful so don't need ui < case_starts.size() - 1
  *             while ci >= self.case_starts_[u+1]:             # <<<<<<<<<<<<<<
  *                 u += 1
  * 
  */
     while (1) {
       __pyx_t_9 = ((__pyx_v_ci >= (__pyx_v_self->case_starts_[(__pyx_v_u + 1)])) != 0);
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":194
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":207
  *             # we've been careful so don't need ui < case_starts.size() - 1
  *             while ci >= self.case_starts_[u+1]:
  *                 u += 1             # <<<<<<<<<<<<<<
  * 
  *             span = self.bqm_.neighborhood(ci)
  */
       __pyx_v_u = (__pyx_v_u + 1);
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":196
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":209
  *                 u += 1
  * 
  *             span = self.bqm_.neighborhood(ci)             # <<<<<<<<<<<<<<
  * 
  *             v = 0
  */
     try {
-      __pyx_t_13 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
+      __pyx_t_19 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 196, __pyx_L1_error)
+      __PYX_ERR(0, 209, __pyx_L1_error)
     }
-    __pyx_v_span = __pyx_t_13;
+    __pyx_v_span = __pyx_t_19;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":198
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":211
  *             span = self.bqm_.neighborhood(ci)
  * 
  *             v = 0             # <<<<<<<<<<<<<<
  *             while span.first != span.second:
  *                 cj = deref(span.first).first
  */
     __pyx_v_v = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":199
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":212
  * 
  *             v = 0
  *             while span.first != span.second:             # <<<<<<<<<<<<<<
  *                 cj = deref(span.first).first
  * 
  */
     while (1) {
       __pyx_t_9 = ((__pyx_v_span.first != __pyx_v_span.second) != 0);
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":200
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":213
  *             v = 0
  *             while span.first != span.second:
  *                 cj = deref(span.first).first             # <<<<<<<<<<<<<<
  * 
  *                 # see above note
  */
-      __pyx_t_14 = (*__pyx_v_span.first).first;
-      __pyx_v_cj = __pyx_t_14;
+      __pyx_t_20 = (*__pyx_v_span.first).first;
+      __pyx_v_cj = __pyx_t_20;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":203
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":216
  * 
  *                 # see above note
  *                 while cj >= self.case_starts_[v+1]:             # <<<<<<<<<<<<<<
  *                     v += 1
  * 
  */
       while (1) {
         __pyx_t_9 = ((__pyx_v_cj >= (__pyx_v_self->case_starts_[(__pyx_v_v + 1)])) != 0);
         if (!__pyx_t_9) break;
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":204
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":217
  *                 # see above note
  *                 while cj >= self.case_starts_[v+1]:
  *                     v += 1             # <<<<<<<<<<<<<<
  * 
  *                 adjset[u].insert(v)
  */
         __pyx_v_v = (__pyx_v_v + 1);
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":206
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":219
  *                     v += 1
  * 
  *                 adjset[u].insert(v)             # <<<<<<<<<<<<<<
  * 
  *                 inc(span.first)
  */
       (void)((__pyx_v_adjset[__pyx_v_u]).insert(__pyx_v_v));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":208
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":221
  *                 adjset[u].insert(v)
  * 
  *                 inc(span.first)             # <<<<<<<<<<<<<<
  * 
  *         # now put adjset into adj
  */
       (void)((++__pyx_v_span.first));
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":211
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":224
  * 
  *         # now put adjset into adj
  *         self.adj_.resize(num_variables)             # <<<<<<<<<<<<<<
  *         for v in range(num_variables):
  *             self.adj_[v].insert(self.adj_[v].begin(),
  */
   try {
     __pyx_v_self->adj_.resize(__pyx_v_num_variables);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 211, __pyx_L1_error)
+    __PYX_ERR(0, 224, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":212
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":225
  *         # now put adjset into adj
  *         self.adj_.resize(num_variables)
  *         for v in range(num_variables):             # <<<<<<<<<<<<<<
  *             self.adj_[v].insert(self.adj_[v].begin(),
  *                                 adjset[v].begin(), adjset[v].end())
  */
   __pyx_t_1 = __pyx_v_num_variables;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_v = __pyx_t_3;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":213
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":226
  *         self.adj_.resize(num_variables)
  *         for v in range(num_variables):
  *             self.adj_[v].insert(self.adj_[v].begin(),             # <<<<<<<<<<<<<<
  *                                 adjset[v].begin(), adjset[v].end())
  *             sort(self.adj_[v].begin(), self.adj_[v].end())
  */
     try {
       (__pyx_v_self->adj_[__pyx_v_v]).insert((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_adjset[__pyx_v_v]).begin(), (__pyx_v_adjset[__pyx_v_v]).end());
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 213, __pyx_L1_error)
+      __PYX_ERR(0, 226, __pyx_L1_error)
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":215
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":228
  *             self.adj_[v].insert(self.adj_[v].begin(),
  *                                 adjset[v].begin(), adjset[v].end())
  *             sort(self.adj_[v].begin(), self.adj_[v].end())             # <<<<<<<<<<<<<<
  * 
  *     @classmethod
  */
     std::sort<std::vector<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> ::iterator>((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_self->adj_[__pyx_v_v]).end());
@@ -10376,20 +11247,26 @@
  *                                   Bias[:] qdata) except *:
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_13);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_14, 1);
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel._from_numpy_vectors", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
+  __PYX_XDEC_MEMVIEW(&__pyx_v_degrees, 1);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "dimod/discrete/cydiscrete_quadratic_model.pyx":218
+/* "dimod/discrete/cydiscrete_quadratic_model.pyx":231
  * 
  *     @classmethod
  *     def from_numpy_vectors(cls, starts, ldata, quadratic):             # <<<<<<<<<<<<<<
  * 
  *         cdef cyDiscreteQuadraticModel obj = cls()
  */
 
@@ -10426,40 +11303,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_starts)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ldata)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("from_numpy_vectors", 1, 3, 3, 1); __PYX_ERR(0, 218, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("from_numpy_vectors", 1, 3, 3, 1); __PYX_ERR(0, 231, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_quadratic)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("from_numpy_vectors", 1, 3, 3, 2); __PYX_ERR(0, 218, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("from_numpy_vectors", 1, 3, 3, 2); __PYX_ERR(0, 231, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "from_numpy_vectors") < 0)) __PYX_ERR(0, 218, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "from_numpy_vectors") < 0)) __PYX_ERR(0, 231, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_starts = values[0];
     __pyx_v_ldata = values[1];
     __pyx_v_quadratic = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("from_numpy_vectors", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 218, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("from_numpy_vectors", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 231, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.from_numpy_vectors", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_8from_numpy_vectors(((PyTypeObject*)__pyx_v_cls), __pyx_v_starts, __pyx_v_ldata, __pyx_v_quadratic);
 
@@ -10510,28 +11387,28 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("from_numpy_vectors", 0);
   __Pyx_INCREF(__pyx_v_starts);
   __Pyx_INCREF(__pyx_v_ldata);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":220
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":233
  *     def from_numpy_vectors(cls, starts, ldata, quadratic):
  * 
  *         cdef cyDiscreteQuadraticModel obj = cls()             # <<<<<<<<<<<<<<
  * 
  *         try:
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_v_cls)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_v_cls)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel))))) __PYX_ERR(0, 220, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel))))) __PYX_ERR(0, 233, __pyx_L1_error)
   __pyx_v_obj = ((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":222
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":235
  *         cdef cyDiscreteQuadraticModel obj = cls()
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             irow, icol, qdata = quadratic
  *         except ValueError:
  */
   {
@@ -10539,28 +11416,28 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":223
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":236
  * 
  *         try:
  *             irow, icol, qdata = quadratic             # <<<<<<<<<<<<<<
  *         except ValueError:
  *             raise ValueError("quadratic should be a 3-tuple")
  */
       if ((likely(PyTuple_CheckExact(__pyx_v_quadratic))) || (PyList_CheckExact(__pyx_v_quadratic))) {
         PyObject* sequence = __pyx_v_quadratic;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 3)) {
           if (size > 3) __Pyx_RaiseTooManyValuesError(3);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 223, __pyx_L3_error)
+          __PYX_ERR(0, 236, __pyx_L3_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
           __pyx_t_6 = PyTuple_GET_ITEM(sequence, 2); 
         } else {
@@ -10568,51 +11445,51 @@
           __pyx_t_5 = PyList_GET_ITEM(sequence, 1); 
           __pyx_t_6 = PyList_GET_ITEM(sequence, 2); 
         }
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         #else
-        __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L3_error)
+        __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 223, __pyx_L3_error)
+        __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 236, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_5);
-        __pyx_t_6 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 223, __pyx_L3_error)
+        __pyx_t_6 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 236, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         #endif
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_7 = PyObject_GetIter(__pyx_v_quadratic); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 223, __pyx_L3_error)
+        __pyx_t_7 = PyObject_GetIter(__pyx_v_quadratic); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 236, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_7);
         __pyx_t_8 = Py_TYPE(__pyx_t_7)->tp_iternext;
         index = 0; __pyx_t_1 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_1)) goto __pyx_L9_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_1);
         index = 1; __pyx_t_5 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_5)) goto __pyx_L9_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_5);
         index = 2; __pyx_t_6 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_6)) goto __pyx_L9_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_6);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_7), 3) < 0) __PYX_ERR(0, 223, __pyx_L3_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_7), 3) < 0) __PYX_ERR(0, 236, __pyx_L3_error)
         __pyx_t_8 = NULL;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         goto __pyx_L10_unpacking_done;
         __pyx_L9_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __pyx_t_8 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 223, __pyx_L3_error)
+        __PYX_ERR(0, 236, __pyx_L3_error)
         __pyx_L10_unpacking_done:;
       }
       __pyx_v_irow = __pyx_t_1;
       __pyx_t_1 = 0;
       __pyx_v_icol = __pyx_t_5;
       __pyx_t_5 = 0;
       __pyx_v_qdata = __pyx_t_6;
       __pyx_t_6 = 0;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":222
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":235
  *         cdef cyDiscreteQuadraticModel obj = cls()
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             irow, icol, qdata = quadratic
  *         except ValueError:
  */
     }
@@ -10622,75 +11499,75 @@
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":224
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":237
  *         try:
  *             irow, icol, qdata = quadratic
  *         except ValueError:             # <<<<<<<<<<<<<<
  *             raise ValueError("quadratic should be a 3-tuple")
  * 
  */
     __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ValueError);
     if (__pyx_t_9) {
       __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.from_numpy_vectors", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(0, 224, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(0, 237, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_1);
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":225
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":238
  *             irow, icol, qdata = quadratic
  *         except ValueError:
  *             raise ValueError("quadratic should be a 3-tuple")             # <<<<<<<<<<<<<<
  * 
  *         # convert to numpy arrays, coercing the types into a simpler set
  */
-      __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 225, __pyx_L5_except_error)
+      __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 238, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_Raise(__pyx_t_7, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __PYX_ERR(0, 225, __pyx_L5_except_error)
+      __PYX_ERR(0, 238, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":222
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":235
  *         cdef cyDiscreteQuadraticModel obj = cls()
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             irow, icol, qdata = quadratic
  *         except ValueError:
  */
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":229
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":242
  *         # convert to numpy arrays, coercing the types into a simpler set
  *         # if necessary
  *         index_dtype = np.result_type(starts, irow, icol, np.uint16)             # <<<<<<<<<<<<<<
  * 
  *         starts = np.asarray(starts, dtype=index_dtype)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_result_type); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_result_type); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint16); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint16); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_5)) {
@@ -10700,31 +11577,31 @@
       __Pyx_DECREF_SET(__pyx_t_6, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[5] = {__pyx_t_5, __pyx_v_starts, __pyx_v_irow, __pyx_v_icol, __pyx_t_7};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 4+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 4+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[5] = {__pyx_t_5, __pyx_v_starts, __pyx_v_irow, __pyx_v_icol, __pyx_t_7};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 4+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 4+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   {
-    __pyx_t_10 = PyTuple_New(4+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 229, __pyx_L1_error)
+    __pyx_t_10 = PyTuple_New(4+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_INCREF(__pyx_v_starts);
     __Pyx_GIVEREF(__pyx_v_starts);
     PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_v_starts);
@@ -10733,193 +11610,193 @@
     PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_v_irow);
     __Pyx_INCREF(__pyx_v_icol);
     __Pyx_GIVEREF(__pyx_v_icol);
     PyTuple_SET_ITEM(__pyx_t_10, 2+__pyx_t_9, __pyx_v_icol);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_10, 3+__pyx_t_9, __pyx_t_7);
     __pyx_t_7 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_index_dtype = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":231
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":244
  *         index_dtype = np.result_type(starts, irow, icol, np.uint16)
  * 
  *         starts = np.asarray(starts, dtype=index_dtype)             # <<<<<<<<<<<<<<
  *         ldata = np.asarray(ldata, dtype=obj.dtype)
  *         irow = np.asarray(irow, dtype=index_dtype)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 231, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_starts);
   __Pyx_GIVEREF(__pyx_v_starts);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_starts);
-  __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 231, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_dtype, __pyx_v_index_dtype) < 0) __PYX_ERR(0, 231, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_1, __pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 231, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_dtype, __pyx_v_index_dtype) < 0) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_1, __pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __Pyx_DECREF_SET(__pyx_v_starts, __pyx_t_7);
   __pyx_t_7 = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":232
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":245
  * 
  *         starts = np.asarray(starts, dtype=index_dtype)
  *         ldata = np.asarray(ldata, dtype=obj.dtype)             # <<<<<<<<<<<<<<
  *         irow = np.asarray(irow, dtype=index_dtype)
  *         icol = np.asarray(icol, dtype=index_dtype)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_asarray); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_asarray); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(__pyx_v_ldata);
   __Pyx_GIVEREF(__pyx_v_ldata);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_ldata);
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_v_obj->dtype) < 0) __PYX_ERR(0, 232, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_7, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 232, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_v_obj->dtype) < 0) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_7, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF_SET(__pyx_v_ldata, __pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":233
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":246
  *         starts = np.asarray(starts, dtype=index_dtype)
  *         ldata = np.asarray(ldata, dtype=obj.dtype)
  *         irow = np.asarray(irow, dtype=index_dtype)             # <<<<<<<<<<<<<<
  *         icol = np.asarray(icol, dtype=index_dtype)
  *         qdata = np.asarray(qdata, dtype=obj.dtype)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_asarray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_asarray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(__pyx_v_irow);
   __Pyx_GIVEREF(__pyx_v_irow);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_irow);
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_v_index_dtype) < 0) __PYX_ERR(0, 233, __pyx_L1_error)
-  __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 233, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_v_index_dtype) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF_SET(__pyx_v_irow, __pyx_t_10);
   __pyx_t_10 = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":234
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":247
  *         ldata = np.asarray(ldata, dtype=obj.dtype)
  *         irow = np.asarray(irow, dtype=index_dtype)
  *         icol = np.asarray(icol, dtype=index_dtype)             # <<<<<<<<<<<<<<
  *         qdata = np.asarray(qdata, dtype=obj.dtype)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_asarray); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_asarray); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_INCREF(__pyx_v_icol);
   __Pyx_GIVEREF(__pyx_v_icol);
   PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_v_icol);
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_v_index_dtype) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_10, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_v_index_dtype) < 0) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_10, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF_SET(__pyx_v_icol, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":235
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":248
  *         irow = np.asarray(irow, dtype=index_dtype)
  *         icol = np.asarray(icol, dtype=index_dtype)
  *         qdata = np.asarray(qdata, dtype=obj.dtype)             # <<<<<<<<<<<<<<
  * 
  *         if index_dtype == np.uint16:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_qdata);
   __Pyx_GIVEREF(__pyx_v_qdata);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_qdata);
-  __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_dtype, __pyx_v_obj->dtype) < 0) __PYX_ERR(0, 235, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_1, __pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_dtype, __pyx_v_obj->dtype) < 0) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_1, __pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __Pyx_DECREF_SET(__pyx_v_qdata, __pyx_t_7);
   __pyx_t_7 = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":237
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":250
  *         qdata = np.asarray(qdata, dtype=obj.dtype)
  * 
  *         if index_dtype == np.uint16:             # <<<<<<<<<<<<<<
  *             obj._from_numpy_vectors[np.uint16_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.uint32:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_uint16); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_uint16); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = PyObject_RichCompare(__pyx_v_index_dtype, __pyx_t_10, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __pyx_t_7 = PyObject_RichCompare(__pyx_v_index_dtype, __pyx_t_10, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (__pyx_t_11) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":238
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":251
  * 
  *         if index_dtype == np.uint16:
  *             obj._from_numpy_vectors[np.uint16_t](starts, ldata, irow, icol, qdata)             # <<<<<<<<<<<<<<
  *         elif index_dtype == np.uint32:
  *             obj._from_numpy_vectors[np.uint32_t](starts, ldata, irow, icol, qdata)
  */
-    __pyx_t_12 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint16_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_12.memview)) __PYX_ERR(0, 238, __pyx_L1_error)
-    __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 238, __pyx_L1_error)
-    __pyx_t_14 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint16_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_14.memview)) __PYX_ERR(0, 238, __pyx_L1_error)
-    __pyx_t_15 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint16_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_15.memview)) __PYX_ERR(0, 238, __pyx_L1_error)
-    __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 238, __pyx_L1_error)
-    ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_obj->__pyx_vtab)->__pyx_fuse_1_from_numpy_vectors(__pyx_v_obj, __pyx_t_12, __pyx_t_13, __pyx_t_14, __pyx_t_15, __pyx_t_16); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint16_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_12.memview)) __PYX_ERR(0, 251, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 251, __pyx_L1_error)
+    __pyx_t_14 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint16_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_14.memview)) __PYX_ERR(0, 251, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint16_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_15.memview)) __PYX_ERR(0, 251, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 251, __pyx_L1_error)
+    ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_obj->__pyx_vtab)->__pyx_fuse_1_from_numpy_vectors(__pyx_v_obj, __pyx_t_12, __pyx_t_13, __pyx_t_14, __pyx_t_15, __pyx_t_16); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 251, __pyx_L1_error)
     __PYX_XDEC_MEMVIEW(&__pyx_t_12, 1);
     __pyx_t_12.memview = NULL;
     __pyx_t_12.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_13, 1);
     __pyx_t_13.memview = NULL;
     __pyx_t_13.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_14, 1);
@@ -10928,55 +11805,55 @@
     __PYX_XDEC_MEMVIEW(&__pyx_t_15, 1);
     __pyx_t_15.memview = NULL;
     __pyx_t_15.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_16, 1);
     __pyx_t_16.memview = NULL;
     __pyx_t_16.data = NULL;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":237
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":250
  *         qdata = np.asarray(qdata, dtype=obj.dtype)
  * 
  *         if index_dtype == np.uint16:             # <<<<<<<<<<<<<<
  *             obj._from_numpy_vectors[np.uint16_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.uint32:
  */
     goto __pyx_L13;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":239
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":252
  *         if index_dtype == np.uint16:
  *             obj._from_numpy_vectors[np.uint16_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.uint32:             # <<<<<<<<<<<<<<
  *             obj._from_numpy_vectors[np.uint32_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.uint64:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 252, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_uint32); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_uint32); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 252, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = PyObject_RichCompare(__pyx_v_index_dtype, __pyx_t_10, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_7 = PyObject_RichCompare(__pyx_v_index_dtype, __pyx_t_10, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 252, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 252, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (__pyx_t_11) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":240
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":253
  *             obj._from_numpy_vectors[np.uint16_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.uint32:
  *             obj._from_numpy_vectors[np.uint32_t](starts, ldata, irow, icol, qdata)             # <<<<<<<<<<<<<<
  *         elif index_dtype == np.uint64:
  *             obj._from_numpy_vectors[np.uint64_t](starts, ldata, irow, icol, qdata)
  */
-    __pyx_t_17 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_17.memview)) __PYX_ERR(0, 240, __pyx_L1_error)
-    __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 240, __pyx_L1_error)
-    __pyx_t_18 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_18.memview)) __PYX_ERR(0, 240, __pyx_L1_error)
-    __pyx_t_19 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_19.memview)) __PYX_ERR(0, 240, __pyx_L1_error)
-    __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 240, __pyx_L1_error)
-    ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_obj->__pyx_vtab)->__pyx_fuse_2_from_numpy_vectors(__pyx_v_obj, __pyx_t_17, __pyx_t_16, __pyx_t_18, __pyx_t_19, __pyx_t_13); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 240, __pyx_L1_error)
+    __pyx_t_17 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_17.memview)) __PYX_ERR(0, 253, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 253, __pyx_L1_error)
+    __pyx_t_18 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_18.memview)) __PYX_ERR(0, 253, __pyx_L1_error)
+    __pyx_t_19 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_19.memview)) __PYX_ERR(0, 253, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 253, __pyx_L1_error)
+    ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_obj->__pyx_vtab)->__pyx_fuse_2_from_numpy_vectors(__pyx_v_obj, __pyx_t_17, __pyx_t_16, __pyx_t_18, __pyx_t_19, __pyx_t_13); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 253, __pyx_L1_error)
     __PYX_XDEC_MEMVIEW(&__pyx_t_17, 1);
     __pyx_t_17.memview = NULL;
     __pyx_t_17.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_16, 1);
     __pyx_t_16.memview = NULL;
     __pyx_t_16.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_18, 1);
@@ -10985,55 +11862,55 @@
     __PYX_XDEC_MEMVIEW(&__pyx_t_19, 1);
     __pyx_t_19.memview = NULL;
     __pyx_t_19.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_13, 1);
     __pyx_t_13.memview = NULL;
     __pyx_t_13.data = NULL;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":239
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":252
  *         if index_dtype == np.uint16:
  *             obj._from_numpy_vectors[np.uint16_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.uint32:             # <<<<<<<<<<<<<<
  *             obj._from_numpy_vectors[np.uint32_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.uint64:
  */
     goto __pyx_L13;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":241
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":254
  *         elif index_dtype == np.uint32:
  *             obj._from_numpy_vectors[np.uint32_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.uint64:             # <<<<<<<<<<<<<<
  *             obj._from_numpy_vectors[np.uint64_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.int16:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_uint64); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_uint64); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = PyObject_RichCompare(__pyx_v_index_dtype, __pyx_t_10, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __pyx_t_7 = PyObject_RichCompare(__pyx_v_index_dtype, __pyx_t_10, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (__pyx_t_11) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":242
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":255
  *             obj._from_numpy_vectors[np.uint32_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.uint64:
  *             obj._from_numpy_vectors[np.uint64_t](starts, ldata, irow, icol, qdata)             # <<<<<<<<<<<<<<
  *         elif index_dtype == np.int16:
  *             obj._from_numpy_vectors[np.int16_t](starts, ldata, irow, icol, qdata)
  */
-    __pyx_t_20 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_20.memview)) __PYX_ERR(0, 242, __pyx_L1_error)
-    __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 242, __pyx_L1_error)
-    __pyx_t_21 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_21.memview)) __PYX_ERR(0, 242, __pyx_L1_error)
-    __pyx_t_22 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_22.memview)) __PYX_ERR(0, 242, __pyx_L1_error)
-    __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 242, __pyx_L1_error)
-    ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_obj->__pyx_vtab)->__pyx_fuse_3_from_numpy_vectors(__pyx_v_obj, __pyx_t_20, __pyx_t_13, __pyx_t_21, __pyx_t_22, __pyx_t_16); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 242, __pyx_L1_error)
+    __pyx_t_20 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_20.memview)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __pyx_t_21 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_21.memview)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __pyx_t_22 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_22.memview)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 255, __pyx_L1_error)
+    ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_obj->__pyx_vtab)->__pyx_fuse_3_from_numpy_vectors(__pyx_v_obj, __pyx_t_20, __pyx_t_13, __pyx_t_21, __pyx_t_22, __pyx_t_16); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 255, __pyx_L1_error)
     __PYX_XDEC_MEMVIEW(&__pyx_t_20, 1);
     __pyx_t_20.memview = NULL;
     __pyx_t_20.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_13, 1);
     __pyx_t_13.memview = NULL;
     __pyx_t_13.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_21, 1);
@@ -11042,55 +11919,55 @@
     __PYX_XDEC_MEMVIEW(&__pyx_t_22, 1);
     __pyx_t_22.memview = NULL;
     __pyx_t_22.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_16, 1);
     __pyx_t_16.memview = NULL;
     __pyx_t_16.data = NULL;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":241
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":254
  *         elif index_dtype == np.uint32:
  *             obj._from_numpy_vectors[np.uint32_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.uint64:             # <<<<<<<<<<<<<<
  *             obj._from_numpy_vectors[np.uint64_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.int16:
  */
     goto __pyx_L13;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":243
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":256
  *         elif index_dtype == np.uint64:
  *             obj._from_numpy_vectors[np.uint64_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.int16:             # <<<<<<<<<<<<<<
  *             obj._from_numpy_vectors[np.int16_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.int32:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int16); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int16); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = PyObject_RichCompare(__pyx_v_index_dtype, __pyx_t_10, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_7 = PyObject_RichCompare(__pyx_v_index_dtype, __pyx_t_10, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (__pyx_t_11) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":244
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":257
  *             obj._from_numpy_vectors[np.uint64_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.int16:
  *             obj._from_numpy_vectors[np.int16_t](starts, ldata, irow, icol, qdata)             # <<<<<<<<<<<<<<
  *         elif index_dtype == np.int32:
  *             obj._from_numpy_vectors[np.int32_t](starts, ldata, irow, icol, qdata)
  */
-    __pyx_t_23 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int16_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_23.memview)) __PYX_ERR(0, 244, __pyx_L1_error)
-    __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 244, __pyx_L1_error)
-    __pyx_t_24 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int16_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_24.memview)) __PYX_ERR(0, 244, __pyx_L1_error)
-    __pyx_t_25 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int16_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_25.memview)) __PYX_ERR(0, 244, __pyx_L1_error)
-    __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 244, __pyx_L1_error)
-    ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_obj->__pyx_vtab)->__pyx_fuse_5_from_numpy_vectors(__pyx_v_obj, __pyx_t_23, __pyx_t_16, __pyx_t_24, __pyx_t_25, __pyx_t_13); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 244, __pyx_L1_error)
+    __pyx_t_23 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int16_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_23.memview)) __PYX_ERR(0, 257, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 257, __pyx_L1_error)
+    __pyx_t_24 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int16_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_24.memview)) __PYX_ERR(0, 257, __pyx_L1_error)
+    __pyx_t_25 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int16_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_25.memview)) __PYX_ERR(0, 257, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 257, __pyx_L1_error)
+    ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_obj->__pyx_vtab)->__pyx_fuse_5_from_numpy_vectors(__pyx_v_obj, __pyx_t_23, __pyx_t_16, __pyx_t_24, __pyx_t_25, __pyx_t_13); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 257, __pyx_L1_error)
     __PYX_XDEC_MEMVIEW(&__pyx_t_23, 1);
     __pyx_t_23.memview = NULL;
     __pyx_t_23.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_16, 1);
     __pyx_t_16.memview = NULL;
     __pyx_t_16.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_24, 1);
@@ -11099,55 +11976,55 @@
     __PYX_XDEC_MEMVIEW(&__pyx_t_25, 1);
     __pyx_t_25.memview = NULL;
     __pyx_t_25.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_13, 1);
     __pyx_t_13.memview = NULL;
     __pyx_t_13.data = NULL;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":243
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":256
  *         elif index_dtype == np.uint64:
  *             obj._from_numpy_vectors[np.uint64_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.int16:             # <<<<<<<<<<<<<<
  *             obj._from_numpy_vectors[np.int16_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.int32:
  */
     goto __pyx_L13;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":245
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":258
  *         elif index_dtype == np.int16:
  *             obj._from_numpy_vectors[np.int16_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.int32:             # <<<<<<<<<<<<<<
  *             obj._from_numpy_vectors[np.int32_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.int64:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int32); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int32); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = PyObject_RichCompare(__pyx_v_index_dtype, __pyx_t_10, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_7 = PyObject_RichCompare(__pyx_v_index_dtype, __pyx_t_10, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 258, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 258, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (__pyx_t_11) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":246
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":259
  *             obj._from_numpy_vectors[np.int16_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.int32:
  *             obj._from_numpy_vectors[np.int32_t](starts, ldata, irow, icol, qdata)             # <<<<<<<<<<<<<<
  *         elif index_dtype == np.int64:
  *             obj._from_numpy_vectors[np.int64_t](starts, ldata, irow, icol, qdata)
  */
-    __pyx_t_26 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int32_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_26.memview)) __PYX_ERR(0, 246, __pyx_L1_error)
-    __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 246, __pyx_L1_error)
-    __pyx_t_27 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int32_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_27.memview)) __PYX_ERR(0, 246, __pyx_L1_error)
-    __pyx_t_28 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int32_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_28.memview)) __PYX_ERR(0, 246, __pyx_L1_error)
-    __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 246, __pyx_L1_error)
-    ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_obj->__pyx_vtab)->__pyx_fuse_6_from_numpy_vectors(__pyx_v_obj, __pyx_t_26, __pyx_t_13, __pyx_t_27, __pyx_t_28, __pyx_t_16); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 246, __pyx_L1_error)
+    __pyx_t_26 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int32_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_26.memview)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __pyx_t_27 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int32_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_27.memview)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __pyx_t_28 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int32_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_28.memview)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 259, __pyx_L1_error)
+    ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_obj->__pyx_vtab)->__pyx_fuse_6_from_numpy_vectors(__pyx_v_obj, __pyx_t_26, __pyx_t_13, __pyx_t_27, __pyx_t_28, __pyx_t_16); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 259, __pyx_L1_error)
     __PYX_XDEC_MEMVIEW(&__pyx_t_26, 1);
     __pyx_t_26.memview = NULL;
     __pyx_t_26.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_13, 1);
     __pyx_t_13.memview = NULL;
     __pyx_t_13.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_27, 1);
@@ -11156,55 +12033,55 @@
     __PYX_XDEC_MEMVIEW(&__pyx_t_28, 1);
     __pyx_t_28.memview = NULL;
     __pyx_t_28.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_16, 1);
     __pyx_t_16.memview = NULL;
     __pyx_t_16.data = NULL;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":245
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":258
  *         elif index_dtype == np.int16:
  *             obj._from_numpy_vectors[np.int16_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.int32:             # <<<<<<<<<<<<<<
  *             obj._from_numpy_vectors[np.int32_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.int64:
  */
     goto __pyx_L13;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":247
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":260
  *         elif index_dtype == np.int32:
  *             obj._from_numpy_vectors[np.int32_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.int64:             # <<<<<<<<<<<<<<
  *             obj._from_numpy_vectors[np.int64_t](starts, ldata, irow, icol, qdata)
  *         else:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int64); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int64); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = PyObject_RichCompare(__pyx_v_index_dtype, __pyx_t_10, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_7 = PyObject_RichCompare(__pyx_v_index_dtype, __pyx_t_10, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (likely(__pyx_t_11)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":248
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":261
  *             obj._from_numpy_vectors[np.int32_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.int64:
  *             obj._from_numpy_vectors[np.int64_t](starts, ldata, irow, icol, qdata)             # <<<<<<<<<<<<<<
  *         else:
  *             raise ValueError("starts, irow and icol must be integers")
  */
-    __pyx_t_29 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int64_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_29.memview)) __PYX_ERR(0, 248, __pyx_L1_error)
-    __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 248, __pyx_L1_error)
-    __pyx_t_30 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int64_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_30.memview)) __PYX_ERR(0, 248, __pyx_L1_error)
-    __pyx_t_31 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int64_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_31.memview)) __PYX_ERR(0, 248, __pyx_L1_error)
-    __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 248, __pyx_L1_error)
-    ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_obj->__pyx_vtab)->__pyx_fuse_7_from_numpy_vectors(__pyx_v_obj, __pyx_t_29, __pyx_t_16, __pyx_t_30, __pyx_t_31, __pyx_t_13); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 248, __pyx_L1_error)
+    __pyx_t_29 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int64_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_29.memview)) __PYX_ERR(0, 261, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 261, __pyx_L1_error)
+    __pyx_t_30 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int64_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_30.memview)) __PYX_ERR(0, 261, __pyx_L1_error)
+    __pyx_t_31 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int64_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_31.memview)) __PYX_ERR(0, 261, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 261, __pyx_L1_error)
+    ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_obj->__pyx_vtab)->__pyx_fuse_7_from_numpy_vectors(__pyx_v_obj, __pyx_t_29, __pyx_t_16, __pyx_t_30, __pyx_t_31, __pyx_t_13); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 261, __pyx_L1_error)
     __PYX_XDEC_MEMVIEW(&__pyx_t_29, 1);
     __pyx_t_29.memview = NULL;
     __pyx_t_29.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_16, 1);
     __pyx_t_16.memview = NULL;
     __pyx_t_16.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_30, 1);
@@ -11213,53 +12090,53 @@
     __PYX_XDEC_MEMVIEW(&__pyx_t_31, 1);
     __pyx_t_31.memview = NULL;
     __pyx_t_31.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_13, 1);
     __pyx_t_13.memview = NULL;
     __pyx_t_13.data = NULL;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":247
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":260
  *         elif index_dtype == np.int32:
  *             obj._from_numpy_vectors[np.int32_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.int64:             # <<<<<<<<<<<<<<
  *             obj._from_numpy_vectors[np.int64_t](starts, ldata, irow, icol, qdata)
  *         else:
  */
     goto __pyx_L13;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":250
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":263
  *             obj._from_numpy_vectors[np.int64_t](starts, ldata, irow, icol, qdata)
  *         else:
  *             raise ValueError("starts, irow and icol must be integers")             # <<<<<<<<<<<<<<
  * 
  *         return obj
  */
   /*else*/ {
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 250, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 263, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_Raise(__pyx_t_7, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __PYX_ERR(0, 250, __pyx_L1_error)
+    __PYX_ERR(0, 263, __pyx_L1_error)
   }
   __pyx_L13:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":252
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":265
  *             raise ValueError("starts, irow and icol must be integers")
  * 
  *         return obj             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_obj));
   __pyx_r = ((PyObject *)__pyx_v_obj);
   goto __pyx_L0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":218
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":231
  * 
  *     @classmethod
  *     def from_numpy_vectors(cls, starts, ldata, quadratic):             # <<<<<<<<<<<<<<
  * 
  *         cdef cyDiscreteQuadraticModel obj = cls()
  */
 
@@ -11301,15 +12178,15 @@
   __Pyx_XDECREF(__pyx_v_starts);
   __Pyx_XDECREF(__pyx_v_ldata);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dimod/discrete/cydiscrete_quadratic_model.pyx":256
+/* "dimod/discrete/cydiscrete_quadratic_model.pyx":269
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     def get_linear(self, VarIndex v):             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t num_cases = self.num_cases(v)
  */
 
@@ -11320,15 +12197,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_linear (wrapper)", 0);
   assert(__pyx_arg_v); {
-    __pyx_v_v = __Pyx_PyInt_As_npy_int64(__pyx_arg_v); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 256, __pyx_L3_error)
+    __pyx_v_v = __Pyx_PyInt_As_npy_int64(__pyx_arg_v); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 269, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.get_linear", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -11359,116 +12236,116 @@
   dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::bias_type __pyx_t_11;
   Py_ssize_t __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_linear", 0);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":258
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":271
  *     def get_linear(self, VarIndex v):
  * 
  *         cdef Py_ssize_t num_cases = self.num_cases(v)             # <<<<<<<<<<<<<<
  * 
  *         biases = np.empty(num_cases, dtype=np.float64)
  */
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.v = __pyx_v_v;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_2); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 258, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_2); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 271, __pyx_L1_error)
   __pyx_v_num_cases = __pyx_t_1;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":260
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":273
  *         cdef Py_ssize_t num_cases = self.num_cases(v)
  * 
  *         biases = np.empty(num_cases, dtype=np.float64)             # <<<<<<<<<<<<<<
  *         cdef Bias[:] biases_view = biases
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_num_cases); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_num_cases); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 260, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_biases = __pyx_t_7;
   __pyx_t_7 = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":261
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":274
  * 
  *         biases = np.empty(num_cases, dtype=np.float64)
  *         cdef Bias[:] biases_view = biases             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t c
  */
-  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_biases, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 261, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_biases, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 274, __pyx_L1_error)
   __pyx_v_biases_view = __pyx_t_8;
   __pyx_t_8.memview = NULL;
   __pyx_t_8.data = NULL;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":264
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":277
  * 
  *         cdef Py_ssize_t c
  *         for c in range(num_cases):             # <<<<<<<<<<<<<<
  *             biases_view[c] = self.bqm_.get_linear(self.case_starts_[v] + c)
  * 
  */
   __pyx_t_1 = __pyx_v_num_cases;
   __pyx_t_9 = __pyx_t_1;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_c = __pyx_t_10;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":265
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":278
  *         cdef Py_ssize_t c
  *         for c in range(num_cases):
  *             biases_view[c] = self.bqm_.get_linear(self.case_starts_[v] + c)             # <<<<<<<<<<<<<<
  * 
  *         return biases
  */
     try {
       __pyx_t_11 = __pyx_v_self->bqm_.get_linear(((__pyx_v_self->case_starts_[__pyx_v_v]) + __pyx_v_c));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 265, __pyx_L1_error)
+      __PYX_ERR(0, 278, __pyx_L1_error)
     }
     __pyx_t_12 = __pyx_v_c;
     *((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_biases_view.data + __pyx_t_12 * __pyx_v_biases_view.strides[0]) )) = __pyx_t_11;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":267
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":280
  *             biases_view[c] = self.bqm_.get_linear(self.case_starts_[v] + c)
  * 
  *         return biases             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_biases);
   __pyx_r = __pyx_v_biases;
   goto __pyx_L0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":256
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":269
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     def get_linear(self, VarIndex v):             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t num_cases = self.num_cases(v)
  */
 
@@ -11486,15 +12363,15 @@
   __Pyx_XDECREF(__pyx_v_biases);
   __PYX_XDEC_MEMVIEW(&__pyx_v_biases_view, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dimod/discrete/cydiscrete_quadratic_model.pyx":271
+/* "dimod/discrete/cydiscrete_quadratic_model.pyx":284
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Bias get_linear_case(self, VarIndex v, CaseIndex case) except? -45.3:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
 
@@ -11525,20 +12402,20 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_linear_case); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_linear_case); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_13get_linear_case)) {
-        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 271, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 284, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyInt_From_npy_int64(__pyx_v_case); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 271, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_npy_int64(__pyx_v_case); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 284, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
           if (likely(__pyx_t_6)) {
@@ -11548,49 +12425,49 @@
             __Pyx_DECREF_SET(__pyx_t_5, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 284, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 284, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         {
-          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 271, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 284, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           if (__pyx_t_6) {
             __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_4);
           PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_4);
           __pyx_t_3 = 0;
           __pyx_t_4 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 284, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_9 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_9 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 271, __pyx_L1_error)
+        __pyx_t_9 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_9 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 284, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -11601,50 +12478,50 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":275
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":288
  *         # self.num_cases checks that the variable is valid
  * 
  *         if case < 0 or case >= self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case, self.num_cases(v)))
  */
   __pyx_t_11 = ((__pyx_v_case < 0) != 0);
   if (!__pyx_t_11) {
   } else {
     __pyx_t_10 = __pyx_t_11;
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_13.__pyx_n = 1;
   __pyx_t_13.v = __pyx_v_v;
-  __pyx_t_12 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_13); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 275, __pyx_L1_error)
+  __pyx_t_12 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_13); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 288, __pyx_L1_error)
   __pyx_t_11 = ((__pyx_v_case >= __pyx_t_12) != 0);
   __pyx_t_10 = __pyx_t_11;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_10)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":277
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":290
  *         if case < 0 or case >= self.num_cases(v):
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case, self.num_cases(v)))             # <<<<<<<<<<<<<<
  * 
  *         return self.bqm_.get_linear(self.case_starts_[v] + case)
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_case_is_invalid_variable_only_su, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 277, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_case_is_invalid_variable_only_su, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 290, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_case); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 277, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_case); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 290, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_13.__pyx_n = 1;
     __pyx_t_13.v = __pyx_v_v;
-    __pyx_t_12 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_13); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 277, __pyx_L1_error)
-    __pyx_t_8 = PyInt_FromSsize_t(__pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 277, __pyx_L1_error)
+    __pyx_t_12 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_13); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 290, __pyx_L1_error)
+    __pyx_t_8 = PyInt_FromSsize_t(__pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 290, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_4 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -11653,89 +12530,89 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_5, __pyx_t_8};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_5, __pyx_t_8};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     } else
     #endif
     {
-      __pyx_t_3 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 277, __pyx_L1_error)
+      __pyx_t_3 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       if (__pyx_t_4) {
         __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4); __pyx_t_4 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_7, __pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_8);
       PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_7, __pyx_t_8);
       __pyx_t_5 = 0;
       __pyx_t_8 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":276
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":289
  * 
  *         if case < 0 or case >= self.num_cases(v):
  *             raise ValueError("case {} is invalid, variable only supports {} "             # <<<<<<<<<<<<<<
  *                              "cases".format(case, self.num_cases(v)))
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 289, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 276, __pyx_L1_error)
+    __PYX_ERR(0, 289, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":275
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":288
  *         # self.num_cases checks that the variable is valid
  * 
  *         if case < 0 or case >= self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case, self.num_cases(v)))
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":279
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":292
  *                              "cases".format(case, self.num_cases(v)))
  * 
  *         return self.bqm_.get_linear(self.case_starts_[v] + case)             # <<<<<<<<<<<<<<
  * 
  *     def get_quadratic(self, VarIndex u, VarIndex v, bint array=False):
  */
   try {
     __pyx_t_14 = __pyx_v_self->bqm_.get_linear(((__pyx_v_self->case_starts_[__pyx_v_v]) + __pyx_v_case));
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 279, __pyx_L1_error)
+    __PYX_ERR(0, 292, __pyx_L1_error)
   }
   __pyx_r = __pyx_t_14;
   goto __pyx_L0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":271
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":284
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Bias get_linear_case(self, VarIndex v, CaseIndex case) except? -45.3:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
 
@@ -11785,32 +12662,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_case)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_linear_case", 1, 2, 2, 1); __PYX_ERR(0, 271, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_linear_case", 1, 2, 2, 1); __PYX_ERR(0, 284, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_linear_case") < 0)) __PYX_ERR(0, 271, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_linear_case") < 0)) __PYX_ERR(0, 284, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 271, __pyx_L3_error)
-    __pyx_v_case = __Pyx_PyInt_As_npy_int64(values[1]); if (unlikely((__pyx_v_case == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 271, __pyx_L3_error)
+    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 284, __pyx_L3_error)
+    __pyx_v_case = __Pyx_PyInt_As_npy_int64(values[1]); if (unlikely((__pyx_v_case == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 284, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_linear_case", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 271, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_linear_case", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 284, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.get_linear_case", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_12get_linear_case(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self), __pyx_v_v, __pyx_v_case);
 
@@ -11825,16 +12702,16 @@
   __pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_linear_case", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_get_linear_case(__pyx_v_self, __pyx_v_v, __pyx_v_case, 1); if (unlikely(__pyx_t_1 == ((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias)(-45.3)) && PyErr_Occurred())) __PYX_ERR(0, 271, __pyx_L1_error)
-  __pyx_t_2 = PyFloat_FromDouble(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_get_linear_case(__pyx_v_self, __pyx_v_v, __pyx_v_case, 1); if (unlikely(__pyx_t_1 == ((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias)(-45.3)) && PyErr_Occurred())) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -11843,15 +12720,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dimod/discrete/cydiscrete_quadratic_model.pyx":281
+/* "dimod/discrete/cydiscrete_quadratic_model.pyx":294
  *         return self.bqm_.get_linear(self.case_starts_[v] + case)
  * 
  *     def get_quadratic(self, VarIndex u, VarIndex v, bint array=False):             # <<<<<<<<<<<<<<
  * 
  *         # check that the interaction does in fact exist
  */
 
@@ -11888,47 +12765,47 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_u)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_quadratic", 0, 2, 3, 1); __PYX_ERR(0, 281, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_quadratic", 0, 2, 3, 1); __PYX_ERR(0, 294, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_array);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_quadratic") < 0)) __PYX_ERR(0, 281, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_quadratic") < 0)) __PYX_ERR(0, 294, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_u = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_u == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 281, __pyx_L3_error)
-    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[1]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 281, __pyx_L3_error)
+    __pyx_v_u = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_u == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 294, __pyx_L3_error)
+    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[1]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 294, __pyx_L3_error)
     if (values[2]) {
-      __pyx_v_array = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_array == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 281, __pyx_L3_error)
+      __pyx_v_array = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_array == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 294, __pyx_L3_error)
     } else {
       __pyx_v_array = ((int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_quadratic", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 281, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_quadratic", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 294, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.get_quadratic", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_14get_quadratic(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self), __pyx_v_u, __pyx_v_v, __pyx_v_array);
 
@@ -11965,15 +12842,15 @@
   Py_ssize_t __pyx_t_16;
   int __pyx_t_17;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_quadratic", 0);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":284
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":297
  * 
  *         # check that the interaction does in fact exist
  *         if u < 0 or u >= self.adj_.size():             # <<<<<<<<<<<<<<
  *             raise ValueError("unknown variable")
  *         if v < 0 or v >= self.adj_.size():
  */
   __pyx_t_2 = ((__pyx_v_u < 0) != 0);
@@ -11983,37 +12860,37 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = ((__pyx_v_u >= __pyx_v_self->adj_.size()) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":285
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":298
  *         # check that the interaction does in fact exist
  *         if u < 0 or u >= self.adj_.size():
  *             raise ValueError("unknown variable")             # <<<<<<<<<<<<<<
  *         if v < 0 or v >= self.adj_.size():
  *             raise ValueError("unknown variable")
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 285, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 298, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 285, __pyx_L1_error)
+    __PYX_ERR(0, 298, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":284
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":297
  * 
  *         # check that the interaction does in fact exist
  *         if u < 0 or u >= self.adj_.size():             # <<<<<<<<<<<<<<
  *             raise ValueError("unknown variable")
  *         if v < 0 or v >= self.adj_.size():
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":286
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":299
  *         if u < 0 or u >= self.adj_.size():
  *             raise ValueError("unknown variable")
  *         if v < 0 or v >= self.adj_.size():             # <<<<<<<<<<<<<<
  *             raise ValueError("unknown variable")
  * 
  */
   __pyx_t_2 = ((__pyx_v_v < 0) != 0);
@@ -12023,46 +12900,46 @@
     goto __pyx_L7_bool_binop_done;
   }
   __pyx_t_2 = ((__pyx_v_v >= __pyx_v_self->adj_.size()) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L7_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":287
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":300
  *             raise ValueError("unknown variable")
  *         if v < 0 or v >= self.adj_.size():
  *             raise ValueError("unknown variable")             # <<<<<<<<<<<<<<
  * 
  *         it = lower_bound(self.adj_[u].begin(), self.adj_[u].end(), v)
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 287, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 300, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 287, __pyx_L1_error)
+    __PYX_ERR(0, 300, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":286
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":299
  *         if u < 0 or u >= self.adj_.size():
  *             raise ValueError("unknown variable")
  *         if v < 0 or v >= self.adj_.size():             # <<<<<<<<<<<<<<
  *             raise ValueError("unknown variable")
  * 
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":289
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":302
  *             raise ValueError("unknown variable")
  * 
  *         it = lower_bound(self.adj_[u].begin(), self.adj_[u].end(), v)             # <<<<<<<<<<<<<<
  *         if it == self.adj_[u].end() or deref(it) != v:
  *             raise ValueError("there is no interaction between given variables")
  */
   __pyx_v_it = std::lower_bound<std::vector<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> ::iterator,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex>((__pyx_v_self->adj_[__pyx_v_u]).begin(), (__pyx_v_self->adj_[__pyx_v_u]).end(), __pyx_v_v);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":290
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":303
  * 
  *         it = lower_bound(self.adj_[u].begin(), self.adj_[u].end(), v)
  *         if it == self.adj_[u].end() or deref(it) != v:             # <<<<<<<<<<<<<<
  *             raise ValueError("there is no interaction between given variables")
  * 
  */
   __pyx_t_2 = ((__pyx_v_it == (__pyx_v_self->adj_[__pyx_v_u]).end()) != 0);
@@ -12072,148 +12949,148 @@
     goto __pyx_L10_bool_binop_done;
   }
   __pyx_t_2 = (((*__pyx_v_it) != __pyx_v_v) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L10_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":291
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":304
  *         it = lower_bound(self.adj_[u].begin(), self.adj_[u].end(), v)
  *         if it == self.adj_[u].end() or deref(it) != v:
  *             raise ValueError("there is no interaction between given variables")             # <<<<<<<<<<<<<<
  * 
  *         cdef CaseIndex ci
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 291, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 304, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 291, __pyx_L1_error)
+    __PYX_ERR(0, 304, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":290
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":303
  * 
  *         it = lower_bound(self.adj_[u].begin(), self.adj_[u].end(), v)
  *         if it == self.adj_[u].end() or deref(it) != v:             # <<<<<<<<<<<<<<
  *             raise ValueError("there is no interaction between given variables")
  * 
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":297
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":310
  *         cdef Bias[:, :] quadratic_view
  * 
  *         if array:             # <<<<<<<<<<<<<<
  *             # build a numpy array
  *             quadratic = np.zeros((self.num_cases(u), self.num_cases(v)),
  */
   __pyx_t_1 = (__pyx_v_array != 0);
   if (__pyx_t_1) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":299
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":312
  *         if array:
  *             # build a numpy array
  *             quadratic = np.zeros((self.num_cases(u), self.num_cases(v)),             # <<<<<<<<<<<<<<
  *                                  dtype=self.dtype)
  *             quadratic_view = quadratic
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 299, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 312, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 312, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_6.__pyx_n = 1;
     __pyx_t_6.v = __pyx_v_u;
-    __pyx_t_5 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_6); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 299, __pyx_L1_error)
-    __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 299, __pyx_L1_error)
+    __pyx_t_5 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_6); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 312, __pyx_L1_error)
+    __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 312, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_6.__pyx_n = 1;
     __pyx_t_6.v = __pyx_v_v;
-    __pyx_t_5 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_6); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 299, __pyx_L1_error)
-    __pyx_t_7 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 299, __pyx_L1_error)
+    __pyx_t_5 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_6); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 312, __pyx_L1_error)
+    __pyx_t_7 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 312, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 299, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 312, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_7);
     __pyx_t_3 = 0;
     __pyx_t_7 = 0;
-    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 299, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 312, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_8);
     __pyx_t_8 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":300
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":313
  *             # build a numpy array
  *             quadratic = np.zeros((self.num_cases(u), self.num_cases(v)),
  *                                  dtype=self.dtype)             # <<<<<<<<<<<<<<
  *             quadratic_view = quadratic
  * 
  */
-    __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 300, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 313, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_v_self->dtype) < 0) __PYX_ERR(0, 300, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_v_self->dtype) < 0) __PYX_ERR(0, 313, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":299
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":312
  *         if array:
  *             # build a numpy array
  *             quadratic = np.zeros((self.num_cases(u), self.num_cases(v)),             # <<<<<<<<<<<<<<
  *                                  dtype=self.dtype)
  *             quadratic_view = quadratic
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 299, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 312, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_v_quadratic = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":301
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":314
  *             quadratic = np.zeros((self.num_cases(u), self.num_cases(v)),
  *                                  dtype=self.dtype)
  *             quadratic_view = quadratic             # <<<<<<<<<<<<<<
  * 
  *             for ci in range(self.case_starts_[u], self.case_starts_[u+1]):
  */
-    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dsds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_quadratic, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 301, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dsds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_quadratic, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 314, __pyx_L1_error)
     __pyx_v_quadratic_view = __pyx_t_9;
     __pyx_t_9.memview = NULL;
     __pyx_t_9.data = NULL;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":303
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":316
  *             quadratic_view = quadratic
  * 
  *             for ci in range(self.case_starts_[u], self.case_starts_[u+1]):             # <<<<<<<<<<<<<<
  * 
  *                 span = self.bqm_.neighborhood(ci, self.case_starts_[v])
  */
     __pyx_t_10 = (__pyx_v_self->case_starts_[(__pyx_v_u + 1)]);
     __pyx_t_11 = __pyx_t_10;
     for (__pyx_t_12 = (__pyx_v_self->case_starts_[__pyx_v_u]); __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
       __pyx_v_ci = __pyx_t_12;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":305
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":318
  *             for ci in range(self.case_starts_[u], self.case_starts_[u+1]):
  * 
  *                 span = self.bqm_.neighborhood(ci, self.case_starts_[v])             # <<<<<<<<<<<<<<
  * 
  *                 while (span.first != span.second and deref(span.first).first < self.case_starts_[v+1]):
  */
       try {
         __pyx_t_13 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci, (__pyx_v_self->case_starts_[__pyx_v_v]));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 305, __pyx_L1_error)
+        __PYX_ERR(0, 318, __pyx_L1_error)
       }
       __pyx_v_span = __pyx_t_13;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":307
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":320
  *                 span = self.bqm_.neighborhood(ci, self.case_starts_[v])
  * 
  *                 while (span.first != span.second and deref(span.first).first < self.case_starts_[v+1]):             # <<<<<<<<<<<<<<
  *                     case_u = ci - self.case_starts_[u]
  *                     case_v = deref(span.first).first - self.case_starts_[v]
  */
       while (1) {
@@ -12224,33 +13101,33 @@
           goto __pyx_L17_bool_binop_done;
         }
         __pyx_t_2 = (((*__pyx_v_span.first).first < (__pyx_v_self->case_starts_[(__pyx_v_v + 1)])) != 0);
         __pyx_t_1 = __pyx_t_2;
         __pyx_L17_bool_binop_done:;
         if (!__pyx_t_1) break;
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":308
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":321
  * 
  *                 while (span.first != span.second and deref(span.first).first < self.case_starts_[v+1]):
  *                     case_u = ci - self.case_starts_[u]             # <<<<<<<<<<<<<<
  *                     case_v = deref(span.first).first - self.case_starts_[v]
  *                     quadratic_view[case_u, case_v] = deref(span.first).second
  */
         __pyx_v_case_u = (__pyx_v_ci - (__pyx_v_self->case_starts_[__pyx_v_u]));
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":309
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":322
  *                 while (span.first != span.second and deref(span.first).first < self.case_starts_[v+1]):
  *                     case_u = ci - self.case_starts_[u]
  *                     case_v = deref(span.first).first - self.case_starts_[v]             # <<<<<<<<<<<<<<
  *                     quadratic_view[case_u, case_v] = deref(span.first).second
  * 
  */
         __pyx_v_case_v = ((*__pyx_v_span.first).first - (__pyx_v_self->case_starts_[__pyx_v_v]));
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":310
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":323
  *                     case_u = ci - self.case_starts_[u]
  *                     case_v = deref(span.first).first - self.case_starts_[v]
  *                     quadratic_view[case_u, case_v] = deref(span.first).second             # <<<<<<<<<<<<<<
  * 
  *                     inc(span.first)
  */
         __pyx_t_14 = (*__pyx_v_span.first).second;
@@ -12263,80 +13140,80 @@
         } else if (unlikely(__pyx_t_15 >= __pyx_v_quadratic_view.shape[0])) __pyx_t_17 = 0;
         if (__pyx_t_16 < 0) {
           __pyx_t_16 += __pyx_v_quadratic_view.shape[1];
           if (unlikely(__pyx_t_16 < 0)) __pyx_t_17 = 1;
         } else if (unlikely(__pyx_t_16 >= __pyx_v_quadratic_view.shape[1])) __pyx_t_17 = 1;
         if (unlikely(__pyx_t_17 != -1)) {
           __Pyx_RaiseBufferIndexError(__pyx_t_17);
-          __PYX_ERR(0, 310, __pyx_L1_error)
+          __PYX_ERR(0, 323, __pyx_L1_error)
         }
         *((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_quadratic_view.data + __pyx_t_15 * __pyx_v_quadratic_view.strides[0]) ) + __pyx_t_16 * __pyx_v_quadratic_view.strides[1]) )) = __pyx_t_14;
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":312
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":325
  *                     quadratic_view[case_u, case_v] = deref(span.first).second
  * 
  *                     inc(span.first)             # <<<<<<<<<<<<<<
  * 
  *         else:
  */
         (void)((++__pyx_v_span.first));
       }
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":297
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":310
  *         cdef Bias[:, :] quadratic_view
  * 
  *         if array:             # <<<<<<<<<<<<<<
  *             # build a numpy array
  *             quadratic = np.zeros((self.num_cases(u), self.num_cases(v)),
  */
     goto __pyx_L12;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":316
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":329
  *         else:
  *             # store in a dict
  *             quadratic = {}             # <<<<<<<<<<<<<<
  * 
  *             for ci in range(self.case_starts_[u], self.case_starts_[u+1]):
  */
   /*else*/ {
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 316, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 329, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_v_quadratic = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":318
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":331
  *             quadratic = {}
  * 
  *             for ci in range(self.case_starts_[u], self.case_starts_[u+1]):             # <<<<<<<<<<<<<<
  * 
  *                 span = self.bqm_.neighborhood(ci, self.case_starts_[v])
  */
     __pyx_t_10 = (__pyx_v_self->case_starts_[(__pyx_v_u + 1)]);
     __pyx_t_11 = __pyx_t_10;
     for (__pyx_t_12 = (__pyx_v_self->case_starts_[__pyx_v_u]); __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
       __pyx_v_ci = __pyx_t_12;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":320
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":333
  *             for ci in range(self.case_starts_[u], self.case_starts_[u+1]):
  * 
  *                 span = self.bqm_.neighborhood(ci, self.case_starts_[v])             # <<<<<<<<<<<<<<
  * 
  *                 while (span.first != span.second and deref(span.first).first < self.case_starts_[v+1]):
  */
       try {
         __pyx_t_13 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci, (__pyx_v_self->case_starts_[__pyx_v_v]));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 320, __pyx_L1_error)
+        __PYX_ERR(0, 333, __pyx_L1_error)
       }
       __pyx_v_span = __pyx_t_13;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":322
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":335
  *                 span = self.bqm_.neighborhood(ci, self.case_starts_[v])
  * 
  *                 while (span.first != span.second and deref(span.first).first < self.case_starts_[v+1]):             # <<<<<<<<<<<<<<
  *                     case_u = ci - self.case_starts_[u]
  *                     case_v = deref(span.first).first - self.case_starts_[v]
  */
       while (1) {
@@ -12347,83 +13224,83 @@
           goto __pyx_L23_bool_binop_done;
         }
         __pyx_t_2 = (((*__pyx_v_span.first).first < (__pyx_v_self->case_starts_[(__pyx_v_v + 1)])) != 0);
         __pyx_t_1 = __pyx_t_2;
         __pyx_L23_bool_binop_done:;
         if (!__pyx_t_1) break;
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":323
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":336
  * 
  *                 while (span.first != span.second and deref(span.first).first < self.case_starts_[v+1]):
  *                     case_u = ci - self.case_starts_[u]             # <<<<<<<<<<<<<<
  *                     case_v = deref(span.first).first - self.case_starts_[v]
  *                     quadratic[case_u, case_v] = deref(span.first).second
  */
         __pyx_v_case_u = (__pyx_v_ci - (__pyx_v_self->case_starts_[__pyx_v_u]));
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":324
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":337
  *                 while (span.first != span.second and deref(span.first).first < self.case_starts_[v+1]):
  *                     case_u = ci - self.case_starts_[u]
  *                     case_v = deref(span.first).first - self.case_starts_[v]             # <<<<<<<<<<<<<<
  *                     quadratic[case_u, case_v] = deref(span.first).second
  * 
  */
         __pyx_v_case_v = ((*__pyx_v_span.first).first - (__pyx_v_self->case_starts_[__pyx_v_v]));
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":325
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":338
  *                     case_u = ci - self.case_starts_[u]
  *                     case_v = deref(span.first).first - self.case_starts_[v]
  *                     quadratic[case_u, case_v] = deref(span.first).second             # <<<<<<<<<<<<<<
  * 
  *                     inc(span.first)
  */
-        __pyx_t_3 = PyFloat_FromDouble((*__pyx_v_span.first).second); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 325, __pyx_L1_error)
+        __pyx_t_3 = PyFloat_FromDouble((*__pyx_v_span.first).second); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 338, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_8 = PyInt_FromSsize_t(__pyx_v_case_u); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 325, __pyx_L1_error)
+        __pyx_t_8 = PyInt_FromSsize_t(__pyx_v_case_u); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 338, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_case_v); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 325, __pyx_L1_error)
+        __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_case_v); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 338, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 325, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 338, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_GIVEREF(__pyx_t_8);
         PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_8);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
         __pyx_t_8 = 0;
         __pyx_t_7 = 0;
-        if (unlikely(PyObject_SetItem(__pyx_v_quadratic, __pyx_t_4, __pyx_t_3) < 0)) __PYX_ERR(0, 325, __pyx_L1_error)
+        if (unlikely(PyObject_SetItem(__pyx_v_quadratic, __pyx_t_4, __pyx_t_3) < 0)) __PYX_ERR(0, 338, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":327
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":340
  *                     quadratic[case_u, case_v] = deref(span.first).second
  * 
  *                     inc(span.first)             # <<<<<<<<<<<<<<
  * 
  *         # todo: support scipy sparse matrices?
  */
         (void)((++__pyx_v_span.first));
       }
     }
   }
   __pyx_L12:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":331
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":344
  *         # todo: support scipy sparse matrices?
  * 
  *         return quadratic             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_quadratic);
   __pyx_r = __pyx_v_quadratic;
   goto __pyx_L0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":281
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":294
  *         return self.bqm_.get_linear(self.case_starts_[v] + case)
  * 
  *     def get_quadratic(self, VarIndex u, VarIndex v, bint array=False):             # <<<<<<<<<<<<<<
  * 
  *         # check that the interaction does in fact exist
  */
 
@@ -12440,15 +13317,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_quadratic_view, 1);
   __Pyx_XDECREF(__pyx_v_quadratic);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dimod/discrete/cydiscrete_quadratic_model.pyx":335
+/* "dimod/discrete/cydiscrete_quadratic_model.pyx":348
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Bias get_quadratic_case(self,             # <<<<<<<<<<<<<<
  *                                   VarIndex u, CaseIndex case_u,
  *                                   VarIndex v, CaseIndex case_v)  except? -45.3:
  */
 
@@ -12483,24 +13360,24 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_quadratic_case); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 335, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_quadratic_case); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 348, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_17get_quadratic_case)) {
-        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_u); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 335, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_u); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 348, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_u); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 335, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_u); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 348, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 335, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 348, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
-        __pyx_t_6 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_v); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 335, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_v); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 348, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_7 = __pyx_t_1; __pyx_t_8 = NULL;
         __pyx_t_9 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
           __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
           if (likely(__pyx_t_8)) {
@@ -12510,37 +13387,37 @@
             __Pyx_DECREF_SET(__pyx_t_7, function);
             __pyx_t_9 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_7)) {
           PyObject *__pyx_temp[5] = {__pyx_t_8, __pyx_t_3, __pyx_t_4, __pyx_t_5, __pyx_t_6};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 4+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 4+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
           PyObject *__pyx_temp[5] = {__pyx_t_8, __pyx_t_3, __pyx_t_4, __pyx_t_5, __pyx_t_6};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 4+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 4+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         } else
         #endif
         {
-          __pyx_t_10 = PyTuple_New(4+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 335, __pyx_L1_error)
+          __pyx_t_10 = PyTuple_New(4+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 348, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_10);
           if (__pyx_t_8) {
             __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_4);
@@ -12549,20 +13426,20 @@
           PyTuple_SET_ITEM(__pyx_t_10, 2+__pyx_t_9, __pyx_t_5);
           __Pyx_GIVEREF(__pyx_t_6);
           PyTuple_SET_ITEM(__pyx_t_10, 3+__pyx_t_9, __pyx_t_6);
           __pyx_t_3 = 0;
           __pyx_t_4 = 0;
           __pyx_t_5 = 0;
           __pyx_t_6 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         }
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __pyx_t_11 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_11 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 335, __pyx_L1_error)
+        __pyx_t_11 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_11 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 348, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_11;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -12573,50 +13450,50 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":339
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":352
  *                                   VarIndex v, CaseIndex case_v)  except? -45.3:
  * 
  *         if case_u < 0 or case_u >= self.num_cases(u):             # <<<<<<<<<<<<<<
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case_u, self.num_cases(u)))
  */
   __pyx_t_13 = ((__pyx_v_case_u < 0) != 0);
   if (!__pyx_t_13) {
   } else {
     __pyx_t_12 = __pyx_t_13;
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_15.__pyx_n = 1;
   __pyx_t_15.v = __pyx_v_u;
-  __pyx_t_14 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_15); if (unlikely(__pyx_t_14 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 339, __pyx_L1_error)
+  __pyx_t_14 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_15); if (unlikely(__pyx_t_14 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 352, __pyx_L1_error)
   __pyx_t_13 = ((__pyx_v_case_u >= __pyx_t_14) != 0);
   __pyx_t_12 = __pyx_t_13;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_12)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":341
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":354
  *         if case_u < 0 or case_u >= self.num_cases(u):
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case_u, self.num_cases(u)))             # <<<<<<<<<<<<<<
  * 
  *         if case_v < 0 or case_v >= self.num_cases(v):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_case_is_invalid_variable_only_su, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 341, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_case_is_invalid_variable_only_su, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_u); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 341, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_u); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_15.__pyx_n = 1;
     __pyx_t_15.v = __pyx_v_u;
-    __pyx_t_14 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_15); if (unlikely(__pyx_t_14 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 341, __pyx_L1_error)
-    __pyx_t_10 = PyInt_FromSsize_t(__pyx_t_14); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 341, __pyx_L1_error)
+    __pyx_t_14 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_15); if (unlikely(__pyx_t_14 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 354, __pyx_L1_error)
+    __pyx_t_10 = PyInt_FromSsize_t(__pyx_t_14); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_6 = NULL;
     __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -12625,108 +13502,108 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_9 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_7, __pyx_t_10};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 354, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_7, __pyx_t_10};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 354, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 341, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 354, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (__pyx_t_6) {
         __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6); __pyx_t_6 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_7);
       PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_9, __pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_10);
       PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_9, __pyx_t_10);
       __pyx_t_7 = 0;
       __pyx_t_10 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 354, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":340
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":353
  * 
  *         if case_u < 0 or case_u >= self.num_cases(u):
  *             raise ValueError("case {} is invalid, variable only supports {} "             # <<<<<<<<<<<<<<
  *                              "cases".format(case_u, self.num_cases(u)))
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 353, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 340, __pyx_L1_error)
+    __PYX_ERR(0, 353, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":339
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":352
  *                                   VarIndex v, CaseIndex case_v)  except? -45.3:
  * 
  *         if case_u < 0 or case_u >= self.num_cases(u):             # <<<<<<<<<<<<<<
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case_u, self.num_cases(u)))
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":343
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":356
  *                              "cases".format(case_u, self.num_cases(u)))
  * 
  *         if case_v < 0 or case_v >= self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case_v, self.num_cases(v)))
  */
   __pyx_t_13 = ((__pyx_v_case_v < 0) != 0);
   if (!__pyx_t_13) {
   } else {
     __pyx_t_12 = __pyx_t_13;
     goto __pyx_L7_bool_binop_done;
   }
   __pyx_t_15.__pyx_n = 1;
   __pyx_t_15.v = __pyx_v_v;
-  __pyx_t_14 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_15); if (unlikely(__pyx_t_14 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 343, __pyx_L1_error)
+  __pyx_t_14 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_15); if (unlikely(__pyx_t_14 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 356, __pyx_L1_error)
   __pyx_t_13 = ((__pyx_v_case_v >= __pyx_t_14) != 0);
   __pyx_t_12 = __pyx_t_13;
   __pyx_L7_bool_binop_done:;
   if (unlikely(__pyx_t_12)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":345
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":358
  *         if case_v < 0 or case_v >= self.num_cases(v):
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case_v, self.num_cases(v)))             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_case_is_invalid_variable_only_su, __pyx_n_s_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 345, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_case_is_invalid_variable_only_su, __pyx_n_s_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 358, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 345, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 358, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_15.__pyx_n = 1;
     __pyx_t_15.v = __pyx_v_v;
-    __pyx_t_14 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_15); if (unlikely(__pyx_t_14 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 345, __pyx_L1_error)
-    __pyx_t_10 = PyInt_FromSsize_t(__pyx_t_14); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 345, __pyx_L1_error)
+    __pyx_t_14 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_15); if (unlikely(__pyx_t_14 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 358, __pyx_L1_error)
+    __pyx_t_10 = PyInt_FromSsize_t(__pyx_t_14); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 358, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_7 = NULL;
     __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -12735,107 +13612,107 @@
         __Pyx_DECREF_SET(__pyx_t_1, function);
         __pyx_t_9 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_1)) {
       PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_5, __pyx_t_10};
-      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 358, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
       PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_5, __pyx_t_10};
-      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 358, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     } else
     #endif
     {
-      __pyx_t_6 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 345, __pyx_L1_error)
+      __pyx_t_6 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 358, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       if (__pyx_t_7) {
         __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7); __pyx_t_7 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_9, __pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_10);
       PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_9, __pyx_t_10);
       __pyx_t_5 = 0;
       __pyx_t_10 = 0;
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 358, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":344
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":357
  * 
  *         if case_v < 0 or case_v >= self.num_cases(v):
  *             raise ValueError("case {} is invalid, variable only supports {} "             # <<<<<<<<<<<<<<
  *                              "cases".format(case_v, self.num_cases(v)))
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 344, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 357, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 344, __pyx_L1_error)
+    __PYX_ERR(0, 357, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":343
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":356
  *                              "cases".format(case_u, self.num_cases(u)))
  * 
  *         if case_v < 0 or case_v >= self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case_v, self.num_cases(v)))
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":348
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":361
  * 
  * 
  *         cdef CaseIndex cu = self.case_starts_[u] + case_u             # <<<<<<<<<<<<<<
  *         cdef CaseIndex cv = self.case_starts_[v] + case_v
  * 
  */
   __pyx_v_cu = ((__pyx_v_self->case_starts_[__pyx_v_u]) + __pyx_v_case_u);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":349
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":362
  * 
  *         cdef CaseIndex cu = self.case_starts_[u] + case_u
  *         cdef CaseIndex cv = self.case_starts_[v] + case_v             # <<<<<<<<<<<<<<
  * 
  *         return self.bqm_.get_quadratic(cu, cv).first
  */
   __pyx_v_cv = ((__pyx_v_self->case_starts_[__pyx_v_v]) + __pyx_v_case_v);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":351
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":364
  *         cdef CaseIndex cv = self.case_starts_[v] + case_v
  * 
  *         return self.bqm_.get_quadratic(cu, cv).first             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
  */
   try {
     __pyx_t_16 = __pyx_v_self->bqm_.get_quadratic(__pyx_v_cu, __pyx_v_cv);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 351, __pyx_L1_error)
+    __PYX_ERR(0, 364, __pyx_L1_error)
   }
   __pyx_r = __pyx_t_16.first;
   goto __pyx_L0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":335
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":348
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Bias get_quadratic_case(self,             # <<<<<<<<<<<<<<
  *                                   VarIndex u, CaseIndex case_u,
  *                                   VarIndex v, CaseIndex case_v)  except? -45.3:
  */
 
@@ -12893,48 +13770,48 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_u)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_case_u)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_quadratic_case", 1, 4, 4, 1); __PYX_ERR(0, 335, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_quadratic_case", 1, 4, 4, 1); __PYX_ERR(0, 348, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_quadratic_case", 1, 4, 4, 2); __PYX_ERR(0, 335, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_quadratic_case", 1, 4, 4, 2); __PYX_ERR(0, 348, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_case_v)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_quadratic_case", 1, 4, 4, 3); __PYX_ERR(0, 335, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_quadratic_case", 1, 4, 4, 3); __PYX_ERR(0, 348, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_quadratic_case") < 0)) __PYX_ERR(0, 335, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_quadratic_case") < 0)) __PYX_ERR(0, 348, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
-    __pyx_v_u = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_u == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 336, __pyx_L3_error)
-    __pyx_v_case_u = __Pyx_PyInt_As_npy_int64(values[1]); if (unlikely((__pyx_v_case_u == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 336, __pyx_L3_error)
-    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[2]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 337, __pyx_L3_error)
-    __pyx_v_case_v = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_case_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 337, __pyx_L3_error)
+    __pyx_v_u = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_u == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 349, __pyx_L3_error)
+    __pyx_v_case_u = __Pyx_PyInt_As_npy_int64(values[1]); if (unlikely((__pyx_v_case_u == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 349, __pyx_L3_error)
+    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[2]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 350, __pyx_L3_error)
+    __pyx_v_case_v = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_case_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 350, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_quadratic_case", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 335, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_quadratic_case", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 348, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.get_quadratic_case", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_16get_quadratic_case(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self), __pyx_v_u, __pyx_v_case_u, __pyx_v_v, __pyx_v_case_v);
 
@@ -12949,16 +13826,16 @@
   __pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_quadratic_case", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_get_quadratic_case(__pyx_v_self, __pyx_v_u, __pyx_v_case_u, __pyx_v_v, __pyx_v_case_v, 1); if (unlikely(__pyx_t_1 == ((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias)(-45.3)) && PyErr_Occurred())) __PYX_ERR(0, 335, __pyx_L1_error)
-  __pyx_t_2 = PyFloat_FromDouble(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_get_quadratic_case(__pyx_v_self, __pyx_v_u, __pyx_v_case_u, __pyx_v_v, __pyx_v_case_v, 1); if (unlikely(__pyx_t_1 == ((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias)(-45.3)) && PyErr_Occurred())) __PYX_ERR(0, 348, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -12967,15 +13844,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dimod/discrete/cydiscrete_quadratic_model.pyx":355
+/* "dimod/discrete/cydiscrete_quadratic_model.pyx":368
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t num_cases(self, Py_ssize_t v=-1) except -1:             # <<<<<<<<<<<<<<
  *         """If v is provided, the number of cases associated with v, otherwise
  *         the total number of cases in the DQM.
  */
 
@@ -13006,18 +13883,18 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_num_cases); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 355, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_num_cases); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 368, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_19num_cases)) {
-        __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 355, __pyx_L1_error)
+        __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 368, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_5 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_5)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -13025,18 +13902,18 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
         __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 355, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 368, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 355, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 368, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_6;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -13047,113 +13924,113 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":359
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":372
  *         the total number of cases in the DQM.
  *         """
  *         if v < 0:             # <<<<<<<<<<<<<<
  *             return self.bqm_.num_variables()
  * 
  */
   __pyx_t_7 = ((__pyx_v_v < 0) != 0);
   if (__pyx_t_7) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":360
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":373
  *         """
  *         if v < 0:
  *             return self.bqm_.num_variables()             # <<<<<<<<<<<<<<
  * 
  *         if v >= self.num_variables():
  */
     try {
       __pyx_t_8 = __pyx_v_self->bqm_.num_variables();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 360, __pyx_L1_error)
+      __PYX_ERR(0, 373, __pyx_L1_error)
     }
     __pyx_r = __pyx_t_8;
     goto __pyx_L0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":359
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":372
  *         the total number of cases in the DQM.
  *         """
  *         if v < 0:             # <<<<<<<<<<<<<<
  *             return self.bqm_.num_variables()
  * 
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":362
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":375
  *             return self.bqm_.num_variables()
  * 
  *         if v >= self.num_variables():             # <<<<<<<<<<<<<<
  *             raise ValueError("unknown variable {}".format(v))
  * 
  */
   __pyx_t_7 = ((__pyx_v_v >= ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_variables(__pyx_v_self, 0)) != 0);
   if (unlikely(__pyx_t_7)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":363
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":376
  * 
  *         if v >= self.num_variables():
  *             raise ValueError("unknown variable {}".format(v))             # <<<<<<<<<<<<<<
  * 
  *         return self.case_starts_[v+1] - self.case_starts_[v]
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_unknown_variable_2, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 363, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_unknown_variable_2, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 376, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_v); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 363, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_v); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 376, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 363, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 376, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 363, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 376, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 363, __pyx_L1_error)
+    __PYX_ERR(0, 376, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":362
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":375
  *             return self.bqm_.num_variables()
  * 
  *         if v >= self.num_variables():             # <<<<<<<<<<<<<<
  *             raise ValueError("unknown variable {}".format(v))
  * 
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":365
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":378
  *             raise ValueError("unknown variable {}".format(v))
  * 
  *         return self.case_starts_[v+1] - self.case_starts_[v]             # <<<<<<<<<<<<<<
  * 
  *     cpdef Py_ssize_t num_case_interactions(self):
  */
   __pyx_r = ((__pyx_v_self->case_starts_[(__pyx_v_v + 1)]) - (__pyx_v_self->case_starts_[__pyx_v_v]));
   goto __pyx_L0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":355
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":368
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t num_cases(self, Py_ssize_t v=-1) except -1:             # <<<<<<<<<<<<<<
  *         """If v is provided, the number of cases associated with v, otherwise
  *         the total number of cases in the DQM.
  */
 
@@ -13199,33 +14076,33 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "num_cases") < 0)) __PYX_ERR(0, 355, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "num_cases") < 0)) __PYX_ERR(0, 368, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
-      __pyx_v_v = __Pyx_PyIndex_AsSsize_t(values[0]); if (unlikely((__pyx_v_v == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 355, __pyx_L3_error)
+      __pyx_v_v = __Pyx_PyIndex_AsSsize_t(values[0]); if (unlikely((__pyx_v_v == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 368, __pyx_L3_error)
     } else {
       __pyx_v_v = ((Py_ssize_t)-1L);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("num_cases", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 355, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("num_cases", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 368, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.num_cases", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_18num_cases(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self), __pyx_v_v);
 
@@ -13243,16 +14120,16 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("num_cases", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.v = __pyx_v_v;
-  __pyx_t_1 = __pyx_vtabptr_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel->num_cases(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 355, __pyx_L1_error)
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel->num_cases(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 368, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 368, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13261,15 +14138,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dimod/discrete/cydiscrete_quadratic_model.pyx":367
+/* "dimod/discrete/cydiscrete_quadratic_model.pyx":380
  *         return self.case_starts_[v+1] - self.case_starts_[v]
  * 
  *     cpdef Py_ssize_t num_case_interactions(self):             # <<<<<<<<<<<<<<
  *         """The total number of case interactions."""
  *         return self.bqm_.num_interactions()
  */
 
@@ -13292,15 +14169,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_num_case_interactions); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 367, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_num_case_interactions); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 380, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_21num_case_interactions)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -13308,18 +14185,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 367, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 380, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 367, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 380, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -13330,31 +14207,31 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":369
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":382
  *     cpdef Py_ssize_t num_case_interactions(self):
  *         """The total number of case interactions."""
  *         return self.bqm_.num_interactions()             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
  */
   try {
     __pyx_t_6 = __pyx_v_self->bqm_.num_interactions();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 369, __pyx_L1_error)
+    __PYX_ERR(0, 382, __pyx_L1_error)
   }
   __pyx_r = __pyx_t_6;
   goto __pyx_L0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":367
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":380
  *         return self.case_starts_[v+1] - self.case_starts_[v]
  * 
  *     cpdef Py_ssize_t num_case_interactions(self):             # <<<<<<<<<<<<<<
  *         """The total number of case interactions."""
  *         return self.bqm_.num_interactions()
  */
 
@@ -13390,15 +14267,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("num_case_interactions", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_num_case_interactions(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_num_case_interactions(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 380, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13407,15 +14284,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dimod/discrete/cydiscrete_quadratic_model.pyx":373
+/* "dimod/discrete/cydiscrete_quadratic_model.pyx":386
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t num_variable_interactions(self) except -1:             # <<<<<<<<<<<<<<
  *         """The total number of case interactions."""
  *         cdef Py_ssize_t num = 0
  */
 
@@ -13441,15 +14318,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_num_variable_interactions); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 373, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_num_variable_interactions); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 386, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_23num_variable_interactions)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -13457,18 +14334,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 373, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 386, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 373, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 386, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -13479,56 +14356,56 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":375
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":388
  *     cpdef Py_ssize_t num_variable_interactions(self) except -1:
  *         """The total number of case interactions."""
  *         cdef Py_ssize_t num = 0             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t v
  *         for v in range(self.num_variables()):
  */
   __pyx_v_num = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":377
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":390
  *         cdef Py_ssize_t num = 0
  *         cdef Py_ssize_t v
  *         for v in range(self.num_variables()):             # <<<<<<<<<<<<<<
  *             num += self.adj_[v].size()
  *         return num // 2
  */
   __pyx_t_5 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_variables(__pyx_v_self, 0);
   __pyx_t_6 = __pyx_t_5;
   for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
     __pyx_v_v = __pyx_t_7;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":378
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
  *         cdef Py_ssize_t v
  *         for v in range(self.num_variables()):
  *             num += self.adj_[v].size()             # <<<<<<<<<<<<<<
  *         return num // 2
  * 
  */
     __pyx_v_num = (__pyx_v_num + (__pyx_v_self->adj_[__pyx_v_v]).size());
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":379
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":392
  *         for v in range(self.num_variables()):
  *             num += self.adj_[v].size()
  *         return num // 2             # <<<<<<<<<<<<<<
  * 
  *     cpdef Py_ssize_t num_variables(self):
  */
   __pyx_r = __Pyx_div_Py_ssize_t(__pyx_v_num, 2);
   goto __pyx_L0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":373
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":386
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t num_variable_interactions(self) except -1:             # <<<<<<<<<<<<<<
  *         """The total number of case interactions."""
  *         cdef Py_ssize_t num = 0
  */
 
@@ -13565,16 +14442,16 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("num_variable_interactions", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_num_variable_interactions(__pyx_v_self, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 373, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 373, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_num_variable_interactions(__pyx_v_self, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 386, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13583,15 +14460,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dimod/discrete/cydiscrete_quadratic_model.pyx":381
+/* "dimod/discrete/cydiscrete_quadratic_model.pyx":394
  *         return num // 2
  * 
  *     cpdef Py_ssize_t num_variables(self):             # <<<<<<<<<<<<<<
  *         """The number of discrete variables in the DQM."""
  *         return self.adj_.size()
  */
 
@@ -13613,15 +14490,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_num_variables); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 381, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_num_variables); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 394, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_25num_variables)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -13629,18 +14506,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 381, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 394, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 381, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 394, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -13651,25 +14528,25 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":383
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":396
  *     cpdef Py_ssize_t num_variables(self):
  *         """The number of discrete variables in the DQM."""
  *         return self.adj_.size()             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
  */
   __pyx_r = __pyx_v_self->adj_.size();
   goto __pyx_L0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":381
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":394
  *         return num // 2
  * 
  *     cpdef Py_ssize_t num_variables(self):             # <<<<<<<<<<<<<<
  *         """The number of discrete variables in the DQM."""
  *         return self.adj_.size()
  */
 
@@ -13705,15 +14582,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("num_variables", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_num_variables(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 381, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_num_variables(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 394, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13722,15 +14599,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dimod/discrete/cydiscrete_quadratic_model.pyx":387
+/* "dimod/discrete/cydiscrete_quadratic_model.pyx":400
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t set_linear(self, VarIndex v, Numeric[:] biases) except -1:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
 
@@ -13768,40 +14645,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_args)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_kwargs)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 3, 3, 1); __PYX_ERR(0, 387, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 3, 3, 1); __PYX_ERR(0, 400, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_defaults)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 3, 3, 2); __PYX_ERR(0, 387, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 3, 3, 2); __PYX_ERR(0, 400, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fused_cpdef") < 0)) __PYX_ERR(0, 387, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fused_cpdef") < 0)) __PYX_ERR(0, 400, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_args = values[0];
     __pyx_v_kwargs = values[1];
     __pyx_v_defaults = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 387, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 400, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.__pyx_fused_cpdef", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_26set_linear(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_signatures), __pyx_v_args, __pyx_v_kwargs, __pyx_v_defaults);
 
@@ -13855,59 +14732,59 @@
   Py_ssize_t __pyx_t_17;
   int __pyx_t_18;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_linear", 0);
   __Pyx_INCREF(__pyx_v_kwargs);
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyList_SET_ITEM(__pyx_t_1, 0, Py_None);
   __pyx_v_dest_sig = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_v_kwargs != Py_None);
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_kwargs); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_kwargs); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
   __pyx_t_3 = ((!__pyx_t_4) != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_2) {
     __Pyx_INCREF(Py_None);
     __Pyx_DECREF_SET(__pyx_v_kwargs, Py_None);
   }
-  __pyx_t_1 = ((PyObject *)__Pyx_ImportNumPyArrayTypeIfAvailable()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__Pyx_ImportNumPyArrayTypeIfAvailable()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_ndarray = ((PyTypeObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   __pyx_v_itemsize = -1L;
   __pyx_v____pyx_uint8_t_is_signed = (!((((__pyx_t_5numpy_uint8_t)-1L) > 0) != 0));
   __pyx_v____pyx_uint16_t_is_signed = (!((((__pyx_t_5numpy_uint16_t)-1L) > 0) != 0));
   __pyx_v____pyx_uint32_t_is_signed = (!((((__pyx_t_5numpy_uint32_t)-1L) > 0) != 0));
   __pyx_v____pyx_uint64_t_is_signed = (!((((__pyx_t_5numpy_uint64_t)-1L) > 0) != 0));
   __pyx_v____pyx_int8_t_is_signed = (!((((__pyx_t_5numpy_int8_t)-1L) > 0) != 0));
   __pyx_v____pyx_int16_t_is_signed = (!((((__pyx_t_5numpy_int16_t)-1L) > 0) != 0));
   __pyx_v____pyx_int32_t_is_signed = (!((((__pyx_t_5numpy_int32_t)-1L) > 0) != 0));
   __pyx_v____pyx_int64_t_is_signed = (!((((__pyx_t_5numpy_int64_t)-1L) > 0) != 0));
   if (unlikely(__pyx_v_args == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 387, __pyx_L1_error)
+    __PYX_ERR(0, 400, __pyx_L1_error)
   }
-  __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 400, __pyx_L1_error)
   __pyx_t_2 = ((2 < __pyx_t_5) != 0);
   if (__pyx_t_2) {
     if (unlikely(__pyx_v_args == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 387, __pyx_L1_error)
+      __PYX_ERR(0, 400, __pyx_L1_error)
     }
     __pyx_t_1 = PyTuple_GET_ITEM(((PyObject*)__pyx_v_args), 2);
     __Pyx_INCREF(__pyx_t_1);
     __pyx_v_arg = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L6;
   }
@@ -13916,85 +14793,85 @@
   if (__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L7_bool_binop_done;
   }
   if (unlikely(__pyx_v_kwargs == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 387, __pyx_L1_error)
+    __PYX_ERR(0, 400, __pyx_L1_error)
   }
-  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_biases, ((PyObject*)__pyx_v_kwargs), Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_biases, ((PyObject*)__pyx_v_kwargs), Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_4 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L7_bool_binop_done:;
   if (__pyx_t_2) {
     if (unlikely(__pyx_v_kwargs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 387, __pyx_L1_error)
+      __PYX_ERR(0, 400, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_kwargs), __pyx_n_s_biases); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_kwargs), __pyx_n_s_biases); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_arg = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L6;
   }
   /*else*/ {
     if (unlikely(__pyx_v_args == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 387, __pyx_L1_error)
+      __PYX_ERR(0, 400, __pyx_L1_error)
     }
-    __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 387, __pyx_L1_error)
-    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 400, __pyx_L1_error)
+    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_int_3);
     __Pyx_GIVEREF(__pyx_int_3);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_int_3);
     __Pyx_INCREF(__pyx_n_s_s);
     __Pyx_GIVEREF(__pyx_n_s_s);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_n_s_s);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_Expected_at_least_d_argument_s_g, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_Expected_at_least_d_argument_s_g, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 387, __pyx_L1_error)
+    __PYX_ERR(0, 400, __pyx_L1_error)
   }
   __pyx_L6:;
   while (1) {
     __pyx_t_2 = (__pyx_v_ndarray != ((PyTypeObject*)Py_None));
     __pyx_t_3 = (__pyx_t_2 != 0);
     if (__pyx_t_3) {
       __pyx_t_3 = __Pyx_TypeCheck(__pyx_v_arg, __pyx_v_ndarray); 
       __pyx_t_2 = (__pyx_t_3 != 0);
       if (__pyx_t_2) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_dtype = __pyx_t_6;
         __pyx_t_6 = 0;
         goto __pyx_L12;
       }
       __pyx_t_2 = __pyx_memoryview_check(__pyx_v_arg); 
       __pyx_t_3 = (__pyx_t_2 != 0);
       if (__pyx_t_3) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_base); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_base); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_arg_base = __pyx_t_6;
         __pyx_t_6 = 0;
         __pyx_t_3 = __Pyx_TypeCheck(__pyx_v_arg_base, __pyx_v_ndarray); 
         __pyx_t_2 = (__pyx_t_3 != 0);
         if (__pyx_t_2) {
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg_base, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg_base, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_v_dtype = __pyx_t_6;
           __pyx_t_6 = 0;
           goto __pyx_L13;
         }
         /*else*/ {
           __Pyx_INCREF(Py_None);
@@ -14008,246 +14885,246 @@
         __pyx_v_dtype = Py_None;
       }
       __pyx_L12:;
       __pyx_v_itemsize = -1L;
       __pyx_t_2 = (__pyx_v_dtype != Py_None);
       __pyx_t_3 = (__pyx_t_2 != 0);
       if (__pyx_t_3) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_itemsize); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_itemsize); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_itemsize = __pyx_t_5;
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_kind); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_kind); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_7 = __Pyx_PyObject_Ord(__pyx_t_6); if (unlikely(__pyx_t_7 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyObject_Ord(__pyx_t_6); if (unlikely(__pyx_t_7 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_kind = __pyx_t_7;
         __pyx_v_dtype_signed = (__pyx_v_kind == 'i');
         switch (__pyx_v_kind) {
           case 'i':
           case 'u':
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_uint8_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L16_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L16_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_uint8_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L16_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_uint16_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L20_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L20_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_uint16_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L20_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_uint32_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L24_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L24_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_uint32_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L24_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_uint64_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L28_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L28_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_uint64_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L28_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_int8_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L32_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L32_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_int8_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L32_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_int16_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L36_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L36_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_int16_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L36_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_int32_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L40_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L40_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_int32_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L40_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_int64_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L44_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L44_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_int64_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L44_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           break;
           case 'f':
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_float32_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L48_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L48_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_float64_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L51_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L51_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           break;
           case 'c':
           break;
           case 'O':
           break;
@@ -14266,15 +15143,15 @@
     __pyx_L54_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint8_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -14288,15 +15165,15 @@
     __pyx_L58_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint16_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -14310,15 +15187,15 @@
     __pyx_L62_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -14332,15 +15209,15 @@
     __pyx_L66_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -14354,15 +15231,15 @@
     __pyx_L70_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int8_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -14376,15 +15253,15 @@
     __pyx_L74_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int16_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -14398,15 +15275,15 @@
     __pyx_L78_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int32_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -14420,15 +15297,15 @@
     __pyx_L82_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int64_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -14442,15 +15319,15 @@
     __pyx_L86_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float32_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -14464,100 +15341,100 @@
     __pyx_L90_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, Py_None, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, Py_None, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
     goto __pyx_L10_break;
   }
   __pyx_L10_break:;
-  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_v_candidates = ((PyObject*)__pyx_t_6);
   __pyx_t_6 = 0;
   __pyx_t_5 = 0;
   if (unlikely(((PyObject *)__pyx_v_signatures) == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 387, __pyx_L1_error)
+    __PYX_ERR(0, 400, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_dict_iterator(((PyObject*)__pyx_v_signatures), 1, ((PyObject *)NULL), (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_dict_iterator(((PyObject*)__pyx_v_signatures), 1, ((PyObject *)NULL), (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_6);
   __pyx_t_6 = __pyx_t_1;
   __pyx_t_1 = 0;
   while (1) {
     __pyx_t_11 = __Pyx_dict_iter_next(__pyx_t_6, __pyx_t_9, &__pyx_t_5, &__pyx_t_1, NULL, NULL, __pyx_t_10);
     if (unlikely(__pyx_t_11 == 0)) break;
-    if (unlikely(__pyx_t_11 == -1)) __PYX_ERR(0, 387, __pyx_L1_error)
+    if (unlikely(__pyx_t_11 == -1)) __PYX_ERR(0, 400, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_sig, __pyx_t_1);
     __pyx_t_1 = 0;
     __pyx_v_match_found = 0;
-    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_sig, __pyx_n_s_strip); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_sig, __pyx_n_s_strip); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 400, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __pyx_t_14 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
       __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_13);
       if (likely(__pyx_t_14)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
         __Pyx_INCREF(__pyx_t_14);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_13, function);
       }
     }
     __pyx_t_12 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_14, __pyx_kp_s__10) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_kp_s__10);
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-    if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 387, __pyx_L1_error)
+    if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 400, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_split); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_split); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 400, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     __pyx_t_12 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
       __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_13);
       if (likely(__pyx_t_12)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
         __Pyx_INCREF(__pyx_t_12);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_13, function);
       }
     }
     __pyx_t_1 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_12, __pyx_kp_s__11) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_kp_s__11);
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
     __Pyx_XDECREF_SET(__pyx_v_src_sig, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_15 = PyList_GET_SIZE(__pyx_v_dest_sig); if (unlikely(__pyx_t_15 == ((Py_ssize_t)-1))) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_15 = PyList_GET_SIZE(__pyx_v_dest_sig); if (unlikely(__pyx_t_15 == ((Py_ssize_t)-1))) __PYX_ERR(0, 400, __pyx_L1_error)
     __pyx_t_16 = __pyx_t_15;
     for (__pyx_t_17 = 0; __pyx_t_17 < __pyx_t_16; __pyx_t_17+=1) {
       __pyx_v_i = __pyx_t_17;
       __pyx_t_1 = PyList_GET_ITEM(__pyx_v_dest_sig, __pyx_v_i);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_dst_type, __pyx_t_1);
       __pyx_t_1 = 0;
       __pyx_t_3 = (__pyx_v_dst_type != Py_None);
       __pyx_t_2 = (__pyx_t_3 != 0);
       if (__pyx_t_2) {
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_src_sig, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_src_sig, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_13 = PyObject_RichCompare(__pyx_t_1, __pyx_v_dst_type, Py_EQ); __Pyx_XGOTREF(__pyx_t_13); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_13 = PyObject_RichCompare(__pyx_t_1, __pyx_v_dst_type, Py_EQ); __Pyx_XGOTREF(__pyx_t_13); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         if (__pyx_t_2) {
           __pyx_v_match_found = 1;
           goto __pyx_L98;
         }
         /*else*/ {
           __pyx_v_match_found = 0;
@@ -14565,43 +15442,43 @@
         }
         __pyx_L98:;
       }
     }
     __pyx_L96_break:;
     __pyx_t_2 = (__pyx_v_match_found != 0);
     if (__pyx_t_2) {
-      __pyx_t_18 = __Pyx_PyList_Append(__pyx_v_candidates, __pyx_v_sig); if (unlikely(__pyx_t_18 == ((int)-1))) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_18 = __Pyx_PyList_Append(__pyx_v_candidates, __pyx_v_sig); if (unlikely(__pyx_t_18 == ((int)-1))) __PYX_ERR(0, 400, __pyx_L1_error)
     }
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_2 = (PyList_GET_SIZE(__pyx_v_candidates) != 0);
   __pyx_t_3 = ((!__pyx_t_2) != 0);
   if (__pyx_t_3) {
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 387, __pyx_L1_error)
+    __PYX_ERR(0, 400, __pyx_L1_error)
   }
-  __pyx_t_9 = PyList_GET_SIZE(__pyx_v_candidates); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_9 = PyList_GET_SIZE(__pyx_v_candidates); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 400, __pyx_L1_error)
   __pyx_t_3 = ((__pyx_t_9 > 1) != 0);
   if (__pyx_t_3) {
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 387, __pyx_L1_error)
+    __PYX_ERR(0, 400, __pyx_L1_error)
   }
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     if (unlikely(((PyObject *)__pyx_v_signatures) == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 387, __pyx_L1_error)
+      __PYX_ERR(0, 400, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_signatures), PyList_GET_ITEM(__pyx_v_candidates, 0)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_signatures), PyList_GET_ITEM(__pyx_v_candidates, 0)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_r = __pyx_t_6;
     __pyx_t_6 = 0;
     goto __pyx_L0;
   }
 
   /* function exit code */
@@ -14658,21 +15535,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_0set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_0set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_37__pyx_fuse_0set_linear)) {
-        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint8_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint8_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint8_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint8_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
           if (likely(__pyx_t_6)) {
@@ -14682,49 +15559,49 @@
             __Pyx_DECREF_SET(__pyx_t_5, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         {
-          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           if (__pyx_t_6) {
             __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_4);
           PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_4);
           __pyx_t_3 = 0;
           __pyx_t_4 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -14743,21 +15620,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_27set_linear)) {
-        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint8_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint8_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint8_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint8_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_3 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_3)) {
@@ -14767,49 +15644,49 @@
             __Pyx_DECREF_SET(__pyx_t_4, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         {
-          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           if (__pyx_t_3) {
             __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3); __pyx_t_3 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_5);
           PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_7, __pyx_t_5);
           __Pyx_GIVEREF(__pyx_t_8);
           PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_7, __pyx_t_8);
           __pyx_t_5 = 0;
           __pyx_t_8 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -14820,42 +15697,42 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   __pyx_t_10.__pyx_n = 1;
   __pyx_t_10.v = __pyx_v_v;
-  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 404, __pyx_L1_error)
   __pyx_t_11 = (((__pyx_v_biases.shape[0]) != __pyx_t_9) != 0);
   if (unlikely(__pyx_t_11)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":393
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":406
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t c
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_10.__pyx_n = 1;
     __pyx_t_10.v = __pyx_v_v;
-    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 393, __pyx_L1_error)
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 406, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -14864,101 +15741,101 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (__pyx_t_8) {
         __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_8); __pyx_t_8 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_7, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_7, __pyx_t_6);
       __pyx_t_4 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":392
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":405
  * 
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'             # <<<<<<<<<<<<<<
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 392, __pyx_L1_error)
+    __PYX_ERR(0, 405, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":396
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":409
  * 
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):             # <<<<<<<<<<<<<<
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])
  * 
  */
   __pyx_t_9 = (__pyx_v_biases.shape[0]);
   __pyx_t_12 = __pyx_t_9;
   for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
     __pyx_v_c = __pyx_t_13;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":397
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":410
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
  */
     __pyx_t_14 = __pyx_v_c;
     try {
       __pyx_v_self->bqm_.set_linear(((__pyx_v_self->case_starts_[__pyx_v_v]) + __pyx_v_c), (*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_biases.data + __pyx_t_14 * __pyx_v_biases.strides[0]) ))));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 397, __pyx_L1_error)
+      __PYX_ERR(0, 410, __pyx_L1_error)
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":387
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":400
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t set_linear(self, VarIndex v, Numeric[:] biases) except -1:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
 
@@ -15011,32 +15888,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_biases)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0set_linear", 1, 2, 2, 1); __PYX_ERR(0, 387, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0set_linear", 1, 2, 2, 1); __PYX_ERR(0, 400, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_0set_linear") < 0)) __PYX_ERR(0, 387, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_0set_linear") < 0)) __PYX_ERR(0, 400, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L3_error)
-    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint8_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 387, __pyx_L3_error)
+    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L3_error)
+    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint8_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 400, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 387, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 400, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.__pyx_fuse_0set_linear", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_36__pyx_fuse_0set_linear(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self), __pyx_v_v, __pyx_v_biases);
 
@@ -15051,17 +15928,17 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_0set_linear", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_fuse_0__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 387, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_fuse_0__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -15104,21 +15981,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_1set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_1set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_39__pyx_fuse_1set_linear)) {
-        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint16_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint16_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint16_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint16_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
           if (likely(__pyx_t_6)) {
@@ -15128,49 +16005,49 @@
             __Pyx_DECREF_SET(__pyx_t_5, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         {
-          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           if (__pyx_t_6) {
             __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_4);
           PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_4);
           __pyx_t_3 = 0;
           __pyx_t_4 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -15189,21 +16066,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_27set_linear)) {
-        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint16_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint16_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint16_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint16_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_3 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_3)) {
@@ -15213,49 +16090,49 @@
             __Pyx_DECREF_SET(__pyx_t_4, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         {
-          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           if (__pyx_t_3) {
             __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3); __pyx_t_3 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_5);
           PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_7, __pyx_t_5);
           __Pyx_GIVEREF(__pyx_t_8);
           PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_7, __pyx_t_8);
           __pyx_t_5 = 0;
           __pyx_t_8 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -15266,42 +16143,42 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   __pyx_t_10.__pyx_n = 1;
   __pyx_t_10.v = __pyx_v_v;
-  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 404, __pyx_L1_error)
   __pyx_t_11 = (((__pyx_v_biases.shape[0]) != __pyx_t_9) != 0);
   if (unlikely(__pyx_t_11)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":393
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":406
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t c
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_10.__pyx_n = 1;
     __pyx_t_10.v = __pyx_v_v;
-    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 393, __pyx_L1_error)
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 406, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -15310,101 +16187,101 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (__pyx_t_8) {
         __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_8); __pyx_t_8 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_7, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_7, __pyx_t_6);
       __pyx_t_4 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":392
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":405
  * 
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'             # <<<<<<<<<<<<<<
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 392, __pyx_L1_error)
+    __PYX_ERR(0, 405, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":396
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":409
  * 
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):             # <<<<<<<<<<<<<<
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])
  * 
  */
   __pyx_t_9 = (__pyx_v_biases.shape[0]);
   __pyx_t_12 = __pyx_t_9;
   for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
     __pyx_v_c = __pyx_t_13;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":397
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":410
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
  */
     __pyx_t_14 = __pyx_v_c;
     try {
       __pyx_v_self->bqm_.set_linear(((__pyx_v_self->case_starts_[__pyx_v_v]) + __pyx_v_c), (*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_biases.data + __pyx_t_14 * __pyx_v_biases.strides[0]) ))));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 397, __pyx_L1_error)
+      __PYX_ERR(0, 410, __pyx_L1_error)
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":387
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":400
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t set_linear(self, VarIndex v, Numeric[:] biases) except -1:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
 
@@ -15457,32 +16334,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_biases)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1set_linear", 1, 2, 2, 1); __PYX_ERR(0, 387, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1set_linear", 1, 2, 2, 1); __PYX_ERR(0, 400, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_1set_linear") < 0)) __PYX_ERR(0, 387, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_1set_linear") < 0)) __PYX_ERR(0, 400, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L3_error)
-    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint16_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 387, __pyx_L3_error)
+    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L3_error)
+    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint16_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 400, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 387, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 400, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.__pyx_fuse_1set_linear", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_38__pyx_fuse_1set_linear(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self), __pyx_v_v, __pyx_v_biases);
 
@@ -15497,17 +16374,17 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_1set_linear", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_fuse_1__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 387, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_fuse_1__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -15550,21 +16427,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_2set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_2set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_41__pyx_fuse_2set_linear)) {
-        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint32_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint32_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
           if (likely(__pyx_t_6)) {
@@ -15574,49 +16451,49 @@
             __Pyx_DECREF_SET(__pyx_t_5, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         {
-          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           if (__pyx_t_6) {
             __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_4);
           PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_4);
           __pyx_t_3 = 0;
           __pyx_t_4 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -15635,21 +16512,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_27set_linear)) {
-        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint32_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint32_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_3 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_3)) {
@@ -15659,49 +16536,49 @@
             __Pyx_DECREF_SET(__pyx_t_4, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         {
-          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           if (__pyx_t_3) {
             __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3); __pyx_t_3 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_5);
           PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_7, __pyx_t_5);
           __Pyx_GIVEREF(__pyx_t_8);
           PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_7, __pyx_t_8);
           __pyx_t_5 = 0;
           __pyx_t_8 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -15712,42 +16589,42 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   __pyx_t_10.__pyx_n = 1;
   __pyx_t_10.v = __pyx_v_v;
-  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 404, __pyx_L1_error)
   __pyx_t_11 = (((__pyx_v_biases.shape[0]) != __pyx_t_9) != 0);
   if (unlikely(__pyx_t_11)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":393
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":406
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t c
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_10.__pyx_n = 1;
     __pyx_t_10.v = __pyx_v_v;
-    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 393, __pyx_L1_error)
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 406, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -15756,101 +16633,101 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (__pyx_t_8) {
         __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_8); __pyx_t_8 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_7, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_7, __pyx_t_6);
       __pyx_t_4 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":392
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":405
  * 
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'             # <<<<<<<<<<<<<<
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 392, __pyx_L1_error)
+    __PYX_ERR(0, 405, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":396
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":409
  * 
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):             # <<<<<<<<<<<<<<
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])
  * 
  */
   __pyx_t_9 = (__pyx_v_biases.shape[0]);
   __pyx_t_12 = __pyx_t_9;
   for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
     __pyx_v_c = __pyx_t_13;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":397
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":410
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
  */
     __pyx_t_14 = __pyx_v_c;
     try {
       __pyx_v_self->bqm_.set_linear(((__pyx_v_self->case_starts_[__pyx_v_v]) + __pyx_v_c), (*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_biases.data + __pyx_t_14 * __pyx_v_biases.strides[0]) ))));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 397, __pyx_L1_error)
+      __PYX_ERR(0, 410, __pyx_L1_error)
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":387
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":400
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t set_linear(self, VarIndex v, Numeric[:] biases) except -1:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
 
@@ -15903,32 +16780,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_biases)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2set_linear", 1, 2, 2, 1); __PYX_ERR(0, 387, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2set_linear", 1, 2, 2, 1); __PYX_ERR(0, 400, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_2set_linear") < 0)) __PYX_ERR(0, 387, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_2set_linear") < 0)) __PYX_ERR(0, 400, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L3_error)
-    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 387, __pyx_L3_error)
+    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L3_error)
+    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 400, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 387, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 400, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.__pyx_fuse_2set_linear", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_40__pyx_fuse_2set_linear(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self), __pyx_v_v, __pyx_v_biases);
 
@@ -15943,17 +16820,17 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_2set_linear", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_fuse_2__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 387, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_fuse_2__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -15996,21 +16873,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_3set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_3set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_43__pyx_fuse_3set_linear)) {
-        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint64_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint64_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
           if (likely(__pyx_t_6)) {
@@ -16020,49 +16897,49 @@
             __Pyx_DECREF_SET(__pyx_t_5, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         {
-          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           if (__pyx_t_6) {
             __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_4);
           PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_4);
           __pyx_t_3 = 0;
           __pyx_t_4 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -16081,21 +16958,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_27set_linear)) {
-        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint64_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint64_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_3 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_3)) {
@@ -16105,49 +16982,49 @@
             __Pyx_DECREF_SET(__pyx_t_4, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         {
-          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           if (__pyx_t_3) {
             __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3); __pyx_t_3 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_5);
           PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_7, __pyx_t_5);
           __Pyx_GIVEREF(__pyx_t_8);
           PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_7, __pyx_t_8);
           __pyx_t_5 = 0;
           __pyx_t_8 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -16158,42 +17035,42 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   __pyx_t_10.__pyx_n = 1;
   __pyx_t_10.v = __pyx_v_v;
-  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 404, __pyx_L1_error)
   __pyx_t_11 = (((__pyx_v_biases.shape[0]) != __pyx_t_9) != 0);
   if (unlikely(__pyx_t_11)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":393
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":406
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t c
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_10.__pyx_n = 1;
     __pyx_t_10.v = __pyx_v_v;
-    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 393, __pyx_L1_error)
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 406, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -16202,101 +17079,101 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (__pyx_t_8) {
         __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_8); __pyx_t_8 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_7, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_7, __pyx_t_6);
       __pyx_t_4 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":392
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":405
  * 
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'             # <<<<<<<<<<<<<<
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 392, __pyx_L1_error)
+    __PYX_ERR(0, 405, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":396
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":409
  * 
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):             # <<<<<<<<<<<<<<
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])
  * 
  */
   __pyx_t_9 = (__pyx_v_biases.shape[0]);
   __pyx_t_12 = __pyx_t_9;
   for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
     __pyx_v_c = __pyx_t_13;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":397
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":410
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
  */
     __pyx_t_14 = __pyx_v_c;
     try {
       __pyx_v_self->bqm_.set_linear(((__pyx_v_self->case_starts_[__pyx_v_v]) + __pyx_v_c), (*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_biases.data + __pyx_t_14 * __pyx_v_biases.strides[0]) ))));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 397, __pyx_L1_error)
+      __PYX_ERR(0, 410, __pyx_L1_error)
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":387
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":400
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t set_linear(self, VarIndex v, Numeric[:] biases) except -1:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
 
@@ -16349,32 +17226,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_biases)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3set_linear", 1, 2, 2, 1); __PYX_ERR(0, 387, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3set_linear", 1, 2, 2, 1); __PYX_ERR(0, 400, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_3set_linear") < 0)) __PYX_ERR(0, 387, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_3set_linear") < 0)) __PYX_ERR(0, 400, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L3_error)
-    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 387, __pyx_L3_error)
+    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L3_error)
+    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 400, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 387, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 400, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.__pyx_fuse_3set_linear", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_42__pyx_fuse_3set_linear(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self), __pyx_v_v, __pyx_v_biases);
 
@@ -16389,17 +17266,17 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_3set_linear", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_fuse_3__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 387, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_fuse_3__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -16442,21 +17319,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_4set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_4set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_45__pyx_fuse_4set_linear)) {
-        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int8_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_int8_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int8_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_int8_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
           if (likely(__pyx_t_6)) {
@@ -16466,49 +17343,49 @@
             __Pyx_DECREF_SET(__pyx_t_5, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         {
-          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           if (__pyx_t_6) {
             __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_4);
           PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_4);
           __pyx_t_3 = 0;
           __pyx_t_4 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -16527,21 +17404,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_27set_linear)) {
-        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int8_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_int8_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int8_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_int8_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_3 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_3)) {
@@ -16551,49 +17428,49 @@
             __Pyx_DECREF_SET(__pyx_t_4, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         {
-          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           if (__pyx_t_3) {
             __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3); __pyx_t_3 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_5);
           PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_7, __pyx_t_5);
           __Pyx_GIVEREF(__pyx_t_8);
           PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_7, __pyx_t_8);
           __pyx_t_5 = 0;
           __pyx_t_8 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -16604,42 +17481,42 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   __pyx_t_10.__pyx_n = 1;
   __pyx_t_10.v = __pyx_v_v;
-  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 404, __pyx_L1_error)
   __pyx_t_11 = (((__pyx_v_biases.shape[0]) != __pyx_t_9) != 0);
   if (unlikely(__pyx_t_11)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":393
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":406
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t c
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_10.__pyx_n = 1;
     __pyx_t_10.v = __pyx_v_v;
-    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 393, __pyx_L1_error)
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 406, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -16648,101 +17525,101 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (__pyx_t_8) {
         __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_8); __pyx_t_8 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_7, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_7, __pyx_t_6);
       __pyx_t_4 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":392
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":405
  * 
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'             # <<<<<<<<<<<<<<
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 392, __pyx_L1_error)
+    __PYX_ERR(0, 405, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":396
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":409
  * 
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):             # <<<<<<<<<<<<<<
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])
  * 
  */
   __pyx_t_9 = (__pyx_v_biases.shape[0]);
   __pyx_t_12 = __pyx_t_9;
   for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
     __pyx_v_c = __pyx_t_13;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":397
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":410
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
  */
     __pyx_t_14 = __pyx_v_c;
     try {
       __pyx_v_self->bqm_.set_linear(((__pyx_v_self->case_starts_[__pyx_v_v]) + __pyx_v_c), (*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ (__pyx_v_biases.data + __pyx_t_14 * __pyx_v_biases.strides[0]) ))));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 397, __pyx_L1_error)
+      __PYX_ERR(0, 410, __pyx_L1_error)
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":387
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":400
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t set_linear(self, VarIndex v, Numeric[:] biases) except -1:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
 
@@ -16795,32 +17672,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_biases)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_4set_linear", 1, 2, 2, 1); __PYX_ERR(0, 387, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_4set_linear", 1, 2, 2, 1); __PYX_ERR(0, 400, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_4set_linear") < 0)) __PYX_ERR(0, 387, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_4set_linear") < 0)) __PYX_ERR(0, 400, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L3_error)
-    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int8_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 387, __pyx_L3_error)
+    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L3_error)
+    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int8_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 400, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_4set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 387, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_4set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 400, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.__pyx_fuse_4set_linear", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_44__pyx_fuse_4set_linear(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self), __pyx_v_v, __pyx_v_biases);
 
@@ -16835,17 +17712,17 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_4set_linear", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_fuse_4__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 387, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_fuse_4__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -16888,21 +17765,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_5set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_5set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_47__pyx_fuse_5set_linear)) {
-        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int16_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_int16_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int16_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_int16_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
           if (likely(__pyx_t_6)) {
@@ -16912,49 +17789,49 @@
             __Pyx_DECREF_SET(__pyx_t_5, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         {
-          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           if (__pyx_t_6) {
             __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_4);
           PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_4);
           __pyx_t_3 = 0;
           __pyx_t_4 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -16973,21 +17850,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_27set_linear)) {
-        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int16_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_int16_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int16_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_int16_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_3 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_3)) {
@@ -16997,49 +17874,49 @@
             __Pyx_DECREF_SET(__pyx_t_4, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         {
-          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           if (__pyx_t_3) {
             __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3); __pyx_t_3 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_5);
           PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_7, __pyx_t_5);
           __Pyx_GIVEREF(__pyx_t_8);
           PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_7, __pyx_t_8);
           __pyx_t_5 = 0;
           __pyx_t_8 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -17050,42 +17927,42 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   __pyx_t_10.__pyx_n = 1;
   __pyx_t_10.v = __pyx_v_v;
-  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 404, __pyx_L1_error)
   __pyx_t_11 = (((__pyx_v_biases.shape[0]) != __pyx_t_9) != 0);
   if (unlikely(__pyx_t_11)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":393
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":406
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t c
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_10.__pyx_n = 1;
     __pyx_t_10.v = __pyx_v_v;
-    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 393, __pyx_L1_error)
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 406, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -17094,101 +17971,101 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (__pyx_t_8) {
         __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_8); __pyx_t_8 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_7, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_7, __pyx_t_6);
       __pyx_t_4 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":392
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":405
  * 
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'             # <<<<<<<<<<<<<<
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 392, __pyx_L1_error)
+    __PYX_ERR(0, 405, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":396
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":409
  * 
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):             # <<<<<<<<<<<<<<
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])
  * 
  */
   __pyx_t_9 = (__pyx_v_biases.shape[0]);
   __pyx_t_12 = __pyx_t_9;
   for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
     __pyx_v_c = __pyx_t_13;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":397
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":410
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
  */
     __pyx_t_14 = __pyx_v_c;
     try {
       __pyx_v_self->bqm_.set_linear(((__pyx_v_self->case_starts_[__pyx_v_v]) + __pyx_v_c), (*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ (__pyx_v_biases.data + __pyx_t_14 * __pyx_v_biases.strides[0]) ))));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 397, __pyx_L1_error)
+      __PYX_ERR(0, 410, __pyx_L1_error)
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":387
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":400
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t set_linear(self, VarIndex v, Numeric[:] biases) except -1:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
 
@@ -17241,32 +18118,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_biases)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_5set_linear", 1, 2, 2, 1); __PYX_ERR(0, 387, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_5set_linear", 1, 2, 2, 1); __PYX_ERR(0, 400, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_5set_linear") < 0)) __PYX_ERR(0, 387, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_5set_linear") < 0)) __PYX_ERR(0, 400, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L3_error)
-    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int16_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 387, __pyx_L3_error)
+    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L3_error)
+    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int16_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 400, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_5set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 387, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_5set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 400, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.__pyx_fuse_5set_linear", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_46__pyx_fuse_5set_linear(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self), __pyx_v_v, __pyx_v_biases);
 
@@ -17281,17 +18158,17 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_5set_linear", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_fuse_5__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 387, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_fuse_5__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -17334,21 +18211,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_6set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_6set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_49__pyx_fuse_6set_linear)) {
-        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_int32_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_int32_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
           if (likely(__pyx_t_6)) {
@@ -17358,49 +18235,49 @@
             __Pyx_DECREF_SET(__pyx_t_5, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         {
-          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           if (__pyx_t_6) {
             __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_4);
           PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_4);
           __pyx_t_3 = 0;
           __pyx_t_4 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -17419,21 +18296,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_27set_linear)) {
-        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_int32_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_int32_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_3 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_3)) {
@@ -17443,49 +18320,49 @@
             __Pyx_DECREF_SET(__pyx_t_4, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         {
-          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           if (__pyx_t_3) {
             __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3); __pyx_t_3 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_5);
           PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_7, __pyx_t_5);
           __Pyx_GIVEREF(__pyx_t_8);
           PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_7, __pyx_t_8);
           __pyx_t_5 = 0;
           __pyx_t_8 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -17496,42 +18373,42 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   __pyx_t_10.__pyx_n = 1;
   __pyx_t_10.v = __pyx_v_v;
-  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 404, __pyx_L1_error)
   __pyx_t_11 = (((__pyx_v_biases.shape[0]) != __pyx_t_9) != 0);
   if (unlikely(__pyx_t_11)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":393
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":406
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t c
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_10.__pyx_n = 1;
     __pyx_t_10.v = __pyx_v_v;
-    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 393, __pyx_L1_error)
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 406, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -17540,101 +18417,101 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (__pyx_t_8) {
         __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_8); __pyx_t_8 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_7, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_7, __pyx_t_6);
       __pyx_t_4 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":392
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":405
  * 
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'             # <<<<<<<<<<<<<<
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 392, __pyx_L1_error)
+    __PYX_ERR(0, 405, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":396
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":409
  * 
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):             # <<<<<<<<<<<<<<
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])
  * 
  */
   __pyx_t_9 = (__pyx_v_biases.shape[0]);
   __pyx_t_12 = __pyx_t_9;
   for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
     __pyx_v_c = __pyx_t_13;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":397
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":410
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
  */
     __pyx_t_14 = __pyx_v_c;
     try {
       __pyx_v_self->bqm_.set_linear(((__pyx_v_self->case_starts_[__pyx_v_v]) + __pyx_v_c), (*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ (__pyx_v_biases.data + __pyx_t_14 * __pyx_v_biases.strides[0]) ))));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 397, __pyx_L1_error)
+      __PYX_ERR(0, 410, __pyx_L1_error)
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":387
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":400
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t set_linear(self, VarIndex v, Numeric[:] biases) except -1:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
 
@@ -17687,32 +18564,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_biases)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_6set_linear", 1, 2, 2, 1); __PYX_ERR(0, 387, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_6set_linear", 1, 2, 2, 1); __PYX_ERR(0, 400, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_6set_linear") < 0)) __PYX_ERR(0, 387, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_6set_linear") < 0)) __PYX_ERR(0, 400, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L3_error)
-    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int32_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 387, __pyx_L3_error)
+    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L3_error)
+    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int32_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 400, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_6set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 387, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_6set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 400, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.__pyx_fuse_6set_linear", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_48__pyx_fuse_6set_linear(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self), __pyx_v_v, __pyx_v_biases);
 
@@ -17727,17 +18604,17 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_6set_linear", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_fuse_6__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 387, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_fuse_6__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -17780,21 +18657,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_7set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_7set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_51__pyx_fuse_7set_linear)) {
-        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_int64_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_int64_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
           if (likely(__pyx_t_6)) {
@@ -17804,49 +18681,49 @@
             __Pyx_DECREF_SET(__pyx_t_5, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         {
-          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           if (__pyx_t_6) {
             __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_4);
           PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_4);
           __pyx_t_3 = 0;
           __pyx_t_4 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -17865,21 +18742,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_27set_linear)) {
-        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_int64_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_int64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_int64_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_3 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_3)) {
@@ -17889,49 +18766,49 @@
             __Pyx_DECREF_SET(__pyx_t_4, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         {
-          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           if (__pyx_t_3) {
             __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3); __pyx_t_3 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_5);
           PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_7, __pyx_t_5);
           __Pyx_GIVEREF(__pyx_t_8);
           PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_7, __pyx_t_8);
           __pyx_t_5 = 0;
           __pyx_t_8 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -17942,42 +18819,42 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   __pyx_t_10.__pyx_n = 1;
   __pyx_t_10.v = __pyx_v_v;
-  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 404, __pyx_L1_error)
   __pyx_t_11 = (((__pyx_v_biases.shape[0]) != __pyx_t_9) != 0);
   if (unlikely(__pyx_t_11)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":393
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":406
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t c
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_10.__pyx_n = 1;
     __pyx_t_10.v = __pyx_v_v;
-    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 393, __pyx_L1_error)
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 406, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -17986,101 +18863,101 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (__pyx_t_8) {
         __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_8); __pyx_t_8 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_7, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_7, __pyx_t_6);
       __pyx_t_4 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":392
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":405
  * 
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'             # <<<<<<<<<<<<<<
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 392, __pyx_L1_error)
+    __PYX_ERR(0, 405, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":396
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":409
  * 
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):             # <<<<<<<<<<<<<<
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])
  * 
  */
   __pyx_t_9 = (__pyx_v_biases.shape[0]);
   __pyx_t_12 = __pyx_t_9;
   for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
     __pyx_v_c = __pyx_t_13;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":397
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":410
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
  */
     __pyx_t_14 = __pyx_v_c;
     try {
       __pyx_v_self->bqm_.set_linear(((__pyx_v_self->case_starts_[__pyx_v_v]) + __pyx_v_c), (*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_biases.data + __pyx_t_14 * __pyx_v_biases.strides[0]) ))));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 397, __pyx_L1_error)
+      __PYX_ERR(0, 410, __pyx_L1_error)
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":387
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":400
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t set_linear(self, VarIndex v, Numeric[:] biases) except -1:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
 
@@ -18133,32 +19010,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_biases)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_7set_linear", 1, 2, 2, 1); __PYX_ERR(0, 387, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_7set_linear", 1, 2, 2, 1); __PYX_ERR(0, 400, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_7set_linear") < 0)) __PYX_ERR(0, 387, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_7set_linear") < 0)) __PYX_ERR(0, 400, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L3_error)
-    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int64_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 387, __pyx_L3_error)
+    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L3_error)
+    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int64_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 400, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_7set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 387, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_7set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 400, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.__pyx_fuse_7set_linear", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_50__pyx_fuse_7set_linear(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self), __pyx_v_v, __pyx_v_biases);
 
@@ -18173,17 +19050,17 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_7set_linear", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_fuse_7__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 387, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_fuse_7__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -18226,21 +19103,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_8set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_8set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_53__pyx_fuse_8set_linear)) {
-        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_float32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_float32_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_float32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_float32_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
           if (likely(__pyx_t_6)) {
@@ -18250,49 +19127,49 @@
             __Pyx_DECREF_SET(__pyx_t_5, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         {
-          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           if (__pyx_t_6) {
             __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_4);
           PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_4);
           __pyx_t_3 = 0;
           __pyx_t_4 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -18311,21 +19188,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_27set_linear)) {
-        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_float32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_float32_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_float32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_float32_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_3 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_3)) {
@@ -18335,49 +19212,49 @@
             __Pyx_DECREF_SET(__pyx_t_4, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         {
-          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           if (__pyx_t_3) {
             __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3); __pyx_t_3 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_5);
           PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_7, __pyx_t_5);
           __Pyx_GIVEREF(__pyx_t_8);
           PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_7, __pyx_t_8);
           __pyx_t_5 = 0;
           __pyx_t_8 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -18388,42 +19265,42 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   __pyx_t_10.__pyx_n = 1;
   __pyx_t_10.v = __pyx_v_v;
-  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 404, __pyx_L1_error)
   __pyx_t_11 = (((__pyx_v_biases.shape[0]) != __pyx_t_9) != 0);
   if (unlikely(__pyx_t_11)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":393
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":406
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t c
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_10.__pyx_n = 1;
     __pyx_t_10.v = __pyx_v_v;
-    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 393, __pyx_L1_error)
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 406, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -18432,101 +19309,101 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (__pyx_t_8) {
         __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_8); __pyx_t_8 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_7, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_7, __pyx_t_6);
       __pyx_t_4 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":392
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":405
  * 
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'             # <<<<<<<<<<<<<<
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 392, __pyx_L1_error)
+    __PYX_ERR(0, 405, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":396
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":409
  * 
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):             # <<<<<<<<<<<<<<
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])
  * 
  */
   __pyx_t_9 = (__pyx_v_biases.shape[0]);
   __pyx_t_12 = __pyx_t_9;
   for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
     __pyx_v_c = __pyx_t_13;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":397
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":410
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
  */
     __pyx_t_14 = __pyx_v_c;
     try {
       __pyx_v_self->bqm_.set_linear(((__pyx_v_self->case_starts_[__pyx_v_v]) + __pyx_v_c), (*((__pyx_t_5numpy_float32_t *) ( /* dim=0 */ (__pyx_v_biases.data + __pyx_t_14 * __pyx_v_biases.strides[0]) ))));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 397, __pyx_L1_error)
+      __PYX_ERR(0, 410, __pyx_L1_error)
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":387
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":400
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t set_linear(self, VarIndex v, Numeric[:] biases) except -1:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
 
@@ -18579,32 +19456,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_biases)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_8set_linear", 1, 2, 2, 1); __PYX_ERR(0, 387, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_8set_linear", 1, 2, 2, 1); __PYX_ERR(0, 400, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_8set_linear") < 0)) __PYX_ERR(0, 387, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_8set_linear") < 0)) __PYX_ERR(0, 400, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L3_error)
-    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float32_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 387, __pyx_L3_error)
+    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L3_error)
+    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float32_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 400, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_8set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 387, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_8set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 400, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.__pyx_fuse_8set_linear", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_52__pyx_fuse_8set_linear(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self), __pyx_v_v, __pyx_v_biases);
 
@@ -18619,17 +19496,17 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_8set_linear", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_fuse_8__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 387, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_fuse_8__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -18672,21 +19549,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_9set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pyx_fuse_9set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_55__pyx_fuse_9set_linear)) {
-        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_float64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_float64_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_float64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_float64_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
           if (likely(__pyx_t_6)) {
@@ -18696,49 +19573,49 @@
             __Pyx_DECREF_SET(__pyx_t_5, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         {
-          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           if (__pyx_t_6) {
             __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_4);
           PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_4);
           __pyx_t_3 = 0;
           __pyx_t_4 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -18757,21 +19634,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_27set_linear)) {
-        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_float64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_float64_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+        if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+        __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_biases, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_float64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_float64_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_3 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_3)) {
@@ -18781,49 +19658,49 @@
             __Pyx_DECREF_SET(__pyx_t_4, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_8};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         {
-          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           if (__pyx_t_3) {
             __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3); __pyx_t_3 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_5);
           PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_7, __pyx_t_5);
           __Pyx_GIVEREF(__pyx_t_8);
           PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_7, __pyx_t_8);
           __pyx_t_5 = 0;
           __pyx_t_8 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_9;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -18834,42 +19711,42 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   __pyx_t_10.__pyx_n = 1;
   __pyx_t_10.v = __pyx_v_v;
-  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 404, __pyx_L1_error)
   __pyx_t_11 = (((__pyx_v_biases.shape[0]) != __pyx_t_9) != 0);
   if (unlikely(__pyx_t_11)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":393
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":406
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t c
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Recieved_bias_es_for_a_variable, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_biases.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_10.__pyx_n = 1;
     __pyx_t_10.v = __pyx_v_v;
-    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 393, __pyx_L1_error)
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_9 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_10); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 406, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -18878,101 +19755,101 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (__pyx_t_8) {
         __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_8); __pyx_t_8 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_7, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_7, __pyx_t_6);
       __pyx_t_4 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":392
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":405
  * 
  *         if biases.shape[0] != self.num_cases(v):
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'             # <<<<<<<<<<<<<<
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 392, __pyx_L1_error)
+    __PYX_ERR(0, 405, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":391
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":404
  *         # self.num_cases checks that the variable is valid
  * 
  *         if biases.shape[0] != self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError('Recieved {} bias(es) for a variable of degree {}'
  *                              ''.format(biases.shape[0], self.num_cases(v)))
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":396
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":409
  * 
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):             # <<<<<<<<<<<<<<
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])
  * 
  */
   __pyx_t_9 = (__pyx_v_biases.shape[0]);
   __pyx_t_12 = __pyx_t_9;
   for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
     __pyx_v_c = __pyx_t_13;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":397
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":410
  *         cdef Py_ssize_t c
  *         for c in range(biases.shape[0]):
  *             self.bqm_.set_linear(self.case_starts_[v] + c, biases[c])             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
  */
     __pyx_t_14 = __pyx_v_c;
     try {
       __pyx_v_self->bqm_.set_linear(((__pyx_v_self->case_starts_[__pyx_v_v]) + __pyx_v_c), (*((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_biases.data + __pyx_t_14 * __pyx_v_biases.strides[0]) ))));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 397, __pyx_L1_error)
+      __PYX_ERR(0, 410, __pyx_L1_error)
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":387
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":400
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t set_linear(self, VarIndex v, Numeric[:] biases) except -1:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
 
@@ -19025,32 +19902,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_biases)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_9set_linear", 1, 2, 2, 1); __PYX_ERR(0, 387, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_9set_linear", 1, 2, 2, 1); __PYX_ERR(0, 400, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_9set_linear") < 0)) __PYX_ERR(0, 387, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_9set_linear") < 0)) __PYX_ERR(0, 400, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L3_error)
-    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 387, __pyx_L3_error)
+    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L3_error)
+    __pyx_v_biases = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_biases.memview)) __PYX_ERR(0, 400, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_9set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 387, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_9set_linear", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 400, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.__pyx_fuse_9set_linear", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_54__pyx_fuse_9set_linear(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self), __pyx_v_v, __pyx_v_biases);
 
@@ -19065,17 +19942,17 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_9set_linear", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 387, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_fuse_9__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 387, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (unlikely(!__pyx_v_biases.memview)) { __Pyx_RaiseUnboundLocalError("biases"); __PYX_ERR(0, 400, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_fuse_9__pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear(__pyx_v_self, __pyx_v_v, __pyx_v_biases, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -19085,15 +19962,15 @@
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_biases, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dimod/discrete/cydiscrete_quadratic_model.pyx":401
+/* "dimod/discrete/cydiscrete_quadratic_model.pyx":414
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t set_linear_case(self, VarIndex v, CaseIndex case, Bias b) except -1:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
 
@@ -19122,22 +19999,22 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear_case); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_linear_case); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 414, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_29set_linear_case)) {
-        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 401, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 414, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyInt_From_npy_int64(__pyx_v_case); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 401, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_npy_int64(__pyx_v_case); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 414, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_5 = PyFloat_FromDouble(__pyx_v_b); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 401, __pyx_L1_error)
+        __pyx_t_5 = PyFloat_FromDouble(__pyx_v_b); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 414, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_6 = __pyx_t_1; __pyx_t_7 = NULL;
         __pyx_t_8 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
           __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
           if (likely(__pyx_t_7)) {
@@ -19147,54 +20024,54 @@
             __Pyx_DECREF_SET(__pyx_t_6, function);
             __pyx_t_8 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_6)) {
           PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_3, __pyx_t_4, __pyx_t_5};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 401, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 414, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
           PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_3, __pyx_t_4, __pyx_t_5};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 401, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 414, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         } else
         #endif
         {
-          __pyx_t_9 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 401, __pyx_L1_error)
+          __pyx_t_9 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 414, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           if (__pyx_t_7) {
             __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_4);
           PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_t_4);
           __Pyx_GIVEREF(__pyx_t_5);
           PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_8, __pyx_t_5);
           __pyx_t_3 = 0;
           __pyx_t_4 = 0;
           __pyx_t_5 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_9, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 401, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_9, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 414, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         }
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 401, __pyx_L1_error)
+        __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 414, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_10;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -19205,74 +20082,74 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":405
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":418
  *         # self.num_cases checks that the variable is valid
  * 
  *         if case < 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("case should be a positive integer")
  *         if case >= self.num_cases(v):
  */
   __pyx_t_11 = ((__pyx_v_case < 0) != 0);
   if (unlikely(__pyx_t_11)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":406
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":419
  * 
  *         if case < 0:
  *             raise ValueError("case should be a positive integer")             # <<<<<<<<<<<<<<
  *         if case >= self.num_cases(v):
  *             raise ValueError("case {} is invalid, variable only supports {} "
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 406, __pyx_L1_error)
+    __PYX_ERR(0, 419, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":405
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":418
  *         # self.num_cases checks that the variable is valid
  * 
  *         if case < 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("case should be a positive integer")
  *         if case >= self.num_cases(v):
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":407
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":420
  *         if case < 0:
  *             raise ValueError("case should be a positive integer")
  *         if case >= self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case, self.num_cases(v)))
  */
   __pyx_t_12.__pyx_n = 1;
   __pyx_t_12.v = __pyx_v_v;
-  __pyx_t_10 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_12); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_10 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_12); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 420, __pyx_L1_error)
   __pyx_t_11 = ((__pyx_v_case >= __pyx_t_10) != 0);
   if (unlikely(__pyx_t_11)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":409
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":422
  *         if case >= self.num_cases(v):
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case, self.num_cases(v)))             # <<<<<<<<<<<<<<
  * 
  *         self.bqm_.set_linear(self.case_starts_[v] + case, b)
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_case_is_invalid_variable_only_su, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 409, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_case_is_invalid_variable_only_su, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyInt_From_npy_int64(__pyx_v_case); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 409, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_npy_int64(__pyx_v_case); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_12.__pyx_n = 1;
     __pyx_t_12.v = __pyx_v_v;
-    __pyx_t_10 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_12); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 409, __pyx_L1_error)
-    __pyx_t_9 = PyInt_FromSsize_t(__pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 409, __pyx_L1_error)
+    __pyx_t_10 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_12); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 422, __pyx_L1_error)
+    __pyx_t_9 = PyInt_FromSsize_t(__pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_5 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -19281,87 +20158,87 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_8 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_6, __pyx_t_9};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 409, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 422, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_6, __pyx_t_9};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 409, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 422, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     } else
     #endif
     {
-      __pyx_t_4 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 409, __pyx_L1_error)
+      __pyx_t_4 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 422, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_8, __pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_9);
       PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_8, __pyx_t_9);
       __pyx_t_6 = 0;
       __pyx_t_9 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 409, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 422, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":408
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":421
  *             raise ValueError("case should be a positive integer")
  *         if case >= self.num_cases(v):
  *             raise ValueError("case {} is invalid, variable only supports {} "             # <<<<<<<<<<<<<<
  *                              "cases".format(case, self.num_cases(v)))
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 421, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 408, __pyx_L1_error)
+    __PYX_ERR(0, 421, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":407
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":420
  *         if case < 0:
  *             raise ValueError("case should be a positive integer")
  *         if case >= self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case, self.num_cases(v)))
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":411
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":424
  *                              "cases".format(case, self.num_cases(v)))
  * 
  *         self.bqm_.set_linear(self.case_starts_[v] + case, b)             # <<<<<<<<<<<<<<
  * 
  *     def set_quadratic(self, VarIndex u, VarIndex v, biases):
  */
   try {
     __pyx_v_self->bqm_.set_linear(((__pyx_v_self->case_starts_[__pyx_v_v]) + __pyx_v_case), __pyx_v_b);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 411, __pyx_L1_error)
+    __PYX_ERR(0, 424, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":401
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":414
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t set_linear_case(self, VarIndex v, CaseIndex case, Bias b) except -1:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
 
@@ -19417,40 +20294,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_case)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("set_linear_case", 1, 3, 3, 1); __PYX_ERR(0, 401, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("set_linear_case", 1, 3, 3, 1); __PYX_ERR(0, 414, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("set_linear_case", 1, 3, 3, 2); __PYX_ERR(0, 401, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("set_linear_case", 1, 3, 3, 2); __PYX_ERR(0, 414, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_linear_case") < 0)) __PYX_ERR(0, 401, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_linear_case") < 0)) __PYX_ERR(0, 414, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 401, __pyx_L3_error)
-    __pyx_v_case = __Pyx_PyInt_As_npy_int64(values[1]); if (unlikely((__pyx_v_case == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 401, __pyx_L3_error)
-    __pyx_v_b = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_b == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 401, __pyx_L3_error)
+    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 414, __pyx_L3_error)
+    __pyx_v_case = __Pyx_PyInt_As_npy_int64(values[1]); if (unlikely((__pyx_v_case == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 414, __pyx_L3_error)
+    __pyx_v_b = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_b == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 414, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("set_linear_case", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 401, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("set_linear_case", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 414, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.set_linear_case", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_28set_linear_case(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self), __pyx_v_v, __pyx_v_case, __pyx_v_b);
 
@@ -19465,16 +20342,16 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_linear_case", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear_case(__pyx_v_self, __pyx_v_v, __pyx_v_case, __pyx_v_b, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 401, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 401, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_linear_case(__pyx_v_self, __pyx_v_v, __pyx_v_case, __pyx_v_b, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 414, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -19483,15 +20360,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dimod/discrete/cydiscrete_quadratic_model.pyx":413
+/* "dimod/discrete/cydiscrete_quadratic_model.pyx":426
  *         self.bqm_.set_linear(self.case_starts_[v] + case, b)
  * 
  *     def set_quadratic(self, VarIndex u, VarIndex v, biases):             # <<<<<<<<<<<<<<
  * 
  *         # check that the interaction does in fact exist
  */
 
@@ -19528,40 +20405,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_u)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("set_quadratic", 1, 3, 3, 1); __PYX_ERR(0, 413, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("set_quadratic", 1, 3, 3, 1); __PYX_ERR(0, 426, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_biases)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("set_quadratic", 1, 3, 3, 2); __PYX_ERR(0, 413, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("set_quadratic", 1, 3, 3, 2); __PYX_ERR(0, 426, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_quadratic") < 0)) __PYX_ERR(0, 413, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_quadratic") < 0)) __PYX_ERR(0, 426, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_u = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_u == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 413, __pyx_L3_error)
-    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[1]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 413, __pyx_L3_error)
+    __pyx_v_u = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_u == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 426, __pyx_L3_error)
+    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[1]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 426, __pyx_L3_error)
     __pyx_v_biases = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("set_quadratic", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 413, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("set_quadratic", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 426, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.set_quadratic", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_30set_quadratic(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self), __pyx_v_u, __pyx_v_v, __pyx_v_biases);
 
@@ -19606,15 +20483,15 @@
   __pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex __pyx_t_22;
   __pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex __pyx_t_23;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_quadratic", 0);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":416
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":429
  * 
  *         # check that the interaction does in fact exist
  *         if u < 0 or u >= self.adj_.size():             # <<<<<<<<<<<<<<
  *             raise ValueError("unknown variable")
  *         if v < 0 or v >= self.adj_.size():
  */
   __pyx_t_2 = ((__pyx_v_u < 0) != 0);
@@ -19624,37 +20501,37 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = ((__pyx_v_u >= __pyx_v_self->adj_.size()) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":417
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":430
  *         # check that the interaction does in fact exist
  *         if u < 0 or u >= self.adj_.size():
  *             raise ValueError("unknown variable")             # <<<<<<<<<<<<<<
  *         if v < 0 or v >= self.adj_.size():
  *             raise ValueError("unknown variable")
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 430, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 417, __pyx_L1_error)
+    __PYX_ERR(0, 430, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":416
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":429
  * 
  *         # check that the interaction does in fact exist
  *         if u < 0 or u >= self.adj_.size():             # <<<<<<<<<<<<<<
  *             raise ValueError("unknown variable")
  *         if v < 0 or v >= self.adj_.size():
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":418
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":431
  *         if u < 0 or u >= self.adj_.size():
  *             raise ValueError("unknown variable")
  *         if v < 0 or v >= self.adj_.size():             # <<<<<<<<<<<<<<
  *             raise ValueError("unknown variable")
  * 
  */
   __pyx_t_2 = ((__pyx_v_v < 0) != 0);
@@ -19664,157 +20541,157 @@
     goto __pyx_L7_bool_binop_done;
   }
   __pyx_t_2 = ((__pyx_v_v >= __pyx_v_self->adj_.size()) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L7_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":419
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":432
  *             raise ValueError("unknown variable")
  *         if v < 0 or v >= self.adj_.size():
  *             raise ValueError("unknown variable")             # <<<<<<<<<<<<<<
  * 
  *         cdef CaseIndex case_u, case_v
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 432, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 419, __pyx_L1_error)
+    __PYX_ERR(0, 432, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":418
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":431
  *         if u < 0 or u >= self.adj_.size():
  *             raise ValueError("unknown variable")
  *         if v < 0 or v >= self.adj_.size():             # <<<<<<<<<<<<<<
  *             raise ValueError("unknown variable")
  * 
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":425
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":438
  *         cdef Bias bias
  * 
  *         cdef Py_ssize_t num_cases_u = self.num_cases(u)             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t num_cases_v = self.num_cases(v)
  * 
  */
   __pyx_t_5.__pyx_n = 1;
   __pyx_t_5.v = __pyx_v_u;
-  __pyx_t_4 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_5); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 425, __pyx_L1_error)
+  __pyx_t_4 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_5); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 438, __pyx_L1_error)
   __pyx_v_num_cases_u = __pyx_t_4;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":426
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":439
  * 
  *         cdef Py_ssize_t num_cases_u = self.num_cases(u)
  *         cdef Py_ssize_t num_cases_v = self.num_cases(v)             # <<<<<<<<<<<<<<
  * 
  *         cdef Bias[:, :] biases_view
  */
   __pyx_t_5.__pyx_n = 1;
   __pyx_t_5.v = __pyx_v_v;
-  __pyx_t_4 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_5); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 426, __pyx_L1_error)
+  __pyx_t_4 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_5); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 439, __pyx_L1_error)
   __pyx_v_num_cases_v = __pyx_t_4;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":430
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":443
  *         cdef Bias[:, :] biases_view
  * 
  *         if isinstance(biases, abc.Mapping):             # <<<<<<<<<<<<<<
  *             for (case_u, case_v), bias in biases.items():
  *                 if case_u < 0 or case_u >= num_cases_u:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_abc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 430, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_abc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 443, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mapping); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 430, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mapping); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 443, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_1 = PyObject_IsInstance(__pyx_v_biases, __pyx_t_6); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 430, __pyx_L1_error)
+  __pyx_t_1 = PyObject_IsInstance(__pyx_v_biases, __pyx_t_6); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 443, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":431
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":444
  * 
  *         if isinstance(biases, abc.Mapping):
  *             for (case_u, case_v), bias in biases.items():             # <<<<<<<<<<<<<<
  *                 if case_u < 0 or case_u >= num_cases_u:
  *                     raise ValueError("case {} is invalid, variable only supports {} "
  */
     __pyx_t_4 = 0;
     if (unlikely(__pyx_v_biases == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-      __PYX_ERR(0, 431, __pyx_L1_error)
+      __PYX_ERR(0, 444, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_dict_iterator(__pyx_v_biases, 0, __pyx_n_s_items, (&__pyx_t_7), (&__pyx_t_8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 431, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_dict_iterator(__pyx_v_biases, 0, __pyx_n_s_items, (&__pyx_t_7), (&__pyx_t_8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 444, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_6);
     __pyx_t_6 = __pyx_t_3;
     __pyx_t_3 = 0;
     while (1) {
       __pyx_t_10 = __Pyx_dict_iter_next(__pyx_t_6, __pyx_t_7, &__pyx_t_4, &__pyx_t_3, &__pyx_t_9, NULL, __pyx_t_8);
       if (unlikely(__pyx_t_10 == 0)) break;
-      if (unlikely(__pyx_t_10 == -1)) __PYX_ERR(0, 431, __pyx_L1_error)
+      if (unlikely(__pyx_t_10 == -1)) __PYX_ERR(0, 444, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_11 = __pyx_PyFloat_AsDouble(__pyx_t_9); if (unlikely((__pyx_t_11 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 431, __pyx_L1_error)
+      __pyx_t_11 = __pyx_PyFloat_AsDouble(__pyx_t_9); if (unlikely((__pyx_t_11 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 444, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
         PyObject* sequence = __pyx_t_3;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 2)) {
           if (size > 2) __Pyx_RaiseTooManyValuesError(2);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 431, __pyx_L1_error)
+          __PYX_ERR(0, 444, __pyx_L1_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_12 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_13 = PyTuple_GET_ITEM(sequence, 1); 
         } else {
           __pyx_t_12 = PyList_GET_ITEM(sequence, 0); 
           __pyx_t_13 = PyList_GET_ITEM(sequence, 1); 
         }
         __Pyx_INCREF(__pyx_t_12);
         __Pyx_INCREF(__pyx_t_13);
         #else
-        __pyx_t_12 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 431, __pyx_L1_error)
+        __pyx_t_12 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 444, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_13 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 431, __pyx_L1_error)
+        __pyx_t_13 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 444, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_13);
         #endif
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_14 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 431, __pyx_L1_error)
+        __pyx_t_14 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 444, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_14);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_t_15 = Py_TYPE(__pyx_t_14)->tp_iternext;
         index = 0; __pyx_t_12 = __pyx_t_15(__pyx_t_14); if (unlikely(!__pyx_t_12)) goto __pyx_L12_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_12);
         index = 1; __pyx_t_13 = __pyx_t_15(__pyx_t_14); if (unlikely(!__pyx_t_13)) goto __pyx_L12_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_13);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_15(__pyx_t_14), 2) < 0) __PYX_ERR(0, 431, __pyx_L1_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_15(__pyx_t_14), 2) < 0) __PYX_ERR(0, 444, __pyx_L1_error)
         __pyx_t_15 = NULL;
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         goto __pyx_L13_unpacking_done;
         __pyx_L12_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __pyx_t_15 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 431, __pyx_L1_error)
+        __PYX_ERR(0, 444, __pyx_L1_error)
         __pyx_L13_unpacking_done:;
       }
-      __pyx_t_16 = __Pyx_PyInt_As_npy_int64(__pyx_t_12); if (unlikely((__pyx_t_16 == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 431, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyInt_As_npy_int64(__pyx_t_12); if (unlikely((__pyx_t_16 == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 444, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-      __pyx_t_17 = __Pyx_PyInt_As_npy_int64(__pyx_t_13); if (unlikely((__pyx_t_17 == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 431, __pyx_L1_error)
+      __pyx_t_17 = __Pyx_PyInt_As_npy_int64(__pyx_t_13); if (unlikely((__pyx_t_17 == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 444, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       __pyx_v_case_u = __pyx_t_16;
       __pyx_v_case_v = __pyx_t_17;
       __pyx_v_bias = __pyx_t_11;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":432
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":445
  *         if isinstance(biases, abc.Mapping):
  *             for (case_u, case_v), bias in biases.items():
  *                 if case_u < 0 or case_u >= num_cases_u:             # <<<<<<<<<<<<<<
  *                     raise ValueError("case {} is invalid, variable only supports {} "
  *                                      "cases".format(case_u, self.num_cases(u)))
  */
       __pyx_t_1 = ((__pyx_v_case_u < 0) != 0);
@@ -19824,29 +20701,29 @@
         goto __pyx_L15_bool_binop_done;
       }
       __pyx_t_1 = ((__pyx_v_case_u >= __pyx_v_num_cases_u) != 0);
       __pyx_t_2 = __pyx_t_1;
       __pyx_L15_bool_binop_done:;
       if (unlikely(__pyx_t_2)) {
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":434
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":447
  *                 if case_u < 0 or case_u >= num_cases_u:
  *                     raise ValueError("case {} is invalid, variable only supports {} "
  *                                      "cases".format(case_u, self.num_cases(u)))             # <<<<<<<<<<<<<<
  * 
  *                 if case_v < 0 or case_v >= num_cases_v:
  */
-        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_case_is_invalid_variable_only_su, __pyx_n_s_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 434, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_case_is_invalid_variable_only_su, __pyx_n_s_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_13 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_u); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 434, __pyx_L1_error)
+        __pyx_t_13 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_u); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 447, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_13);
         __pyx_t_5.__pyx_n = 1;
         __pyx_t_5.v = __pyx_v_u;
-        __pyx_t_18 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_5); if (unlikely(__pyx_t_18 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 434, __pyx_L1_error)
-        __pyx_t_12 = PyInt_FromSsize_t(__pyx_t_18); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 434, __pyx_L1_error)
+        __pyx_t_18 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_5); if (unlikely(__pyx_t_18 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 447, __pyx_L1_error)
+        __pyx_t_12 = PyInt_FromSsize_t(__pyx_t_18); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 447, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         __pyx_t_14 = NULL;
         __pyx_t_10 = 0;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_14)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -19855,73 +20732,73 @@
             __Pyx_DECREF_SET(__pyx_t_3, function);
             __pyx_t_10 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_3)) {
           PyObject *__pyx_temp[3] = {__pyx_t_14, __pyx_t_13, __pyx_t_12};
-          __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 434, __pyx_L1_error)
+          __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 447, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
           PyObject *__pyx_temp[3] = {__pyx_t_14, __pyx_t_13, __pyx_t_12};
-          __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 434, __pyx_L1_error)
+          __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 447, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         } else
         #endif
         {
-          __pyx_t_19 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 434, __pyx_L1_error)
+          __pyx_t_19 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 447, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_19);
           if (__pyx_t_14) {
             __Pyx_GIVEREF(__pyx_t_14); PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_t_14); __pyx_t_14 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_13);
           PyTuple_SET_ITEM(__pyx_t_19, 0+__pyx_t_10, __pyx_t_13);
           __Pyx_GIVEREF(__pyx_t_12);
           PyTuple_SET_ITEM(__pyx_t_19, 1+__pyx_t_10, __pyx_t_12);
           __pyx_t_13 = 0;
           __pyx_t_12 = 0;
-          __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_19, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 434, __pyx_L1_error)
+          __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_19, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 447, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
         }
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":433
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":446
  *             for (case_u, case_v), bias in biases.items():
  *                 if case_u < 0 or case_u >= num_cases_u:
  *                     raise ValueError("case {} is invalid, variable only supports {} "             # <<<<<<<<<<<<<<
  *                                      "cases".format(case_u, self.num_cases(u)))
  * 
  */
-        __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 433, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 446, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_Raise(__pyx_t_3, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __PYX_ERR(0, 433, __pyx_L1_error)
+        __PYX_ERR(0, 446, __pyx_L1_error)
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":432
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":445
  *         if isinstance(biases, abc.Mapping):
  *             for (case_u, case_v), bias in biases.items():
  *                 if case_u < 0 or case_u >= num_cases_u:             # <<<<<<<<<<<<<<
  *                     raise ValueError("case {} is invalid, variable only supports {} "
  *                                      "cases".format(case_u, self.num_cases(u)))
  */
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":436
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":449
  *                                      "cases".format(case_u, self.num_cases(u)))
  * 
  *                 if case_v < 0 or case_v >= num_cases_v:             # <<<<<<<<<<<<<<
  *                     raise ValueError("case {} is invalid, variable only supports {} "
  *                                      "cases".format(case_v, self.num_cases(v)))
  */
       __pyx_t_1 = ((__pyx_v_case_v < 0) != 0);
@@ -19931,29 +20808,29 @@
         goto __pyx_L18_bool_binop_done;
       }
       __pyx_t_1 = ((__pyx_v_case_v >= __pyx_v_num_cases_v) != 0);
       __pyx_t_2 = __pyx_t_1;
       __pyx_L18_bool_binop_done:;
       if (unlikely(__pyx_t_2)) {
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":438
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":451
  *                 if case_v < 0 or case_v >= num_cases_v:
  *                     raise ValueError("case {} is invalid, variable only supports {} "
  *                                      "cases".format(case_v, self.num_cases(v)))             # <<<<<<<<<<<<<<
  * 
  *                 cu = self.case_starts_[u] + case_u
  */
-        __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_case_is_invalid_variable_only_su, __pyx_n_s_format); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 438, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_case_is_invalid_variable_only_su, __pyx_n_s_format); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 451, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
-        __pyx_t_19 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_v); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 438, __pyx_L1_error)
+        __pyx_t_19 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_v); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 451, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_19);
         __pyx_t_5.__pyx_n = 1;
         __pyx_t_5.v = __pyx_v_v;
-        __pyx_t_18 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_5); if (unlikely(__pyx_t_18 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 438, __pyx_L1_error)
-        __pyx_t_12 = PyInt_FromSsize_t(__pyx_t_18); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 438, __pyx_L1_error)
+        __pyx_t_18 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_5); if (unlikely(__pyx_t_18 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 451, __pyx_L1_error)
+        __pyx_t_12 = PyInt_FromSsize_t(__pyx_t_18); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 451, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         __pyx_t_13 = NULL;
         __pyx_t_10 = 0;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
           __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_9);
           if (likely(__pyx_t_13)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
@@ -19962,148 +20839,148 @@
             __Pyx_DECREF_SET(__pyx_t_9, function);
             __pyx_t_10 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_9)) {
           PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_t_19, __pyx_t_12};
-          __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 438, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 451, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
           PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_t_19, __pyx_t_12};
-          __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 438, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 451, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         } else
         #endif
         {
-          __pyx_t_14 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 438, __pyx_L1_error)
+          __pyx_t_14 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 451, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_14);
           if (__pyx_t_13) {
             __Pyx_GIVEREF(__pyx_t_13); PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_13); __pyx_t_13 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_19);
           PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_10, __pyx_t_19);
           __Pyx_GIVEREF(__pyx_t_12);
           PyTuple_SET_ITEM(__pyx_t_14, 1+__pyx_t_10, __pyx_t_12);
           __pyx_t_19 = 0;
           __pyx_t_12 = 0;
-          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_14, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 438, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_14, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 451, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         }
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":437
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":450
  * 
  *                 if case_v < 0 or case_v >= num_cases_v:
  *                     raise ValueError("case {} is invalid, variable only supports {} "             # <<<<<<<<<<<<<<
  *                                      "cases".format(case_v, self.num_cases(v)))
  * 
  */
-        __pyx_t_9 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 437, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 450, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_Raise(__pyx_t_9, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        __PYX_ERR(0, 437, __pyx_L1_error)
+        __PYX_ERR(0, 450, __pyx_L1_error)
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":436
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":449
  *                                      "cases".format(case_u, self.num_cases(u)))
  * 
  *                 if case_v < 0 or case_v >= num_cases_v:             # <<<<<<<<<<<<<<
  *                     raise ValueError("case {} is invalid, variable only supports {} "
  *                                      "cases".format(case_v, self.num_cases(v)))
  */
       }
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":440
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":453
  *                                      "cases".format(case_v, self.num_cases(v)))
  * 
  *                 cu = self.case_starts_[u] + case_u             # <<<<<<<<<<<<<<
  *                 cv = self.case_starts_[v] + case_v
  * 
  */
       __pyx_v_cu = ((__pyx_v_self->case_starts_[__pyx_v_u]) + __pyx_v_case_u);
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":441
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":454
  * 
  *                 cu = self.case_starts_[u] + case_u
  *                 cv = self.case_starts_[v] + case_v             # <<<<<<<<<<<<<<
  * 
  *                 self.bqm_.set_quadratic(cu, cv, bias)
  */
       __pyx_v_cv = ((__pyx_v_self->case_starts_[__pyx_v_v]) + __pyx_v_case_v);
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":443
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":456
  *                 cv = self.case_starts_[v] + case_v
  * 
  *                 self.bqm_.set_quadratic(cu, cv, bias)             # <<<<<<<<<<<<<<
  *         else:
  * 
  */
       try {
         __pyx_v_self->bqm_.set_quadratic(__pyx_v_cu, __pyx_v_cv, __pyx_v_bias);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 443, __pyx_L1_error)
+        __PYX_ERR(0, 456, __pyx_L1_error)
       }
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":430
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":443
  *         cdef Bias[:, :] biases_view
  * 
  *         if isinstance(biases, abc.Mapping):             # <<<<<<<<<<<<<<
  *             for (case_u, case_v), bias in biases.items():
  *                 if case_u < 0 or case_u >= num_cases_u:
  */
     goto __pyx_L9;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":446
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":459
  *         else:
  * 
  *             biases_view = np.asarray(biases, dtype=self.dtype).reshape(num_cases_u, num_cases_v)             # <<<<<<<<<<<<<<
  * 
  *             for case_u in range(biases_view.shape[0]):
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 446, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 459, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 446, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 446, __pyx_L1_error)
+    __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 459, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_INCREF(__pyx_v_biases);
     __Pyx_GIVEREF(__pyx_v_biases);
     PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_biases);
-    __pyx_t_14 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 446, __pyx_L1_error)
+    __pyx_t_14 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 459, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_14);
-    if (PyDict_SetItem(__pyx_t_14, __pyx_n_s_dtype, __pyx_v_self->dtype) < 0) __PYX_ERR(0, 446, __pyx_L1_error)
-    __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_9, __pyx_t_14); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 446, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_14, __pyx_n_s_dtype, __pyx_v_self->dtype) < 0) __PYX_ERR(0, 459, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_9, __pyx_t_14); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 459, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-    __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_reshape); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 446, __pyx_L1_error)
+    __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_reshape); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 459, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_14);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __pyx_t_12 = PyInt_FromSsize_t(__pyx_v_num_cases_u); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 446, __pyx_L1_error)
+    __pyx_t_12 = PyInt_FromSsize_t(__pyx_v_num_cases_u); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 459, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
-    __pyx_t_9 = PyInt_FromSsize_t(__pyx_v_num_cases_v); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 446, __pyx_L1_error)
+    __pyx_t_9 = PyInt_FromSsize_t(__pyx_v_num_cases_v); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 459, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_3 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_14))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_14);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
@@ -20112,97 +20989,97 @@
         __Pyx_DECREF_SET(__pyx_t_14, function);
         __pyx_t_8 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_14)) {
       PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_12, __pyx_t_9};
-      __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_14, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 446, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_14, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 459, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_14)) {
       PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_12, __pyx_t_9};
-      __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_14, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 446, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_14, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 459, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     } else
     #endif
     {
-      __pyx_t_19 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 446, __pyx_L1_error)
+      __pyx_t_19 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 459, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_19);
       if (__pyx_t_3) {
         __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_t_3); __pyx_t_3 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_12);
       PyTuple_SET_ITEM(__pyx_t_19, 0+__pyx_t_8, __pyx_t_12);
       __Pyx_GIVEREF(__pyx_t_9);
       PyTuple_SET_ITEM(__pyx_t_19, 1+__pyx_t_8, __pyx_t_9);
       __pyx_t_12 = 0;
       __pyx_t_9 = 0;
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_14, __pyx_t_19, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 446, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_14, __pyx_t_19, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 459, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
     }
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-    __pyx_t_20 = __Pyx_PyObject_to_MemoryviewSlice_dsds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_20.memview)) __PYX_ERR(0, 446, __pyx_L1_error)
+    __pyx_t_20 = __Pyx_PyObject_to_MemoryviewSlice_dsds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_20.memview)) __PYX_ERR(0, 459, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_v_biases_view = __pyx_t_20;
     __pyx_t_20.memview = NULL;
     __pyx_t_20.data = NULL;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":448
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":461
  *             biases_view = np.asarray(biases, dtype=self.dtype).reshape(num_cases_u, num_cases_v)
  * 
  *             for case_u in range(biases_view.shape[0]):             # <<<<<<<<<<<<<<
  *                 cu = self.case_starts_[u] + case_u
  *                 for case_v in range(biases_view.shape[1]):
  */
     __pyx_t_7 = (__pyx_v_biases_view.shape[0]);
     __pyx_t_4 = __pyx_t_7;
     for (__pyx_t_17 = 0; __pyx_t_17 < __pyx_t_4; __pyx_t_17+=1) {
       __pyx_v_case_u = __pyx_t_17;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":449
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":462
  * 
  *             for case_u in range(biases_view.shape[0]):
  *                 cu = self.case_starts_[u] + case_u             # <<<<<<<<<<<<<<
  *                 for case_v in range(biases_view.shape[1]):
  *                      cv = self.case_starts_[v] + case_v
  */
       __pyx_v_cu = ((__pyx_v_self->case_starts_[__pyx_v_u]) + __pyx_v_case_u);
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":450
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":463
  *             for case_u in range(biases_view.shape[0]):
  *                 cu = self.case_starts_[u] + case_u
  *                 for case_v in range(biases_view.shape[1]):             # <<<<<<<<<<<<<<
  *                      cv = self.case_starts_[v] + case_v
  * 
  */
       __pyx_t_18 = (__pyx_v_biases_view.shape[1]);
       __pyx_t_21 = __pyx_t_18;
       for (__pyx_t_16 = 0; __pyx_t_16 < __pyx_t_21; __pyx_t_16+=1) {
         __pyx_v_case_v = __pyx_t_16;
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":451
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":464
  *                 cu = self.case_starts_[u] + case_u
  *                 for case_v in range(biases_view.shape[1]):
  *                      cv = self.case_starts_[v] + case_v             # <<<<<<<<<<<<<<
  * 
  *                      bias = biases_view[case_u, case_v]
  */
         __pyx_v_cv = ((__pyx_v_self->case_starts_[__pyx_v_v]) + __pyx_v_case_v);
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":453
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":466
  *                      cv = self.case_starts_[v] + case_v
  * 
  *                      bias = biases_view[case_u, case_v]             # <<<<<<<<<<<<<<
  * 
  *                      if bias:
  */
         __pyx_t_22 = __pyx_v_case_u;
@@ -20214,65 +21091,65 @@
         } else if (unlikely(__pyx_t_22 >= __pyx_v_biases_view.shape[0])) __pyx_t_8 = 0;
         if (__pyx_t_23 < 0) {
           __pyx_t_23 += __pyx_v_biases_view.shape[1];
           if (unlikely(__pyx_t_23 < 0)) __pyx_t_8 = 1;
         } else if (unlikely(__pyx_t_23 >= __pyx_v_biases_view.shape[1])) __pyx_t_8 = 1;
         if (unlikely(__pyx_t_8 != -1)) {
           __Pyx_RaiseBufferIndexError(__pyx_t_8);
-          __PYX_ERR(0, 453, __pyx_L1_error)
+          __PYX_ERR(0, 466, __pyx_L1_error)
         }
         __pyx_v_bias = (*((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_biases_view.data + __pyx_t_22 * __pyx_v_biases_view.strides[0]) ) + __pyx_t_23 * __pyx_v_biases_view.strides[1]) )));
 
-        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":455
+        /* "dimod/discrete/cydiscrete_quadratic_model.pyx":468
  *                      bias = biases_view[case_u, case_v]
  * 
  *                      if bias:             # <<<<<<<<<<<<<<
  *                          self.bqm_.set_quadratic(cu, cv, bias)
  * 
  */
         __pyx_t_2 = (__pyx_v_bias != 0);
         if (__pyx_t_2) {
 
-          /* "dimod/discrete/cydiscrete_quadratic_model.pyx":456
+          /* "dimod/discrete/cydiscrete_quadratic_model.pyx":469
  * 
  *                      if bias:
  *                          self.bqm_.set_quadratic(cu, cv, bias)             # <<<<<<<<<<<<<<
  * 
  *         # track in adjacency
  */
           try {
             __pyx_v_self->bqm_.set_quadratic(__pyx_v_cu, __pyx_v_cv, __pyx_v_bias);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 456, __pyx_L1_error)
+            __PYX_ERR(0, 469, __pyx_L1_error)
           }
 
-          /* "dimod/discrete/cydiscrete_quadratic_model.pyx":455
+          /* "dimod/discrete/cydiscrete_quadratic_model.pyx":468
  *                      bias = biases_view[case_u, case_v]
  * 
  *                      if bias:             # <<<<<<<<<<<<<<
  *                          self.bqm_.set_quadratic(cu, cv, bias)
  * 
  */
         }
       }
     }
   }
   __pyx_L9:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":459
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":472
  * 
  *         # track in adjacency
  *         low = lower_bound(self.adj_[u].begin(), self.adj_[u].end(), v)             # <<<<<<<<<<<<<<
  *         if low == self.adj_[u].end() or deref(low) != v:
  *             # need to add
  */
   __pyx_v_low = std::lower_bound<std::vector<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> ::iterator,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex>((__pyx_v_self->adj_[__pyx_v_u]).begin(), (__pyx_v_self->adj_[__pyx_v_u]).end(), __pyx_v_v);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":460
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":473
  *         # track in adjacency
  *         low = lower_bound(self.adj_[u].begin(), self.adj_[u].end(), v)
  *         if low == self.adj_[u].end() or deref(low) != v:             # <<<<<<<<<<<<<<
  *             # need to add
  *             self.adj_[u].insert(low, v)
  */
   __pyx_t_1 = ((__pyx_v_low == (__pyx_v_self->adj_[__pyx_v_u]).end()) != 0);
@@ -20282,52 +21159,52 @@
     goto __pyx_L26_bool_binop_done;
   }
   __pyx_t_1 = (((*__pyx_v_low) != __pyx_v_v) != 0);
   __pyx_t_2 = __pyx_t_1;
   __pyx_L26_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":462
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":475
  *         if low == self.adj_[u].end() or deref(low) != v:
  *             # need to add
  *             self.adj_[u].insert(low, v)             # <<<<<<<<<<<<<<
  *             self.adj_[v].insert(
  *                 lower_bound(self.adj_[v].begin(), self.adj_[v].end(), u),
  */
     try {
       (__pyx_v_self->adj_[__pyx_v_u]).insert(__pyx_v_low, __pyx_v_v);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 462, __pyx_L1_error)
+      __PYX_ERR(0, 475, __pyx_L1_error)
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":463
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":476
  *             # need to add
  *             self.adj_[u].insert(low, v)
  *             self.adj_[v].insert(             # <<<<<<<<<<<<<<
  *                 lower_bound(self.adj_[v].begin(), self.adj_[v].end(), u),
  *                 u)
  */
     try {
       (__pyx_v_self->adj_[__pyx_v_v]).insert(std::lower_bound<std::vector<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> ::iterator,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex>((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_self->adj_[__pyx_v_v]).end(), __pyx_v_u), __pyx_v_u);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 463, __pyx_L1_error)
+      __PYX_ERR(0, 476, __pyx_L1_error)
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":460
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":473
  *         # track in adjacency
  *         low = lower_bound(self.adj_[u].begin(), self.adj_[u].end(), v)
  *         if low == self.adj_[u].end() or deref(low) != v:             # <<<<<<<<<<<<<<
  *             # need to add
  *             self.adj_[u].insert(low, v)
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":413
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":426
  *         self.bqm_.set_linear(self.case_starts_[v] + case, b)
  * 
  *     def set_quadratic(self, VarIndex u, VarIndex v, biases):             # <<<<<<<<<<<<<<
  * 
  *         # check that the interaction does in fact exist
  */
 
@@ -20348,15 +21225,15 @@
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_biases_view, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dimod/discrete/cydiscrete_quadratic_model.pyx":467
+/* "dimod/discrete/cydiscrete_quadratic_model.pyx":480
  *                 u)
  * 
  *     cpdef Py_ssize_t set_quadratic_case(self,             # <<<<<<<<<<<<<<
  *                                         VarIndex u, CaseIndex case_u,
  *                                         VarIndex v, CaseIndex case_v,
  */
 
@@ -20391,26 +21268,26 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_quadratic_case); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 467, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_quadratic_case); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 480, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_33set_quadratic_case)) {
-        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_u); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 467, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_npy_int64(__pyx_v_u); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 480, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_u); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 467, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_u); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 480, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 467, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_v); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 480, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
-        __pyx_t_6 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_v); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 467, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_v); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 480, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_7 = PyFloat_FromDouble(__pyx_v_bias); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 467, __pyx_L1_error)
+        __pyx_t_7 = PyFloat_FromDouble(__pyx_v_bias); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 480, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_8 = __pyx_t_1; __pyx_t_9 = NULL;
         __pyx_t_10 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
           __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
           if (likely(__pyx_t_9)) {
@@ -20420,39 +21297,39 @@
             __Pyx_DECREF_SET(__pyx_t_8, function);
             __pyx_t_10 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_8)) {
           PyObject *__pyx_temp[6] = {__pyx_t_9, __pyx_t_3, __pyx_t_4, __pyx_t_5, __pyx_t_6, __pyx_t_7};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_10, 5+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 467, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_10, 5+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 480, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_8)) {
           PyObject *__pyx_temp[6] = {__pyx_t_9, __pyx_t_3, __pyx_t_4, __pyx_t_5, __pyx_t_6, __pyx_t_7};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_10, 5+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 467, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_10, 5+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 480, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         } else
         #endif
         {
-          __pyx_t_11 = PyTuple_New(5+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 467, __pyx_L1_error)
+          __pyx_t_11 = PyTuple_New(5+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 480, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_11);
           if (__pyx_t_9) {
             __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_9); __pyx_t_9 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_10, __pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_4);
@@ -20464,20 +21341,20 @@
           __Pyx_GIVEREF(__pyx_t_7);
           PyTuple_SET_ITEM(__pyx_t_11, 4+__pyx_t_10, __pyx_t_7);
           __pyx_t_3 = 0;
           __pyx_t_4 = 0;
           __pyx_t_5 = 0;
           __pyx_t_6 = 0;
           __pyx_t_7 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 467, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 480, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         }
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 467, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 480, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -20488,50 +21365,50 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":474
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":487
  *         # self.num_cases checks that the variables are valid
  * 
  *         if case_u < 0 or case_u >= self.num_cases(u):             # <<<<<<<<<<<<<<
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case_u, self.num_cases(u)))
  */
   __pyx_t_14 = ((__pyx_v_case_u < 0) != 0);
   if (!__pyx_t_14) {
   } else {
     __pyx_t_13 = __pyx_t_14;
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_15.__pyx_n = 1;
   __pyx_t_15.v = __pyx_v_u;
-  __pyx_t_12 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_15); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 474, __pyx_L1_error)
+  __pyx_t_12 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_15); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 487, __pyx_L1_error)
   __pyx_t_14 = ((__pyx_v_case_u >= __pyx_t_12) != 0);
   __pyx_t_13 = __pyx_t_14;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_13)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":476
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":489
  *         if case_u < 0 or case_u >= self.num_cases(u):
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case_u, self.num_cases(u)))             # <<<<<<<<<<<<<<
  * 
  *         if case_v < 0 or case_v >= self.num_cases(v):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_case_is_invalid_variable_only_su, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 476, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_case_is_invalid_variable_only_su, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 489, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_8 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_u); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 476, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_u); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 489, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_15.__pyx_n = 1;
     __pyx_t_15.v = __pyx_v_u;
-    __pyx_t_12 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_15); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 476, __pyx_L1_error)
-    __pyx_t_11 = PyInt_FromSsize_t(__pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 476, __pyx_L1_error)
+    __pyx_t_12 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_15); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 489, __pyx_L1_error)
+    __pyx_t_11 = PyInt_FromSsize_t(__pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 489, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __pyx_t_7 = NULL;
     __pyx_t_10 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -20540,108 +21417,108 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_10 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_8, __pyx_t_11};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 476, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 489, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_8, __pyx_t_11};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 476, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 489, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     } else
     #endif
     {
-      __pyx_t_6 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 476, __pyx_L1_error)
+      __pyx_t_6 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 489, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       if (__pyx_t_7) {
         __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7); __pyx_t_7 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_8);
       PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_10, __pyx_t_8);
       __Pyx_GIVEREF(__pyx_t_11);
       PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_10, __pyx_t_11);
       __pyx_t_8 = 0;
       __pyx_t_11 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 476, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 489, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":475
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":488
  * 
  *         if case_u < 0 or case_u >= self.num_cases(u):
  *             raise ValueError("case {} is invalid, variable only supports {} "             # <<<<<<<<<<<<<<
  *                              "cases".format(case_u, self.num_cases(u)))
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 475, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 488, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 475, __pyx_L1_error)
+    __PYX_ERR(0, 488, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":474
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":487
  *         # self.num_cases checks that the variables are valid
  * 
  *         if case_u < 0 or case_u >= self.num_cases(u):             # <<<<<<<<<<<<<<
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case_u, self.num_cases(u)))
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":478
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":491
  *                              "cases".format(case_u, self.num_cases(u)))
  * 
  *         if case_v < 0 or case_v >= self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case_v, self.num_cases(v)))
  */
   __pyx_t_14 = ((__pyx_v_case_v < 0) != 0);
   if (!__pyx_t_14) {
   } else {
     __pyx_t_13 = __pyx_t_14;
     goto __pyx_L7_bool_binop_done;
   }
   __pyx_t_15.__pyx_n = 1;
   __pyx_t_15.v = __pyx_v_v;
-  __pyx_t_12 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_15); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 478, __pyx_L1_error)
+  __pyx_t_12 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_15); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 491, __pyx_L1_error)
   __pyx_t_14 = ((__pyx_v_case_v >= __pyx_t_12) != 0);
   __pyx_t_13 = __pyx_t_14;
   __pyx_L7_bool_binop_done:;
   if (unlikely(__pyx_t_13)) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":480
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":493
  *         if case_v < 0 or case_v >= self.num_cases(v):
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case_v, self.num_cases(v)))             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_case_is_invalid_variable_only_su, __pyx_n_s_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 480, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_case_is_invalid_variable_only_su, __pyx_n_s_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 493, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_v); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 480, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_npy_int64(__pyx_v_case_v); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 493, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_15.__pyx_n = 1;
     __pyx_t_15.v = __pyx_v_v;
-    __pyx_t_12 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_15); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 480, __pyx_L1_error)
-    __pyx_t_11 = PyInt_FromSsize_t(__pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 480, __pyx_L1_error)
+    __pyx_t_12 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, &__pyx_t_15); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 493, __pyx_L1_error)
+    __pyx_t_11 = PyInt_FromSsize_t(__pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 493, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __pyx_t_8 = NULL;
     __pyx_t_10 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -20650,114 +21527,114 @@
         __Pyx_DECREF_SET(__pyx_t_1, function);
         __pyx_t_10 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_1)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_6, __pyx_t_11};
-      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 480, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 493, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_6, __pyx_t_11};
-      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 480, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 493, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     } else
     #endif
     {
-      __pyx_t_7 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 480, __pyx_L1_error)
+      __pyx_t_7 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 493, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       if (__pyx_t_8) {
         __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_8); __pyx_t_8 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_10, __pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_11);
       PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_10, __pyx_t_11);
       __pyx_t_6 = 0;
       __pyx_t_11 = 0;
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 480, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 493, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":479
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":492
  * 
  *         if case_v < 0 or case_v >= self.num_cases(v):
  *             raise ValueError("case {} is invalid, variable only supports {} "             # <<<<<<<<<<<<<<
  *                              "cases".format(case_v, self.num_cases(v)))
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 479, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 492, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 479, __pyx_L1_error)
+    __PYX_ERR(0, 492, __pyx_L1_error)
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":478
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":491
  *                              "cases".format(case_u, self.num_cases(u)))
  * 
  *         if case_v < 0 or case_v >= self.num_cases(v):             # <<<<<<<<<<<<<<
  *             raise ValueError("case {} is invalid, variable only supports {} "
  *                              "cases".format(case_v, self.num_cases(v)))
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":483
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":496
  * 
  * 
  *         cdef CaseIndex cu = self.case_starts_[u] + case_u             # <<<<<<<<<<<<<<
  *         cdef CaseIndex cv = self.case_starts_[v] + case_v
  * 
  */
   __pyx_v_cu = ((__pyx_v_self->case_starts_[__pyx_v_u]) + __pyx_v_case_u);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":484
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":497
  * 
  *         cdef CaseIndex cu = self.case_starts_[u] + case_u
  *         cdef CaseIndex cv = self.case_starts_[v] + case_v             # <<<<<<<<<<<<<<
  * 
  *         self.bqm_.set_quadratic(cu, cv, bias)
  */
   __pyx_v_cv = ((__pyx_v_self->case_starts_[__pyx_v_v]) + __pyx_v_case_v);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":486
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":499
  *         cdef CaseIndex cv = self.case_starts_[v] + case_v
  * 
  *         self.bqm_.set_quadratic(cu, cv, bias)             # <<<<<<<<<<<<<<
  * 
  *         # track in adjacency
  */
   try {
     __pyx_v_self->bqm_.set_quadratic(__pyx_v_cu, __pyx_v_cv, __pyx_v_bias);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 486, __pyx_L1_error)
+    __PYX_ERR(0, 499, __pyx_L1_error)
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":489
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":502
  * 
  *         # track in adjacency
  *         low = lower_bound(self.adj_[u].begin(), self.adj_[u].end(), v)             # <<<<<<<<<<<<<<
  *         if low == self.adj_[u].end() or deref(low) != v:
  *             # need to add
  */
   __pyx_v_low = std::lower_bound<std::vector<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> ::iterator,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex>((__pyx_v_self->adj_[__pyx_v_u]).begin(), (__pyx_v_self->adj_[__pyx_v_u]).end(), __pyx_v_v);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":490
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":503
  *         # track in adjacency
  *         low = lower_bound(self.adj_[u].begin(), self.adj_[u].end(), v)
  *         if low == self.adj_[u].end() or deref(low) != v:             # <<<<<<<<<<<<<<
  *             # need to add
  *             self.adj_[u].insert(low, v)
  */
   __pyx_t_14 = ((__pyx_v_low == (__pyx_v_self->adj_[__pyx_v_u]).end()) != 0);
@@ -20767,52 +21644,52 @@
     goto __pyx_L10_bool_binop_done;
   }
   __pyx_t_14 = (((*__pyx_v_low) != __pyx_v_v) != 0);
   __pyx_t_13 = __pyx_t_14;
   __pyx_L10_bool_binop_done:;
   if (__pyx_t_13) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":492
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":505
  *         if low == self.adj_[u].end() or deref(low) != v:
  *             # need to add
  *             self.adj_[u].insert(low, v)             # <<<<<<<<<<<<<<
  *             self.adj_[v].insert(
  *                 lower_bound(self.adj_[v].begin(), self.adj_[v].end(), u),
  */
     try {
       (__pyx_v_self->adj_[__pyx_v_u]).insert(__pyx_v_low, __pyx_v_v);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 492, __pyx_L1_error)
+      __PYX_ERR(0, 505, __pyx_L1_error)
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":493
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":506
  *             # need to add
  *             self.adj_[u].insert(low, v)
  *             self.adj_[v].insert(             # <<<<<<<<<<<<<<
  *                 lower_bound(self.adj_[v].begin(), self.adj_[v].end(), u),
  *                 u)
  */
     try {
       (__pyx_v_self->adj_[__pyx_v_v]).insert(std::lower_bound<std::vector<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex> ::iterator,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_VarIndex>((__pyx_v_self->adj_[__pyx_v_v]).begin(), (__pyx_v_self->adj_[__pyx_v_v]).end(), __pyx_v_u), __pyx_v_u);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 493, __pyx_L1_error)
+      __PYX_ERR(0, 506, __pyx_L1_error)
     }
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":490
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":503
  *         # track in adjacency
  *         low = lower_bound(self.adj_[u].begin(), self.adj_[u].end(), v)
  *         if low == self.adj_[u].end() or deref(low) != v:             # <<<<<<<<<<<<<<
  *             # need to add
  *             self.adj_[u].insert(low, v)
  */
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":467
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":480
  *                 u)
  * 
  *     cpdef Py_ssize_t set_quadratic_case(self,             # <<<<<<<<<<<<<<
  *                                         VarIndex u, CaseIndex case_u,
  *                                         VarIndex v, CaseIndex case_v,
  */
 
@@ -20876,56 +21753,56 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_u)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_case_u)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("set_quadratic_case", 1, 5, 5, 1); __PYX_ERR(0, 467, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("set_quadratic_case", 1, 5, 5, 1); __PYX_ERR(0, 480, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("set_quadratic_case", 1, 5, 5, 2); __PYX_ERR(0, 467, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("set_quadratic_case", 1, 5, 5, 2); __PYX_ERR(0, 480, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_case_v)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("set_quadratic_case", 1, 5, 5, 3); __PYX_ERR(0, 467, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("set_quadratic_case", 1, 5, 5, 3); __PYX_ERR(0, 480, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_bias)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("set_quadratic_case", 1, 5, 5, 4); __PYX_ERR(0, 467, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("set_quadratic_case", 1, 5, 5, 4); __PYX_ERR(0, 480, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_quadratic_case") < 0)) __PYX_ERR(0, 467, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_quadratic_case") < 0)) __PYX_ERR(0, 480, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 5) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
     }
-    __pyx_v_u = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_u == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 468, __pyx_L3_error)
-    __pyx_v_case_u = __Pyx_PyInt_As_npy_int64(values[1]); if (unlikely((__pyx_v_case_u == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 468, __pyx_L3_error)
-    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[2]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 469, __pyx_L3_error)
-    __pyx_v_case_v = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_case_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 469, __pyx_L3_error)
-    __pyx_v_bias = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_bias == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 470, __pyx_L3_error)
+    __pyx_v_u = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_u == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 481, __pyx_L3_error)
+    __pyx_v_case_u = __Pyx_PyInt_As_npy_int64(values[1]); if (unlikely((__pyx_v_case_u == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 481, __pyx_L3_error)
+    __pyx_v_v = __Pyx_PyInt_As_npy_int64(values[2]); if (unlikely((__pyx_v_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 482, __pyx_L3_error)
+    __pyx_v_case_v = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_case_v == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 482, __pyx_L3_error)
+    __pyx_v_bias = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_bias == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 483, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("set_quadratic_case", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 467, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("set_quadratic_case", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 480, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel.set_quadratic_case", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_32set_quadratic_case(((struct __pyx_obj_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self), __pyx_v_u, __pyx_v_case_u, __pyx_v_v, __pyx_v_case_v, __pyx_v_bias);
 
@@ -20940,16 +21817,16 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_quadratic_case", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_quadratic_case(__pyx_v_self, __pyx_v_u, __pyx_v_case_u, __pyx_v_v, __pyx_v_case_v, __pyx_v_bias, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 467, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 467, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_set_quadratic_case(__pyx_v_self, __pyx_v_u, __pyx_v_case_u, __pyx_v_v, __pyx_v_case_v, __pyx_v_bias, 1); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 480, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 480, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -20958,15 +21835,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dimod/discrete/cydiscrete_quadratic_model.pyx":499
+/* "dimod/discrete/cydiscrete_quadratic_model.pyx":512
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cdef void _into_numpy_vectors(self, Unsigned[:] starts, Bias[:] ldata,             # <<<<<<<<<<<<<<
  *                                   Unsigned[:] irow, Unsigned[:] icol, Bias[:] qdata):
  *         # we don't do array length checking so be careful! This can segfault
  */
 
@@ -20989,104 +21866,104 @@
   dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_11;
   dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::bias_type __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_0_into_numpy_vectors", 0);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":505
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":518
  * 
  *         cdef Py_ssize_t vi
  *         for vi in range(self.num_variables()):             # <<<<<<<<<<<<<<
  *             starts[vi] = self.case_starts_[vi]
  * 
  */
   __pyx_t_1 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_variables(__pyx_v_self, 0);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_vi = __pyx_t_3;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":506
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":519
  *         cdef Py_ssize_t vi
  *         for vi in range(self.num_variables()):
  *             starts[vi] = self.case_starts_[vi]             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t ci = 0
  */
     __pyx_t_4 = __pyx_v_vi;
     *((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_starts.data + __pyx_t_4 * __pyx_v_starts.strides[0]) )) = (__pyx_v_self->case_starts_[__pyx_v_vi]);
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":508
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":521
  *             starts[vi] = self.case_starts_[vi]
  * 
  *         cdef Py_ssize_t ci = 0             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t qi = 0
  *         for ci in range(self.bqm_.num_variables()):
  */
   __pyx_v_ci = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":509
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":522
  * 
  *         cdef Py_ssize_t ci = 0
  *         cdef Py_ssize_t qi = 0             # <<<<<<<<<<<<<<
  *         for ci in range(self.bqm_.num_variables()):
  *             ldata[ci] = self.bqm_.linear(ci)
  */
   __pyx_v_qi = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":510
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":523
  *         cdef Py_ssize_t ci = 0
  *         cdef Py_ssize_t qi = 0
  *         for ci in range(self.bqm_.num_variables()):             # <<<<<<<<<<<<<<
  *             ldata[ci] = self.bqm_.linear(ci)
  * 
  */
   try {
     __pyx_t_5 = __pyx_v_self->bqm_.num_variables();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 510, __pyx_L1_error)
+    __PYX_ERR(0, 523, __pyx_L1_error)
   }
   __pyx_t_6 = __pyx_t_5;
   for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_6; __pyx_t_1+=1) {
     __pyx_v_ci = __pyx_t_1;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":511
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":524
  *         cdef Py_ssize_t qi = 0
  *         for ci in range(self.bqm_.num_variables()):
  *             ldata[ci] = self.bqm_.linear(ci)             # <<<<<<<<<<<<<<
  * 
  *             span = self.bqm_.neighborhood(ci)
  */
     try {
       __pyx_t_7 = __pyx_v_self->bqm_.linear(__pyx_v_ci);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 511, __pyx_L1_error)
+      __PYX_ERR(0, 524, __pyx_L1_error)
     }
     __pyx_t_4 = __pyx_v_ci;
     *((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_ldata.data + __pyx_t_4 * __pyx_v_ldata.strides[0]) )) = __pyx_t_7;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":513
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":526
  *             ldata[ci] = self.bqm_.linear(ci)
  * 
  *             span = self.bqm_.neighborhood(ci)             # <<<<<<<<<<<<<<
  *             while span.first != span.second and deref(span.first).first < ci:
  * 
  */
     try {
       __pyx_t_8 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 513, __pyx_L1_error)
+      __PYX_ERR(0, 526, __pyx_L1_error)
     }
     __pyx_v_span = __pyx_t_8;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":514
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":527
  * 
  *             span = self.bqm_.neighborhood(ci)
  *             while span.first != span.second and deref(span.first).first < ci:             # <<<<<<<<<<<<<<
  * 
  *                 irow[qi] = ci
  */
     while (1) {
@@ -21097,67 +21974,67 @@
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = (((*__pyx_v_span.first).first < __pyx_v_ci) != 0);
       __pyx_t_9 = __pyx_t_10;
       __pyx_L9_bool_binop_done:;
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":516
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":529
  *             while span.first != span.second and deref(span.first).first < ci:
  * 
  *                 irow[qi] = ci             # <<<<<<<<<<<<<<
  *                 icol[qi] = deref(span.first).first
  *                 qdata[qi] = deref(span.first).second
  */
       __pyx_t_4 = __pyx_v_qi;
       *((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )) = __pyx_v_ci;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":517
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":530
  * 
  *                 irow[qi] = ci
  *                 icol[qi] = deref(span.first).first             # <<<<<<<<<<<<<<
  *                 qdata[qi] = deref(span.first).second
  * 
  */
       __pyx_t_11 = (*__pyx_v_span.first).first;
       __pyx_t_4 = __pyx_v_qi;
       *((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )) = __pyx_t_11;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":518
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":531
  *                 irow[qi] = ci
  *                 icol[qi] = deref(span.first).first
  *                 qdata[qi] = deref(span.first).second             # <<<<<<<<<<<<<<
  * 
  *                 inc(span.first)
  */
       __pyx_t_12 = (*__pyx_v_span.first).second;
       __pyx_t_4 = __pyx_v_qi;
       *((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_4 * __pyx_v_qdata.strides[0]) )) = __pyx_t_12;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":520
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":533
  *                 qdata[qi] = deref(span.first).second
  * 
  *                 inc(span.first)             # <<<<<<<<<<<<<<
  *                 qi += 1
  * 
  */
       (void)((++__pyx_v_span.first));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":521
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":534
  * 
  *                 inc(span.first)
  *                 qi += 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_qi = (__pyx_v_qi + 1);
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":499
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":512
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cdef void _into_numpy_vectors(self, Unsigned[:] starts, Bias[:] ldata,             # <<<<<<<<<<<<<<
  *                                   Unsigned[:] irow, Unsigned[:] icol, Bias[:] qdata):
  *         # we don't do array length checking so be careful! This can segfault
  */
 
@@ -21188,104 +22065,104 @@
   dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_11;
   dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::bias_type __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_1_into_numpy_vectors", 0);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":505
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":518
  * 
  *         cdef Py_ssize_t vi
  *         for vi in range(self.num_variables()):             # <<<<<<<<<<<<<<
  *             starts[vi] = self.case_starts_[vi]
  * 
  */
   __pyx_t_1 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_variables(__pyx_v_self, 0);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_vi = __pyx_t_3;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":506
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":519
  *         cdef Py_ssize_t vi
  *         for vi in range(self.num_variables()):
  *             starts[vi] = self.case_starts_[vi]             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t ci = 0
  */
     __pyx_t_4 = __pyx_v_vi;
     *((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_starts.data + __pyx_t_4 * __pyx_v_starts.strides[0]) )) = (__pyx_v_self->case_starts_[__pyx_v_vi]);
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":508
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":521
  *             starts[vi] = self.case_starts_[vi]
  * 
  *         cdef Py_ssize_t ci = 0             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t qi = 0
  *         for ci in range(self.bqm_.num_variables()):
  */
   __pyx_v_ci = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":509
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":522
  * 
  *         cdef Py_ssize_t ci = 0
  *         cdef Py_ssize_t qi = 0             # <<<<<<<<<<<<<<
  *         for ci in range(self.bqm_.num_variables()):
  *             ldata[ci] = self.bqm_.linear(ci)
  */
   __pyx_v_qi = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":510
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":523
  *         cdef Py_ssize_t ci = 0
  *         cdef Py_ssize_t qi = 0
  *         for ci in range(self.bqm_.num_variables()):             # <<<<<<<<<<<<<<
  *             ldata[ci] = self.bqm_.linear(ci)
  * 
  */
   try {
     __pyx_t_5 = __pyx_v_self->bqm_.num_variables();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 510, __pyx_L1_error)
+    __PYX_ERR(0, 523, __pyx_L1_error)
   }
   __pyx_t_6 = __pyx_t_5;
   for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_6; __pyx_t_1+=1) {
     __pyx_v_ci = __pyx_t_1;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":511
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":524
  *         cdef Py_ssize_t qi = 0
  *         for ci in range(self.bqm_.num_variables()):
  *             ldata[ci] = self.bqm_.linear(ci)             # <<<<<<<<<<<<<<
  * 
  *             span = self.bqm_.neighborhood(ci)
  */
     try {
       __pyx_t_7 = __pyx_v_self->bqm_.linear(__pyx_v_ci);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 511, __pyx_L1_error)
+      __PYX_ERR(0, 524, __pyx_L1_error)
     }
     __pyx_t_4 = __pyx_v_ci;
     *((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_ldata.data + __pyx_t_4 * __pyx_v_ldata.strides[0]) )) = __pyx_t_7;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":513
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":526
  *             ldata[ci] = self.bqm_.linear(ci)
  * 
  *             span = self.bqm_.neighborhood(ci)             # <<<<<<<<<<<<<<
  *             while span.first != span.second and deref(span.first).first < ci:
  * 
  */
     try {
       __pyx_t_8 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 513, __pyx_L1_error)
+      __PYX_ERR(0, 526, __pyx_L1_error)
     }
     __pyx_v_span = __pyx_t_8;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":514
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":527
  * 
  *             span = self.bqm_.neighborhood(ci)
  *             while span.first != span.second and deref(span.first).first < ci:             # <<<<<<<<<<<<<<
  * 
  *                 irow[qi] = ci
  */
     while (1) {
@@ -21296,67 +22173,67 @@
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = (((*__pyx_v_span.first).first < __pyx_v_ci) != 0);
       __pyx_t_9 = __pyx_t_10;
       __pyx_L9_bool_binop_done:;
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":516
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":529
  *             while span.first != span.second and deref(span.first).first < ci:
  * 
  *                 irow[qi] = ci             # <<<<<<<<<<<<<<
  *                 icol[qi] = deref(span.first).first
  *                 qdata[qi] = deref(span.first).second
  */
       __pyx_t_4 = __pyx_v_qi;
       *((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )) = __pyx_v_ci;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":517
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":530
  * 
  *                 irow[qi] = ci
  *                 icol[qi] = deref(span.first).first             # <<<<<<<<<<<<<<
  *                 qdata[qi] = deref(span.first).second
  * 
  */
       __pyx_t_11 = (*__pyx_v_span.first).first;
       __pyx_t_4 = __pyx_v_qi;
       *((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )) = __pyx_t_11;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":518
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":531
  *                 irow[qi] = ci
  *                 icol[qi] = deref(span.first).first
  *                 qdata[qi] = deref(span.first).second             # <<<<<<<<<<<<<<
  * 
  *                 inc(span.first)
  */
       __pyx_t_12 = (*__pyx_v_span.first).second;
       __pyx_t_4 = __pyx_v_qi;
       *((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_4 * __pyx_v_qdata.strides[0]) )) = __pyx_t_12;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":520
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":533
  *                 qdata[qi] = deref(span.first).second
  * 
  *                 inc(span.first)             # <<<<<<<<<<<<<<
  *                 qi += 1
  * 
  */
       (void)((++__pyx_v_span.first));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":521
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":534
  * 
  *                 inc(span.first)
  *                 qi += 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_qi = (__pyx_v_qi + 1);
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":499
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":512
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cdef void _into_numpy_vectors(self, Unsigned[:] starts, Bias[:] ldata,             # <<<<<<<<<<<<<<
  *                                   Unsigned[:] irow, Unsigned[:] icol, Bias[:] qdata):
  *         # we don't do array length checking so be careful! This can segfault
  */
 
@@ -21387,104 +22264,104 @@
   dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_11;
   dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::bias_type __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_2_into_numpy_vectors", 0);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":505
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":518
  * 
  *         cdef Py_ssize_t vi
  *         for vi in range(self.num_variables()):             # <<<<<<<<<<<<<<
  *             starts[vi] = self.case_starts_[vi]
  * 
  */
   __pyx_t_1 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_variables(__pyx_v_self, 0);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_vi = __pyx_t_3;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":506
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":519
  *         cdef Py_ssize_t vi
  *         for vi in range(self.num_variables()):
  *             starts[vi] = self.case_starts_[vi]             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t ci = 0
  */
     __pyx_t_4 = __pyx_v_vi;
     *((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_starts.data + __pyx_t_4 * __pyx_v_starts.strides[0]) )) = (__pyx_v_self->case_starts_[__pyx_v_vi]);
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":508
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":521
  *             starts[vi] = self.case_starts_[vi]
  * 
  *         cdef Py_ssize_t ci = 0             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t qi = 0
  *         for ci in range(self.bqm_.num_variables()):
  */
   __pyx_v_ci = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":509
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":522
  * 
  *         cdef Py_ssize_t ci = 0
  *         cdef Py_ssize_t qi = 0             # <<<<<<<<<<<<<<
  *         for ci in range(self.bqm_.num_variables()):
  *             ldata[ci] = self.bqm_.linear(ci)
  */
   __pyx_v_qi = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":510
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":523
  *         cdef Py_ssize_t ci = 0
  *         cdef Py_ssize_t qi = 0
  *         for ci in range(self.bqm_.num_variables()):             # <<<<<<<<<<<<<<
  *             ldata[ci] = self.bqm_.linear(ci)
  * 
  */
   try {
     __pyx_t_5 = __pyx_v_self->bqm_.num_variables();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 510, __pyx_L1_error)
+    __PYX_ERR(0, 523, __pyx_L1_error)
   }
   __pyx_t_6 = __pyx_t_5;
   for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_6; __pyx_t_1+=1) {
     __pyx_v_ci = __pyx_t_1;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":511
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":524
  *         cdef Py_ssize_t qi = 0
  *         for ci in range(self.bqm_.num_variables()):
  *             ldata[ci] = self.bqm_.linear(ci)             # <<<<<<<<<<<<<<
  * 
  *             span = self.bqm_.neighborhood(ci)
  */
     try {
       __pyx_t_7 = __pyx_v_self->bqm_.linear(__pyx_v_ci);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 511, __pyx_L1_error)
+      __PYX_ERR(0, 524, __pyx_L1_error)
     }
     __pyx_t_4 = __pyx_v_ci;
     *((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_ldata.data + __pyx_t_4 * __pyx_v_ldata.strides[0]) )) = __pyx_t_7;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":513
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":526
  *             ldata[ci] = self.bqm_.linear(ci)
  * 
  *             span = self.bqm_.neighborhood(ci)             # <<<<<<<<<<<<<<
  *             while span.first != span.second and deref(span.first).first < ci:
  * 
  */
     try {
       __pyx_t_8 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 513, __pyx_L1_error)
+      __PYX_ERR(0, 526, __pyx_L1_error)
     }
     __pyx_v_span = __pyx_t_8;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":514
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":527
  * 
  *             span = self.bqm_.neighborhood(ci)
  *             while span.first != span.second and deref(span.first).first < ci:             # <<<<<<<<<<<<<<
  * 
  *                 irow[qi] = ci
  */
     while (1) {
@@ -21495,67 +22372,67 @@
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = (((*__pyx_v_span.first).first < __pyx_v_ci) != 0);
       __pyx_t_9 = __pyx_t_10;
       __pyx_L9_bool_binop_done:;
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":516
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":529
  *             while span.first != span.second and deref(span.first).first < ci:
  * 
  *                 irow[qi] = ci             # <<<<<<<<<<<<<<
  *                 icol[qi] = deref(span.first).first
  *                 qdata[qi] = deref(span.first).second
  */
       __pyx_t_4 = __pyx_v_qi;
       *((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )) = __pyx_v_ci;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":517
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":530
  * 
  *                 irow[qi] = ci
  *                 icol[qi] = deref(span.first).first             # <<<<<<<<<<<<<<
  *                 qdata[qi] = deref(span.first).second
  * 
  */
       __pyx_t_11 = (*__pyx_v_span.first).first;
       __pyx_t_4 = __pyx_v_qi;
       *((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )) = __pyx_t_11;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":518
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":531
  *                 irow[qi] = ci
  *                 icol[qi] = deref(span.first).first
  *                 qdata[qi] = deref(span.first).second             # <<<<<<<<<<<<<<
  * 
  *                 inc(span.first)
  */
       __pyx_t_12 = (*__pyx_v_span.first).second;
       __pyx_t_4 = __pyx_v_qi;
       *((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_4 * __pyx_v_qdata.strides[0]) )) = __pyx_t_12;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":520
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":533
  *                 qdata[qi] = deref(span.first).second
  * 
  *                 inc(span.first)             # <<<<<<<<<<<<<<
  *                 qi += 1
  * 
  */
       (void)((++__pyx_v_span.first));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":521
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":534
  * 
  *                 inc(span.first)
  *                 qi += 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_qi = (__pyx_v_qi + 1);
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":499
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":512
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cdef void _into_numpy_vectors(self, Unsigned[:] starts, Bias[:] ldata,             # <<<<<<<<<<<<<<
  *                                   Unsigned[:] irow, Unsigned[:] icol, Bias[:] qdata):
  *         # we don't do array length checking so be careful! This can segfault
  */
 
@@ -21586,104 +22463,104 @@
   dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::variable_type __pyx_t_11;
   dimod::AdjVectorBQM<__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_CaseIndex,__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias> ::bias_type __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_3_into_numpy_vectors", 0);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":505
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":518
  * 
  *         cdef Py_ssize_t vi
  *         for vi in range(self.num_variables()):             # <<<<<<<<<<<<<<
  *             starts[vi] = self.case_starts_[vi]
  * 
  */
   __pyx_t_1 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_variables(__pyx_v_self, 0);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_vi = __pyx_t_3;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":506
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":519
  *         cdef Py_ssize_t vi
  *         for vi in range(self.num_variables()):
  *             starts[vi] = self.case_starts_[vi]             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t ci = 0
  */
     __pyx_t_4 = __pyx_v_vi;
     *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_starts.data + __pyx_t_4 * __pyx_v_starts.strides[0]) )) = (__pyx_v_self->case_starts_[__pyx_v_vi]);
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":508
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":521
  *             starts[vi] = self.case_starts_[vi]
  * 
  *         cdef Py_ssize_t ci = 0             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t qi = 0
  *         for ci in range(self.bqm_.num_variables()):
  */
   __pyx_v_ci = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":509
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":522
  * 
  *         cdef Py_ssize_t ci = 0
  *         cdef Py_ssize_t qi = 0             # <<<<<<<<<<<<<<
  *         for ci in range(self.bqm_.num_variables()):
  *             ldata[ci] = self.bqm_.linear(ci)
  */
   __pyx_v_qi = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":510
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":523
  *         cdef Py_ssize_t ci = 0
  *         cdef Py_ssize_t qi = 0
  *         for ci in range(self.bqm_.num_variables()):             # <<<<<<<<<<<<<<
  *             ldata[ci] = self.bqm_.linear(ci)
  * 
  */
   try {
     __pyx_t_5 = __pyx_v_self->bqm_.num_variables();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 510, __pyx_L1_error)
+    __PYX_ERR(0, 523, __pyx_L1_error)
   }
   __pyx_t_6 = __pyx_t_5;
   for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_6; __pyx_t_1+=1) {
     __pyx_v_ci = __pyx_t_1;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":511
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":524
  *         cdef Py_ssize_t qi = 0
  *         for ci in range(self.bqm_.num_variables()):
  *             ldata[ci] = self.bqm_.linear(ci)             # <<<<<<<<<<<<<<
  * 
  *             span = self.bqm_.neighborhood(ci)
  */
     try {
       __pyx_t_7 = __pyx_v_self->bqm_.linear(__pyx_v_ci);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 511, __pyx_L1_error)
+      __PYX_ERR(0, 524, __pyx_L1_error)
     }
     __pyx_t_4 = __pyx_v_ci;
     *((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_ldata.data + __pyx_t_4 * __pyx_v_ldata.strides[0]) )) = __pyx_t_7;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":513
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":526
  *             ldata[ci] = self.bqm_.linear(ci)
  * 
  *             span = self.bqm_.neighborhood(ci)             # <<<<<<<<<<<<<<
  *             while span.first != span.second and deref(span.first).first < ci:
  * 
  */
     try {
       __pyx_t_8 = __pyx_v_self->bqm_.neighborhood(__pyx_v_ci);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 513, __pyx_L1_error)
+      __PYX_ERR(0, 526, __pyx_L1_error)
     }
     __pyx_v_span = __pyx_t_8;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":514
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":527
  * 
  *             span = self.bqm_.neighborhood(ci)
  *             while span.first != span.second and deref(span.first).first < ci:             # <<<<<<<<<<<<<<
  * 
  *                 irow[qi] = ci
  */
     while (1) {
@@ -21694,67 +22571,67 @@
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = (((*__pyx_v_span.first).first < __pyx_v_ci) != 0);
       __pyx_t_9 = __pyx_t_10;
       __pyx_L9_bool_binop_done:;
       if (!__pyx_t_9) break;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":516
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":529
  *             while span.first != span.second and deref(span.first).first < ci:
  * 
  *                 irow[qi] = ci             # <<<<<<<<<<<<<<
  *                 icol[qi] = deref(span.first).first
  *                 qdata[qi] = deref(span.first).second
  */
       __pyx_t_4 = __pyx_v_qi;
       *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_irow.data + __pyx_t_4 * __pyx_v_irow.strides[0]) )) = __pyx_v_ci;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":517
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":530
  * 
  *                 irow[qi] = ci
  *                 icol[qi] = deref(span.first).first             # <<<<<<<<<<<<<<
  *                 qdata[qi] = deref(span.first).second
  * 
  */
       __pyx_t_11 = (*__pyx_v_span.first).first;
       __pyx_t_4 = __pyx_v_qi;
       *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_icol.data + __pyx_t_4 * __pyx_v_icol.strides[0]) )) = __pyx_t_11;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":518
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":531
  *                 irow[qi] = ci
  *                 icol[qi] = deref(span.first).first
  *                 qdata[qi] = deref(span.first).second             # <<<<<<<<<<<<<<
  * 
  *                 inc(span.first)
  */
       __pyx_t_12 = (*__pyx_v_span.first).second;
       __pyx_t_4 = __pyx_v_qi;
       *((__pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias *) ( /* dim=0 */ (__pyx_v_qdata.data + __pyx_t_4 * __pyx_v_qdata.strides[0]) )) = __pyx_t_12;
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":520
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":533
  *                 qdata[qi] = deref(span.first).second
  * 
  *                 inc(span.first)             # <<<<<<<<<<<<<<
  *                 qi += 1
  * 
  */
       (void)((++__pyx_v_span.first));
 
-      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":521
+      /* "dimod/discrete/cydiscrete_quadratic_model.pyx":534
  * 
  *                 inc(span.first)
  *                 qi += 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_qi = (__pyx_v_qi + 1);
     }
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":499
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":512
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cdef void _into_numpy_vectors(self, Unsigned[:] starts, Bias[:] ldata,             # <<<<<<<<<<<<<<
  *                                   Unsigned[:] irow, Unsigned[:] icol, Bias[:] qdata):
  *         # we don't do array length checking so be careful! This can segfault
  */
 
@@ -21762,15 +22639,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("dimod.discrete.cydiscrete_quadratic_model.cyDiscreteQuadraticModel._into_numpy_vectors", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "dimod/discrete/cydiscrete_quadratic_model.pyx":524
+/* "dimod/discrete/cydiscrete_quadratic_model.pyx":537
  * 
  * 
  *     def to_numpy_vectors(self):             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t num_variables = self.num_variables()
  */
 
@@ -21818,321 +22695,321 @@
   __Pyx_memviewslice __pyx_t_17 = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_t_18 = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("to_numpy_vectors", 0);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":526
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":539
  *     def to_numpy_vectors(self):
  * 
  *         cdef Py_ssize_t num_variables = self.num_variables()             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t num_cases = self.num_cases()
  *         cdef Py_ssize_t num_interactions = self.bqm_.num_interactions()
  */
   __pyx_v_num_variables = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_variables(__pyx_v_self, 0);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":527
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":540
  * 
  *         cdef Py_ssize_t num_variables = self.num_variables()
  *         cdef Py_ssize_t num_cases = self.num_cases()             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t num_interactions = self.bqm_.num_interactions()
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, NULL); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 527, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->num_cases(__pyx_v_self, 0, NULL); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(0, 540, __pyx_L1_error)
   __pyx_v_num_cases = __pyx_t_1;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":528
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":541
  *         cdef Py_ssize_t num_variables = self.num_variables()
  *         cdef Py_ssize_t num_cases = self.num_cases()
  *         cdef Py_ssize_t num_interactions = self.bqm_.num_interactions()             # <<<<<<<<<<<<<<
  * 
  *         # use the minimum sizes of the various index types. We combine for
  */
   try {
     __pyx_t_2 = __pyx_v_self->bqm_.num_interactions();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 528, __pyx_L1_error)
+    __PYX_ERR(0, 541, __pyx_L1_error)
   }
   __pyx_v_num_interactions = __pyx_t_2;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":533
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":546
  *         # variables and cases and exclude int8 to keep the total number of
  *         # cases down
  *         if num_cases < 1 << 16:             # <<<<<<<<<<<<<<
  *             index_dtype = np.uint16
  *         elif num_cases < 1 << 32:
  */
   __pyx_t_3 = ((__pyx_v_num_cases < 0x10000) != 0);
   if (__pyx_t_3) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":534
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":547
  *         # cases down
  *         if num_cases < 1 << 16:
  *             index_dtype = np.uint16             # <<<<<<<<<<<<<<
  *         elif num_cases < 1 << 32:
  *             index_dtype = np.uint32
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 534, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 547, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint16); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 534, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint16); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 547, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_index_dtype = __pyx_t_5;
     __pyx_t_5 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":533
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":546
  *         # variables and cases and exclude int8 to keep the total number of
  *         # cases down
  *         if num_cases < 1 << 16:             # <<<<<<<<<<<<<<
  *             index_dtype = np.uint16
  *         elif num_cases < 1 << 32:
  */
     goto __pyx_L3;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":535
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":548
  *         if num_cases < 1 << 16:
  *             index_dtype = np.uint16
  *         elif num_cases < 1 << 32:             # <<<<<<<<<<<<<<
  *             index_dtype = np.uint32
  *         else:
  */
-  __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_num_cases); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 535, __pyx_L1_error)
+  __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_num_cases); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_5, __pyx_int_4294967296, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 535, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_5, __pyx_int_4294967296, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 548, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 535, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 548, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_3) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":536
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":549
  *             index_dtype = np.uint16
  *         elif num_cases < 1 << 32:
  *             index_dtype = np.uint32             # <<<<<<<<<<<<<<
  *         else:
  *             index_dtype = np.uint64
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 536, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 549, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 536, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 549, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_index_dtype = __pyx_t_5;
     __pyx_t_5 = 0;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":535
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":548
  *         if num_cases < 1 << 16:
  *             index_dtype = np.uint16
  *         elif num_cases < 1 << 32:             # <<<<<<<<<<<<<<
  *             index_dtype = np.uint32
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":538
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":551
  *             index_dtype = np.uint32
  *         else:
  *             index_dtype = np.uint64             # <<<<<<<<<<<<<<
  * 
  *         starts = np.empty(num_variables, dtype=index_dtype)
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 538, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 551, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 538, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 551, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_index_dtype = __pyx_t_4;
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":540
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":553
  *             index_dtype = np.uint64
  * 
  *         starts = np.empty(num_variables, dtype=index_dtype)             # <<<<<<<<<<<<<<
  *         ldata = np.empty(num_cases, dtype=self.dtype)
  *         irow = np.empty(num_interactions, dtype=index_dtype)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 553, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 553, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_num_variables); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_num_variables); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 553, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 553, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 553, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_v_index_dtype) < 0) __PYX_ERR(0, 540, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 540, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_v_index_dtype) < 0) __PYX_ERR(0, 553, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 553, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_starts = __pyx_t_7;
   __pyx_t_7 = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":541
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":554
  * 
  *         starts = np.empty(num_variables, dtype=index_dtype)
  *         ldata = np.empty(num_cases, dtype=self.dtype)             # <<<<<<<<<<<<<<
  *         irow = np.empty(num_interactions, dtype=index_dtype)
  *         icol = np.empty(num_interactions, dtype=index_dtype)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 541, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 554, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 541, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 554, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_num_cases); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 541, __pyx_L1_error)
+  __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_num_cases); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 554, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 541, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 554, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7);
   __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 541, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 554, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_v_self->dtype) < 0) __PYX_ERR(0, 541, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 541, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_v_self->dtype) < 0) __PYX_ERR(0, 554, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 554, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_ldata = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":542
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":555
  *         starts = np.empty(num_variables, dtype=index_dtype)
  *         ldata = np.empty(num_cases, dtype=self.dtype)
  *         irow = np.empty(num_interactions, dtype=index_dtype)             # <<<<<<<<<<<<<<
  *         icol = np.empty(num_interactions, dtype=index_dtype)
  *         qdata = np.empty(num_interactions, dtype=self.dtype)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 542, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 555, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 542, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 555, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_num_interactions); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 542, __pyx_L1_error)
+  __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_num_interactions); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 555, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 542, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 555, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 542, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 555, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_v_index_dtype) < 0) __PYX_ERR(0, 542, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 542, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_v_index_dtype) < 0) __PYX_ERR(0, 555, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 555, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_irow = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":543
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":556
  *         ldata = np.empty(num_cases, dtype=self.dtype)
  *         irow = np.empty(num_interactions, dtype=index_dtype)
  *         icol = np.empty(num_interactions, dtype=index_dtype)             # <<<<<<<<<<<<<<
  *         qdata = np.empty(num_interactions, dtype=self.dtype)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 556, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 556, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_num_interactions); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_num_interactions); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 556, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 556, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 556, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_v_index_dtype) < 0) __PYX_ERR(0, 543, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 543, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_v_index_dtype) < 0) __PYX_ERR(0, 556, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 556, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_icol = __pyx_t_7;
   __pyx_t_7 = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":544
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":557
  *         irow = np.empty(num_interactions, dtype=index_dtype)
  *         icol = np.empty(num_interactions, dtype=index_dtype)
  *         qdata = np.empty(num_interactions, dtype=self.dtype)             # <<<<<<<<<<<<<<
  * 
  *         if index_dtype == np.uint16:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 544, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 544, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_num_interactions); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 544, __pyx_L1_error)
+  __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_num_interactions); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 544, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7);
   __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 544, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_v_self->dtype) < 0) __PYX_ERR(0, 544, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 544, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_v_self->dtype) < 0) __PYX_ERR(0, 557, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_qdata = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":546
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":559
  *         qdata = np.empty(num_interactions, dtype=self.dtype)
  * 
  *         if index_dtype == np.uint16:             # <<<<<<<<<<<<<<
  *             self._into_numpy_vectors[np.uint16_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.uint32:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 546, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 559, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint16); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 546, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint16); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 559, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyObject_RichCompare(__pyx_v_index_dtype, __pyx_t_7, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 546, __pyx_L1_error)
+  __pyx_t_5 = PyObject_RichCompare(__pyx_v_index_dtype, __pyx_t_7, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 559, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 546, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 559, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__pyx_t_3) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":547
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":560
  * 
  *         if index_dtype == np.uint16:
  *             self._into_numpy_vectors[np.uint16_t](starts, ldata, irow, icol, qdata)             # <<<<<<<<<<<<<<
  *         elif index_dtype == np.uint32:
  *             self._into_numpy_vectors[np.uint32_t](starts, ldata, irow, icol, qdata)
  */
-    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint16_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 547, __pyx_L1_error)
-    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 547, __pyx_L1_error)
-    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint16_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 547, __pyx_L1_error)
-    __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint16_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 547, __pyx_L1_error)
-    __pyx_t_12 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_12.memview)) __PYX_ERR(0, 547, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint16_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 560, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 560, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint16_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 560, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint16_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 560, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_12.memview)) __PYX_ERR(0, 560, __pyx_L1_error)
     ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->__pyx_fuse_1_into_numpy_vectors(__pyx_v_self, __pyx_t_8, __pyx_t_9, __pyx_t_10, __pyx_t_11, __pyx_t_12);
     __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
     __pyx_t_8.memview = NULL;
     __pyx_t_8.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
     __pyx_t_9.memview = NULL;
     __pyx_t_9.data = NULL;
@@ -22142,54 +23019,54 @@
     __PYX_XDEC_MEMVIEW(&__pyx_t_11, 1);
     __pyx_t_11.memview = NULL;
     __pyx_t_11.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_12, 1);
     __pyx_t_12.memview = NULL;
     __pyx_t_12.data = NULL;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":546
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":559
  *         qdata = np.empty(num_interactions, dtype=self.dtype)
  * 
  *         if index_dtype == np.uint16:             # <<<<<<<<<<<<<<
  *             self._into_numpy_vectors[np.uint16_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.uint32:
  */
     goto __pyx_L4;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":548
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":561
  *         if index_dtype == np.uint16:
  *             self._into_numpy_vectors[np.uint16_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.uint32:             # <<<<<<<<<<<<<<
  *             self._into_numpy_vectors[np.uint32_t](starts, ldata, irow, icol, qdata)
  *         else:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 548, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 548, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyObject_RichCompare(__pyx_v_index_dtype, __pyx_t_7, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 548, __pyx_L1_error)
+  __pyx_t_5 = PyObject_RichCompare(__pyx_v_index_dtype, __pyx_t_7, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 548, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__pyx_t_3) {
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":549
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":562
  *             self._into_numpy_vectors[np.uint16_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.uint32:
  *             self._into_numpy_vectors[np.uint32_t](starts, ldata, irow, icol, qdata)             # <<<<<<<<<<<<<<
  *         else:
  *             self._into_numpy_vectors[np.uint64_t](starts, ldata, irow, icol, qdata)
  */
-    __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 549, __pyx_L1_error)
-    __pyx_t_12 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_12.memview)) __PYX_ERR(0, 549, __pyx_L1_error)
-    __pyx_t_14 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_14.memview)) __PYX_ERR(0, 549, __pyx_L1_error)
-    __pyx_t_15 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_15.memview)) __PYX_ERR(0, 549, __pyx_L1_error)
-    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 549, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 562, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_12.memview)) __PYX_ERR(0, 562, __pyx_L1_error)
+    __pyx_t_14 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_14.memview)) __PYX_ERR(0, 562, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_15.memview)) __PYX_ERR(0, 562, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 562, __pyx_L1_error)
     ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->__pyx_fuse_2_into_numpy_vectors(__pyx_v_self, __pyx_t_13, __pyx_t_12, __pyx_t_14, __pyx_t_15, __pyx_t_9);
     __PYX_XDEC_MEMVIEW(&__pyx_t_13, 1);
     __pyx_t_13.memview = NULL;
     __pyx_t_13.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_12, 1);
     __pyx_t_12.memview = NULL;
     __pyx_t_12.data = NULL;
@@ -22199,37 +23076,37 @@
     __PYX_XDEC_MEMVIEW(&__pyx_t_15, 1);
     __pyx_t_15.memview = NULL;
     __pyx_t_15.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
     __pyx_t_9.memview = NULL;
     __pyx_t_9.data = NULL;
 
-    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":548
+    /* "dimod/discrete/cydiscrete_quadratic_model.pyx":561
  *         if index_dtype == np.uint16:
  *             self._into_numpy_vectors[np.uint16_t](starts, ldata, irow, icol, qdata)
  *         elif index_dtype == np.uint32:             # <<<<<<<<<<<<<<
  *             self._into_numpy_vectors[np.uint32_t](starts, ldata, irow, icol, qdata)
  *         else:
  */
     goto __pyx_L4;
   }
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":551
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":564
  *             self._into_numpy_vectors[np.uint32_t](starts, ldata, irow, icol, qdata)
  *         else:
  *             self._into_numpy_vectors[np.uint64_t](starts, ldata, irow, icol, qdata)             # <<<<<<<<<<<<<<
  * 
  *         return starts, ldata, (irow, icol, qdata)
  */
   /*else*/ {
-    __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 551, __pyx_L1_error)
-    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 551, __pyx_L1_error)
-    __pyx_t_17 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_17.memview)) __PYX_ERR(0, 551, __pyx_L1_error)
-    __pyx_t_18 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_18.memview)) __PYX_ERR(0, 551, __pyx_L1_error)
-    __pyx_t_12 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_12.memview)) __PYX_ERR(0, 551, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_v_starts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 564, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_ldata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 564, __pyx_L1_error)
+    __pyx_t_17 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_v_irow, PyBUF_WRITABLE); if (unlikely(!__pyx_t_17.memview)) __PYX_ERR(0, 564, __pyx_L1_error)
+    __pyx_t_18 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_v_icol, PyBUF_WRITABLE); if (unlikely(!__pyx_t_18.memview)) __PYX_ERR(0, 564, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5dimod_8discrete_26cydiscrete_quadratic_model_Bias(__pyx_v_qdata, PyBUF_WRITABLE); if (unlikely(!__pyx_t_12.memview)) __PYX_ERR(0, 564, __pyx_L1_error)
     ((struct __pyx_vtabstruct_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel *)__pyx_v_self->__pyx_vtab)->__pyx_fuse_3_into_numpy_vectors(__pyx_v_self, __pyx_t_16, __pyx_t_9, __pyx_t_17, __pyx_t_18, __pyx_t_12);
     __PYX_XDEC_MEMVIEW(&__pyx_t_16, 1);
     __pyx_t_16.memview = NULL;
     __pyx_t_16.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
     __pyx_t_9.memview = NULL;
     __pyx_t_9.data = NULL;
@@ -22241,47 +23118,47 @@
     __pyx_t_18.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_12, 1);
     __pyx_t_12.memview = NULL;
     __pyx_t_12.data = NULL;
   }
   __pyx_L4:;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":553
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":566
  *             self._into_numpy_vectors[np.uint64_t](starts, ldata, irow, icol, qdata)
  * 
  *         return starts, ldata, (irow, icol, qdata)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 553, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_irow);
   __Pyx_GIVEREF(__pyx_v_irow);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_irow);
   __Pyx_INCREF(__pyx_v_icol);
   __Pyx_GIVEREF(__pyx_v_icol);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_v_icol);
   __Pyx_INCREF(__pyx_v_qdata);
   __Pyx_GIVEREF(__pyx_v_qdata);
   PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_v_qdata);
-  __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 553, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(__pyx_v_starts);
   __Pyx_GIVEREF(__pyx_v_starts);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_starts);
   __Pyx_INCREF(__pyx_v_ldata);
   __Pyx_GIVEREF(__pyx_v_ldata);
   PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_v_ldata);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_t_5);
   __pyx_t_5 = 0;
   __pyx_r = __pyx_t_7;
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":524
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":537
  * 
  * 
  *     def to_numpy_vectors(self):             # <<<<<<<<<<<<<<
  * 
  *         cdef Py_ssize_t num_variables = self.num_variables()
  */
 
@@ -39224,15 +40101,15 @@
   {&__pyx_n_s_v, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 50, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 57, __pyx_L1_error)
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 400, __pyx_L1_error)
   __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(2, 855, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 1037, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 148, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 151, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 404, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 613, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 832, __pyx_L1_error)
@@ -39296,80 +40173,80 @@
  * 
  *         # if this was sorted (as it is by default from .to_numpy_vectors) then
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_inconsistent_lengths_for_irow_ic); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":225
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":238
  *             irow, icol, qdata = quadratic
  *         except ValueError:
  *             raise ValueError("quadratic should be a 3-tuple")             # <<<<<<<<<<<<<<
  * 
  *         # convert to numpy arrays, coercing the types into a simpler set
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_quadratic_should_be_a_3_tuple); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_quadratic_should_be_a_3_tuple); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":250
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":263
  *             obj._from_numpy_vectors[np.int64_t](starts, ldata, irow, icol, qdata)
  *         else:
  *             raise ValueError("starts, irow and icol must be integers")             # <<<<<<<<<<<<<<
  * 
  *         return obj
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_starts_irow_and_icol_must_be_int); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 250, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_starts_irow_and_icol_must_be_int); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 263, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":285
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":298
  *         # check that the interaction does in fact exist
  *         if u < 0 or u >= self.adj_.size():
  *             raise ValueError("unknown variable")             # <<<<<<<<<<<<<<
  *         if v < 0 or v >= self.adj_.size():
  *             raise ValueError("unknown variable")
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_unknown_variable); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_unknown_variable); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":291
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":304
  *         it = lower_bound(self.adj_[u].begin(), self.adj_[u].end(), v)
  *         if it == self.adj_[u].end() or deref(it) != v:
  *             raise ValueError("there is no interaction between given variables")             # <<<<<<<<<<<<<<
  * 
  *         cdef CaseIndex ci
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_there_is_no_interaction_between); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_there_is_no_interaction_between); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":387
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":400
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t set_linear(self, VarIndex v, Numeric[:] biases) except -1:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_No_matching_signature_found); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_No_matching_signature_found); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_Function_call_with_ambiguous_arg); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_Function_call_with_ambiguous_arg); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":406
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":419
  * 
  *         if case < 0:
  *             raise ValueError("case should be a positive integer")             # <<<<<<<<<<<<<<
  *         if case >= self.num_cases(v):
  *             raise ValueError("case {} is invalid, variable only supports {} "
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_case_should_be_a_positive_intege); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_case_should_be_a_positive_intege); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self.bqm_ cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -39653,25 +40530,25 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__41 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__41);
   __Pyx_GIVEREF(__pyx_tuple__41);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":387
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":400
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t set_linear(self, VarIndex v, Numeric[:] biases) except -1:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
-  __pyx_tuple__43 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_v, __pyx_n_s_biases); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_tuple__43 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_v, __pyx_n_s_biases); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__43);
   __Pyx_GIVEREF(__pyx_tuple__43);
-  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dimod_discrete_cydiscrete_quadra, __pyx_n_s_pyx_fuse_0set_linear, 387, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dimod_discrete_cydiscrete_quadra, __pyx_n_s_pyx_fuse_0set_linear, 400, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 400, __pyx_L1_error)
 
   /* "View.MemoryView":286
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
@@ -40185,104 +41062,104 @@
  * 
  */
   __pyx_t_2 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_2) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":218
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":231
  * 
  *     @classmethod
  *     def from_numpy_vectors(cls, starts, ldata, quadratic):             # <<<<<<<<<<<<<<
  * 
  *         cdef cyDiscreteQuadraticModel obj = cls()
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel, __pyx_n_s_from_numpy_vectors); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel, __pyx_n_s_from_numpy_vectors); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":217
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":230
  *             sort(self.adj_[v].begin(), self.adj_[v].end())
  * 
  *     @classmethod             # <<<<<<<<<<<<<<
  *     def from_numpy_vectors(cls, starts, ldata, quadratic):
  * 
  */
-  __pyx_t_1 = __Pyx_Method_ClassMethod(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 217, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Method_ClassMethod(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel->tp_dict, __pyx_n_s_from_numpy_vectors, __pyx_t_1) < 0) __PYX_ERR(0, 218, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel->tp_dict, __pyx_n_s_from_numpy_vectors, __pyx_t_1) < 0) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel);
 
-  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":387
+  /* "dimod/discrete/cydiscrete_quadratic_model.pyx":400
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef Py_ssize_t set_linear(self, VarIndex v, Numeric[:] biases) except -1:             # <<<<<<<<<<<<<<
  * 
  *         # self.num_cases checks that the variable is valid
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_0__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_37__pyx_fuse_0set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_0__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_37__pyx_fuse_0set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_uint8_t, __pyx_t_2) < 0) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_uint8_t, __pyx_t_2) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_1__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_39__pyx_fuse_1set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_2, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_1__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_39__pyx_fuse_1set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_2, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_uint16_t, __pyx_t_2) < 0) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_uint16_t, __pyx_t_2) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_2__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_41__pyx_fuse_2set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_3, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_2__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_41__pyx_fuse_2set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_3, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_uint32_t, __pyx_t_2) < 0) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_uint32_t, __pyx_t_2) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_3__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_43__pyx_fuse_3set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_4, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_3__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_43__pyx_fuse_3set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_4, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_uint64_t, __pyx_t_2) < 0) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_uint64_t, __pyx_t_2) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_4__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_45__pyx_fuse_4set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_5, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_4__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_45__pyx_fuse_4set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_5, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_int8_t, __pyx_t_2) < 0) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_int8_t, __pyx_t_2) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_5__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_47__pyx_fuse_5set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_6, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_5__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_47__pyx_fuse_5set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_6, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_int16_t, __pyx_t_2) < 0) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_int16_t, __pyx_t_2) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_6__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_49__pyx_fuse_6set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_7, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_6__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_49__pyx_fuse_6set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_7, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_int32_t, __pyx_t_2) < 0) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_int32_t, __pyx_t_2) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_7__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_51__pyx_fuse_7set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_8, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_7__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_51__pyx_fuse_7set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_8, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_int64_t, __pyx_t_2) < 0) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_int64_t, __pyx_t_2) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_8__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_53__pyx_fuse_8set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_9, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_8__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_53__pyx_fuse_8set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_9, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_float32_t, __pyx_t_2) < 0) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_float32_t, __pyx_t_2) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_9__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_55__pyx_fuse_9set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_10, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_9__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_55__pyx_fuse_9set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel___pyx_f_10, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_float64_t, __pyx_t_2) < 0) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_float64_t, __pyx_t_2) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_27set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel_set_lin, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_mdef_5dimod_8discrete_26cydiscrete_quadratic_model_24cyDiscreteQuadraticModel_27set_linear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyDiscreteQuadraticModel_set_lin, NULL, __pyx_n_s_dimod_discrete_cydiscrete_quadra_2, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
   ((__pyx_FusedFunctionObject *) __pyx_t_2)->__signatures__ = __pyx_t_1;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel->tp_dict, __pyx_n_s_set_linear, __pyx_t_2) < 0) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel->tp_dict, __pyx_n_s_set_linear, __pyx_t_2) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
   PyType_Modified(__pyx_ptype_5dimod_8discrete_26cydiscrete_quadratic_model_cyDiscreteQuadraticModel);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "dimod/discrete/cydiscrete_quadratic_model.pyx":1
  * # Copyright 2020 D-Wave Systems Inc.             # <<<<<<<<<<<<<<
  * #
  * #    Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `dimod-0.9.8/dimod/discrete/cydiscrete_quadratic_model.pxd` & `dimod-0.9.9/dimod/discrete/cydiscrete_quadratic_model.pxd`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/discrete/cydiscrete_quadratic_model.pyx` & `dimod-0.9.9/dimod/discrete/cydiscrete_quadratic_model.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,27 @@
                 is_sorted = False
                 break
 
             if irow[qi] == irow[qi + 1] and icol[qi] >= icol[qi+1]:
                 is_sorted = False
                 break
 
+
+        # reserve the memory for the vectors, this helps use less memory
+        # and speeds things up
+        cdef np.uint64_t[:] degrees = np.zeros(num_cases, dtype=np.uint64)
+
+        for qi in range(num_interactions):
+            degrees[irow[qi]] += 1
+            degrees[icol[qi]] += 1
+
+        for ci in range(num_cases):
+            self.bqm_.adj[ci].first.reserve(degrees[ci])
+
+        # set the quadratic
         if is_sorted:
             for qi in range(num_interactions):
                 # cython really has a hard time with push_back so we do this
                 # workaround
                 self.bqm_.adj[irow[qi]].first.resize(
                     self.bqm_.adj[irow[qi]].first.size() + 1)
                 self.bqm_.adj[irow[qi]].first.back().first = icol[qi]
```

### Comparing `dimod-0.9.8/dimod/discrete/discrete_quadratic_model.py` & `dimod-0.9.9/dimod/discrete/discrete_quadratic_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 import collections.abc as abc
 import io
 import json
 import tempfile
+import warnings
 
 from collections import namedtuple
 from operator import eq
 
 import numpy as np
 
 from dimod.discrete.cydiscrete_quadratic_model import cyDiscreteQuadraticModel
@@ -40,14 +41,33 @@
 # todo: update BinaryQuadraticModel.to_numpy_vectors to also use namedtuple
 DQMVectors = namedtuple(
     'DQMVectors', ['case_starts', 'linear_biases', 'quadratic', 'labels'])
 QuadraticVectors = namedtuple(
     'QuadraticVectors', ['row_indices', 'col_indices', 'biases'])
 
 
+# we want to use SpooledTemporaryFile but have it also include the methods
+# from io.IOBase. This is (probably) forthcoming in future python, see
+# https://bugs.python.org/issue35112
+if issubclass(tempfile.SpooledTemporaryFile, io.IOBase):
+    warnings.warn("Using deprecated SpooledTemporaryFile wrapper, "
+                  "functionality is now included in SpooledTemporaryFile",
+                  DeprecationWarning)
+
+
+class _SpooledTemporaryFile(tempfile.SpooledTemporaryFile, io.IOBase):
+    def seekable(self):
+        return self._file.seekable()
+
+    # This is not part of io.IOBase, but it is implemented in io.BytesIO
+    # and io.TextIOWrapper
+    def readinto(self, *args, **kwargs):
+        return self._file.readinto(*args, **kwargs)
+
+
 # this is the third(!) variables implementation in dimod. It differs from
 # dimod.variables in that it stores its labels sparsely. It has the same
 # behaviour as the cyBQM ones, except that it rolls the logic up into a
 # object. These need to be unified.
 class _Variables(abc.Sequence, abc.Set):
     def __init__(self):
         self._label_to_idx = dict()
@@ -331,28 +351,28 @@
     def from_file(cls, file_like):
         """Construct a DQM from a file-like object.
 
         The inverse of :meth:`~DiscreteQuadraticModel.to_file`.
         """
 
         if isinstance(file_like, (bytes, bytearray, memoryview)):
-            fp = _BytesIO(fp)
+            file_like = _BytesIO(file_like)
 
         magic = file_like.read(len(DQM_MAGIC_PREFIX))
         if magic != DQM_MAGIC_PREFIX:
             raise ValueError("unknown file type, expected magic string {} but "
                              "got {}".format(DQM_MAGIC_PREFIX, magic))
 
         version = tuple(file_like.read(2))
         if version[0] != 1:
             raise ValueError("cannot load a DQM serialized with version {!r}, "
                              "try upgrading your dimod version"
                              "".format(version))
 
-        header_len = np.frombuffer(file_like.read(4), '<u4')[0]
+        header_len = int(np.frombuffer(file_like.read(4), '<u4')[0])
 
         header_data = json.loads(file_like.read(header_len).decode('ascii'))
 
         obj = cls._from_file_numpy(file_like)
 
         if header_data['variables']:
             obj.variables = _Variables()
@@ -608,27 +628,27 @@
 
         """
         self._cydqm.set_quadratic_case(
             self.variables.index(u), u_case,
             self.variables.index(v), v_case,
             bias)
 
-    def _to_file_numpy(self, file, compressed):
+    def _to_file_numpy(self, file, compress):
         # the biases etc, saved using numpy
 
         # we'd like to just let numpy handle the header etc, but it doesn't
         # do a good job of cleaning up after itself in np.load, so we record
         # the section length ourselves
         file.write(DATA_MAGIC_PREFIX)
         file.write(b'    ')  # will be replaced by the length
         start = file.tell()
 
         vectors = self.to_numpy_vectors()
 
-        if compressed:
+        if compress:
             save = np.savez_compressed
         else:
             save = np.savez
 
         save(file,
              case_starts=vectors.case_starts,
              linear_biases=vectors.linear_biases,
@@ -639,35 +659,40 @@
 
         # record the length
         end = file.tell()
         file.seek(start-4)
         file.write(np.dtype('<u4').type(end - start).tobytes())
         file.seek(end)
 
-    def to_file(self, compressed=False, ignore_labels=False,
+    def to_file(self, compress=False, compressed=None, ignore_labels=False,
                 spool_size=int(1e9)):
         """Convert the DQM to a file-like object.
 
         Args:
-            compressed (bool, optional default=False):
+            compress (bool, optional default=False):
                 If True, most of the data will be compressed.
 
+            compressed (bool, optional default=None):
+                Deprecated; please use ``compress`` instead.
+
             ignore_labels (bool, optional, default=False):
                 Treat the DQM as unlabeled. This is useful for large DQMs to
                 save on space.
 
             spool_size (int, optional, default=int(1e9)):
                 Defines the `max_size` passed to the constructor of
                 :class:`tempfile.SpooledTemporaryFile`. Determines whether
                 the returned file-like's contents will be kept on disk or in
                 memory.
 
         Returns:
-            :class:`tempfile.SpooledTemporaryFile`: A file-like object
-            that can be used to construct a copy of the DQM.
+            A file-like object that can be used to construct a copy of the DQM.
+            The class is a thin wrapper of
+            :class:`tempfile.SpooledTemporaryFile` that also inherits from
+            `io.IOBase`.
 
         Format Specification (Version 1.0):
 
             This format is inspired by the `NPY format`_
 
             **Header**
 
@@ -721,15 +746,15 @@
         .. _NPY format: https://docs.scipy.org/doc/numpy/reference/generated/numpy.lib.format.html
 
         See Also:
             :meth:`DiscreteQuadraticModel.from_file`
 
         """
 
-        file = tempfile.SpooledTemporaryFile(max_size=spool_size)
+        file = _SpooledTemporaryFile(max_size=spool_size)
 
         # attach the header
         header_parts = [DQM_MAGIC_PREFIX,
                         VERSION,
                         bytes(4),  # placeholder for HEADER_LEN
                         ]
 
@@ -757,15 +782,25 @@
         HEADER_LEN = len(padding) + len(header_data)
         header_parts[2] = np.dtype('<u4').type(HEADER_LEN).tobytes()
 
         for part in header_parts:
             file.write(part)
 
         # the section containing most of the data, encoded with numpy
-        self._to_file_numpy(file, compressed)
+
+        if compressed is not None:
+            warning.warn(
+                "Argument 'compressed' is deprecated and in future will raise an "
+                "exception; please use 'compress' instead.",
+                DeprecationWarning, stacklevel=2
+                )
+            compress = compressed or compress
+
+
+        self._to_file_numpy(file, compress)
 
         if not index_labeled:
             file.write(VariablesSection(self.variables).dumps())
 
         file.seek(0)
 
         return file
```

### Comparing `dimod-0.9.8/dimod/exceptions.py` & `dimod-0.9.9/dimod/exceptions.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/generators/__init__.py` & `dimod-0.9.9/dimod/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/generators/anti_crossing.py` & `dimod-0.9.9/dimod/generators/anti_crossing.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/generators/chimera.py` & `dimod-0.9.9/dimod/generators/chimera.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/generators/constraints.py` & `dimod-0.9.9/dimod/generators/constraints.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/generators/fcl.py` & `dimod-0.9.9/dimod/generators/fcl.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/generators/random.py` & `dimod-0.9.9/dimod/generators/random.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/higherorder/__init__.py` & `dimod-0.9.9/dimod/higherorder/__init__.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/higherorder/polynomial.py` & `dimod-0.9.9/dimod/higherorder/polynomial.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/higherorder/utils.py` & `dimod-0.9.9/dimod/higherorder/utils.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/include/dimod/adjarraybqm.h` & `dimod-0.9.9/dimod/include/dimod/adjarraybqm.h`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/include/dimod/adjvectorbqm.h` & `dimod-0.9.9/dimod/include/dimod/adjvectorbqm.h`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/include/dimod/utils.h` & `dimod-0.9.9/dimod/include/dimod/utils.h`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/meta.py` & `dimod-0.9.9/dimod/meta.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/package_info.py` & `dimod-0.9.9/dimod/package_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 #
 # ================================================================================================
 
-__version__ = '0.9.8'
+__version__ = '0.9.9'
 __author__ = 'D-Wave Systems Inc.'
 __authoremail__ = 'acondello@dwavesys.com'
 __description__ = 'A shared API for binary quadratic model samplers.'
```

### Comparing `dimod-0.9.8/dimod/reference/__init__.py` & `dimod-0.9.9/dimod/reference/__init__.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/reference/composites/__init__.py` & `dimod-0.9.9/dimod/reference/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/reference/composites/clipcomposite.py` & `dimod-0.9.9/dimod/reference/composites/clipcomposite.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/reference/composites/connectedcomponent.py` & `dimod-0.9.9/dimod/reference/composites/connectedcomponent.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/reference/composites/fixedvariable.py` & `dimod-0.9.9/dimod/reference/composites/fixedvariable.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/reference/composites/higherordercomposites.py` & `dimod-0.9.9/dimod/reference/composites/higherordercomposites.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/reference/composites/roofduality.py` & `dimod-0.9.9/dimod/reference/composites/roofduality.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/reference/composites/scalecomposite.py` & `dimod-0.9.9/dimod/reference/composites/scalecomposite.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/reference/composites/spin_transform.py` & `dimod-0.9.9/dimod/reference/composites/spin_transform.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/reference/composites/structure.py` & `dimod-0.9.9/dimod/reference/composites/structure.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/reference/composites/tracking.py` & `dimod-0.9.9/dimod/reference/composites/tracking.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/reference/composites/truncatecomposite.py` & `dimod-0.9.9/dimod/reference/composites/truncatecomposite.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/reference/samplers/__init__.py` & `dimod-0.9.9/dimod/reference/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/reference/samplers/exact_solver.py` & `dimod-0.9.9/dimod/reference/samplers/exact_solver.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/reference/samplers/identity_sampler.py` & `dimod-0.9.9/dimod/reference/samplers/identity_sampler.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/reference/samplers/null_sampler.py` & `dimod-0.9.9/dimod/reference/samplers/null_sampler.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/reference/samplers/random_sampler.py` & `dimod-0.9.9/dimod/reference/samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/reference/samplers/simulated_annealing.py` & `dimod-0.9.9/dimod/reference/samplers/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/roof_duality/__init__.py` & `dimod-0.9.9/dimod/roof_duality/__init__.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/roof_duality/_fix_variables.cpp` & `dimod-0.9.9/dimod/roof_duality/_fix_variables.cpp`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/roof_duality/_fix_variables.pyx` & `dimod-0.9.9/dimod/roof_duality/_fix_variables.pyx`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/roof_duality/fix_variables.py` & `dimod-0.9.9/dimod/roof_duality/fix_variables.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/roof_duality/src/compressed_matrix.hpp` & `dimod-0.9.9/dimod/roof_duality/src/compressed_matrix.hpp`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/roof_duality/src/fix_variables.cpp` & `dimod-0.9.9/dimod/roof_duality/src/fix_variables.cpp`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/roof_duality/src/fix_variables.hpp` & `dimod-0.9.9/dimod/roof_duality/src/fix_variables.hpp`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/sampleset.py` & `dimod-0.9.9/dimod/sampleset.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/serialization/coo.py` & `dimod-0.9.9/dimod/serialization/coo.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/serialization/fileview.py` & `dimod-0.9.9/dimod/serialization/fileview.py`

 * *Files 0% similar despite different names*

```diff
@@ -629,15 +629,15 @@
             self._pos = max(0, self._pos + pos)
         elif whence == 2:
             self._pos = max(0, len(self._buffer) + pos)
         else:
             raise ValueError("unsupported whence value")
         return self._pos
 
-    def seekable():
+    def seekable(self):
         return True
 
 
 def load(fp, cls=None):
     """Load a binary quadratic model from a file.
 
     Args:
```

### Comparing `dimod-0.9.8/dimod/serialization/format.py` & `dimod-0.9.9/dimod/serialization/format.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/serialization/json.py` & `dimod-0.9.9/dimod/serialization/json.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/serialization/utils.py` & `dimod-0.9.9/dimod/serialization/utils.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/testing/__init__.py` & `dimod-0.9.9/dimod/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/testing/asserts.py` & `dimod-0.9.9/dimod/testing/asserts.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/testing/sampler.py` & `dimod-0.9.9/dimod/testing/sampler.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/traversal.py` & `dimod-0.9.9/dimod/traversal.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/utilities.py` & `dimod-0.9.9/dimod/utilities.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/variables.py` & `dimod-0.9.9/dimod/variables.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/vartypes.py` & `dimod-0.9.9/dimod/vartypes.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod/views/samples.py` & `dimod-0.9.9/dimod/views/samples.py`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/dimod.egg-info/PKG-INFO` & `dimod-0.9.9/dimod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimod
-Version: 0.9.8
+Version: 0.9.9
 Summary: A shared API for binary quadratic model samplers.
 Home-page: https://github.com/dwavesystems/dimod
 Author: D-Wave Systems Inc.
 Author-email: acondello@dwavesys.com
 License: Apache 2.0
 Download-URL: https://github.com/dwavesystems/dimod/releases
 Description: .. image:: https://img.shields.io/pypi/v/dimod.svg
```

### Comparing `dimod-0.9.8/dimod.egg-info/SOURCES.txt` & `dimod-0.9.9/dimod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dimod-0.9.8/setup.py` & `dimod-0.9.9/setup.py`

 * *Files identical despite different names*

