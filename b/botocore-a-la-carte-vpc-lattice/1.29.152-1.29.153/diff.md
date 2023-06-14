# Comparing `tmp/botocore-a-la-carte-vpc-lattice-1.29.152.tar.gz` & `tmp/botocore-a-la-carte-vpc-lattice-1.29.153.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-vpc-lattice-1.29.152.tar", last modified: Tue Jun 13 01:27:47 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-vpc-lattice-1.29.153.tar", last modified: Wed Jun 14 01:25:52 2023, max compression
```

## Comparing `botocore-a-la-carte-vpc-lattice-1.29.152.tar` & `botocore-a-la-carte-vpc-lattice-1.29.153.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:27:47.497999 botocore-a-la-carte-vpc-lattice-1.29.152/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-13 01:27:47.000000 botocore-a-la-carte-vpc-lattice-1.29.152/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-13 01:27:47.497999 botocore-a-la-carte-vpc-lattice-1.29.152/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:27:47.497999 botocore-a-la-carte-vpc-lattice-1.29.152/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:27:47.497999 botocore-a-la-carte-vpc-lattice-1.29.152/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:27:47.497999 botocore-a-la-carte-vpc-lattice-1.29.152/botocore/data/vpc-lattice/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:27:47.497999 botocore-a-la-carte-vpc-lattice-1.29.152/botocore/data/vpc-lattice/2022-11-30/
--rw-r--r--   0 runner    (1001) docker     (123)    17644 2023-06-13 01:26:44.000000 botocore-a-la-carte-vpc-lattice-1.29.152/botocore/data/vpc-lattice/2022-11-30/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-13 01:26:44.000000 botocore-a-la-carte-vpc-lattice-1.29.152/botocore/data/vpc-lattice/2022-11-30/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   175550 2023-06-13 01:26:44.000000 botocore-a-la-carte-vpc-lattice-1.29.152/botocore/data/vpc-lattice/2022-11-30/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:27:47.497999 botocore-a-la-carte-vpc-lattice-1.29.152/botocore_a_la_carte_vpc_lattice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-13 01:27:47.000000 botocore-a-la-carte-vpc-lattice-1.29.152/botocore_a_la_carte_vpc_lattice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-13 01:27:47.000000 botocore-a-la-carte-vpc-lattice-1.29.152/botocore_a_la_carte_vpc_lattice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:27:47.000000 botocore-a-la-carte-vpc-lattice-1.29.152/botocore_a_la_carte_vpc_lattice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 01:27:47.000000 botocore-a-la-carte-vpc-lattice-1.29.152/botocore_a_la_carte_vpc_lattice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 01:27:47.497999 botocore-a-la-carte-vpc-lattice-1.29.152/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-13 01:27:47.000000 botocore-a-la-carte-vpc-lattice-1.29.152/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:25:52.468922 botocore-a-la-carte-vpc-lattice-1.29.153/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-14 01:25:52.000000 botocore-a-la-carte-vpc-lattice-1.29.153/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-14 01:25:52.468922 botocore-a-la-carte-vpc-lattice-1.29.153/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:25:52.468922 botocore-a-la-carte-vpc-lattice-1.29.153/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:25:52.468922 botocore-a-la-carte-vpc-lattice-1.29.153/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:25:52.468922 botocore-a-la-carte-vpc-lattice-1.29.153/botocore/data/vpc-lattice/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:25:52.468922 botocore-a-la-carte-vpc-lattice-1.29.153/botocore/data/vpc-lattice/2022-11-30/
+-rw-r--r--   0 runner    (1001) docker     (123)    17644 2023-06-14 01:25:05.000000 botocore-a-la-carte-vpc-lattice-1.29.153/botocore/data/vpc-lattice/2022-11-30/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-14 01:25:05.000000 botocore-a-la-carte-vpc-lattice-1.29.153/botocore/data/vpc-lattice/2022-11-30/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   175550 2023-06-14 01:25:05.000000 botocore-a-la-carte-vpc-lattice-1.29.153/botocore/data/vpc-lattice/2022-11-30/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:25:52.468922 botocore-a-la-carte-vpc-lattice-1.29.153/botocore_a_la_carte_vpc_lattice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-14 01:25:52.000000 botocore-a-la-carte-vpc-lattice-1.29.153/botocore_a_la_carte_vpc_lattice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-14 01:25:52.000000 botocore-a-la-carte-vpc-lattice-1.29.153/botocore_a_la_carte_vpc_lattice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:25:52.000000 botocore-a-la-carte-vpc-lattice-1.29.153/botocore_a_la_carte_vpc_lattice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 01:25:52.000000 botocore-a-la-carte-vpc-lattice-1.29.153/botocore_a_la_carte_vpc_lattice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 01:25:52.468922 botocore-a-la-carte-vpc-lattice-1.29.153/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-14 01:25:52.000000 botocore-a-la-carte-vpc-lattice-1.29.153/setup.py
```

### Comparing `botocore-a-la-carte-vpc-lattice-1.29.152/LICENSE.txt` & `botocore-a-la-carte-vpc-lattice-1.29.153/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-vpc-lattice-1.29.152/PKG-INFO` & `botocore-a-la-carte-vpc-lattice-1.29.153/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-vpc-lattice
-Version: 1.29.152
+Version: 1.29.153
 Summary: vpc-lattice data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-vpc-lattice-1.29.152/botocore/data/vpc-lattice/2022-11-30/endpoint-rule-set-1.json` & `botocore-a-la-carte-vpc-lattice-1.29.153/botocore/data/vpc-lattice/2022-11-30/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-vpc-lattice-1.29.152/botocore/data/vpc-lattice/2022-11-30/paginators-1.json` & `botocore-a-la-carte-vpc-lattice-1.29.153/botocore/data/vpc-lattice/2022-11-30/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-vpc-lattice-1.29.152/botocore/data/vpc-lattice/2022-11-30/service-2.json` & `botocore-a-la-carte-vpc-lattice-1.29.153/botocore/data/vpc-lattice/2022-11-30/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-vpc-lattice-1.29.152/botocore_a_la_carte_vpc_lattice.egg-info/PKG-INFO` & `botocore-a-la-carte-vpc-lattice-1.29.153/botocore_a_la_carte_vpc_lattice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-vpc-lattice
-Version: 1.29.152
+Version: 1.29.153
 Summary: vpc-lattice data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-vpc-lattice-1.29.152/setup.py` & `botocore-a-la-carte-vpc-lattice-1.29.153/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-vpc-lattice',
-    version="1.29.152",
+    version="1.29.153",
     description='vpc-lattice data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/vpc-lattice/*/*.json'],
```

