# Comparing `tmp/jVMC-1.2.1.tar.gz` & `tmp/jVMC-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jVMC-1.2.1.tar", last modified: Sun Jun 11 11:34:34 2023, max compression
+gzip compressed data, was "jVMC-1.2.2.tar", last modified: Wed Jun 14 08:48:26 2023, max compression
```

## Comparing `jVMC-1.2.1.tar` & `jVMC-1.2.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:34:34.149438 jVMC-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-11 11:34:23.000000 jVMC-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-11 11:34:34.149438 jVMC-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-11 11:34:23.000000 jVMC-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:34:34.145439 jVMC-1.2.1/jVMC/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/global_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/mpi_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:34:34.149438 jVMC-1.2.1/jVMC/nets/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/nets/activation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/nets/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/nets/ffn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/nets/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/nets/rbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/nets/rnn1d_general.py
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/nets/rnn2d_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/nets/sym_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/nets/two_nets_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:34:34.149438 jVMC-1.2.1/jVMC/operator/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11998 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/operator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/operator/branch_free.py
--rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/operator/povm.py
--rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:34:34.149438 jVMC-1.2.1/jVMC/util/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/util/minsr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/util/output_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/util/stepper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/util/symmetries.py
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/util/tdvp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18494 2023-06-11 11:34:23.000000 jVMC-1.2.1/jVMC/vqs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:34:34.145439 jVMC-1.2.1/jVMC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-11 11:34:34.000000 jVMC-1.2.1/jVMC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-11 11:34:34.000000 jVMC-1.2.1/jVMC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 11:34:34.000000 jVMC-1.2.1/jVMC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-11 11:34:34.000000 jVMC-1.2.1/jVMC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-11 11:34:34.000000 jVMC-1.2.1/jVMC.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 11:34:34.149438 jVMC-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-11 11:34:23.000000 jVMC-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:34:34.149438 jVMC-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 11:34:23.000000 jVMC-1.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-11 11:34:23.000000 jVMC-1.2.1/tests/minsr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-11 11:34:23.000000 jVMC-1.2.1/tests/mpi_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-11 11:34:23.000000 jVMC-1.2.1/tests/nets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-11 11:34:23.000000 jVMC-1.2.1/tests/operator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-06-11 11:34:23.000000 jVMC-1.2.1/tests/povm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-06-11 11:34:23.000000 jVMC-1.2.1/tests/sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-11 11:34:23.000000 jVMC-1.2.1/tests/stats_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-11 11:34:23.000000 jVMC-1.2.1/tests/stepper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-11 11:34:23.000000 jVMC-1.2.1/tests/symmetries_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-06-11 11:34:23.000000 jVMC-1.2.1/tests/tdvp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-06-11 11:34:23.000000 jVMC-1.2.1/tests/vqs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:48:26.857486 jVMC-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 08:48:12.000000 jVMC-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-14 08:48:26.857486 jVMC-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-14 08:48:12.000000 jVMC-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:48:26.853486 jVMC-1.2.2/jVMC/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/global_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/mpi_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:48:26.853486 jVMC-1.2.2/jVMC/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/activation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/ffn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/rbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/rnn1d_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/rnn2d_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/sym_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/two_nets_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:48:26.857486 jVMC-1.2.2/jVMC/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/operator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/operator/branch_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/operator/povm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:48:26.857486 jVMC-1.2.2/jVMC/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/util/minsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/util/output_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/util/stepper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/util/symmetries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/util/tdvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18494 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/vqs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:48:26.853486 jVMC-1.2.2/jVMC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-14 08:48:26.000000 jVMC-1.2.2/jVMC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-14 08:48:26.000000 jVMC-1.2.2/jVMC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:48:26.000000 jVMC-1.2.2/jVMC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-14 08:48:26.000000 jVMC-1.2.2/jVMC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 08:48:26.000000 jVMC-1.2.2/jVMC.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:48:26.857486 jVMC-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-14 08:48:12.000000 jVMC-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:48:26.857486 jVMC-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/minsr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/mpi_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/nets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/operator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/povm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/stats_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/stepper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/symmetries_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/tdvp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/vqs_test.py
```

### Comparing `jVMC-1.2.1/LICENSE` & `jVMC-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/PKG-INFO` & `jVMC-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jVMC
-Version: 1.2.1
+Version: 1.2.2
 Summary: jVMC: Versatile and performant variational Monte Carlo
 Home-page: https://jvmc.readthedocs.io/en/latest/#
 Author: Markus Schmitt, Moritz Reh
 Author-email: markus.schmitt@uni-koeln.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jVMC-1.2.1/README.md` & `jVMC-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/global_defs.py` & `jVMC-1.2.2/jVMC/global_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,15 @@
     myDevice = jax.devices()[0]
     print("WARNING: Could not assign devices based on MPI ranks. Assigning default device ", myDevice)
 
 myPmapDevices = jax.devices()  # [myDevice]
 myDeviceCount = len(myPmapDevices)
 pmap_for_my_devices = partial(jax.pmap, devices=myPmapDevices)
 
