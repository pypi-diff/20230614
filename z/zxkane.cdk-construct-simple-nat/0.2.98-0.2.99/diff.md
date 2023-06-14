# Comparing `tmp/zxkane.cdk-construct-simple-nat-0.2.98.tar.gz` & `tmp/zxkane.cdk-construct-simple-nat-0.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zxkane.cdk-construct-simple-nat-0.2.98.tar", last modified: Wed Mar 23 00:17:16 2022, max compression
+gzip compressed data, was "zxkane.cdk-construct-simple-nat-0.2.99.tar", last modified: Thu Mar 24 00:16:15 2022, max compression
```

## Comparing `zxkane.cdk-construct-simple-nat-0.2.98.tar` & `zxkane.cdk-construct-simple-nat-0.2.99.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 00:17:16.612440 zxkane.cdk-construct-simple-nat-0.2.98/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-03-23 00:17:02.000000 zxkane.cdk-construct-simple-nat-0.2.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-03-23 00:17:02.000000 zxkane.cdk-construct-simple-nat-0.2.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3777 2022-03-23 00:17:16.612440 zxkane.cdk-construct-simple-nat-0.2.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2876 2022-03-23 00:17:02.000000 zxkane.cdk-construct-simple-nat-0.2.98/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-03-23 00:17:02.000000 zxkane.cdk-construct-simple-nat-0.2.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-23 00:17:16.612440 zxkane.cdk-construct-simple-nat-0.2.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1774 2022-03-23 00:17:02.000000 zxkane.cdk-construct-simple-nat-0.2.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 00:17:16.608440 zxkane.cdk-construct-simple-nat-0.2.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 00:17:16.608440 zxkane.cdk-construct-simple-nat-0.2.98/src/zxkane/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 00:17:16.608440 zxkane.cdk-construct-simple-nat-0.2.98/src/zxkane/cdk_construct_simple_nat/
--rw-r--r--   0 runner    (1001) docker     (121)    15285 2022-03-23 00:17:02.000000 zxkane.cdk-construct-simple-nat-0.2.98/src/zxkane/cdk_construct_simple_nat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 00:17:16.608440 zxkane.cdk-construct-simple-nat-0.2.98/src/zxkane/cdk_construct_simple_nat/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-03-23 00:17:02.000000 zxkane.cdk-construct-simple-nat-0.2.98/src/zxkane/cdk_construct_simple_nat/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   244802 2022-03-23 00:17:02.000000 zxkane.cdk-construct-simple-nat-0.2.98/src/zxkane/cdk_construct_simple_nat/_jsii/cdk-construct-simple-nat@0.2.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 00:17:02.000000 zxkane.cdk-construct-simple-nat-0.2.98/src/zxkane/cdk_construct_simple_nat/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 00:17:16.608440 zxkane.cdk-construct-simple-nat-0.2.98/src/zxkane.cdk_construct_simple_nat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3777 2022-03-23 00:17:16.000000 zxkane.cdk-construct-simple-nat-0.2.98/src/zxkane.cdk_construct_simple_nat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-03-23 00:17:16.000000 zxkane.cdk-construct-simple-nat-0.2.98/src/zxkane.cdk_construct_simple_nat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 00:17:16.000000 zxkane.cdk-construct-simple-nat-0.2.98/src/zxkane.cdk_construct_simple_nat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-03-23 00:17:16.000000 zxkane.cdk-construct-simple-nat-0.2.98/src/zxkane.cdk_construct_simple_nat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-23 00:17:16.000000 zxkane.cdk-construct-simple-nat-0.2.98/src/zxkane.cdk_construct_simple_nat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 00:16:15.051197 zxkane.cdk-construct-simple-nat-0.2.99/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-03-24 00:16:00.000000 zxkane.cdk-construct-simple-nat-0.2.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-03-24 00:16:00.000000 zxkane.cdk-construct-simple-nat-0.2.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3777 2022-03-24 00:16:15.051197 zxkane.cdk-construct-simple-nat-0.2.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2876 2022-03-24 00:16:00.000000 zxkane.cdk-construct-simple-nat-0.2.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-03-24 00:16:00.000000 zxkane.cdk-construct-simple-nat-0.2.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-24 00:16:15.051197 zxkane.cdk-construct-simple-nat-0.2.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1774 2022-03-24 00:16:00.000000 zxkane.cdk-construct-simple-nat-0.2.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 00:16:15.047197 zxkane.cdk-construct-simple-nat-0.2.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 00:16:15.047197 zxkane.cdk-construct-simple-nat-0.2.99/src/zxkane/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 00:16:15.051197 zxkane.cdk-construct-simple-nat-0.2.99/src/zxkane/cdk_construct_simple_nat/
+-rw-r--r--   0 runner    (1001) docker     (121)    15285 2022-03-24 00:16:00.000000 zxkane.cdk-construct-simple-nat-0.2.99/src/zxkane/cdk_construct_simple_nat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 00:16:15.051197 zxkane.cdk-construct-simple-nat-0.2.99/src/zxkane/cdk_construct_simple_nat/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2022-03-24 00:16:00.000000 zxkane.cdk-construct-simple-nat-0.2.99/src/zxkane/cdk_construct_simple_nat/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   244801 2022-03-24 00:16:00.000000 zxkane.cdk-construct-simple-nat-0.2.99/src/zxkane/cdk_construct_simple_nat/_jsii/cdk-construct-simple-nat@0.2.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-24 00:16:00.000000 zxkane.cdk-construct-simple-nat-0.2.99/src/zxkane/cdk_construct_simple_nat/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 00:16:15.051197 zxkane.cdk-construct-simple-nat-0.2.99/src/zxkane.cdk_construct_simple_nat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3777 2022-03-24 00:16:14.000000 zxkane.cdk-construct-simple-nat-0.2.99/src/zxkane.cdk_construct_simple_nat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      577 2022-03-24 00:16:14.000000 zxkane.cdk-construct-simple-nat-0.2.99/src/zxkane.cdk_construct_simple_nat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-24 00:16:14.000000 zxkane.cdk-construct-simple-nat-0.2.99/src/zxkane.cdk_construct_simple_nat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-03-24 00:16:14.000000 zxkane.cdk-construct-simple-nat-0.2.99/src/zxkane.cdk_construct_simple_nat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-24 00:16:14.000000 zxkane.cdk-construct-simple-nat-0.2.99/src/zxkane.cdk_construct_simple_nat.egg-info/top_level.txt
```

### Comparing `zxkane.cdk-construct-simple-nat-0.2.98/LICENSE` & `zxkane.cdk-construct-simple-nat-0.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `zxkane.cdk-construct-simple-nat-0.2.98/PKG-INFO` & `zxkane.cdk-construct-simple-nat-0.2.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zxkane.cdk-construct-simple-nat
-Version: 0.2.98
+Version: 0.2.99
 Summary: A CDK construct to build Simple NAT instance on AWS.
 Home-page: https://github.com/zxkane/snat
 Author: Kane Zhu<me@kane.mx>
 License: Apache-2.0
 Project-URL: Source, https://github.com/zxkane/snat
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `zxkane.cdk-construct-simple-nat-0.2.98/README.md` & `zxkane.cdk-construct-simple-nat-0.2.99/README.md`

 * *Files identical despite different names*

### Comparing `zxkane.cdk-construct-simple-nat-0.2.98/setup.py` & `zxkane.cdk-construct-simple-nat-0.2.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "zxkane.cdk-construct-simple-nat",
-    "version": "0.2.98",
+    "version": "0.2.99",
     "description": "A CDK construct to build Simple NAT instance on AWS.",
     "license": "Apache-2.0",
     "url": "https://github.com/zxkane/snat",
     "long_description_content_type": "text/markdown",
     "author": "Kane Zhu<me@kane.mx>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "zxkane.cdk_construct_simple_nat",
         "zxkane.cdk_construct_simple_nat._jsii"
     ],
     "package_data": {
         "zxkane.cdk_construct_simple_nat._jsii": [
-            "cdk-construct-simple-nat@0.2.98.jsii.tgz"
+            "cdk-construct-simple-nat@0.2.99.jsii.tgz"
         ],
         "zxkane.cdk_construct_simple_nat": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
```

### Comparing `zxkane.cdk-construct-simple-nat-0.2.98/src/zxkane/cdk_construct_simple_nat/__init__.py` & `zxkane.cdk-construct-simple-nat-0.2.99/src/zxkane/cdk_construct_simple_nat/__init__.py`

 * *Files identical despite different names*

### Comparing `zxkane.cdk-construct-simple-nat-0.2.98/src/zxkane.cdk_construct_simple_nat.egg-info/PKG-INFO` & `zxkane.cdk-construct-simple-nat-0.2.99/src/zxkane.cdk_construct_simple_nat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zxkane.cdk-construct-simple-nat
-Version: 0.2.98
+Version: 0.2.99
 Summary: A CDK construct to build Simple NAT instance on AWS.
 Home-page: https://github.com/zxkane/snat
 Author: Kane Zhu<me@kane.mx>
 License: Apache-2.0
 Project-URL: Source, https://github.com/zxkane/snat
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `zxkane.cdk-construct-simple-nat-0.2.98/src/zxkane.cdk_construct_simple_nat.egg-info/SOURCES.txt` & `zxkane.cdk-construct-simple-nat-0.2.99/src/zxkane.cdk_construct_simple_nat.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/zxkane.cdk_construct_simple_nat.egg-info/SOURCES.txt
 src/zxkane.cdk_construct_simple_nat.egg-info/dependency_links.txt
 src/zxkane.cdk_construct_simple_nat.egg-info/requires.txt
 src/zxkane.cdk_construct_simple_nat.egg-info/top_level.txt
 src/zxkane/cdk_construct_simple_nat/__init__.py
 src/zxkane/cdk_construct_simple_nat/py.typed
 src/zxkane/cdk_construct_simple_nat/_jsii/__init__.py
-src/zxkane/cdk_construct_simple_nat/_jsii/cdk-construct-simple-nat@0.2.98.jsii.tgz
+src/zxkane/cdk_construct_simple_nat/_jsii/cdk-construct-simple-nat@0.2.99.jsii.tgz
```

