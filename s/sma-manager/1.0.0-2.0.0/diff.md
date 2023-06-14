# Comparing `tmp/sma-manager-1.0.0.tar.gz` & `tmp/sma-manager-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sma-manager-1.0.0.tar", last modified: Tue Jun 13 17:00:13 2023, max compression
+gzip compressed data, was "sma-manager-2.0.0.tar", last modified: Wed Jun 14 09:12:49 2023, max compression
```

## Comparing `sma-manager-1.0.0.tar` & `sma-manager-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:00:13.151036 sma-manager-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 17:00:03.000000 sma-manager-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-13 17:00:13.151036 sma-manager-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-13 17:00:03.000000 sma-manager-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:00:13.151036 sma-manager-1.0.0/SMA/
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-13 17:00:03.000000 sma-manager-1.0.0/SMA/SMA.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 17:00:03.000000 sma-manager-1.0.0/SMA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:00:13.151036 sma-manager-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-13 17:00:03.000000 sma-manager-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:00:13.151036 sma-manager-1.0.0/sma_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-13 17:00:13.000000 sma-manager-1.0.0/sma_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 17:00:13.000000 sma-manager-1.0.0/sma_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:00:13.000000 sma-manager-1.0.0/sma_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 17:00:13.000000 sma-manager-1.0.0/sma_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:12:49.992417 sma-manager-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 09:12:39.000000 sma-manager-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-14 09:12:49.988417 sma-manager-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-14 09:12:39.000000 sma-manager-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:12:49.992417 sma-manager-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-14 09:12:39.000000 sma-manager-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:12:49.988417 sma-manager-2.0.0/sma_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-14 09:12:49.000000 sma-manager-2.0.0/sma_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-14 09:12:49.000000 sma-manager-2.0.0/sma_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:12:49.000000 sma-manager-2.0.0/sma_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 09:12:49.000000 sma-manager-2.0.0/sma_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:12:49.988417 sma-manager-2.0.0/sma_manager_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-14 09:12:39.000000 sma-manager-2.0.0/sma_manager_api/SMA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-14 09:12:39.000000 sma-manager-2.0.0/sma_manager_api/__init__.py
```

### Comparing `sma-manager-1.0.0/LICENSE` & `sma-manager-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sma-manager-1.0.0/SMA/SMA.py` & `sma-manager-2.0.0/sma_manager_api/SMA.py`

 * *Files identical despite different names*

### Comparing `sma-manager-1.0.0/setup.py` & `sma-manager-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import pathlib
 
 README = (pathlib.Path(__file__).parent / "README.md").read_text(encoding='utf8')
 
 setup(
     name='sma-manager',
     packages=find_packages(),
-    version='1.0.0',
+    version='2.0.0',
     description='Package for collecting information from the SMA Manager device of solar panels.',
     long_description=README,
     long_description_content_type='text/markdown',
     author='DeadSec-Security',
     author_email='amng835@gmail.com',
     url='https://github.com/DEADSEC-SECURITY/sma-manager',
     keywords=[
```

