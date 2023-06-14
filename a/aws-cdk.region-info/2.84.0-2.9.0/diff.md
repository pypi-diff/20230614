# Comparing `tmp/aws-cdk.region-info-2.84.0.tar.gz` & `tmp/aws-cdk.region-info-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/region-info/dist/python/aws-cdk.region-info-2.84.0.tar", last modified: Tue Jun 13 23:46:46 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/@aws-cdk/region-info/dist/python/aws-cdk.region-info-2.9.0.tar", last modified: Wed Jan 26 10:30:18 2022, max compression
```

## Comparing `aws-cdk.region-info-2.84.0.tar` & `aws-cdk.region-info-2.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.region-info-2.84.0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:37.000000 aws-cdk.region-info-2.84.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:37.000000 aws-cdk.region-info-2.84.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 23:46:37.000000 aws-cdk.region-info-2.84.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3487 2023-06-13 23:46:46.000000 aws-cdk.region-info-2.84.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2468 2023-06-13 23:46:37.000000 aws-cdk.region-info-2.84.0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:37.000000 aws-cdk.region-info-2.84.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:46:46.000000 aws-cdk.region-info-2.84.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1779 2023-06-13 23:46:37.000000 aws-cdk.region-info-2.84.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.region-info-2.84.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.region-info-2.84.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.region-info-2.84.0/src/aws_cdk/region_info/
--rw-r--r--   0 root         (0) root         (0)    34413 2023-06-13 23:46:37.000000 aws-cdk.region-info-2.84.0/src/aws_cdk/region_info/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.region-info-2.84.0/src/aws_cdk/region_info/_jsii/
--rw-r--r--   0 root         (0) root         (0)      354 2023-06-13 23:46:37.000000 aws-cdk.region-info-2.84.0/src/aws_cdk/region_info/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150359 2023-06-13 23:46:37.000000 aws-cdk.region-info-2.84.0/src/aws_cdk/region_info/_jsii/region-info@2.84.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:37.000000 aws-cdk.region-info-2.84.0/src/aws_cdk/region_info/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.region-info-2.84.0/src/aws_cdk.region_info.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3487 2023-06-13 23:46:46.000000 aws-cdk.region-info-2.84.0/src/aws_cdk.region_info.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      463 2023-06-13 23:46:46.000000 aws-cdk.region-info-2.84.0/src/aws_cdk.region_info.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:46.000000 aws-cdk.region-info-2.84.0/src/aws_cdk.region_info.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-13 23:46:46.000000 aws-cdk.region-info-2.84.0/src/aws_cdk.region_info.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:46:46.000000 aws-cdk.region-info-2.84.0/src/aws_cdk.region_info.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:18.000000 aws-cdk.region-info-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 10:30:14.000000 aws-cdk.region-info-2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 10:30:14.000000 aws-cdk.region-info-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 10:30:14.000000 aws-cdk.region-info-2.9.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4068 2022-01-26 10:30:18.000000 aws-cdk.region-info-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3082 2022-01-26 10:30:14.000000 aws-cdk.region-info-2.9.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 10:30:14.000000 aws-cdk.region-info-2.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 10:30:18.000000 aws-cdk.region-info-2.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1697 2022-01-26 10:30:14.000000 aws-cdk.region-info-2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:18.000000 aws-cdk.region-info-2.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:18.000000 aws-cdk.region-info-2.9.0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:18.000000 aws-cdk.region-info-2.9.0/src/aws_cdk/region_info/
+-rw-r--r--   0 root         (0) root         (0)    23975 2022-01-26 10:30:14.000000 aws-cdk.region-info-2.9.0/src/aws_cdk/region_info/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:18.000000 aws-cdk.region-info-2.9.0/src/aws_cdk/region_info/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      318 2022-01-26 10:30:14.000000 aws-cdk.region-info-2.9.0/src/aws_cdk/region_info/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77441 2022-01-26 10:30:14.000000 aws-cdk.region-info-2.9.0/src/aws_cdk/region_info/_jsii/region-info@2.9.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 10:30:14.000000 aws-cdk.region-info-2.9.0/src/aws_cdk/region_info/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:18.000000 aws-cdk.region-info-2.9.0/src/aws_cdk.region_info.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4068 2022-01-26 10:30:18.000000 aws-cdk.region-info-2.9.0/src/aws_cdk.region_info.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      462 2022-01-26 10:30:18.000000 aws-cdk.region-info-2.9.0/src/aws_cdk.region_info.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 10:30:18.000000 aws-cdk.region-info-2.9.0/src/aws_cdk.region_info.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2022-01-26 10:30:18.000000 aws-cdk.region-info-2.9.0/src/aws_cdk.region_info.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 10:30:18.000000 aws-cdk.region-info-2.9.0/src/aws_cdk.region_info.egg-info/top_level.txt
```

### Comparing `aws-cdk.region-info-2.84.0/LICENSE` & `aws-cdk.region-info-2.9.0/LICENSE`

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

### Comparing `aws-cdk.region-info-2.84.0/PKG-INFO` & `aws-cdk.region-info-2.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 Metadata-Version: 2.1
 Name: aws-cdk.region-info