-pmapDevices = None
-def pmap_devices_updated():
+def pmap_devices_updated(pmapDevices):
     if collections.Counter(pmapDevices) == collections.Counter(myPmapDevices):
         return False
     return True
 
 
 def get_iterable(x):
     if isinstance(x, collections.abc.Iterable):
```

### Comparing `jVMC-1.2.1/jVMC/mpi_wrapper.py` & `jVMC-1.2.2/jVMC/mpi_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,33 +25,33 @@
 
 
 _sum_up_pmapd = None
 _sum_sq_pmapd = None
 mean_helper = None
 cov_helper = None
 
-
+mpiPmapDevices = None
 def jit_my_stuff():
     # This is a helper function to make sure that pmap'd functions work with the actual choice of devices
     # at all times.
 
     global _sum_up_pmapd
     global _sum_sq_pmapd
     global mean_helper
     global cov_helper
-    global pmapDevices
+    global mpiPmapDevices
 
-    if global_defs.pmap_devices_updated():
+    if global_defs.pmap_devices_updated(mpiPmapDevices):
         _sum_up_pmapd = global_defs.pmap_for_my_devices(lambda x: jax.lax.psum(jnp.sum(x, axis=0), 'i'), axis_name='i')
         # _sum_sq_pmapd = global_defs.pmap_for_my_devices(lambda data, mean, p: jax.lax.psum(jnp.conj(data - mean).dot(p[..., None] * (data - mean)), 'i'), axis_name='i', in_axes=(0, None, 0))
         _sum_sq_pmapd = global_defs.pmap_for_my_devices(lambda data, mean, p: jnp.einsum('ij, ij, i -> j', jnp.conj(data - mean[None, ...]), (data - mean[None, ...]), p), in_axes=(0, None, 0))
         mean_helper = global_defs.pmap_for_my_devices(lambda data, p: jnp.expand_dims(jnp.dot(p, data), axis=0), in_axes=(0, 0))
         cov_helper = global_defs.pmap_for_my_devices(_cov_helper, in_axes=(0, 0))
 
-        pmapDevices = global_defs.myPmapDevices
+        mpiPmapDevices = global_defs.myPmapDevices
 
 
 def distribute_sampling(numSamples, localDevices=None, numChainsPerDevice=1) -> int:
     """Distribute sampling tasks across processes and devices.
 
     For a desired total number of samples this function determines how many samples
     should be generated by each Monte Carlo chain.
```

### Comparing `jVMC-1.2.1/jVMC/nets/activation_functions.py` & `jVMC-1.2.2/jVMC/nets/activation_functions.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/nets/cnn.py` & `jVMC-1.2.2/jVMC/nets/cnn.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/nets/ffn.py` & `jVMC-1.2.2/jVMC/nets/ffn.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/nets/initializers.py` & `jVMC-1.2.2/jVMC/nets/initializers.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/nets/rbm.py` & `jVMC-1.2.2/jVMC/nets/rbm.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/nets/rnn1d_general.py` & `jVMC-1.2.2/jVMC/nets/rnn1d_general.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/nets/rnn2d_general.py` & `jVMC-1.2.2/jVMC/nets/rnn2d_general.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/nets/sym_wrapper.py` & `jVMC-1.2.2/jVMC/nets/sym_wrapper.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/nets/two_nets_wrapper.py` & `jVMC-1.2.2/jVMC/nets/two_nets_wrapper.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/operator/base.py` & `jVMC-1.2.2/jVMC/operator/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 
 import sys
 
 import jVMC.global_defs as global_defs
 
 opDtype = global_defs.tCpx
 
+def expand_batch(batch, batchSize):
+                outShape = list(batch.shape)
+                outShape[0] = batchSize
+                outp = jnp.zeros(tuple(outShape), dtype=batch.dtype)
+                return outp.at[:batch.shape[0]].set(batch)
 
 class Operator(metaclass=abc.ABCMeta):
     """This class defines an interface and provides functionality to compute operator matrix elements
 
     This is an abstract class. It provides the general interface to compute operator matrix elements, \
     but it lacks the implementation of operator definitions. Arbitrary operators can be constructed \
     as classes that inherit from ``Operator`` and implement the ``compile()`` method.
