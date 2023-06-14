# Comparing `tmp/aws-cdk.aws-synthetics-alpha-2.84.0a0.tar.gz` & `tmp/aws-cdk.aws-synthetics-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/aws-synthetics-alpha/dist/python/aws-cdk.aws-synthetics-alpha-2.84.0a0.tar", last modified: Tue Jun 13 23:47:06 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-synthetics/dist/python/aws-cdk.aws-synthetics-alpha-2.9.0a0", last modified: Wed Jan 26 11:22:06 2022, max compression
```

## Comparing `aws-cdk.aws-synthetics-alpha-2.84.0a0.tar` & `aws-cdk.aws-synthetics-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:57.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:57.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 23:46:57.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10993 2023-06-13 23:47:06.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9986 2023-06-13 23:46:57.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:57.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:47:06.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1891 2023-06-13 23:46:57.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/src/aws_cdk/aws_synthetics_alpha/
--rw-r--r--   0 root         (0) root         (0)   114046 2023-06-13 23:46:57.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/src/aws_cdk/aws_synthetics_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/src/aws_cdk/aws_synthetics_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      447 2023-06-13 23:46:57.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/src/aws_cdk/aws_synthetics_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   119560 2023-06-13 23:46:57.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/src/aws_cdk/aws_synthetics_alpha/_jsii/aws-synthetics-alpha@2.84.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:57.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/src/aws_cdk/aws_synthetics_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/src/aws_cdk.aws_synthetics_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10993 2023-06-13 23:47:06.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/src/aws_cdk.aws_synthetics_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      561 2023-06-13 23:47:06.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/src/aws_cdk.aws_synthetics_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:47:06.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/src/aws_cdk.aws_synthetics_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-13 23:47:06.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/src/aws_cdk.aws_synthetics_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:47:06.000000 aws-cdk.aws-synthetics-alpha-2.84.0a0/src/aws_cdk.aws_synthetics_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:01.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8650 2022-01-26 11:22:06.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7676 2022-01-26 11:22:01.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:06.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1816 2022-01-26 11:22:01.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/src/aws_cdk/aws_synthetics_alpha/
+-rw-r--r--   0 root         (0) root         (0)    76309 2022-01-26 11:22:01.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/src/aws_cdk/aws_synthetics_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/src/aws_cdk/aws_synthetics_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      411 2022-01-26 11:22:01.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/src/aws_cdk/aws_synthetics_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   101979 2022-01-26 11:22:01.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/src/aws_cdk/aws_synthetics_alpha/_jsii/aws-synthetics-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/src/aws_cdk/aws_synthetics_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/src/aws_cdk.aws_synthetics_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8650 2022-01-26 11:22:06.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/src/aws_cdk.aws_synthetics_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      560 2022-01-26 11:22:06.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/src/aws_cdk.aws_synthetics_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:06.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/src/aws_cdk.aws_synthetics_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:06.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/src/aws_cdk.aws_synthetics_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:06.000000 aws-cdk.aws-synthetics-alpha-2.9.0a0/src/aws_cdk.aws_synthetics_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-synthetics-alpha-2.84.0a0/LICENSE` & `aws-cdk.aws-synthetics-alpha-2.9.0a0/LICENSE`

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

### Comparing `aws-cdk.aws-synthetics-alpha-2.84.0a0/PKG-INFO` & `aws-cdk.aws-synthetics-alpha-2.9.0a0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-synthetics-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::Synthetics
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
 
 # Amazon CloudWatch Synthetics Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -58,15 +58,15 @@
 ```python
 canary = synthetics.Canary(self, "MyCanary",
     schedule=synthetics.Schedule.rate(Duration.minutes(5)),
     test=synthetics.Test.custom(
         code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
         handler="index.handler"
     ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0,
+    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_1,
     environment_variables={
         "stage": "prod"
     }
 )
 ```
 
 The following is an example of an `index.js` file which exports the `handler` function:
@@ -125,36 +125,14 @@
 schedule = synthetics.Schedule.cron(
     hour="0,8,16"
 )
 ```
 
 If you want the canary to run just once upon deployment, you can use `Schedule.once()`.
 
-### Canary DeleteLambdaResourcesOnCanaryDeletion
-
-You can specify whether the AWS CloudFormation is to also delete the Lambda functions and layers used by this canary, when the canary is deleted.
-
-This can be provisioned by setting the `enableAutoDeleteLambdas` property to `true` when we define the canary.
-
-```python
-stack = Stack()
-
-canary = synthetics.Canary(stack, "Canary",
-    test=synthetics.Test.custom(
-        handler="index.handler",
-        code=synthetics.Code.from_inline("/* Synthetics handler code")
-    ),
-    enable_auto_delete_lambdas=True,
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0
-)
-```
-
-Synthetic Canaries create additional resources under the hood beyond Lambda functions. Setting `enableAutoDeleteLambdas: true` will take care of
-cleaning up Lambda functions on deletion, but you still have to manually delete other resources like S3 buckets and CloudWatch logs.
-
 ### Configuring the Canary Script
 
 To configure the script the canary executes, use the `test` property. The `test` property accepts a `Test` instance that can be initialized by the `Test` class static methods. Currently, the only implemented method is `Test.custom()`, which allows you to bring your own code. In the future, other methods will be added. `Test.custom()` accepts `code` and `handler` properties -- both are required by Synthetics to create a lambda function on your behalf.
 
 The `synthetics.Code` class exposes static methods to bundle your code artifacts:
 
 * `code.fromInline(code)` - specify an inline script.
@@ -168,32 +146,32 @@
 import aws_cdk.aws_s3 as s3
 # To supply the code inline:
 synthetics.Canary(self, "Inline Canary",
     test=synthetics.Test.custom(
         code=synthetics.Code.from_inline("/* Synthetics handler code */"),
         handler="index.handler"
     ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0
+    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_3
 )
 
 # To supply the code from your local filesystem:
 synthetics.Canary(self, "Asset Canary",
     test=synthetics.Test.custom(
         code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
         handler="index.handler"
     ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0
+    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_3
 )
 bucket = s3.Bucket(self, "Code Bucket")
 synthetics.Canary(self, "Bucket Canary",
     test=synthetics.Test.custom(
         code=synthetics.Code.from_bucket(bucket, "canary.zip"),
         handler="index.handler"
     ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0
+    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_3
 )
 ```
 
 > **Note:** Synthetics have a specified folder structure for canaries. For Node scripts supplied via `code.fromAsset()` or `code.fromBucket()`, the canary resource requires the following folder structure:
 >
 > ```plaintext
 > canary/
@@ -208,41 +186,14 @@
 > canary/
 > ├── python/
 >     ├── <filename>.py
 > ```
 >
 > See Synthetics [docs](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Canaries_WritingCanary.html).
 
-### Running a canary on a VPC
-
-You can specify what [VPC a canary executes in](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Canaries_VPC.html).
-This can allow for monitoring services that may be internal to a specific VPC. To place a canary within a VPC, you can specify the `vpc` property with the desired `VPC` to place then canary in.
-This will automatically attach the appropriate IAM permissions to attach to the VPC. This will also create a Security Group and attach to the default subnets for the VPC unless specified via `vpcSubnets` and `securityGroups`.
-
-```python
-import aws_cdk.aws_ec2 as ec2
-
-# vpc: ec2.IVpc
-
-synthetics.Canary(self, "Vpc Canary",
-    test=synthetics.Test.custom(
-        code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
-        handler="index.handler"
-    ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0,
-    vpc=vpc
-)
-```
-
-> **Note:** By default, the Synthetics runtime needs access to the S3 and CloudWatch APIs, which will fail in a private subnet without internet access enabled (e.g. an isolated subnnet).
->
-> Ensure that the Canary is placed in a VPC either with internet connectivity or with VPC Endpoints for S3 and CloudWatch enabled and configured.
->
-> See [Synthetics VPC docs](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Canaries_VPC.html).
-
 ### Alarms
 
 You can configure a CloudWatch Alarm on a canary metric. Metrics are emitted by CloudWatch automatically and can be accessed by the following APIs:
 
 * `canary.metricSuccessPercent()` - percentage of successful canary runs over a given time
 * `canary.metricDuration()` - how much time each canary run takes, in seconds.
 * `canary.metricFailed()` - number of failed canary runs over a given time
@@ -257,7 +208,9 @@
 cloudwatch.Alarm(self, "CanaryAlarm",
     metric=canary.metric_success_percent(),
     evaluation_periods=2,
     threshold=90,
     comparison_operator=cloudwatch.ComparisonOperator.LESS_THAN_THRESHOLD
 )
 ```
+
+
```

