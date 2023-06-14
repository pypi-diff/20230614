# Comparing `tmp/flytekitplugins-kfpytorch-1.6.2b1.tar.gz` & `tmp/flytekitplugins-kfpytorch-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kfpytorch-1.6.2b1.tar", last modified: Thu Jun  8 23:49:47 2023, max compression
+gzip compressed data, was "flytekitplugins-kfpytorch-1.7.0.tar", last modified: Wed Jun 14 04:33:31 2023, max compression
```

## Comparing `flytekitplugins-kfpytorch-1.6.2b1.tar` & `flytekitplugins-kfpytorch-1.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:47.559252 flytekitplugins-kfpytorch-1.6.2b1/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-08 23:49:47.559252 flytekitplugins-kfpytorch-1.6.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-08 23:49:15.000000 flytekitplugins-kfpytorch-1.6.2b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:47.559252 flytekitplugins-kfpytorch-1.6.2b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:47.559252 flytekitplugins-kfpytorch-1.6.2b1/flytekitplugins/kfpytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-08 23:49:15.000000 flytekitplugins-kfpytorch-1.6.2b1/flytekitplugins/kfpytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14362 2023-06-08 23:49:15.000000 flytekitplugins-kfpytorch-1.6.2b1/flytekitplugins/kfpytorch/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:47.559252 flytekitplugins-kfpytorch-1.6.2b1/flytekitplugins_kfpytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-08 23:49:47.000000 flytekitplugins-kfpytorch-1.6.2b1/flytekitplugins_kfpytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-08 23:49:47.000000 flytekitplugins-kfpytorch-1.6.2b1/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:49:47.000000 flytekitplugins-kfpytorch-1.6.2b1/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:47.000000 flytekitplugins-kfpytorch-1.6.2b1/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 23:49:47.000000 flytekitplugins-kfpytorch-1.6.2b1/flytekitplugins_kfpytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:47.000000 flytekitplugins-kfpytorch-1.6.2b1/flytekitplugins_kfpytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 23:49:47.559252 flytekitplugins-kfpytorch-1.6.2b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-08 23:49:38.000000 flytekitplugins-kfpytorch-1.6.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:31.229368 flytekitplugins-kfpytorch-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-14 04:33:31.229368 flytekitplugins-kfpytorch-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-14 04:33:05.000000 flytekitplugins-kfpytorch-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:31.229368 flytekitplugins-kfpytorch-1.7.0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:31.229368 flytekitplugins-kfpytorch-1.7.0/flytekitplugins/kfpytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-14 04:33:05.000000 flytekitplugins-kfpytorch-1.7.0/flytekitplugins/kfpytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14362 2023-06-14 04:33:05.000000 flytekitplugins-kfpytorch-1.7.0/flytekitplugins/kfpytorch/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:31.229368 flytekitplugins-kfpytorch-1.7.0/flytekitplugins_kfpytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-14 04:33:31.000000 flytekitplugins-kfpytorch-1.7.0/flytekitplugins_kfpytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-14 04:33:31.000000 flytekitplugins-kfpytorch-1.7.0/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:33:31.000000 flytekitplugins-kfpytorch-1.7.0/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:31.000000 flytekitplugins-kfpytorch-1.7.0/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-14 04:33:31.000000 flytekitplugins-kfpytorch-1.7.0/flytekitplugins_kfpytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:31.000000 flytekitplugins-kfpytorch-1.7.0/flytekitplugins_kfpytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:33:31.229368 flytekitplugins-kfpytorch-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-14 04:33:24.000000 flytekitplugins-kfpytorch-1.7.0/setup.py
```

### Comparing `flytekitplugins-kfpytorch-1.6.2b1/PKG-INFO` & `flytekitplugins-kfpytorch-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.6.2b1
+Version: 1.7.0
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfpytorch-1.6.2b1/README.md` & `flytekitplugins-kfpytorch-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kfpytorch-1.6.2b1/flytekitplugins/kfpytorch/task.py` & `flytekitplugins-kfpytorch-1.7.0/flytekitplugins/kfpytorch/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kfpytorch-1.6.2b1/flytekitplugins_kfpytorch.egg-info/PKG-INFO` & `flytekitplugins-kfpytorch-1.7.0/flytekitplugins_kfpytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.6.2b1
+Version: 1.7.0
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfpytorch-1.6.2b1/setup.py` & `flytekitplugins-kfpytorch-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "kfpytorch"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["cloudpickle", "flyteidl>=1.5.1", "flytekit>=1.6.1"]
 
-__version__ = "1.6.2b1"
+__version__ = "1.7.0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based Pytorch plugin for Flytekit",
```