@@ -71,17 +76,21 @@
         self._alloc_Oloc_cpx_pmapd = global_defs.pmap_for_my_devices(lambda s: jnp.zeros(s.shape[0],
                                                                                          dtype=global_defs.tCpx))
         self._alloc_Oloc_real_pmapd = global_defs.pmap_for_my_devices(lambda s: jnp.zeros(s.shape[0],
                                                                                           dtype=global_defs.tReal))
         self._get_config_batch_pmapd = global_defs.pmap_for_my_devices(lambda d, startIdx, sliceSize: jax.lax.dynamic_slice_in_dim(d, startIdx, sliceSize), in_axes=(0, None, None), static_broadcasted_argnums=(2,))
         self._get_logPsi_batch_pmapd = global_defs.pmap_for_my_devices(lambda d, startIdx, sliceSize: jax.lax.dynamic_slice_in_dim(d, startIdx, sliceSize), in_axes=(0, None, None), static_broadcasted_argnums=(2,))
         self._insert_Oloc_batch_pmapd = global_defs.pmap_for_my_devices(
-            lambda dst, src, beg: jax.lax.dynamic_update_slice(dst, src, [beg, ]),
-            in_axes=(0, 0, None)
-        )
+                                            lambda dst, src, beg: jax.lax.dynamic_update_slice(dst, src, [beg, ]),
+                                            in_axes=(0, 0, None)
+                                        )
+        self._get_Oloc_slice_pmapd = global_defs.pmap_for_my_devices(
+                                            lambda d, startIdx, sliceSize: jax.lax.dynamic_slice_in_dim(d, startIdx, sliceSize), 
+                                            in_axes=(0, None, None), static_broadcasted_argnums=(2,)
+                                        )
 
     def _find_nonzero(self, m):
 
         choice = jnp.zeros(m.shape, dtype=np.int64) + m.shape[0] - 1
 
         def scan_fun(c, x):
             b = jnp.abs(x[0]) > 1e-6
@@ -244,32 +253,24 @@
                 else:
                     Oloc = self._alloc_Oloc_real_pmapd(samples)
 
             Oloc = self._insert_Oloc_batch_pmapd(Oloc, OlocBatch, b * batchSize)
         
         if remainder > 0:
 
-            def expand_batch(batch, batchSize):
-                outShape = list(batch.shape)
-                outShape[0] = batchSize
-                outp = jnp.zeros(tuple(outShape), dtype=batch.dtype)
-                return outp.at[:batch.shape[0]].set(batch)
             batch = self._get_config_batch_pmapd(samples, numBatches * batchSize, remainder)
             batch = global_defs.pmap_for_my_devices(expand_batch, static_broadcasted_argnums=(1,))(batch, batchSize)
             logPsiSbatch = self._get_logPsi_batch_pmapd(logPsiS, numBatches * batchSize, numSamples % batchSize)
             logPsiSbatch = global_defs.pmap_for_my_devices(expand_batch, static_broadcasted_argnums=(1,))(logPsiSbatch, batchSize)
 
             sp, _ = self.get_s_primes(batch, *args)
 
             OlocBatch = self.get_O_loc_unbatched(logPsiSbatch, psi(sp))
         
-            OlocBatch = global_defs.pmap_for_my_devices(
-                            lambda d, startIdx, sliceSize: jax.lax.dynamic_slice_in_dim(d, startIdx, sliceSize), 
-                            in_axes=(0, None, None), static_broadcasted_argnums=(2,)
-                        )(OlocBatch, 0, remainder)
+            OlocBatch = self._get_Oloc_slice_pmapd(OlocBatch, 0, remainder)
 
             Oloc = self._insert_Oloc_batch_pmapd(Oloc, OlocBatch, numBatches * batchSize)
 
         return Oloc
 
     @abc.abstractmethod
     def compile():
```

### Comparing `jVMC-1.2.1/jVMC/operator/branch_free.py` & `jVMC-1.2.2/jVMC/operator/branch_free.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/operator/povm.py` & `jVMC-1.2.2/jVMC/operator/povm.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/sampler.py` & `jVMC-1.2.2/jVMC/sampler.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/stats.py` & `jVMC-1.2.2/jVMC/stats.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,122 @@
 import jax
 import jax.numpy as jnp
 
 import jVMC
 import jVMC.mpi_wrapper as mpi
+import jVMC.global_defs as global_defs
 from jVMC.global_defs import pmap_for_my_devices
 
