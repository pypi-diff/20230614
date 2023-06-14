# Comparing `tmp/aws-cdk.aws-msk-alpha-2.83.1a0.tar.gz` & `tmp/aws-cdk.aws-msk-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src629398401/src/packages/@aws-cdk/aws-msk-alpha/dist/python/aws-cdk.aws-msk-alpha-2.83.1a0.tar", last modified: Fri Jun  9 09:55:05 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-msk/dist/python/aws-cdk.aws-msk-alpha-2.9.0a0.tar", last modified: Wed Jan 26 11:22:07 2022, max compression
```

## Comparing `aws-cdk.aws-msk-alpha-2.83.1a0.tar` & `aws-cdk.aws-msk-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:05.000000 aws-cdk.aws-msk-alpha-2.83.1a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-09 09:54:54.000000 aws-cdk.aws-msk-alpha-2.83.1a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-09 09:54:54.000000 aws-cdk.aws-msk-alpha-2.83.1a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-09 09:54:54.000000 aws-cdk.aws-msk-alpha-2.83.1a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     7737 2023-06-09 09:55:05.000000 aws-cdk.aws-msk-alpha-2.83.1a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6744 2023-06-09 09:54:54.000000 aws-cdk.aws-msk-alpha-2.83.1a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-09 09:54:54.000000 aws-cdk.aws-msk-alpha-2.83.1a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 09:55:05.000000 aws-cdk.aws-msk-alpha-2.83.1a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1842 2023-06-09 09:54:54.000000 aws-cdk.aws-msk-alpha-2.83.1a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:05.000000 aws-cdk.aws-msk-alpha-2.83.1a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:05.000000 aws-cdk.aws-msk-alpha-2.83.1a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:05.000000 aws-cdk.aws-msk-alpha-2.83.1a0/src/aws_cdk/aws_msk_alpha/
--rw-r--r--   0 root         (0) root         (0)    91185 2023-06-09 09:54:54.000000 aws-cdk.aws-msk-alpha-2.83.1a0/src/aws_cdk/aws_msk_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:05.000000 aws-cdk.aws-msk-alpha-2.83.1a0/src/aws_cdk/aws_msk_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      433 2023-06-09 09:54:54.000000 aws-cdk.aws-msk-alpha-2.83.1a0/src/aws_cdk/aws_msk_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    57061 2023-06-09 09:54:54.000000 aws-cdk.aws-msk-alpha-2.83.1a0/src/aws_cdk/aws_msk_alpha/_jsii/aws-msk-alpha@2.83.1-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:54:54.000000 aws-cdk.aws-msk-alpha-2.83.1a0/src/aws_cdk/aws_msk_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:05.000000 aws-cdk.aws-msk-alpha-2.83.1a0/src/aws_cdk.aws_msk_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7737 2023-06-09 09:55:05.000000 aws-cdk.aws-msk-alpha-2.83.1a0/src/aws_cdk.aws_msk_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      491 2023-06-09 09:55:05.000000 aws-cdk.aws-msk-alpha-2.83.1a0/src/aws_cdk.aws_msk_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:55:05.000000 aws-cdk.aws-msk-alpha-2.83.1a0/src/aws_cdk.aws_msk_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-09 09:55:05.000000 aws-cdk.aws-msk-alpha-2.83.1a0/src/aws_cdk.aws_msk_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-09 09:55:05.000000 aws-cdk.aws-msk-alpha-2.83.1a0/src/aws_cdk.aws_msk_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-msk-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-msk-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-msk-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:01.000000 aws-cdk.aws-msk-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5547 2022-01-26 11:22:07.000000 aws-cdk.aws-msk-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4587 2022-01-26 11:22:01.000000 aws-cdk.aws-msk-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-msk-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:07.000000 aws-cdk.aws-msk-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1767 2022-01-26 11:22:01.000000 aws-cdk.aws-msk-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-msk-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-msk-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-msk-alpha-2.9.0a0/src/aws_cdk/aws_msk_alpha/
+-rw-r--r--   0 root         (0) root         (0)    65890 2022-01-26 11:22:01.000000 aws-cdk.aws-msk-alpha-2.9.0a0/src/aws_cdk/aws_msk_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-msk-alpha-2.9.0a0/src/aws_cdk/aws_msk_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      397 2022-01-26 11:22:01.000000 aws-cdk.aws-msk-alpha-2.9.0a0/src/aws_cdk/aws_msk_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47994 2022-01-26 11:22:01.000000 aws-cdk.aws-msk-alpha-2.9.0a0/src/aws_cdk/aws_msk_alpha/_jsii/aws-msk-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-msk-alpha-2.9.0a0/src/aws_cdk/aws_msk_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-msk-alpha-2.9.0a0/src/aws_cdk.aws_msk_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5547 2022-01-26 11:22:07.000000 aws-cdk.aws-msk-alpha-2.9.0a0/src/aws_cdk.aws_msk_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      490 2022-01-26 11:22:07.000000 aws-cdk.aws-msk-alpha-2.9.0a0/src/aws_cdk.aws_msk_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:07.000000 aws-cdk.aws-msk-alpha-2.9.0a0/src/aws_cdk.aws_msk_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:07.000000 aws-cdk.aws-msk-alpha-2.9.0a0/src/aws_cdk.aws_msk_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:07.000000 aws-cdk.aws-msk-alpha-2.9.0a0/src/aws_cdk.aws_msk_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-msk-alpha-2.83.1a0/LICENSE` & `aws-cdk.aws-msk-alpha-2.9.0a0/LICENSE`

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

### Comparing `aws-cdk.aws-msk-alpha-2.83.1a0/PKG-INFO` & `aws-cdk.aws-msk-alpha-2.9.0a0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-msk-alpha
-Version: 2.83.1a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::MSK
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
 
 # Amazon Managed Streaming for Apache Kafka Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -82,15 +82,14 @@
 
 ```python
 # cluster: msk.Cluster
 
 CfnOutput(self, "BootstrapBrokers", value=cluster.bootstrap_brokers)
 CfnOutput(self, "BootstrapBrokersTls", value=cluster.bootstrap_brokers_tls)
 CfnOutput(self, "BootstrapBrokersSaslScram", value=cluster.bootstrap_brokers_sasl_scram)
-CfnOutput(self, "BootstrapBrokerStringSaslIam", value=cluster.bootstrap_brokers_sasl_iam)
 CfnOutput(self, "ZookeeperConnection", value=cluster.zookeeper_connection_string)
 CfnOutput(self, "ZookeeperConnectionTls", value=cluster.zookeeper_connection_string_tls)
 ```
 
 ## Importing an existing Cluster
 
 To import an existing MSK cluster into your CDK app use the `.fromClusterArn()` method.
@@ -99,14 +98,16 @@
 cluster = msk.Cluster.from_cluster_arn(self, "Cluster", "arn:aws:kafka:us-west-2:1234567890:cluster/a-cluster/11111111-1111-1111-1111-111111111111-1")
 ```
 
 ## Client Authentication
 
 [MSK supports](https://docs.aws.amazon.com/msk/latest/developerguide/kafka_apis_iam.html) the following authentication mechanisms.
 
+> Only one authentication method can be enabled.
+
 ### TLS
 
 To enable client authentication with TLS set the `certificateAuthorityArns` property to reference your ACM Private CA. [More info on Private CAs.](https://docs.aws.amazon.com/msk/latest/developerguide/msk-authentication.html)
 
 ```python
 import aws_cdk.aws_acmpca as acmpca
 
@@ -163,69 +164,8 @@
     ),
     client_authentication=msk.ClientAuthentication.sasl(
         iam=True
     )
 )
 ```
 
-### SASL/IAM + TLS
-
-Enable client authentication with [IAM](https://docs.aws.amazon.com/msk/latest/developerguide/iam-access-control.html)
-as well as enable client authentication with TLS by setting the `certificateAuthorityArns` property to reference your ACM Private CA. [More info on Private CAs.](https://docs.aws.amazon.com/msk/latest/developerguide/msk-authentication.html)
-
-```python
-import aws_cdk.aws_acmpca as acmpca
-
-# vpc: ec2.Vpc
-
-cluster = msk.Cluster(self, "Cluster",
-    cluster_name="myCluster",
-    kafka_version=msk.KafkaVersion.V2_8_1,
-    vpc=vpc,
-    encryption_in_transit=msk.EncryptionInTransitConfig(
-        client_broker=msk.ClientBrokerEncryption.TLS
-    ),
-    client_authentication=msk.ClientAuthentication.sasl_tls(
-        iam=True,
-        certificate_authorities=[
-            acmpca.CertificateAuthority.from_certificate_authority_arn(self, "CertificateAuthority", "arn:aws:acm-pca:us-west-2:1234567890:certificate-authority/11111111-1111-1111-1111-111111111111")
-        ]
-    )
-)
-```
-
-## Logging
-
-You can deliver Apache Kafka broker logs to one or more of the following destination types:
-Amazon CloudWatch Logs, Amazon S3, Amazon Kinesis Data Firehose.
-
-To configure logs to be sent to an S3 bucket, provide a bucket in the `logging` config.
-
-```python
-# vpc: ec2.Vpc
-# bucket: s3.IBucket
-
-cluster = msk.Cluster(self, "cluster",
-    cluster_name="myCluster",
-    kafka_version=msk.KafkaVersion.V2_8_1,
-    vpc=vpc,
-    logging=msk.BrokerLogging(
-        s3=msk.S3LoggingConfiguration(
-            bucket=bucket
-        )
-    )
-)
-```
 
-When the S3 destination is configured, AWS will automatically create an S3 bucket policy
-that allows the service to write logs to the bucket. This makes it impossible to later update
-that bucket policy. To have CDK create the bucket policy so that future updates can be made,
-the `@aws-cdk/aws-s3:createDefaultLoggingPolicy` [feature flag](https://docs.aws.amazon.com/cdk/v2/guide/featureflags.html) can be used. This can be set
-in the `cdk.json` file.
-
-```json
-{
-  "context": {
-    "@aws-cdk/aws-s3:createDefaultLoggingPolicy": true
-  }
-}
-```
```

