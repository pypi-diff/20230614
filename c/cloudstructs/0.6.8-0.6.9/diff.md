# Comparing `tmp/cloudstructs-0.6.8.tar.gz` & `tmp/cloudstructs-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudstructs-0.6.8.tar", last modified: Mon Aug 29 12:26:23 2022, max compression
+gzip compressed data, was "cloudstructs-0.6.9.tar", last modified: Wed Aug 31 09:02:15 2022, max compression
```

## Comparing `cloudstructs-0.6.8.tar` & `cloudstructs-0.6.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 12:26:23.194462 cloudstructs-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-08-29 12:26:11.000000 cloudstructs-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-29 12:26:11.000000 cloudstructs-0.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-08-29 12:26:23.194462 cloudstructs-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-08-29 12:26:11.000000 cloudstructs-0.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-08-29 12:26:11.000000 cloudstructs-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-29 12:26:23.194462 cloudstructs-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-08-29 12:26:11.000000 cloudstructs-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 12:26:23.190462 cloudstructs-0.6.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 12:26:23.190462 cloudstructs-0.6.8/src/cloudstructs/
--rw-r--r--   0 runner    (1001) docker     (121)   138639 2022-08-29 12:26:11.000000 cloudstructs-0.6.8/src/cloudstructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 12:26:23.194462 cloudstructs-0.6.8/src/cloudstructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-08-29 12:26:11.000000 cloudstructs-0.6.8/src/cloudstructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)  2260752 2022-08-29 12:26:11.000000 cloudstructs-0.6.8/src/cloudstructs/_jsii/cloudstructs@0.6.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-29 12:26:11.000000 cloudstructs-0.6.8/src/cloudstructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 12:26:23.194462 cloudstructs-0.6.8/src/cloudstructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-08-29 12:26:22.000000 cloudstructs-0.6.8/src/cloudstructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-08-29 12:26:23.000000 cloudstructs-0.6.8/src/cloudstructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-29 12:26:22.000000 cloudstructs-0.6.8/src/cloudstructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-08-29 12:26:22.000000 cloudstructs-0.6.8/src/cloudstructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-29 12:26:23.000000 cloudstructs-0.6.8/src/cloudstructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 09:02:15.076312 cloudstructs-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-08-31 09:02:02.000000 cloudstructs-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-31 09:02:02.000000 cloudstructs-0.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-08-31 09:02:15.076312 cloudstructs-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-08-31 09:02:02.000000 cloudstructs-0.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-08-31 09:02:02.000000 cloudstructs-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-31 09:02:15.076312 cloudstructs-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-08-31 09:02:02.000000 cloudstructs-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 09:02:15.072312 cloudstructs-0.6.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 09:02:15.072312 cloudstructs-0.6.9/src/cloudstructs/
+-rw-r--r--   0 runner    (1001) docker     (121)   138639 2022-08-31 09:02:02.000000 cloudstructs-0.6.9/src/cloudstructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 09:02:15.072312 cloudstructs-0.6.9/src/cloudstructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      492 2022-08-31 09:02:02.000000 cloudstructs-0.6.9/src/cloudstructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)  2260749 2022-08-31 09:02:02.000000 cloudstructs-0.6.9/src/cloudstructs/_jsii/cloudstructs@0.6.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-31 09:02:02.000000 cloudstructs-0.6.9/src/cloudstructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 09:02:15.072312 cloudstructs-0.6.9/src/cloudstructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-08-31 09:02:14.000000 cloudstructs-0.6.9/src/cloudstructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-08-31 09:02:15.000000 cloudstructs-0.6.9/src/cloudstructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-31 09:02:14.000000 cloudstructs-0.6.9/src/cloudstructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-08-31 09:02:14.000000 cloudstructs-0.6.9/src/cloudstructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-31 09:02:14.000000 cloudstructs-0.6.9/src/cloudstructs.egg-info/top_level.txt
```

### Comparing `cloudstructs-0.6.8/LICENSE` & `cloudstructs-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudstructs-0.6.8/PKG-INFO` & `cloudstructs-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudstructs
-Version: 0.6.8
+Version: 0.6.9
 Summary: High-level constructs for AWS CDK
 Home-page: https://github.com/jogold/cloudstructs.git
 Author: Jonathan Goldwasser<jonathan.goldwasser@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/jogold/cloudstructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudstructs-0.6.8/README.md` & `cloudstructs-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `cloudstructs-0.6.8/setup.py` & `cloudstructs-0.6.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudstructs",
-    "version": "0.6.8",
+    "version": "0.6.9",
     "description": "High-level constructs for AWS CDK",
     "license": "Apache-2.0",
     "url": "https://github.com/jogold/cloudstructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Jonathan Goldwasser<jonathan.goldwasser@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudstructs",
         "cloudstructs._jsii"
     ],
     "package_data": {
         "cloudstructs._jsii": [
-            "cloudstructs@0.6.8.jsii.tgz"
+            "cloudstructs@0.6.9.jsii.tgz"
         ],
         "cloudstructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cloudstructs-0.6.8/src/cloudstructs/__init__.py` & `cloudstructs-0.6.9/src/cloudstructs/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudstructs-0.6.8/src/cloudstructs.egg-info/PKG-INFO` & `cloudstructs-0.6.9/src/cloudstructs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudstructs
-Version: 0.6.8
+Version: 0.6.9
 Summary: High-level constructs for AWS CDK
 Home-page: https://github.com/jogold/cloudstructs.git
 Author: Jonathan Goldwasser<jonathan.goldwasser@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/jogold/cloudstructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

