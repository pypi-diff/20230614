# Comparing `tmp/autogluon-0.7.1b20230613.tar.gz` & `tmp/autogluon-0.7.1b20230614.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-0.7.1b20230613.tar", last modified: Tue Jun 13 09:04:30 2023, max compression
+gzip compressed data, was "autogluon-0.7.1b20230614.tar", last modified: Wed Jun 14 09:04:24 2023, max compression
```

## Comparing `autogluon-0.7.1b20230613.tar` & `autogluon-0.7.1b20230614.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:30.227723 autogluon-0.7.1b20230613/
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-13 09:04:30.227723 autogluon-0.7.1b20230613/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:04:30.227723 autogluon-0.7.1b20230613/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-13 09:03:45.000000 autogluon-0.7.1b20230613/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:30.227723 autogluon-0.7.1b20230613/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:30.227723 autogluon-0.7.1b20230613/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:30.227723 autogluon-0.7.1b20230613/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:03:45.000000 autogluon-0.7.1b20230613/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:30.227723 autogluon-0.7.1b20230613/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-13 09:04:30.000000 autogluon-0.7.1b20230613/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-13 09:04:30.000000 autogluon-0.7.1b20230613/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:04:30.000000 autogluon-0.7.1b20230613/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 09:04:30.000000 autogluon-0.7.1b20230613/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 09:04:30.000000 autogluon-0.7.1b20230613/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 09:04:30.000000 autogluon-0.7.1b20230613/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:04:30.000000 autogluon-0.7.1b20230613/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:24.198775 autogluon-0.7.1b20230614/
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-14 09:04:24.198775 autogluon-0.7.1b20230614/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:04:24.198775 autogluon-0.7.1b20230614/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-14 09:03:34.000000 autogluon-0.7.1b20230614/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:24.194775 autogluon-0.7.1b20230614/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:24.194775 autogluon-0.7.1b20230614/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:24.194775 autogluon-0.7.1b20230614/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:03:34.000000 autogluon-0.7.1b20230614/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:24.194775 autogluon-0.7.1b20230614/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-14 09:04:24.000000 autogluon-0.7.1b20230614/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-14 09:04:24.000000 autogluon-0.7.1b20230614/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:04:24.000000 autogluon-0.7.1b20230614/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 09:04:24.000000 autogluon-0.7.1b20230614/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-14 09:04:24.000000 autogluon-0.7.1b20230614/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 09:04:24.000000 autogluon-0.7.1b20230614/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:04:24.000000 autogluon-0.7.1b20230614/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-0.7.1b20230613/PKG-INFO` & `autogluon-0.7.1b20230614/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.7.1b20230613
+Version: 0.7.1b20230614
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-0.7.1b20230613/setup.py` & `autogluon-0.7.1b20230614/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-0.7.1b20230613/src/autogluon.egg-info/PKG-INFO` & `autogluon-0.7.1b20230614/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.7.1b20230613
+Version: 0.7.1b20230614
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

