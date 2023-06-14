# Comparing `tmp/flytekitplugins-whylogs-1.6.2b1.tar.gz` & `tmp/flytekitplugins-whylogs-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-whylogs-1.6.2b1.tar", last modified: Thu Jun  8 23:49:54 2023, max compression
+gzip compressed data, was "flytekitplugins-whylogs-1.7.0.tar", last modified: Wed Jun 14 04:33:36 2023, max compression
```

## Comparing `flytekitplugins-whylogs-1.6.2b1.tar` & `flytekitplugins-whylogs-1.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:54.887291 flytekitplugins-whylogs-1.6.2b1/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-08 23:49:54.887291 flytekitplugins-whylogs-1.6.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-08 23:49:15.000000 flytekitplugins-whylogs-1.6.2b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:54.883291 flytekitplugins-whylogs-1.6.2b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:54.883291 flytekitplugins-whylogs-1.6.2b1/flytekitplugins/whylogs/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-08 23:49:15.000000 flytekitplugins-whylogs-1.6.2b1/flytekitplugins/whylogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-08 23:49:15.000000 flytekitplugins-whylogs-1.6.2b1/flytekitplugins/whylogs/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-08 23:49:15.000000 flytekitplugins-whylogs-1.6.2b1/flytekitplugins/whylogs/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:54.887291 flytekitplugins-whylogs-1.6.2b1/flytekitplugins_whylogs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-08 23:49:54.000000 flytekitplugins-whylogs-1.6.2b1/flytekitplugins_whylogs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-08 23:49:54.000000 flytekitplugins-whylogs-1.6.2b1/flytekitplugins_whylogs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:49:54.000000 flytekitplugins-whylogs-1.6.2b1/flytekitplugins_whylogs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-08 23:49:54.000000 flytekitplugins-whylogs-1.6.2b1/flytekitplugins_whylogs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:54.000000 flytekitplugins-whylogs-1.6.2b1/flytekitplugins_whylogs.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-08 23:49:54.000000 flytekitplugins-whylogs-1.6.2b1/flytekitplugins_whylogs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:54.000000 flytekitplugins-whylogs-1.6.2b1/flytekitplugins_whylogs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 23:49:54.887291 flytekitplugins-whylogs-1.6.2b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-08 23:49:38.000000 flytekitplugins-whylogs-1.6.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:36.409446 flytekitplugins-whylogs-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-14 04:33:36.409446 flytekitplugins-whylogs-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-14 04:33:05.000000 flytekitplugins-whylogs-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:36.409446 flytekitplugins-whylogs-1.7.0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:36.409446 flytekitplugins-whylogs-1.7.0/flytekitplugins/whylogs/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-14 04:33:05.000000 flytekitplugins-whylogs-1.7.0/flytekitplugins/whylogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-14 04:33:05.000000 flytekitplugins-whylogs-1.7.0/flytekitplugins/whylogs/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-14 04:33:05.000000 flytekitplugins-whylogs-1.7.0/flytekitplugins/whylogs/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:36.409446 flytekitplugins-whylogs-1.7.0/flytekitplugins_whylogs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-14 04:33:36.000000 flytekitplugins-whylogs-1.7.0/flytekitplugins_whylogs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-14 04:33:36.000000 flytekitplugins-whylogs-1.7.0/flytekitplugins_whylogs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:33:36.000000 flytekitplugins-whylogs-1.7.0/flytekitplugins_whylogs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-14 04:33:36.000000 flytekitplugins-whylogs-1.7.0/flytekitplugins_whylogs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:36.000000 flytekitplugins-whylogs-1.7.0/flytekitplugins_whylogs.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-14 04:33:36.000000 flytekitplugins-whylogs-1.7.0/flytekitplugins_whylogs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:36.000000 flytekitplugins-whylogs-1.7.0/flytekitplugins_whylogs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:33:36.409446 flytekitplugins-whylogs-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-14 04:33:24.000000 flytekitplugins-whylogs-1.7.0/setup.py
```

### Comparing `flytekitplugins-whylogs-1.6.2b1/PKG-INFO` & `flytekitplugins-whylogs-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-whylogs
-Version: 1.6.2b1
+Version: 1.7.0
 Summary: Enable the use of whylogs profiles to be used in flyte tasks to get aggregate statistics about data.
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-whylogs
 Author: whylabs
 Author-email: support@whylabs.ai
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-whylogs-1.6.2b1/README.md` & `flytekitplugins-whylogs-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-whylogs-1.6.2b1/flytekitplugins/whylogs/renderer.py` & `flytekitplugins-whylogs-1.7.0/flytekitplugins/whylogs/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-whylogs-1.6.2b1/flytekitplugins/whylogs/schema.py` & `flytekitplugins-whylogs-1.7.0/flytekitplugins/whylogs/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-whylogs-1.6.2b1/flytekitplugins_whylogs.egg-info/PKG-INFO` & `flytekitplugins-whylogs-1.7.0/flytekitplugins_whylogs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-whylogs
-Version: 1.6.2b1
+Version: 1.7.0
 Summary: Enable the use of whylogs profiles to be used in flyte tasks to get aggregate statistics about data.
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-whylogs
 Author: whylabs
 Author-email: support@whylabs.ai
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-whylogs-1.6.2b1/setup.py` & `flytekitplugins-whylogs-1.7.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "whylogs"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "whylogs[viz]>=1.1.16"]
 
-__version__ = "1.6.2b1"
+__version__ = "1.7.0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="whylabs",
     author_email="support@whylabs.ai",
     description="Enable the use of whylogs profiles to be used in flyte tasks to get aggregate statistics about data.",
```

