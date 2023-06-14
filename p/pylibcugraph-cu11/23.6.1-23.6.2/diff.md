# Comparing `tmp/pylibcugraph-cu11-23.6.1.tar.gz` & `tmp/pylibcugraph-cu11-23.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibcugraph-cu11-23.6.1.tar", last modified: Fri Jun  9 18:53:46 2023, max compression
+gzip compressed data, was "pylibcugraph-cu11-23.6.2.tar", last modified: Wed Jun 14 14:14:36 2023, max compression
```

## Comparing `pylibcugraph-cu11-23.6.1.tar` & `pylibcugraph-cu11-23.6.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-09 18:53:46.294228 pylibcugraph-cu11-23.6.1/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      449 2023-06-09 18:53:46.000000 pylibcugraph-cu11-23.6.1/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-08 22:12:21.000000 pylibcugraph-cu11-23.6.1/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       17 2023-06-09 18:53:46.000000 pylibcugraph-cu11-23.6.1/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1616 2023-06-09 18:53:46.294228 pylibcugraph-cu11-23.6.1/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      256 2023-06-09 18:53:46.000000 pylibcugraph-cu11-23.6.1/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-09 18:53:46.293228 pylibcugraph-cu11-23.6.1/pylibcugraph_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1616 2023-06-09 18:53:46.000000 pylibcugraph-cu11-23.6.1/pylibcugraph_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      217 2023-06-09 18:53:46.000000 pylibcugraph-cu11-23.6.1/pylibcugraph_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-09 18:53:46.000000 pylibcugraph-cu11-23.6.1/pylibcugraph_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-09 18:53:46.000000 pylibcugraph-cu11-23.6.1/pylibcugraph_cu11.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-09 18:53:46.294228 pylibcugraph-cu11-23.6.1/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-08 22:12:21.000000 pylibcugraph-cu11-23.6.1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-14 14:14:36.576633 pylibcugraph-cu11-23.6.2/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      449 2023-06-14 14:14:36.000000 pylibcugraph-cu11-23.6.2/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 14:12:21.000000 pylibcugraph-cu11-23.6.2/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       17 2023-06-14 14:14:36.000000 pylibcugraph-cu11-23.6.2/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1616 2023-06-14 14:14:36.576633 pylibcugraph-cu11-23.6.2/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      256 2023-06-14 14:14:36.000000 pylibcugraph-cu11-23.6.2/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-14 14:14:36.576633 pylibcugraph-cu11-23.6.2/pylibcugraph_cu11.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1616 2023-06-14 14:14:36.000000 pylibcugraph-cu11-23.6.2/pylibcugraph_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      217 2023-06-14 14:14:36.000000 pylibcugraph-cu11-23.6.2/pylibcugraph_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-14 14:14:36.000000 pylibcugraph-cu11-23.6.2/pylibcugraph_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-14 14:14:36.000000 pylibcugraph-cu11-23.6.2/pylibcugraph_cu11.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-14 14:14:36.576633 pylibcugraph-cu11-23.6.2/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 14:12:21.000000 pylibcugraph-cu11-23.6.2/setup.py
```

### Comparing `pylibcugraph-cu11-23.6.1/LICENSE.md` & `pylibcugraph-cu11-23.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pylibcugraph-cu11-23.6.1/PKG-INFO` & `pylibcugraph-cu11-23.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibcugraph-cu11
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

### Comparing `pylibcugraph-cu11-23.6.1/pylibcugraph_cu11.egg-info/PKG-INFO` & `pylibcugraph-cu11-23.6.2/pylibcugraph_cu11.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibcugraph-cu11
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

### Comparing `pylibcugraph-cu11-23.6.1/setup.py` & `pylibcugraph-cu11-23.6.2/setup.py`

 * *Files identical despite different names*

