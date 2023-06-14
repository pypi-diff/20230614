# Comparing `tmp/everdrop-aws-cdk-constructs-0.0.82.tar.gz` & `tmp/everdrop-aws-cdk-constructs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "everdrop-aws-cdk-constructs-0.0.82.tar", last modified: Wed Jun 14 00:31:20 2023, max compression
+gzip compressed data, was "everdrop-aws-cdk-constructs-0.0.9.tar", last modified: Sun Mar 19 00:36:36 2023, max compression
```

## Comparing `everdrop-aws-cdk-constructs-0.0.82.tar` & `everdrop-aws-cdk-constructs-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:31:20.633016 everdrop-aws-cdk-constructs-0.0.82/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-14 00:31:04.000000 everdrop-aws-cdk-constructs-0.0.82/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 00:31:04.000000 everdrop-aws-cdk-constructs-0.0.82/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-14 00:31:20.629016 everdrop-aws-cdk-constructs-0.0.82/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-14 00:31:04.000000 everdrop-aws-cdk-constructs-0.0.82/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-14 00:31:04.000000 everdrop-aws-cdk-constructs-0.0.82/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 00:31:20.633016 everdrop-aws-cdk-constructs-0.0.82/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-14 00:31:04.000000 everdrop-aws-cdk-constructs-0.0.82/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:31:20.629016 everdrop-aws-cdk-constructs-0.0.82/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:31:20.629016 everdrop-aws-cdk-constructs-0.0.82/src/everdrop_aws_cdk_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-06-14 00:31:04.000000 everdrop-aws-cdk-constructs-0.0.82/src/everdrop_aws_cdk_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:31:20.629016 everdrop-aws-cdk-constructs-0.0.82/src/everdrop_aws_cdk_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-14 00:31:04.000000 everdrop-aws-cdk-constructs-0.0.82/src/everdrop_aws_cdk_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-06-14 00:31:04.000000 everdrop-aws-cdk-constructs-0.0.82/src/everdrop_aws_cdk_constructs/_jsii/everdrop-aws-cdk-constructs@0.0.82.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:31:04.000000 everdrop-aws-cdk-constructs-0.0.82/src/everdrop_aws_cdk_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:31:20.629016 everdrop-aws-cdk-constructs-0.0.82/src/everdrop_aws_cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-14 00:31:20.000000 everdrop-aws-cdk-constructs-0.0.82/src/everdrop_aws_cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-14 00:31:20.000000 everdrop-aws-cdk-constructs-0.0.82/src/everdrop_aws_cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:31:20.000000 everdrop-aws-cdk-constructs-0.0.82/src/everdrop_aws_cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-14 00:31:20.000000 everdrop-aws-cdk-constructs-0.0.82/src/everdrop_aws_cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 00:31:20.000000 everdrop-aws-cdk-constructs-0.0.82/src/everdrop_aws_cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 00:36:36.395744 everdrop-aws-cdk-constructs-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-19 00:36:24.000000 everdrop-aws-cdk-constructs-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-19 00:36:24.000000 everdrop-aws-cdk-constructs-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-19 00:36:36.395744 everdrop-aws-cdk-constructs-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-19 00:36:24.000000 everdrop-aws-cdk-constructs-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-19 00:36:24.000000 everdrop-aws-cdk-constructs-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 00:36:36.395744 everdrop-aws-cdk-constructs-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-03-19 00:36:24.000000 everdrop-aws-cdk-constructs-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 00:36:36.391744 everdrop-aws-cdk-constructs-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 00:36:36.391744 everdrop-aws-cdk-constructs-0.0.9/src/everdrop_aws_cdk_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-03-19 00:36:24.000000 everdrop-aws-cdk-constructs-0.0.9/src/everdrop_aws_cdk_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 00:36:36.391744 everdrop-aws-cdk-constructs-0.0.9/src/everdrop_aws_cdk_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-19 00:36:24.000000 everdrop-aws-cdk-constructs-0.0.9/src/everdrop_aws_cdk_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-03-19 00:36:24.000000 everdrop-aws-cdk-constructs-0.0.9/src/everdrop_aws_cdk_constructs/_jsii/everdrop-aws-cdk-constructs@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 00:36:24.000000 everdrop-aws-cdk-constructs-0.0.9/src/everdrop_aws_cdk_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 00:36:36.391744 everdrop-aws-cdk-constructs-0.0.9/src/everdrop_aws_cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-19 00:36:36.000000 everdrop-aws-cdk-constructs-0.0.9/src/everdrop_aws_cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-19 00:36:36.000000 everdrop-aws-cdk-constructs-0.0.9/src/everdrop_aws_cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 00:36:36.000000 everdrop-aws-cdk-constructs-0.0.9/src/everdrop_aws_cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-19 00:36:36.000000 everdrop-aws-cdk-constructs-0.0.9/src/everdrop_aws_cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-19 00:36:36.000000 everdrop-aws-cdk-constructs-0.0.9/src/everdrop_aws_cdk_constructs.egg-info/top_level.txt
```

### Comparing `everdrop-aws-cdk-constructs-0.0.82/LICENSE` & `everdrop-aws-cdk-constructs-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `everdrop-aws-cdk-constructs-0.0.82/PKG-INFO` & `everdrop-aws-cdk-constructs-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everdrop-aws-cdk-constructs
-Version: 0.0.82
+Version: 0.0.9
 Summary: Package provides opinionated constrcuts for common patterns used in everdrop infrastructure
 Home-page: https://github.com/everdropde/ed-aws-cdk-constructs.git
 Author: Fabian Bosler<FBosler@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/everdropde/ed-aws-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `everdrop-aws-cdk-constructs-0.0.82/setup.py` & `everdrop-aws-cdk-constructs-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "everdrop-aws-cdk-constructs",
