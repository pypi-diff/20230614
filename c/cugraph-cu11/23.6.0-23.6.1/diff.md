# Comparing `tmp/cugraph-cu11-23.6.0.tar.gz` & `tmp/cugraph-cu11-23.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cugraph-cu11-23.6.0.tar", last modified: Fri Jun  9 15:17:28 2023, max compression
+gzip compressed data, was "cugraph-cu11-23.6.1.tar", last modified: Fri Jun  9 19:02:51 2023, max compression
```

## Comparing `cugraph-cu11-23.6.0.tar` & `cugraph-cu11-23.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-09 15:17:28.082435 cugraph-cu11-23.6.0/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      444 2023-06-09 15:17:28.000000 cugraph-cu11-23.6.0/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-08 22:12:21.000000 cugraph-cu11-23.6.0/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       12 2023-06-09 15:17:28.000000 cugraph-cu11-23.6.0/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1596 2023-06-09 15:17:28.082435 cugraph-cu11-23.6.0/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      241 2023-06-09 15:17:28.000000 cugraph-cu11-23.6.0/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-09 15:17:28.081435 cugraph-cu11-23.6.0/cugraph_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1596 2023-06-09 15:17:28.000000 cugraph-cu11-23.6.0/cugraph_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      197 2023-06-09 15:17:28.000000 cugraph-cu11-23.6.0/cugraph_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-09 15:17:28.000000 cugraph-cu11-23.6.0/cugraph_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-09 15:17:28.000000 cugraph-cu11-23.6.0/cugraph_cu11.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-09 15:17:28.082435 cugraph-cu11-23.6.0/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-08 22:12:21.000000 cugraph-cu11-23.6.0/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-09 19:02:51.660153 cugraph-cu11-23.6.1/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      444 2023-06-09 19:02:51.000000 cugraph-cu11-23.6.1/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-08 22:12:21.000000 cugraph-cu11-23.6.1/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       12 2023-06-09 19:02:51.000000 cugraph-cu11-23.6.1/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1596 2023-06-09 19:02:51.660153 cugraph-cu11-23.6.1/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      241 2023-06-09 19:02:51.000000 cugraph-cu11-23.6.1/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-09 19:02:51.660153 cugraph-cu11-23.6.1/cugraph_cu11.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1596 2023-06-09 19:02:51.000000 cugraph-cu11-23.6.1/cugraph_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      197 2023-06-09 19:02:51.000000 cugraph-cu11-23.6.1/cugraph_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-09 19:02:51.000000 cugraph-cu11-23.6.1/cugraph_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-09 19:02:51.000000 cugraph-cu11-23.6.1/cugraph_cu11.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-09 19:02:51.660153 cugraph-cu11-23.6.1/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-08 22:12:21.000000 cugraph-cu11-23.6.1/setup.py
```

### Comparing `cugraph-cu11-23.6.0/LICENSE.md` & `cugraph-cu11-23.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cugraph-cu11-23.6.0/PKG-INFO` & `cugraph-cu11-23.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cugraph-cu11
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

### Comparing `cugraph-cu11-23.6.0/cugraph_cu11.egg-info/PKG-INFO` & `cugraph-cu11-23.6.1/cugraph_cu11.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cugraph-cu11
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

### Comparing `cugraph-cu11-23.6.0/setup.py` & `cugraph-cu11-23.6.1/setup.py`

 * *Files identical despite different names*

