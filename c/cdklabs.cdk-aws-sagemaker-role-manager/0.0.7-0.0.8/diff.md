# Comparing `tmp/cdklabs.cdk-aws-sagemaker-role-manager-0.0.7.tar.gz` & `tmp/cdklabs.cdk-aws-sagemaker-role-manager-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.cdk-aws-sagemaker-role-manager-0.0.7.tar", last modified: Wed Jun 14 19:19:26 2023, max compression
+gzip compressed data, was "cdklabs.cdk-aws-sagemaker-role-manager-0.0.8.tar", last modified: Wed Jun 14 19:26:38 2023, max compression
```

## Comparing `cdklabs.cdk-aws-sagemaker-role-manager-0.0.7.tar` & `cdklabs.cdk-aws-sagemaker-role-manager-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:19:26.878718 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-14 19:19:13.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 19:19:13.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 19:19:13.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-06-14 19:19:26.878718 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-06-14 19:19:13.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-14 19:19:13.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 19:19:26.878718 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-14 19:19:13.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:19:26.878718 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:19:26.878718 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:19:26.878718 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/src/cdklabs/cdk_aws_sagemaker_role_manager/
--rw-r--r--   0 runner    (1001) docker     (123)   157030 2023-06-14 19:19:13.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/src/cdklabs/cdk_aws_sagemaker_role_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:19:26.878718 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-14 19:19:13.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57125 2023-06-14 19:19:13.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/cdk-aws-sagemaker-role-manager@0.0.7.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:19:13.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/src/cdklabs/cdk_aws_sagemaker_role_manager/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:19:26.878718 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-06-14 19:19:26.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-14 19:19:26.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:19:26.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-14 19:19:26.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 19:19:26.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:26:38.373669 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-06-14 19:26:38.373669 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 19:26:38.373669 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:26:38.373669 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:26:38.373669 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:26:38.373669 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs/cdk_aws_sagemaker_role_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)   157030 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs/cdk_aws_sagemaker_role_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:26:38.373669 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57129 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/cdk-aws-sagemaker-role-manager@0.0.8.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs/cdk_aws_sagemaker_role_manager/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:26:38.373669 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-06-14 19:26:38.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-14 19:26:38.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:26:38.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-14 19:26:38.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 19:26:38.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/top_level.txt
```

### Comparing `cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/LICENSE` & `cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/PKG-INFO` & `cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-aws-sagemaker-role-manager
-Version: 0.0.7
+Version: 0.0.8
 Summary: Create roles and policies for ML Activities and ML Personas
 Home-page: https://github.com/cdklabs/cdk-aws-sagemaker-role-manager
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-aws-sagemaker-role-manager
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/README.md` & `cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/setup.py` & `cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.cdk-aws-sagemaker-role-manager",
-    "version": "0.0.7",
+    "version": "0.0.8",
     "description": "Create roles and policies for ML Activities and ML Personas",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-aws-sagemaker-role-manager",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdklabs.cdk_aws_sagemaker_role_manager",
         "cdklabs.cdk_aws_sagemaker_role_manager._jsii"
     ],
     "package_data": {
         "cdklabs.cdk_aws_sagemaker_role_manager._jsii": [
-            "cdk-aws-sagemaker-role-manager@0.0.7.jsii.tgz"
+            "cdk-aws-sagemaker-role-manager@0.0.8.jsii.tgz"
         ],
         "cdklabs.cdk_aws_sagemaker_role_manager": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.83.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.83.0, <2.0.0",
+        "jsii>=1.84.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/src/cdklabs/cdk_aws_sagemaker_role_manager/__init__.py` & `cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs/cdk_aws_sagemaker_role_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/PKG-INFO` & `cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-aws-sagemaker-role-manager
-Version: 0.0.7
+Version: 0.0.8
 Summary: Create roles and policies for ML Activities and ML Personas
 Home-page: https://github.com/cdklabs/cdk-aws-sagemaker-role-manager
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-aws-sagemaker-role-manager
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.cdk-aws-sagemaker-role-manager-0.0.7/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/SOURCES.txt` & `cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/SOURCES.txt
 src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/dependency_links.txt
 src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/requires.txt
 src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/top_level.txt
 src/cdklabs/cdk_aws_sagemaker_role_manager/__init__.py
 src/cdklabs/cdk_aws_sagemaker_role_manager/py.typed
 src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/__init__.py
-src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/cdk-aws-sagemaker-role-manager@0.0.7.jsii.tgz
+src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/cdk-aws-sagemaker-role-manager@0.0.8.jsii.tgz
```

