# Comparing `tmp/aws-cdk.aws-apprunner-alpha-2.83.1a0.tar.gz` & `tmp/aws-cdk.aws-apprunner-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src629398401/src/packages/@aws-cdk/aws-apprunner-alpha/dist/python/aws-cdk.aws-apprunner-alpha-2.83.1a0.tar", last modified: Fri Jun  9 09:55:03 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-apprunner/dist/python/aws-cdk.aws-apprunner-alpha-2.9.0a0.t", last modified: Wed Jan 26 11:22:04 2022, max compression
```

## Comparing `aws-cdk.aws-apprunner-alpha-2.83.1a0.tar` & `aws-cdk.aws-apprunner-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:03.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-09 09:54:54.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-09 09:54:54.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-09 09:54:54.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8250 2023-06-09 09:55:03.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7245 2023-06-09 09:54:54.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-09 09:54:54.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 09:55:03.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1884 2023-06-09 09:54:54.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:03.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:03.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:03.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/src/aws_cdk/aws_apprunner_alpha/
--rw-r--r--   0 root         (0) root         (0)   170531 2023-06-09 09:54:54.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/src/aws_cdk/aws_apprunner_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:03.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/src/aws_cdk/aws_apprunner_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 09:54:54.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/src/aws_cdk/aws_apprunner_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77529 2023-06-09 09:54:54.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/src/aws_cdk/aws_apprunner_alpha/_jsii/aws-apprunner-alpha@2.83.1-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:54:54.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/src/aws_cdk/aws_apprunner_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:03.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/src/aws_cdk.aws_apprunner_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8250 2023-06-09 09:55:03.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/src/aws_cdk.aws_apprunner_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-09 09:55:03.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/src/aws_cdk.aws_apprunner_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:55:03.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/src/aws_cdk.aws_apprunner_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-09 09:55:03.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/src/aws_cdk.aws_apprunner_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-09 09:55:03.000000 aws-cdk.aws-apprunner-alpha-2.83.1a0/src/aws_cdk.aws_apprunner_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:04.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:01.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6001 2022-01-26 11:22:04.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5029 2022-01-26 11:22:01.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:04.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1809 2022-01-26 11:22:01.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:04.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:04.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:04.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/src/aws_cdk/aws_apprunner_alpha/
+-rw-r--r--   0 root         (0) root         (0)    93730 2022-01-26 11:22:01.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/src/aws_cdk/aws_apprunner_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:04.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/src/aws_cdk/aws_apprunner_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      409 2022-01-26 11:22:01.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/src/aws_cdk/aws_apprunner_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47965 2022-01-26 11:22:01.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/src/aws_cdk/aws_apprunner_alpha/_jsii/aws-apprunner-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/src/aws_cdk/aws_apprunner_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:04.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/src/aws_cdk.aws_apprunner_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6001 2022-01-26 11:22:04.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/src/aws_cdk.aws_apprunner_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      550 2022-01-26 11:22:04.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/src/aws_cdk.aws_apprunner_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:04.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/src/aws_cdk.aws_apprunner_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:04.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/src/aws_cdk.aws_apprunner_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:04.000000 aws-cdk.aws-apprunner-alpha-2.9.0a0/src/aws_cdk.aws_apprunner_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-apprunner-alpha-2.83.1a0/LICENSE` & `aws-cdk.aws-apprunner-alpha-2.9.0a0/LICENSE`

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

### Comparing `aws-cdk.aws-apprunner-alpha-2.83.1a0/PKG-INFO` & `aws-cdk.aws-apprunner-alpha-2.9.0a0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-apprunner-alpha
-Version: 2.83.1a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::AppRunner
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
 
 # AWS::AppRunner Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -81,36 +81,33 @@
 import aws_cdk.aws_ecr as ecr
 
 
 apprunner.Service(self, "Service",
     source=apprunner.Source.from_ecr(
         image_configuration=apprunner.ImageConfiguration(port=80),
         repository=ecr.Repository.from_repository_name(self, "NginxRepository", "nginx"),
-        tag_or_digest="latest"
+        tag="latest"
     )
 )
 ```
 
-To create a `Service` from local docker image asset directory built and pushed to Amazon ECR:
-
-You can specify whether to enable continuous integration from the source repository with the `autoDeploymentsEnabled` flag.
+To create a `Service` from local docker image asset directory  built and pushed to Amazon ECR:
 
 ```python
 import aws_cdk.aws_ecr_assets as assets
 
 
 image_asset = assets.DockerImageAsset(self, "ImageAssets",
     directory=path.join(__dirname, "./docker.assets")
 )
 apprunner.Service(self, "Service",
     source=apprunner.Source.from_asset(
         image_configuration=apprunner.ImageConfiguration(port=8000),
         asset=image_asset
-    ),
-    auto_deployments_enabled=True
+    )
 )
 ```
 
 ## GitHub
 
 To create a `Service` from the GitHub repository, you need to specify an existing App Runner `Connection`.
 
@@ -155,70 +152,8 @@
 
 `accessRole` - The IAM role that grants the App Runner service access to a source repository. It's required for
 ECR image repositories (but not for ECR Public repositories). If not defined, a new access role will be generated
 when required.
 
 See [App Runner IAM Roles](https://docs.aws.amazon.com/apprunner/latest/dg/security_iam_service-with-iam.html#security_iam_service-with-iam-roles) for more details.
 
-## VPC Connector
-
-To associate an App Runner service with a custom VPC, define `vpcConnector` for the service.
-
-```python
-import aws_cdk.aws_ec2 as ec2
-
-
-vpc = ec2.Vpc(self, "Vpc",
-    ip_addresses=ec2.IpAddresses.cidr("10.0.0.0/16")
-)
-
-vpc_connector = apprunner.VpcConnector(self, "VpcConnector",
-    vpc=vpc,
-    vpc_subnets=vpc.select_subnets(subnet_type=ec2.SubnetType.PUBLIC),
-    vpc_connector_name="MyVpcConnector"
-)
-
-apprunner.Service(self, "Service",
-    source=apprunner.Source.from_ecr_public(
-        image_configuration=apprunner.ImageConfiguration(port=8000),
-        image_identifier="public.ecr.aws/aws-containers/hello-app-runner:latest"
-    ),
-    vpc_connector=vpc_connector
-)
-```
-
-## Secrets Manager
-
-To include environment variables integrated with AWS Secrets Manager, use the `environmentSecrets` attribute.
-You can use the `addSecret` method from the App Runner `Service` class to include secrets from outside the
-service definition.
-
-```python
-import aws_cdk.aws_secretsmanager as secretsmanager
-import aws_cdk.aws_ssm as ssm
-
-# stack: Stack
-
-
-secret = secretsmanager.Secret(stack, "Secret")
-parameter = ssm.StringParameter.from_secure_string_parameter_attributes(stack, "Parameter",
-    parameter_name="/name",
-    version=1
-)
-
-service = apprunner.Service(stack, "Service",
-    source=apprunner.Source.from_ecr_public(
-        image_configuration=apprunner.ImageConfiguration(
-            port=8000,
-            environment_secrets={
-                "SECRET": apprunner.Secret.from_secrets_manager(secret),
-                "PARAMETER": apprunner.Secret.from_ssm_parameter(parameter),
-                "SECRET_ID": apprunner.Secret.from_secrets_manager_version(secret, version_id="version-id"),
-                "SECRET_STAGE": apprunner.Secret.from_secrets_manager_version(secret, version_stage="version-stage")
-            }
-        ),
-        image_identifier="public.ecr.aws/aws-containers/hello-app-runner:latest"
-    )
-)
 
