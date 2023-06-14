# Comparing `tmp/aws-cdk.integ-tests-alpha-2.83.1a0.tar.gz` & `tmp/aws-cdk.integ-tests-alpha-2.84.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src629398401/src/packages/@aws-cdk/integ-tests-alpha/dist/python/aws-cdk.integ-tests-alpha-2.83.1a0.tar", last modified: Fri Jun  9 09:54:43 2023, max compression
+gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/integ-tests-alpha/dist/python/aws-cdk.integ-tests-alpha-2.84.0a0.tar", last modified: Tue Jun 13 23:46:46 2023, max compression
```

## Comparing `aws-cdk.integ-tests-alpha-2.83.1a0.tar` & `aws-cdk.integ-tests-alpha-2.84.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:54:43.000000 aws-cdk.integ-tests-alpha-2.83.1a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-09 09:54:35.000000 aws-cdk.integ-tests-alpha-2.83.1a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-09 09:54:35.000000 aws-cdk.integ-tests-alpha-2.83.1a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-09 09:54:35.000000 aws-cdk.integ-tests-alpha-2.83.1a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    16319 2023-06-09 09:54:43.000000 aws-cdk.integ-tests-alpha-2.83.1a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15326 2023-06-09 09:54:35.000000 aws-cdk.integ-tests-alpha-2.83.1a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-09 09:54:35.000000 aws-cdk.integ-tests-alpha-2.83.1a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 09:54:43.000000 aws-cdk.integ-tests-alpha-2.83.1a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1862 2023-06-09 09:54:35.000000 aws-cdk.integ-tests-alpha-2.83.1a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:54:43.000000 aws-cdk.integ-tests-alpha-2.83.1a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:54:43.000000 aws-cdk.integ-tests-alpha-2.83.1a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:54:43.000000 aws-cdk.integ-tests-alpha-2.83.1a0/src/aws_cdk/integ_tests_alpha/
--rw-r--r--   0 root         (0) root         (0)   225405 2023-06-09 09:54:35.000000 aws-cdk.integ-tests-alpha-2.83.1a0/src/aws_cdk/integ_tests_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:54:43.000000 aws-cdk.integ-tests-alpha-2.83.1a0/src/aws_cdk/integ_tests_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      441 2023-06-09 09:54:35.000000 aws-cdk.integ-tests-alpha-2.83.1a0/src/aws_cdk/integ_tests_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   147006 2023-06-09 09:54:35.000000 aws-cdk.integ-tests-alpha-2.83.1a0/src/aws_cdk/integ_tests_alpha/_jsii/integ-tests-alpha@2.83.1-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:54:35.000000 aws-cdk.integ-tests-alpha-2.83.1a0/src/aws_cdk/integ_tests_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:54:43.000000 aws-cdk.integ-tests-alpha-2.83.1a0/src/aws_cdk.integ_tests_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16319 2023-06-09 09:54:43.000000 aws-cdk.integ-tests-alpha-2.83.1a0/src/aws_cdk.integ_tests_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-09 09:54:43.000000 aws-cdk.integ-tests-alpha-2.83.1a0/src/aws_cdk.integ_tests_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:54:43.000000 aws-cdk.integ-tests-alpha-2.83.1a0/src/aws_cdk.integ_tests_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-09 09:54:43.000000 aws-cdk.integ-tests-alpha-2.83.1a0/src/aws_cdk.integ_tests_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-09 09:54:43.000000 aws-cdk.integ-tests-alpha-2.83.1a0/src/aws_cdk.integ_tests_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    16319 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15326 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1862 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk/integ_tests_alpha/
+-rw-r--r--   0 root         (0) root         (0)   225405 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk/integ_tests_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk/integ_tests_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk/integ_tests_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   146957 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk/integ_tests_alpha/_jsii/integ-tests-alpha@2.84.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk/integ_tests_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk.integ_tests_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16319 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk.integ_tests_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk.integ_tests_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk.integ_tests_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk.integ_tests_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk.integ_tests_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.integ-tests-alpha-2.83.1a0/LICENSE` & `aws-cdk.integ-tests-alpha-2.84.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.integ-tests-alpha-2.83.1a0/PKG-INFO` & `aws-cdk.integ-tests-alpha-2.84.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.integ-tests-alpha
-Version: 2.83.1a0
+Version: 2.84.0a0
 Summary: CDK Integration Testing Constructs
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.integ-tests-alpha-2.83.1a0/README.md` & `aws-cdk.integ-tests-alpha-2.84.0a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.integ-tests-alpha-2.83.1a0/setup.py` & `aws-cdk.integ-tests-alpha-2.84.0a0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.integ-tests-alpha",
-    "version": "2.83.1.a0",
+    "version": "2.84.0.a0",
     "description": "CDK Integration Testing Constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aws_cdk.integ_tests_alpha",
         "aws_cdk.integ_tests_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.integ_tests_alpha._jsii": [
-            "integ-tests-alpha@2.83.1-alpha.0.jsii.tgz"
+            "integ-tests-alpha@2.84.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.integ_tests_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.83.1",
+        "aws-cdk-lib==2.84.0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.integ-tests-alpha-2.83.1a0/src/aws_cdk/integ_tests_alpha/__init__.py` & `aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk/integ_tests_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.integ-tests-alpha-2.83.1a0/src/aws_cdk.integ_tests_alpha.egg-info/PKG-INFO` & `aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk.integ_tests_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.integ-tests-alpha
-Version: 2.83.1a0
+Version: 2.84.0a0
 Summary: CDK Integration Testing Constructs
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.integ-tests-alpha-2.83.1a0/src/aws_cdk.integ_tests_alpha.egg-info/SOURCES.txt` & `aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk.integ_tests_alpha.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.integ_tests_alpha.egg-info/SOURCES.txt
 src/aws_cdk.integ_tests_alpha.egg-info/dependency_links.txt
 src/aws_cdk.integ_tests_alpha.egg-info/requires.txt
 src/aws_cdk.integ_tests_alpha.egg-info/top_level.txt
 src/aws_cdk/integ_tests_alpha/__init__.py
 src/aws_cdk/integ_tests_alpha/py.typed
 src/aws_cdk/integ_tests_alpha/_jsii/__init__.py
-src/aws_cdk/integ_tests_alpha/_jsii/integ-tests-alpha@2.83.1-alpha.0.jsii.tgz
+src/aws_cdk/integ_tests_alpha/_jsii/integ-tests-alpha@2.84.0-alpha.0.jsii.tgz
```

