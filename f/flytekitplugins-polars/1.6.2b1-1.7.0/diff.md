# Comparing `tmp/flytekitplugins-polars-1.6.2b1.tar.gz` & `tmp/flytekitplugins-polars-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-polars-1.6.2b1.tar", last modified: Thu Jun  8 23:49:51 2023, max compression
+gzip compressed data, was "flytekitplugins-polars-1.7.0.tar", last modified: Wed Jun 14 04:33:34 2023, max compression
```

## Comparing `flytekitplugins-polars-1.6.2b1.tar` & `flytekitplugins-polars-1.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:51.731274 flytekitplugins-polars-1.6.2b1/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-08 23:49:51.731274 flytekitplugins-polars-1.6.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-08 23:49:15.000000 flytekitplugins-polars-1.6.2b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:51.727274 flytekitplugins-polars-1.6.2b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:51.727274 flytekitplugins-polars-1.6.2b1/flytekitplugins/polars/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-08 23:49:15.000000 flytekitplugins-polars-1.6.2b1/flytekitplugins/polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-08 23:49:15.000000 flytekitplugins-polars-1.6.2b1/flytekitplugins/polars/sd_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:51.731274 flytekitplugins-polars-1.6.2b1/flytekitplugins_polars.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-08 23:49:51.000000 flytekitplugins-polars-1.6.2b1/flytekitplugins_polars.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-08 23:49:51.000000 flytekitplugins-polars-1.6.2b1/flytekitplugins_polars.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:49:51.000000 flytekitplugins-polars-1.6.2b1/flytekitplugins_polars.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-08 23:49:51.000000 flytekitplugins-polars-1.6.2b1/flytekitplugins_polars.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:51.000000 flytekitplugins-polars-1.6.2b1/flytekitplugins_polars.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-08 23:49:51.000000 flytekitplugins-polars-1.6.2b1/flytekitplugins_polars.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:51.000000 flytekitplugins-polars-1.6.2b1/flytekitplugins_polars.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 23:49:51.731274 flytekitplugins-polars-1.6.2b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-08 23:49:38.000000 flytekitplugins-polars-1.6.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:34.181412 flytekitplugins-polars-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-14 04:33:34.181412 flytekitplugins-polars-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-14 04:33:05.000000 flytekitplugins-polars-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:34.181412 flytekitplugins-polars-1.7.0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:34.181412 flytekitplugins-polars-1.7.0/flytekitplugins/polars/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-14 04:33:05.000000 flytekitplugins-polars-1.7.0/flytekitplugins/polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-14 04:33:05.000000 flytekitplugins-polars-1.7.0/flytekitplugins/polars/sd_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:34.181412 flytekitplugins-polars-1.7.0/flytekitplugins_polars.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-14 04:33:34.000000 flytekitplugins-polars-1.7.0/flytekitplugins_polars.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-14 04:33:34.000000 flytekitplugins-polars-1.7.0/flytekitplugins_polars.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:33:34.000000 flytekitplugins-polars-1.7.0/flytekitplugins_polars.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-14 04:33:34.000000 flytekitplugins-polars-1.7.0/flytekitplugins_polars.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:34.000000 flytekitplugins-polars-1.7.0/flytekitplugins_polars.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-14 04:33:34.000000 flytekitplugins-polars-1.7.0/flytekitplugins_polars.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:34.000000 flytekitplugins-polars-1.7.0/flytekitplugins_polars.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:33:34.181412 flytekitplugins-polars-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-14 04:33:24.000000 flytekitplugins-polars-1.7.0/setup.py
```

### Comparing `flytekitplugins-polars-1.6.2b1/PKG-INFO` & `flytekitplugins-polars-1.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-polars
-Version: 1.6.2b1
+Version: 1.7.0
 Summary: Polars plugin for flytekit
 Author: Robin Kahlow
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-polars-1.6.2b1/flytekitplugins/polars/sd_transformers.py` & `flytekitplugins-polars-1.7.0/flytekitplugins/polars/sd_transformers.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-polars-1.6.2b1/flytekitplugins_polars.egg-info/PKG-INFO` & `flytekitplugins-polars-1.7.0/flytekitplugins_polars.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-polars
-Version: 1.6.2b1
+Version: 1.7.0
 Summary: Polars plugin for flytekit
 Author: Robin Kahlow
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-polars-1.6.2b1/setup.py` & `flytekitplugins-polars-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = [
     "flytekit>=1.3.0b2,<2.0.0",
     "polars>=0.8.27",
 ]
 
-__version__ = "1.6.2b1"
+__version__ = "1.7.0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="Robin Kahlow",
     description="Polars plugin for flytekit",
     namespace_packages=["flytekitplugins"],
```

