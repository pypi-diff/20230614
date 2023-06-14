# Comparing `tmp/pwrdrvr.microapps.cdk-0.4.0a8.tar.gz` & `tmp/pwrdrvr.microapps.cdk-0.4.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwrdrvr.microapps.cdk-0.4.0a8.tar", last modified: Thu Apr  6 02:18:36 2023, max compression
+gzip compressed data, was "pwrdrvr.microapps.cdk-0.4.0a9.tar", last modified: Fri Apr 21 00:08:33 2023, max compression
```

## Comparing `pwrdrvr.microapps.cdk-0.4.0a8.tar` & `pwrdrvr.microapps.cdk-0.4.0a9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:18:36.413425 pwrdrvr.microapps.cdk-0.4.0a8/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-06 02:18:24.000000 pwrdrvr.microapps.cdk-0.4.0a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-06 02:18:24.000000 pwrdrvr.microapps.cdk-0.4.0a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19198 2023-04-06 02:18:36.413425 pwrdrvr.microapps.cdk-0.4.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-04-06 02:18:24.000000 pwrdrvr.microapps.cdk-0.4.0a8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-06 02:18:24.000000 pwrdrvr.microapps.cdk-0.4.0a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 02:18:36.413425 pwrdrvr.microapps.cdk-0.4.0a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-06 02:18:24.000000 pwrdrvr.microapps.cdk-0.4.0a8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:18:36.409425 pwrdrvr.microapps.cdk-0.4.0a8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:18:36.409425 pwrdrvr.microapps.cdk-0.4.0a8/src/pwrdrvr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:18:36.409425 pwrdrvr.microapps.cdk-0.4.0a8/src/pwrdrvr/microapps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:18:36.413425 pwrdrvr.microapps.cdk-0.4.0a8/src/pwrdrvr/microapps/cdk/
--rw-r--r--   0 runner    (1001) docker     (123)   232677 2023-04-06 02:18:24.000000 pwrdrvr.microapps.cdk-0.4.0a8/src/pwrdrvr/microapps/cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:18:36.413425 pwrdrvr.microapps.cdk-0.4.0a8/src/pwrdrvr/microapps/cdk/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-06 02:18:24.000000 pwrdrvr.microapps.cdk-0.4.0a8/src/pwrdrvr/microapps/cdk/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2655749 2023-04-06 02:18:24.000000 pwrdrvr.microapps.cdk-0.4.0a8/src/pwrdrvr/microapps/cdk/_jsii/microapps-cdk@0.4.0-alpha.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 02:18:24.000000 pwrdrvr.microapps.cdk-0.4.0a8/src/pwrdrvr/microapps/cdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:18:36.409425 pwrdrvr.microapps.cdk-0.4.0a8/src/pwrdrvr.microapps.cdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19198 2023-04-06 02:18:36.000000 pwrdrvr.microapps.cdk-0.4.0a8/src/pwrdrvr.microapps.cdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-06 02:18:36.000000 pwrdrvr.microapps.cdk-0.4.0a8/src/pwrdrvr.microapps.cdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 02:18:36.000000 pwrdrvr.microapps.cdk-0.4.0a8/src/pwrdrvr.microapps.cdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-06 02:18:36.000000 pwrdrvr.microapps.cdk-0.4.0a8/src/pwrdrvr.microapps.cdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-06 02:18:36.000000 pwrdrvr.microapps.cdk-0.4.0a8/src/pwrdrvr.microapps.cdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:33.674155 pwrdrvr.microapps.cdk-0.4.0a9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-21 00:08:17.000000 pwrdrvr.microapps.cdk-0.4.0a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 00:08:17.000000 pwrdrvr.microapps.cdk-0.4.0a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19198 2023-04-21 00:08:33.674155 pwrdrvr.microapps.cdk-0.4.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-04-21 00:08:17.000000 pwrdrvr.microapps.cdk-0.4.0a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-21 00:08:17.000000 pwrdrvr.microapps.cdk-0.4.0a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 00:08:33.674155 pwrdrvr.microapps.cdk-0.4.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-21 00:08:17.000000 pwrdrvr.microapps.cdk-0.4.0a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:33.670155 pwrdrvr.microapps.cdk-0.4.0a9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:33.670155 pwrdrvr.microapps.cdk-0.4.0a9/src/pwrdrvr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:33.670155 pwrdrvr.microapps.cdk-0.4.0a9/src/pwrdrvr/microapps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:33.670155 pwrdrvr.microapps.cdk-0.4.0a9/src/pwrdrvr/microapps/cdk/
+-rw-r--r--   0 runner    (1001) docker     (123)   232677 2023-04-21 00:08:17.000000 pwrdrvr.microapps.cdk-0.4.0a9/src/pwrdrvr/microapps/cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:33.670155 pwrdrvr.microapps.cdk-0.4.0a9/src/pwrdrvr/microapps/cdk/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-21 00:08:17.000000 pwrdrvr.microapps.cdk-0.4.0a9/src/pwrdrvr/microapps/cdk/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2658613 2023-04-21 00:08:17.000000 pwrdrvr.microapps.cdk-0.4.0a9/src/pwrdrvr/microapps/cdk/_jsii/microapps-cdk@0.4.0-alpha.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:08:17.000000 pwrdrvr.microapps.cdk-0.4.0a9/src/pwrdrvr/microapps/cdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:33.670155 pwrdrvr.microapps.cdk-0.4.0a9/src/pwrdrvr.microapps.cdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19198 2023-04-21 00:08:33.000000 pwrdrvr.microapps.cdk-0.4.0a9/src/pwrdrvr.microapps.cdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-21 00:08:33.000000 pwrdrvr.microapps.cdk-0.4.0a9/src/pwrdrvr.microapps.cdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:08:33.000000 pwrdrvr.microapps.cdk-0.4.0a9/src/pwrdrvr.microapps.cdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-21 00:08:33.000000 pwrdrvr.microapps.cdk-0.4.0a9/src/pwrdrvr.microapps.cdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 00:08:33.000000 pwrdrvr.microapps.cdk-0.4.0a9/src/pwrdrvr.microapps.cdk.egg-info/top_level.txt
```

### Comparing `pwrdrvr.microapps.cdk-0.4.0a8/LICENSE` & `pwrdrvr.microapps.cdk-0.4.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `pwrdrvr.microapps.cdk-0.4.0a8/PKG-INFO` & `pwrdrvr.microapps.cdk-0.4.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwrdrvr.microapps.cdk
-Version: 0.4.0a8
+Version: 0.4.0a9
 Summary: MicroApps framework, by PwrDrvr LLC, delivered as an AWS CDK construct that provides the DynamoDB, Router service, Deploy service, API Gateway, and CloudFront distribution.
 Home-page: https://github.com/pwrdrvr/microapps-core
 Author: PwrDrvr LLC<harold@pwrdrvr.com>
 License: MIT
 Project-URL: Source, https://github.com/pwrdrvr/microapps-core
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pwrdrvr.microapps.cdk-0.4.0a8/README.md` & `pwrdrvr.microapps.cdk-0.4.0a9/README.md`

 * *Files identical despite different names*