-Version: 2.84.0
+Version: 2.9.0
 Summary: AWS region information, such as service principal names
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Classifier: Framework :: AWS CDK
-Classifier: Framework :: AWS CDK :: 2
-Requires-Python: ~=3.7
+Classifier: Framework :: AWS CDK :: 1
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # AWS Region-Specific Information Directory
 
+<!--BEGIN STABILITY BANNER-->---
+
+
+![cdk-constructs: Stable](https://img.shields.io/badge/cdk--constructs-stable-success.svg?style=for-the-badge)
+
+---
+<!--END STABILITY BANNER-->
+
 ## Usage
 
 Some information used in CDK Applications differs from one AWS region to
 another, such as service principals used in IAM policies, S3 static website
 endpoints, ...
 
 ### The `RegionInfo` class
 
 The library offers a simple interface to obtain region specific information in
 the form of the `RegionInfo` class. This is the preferred way to interact with
 the regional information database:
 
 ```python
+from aws_cdk.region_info import RegionInfo
+
 # Get the information for "eu-west-1":
-region = region_info.RegionInfo.get("eu-west-1")
+region = RegionInfo.get("eu-west-1")
 
 # Access attributes:
 region.s3_static_website_endpoint # s3-website-eu-west-1.amazonaws.com
 region.service_principal("logs.amazonaws.com")
 ```
 
 The `RegionInfo` layer is built on top of the Low-Level API, which is described
@@ -56,47 +66,55 @@
 
 This library offers a primitive database of such information so that CDK
 constructs can easily access regional information. The `FactName` class provides
 a list of known fact names, which can then be used with the `RegionInfo` to
 retrieve a particular value:
 
 ```python
+import aws_cdk.region_info as region_info
+
 code_deploy_principal = region_info.Fact.find("us-east-1", region_info.FactName.service_principal("codedeploy.amazonaws.com"))
 # => codedeploy.us-east-1.amazonaws.com
 
 static_website = region_info.Fact.find("ap-northeast-1", region_info.FactName.S3_STATIC_WEBSITE_ENDPOINT)
 ```
 
 ## Supplying new or missing information
 
 As new regions are released, it might happen that a particular fact you need is
 missing from the library. In such cases, the `Fact.register` method can be used
 to inject FactName into the database:
 
 ```python
-@jsii.implements(region_info.IFact)
-class MyFact:
-
-region_info.Fact.register(MyFact())
+# Example automatically generated from non-compiling source. May contain errors.
+region_info.Fact.register(
+    region="bermuda-triangle-1",
+    name=region_info.FactName.service_principal("s3.amazonaws.com"),
+    value="s3-website.bermuda-triangle-1.nowhere.com"
+)
 ```
 
 ## Overriding incorrect information
 
 In the event information provided by the library is incorrect, it can be
 overridden using the same `Fact.register` method demonstrated above, simply
 adding an extra boolean argument:
 
 ```python
-@jsii.implements(region_info.IFact)
-class MyFact:
-
-region_info.Fact.register(MyFact(), True)
+# Example automatically generated from non-compiling source. May contain errors.
+region_info.Fact.register({
+    "region": "us-east-1",
+    "name": region_info.FactName.service_principal("service.amazonaws.com"),
+    "value": "the-correct-principal.amazonaws.com"
+}, True)
 ```
 
 If you happen to have stumbled upon incorrect data built into this library, it
 is always a good idea to report your findings in a [GitHub issue](https://github.com/aws/aws-cdk/issues), so we can fix
 it for everyone else!
 
 ---
 
 
 This module is part of the [AWS Cloud Development Kit](https://github.com/aws/aws-cdk) project.
+
+
```

### Comparing `aws-cdk.region-info-2.84.0/README.md` & `aws-cdk.region-info-2.9.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 # AWS Region-Specific Information Directory
 
+<!--BEGIN STABILITY BANNER-->---
+
+
+![cdk-constructs: Stable](https://img.shields.io/badge/cdk--constructs-stable-success.svg?style=for-the-badge)
+
+---
+<!--END STABILITY BANNER-->
+
 ## Usage
 
 Some information used in CDK Applications differs from one AWS region to
 another, such as service principals used in IAM policies, S3 static website
 endpoints, ...
 
 ### The `RegionInfo` class
 
 The library offers a simple interface to obtain region specific information in
 the form of the `RegionInfo` class. This is the preferred way to interact with
 the regional information database:
 
 ```python
+from aws_cdk.region_info import RegionInfo
+
 # Get the information for "eu-west-1":
-region = region_info.RegionInfo.get("eu-west-1")
+region = RegionInfo.get("eu-west-1")
 
 # Access attributes:
 region.s3_static_website_endpoint # s3-website-eu-west-1.amazonaws.com
 region.service_principal("logs.amazonaws.com")
 ```
 
 The `RegionInfo` layer is built on top of the Low-Level API, which is described
@@ -29,44 +39,50 @@
 
 This library offers a primitive database of such information so that CDK
 constructs can easily access regional information. The `FactName` class provides
 a list of known fact names, which can then be used with the `RegionInfo` to
 retrieve a particular value:
 
 ```python
+import aws_cdk.region_info as region_info
+
 code_deploy_principal = region_info.Fact.find("us-east-1", region_info.FactName.service_principal("codedeploy.amazonaws.com"))
 # => codedeploy.us-east-1.amazonaws.com
 
 static_website = region_info.Fact.find("ap-northeast-1", region_info.FactName.S3_STATIC_WEBSITE_ENDPOINT)
 ```
 
 ## Supplying new or missing information
 
 As new regions are released, it might happen that a particular fact you need is
 missing from the library. In such cases, the `Fact.register` method can be used
 to inject FactName into the database:
 
 ```python
-@jsii.implements(region_info.IFact)
-class MyFact:
-
-region_info.Fact.register(MyFact())
+# Example automatically generated from non-compiling source. May contain errors.
+region_info.Fact.register(
+    region="bermuda-triangle-1",
+    name=region_info.FactName.service_principal("s3.amazonaws.com"),
+    value="s3-website.bermuda-triangle-1.nowhere.com"
+)
 ```
 
 ## Overriding incorrect information
 
 In the event information provided by the library is incorrect, it can be
 overridden using the same `Fact.register` method demonstrated above, simply
 adding an extra boolean argument:
 
 ```python
-@jsii.implements(region_info.IFact)
-class MyFact:
-
-region_info.Fact.register(MyFact(), True)
+# Example automatically generated from non-compiling source. May contain errors.
+region_info.Fact.register({
+    "region": "us-east-1",
+    "name": region_info.FactName.service_principal("service.amazonaws.com"),
+    "value": "the-correct-principal.amazonaws.com"
+}, True)
 ```
 
 If you happen to have stumbled upon incorrect data built into this library, it
 is always a good idea to report your findings in a [GitHub issue](https://github.com/aws/aws-cdk/issues), so we can fix
 it for everyone else!
 
 ---
```

### Comparing `aws-cdk.region-info-2.84.0/setup.py` & `aws-cdk.region-info-2.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.region-info",
-    "version": "2.84.0",
+    "version": "2.9.0",
     "description": "AWS region information, such as service principal names",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,41 +22,39 @@
     },
     "packages": [
         "aws_cdk.region_info",
         "aws_cdk.region_info._jsii"
     ],
     "package_data": {
         "aws_cdk.region_info._jsii": [
-            "region-info@2.84.0.jsii.tgz"
+            "region-info@2.9.0.jsii.tgz"
         ],
         "aws_cdk.region_info": [
             "py.typed"
         ]
     },
-    "python_requires": "~=3.7",
+    "python_requires": ">=3.6",
     "install_requires": [
-        "jsii>=1.82.0, <2.0.0",
-        "publication>=0.0.3",
-        "typeguard~=2.13.3"
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

### Comparing `aws-cdk.region-info-2.84.0/src/aws_cdk.region_info.egg-info/PKG-INFO` & `aws-cdk.region-info-2.9.0/src/aws_cdk.region_info.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 Metadata-Version: 2.1
 Name: aws-cdk.region-info
-Version: 2.84.0
+Version: 2.9.0
 Summary: AWS region information, such as service principal names
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Classifier: Framework :: AWS CDK
-Classifier: Framework :: AWS CDK :: 2
-Requires-Python: ~=3.7
+Classifier: Framework :: AWS CDK :: 1
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # AWS Region-Specific Information Directory
 
+<!--BEGIN STABILITY BANNER-->---
+
+
+![cdk-constructs: Stable](https://img.shields.io/badge/cdk--constructs-stable-success.svg?style=for-the-badge)
+
+---
+<!--END STABILITY BANNER-->
+
 ## Usage
 
 Some information used in CDK Applications differs from one AWS region to
 another, such as service principals used in IAM policies, S3 static website
 endpoints, ...
 
 ### The `RegionInfo` class
 
 The library offers a simple interface to obtain region specific information in
 the form of the `RegionInfo` class. This is the preferred way to interact with
 the regional information database:
 
 ```python
+from aws_cdk.region_info import RegionInfo
+
 # Get the information for "eu-west-1":
-region = region_info.RegionInfo.get("eu-west-1")
+region = RegionInfo.get("eu-west-1")
 
 # Access attributes:
 region.s3_static_website_endpoint # s3-website-eu-west-1.amazonaws.com
 region.service_principal("logs.amazonaws.com")
 ```
 
 The `RegionInfo` layer is built on top of the Low-Level API, which is described
@@ -56,47 +66,55 @@
 
 This library offers a primitive database of such information so that CDK
 constructs can easily access regional information. The `FactName` class provides
 a list of known fact names, which can then be used with the `RegionInfo` to
 retrieve a particular value:
 
 ```python
+import aws_cdk.region_info as region_info
+
 code_deploy_principal = region_info.Fact.find("us-east-1", region_info.FactName.service_principal("codedeploy.amazonaws.com"))
 # => codedeploy.us-east-1.amazonaws.com
 
 static_website = region_info.Fact.find("ap-northeast-1", region_info.FactName.S3_STATIC_WEBSITE_ENDPOINT)
 ```
 
 ## Supplying new or missing information
 
 As new regions are released, it might happen that a particular fact you need is
 missing from the library. In such cases, the `Fact.register` method can be used
 to inject FactName into the database:
 
 ```python
-@jsii.implements(region_info.IFact)
-class MyFact:
-
-region_info.Fact.register(MyFact())
+# Example automatically generated from non-compiling source. May contain errors.
+region_info.Fact.register(
+    region="bermuda-triangle-1",
+    name=region_info.FactName.service_principal("s3.amazonaws.com"),
+    value="s3-website.bermuda-triangle-1.nowhere.com"
+)
 ```
 
 ## Overriding incorrect information
 
 In the event information provided by the library is incorrect, it can be
 overridden using the same `Fact.register` method demonstrated above, simply
 adding an extra boolean argument:
 
 ```python
-@jsii.implements(region_info.IFact)
-class MyFact:
-
-region_info.Fact.register(MyFact(), True)
+# Example automatically generated from non-compiling source. May contain errors.
+region_info.Fact.register({
+    "region": "us-east-1",
+    "name": region_info.FactName.service_principal("service.amazonaws.com"),
+    "value": "the-correct-principal.amazonaws.com"
+}, True)
 ```
 
 If you happen to have stumbled upon incorrect data built into this library, it
 is always a good idea to report your findings in a [GitHub issue](https://github.com/aws/aws-cdk/issues), so we can fix
 it for everyone else!
 
 ---
 
 
 This module is part of the [AWS Cloud Development Kit](https://github.com/aws/aws-cdk) project.
+
+
```