+_mean_helper = None
+_data_prep = None
+_covar_helper = None
+_covar_var_helper = None
+_covar_data_helper = None
+_trafo_helper_1 = None
+_trafo_helper_2 = None
+_select_helper = None
+_get_subset_helper = None
+_subset_mean_helper = None
+_subset_data_prep = None
+
+statsPmapDevices = None
+
+def jit_my_stuff():
+    # This is a helper function to make sure that pmap'd functions work with the actual choice of devices
+    # at all times.
+
+    global _mean_helper
+    global _covar_helper
+    global _covar_var_helper
+    global _covar_data_helper
+    global _trafo_helper_1
+    global _trafo_helper_2
+    global _select_helper
+    global _data_prep
+    global _get_subset_helper
+    global _subset_mean_helper
+    global _subset_data_prep
+
+    global statsPmapDevices
+
+    if jVMC.global_defs.pmap_devices_updated(statsPmapDevices):
+
+        statsPmapDevices = global_defs.myPmapDevices
+
+        _mean_helper = pmap_for_my_devices(lambda data, w: jnp.tensordot(w, data, axes=(0,0)), in_axes=(0, 0))
+        _data_prep = pmap_for_my_devices(lambda data, w, mean: jax.vmap(lambda d, w, m: jnp.sqrt(w) * (d - m), in_axes=(0,0,None))(data, w, mean), in_axes=(0, 0, None))
+        _covar_helper = pmap_for_my_devices(
+                                lambda data1, data2:
+                                    jnp.tensordot(
+                                        jnp.conj(data1),
+                                        data2, axes=(0,0)), 
+                                in_axes=(0, 0)
+                                )
+        _covar_var_helper = pmap_for_my_devices(
+                                    lambda data1, data2, w: 
+                                        jnp.sum(
+                                            jnp.abs( 
+                                                jax.vmap(lambda a,b: jnp.outer(a,b))(jnp.conj(data1), data2),
+                                            )**2 / w[...,None,None],
+                                            axis=0),
+                                    in_axes=(0, 0, 0)
+                                    )
+        _covar_data_helper = pmap_for_my_devices(lambda data1, data2, w: jax.vmap(lambda a,b,w: jnp.outer(a,b) / w)(jnp.conj(data1), data2, w), in_axes=(0, 0, 0))
+        _trafo_helper_1 = pmap_for_my_devices(
+                                lambda data, w, mean, f: f(
+                                    jax.vmap(lambda x,y: x/jnp.sqrt(y), in_axes=(0,0))(data, w) 
+                                    + mean
+                                    ), 
+                                in_axes=(0, 0, None), static_broadcasted_argnums=(3,))
+        _trafo_helper_2 = pmap_for_my_devices(
+                                lambda data, w, mean, v, f: 
+                                    jnp.matmul(v, 
+                                                f(
+                                                jax.vmap(lambda x,y: x/jnp.sqrt(y), in_axes=(0,0))(data, w) 
+                                                + mean
+                                                )
+                                    ), 
+                                in_axes=(0, 0, None, None), static_broadcasted_argnums=(4,))
+        _select_helper = pmap_for_my_devices( lambda ix,g: jax.vmap(lambda ix,g: g[ix], in_axes=(None, 0))(ix,g), in_axes=(None, 0) )
+        _get_subset_helper = pmap_for_my_devices(lambda x, ixs: x[slice(*ixs)], in_axes=(0,), static_broadcasted_argnums=(1,))
+        _subset_mean_helper = pmap_for_my_devices(lambda d, w, m: jnp.tensordot(jnp.sqrt(w), d, axes=(0,0)) + m, in_axes=(0,0,None))
+        _subset_data_prep = pmap_for_my_devices(jax.vmap(lambda d, w, m1, m2: d+jnp.sqrt(w)*(m1-m2), in_axes=(0,0,None,None)), in_axes=(0,0,None,None))
+
 
 class SampledObs():
     """This class implements the computation of statistics from Monte Carlo or exact samples.
 
     Initializer arguments:
         * ``observations``: Observations :math:`O_n` in the sample. The array must have a leading device \
             dimension plus a batch dimension.
         * ``weights``: Weights :math:`w_n` associated with observation :math:`O_n`.
     """
 
-    def __init__(self, observations, weights):
+    def __init__(self, observations=None, weights=None):
         """Initializes SampledObs class.
 
         Args:
             * ``observations``: Observations :math:`O_n` in the sample. The array must have a leading device \
                 dimension plus a batch dimension.
             * ``weights``: Weights :math:`w_n` associated with observation :math:`O_n`.
         """
 
-        self.jit_my_stuff()
-
-        if len(observations.shape) == 2:
-            observations = observations[...,None]
+        jit_my_stuff()
 
-        self._weights = weights
-        self._mean = mpi.global_sum( self._mean_helper(observations,self._weights)[None,...] )
-        #self._data = self._data_prep(observations, self._mean)
-        self._data = self._data_prep(observations, self._weights, self._mean)
+        if (observations is not None) and (weights is not None):
+            if len(observations.shape) == 2:
+                observations = observations[...,None]
+
+            self._weights = weights
+            self._mean = mpi.global_sum( _mean_helper(observations,self._weights)[None,...] )
+            self._data = _data_prep(observations, self._weights, self._mean)
+        else:
+            self._weights = weights
+            self._data = observations
+            self._mean = None
 
 
     def mean(self):
         """Returns the mean.
         """
 
         return self._mean
