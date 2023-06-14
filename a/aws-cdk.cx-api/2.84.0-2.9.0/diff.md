# Comparing `tmp/aws-cdk.cx-api-2.84.0.tar.gz` & `tmp/aws-cdk.cx-api-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/cx-api/dist/python/aws-cdk.cx-api-2.84.0.tar", last modified: Tue Jun 13 23:47:06 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/@aws-cdk/cx-api/dist/python/aws-cdk.cx-api-2.9.0.tar", last modified: Wed Jan 26 10:30:25 2022, max compression
```

## Comparing `aws-cdk.cx-api-2.84.0.tar` & `aws-cdk.cx-api-2.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.cx-api-2.84.0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:57.000000 aws-cdk.cx-api-2.84.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:57.000000 aws-cdk.cx-api-2.84.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2718 2023-06-13 23:46:57.000000 aws-cdk.cx-api-2.84.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8250 2023-06-13 23:47:06.000000 aws-cdk.cx-api-2.84.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7266 2023-06-13 23:46:57.000000 aws-cdk.cx-api-2.84.0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:57.000000 aws-cdk.cx-api-2.84.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:47:06.000000 aws-cdk.cx-api-2.84.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1768 2023-06-13 23:46:57.000000 aws-cdk.cx-api-2.84.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.cx-api-2.84.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.cx-api-2.84.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.cx-api-2.84.0/src/aws_cdk/cx_api/
--rw-r--r--   0 root         (0) root         (0)   174545 2023-06-13 23:46:57.000000 aws-cdk.cx-api-2.84.0/src/aws_cdk/cx_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.cx-api-2.84.0/src/aws_cdk/cx_api/_jsii/
--rw-r--r--   0 root         (0) root         (0)      388 2023-06-13 23:46:57.000000 aws-cdk.cx-api-2.84.0/src/aws_cdk/cx_api/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   200952 2023-06-13 23:46:57.000000 aws-cdk.cx-api-2.84.0/src/aws_cdk/cx_api/_jsii/cx-api@2.84.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:57.000000 aws-cdk.cx-api-2.84.0/src/aws_cdk/cx_api/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.cx-api-2.84.0/src/aws_cdk.cx_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8250 2023-06-13 23:47:05.000000 aws-cdk.cx-api-2.84.0/src/aws_cdk.cx_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      413 2023-06-13 23:47:06.000000 aws-cdk.cx-api-2.84.0/src/aws_cdk.cx_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:47:05.000000 aws-cdk.cx-api-2.84.0/src/aws_cdk.cx_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-06-13 23:47:05.000000 aws-cdk.cx-api-2.84.0/src/aws_cdk.cx_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:47:05.000000 aws-cdk.cx-api-2.84.0/src/aws_cdk.cx_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:25.000000 aws-cdk.cx-api-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 10:30:21.000000 aws-cdk.cx-api-2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 10:30:21.000000 aws-cdk.cx-api-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2700 2022-01-26 10:30:21.000000 aws-cdk.cx-api-2.9.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1251 2022-01-26 10:30:25.000000 aws-cdk.cx-api-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      300 2022-01-26 10:30:21.000000 aws-cdk.cx-api-2.9.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 10:30:21.000000 aws-cdk.cx-api-2.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 10:30:25.000000 aws-cdk.cx-api-2.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1685 2022-01-26 10:30:21.000000 aws-cdk.cx-api-2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:25.000000 aws-cdk.cx-api-2.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:25.000000 aws-cdk.cx-api-2.9.0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:25.000000 aws-cdk.cx-api-2.9.0/src/aws_cdk/cx_api/
+-rw-r--r--   0 root         (0) root         (0)   119177 2022-01-26 10:30:21.000000 aws-cdk.cx-api-2.9.0/src/aws_cdk/cx_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:25.000000 aws-cdk.cx-api-2.9.0/src/aws_cdk/cx_api/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      352 2022-01-26 10:30:21.000000 aws-cdk.cx-api-2.9.0/src/aws_cdk/cx_api/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   131461 2022-01-26 10:30:21.000000 aws-cdk.cx-api-2.9.0/src/aws_cdk/cx_api/_jsii/cx-api@2.9.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 10:30:21.000000 aws-cdk.cx-api-2.9.0/src/aws_cdk/cx_api/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:25.000000 aws-cdk.cx-api-2.9.0/src/aws_cdk.cx_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1251 2022-01-26 10:30:25.000000 aws-cdk.cx-api-2.9.0/src/aws_cdk.cx_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2022-01-26 10:30:25.000000 aws-cdk.cx-api-2.9.0/src/aws_cdk.cx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 10:30:25.000000 aws-cdk.cx-api-2.9.0/src/aws_cdk.cx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2022-01-26 10:30:25.000000 aws-cdk.cx-api-2.9.0/src/aws_cdk.cx_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 10:30:25.000000 aws-cdk.cx-api-2.9.0/src/aws_cdk.cx_api.egg-info/top_level.txt
```

### Comparing `aws-cdk.cx-api-2.84.0/LICENSE` & `aws-cdk.cx-api-2.9.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2018-2023 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+   Copyright 2018-2022 Amazon.com, Inc. or its affiliates. All Rights Reserved.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `aws-cdk.cx-api-2.84.0/NOTICE` & `aws-cdk.cx-api-2.9.0/NOTICE`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 AWS Cloud Development Kit (AWS CDK)
-Copyright 2018-2023 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+Copyright 2018-2022 Amazon.com, Inc. or its affiliates. All Rights Reserved.
 
 -------------------------------------------------------------------------------
 
 The AWS CDK includes the following third-party software/licensing:
 
 ** semver - https://www.npmjs.com/package/semver
 Copyright (c) Isaac Z. Schlueter and Contributors
@@ -49,9 +49,7 @@
 THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
 WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR
 IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
-
-----------------
```

### Comparing `aws-cdk.cx-api-2.84.0/setup.py` & `aws-cdk.cx-api-2.9.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.cx-api",
-    "version": "2.84.0",
+    "version": "2.9.0",
     "description": "Cloud executable protocol",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,42 +22,40 @@
     },
     "packages": [
         "aws_cdk.cx_api",
         "aws_cdk.cx_api._jsii"
     ],
     "package_data": {
         "aws_cdk.cx_api._jsii": [
-            "cx-api@2.84.0.jsii.tgz"
+            "cx-api@2.9.0.jsii.tgz"
         ],
         "aws_cdk.cx_api": [
             "py.typed"
         ]
     },
-    "python_requires": "~=3.7",
+    "python_requires": ">=3.6",
     "install_requires": [
-        "aws-cdk.cloud-assembly-schema==2.84.0",
-        "jsii>=1.82.0, <2.0.0",
-        "publication>=0.0.3",
-        "typeguard~=2.13.3"
+        "aws-cdk.cloud-assembly-schema==2.9.0",
+        "jsii>=1.52.1, <2.0.0",
+        "publication>=0.0.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved",
         "Framework :: AWS CDK",
-        "Framework :: AWS CDK :: 2"
+        "Framework :: AWS CDK :: 1"
     ],
     "scripts": []
 }
 """
 )
 
 with open("README.md", encoding="utf8") as fp:
```

