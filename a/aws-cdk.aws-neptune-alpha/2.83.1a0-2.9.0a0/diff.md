# Comparing `tmp/aws-cdk.aws-neptune-alpha-2.83.1a0.tar.gz` & `tmp/aws-cdk.aws-neptune-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src629398401/src/packages/@aws-cdk/aws-neptune-alpha/dist/python/aws-cdk.aws-neptune-alpha-2.83.1a0.tar", last modified: Fri Jun  9 09:55:06 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-neptune/dist/python/aws-cdk.aws-neptune-alpha-2.9.0a0.tar", last modified: Wed Jan 26 11:22:06 2022, max compression
```

## Comparing `aws-cdk.aws-neptune-alpha-2.83.1a0.tar` & `aws-cdk.aws-neptune-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:06.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-09 09:54:54.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-09 09:54:54.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-09 09:54:54.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8200 2023-06-09 09:55:06.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7199 2023-06-09 09:54:54.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-09 09:54:54.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 09:55:06.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1870 2023-06-09 09:54:54.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:06.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:06.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:06.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/src/aws_cdk/aws_neptune_alpha/
--rw-r--r--   0 root         (0) root         (0)   183368 2023-06-09 09:54:54.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/src/aws_cdk/aws_neptune_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:06.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/src/aws_cdk/aws_neptune_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      441 2023-06-09 09:54:54.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/src/aws_cdk/aws_neptune_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69268 2023-06-09 09:54:54.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/src/aws_cdk/aws_neptune_alpha/_jsii/aws-neptune-alpha@2.83.1-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:54:54.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/src/aws_cdk/aws_neptune_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:06.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/src/aws_cdk.aws_neptune_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8200 2023-06-09 09:55:05.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/src/aws_cdk.aws_neptune_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-09 09:55:06.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/src/aws_cdk.aws_neptune_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:55:05.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/src/aws_cdk.aws_neptune_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-09 09:55:05.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/src/aws_cdk.aws_neptune_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-09 09:55:05.000000 aws-cdk.aws-neptune-alpha-2.83.1a0/src/aws_cdk.aws_neptune_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5750 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4782 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1795 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk/aws_neptune_alpha/
+-rw-r--r--   0 root         (0) root         (0)   111643 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk/aws_neptune_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk/aws_neptune_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      405 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk/aws_neptune_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55214 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk/aws_neptune_alpha/_jsii/aws-neptune-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk/aws_neptune_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5750 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      530 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-neptune-alpha-2.83.1a0/LICENSE` & `aws-cdk.aws-neptune-alpha-2.9.0a0/LICENSE`

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

### Comparing `aws-cdk.aws-neptune-alpha-2.83.1a0/PKG-INFO` & `aws-cdk.aws-neptune-alpha-2.9.0a0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-neptune-alpha
-Version: 2.83.1a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::Neptune
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
 
 # Amazon Neptune Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -89,17 +89,15 @@
 ```python
 cluster = neptune.DatabaseCluster(self, "Cluster",
     vpc=vpc,
     instance_type=neptune.InstanceType.R5_LARGE,
     iam_authentication=True
 )
 role = iam.Role(self, "DBRole", assumed_by=iam.AccountPrincipal(self.account))
-# Use one of the following statements to grant the role the necessary permissions
-cluster.grant_connect(role) # Grant the role neptune-db:* access to the DB
-cluster.grant(role, "neptune-db:ReadDataViaQuery", "neptune-db:WriteDataViaQuery")
+cluster.grant_connect(role)
 ```
 
 ## Customizing parameters
 
 Neptune allows configuring database behavior by supplying custom parameter groups.  For more details, refer to the
 following link: [https://docs.aws.amazon.com/neptune/latest/userguide/parameters.html](https://docs.aws.amazon.com/neptune/latest/userguide/parameters.html)
 
@@ -122,30 +120,28 @@
     vpc=vpc,
     instance_type=neptune.InstanceType.R5_LARGE,
     cluster_parameter_group=cluster_params,
     parameter_group=db_params
 )
 ```
 
-Note: if you want to use Neptune engine `1.2.0.0` or later, you need to specify the corresponding `engineVersion` prop to `neptune.DatabaseCluster` and `family` prop of `ParameterGroupFamily.NEPTUNE_1_2` to `neptune.ClusterParameterGroup` and `neptune.ParameterGroup`.
-
 ## Adding replicas
 
 `DatabaseCluster` allows launching replicas along with the writer instance. This can be specified using the `instanceCount`
 attribute.
 
 ```python
 cluster = neptune.DatabaseCluster(self, "Database",
     vpc=vpc,
     instance_type=neptune.InstanceType.R5_LARGE,
     instances=2
 )
 ```
 
-Additionally, it is also possible to add replicas using `DatabaseInstance` for an existing cluster.
+Additionally it is also possible to add replicas using `DatabaseInstance` for an existing cluster.
 
 ```python
 replica1 = neptune.DatabaseInstance(self, "Instance",
     cluster=cluster,
     instance_type=neptune.InstanceType.R5_LARGE
 )
 ```
@@ -153,60 +149,16 @@
 ## Automatic minor version upgrades
 
 By setting `autoMinorVersionUpgrade` to true, Neptune will automatically update
 the engine of the entire cluster to the latest minor version after a stabilization
 window of 2 to 3 weeks.
 
 ```python
