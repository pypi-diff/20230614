# Comparing `tmp/aws-cdk.cli-lib-alpha-2.83.1a0.tar.gz` & `tmp/aws-cdk.cli-lib-alpha-2.84.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src629398401/src/packages/@aws-cdk/cli-lib-alpha/dist/python/aws-cdk.cli-lib-alpha-2.83.1a0.tar", last modified: Fri Jun  9 09:54:45 2023, max compression
+gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/cli-lib-alpha/dist/python/aws-cdk.cli-lib-alpha-2.84.0a0.tar", last modified: Tue Jun 13 23:46:49 2023, max compression
```

## Comparing `aws-cdk.cli-lib-alpha-2.83.1a0.tar` & `aws-cdk.cli-lib-alpha-2.84.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:54:45.000000 aws-cdk.cli-lib-alpha-2.83.1a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-09 09:54:35.000000 aws-cdk.cli-lib-alpha-2.83.1a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-09 09:54:40.000000 aws-cdk.cli-lib-alpha-2.83.1a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      726 2023-06-09 09:54:37.000000 aws-cdk.cli-lib-alpha-2.83.1a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4179 2023-06-09 09:54:45.000000 aws-cdk.cli-lib-alpha-2.83.1a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3192 2023-06-09 09:54:40.000000 aws-cdk.cli-lib-alpha-2.83.1a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-09 09:54:40.000000 aws-cdk.cli-lib-alpha-2.83.1a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 09:54:45.000000 aws-cdk.cli-lib-alpha-2.83.1a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1766 2023-06-09 09:54:40.000000 aws-cdk.cli-lib-alpha-2.83.1a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:54:45.000000 aws-cdk.cli-lib-alpha-2.83.1a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:54:45.000000 aws-cdk.cli-lib-alpha-2.83.1a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:54:45.000000 aws-cdk.cli-lib-alpha-2.83.1a0/src/aws_cdk/cli_lib_alpha/
--rw-r--r--   0 root         (0) root         (0)   194202 2023-06-09 09:54:40.000000 aws-cdk.cli-lib-alpha-2.83.1a0/src/aws_cdk/cli_lib_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:54:45.000000 aws-cdk.cli-lib-alpha-2.83.1a0/src/aws_cdk/cli_lib_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      387 2023-06-09 09:54:40.000000 aws-cdk.cli-lib-alpha-2.83.1a0/src/aws_cdk/cli_lib_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)  3699112 2023-06-09 09:54:35.000000 aws-cdk.cli-lib-alpha-2.83.1a0/src/aws_cdk/cli_lib_alpha/_jsii/cli-lib-alpha@2.83.1-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:54:40.000000 aws-cdk.cli-lib-alpha-2.83.1a0/src/aws_cdk/cli_lib_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:54:45.000000 aws-cdk.cli-lib-alpha-2.83.1a0/src/aws_cdk.cli_lib_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4179 2023-06-09 09:54:45.000000 aws-cdk.cli-lib-alpha-2.83.1a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      491 2023-06-09 09:54:45.000000 aws-cdk.cli-lib-alpha-2.83.1a0/src/aws_cdk.cli_lib_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:54:45.000000 aws-cdk.cli-lib-alpha-2.83.1a0/src/aws_cdk.cli_lib_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-09 09:54:45.000000 aws-cdk.cli-lib-alpha-2.83.1a0/src/aws_cdk.cli_lib_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-09 09:54:45.000000 aws-cdk.cli-lib-alpha-2.83.1a0/src/aws_cdk.cli_lib_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:49.000000 aws-cdk.cli-lib-alpha-2.84.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:37.000000 aws-cdk.cli-lib-alpha-2.84.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:42.000000 aws-cdk.cli-lib-alpha-2.84.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-13 23:46:40.000000 aws-cdk.cli-lib-alpha-2.84.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-06-13 23:46:49.000000 aws-cdk.cli-lib-alpha-2.84.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-06-13 23:46:42.000000 aws-cdk.cli-lib-alpha-2.84.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:42.000000 aws-cdk.cli-lib-alpha-2.84.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:46:49.000000 aws-cdk.cli-lib-alpha-2.84.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-06-13 23:46:42.000000 aws-cdk.cli-lib-alpha-2.84.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:49.000000 aws-cdk.cli-lib-alpha-2.84.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:49.000000 aws-cdk.cli-lib-alpha-2.84.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:49.000000 aws-cdk.cli-lib-alpha-2.84.0a0/src/aws_cdk/cli_lib_alpha/
+-rw-r--r--   0 root         (0) root         (0)   194202 2023-06-13 23:46:42.000000 aws-cdk.cli-lib-alpha-2.84.0a0/src/aws_cdk/cli_lib_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:49.000000 aws-cdk.cli-lib-alpha-2.84.0a0/src/aws_cdk/cli_lib_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      387 2023-06-13 23:46:42.000000 aws-cdk.cli-lib-alpha-2.84.0a0/src/aws_cdk/cli_lib_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  3700915 2023-06-13 23:46:37.000000 aws-cdk.cli-lib-alpha-2.84.0a0/src/aws_cdk/cli_lib_alpha/_jsii/cli-lib-alpha@2.84.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:42.000000 aws-cdk.cli-lib-alpha-2.84.0a0/src/aws_cdk/cli_lib_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:49.000000 aws-cdk.cli-lib-alpha-2.84.0a0/src/aws_cdk.cli_lib_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-06-13 23:46:49.000000 aws-cdk.cli-lib-alpha-2.84.0a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      491 2023-06-13 23:46:49.000000 aws-cdk.cli-lib-alpha-2.84.0a0/src/aws_cdk.cli_lib_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:49.000000 aws-cdk.cli-lib-alpha-2.84.0a0/src/aws_cdk.cli_lib_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-13 23:46:49.000000 aws-cdk.cli-lib-alpha-2.84.0a0/src/aws_cdk.cli_lib_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:46:49.000000 aws-cdk.cli-lib-alpha-2.84.0a0/src/aws_cdk.cli_lib_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.cli-lib-alpha-2.83.1a0/LICENSE` & `aws-cdk.cli-lib-alpha-2.84.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.83.1a0/NOTICE` & `aws-cdk.cli-lib-alpha-2.84.0a0/NOTICE`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.83.1a0/PKG-INFO` & `aws-cdk.cli-lib-alpha-2.84.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cli-lib-alpha
-Version: 2.83.1a0
+Version: 2.84.0a0
 Summary: AWS CDK Programmatic CLI library
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.cli-lib-alpha-2.83.1a0/README.md` & `aws-cdk.cli-lib-alpha-2.84.0a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.83.1a0/setup.py` & `aws-cdk.cli-lib-alpha-2.84.0a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.cli-lib-alpha",
-    "version": "2.83.1.a0",
+    "version": "2.84.0.a0",
     "description": "AWS CDK Programmatic CLI library",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_cdk.cli_lib_alpha",
         "aws_cdk.cli_lib_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.cli_lib_alpha._jsii": [
-            "cli-lib-alpha@2.83.1-alpha.0.jsii.tgz"
+            "cli-lib-alpha@2.84.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.cli_lib_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-cdk.cli-lib-alpha-2.83.1a0/src/aws_cdk/cli_lib_alpha/__init__.py` & `aws-cdk.cli-lib-alpha-2.84.0a0/src/aws_cdk/cli_lib_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.83.1a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO` & `aws-cdk.cli-lib-alpha-2.84.0a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cli-lib-alpha
-Version: 2.83.1a0
+Version: 2.84.0a0
 Summary: AWS CDK Programmatic CLI library
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

