# Comparing `tmp/lightning-habana-1.0.0rc0.tar.gz` & `tmp/lightning-habana-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-habana-1.0.0rc0.tar", last modified: Mon Jun  5 13:08:50 2023, max compression
+gzip compressed data, was "lightning-habana-1.0.0rc1.tar", last modified: Tue Jun  6 02:42:49 2023, max compression
```

## Comparing `lightning-habana-1.0.0rc0.tar` & `lightning-habana-1.0.0rc1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:50.111267 lightning-habana-1.0.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-06-05 13:08:50.111267 lightning-habana-1.0.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:08:50.111267 lightning-habana-1.0.0rc0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4144 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:50.103267 lightning-habana-1.0.0rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:50.107267 lightning-habana-1.0.0rc0/src/lightning_habana/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:50.107267 lightning-habana-1.0.0rc0/src/lightning_habana/fabric/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/fabric/accelerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:50.107267 lightning-habana-1.0.0rc0/src/lightning_habana/fabric/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/fabric/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/fabric/plugins/io_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/fabric/plugins/precision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:50.107267 lightning-habana-1.0.0rc0/src/lightning_habana/fabric/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/fabric/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/fabric/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/fabric/strategies/single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:50.107267 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/accelerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:50.107267 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/datamodule/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/datamodule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:50.107267 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/datamodule/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/datamodule/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/datamodule/dataloaders/resnet_media_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/datamodule/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/datamodule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:50.107267 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/plugins/io_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/plugins/precision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:50.107267 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/profiler/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:50.111267 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44163 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/strategies/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/strategies/single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:50.111267 lightning-habana-1.0.0rc0/src/lightning_habana/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-05 13:08:39.000000 lightning-habana-1.0.0rc0/src/lightning_habana/utils/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:50.107267 lightning-habana-1.0.0rc0/src/lightning_habana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-06-05 13:08:50.000000 lightning-habana-1.0.0rc0/src/lightning_habana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-05 13:08:50.000000 lightning-habana-1.0.0rc0/src/lightning_habana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:08:50.000000 lightning-habana-1.0.0rc0/src/lightning_habana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:08:50.000000 lightning-habana-1.0.0rc0/src/lightning_habana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-05 13:08:50.000000 lightning-habana-1.0.0rc0/src/lightning_habana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-05 13:08:50.000000 lightning-habana-1.0.0rc0/src/lightning_habana.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.695874 lightning-habana-1.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 02:42:49.695874 lightning-habana-1.0.0rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4144 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.687873 lightning-habana-1.0.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.687873 lightning-habana-1.0.0rc1/src/lightning_habana/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/accelerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/plugins/io_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/plugins/precision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/strategies/single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/accelerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/dataloaders/resnet_media_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/plugins/io_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/plugins/precision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/profiler/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44163 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/utils/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-06 02:42:49.000000 lightning-habana-1.0.0rc1/src/lightning_habana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-06 02:42:49.000000 lightning-habana-1.0.0rc1/src/lightning_habana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 02:42:49.000000 lightning-habana-1.0.0rc1/src/lightning_habana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 02:42:49.000000 lightning-habana-1.0.0rc1/src/lightning_habana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-06 02:42:49.000000 lightning-habana-1.0.0rc1/src/lightning_habana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 02:42:49.000000 lightning-habana-1.0.0rc1/src/lightning_habana.egg-info/top_level.txt
```

### Comparing `lightning-habana-1.0.0rc0/CHANGELOG.md` & `lightning-habana-1.0.0rc1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/LICENSE` & `lightning-habana-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/MANIFEST.in` & `lightning-habana-1.0.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/PKG-INFO` & `lightning-habana-1.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-habana
-Version: 1.0.0rc0
+Version: 1.0.0rc1
 Summary: Lightning suport for Intel Habana accelerators
 Home-page: https://github.com/Lightning-AI/lightning-habana
 Download-URL: https://github.com/Lightning-AI/lightning-habana
 Author: Lightning-AI et al.
 Author-email: name@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning-habana/issues