-neptune.DatabaseCluster(self, "Cluster",
+# Example automatically generated from non-compiling source. May contain errors.
+neptune.DatabaseCluster(stack, "Cluster",
     vpc=vpc,
-    instance_type=neptune.InstanceType.R5_LARGE,
+    instance_type=InstanceType.R5_LARGE,
     auto_minor_version_upgrade=True
 )
 ```
 
-## Logging
-
-Neptune supports various methods for monitoring performance and usage. One of those methods is logging
-
-1. Neptune provides logs e.g. audit logs which can be viewed or downloaded via the AWS Console. Audit logs can be enabled using the `neptune_enable_audit_log` parameter in `ClusterParameterGroup` or `ParameterGroup`
-2. Neptune provides the ability to export those logs to CloudWatch Logs
-
-```python
-# Cluster parameter group with the neptune_enable_audit_log param set to 1
-cluster_parameter_group = neptune.ClusterParameterGroup(self, "ClusterParams",
-    description="Cluster parameter group",
-    parameters={
-        "neptune_enable_audit_log": "1"
-    }
-)
-
-cluster = neptune.DatabaseCluster(self, "Database",
-    vpc=vpc,
-    instance_type=neptune.InstanceType.R5_LARGE,
-    # Audit logs are enabled via the clusterParameterGroup
-    cluster_parameter_group=cluster_parameter_group,
-    # Optionally configuring audit logs to be exported to CloudWatch Logs
-    cloudwatch_logs_exports=[neptune.LogType.AUDIT],
-    # Optionally set a retention period on exported CloudWatch Logs
-    cloudwatch_logs_retention=logs.RetentionDays.ONE_MONTH
-)
-```
-
-For more information on monitoring, refer to https://docs.aws.amazon.com/neptune/latest/userguide/monitoring.html.
-For more information on audit logs, refer to https://docs.aws.amazon.com/neptune/latest/userguide/auditing.html.
-For more information on exporting logs to CloudWatch Logs, refer to https://docs.aws.amazon.com/neptune/latest/userguide/cloudwatch-logs.html.
-
-## Metrics
-
-Both `DatabaseCluster` and `DatabaseInstance` provide a `metric()` method to help with cluster-level and instance-level monitoring.
-
-```python
-# cluster: neptune.DatabaseCluster
-# instance: neptune.DatabaseInstance
-
-
-cluster.metric("SparqlRequestsPerSec") # cluster-level SparqlErrors metric
-instance.metric("SparqlRequestsPerSec")
-```
 
-For more details on the available metrics, refer to https://docs.aws.amazon.com/neptune/latest/userguide/cw-metrics.html
```

### Comparing `aws-cdk.aws-neptune-alpha-2.83.1a0/README.md` & `aws-cdk.aws-neptune-alpha-2.9.0a0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -62,17 +62,15 @@
 ```python
 cluster = neptune.DatabaseCluster(self, "Cluster",
     vpc=vpc,
     instance_type=neptune.InstanceType.R5_LARGE,
     iam_authentication=True
 )
 role = iam.Role(self, "DBRole", assumed_by=iam.AccountPrincipal(self.account))
-# Use one of the following statements to grant the role the necessary permissions
-cluster.grant_connect(role) # Grant the role neptune-db:* access to the DB
-cluster.grant(role, "neptune-db:ReadDataViaQuery", "neptune-db:WriteDataViaQuery")
+cluster.grant_connect(role)
 ```
 
 ## Customizing parameters
 
 Neptune allows configuring database behavior by supplying custom parameter groups.  For more details, refer to the
 following link: [https://docs.aws.amazon.com/neptune/latest/userguide/parameters.html](https://docs.aws.amazon.com/neptune/latest/userguide/parameters.html)
 
@@ -95,30 +93,28 @@
     vpc=vpc,
     instance_type=neptune.InstanceType.R5_LARGE,
     cluster_parameter_group=cluster_params,
     parameter_group=db_params
 )
 ```
 
-Note: if you want to use Neptune engine `1.2.0.0` or later, you need to specify the corresponding `engineVersion` prop to `neptune.DatabaseCluster` and `family` prop of `ParameterGroupFamily.NEPTUNE_1_2` to `neptune.ClusterParameterGroup` and `neptune.ParameterGroup`.
-
 ## Adding replicas
 
 `DatabaseCluster` allows launching replicas along with the writer instance. This can be specified using the `instanceCount`
 attribute.
 
 ```python
 cluster = neptune.DatabaseCluster(self, "Database",
     vpc=vpc,
     instance_type=neptune.InstanceType.R5_LARGE,
     instances=2
 )
 ```
 
-Additionally, it is also possible to add replicas using `DatabaseInstance` for an existing cluster.
+Additionally it is also possible to add replicas using `DatabaseInstance` for an existing cluster.
 
 ```python
 replica1 = neptune.DatabaseInstance(self, "Instance",
     cluster=cluster,
     instance_type=neptune.InstanceType.R5_LARGE
 )
 ```
@@ -126,60 +122,14 @@
 ## Automatic minor version upgrades
 
 By setting `autoMinorVersionUpgrade` to true, Neptune will automatically update
 the engine of the entire cluster to the latest minor version after a stabilization
 window of 2 to 3 weeks.
 
 ```python
-neptune.DatabaseCluster(self, "Cluster",
+# Example automatically generated from non-compiling source. May contain errors.
+neptune.DatabaseCluster(stack, "Cluster",
     vpc=vpc,
-    instance_type=neptune.InstanceType.R5_LARGE,
+    instance_type=InstanceType.R5_LARGE,
     auto_minor_version_upgrade=True
 )
 ```
-
-## Logging
-
-Neptune supports various methods for monitoring performance and usage. One of those methods is logging
-
-1. Neptune provides logs e.g. audit logs which can be viewed or downloaded via the AWS Console. Audit logs can be enabled using the `neptune_enable_audit_log` parameter in `ClusterParameterGroup` or `ParameterGroup`
-2. Neptune provides the ability to export those logs to CloudWatch Logs
-
-```python
-# Cluster parameter group with the neptune_enable_audit_log param set to 1
-cluster_parameter_group = neptune.ClusterParameterGroup(self, "ClusterParams",
-    description="Cluster parameter group",
-    parameters={
-        "neptune_enable_audit_log": "1"
-    }
-)
-
-cluster = neptune.DatabaseCluster(self, "Database",
-    vpc=vpc,
-    instance_type=neptune.InstanceType.R5_LARGE,
-    # Audit logs are enabled via the clusterParameterGroup
-    cluster_parameter_group=cluster_parameter_group,
-    # Optionally configuring audit logs to be exported to CloudWatch Logs
-    cloudwatch_logs_exports=[neptune.LogType.AUDIT],
-    # Optionally set a retention period on exported CloudWatch Logs
-    cloudwatch_logs_retention=logs.RetentionDays.ONE_MONTH
-)
-```
-
-For more information on monitoring, refer to https://docs.aws.amazon.com/neptune/latest/userguide/monitoring.html.
-For more information on audit logs, refer to https://docs.aws.amazon.com/neptune/latest/userguide/auditing.html.
-For more information on exporting logs to CloudWatch Logs, refer to https://docs.aws.amazon.com/neptune/latest/userguide/cloudwatch-logs.html.
-
-## Metrics
-
-Both `DatabaseCluster` and `DatabaseInstance` provide a `metric()` method to help with cluster-level and instance-level monitoring.
-
-```python
-# cluster: neptune.DatabaseCluster
-# instance: neptune.DatabaseInstance
-
-
-cluster.metric("SparqlRequestsPerSec") # cluster-level SparqlErrors metric
-instance.metric("SparqlRequestsPerSec")
-```
-
-For more details on the available metrics, refer to https://docs.aws.amazon.com/neptune/latest/userguide/cw-metrics.html
```

### Comparing `aws-cdk.aws-neptune-alpha-2.83.1a0/setup.py` & `aws-cdk.aws-neptune-alpha-2.9.0a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-neptune-alpha",
-    "version": "2.83.1.a0",
+    "version": "2.9.0.a0",
     "description": "The CDK Construct Library for AWS::Neptune",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,43 +22,41 @@
     },
     "packages": [
         "aws_cdk.aws_neptune_alpha",
         "aws_cdk.aws_neptune_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_neptune_alpha._jsii": [
-            "aws-neptune-alpha@2.83.1-alpha.0.jsii.tgz"
+            "aws-neptune-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_neptune_alpha": [
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

### Comparing `aws-cdk.aws-neptune-alpha-2.83.1a0/src/aws_cdk.aws_neptune_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-neptune-alpha
-Version: 2.83.1a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::Neptune
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
 
 # Amazon Neptune Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -89,17 +89,15 @@
 ```python
 cluster = neptune.DatabaseCluster(self, "Cluster",
     vpc=vpc,
     instance_type=neptune.InstanceType.R5_LARGE,
     iam_authentication=True
 )
 role = iam.Role(self, "DBRole", assumed_by=iam.AccountPrincipal(self.account))
-# Use one of the following statements to grant the role the necessary permissions
-cluster.grant_connect(role) # Grant the role neptune-db:* access to the DB
-cluster.grant(role, "neptune-db:ReadDataViaQuery", "neptune-db:WriteDataViaQuery")
+cluster.grant_connect(role)
 ```
 
 ## Customizing parameters
 
 Neptune allows configuring database behavior by supplying custom parameter groups.  For more details, refer to the
 following link: [https://docs.aws.amazon.com/neptune/latest/userguide/parameters.html](https://docs.aws.amazon.com/neptune/latest/userguide/parameters.html)
 
@@ -122,30 +120,28 @@
     vpc=vpc,
     instance_type=neptune.InstanceType.R5_LARGE,
     cluster_parameter_group=cluster_params,
     parameter_group=db_params
 )
 ```
 
-Note: if you want to use Neptune engine `1.2.0.0` or later, you need to specify the corresponding `engineVersion` prop to `neptune.DatabaseCluster` and `family` prop of `ParameterGroupFamily.NEPTUNE_1_2` to `neptune.ClusterParameterGroup` and `neptune.ParameterGroup`.
-
 ## Adding replicas
 
 `DatabaseCluster` allows launching replicas along with the writer instance. This can be specified using the `instanceCount`
 attribute.
 
 ```python
 cluster = neptune.DatabaseCluster(self, "Database",
     vpc=vpc,
     instance_type=neptune.InstanceType.R5_LARGE,
     instances=2
 )
 ```
 
-Additionally, it is also possible to add replicas using `DatabaseInstance` for an existing cluster.
+Additionally it is also possible to add replicas using `DatabaseInstance` for an existing cluster.
 
 ```python
 replica1 = neptune.DatabaseInstance(self, "Instance",
     cluster=cluster,
     instance_type=neptune.InstanceType.R5_LARGE
 )
 ```
@@ -153,60 +149,16 @@
 ## Automatic minor version upgrades
 
 By setting `autoMinorVersionUpgrade` to true, Neptune will automatically update
 the engine of the entire cluster to the latest minor version after a stabilization
 window of 2 to 3 weeks.
 
 ```python
-neptune.DatabaseCluster(self, "Cluster",
+# Example automatically generated from non-compiling source. May contain errors.
+neptune.DatabaseCluster(stack, "Cluster",
     vpc=vpc,
-    instance_type=neptune.InstanceType.R5_LARGE,
+    instance_type=InstanceType.R5_LARGE,
     auto_minor_version_upgrade=True
 )
 ```
 
-## Logging
-
-Neptune supports various methods for monitoring performance and usage. One of those methods is logging
-
-1. Neptune provides logs e.g. audit logs which can be viewed or downloaded via the AWS Console. Audit logs can be enabled using the `neptune_enable_audit_log` parameter in `ClusterParameterGroup` or `ParameterGroup`
-2. Neptune provides the ability to export those logs to CloudWatch Logs
-
-```python
-# Cluster parameter group with the neptune_enable_audit_log param set to 1
-cluster_parameter_group = neptune.ClusterParameterGroup(self, "ClusterParams",
-    description="Cluster parameter group",
-    parameters={
-        "neptune_enable_audit_log": "1"
-    }
-)
-
-cluster = neptune.DatabaseCluster(self, "Database",
-    vpc=vpc,
-    instance_type=neptune.InstanceType.R5_LARGE,
-    # Audit logs are enabled via the clusterParameterGroup
-    cluster_parameter_group=cluster_parameter_group,
-    # Optionally configuring audit logs to be exported to CloudWatch Logs
-    cloudwatch_logs_exports=[neptune.LogType.AUDIT],
-    # Optionally set a retention period on exported CloudWatch Logs
-    cloudwatch_logs_retention=logs.RetentionDays.ONE_MONTH
-)
-```
-
-For more information on monitoring, refer to https://docs.aws.amazon.com/neptune/latest/userguide/monitoring.html.
-For more information on audit logs, refer to https://docs.aws.amazon.com/neptune/latest/userguide/auditing.html.
-For more information on exporting logs to CloudWatch Logs, refer to https://docs.aws.amazon.com/neptune/latest/userguide/cloudwatch-logs.html.
-
-## Metrics
-
-Both `DatabaseCluster` and `DatabaseInstance` provide a `metric()` method to help with cluster-level and instance-level monitoring.
-
-```python
-# cluster: neptune.DatabaseCluster
-# instance: neptune.DatabaseInstance
-
-
-cluster.metric("SparqlRequestsPerSec") # cluster-level SparqlErrors metric
-instance.metric("SparqlRequestsPerSec")
-```
 
-For more details on the available metrics, refer to https://docs.aws.amazon.com/neptune/latest/userguide/cw-metrics.html
```

### Comparing `aws-cdk.aws-neptune-alpha-2.83.1a0/src/aws_cdk.aws_neptune_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_neptune_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_neptune_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_neptune_alpha.egg-info/requires.txt
 src/aws_cdk.aws_neptune_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_neptune_alpha/__init__.py
 src/aws_cdk/aws_neptune_alpha/py.typed
 src/aws_cdk/aws_neptune_alpha/_jsii/__init__.py
-src/aws_cdk/aws_neptune_alpha/_jsii/aws-neptune-alpha@2.83.1-alpha.0.jsii.tgz
+src/aws_cdk/aws_neptune_alpha/_jsii/aws-neptune-alpha@2.9.0-alpha.0.jsii.tgz
```

