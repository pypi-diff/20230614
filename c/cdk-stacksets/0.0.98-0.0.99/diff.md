# Comparing `tmp/cdk-stacksets-0.0.98.tar.gz` & `tmp/cdk-stacksets-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-stacksets-0.0.98.tar", last modified: Wed May 10 00:16:31 2023, max compression
+gzip compressed data, was "cdk-stacksets-0.0.99.tar", last modified: Thu May 11 00:15:46 2023, max compression
```

## Comparing `cdk-stacksets-0.0.98.tar` & `cdk-stacksets-0.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:16:31.248536 cdk-stacksets-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-10 00:16:16.000000 cdk-stacksets-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 00:16:16.000000 cdk-stacksets-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-10 00:16:31.248536 cdk-stacksets-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-05-10 00:16:16.000000 cdk-stacksets-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-10 00:16:16.000000 cdk-stacksets-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 00:16:31.248536 cdk-stacksets-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-10 00:16:16.000000 cdk-stacksets-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:16:31.244536 cdk-stacksets-0.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:16:31.248536 cdk-stacksets-0.0.98/src/cdk_stacksets/
--rw-r--r--   0 runner    (1001) docker     (123)    83981 2023-05-10 00:16:16.000000 cdk-stacksets-0.0.98/src/cdk_stacksets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:16:31.248536 cdk-stacksets-0.0.98/src/cdk_stacksets/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-10 00:16:16.000000 cdk-stacksets-0.0.98/src/cdk_stacksets/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71109 2023-05-10 00:16:16.000000 cdk-stacksets-0.0.98/src/cdk_stacksets/_jsii/cdk-stacksets@0.0.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 00:16:16.000000 cdk-stacksets-0.0.98/src/cdk_stacksets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:16:31.248536 cdk-stacksets-0.0.98/src/cdk_stacksets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-10 00:16:31.000000 cdk-stacksets-0.0.98/src/cdk_stacksets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-10 00:16:31.000000 cdk-stacksets-0.0.98/src/cdk_stacksets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 00:16:31.000000 cdk-stacksets-0.0.98/src/cdk_stacksets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-10 00:16:31.000000 cdk-stacksets-0.0.98/src/cdk_stacksets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 00:16:31.000000 cdk-stacksets-0.0.98/src/cdk_stacksets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:15:46.322186 cdk-stacksets-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-11 00:15:32.000000 cdk-stacksets-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 00:15:32.000000 cdk-stacksets-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-11 00:15:46.322186 cdk-stacksets-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-05-11 00:15:32.000000 cdk-stacksets-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-11 00:15:32.000000 cdk-stacksets-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 00:15:46.322186 cdk-stacksets-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-11 00:15:32.000000 cdk-stacksets-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:15:46.322186 cdk-stacksets-0.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:15:46.322186 cdk-stacksets-0.0.99/src/cdk_stacksets/
+-rw-r--r--   0 runner    (1001) docker     (123)    83981 2023-05-11 00:15:32.000000 cdk-stacksets-0.0.99/src/cdk_stacksets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:15:46.322186 cdk-stacksets-0.0.99/src/cdk_stacksets/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-11 00:15:32.000000 cdk-stacksets-0.0.99/src/cdk_stacksets/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71116 2023-05-11 00:15:32.000000 cdk-stacksets-0.0.99/src/cdk_stacksets/_jsii/cdk-stacksets@0.0.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:15:32.000000 cdk-stacksets-0.0.99/src/cdk_stacksets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:15:46.322186 cdk-stacksets-0.0.99/src/cdk_stacksets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-11 00:15:46.000000 cdk-stacksets-0.0.99/src/cdk_stacksets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-11 00:15:46.000000 cdk-stacksets-0.0.99/src/cdk_stacksets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:15:46.000000 cdk-stacksets-0.0.99/src/cdk_stacksets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-11 00:15:46.000000 cdk-stacksets-0.0.99/src/cdk_stacksets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 00:15:46.000000 cdk-stacksets-0.0.99/src/cdk_stacksets.egg-info/top_level.txt
```

### Comparing `cdk-stacksets-0.0.98/LICENSE` & `cdk-stacksets-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-stacksets-0.0.98/PKG-INFO` & `cdk-stacksets-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-stacksets
-Version: 0.0.98
+Version: 0.0.99
 Summary: cdk-stacksets
 Home-page: https://github.com/cdklabs/cdk-stacksets.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-stacksets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-stacksets-0.0.98/README.md` & `cdk-stacksets-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk-stacksets-0.0.98/setup.py` & `cdk-stacksets-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-stacksets",
-    "version": "0.0.98",
+    "version": "0.0.99",
     "description": "cdk-stacksets",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-stacksets.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_stacksets",
         "cdk_stacksets._jsii"
     ],
     "package_data": {
         "cdk_stacksets._jsii": [
-            "cdk-stacksets@0.0.98.jsii.tgz"
+            "cdk-stacksets@0.0.99.jsii.tgz"
         ],
         "cdk_stacksets": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.45.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.80.0, <2.0.0",
+        "jsii>=1.81.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-stacksets-0.0.98/src/cdk_stacksets/__init__.py` & `cdk-stacksets-0.0.99/src/cdk_stacksets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-stacksets-0.0.98/src/cdk_stacksets.egg-info/PKG-INFO` & `cdk-stacksets-0.0.99/src/cdk_stacksets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-stacksets
-Version: 0.0.98
+Version: 0.0.99
 Summary: cdk-stacksets
 Home-page: https://github.com/cdklabs/cdk-stacksets.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-stacksets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