@@ -22,15 +22,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: pytorch-lightning
 Provides-Extra: examples
+Provides-Extra: lightning
 Provides-Extra: test
 License-File: LICENSE
 
 # Lightning ⚡ Intel Habana
 
 [![lightning](https://img.shields.io/badge/-Lightning_2.0+-792ee5?logo=pytorchlightning&logoColor=white)](https://lightning.ai/)
 [![PyPI Status](https://badge.fury.io/py/lightning-habana.svg)](https://badge.fury.io/py/lightning-habana)
```

### Comparing `lightning-habana-1.0.0rc0/README.md` & `lightning-habana-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/setup.py` & `lightning-habana-1.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/__init__.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,29 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from lightning_habana.__about__ import *  # noqa: F401, F403
 from lightning_habana.pytorch.accelerator import HPUAccelerator
 from lightning_habana.pytorch.datamodule.datamodule import HPUDataModule
 from lightning_habana.pytorch.plugins.io_plugin import HPUCheckpointIO
 from lightning_habana.pytorch.plugins.precision import HPUPrecisionPlugin
 from lightning_habana.pytorch.profiler.profiler import HPUProfiler
 from lightning_habana.pytorch.strategies.deepspeed import HPUDeepSpeedStrategy
 from lightning_habana.pytorch.strategies.parallel import HPUParallelStrategy
 from lightning_habana.pytorch.strategies.single import SingleHPUStrategy
-from lightning_habana.utils.imports import _HPU_AVAILABLE
 
 __all__ = [
     "HPUAccelerator",
     "HPUDeepSpeedStrategy",
     "HPUParallelStrategy",
     "SingleHPUStrategy",
     "HPUPrecisionPlugin",
     "HPUCheckpointIO",
-    "HPUDataModule",
     "HPUProfiler",
-    "_HPU_AVAILABLE",
+    "HPUDataModule",
 ]
```

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/fabric/__init__.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/fabric/accelerator.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/fabric/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/fabric/plugins/__init__.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/fabric/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/fabric/plugins/io_plugin.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/fabric/plugins/io_plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 from typing import Any, Dict, Optional
 
 import torch
-from lightning.fabric.plugins import TorchCheckpointIO
-from lightning.fabric.utilities import move_data_to_device
-from lightning.fabric.utilities.cloud_io import _atomic_save, get_filesystem
-from lightning.fabric.utilities.rank_zero import rank_zero_warn
-from lightning.fabric.utilities.types import _PATH
+from lightning_utilities import module_available
+
+if module_available("lightning"):
+    from lightning.fabric.plugins import TorchCheckpointIO
+    from lightning.fabric.utilities import move_data_to_device
+    from lightning.fabric.utilities.cloud_io import _atomic_save, get_filesystem
+    from lightning.fabric.utilities.rank_zero import rank_zero_warn
+    from lightning.fabric.utilities.types import _PATH
+elif module_available("pytorch_lightning"):
+    from lightning_fabric.plugins import TorchCheckpointIO
+    from lightning_fabric.utilities import move_data_to_device
+    from lightning_fabric.utilities.cloud_io import _atomic_save, get_filesystem
+    from lightning_fabric.utilities.rank_zero import rank_zero_warn
+    from lightning_fabric.utilities.types import _PATH
+else:
+    raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 
 
 class HPUCheckpointIO(TorchCheckpointIO):
     """CheckpointIO to save checkpoints for HPU training strategies."""
 
     def save_checkpoint(self, checkpoint: Dict[str, Any], path: _PATH, storage_options: Optional[Any] = None) -> None:
         """Save model/training states as a checkpoint file through state-dump and file-write.
```

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/fabric/plugins/precision.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/fabric/plugins/precision.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Literal, Optional, Union, cast
 
-from lightning.fabric.plugins.precision.precision import Precision
+from lightning_utilities import module_available
 from typing_extensions import get_args
 
+if module_available("lightning"):
+    from lightning.fabric.plugins.precision.precision import Precision
+elif module_available("pytorch_lightning"):
+    from lightning_fabric.plugins.precision.precision import Precision
+else:
+    raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
+
+
 from lightning_habana.utils.imports import _HPU_AVAILABLE
 
 if _HPU_AVAILABLE:
     from habana_frameworks.torch.hpex import hmp
 
 _PRECISION_INPUT_INT = Literal[32]
 _PRECISION_INPUT_STR = Literal["32", "bf16", "32-true", "bf16-mixed"]
```

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/fabric/strategies/__init__.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/fabric/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/__init__.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,27 +7,38 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import operator
 
+from lightning_utilities import compare_version
+
+from lightning_habana.__about__ import *  # noqa: F401, F403
 from lightning_habana.pytorch.accelerator import HPUAccelerator
 from lightning_habana.pytorch.datamodule.datamodule import HPUDataModule
 from lightning_habana.pytorch.plugins.io_plugin import HPUCheckpointIO
 from lightning_habana.pytorch.plugins.precision import HPUPrecisionPlugin
 from lightning_habana.pytorch.profiler.profiler import HPUProfiler
 from lightning_habana.pytorch.strategies.deepspeed import HPUDeepSpeedStrategy
 from lightning_habana.pytorch.strategies.parallel import HPUParallelStrategy
 from lightning_habana.pytorch.strategies.single import SingleHPUStrategy
+from lightning_habana.utils.imports import _HPU_AVAILABLE
+
+if compare_version("lightning", operator.lt, "2.0.0") and compare_version("pytorch_lightning", operator.lt, "2.0.0"):
+    raise ImportError(
+        "You are missing `lightning` or `pytorch-lightning` package or neither of them is in version 2.0+"
+    )
 
 __all__ = [
     "HPUAccelerator",
     "HPUDeepSpeedStrategy",
     "HPUParallelStrategy",
     "SingleHPUStrategy",
     "HPUPrecisionPlugin",
     "HPUCheckpointIO",
-    "HPUProfiler",
     "HPUDataModule",
+    "HPUProfiler",
+    "_HPU_AVAILABLE",
 ]
```

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/accelerator.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/datamodule/__init__.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/datamodule/dataloaders/__init__.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/dataloaders/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/datamodule/dataloaders/resnet_media_pipe.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/dataloaders/resnet_media_pipe.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/datamodule/datamodule.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/datamodule.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/datamodule/utils.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/plugins/__init__.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/plugins/io_plugin.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/plugins/io_plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/plugins/precision.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/plugins/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/profiler/__init__.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/profiler/profiler.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/strategies/__init__.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/strategies/deepspeed.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/strategies/parallel.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/parallel.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/pytorch/strategies/single.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/single.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana/utils/imports.py` & `lightning-habana-1.0.0rc1/src/lightning_habana/utils/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana.egg-info/PKG-INFO` & `lightning-habana-1.0.0rc1/src/lightning_habana.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-habana
-Version: 1.0.0rc0
+Version: 1.0.0rc1
 Summary: Lightning suport for Intel Habana accelerators
 Home-page: https://github.com/Lightning-AI/lightning-habana
 Download-URL: https://github.com/Lightning-AI/lightning-habana
 Author: Lightning-AI et al.
 Author-email: name@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning-habana/issues
@@ -22,15 +22,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: pytorch-lightning
 Provides-Extra: examples
+Provides-Extra: lightning
 Provides-Extra: test
 License-File: LICENSE
 
 # Lightning ⚡ Intel Habana
 
 [![lightning](https://img.shields.io/badge/-Lightning_2.0+-792ee5?logo=pytorchlightning&logoColor=white)](https://lightning.ai/)
 [![PyPI Status](https://badge.fury.io/py/lightning-habana.svg)](https://badge.fury.io/py/lightning-habana)
```

### Comparing `lightning-habana-1.0.0rc0/src/lightning_habana.egg-info/SOURCES.txt` & `lightning-habana-1.0.0rc1/src/lightning_habana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