-service.add_secret("LATER_SECRET", apprunner.Secret.from_secrets_manager(secret, "field"))
-```
```

### Comparing `aws-cdk.aws-apprunner-alpha-2.83.1a0/README.md` & `aws-cdk.aws-apprunner-alpha-2.9.0a0/src/aws_cdk.aws_apprunner_alpha.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: aws-cdk.aws-apprunner-alpha
+Version: 2.9.0a0
+Summary: The CDK Construct Library for AWS::AppRunner
+Home-page: https://github.com/aws/aws-cdk
+Author: Amazon Web Services
+License: Apache-2.0
+Project-URL: Source, https://github.com/aws/aws-cdk.git
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Typing :: Typed
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved
+Classifier: Framework :: AWS CDK
+Classifier: Framework :: AWS CDK :: 1
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
+
 # AWS::AppRunner Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
 
 
 ![cdk-constructs: Experimental](https://img.shields.io/badge/cdk--constructs-experimental-important.svg?style=for-the-badge)
 
@@ -54,36 +81,33 @@
 import aws_cdk.aws_ecr as ecr
 
 
 apprunner.Service(self, "Service",
     source=apprunner.Source.from_ecr(
         image_configuration=apprunner.ImageConfiguration(port=80),
         repository=ecr.Repository.from_repository_name(self, "NginxRepository", "nginx"),
-        tag_or_digest="latest"
+        tag="latest"
     )
 )
 ```
 
-To create a `Service` from local docker image asset directory built and pushed to Amazon ECR:
-
-You can specify whether to enable continuous integration from the source repository with the `autoDeploymentsEnabled` flag.
+To create a `Service` from local docker image asset directory  built and pushed to Amazon ECR:
 
 ```python
 import aws_cdk.aws_ecr_assets as assets
 
 
 image_asset = assets.DockerImageAsset(self, "ImageAssets",
     directory=path.join(__dirname, "./docker.assets")
 )
 apprunner.Service(self, "Service",
     source=apprunner.Source.from_asset(
         image_configuration=apprunner.ImageConfiguration(port=8000),
         asset=image_asset
-    ),
-    auto_deployments_enabled=True
+    )
 )
 ```
 
 ## GitHub
 
 To create a `Service` from the GitHub repository, you need to specify an existing App Runner `Connection`.
 
@@ -128,70 +152,8 @@
 
 `accessRole` - The IAM role that grants the App Runner service access to a source repository. It's required for
 ECR image repositories (but not for ECR Public repositories). If not defined, a new access role will be generated
 when required.
 
 See [App Runner IAM Roles](https://docs.aws.amazon.com/apprunner/latest/dg/security_iam_service-with-iam.html#security_iam_service-with-iam-roles) for more details.
 
-## VPC Connector
-
-To associate an App Runner service with a custom VPC, define `vpcConnector` for the service.
-
-```python
-import aws_cdk.aws_ec2 as ec2
-
-
-vpc = ec2.Vpc(self, "Vpc",
-    ip_addresses=ec2.IpAddresses.cidr("10.0.0.0/16")
-)
 