@@ -45,130 +125,103 @@
     def covar(self, other=None):
         """Returns the covariance.
 
         Args:
             * ``other`` [optional]: Another instance of `SampledObs`.
         """
 
-        self.jit_my_stuff()
-
         if other is None:
             other = self
         
-        #return mpi.global_sum( self._covar_helper(self._data, other._data, self._weights)[None,...] )
-        return mpi.global_sum( self._covar_helper(self._data, other._data)[None,...] )
+        return mpi.global_sum( _covar_helper(self._data, other._data)[None,...] )
     
 
     def var(self):
         """Returns the variance.
         """
 
-        #return mpi.global_sum( self._mean_helper(jnp.abs(self._data)**2, self._weights)[None,...] )
         return mpi.global_sum( jnp.abs(self._data)**2 )
     
 
     def covar_data(self, other=None):
         """Returns the covariance.
 
         Args:
             * ``other`` [optional]: Another instance of `SampledObs`.
         """
 
-        self.jit_my_stuff()
-
         if other is None:
             other = self
 
-        #return SampledObs( self._covar_data_helper(self._data, other._data), self._weights )
-        return SampledObs( self._covar_data_helper(self._data, other._data, self._weights), self._weights )
+        return SampledObs( _covar_data_helper(self._data, other._data, self._weights), self._weights )
     
 
     def covar_var(self, other=None):
         """Returns the variance of the covariance.
 
         Args:
             * ``other`` [optional]: Another instance of `SampledObs`.
         """
 
-        self.jit_my_stuff()
-
         if other is None:
             other = self
         
-        return mpi.global_sum( self._covar_var_helper(self._data, other._data, self._weights)[None,...] ) \
+        return mpi.global_sum( _covar_var_helper(self._data, other._data, self._weights)[None,...] ) \
                     - jnp.abs(self.covar(other))**2
 
 
-    def transform(self, fun=lambda x: x):
+    def transform(self, nonLinearFun=lambda x: x, linearFun=None):
         """Returns a `SampledObs` for the transformed data.
 
         Args:
             * ``fun``: A function.
         """
 
-        #return SampledObs( self._trafo_helper(self._data, self._mean, fun), self._weights )
-        return SampledObs( self._trafo_helper(self._data, self._weights, self._mean, fun), self._weights )
+        if linearFun is None:
+            return SampledObs( _trafo_helper_1(self._data, self._weights, self._mean, nonLinearFun), self._weights )
+        
+        return SampledObs( _trafo_helper_2(self._data, self._weights, self._mean, linearFun, nonLinearFun), self._weights )
+
+
+    def select(self, ixs):
+        """Returns a `SampledObs` for the data selection indicated by the given indices.
+
+        Args:
+            * ``ixs``: Indices of selected data.
+        """
+
+        newObs = SampledObs()
+        newObs._data = _select_helper(ixs, self._data)
+        newObs._mean = self._mean[ixs]
+        newObs._weights = self._weights
+
+        return newObs
+    
     
+    def subset(self, start=None, end=None, step=None):
+        """Returns a `SampledObs` for a subset of the data.
+
+        Args:
+            * ``start``: Start sample index for subset selection
+            * ``end``: End sample index for subset selection
+            * ``step``: Sample index step for subset selection
+        """ 
+
+        newObs = SampledObs()
+        newObs._weights = _get_subset_helper(self._weights, (start, end, step))
+        normalization = mpi.global_sum(newObs._weights)
+        newObs._data = _get_subset_helper(self._data, (start, end, step))
+        newObs._weights = newObs._weights / normalization
+        newObs._data = newObs._data / jnp.sqrt(normalization)
+        newObs._mean = mpi.global_sum( _subset_mean_helper(newObs._data, newObs._weights, self._mean)[None,...] ) 
+        newObs._data = _subset_data_prep(newObs._data, newObs._weights, self._mean, newObs._mean)
+
+        return newObs
+
 
     def tangent_kernel(self):
 
         all_data = mpi.gather(self._data)
         
         return jnp.matmul(all_data, jnp.conj(jnp.transpose(all_data)))
 
 