### Comparing `aws-cdk.aws-msk-alpha-2.83.1a0/README.md` & `aws-cdk.aws-msk-alpha-2.9.0a0/src/aws_cdk.aws_msk_alpha.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: aws-cdk.aws-msk-alpha
+Version: 2.9.0a0
+Summary: The CDK Construct Library for AWS::MSK
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
 # Amazon Managed Streaming for Apache Kafka Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
 
 
 ![cdk-constructs: Experimental](https://img.shields.io/badge/cdk--constructs-experimental-important.svg?style=for-the-badge)
 
@@ -55,15 +82,14 @@
 
 ```python
 # cluster: msk.Cluster
 
 CfnOutput(self, "BootstrapBrokers", value=cluster.bootstrap_brokers)
 CfnOutput(self, "BootstrapBrokersTls", value=cluster.bootstrap_brokers_tls)
 CfnOutput(self, "BootstrapBrokersSaslScram", value=cluster.bootstrap_brokers_sasl_scram)
-CfnOutput(self, "BootstrapBrokerStringSaslIam", value=cluster.bootstrap_brokers_sasl_iam)
 CfnOutput(self, "ZookeeperConnection", value=cluster.zookeeper_connection_string)
 CfnOutput(self, "ZookeeperConnectionTls", value=cluster.zookeeper_connection_string_tls)
 ```
 
 ## Importing an existing Cluster
 
 To import an existing MSK cluster into your CDK app use the `.fromClusterArn()` method.
@@ -72,14 +98,16 @@
 cluster = msk.Cluster.from_cluster_arn(self, "Cluster", "arn:aws:kafka:us-west-2:1234567890:cluster/a-cluster/11111111-1111-1111-1111-111111111111-1")
 ```
 
 ## Client Authentication
 
 [MSK supports](https://docs.aws.amazon.com/msk/latest/developerguide/kafka_apis_iam.html) the following authentication mechanisms.
 
+> Only one authentication method can be enabled.
+
 ### TLS
 
 To enable client authentication with TLS set the `certificateAuthorityArns` property to reference your ACM Private CA. [More info on Private CAs.](https://docs.aws.amazon.com/msk/latest/developerguide/msk-authentication.html)
 
 ```python
 import aws_cdk.aws_acmpca as acmpca
 
@@ -136,69 +164,8 @@
     ),
     client_authentication=msk.ClientAuthentication.sasl(
         iam=True
     )
 )
 ```
 
-### SASL/IAM + TLS
-
-Enable client authentication with [IAM](https://docs.aws.amazon.com/msk/latest/developerguide/iam-access-control.html)
-as well as enable client authentication with TLS by setting the `certificateAuthorityArns` property to reference your ACM Private CA. [More info on Private CAs.](https://docs.aws.amazon.com/msk/latest/developerguide/msk-authentication.html)
-
-```python
-import aws_cdk.aws_acmpca as acmpca
-
-# vpc: ec2.Vpc
 
-cluster = msk.Cluster(self, "Cluster",
-    cluster_name="myCluster",
-    kafka_version=msk.KafkaVersion.V2_8_1,
-    vpc=vpc,
-    encryption_in_transit=msk.EncryptionInTransitConfig(
-        client_broker=msk.ClientBrokerEncryption.TLS
-    ),
-    client_authentication=msk.ClientAuthentication.sasl_tls(
-        iam=True,
-        certificate_authorities=[
-            acmpca.CertificateAuthority.from_certificate_authority_arn(self, "CertificateAuthority", "arn:aws:acm-pca:us-west-2:1234567890:certificate-authority/11111111-1111-1111-1111-111111111111")
-        ]
-    )
-)
-```
-
-## Logging
-
-You can deliver Apache Kafka broker logs to one or more of the following destination types:
-Amazon CloudWatch Logs, Amazon S3, Amazon Kinesis Data Firehose.
-
-To configure logs to be sent to an S3 bucket, provide a bucket in the `logging` config.
-
-```python
-# vpc: ec2.Vpc
-# bucket: s3.IBucket
-
-cluster = msk.Cluster(self, "cluster",
-    cluster_name="myCluster",
-    kafka_version=msk.KafkaVersion.V2_8_1,
-    vpc=vpc,
-    logging=msk.BrokerLogging(
-        s3=msk.S3LoggingConfiguration(
-            bucket=bucket
-        )
-    )
-)
-```
-
-When the S3 destination is configured, AWS will automatically create an S3 bucket policy
-that allows the service to write logs to the bucket. This makes it impossible to later update
-that bucket policy. To have CDK create the bucket policy so that future updates can be made,
-the `@aws-cdk/aws-s3:createDefaultLoggingPolicy` [feature flag](https://docs.aws.amazon.com/cdk/v2/guide/featureflags.html) can be used. This can be set
-in the `cdk.json` file.
-
-```json
-{
-  "context": {
-    "@aws-cdk/aws-s3:createDefaultLoggingPolicy": true
-  }
-}
-```
```

