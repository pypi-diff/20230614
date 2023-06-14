# Comparing `tmp/pylibcugraph-cu12-23.6.1.tar.gz` & `tmp/pylibcugraph-cu12-23.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibcugraph-cu12-23.6.1.tar", last modified: Mon Jun 12 22:37:14 2023, max compression
+gzip compressed data, was "pylibcugraph-cu12-23.6.2.tar", last modified: Wed Jun 14 14:12:39 2023, max compression
```

## Comparing `pylibcugraph-cu12-23.6.1.tar` & `pylibcugraph-cu12-23.6.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-12 22:37:14.382505 pylibcugraph-cu12-23.6.1/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      449 2023-06-12 22:37:14.000000 pylibcugraph-cu12-23.6.1/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-12 22:31:26.000000 pylibcugraph-cu12-23.6.1/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       17 2023-06-12 22:37:14.000000 pylibcugraph-cu12-23.6.1/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1616 2023-06-12 22:37:14.382505 pylibcugraph-cu12-23.6.1/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      256 2023-06-12 22:37:14.000000 pylibcugraph-cu12-23.6.1/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-12 22:37:14.382505 pylibcugraph-cu12-23.6.1/pylibcugraph_cu12.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1616 2023-06-12 22:37:14.000000 pylibcugraph-cu12-23.6.1/pylibcugraph_cu12.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      217 2023-06-12 22:37:14.000000 pylibcugraph-cu12-23.6.1/pylibcugraph_cu12.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-12 22:37:14.000000 pylibcugraph-cu12-23.6.1/pylibcugraph_cu12.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-12 22:37:14.000000 pylibcugraph-cu12-23.6.1/pylibcugraph_cu12.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-12 22:37:14.382505 pylibcugraph-cu12-23.6.1/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-12 22:31:26.000000 pylibcugraph-cu12-23.6.1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-14 14:12:39.282394 pylibcugraph-cu12-23.6.2/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      449 2023-06-14 14:12:39.000000 pylibcugraph-cu12-23.6.2/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 00:28:35.000000 pylibcugraph-cu12-23.6.2/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       17 2023-06-14 14:12:39.000000 pylibcugraph-cu12-23.6.2/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1616 2023-06-14 14:12:39.282394 pylibcugraph-cu12-23.6.2/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      256 2023-06-14 14:12:39.000000 pylibcugraph-cu12-23.6.2/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-14 14:12:39.282394 pylibcugraph-cu12-23.6.2/pylibcugraph_cu12.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1616 2023-06-14 14:12:39.000000 pylibcugraph-cu12-23.6.2/pylibcugraph_cu12.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      217 2023-06-14 14:12:39.000000 pylibcugraph-cu12-23.6.2/pylibcugraph_cu12.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-14 14:12:39.000000 pylibcugraph-cu12-23.6.2/pylibcugraph_cu12.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-14 14:12:39.000000 pylibcugraph-cu12-23.6.2/pylibcugraph_cu12.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-14 14:12:39.282394 pylibcugraph-cu12-23.6.2/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 00:28:35.000000 pylibcugraph-cu12-23.6.2/setup.py
```

### Comparing `pylibcugraph-cu12-23.6.1/LICENSE.md` & `pylibcugraph-cu12-23.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pylibcugraph-cu12-23.6.1/PKG-INFO` & `pylibcugraph-cu12-23.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibcugraph-cu12
-Version: 23.6.1
+Version: 23.6.2
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `pylibcugraph-cu12-23.6.1/pylibcugraph_cu12.egg-info/PKG-INFO` & `pylibcugraph-cu12-23.6.2/pylibcugraph_cu12.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibcugraph-cu12
-Version: 23.6.1
+Version: 23.6.2
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `pylibcugraph-cu12-23.6.1/setup.py` & `pylibcugraph-cu12-23.6.2/setup.py`

 * *Files identical despite different names*

