# Comparing `tmp/raft-dask-cu12-23.6.0.tar.gz` & `tmp/raft-dask-cu12-23.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raft-dask-cu12-23.6.0.tar", last modified: Mon Jun 12 22:48:05 2023, max compression
+gzip compressed data, was "raft-dask-cu12-23.6.1.tar", last modified: Wed Jun 14 14:27:58 2023, max compression
```

## Comparing `raft-dask-cu12-23.6.0.tar` & `raft-dask-cu12-23.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-12 22:48:05.812189 raft-dask-cu12-23.6.0/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      446 2023-06-12 22:48:05.000000 raft-dask-cu12-23.6.0/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-08 22:35:55.000000 raft-dask-cu12-23.6.0/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       14 2023-06-12 22:48:05.000000 raft-dask-cu12-23.6.0/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-06-12 22:48:05.808189 raft-dask-cu12-23.6.0/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      247 2023-06-12 22:48:05.000000 raft-dask-cu12-23.6.0/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-12 22:48:05.808189 raft-dask-cu12-23.6.0/raft_dask_cu12.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-06-12 22:48:05.000000 raft-dask-cu12-23.6.0/raft_dask_cu12.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      205 2023-06-12 22:48:05.000000 raft-dask-cu12-23.6.0/raft_dask_cu12.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-12 22:48:05.000000 raft-dask-cu12-23.6.0/raft_dask_cu12.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-12 22:48:05.000000 raft-dask-cu12-23.6.0/raft_dask_cu12.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-12 22:48:05.812189 raft-dask-cu12-23.6.0/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-08 22:35:55.000000 raft-dask-cu12-23.6.0/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-14 14:27:58.340673 raft-dask-cu12-23.6.1/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      446 2023-06-14 14:27:58.000000 raft-dask-cu12-23.6.1/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 04:13:36.000000 raft-dask-cu12-23.6.1/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       14 2023-06-14 14:27:58.000000 raft-dask-cu12-23.6.1/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-06-14 14:27:58.340673 raft-dask-cu12-23.6.1/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      247 2023-06-14 14:27:58.000000 raft-dask-cu12-23.6.1/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-14 14:27:58.340673 raft-dask-cu12-23.6.1/raft_dask_cu12.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-06-14 14:27:58.000000 raft-dask-cu12-23.6.1/raft_dask_cu12.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      205 2023-06-14 14:27:58.000000 raft-dask-cu12-23.6.1/raft_dask_cu12.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-14 14:27:58.000000 raft-dask-cu12-23.6.1/raft_dask_cu12.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-14 14:27:58.000000 raft-dask-cu12-23.6.1/raft_dask_cu12.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-14 14:27:58.340673 raft-dask-cu12-23.6.1/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 04:13:36.000000 raft-dask-cu12-23.6.1/setup.py
```

### Comparing `raft-dask-cu12-23.6.0/LICENSE.md` & `raft-dask-cu12-23.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `raft-dask-cu12-23.6.0/PKG-INFO` & `raft-dask-cu12-23.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raft-dask-cu12
-Version: 23.6.0
+Version: 23.6.1
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `raft-dask-cu12-23.6.0/raft_dask_cu12.egg-info/PKG-INFO` & `raft-dask-cu12-23.6.1/raft_dask_cu12.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raft-dask-cu12
-Version: 23.6.0
+Version: 23.6.1
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `raft-dask-cu12-23.6.0/setup.py` & `raft-dask-cu12-23.6.1/setup.py`

 * *Files identical despite different names*