### Comparing `aws-cdk.aws-msk-alpha-2.83.1a0/setup.py` & `aws-cdk.aws-msk-alpha-2.9.0a0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-msk-alpha",
-    "version": "2.83.1.a0",
+    "version": "2.9.0.a0",
     "description": "The CDK Construct Library for AWS::MSK",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,43 +22,41 @@
     },
     "packages": [
         "aws_cdk.aws_msk_alpha",
         "aws_cdk.aws_msk_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_msk_alpha._jsii": [
-            "aws-msk-alpha@2.83.1-alpha.0.jsii.tgz"
+            "aws-msk-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_msk_alpha": [
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

### Comparing `aws-cdk.aws-msk-alpha-2.83.1a0/src/aws_cdk/aws_msk_alpha/__init__.py` & `aws-cdk.aws-msk-alpha-2.9.0a0/src/aws_cdk/aws_msk_alpha/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 
 ```python
 # cluster: msk.Cluster
 
 CfnOutput(self, "BootstrapBrokers", value=cluster.bootstrap_brokers)
 CfnOutput(self, "BootstrapBrokersTls", value=cluster.bootstrap_brokers_tls)
 CfnOutput(self, "BootstrapBrokersSaslScram", value=cluster.bootstrap_brokers_sasl_scram)
-CfnOutput(self, "BootstrapBrokerStringSaslIam", value=cluster.bootstrap_brokers_sasl_iam)
 CfnOutput(self, "ZookeeperConnection", value=cluster.zookeeper_connection_string)
 CfnOutput(self, "ZookeeperConnectionTls", value=cluster.zookeeper_connection_string_tls)
 ```
 
 ## Importing an existing Cluster
 
 To import an existing MSK cluster into your CDK app use the `.fromClusterArn()` method.
@@ -73,14 +72,16 @@
 cluster = msk.Cluster.from_cluster_arn(self, "Cluster", "arn:aws:kafka:us-west-2:1234567890:cluster/a-cluster/11111111-1111-1111-1111-111111111111-1")
 ```
 
 ## Client Authentication
 
 [MSK supports](https://docs.aws.amazon.com/msk/latest/developerguide/kafka_apis_iam.html) the following authentication mechanisms.
 
+> Only one authentication method can be enabled.
+
 ### TLS
 
 To enable client authentication with TLS set the `certificateAuthorityArns` property to reference your ACM Private CA. [More info on Private CAs.](https://docs.aws.amazon.com/msk/latest/developerguide/msk-authentication.html)
 
 ```python
 import aws_cdk.aws_acmpca as acmpca
 
@@ -136,99 +137,34 @@
         client_broker=msk.ClientBrokerEncryption.TLS
     ),
     client_authentication=msk.ClientAuthentication.sasl(
         iam=True
     )
 )
 ```
-
-### SASL/IAM + TLS
-
-Enable client authentication with [IAM](https://docs.aws.amazon.com/msk/latest/developerguide/iam-access-control.html)
-as well as enable client authentication with TLS by setting the `certificateAuthorityArns` property to reference your ACM Private CA. [More info on Private CAs.](https://docs.aws.amazon.com/msk/latest/developerguide/msk-authentication.html)
-
-```python
-import aws_cdk.aws_acmpca as acmpca
-
-# vpc: ec2.Vpc
-
-cluster = msk.Cluster(self, "Cluster",
-    cluster_name="myCluster",
-    kafka_version=msk.KafkaVersion.V2_8_1,
-    vpc=vpc,
-    encryption_in_transit=msk.EncryptionInTransitConfig(
-        client_broker=msk.ClientBrokerEncryption.TLS
-    ),
-    client_authentication=msk.ClientAuthentication.sasl_tls(
-        iam=True,
-        certificate_authorities=[
-            acmpca.CertificateAuthority.from_certificate_authority_arn(self, "CertificateAuthority", "arn:aws:acm-pca:us-west-2:1234567890:certificate-authority/11111111-1111-1111-1111-111111111111")
-        ]
-    )
-)
-```
-
-## Logging
-
-You can deliver Apache Kafka broker logs to one or more of the following destination types:
-Amazon CloudWatch Logs, Amazon S3, Amazon Kinesis Data Firehose.
-
-To configure logs to be sent to an S3 bucket, provide a bucket in the `logging` config.
-
-```python
-# vpc: ec2.Vpc
-# bucket: s3.IBucket
-
-cluster = msk.Cluster(self, "cluster",
-    cluster_name="myCluster",
-    kafka_version=msk.KafkaVersion.V2_8_1,
-    vpc=vpc,
-    logging=msk.BrokerLogging(
-        s3=msk.S3LoggingConfiguration(
-            bucket=bucket
-        )
-    )
-)
-```
-
-When the S3 destination is configured, AWS will automatically create an S3 bucket policy
-that allows the service to write logs to the bucket. This makes it impossible to later update
-that bucket policy. To have CDK create the bucket policy so that future updates can be made,
-the `@aws-cdk/aws-s3:createDefaultLoggingPolicy` [feature flag](https://docs.aws.amazon.com/cdk/v2/guide/featureflags.html) can be used. This can be set
-in the `cdk.json` file.
-
-```json
-{
-  "context": {
-    "@aws-cdk/aws-s3:createDefaultLoggingPolicy": true
-  }
-}
-```
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
 import publication
 import typing_extensions
 
-from typeguard import check_type
-
 from ._jsii import *
 
-import aws_cdk as _aws_cdk_ceddda9d
-import aws_cdk.aws_acmpca as _aws_cdk_aws_acmpca_ceddda9d
-import aws_cdk.aws_ec2 as _aws_cdk_aws_ec2_ceddda9d
-import aws_cdk.aws_kms as _aws_cdk_aws_kms_ceddda9d
-import aws_cdk.aws_logs as _aws_cdk_aws_logs_ceddda9d
-import aws_cdk.aws_s3 as _aws_cdk_aws_s3_ceddda9d
-import constructs as _constructs_77d1e7e8
+import aws_cdk
+import aws_cdk.aws_acmpca
+import aws_cdk.aws_ec2
+import aws_cdk.aws_kms
+import aws_cdk.aws_logs
+import aws_cdk.aws_s3
+import constructs
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-msk-alpha.BrokerLogging",
     jsii_struct_bases=[],
     name_mapping={
         "cloudwatch_log_group": "cloudwatchLogGroup",
@@ -236,70 +172,69 @@
         "s3": "s3",
     },
 )
 class BrokerLogging:
     def __init__(
         self,
         *,
-        cloudwatch_log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
+        cloudwatch_log_group: typing.Optional[aws_cdk.aws_logs.ILogGroup] = None,
         firehose_delivery_stream_name: typing.Optional[builtins.str] = None,
-        s3: typing.Optional[typing.Union["S3LoggingConfiguration", typing.Dict[builtins.str, typing.Any]]] = None,
+        s3: typing.Optional["S3LoggingConfiguration"] = None,
     ) -> None:
         '''(experimental) Configuration details related to broker logs.
 
         :param cloudwatch_log_group: (experimental) The CloudWatch Logs group that is the destination for broker logs. Default: - disabled
         :param firehose_delivery_stream_name: (experimental) The Kinesis Data Firehose delivery stream that is the destination for broker logs. Default: - disabled
         :param s3: (experimental) Details of the Amazon S3 destination for broker logs. Default: - disabled
 
         :stability: experimental
-        :exampleMetadata: infused
+        :exampleMetadata: fixture=_generated
 
         Example::
 
-            # vpc: ec2.Vpc
-            # bucket: s3.IBucket
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.aws_msk_alpha as msk_alpha
+            from aws_cdk import aws_logs as logs
+            from aws_cdk import aws_s3 as s3
             
-            cluster = msk.Cluster(self, "cluster",
-                cluster_name="myCluster",
-                kafka_version=msk.KafkaVersion.V2_8_1,
-                vpc=vpc,
-                logging=msk.BrokerLogging(
-                    s3=msk.S3LoggingConfiguration(
-                        bucket=bucket
-                    )
+            # bucket: s3.Bucket
+            # log_group: logs.LogGroup
+            
+            broker_logging = msk_alpha.BrokerLogging(
+                cloudwatch_log_group=log_group,
+                firehose_delivery_stream_name="firehoseDeliveryStreamName",
+                s3=msk_alpha.S3LoggingConfiguration(
+                    bucket=bucket,
+            
+                    # the properties below are optional
+                    prefix="prefix"
                 )
             )
         '''
         if isinstance(s3, dict):
             s3 = S3LoggingConfiguration(**s3)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9ba586b7db9e5dd092a5b8f9676408abd0e8865e17a5980b7acb9ac4b970f225)
-            check_type(argname="argument cloudwatch_log_group", value=cloudwatch_log_group, expected_type=type_hints["cloudwatch_log_group"])
-            check_type(argname="argument firehose_delivery_stream_name", value=firehose_delivery_stream_name, expected_type=type_hints["firehose_delivery_stream_name"])
-            check_type(argname="argument s3", value=s3, expected_type=type_hints["s3"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if cloudwatch_log_group is not None:
             self._values["cloudwatch_log_group"] = cloudwatch_log_group
         if firehose_delivery_stream_name is not None:
             self._values["firehose_delivery_stream_name"] = firehose_delivery_stream_name
         if s3 is not None:
             self._values["s3"] = s3
 
     @builtins.property
-    def cloudwatch_log_group(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup]:
+    def cloudwatch_log_group(self) -> typing.Optional[aws_cdk.aws_logs.ILogGroup]:
         '''(experimental) The CloudWatch Logs group that is the destination for broker logs.
 
         :default: - disabled
 
         :stability: experimental
         '''
         result = self._values.get("cloudwatch_log_group")
-        return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_logs.ILogGroup], result)
 
     @builtins.property
     def firehose_delivery_stream_name(self) -> typing.Optional[builtins.str]:
         '''(experimental) The Kinesis Data Firehose delivery stream that is the destination for broker logs.
 
         :default: - disabled
 
@@ -338,109 +273,77 @@
     '''(experimental) Configuration properties for client authentication.
 
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
-        import aws_cdk.aws_acmpca as acmpca
-        
         # vpc: ec2.Vpc
         
-        cluster = msk.Cluster(self, "Cluster",
+        cluster = msk.Cluster(self, "cluster",
             cluster_name="myCluster",
             kafka_version=msk.KafkaVersion.V2_8_1,
             vpc=vpc,
             encryption_in_transit=msk.EncryptionInTransitConfig(
                 client_broker=msk.ClientBrokerEncryption.TLS
             ),
-            client_authentication=msk.ClientAuthentication.tls(
-                certificate_authorities=[
-                    acmpca.CertificateAuthority.from_certificate_authority_arn(self, "CertificateAuthority", "arn:aws:acm-pca:us-west-2:1234567890:certificate-authority/11111111-1111-1111-1111-111111111111")
-                ]
+            client_authentication=msk.ClientAuthentication.sasl(
+                scram=True
             )
         )
     '''
 
-    @jsii.member(jsii_name="sasl")
+    @jsii.member(jsii_name="sasl") # type: ignore[misc]
     @builtins.classmethod
     def sasl(
         cls,
         *,
         iam: typing.Optional[builtins.bool] = None,
-        key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
         scram: typing.Optional[builtins.bool] = None,
     ) -> "ClientAuthentication":
         '''(experimental) SASL authentication.
 
         :param iam: (experimental) Enable IAM access control. Default: false
         :param key: (experimental) KMS Key to encrypt SASL/SCRAM secrets. You must use a customer master key (CMK) when creating users in secrets manager. You cannot use a Secret with Amazon MSK that uses the default Secrets Manager encryption key. Default: - CMK will be created with alias msk/{clusterName}/sasl/scram
         :param scram: (experimental) Enable SASL/SCRAM authentication. Default: false
 
         :stability: experimental
         '''
         props = SaslAuthProps(iam=iam, key=key, scram=scram)
 
         return typing.cast("ClientAuthentication", jsii.sinvoke(cls, "sasl", [props]))
 
-    @jsii.member(jsii_name="saslTls")
-    @builtins.classmethod
-    def sasl_tls(
-        cls,
-        *,
-        iam: typing.Optional[builtins.bool] = None,
-        key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-        scram: typing.Optional[builtins.bool] = None,
-        certificate_authorities: typing.Optional[typing.Sequence[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]] = None,
-    ) -> "ClientAuthentication":
-        '''(experimental) SASL + TLS authentication.
-
-        :param iam: (experimental) Enable IAM access control. Default: false
-        :param key: (experimental) KMS Key to encrypt SASL/SCRAM secrets. You must use a customer master key (CMK) when creating users in secrets manager. You cannot use a Secret with Amazon MSK that uses the default Secrets Manager encryption key. Default: - CMK will be created with alias msk/{clusterName}/sasl/scram
-        :param scram: (experimental) Enable SASL/SCRAM authentication. Default: false
-        :param certificate_authorities: (experimental) List of ACM Certificate Authorities to enable TLS authentication. Default: - none
-
-        :stability: experimental
-        '''
-        sasl_tls_props = SaslTlsAuthProps(
-            iam=iam,
-            key=key,
-            scram=scram,
-            certificate_authorities=certificate_authorities,
-        )
-
-        return typing.cast("ClientAuthentication", jsii.sinvoke(cls, "saslTls", [sasl_tls_props]))
-
-    @jsii.member(jsii_name="tls")
+    @jsii.member(jsii_name="tls") # type: ignore[misc]
     @builtins.classmethod
     def tls(
         cls,
         *,
-        certificate_authorities: typing.Optional[typing.Sequence[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]] = None,
+        certificate_authorities: typing.Optional[typing.Sequence[aws_cdk.aws_acmpca.ICertificateAuthority]] = None,
     ) -> "ClientAuthentication":
         '''(experimental) TLS authentication.
 
         :param certificate_authorities: (experimental) List of ACM Certificate Authorities to enable TLS authentication. Default: - none
 
         :stability: experimental
         '''
         props = TlsAuthProps(certificate_authorities=certificate_authorities)
 
         return typing.cast("ClientAuthentication", jsii.sinvoke(cls, "tls", [props]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="saslProps")
     def sasl_props(self) -> typing.Optional["SaslAuthProps"]:
         '''(experimental) - properties for SASL authentication.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional["SaslAuthProps"], jsii.get(self, "saslProps"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="tlsProps")
     def tls_props(self) -> typing.Optional["TlsAuthProps"]:
         '''(experimental) - properties for TLS authentication.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional["TlsAuthProps"], jsii.get(self, "tlsProps"))
@@ -451,29 +354,25 @@
     '''(experimental) Indicates the encryption setting for data in transit between clients and brokers.
 
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
-        import aws_cdk.aws_acmpca as acmpca
-        
         # vpc: ec2.Vpc
         
-        cluster = msk.Cluster(self, "Cluster",
+        cluster = msk.Cluster(self, "cluster",
             cluster_name="myCluster",
             kafka_version=msk.KafkaVersion.V2_8_1,
             vpc=vpc,
             encryption_in_transit=msk.EncryptionInTransitConfig(
                 client_broker=msk.ClientBrokerEncryption.TLS
             ),
-            client_authentication=msk.ClientAuthentication.tls(
-                certificate_authorities=[
-                    acmpca.CertificateAuthority.from_certificate_authority_arn(self, "CertificateAuthority", "arn:aws:acm-pca:us-west-2:1234567890:certificate-authority/11111111-1111-1111-1111-111111111111")
-                ]
+            client_authentication=msk.ClientAuthentication.sasl(
+                scram=True
             )
         )
     '''
 
     TLS = "TLS"
     '''(experimental) TLS means that client-broker communication is enabled with TLS only.
 
@@ -515,19 +414,15 @@
             import aws_cdk.aws_msk_alpha as msk_alpha
             
             cluster_configuration_info = msk_alpha.ClusterConfigurationInfo(
                 arn="arn",
                 revision=123
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a3c843d4de610e7657dc25ae7cbdd2c8bba8b60a980c8877eba757e6e63c7ebd)
-            check_type(argname="argument arn", value=arn, expected_type=type_hints["arn"])
-            check_type(argname="argument revision", value=revision, expected_type=type_hints["revision"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "arn": arn,
             "revision": revision,
         }
 
     @builtins.property
     def arn(self) -> builtins.str:
         '''(experimental) The Amazon Resource Name (ARN) of the MSK configuration to use.
@@ -614,26 +509,26 @@
 )
 class ClusterProps:
     def __init__(
         self,
         *,
         cluster_name: builtins.str,
         kafka_version: "KafkaVersion",
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
+        vpc: aws_cdk.aws_ec2.IVpc,
         client_authentication: typing.Optional[ClientAuthentication] = None,
-        configuration_info: typing.Optional[typing.Union[ClusterConfigurationInfo, typing.Dict[builtins.str, typing.Any]]] = None,
-        ebs_storage_info: typing.Optional[typing.Union["EbsStorageInfo", typing.Dict[builtins.str, typing.Any]]] = None,
-        encryption_in_transit: typing.Optional[typing.Union["EncryptionInTransitConfig", typing.Dict[builtins.str, typing.Any]]] = None,
-        instance_type: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.InstanceType] = None,
-        logging: typing.Optional[typing.Union[BrokerLogging, typing.Dict[builtins.str, typing.Any]]] = None,
-        monitoring: typing.Optional[typing.Union["MonitoringConfiguration", typing.Dict[builtins.str, typing.Any]]] = None,
+        configuration_info: typing.Optional[ClusterConfigurationInfo] = None,
+        ebs_storage_info: typing.Optional["EbsStorageInfo"] = None,
+        encryption_in_transit: typing.Optional["EncryptionInTransitConfig"] = None,
+        instance_type: typing.Optional[aws_cdk.aws_ec2.InstanceType] = None,
+        logging: typing.Optional[BrokerLogging] = None,
+        monitoring: typing.Optional["MonitoringConfiguration"] = None,
         number_of_broker_nodes: typing.Optional[jsii.Number] = None,
-        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-        vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        removal_policy: typing.Optional[aws_cdk.RemovalPolicy] = None,
+        security_groups: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.ISecurityGroup]] = None,
+        vpc_subnets: typing.Optional[aws_cdk.aws_ec2.SubnetSelection] = None,
     ) -> None:
         '''(experimental) Properties for a MSK Cluster.
 
         :param cluster_name: (experimental) The physical name of the cluster.
         :param kafka_version: (experimental) The version of Apache Kafka.
         :param vpc: (experimental) Defines the virtual networking environment for this cluster. Must have at least 2 subnets in two different AZs.
         :param client_authentication: (experimental) Configuration properties for client authentication. MSK supports using private TLS certificates or SASL/SCRAM to authenticate the identity of clients. Default: - disabled
@@ -674,32 +569,16 @@
         if isinstance(encryption_in_transit, dict):
             encryption_in_transit = EncryptionInTransitConfig(**encryption_in_transit)
         if isinstance(logging, dict):
             logging = BrokerLogging(**logging)
         if isinstance(monitoring, dict):
             monitoring = MonitoringConfiguration(**monitoring)
         if isinstance(vpc_subnets, dict):
-            vpc_subnets = _aws_cdk_aws_ec2_ceddda9d.SubnetSelection(**vpc_subnets)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7acb1d0e21413d16efb1d11f4a29cc860b92ac278e0b0187d75e3eb1f71b1492)
-            check_type(argname="argument cluster_name", value=cluster_name, expected_type=type_hints["cluster_name"])
-            check_type(argname="argument kafka_version", value=kafka_version, expected_type=type_hints["kafka_version"])
-            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
-            check_type(argname="argument client_authentication", value=client_authentication, expected_type=type_hints["client_authentication"])
-            check_type(argname="argument configuration_info", value=configuration_info, expected_type=type_hints["configuration_info"])
-            check_type(argname="argument ebs_storage_info", value=ebs_storage_info, expected_type=type_hints["ebs_storage_info"])
-            check_type(argname="argument encryption_in_transit", value=encryption_in_transit, expected_type=type_hints["encryption_in_transit"])
-            check_type(argname="argument instance_type", value=instance_type, expected_type=type_hints["instance_type"])
-            check_type(argname="argument logging", value=logging, expected_type=type_hints["logging"])
-            check_type(argname="argument monitoring", value=monitoring, expected_type=type_hints["monitoring"])
-            check_type(argname="argument number_of_broker_nodes", value=number_of_broker_nodes, expected_type=type_hints["number_of_broker_nodes"])
-            check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
-            check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
-            check_type(argname="argument vpc_subnets", value=vpc_subnets, expected_type=type_hints["vpc_subnets"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+            vpc_subnets = aws_cdk.aws_ec2.SubnetSelection(**vpc_subnets)
+        self._values: typing.Dict[str, typing.Any] = {
             "cluster_name": cluster_name,
             "kafka_version": kafka_version,
             "vpc": vpc,
         }
         if client_authentication is not None:
             self._values["client_authentication"] = client_authentication
         if configuration_info is not None:
@@ -740,24 +619,24 @@
         :stability: experimental
         '''
         result = self._values.get("kafka_version")
         assert result is not None, "Required property 'kafka_version' is missing"
         return typing.cast("KafkaVersion", result)
 
     @builtins.property
-    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
+    def vpc(self) -> aws_cdk.aws_ec2.IVpc:
         '''(experimental) Defines the virtual networking environment for this cluster.
 
         Must have at least 2 subnets in two different AZs.
 
         :stability: experimental
         '''
         result = self._values.get("vpc")
         assert result is not None, "Required property 'vpc' is missing"
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, result)
+        return typing.cast(aws_cdk.aws_ec2.IVpc, result)
 
     @builtins.property
     def client_authentication(self) -> typing.Optional[ClientAuthentication]:
         '''(experimental) Configuration properties for client authentication.
 
         MSK supports using private TLS certificates or SASL/SCRAM to authenticate the identity of clients.
 
@@ -798,24 +677,24 @@
 
         :stability: experimental
         '''
         result = self._values.get("encryption_in_transit")
         return typing.cast(typing.Optional["EncryptionInTransitConfig"], result)
 
     @builtins.property
-    def instance_type(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.InstanceType]:
+    def instance_type(self) -> typing.Optional[aws_cdk.aws_ec2.InstanceType]:
         '''(experimental) The EC2 instance type that you want Amazon MSK to use when it creates your brokers.
 
         :default: kafka.m5.large
 
         :see: https://docs.aws.amazon.com/msk/latest/developerguide/msk-create-cluster.html#broker-instance-types
         :stability: experimental
         '''
         result = self._values.get("instance_type")
-        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.InstanceType], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_ec2.InstanceType], result)
 
     @builtins.property
     def logging(self) -> typing.Optional[BrokerLogging]:
         '''(experimental) Configure your MSK cluster to send broker logs to different destination types.
 
         :default: - disabled
 
@@ -843,51 +722,51 @@
 
         :stability: experimental
         '''
         result = self._values.get("number_of_broker_nodes")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
-    def removal_policy(self) -> typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy]:
+    def removal_policy(self) -> typing.Optional[aws_cdk.RemovalPolicy]:
         '''(experimental) What to do when this resource is deleted from a stack.
 
         :default: RemovalPolicy.RETAIN
 
         :stability: experimental
         '''
         result = self._values.get("removal_policy")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy], result)
+        return typing.cast(typing.Optional[aws_cdk.RemovalPolicy], result)
 
     @builtins.property
     def security_groups(
         self,
-    ) -> typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]]:
+    ) -> typing.Optional[typing.List[aws_cdk.aws_ec2.ISecurityGroup]]:
         '''(experimental) The AWS security groups to associate with the elastic network interfaces in order to specify who can connect to and communicate with the Amazon MSK cluster.
 
         :default: - create new security group
 
         :stability: experimental
         '''
         result = self._values.get("security_groups")
-        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]], result)
+        return typing.cast(typing.Optional[typing.List[aws_cdk.aws_ec2.ISecurityGroup]], result)
 
     @builtins.property
-    def vpc_subnets(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection]:
+    def vpc_subnets(self) -> typing.Optional[aws_cdk.aws_ec2.SubnetSelection]:
         '''(experimental) Where to place the nodes within the VPC.
 
         Amazon MSK distributes the broker nodes evenly across the subnets that you specify.
         The subnets that you specify must be in distinct Availability Zones.
         Client subnets can't be in Availability Zone us-east-1e.
 
         :default: - the Vpc default strategy if not specified.
 
         :stability: experimental
         '''
         result = self._values.get("vpc_subnets")
-        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_ec2.SubnetSelection], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -902,15 +781,15 @@
     jsii_struct_bases=[],
     name_mapping={"encryption_key": "encryptionKey", "volume_size": "volumeSize"},
 )
 class EbsStorageInfo:
     def __init__(
         self,
         *,
-        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
         volume_size: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''(experimental) EBS volume information.
 
         :param encryption_key: (experimental) The AWS KMS key for encrypting data at rest. Default: Uses AWS managed CMK (aws/kafka)
         :param volume_size: (experimental) The size in GiB of the EBS volume for the data drive on each broker node. Default: 1000
 
@@ -927,34 +806,30 @@
             # key: kms.Key
             
             ebs_storage_info = msk_alpha.EbsStorageInfo(
                 encryption_key=key,
                 volume_size=123
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__71f71898e3644c01cacd375914aebc2f51bc973e16dca3550d856073a05c90ee)
-            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
-            check_type(argname="argument volume_size", value=volume_size, expected_type=type_hints["volume_size"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if encryption_key is not None:
             self._values["encryption_key"] = encryption_key
         if volume_size is not None:
             self._values["volume_size"] = volume_size
 
     @builtins.property
-    def encryption_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def encryption_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) The AWS KMS key for encrypting data at rest.
 
         :default: Uses AWS managed CMK (aws/kafka)
 
         :stability: experimental
         '''
         result = self._values.get("encryption_key")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], result)
 
     @builtins.property
     def volume_size(self) -> typing.Optional[jsii.Number]:
         '''(experimental) The size in GiB of the EBS volume for the data drive on each broker node.
 
         :default: 1000
 
@@ -997,37 +872,29 @@
 
         :see: https://docs.aws.amazon.com/msk/latest/developerguide/msk-encryption.html#msk-encryption-in-transit
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
-            import aws_cdk.aws_acmpca as acmpca
-            
             # vpc: ec2.Vpc
             
-            cluster = msk.Cluster(self, "Cluster",
+            cluster = msk.Cluster(self, "cluster",
                 cluster_name="myCluster",
                 kafka_version=msk.KafkaVersion.V2_8_1,
                 vpc=vpc,
                 encryption_in_transit=msk.EncryptionInTransitConfig(
                     client_broker=msk.ClientBrokerEncryption.TLS
                 ),
-                client_authentication=msk.ClientAuthentication.tls(
-                    certificate_authorities=[
-                        acmpca.CertificateAuthority.from_certificate_authority_arn(self, "CertificateAuthority", "arn:aws:acm-pca:us-west-2:1234567890:certificate-authority/11111111-1111-1111-1111-111111111111")
-                    ]
+                client_authentication=msk.ClientAuthentication.sasl(
+                    scram=True
                 )
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__72b66a42c0d765a1bd551981cf4b9d5840e1974336776a8da3877d190634cf50)
-            check_type(argname="argument client_broker", value=client_broker, expected_type=type_hints["client_broker"])
-            check_type(argname="argument enable_in_cluster", value=enable_in_cluster, expected_type=type_hints["enable_in_cluster"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if client_broker is not None:
             self._values["client_broker"] = client_broker
         if enable_in_cluster is not None:
             self._values["enable_in_cluster"] = enable_in_cluster
 
     @builtins.property
     def client_broker(self) -> typing.Optional[ClientBrokerEncryption]:
@@ -1061,66 +928,66 @@
         return "EncryptionInTransitConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-msk-alpha.ICluster")
 class ICluster(
-    _aws_cdk_ceddda9d.IResource,
-    _aws_cdk_aws_ec2_ceddda9d.IConnectable,
+    aws_cdk.IResource,
+    aws_cdk.aws_ec2.IConnectable,
     typing_extensions.Protocol,
 ):
     '''(experimental) Represents a MSK Cluster.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterArn")
     def cluster_arn(self) -> builtins.str:
         '''(experimental) The ARN of cluster.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterName")
     def cluster_name(self) -> builtins.str:
         '''(experimental) The physical name of the cluster.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _IClusterProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
-    jsii.proxy_for(_aws_cdk_aws_ec2_ceddda9d.IConnectable), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.aws_ec2.IConnectable), # type: ignore[misc]
 ):
     '''(experimental) Represents a MSK Cluster.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-msk-alpha.ICluster"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterArn")
     def cluster_arn(self) -> builtins.str:
         '''(experimental) The ARN of cluster.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "clusterArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterName")
     def cluster_name(self) -> builtins.str:
         '''(experimental) The physical name of the cluster.
 
         :stability: experimental
         :attribute: true
         '''
@@ -1152,204 +1019,152 @@
             ),
             client_authentication=msk.ClientAuthentication.sasl(
                 scram=True
             )
         )
     '''
 
-    @jsii.member(jsii_name="of")
+    @jsii.member(jsii_name="of") # type: ignore[misc]
     @builtins.classmethod
     def of(cls, version: builtins.str) -> "KafkaVersion":
         '''(experimental) Custom cluster version.
 
         :param version: custom version number.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e717a461a7dfd2af4c0ea436fee0dcfb2c9d05e9d05e0ff37e25c47c088b68ff)
-            check_type(argname="argument version", value=version, expected_type=type_hints["version"])
         return typing.cast("KafkaVersion", jsii.sinvoke(cls, "of", [version]))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V1_1_1")
     def V1_1_1(cls) -> "KafkaVersion":
-        '''(deprecated) **Deprecated by Amazon MSK. You can't create a Kafka cluster with a deprecated version.**.
-
-        Kafka version 1.1.1
-
-        :deprecated: use the latest runtime instead
+        '''(experimental) Kafka version 1.1.1.
 
-        :stability: deprecated
+        :stability: experimental
         '''
         return typing.cast("KafkaVersion", jsii.sget(cls, "V1_1_1"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V2_2_1")
     def V2_2_1(cls) -> "KafkaVersion":
         '''(experimental) Kafka version 2.2.1.
 
         :stability: experimental
         '''
         return typing.cast("KafkaVersion", jsii.sget(cls, "V2_2_1"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V2_3_1")
     def V2_3_1(cls) -> "KafkaVersion":
         '''(experimental) Kafka version 2.3.1.
 
         :stability: experimental
         '''
         return typing.cast("KafkaVersion", jsii.sget(cls, "V2_3_1"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V2_4_1_1")
     def V2_4_1_1(cls) -> "KafkaVersion":
         '''(experimental) Kafka version 2.4.1.
 
         :stability: experimental
         '''
         return typing.cast("KafkaVersion", jsii.sget(cls, "V2_4_1_1"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V2_5_1")
     def V2_5_1(cls) -> "KafkaVersion":
         '''(experimental) Kafka version 2.5.1.
 
         :stability: experimental
         '''
         return typing.cast("KafkaVersion", jsii.sget(cls, "V2_5_1"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V2_6_0")
     def V2_6_0(cls) -> "KafkaVersion":
         '''(experimental) Kafka version 2.6.0.
 
         :stability: experimental
         '''
         return typing.cast("KafkaVersion", jsii.sget(cls, "V2_6_0"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V2_6_1")
     def V2_6_1(cls) -> "KafkaVersion":
         '''(experimental) Kafka version 2.6.1.
 
         :stability: experimental
         '''
         return typing.cast("KafkaVersion", jsii.sget(cls, "V2_6_1"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V2_6_2")
     def V2_6_2(cls) -> "KafkaVersion":
         '''(experimental) Kafka version 2.6.2.
 
         :stability: experimental
         '''
         return typing.cast("KafkaVersion", jsii.sget(cls, "V2_6_2"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V2_6_3")
     def V2_6_3(cls) -> "KafkaVersion":
         '''(experimental) Kafka version 2.6.3.
 
         :stability: experimental
         '''
         return typing.cast("KafkaVersion", jsii.sget(cls, "V2_6_3"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V2_7_0")
     def V2_7_0(cls) -> "KafkaVersion":
         '''(experimental) Kafka version 2.7.0.
 
         :stability: experimental
         '''
         return typing.cast("KafkaVersion", jsii.sget(cls, "V2_7_0"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V2_7_1")
     def V2_7_1(cls) -> "KafkaVersion":
         '''(experimental) Kafka version 2.7.1.
 
         :stability: experimental
         '''
         return typing.cast("KafkaVersion", jsii.sget(cls, "V2_7_1"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V2_7_2")
     def V2_7_2(cls) -> "KafkaVersion":
         '''(experimental) Kafka version 2.7.2.
 
         :stability: experimental
         '''
         return typing.cast("KafkaVersion", jsii.sget(cls, "V2_7_2"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V2_8_0")
     def V2_8_0(cls) -> "KafkaVersion":
         '''(experimental) Kafka version 2.8.0.
 
         :stability: experimental
         '''
         return typing.cast("KafkaVersion", jsii.sget(cls, "V2_8_0"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V2_8_1")
     def V2_8_1(cls) -> "KafkaVersion":
         '''(experimental) Kafka version 2.8.1.
 
         :stability: experimental
         '''
         return typing.cast("KafkaVersion", jsii.sget(cls, "V2_8_1"))
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V3_1_1")
-    def V3_1_1(cls) -> "KafkaVersion":
-        '''(experimental) Kafka version 3.1.1.
-
-        :stability: experimental
-        '''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V3_1_1"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V3_2_0")
-    def V3_2_0(cls) -> "KafkaVersion":
-        '''(experimental) Kafka version 3.2.0.
-
-        :stability: experimental
-        '''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V3_2_0"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V3_3_1")
-    def V3_3_1(cls) -> "KafkaVersion":
-        '''(experimental) Kafka version 3.3.1.
-
-        :stability: experimental
-        '''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V3_3_1"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V3_3_2")
-    def V3_3_2(cls) -> "KafkaVersion":
-        '''(experimental) Kafka version 3.3.2.
-
-        :stability: experimental
-        '''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V3_3_2"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V3_4_0")
-    def V3_4_0(cls) -> "KafkaVersion":
-        '''(experimental) Kafka version 3.4.0.
-
-        :stability: experimental
-        '''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V3_4_0"))
-
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="version")
     def version(self) -> builtins.str:
         '''(experimental) cluster version number.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "version"))
@@ -1389,20 +1204,15 @@
             
             monitoring_configuration = msk_alpha.MonitoringConfiguration(
                 cluster_monitoring_level=msk_alpha.ClusterMonitoringLevel.DEFAULT,
                 enable_prometheus_jmx_exporter=False,
                 enable_prometheus_node_exporter=False
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__af85a63aa3f07c68569eb1f6e9732a882ddeb2b7738ae8b80717edf2c96ef123)
-            check_type(argname="argument cluster_monitoring_level", value=cluster_monitoring_level, expected_type=type_hints["cluster_monitoring_level"])
-            check_type(argname="argument enable_prometheus_jmx_exporter", value=enable_prometheus_jmx_exporter, expected_type=type_hints["enable_prometheus_jmx_exporter"])
-            check_type(argname="argument enable_prometheus_node_exporter", value=enable_prometheus_node_exporter, expected_type=type_hints["enable_prometheus_node_exporter"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if cluster_monitoring_level is not None:
             self._values["cluster_monitoring_level"] = cluster_monitoring_level
         if enable_prometheus_jmx_exporter is not None:
             self._values["enable_prometheus_jmx_exporter"] = enable_prometheus_jmx_exporter
         if enable_prometheus_node_exporter is not None:
             self._values["enable_prometheus_node_exporter"] = enable_prometheus_node_exporter
 
@@ -1458,60 +1268,56 @@
     jsii_struct_bases=[],
     name_mapping={"bucket": "bucket", "prefix": "prefix"},
 )
 class S3LoggingConfiguration:
     def __init__(
         self,
         *,
-        bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        bucket: aws_cdk.aws_s3.IBucket,
         prefix: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Details of the Amazon S3 destination for broker logs.
 
         :param bucket: (experimental) The S3 bucket that is the destination for broker logs.
         :param prefix: (experimental) The S3 prefix that is the destination for broker logs. Default: - no prefix
 
         :stability: experimental
-        :exampleMetadata: infused
+        :exampleMetadata: fixture=_generated
 
         Example::
 
-            # vpc: ec2.Vpc
-            # bucket: s3.IBucket
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.aws_msk_alpha as msk_alpha
+            from aws_cdk import aws_s3 as s3
             
-            cluster = msk.Cluster(self, "cluster",
-                cluster_name="myCluster",
-                kafka_version=msk.KafkaVersion.V2_8_1,
-                vpc=vpc,
-                logging=msk.BrokerLogging(
-                    s3=msk.S3LoggingConfiguration(
-                        bucket=bucket
-                    )
-                )
+            # bucket: s3.Bucket
+            
+            s3_logging_configuration = msk_alpha.S3LoggingConfiguration(
+                bucket=bucket,
+            
+                # the properties below are optional
+                prefix="prefix"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__51fbd5191484562bb80360937520b2fcdc78a672c23d4c600aff0554ad23aa62)
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
         '''(experimental) The S3 bucket that is the destination for broker logs.
 
         :stability: experimental
         '''
         result = self._values.get("bucket")
         assert result is not None, "Required property 'bucket' is missing"
-        return typing.cast(_aws_cdk_aws_s3_ceddda9d.IBucket, result)
+        return typing.cast(aws_cdk.aws_s3.IBucket, result)
 
     @builtins.property
     def prefix(self) -> typing.Optional[builtins.str]:
         '''(experimental) The S3 prefix that is the destination for broker logs.
 
         :default: - no prefix
 
@@ -1538,15 +1344,15 @@
     name_mapping={"iam": "iam", "key": "key", "scram": "scram"},
 )
 class SaslAuthProps:
     def __init__(
         self,
         *,
         iam: typing.Optional[builtins.bool] = None,
-        key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
         scram: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''(experimental) SASL authentication properties.
 
         :param iam: (experimental) Enable IAM access control. Default: false
         :param key: (experimental) KMS Key to encrypt SASL/SCRAM secrets. You must use a customer master key (CMK) when creating users in secrets manager. You cannot use a Secret with Amazon MSK that uses the default Secrets Manager encryption key. Default: - CMK will be created with alias msk/{clusterName}/sasl/scram
         :param scram: (experimental) Enable SASL/SCRAM authentication. Default: false
@@ -1566,20 +1372,15 @@
                     client_broker=msk.ClientBrokerEncryption.TLS
                 ),
                 client_authentication=msk.ClientAuthentication.sasl(
                     scram=True
                 )
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f186e6270f30759471573a6fdea8241e1a52ec3ddb6f61ac669172717e5a8ea6)
-            check_type(argname="argument iam", value=iam, expected_type=type_hints["iam"])
-            check_type(argname="argument key", value=key, expected_type=type_hints["key"])
-            check_type(argname="argument scram", value=scram, expected_type=type_hints["scram"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if iam is not None:
             self._values["iam"] = iam
         if key is not None:
             self._values["key"] = key
         if scram is not None:
             self._values["scram"] = scram
 
@@ -1591,26 +1392,26 @@
 
         :stability: experimental
         '''
         result = self._values.get("iam")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) KMS Key to encrypt SASL/SCRAM secrets.
 
         You must use a customer master key (CMK) when creating users in secrets manager.
         You cannot use a Secret with Amazon MSK that uses the default Secrets Manager encryption key.
 
         :default: - CMK will be created with alias msk/{clusterName}/sasl/scram
 
         :stability: experimental
         '''
         result = self._values.get("key")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], result)
 
     @builtins.property
     def scram(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Enable SASL/SCRAM authentication.
 
         :default: false
 
@@ -1636,15 +1437,15 @@
     jsii_struct_bases=[],
     name_mapping={"certificate_authorities": "certificateAuthorities"},
 )
 class TlsAuthProps:
     def __init__(
         self,
         *,
-        certificate_authorities: typing.Optional[typing.Sequence[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]] = None,
+        certificate_authorities: typing.Optional[typing.Sequence[aws_cdk.aws_acmpca.ICertificateAuthority]] = None,
     ) -> None:
         '''(experimental) TLS authentication properties.
 
         :param certificate_authorities: (experimental) List of ACM Certificate Authorities to enable TLS authentication. Default: - none
 
         :stability: experimental
         :exampleMetadata: infused
@@ -1665,33 +1466,30 @@
                 client_authentication=msk.ClientAuthentication.tls(
                     certificate_authorities=[
                         acmpca.CertificateAuthority.from_certificate_authority_arn(self, "CertificateAuthority", "arn:aws:acm-pca:us-west-2:1234567890:certificate-authority/11111111-1111-1111-1111-111111111111")
                     ]
                 )
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e699112e7fd831ecbdb6721274774f9c6ca4c3a0a7bee752f311fcbdf1e3eb25)
-            check_type(argname="argument certificate_authorities", value=certificate_authorities, expected_type=type_hints["certificate_authorities"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if certificate_authorities is not None:
             self._values["certificate_authorities"] = certificate_authorities
 
     @builtins.property
     def certificate_authorities(
         self,
-    ) -> typing.Optional[typing.List[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]]:
+    ) -> typing.Optional[typing.List[aws_cdk.aws_acmpca.ICertificateAuthority]]:
         '''(experimental) List of ACM Certificate Authorities to enable TLS authentication.
 
         :default: - none
 
         :stability: experimental
         '''
         result = self._values.get("certificate_authorities")
-        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]], result)
+        return typing.cast(typing.Optional[typing.List[aws_cdk.aws_acmpca.ICertificateAuthority]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -1699,23 +1497,23 @@
         return "TlsAuthProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.implements(ICluster)
 class Cluster(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-msk-alpha.Cluster",
 ):
     '''(experimental) Create a MSK Cluster.
 
     :stability: experimental
-    :resource: AWS::MSK::Cluster
     :exampleMetadata: infused
+    :resource: AWS::MSK::Cluster
 
     Example::
 
         # vpc: ec2.Vpc
         
         cluster = msk.Cluster(self, "cluster",
             cluster_name="myCluster",
@@ -1728,31 +1526,31 @@
                 scram=True
             )
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         cluster_name: builtins.str,
         kafka_version: KafkaVersion,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
+        vpc: aws_cdk.aws_ec2.IVpc,
         client_authentication: typing.Optional[ClientAuthentication] = None,
-        configuration_info: typing.Optional[typing.Union[ClusterConfigurationInfo, typing.Dict[builtins.str, typing.Any]]] = None,
-        ebs_storage_info: typing.Optional[typing.Union[EbsStorageInfo, typing.Dict[builtins.str, typing.Any]]] = None,
-        encryption_in_transit: typing.Optional[typing.Union[EncryptionInTransitConfig, typing.Dict[builtins.str, typing.Any]]] = None,
-        instance_type: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.InstanceType] = None,
-        logging: typing.Optional[typing.Union[BrokerLogging, typing.Dict[builtins.str, typing.Any]]] = None,
-        monitoring: typing.Optional[typing.Union[MonitoringConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
+        configuration_info: typing.Optional[ClusterConfigurationInfo] = None,
+        ebs_storage_info: typing.Optional[EbsStorageInfo] = None,
+        encryption_in_transit: typing.Optional[EncryptionInTransitConfig] = None,
+        instance_type: typing.Optional[aws_cdk.aws_ec2.InstanceType] = None,
+        logging: typing.Optional[BrokerLogging] = None,
+        monitoring: typing.Optional[MonitoringConfiguration] = None,
         number_of_broker_nodes: typing.Optional[jsii.Number] = None,
-        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-        vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        removal_policy: typing.Optional[aws_cdk.RemovalPolicy] = None,
+        security_groups: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.ISecurityGroup]] = None,
+        vpc_subnets: typing.Optional[aws_cdk.aws_ec2.SubnetSelection] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param cluster_name: (experimental) The physical name of the cluster.
         :param kafka_version: (experimental) The version of Apache Kafka.
         :param vpc: (experimental) Defines the virtual networking environment for this cluster. Must have at least 2 subnets in two different AZs.
@@ -1766,18 +1564,14 @@
         :param number_of_broker_nodes: (experimental) Number of Apache Kafka brokers deployed in each Availability Zone. Default: 1
         :param removal_policy: (experimental) What to do when this resource is deleted from a stack. Default: RemovalPolicy.RETAIN
         :param security_groups: (experimental) The AWS security groups to associate with the elastic network interfaces in order to specify who can connect to and communicate with the Amazon MSK cluster. Default: - create new security group
         :param vpc_subnets: (experimental) Where to place the nodes within the VPC. Amazon MSK distributes the broker nodes evenly across the subnets that you specify. The subnets that you specify must be in distinct Availability Zones. Client subnets can't be in Availability Zone us-east-1e. Default: - the Vpc default strategy if not specified.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__915d701802577130bfeeac000a90d2329d756ddabd799173074e0b31599dc1da)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = ClusterProps(
             cluster_name=cluster_name,
             kafka_version=kafka_version,
             vpc=vpc,
             client_authentication=client_authentication,
             configuration_info=configuration_info,
             ebs_storage_info=ebs_storage_info,
@@ -1789,35 +1583,30 @@
             removal_policy=removal_policy,
             security_groups=security_groups,
             vpc_subnets=vpc_subnets,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromClusterArn")
+    @jsii.member(jsii_name="fromClusterArn") # type: ignore[misc]
     @builtins.classmethod
     def from_cluster_arn(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         cluster_arn: builtins.str,
     ) -> ICluster:
         '''(experimental) Reference an existing cluster, defined outside of the CDK code, by name.
 
         :param scope: -
         :param id: -
         :param cluster_arn: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0fc7f5a603e4a4a7570b1cb9dd88e7dc03e0e3a033edb8431d1c192ea70e3d31)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument cluster_arn", value=cluster_arn, expected_type=type_hints["cluster_arn"])
         return typing.cast(ICluster, jsii.sinvoke(cls, "fromClusterArn", [scope, id, cluster_arn]))
 
     @jsii.member(jsii_name="addUser")
     def add_user(self, *usernames: builtins.str) -> None:
         '''(experimental) A list of usersnames to register with the cluster.
 
         The password will automatically be generated using Secrets
@@ -1825,261 +1614,116 @@
 
         Must be using the SASL/SCRAM authentication mechanism.
 
         :param usernames: - username(s) to register with the cluster.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__086a8d99e45ecd0f3befc0016a11c7cd032f40be57774b5485d2c4cf9efbda59)
-            check_type(argname="argument usernames", value=usernames, expected_type=typing.Tuple[type_hints["usernames"], ...]) # pyright: ignore [reportGeneralTypeIssues]
         return typing.cast(None, jsii.invoke(self, "addUser", [*usernames]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="bootstrapBrokers")
     def bootstrap_brokers(self) -> builtins.str:
         '''(experimental) Get the list of brokers that a client application can use to bootstrap.
 
         Uses a Custom Resource to make an API call to ``getBootstrapBrokers`` using the Javascript SDK
 
         :return: - A string containing one or more hostname:port pairs.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "bootstrapBrokers"))
 
-    @builtins.property
-    @jsii.member(jsii_name="bootstrapBrokersSaslIam")
-    def bootstrap_brokers_sasl_iam(self) -> builtins.str:
-        '''(experimental) Get the list of brokers that a SASL/IAM authenticated client application can use to bootstrap.
-
-        Uses a Custom Resource to make an API call to ``getBootstrapBrokers`` using the Javascript SDK
-
-        :return: - A string containing one or more DNS names (or IP) and TLS port pairs.
-
-        :stability: experimental
-        '''
-        return typing.cast(builtins.str, jsii.get(self, "bootstrapBrokersSaslIam"))
-
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="bootstrapBrokersSaslScram")
     def bootstrap_brokers_sasl_scram(self) -> builtins.str:
         '''(experimental) Get the list of brokers that a SASL/SCRAM authenticated client application can use to bootstrap.
 
         Uses a Custom Resource to make an API call to ``getBootstrapBrokers`` using the Javascript SDK
 
         :return: - A string containing one or more dns name (or IP) and SASL SCRAM port pairs.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "bootstrapBrokersSaslScram"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="bootstrapBrokersTls")
     def bootstrap_brokers_tls(self) -> builtins.str:
         '''(experimental) Get the list of brokers that a TLS authenticated client application can use to bootstrap.
 
         Uses a Custom Resource to make an API call to ``getBootstrapBrokers`` using the Javascript SDK
 
         :return: - A string containing one or more DNS names (or IP) and TLS port pairs.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "bootstrapBrokersTls"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterArn")
     def cluster_arn(self) -> builtins.str:
         '''(experimental) The ARN of cluster.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "clusterArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterName")
     def cluster_name(self) -> builtins.str:
         '''(experimental) The physical name of the cluster.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "clusterName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="connections")
-    def connections(self) -> _aws_cdk_aws_ec2_ceddda9d.Connections:
+    def connections(self) -> aws_cdk.aws_ec2.Connections:
         '''(experimental) Manages connections for the cluster.
 
         :stability: experimental
         '''
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.Connections, jsii.get(self, "connections"))
+        return typing.cast(aws_cdk.aws_ec2.Connections, jsii.get(self, "connections"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="zookeeperConnectionString")
     def zookeeper_connection_string(self) -> builtins.str:
         '''(experimental) Get the ZooKeeper Connection string.
 
         Uses a Custom Resource to make an API call to ``describeCluster`` using the Javascript SDK
 
         :return: - The connection string to use to connect to the Apache ZooKeeper cluster.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "zookeeperConnectionString"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="zookeeperConnectionStringTls")
     def zookeeper_connection_string_tls(self) -> builtins.str:
         '''(experimental) Get the ZooKeeper Connection string for a TLS enabled cluster.
 
         Uses a Custom Resource to make an API call to ``describeCluster`` using the Javascript SDK
 
         :return: - The connection string to use to connect to zookeeper cluster on TLS port.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "zookeeperConnectionStringTls"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="saslScramAuthenticationKey")
-    def sasl_scram_authentication_key(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def sasl_scram_authentication_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) Key used to encrypt SASL/SCRAM users.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], jsii.get(self, "saslScramAuthenticationKey"))
-
-
-@jsii.data_type(
-    jsii_type="@aws-cdk/aws-msk-alpha.SaslTlsAuthProps",
-    jsii_struct_bases=[SaslAuthProps, TlsAuthProps],
-    name_mapping={
-        "iam": "iam",
-        "key": "key",
-        "scram": "scram",
-        "certificate_authorities": "certificateAuthorities",
-    },
-)
-class SaslTlsAuthProps(SaslAuthProps, TlsAuthProps):
-    def __init__(
-        self,
-        *,
-        iam: typing.Optional[builtins.bool] = None,
-        key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-        scram: typing.Optional[builtins.bool] = None,
-        certificate_authorities: typing.Optional[typing.Sequence[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]] = None,
-    ) -> None:
-        '''(experimental) SASL + TLS authentication properties.
-
-        :param iam: (experimental) Enable IAM access control. Default: false
-        :param key: (experimental) KMS Key to encrypt SASL/SCRAM secrets. You must use a customer master key (CMK) when creating users in secrets manager. You cannot use a Secret with Amazon MSK that uses the default Secrets Manager encryption key. Default: - CMK will be created with alias msk/{clusterName}/sasl/scram
-        :param scram: (experimental) Enable SASL/SCRAM authentication. Default: false
-        :param certificate_authorities: (experimental) List of ACM Certificate Authorities to enable TLS authentication. Default: - none
-
-        :stability: experimental
-        :exampleMetadata: infused
-
-        Example::
-
-            import aws_cdk.aws_acmpca as acmpca
-            
-            # vpc: ec2.Vpc
-            
-            cluster = msk.Cluster(self, "Cluster",
-                cluster_name="myCluster",
-                kafka_version=msk.KafkaVersion.V2_8_1,
-                vpc=vpc,
-                encryption_in_transit=msk.EncryptionInTransitConfig(
-                    client_broker=msk.ClientBrokerEncryption.TLS
-                ),
-                client_authentication=msk.ClientAuthentication.sasl_tls(
-                    iam=True,
-                    certificate_authorities=[
-                        acmpca.CertificateAuthority.from_certificate_authority_arn(self, "CertificateAuthority", "arn:aws:acm-pca:us-west-2:1234567890:certificate-authority/11111111-1111-1111-1111-111111111111")
-                    ]
-                )
-            )
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a26cb615593ec2787153e2c44f8002c0d2c4cc00110f82aa3f2d4f8d6666b9b1)
-            check_type(argname="argument iam", value=iam, expected_type=type_hints["iam"])
-            check_type(argname="argument key", value=key, expected_type=type_hints["key"])
-            check_type(argname="argument scram", value=scram, expected_type=type_hints["scram"])
-            check_type(argname="argument certificate_authorities", value=certificate_authorities, expected_type=type_hints["certificate_authorities"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
-        if iam is not None:
-            self._values["iam"] = iam
-        if key is not None:
-            self._values["key"] = key
-        if scram is not None:
-            self._values["scram"] = scram
-        if certificate_authorities is not None:
-            self._values["certificate_authorities"] = certificate_authorities
-
-    @builtins.property
-    def iam(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Enable IAM access control.
-
-        :default: false
-
-        :stability: experimental
-        '''
-        result = self._values.get("iam")
-        return typing.cast(typing.Optional[builtins.bool], result)
-
-    @builtins.property
-    def key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
-        '''(experimental) KMS Key to encrypt SASL/SCRAM secrets.
-
-        You must use a customer master key (CMK) when creating users in secrets manager.
-        You cannot use a Secret with Amazon MSK that uses the default Secrets Manager encryption key.
-
-        :default: - CMK will be created with alias msk/{clusterName}/sasl/scram
-
-        :stability: experimental
-        '''
-        result = self._values.get("key")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
-
-    @builtins.property
-    def scram(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Enable SASL/SCRAM authentication.
-
-        :default: false
-
-        :stability: experimental
-        '''
-        result = self._values.get("scram")
-        return typing.cast(typing.Optional[builtins.bool], result)
-
-    @builtins.property
-    def certificate_authorities(
-        self,
-    ) -> typing.Optional[typing.List[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]]:
-        '''(experimental) List of ACM Certificate Authorities to enable TLS authentication.
-
-        :default: - none
-
-        :stability: experimental
-        '''
-        result = self._values.get("certificate_authorities")
-        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]], result)
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "SaslTlsAuthProps(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], jsii.get(self, "saslScramAuthenticationKey"))
 
 
 __all__ = [
     "BrokerLogging",
     "ClientAuthentication",
     "ClientBrokerEncryption",
     "Cluster",
@@ -2089,150 +1733,11 @@
     "EbsStorageInfo",
     "EncryptionInTransitConfig",
     "ICluster",
     "KafkaVersion",
     "MonitoringConfiguration",
     "S3LoggingConfiguration",
     "SaslAuthProps",
-    "SaslTlsAuthProps",
     "TlsAuthProps",
 ]
 
 publication.publish()
-
-def _typecheckingstub__9ba586b7db9e5dd092a5b8f9676408abd0e8865e17a5980b7acb9ac4b970f225(
-    *,
-    cloudwatch_log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
-    firehose_delivery_stream_name: typing.Optional[builtins.str] = None,
-    s3: typing.Optional[typing.Union[S3LoggingConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a3c843d4de610e7657dc25ae7cbdd2c8bba8b60a980c8877eba757e6e63c7ebd(
-    *,
-    arn: builtins.str,
-    revision: jsii.Number,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__7acb1d0e21413d16efb1d11f4a29cc860b92ac278e0b0187d75e3eb1f71b1492(
-    *,
-    cluster_name: builtins.str,
-    kafka_version: KafkaVersion,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-    client_authentication: typing.Optional[ClientAuthentication] = None,
-    configuration_info: typing.Optional[typing.Union[ClusterConfigurationInfo, typing.Dict[builtins.str, typing.Any]]] = None,
-    ebs_storage_info: typing.Optional[typing.Union[EbsStorageInfo, typing.Dict[builtins.str, typing.Any]]] = None,
-    encryption_in_transit: typing.Optional[typing.Union[EncryptionInTransitConfig, typing.Dict[builtins.str, typing.Any]]] = None,
-    instance_type: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.InstanceType] = None,
-    logging: typing.Optional[typing.Union[BrokerLogging, typing.Dict[builtins.str, typing.Any]]] = None,
-    monitoring: typing.Optional[typing.Union[MonitoringConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
-    number_of_broker_nodes: typing.Optional[jsii.Number] = None,
-    removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-    vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__71f71898e3644c01cacd375914aebc2f51bc973e16dca3550d856073a05c90ee(
-    *,
-    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-    volume_size: typing.Optional[jsii.Number] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__72b66a42c0d765a1bd551981cf4b9d5840e1974336776a8da3877d190634cf50(
-    *,
-    client_broker: typing.Optional[ClientBrokerEncryption] = None,
-    enable_in_cluster: typing.Optional[builtins.bool] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e717a461a7dfd2af4c0ea436fee0dcfb2c9d05e9d05e0ff37e25c47c088b68ff(
-    version: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__af85a63aa3f07c68569eb1f6e9732a882ddeb2b7738ae8b80717edf2c96ef123(
-    *,
-    cluster_monitoring_level: typing.Optional[ClusterMonitoringLevel] = None,
-    enable_prometheus_jmx_exporter: typing.Optional[builtins.bool] = None,
-    enable_prometheus_node_exporter: typing.Optional[builtins.bool] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__51fbd5191484562bb80360937520b2fcdc78a672c23d4c600aff0554ad23aa62(
-    *,
-    bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
-    prefix: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__f186e6270f30759471573a6fdea8241e1a52ec3ddb6f61ac669172717e5a8ea6(
-    *,
-    iam: typing.Optional[builtins.bool] = None,
-    key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-    scram: typing.Optional[builtins.bool] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e699112e7fd831ecbdb6721274774f9c6ca4c3a0a7bee752f311fcbdf1e3eb25(
-    *,
-    certificate_authorities: typing.Optional[typing.Sequence[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__915d701802577130bfeeac000a90d2329d756ddabd799173074e0b31599dc1da(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    cluster_name: builtins.str,
-    kafka_version: KafkaVersion,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-    client_authentication: typing.Optional[ClientAuthentication] = None,
-    configuration_info: typing.Optional[typing.Union[ClusterConfigurationInfo, typing.Dict[builtins.str, typing.Any]]] = None,
-    ebs_storage_info: typing.Optional[typing.Union[EbsStorageInfo, typing.Dict[builtins.str, typing.Any]]] = None,
-    encryption_in_transit: typing.Optional[typing.Union[EncryptionInTransitConfig, typing.Dict[builtins.str, typing.Any]]] = None,
-    instance_type: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.InstanceType] = None,
-    logging: typing.Optional[typing.Union[BrokerLogging, typing.Dict[builtins.str, typing.Any]]] = None,
-    monitoring: typing.Optional[typing.Union[MonitoringConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
-    number_of_broker_nodes: typing.Optional[jsii.Number] = None,
-    removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-    vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0fc7f5a603e4a4a7570b1cb9dd88e7dc03e0e3a033edb8431d1c192ea70e3d31(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    cluster_arn: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__086a8d99e45ecd0f3befc0016a11c7cd032f40be57774b5485d2c4cf9efbda59(
-    *usernames: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a26cb615593ec2787153e2c44f8002c0d2c4cc00110f82aa3f2d4f8d6666b9b1(
-    *,
-    iam: typing.Optional[builtins.bool] = None,
-    key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-    scram: typing.Optional[builtins.bool] = None,
-    certificate_authorities: typing.Optional[typing.Sequence[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
```

