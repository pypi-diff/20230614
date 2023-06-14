# Comparing `tmp/flytekitplugins-kftensorflow-1.6.2b1.tar.gz` & `tmp/flytekitplugins-kftensorflow-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kftensorflow-1.6.2b1.tar", last modified: Thu Jun  8 23:49:48 2023, max compression
+gzip compressed data, was "flytekitplugins-kftensorflow-1.7.0.tar", last modified: Wed Jun 14 04:33:31 2023, max compression
```

## Comparing `flytekitplugins-kftensorflow-1.6.2b1.tar` & `flytekitplugins-kftensorflow-1.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:48.087255 flytekitplugins-kftensorflow-1.6.2b1/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-08 23:49:48.087255 flytekitplugins-kftensorflow-1.6.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-08 23:49:15.000000 flytekitplugins-kftensorflow-1.6.2b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:48.083255 flytekitplugins-kftensorflow-1.6.2b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:48.087255 flytekitplugins-kftensorflow-1.6.2b1/flytekitplugins/kftensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-08 23:49:15.000000 flytekitplugins-kftensorflow-1.6.2b1/flytekitplugins/kftensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-06-08 23:49:15.000000 flytekitplugins-kftensorflow-1.6.2b1/flytekitplugins/kftensorflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:48.087255 flytekitplugins-kftensorflow-1.6.2b1/flytekitplugins_kftensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-08 23:49:48.000000 flytekitplugins-kftensorflow-1.6.2b1/flytekitplugins_kftensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-08 23:49:48.000000 flytekitplugins-kftensorflow-1.6.2b1/flytekitplugins_kftensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:49:48.000000 flytekitplugins-kftensorflow-1.6.2b1/flytekitplugins_kftensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:48.000000 flytekitplugins-kftensorflow-1.6.2b1/flytekitplugins_kftensorflow.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:48.000000 flytekitplugins-kftensorflow-1.6.2b1/flytekitplugins_kftensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:48.000000 flytekitplugins-kftensorflow-1.6.2b1/flytekitplugins_kftensorflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 23:49:48.087255 flytekitplugins-kftensorflow-1.6.2b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-08 23:49:38.000000 flytekitplugins-kftensorflow-1.6.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:31.601373 flytekitplugins-kftensorflow-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-14 04:33:31.597373 flytekitplugins-kftensorflow-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-14 04:33:05.000000 flytekitplugins-kftensorflow-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:31.597373 flytekitplugins-kftensorflow-1.7.0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:31.597373 flytekitplugins-kftensorflow-1.7.0/flytekitplugins/kftensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-14 04:33:05.000000 flytekitplugins-kftensorflow-1.7.0/flytekitplugins/kftensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-06-14 04:33:05.000000 flytekitplugins-kftensorflow-1.7.0/flytekitplugins/kftensorflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:31.597373 flytekitplugins-kftensorflow-1.7.0/flytekitplugins_kftensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-14 04:33:31.000000 flytekitplugins-kftensorflow-1.7.0/flytekitplugins_kftensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-14 04:33:31.000000 flytekitplugins-kftensorflow-1.7.0/flytekitplugins_kftensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:33:31.000000 flytekitplugins-kftensorflow-1.7.0/flytekitplugins_kftensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:31.000000 flytekitplugins-kftensorflow-1.7.0/flytekitplugins_kftensorflow.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:31.000000 flytekitplugins-kftensorflow-1.7.0/flytekitplugins_kftensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:31.000000 flytekitplugins-kftensorflow-1.7.0/flytekitplugins_kftensorflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:33:31.601373 flytekitplugins-kftensorflow-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-14 04:33:24.000000 flytekitplugins-kftensorflow-1.7.0/setup.py
```

### Comparing `flytekitplugins-kftensorflow-1.6.2b1/PKG-INFO` & `flytekitplugins-kftensorflow-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kftensorflow
-Version: 1.6.2b1
+Version: 1.7.0
 Summary: K8s based Tensorflow plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kftensorflow-1.6.2b1/README.md` & `flytekitplugins-kftensorflow-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kftensorflow-1.6.2b1/flytekitplugins/kftensorflow/task.py` & `flytekitplugins-kftensorflow-1.7.0/flytekitplugins/kftensorflow/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kftensorflow-1.6.2b1/flytekitplugins_kftensorflow.egg-info/PKG-INFO` & `flytekitplugins-kftensorflow-1.7.0/flytekitplugins_kftensorflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kftensorflow
-Version: 1.6.2b1
+Version: 1.7.0
 Summary: K8s based Tensorflow plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kftensorflow-1.6.2b1/setup.py` & `flytekitplugins-kftensorflow-1.7.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "kftensorflow"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.6.1"]
 
-__version__ = "1.6.2b1"
+__version__ = "1.7.0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based Tensorflow plugin for flytekit",
```