-    def jit_my_stuff(self):
-        # This is a helper function to make sure that pmap'd functions work with the actual choice of devices
-        # at all times.
-
-        if jVMC.global_defs.pmap_devices_updated():
-            self._mean_helper = pmap_for_my_devices(lambda data, w: jnp.tensordot(w, data, axes=(0,0)), in_axes=(0, 0))
-            #self._data_prep = pmap_for_my_devices(lambda data, mean: data - mean, in_axes=(0, None))
-            self._data_prep = pmap_for_my_devices(lambda data, w, mean: jax.vmap(lambda d, w, m: jnp.sqrt(w) * (d - m), in_axes=(0,0,None))(data, w, mean), in_axes=(0, 0, None))
-            # self._covar_helper = pmap_for_my_devices(
-            #                         lambda data1, data2, w:
-            #                             jnp.tensordot(
-            #                                 jnp.conj(
-            #                                     jax.vmap(lambda a,b: a*b, in_axes=(0,0))(w, data1)
-            #                                     ),
-            #                                 data2, axes=(0,0)), 
-            #                         in_axes=(0, 0, 0)
-            #                         )
-            self._covar_helper = pmap_for_my_devices(
-                                    lambda data1, data2:
-                                        jnp.tensordot(
-                                            jnp.conj(data1),
-                                            data2, axes=(0,0)), 
-                                    in_axes=(0, 0)
-                                    )
-            # self._covar_var_helper = pmap_for_my_devices(
-            #                             lambda data1, data2, w: 
-            #                                 jnp.sum(
-            #                                     w[...,None,None] * 
-            #                                     jnp.abs( 
-            #                                         jax.vmap(lambda a,b: jnp.outer(a,b))(jnp.conj(data1), data2),
-            #                                     )**2,
-            #                                     axis=0),
-            #                             in_axes=(0, 0, 0)
-            #                             )
-            self._covar_var_helper = pmap_for_my_devices(
-                                        lambda data1, data2, w: 
-                                            jnp.sum(
-                                                jnp.abs( 
-                                                    jax.vmap(lambda a,b: jnp.outer(a,b))(jnp.conj(data1), data2),
-                                                )**2 / w[...,None,None],
-                                                axis=0),
-                                        in_axes=(0, 0, 0)
-                                        )
-            self._covar_data_helper = pmap_for_my_devices(lambda data1, data2, w: jax.vmap(lambda a,b,w: jnp.outer(a,b) / w)(jnp.conj(data1), data2, w), in_axes=(0, 0, 0))
-            #self._trafo_helper = pmap_for_my_devices(lambda data, mean, f: f(data + mean), in_axes=(0, None), static_broadcasted_argnums=(2,))
-            self._trafo_helper = pmap_for_my_devices(
-                                    lambda data, w, mean, f: f(
-                                        jax.vmap(lambda x,y: x/jnp.sqrt(y), in_axes=(0,0))(data, w) 
-                                        + mean
-                                        ), 
-                                    in_axes=(0, 0, None), static_broadcasted_argnums=(3,))
-
-
-        
-
-
```

### Comparing `jVMC-1.2.1/jVMC/util/minsr.py` & `jVMC-1.2.2/jVMC/util/minsr.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/util/output_manager.py` & `jVMC-1.2.2/jVMC/util/output_manager.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/util/stepper.py` & `jVMC-1.2.2/jVMC/util/stepper.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/util/symmetries.py` & `jVMC-1.2.2/jVMC/util/symmetries.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/util/tdvp.py` & `jVMC-1.2.2/jVMC/util/tdvp.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,22 +4,27 @@
 
 import jVMC
 import jVMC.mpi_wrapper as mpi
 import jVMC.global_defs as global_defs
 from jVMC.stats import SampledObs
 
 import warnings
+from functools import partial
 
 
 def realFun(x):
     return jnp.real(x)
 
 
 def imagFun(x):
     return 0.5 * (x - jnp.conj(x))