### Comparing `pwrdrvr.microapps.cdk-0.4.0a8/setup.py` & `pwrdrvr.microapps.cdk-0.4.0a9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "pwrdrvr.microapps.cdk",
-    "version": "0.4.0.a8",
+    "version": "0.4.0.a9",
     "description": "MicroApps framework, by PwrDrvr LLC, delivered as an AWS CDK construct that provides the DynamoDB, Router service, Deploy service, API Gateway, and CloudFront distribution.",
     "license": "MIT",
     "url": "https://github.com/pwrdrvr/microapps-core",
     "long_description_content_type": "text/markdown",
     "author": "PwrDrvr LLC<harold@pwrdrvr.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "pwrdrvr.microapps.cdk",
         "pwrdrvr.microapps.cdk._jsii"
     ],
     "package_data": {
         "pwrdrvr.microapps.cdk._jsii": [
-            "microapps-cdk@0.4.0-alpha.8.jsii.tgz"
+            "microapps-cdk@0.4.0-alpha.9.jsii.tgz"
         ],
         "pwrdrvr.microapps.cdk": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `pwrdrvr.microapps.cdk-0.4.0a8/src/pwrdrvr/microapps/cdk/__init__.py` & `pwrdrvr.microapps.cdk-0.4.0a9/src/pwrdrvr/microapps/cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `pwrdrvr.microapps.cdk-0.4.0a8/src/pwrdrvr/microapps/cdk/_jsii/__init__.py` & `pwrdrvr.microapps.cdk-0.4.0a9/src/pwrdrvr/microapps/cdk/_jsii/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 import aws_cdk.aws_apigatewayv2_alpha._jsii
 import aws_cdk.aws_apigatewayv2_authorizers_alpha._jsii
 import aws_cdk.aws_apigatewayv2_integrations_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@pwrdrvr/microapps-cdk",
-    "0.4.0-alpha.8",
+    "0.4.0-alpha.9",
     __name__[0:-6],
-    "microapps-cdk@0.4.0-alpha.8.jsii.tgz",
+    "microapps-cdk@0.4.0-alpha.9.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `pwrdrvr.microapps.cdk-0.4.0a8/src/pwrdrvr.microapps.cdk.egg-info/PKG-INFO` & `pwrdrvr.microapps.cdk-0.4.0a9/src/pwrdrvr.microapps.cdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwrdrvr.microapps.cdk
-Version: 0.4.0a8
+Version: 0.4.0a9
 Summary: MicroApps framework, by PwrDrvr LLC, delivered as an AWS CDK construct that provides the DynamoDB, Router service, Deploy service, API Gateway, and CloudFront distribution.
 Home-page: https://github.com/pwrdrvr/microapps-core
 Author: PwrDrvr LLC<harold@pwrdrvr.com>
 License: MIT
 Project-URL: Source, https://github.com/pwrdrvr/microapps-core
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

