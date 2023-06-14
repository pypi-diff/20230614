# Comparing `tmp/aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0.tar.gz` & `tmp/aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/aws-kinesisanalytics-flink-alpha/dist/python/aws-cdk.aws-kinesisanalytics-", last modified: Tue Jun 13 23:47:04 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-kinesisanalytics-flink/dist/python/aws-cdk.aws-kinesisanaly", last modified: Wed Jan 26 11:22:06 2022, max compression
```

## Comparing `aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0.tar` & `aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:57.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:57.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 23:46:57.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5139 2023-06-13 23:47:04.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4101 2023-06-13 23:46:57.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:57.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:47:04.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1982 2023-06-13 23:46:57.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/src/aws_cdk/aws_kinesisanalytics_flink_alpha/
--rw-r--r--   0 root         (0) root         (0)   332684 2023-06-13 23:46:57.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/src/aws_cdk/aws_kinesisanalytics_flink_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/src/aws_cdk/aws_kinesisanalytics_flink_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      471 2023-06-13 23:46:57.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/src/aws_cdk/aws_kinesisanalytics_flink_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70985 2023-06-13 23:46:57.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/src/aws_cdk/aws_kinesisanalytics_flink_alpha/_jsii/aws-kinesisanalytics-flink-alpha@2.84.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:57.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/src/aws_cdk/aws_kinesisanalytics_flink_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5139 2023-06-13 23:47:04.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      681 2023-06-13 23:47:04.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:47:04.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-13 23:47:04.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:47:04.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4679 2022-01-26 11:22:06.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3674 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:06.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1907 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/src/aws_cdk/aws_kinesisanalytics_flink_alpha/
+-rw-r--r--   0 root         (0) root         (0)    53164 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/src/aws_cdk/aws_kinesisanalytics_flink_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/src/aws_cdk/aws_kinesisanalytics_flink_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      435 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/src/aws_cdk/aws_kinesisanalytics_flink_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45998 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/src/aws_cdk/aws_kinesisanalytics_flink_alpha/_jsii/aws-kinesisanalytics-flink-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/src/aws_cdk/aws_kinesisanalytics_flink_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4679 2022-01-26 11:22:06.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      680 2022-01-26 11:22:06.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:06.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:06.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:06.000000 aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/LICENSE` & `aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/LICENSE`

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

### Comparing `aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/PKG-INFO` & `aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-kinesisanalytics-flink-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: A CDK Construct Library for Kinesis Analytics Flink applications
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
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Classifier: Framework :: AWS CDK
-Classifier: Framework :: AWS CDK :: 2
-Requires-Python: ~=3.7
+Classifier: Framework :: AWS CDK :: 1
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # Kinesis Analytics Flink
 
 <!--BEGIN STABILITY BANNER-->---
