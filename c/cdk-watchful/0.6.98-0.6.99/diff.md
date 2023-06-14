# Comparing `tmp/cdk-watchful-0.6.98.tar.gz` & `tmp/cdk-watchful-0.6.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-watchful-0.6.98.tar", last modified: Sun Apr 24 00:11:32 2022, max compression
+gzip compressed data, was "cdk-watchful-0.6.99.tar", last modified: Mon Apr 25 00:26:00 2022, max compression
```

## Comparing `cdk-watchful-0.6.98.tar` & `cdk-watchful-0.6.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 00:11:32.909822 cdk-watchful-0.6.98/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-04-24 00:11:16.000000 cdk-watchful-0.6.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-04-24 00:11:16.000000 cdk-watchful-0.6.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3482 2022-04-24 00:11:32.905822 cdk-watchful-0.6.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2576 2022-04-24 00:11:16.000000 cdk-watchful-0.6.98/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-04-24 00:11:16.000000 cdk-watchful-0.6.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-24 00:11:32.909822 cdk-watchful-0.6.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1691 2022-04-24 00:11:16.000000 cdk-watchful-0.6.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 00:11:32.905822 cdk-watchful-0.6.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 00:11:32.905822 cdk-watchful-0.6.98/src/cdk_watchful/
--rw-r--r--   0 runner    (1001) docker     (121)    90983 2022-04-24 00:11:16.000000 cdk-watchful-0.6.98/src/cdk_watchful/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 00:11:32.905822 cdk-watchful-0.6.98/src/cdk_watchful/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-04-24 00:11:16.000000 cdk-watchful-0.6.98/src/cdk_watchful/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   171169 2022-04-24 00:11:16.000000 cdk-watchful-0.6.98/src/cdk_watchful/_jsii/cdk-watchful@0.6.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-24 00:11:16.000000 cdk-watchful-0.6.98/src/cdk_watchful/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 00:11:32.905822 cdk-watchful-0.6.98/src/cdk_watchful.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3482 2022-04-24 00:11:32.000000 cdk-watchful-0.6.98/src/cdk_watchful.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-04-24 00:11:32.000000 cdk-watchful-0.6.98/src/cdk_watchful.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-24 00:11:32.000000 cdk-watchful-0.6.98/src/cdk_watchful.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-04-24 00:11:32.000000 cdk-watchful-0.6.98/src/cdk_watchful.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-24 00:11:32.000000 cdk-watchful-0.6.98/src/cdk_watchful.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 00:26:00.795865 cdk-watchful-0.6.99/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-04-25 00:25:48.000000 cdk-watchful-0.6.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-04-25 00:25:48.000000 cdk-watchful-0.6.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3482 2022-04-25 00:26:00.795865 cdk-watchful-0.6.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2576 2022-04-25 00:25:48.000000 cdk-watchful-0.6.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-04-25 00:25:48.000000 cdk-watchful-0.6.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-25 00:26:00.795865 cdk-watchful-0.6.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1691 2022-04-25 00:25:48.000000 cdk-watchful-0.6.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 00:26:00.795865 cdk-watchful-0.6.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 00:26:00.795865 cdk-watchful-0.6.99/src/cdk_watchful/
+-rw-r--r--   0 runner    (1001) docker     (121)    90983 2022-04-25 00:25:48.000000 cdk-watchful-0.6.99/src/cdk_watchful/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 00:26:00.795865 cdk-watchful-0.6.99/src/cdk_watchful/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2022-04-25 00:25:48.000000 cdk-watchful-0.6.99/src/cdk_watchful/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   171167 2022-04-25 00:25:48.000000 cdk-watchful-0.6.99/src/cdk_watchful/_jsii/cdk-watchful@0.6.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-25 00:25:48.000000 cdk-watchful-0.6.99/src/cdk_watchful/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 00:26:00.795865 cdk-watchful-0.6.99/src/cdk_watchful.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3482 2022-04-25 00:26:00.000000 cdk-watchful-0.6.99/src/cdk_watchful.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2022-04-25 00:26:00.000000 cdk-watchful-0.6.99/src/cdk_watchful.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-25 00:26:00.000000 cdk-watchful-0.6.99/src/cdk_watchful.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-04-25 00:26:00.000000 cdk-watchful-0.6.99/src/cdk_watchful.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-25 00:26:00.000000 cdk-watchful-0.6.99/src/cdk_watchful.egg-info/top_level.txt
```

### Comparing `cdk-watchful-0.6.98/LICENSE` & `cdk-watchful-0.6.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-watchful-0.6.98/PKG-INFO` & `cdk-watchful-0.6.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-watchful
-Version: 0.6.98
+Version: 0.6.99
 Summary: Watching your CDK apps since 2019
 Home-page: https://github.com/eladb/cdk-watchful.git
 Author: Elad Ben-Israel<elad.benisrael@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/eladb/cdk-watchful.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-watchful-0.6.98/README.md` & `cdk-watchful-0.6.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk-watchful-0.6.98/setup.py` & `cdk-watchful-0.6.99/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-watchful",
-    "version": "0.6.98",
+    "version": "0.6.99",
     "description": "Watching your CDK apps since 2019",
     "license": "Apache-2.0",
     "url": "https://github.com/eladb/cdk-watchful.git",
     "long_description_content_type": "text/markdown",
     "author": "Elad Ben-Israel<elad.benisrael@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_watchful",
         "cdk_watchful._jsii"
     ],
     "package_data": {
         "cdk_watchful._jsii": [
-            "cdk-watchful@0.6.98.jsii.tgz"
+            "cdk-watchful@0.6.99.jsii.tgz"
         ],
         "cdk_watchful": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
```

### Comparing `cdk-watchful-0.6.98/src/cdk_watchful/__init__.py` & `cdk-watchful-0.6.99/src/cdk_watchful/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-watchful-0.6.98/src/cdk_watchful.egg-info/PKG-INFO` & `cdk-watchful-0.6.99/src/cdk_watchful.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-watchful
-Version: 0.6.98
+Version: 0.6.99
 Summary: Watching your CDK apps since 2019
 Home-page: https://github.com/eladb/cdk-watchful.git
 Author: Elad Ben-Israel<elad.benisrael@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/eladb/cdk-watchful.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