+                        
+
+def transform_helper(x, rhsPrefactor, makeReal):
+    return makeReal((-rhsPrefactor) * x)
 
 
 class TDVP:
     """ This class provides functionality to solve a time-dependent variational principle (TDVP).
 
     With the force vector
 
@@ -81,14 +86,15 @@
         self.diagonalizeOnDevice = diagonalizeOnDevice
 
         self.metaData = None
 
         self.makeReal = realFun
         if makeReal == 'imag':
             self.makeReal = imagFun
+        self.trafo_helper = partial(transform_helper, rhsPrefactor=rhsPrefactor, makeReal=self.makeReal)
 
         # pmap'd member functions
         self.makeReal_pmapd = global_defs.pmap_for_my_devices(jax.vmap(lambda x: self.makeReal(x)))
 
     def set_diagonal_shift(self, delta):
         self.diagonalShift = delta
 
@@ -165,18 +171,16 @@
             self.V = jnp.array(tmpV)
 
         self.VtF = jnp.dot(jnp.transpose(jnp.conj(self.V)), F)
 
     def _get_snr(self, Eloc, gradients):
 
         EO = gradients.covar_data(Eloc).transform(
-                        fun=lambda x: jnp.matmul(
-                                        jnp.transpose(jnp.conj(self.V)), 
-                                        jVMC.util.imagFun((-self.rhsPrefactor) * x)
-                                        )
+                        linearFun = jnp.transpose(jnp.conj(self.V)),
+                        nonLinearFun=self.trafo_helper
                     )
         self.rhoVar = EO.var().ravel()
 
         self.snr = jnp.sqrt(jnp.abs(mpi.globNumSamples * (jnp.conj(self.VtF) * self.VtF) / self.rhoVar)).ravel()
 
     def solve(self, Eloc, gradients):
         # Get TDVP equation from MC data
@@ -197,42 +201,14 @@
             # Construct a soft cutoff based on the SNR
             regularizer *= 1. / (1. + (self.snrTol / self.snr)**6)
 
         update = jnp.real(jnp.dot(self.V, (self.invEv * regularizer * self.VtF)))
 
         return update, jnp.linalg.norm(self.S.dot(update) - F) / jnp.linalg.norm(F)
 
-    def solve_minSR(self, eloc, gradients, p=None, r_pinv=1e-8):
-        """
-        Uses the techique proposed in arXiv:2302.01941 to compute the updates.
-        Efficient only if number of samples << number of parameters.
-        """
-
-        # Collect all gradients & local energies
-        def soft_cutoff(eigvals):
-            return 1 / (eigvals * (1 + (r_pinv * jnp.max(eigvals) / eigvals)**6))
-
-        def hard_cutoff(eigvals):
-            return jnp.where(eigvals / jnp.max(eigvals) > r_pinv, 1 / eigvals, 0)
-
-        eloc = mpi.gather(eloc).reshape((-1,))
-        gradients = mpi.gather(gradients).reshape((-1, gradients.shape[-1]))
-        n_samples = eloc.shape[0]
-
-        eloc_bar = (eloc - jnp.mean(eloc)) / jnp.sqrt(n_samples)
-        gradients_bar = (gradients - jnp.mean(gradients, axis=0)) / jnp.sqrt(n_samples)
-
-        T = gradients_bar @ gradients_bar.conj().T
-        eigvals, eigvecs = jnp.linalg.eigh(T)
-        inv_eigvals = hard_cutoff(eigvals)
-        T_inv = eigvecs @ jnp.diag(inv_eigvals) @ eigvecs.conj().T
-        self.update = - self.rhsPrefactor * gradients_bar.conj().T @ T_inv @ eloc_bar
-
-        return self.update, None
-
     def S_dot(self, v):
 
         return jnp.dot(self.S0, v)
 
     def __call__(self, netParameters, t, *, psi, hamiltonian, **rhsArgs):
         """ For given network parameters this function solves the TDVP equation.
 
@@ -317,24 +293,26 @@
                     "tdvp_residual": solverResidual,
                     "SNR": self.snr, 
                     "spectrum": self.ev,
                 }
 
                 if self.crossValidation:
 
-                    if isinstance(self.sampler, jVMC.sampler.ExactSampler):
-                        update_1, _ = self.solve(Eloc[:, 0::2], sampleGradients[:, 0::2], p[:, 0::2])
-                        S2, F2, _ = self.get_tdvp_equation(Eloc[:, 1::2], sampleGradients[:, 1::2], p[:, 1::2])
-                    else:
-                        update_1, _ = self.solve(Eloc[:, 0::2], sampleGradients[:, 0::2])
-                        S2, F2, _ = self.get_tdvp_equation(Eloc[:, 1::2], sampleGradients[:, 1::2])
+                    Eloc1 = Eloc.subset(start=0, step=2)
+                    sampleGradients1 = sampleGradients.subset(start=0, step=2)
+                    Eloc2 = Eloc.subset(start=1, step=2)
+                    sampleGradients2 = sampleGradients.subset(start=1, step=2)
+                    update_1, _ = self.solve(Eloc1, sampleGradients1)
+                    S2, F2 = self.get_tdvp_equation(Eloc2, sampleGradients2)
 
                     validation_tdvpErr = self._get_tdvp_error(update_1)
-                    update, solverResidual = self.solve(Eloc, sampleGradients, p)
+                    update, solverResidual = self.solve(Eloc, sampleGradients)
                     validation_residual = (jnp.linalg.norm(S2.dot(update_1) - F2) / jnp.linalg.norm(F2)) / solverResidual
 
                     self.crossValidationFactor_residual = validation_residual
                     self.crossValidationFactor_tdvpErr = validation_tdvpErr / self.metaData["tdvp_error"]
+                    self.metaData["tdvp_residual_cross_validation_ratio"] = self.crossValidationFactor_residual
+                    self.metaData["tdvp_error_cross_validation_ratio"] = self.crossValidationFactor_tdvpErr
 