### Comparing `aws-cdk.aws-synthetics-alpha-2.84.0a0/README.md` & `aws-cdk.aws-synthetics-alpha-2.9.0a0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 ```python
 canary = synthetics.Canary(self, "MyCanary",
     schedule=synthetics.Schedule.rate(Duration.minutes(5)),
     test=synthetics.Test.custom(
         code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
         handler="index.handler"
     ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0,
+    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_1,
     environment_variables={
         "stage": "prod"
     }
 )
 ```
 
 The following is an example of an `index.js` file which exports the `handler` function:
@@ -98,36 +98,14 @@
 schedule = synthetics.Schedule.cron(
     hour="0,8,16"
 )
 ```
 
 If you want the canary to run just once upon deployment, you can use `Schedule.once()`.
 
-### Canary DeleteLambdaResourcesOnCanaryDeletion
-
-You can specify whether the AWS CloudFormation is to also delete the Lambda functions and layers used by this canary, when the canary is deleted.
-
-This can be provisioned by setting the `enableAutoDeleteLambdas` property to `true` when we define the canary.
-
-```python
-stack = Stack()
-
-canary = synthetics.Canary(stack, "Canary",
-    test=synthetics.Test.custom(
-        handler="index.handler",
-        code=synthetics.Code.from_inline("/* Synthetics handler code")
-    ),
-    enable_auto_delete_lambdas=True,
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0
-)
-```
-
-Synthetic Canaries create additional resources under the hood beyond Lambda functions. Setting `enableAutoDeleteLambdas: true` will take care of
-cleaning up Lambda functions on deletion, but you still have to manually delete other resources like S3 buckets and CloudWatch logs.
-
 ### Configuring the Canary Script
 
 To configure the script the canary executes, use the `test` property. The `test` property accepts a `Test` instance that can be initialized by the `Test` class static methods. Currently, the only implemented method is `Test.custom()`, which allows you to bring your own code. In the future, other methods will be added. `Test.custom()` accepts `code` and `handler` properties -- both are required by Synthetics to create a lambda function on your behalf.
 
 The `synthetics.Code` class exposes static methods to bundle your code artifacts:
 
 * `code.fromInline(code)` - specify an inline script.
@@ -141,32 +119,32 @@
 import aws_cdk.aws_s3 as s3
 # To supply the code inline:
 synthetics.Canary(self, "Inline Canary",
     test=synthetics.Test.custom(
         code=synthetics.Code.from_inline("/* Synthetics handler code */"),
         handler="index.handler"
     ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0
+    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_3
 )
 
 # To supply the code from your local filesystem:
 synthetics.Canary(self, "Asset Canary",
     test=synthetics.Test.custom(
         code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
         handler="index.handler"
     ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0
+    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_3
 )
 bucket = s3.Bucket(self, "Code Bucket")
 synthetics.Canary(self, "Bucket Canary",
     test=synthetics.Test.custom(
         code=synthetics.Code.from_bucket(bucket, "canary.zip"),
         handler="index.handler"
     ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0
+    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_3
 )
 ```
 
 > **Note:** Synthetics have a specified folder structure for canaries. For Node scripts supplied via `code.fromAsset()` or `code.fromBucket()`, the canary resource requires the following folder structure:
 >
 > ```plaintext
 > canary/
@@ -181,41 +159,14 @@
 > canary/
 > ├── python/
 >     ├── <filename>.py
 > ```
 >
 > See Synthetics [docs](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Canaries_WritingCanary.html).
 
-### Running a canary on a VPC
-
-You can specify what [VPC a canary executes in](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Canaries_VPC.html).
-This can allow for monitoring services that may be internal to a specific VPC. To place a canary within a VPC, you can specify the `vpc` property with the desired `VPC` to place then canary in.
-This will automatically attach the appropriate IAM permissions to attach to the VPC. This will also create a Security Group and attach to the default subnets for the VPC unless specified via `vpcSubnets` and `securityGroups`.
-
-```python
-import aws_cdk.aws_ec2 as ec2
-
-# vpc: ec2.IVpc
-
-synthetics.Canary(self, "Vpc Canary",
-    test=synthetics.Test.custom(
-        code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
-        handler="index.handler"
-    ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0,
-    vpc=vpc
-)
-```
-
-> **Note:** By default, the Synthetics runtime needs access to the S3 and CloudWatch APIs, which will fail in a private subnet without internet access enabled (e.g. an isolated subnnet).
->
-> Ensure that the Canary is placed in a VPC either with internet connectivity or with VPC Endpoints for S3 and CloudWatch enabled and configured.
->
-> See [Synthetics VPC docs](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Canaries_VPC.html).
-
 ### Alarms
 
 You can configure a CloudWatch Alarm on a canary metric. Metrics are emitted by CloudWatch automatically and can be accessed by the following APIs:
 
 * `canary.metricSuccessPercent()` - percentage of successful canary runs over a given time
 * `canary.metricDuration()` - how much time each canary run takes, in seconds.
 * `canary.metricFailed()` - number of failed canary runs over a given time
```

### Comparing `aws-cdk.aws-synthetics-alpha-2.84.0a0/setup.py` & `aws-cdk.aws-synthetics-alpha-2.9.0a0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-synthetics-alpha",
-    "version": "2.84.0.a0",
+    "version": "2.9.0.a0",
     "description": "The CDK Construct Library for AWS::Synthetics",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,43 +22,41 @@
     },
     "packages": [
         "aws_cdk.aws_synthetics_alpha",
         "aws_cdk.aws_synthetics_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_synthetics_alpha._jsii": [
-            "aws-synthetics-alpha@2.84.0-alpha.0.jsii.tgz"
+            "aws-synthetics-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_synthetics_alpha": [
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

### Comparing `aws-cdk.aws-synthetics-alpha-2.84.0a0/src/aws_cdk/aws_synthetics_alpha/__init__.py` & `aws-cdk.aws-synthetics-alpha-2.9.0a0/src/aws_cdk/aws_synthetics_alpha/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ```python
 canary = synthetics.Canary(self, "MyCanary",
     schedule=synthetics.Schedule.rate(Duration.minutes(5)),
     test=synthetics.Test.custom(
         code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
         handler="index.handler"
     ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0,
+    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_1,
     environment_variables={
         "stage": "prod"
     }
 )
 ```
 
 The following is an example of an `index.js` file which exports the `handler` function:
@@ -99,36 +99,14 @@
 schedule = synthetics.Schedule.cron(
     hour="0,8,16"
 )
 ```
 
 If you want the canary to run just once upon deployment, you can use `Schedule.once()`.
 
-### Canary DeleteLambdaResourcesOnCanaryDeletion
-
-You can specify whether the AWS CloudFormation is to also delete the Lambda functions and layers used by this canary, when the canary is deleted.
-
-This can be provisioned by setting the `enableAutoDeleteLambdas` property to `true` when we define the canary.
-
-```python
-stack = Stack()
-
-canary = synthetics.Canary(stack, "Canary",
-    test=synthetics.Test.custom(
-        handler="index.handler",
-        code=synthetics.Code.from_inline("/* Synthetics handler code")
-    ),
-    enable_auto_delete_lambdas=True,
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0
-)
-```
-
-Synthetic Canaries create additional resources under the hood beyond Lambda functions. Setting `enableAutoDeleteLambdas: true` will take care of
-cleaning up Lambda functions on deletion, but you still have to manually delete other resources like S3 buckets and CloudWatch logs.
-
 ### Configuring the Canary Script
 
 To configure the script the canary executes, use the `test` property. The `test` property accepts a `Test` instance that can be initialized by the `Test` class static methods. Currently, the only implemented method is `Test.custom()`, which allows you to bring your own code. In the future, other methods will be added. `Test.custom()` accepts `code` and `handler` properties -- both are required by Synthetics to create a lambda function on your behalf.
 
 The `synthetics.Code` class exposes static methods to bundle your code artifacts:
 
 * `code.fromInline(code)` - specify an inline script.
@@ -142,32 +120,32 @@
 import aws_cdk.aws_s3 as s3
 # To supply the code inline:
 synthetics.Canary(self, "Inline Canary",
     test=synthetics.Test.custom(
         code=synthetics.Code.from_inline("/* Synthetics handler code */"),
         handler="index.handler"
     ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0
+    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_3
 )
 
 # To supply the code from your local filesystem:
 synthetics.Canary(self, "Asset Canary",
     test=synthetics.Test.custom(
         code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
         handler="index.handler"
     ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0
+    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_3
 )
 bucket = s3.Bucket(self, "Code Bucket")
 synthetics.Canary(self, "Bucket Canary",
     test=synthetics.Test.custom(
         code=synthetics.Code.from_bucket(bucket, "canary.zip"),
         handler="index.handler"
     ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0
+    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_3
 )
 ```
 
 > **Note:** Synthetics have a specified folder structure for canaries. For Node scripts supplied via `code.fromAsset()` or `code.fromBucket()`, the canary resource requires the following folder structure:
 >
 > ```plaintext
 > canary/
@@ -182,41 +160,14 @@
 > canary/
 > ├── python/
 >     ├── <filename>.py
 > ```
 >
 > See Synthetics [docs](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Canaries_WritingCanary.html).
 
-### Running a canary on a VPC
-
-You can specify what [VPC a canary executes in](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Canaries_VPC.html).
-This can allow for monitoring services that may be internal to a specific VPC. To place a canary within a VPC, you can specify the `vpc` property with the desired `VPC` to place then canary in.
-This will automatically attach the appropriate IAM permissions to attach to the VPC. This will also create a Security Group and attach to the default subnets for the VPC unless specified via `vpcSubnets` and `securityGroups`.
-
-```python
-import aws_cdk.aws_ec2 as ec2
-
-# vpc: ec2.IVpc
-
-synthetics.Canary(self, "Vpc Canary",
-    test=synthetics.Test.custom(
-        code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
-        handler="index.handler"
-    ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0,
-    vpc=vpc
-)
-```
-
-> **Note:** By default, the Synthetics runtime needs access to the S3 and CloudWatch APIs, which will fail in a private subnet without internet access enabled (e.g. an isolated subnnet).
->
-> Ensure that the Canary is placed in a VPC either with internet connectivity or with VPC Endpoints for S3 and CloudWatch enabled and configured.
->
-> See [Synthetics VPC docs](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Canaries_VPC.html).
-
 ### Alarms
 
 You can configure a CloudWatch Alarm on a canary metric. Metrics are emitted by CloudWatch automatically and can be accessed by the following APIs:
 
 * `canary.metricSuccessPercent()` - percentage of successful canary runs over a given time
 * `canary.metricDuration()` - how much time each canary run takes, in seconds.
 * `canary.metricFailed()` - number of failed canary runs over a given time
@@ -242,37 +193,34 @@
 import enum
 import typing
 
 import jsii
 import publication
 import typing_extensions
 
-from typeguard import check_type
-
 from ._jsii import *
 
-import aws_cdk as _aws_cdk_ceddda9d
-import aws_cdk.aws_cloudwatch as _aws_cdk_aws_cloudwatch_ceddda9d
-import aws_cdk.aws_ec2 as _aws_cdk_aws_ec2_ceddda9d
-import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
-import aws_cdk.aws_s3 as _aws_cdk_aws_s3_ceddda9d
-import aws_cdk.aws_s3_assets as _aws_cdk_aws_s3_assets_ceddda9d
-import constructs as _constructs_77d1e7e8
+import aws_cdk
+import aws_cdk.aws_cloudwatch
+import aws_cdk.aws_iam
+import aws_cdk.aws_s3
+import aws_cdk.aws_s3_assets
+import constructs
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-synthetics-alpha.ArtifactsBucketLocation",
     jsii_struct_bases=[],
     name_mapping={"bucket": "bucket", "prefix": "prefix"},
 )
 class ArtifactsBucketLocation:
     def __init__(
         self,
         *,
-        bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        bucket: aws_cdk.aws_s3.IBucket,
         prefix: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Options for specifying the s3 location that stores the data of each canary run.
 
         The artifacts bucket location **cannot**
         be updated once the canary is created.
 
@@ -294,33 +242,29 @@
             artifacts_bucket_location = synthetics_alpha.ArtifactsBucketLocation(
                 bucket=bucket,
             
                 # the properties below are optional
                 prefix="prefix"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c97027ffb7c3e1ed6531ba25f1eb4e6e2af525b8b67b6ace4855effcca2b9919)
-            check_type(argname="argument bucket", value=bucket, expected_type=type_hints["bucket"])
-            check_type(argname="argument prefix", value=prefix, expected_type=type_hints["prefix"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "bucket": bucket,
         }
         if prefix is not None:
             self._values["prefix"] = prefix
 
     @builtins.property
-    def bucket(self) -> _aws_cdk_aws_s3_ceddda9d.IBucket:
+    def bucket(self) -> aws_cdk.aws_s3.IBucket:
         '''(experimental) The s3 location that stores the data of each run.
 
         :stability: experimental
         '''
         result = self._values.get("bucket")
         assert result is not None, "Required property 'bucket' is missing"
-        return typing.cast(_aws_cdk_aws_s3_ceddda9d.IBucket, result)
+        return typing.cast(aws_cdk.aws_s3.IBucket, result)
 
     @builtins.property
     def prefix(self) -> typing.Optional[builtins.str]:
         '''(experimental) The S3 bucket prefix.
 
         Specify this if you want a more specific path within the artifacts bucket.
 
@@ -339,17 +283,16 @@
 
     def __repr__(self) -> str:
         return "ArtifactsBucketLocation(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-@jsii.implements(_aws_cdk_aws_ec2_ceddda9d.IConnectable)
 class Canary(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-synthetics-alpha.Canary",
 ):
     '''(experimental) Define a new Canary.
 
     :stability: experimental
     :exampleMetadata: infused
@@ -358,399 +301,333 @@
 
         canary = synthetics.Canary(self, "MyCanary",
             schedule=synthetics.Schedule.rate(Duration.minutes(5)),
             test=synthetics.Test.custom(
                 code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
                 handler="index.handler"
             ),
-            runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0,
+            runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_1,
             environment_variables={
                 "stage": "prod"
             }
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         runtime: "Runtime",
         test: "Test",
-        artifacts_bucket_location: typing.Optional[typing.Union[ArtifactsBucketLocation, typing.Dict[builtins.str, typing.Any]]] = None,
+        artifacts_bucket_location: typing.Optional[ArtifactsBucketLocation] = None,
         canary_name: typing.Optional[builtins.str] = None,
-        enable_auto_delete_lambdas: typing.Optional[builtins.bool] = None,
         environment_variables: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-        failure_retention_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-        role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        failure_retention_period: typing.Optional[aws_cdk.Duration] = None,
+        role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
         schedule: typing.Optional["Schedule"] = None,
-        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
         start_after_creation: typing.Optional[builtins.bool] = None,
-        success_retention_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-        time_to_live: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
-        vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        success_retention_period: typing.Optional[aws_cdk.Duration] = None,
+        time_to_live: typing.Optional[aws_cdk.Duration] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param runtime: (experimental) Specify the runtime version to use for the canary.
         :param test: (experimental) The type of test that you want your canary to run. Use ``Test.custom()`` to specify the test to run.
         :param artifacts_bucket_location: (experimental) The s3 location that stores the data of the canary runs. Default: - A new s3 bucket will be created without a prefix.
         :param canary_name: (experimental) The name of the canary. Be sure to give it a descriptive name that distinguishes it from other canaries in your account. Do not include secrets or proprietary information in your canary name. The canary name makes up part of the canary ARN, which is included in outbound calls over the internet. Default: - A unique name will be generated from the construct ID
-        :param enable_auto_delete_lambdas: (experimental) Whether or not to delete the lambda resources when the canary is deleted. Default: false
         :param environment_variables: (experimental) Key-value pairs that the Synthetics caches and makes available for your canary scripts. Use environment variables to apply configuration changes, such as test and production environment configurations, without changing your Canary script source code. Default: - No environment variables.
         :param failure_retention_period: (experimental) How many days should failed runs be retained. Default: Duration.days(31)
         :param role: (experimental) Canary execution role. This is the role that will be assumed by the canary upon execution. It controls the permissions that the canary will have. The role must be assumable by the AWS Lambda service principal. If not supplied, a role will be created with all the required permissions. If you provide a Role, you must add the required permissions. Default: - A unique role will be generated for this canary. You can add permissions to roles by calling 'addToRolePolicy'.
         :param schedule: (experimental) Specify the schedule for how often the canary runs. For example, if you set ``schedule`` to ``rate(10 minutes)``, then the canary will run every 10 minutes. You can set the schedule with ``Schedule.rate(Duration)`` (recommended) or you can specify an expression using ``Schedule.expression()``. Default: 'rate(5 minutes)'
-        :param security_groups: (experimental) The list of security groups to associate with the canary's network interfaces. You must provide ``vpc`` when using this prop. Default: - If the canary is placed within a VPC and a security group is not specified a dedicated security group will be created for this canary.
         :param start_after_creation: (experimental) Whether or not the canary should start after creation. Default: true
         :param success_retention_period: (experimental) How many days should successful runs be retained. Default: Duration.days(31)
         :param time_to_live: (experimental) How long the canary will be in a 'RUNNING' state. For example, if you set ``timeToLive`` to be 1 hour and ``schedule`` to be ``rate(10 minutes)``, your canary will run at 10 minute intervals for an hour, for a total of 6 times. Default: - no limit
-        :param vpc: (experimental) The VPC where this canary is run. Specify this if the canary needs to access resources in a VPC. Default: - Not in VPC
-        :param vpc_subnets: (experimental) Where to place the network interfaces within the VPC. You must provide ``vpc`` when using this prop. Default: - the Vpc default strategy if not specified
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__77f74ffae78f48cc052608780149daa4ac131f47fdbfc7d99da3a7883cc0e8a3)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = CanaryProps(
             runtime=runtime,
             test=test,
             artifacts_bucket_location=artifacts_bucket_location,
             canary_name=canary_name,
-            enable_auto_delete_lambdas=enable_auto_delete_lambdas,
             environment_variables=environment_variables,
             failure_retention_period=failure_retention_period,
             role=role,
             schedule=schedule,
-            security_groups=security_groups,
             start_after_creation=start_after_creation,
             success_retention_period=success_retention_period,
             time_to_live=time_to_live,
-            vpc=vpc,
-            vpc_subnets=vpc_subnets,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @jsii.member(jsii_name="metricDuration")
     def metric_duration(
         self,
         *,
         account: typing.Optional[builtins.str] = None,
         color: typing.Optional[builtins.str] = None,
         dimensions_map: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         label: typing.Optional[builtins.str] = None,
-        period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        period: typing.Optional[aws_cdk.Duration] = None,
         region: typing.Optional[builtins.str] = None,
         statistic: typing.Optional[builtins.str] = None,
-        unit: typing.Optional[_aws_cdk_aws_cloudwatch_ceddda9d.Unit] = None,
-    ) -> _aws_cdk_aws_cloudwatch_ceddda9d.Metric:
+        unit: typing.Optional[aws_cdk.aws_cloudwatch.Unit] = None,
+    ) -> aws_cdk.aws_cloudwatch.Metric:
         '''(experimental) Measure the Duration of a single canary run, in seconds.
 
         :param account: Account which this metric comes from. Default: - Deployment account.
         :param color: The hex color code, prefixed with '#' (e.g. '#00ff00'), to use when this metric is rendered on a graph. The ``Color`` class has a set of standard colors that can be used here. Default: - Automatic color
         :param dimensions_map: Dimensions of the metric. Default: - No dimensions.
-        :param label: Label for this metric when added to a Graph in a Dashboard. You can use `dynamic labels <https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/graph-dynamic-labels.html>`_ to show summary information about the entire displayed time series in the legend. For example, if you use:: [max: ${MAX}] MyMetric As the metric label, the maximum value in the visible range will be shown next to the time series name in the graph's legend. Default: - No label
+        :param label: Label for this metric when added to a Graph in a Dashboard. Default: - No label
         :param period: The period over which the specified statistic is applied. Default: Duration.minutes(5)
         :param region: Region which this metric comes from. Default: - Deployment region.
-        :param statistic: What function to use for aggregating. Use the ``aws_cloudwatch.Stats`` helper class to construct valid input strings. Can be one of the following: - "Minimum" | "min" - "Maximum" | "max" - "Average" | "avg" - "Sum" | "sum" - "SampleCount | "n" - "pNN.NN" - "tmNN.NN" | "tm(NN.NN%:NN.NN%)" - "iqm" - "wmNN.NN" | "wm(NN.NN%:NN.NN%)" - "tcNN.NN" | "tc(NN.NN%:NN.NN%)" - "tsNN.NN" | "ts(NN.NN%:NN.NN%)" Default: Average
+        :param statistic: What function to use for aggregating. Can be one of the following: - "Minimum" | "min" - "Maximum" | "max" - "Average" | "avg" - "Sum" | "sum" - "SampleCount | "n" - "pNN.NN" Default: Average
         :param unit: Unit used to filter the metric stream. Only refer to datums emitted to the metric stream with the given unit and ignore all others. Only useful when datums are being emitted to the same metric stream under different units. The default is to use all matric datums in the stream, regardless of unit, which is recommended in nearly all cases. CloudWatch does not honor this property for graphs. Default: - All metric datums in the given metric stream
 
         :default: avg over 5 minutes
 
         :stability: experimental
         '''
-        options = _aws_cdk_aws_cloudwatch_ceddda9d.MetricOptions(
+        options = aws_cdk.aws_cloudwatch.MetricOptions(
             account=account,
             color=color,
             dimensions_map=dimensions_map,
             label=label,
             period=period,
             region=region,
             statistic=statistic,
             unit=unit,
         )
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricDuration", [options]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricDuration", [options]))
 
     @jsii.member(jsii_name="metricFailed")
     def metric_failed(
         self,
         *,
         account: typing.Optional[builtins.str] = None,
         color: typing.Optional[builtins.str] = None,
         dimensions_map: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         label: typing.Optional[builtins.str] = None,
-        period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        period: typing.Optional[aws_cdk.Duration] = None,
         region: typing.Optional[builtins.str] = None,
         statistic: typing.Optional[builtins.str] = None,
-        unit: typing.Optional[_aws_cdk_aws_cloudwatch_ceddda9d.Unit] = None,
-    ) -> _aws_cdk_aws_cloudwatch_ceddda9d.Metric:
+        unit: typing.Optional[aws_cdk.aws_cloudwatch.Unit] = None,
+    ) -> aws_cdk.aws_cloudwatch.Metric:
         '''(experimental) Measure the number of failed canary runs over a given time period.
 
         Default: sum over 5 minutes
 
         :param account: Account which this metric comes from. Default: - Deployment account.
         :param color: The hex color code, prefixed with '#' (e.g. '#00ff00'), to use when this metric is rendered on a graph. The ``Color`` class has a set of standard colors that can be used here. Default: - Automatic color
         :param dimensions_map: Dimensions of the metric. Default: - No dimensions.
-        :param label: Label for this metric when added to a Graph in a Dashboard. You can use `dynamic labels <https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/graph-dynamic-labels.html>`_ to show summary information about the entire displayed time series in the legend. For example, if you use:: [max: ${MAX}] MyMetric As the metric label, the maximum value in the visible range will be shown next to the time series name in the graph's legend. Default: - No label
+        :param label: Label for this metric when added to a Graph in a Dashboard. Default: - No label
         :param period: The period over which the specified statistic is applied. Default: Duration.minutes(5)
         :param region: Region which this metric comes from. Default: - Deployment region.
-        :param statistic: What function to use for aggregating. Use the ``aws_cloudwatch.Stats`` helper class to construct valid input strings. Can be one of the following: - "Minimum" | "min" - "Maximum" | "max" - "Average" | "avg" - "Sum" | "sum" - "SampleCount | "n" - "pNN.NN" - "tmNN.NN" | "tm(NN.NN%:NN.NN%)" - "iqm" - "wmNN.NN" | "wm(NN.NN%:NN.NN%)" - "tcNN.NN" | "tc(NN.NN%:NN.NN%)" - "tsNN.NN" | "ts(NN.NN%:NN.NN%)" Default: Average
+        :param statistic: What function to use for aggregating. Can be one of the following: - "Minimum" | "min" - "Maximum" | "max" - "Average" | "avg" - "Sum" | "sum" - "SampleCount | "n" - "pNN.NN" Default: Average
         :param unit: Unit used to filter the metric stream. Only refer to datums emitted to the metric stream with the given unit and ignore all others. Only useful when datums are being emitted to the same metric stream under different units. The default is to use all matric datums in the stream, regardless of unit, which is recommended in nearly all cases. CloudWatch does not honor this property for graphs. Default: - All metric datums in the given metric stream
 
         :stability: experimental
         '''
-        options = _aws_cdk_aws_cloudwatch_ceddda9d.MetricOptions(
+        options = aws_cdk.aws_cloudwatch.MetricOptions(
             account=account,
             color=color,
             dimensions_map=dimensions_map,
             label=label,
             period=period,
             region=region,
             statistic=statistic,
             unit=unit,
         )
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricFailed", [options]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricFailed", [options]))
 
     @jsii.member(jsii_name="metricSuccessPercent")
     def metric_success_percent(
         self,
         *,
         account: typing.Optional[builtins.str] = None,
         color: typing.Optional[builtins.str] = None,
         dimensions_map: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         label: typing.Optional[builtins.str] = None,
-        period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        period: typing.Optional[aws_cdk.Duration] = None,
         region: typing.Optional[builtins.str] = None,
         statistic: typing.Optional[builtins.str] = None,
-        unit: typing.Optional[_aws_cdk_aws_cloudwatch_ceddda9d.Unit] = None,
-    ) -> _aws_cdk_aws_cloudwatch_ceddda9d.Metric:
+        unit: typing.Optional[aws_cdk.aws_cloudwatch.Unit] = None,
+    ) -> aws_cdk.aws_cloudwatch.Metric:
         '''(experimental) Measure the percentage of successful canary runs.
 
         :param account: Account which this metric comes from. Default: - Deployment account.
         :param color: The hex color code, prefixed with '#' (e.g. '#00ff00'), to use when this metric is rendered on a graph. The ``Color`` class has a set of standard colors that can be used here. Default: - Automatic color
         :param dimensions_map: Dimensions of the metric. Default: - No dimensions.
-        :param label: Label for this metric when added to a Graph in a Dashboard. You can use `dynamic labels <https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/graph-dynamic-labels.html>`_ to show summary information about the entire displayed time series in the legend. For example, if you use:: [max: ${MAX}] MyMetric As the metric label, the maximum value in the visible range will be shown next to the time series name in the graph's legend. Default: - No label
+        :param label: Label for this metric when added to a Graph in a Dashboard. Default: - No label
         :param period: The period over which the specified statistic is applied. Default: Duration.minutes(5)
         :param region: Region which this metric comes from. Default: - Deployment region.
-        :param statistic: What function to use for aggregating. Use the ``aws_cloudwatch.Stats`` helper class to construct valid input strings. Can be one of the following: - "Minimum" | "min" - "Maximum" | "max" - "Average" | "avg" - "Sum" | "sum" - "SampleCount | "n" - "pNN.NN" - "tmNN.NN" | "tm(NN.NN%:NN.NN%)" - "iqm" - "wmNN.NN" | "wm(NN.NN%:NN.NN%)" - "tcNN.NN" | "tc(NN.NN%:NN.NN%)" - "tsNN.NN" | "ts(NN.NN%:NN.NN%)" Default: Average
+        :param statistic: What function to use for aggregating. Can be one of the following: - "Minimum" | "min" - "Maximum" | "max" - "Average" | "avg" - "Sum" | "sum" - "SampleCount | "n" - "pNN.NN" Default: Average
         :param unit: Unit used to filter the metric stream. Only refer to datums emitted to the metric stream with the given unit and ignore all others. Only useful when datums are being emitted to the same metric stream under different units. The default is to use all matric datums in the stream, regardless of unit, which is recommended in nearly all cases. CloudWatch does not honor this property for graphs. Default: - All metric datums in the given metric stream
 
         :default: avg over 5 minutes
 
         :stability: experimental
         '''
-        options = _aws_cdk_aws_cloudwatch_ceddda9d.MetricOptions(
+        options = aws_cdk.aws_cloudwatch.MetricOptions(
             account=account,
             color=color,
             dimensions_map=dimensions_map,
             label=label,
             period=period,
             region=region,
             statistic=statistic,
             unit=unit,
         )
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricSuccessPercent", [options]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricSuccessPercent", [options]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="artifactsBucket")
-    def artifacts_bucket(self) -> _aws_cdk_aws_s3_ceddda9d.IBucket:
+    def artifacts_bucket(self) -> aws_cdk.aws_s3.IBucket:
         '''(experimental) Bucket where data from each canary run is stored.
 
         :stability: experimental
         '''
-        return typing.cast(_aws_cdk_aws_s3_ceddda9d.IBucket, jsii.get(self, "artifactsBucket"))
+        return typing.cast(aws_cdk.aws_s3.IBucket, jsii.get(self, "artifactsBucket"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="canaryId")
     def canary_id(self) -> builtins.str:
         '''(experimental) The canary ID.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "canaryId"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="canaryName")
     def canary_name(self) -> builtins.str:
         '''(experimental) The canary Name.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "canaryName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="canaryState")
     def canary_state(self) -> builtins.str:
         '''(experimental) The state of the canary.
 
         For example, 'RUNNING', 'STOPPED', 'NOT STARTED', or 'ERROR'.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "canaryState"))
 
-    @builtins.property
-    @jsii.member(jsii_name="connections")
-    def connections(self) -> _aws_cdk_aws_ec2_ceddda9d.Connections:
-        '''(experimental) Access the Connections object.
-
-        Will fail if not a VPC-enabled Canary
-
-        :stability: experimental
-        '''
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.Connections, jsii.get(self, "connections"))
-
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="role")
-    def role(self) -> _aws_cdk_aws_iam_ceddda9d.IRole:
+    def role(self) -> aws_cdk.aws_iam.IRole:
         '''(experimental) Execution role associated with this Canary.
 
         :stability: experimental
         '''
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.IRole, jsii.get(self, "role"))
+        return typing.cast(aws_cdk.aws_iam.IRole, jsii.get(self, "role"))
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-synthetics-alpha.CanaryProps",
     jsii_struct_bases=[],
     name_mapping={
         "runtime": "runtime",
         "test": "test",
         "artifacts_bucket_location": "artifactsBucketLocation",
         "canary_name": "canaryName",
-        "enable_auto_delete_lambdas": "enableAutoDeleteLambdas",
         "environment_variables": "environmentVariables",
         "failure_retention_period": "failureRetentionPeriod",
         "role": "role",
         "schedule": "schedule",
-        "security_groups": "securityGroups",
         "start_after_creation": "startAfterCreation",
         "success_retention_period": "successRetentionPeriod",
         "time_to_live": "timeToLive",
-        "vpc": "vpc",
-        "vpc_subnets": "vpcSubnets",
     },
 )
 class CanaryProps:
     def __init__(
         self,
         *,
         runtime: "Runtime",
         test: "Test",
-        artifacts_bucket_location: typing.Optional[typing.Union[ArtifactsBucketLocation, typing.Dict[builtins.str, typing.Any]]] = None,
+        artifacts_bucket_location: typing.Optional[ArtifactsBucketLocation] = None,
         canary_name: typing.Optional[builtins.str] = None,
-        enable_auto_delete_lambdas: typing.Optional[builtins.bool] = None,
         environment_variables: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-        failure_retention_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-        role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        failure_retention_period: typing.Optional[aws_cdk.Duration] = None,
+        role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
         schedule: typing.Optional["Schedule"] = None,
-        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
         start_after_creation: typing.Optional[builtins.bool] = None,
-        success_retention_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-        time_to_live: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
-        vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        success_retention_period: typing.Optional[aws_cdk.Duration] = None,
+        time_to_live: typing.Optional[aws_cdk.Duration] = None,
     ) -> None:
         '''(experimental) Properties for a canary.
 
         :param runtime: (experimental) Specify the runtime version to use for the canary.
         :param test: (experimental) The type of test that you want your canary to run. Use ``Test.custom()`` to specify the test to run.
         :param artifacts_bucket_location: (experimental) The s3 location that stores the data of the canary runs. Default: - A new s3 bucket will be created without a prefix.
         :param canary_name: (experimental) The name of the canary. Be sure to give it a descriptive name that distinguishes it from other canaries in your account. Do not include secrets or proprietary information in your canary name. The canary name makes up part of the canary ARN, which is included in outbound calls over the internet. Default: - A unique name will be generated from the construct ID
-        :param enable_auto_delete_lambdas: (experimental) Whether or not to delete the lambda resources when the canary is deleted. Default: false
         :param environment_variables: (experimental) Key-value pairs that the Synthetics caches and makes available for your canary scripts. Use environment variables to apply configuration changes, such as test and production environment configurations, without changing your Canary script source code. Default: - No environment variables.
         :param failure_retention_period: (experimental) How many days should failed runs be retained. Default: Duration.days(31)
         :param role: (experimental) Canary execution role. This is the role that will be assumed by the canary upon execution. It controls the permissions that the canary will have. The role must be assumable by the AWS Lambda service principal. If not supplied, a role will be created with all the required permissions. If you provide a Role, you must add the required permissions. Default: - A unique role will be generated for this canary. You can add permissions to roles by calling 'addToRolePolicy'.
         :param schedule: (experimental) Specify the schedule for how often the canary runs. For example, if you set ``schedule`` to ``rate(10 minutes)``, then the canary will run every 10 minutes. You can set the schedule with ``Schedule.rate(Duration)`` (recommended) or you can specify an expression using ``Schedule.expression()``. Default: 'rate(5 minutes)'
-        :param security_groups: (experimental) The list of security groups to associate with the canary's network interfaces. You must provide ``vpc`` when using this prop. Default: - If the canary is placed within a VPC and a security group is not specified a dedicated security group will be created for this canary.
         :param start_after_creation: (experimental) Whether or not the canary should start after creation. Default: true
         :param success_retention_period: (experimental) How many days should successful runs be retained. Default: Duration.days(31)
         :param time_to_live: (experimental) How long the canary will be in a 'RUNNING' state. For example, if you set ``timeToLive`` to be 1 hour and ``schedule`` to be ``rate(10 minutes)``, your canary will run at 10 minute intervals for an hour, for a total of 6 times. Default: - no limit
-        :param vpc: (experimental) The VPC where this canary is run. Specify this if the canary needs to access resources in a VPC. Default: - Not in VPC
-        :param vpc_subnets: (experimental) Where to place the network interfaces within the VPC. You must provide ``vpc`` when using this prop. Default: - the Vpc default strategy if not specified
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
             canary = synthetics.Canary(self, "MyCanary",
                 schedule=synthetics.Schedule.rate(Duration.minutes(5)),
                 test=synthetics.Test.custom(
                     code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
                     handler="index.handler"
                 ),
-                runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0,
+                runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_1,
                 environment_variables={
                     "stage": "prod"
                 }
             )
         '''
         if isinstance(artifacts_bucket_location, dict):
             artifacts_bucket_location = ArtifactsBucketLocation(**artifacts_bucket_location)
-        if isinstance(vpc_subnets, dict):
-            vpc_subnets = _aws_cdk_aws_ec2_ceddda9d.SubnetSelection(**vpc_subnets)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ae7e63c36ba56bf570a16580ca3cc6aa4f4d25f66ba54d26f3f7a90413d04d63)
-            check_type(argname="argument runtime", value=runtime, expected_type=type_hints["runtime"])
-            check_type(argname="argument test", value=test, expected_type=type_hints["test"])
-            check_type(argname="argument artifacts_bucket_location", value=artifacts_bucket_location, expected_type=type_hints["artifacts_bucket_location"])
-            check_type(argname="argument canary_name", value=canary_name, expected_type=type_hints["canary_name"])
-            check_type(argname="argument enable_auto_delete_lambdas", value=enable_auto_delete_lambdas, expected_type=type_hints["enable_auto_delete_lambdas"])
-            check_type(argname="argument environment_variables", value=environment_variables, expected_type=type_hints["environment_variables"])
-            check_type(argname="argument failure_retention_period", value=failure_retention_period, expected_type=type_hints["failure_retention_period"])
-            check_type(argname="argument role", value=role, expected_type=type_hints["role"])
-            check_type(argname="argument schedule", value=schedule, expected_type=type_hints["schedule"])
-            check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
-            check_type(argname="argument start_after_creation", value=start_after_creation, expected_type=type_hints["start_after_creation"])
-            check_type(argname="argument success_retention_period", value=success_retention_period, expected_type=type_hints["success_retention_period"])
-            check_type(argname="argument time_to_live", value=time_to_live, expected_type=type_hints["time_to_live"])
-            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
-            check_type(argname="argument vpc_subnets", value=vpc_subnets, expected_type=type_hints["vpc_subnets"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "runtime": runtime,
             "test": test,
         }
         if artifacts_bucket_location is not None:
             self._values["artifacts_bucket_location"] = artifacts_bucket_location
         if canary_name is not None:
             self._values["canary_name"] = canary_name
-        if enable_auto_delete_lambdas is not None:
-            self._values["enable_auto_delete_lambdas"] = enable_auto_delete_lambdas
         if environment_variables is not None:
             self._values["environment_variables"] = environment_variables
         if failure_retention_period is not None:
             self._values["failure_retention_period"] = failure_retention_period
         if role is not None:
             self._values["role"] = role
         if schedule is not None:
             self._values["schedule"] = schedule
-        if security_groups is not None:
-            self._values["security_groups"] = security_groups
         if start_after_creation is not None:
             self._values["start_after_creation"] = start_after_creation
         if success_retention_period is not None:
             self._values["success_retention_period"] = success_retention_period
         if time_to_live is not None:
             self._values["time_to_live"] = time_to_live
-        if vpc is not None:
-            self._values["vpc"] = vpc
-        if vpc_subnets is not None:
-            self._values["vpc_subnets"] = vpc_subnets
 
     @builtins.property
     def runtime(self) -> "Runtime":
         '''(experimental) Specify the runtime version to use for the canary.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Canaries_Library.html
         :stability: experimental
@@ -797,26 +674,14 @@
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/servicelens_canaries_security.html
         :stability: experimental
         '''
         result = self._values.get("canary_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def enable_auto_delete_lambdas(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Whether or not to delete the lambda resources when the canary is deleted.
-
-        :default: false
-
-        :see: https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-synthetics-canary.html#cfn-synthetics-canary-deletelambdaresourcesoncanarydeletion
-        :stability: experimental
-        '''
-        result = self._values.get("enable_auto_delete_lambdas")
-        return typing.cast(typing.Optional[builtins.bool], result)
-
-    @builtins.property
     def environment_variables(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''(experimental) Key-value pairs that the Synthetics caches and makes available for your canary scripts.
 
         Use environment variables
         to apply configuration changes, such as test and production environment configurations, without changing your
@@ -826,26 +691,26 @@
 
         :stability: experimental
         '''
         result = self._values.get("environment_variables")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
-    def failure_retention_period(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+    def failure_retention_period(self) -> typing.Optional[aws_cdk.Duration]:
         '''(experimental) How many days should failed runs be retained.
 
         :default: Duration.days(31)
 
         :stability: experimental
         '''
         result = self._values.get("failure_retention_period")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
+        return typing.cast(typing.Optional[aws_cdk.Duration], result)
 
     @builtins.property
-    def role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+    def role(self) -> typing.Optional[aws_cdk.aws_iam.IRole]:
         '''(experimental) Canary execution role.
 
         This is the role that will be assumed by the canary upon execution.
         It controls the permissions that the canary will have. The role must
         be assumable by the AWS Lambda service principal.
 
         If not supplied, a role will be created with all the required permissions.
@@ -856,15 +721,15 @@
         - A unique role will be generated for this canary.
         You can add permissions to roles by calling 'addToRolePolicy'.
 
         :see: required permissions: https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-synthetics-canary.html#cfn-synthetics-canary-executionrolearn
         :stability: experimental
         '''
         result = self._values.get("role")
-        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_iam.IRole], result)
 
     @builtins.property
     def schedule(self) -> typing.Optional["Schedule"]:
         '''(experimental) Specify the schedule for how often the canary runs.
 
         For example, if you set ``schedule`` to ``rate(10 minutes)``, then the canary will run every 10 minutes.
         You can set the schedule with ``Schedule.rate(Duration)`` (recommended) or you can specify an expression using ``Schedule.expression()``.
@@ -873,92 +738,48 @@
 
         :stability: experimental
         '''
         result = self._values.get("schedule")
         return typing.cast(typing.Optional["Schedule"], result)
 
     @builtins.property
-    def security_groups(
-        self,
-    ) -> typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]]:
-        '''(experimental) The list of security groups to associate with the canary's network interfaces.
-
-        You must provide ``vpc`` when using this prop.
-
-        :default:
-
-        - If the canary is placed within a VPC and a security group is
-        not specified a dedicated security group will be created for this canary.
-
-        :stability: experimental
-        '''
-        result = self._values.get("security_groups")
-        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]], result)
-
-    @builtins.property
     def start_after_creation(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Whether or not the canary should start after creation.
 
         :default: true
 
         :stability: experimental
         '''
         result = self._values.get("start_after_creation")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def success_retention_period(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+    def success_retention_period(self) -> typing.Optional[aws_cdk.Duration]:
         '''(experimental) How many days should successful runs be retained.
 
         :default: Duration.days(31)
 
         :stability: experimental
         '''
         result = self._values.get("success_retention_period")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
+        return typing.cast(typing.Optional[aws_cdk.Duration], result)
 
     @builtins.property
-    def time_to_live(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+    def time_to_live(self) -> typing.Optional[aws_cdk.Duration]:
         '''(experimental) How long the canary will be in a 'RUNNING' state.
 
         For example, if you set ``timeToLive`` to be 1 hour and ``schedule`` to be ``rate(10 minutes)``,
         your canary will run at 10 minute intervals for an hour, for a total of 6 times.
 
         :default: - no limit
 
         :stability: experimental
         '''
         result = self._values.get("time_to_live")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
-
-    @builtins.property
-    def vpc(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc]:
-        '''(experimental) The VPC where this canary is run.
-
-        Specify this if the canary needs to access resources in a VPC.
-
-        :default: - Not in VPC
-
-        :stability: experimental
-        '''
-        result = self._values.get("vpc")
-        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc], result)
-
-    @builtins.property
-    def vpc_subnets(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection]:
-        '''(experimental) Where to place the network interfaces within the VPC.
-
-        You must provide ``vpc`` when using this prop.
-
-        :default: - the Vpc default strategy if not specified
-
-        :stability: experimental
-        '''
-        result = self._values.get("vpc_subnets")
-        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection], result)
+        return typing.cast(typing.Optional[aws_cdk.Duration], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -981,82 +802,76 @@
 
         canary = synthetics.Canary(self, "MyCanary",
             schedule=synthetics.Schedule.rate(Duration.minutes(5)),
             test=synthetics.Test.custom(
                 code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
                 handler="index.handler"
             ),
-            runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0,
+            runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_1,
             environment_variables={
                 "stage": "prod"
             }
         )
     '''
 
     def __init__(self) -> None:
         '''
         :stability: experimental
         '''
         jsii.create(self.__class__, self, [])
 
-    @jsii.member(jsii_name="fromAsset")
+    @jsii.member(jsii_name="fromAsset") # type: ignore[misc]
     @builtins.classmethod
     def from_asset(
         cls,
         asset_path: builtins.str,
         *,
-        deploy_time: typing.Optional[builtins.bool] = None,
-        readers: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.IGrantable]] = None,
+        readers: typing.Optional[typing.Sequence[aws_cdk.aws_iam.IGrantable]] = None,
         asset_hash: typing.Optional[builtins.str] = None,
-        asset_hash_type: typing.Optional[_aws_cdk_ceddda9d.AssetHashType] = None,
-        bundling: typing.Optional[typing.Union[_aws_cdk_ceddda9d.BundlingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        asset_hash_type: typing.Optional[aws_cdk.AssetHashType] = None,
+        bundling: typing.Optional[aws_cdk.BundlingOptions] = None,
         exclude: typing.Optional[typing.Sequence[builtins.str]] = None,
-        follow_symlinks: typing.Optional[_aws_cdk_ceddda9d.SymlinkFollowMode] = None,
-        ignore_mode: typing.Optional[_aws_cdk_ceddda9d.IgnoreMode] = None,
+        follow_symlinks: typing.Optional[aws_cdk.SymlinkFollowMode] = None,
+        ignore_mode: typing.Optional[aws_cdk.IgnoreMode] = None,
     ) -> "AssetCode":
         '''(experimental) Specify code from a local path.
 
         Path must include the folder structure ``nodejs/node_modules/myCanaryFilename.js``.
 
         :param asset_path: Either a directory or a .zip file.
-        :param deploy_time: Whether or not the asset needs to exist beyond deployment time; i.e. are copied over to a different location and not needed afterwards. Setting this property to true has an impact on the lifecycle of the asset, because we will assume that it is safe to delete after the CloudFormation deployment succeeds. For example, Lambda Function assets are copied over to Lambda during deployment. Therefore, it is not necessary to store the asset in S3, so we consider those deployTime assets. Default: false
         :param readers: A list of principals that should be able to read this asset from S3. You can use ``asset.grantRead(principal)`` to grant read permissions later. Default: - No principals that can read file asset.
         :param asset_hash: Specify a custom hash for this asset. If ``assetHashType`` is set it must be set to ``AssetHashType.CUSTOM``. For consistency, this custom hash will be SHA256 hashed and encoded as hex. The resulting hash will be the asset hash. NOTE: the hash is used in order to identify a specific revision of the asset, and used for optimizing and caching deployment activities related to this asset such as packaging, uploading to Amazon S3, etc. If you chose to customize the hash, you will need to make sure it is updated every time the asset changes, or otherwise it is possible that some deployments will not be invalidated. Default: - based on ``assetHashType``
         :param asset_hash_type: Specifies the type of hash to calculate for this asset. If ``assetHash`` is configured, this option must be ``undefined`` or ``AssetHashType.CUSTOM``. Default: - the default is ``AssetHashType.SOURCE``, but if ``assetHash`` is explicitly specified this value defaults to ``AssetHashType.CUSTOM``.
         :param bundling: Bundle the asset by executing a command in a Docker container or a custom bundling provider. The asset path will be mounted at ``/asset-input``. The Docker container is responsible for putting content at ``/asset-output``. The content at ``/asset-output`` will be zipped and used as the final asset. Default: - uploaded as-is to S3 if the asset is a regular file or a .zip file, archived into a .zip file and uploaded to S3 otherwise
-        :param exclude: File paths matching the patterns will be excluded. See ``ignoreMode`` to set the matching behavior. Has no effect on Assets bundled using the ``bundling`` property. Default: - nothing is excluded
+        :param exclude: Glob patterns to exclude from the copy. Default: - nothing is excluded
         :param follow_symlinks: A strategy for how to handle symlinks. Default: SymlinkFollowMode.NEVER
-        :param ignore_mode: The ignore behavior to use for ``exclude`` patterns. Default: IgnoreMode.GLOB
+        :param ignore_mode: The ignore behavior to use for exclude patterns. Default: IgnoreMode.GLOB
 
         :return: ``AssetCode`` associated with the specified path.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Canaries_WritingCanary.html#CloudWatch_Synthetics_Canaries_write_from_scratch
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4c04ee0a7f625fce33d3003e388d6a831237f31cbc709e9c551a1bc356475ede)
-            check_type(argname="argument asset_path", value=asset_path, expected_type=type_hints["asset_path"])
-        options = _aws_cdk_aws_s3_assets_ceddda9d.AssetOptions(
-            deploy_time=deploy_time,
+        options = aws_cdk.aws_s3_assets.AssetOptions(
             readers=readers,
             asset_hash=asset_hash,
             asset_hash_type=asset_hash_type,
             bundling=bundling,
             exclude=exclude,
             follow_symlinks=follow_symlinks,
             ignore_mode=ignore_mode,
         )
 
         return typing.cast("AssetCode", jsii.sinvoke(cls, "fromAsset", [asset_path, options]))
 
-    @jsii.member(jsii_name="fromBucket")
+    @jsii.member(jsii_name="fromBucket") # type: ignore[misc]
     @builtins.classmethod
     def from_bucket(
         cls,
-        bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        bucket: aws_cdk.aws_s3.IBucket,
         key: builtins.str,
         object_version: typing.Optional[builtins.str] = None,
     ) -> "S3Code":
         '''(experimental) Specify code from an s3 bucket.
 
         The object in the s3 bucket must be a .zip file that contains
         the structure ``nodejs/node_modules/myCanaryFilename.js``.
@@ -1066,42 +881,34 @@
         :param object_version: Optional S3 object version.
 
         :return: ``S3Code`` associated with the specified S3 object.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Canaries_WritingCanary.html#CloudWatch_Synthetics_Canaries_write_from_scratch
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__628908b4951e36d41574e89af118f4b8a140822fc9499275e081e1168a75bf43)
-            check_type(argname="argument bucket", value=bucket, expected_type=type_hints["bucket"])
-            check_type(argname="argument key", value=key, expected_type=type_hints["key"])
-            check_type(argname="argument object_version", value=object_version, expected_type=type_hints["object_version"])
         return typing.cast("S3Code", jsii.sinvoke(cls, "fromBucket", [bucket, key, object_version]))
 
-    @jsii.member(jsii_name="fromInline")
+    @jsii.member(jsii_name="fromInline") # type: ignore[misc]
     @builtins.classmethod
     def from_inline(cls, code: builtins.str) -> "InlineCode":
         '''(experimental) Specify code inline.
 
-        :param code: The actual handler code (limited to 5MB).
+        :param code: The actual handler code (limited to 4KiB).
 
         :return: ``InlineCode`` with inline code.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__534ebde2ca6177d2b07962ff163fa4be8fff02237e20a67c89fca238f2a43b12)
-            check_type(argname="argument code", value=code, expected_type=type_hints["code"])
         return typing.cast("InlineCode", jsii.sinvoke(cls, "fromInline", [code]))
 
-    @jsii.member(jsii_name="bind")
+    @jsii.member(jsii_name="bind") # type: ignore[misc]
     @abc.abstractmethod
     def bind(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         handler: builtins.str,
         family: "RuntimeFamily",
     ) -> "CodeConfig":
         '''(experimental) Called when the canary is initialized to allow this object to bind to the stack, add resources and have fun.
 
         :param scope: The binding scope. Don't be smart about trying to down-cast or assume it's initialized. You may just use it as a construct scope.
         :param handler: -
@@ -1114,33 +921,28 @@
         ...
 
 
 class _CodeProxy(Code):
     @jsii.member(jsii_name="bind")
     def bind(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         handler: builtins.str,
         family: "RuntimeFamily",
     ) -> "CodeConfig":
         '''(experimental) Called when the canary is initialized to allow this object to bind to the stack, add resources and have fun.
 
         :param scope: The binding scope. Don't be smart about trying to down-cast or assume it's initialized. You may just use it as a construct scope.
         :param handler: -
         :param family: -
 
         :return: a bound ``CodeConfig``.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5d4fce9f2879e280253f79f346736f1e74cabefddf0199d5d40b9e187d207f46)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument handler", value=handler, expected_type=type_hints["handler"])
-            check_type(argname="argument family", value=family, expected_type=type_hints["family"])
         return typing.cast("CodeConfig", jsii.invoke(self, "bind", [scope, handler, family]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the abstract class
 typing.cast(typing.Any, Code).__jsii_proxy_class__ = lambda : _CodeProxy
 
 
 @jsii.data_type(
@@ -1149,15 +951,15 @@
     name_mapping={"inline_code": "inlineCode", "s3_location": "s3Location"},
 )
 class CodeConfig:
     def __init__(
         self,
         *,
         inline_code: typing.Optional[builtins.str] = None,
-        s3_location: typing.Optional[typing.Union[_aws_cdk_aws_s3_ceddda9d.Location, typing.Dict[builtins.str, typing.Any]]] = None,
+        s3_location: typing.Optional[aws_cdk.aws_s3.Location] = None,
     ) -> None:
         '''(experimental) Configuration of the code class.
 
         :param inline_code: (experimental) Inline code (mutually exclusive with ``s3Location``). Default: - none
         :param s3_location: (experimental) The location of the code in S3 (mutually exclusive with ``inlineCode``). Default: - none
 
         :stability: experimental
@@ -1177,20 +979,16 @@
             
                     # the properties below are optional
                     object_version="objectVersion"
                 )
             )
         '''
         if isinstance(s3_location, dict):
-            s3_location = _aws_cdk_aws_s3_ceddda9d.Location(**s3_location)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__651318556062d0bfa41111177f4d584c07af87721369012008e7234cd7a9bc9d)
-            check_type(argname="argument inline_code", value=inline_code, expected_type=type_hints["inline_code"])
-            check_type(argname="argument s3_location", value=s3_location, expected_type=type_hints["s3_location"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+            s3_location = aws_cdk.aws_s3.Location(**s3_location)
+        self._values: typing.Dict[str, typing.Any] = {}
         if inline_code is not None:
             self._values["inline_code"] = inline_code
         if s3_location is not None:
             self._values["s3_location"] = s3_location
 
     @builtins.property
     def inline_code(self) -> typing.Optional[builtins.str]:
@@ -1200,23 +998,23 @@
 
         :stability: experimental
         '''
         result = self._values.get("inline_code")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def s3_location(self) -> typing.Optional[_aws_cdk_aws_s3_ceddda9d.Location]:
+    def s3_location(self) -> typing.Optional[aws_cdk.aws_s3.Location]:
         '''(experimental) The location of the code in S3 (mutually exclusive with ``inlineCode``).
 
         :default: - none
 
         :stability: experimental
         '''
         result = self._values.get("s3_location")
-        return typing.cast(typing.Optional[_aws_cdk_aws_s3_ceddda9d.Location], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_s3.Location], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -1264,22 +1062,15 @@
 
         Example::
 
             schedule = synthetics.Schedule.cron(
                 hour="0,8,16"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__742d0a0d854616bacaf4bdd6a72aad127dcb8726f67f61aa6c6b3864b56f48d9)
-            check_type(argname="argument day", value=day, expected_type=type_hints["day"])
-            check_type(argname="argument hour", value=hour, expected_type=type_hints["hour"])
-            check_type(argname="argument minute", value=minute, expected_type=type_hints["minute"])
-            check_type(argname="argument month", value=month, expected_type=type_hints["month"])
-            check_type(argname="argument week_day", value=week_day, expected_type=type_hints["week_day"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if day is not None:
             self._values["day"] = day
         if hour is not None:
             self._values["hour"] = hour
         if minute is not None:
             self._values["minute"] = minute
         if month is not None:
@@ -1373,25 +1164,21 @@
 
             canary = synthetics.Canary(self, "MyCanary",
                 schedule=synthetics.Schedule.rate(Duration.minutes(5)),
                 test=synthetics.Test.custom(
                     code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
                     handler="index.handler"
                 ),
-                runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0,
+                runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_1,
                 environment_variables={
                     "stage": "prod"
                 }
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d39435eead5e47a061f03cad4755b1155a750477abcae0773406c33664c00ba2)
-            check_type(argname="argument code", value=code, expected_type=type_hints["code"])
-            check_type(argname="argument handler", value=handler, expected_type=type_hints["handler"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "code": code,
             "handler": handler,
         }
 
     @builtins.property
     def code(self) -> Code:
         '''(experimental) The code of the canary script.
@@ -1447,39 +1234,31 @@
 
     def __init__(self, code: builtins.str) -> None:
         '''
         :param code: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__da247d1ca5cbecd8aaea9b8c84a618be5cc639917820e7ecc42df6986fc5041c)
-            check_type(argname="argument code", value=code, expected_type=type_hints["code"])
         jsii.create(self.__class__, self, [code])
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
-        _scope: _constructs_77d1e7e8.Construct,
+        _scope: constructs.Construct,
         handler: builtins.str,
         _family: "RuntimeFamily",
     ) -> CodeConfig:
         '''(experimental) Called when the canary is initialized to allow this object to bind to the stack, add resources and have fun.
 
         :param _scope: -
         :param handler: -
         :param _family: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6275d20cffbb7f9580a932831ea3fe3cd5b65bfb421b1f8b04d770dc3508f7f3)
-            check_type(argname="argument _scope", value=_scope, expected_type=type_hints["_scope"])
-            check_type(argname="argument handler", value=handler, expected_type=type_hints["handler"])
-            check_type(argname="argument _family", value=_family, expected_type=type_hints["_family"])
         return typing.cast(CodeConfig, jsii.invoke(self, "bind", [_scope, handler, _family]))
 
 
 class Runtime(
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-synthetics-alpha.Runtime",
 ):
@@ -1492,342 +1271,156 @@
 
         canary = synthetics.Canary(self, "MyCanary",
             schedule=synthetics.Schedule.rate(Duration.minutes(5)),
             test=synthetics.Test.custom(
                 code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
                 handler="index.handler"
             ),
-            runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0,
+            runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_1,
             environment_variables={
                 "stage": "prod"
             }
         )
     '''
 
     def __init__(self, name: builtins.str, family: "RuntimeFamily") -> None:
         '''
         :param name: The name of the runtime version.
         :param family: The Lambda runtime family.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4f432dbd029db5a952a9c04e6756b31fce0e5e19c4f214b45729fe31a4228a68)
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
-            check_type(argname="argument family", value=family, expected_type=type_hints["family"])
         jsii.create(self.__class__, self, [name, family])
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="SYNTHETICS_1_0")
     def SYNTHETICS_1_0(cls) -> "Runtime":
-        '''(deprecated) **Deprecated by AWS Synthetics. You can't create canaries with deprecated runtimes.**.
+        '''(experimental) **Deprecated by AWS Synthetics. You can't create canaries with deprecated runtimes.**.
 
         ``syn-1.0`` includes the following:
 
         - Synthetics library 1.0
         - Synthetics handler code 1.0
         - Lambda runtime Node.js 10.x
         - Puppeteer-core version 1.14.0
         - The Chromium version that matches Puppeteer-core 1.14.0
 
-        :deprecated: Use the latest version instead
-
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_nodejs_puppeteer.html#CloudWatch_Synthetics_runtimeversion-1.0
-        :stability: deprecated
+        :stability: experimental
         '''
         return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_1_0"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="SYNTHETICS_NODEJS_2_0")
     def SYNTHETICS_NODEJS_2_0(cls) -> "Runtime":
-        '''(deprecated) **Deprecated by AWS Synthetics. You can't create canaries with deprecated runtimes.**.
+        '''(experimental) **Deprecated by AWS Synthetics. You can't create canaries with deprecated runtimes.**.
 
         ``syn-nodejs-2.0`` includes the following:
 
         - Lambda runtime Node.js 10.x
         - Puppeteer-core version 3.3.0
         - Chromium version 83.0.4103.0
 
-        :deprecated: Use the latest version instead
-
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_nodejs_puppeteer.html#CloudWatch_Synthetics_runtimeversion-2.0
-        :stability: deprecated
+        :stability: experimental
         '''
         return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_NODEJS_2_0"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="SYNTHETICS_NODEJS_2_1")
     def SYNTHETICS_NODEJS_2_1(cls) -> "Runtime":
-        '''(deprecated) **Deprecated by AWS Synthetics. You can't create canaries with deprecated runtimes.**.
+        '''(experimental) **Deprecated by AWS Synthetics. You can't create canaries with deprecated runtimes.**.
 
         ``syn-nodejs-2.1`` includes the following:
 
         - Lambda runtime Node.js 10.x
         - Puppeteer-core version 3.3.0
         - Chromium version 83.0.4103.0
 
-        :deprecated: Use the latest version instead
-
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_nodejs_puppeteer.html#CloudWatch_Synthetics_runtimeversion-2.1
-        :stability: deprecated
+        :stability: experimental
         '''
         return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_NODEJS_2_1"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="SYNTHETICS_NODEJS_2_2")
     def SYNTHETICS_NODEJS_2_2(cls) -> "Runtime":
-        '''(deprecated) **Deprecated by AWS Synthetics. You can't create canaries with deprecated runtimes.**.
+        '''(experimental) **Deprecated by AWS Synthetics. You can't create canaries with deprecated runtimes.**.
 
         ``syn-nodejs-2.2`` includes the following:
 
         - Lambda runtime Node.js 10.x
         - Puppeteer-core version 3.3.0
         - Chromium version 83.0.4103.0
 
-        :deprecated: Use the latest version instead
-
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_nodejs_puppeteer.html#CloudWatch_Synthetics_runtimeversion-2.2
-        :stability: deprecated
+        :stability: experimental
         '''
         return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_NODEJS_2_2"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="SYNTHETICS_NODEJS_PUPPETEER_3_0")
     def SYNTHETICS_NODEJS_PUPPETEER_3_0(cls) -> "Runtime":
-        '''(deprecated) **Deprecated by AWS Synthetics. You can't create canaries with deprecated runtimes.**.
-
-        ``syn-nodejs-puppeteer-3.0`` includes the following:
-
-        - Lambda runtime Node.js 12.x
-        - Puppeteer-core version 5.5.0
-        - Chromium version 88.0.4298.0
-
-        :deprecated: Use the latest version instead
+        '''(experimental) ``syn-nodejs-puppeteer-3.0`` includes the following: - Lambda runtime Node.js 12.x - Puppeteer-core version 5.5.0 - Chromium version 88.0.4298.0.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_nodejs_puppeteer.html#CloudWatch_Synthetics_runtimeversion-nodejs-puppeteer-3.0
-        :stability: deprecated
+        :stability: experimental
         '''
         return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_NODEJS_PUPPETEER_3_0"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="SYNTHETICS_NODEJS_PUPPETEER_3_1")
     def SYNTHETICS_NODEJS_PUPPETEER_3_1(cls) -> "Runtime":
-        '''(deprecated) **Deprecated by AWS Synthetics. You can't create canaries with deprecated runtimes.**.
-
-        ``syn-nodejs-puppeteer-3.1`` includes the following:
-
-        - Lambda runtime Node.js 12.x
-        - Puppeteer-core version 5.5.0
-        - Chromium version 88.0.4298.0
-
-        :deprecated: Use the latest version instead
+        '''(experimental) ``syn-nodejs-puppeteer-3.1`` includes the following: - Lambda runtime Node.js 12.x - Puppeteer-core version 5.5.0 - Chromium version 88.0.4298.0.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_nodejs_puppeteer.html#CloudWatch_Synthetics_runtimeversion-nodejs-puppeteer-3.1
-        :stability: deprecated
+        :stability: experimental
         '''
         return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_NODEJS_PUPPETEER_3_1"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="SYNTHETICS_NODEJS_PUPPETEER_3_2")
     def SYNTHETICS_NODEJS_PUPPETEER_3_2(cls) -> "Runtime":
-        '''(deprecated) **Deprecated by AWS Synthetics. You can't create canaries with deprecated runtimes.**.
-
-        ``syn-nodejs-puppeteer-3.2`` includes the following:
-
-        - Lambda runtime Node.js 12.x
-        - Puppeteer-core version 5.5.0
-        - Chromium version 88.0.4298.0
-
-        :deprecated: Use the latest version instead
+        '''(experimental) ``syn-nodejs-puppeteer-3.2`` includes the following: - Lambda runtime Node.js 12.x - Puppeteer-core version 5.5.0 - Chromium version 88.0.4298.0.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_nodejs_puppeteer.html#CloudWatch_Synthetics_runtimeversion-nodejs-puppeteer-3.2
-        :stability: deprecated
+        :stability: experimental
         '''
         return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_NODEJS_PUPPETEER_3_2"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="SYNTHETICS_NODEJS_PUPPETEER_3_3")
     def SYNTHETICS_NODEJS_PUPPETEER_3_3(cls) -> "Runtime":
-        '''(deprecated) ``syn-nodejs-puppeteer-3.3`` includes the following: **Deprecated by AWS Synthetics. You can't create canaries with deprecated runtimes.**.
-
-        - Lambda runtime Node.js 12.x
-        - Puppeteer-core version 5.5.0
-        - Chromium version 88.0.4298.0
-
-        :deprecated: Use the latest version instead
+        '''(experimental) ``syn-nodejs-puppeteer-3.3`` includes the following: - Lambda runtime Node.js 12.x - Puppeteer-core version 5.5.0 - Chromium version 88.0.4298.0.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_nodejs_puppeteer.html#CloudWatch_Synthetics_runtimeversion-nodejs-puppeteer-3.3
-        :stability: deprecated
-        '''
-        return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_NODEJS_PUPPETEER_3_3"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="SYNTHETICS_NODEJS_PUPPETEER_3_4")
-    def SYNTHETICS_NODEJS_PUPPETEER_3_4(cls) -> "Runtime":
-        '''(deprecated) **Deprecated by AWS Synthetics. You can't create canaries with deprecated runtimes.**.
-
-        ``syn-nodejs-puppeteer-3.4`` includes the following:
-
-        - Lambda runtime Node.js 12.x
-        - Puppeteer-core version 5.5.0
-        - Chromium version 88.0.4298.0
-
-        :deprecated: Use the latest version instead
-
-        :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_nodejs_puppeteer.html#CloudWatch_Synthetics_runtimeversion-nodejs-puppeteer-3.4
-        :stability: deprecated
-        '''
-        return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_NODEJS_PUPPETEER_3_4"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="SYNTHETICS_NODEJS_PUPPETEER_3_5")
-    def SYNTHETICS_NODEJS_PUPPETEER_3_5(cls) -> "Runtime":
-        '''(experimental) ``syn-nodejs-puppeteer-3.5`` includes the following: - Lambda runtime Node.js 14.x - Puppeteer-core version 10.1.0 - Chromium version 92.0.4512.
-
-        :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_nodejs_puppeteer.html#CloudWatch_Synthetics_runtimeversion-nodejs-puppeteer-3.5
-        :stability: experimental
-        '''
-        return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_NODEJS_PUPPETEER_3_5"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="SYNTHETICS_NODEJS_PUPPETEER_3_6")
-    def SYNTHETICS_NODEJS_PUPPETEER_3_6(cls) -> "Runtime":
-        '''(experimental) ``syn-nodejs-puppeteer-3.6`` includes the following: - Lambda runtime Node.js 14.x - Puppeteer-core version 10.1.0 - Chromium version 92.0.4512.
-
-        :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_nodejs_puppeteer.html#CloudWatch_Synthetics_runtimeversion-nodejs-puppeteer-3.6
-        :stability: experimental
-        '''
-        return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_NODEJS_PUPPETEER_3_6"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="SYNTHETICS_NODEJS_PUPPETEER_3_7")
-    def SYNTHETICS_NODEJS_PUPPETEER_3_7(cls) -> "Runtime":
-        '''(experimental) ``syn-nodejs-puppeteer-3.7`` includes the following: - Lambda runtime Node.js 14.x - Puppeteer-core version 10.1.0 - Chromium version 92.0.4512.
-
-        New Features:
-
-        - **Logging enhancement**: The canary will upload logs to Amazon S3 even if it times out or crashes.
-        - **Lambda layer size reduced**: The size of the Lambda layer used for canaries is reduced by 34%.
-
-        :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_nodejs_puppeteer.html#CloudWatch_Synthetics_runtimeversion-nodejs-puppeteer-3.7
-        :stability: experimental
-        '''
-        return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_NODEJS_PUPPETEER_3_7"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="SYNTHETICS_NODEJS_PUPPETEER_3_8")
-    def SYNTHETICS_NODEJS_PUPPETEER_3_8(cls) -> "Runtime":
-        '''(experimental) ``syn-nodejs-puppeteer-3.8`` includes the following: - Lambda runtime Node.js 14.x - Puppeteer-core version 10.1.0 - Chromium version 92.0.4512.
-
-        New Features:
-
-        - **Profile cleanup**: Chromium profiles are now cleaned up after each canary run.
-
-        :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_nodejs_puppeteer.html#CloudWatch_Synthetics_runtimeversion-nodejs-puppeteer-3.8
-        :stability: experimental
-        '''
-        return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_NODEJS_PUPPETEER_3_8"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="SYNTHETICS_NODEJS_PUPPETEER_3_9")
-    def SYNTHETICS_NODEJS_PUPPETEER_3_9(cls) -> "Runtime":
-        '''(experimental) ``syn-nodejs-puppeteer-3.9`` includes the following:.
-
-        - Lambda runtime Node.js 14.x
-        - Puppeteer-core version 5.5.0
-        - Chromium version 92.0.4512
-
-        New Features:
-
-        - **Dependency upgrades**: Upgrades some third-party dependency packages.
-
-        :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_nodejs_puppeteer.html#CloudWatch_Synthetics_runtimeversion-nodejs-puppeteer-3.9
-        :stability: experimental
-        '''
-        return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_NODEJS_PUPPETEER_3_9"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="SYNTHETICS_NODEJS_PUPPETEER_4_0")
-    def SYNTHETICS_NODEJS_PUPPETEER_4_0(cls) -> "Runtime":
-        '''(experimental) ``syn-nodejs-puppeteer-4.0`` includes the following: - Lambda runtime Node.js 16.x - Puppeteer-core version 5.5.0 - Chromium version 92.0.4512.
-
-        New Features:
-
-        - **Dependency upgrades**: The Node.js dependency is updated to 16.x.
-
-        :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_nodejs_puppeteer.html#CloudWatch_Synthetics_runtimeversion-nodejs-puppeteer-4.0
         :stability: experimental
         '''
-        return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_NODEJS_PUPPETEER_4_0"))
+        return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_NODEJS_PUPPETEER_3_3"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="SYNTHETICS_PYTHON_SELENIUM_1_0")
     def SYNTHETICS_PYTHON_SELENIUM_1_0(cls) -> "Runtime":
         '''(experimental) ``syn-python-selenium-1.0`` includes the following: - Lambda runtime Python 3.8 - Selenium version 3.141.0 - Chromium version 83.0.4103.0.
 
-        :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_python_selenium.html#CloudWatch_Synthetics_runtimeversion-syn-python-selenium-1.0
+        :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_python_selenium.html
         :stability: experimental
         '''
         return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_PYTHON_SELENIUM_1_0"))
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="SYNTHETICS_PYTHON_SELENIUM_1_1")
-    def SYNTHETICS_PYTHON_SELENIUM_1_1(cls) -> "Runtime":
-        '''(experimental) ``syn-python-selenium-1.1`` includes the following: - Lambda runtime Python 3.8 - Selenium version 3.141.0 - Chromium version 83.0.4103.0.
-
-        New Features:
-
-        - **Custom handler function**: You can now use a custom handler function for your canary scripts.
-        - **Configuration options for adding metrics and step failure configurations**: These options were already available in runtimes for Node.js canaries.
-        - **Custom arguments in Chrome**: You can now open a browser in incognito mode or pass in proxy server configuration.
-        - **Cross-Region artifact buckets**: A canary can store its artifacts in an Amazon S3 bucket in a different Region.
-
-        :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_python_selenium.html#CloudWatch_Synthetics_runtimeversion-syn-python-selenium-1.1
-        :stability: experimental
-        '''
-        return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_PYTHON_SELENIUM_1_1"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="SYNTHETICS_PYTHON_SELENIUM_1_2")
-    def SYNTHETICS_PYTHON_SELENIUM_1_2(cls) -> "Runtime":
-        '''(experimental) ``syn-python-selenium-1.2`` includes the following: - Lambda runtime Python 3.8 - Selenium version 3.141.0 - Chromium version 92.0.4512.0.
-
-        New Features:
-
-        - **Updated dependencies**: The only new features in this runtime are the updated dependencies.
-
-        :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_python_selenium.html#CloudWatch_Synthetics_runtimeversion-syn-python-selenium-1.2
-        :stability: experimental
-        '''
-        return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_PYTHON_SELENIUM_1_2"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="SYNTHETICS_PYTHON_SELENIUM_1_3")
-    def SYNTHETICS_PYTHON_SELENIUM_1_3(cls) -> "Runtime":
-        '''(experimental) ``syn-python-selenium-1.3`` includes the following: - Lambda runtime Python 3.8 - Selenium version 3.141.0 - Chromium version 92.0.4512.0.
-
-        New Features:
-
-        - **More precise timestamps**: The start time and stop time of canary runs are now precise to the millisecond.
-
-        :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Library_python_selenium.html#CloudWatch_Synthetics_runtimeversion-syn-python-selenium-1.3
-        :stability: experimental
-        '''
-        return typing.cast("Runtime", jsii.sget(cls, "SYNTHETICS_PYTHON_SELENIUM_1_3"))
-
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="family")
     def family(self) -> "RuntimeFamily":
         '''(experimental) The Lambda runtime family.
 
         :stability: experimental
         '''
         return typing.cast("RuntimeFamily", jsii.get(self, "family"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         '''(experimental) The name of the runtime version.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "name"))
@@ -1877,52 +1470,42 @@
         # bucket: s3.Bucket
         
         s3_code = synthetics_alpha.S3Code(bucket, "key", "objectVersion")
     '''
 
     def __init__(
         self,
-        bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        bucket: aws_cdk.aws_s3.IBucket,
         key: builtins.str,
         object_version: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param bucket: -
         :param key: -
         :param object_version: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b38ad713f473c7c074c298bcd50e4520db7596d9bbfee5b75e35fd29ecc2ae71)
-            check_type(argname="argument bucket", value=bucket, expected_type=type_hints["bucket"])
-            check_type(argname="argument key", value=key, expected_type=type_hints["key"])
-            check_type(argname="argument object_version", value=object_version, expected_type=type_hints["object_version"])
         jsii.create(self.__class__, self, [bucket, key, object_version])
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
-        _scope: _constructs_77d1e7e8.Construct,
+        _scope: constructs.Construct,
         _handler: builtins.str,
         _family: RuntimeFamily,
     ) -> CodeConfig:
         '''(experimental) Called when the canary is initialized to allow this object to bind to the stack, add resources and have fun.
 
         :param _scope: -
         :param _handler: -
         :param _family: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5715f987d53b5baf64123cc83ba9844c119abb443bcd5f14c619000f4687689b)
-            check_type(argname="argument _scope", value=_scope, expected_type=type_hints["_scope"])
-            check_type(argname="argument _handler", value=_handler, expected_type=type_hints["_handler"])
-            check_type(argname="argument _family", value=_family, expected_type=type_hints["_family"])
         return typing.cast(CodeConfig, jsii.invoke(self, "bind", [_scope, _handler, _family]))
 
 
 class Schedule(
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-synthetics-alpha.Schedule",
 ):
@@ -1932,15 +1515,15 @@
     :exampleMetadata: infused
 
     Example::
 
         schedule = synthetics.Schedule.rate(Duration.minutes(5))
     '''
 
-    @jsii.member(jsii_name="cron")
+    @jsii.member(jsii_name="cron") # type: ignore[misc]
     @builtins.classmethod
     def cron(
         cls,
         *,
         day: typing.Optional[builtins.str] = None,
         hour: typing.Optional[builtins.str] = None,
         minute: typing.Optional[builtins.str] = None,
@@ -1959,58 +1542,52 @@
         '''
         options = CronOptions(
             day=day, hour=hour, minute=minute, month=month, week_day=week_day
         )
 
         return typing.cast("Schedule", jsii.sinvoke(cls, "cron", [options]))
 
-    @jsii.member(jsii_name="expression")
+    @jsii.member(jsii_name="expression") # type: ignore[misc]
     @builtins.classmethod
     def expression(cls, expression: builtins.str) -> "Schedule":
         '''(experimental) Construct a schedule from a literal schedule expression.
 
         The expression must be in a ``rate(number units)`` format.
         For example, ``Schedule.expression('rate(10 minutes)')``
 
         :param expression: The expression to use.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__67f4f45e1902e3d8ba8eb545d45bd88f6630cdbcfd293fb8ce069c9a9d32e633)
-            check_type(argname="argument expression", value=expression, expected_type=type_hints["expression"])
         return typing.cast("Schedule", jsii.sinvoke(cls, "expression", [expression]))
 
-    @jsii.member(jsii_name="once")
+    @jsii.member(jsii_name="once") # type: ignore[misc]
     @builtins.classmethod
     def once(cls) -> "Schedule":
         '''(experimental) The canary will be executed once.
 
         :stability: experimental
         '''
         return typing.cast("Schedule", jsii.sinvoke(cls, "once", []))
 
-    @jsii.member(jsii_name="rate")
+    @jsii.member(jsii_name="rate") # type: ignore[misc]
     @builtins.classmethod
-    def rate(cls, interval: _aws_cdk_ceddda9d.Duration) -> "Schedule":
+    def rate(cls, interval: aws_cdk.Duration) -> "Schedule":
         '''(experimental) Construct a schedule from an interval.
 
         Allowed values: 0 (for a single run) or between 1 and 60 minutes.
         To specify a single run, you can use ``Schedule.once()``.
 
         :param interval: The interval at which to run the canary.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ed81e99d860f614edbd9653f58417542e72548f67d8562ec60e3581ea3c1b7a5)
-            check_type(argname="argument interval", value=interval, expected_type=type_hints["interval"])
         return typing.cast("Schedule", jsii.sinvoke(cls, "rate", [interval]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="expressionString")
     def expression_string(self) -> builtins.str:
         '''(experimental) The Schedule expression.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "expressionString"))
@@ -2026,22 +1603,22 @@
 
         canary = synthetics.Canary(self, "MyCanary",
             schedule=synthetics.Schedule.rate(Duration.minutes(5)),
             test=synthetics.Test.custom(
                 code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
                 handler="index.handler"
             ),
-            runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0,
+            runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_1,
             environment_variables={
                 "stage": "prod"
             }
         )
     '''
 
-    @jsii.member(jsii_name="custom")
+    @jsii.member(jsii_name="custom") # type: ignore[misc]
     @builtins.classmethod
     def custom(cls, *, code: Code, handler: builtins.str) -> "Test":
         '''(experimental) Specify a custom test with your own code.
 
         :param code: (experimental) The code of the canary script.
         :param handler: (experimental) The handler for the code. Must end with ``.handler``.
 
@@ -2049,24 +1626,24 @@
 
         :stability: experimental
         '''
         options = CustomTestOptions(code=code, handler=handler)
 
         return typing.cast("Test", jsii.sinvoke(cls, "custom", [options]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="code")
     def code(self) -> Code:
         '''(experimental) The code that the canary should run.
 
         :stability: experimental
         '''
         return typing.cast(Code, jsii.get(self, "code"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="handler")
     def handler(self) -> builtins.str:
         '''(experimental) The handler of the canary.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "handler"))
@@ -2097,105 +1674,90 @@
         asset_code = synthetics_alpha.AssetCode("assetPath",
             asset_hash="assetHash",
             asset_hash_type=cdk.AssetHashType.SOURCE,
             bundling=cdk.BundlingOptions(
                 image=docker_image,
         
                 # the properties below are optional
-                bundling_file_access=cdk.BundlingFileAccess.VOLUME_COPY,
                 command=["command"],
                 entrypoint=["entrypoint"],
                 environment={
                     "environment_key": "environment"
                 },
                 local=local_bundling,
-                network="network",
                 output_type=cdk.BundlingOutput.ARCHIVED,
                 security_opt="securityOpt",
                 user="user",
                 volumes=[cdk.DockerVolume(
                     container_path="containerPath",
                     host_path="hostPath",
         
                     # the properties below are optional
                     consistency=cdk.DockerVolumeConsistency.CONSISTENT
                 )],
-                volumes_from=["volumesFrom"],
                 working_directory="workingDirectory"
             ),
-            deploy_time=False,
             exclude=["exclude"],
             follow_symlinks=cdk.SymlinkFollowMode.NEVER,
             ignore_mode=cdk.IgnoreMode.GLOB,
             readers=[grantable]
         )
     '''
 
     def __init__(
         self,
         asset_path: builtins.str,
         *,
-        deploy_time: typing.Optional[builtins.bool] = None,
-        readers: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.IGrantable]] = None,
+        readers: typing.Optional[typing.Sequence[aws_cdk.aws_iam.IGrantable]] = None,
         asset_hash: typing.Optional[builtins.str] = None,
-        asset_hash_type: typing.Optional[_aws_cdk_ceddda9d.AssetHashType] = None,
-        bundling: typing.Optional[typing.Union[_aws_cdk_ceddda9d.BundlingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        asset_hash_type: typing.Optional[aws_cdk.AssetHashType] = None,
+        bundling: typing.Optional[aws_cdk.BundlingOptions] = None,
         exclude: typing.Optional[typing.Sequence[builtins.str]] = None,
-        follow_symlinks: typing.Optional[_aws_cdk_ceddda9d.SymlinkFollowMode] = None,
-        ignore_mode: typing.Optional[_aws_cdk_ceddda9d.IgnoreMode] = None,
+        follow_symlinks: typing.Optional[aws_cdk.SymlinkFollowMode] = None,
+        ignore_mode: typing.Optional[aws_cdk.IgnoreMode] = None,
     ) -> None:
         '''
         :param asset_path: The path to the asset file or directory.
-        :param deploy_time: Whether or not the asset needs to exist beyond deployment time; i.e. are copied over to a different location and not needed afterwards. Setting this property to true has an impact on the lifecycle of the asset, because we will assume that it is safe to delete after the CloudFormation deployment succeeds. For example, Lambda Function assets are copied over to Lambda during deployment. Therefore, it is not necessary to store the asset in S3, so we consider those deployTime assets. Default: false
         :param readers: A list of principals that should be able to read this asset from S3. You can use ``asset.grantRead(principal)`` to grant read permissions later. Default: - No principals that can read file asset.
         :param asset_hash: Specify a custom hash for this asset. If ``assetHashType`` is set it must be set to ``AssetHashType.CUSTOM``. For consistency, this custom hash will be SHA256 hashed and encoded as hex. The resulting hash will be the asset hash. NOTE: the hash is used in order to identify a specific revision of the asset, and used for optimizing and caching deployment activities related to this asset such as packaging, uploading to Amazon S3, etc. If you chose to customize the hash, you will need to make sure it is updated every time the asset changes, or otherwise it is possible that some deployments will not be invalidated. Default: - based on ``assetHashType``
         :param asset_hash_type: Specifies the type of hash to calculate for this asset. If ``assetHash`` is configured, this option must be ``undefined`` or ``AssetHashType.CUSTOM``. Default: - the default is ``AssetHashType.SOURCE``, but if ``assetHash`` is explicitly specified this value defaults to ``AssetHashType.CUSTOM``.
         :param bundling: Bundle the asset by executing a command in a Docker container or a custom bundling provider. The asset path will be mounted at ``/asset-input``. The Docker container is responsible for putting content at ``/asset-output``. The content at ``/asset-output`` will be zipped and used as the final asset. Default: - uploaded as-is to S3 if the asset is a regular file or a .zip file, archived into a .zip file and uploaded to S3 otherwise
-        :param exclude: File paths matching the patterns will be excluded. See ``ignoreMode`` to set the matching behavior. Has no effect on Assets bundled using the ``bundling`` property. Default: - nothing is excluded
+        :param exclude: Glob patterns to exclude from the copy. Default: - nothing is excluded
         :param follow_symlinks: A strategy for how to handle symlinks. Default: SymlinkFollowMode.NEVER
-        :param ignore_mode: The ignore behavior to use for ``exclude`` patterns. Default: IgnoreMode.GLOB
+        :param ignore_mode: The ignore behavior to use for exclude patterns. Default: IgnoreMode.GLOB
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8bf4f7b9198aa65c5cde28608e12d3a1aaeec0ce84754b8fbb221ea9a3432c7d)
-            check_type(argname="argument asset_path", value=asset_path, expected_type=type_hints["asset_path"])
-        options = _aws_cdk_aws_s3_assets_ceddda9d.AssetOptions(
-            deploy_time=deploy_time,
+        options = aws_cdk.aws_s3_assets.AssetOptions(
             readers=readers,
             asset_hash=asset_hash,
             asset_hash_type=asset_hash_type,
             bundling=bundling,
             exclude=exclude,
             follow_symlinks=follow_symlinks,
             ignore_mode=ignore_mode,
         )
 
         jsii.create(self.__class__, self, [asset_path, options])
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         handler: builtins.str,
         family: RuntimeFamily,
     ) -> CodeConfig:
         '''(experimental) Called when the canary is initialized to allow this object to bind to the stack, add resources and have fun.
 
         :param scope: -
         :param handler: -
         :param family: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__143fc4bffb5cfb09c7d51862845fedf3824b9a58f7e721a8ed7a6f4907e17f47)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument handler", value=handler, expected_type=type_hints["handler"])
-            check_type(argname="argument family", value=family, expected_type=type_hints["family"])
         return typing.cast(CodeConfig, jsii.invoke(self, "bind", [scope, handler, family]))
 
 
 __all__ = [
     "ArtifactsBucketLocation",
     "AssetCode",
     "Canary",
@@ -2209,195 +1771,7 @@
     "RuntimeFamily",
     "S3Code",
     "Schedule",
     "Test",
 ]
 
 publication.publish()
-
-def _typecheckingstub__c97027ffb7c3e1ed6531ba25f1eb4e6e2af525b8b67b6ace4855effcca2b9919(
-    *,
-    bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
-    prefix: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__77f74ffae78f48cc052608780149daa4ac131f47fdbfc7d99da3a7883cc0e8a3(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    runtime: Runtime,
-    test: Test,
-    artifacts_bucket_location: typing.Optional[typing.Union[ArtifactsBucketLocation, typing.Dict[builtins.str, typing.Any]]] = None,
-    canary_name: typing.Optional[builtins.str] = None,
-    enable_auto_delete_lambdas: typing.Optional[builtins.bool] = None,
-    environment_variables: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-    failure_retention_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-    schedule: typing.Optional[Schedule] = None,
-    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-    start_after_creation: typing.Optional[builtins.bool] = None,
-    success_retention_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    time_to_live: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
-    vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__ae7e63c36ba56bf570a16580ca3cc6aa4f4d25f66ba54d26f3f7a90413d04d63(
-    *,
-    runtime: Runtime,
-    test: Test,
-    artifacts_bucket_location: typing.Optional[typing.Union[ArtifactsBucketLocation, typing.Dict[builtins.str, typing.Any]]] = None,
-    canary_name: typing.Optional[builtins.str] = None,
-    enable_auto_delete_lambdas: typing.Optional[builtins.bool] = None,
-    environment_variables: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-    failure_retention_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-    schedule: typing.Optional[Schedule] = None,
-    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-    start_after_creation: typing.Optional[builtins.bool] = None,
-    success_retention_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    time_to_live: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
-    vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__4c04ee0a7f625fce33d3003e388d6a831237f31cbc709e9c551a1bc356475ede(
-    asset_path: builtins.str,
-    *,
-    deploy_time: typing.Optional[builtins.bool] = None,
-    readers: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.IGrantable]] = None,
-    asset_hash: typing.Optional[builtins.str] = None,
-    asset_hash_type: typing.Optional[_aws_cdk_ceddda9d.AssetHashType] = None,
-    bundling: typing.Optional[typing.Union[_aws_cdk_ceddda9d.BundlingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    exclude: typing.Optional[typing.Sequence[builtins.str]] = None,
-    follow_symlinks: typing.Optional[_aws_cdk_ceddda9d.SymlinkFollowMode] = None,
-    ignore_mode: typing.Optional[_aws_cdk_ceddda9d.IgnoreMode] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__628908b4951e36d41574e89af118f4b8a140822fc9499275e081e1168a75bf43(
-    bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
-    key: builtins.str,
-    object_version: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__534ebde2ca6177d2b07962ff163fa4be8fff02237e20a67c89fca238f2a43b12(
-    code: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__5d4fce9f2879e280253f79f346736f1e74cabefddf0199d5d40b9e187d207f46(
-    scope: _constructs_77d1e7e8.Construct,
-    handler: builtins.str,
-    family: RuntimeFamily,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__651318556062d0bfa41111177f4d584c07af87721369012008e7234cd7a9bc9d(
-    *,
-    inline_code: typing.Optional[builtins.str] = None,
-    s3_location: typing.Optional[typing.Union[_aws_cdk_aws_s3_ceddda9d.Location, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__742d0a0d854616bacaf4bdd6a72aad127dcb8726f67f61aa6c6b3864b56f48d9(
-    *,
-    day: typing.Optional[builtins.str] = None,
-    hour: typing.Optional[builtins.str] = None,
-    minute: typing.Optional[builtins.str] = None,
-    month: typing.Optional[builtins.str] = None,
-    week_day: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__d39435eead5e47a061f03cad4755b1155a750477abcae0773406c33664c00ba2(
-    *,
-    code: Code,
-    handler: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__da247d1ca5cbecd8aaea9b8c84a618be5cc639917820e7ecc42df6986fc5041c(
-    code: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__6275d20cffbb7f9580a932831ea3fe3cd5b65bfb421b1f8b04d770dc3508f7f3(
-    _scope: _constructs_77d1e7e8.Construct,
-    handler: builtins.str,
-    _family: RuntimeFamily,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__4f432dbd029db5a952a9c04e6756b31fce0e5e19c4f214b45729fe31a4228a68(
-    name: builtins.str,
-    family: RuntimeFamily,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b38ad713f473c7c074c298bcd50e4520db7596d9bbfee5b75e35fd29ecc2ae71(
-    bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
-    key: builtins.str,
-    object_version: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__5715f987d53b5baf64123cc83ba9844c119abb443bcd5f14c619000f4687689b(
-    _scope: _constructs_77d1e7e8.Construct,
-    _handler: builtins.str,
-    _family: RuntimeFamily,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__67f4f45e1902e3d8ba8eb545d45bd88f6630cdbcfd293fb8ce069c9a9d32e633(
-    expression: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__ed81e99d860f614edbd9653f58417542e72548f67d8562ec60e3581ea3c1b7a5(
-    interval: _aws_cdk_ceddda9d.Duration,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__8bf4f7b9198aa65c5cde28608e12d3a1aaeec0ce84754b8fbb221ea9a3432c7d(
-    asset_path: builtins.str,
-    *,
-    deploy_time: typing.Optional[builtins.bool] = None,
-    readers: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.IGrantable]] = None,
-    asset_hash: typing.Optional[builtins.str] = None,
-    asset_hash_type: typing.Optional[_aws_cdk_ceddda9d.AssetHashType] = None,
-    bundling: typing.Optional[typing.Union[_aws_cdk_ceddda9d.BundlingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    exclude: typing.Optional[typing.Sequence[builtins.str]] = None,
-    follow_symlinks: typing.Optional[_aws_cdk_ceddda9d.SymlinkFollowMode] = None,
-    ignore_mode: typing.Optional[_aws_cdk_ceddda9d.IgnoreMode] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__143fc4bffb5cfb09c7d51862845fedf3824b9a58f7e721a8ed7a6f4907e17f47(
-    scope: _constructs_77d1e7e8.Construct,
-    handler: builtins.str,
-    family: RuntimeFamily,
-) -> None:
-    """Type checking stubs"""
-    pass
```

### Comparing `aws-cdk.aws-synthetics-alpha-2.84.0a0/src/aws_cdk.aws_synthetics_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-synthetics-alpha-2.9.0a0/src/aws_cdk.aws_synthetics_alpha.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-synthetics-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::Synthetics
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
 
 # Amazon CloudWatch Synthetics Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -58,15 +58,15 @@
 ```python
 canary = synthetics.Canary(self, "MyCanary",
     schedule=synthetics.Schedule.rate(Duration.minutes(5)),
     test=synthetics.Test.custom(
         code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
         handler="index.handler"
     ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0,
+    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_1,
     environment_variables={
         "stage": "prod"
     }
 )
 ```
 
 The following is an example of an `index.js` file which exports the `handler` function:
@@ -125,36 +125,14 @@
 schedule = synthetics.Schedule.cron(
     hour="0,8,16"
 )
 ```
 
 If you want the canary to run just once upon deployment, you can use `Schedule.once()`.
 
-### Canary DeleteLambdaResourcesOnCanaryDeletion
-
-You can specify whether the AWS CloudFormation is to also delete the Lambda functions and layers used by this canary, when the canary is deleted.
-
-This can be provisioned by setting the `enableAutoDeleteLambdas` property to `true` when we define the canary.
-
-```python
-stack = Stack()
-
-canary = synthetics.Canary(stack, "Canary",
-    test=synthetics.Test.custom(
-        handler="index.handler",
-        code=synthetics.Code.from_inline("/* Synthetics handler code")
-    ),
-    enable_auto_delete_lambdas=True,
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0
-)
-```
-
-Synthetic Canaries create additional resources under the hood beyond Lambda functions. Setting `enableAutoDeleteLambdas: true` will take care of
-cleaning up Lambda functions on deletion, but you still have to manually delete other resources like S3 buckets and CloudWatch logs.
-
 ### Configuring the Canary Script
 
 To configure the script the canary executes, use the `test` property. The `test` property accepts a `Test` instance that can be initialized by the `Test` class static methods. Currently, the only implemented method is `Test.custom()`, which allows you to bring your own code. In the future, other methods will be added. `Test.custom()` accepts `code` and `handler` properties -- both are required by Synthetics to create a lambda function on your behalf.
 
 The `synthetics.Code` class exposes static methods to bundle your code artifacts:
 
 * `code.fromInline(code)` - specify an inline script.
@@ -168,32 +146,32 @@
 import aws_cdk.aws_s3 as s3
 # To supply the code inline:
 synthetics.Canary(self, "Inline Canary",
     test=synthetics.Test.custom(
         code=synthetics.Code.from_inline("/* Synthetics handler code */"),
         handler="index.handler"
     ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0
+    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_3
 )
 
 # To supply the code from your local filesystem:
 synthetics.Canary(self, "Asset Canary",
     test=synthetics.Test.custom(
         code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
         handler="index.handler"
     ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0
+    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_3
 )
 bucket = s3.Bucket(self, "Code Bucket")
 synthetics.Canary(self, "Bucket Canary",
     test=synthetics.Test.custom(
         code=synthetics.Code.from_bucket(bucket, "canary.zip"),
         handler="index.handler"
     ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0
+    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_3_3
 )
 ```
 
 > **Note:** Synthetics have a specified folder structure for canaries. For Node scripts supplied via `code.fromAsset()` or `code.fromBucket()`, the canary resource requires the following folder structure:
 >
 > ```plaintext
 > canary/
@@ -208,41 +186,14 @@
 > canary/
 > ├── python/
 >     ├── <filename>.py
 > ```
 >
 > See Synthetics [docs](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Canaries_WritingCanary.html).
 
-### Running a canary on a VPC
-
-You can specify what [VPC a canary executes in](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Canaries_VPC.html).
-This can allow for monitoring services that may be internal to a specific VPC. To place a canary within a VPC, you can specify the `vpc` property with the desired `VPC` to place then canary in.
-This will automatically attach the appropriate IAM permissions to attach to the VPC. This will also create a Security Group and attach to the default subnets for the VPC unless specified via `vpcSubnets` and `securityGroups`.
-
-```python
-import aws_cdk.aws_ec2 as ec2
-
-# vpc: ec2.IVpc
-
-synthetics.Canary(self, "Vpc Canary",
-    test=synthetics.Test.custom(
-        code=synthetics.Code.from_asset(path.join(__dirname, "canary")),
-        handler="index.handler"
-    ),
-    runtime=synthetics.Runtime.SYNTHETICS_NODEJS_PUPPETEER_4_0,
-    vpc=vpc
-)
-```
-
-> **Note:** By default, the Synthetics runtime needs access to the S3 and CloudWatch APIs, which will fail in a private subnet without internet access enabled (e.g. an isolated subnnet).
->
-> Ensure that the Canary is placed in a VPC either with internet connectivity or with VPC Endpoints for S3 and CloudWatch enabled and configured.
->
-> See [Synthetics VPC docs](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Canaries_VPC.html).
-
 ### Alarms
 
 You can configure a CloudWatch Alarm on a canary metric. Metrics are emitted by CloudWatch automatically and can be accessed by the following APIs:
 
 * `canary.metricSuccessPercent()` - percentage of successful canary runs over a given time
 * `canary.metricDuration()` - how much time each canary run takes, in seconds.
 * `canary.metricFailed()` - number of failed canary runs over a given time
@@ -257,7 +208,9 @@
 cloudwatch.Alarm(self, "CanaryAlarm",
     metric=canary.metric_success_percent(),
     evaluation_periods=2,
     threshold=90,
     comparison_operator=cloudwatch.ComparisonOperator.LESS_THAN_THRESHOLD
 )
 ```
+
+
```

### Comparing `aws-cdk.aws-synthetics-alpha-2.84.0a0/src/aws_cdk.aws_synthetics_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-synthetics-alpha-2.9.0a0/src/aws_cdk.aws_synthetics_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_synthetics_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_synthetics_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_synthetics_alpha.egg-info/requires.txt
 src/aws_cdk.aws_synthetics_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_synthetics_alpha/__init__.py
 src/aws_cdk/aws_synthetics_alpha/py.typed
 src/aws_cdk/aws_synthetics_alpha/_jsii/__init__.py
-src/aws_cdk/aws_synthetics_alpha/_jsii/aws-synthetics-alpha@2.84.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_synthetics_alpha/_jsii/aws-synthetics-alpha@2.9.0-alpha.0.jsii.tgz
```