@@ -40,40 +40,33 @@
 
 ---
 <!--END STABILITY BANNER-->
 
 This package provides constructs for creating Kinesis Analytics Flink
 applications. To learn more about using using managed Flink applications, see
 the [AWS developer
-guide](https://docs.aws.amazon.com/kinesisanalytics/latest/java/).
+guide](https://docs.aws.amazon.com/kinesisanalytics/latest/java/what-is.html).
 
 ## Creating Flink Applications
 
 To create a new Flink application, use the `Application` construct:
 
 ```python
 import path as path
-import aws_cdk.aws_cloudwatch as cloudwatch
 import aws_cdk as core
 import aws_cdk.aws_kinesisanalytics_flink_alpha as flink
 
 app = core.App()
 stack = core.Stack(app, "FlinkAppTest")
 
-flink_app = flink.Application(stack, "App",
+flink.Application(stack, "App",
     code=flink.ApplicationCode.from_asset(path.join(__dirname, "code-asset")),
     runtime=flink.Runtime.FLINK_1_11
 )
 
-cloudwatch.Alarm(stack, "Alarm",
-    metric=flink_app.metric_full_restarts(),
-    evaluation_periods=1,
-    threshold=3
-)
-
 app.synth()
 ```
 
 The `code` property can use `fromAsset` as shown above to reference a local jar
 file in s3 or `fromBucket` to reference a file in s3.
 
 ```python
@@ -104,54 +97,43 @@
 aws-kinesisanalytics-runtime library to [retrieve these
 properties](https://docs.aws.amazon.com/kinesisanalytics/latest/java/how-properties.html#how-properties-access).
 
 ```python
 # bucket: s3.Bucket
 
 flink_app = flink.Application(self, "Application",
-    property_groups={
-        "FlinkApplicationProperties": {
+    property_groups=flink.PropertyGroups(
+        FlinkApplicationProperties={
             "input_stream_name": "my-input-kinesis-stream",
             "output_stream_name": "my-output-kinesis-stream"
         }
-    },
+    ),
     # ...
-    runtime=flink.Runtime.FLINK_1_15,
+    runtime=flink.Runtime.FLINK_1_13,
     code=flink.ApplicationCode.from_bucket(bucket, "my-app.jar")
 )
 ```
 
 Flink applications also have specific configuration for passing parameters
 when the Flink job starts. These include parameters for checkpointing,
 snapshotting, monitoring, and parallelism.
 
 ```python
 # bucket: s3.Bucket
 
 flink_app = flink.Application(self, "Application",
     code=flink.ApplicationCode.from_bucket(bucket, "my-app.jar"),
-    runtime=flink.Runtime.FLINK_1_15,
+    runtime=flink.Runtime.FLINK_1_13,
     checkpointing_enabled=True,  # default is true
     checkpoint_interval=Duration.seconds(30),  # default is 1 minute
     min_pause_between_checkpoints=Duration.seconds(10),  # default is 5 seconds
     log_level=flink.LogLevel.ERROR,  # default is INFO
     metrics_level=flink.MetricsLevel.PARALLELISM,  # default is APPLICATION
     auto_scaling_enabled=False,  # default is true
     parallelism=32,  # default is 1
     parallelism_per_kpu=2,  # default is 1
     snapshots_enabled=False,  # default is true
     log_group=logs.LogGroup(self, "LogGroup")
 )
 ```
 
-Flink applications can optionally be deployed in a VPC:
-
-```python
-# bucket: s3.Bucket
-# vpc: ec2.Vpc
 
-flink_app = flink.Application(self, "Application",
-    code=flink.ApplicationCode.from_bucket(bucket, "my-app.jar"),
-    runtime=flink.Runtime.FLINK_1_15,
-    vpc=vpc
-)
-```
```

### Comparing `aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/README.md` & `aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,40 +13,33 @@
 
 ---
 <!--END STABILITY BANNER-->
 
 This package provides constructs for creating Kinesis Analytics Flink
 applications. To learn more about using using managed Flink applications, see
 the [AWS developer
-guide](https://docs.aws.amazon.com/kinesisanalytics/latest/java/).
+guide](https://docs.aws.amazon.com/kinesisanalytics/latest/java/what-is.html).
 
 ## Creating Flink Applications
 
 To create a new Flink application, use the `Application` construct:
 
 ```python
 import path as path
-import aws_cdk.aws_cloudwatch as cloudwatch
 import aws_cdk as core
 import aws_cdk.aws_kinesisanalytics_flink_alpha as flink
 
 app = core.App()
 stack = core.Stack(app, "FlinkAppTest")
 
-flink_app = flink.Application(stack, "App",
+flink.Application(stack, "App",
     code=flink.ApplicationCode.from_asset(path.join(__dirname, "code-asset")),
     runtime=flink.Runtime.FLINK_1_11
 )
 
-cloudwatch.Alarm(stack, "Alarm",
-    metric=flink_app.metric_full_restarts(),
-    evaluation_periods=1,
-    threshold=3
-)
-
 app.synth()
 ```
 
 The `code` property can use `fromAsset` as shown above to reference a local jar
 file in s3 or `fromBucket` to reference a file in s3.
 
 ```python
@@ -77,54 +70,41 @@
 aws-kinesisanalytics-runtime library to [retrieve these
 properties](https://docs.aws.amazon.com/kinesisanalytics/latest/java/how-properties.html#how-properties-access).
 
 ```python
 # bucket: s3.Bucket
 
 flink_app = flink.Application(self, "Application",
-    property_groups={
-        "FlinkApplicationProperties": {
+    property_groups=flink.PropertyGroups(
+        FlinkApplicationProperties={
             "input_stream_name": "my-input-kinesis-stream",
             "output_stream_name": "my-output-kinesis-stream"
         }
-    },
+    ),
     # ...
-    runtime=flink.Runtime.FLINK_1_15,
+    runtime=flink.Runtime.FLINK_1_13,
     code=flink.ApplicationCode.from_bucket(bucket, "my-app.jar")
 )
 ```
 
 Flink applications also have specific configuration for passing parameters
 when the Flink job starts. These include parameters for checkpointing,
 snapshotting, monitoring, and parallelism.
 
 ```python
 # bucket: s3.Bucket
 
 flink_app = flink.Application(self, "Application",
     code=flink.ApplicationCode.from_bucket(bucket, "my-app.jar"),
-    runtime=flink.Runtime.FLINK_1_15,
+    runtime=flink.Runtime.FLINK_1_13,
     checkpointing_enabled=True,  # default is true
     checkpoint_interval=Duration.seconds(30),  # default is 1 minute
     min_pause_between_checkpoints=Duration.seconds(10),  # default is 5 seconds
     log_level=flink.LogLevel.ERROR,  # default is INFO
     metrics_level=flink.MetricsLevel.PARALLELISM,  # default is APPLICATION
     auto_scaling_enabled=False,  # default is true
     parallelism=32,  # default is 1
     parallelism_per_kpu=2,  # default is 1
     snapshots_enabled=False,  # default is true
     log_group=logs.LogGroup(self, "LogGroup")
 )
 ```
-
-Flink applications can optionally be deployed in a VPC:
-
-```python
-# bucket: s3.Bucket
-# vpc: ec2.Vpc
-
-flink_app = flink.Application(self, "Application",
-    code=flink.ApplicationCode.from_bucket(bucket, "my-app.jar"),
-    runtime=flink.Runtime.FLINK_1_15,
-    vpc=vpc
-)
-```
```

### Comparing `aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/setup.py` & `aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-kinesisanalytics-flink-alpha",
-    "version": "2.84.0.a0",
+    "version": "2.9.0.a0",
     "description": "A CDK Construct Library for Kinesis Analytics Flink applications",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,43 +22,41 @@
     },
     "packages": [
         "aws_cdk.aws_kinesisanalytics_flink_alpha",
         "aws_cdk.aws_kinesisanalytics_flink_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_kinesisanalytics_flink_alpha._jsii": [
-            "aws-kinesisanalytics-flink-alpha@2.84.0-alpha.0.jsii.tgz"
+            "aws-kinesisanalytics-flink-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_kinesisanalytics_flink_alpha": [
             "py.typed"
         ]
     },
-    "python_requires": "~=3.7",
+    "python_requires": ">=3.6",
     "install_requires": [
-        "aws-cdk-lib==2.84.0",
+        "aws-cdk-lib>=2.9.0, <3.0.0",
         "constructs>=10.0.0, <11.0.0",
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
         "Development Status :: 4 - Beta",
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

### Comparing `aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-kinesisanalytics-flink-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: A CDK Construct Library for Kinesis Analytics Flink applications
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
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Classifier: Framework :: AWS CDK
-Classifier: Framework :: AWS CDK :: 2
-Requires-Python: ~=3.7
+Classifier: Framework :: AWS CDK :: 1
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # Kinesis Analytics Flink
 
 <!--BEGIN STABILITY BANNER-->---
@@ -40,40 +40,33 @@
 
 ---
 <!--END STABILITY BANNER-->
 
 This package provides constructs for creating Kinesis Analytics Flink
 applications. To learn more about using using managed Flink applications, see
 the [AWS developer
-guide](https://docs.aws.amazon.com/kinesisanalytics/latest/java/).
+guide](https://docs.aws.amazon.com/kinesisanalytics/latest/java/what-is.html).
 
 ## Creating Flink Applications
 
 To create a new Flink application, use the `Application` construct:
 
 ```python
 import path as path
-import aws_cdk.aws_cloudwatch as cloudwatch
 import aws_cdk as core
 import aws_cdk.aws_kinesisanalytics_flink_alpha as flink
 
 app = core.App()
 stack = core.Stack(app, "FlinkAppTest")
 
-flink_app = flink.Application(stack, "App",
+flink.Application(stack, "App",
     code=flink.ApplicationCode.from_asset(path.join(__dirname, "code-asset")),
     runtime=flink.Runtime.FLINK_1_11
 )
 
-cloudwatch.Alarm(stack, "Alarm",
-    metric=flink_app.metric_full_restarts(),
-    evaluation_periods=1,
-    threshold=3
-)
-
 app.synth()
 ```
 
 The `code` property can use `fromAsset` as shown above to reference a local jar
 file in s3 or `fromBucket` to reference a file in s3.
 
 ```python
@@ -104,54 +97,43 @@
 aws-kinesisanalytics-runtime library to [retrieve these
 properties](https://docs.aws.amazon.com/kinesisanalytics/latest/java/how-properties.html#how-properties-access).
 
 ```python
 # bucket: s3.Bucket
 
 flink_app = flink.Application(self, "Application",
-    property_groups={
-        "FlinkApplicationProperties": {
+    property_groups=flink.PropertyGroups(
+        FlinkApplicationProperties={
             "input_stream_name": "my-input-kinesis-stream",
             "output_stream_name": "my-output-kinesis-stream"
         }
-    },
+    ),
     # ...
-    runtime=flink.Runtime.FLINK_1_15,
+    runtime=flink.Runtime.FLINK_1_13,
     code=flink.ApplicationCode.from_bucket(bucket, "my-app.jar")
 )
 ```
 
 Flink applications also have specific configuration for passing parameters
 when the Flink job starts. These include parameters for checkpointing,
 snapshotting, monitoring, and parallelism.
 
 ```python
 # bucket: s3.Bucket
 
 flink_app = flink.Application(self, "Application",
     code=flink.ApplicationCode.from_bucket(bucket, "my-app.jar"),
-    runtime=flink.Runtime.FLINK_1_15,
+    runtime=flink.Runtime.FLINK_1_13,
     checkpointing_enabled=True,  # default is true
     checkpoint_interval=Duration.seconds(30),  # default is 1 minute
     min_pause_between_checkpoints=Duration.seconds(10),  # default is 5 seconds
     log_level=flink.LogLevel.ERROR,  # default is INFO
     metrics_level=flink.MetricsLevel.PARALLELISM,  # default is APPLICATION
     auto_scaling_enabled=False,  # default is true
     parallelism=32,  # default is 1
     parallelism_per_kpu=2,  # default is 1
     snapshots_enabled=False,  # default is true
     log_group=logs.LogGroup(self, "LogGroup")
 )
 ```
 
-Flink applications can optionally be deployed in a VPC:
-
-```python
-# bucket: s3.Bucket
-# vpc: ec2.Vpc
 
-flink_app = flink.Application(self, "Application",
-    code=flink.ApplicationCode.from_bucket(bucket, "my-app.jar"),
-    runtime=flink.Runtime.FLINK_1_15,
-    vpc=vpc
-)
-```
```

### Comparing `aws-cdk.aws-kinesisanalytics-flink-alpha-2.84.0a0/src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-kinesisanalytics-flink-alpha-2.9.0a0/src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/requires.txt
 src/aws_cdk.aws_kinesisanalytics_flink_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_kinesisanalytics_flink_alpha/__init__.py
 src/aws_cdk/aws_kinesisanalytics_flink_alpha/py.typed
 src/aws_cdk/aws_kinesisanalytics_flink_alpha/_jsii/__init__.py
-src/aws_cdk/aws_kinesisanalytics_flink_alpha/_jsii/aws-kinesisanalytics-flink-alpha@2.84.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_kinesisanalytics_flink_alpha/_jsii/aws-kinesisanalytics-flink-alpha@2.9.0-alpha.0.jsii.tgz
```