-                    self.S, _, _ = self.get_tdvp_equation(Eloc, sampleGradients, p)
+                    self.S, _ = self.get_tdvp_equation(Eloc, sampleGradients)
 
         return update
```

### Comparing `jVMC-1.2.1/jVMC/util/util.py` & `jVMC-1.2.2/jVMC/util/util.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC/vqs.py` & `jVMC-1.2.2/jVMC/vqs.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/jVMC.egg-info/PKG-INFO` & `jVMC-1.2.2/jVMC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jVMC
-Version: 1.2.1
+Version: 1.2.2
 Summary: jVMC: Versatile and performant variational Monte Carlo
 Home-page: https://jvmc.readthedocs.io/en/latest/#
 Author: Markus Schmitt, Moritz Reh
 Author-email: markus.schmitt@uni-koeln.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jVMC-1.2.1/jVMC.egg-info/SOURCES.txt` & `jVMC-1.2.2/jVMC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/setup.py` & `jVMC-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/tests/minsr_test.py` & `jVMC-1.2.2/tests/minsr_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/tests/mpi_wrapper_test.py` & `jVMC-1.2.2/tests/mpi_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/tests/nets_test.py` & `jVMC-1.2.2/tests/nets_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/tests/operator_test.py` & `jVMC-1.2.2/tests/operator_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/tests/povm_test.py` & `jVMC-1.2.2/tests/povm_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/tests/sampler_test.py` & `jVMC-1.2.2/tests/sampler_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/tests/stats_test.py` & `jVMC-1.2.2/tests/stats_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/tests/stepper_test.py` & `jVMC-1.2.2/tests/stepper_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/tests/symmetries_test.py` & `jVMC-1.2.2/tests/symmetries_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.1/tests/tdvp_test.py` & `jVMC-1.2.2/tests/tdvp_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from jVMC.vqs import NQS
 import jVMC.operator as op
 import jVMC.sampler as sampler
 import jVMC.mpi_wrapper as mpi
 
 from jVMC.util import measure, ground_state_search
 
+from functools import partial
+
 
 class TestGsSearch(unittest.TestCase):
     def test_gs_search_cpx(self):
         L = 4
         J = -1.0
         hxs = [-1.3, -0.3]
 
@@ -158,15 +160,15 @@
 
         # Set up exact sampler
         MCsampler = sampler.MCSampler(psi, (L,), jax.random.PRNGKey(0), numSamples=50000, updateProposer=sampler.propose_spin_flip, mu=1, numChains=500)
 
         # Set up adaptive time stepper
         stepper = jVMCstepper.AdaptiveHeun(timeStep=1e-3, tol=1e-4)
 
-        tdvpEquation = jVMC.util.TDVP(MCsampler, snrTol=1, svdTol=1e-8, rhsPrefactor=1.j, diagonalShift=0., makeReal='imag')
+        tdvpEquation = jVMC.util.TDVP(MCsampler, snrTol=1, pinvTol=1e-8, rhsPrefactor=1.j, diagonalShift=0., makeReal='imag', crossValidation=True)
 
         t = 0
         obs = []
         times = []
         times.append(t)
         newMeas = measure({'E': hamiltonian, 'ZZ': ZZ}, psi, MCsampler)
         obs.append([newMeas['E']['mean'], newMeas['ZZ']['mean']])
@@ -251,15 +253,16 @@
         Eloc_old = subtract_helper_Eloc(Eloc_old, mpi.global_mean(Eloc_old, p))
         sampleGradients_old = subtract_helper_grad(sampleGradients_old, mpi.global_mean(sampleGradients_old, p))
         EOdata = get_EO(-1., p, Eloc_old, sampleGradients_old) * mpi.globNumSamples
         EOdata = transform_EO(jVMC.util.imagFun(EOdata), V)
         EOdata.block_until_ready()
         rhoVar_old = mpi.global_variance(EOdata, jnp.ones(EOdata.shape[:2]) / mpi.globNumSamples)
 
-        EO = sampleGradients.covar_data(Eloc).transform(fun=lambda x: jnp.matmul(jnp.transpose(jnp.conj(V)), jVMC.util.imagFun(x)))
+        EO = sampleGradients.covar_data(Eloc).transform(linearFun = jnp.transpose(jnp.conj(V)),
+                                                        nonLinearFun=lambda x: jVMC.util.imagFun(x))
         rhoVar_new = EO.var().ravel()
 
         self.assertTrue( jnp.allclose(rhoVar_old, rhoVar_new) )
 
 
 
 if __name__ == "__main__":
```

### Comparing `jVMC-1.2.1/tests/vqs_test.py` & `jVMC-1.2.2/tests/vqs_test.py`

 * *Files identical despite different names*