-vpc_connector = apprunner.VpcConnector(self, "VpcConnector",
-    vpc=vpc,
-    vpc_subnets=vpc.select_subnets(subnet_type=ec2.SubnetType.PUBLIC),
-    vpc_connector_name="MyVpcConnector"
-)
-
-apprunner.Service(self, "Service",
-    source=apprunner.Source.from_ecr_public(
-        image_configuration=apprunner.ImageConfiguration(port=8000),
-        image_identifier="public.ecr.aws/aws-containers/hello-app-runner:latest"
-    ),
-    vpc_connector=vpc_connector
-)
-```
-
-## Secrets Manager
-
-To include environment variables integrated with AWS Secrets Manager, use the `environmentSecrets` attribute.
-You can use the `addSecret` method from the App Runner `Service` class to include secrets from outside the
-service definition.
-
-```python
-import aws_cdk.aws_secretsmanager as secretsmanager
-import aws_cdk.aws_ssm as ssm
-
-# stack: Stack
-
-
-secret = secretsmanager.Secret(stack, "Secret")
-parameter = ssm.StringParameter.from_secure_string_parameter_attributes(stack, "Parameter",
-    parameter_name="/name",
-    version=1
-)
-
-service = apprunner.Service(stack, "Service",
-    source=apprunner.Source.from_ecr_public(
-        image_configuration=apprunner.ImageConfiguration(
-            port=8000,
-            environment_secrets={
-                "SECRET": apprunner.Secret.from_secrets_manager(secret),
-                "PARAMETER": apprunner.Secret.from_ssm_parameter(parameter),
-                "SECRET_ID": apprunner.Secret.from_secrets_manager_version(secret, version_id="version-id"),
-                "SECRET_STAGE": apprunner.Secret.from_secrets_manager_version(secret, version_stage="version-stage")
-            }
-        ),
-        image_identifier="public.ecr.aws/aws-containers/hello-app-runner:latest"
-    )
-)
-
-service.add_secret("LATER_SECRET", apprunner.Secret.from_secrets_manager(secret, "field"))
-```
```

### Comparing `aws-cdk.aws-apprunner-alpha-2.83.1a0/setup.py` & `aws-cdk.aws-apprunner-alpha-2.9.0a0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-apprunner-alpha",
-    "version": "2.83.1.a0",
+    "version": "2.9.0.a0",
     "description": "The CDK Construct Library for AWS::AppRunner",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,43 +22,41 @@
     },
     "packages": [
         "aws_cdk.aws_apprunner_alpha",
         "aws_cdk.aws_apprunner_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_apprunner_alpha._jsii": [
-            "aws-apprunner-alpha@2.83.1-alpha.0.jsii.tgz"
+            "aws-apprunner-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_apprunner_alpha": [
             "py.typed"
         ]
     },
-    "python_requires": "~=3.7",
+    "python_requires": ">=3.6",
     "install_requires": [
-        "aws-cdk-lib==2.83.1",
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

### Comparing `aws-cdk.aws-apprunner-alpha-2.83.1a0/src/aws_cdk.aws_apprunner_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-apprunner-alpha-2.9.0a0/src/aws_cdk.aws_apprunner_alpha.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_apprunner_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_apprunner_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_apprunner_alpha.egg-info/requires.txt
 src/aws_cdk.aws_apprunner_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_apprunner_alpha/__init__.py
 src/aws_cdk/aws_apprunner_alpha/py.typed
 src/aws_cdk/aws_apprunner_alpha/_jsii/__init__.py
-src/aws_cdk/aws_apprunner_alpha/_jsii/aws-apprunner-alpha@2.83.1-alpha.0.jsii.tgz
+src/aws_cdk/aws_apprunner_alpha/_jsii/aws-apprunner-alpha@2.9.0-alpha.0.jsii.tgz
```