-    "version": "0.0.82",
+    "version": "0.0.9",
     "description": "Package provides opinionated constrcuts for common patterns used in everdrop infrastructure",
     "license": "Apache-2.0",
     "url": "https://github.com/everdropde/ed-aws-cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Fabian Bosler<FBosler@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,26 @@
     },
     "packages": [
         "everdrop_aws_cdk_constructs",
         "everdrop_aws_cdk_constructs._jsii"
     ],
     "package_data": {
         "everdrop_aws_cdk_constructs._jsii": [
-            "everdrop-aws-cdk-constructs@0.0.82.jsii.tgz"
+            "everdrop-aws-cdk-constructs@0.0.9.jsii.tgz"
         ],
         "everdrop_aws_cdk_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.1.0, <3.0.0",
         "aws-solutions-constructs.core>=2.25.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.83.0, <2.0.0",
+        "jsii>=1.78.1, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `everdrop-aws-cdk-constructs-0.0.82/src/everdrop_aws_cdk_constructs/__init__.py` & `everdrop-aws-cdk-constructs-0.0.9/src/everdrop_aws_cdk_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `everdrop-aws-cdk-constructs-0.0.82/src/everdrop_aws_cdk_constructs.egg-info/PKG-INFO` & `everdrop-aws-cdk-constructs-0.0.9/src/everdrop_aws_cdk_constructs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everdrop-aws-cdk-constructs
-Version: 0.0.82
+Version: 0.0.9
 Summary: Package provides opinionated constrcuts for common patterns used in everdrop infrastructure
 Home-page: https://github.com/everdropde/ed-aws-cdk-constructs.git
 Author: Fabian Bosler<FBosler@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/everdropde/ed-aws-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `everdrop-aws-cdk-constructs-0.0.82/src/everdrop_aws_cdk_constructs.egg-info/SOURCES.txt` & `everdrop-aws-cdk-constructs-0.0.9/src/everdrop_aws_cdk_constructs.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/everdrop_aws_cdk_constructs/py.typed
 src/everdrop_aws_cdk_constructs.egg-info/PKG-INFO
 src/everdrop_aws_cdk_constructs.egg-info/SOURCES.txt
 src/everdrop_aws_cdk_constructs.egg-info/dependency_links.txt
 src/everdrop_aws_cdk_constructs.egg-info/requires.txt
 src/everdrop_aws_cdk_constructs.egg-info/top_level.txt
 src/everdrop_aws_cdk_constructs/_jsii/__init__.py
-src/everdrop_aws_cdk_constructs/_jsii/everdrop-aws-cdk-constructs@0.0.82.jsii.tgz
+src/everdrop_aws_cdk_constructs/_jsii/everdrop-aws-cdk-constructs@0.0.9.jsii.tgz
```

