# Comparing `tmp/cdk-pipelines-github-0.4.87.tar.gz` & `tmp/cdk-pipelines-github-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-pipelines-github-0.4.87.tar", last modified: Wed Jun 14 00:20:25 2023, max compression
+gzip compressed data, was "cdk-pipelines-github-0.4.9.tar", last modified: Thu Mar 23 00:19:21 2023, max compression
```

## Comparing `cdk-pipelines-github-0.4.87.tar` & `cdk-pipelines-github-0.4.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:20:25.615224 cdk-pipelines-github-0.4.87/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-14 00:20:11.000000 cdk-pipelines-github-0.4.87/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 00:20:11.000000 cdk-pipelines-github-0.4.87/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 00:20:11.000000 cdk-pipelines-github-0.4.87/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    24130 2023-06-14 00:20:25.615224 cdk-pipelines-github-0.4.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-06-14 00:20:11.000000 cdk-pipelines-github-0.4.87/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-14 00:20:11.000000 cdk-pipelines-github-0.4.87/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 00:20:25.615224 cdk-pipelines-github-0.4.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-14 00:20:11.000000 cdk-pipelines-github-0.4.87/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:20:25.611224 cdk-pipelines-github-0.4.87/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:20:25.615224 cdk-pipelines-github-0.4.87/src/cdk_pipelines_github/
--rw-r--r--   0 runner    (1001) docker     (123)   312642 2023-06-14 00:20:11.000000 cdk-pipelines-github-0.4.87/src/cdk_pipelines_github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:20:25.615224 cdk-pipelines-github-0.4.87/src/cdk_pipelines_github/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-14 00:20:11.000000 cdk-pipelines-github-0.4.87/src/cdk_pipelines_github/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   325904 2023-06-14 00:20:11.000000 cdk-pipelines-github-0.4.87/src/cdk_pipelines_github/_jsii/cdk-pipelines-github@0.4.87.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:20:11.000000 cdk-pipelines-github-0.4.87/src/cdk_pipelines_github/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:20:25.615224 cdk-pipelines-github-0.4.87/src/cdk_pipelines_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24130 2023-06-14 00:20:25.000000 cdk-pipelines-github-0.4.87/src/cdk_pipelines_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-14 00:20:25.000000 cdk-pipelines-github-0.4.87/src/cdk_pipelines_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:20:25.000000 cdk-pipelines-github-0.4.87/src/cdk_pipelines_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-14 00:20:25.000000 cdk-pipelines-github-0.4.87/src/cdk_pipelines_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 00:20:25.000000 cdk-pipelines-github-0.4.87/src/cdk_pipelines_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 00:19:21.106676 cdk-pipelines-github-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-23 00:19:06.000000 cdk-pipelines-github-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-23 00:19:06.000000 cdk-pipelines-github-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-23 00:19:06.000000 cdk-pipelines-github-0.4.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    24129 2023-03-23 00:19:21.106676 cdk-pipelines-github-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-03-23 00:19:06.000000 cdk-pipelines-github-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-23 00:19:06.000000 cdk-pipelines-github-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 00:19:21.106676 cdk-pipelines-github-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-03-23 00:19:06.000000 cdk-pipelines-github-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 00:19:21.102676 cdk-pipelines-github-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 00:19:21.102676 cdk-pipelines-github-0.4.9/src/cdk_pipelines_github/
+-rw-r--r--   0 runner    (1001) docker     (123)   312642 2023-03-23 00:19:06.000000 cdk-pipelines-github-0.4.9/src/cdk_pipelines_github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 00:19:21.106676 cdk-pipelines-github-0.4.9/src/cdk_pipelines_github/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-23 00:19:06.000000 cdk-pipelines-github-0.4.9/src/cdk_pipelines_github/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   318236 2023-03-23 00:19:06.000000 cdk-pipelines-github-0.4.9/src/cdk_pipelines_github/_jsii/cdk-pipelines-github@0.4.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 00:19:06.000000 cdk-pipelines-github-0.4.9/src/cdk_pipelines_github/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 00:19:21.106676 cdk-pipelines-github-0.4.9/src/cdk_pipelines_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24129 2023-03-23 00:19:21.000000 cdk-pipelines-github-0.4.9/src/cdk_pipelines_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-23 00:19:21.000000 cdk-pipelines-github-0.4.9/src/cdk_pipelines_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 00:19:21.000000 cdk-pipelines-github-0.4.9/src/cdk_pipelines_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-23 00:19:21.000000 cdk-pipelines-github-0.4.9/src/cdk_pipelines_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-23 00:19:21.000000 cdk-pipelines-github-0.4.9/src/cdk_pipelines_github.egg-info/top_level.txt
```

### Comparing `cdk-pipelines-github-0.4.87/LICENSE` & `cdk-pipelines-github-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-pipelines-github-0.4.87/PKG-INFO` & `cdk-pipelines-github-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-pipelines-github
-Version: 0.4.87
+Version: 0.4.9
 Summary: GitHub Workflows support for CDK Pipelines
 Home-page: https://github.com/cdklabs/cdk-pipelines-github.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-pipelines-github.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-pipelines-github-0.4.87/README.md` & `cdk-pipelines-github-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk-pipelines-github-0.4.87/setup.py` & `cdk-pipelines-github-0.4.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-pipelines-github",
-    "version": "0.4.87",
+    "version": "0.4.9",
     "description": "GitHub Workflows support for CDK Pipelines",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-pipelines-github.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_pipelines_github",
         "cdk_pipelines_github._jsii"
     ],
     "package_data": {
         "cdk_pipelines_github._jsii": [
-            "cdk-pipelines-github@0.4.87.jsii.tgz"
+            "cdk-pipelines-github@0.4.9.jsii.tgz"
         ],
         "cdk_pipelines_github": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.9.0, <3.0.0",
         "constructs>=10.0.46, <11.0.0",
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

### Comparing `cdk-pipelines-github-0.4.87/src/cdk_pipelines_github/__init__.py` & `cdk-pipelines-github-0.4.9/src/cdk_pipelines_github/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-pipelines-github-0.4.87/src/cdk_pipelines_github.egg-info/PKG-INFO` & `cdk-pipelines-github-0.4.9/src/cdk_pipelines_github.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-pipelines-github
-Version: 0.4.87
+Version: 0.4.9
 Summary: GitHub Workflows support for CDK Pipelines
 Home-page: https://github.com/cdklabs/cdk-pipelines-github.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-pipelines-github.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

