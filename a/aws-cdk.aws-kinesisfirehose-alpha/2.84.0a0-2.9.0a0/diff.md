# Comparing `tmp/aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0.tar.gz` & `tmp/aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/aws-kinesisfirehose-alpha/dist/python/aws-cdk.aws-kinesisfirehose-alpha-2.", last modified: Tue Jun 13 23:46:47 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-kinesisfirehose/dist/python/aws-cdk.aws-kinesisfirehose-alp", last modified: Wed Jan 26 11:22:05 2022, max compression
```

## Comparing `aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0.tar` & `aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:37.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:37.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 23:46:37.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    25354 2023-06-13 23:46:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24337 2023-06-13 23:46:37.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:37.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:46:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1926 2023-06-13 23:46:37.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/
--rw-r--r--   0 root         (0) root         (0)   156073 2023-06-13 23:46:37.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      457 2023-06-13 23:46:37.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72561 2023-06-13 23:46:37.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/aws-kinesisfirehose-alpha@2.84.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:37.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25354 2023-06-13 23:46:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      611 2023-06-13 23:46:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-13 23:46:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:46:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    27613 2022-01-26 11:22:05.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    26629 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:05.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1851 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/
+-rw-r--r--   0 root         (0) root         (0)   134580 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      421 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70811 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/aws-kinesisfirehose-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    27613 2022-01-26 11:22:05.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      610 2022-01-26 11:22:05.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:05.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:05.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:05.000000 aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/LICENSE` & `aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/LICENSE`

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

### Comparing `aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/PKG-INFO` & `aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-kinesisfirehose-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::KinesisFirehose
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
 
 # Amazon Kinesis Data Firehose Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -44,15 +44,15 @@
 [Amazon Kinesis Data Firehose](https://docs.aws.amazon.com/firehose/latest/dev/what-is-this-service.html)
 is a service for fully-managed delivery of real-time streaming data to storage services
 such as Amazon S3, Amazon Redshift, Amazon Elasticsearch, Splunk, or any custom HTTP
 endpoint or third-party services such as Datadog, Dynatrace, LogicMonitor, MongoDB, New
 Relic, and Sumo Logic.
 
 Kinesis Data Firehose delivery streams are distinguished from Kinesis data streams in
-their models of consumption. Whereas consumers read from a data stream by actively pulling
+their models of consumtpion. Whereas consumers read from a data stream by actively pulling
 data from the stream, a delivery stream pushes data to its destination on a regular
 cadence. This means that data streams are intended to have consumers that do on-demand
 processing, like AWS Lambda or Amazon EC2. On the other hand, delivery streams are
 intended to have destinations that are sources for offline processing and analytics, such
 as Amazon S3 and Amazon Redshift.
 
 This module is part of the [AWS Cloud Development Kit](https://github.com/aws/aws-cdk)
@@ -99,16 +99,16 @@
     source_stream=source_stream,
     destinations=[destination]
 )
 ```
 
 ### Direct Put
 
-Data must be provided via "direct put", ie., by using a `PutRecord` or
-`PutRecordBatch` API call. There are a number of ways of doing so, such as:
+Data must be provided via "direct put", ie., by using a `PutRecord` or `PutRecordBatch` API call. There are a number of ways of doing
+so, such as:
 
 * Kinesis Agent: a standalone Java application that monitors and delivers files while
   handling file rotation, checkpointing, and retries. See: [Writing to Kinesis Data Firehose Using Kinesis Agent](https://docs.aws.amazon.com/firehose/latest/dev/writing-with-agents.html)
   in the *Kinesis Data Firehose Developer Guide*.
 * AWS SDK: a general purpose solution that allows you to deliver data to a delivery stream
   from anywhere using Java, .NET, Node.js, Python, or Ruby. See: [Writing to Kinesis Data Firehose Using the AWS SDK](https://docs.aws.amazon.com/firehose/latest/dev/writing-with-sdk.html)
   in the *Kinesis Data Firehose Developer Guide*.
@@ -135,100 +135,99 @@
 s3_destination = destinations.S3Bucket(bucket)
 
 firehose.DeliveryStream(self, "Delivery Stream",
     destinations=[s3_destination]
 )
 ```
 
-The S3 destination also supports custom dynamic prefixes. `dataOutputPrefix`
-will be used for files successfully delivered to S3. `errorOutputPrefix` will be added to
-failed records before writing them to S3.
+The S3 destination also supports custom dynamic prefixes. `prefix` will be used for files
+successfully delivered to S3. `errorOutputPrefix` will be added to failed records before
+writing them to S3.
 
 ```python
 # bucket: s3.Bucket
 
 s3_destination = destinations.S3Bucket(bucket,
     data_output_prefix="myFirehose/DeliveredYear=!{timestamp:yyyy}/anyMonth/rand=!{firehose:random-string}",
     error_output_prefix="myFirehoseFailures/!{firehose:error-output-type}/!{timestamp:yyyy}/anyMonth/!{timestamp:dd}"
 )
 ```
 
-See: [Custom S3 Prefixes](https://docs.aws.amazon.com/firehose/latest/dev/s3-prefixes.html)
-in the *Kinesis Data Firehose Developer Guide*.
+See: [Custom S3 Prefixes](https://docs.aws.amazon.com/firehose/latest/dev/s3-prefixes.html) in the *Kinesis Data Firehose Developer Guide*.
 
 ## Server-side Encryption
 
 Enabling server-side encryption (SSE) requires Kinesis Data Firehose to encrypt all data
 sent to delivery stream when it is stored at rest. This means that data is encrypted
 before being written to the service's internal storage layer and decrypted after it is
 received from the internal storage layer. The service manages keys and cryptographic
 operations so that sources and destinations do not need to, as the data is encrypted and
-decrypted at the boundaries of the service (i.e., before the data is delivered to a
+decrypted at the boundaries of the service (ie., before the data is delivered to a
 destination). By default, delivery streams do not have SSE enabled.
 
-The Key Management Service keys (KMS keys) used for SSE can either be AWS-owned or
-customer-managed. AWS-owned KMS keys are created, owned and managed by AWS for use in
-multiple AWS accounts. As a customer, you cannot view, use, track, or manage these keys,
-and you are not charged for their use. On the other hand, customer-managed KMS keys are
-created and owned within your account and managed entirely by you. As a customer, you are
-responsible for managing access, rotation, aliases, and deletion for these keys, and you
-are changed for their use.
-
-See: [AWS KMS keys](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#kms_keys)
+The Key Management Service (KMS) Customer Managed Key (CMK) used for SSE can either be
+AWS-owned or customer-managed. AWS-owned CMKs are keys that an AWS service (in this case
+Kinesis Data Firehose) owns and manages for use in multiple AWS accounts. As a customer,
+you cannot view, use, track, or manage these keys, and you are not charged for their
+use. On the other hand, customer-managed CMKs are keys that are created and owned within
+your account and managed entirely by you. As a customer, you are responsible for managing
+access, rotation, aliases, and deletion for these keys, and you are changed for their
+use. See: [Customer master keys](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#master_keys)
 in the *KMS Developer Guide*.
 
 ```python
 # destination: firehose.IDestination
-# SSE with an customer-managed key that is explicitly specified
+# SSE with an customer-managed CMK that is explicitly specified
 # key: kms.Key
 
 
-# SSE with an AWS-owned key
+# SSE with an AWS-owned CMK
 firehose.DeliveryStream(self, "Delivery Stream AWS Owned",
     encryption=firehose.StreamEncryption.AWS_OWNED,
     destinations=[destination]
 )
-# SSE with an customer-managed key that is created automatically by the CDK
+# SSE with an customer-managed CMK that is created automatically by the CDK
 firehose.DeliveryStream(self, "Delivery Stream Implicit Customer Managed",
     encryption=firehose.StreamEncryption.CUSTOMER_MANAGED,
     destinations=[destination]
 )
 firehose.DeliveryStream(self, "Delivery Stream Explicit Customer Managed",
     encryption_key=key,
     destinations=[destination]
 )
 ```
 
-See: [Data Protection](https://docs.aws.amazon.com/firehose/latest/dev/encryption.html)
-in the *Kinesis Data Firehose Developer Guide*.
+See: [Data Protection](https://docs.aws.amazon.com/firehose/latest/dev/encryption.html) in
+the *Kinesis Data Firehose Developer Guide*.
 
 ## Monitoring
 
 Kinesis Data Firehose is integrated with CloudWatch, so you can monitor the performance of
 your delivery streams via logs and metrics.
 
 ### Logs
 
 Kinesis Data Firehose will send logs to CloudWatch when data transformation or data
 delivery fails. The CDK will enable logging by default and create a CloudWatch LogGroup
 and LogStream for your Delivery Stream.
 
-When you create a destination, you can specify a log group. In this log group, The CDK
-will create log streams where log events will be sent:
+You can provide a specific log group to specify where the CDK will create the log streams
+where log events will be sent:
 
 ```python
 import aws_cdk.aws_logs as logs
 # bucket: s3.Bucket
 
+# destination: firehose.IDestination
+
 
 log_group = logs.LogGroup(self, "Log Group")
 destination = destinations.S3Bucket(bucket,
     log_group=log_group
 )
-
 firehose.DeliveryStream(self, "Delivery Stream",
     destinations=[destination]
 )
 ```
 
 Logging can also be disabled:
 
@@ -261,15 +260,14 @@
 such as `metricIncomingBytes`, and `metricIncomingRecords` (see [`IDeliveryStream`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-kinesisfirehose.IDeliveryStream.html)
 for a full list). CDK also provides a generic `metric` method that can be used to produce
 metric configurations for any metric provided by Kinesis Data Firehose; the configurations
 are pre-populated with the correct dimensions for the delivery stream.
 
 ```python
 import aws_cdk.aws_cloudwatch as cloudwatch
-
 # delivery_stream: firehose.DeliveryStream
 
 
 # Alarm that triggers when the per-second average of incoming bytes exceeds 90% of the current service limit
 incoming_bytes_percent_of_limit = cloudwatch.MathExpression(
     expression="incomingBytes / 300 / bytePerSecLimit",
     using_metrics={
@@ -331,21 +329,20 @@
 ```
 
 See: [Data Delivery Frequency](https://docs.aws.amazon.com/firehose/latest/dev/basic-deliver.html#frequency)
 in the *Kinesis Data Firehose Developer Guide*.
 
 ## Destination Encryption
 
-Your data can be automatically encrypted when it is delivered to S3 as a final or an
-intermediary/backup destination. Kinesis Data Firehose supports Amazon S3 server-side
-encryption with AWS Key Management Service (AWS KMS) for encrypting delivered data in
-Amazon S3. You can choose to not encrypt the data or to encrypt with a key from the list
-of AWS KMS keys that you own. For more information,
-see [Protecting Data Using Server-Side Encryption with AWS KMS–Managed Keys (SSE-KMS)](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingKMSEncryption.html).
-Data is not encrypted by default.
+Your data can be automatically encrypted when it is delivered to S3 as a final or
+an intermediary/backup destination. Kinesis Data Firehose supports Amazon S3 server-side
+encryption with AWS Key Management Service (AWS KMS) for encrypting delivered data
+in Amazon S3. You can choose to not encrypt the data or to encrypt with a key from
+the list of AWS KMS keys that you own. For more information, see [Protecting Data
+Using Server-Side Encryption with AWS KMS–Managed Keys (SSE-KMS)](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingKMSEncryption.html). Data is not encrypted by default.
 
 ```python
 # bucket: s3.Bucket
 # key: kms.Key
 
 destination = destinations.S3Bucket(bucket,
     encryption_key=key
@@ -353,18 +350,18 @@
 firehose.DeliveryStream(self, "Delivery Stream",
     destinations=[destination]
 )
 ```
 
 ## Backup
 
-A delivery stream can be configured to back up data to S3 that it attempted to deliver to
+A delivery stream can be configured to backup data to S3 that it attempted to deliver to
 the configured destination. Backed up data can be all the data that the delivery stream
 attempted to deliver or just data that it failed to deliver (Redshift and S3 destinations
-can only back up all data). CDK can create a new S3 bucket where it will back up data, or
+can only backup all data). CDK can create a new S3 bucket where it will back up data or
 you can provide a bucket where data will be backed up. You can also provide a prefix under
 which your backed-up data will be placed within the bucket. By default, source data is not
 backed up to S3.
 
 ```python
 # Enable backup of all source records (to an S3 bucket created by CDK).
 # bucket: s3.Bucket
@@ -423,26 +420,25 @@
 
 * `recordId` -- the ID of the input record that corresponds the results.
 * `result` -- the status of the transformation of the record: "Ok" (success), "Dropped"
   (not processed intentionally), or "ProcessingFailed" (not processed due to an error).
 * `data` -- the transformed data, Base64-encoded.
 
 The data is buffered up to 1 minute and up to 3 MiB by default before being sent to the
-function, but can be configured using `bufferInterval` and `bufferSize`
-in the processor configuration (see: [Buffering](#buffering)). If the function invocation
-fails due to a network timeout or because of hitting an invocation limit, the invocation
-is retried 3 times by default, but can be configured using `retries` in the processor
-configuration.
+function, but can be configured using `bufferInterval` and `bufferSize` in the processor
+configuration (see: [Buffering](#buffering)). If the function invocation fails due to a
+network timeout or because of hitting an invocation limit, the invocation is retried 3
+times by default, but can be configured using `retries` in the processor configuration.
 
 ```python
 # bucket: s3.Bucket
 # Provide a Lambda function that will transform records before delivery, with custom
 # buffering and retry configuration
 lambda_function = lambda_.Function(self, "Processor",
-    runtime=lambda_.Runtime.NODEJS_14_X,
+    runtime=lambda_.Runtime.NODEJS_12_X,
     handler="index.handler",
     code=lambda_.Code.from_asset(path.join(__dirname, "process-records"))
 )
 lambda_processor = firehose.LambdaFunctionProcessor(lambda_function,
     buffer_interval=Duration.minutes(5),
     buffer_size=Size.mebibytes(5),
     retries=5
@@ -524,14 +520,89 @@
         )
     )]
 )
 
 app.synth()
 ```
 
+!cdk-integ pragma:ignore-assets
+
+```python
+import path as path
+import aws_cdk.aws_kinesisfirehose_alpha as firehose
+import aws_cdk.aws_kms as kms
+import aws_cdk.aws_lambda_nodejs as lambdanodejs
+import aws_cdk.aws_logs as logs
+import aws_cdk.aws_s3 as s3
+import aws_cdk as cdk
+import aws_cdk.aws_kinesisfirehose_destinations_alpha as destinations
+
+app = cdk.App()
+
+stack = cdk.Stack(app, "aws-cdk-firehose-delivery-stream-s3-all-properties")
+
+bucket = s3.Bucket(stack, "Bucket",
+    removal_policy=cdk.RemovalPolicy.DESTROY,
+    auto_delete_objects=True
+)
+
+backup_bucket = s3.Bucket(stack, "BackupBucket",
+    removal_policy=cdk.RemovalPolicy.DESTROY,
+    auto_delete_objects=True
+)
+log_group = logs.LogGroup(stack, "LogGroup",
+    removal_policy=cdk.RemovalPolicy.DESTROY
+)
+
+data_processor_function = lambdanodejs.NodejsFunction(stack, "DataProcessorFunction",
+    entry=path.join(__dirname, "lambda-data-processor.js"),
+    timeout=cdk.Duration.minutes(1)
+)
+
+processor = firehose.LambdaFunctionProcessor(data_processor_function,
+    buffer_interval=cdk.Duration.seconds(60),
+    buffer_size=cdk.Size.mebibytes(1),
+    retries=1
+)
+
+key = kms.Key(stack, "Key",
+    removal_policy=cdk.RemovalPolicy.DESTROY
+)
+
+backup_key = kms.Key(stack, "BackupKey",
+    removal_policy=cdk.RemovalPolicy.DESTROY
+)
+
+firehose.DeliveryStream(stack, "Delivery Stream",
+    destinations=[destinations.S3Bucket(bucket,
+        logging=True,
+        log_group=log_group,
+        processor=processor,
+        compression=destinations.Compression.GZIP,
+        data_output_prefix="regularPrefix",
+        error_output_prefix="errorPrefix",
+        buffering_interval=cdk.Duration.seconds(60),
+        buffering_size=cdk.Size.mebibytes(1),
+        encryption_key=key,
+        s3_backup=destinations.DestinationS3BackupProps(
+            mode=destinations.BackupMode.ALL,
+            bucket=backup_bucket,
+            compression=destinations.Compression.ZIP,
+            data_output_prefix="backupPrefix",
+            error_output_prefix="backupErrorPrefix",
+            buffering_interval=cdk.Duration.seconds(60),
+            buffering_size=cdk.Size.mebibytes(1),
+            encryption_key=backup_key
+        )
+    )]
+)
+
+app.synth()
+```
+
 See: [Data Transformation](https://docs.aws.amazon.com/firehose/latest/dev/data-transformation.html)
 in the *Kinesis Data Firehose Developer Guide*.
 
 ## Specifying an IAM role
 
 The DeliveryStream class automatically creates IAM service roles with all the minimum
 necessary permissions for Kinesis Data Firehose to access the resources referenced by your
@@ -570,15 +641,15 @@
 in the *Kinesis Data Firehose Developer Guide*.
 
 ## Granting application access to a delivery stream
 
 IAM roles, users or groups which need to be able to work with delivery streams should be
 granted IAM permissions.
 
-Any object that implements the `IGrantable` interface (i.e., has an associated principal)
+Any object that implements the `IGrantable` interface (ie., has an associated principal)
 can be granted permissions to a delivery stream by calling:
 
 * `grantPutRecords(principal)` - grants the principal the ability to put records onto the
   delivery stream
 * `grant(principal, ...actions)` - grants the principal permission to a custom set of
   actions
 
@@ -587,16 +658,15 @@
 # delivery_stream: firehose.DeliveryStream
 lambda_role = iam.Role(self, "Role",
     assumed_by=iam.ServicePrincipal("lambda.amazonaws.com")
 )
 delivery_stream.grant_put_records(lambda_role)
 ```
 
-The following write permissions are provided to a service principal by the
-`grantPutRecords()` method:
+The following write permissions are provided to a service principal by the `grantPutRecords()` method:
 
 * `firehose:PutRecord`
 * `firehose:PutRecordBatch`
 
 ## Granting a delivery stream access to a resource
 
 Conversely to the above, Kinesis Data Firehose requires permissions in order for delivery
@@ -618,7 +688,9 @@
 ```
 
 ## Multiple destinations
 
 Though the delivery stream allows specifying an array of destinations, only one
 destination per delivery stream is currently allowed. This limitation is enforced at CDK
 synthesis time and will throw an error.
+
+
```

### Comparing `aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/README.md` & `aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 [Amazon Kinesis Data Firehose](https://docs.aws.amazon.com/firehose/latest/dev/what-is-this-service.html)
 is a service for fully-managed delivery of real-time streaming data to storage services
 such as Amazon S3, Amazon Redshift, Amazon Elasticsearch, Splunk, or any custom HTTP
 endpoint or third-party services such as Datadog, Dynatrace, LogicMonitor, MongoDB, New
 Relic, and Sumo Logic.
 
 Kinesis Data Firehose delivery streams are distinguished from Kinesis data streams in
-their models of consumption. Whereas consumers read from a data stream by actively pulling
+their models of consumtpion. Whereas consumers read from a data stream by actively pulling
 data from the stream, a delivery stream pushes data to its destination on a regular
 cadence. This means that data streams are intended to have consumers that do on-demand
 processing, like AWS Lambda or Amazon EC2. On the other hand, delivery streams are
 intended to have destinations that are sources for offline processing and analytics, such
 as Amazon S3 and Amazon Redshift.
 
 This module is part of the [AWS Cloud Development Kit](https://github.com/aws/aws-cdk)
@@ -72,16 +72,16 @@
     source_stream=source_stream,
     destinations=[destination]
 )
 ```
 
 ### Direct Put
 
-Data must be provided via "direct put", ie., by using a `PutRecord` or
-`PutRecordBatch` API call. There are a number of ways of doing so, such as:
+Data must be provided via "direct put", ie., by using a `PutRecord` or `PutRecordBatch` API call. There are a number of ways of doing
+so, such as:
 
 * Kinesis Agent: a standalone Java application that monitors and delivers files while
   handling file rotation, checkpointing, and retries. See: [Writing to Kinesis Data Firehose Using Kinesis Agent](https://docs.aws.amazon.com/firehose/latest/dev/writing-with-agents.html)
   in the *Kinesis Data Firehose Developer Guide*.
 * AWS SDK: a general purpose solution that allows you to deliver data to a delivery stream
   from anywhere using Java, .NET, Node.js, Python, or Ruby. See: [Writing to Kinesis Data Firehose Using the AWS SDK](https://docs.aws.amazon.com/firehose/latest/dev/writing-with-sdk.html)
   in the *Kinesis Data Firehose Developer Guide*.
@@ -108,100 +108,99 @@
 s3_destination = destinations.S3Bucket(bucket)
 
 firehose.DeliveryStream(self, "Delivery Stream",
     destinations=[s3_destination]
 )
 ```
 
-The S3 destination also supports custom dynamic prefixes. `dataOutputPrefix`
-will be used for files successfully delivered to S3. `errorOutputPrefix` will be added to
-failed records before writing them to S3.
+The S3 destination also supports custom dynamic prefixes. `prefix` will be used for files
+successfully delivered to S3. `errorOutputPrefix` will be added to failed records before
+writing them to S3.
 
 ```python
 # bucket: s3.Bucket
 
 s3_destination = destinations.S3Bucket(bucket,
     data_output_prefix="myFirehose/DeliveredYear=!{timestamp:yyyy}/anyMonth/rand=!{firehose:random-string}",
     error_output_prefix="myFirehoseFailures/!{firehose:error-output-type}/!{timestamp:yyyy}/anyMonth/!{timestamp:dd}"
 )
 ```
 
-See: [Custom S3 Prefixes](https://docs.aws.amazon.com/firehose/latest/dev/s3-prefixes.html)
-in the *Kinesis Data Firehose Developer Guide*.
+See: [Custom S3 Prefixes](https://docs.aws.amazon.com/firehose/latest/dev/s3-prefixes.html) in the *Kinesis Data Firehose Developer Guide*.
 
 ## Server-side Encryption
 
 Enabling server-side encryption (SSE) requires Kinesis Data Firehose to encrypt all data
 sent to delivery stream when it is stored at rest. This means that data is encrypted
 before being written to the service's internal storage layer and decrypted after it is
 received from the internal storage layer. The service manages keys and cryptographic
 operations so that sources and destinations do not need to, as the data is encrypted and
-decrypted at the boundaries of the service (i.e., before the data is delivered to a
+decrypted at the boundaries of the service (ie., before the data is delivered to a
 destination). By default, delivery streams do not have SSE enabled.
 
-The Key Management Service keys (KMS keys) used for SSE can either be AWS-owned or
-customer-managed. AWS-owned KMS keys are created, owned and managed by AWS for use in
-multiple AWS accounts. As a customer, you cannot view, use, track, or manage these keys,
-and you are not charged for their use. On the other hand, customer-managed KMS keys are
-created and owned within your account and managed entirely by you. As a customer, you are
-responsible for managing access, rotation, aliases, and deletion for these keys, and you
-are changed for their use.
-
-See: [AWS KMS keys](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#kms_keys)
+The Key Management Service (KMS) Customer Managed Key (CMK) used for SSE can either be
+AWS-owned or customer-managed. AWS-owned CMKs are keys that an AWS service (in this case
+Kinesis Data Firehose) owns and manages for use in multiple AWS accounts. As a customer,
+you cannot view, use, track, or manage these keys, and you are not charged for their
+use. On the other hand, customer-managed CMKs are keys that are created and owned within
+your account and managed entirely by you. As a customer, you are responsible for managing
+access, rotation, aliases, and deletion for these keys, and you are changed for their
+use. See: [Customer master keys](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#master_keys)
 in the *KMS Developer Guide*.
 
 ```python
 # destination: firehose.IDestination
-# SSE with an customer-managed key that is explicitly specified
+# SSE with an customer-managed CMK that is explicitly specified
 # key: kms.Key
 
 
-# SSE with an AWS-owned key
+# SSE with an AWS-owned CMK
 firehose.DeliveryStream(self, "Delivery Stream AWS Owned",
     encryption=firehose.StreamEncryption.AWS_OWNED,
     destinations=[destination]
 )
-# SSE with an customer-managed key that is created automatically by the CDK
+# SSE with an customer-managed CMK that is created automatically by the CDK
 firehose.DeliveryStream(self, "Delivery Stream Implicit Customer Managed",
     encryption=firehose.StreamEncryption.CUSTOMER_MANAGED,
     destinations=[destination]
 )
 firehose.DeliveryStream(self, "Delivery Stream Explicit Customer Managed",
     encryption_key=key,
     destinations=[destination]
 )
 ```
 
-See: [Data Protection](https://docs.aws.amazon.com/firehose/latest/dev/encryption.html)
-in the *Kinesis Data Firehose Developer Guide*.
+See: [Data Protection](https://docs.aws.amazon.com/firehose/latest/dev/encryption.html) in
+the *Kinesis Data Firehose Developer Guide*.
 
 ## Monitoring
 
 Kinesis Data Firehose is integrated with CloudWatch, so you can monitor the performance of
 your delivery streams via logs and metrics.
 
 ### Logs
 
 Kinesis Data Firehose will send logs to CloudWatch when data transformation or data
 delivery fails. The CDK will enable logging by default and create a CloudWatch LogGroup
 and LogStream for your Delivery Stream.
 
-When you create a destination, you can specify a log group. In this log group, The CDK
-will create log streams where log events will be sent:
+You can provide a specific log group to specify where the CDK will create the log streams
+where log events will be sent:
 
 ```python
 import aws_cdk.aws_logs as logs
 # bucket: s3.Bucket
 
+# destination: firehose.IDestination
+
 
 log_group = logs.LogGroup(self, "Log Group")
 destination = destinations.S3Bucket(bucket,
     log_group=log_group
 )
-
 firehose.DeliveryStream(self, "Delivery Stream",
     destinations=[destination]
 )
 ```
 
 Logging can also be disabled:
 
@@ -234,15 +233,14 @@
 such as `metricIncomingBytes`, and `metricIncomingRecords` (see [`IDeliveryStream`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-kinesisfirehose.IDeliveryStream.html)
 for a full list). CDK also provides a generic `metric` method that can be used to produce
 metric configurations for any metric provided by Kinesis Data Firehose; the configurations
 are pre-populated with the correct dimensions for the delivery stream.
 
 ```python
 import aws_cdk.aws_cloudwatch as cloudwatch
-
 # delivery_stream: firehose.DeliveryStream
 
 
 # Alarm that triggers when the per-second average of incoming bytes exceeds 90% of the current service limit
 incoming_bytes_percent_of_limit = cloudwatch.MathExpression(
     expression="incomingBytes / 300 / bytePerSecLimit",
     using_metrics={
@@ -304,21 +302,20 @@
 ```
 
 See: [Data Delivery Frequency](https://docs.aws.amazon.com/firehose/latest/dev/basic-deliver.html#frequency)
 in the *Kinesis Data Firehose Developer Guide*.
 
 ## Destination Encryption
 
-Your data can be automatically encrypted when it is delivered to S3 as a final or an
-intermediary/backup destination. Kinesis Data Firehose supports Amazon S3 server-side
-encryption with AWS Key Management Service (AWS KMS) for encrypting delivered data in
-Amazon S3. You can choose to not encrypt the data or to encrypt with a key from the list
-of AWS KMS keys that you own. For more information,
-see [Protecting Data Using Server-Side Encryption with AWS KMS–Managed Keys (SSE-KMS)](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingKMSEncryption.html).
-Data is not encrypted by default.
+Your data can be automatically encrypted when it is delivered to S3 as a final or
+an intermediary/backup destination. Kinesis Data Firehose supports Amazon S3 server-side
+encryption with AWS Key Management Service (AWS KMS) for encrypting delivered data
+in Amazon S3. You can choose to not encrypt the data or to encrypt with a key from
+the list of AWS KMS keys that you own. For more information, see [Protecting Data
+Using Server-Side Encryption with AWS KMS–Managed Keys (SSE-KMS)](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingKMSEncryption.html). Data is not encrypted by default.
 
 ```python
 # bucket: s3.Bucket
 # key: kms.Key
 
 destination = destinations.S3Bucket(bucket,
     encryption_key=key
@@ -326,18 +323,18 @@
 firehose.DeliveryStream(self, "Delivery Stream",
     destinations=[destination]
 )
 ```
 
 ## Backup
 
-A delivery stream can be configured to back up data to S3 that it attempted to deliver to
+A delivery stream can be configured to backup data to S3 that it attempted to deliver to
 the configured destination. Backed up data can be all the data that the delivery stream
 attempted to deliver or just data that it failed to deliver (Redshift and S3 destinations
-can only back up all data). CDK can create a new S3 bucket where it will back up data, or
+can only backup all data). CDK can create a new S3 bucket where it will back up data or
 you can provide a bucket where data will be backed up. You can also provide a prefix under
 which your backed-up data will be placed within the bucket. By default, source data is not
 backed up to S3.
 
 ```python
 # Enable backup of all source records (to an S3 bucket created by CDK).
 # bucket: s3.Bucket
@@ -396,26 +393,25 @@
 
 * `recordId` -- the ID of the input record that corresponds the results.
 * `result` -- the status of the transformation of the record: "Ok" (success), "Dropped"
   (not processed intentionally), or "ProcessingFailed" (not processed due to an error).
 * `data` -- the transformed data, Base64-encoded.
 
 The data is buffered up to 1 minute and up to 3 MiB by default before being sent to the
-function, but can be configured using `bufferInterval` and `bufferSize`
-in the processor configuration (see: [Buffering](#buffering)). If the function invocation
-fails due to a network timeout or because of hitting an invocation limit, the invocation
-is retried 3 times by default, but can be configured using `retries` in the processor
-configuration.
+function, but can be configured using `bufferInterval` and `bufferSize` in the processor
+configuration (see: [Buffering](#buffering)). If the function invocation fails due to a
+network timeout or because of hitting an invocation limit, the invocation is retried 3
+times by default, but can be configured using `retries` in the processor configuration.
 
 ```python
 # bucket: s3.Bucket
 # Provide a Lambda function that will transform records before delivery, with custom
 # buffering and retry configuration
 lambda_function = lambda_.Function(self, "Processor",
-    runtime=lambda_.Runtime.NODEJS_14_X,
+    runtime=lambda_.Runtime.NODEJS_12_X,
     handler="index.handler",
     code=lambda_.Code.from_asset(path.join(__dirname, "process-records"))
 )
 lambda_processor = firehose.LambdaFunctionProcessor(lambda_function,
     buffer_interval=Duration.minutes(5),
     buffer_size=Size.mebibytes(5),
     retries=5
@@ -497,14 +493,89 @@
         )
     )]
 )
 
 app.synth()
 ```
 
+!cdk-integ pragma:ignore-assets
+
+```python
+import path as path
+import aws_cdk.aws_kinesisfirehose_alpha as firehose
+import aws_cdk.aws_kms as kms
+import aws_cdk.aws_lambda_nodejs as lambdanodejs
+import aws_cdk.aws_logs as logs
+import aws_cdk.aws_s3 as s3
+import aws_cdk as cdk
+import aws_cdk.aws_kinesisfirehose_destinations_alpha as destinations
+
+app = cdk.App()
+
+stack = cdk.Stack(app, "aws-cdk-firehose-delivery-stream-s3-all-properties")
+
+bucket = s3.Bucket(stack, "Bucket",
+    removal_policy=cdk.RemovalPolicy.DESTROY,
+    auto_delete_objects=True
+)
+
+backup_bucket = s3.Bucket(stack, "BackupBucket",
+    removal_policy=cdk.RemovalPolicy.DESTROY,
+    auto_delete_objects=True
+)
+log_group = logs.LogGroup(stack, "LogGroup",
+    removal_policy=cdk.RemovalPolicy.DESTROY
+)
+
+data_processor_function = lambdanodejs.NodejsFunction(stack, "DataProcessorFunction",
+    entry=path.join(__dirname, "lambda-data-processor.js"),
+    timeout=cdk.Duration.minutes(1)
+)
+
+processor = firehose.LambdaFunctionProcessor(data_processor_function,
+    buffer_interval=cdk.Duration.seconds(60),
+    buffer_size=cdk.Size.mebibytes(1),
+    retries=1
+)
+
+key = kms.Key(stack, "Key",
+    removal_policy=cdk.RemovalPolicy.DESTROY
+)
+
+backup_key = kms.Key(stack, "BackupKey",
+    removal_policy=cdk.RemovalPolicy.DESTROY
+)
+
+firehose.DeliveryStream(stack, "Delivery Stream",
+    destinations=[destinations.S3Bucket(bucket,
+        logging=True,
+        log_group=log_group,
+        processor=processor,
+        compression=destinations.Compression.GZIP,
+        data_output_prefix="regularPrefix",
+        error_output_prefix="errorPrefix",
+        buffering_interval=cdk.Duration.seconds(60),
+        buffering_size=cdk.Size.mebibytes(1),
+        encryption_key=key,
+        s3_backup=destinations.DestinationS3BackupProps(
+            mode=destinations.BackupMode.ALL,
+            bucket=backup_bucket,
+            compression=destinations.Compression.ZIP,
+            data_output_prefix="backupPrefix",
+            error_output_prefix="backupErrorPrefix",
+            buffering_interval=cdk.Duration.seconds(60),
+            buffering_size=cdk.Size.mebibytes(1),
+            encryption_key=backup_key
+        )
+    )]
+)
+
+app.synth()
+```
+
 See: [Data Transformation](https://docs.aws.amazon.com/firehose/latest/dev/data-transformation.html)
 in the *Kinesis Data Firehose Developer Guide*.
 
 ## Specifying an IAM role
 
 The DeliveryStream class automatically creates IAM service roles with all the minimum
 necessary permissions for Kinesis Data Firehose to access the resources referenced by your
@@ -543,15 +614,15 @@
 in the *Kinesis Data Firehose Developer Guide*.
 
 ## Granting application access to a delivery stream
 
 IAM roles, users or groups which need to be able to work with delivery streams should be
 granted IAM permissions.
 
-Any object that implements the `IGrantable` interface (i.e., has an associated principal)
+Any object that implements the `IGrantable` interface (ie., has an associated principal)
 can be granted permissions to a delivery stream by calling:
 
 * `grantPutRecords(principal)` - grants the principal the ability to put records onto the
   delivery stream
 * `grant(principal, ...actions)` - grants the principal permission to a custom set of
   actions
 
@@ -560,16 +631,15 @@
 # delivery_stream: firehose.DeliveryStream
 lambda_role = iam.Role(self, "Role",
     assumed_by=iam.ServicePrincipal("lambda.amazonaws.com")
 )
 delivery_stream.grant_put_records(lambda_role)
 ```
 
-The following write permissions are provided to a service principal by the
-`grantPutRecords()` method:
+The following write permissions are provided to a service principal by the `grantPutRecords()` method:
 
 * `firehose:PutRecord`
 * `firehose:PutRecordBatch`
 
 ## Granting a delivery stream access to a resource
 
 Conversely to the above, Kinesis Data Firehose requires permissions in order for delivery
```

### Comparing `aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/setup.py` & `aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-kinesisfirehose-alpha",
-    "version": "2.84.0.a0",
+    "version": "2.9.0.a0",
     "description": "The CDK Construct Library for AWS::KinesisFirehose",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,43 +22,41 @@
     },
     "packages": [
         "aws_cdk.aws_kinesisfirehose_alpha",
         "aws_cdk.aws_kinesisfirehose_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_kinesisfirehose_alpha._jsii": [
-            "aws-kinesisfirehose-alpha@2.84.0-alpha.0.jsii.tgz"
+            "aws-kinesisfirehose-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_kinesisfirehose_alpha": [
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

### Comparing `aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/__init__.py` & `aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [Amazon Kinesis Data Firehose](https://docs.aws.amazon.com/firehose/latest/dev/what-is-this-service.html)
 is a service for fully-managed delivery of real-time streaming data to storage services
 such as Amazon S3, Amazon Redshift, Amazon Elasticsearch, Splunk, or any custom HTTP
 endpoint or third-party services such as Datadog, Dynatrace, LogicMonitor, MongoDB, New
 Relic, and Sumo Logic.
 
 Kinesis Data Firehose delivery streams are distinguished from Kinesis data streams in
-their models of consumption. Whereas consumers read from a data stream by actively pulling
+their models of consumtpion. Whereas consumers read from a data stream by actively pulling
 data from the stream, a delivery stream pushes data to its destination on a regular
 cadence. This means that data streams are intended to have consumers that do on-demand
 processing, like AWS Lambda or Amazon EC2. On the other hand, delivery streams are
 intended to have destinations that are sources for offline processing and analytics, such
 as Amazon S3 and Amazon Redshift.
 
 This module is part of the [AWS Cloud Development Kit](https://github.com/aws/aws-cdk)
@@ -73,16 +73,16 @@
     source_stream=source_stream,
     destinations=[destination]
 )
 ```
 
 ### Direct Put
 
-Data must be provided via "direct put", ie., by using a `PutRecord` or
-`PutRecordBatch` API call. There are a number of ways of doing so, such as:
+Data must be provided via "direct put", ie., by using a `PutRecord` or `PutRecordBatch` API call. There are a number of ways of doing
+so, such as:
 
 * Kinesis Agent: a standalone Java application that monitors and delivers files while
   handling file rotation, checkpointing, and retries. See: [Writing to Kinesis Data Firehose Using Kinesis Agent](https://docs.aws.amazon.com/firehose/latest/dev/writing-with-agents.html)
   in the *Kinesis Data Firehose Developer Guide*.
 * AWS SDK: a general purpose solution that allows you to deliver data to a delivery stream
   from anywhere using Java, .NET, Node.js, Python, or Ruby. See: [Writing to Kinesis Data Firehose Using the AWS SDK](https://docs.aws.amazon.com/firehose/latest/dev/writing-with-sdk.html)
   in the *Kinesis Data Firehose Developer Guide*.
@@ -109,100 +109,99 @@
 s3_destination = destinations.S3Bucket(bucket)
 
 firehose.DeliveryStream(self, "Delivery Stream",
     destinations=[s3_destination]
 )
 ```
 
-The S3 destination also supports custom dynamic prefixes. `dataOutputPrefix`
-will be used for files successfully delivered to S3. `errorOutputPrefix` will be added to
-failed records before writing them to S3.
+The S3 destination also supports custom dynamic prefixes. `prefix` will be used for files
+successfully delivered to S3. `errorOutputPrefix` will be added to failed records before
+writing them to S3.
 
 ```python
 # bucket: s3.Bucket
 
 s3_destination = destinations.S3Bucket(bucket,
     data_output_prefix="myFirehose/DeliveredYear=!{timestamp:yyyy}/anyMonth/rand=!{firehose:random-string}",
     error_output_prefix="myFirehoseFailures/!{firehose:error-output-type}/!{timestamp:yyyy}/anyMonth/!{timestamp:dd}"
 )
 ```
 
-See: [Custom S3 Prefixes](https://docs.aws.amazon.com/firehose/latest/dev/s3-prefixes.html)
-in the *Kinesis Data Firehose Developer Guide*.
+See: [Custom S3 Prefixes](https://docs.aws.amazon.com/firehose/latest/dev/s3-prefixes.html) in the *Kinesis Data Firehose Developer Guide*.
 
 ## Server-side Encryption
 
 Enabling server-side encryption (SSE) requires Kinesis Data Firehose to encrypt all data
 sent to delivery stream when it is stored at rest. This means that data is encrypted
 before being written to the service's internal storage layer and decrypted after it is
 received from the internal storage layer. The service manages keys and cryptographic
 operations so that sources and destinations do not need to, as the data is encrypted and
-decrypted at the boundaries of the service (i.e., before the data is delivered to a
+decrypted at the boundaries of the service (ie., before the data is delivered to a
 destination). By default, delivery streams do not have SSE enabled.
 
-The Key Management Service keys (KMS keys) used for SSE can either be AWS-owned or
-customer-managed. AWS-owned KMS keys are created, owned and managed by AWS for use in
-multiple AWS accounts. As a customer, you cannot view, use, track, or manage these keys,
-and you are not charged for their use. On the other hand, customer-managed KMS keys are
-created and owned within your account and managed entirely by you. As a customer, you are
-responsible for managing access, rotation, aliases, and deletion for these keys, and you
-are changed for their use.
-
-See: [AWS KMS keys](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#kms_keys)
+The Key Management Service (KMS) Customer Managed Key (CMK) used for SSE can either be
+AWS-owned or customer-managed. AWS-owned CMKs are keys that an AWS service (in this case
+Kinesis Data Firehose) owns and manages for use in multiple AWS accounts. As a customer,
+you cannot view, use, track, or manage these keys, and you are not charged for their
+use. On the other hand, customer-managed CMKs are keys that are created and owned within
+your account and managed entirely by you. As a customer, you are responsible for managing
+access, rotation, aliases, and deletion for these keys, and you are changed for their
+use. See: [Customer master keys](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#master_keys)
 in the *KMS Developer Guide*.
 
 ```python
 # destination: firehose.IDestination
-# SSE with an customer-managed key that is explicitly specified
+# SSE with an customer-managed CMK that is explicitly specified
 # key: kms.Key
 
 
-# SSE with an AWS-owned key
+# SSE with an AWS-owned CMK
 firehose.DeliveryStream(self, "Delivery Stream AWS Owned",
     encryption=firehose.StreamEncryption.AWS_OWNED,
     destinations=[destination]
 )
-# SSE with an customer-managed key that is created automatically by the CDK
+# SSE with an customer-managed CMK that is created automatically by the CDK
 firehose.DeliveryStream(self, "Delivery Stream Implicit Customer Managed",
     encryption=firehose.StreamEncryption.CUSTOMER_MANAGED,
     destinations=[destination]
 )
 firehose.DeliveryStream(self, "Delivery Stream Explicit Customer Managed",
     encryption_key=key,
     destinations=[destination]
 )
 ```
 
-See: [Data Protection](https://docs.aws.amazon.com/firehose/latest/dev/encryption.html)
-in the *Kinesis Data Firehose Developer Guide*.
+See: [Data Protection](https://docs.aws.amazon.com/firehose/latest/dev/encryption.html) in
+the *Kinesis Data Firehose Developer Guide*.
 
 ## Monitoring
 
 Kinesis Data Firehose is integrated with CloudWatch, so you can monitor the performance of
 your delivery streams via logs and metrics.
 
 ### Logs
 
 Kinesis Data Firehose will send logs to CloudWatch when data transformation or data
 delivery fails. The CDK will enable logging by default and create a CloudWatch LogGroup
 and LogStream for your Delivery Stream.
 
-When you create a destination, you can specify a log group. In this log group, The CDK
-will create log streams where log events will be sent:
+You can provide a specific log group to specify where the CDK will create the log streams
+where log events will be sent:
 
 ```python
 import aws_cdk.aws_logs as logs
 # bucket: s3.Bucket
 
+# destination: firehose.IDestination
+
 
 log_group = logs.LogGroup(self, "Log Group")
 destination = destinations.S3Bucket(bucket,
     log_group=log_group
 )
-
 firehose.DeliveryStream(self, "Delivery Stream",
     destinations=[destination]
 )
 ```
 
 Logging can also be disabled:
 
@@ -235,15 +234,14 @@
 such as `metricIncomingBytes`, and `metricIncomingRecords` (see [`IDeliveryStream`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-kinesisfirehose.IDeliveryStream.html)
 for a full list). CDK also provides a generic `metric` method that can be used to produce
 metric configurations for any metric provided by Kinesis Data Firehose; the configurations
 are pre-populated with the correct dimensions for the delivery stream.
 
 ```python
 import aws_cdk.aws_cloudwatch as cloudwatch
-
 # delivery_stream: firehose.DeliveryStream
 
 
 # Alarm that triggers when the per-second average of incoming bytes exceeds 90% of the current service limit
 incoming_bytes_percent_of_limit = cloudwatch.MathExpression(
     expression="incomingBytes / 300 / bytePerSecLimit",
     using_metrics={
@@ -305,21 +303,20 @@
 ```
 
 See: [Data Delivery Frequency](https://docs.aws.amazon.com/firehose/latest/dev/basic-deliver.html#frequency)
 in the *Kinesis Data Firehose Developer Guide*.
 
 ## Destination Encryption
 
-Your data can be automatically encrypted when it is delivered to S3 as a final or an
-intermediary/backup destination. Kinesis Data Firehose supports Amazon S3 server-side
-encryption with AWS Key Management Service (AWS KMS) for encrypting delivered data in
-Amazon S3. You can choose to not encrypt the data or to encrypt with a key from the list
-of AWS KMS keys that you own. For more information,
-see [Protecting Data Using Server-Side Encryption with AWS KMS–Managed Keys (SSE-KMS)](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingKMSEncryption.html).
-Data is not encrypted by default.
+Your data can be automatically encrypted when it is delivered to S3 as a final or
+an intermediary/backup destination. Kinesis Data Firehose supports Amazon S3 server-side
+encryption with AWS Key Management Service (AWS KMS) for encrypting delivered data
+in Amazon S3. You can choose to not encrypt the data or to encrypt with a key from
+the list of AWS KMS keys that you own. For more information, see [Protecting Data
+Using Server-Side Encryption with AWS KMS–Managed Keys (SSE-KMS)](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingKMSEncryption.html). Data is not encrypted by default.
 
 ```python
 # bucket: s3.Bucket
 # key: kms.Key
 
 destination = destinations.S3Bucket(bucket,
     encryption_key=key
@@ -327,18 +324,18 @@
 firehose.DeliveryStream(self, "Delivery Stream",
     destinations=[destination]
 )
 ```
 
 ## Backup
 
-A delivery stream can be configured to back up data to S3 that it attempted to deliver to
+A delivery stream can be configured to backup data to S3 that it attempted to deliver to
 the configured destination. Backed up data can be all the data that the delivery stream
 attempted to deliver or just data that it failed to deliver (Redshift and S3 destinations
-can only back up all data). CDK can create a new S3 bucket where it will back up data, or
+can only backup all data). CDK can create a new S3 bucket where it will back up data or
 you can provide a bucket where data will be backed up. You can also provide a prefix under
 which your backed-up data will be placed within the bucket. By default, source data is not
 backed up to S3.
 
 ```python
 # Enable backup of all source records (to an S3 bucket created by CDK).
 # bucket: s3.Bucket
@@ -397,26 +394,25 @@
 
 * `recordId` -- the ID of the input record that corresponds the results.
 * `result` -- the status of the transformation of the record: "Ok" (success), "Dropped"
   (not processed intentionally), or "ProcessingFailed" (not processed due to an error).
 * `data` -- the transformed data, Base64-encoded.
 
 The data is buffered up to 1 minute and up to 3 MiB by default before being sent to the
-function, but can be configured using `bufferInterval` and `bufferSize`
-in the processor configuration (see: [Buffering](#buffering)). If the function invocation
-fails due to a network timeout or because of hitting an invocation limit, the invocation
-is retried 3 times by default, but can be configured using `retries` in the processor
-configuration.
+function, but can be configured using `bufferInterval` and `bufferSize` in the processor
+configuration (see: [Buffering](#buffering)). If the function invocation fails due to a
+network timeout or because of hitting an invocation limit, the invocation is retried 3
+times by default, but can be configured using `retries` in the processor configuration.
 
 ```python
 # bucket: s3.Bucket
 # Provide a Lambda function that will transform records before delivery, with custom
 # buffering and retry configuration
 lambda_function = lambda_.Function(self, "Processor",
-    runtime=lambda_.Runtime.NODEJS_14_X,
+    runtime=lambda_.Runtime.NODEJS_12_X,
     handler="index.handler",
     code=lambda_.Code.from_asset(path.join(__dirname, "process-records"))
 )
 lambda_processor = firehose.LambdaFunctionProcessor(lambda_function,
     buffer_interval=Duration.minutes(5),
     buffer_size=Size.mebibytes(5),
     retries=5
@@ -498,14 +494,89 @@
         )
     )]
 )
 
 app.synth()
 ```
 
+!cdk-integ pragma:ignore-assets
+
+```python
+import path as path
+import aws_cdk.aws_kinesisfirehose_alpha as firehose
+import aws_cdk.aws_kms as kms
+import aws_cdk.aws_lambda_nodejs as lambdanodejs
+import aws_cdk.aws_logs as logs
+import aws_cdk.aws_s3 as s3
+import aws_cdk as cdk
+import aws_cdk.aws_kinesisfirehose_destinations_alpha as destinations
+
+app = cdk.App()
+
+stack = cdk.Stack(app, "aws-cdk-firehose-delivery-stream-s3-all-properties")
+
+bucket = s3.Bucket(stack, "Bucket",
+    removal_policy=cdk.RemovalPolicy.DESTROY,
+    auto_delete_objects=True
+)
+
+backup_bucket = s3.Bucket(stack, "BackupBucket",
+    removal_policy=cdk.RemovalPolicy.DESTROY,
+    auto_delete_objects=True
+)
+log_group = logs.LogGroup(stack, "LogGroup",
+    removal_policy=cdk.RemovalPolicy.DESTROY
+)
+
+data_processor_function = lambdanodejs.NodejsFunction(stack, "DataProcessorFunction",
+    entry=path.join(__dirname, "lambda-data-processor.js"),
+    timeout=cdk.Duration.minutes(1)
+)
+
+processor = firehose.LambdaFunctionProcessor(data_processor_function,
+    buffer_interval=cdk.Duration.seconds(60),
+    buffer_size=cdk.Size.mebibytes(1),
+    retries=1
+)
+
+key = kms.Key(stack, "Key",
+    removal_policy=cdk.RemovalPolicy.DESTROY
+)
+
+backup_key = kms.Key(stack, "BackupKey",
+    removal_policy=cdk.RemovalPolicy.DESTROY
+)
+
+firehose.DeliveryStream(stack, "Delivery Stream",
+    destinations=[destinations.S3Bucket(bucket,
+        logging=True,
+        log_group=log_group,
+        processor=processor,
+        compression=destinations.Compression.GZIP,
+        data_output_prefix="regularPrefix",
+        error_output_prefix="errorPrefix",
+        buffering_interval=cdk.Duration.seconds(60),
+        buffering_size=cdk.Size.mebibytes(1),
+        encryption_key=key,
+        s3_backup=destinations.DestinationS3BackupProps(
+            mode=destinations.BackupMode.ALL,
+            bucket=backup_bucket,
+            compression=destinations.Compression.ZIP,
+            data_output_prefix="backupPrefix",
+            error_output_prefix="backupErrorPrefix",
+            buffering_interval=cdk.Duration.seconds(60),
+            buffering_size=cdk.Size.mebibytes(1),
+            encryption_key=backup_key
+        )
+    )]
+)
+
+app.synth()
+```
+
 See: [Data Transformation](https://docs.aws.amazon.com/firehose/latest/dev/data-transformation.html)
 in the *Kinesis Data Firehose Developer Guide*.
 
 ## Specifying an IAM role
 
 The DeliveryStream class automatically creates IAM service roles with all the minimum
 necessary permissions for Kinesis Data Firehose to access the resources referenced by your
@@ -544,15 +615,15 @@
 in the *Kinesis Data Firehose Developer Guide*.
 
 ## Granting application access to a delivery stream
 
 IAM roles, users or groups which need to be able to work with delivery streams should be
 granted IAM permissions.
 
-Any object that implements the `IGrantable` interface (i.e., has an associated principal)
+Any object that implements the `IGrantable` interface (ie., has an associated principal)
 can be granted permissions to a delivery stream by calling:
 
 * `grantPutRecords(principal)` - grants the principal the ability to put records onto the
   delivery stream
 * `grant(principal, ...actions)` - grants the principal permission to a custom set of
   actions
 
@@ -561,16 +632,15 @@
 # delivery_stream: firehose.DeliveryStream
 lambda_role = iam.Role(self, "Role",
     assumed_by=iam.ServicePrincipal("lambda.amazonaws.com")
 )
 delivery_stream.grant_put_records(lambda_role)
 ```
 
-The following write permissions are provided to a service principal by the
-`grantPutRecords()` method:
+The following write permissions are provided to a service principal by the `grantPutRecords()` method:
 
 * `firehose:PutRecord`
 * `firehose:PutRecordBatch`
 
 ## Granting a delivery stream access to a resource
 
 Conversely to the above, Kinesis Data Firehose requires permissions in order for delivery
@@ -603,36 +673,34 @@
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
-import aws_cdk.aws_kinesis as _aws_cdk_aws_kinesis_ceddda9d
-import aws_cdk.aws_kinesisfirehose as _aws_cdk_aws_kinesisfirehose_ceddda9d
-import aws_cdk.aws_kms as _aws_cdk_aws_kms_ceddda9d
-import aws_cdk.aws_lambda as _aws_cdk_aws_lambda_ceddda9d
-import constructs as _constructs_77d1e7e8
+import aws_cdk
+import aws_cdk.aws_cloudwatch
+import aws_cdk.aws_ec2
+import aws_cdk.aws_iam
+import aws_cdk.aws_kinesis
+import aws_cdk.aws_kinesisfirehose
+import aws_cdk.aws_kms
+import aws_cdk.aws_lambda
+import constructs
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-kinesisfirehose-alpha.DataProcessorBindOptions",
     jsii_struct_bases=[],
     name_mapping={"role": "role"},
 )
 class DataProcessorBindOptions:
-    def __init__(self, *, role: _aws_cdk_aws_iam_ceddda9d.IRole) -> None:
+    def __init__(self, *, role: aws_cdk.aws_iam.IRole) -> None:
         '''(experimental) Options when binding a DataProcessor to a delivery stream destination.
 
         :param role: (experimental) The IAM role assumed by Kinesis Data Firehose to write to the destination that this DataProcessor will bind to.
 
         :stability: experimental
         :exampleMetadata: fixture=_generated
 
@@ -645,30 +713,27 @@
             
             # role: iam.Role
             
             data_processor_bind_options = kinesisfirehose_alpha.DataProcessorBindOptions(
                 role=role
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fb128eca4e7ba1f83c4f0e58098f008795374fee30ada93711dd3b253dad0ef8)
-            check_type(argname="argument role", value=role, expected_type=type_hints["role"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "role": role,
         }
 
     @builtins.property
-    def role(self) -> _aws_cdk_aws_iam_ceddda9d.IRole:
+    def role(self) -> aws_cdk.aws_iam.IRole:
         '''(experimental) The IAM role assumed by Kinesis Data Firehose to write to the destination that this DataProcessor will bind to.
 
         :stability: experimental
         '''
         result = self._values.get("role")
         assert result is not None, "Required property 'role' is missing"
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.IRole, result)
+        return typing.cast(aws_cdk.aws_iam.IRole, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -686,15 +751,15 @@
         "processor_type": "processorType",
     },
 )
 class DataProcessorConfig:
     def __init__(
         self,
         *,
-        processor_identifier: typing.Union["DataProcessorIdentifier", typing.Dict[builtins.str, typing.Any]],
+        processor_identifier: "DataProcessorIdentifier",
         processor_type: builtins.str,
     ) -> None:
         '''(experimental) The full configuration of a data processor.
 
         :param processor_identifier: (experimental) The key-value pair that identifies the underlying processor resource.
         :param processor_type: (experimental) The type of the underlying processor resource. Must be an accepted value in ``CfnDeliveryStream.ProcessorProperty.Type``.
 
@@ -713,19 +778,15 @@
                     parameter_value="parameterValue"
                 ),
                 processor_type="processorType"
             )
         '''
         if isinstance(processor_identifier, dict):
             processor_identifier = DataProcessorIdentifier(**processor_identifier)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__99d8516a4394f7676eff7b29cec88a391ff919bb6bbda458b6e8e06f6ddb7a88)
-            check_type(argname="argument processor_identifier", value=processor_identifier, expected_type=type_hints["processor_identifier"])
-            check_type(argname="argument processor_type", value=processor_type, expected_type=type_hints["processor_type"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "processor_identifier": processor_identifier,
             "processor_type": processor_type,
         }
 
     @builtins.property
     def processor_identifier(self) -> "DataProcessorIdentifier":
         '''(experimental) The key-value pair that identifies the underlying processor resource.
@@ -796,19 +857,15 @@
             import aws_cdk.aws_kinesisfirehose_alpha as kinesisfirehose_alpha
             
             data_processor_identifier = kinesisfirehose_alpha.DataProcessorIdentifier(
                 parameter_name="parameterName",
                 parameter_value="parameterValue"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3c5e177461759fec4dd89a5e4a7730bec0e39ea197243fa5f2eceea512a39f24)
-            check_type(argname="argument parameter_name", value=parameter_name, expected_type=type_hints["parameter_name"])
-            check_type(argname="argument parameter_value", value=parameter_value, expected_type=type_hints["parameter_value"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "parameter_name": parameter_name,
             "parameter_value": parameter_value,
         }
 
     @builtins.property
     def parameter_name(self) -> builtins.str:
         '''(experimental) The parameter name that corresponds to the processor resource's identifier.
@@ -852,85 +909,131 @@
         "retries": "retries",
     },
 )
 class DataProcessorProps:
     def __init__(
         self,
         *,
-        buffer_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-        buffer_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
+        buffer_interval: typing.Optional[aws_cdk.Duration] = None,
+        buffer_size: typing.Optional[aws_cdk.Size] = None,
         retries: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''(experimental) Configure the data processor.
 
         :param buffer_interval: (experimental) The length of time Kinesis Data Firehose will buffer incoming data before calling the processor. s Default: Duration.minutes(1)
         :param buffer_size: (experimental) The amount of incoming data Kinesis Data Firehose will buffer before calling the processor. Default: Size.mebibytes(3)
         :param retries: (experimental) The number of times Kinesis Data Firehose will retry the processor invocation after a failure due to network timeout or invocation limits. Default: 3
 
         :stability: experimental
-        :exampleMetadata: infused
+        :exampleMetadata: lit=../aws-kinesisfirehose-destinations/test/integ.s3-bucket.lit.ts infused
 
         Example::
 
-            # bucket: s3.Bucket
-            # Provide a Lambda function that will transform records before delivery, with custom
-            # buffering and retry configuration
-            lambda_function = lambda_.Function(self, "Processor",
-                runtime=lambda_.Runtime.NODEJS_14_X,
-                handler="index.handler",
-                code=lambda_.Code.from_asset(path.join(__dirname, "process-records"))
+            import path as path
+            import aws_cdk.aws_kinesisfirehose_alpha as firehose
+            import aws_cdk.aws_kms as kms
+            import aws_cdk.aws_lambda_nodejs as lambdanodejs
+            import aws_cdk.aws_logs as logs
+            import aws_cdk.aws_s3 as s3
+            import aws_cdk as cdk
+            import aws_cdk.aws_kinesisfirehose_destinations_alpha as destinations
+            
+            app = cdk.App()
+            
+            stack = cdk.Stack(app, "aws-cdk-firehose-delivery-stream-s3-all-properties")
+            
+            bucket = s3.Bucket(stack, "Bucket",
+                removal_policy=cdk.RemovalPolicy.DESTROY,
+                auto_delete_objects=True
             )
-            lambda_processor = firehose.LambdaFunctionProcessor(lambda_function,
-                buffer_interval=Duration.minutes(5),
-                buffer_size=Size.mebibytes(5),
-                retries=5
+            
+            backup_bucket = s3.Bucket(stack, "BackupBucket",
+                removal_policy=cdk.RemovalPolicy.DESTROY,
+                auto_delete_objects=True
             )
-            s3_destination = destinations.S3Bucket(bucket,
-                processor=lambda_processor
+            log_group = logs.LogGroup(stack, "LogGroup",
+                removal_policy=cdk.RemovalPolicy.DESTROY
             )
-            firehose.DeliveryStream(self, "Delivery Stream",
-                destinations=[s3_destination]
+            
+            data_processor_function = lambdanodejs.NodejsFunction(stack, "DataProcessorFunction",
+                entry=path.join(__dirname, "lambda-data-processor.js"),
+                timeout=cdk.Duration.minutes(1)
             )
+            
+            processor = firehose.LambdaFunctionProcessor(data_processor_function,
+                buffer_interval=cdk.Duration.seconds(60),
+                buffer_size=cdk.Size.mebibytes(1),
+                retries=1
+            )
+            
+            key = kms.Key(stack, "Key",
+                removal_policy=cdk.RemovalPolicy.DESTROY
+            )
+            
+            backup_key = kms.Key(stack, "BackupKey",
+                removal_policy=cdk.RemovalPolicy.DESTROY
+            )
+            
+            firehose.DeliveryStream(stack, "Delivery Stream",
+                destinations=[destinations.S3Bucket(bucket,
+                    logging=True,
+                    log_group=log_group,
+                    processor=processor,
+                    compression=destinations.Compression.GZIP,
+                    data_output_prefix="regularPrefix",
+                    error_output_prefix="errorPrefix",
+                    buffering_interval=cdk.Duration.seconds(60),
+                    buffering_size=cdk.Size.mebibytes(1),
+                    encryption_key=key,
+                    s3_backup=destinations.DestinationS3BackupProps(
+                        mode=destinations.BackupMode.ALL,
+                        bucket=backup_bucket,
+                        compression=destinations.Compression.ZIP,
+                        data_output_prefix="backupPrefix",
+                        error_output_prefix="backupErrorPrefix",
+                        buffering_interval=cdk.Duration.seconds(60),
+                        buffering_size=cdk.Size.mebibytes(1),
+                        encryption_key=backup_key
+                    )
+                )]
+            )
+            
+            app.synth()
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b6f8aa68afc823d87c695ee05759728c85e4023a37cf01cf765a10be84fbcac8)
-            check_type(argname="argument buffer_interval", value=buffer_interval, expected_type=type_hints["buffer_interval"])
-            check_type(argname="argument buffer_size", value=buffer_size, expected_type=type_hints["buffer_size"])
-            check_type(argname="argument retries", value=retries, expected_type=type_hints["retries"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if buffer_interval is not None:
             self._values["buffer_interval"] = buffer_interval
         if buffer_size is not None:
             self._values["buffer_size"] = buffer_size
         if retries is not None:
             self._values["retries"] = retries
 
     @builtins.property
-    def buffer_interval(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+    def buffer_interval(self) -> typing.Optional[aws_cdk.Duration]:
         '''(experimental) The length of time Kinesis Data Firehose will buffer incoming data before calling the processor.
 
         s
 
         :default: Duration.minutes(1)
 
         :stability: experimental
         '''
         result = self._values.get("buffer_interval")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
+        return typing.cast(typing.Optional[aws_cdk.Duration], result)
 
     @builtins.property
-    def buffer_size(self) -> typing.Optional[_aws_cdk_ceddda9d.Size]:
+    def buffer_size(self) -> typing.Optional[aws_cdk.Size]:
         '''(experimental) The amount of incoming data Kinesis Data Firehose will buffer before calling the processor.
 
         :default: Size.mebibytes(3)
 
         :stability: experimental
         '''
         result = self._values.get("buffer_size")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Size], result)
+        return typing.cast(typing.Optional[aws_cdk.Size], result)
 
     @builtins.property
     def retries(self) -> typing.Optional[jsii.Number]:
         '''(experimental) The number of times Kinesis Data Firehose will retry the processor invocation after a failure due to network timeout or invocation limits.
 
         :default: 3
 
@@ -962,15 +1065,15 @@
 )
 class DeliveryStreamAttributes:
     def __init__(
         self,
         *,
         delivery_stream_arn: typing.Optional[builtins.str] = None,
         delivery_stream_name: typing.Optional[builtins.str] = None,
-        role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
     ) -> None:
         '''(experimental) A full specification of a delivery stream that can be used to import it fluently into the CDK application.
 
         :param delivery_stream_arn: (experimental) The ARN of the delivery stream. At least one of deliveryStreamArn and deliveryStreamName must be provided. Default: - derived from ``deliveryStreamName``.
         :param delivery_stream_name: (experimental) The name of the delivery stream. At least one of deliveryStreamName and deliveryStreamArn must be provided. Default: - derived from ``deliveryStreamArn``.
         :param role: (experimental) The IAM role associated with this delivery stream. Assumed by Kinesis Data Firehose to read from sources and encrypt data server-side. Default: - the imported stream cannot be granted access to other resources as an ``iam.IGrantable``.
 
@@ -988,20 +1091,15 @@
             
             delivery_stream_attributes = kinesisfirehose_alpha.DeliveryStreamAttributes(
                 delivery_stream_arn="deliveryStreamArn",
                 delivery_stream_name="deliveryStreamName",
                 role=role
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5a349f2444857db9da26d39113740e8ab10e954d7aef8340312a07dcb3ca0c72)
-            check_type(argname="argument delivery_stream_arn", value=delivery_stream_arn, expected_type=type_hints["delivery_stream_arn"])
-            check_type(argname="argument delivery_stream_name", value=delivery_stream_name, expected_type=type_hints["delivery_stream_name"])
-            check_type(argname="argument role", value=role, expected_type=type_hints["role"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if delivery_stream_arn is not None:
             self._values["delivery_stream_arn"] = delivery_stream_arn
         if delivery_stream_name is not None:
             self._values["delivery_stream_name"] = delivery_stream_name
         if role is not None:
             self._values["role"] = role
 
@@ -1028,25 +1126,25 @@
 
         :stability: experimental
         '''
         result = self._values.get("delivery_stream_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+    def role(self) -> typing.Optional[aws_cdk.aws_iam.IRole]:
         '''(experimental) The IAM role associated with this delivery stream.
 
         Assumed by Kinesis Data Firehose to read from sources and encrypt data server-side.
 
         :default: - the imported stream cannot be granted access to other resources as an ``iam.IGrantable``.
 
         :stability: experimental
         '''
         result = self._values.get("role")
-        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_iam.IRole], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -1071,17 +1169,17 @@
 class DeliveryStreamProps:
     def __init__(
         self,
         *,
         destinations: typing.Sequence["IDestination"],
         delivery_stream_name: typing.Optional[builtins.str] = None,
         encryption: typing.Optional["StreamEncryption"] = None,
-        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-        role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-        source_stream: typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.IStream] = None,
+        encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
+        role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
+        source_stream: typing.Optional[aws_cdk.aws_kinesis.IStream] = None,
     ) -> None:
         '''(experimental) Properties for a new delivery stream.
 
         :param destinations: (experimental) The destinations that this delivery stream will deliver data to. Only a singleton array is supported at this time.
         :param delivery_stream_name: (experimental) A name for the delivery stream. Default: - a name is generated by CloudFormation.
         :param encryption: (experimental) Indicates the type of customer master key (CMK) to use for server-side encryption, if any. Default: StreamEncryption.UNENCRYPTED - unless ``encryptionKey`` is provided, in which case this will be implicitly set to ``StreamEncryption.CUSTOMER_MANAGED``
         :param encryption_key: (experimental) Customer managed key to server-side encrypt data in the stream. Default: - no KMS key will be used; if ``encryption`` is set to ``CUSTOMER_MANAGED``, a KMS key will be created for you
@@ -1089,41 +1187,35 @@
         :param source_stream: (experimental) The Kinesis data stream to use as a source for this delivery stream. Default: - data must be written to the delivery stream via a direct put.
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
-            # Specify the roles created above when defining the destination and delivery stream.
             # bucket: s3.Bucket
-            # Create service roles for the delivery stream and destination.
-            # These can be used for other purposes and granted access to different resources.
-            # They must include the Kinesis Data Firehose service principal in their trust policies.
-            # Two separate roles are shown below, but the same role can be used for both purposes.
-            delivery_stream_role = iam.Role(self, "Delivery Stream Role",
-                assumed_by=iam.ServicePrincipal("firehose.amazonaws.com")
+            # Provide a Lambda function that will transform records before delivery, with custom
+            # buffering and retry configuration
+            lambda_function = lambda_.Function(self, "Processor",
+                runtime=lambda_.Runtime.NODEJS_12_X,
+                handler="index.handler",
+                code=lambda_.Code.from_asset(path.join(__dirname, "process-records"))
+            )
+            lambda_processor = firehose.LambdaFunctionProcessor(lambda_function,
+                buffer_interval=Duration.minutes(5),
+                buffer_size=Size.mebibytes(5),
+                retries=5
             )
-            destination_role = iam.Role(self, "Destination Role",
-                assumed_by=iam.ServicePrincipal("firehose.amazonaws.com")
+            s3_destination = destinations.S3Bucket(bucket,
+                processor=lambda_processor
             )
-            destination = destinations.S3Bucket(bucket, role=destination_role)
             firehose.DeliveryStream(self, "Delivery Stream",
-                destinations=[destination],
-                role=delivery_stream_role
+                destinations=[s3_destination]
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5b9413f788fdc9578de6565f85eb1d6d397a1047293bb85b71a059af7643ba38)
-            check_type(argname="argument destinations", value=destinations, expected_type=type_hints["destinations"])
-            check_type(argname="argument delivery_stream_name", value=delivery_stream_name, expected_type=type_hints["delivery_stream_name"])
-            check_type(argname="argument encryption", value=encryption, expected_type=type_hints["encryption"])
-            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
-            check_type(argname="argument role", value=role, expected_type=type_hints["role"])
-            check_type(argname="argument source_stream", value=source_stream, expected_type=type_hints["source_stream"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "destinations": destinations,
         }
         if delivery_stream_name is not None:
             self._values["delivery_stream_name"] = delivery_stream_name
         if encryption is not None:
             self._values["encryption"] = encryption
         if encryption_key is not None:
@@ -1164,47 +1256,47 @@
 
         :stability: experimental
         '''
         result = self._values.get("encryption")
         return typing.cast(typing.Optional["StreamEncryption"], result)
 
     @builtins.property
-    def encryption_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def encryption_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) Customer managed key to server-side encrypt data in the stream.
 
         :default: - no KMS key will be used; if ``encryption`` is set to ``CUSTOMER_MANAGED``, a KMS key will be created for you
 
         :stability: experimental
         '''
         result = self._values.get("encryption_key")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], result)
 
     @builtins.property
-    def role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+    def role(self) -> typing.Optional[aws_cdk.aws_iam.IRole]:
         '''(experimental) The IAM role associated with this delivery stream.
 
         Assumed by Kinesis Data Firehose to read from sources and encrypt data server-side.
 
         :default: - a role will be created with default permissions.
 
         :stability: experimental
         '''
         result = self._values.get("role")
-        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_iam.IRole], result)
 
     @builtins.property
-    def source_stream(self) -> typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.IStream]:
+    def source_stream(self) -> typing.Optional[aws_cdk.aws_kinesis.IStream]:
         '''(experimental) The Kinesis data stream to use as a source for this delivery stream.
 
         :default: - data must be written to the delivery stream via a direct put.
 
         :stability: experimental
         '''
         result = self._values.get("source_stream")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.IStream], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kinesis.IStream], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -1230,15 +1322,15 @@
 
             # The code below shows an example of how to instantiate this type.
             # The values are placeholders you should change.
             import aws_cdk.aws_kinesisfirehose_alpha as kinesisfirehose_alpha
             
             destination_bind_options = kinesisfirehose_alpha.DestinationBindOptions()
         '''
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -1256,16 +1348,16 @@
         "extended_s3_destination_configuration": "extendedS3DestinationConfiguration",
     },
 )
 class DestinationConfig:
     def __init__(
         self,
         *,
-        dependables: typing.Optional[typing.Sequence[_constructs_77d1e7e8.IDependable]] = None,
-        extended_s3_destination_configuration: typing.Optional[typing.Union[_aws_cdk_aws_kinesisfirehose_ceddda9d.CfnDeliveryStream.ExtendedS3DestinationConfigurationProperty, typing.Dict[builtins.str, typing.Any]]] = None,
+        dependables: typing.Optional[typing.Sequence[constructs.IDependable]] = None,
+        extended_s3_destination_configuration: typing.Optional[aws_cdk.aws_kinesisfirehose.CfnDeliveryStream.ExtendedS3DestinationConfigurationProperty] = None,
     ) -> None:
         '''(experimental) A Kinesis Data Firehose delivery stream destination configuration.
 
         :param dependables: (experimental) Any resources that were created by the destination when binding it to the stack that must be deployed before the delivery stream is deployed. Default: []
         :param extended_s3_destination_configuration: (experimental) S3 destination configuration properties. Default: - S3 destination is not used.
 
         :stability: experimental
@@ -1397,50 +1489,44 @@
                         prefix="prefix"
                     ),
                     s3_backup_mode="s3BackupMode"
                 )
             )
         '''
         if isinstance(extended_s3_destination_configuration, dict):
-            extended_s3_destination_configuration = _aws_cdk_aws_kinesisfirehose_ceddda9d.CfnDeliveryStream.ExtendedS3DestinationConfigurationProperty(**extended_s3_destination_configuration)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__173daa2306128c47572263a530e0a02f73aa7e3f60be737ce497d123e3edc32d)
-            check_type(argname="argument dependables", value=dependables, expected_type=type_hints["dependables"])
-            check_type(argname="argument extended_s3_destination_configuration", value=extended_s3_destination_configuration, expected_type=type_hints["extended_s3_destination_configuration"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+            extended_s3_destination_configuration = aws_cdk.aws_kinesisfirehose.CfnDeliveryStream.ExtendedS3DestinationConfigurationProperty(**extended_s3_destination_configuration)
+        self._values: typing.Dict[str, typing.Any] = {}
         if dependables is not None:
             self._values["dependables"] = dependables
         if extended_s3_destination_configuration is not None:
             self._values["extended_s3_destination_configuration"] = extended_s3_destination_configuration
 
     @builtins.property
-    def dependables(
-        self,
-    ) -> typing.Optional[typing.List[_constructs_77d1e7e8.IDependable]]:
+    def dependables(self) -> typing.Optional[typing.List[constructs.IDependable]]:
         '''(experimental) Any resources that were created by the destination when binding it to the stack that must be deployed before the delivery stream is deployed.
 
         :default: []
 
         :stability: experimental
         '''
         result = self._values.get("dependables")
-        return typing.cast(typing.Optional[typing.List[_constructs_77d1e7e8.IDependable]], result)
+        return typing.cast(typing.Optional[typing.List[constructs.IDependable]], result)
 
     @builtins.property
     def extended_s3_destination_configuration(
         self,
-    ) -> typing.Optional[_aws_cdk_aws_kinesisfirehose_ceddda9d.CfnDeliveryStream.ExtendedS3DestinationConfigurationProperty]:
+    ) -> typing.Optional[aws_cdk.aws_kinesisfirehose.CfnDeliveryStream.ExtendedS3DestinationConfigurationProperty]:
         '''(experimental) S3 destination configuration properties.
 
         :default: - S3 destination is not used.
 
         :stability: experimental
         '''
         result = self._values.get("extended_s3_destination_configuration")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kinesisfirehose_ceddda9d.CfnDeliveryStream.ExtendedS3DestinationConfigurationProperty], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kinesisfirehose.CfnDeliveryStream.ExtendedS3DestinationConfigurationProperty], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -1453,29 +1539,29 @@
 @jsii.interface(jsii_type="@aws-cdk/aws-kinesisfirehose-alpha.IDataProcessor")
 class IDataProcessor(typing_extensions.Protocol):
     '''(experimental) A data processor that Kinesis Data Firehose will call to transform records before delivering data.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="props")
     def props(self) -> DataProcessorProps:
         '''(experimental) The constructor props of the DataProcessor.
 
         :stability: experimental
         '''
         ...
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         *,
-        role: _aws_cdk_aws_iam_ceddda9d.IRole,
+        role: aws_cdk.aws_iam.IRole,
     ) -> DataProcessorConfig:
         '''(experimental) Binds this processor to a destination of a delivery stream.
 
         Implementers should use this method to grant processor invocation permissions to the provided stream and return the
         necessary configuration to register as a processor.
 
         :param scope: -
@@ -1490,103 +1576,100 @@
     '''(experimental) A data processor that Kinesis Data Firehose will call to transform records before delivering data.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-kinesisfirehose-alpha.IDataProcessor"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="props")
     def props(self) -> DataProcessorProps:
         '''(experimental) The constructor props of the DataProcessor.
 
         :stability: experimental
         '''
         return typing.cast(DataProcessorProps, jsii.get(self, "props"))
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         *,
-        role: _aws_cdk_aws_iam_ceddda9d.IRole,
+        role: aws_cdk.aws_iam.IRole,
     ) -> DataProcessorConfig:
         '''(experimental) Binds this processor to a destination of a delivery stream.
 
         Implementers should use this method to grant processor invocation permissions to the provided stream and return the
         necessary configuration to register as a processor.
 
         :param scope: -
         :param role: (experimental) The IAM role assumed by Kinesis Data Firehose to write to the destination that this DataProcessor will bind to.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__22c1e85da04925f59501768e65d47bdfdedeb6e3e0dfcee70ee80c529df93f3a)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
         options = DataProcessorBindOptions(role=role)
 
         return typing.cast(DataProcessorConfig, jsii.invoke(self, "bind", [scope, options]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IDataProcessor).__jsii_proxy_class__ = lambda : _IDataProcessorProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-kinesisfirehose-alpha.IDeliveryStream")
 class IDeliveryStream(
-    _aws_cdk_ceddda9d.IResource,
-    _aws_cdk_aws_iam_ceddda9d.IGrantable,
-    _aws_cdk_aws_ec2_ceddda9d.IConnectable,
+    aws_cdk.IResource,
+    aws_cdk.aws_iam.IGrantable,
+    aws_cdk.aws_ec2.IConnectable,
     typing_extensions.Protocol,
 ):
     '''(experimental) Represents a Kinesis Data Firehose delivery stream.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="deliveryStreamArn")
     def delivery_stream_arn(self) -> builtins.str:
         '''(experimental) The ARN of the delivery stream.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="deliveryStreamName")
     def delivery_stream_name(self) -> builtins.str:
         '''(experimental) The name of the delivery stream.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
     @jsii.member(jsii_name="grant")
     def grant(
         self,
-        grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
+        grantee: aws_cdk.aws_iam.IGrantable,
         *actions: builtins.str,
-    ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
+    ) -> aws_cdk.aws_iam.Grant:
         '''(experimental) Grant the ``grantee`` identity permissions to perform ``actions``.
 
         :param grantee: -
         :param actions: -
 
         :stability: experimental
         '''
         ...
 
     @jsii.member(jsii_name="grantPutRecords")
     def grant_put_records(
         self,
-        grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-    ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
+        grantee: aws_cdk.aws_iam.IGrantable,
+    ) -> aws_cdk.aws_iam.Grant:
         '''(experimental) Grant the ``grantee`` identity permissions to perform ``firehose:PutRecord`` and ``firehose:PutRecordBatch`` actions on this delivery stream.
 
         :param grantee: -
 
         :stability: experimental
         '''
         ...
@@ -1596,519 +1679,509 @@
         self,
         metric_name: builtins.str,
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
         '''(experimental) Return the given named metric for this delivery stream.
 
         :param metric_name: -
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
         ...
 
     @jsii.member(jsii_name="metricBackupToS3Bytes")
     def metric_backup_to_s3_bytes(
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
         '''(experimental) Metric for the number of bytes delivered to Amazon S3 for backup over the specified time period.
 
         By default, this metric will be calculated as an average over a period of 5 minutes.
 
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
         ...
 
     @jsii.member(jsii_name="metricBackupToS3DataFreshness")
     def metric_backup_to_s3_data_freshness(
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
         '''(experimental) Metric for the age (from getting into Kinesis Data Firehose to now) of the oldest record in Kinesis Data Firehose.
 
         Any record older than this age has been delivered to the Amazon S3 bucket for backup.
 
         By default, this metric will be calculated as an average over a period of 5 minutes.
 
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
         ...
 
     @jsii.member(jsii_name="metricBackupToS3Records")
     def metric_backup_to_s3_records(
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
         '''(experimental) Metric for the number of records delivered to Amazon S3 for backup over the specified time period.
 
         By default, this metric will be calculated as an average over a period of 5 minutes.
 
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
         ...
 
     @jsii.member(jsii_name="metricIncomingBytes")
     def metric_incoming_bytes(
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
         '''(experimental) Metric for the number of bytes ingested successfully into the delivery stream over the specified time period after throttling.
 
         By default, this metric will be calculated as an average over a period of 5 minutes.
 
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
         ...
 
     @jsii.member(jsii_name="metricIncomingRecords")
     def metric_incoming_records(
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
         '''(experimental) Metric for the number of records ingested successfully into the delivery stream over the specified time period after throttling.
 
         By default, this metric will be calculated as an average over a period of 5 minutes.
 
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
         ...
 
 
 class _IDeliveryStreamProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
-    jsii.proxy_for(_aws_cdk_aws_iam_ceddda9d.IGrantable), # type: ignore[misc]
-    jsii.proxy_for(_aws_cdk_aws_ec2_ceddda9d.IConnectable), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.aws_iam.IGrantable), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.aws_ec2.IConnectable), # type: ignore[misc]
 ):
     '''(experimental) Represents a Kinesis Data Firehose delivery stream.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-kinesisfirehose-alpha.IDeliveryStream"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="deliveryStreamArn")
     def delivery_stream_arn(self) -> builtins.str:
         '''(experimental) The ARN of the delivery stream.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "deliveryStreamArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="deliveryStreamName")
     def delivery_stream_name(self) -> builtins.str:
         '''(experimental) The name of the delivery stream.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "deliveryStreamName"))
 
     @jsii.member(jsii_name="grant")
     def grant(
         self,
-        grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
+        grantee: aws_cdk.aws_iam.IGrantable,
         *actions: builtins.str,
-    ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
+    ) -> aws_cdk.aws_iam.Grant:
         '''(experimental) Grant the ``grantee`` identity permissions to perform ``actions``.
 
         :param grantee: -
         :param actions: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4e83b2c41b0be3872a96c9d852da78dc5625213352508d0b4a5e81440d9d1a8e)
-            check_type(argname="argument grantee", value=grantee, expected_type=type_hints["grantee"])
-            check_type(argname="argument actions", value=actions, expected_type=typing.Tuple[type_hints["actions"], ...]) # pyright: ignore [reportGeneralTypeIssues]
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.Grant, jsii.invoke(self, "grant", [grantee, *actions]))
+        return typing.cast(aws_cdk.aws_iam.Grant, jsii.invoke(self, "grant", [grantee, *actions]))
 
     @jsii.member(jsii_name="grantPutRecords")
     def grant_put_records(
         self,
-        grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-    ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
+        grantee: aws_cdk.aws_iam.IGrantable,
+    ) -> aws_cdk.aws_iam.Grant:
         '''(experimental) Grant the ``grantee`` identity permissions to perform ``firehose:PutRecord`` and ``firehose:PutRecordBatch`` actions on this delivery stream.
 
         :param grantee: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ce79dffc4fc87d6b02f31af6954926f1cdb38d458bb0706848609d95b5e62915)
-            check_type(argname="argument grantee", value=grantee, expected_type=type_hints["grantee"])
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.Grant, jsii.invoke(self, "grantPutRecords", [grantee]))
+        return typing.cast(aws_cdk.aws_iam.Grant, jsii.invoke(self, "grantPutRecords", [grantee]))
 
     @jsii.member(jsii_name="metric")
     def metric(
         self,
         metric_name: builtins.str,
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
         '''(experimental) Return the given named metric for this delivery stream.
 
         :param metric_name: -
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
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__52389e5ce1f5828630ba548c0c34e45b5f8dfbc1ad4857c9e91cc7ac36dac99f)
-            check_type(argname="argument metric_name", value=metric_name, expected_type=type_hints["metric_name"])
-        props = _aws_cdk_aws_cloudwatch_ceddda9d.MetricOptions(
+        props = aws_cdk.aws_cloudwatch.MetricOptions(
             account=account,
             color=color,
             dimensions_map=dimensions_map,
             label=label,
             period=period,
             region=region,
             statistic=statistic,
             unit=unit,
         )
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metric", [metric_name, props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metric", [metric_name, props]))
 
     @jsii.member(jsii_name="metricBackupToS3Bytes")
     def metric_backup_to_s3_bytes(
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
         '''(experimental) Metric for the number of bytes delivered to Amazon S3 for backup over the specified time period.
 
         By default, this metric will be calculated as an average over a period of 5 minutes.
 
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
-        props = _aws_cdk_aws_cloudwatch_ceddda9d.MetricOptions(
+        props = aws_cdk.aws_cloudwatch.MetricOptions(
             account=account,
             color=color,
             dimensions_map=dimensions_map,
             label=label,
             period=period,
             region=region,
             statistic=statistic,
             unit=unit,
         )
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricBackupToS3Bytes", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricBackupToS3Bytes", [props]))
 
     @jsii.member(jsii_name="metricBackupToS3DataFreshness")
     def metric_backup_to_s3_data_freshness(
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
         '''(experimental) Metric for the age (from getting into Kinesis Data Firehose to now) of the oldest record in Kinesis Data Firehose.
 
         Any record older than this age has been delivered to the Amazon S3 bucket for backup.
 
         By default, this metric will be calculated as an average over a period of 5 minutes.
 
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
-        props = _aws_cdk_aws_cloudwatch_ceddda9d.MetricOptions(
+        props = aws_cdk.aws_cloudwatch.MetricOptions(
             account=account,
             color=color,
             dimensions_map=dimensions_map,
             label=label,
             period=period,
             region=region,
             statistic=statistic,
             unit=unit,
         )
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricBackupToS3DataFreshness", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricBackupToS3DataFreshness", [props]))
 
     @jsii.member(jsii_name="metricBackupToS3Records")
     def metric_backup_to_s3_records(
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
         '''(experimental) Metric for the number of records delivered to Amazon S3 for backup over the specified time period.
 
         By default, this metric will be calculated as an average over a period of 5 minutes.
 
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
-        props = _aws_cdk_aws_cloudwatch_ceddda9d.MetricOptions(
+        props = aws_cdk.aws_cloudwatch.MetricOptions(
             account=account,
             color=color,
             dimensions_map=dimensions_map,
             label=label,
             period=period,
             region=region,
             statistic=statistic,
             unit=unit,
         )
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricBackupToS3Records", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricBackupToS3Records", [props]))
 
     @jsii.member(jsii_name="metricIncomingBytes")
     def metric_incoming_bytes(
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
         '''(experimental) Metric for the number of bytes ingested successfully into the delivery stream over the specified time period after throttling.
 
         By default, this metric will be calculated as an average over a period of 5 minutes.
 
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
-        props = _aws_cdk_aws_cloudwatch_ceddda9d.MetricOptions(
+        props = aws_cdk.aws_cloudwatch.MetricOptions(
             account=account,
             color=color,
             dimensions_map=dimensions_map,
             label=label,
             period=period,
             region=region,
             statistic=statistic,
             unit=unit,
         )
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricIncomingBytes", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricIncomingBytes", [props]))
 
     @jsii.member(jsii_name="metricIncomingRecords")
     def metric_incoming_records(
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
         '''(experimental) Metric for the number of records ingested successfully into the delivery stream over the specified time period after throttling.
 
         By default, this metric will be calculated as an average over a period of 5 minutes.
 
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
-        props = _aws_cdk_aws_cloudwatch_ceddda9d.MetricOptions(
+        props = aws_cdk.aws_cloudwatch.MetricOptions(
             account=account,
             color=color,
             dimensions_map=dimensions_map,
             label=label,
             period=period,
             region=region,
             statistic=statistic,
             unit=unit,
         )
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricIncomingRecords", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricIncomingRecords", [props]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IDeliveryStream).__jsii_proxy_class__ = lambda : _IDeliveryStreamProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-kinesisfirehose-alpha.IDestination")
 class IDestination(typing_extensions.Protocol):
     '''(experimental) A Kinesis Data Firehose delivery stream destination.
 
     :stability: experimental
     '''
 
     @jsii.member(jsii_name="bind")
-    def bind(self, scope: _constructs_77d1e7e8.Construct) -> DestinationConfig:
+    def bind(self, scope: constructs.Construct) -> DestinationConfig:
         '''(experimental) Binds this destination to the Kinesis Data Firehose delivery stream.
 
         Implementers should use this method to bind resources to the stack and initialize values using the provided stream.
 
         :param scope: -
 
         :stability: experimental
@@ -2121,26 +2194,23 @@
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-kinesisfirehose-alpha.IDestination"
 
     @jsii.member(jsii_name="bind")
-    def bind(self, scope: _constructs_77d1e7e8.Construct) -> DestinationConfig:
+    def bind(self, scope: constructs.Construct) -> DestinationConfig:
         '''(experimental) Binds this destination to the Kinesis Data Firehose delivery stream.
 
         Implementers should use this method to bind resources to the stack and initialize values using the provided stream.
 
         :param scope: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b51d023ede755a18ed86b3caecd01c91773858417bf2e779e934ccc241569676)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
         options = DestinationBindOptions()
 
         return typing.cast(DestinationConfig, jsii.invoke(self, "bind", [scope, options]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IDestination).__jsii_proxy_class__ = lambda : _IDestinationProxy
 
@@ -2149,89 +2219,134 @@
 class LambdaFunctionProcessor(
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-kinesisfirehose-alpha.LambdaFunctionProcessor",
 ):
     '''(experimental) Use an AWS Lambda function to transform records.
 
     :stability: experimental
-    :exampleMetadata: infused
+    :exampleMetadata: lit=../aws-kinesisfirehose-destinations/test/integ.s3-bucket.lit.ts infused
 
     Example::
 
-        # bucket: s3.Bucket
-        # Provide a Lambda function that will transform records before delivery, with custom
-        # buffering and retry configuration
-        lambda_function = lambda_.Function(self, "Processor",
-            runtime=lambda_.Runtime.NODEJS_14_X,
-            handler="index.handler",
-            code=lambda_.Code.from_asset(path.join(__dirname, "process-records"))
+        import path as path
+        import aws_cdk.aws_kinesisfirehose_alpha as firehose
+        import aws_cdk.aws_kms as kms
+        import aws_cdk.aws_lambda_nodejs as lambdanodejs
+        import aws_cdk.aws_logs as logs
+        import aws_cdk.aws_s3 as s3
+        import aws_cdk as cdk
+        import aws_cdk.aws_kinesisfirehose_destinations_alpha as destinations
+        
+        app = cdk.App()
+        
+        stack = cdk.Stack(app, "aws-cdk-firehose-delivery-stream-s3-all-properties")
+        
+        bucket = s3.Bucket(stack, "Bucket",
+            removal_policy=cdk.RemovalPolicy.DESTROY,
+            auto_delete_objects=True
         )
-        lambda_processor = firehose.LambdaFunctionProcessor(lambda_function,
-            buffer_interval=Duration.minutes(5),
-            buffer_size=Size.mebibytes(5),
-            retries=5
+        
+        backup_bucket = s3.Bucket(stack, "BackupBucket",
+            removal_policy=cdk.RemovalPolicy.DESTROY,
+            auto_delete_objects=True
         )
-        s3_destination = destinations.S3Bucket(bucket,
-            processor=lambda_processor
+        log_group = logs.LogGroup(stack, "LogGroup",
+            removal_policy=cdk.RemovalPolicy.DESTROY
         )
-        firehose.DeliveryStream(self, "Delivery Stream",
-            destinations=[s3_destination]
+        
+        data_processor_function = lambdanodejs.NodejsFunction(stack, "DataProcessorFunction",
+            entry=path.join(__dirname, "lambda-data-processor.js"),
+            timeout=cdk.Duration.minutes(1)
+        )
+        
+        processor = firehose.LambdaFunctionProcessor(data_processor_function,
+            buffer_interval=cdk.Duration.seconds(60),
+            buffer_size=cdk.Size.mebibytes(1),
+            retries=1
+        )
+        
+        key = kms.Key(stack, "Key",
+            removal_policy=cdk.RemovalPolicy.DESTROY
+        )
+        
+        backup_key = kms.Key(stack, "BackupKey",
+            removal_policy=cdk.RemovalPolicy.DESTROY
+        )
+        
+        firehose.DeliveryStream(stack, "Delivery Stream",
+            destinations=[destinations.S3Bucket(bucket,
+                logging=True,
+                log_group=log_group,
+                processor=processor,
+                compression=destinations.Compression.GZIP,
+                data_output_prefix="regularPrefix",
+                error_output_prefix="errorPrefix",
+                buffering_interval=cdk.Duration.seconds(60),
+                buffering_size=cdk.Size.mebibytes(1),
+                encryption_key=key,
+                s3_backup=destinations.DestinationS3BackupProps(
+                    mode=destinations.BackupMode.ALL,
+                    bucket=backup_bucket,
+                    compression=destinations.Compression.ZIP,
+                    data_output_prefix="backupPrefix",
+                    error_output_prefix="backupErrorPrefix",
+                    buffering_interval=cdk.Duration.seconds(60),
+                    buffering_size=cdk.Size.mebibytes(1),
+                    encryption_key=backup_key
+                )
+            )]
         )
+        
+        app.synth()
     '''
 
     def __init__(
         self,
-        lambda_function: _aws_cdk_aws_lambda_ceddda9d.IFunction,
+        lambda_function: aws_cdk.aws_lambda.IFunction,
         *,
-        buffer_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-        buffer_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
+        buffer_interval: typing.Optional[aws_cdk.Duration] = None,
+        buffer_size: typing.Optional[aws_cdk.Size] = None,
         retries: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
         :param lambda_function: -
         :param buffer_interval: (experimental) The length of time Kinesis Data Firehose will buffer incoming data before calling the processor. s Default: Duration.minutes(1)
         :param buffer_size: (experimental) The amount of incoming data Kinesis Data Firehose will buffer before calling the processor. Default: Size.mebibytes(3)
         :param retries: (experimental) The number of times Kinesis Data Firehose will retry the processor invocation after a failure due to network timeout or invocation limits. Default: 3
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__55ad5ddd8cb82f7d48b10e7568eedd0f96f6c1002a8170490a68123a94b247e0)
-            check_type(argname="argument lambda_function", value=lambda_function, expected_type=type_hints["lambda_function"])
         props = DataProcessorProps(
             buffer_interval=buffer_interval, buffer_size=buffer_size, retries=retries
         )
 
         jsii.create(self.__class__, self, [lambda_function, props])
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
-        _scope: _constructs_77d1e7e8.Construct,
+        _scope: constructs.Construct,
         *,
-        role: _aws_cdk_aws_iam_ceddda9d.IRole,
+        role: aws_cdk.aws_iam.IRole,
     ) -> DataProcessorConfig:
         '''(experimental) Binds this processor to a destination of a delivery stream.
 
         Implementers should use this method to grant processor invocation permissions to the provided stream and return the
         necessary configuration to register as a processor.
 
         :param _scope: -
         :param role: (experimental) The IAM role assumed by Kinesis Data Firehose to write to the destination that this DataProcessor will bind to.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d5ab51e341f9a14a9cabc6a1c4031e599b81834c9b42a486091b78758471db6d)
-            check_type(argname="argument _scope", value=_scope, expected_type=type_hints["_scope"])
         options = DataProcessorBindOptions(role=role)
 
         return typing.cast(DataProcessorConfig, jsii.invoke(self, "bind", [_scope, options]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="props")
     def props(self) -> DataProcessorProps:
         '''(experimental) The constructor props of the LambdaFunctionProcessor.
 
         :stability: experimental
         '''
         return typing.cast(DataProcessorProps, jsii.get(self, "props"))
@@ -2243,24 +2358,24 @@
 
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
         # destination: firehose.IDestination
-        # SSE with an customer-managed key that is explicitly specified
+        # SSE with an customer-managed CMK that is explicitly specified
         # key: kms.Key
         
         
-        # SSE with an AWS-owned key
+        # SSE with an AWS-owned CMK
         firehose.DeliveryStream(self, "Delivery Stream AWS Owned",
             encryption=firehose.StreamEncryption.AWS_OWNED,
             destinations=[destination]
         )
-        # SSE with an customer-managed key that is created automatically by the CDK
+        # SSE with an customer-managed CMK that is created automatically by the CDK
         firehose.DeliveryStream(self, "Delivery Stream Implicit Customer Managed",
             encryption=firehose.StreamEncryption.CUSTOMER_MANAGED,
             destinations=[destination]
         )
         firehose.DeliveryStream(self, "Delivery Stream Explicit Customer Managed",
             encryption_key=key,
             destinations=[destination]
@@ -2282,484 +2397,458 @@
 
     :stability: experimental
     '''
 
 
 @jsii.implements(IDeliveryStream)
 class DeliveryStream(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-kinesisfirehose-alpha.DeliveryStream",
 ):
     '''(experimental) Create a Kinesis Data Firehose delivery stream.
 
     :stability: experimental
-    :resource: AWS::KinesisFirehose::DeliveryStream
     :exampleMetadata: infused
+    :resource: AWS::KinesisFirehose::DeliveryStream
 
     Example::
 
-        # Specify the roles created above when defining the destination and delivery stream.
         # bucket: s3.Bucket
-        # Create service roles for the delivery stream and destination.
-        # These can be used for other purposes and granted access to different resources.
-        # They must include the Kinesis Data Firehose service principal in their trust policies.
-        # Two separate roles are shown below, but the same role can be used for both purposes.
-        delivery_stream_role = iam.Role(self, "Delivery Stream Role",
-            assumed_by=iam.ServicePrincipal("firehose.amazonaws.com")
+        # Provide a Lambda function that will transform records before delivery, with custom
+        # buffering and retry configuration
+        lambda_function = lambda_.Function(self, "Processor",
+            runtime=lambda_.Runtime.NODEJS_12_X,
+            handler="index.handler",
+            code=lambda_.Code.from_asset(path.join(__dirname, "process-records"))
+        )
+        lambda_processor = firehose.LambdaFunctionProcessor(lambda_function,
+            buffer_interval=Duration.minutes(5),
+            buffer_size=Size.mebibytes(5),
+            retries=5
         )
-        destination_role = iam.Role(self, "Destination Role",
-            assumed_by=iam.ServicePrincipal("firehose.amazonaws.com")
+        s3_destination = destinations.S3Bucket(bucket,
+            processor=lambda_processor
         )
-        destination = destinations.S3Bucket(bucket, role=destination_role)
         firehose.DeliveryStream(self, "Delivery Stream",
-            destinations=[destination],
-            role=delivery_stream_role
+            destinations=[s3_destination]
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         destinations: typing.Sequence[IDestination],
         delivery_stream_name: typing.Optional[builtins.str] = None,
         encryption: typing.Optional[StreamEncryption] = None,
-        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-        role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-        source_stream: typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.IStream] = None,
+        encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
+        role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
+        source_stream: typing.Optional[aws_cdk.aws_kinesis.IStream] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param destinations: (experimental) The destinations that this delivery stream will deliver data to. Only a singleton array is supported at this time.
         :param delivery_stream_name: (experimental) A name for the delivery stream. Default: - a name is generated by CloudFormation.
         :param encryption: (experimental) Indicates the type of customer master key (CMK) to use for server-side encryption, if any. Default: StreamEncryption.UNENCRYPTED - unless ``encryptionKey`` is provided, in which case this will be implicitly set to ``StreamEncryption.CUSTOMER_MANAGED``
         :param encryption_key: (experimental) Customer managed key to server-side encrypt data in the stream. Default: - no KMS key will be used; if ``encryption`` is set to ``CUSTOMER_MANAGED``, a KMS key will be created for you
         :param role: (experimental) The IAM role associated with this delivery stream. Assumed by Kinesis Data Firehose to read from sources and encrypt data server-side. Default: - a role will be created with default permissions.
         :param source_stream: (experimental) The Kinesis data stream to use as a source for this delivery stream. Default: - data must be written to the delivery stream via a direct put.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__208f5c89209d3c20b3a3c0084efb06d5b736bd75af4a592867db25f4a68945e0)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = DeliveryStreamProps(
             destinations=destinations,
             delivery_stream_name=delivery_stream_name,
             encryption=encryption,
             encryption_key=encryption_key,
             role=role,
             source_stream=source_stream,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromDeliveryStreamArn")
+    @jsii.member(jsii_name="fromDeliveryStreamArn") # type: ignore[misc]
     @builtins.classmethod
     def from_delivery_stream_arn(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         delivery_stream_arn: builtins.str,
     ) -> IDeliveryStream:
         '''(experimental) Import an existing delivery stream from its ARN.
 
         :param scope: -
         :param id: -
         :param delivery_stream_arn: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8e9fcc25a75b7a9f5bc9babea310bb6c89fb28bda587f324f1e0fc18ad762f10)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument delivery_stream_arn", value=delivery_stream_arn, expected_type=type_hints["delivery_stream_arn"])
         return typing.cast(IDeliveryStream, jsii.sinvoke(cls, "fromDeliveryStreamArn", [scope, id, delivery_stream_arn]))
 
-    @jsii.member(jsii_name="fromDeliveryStreamAttributes")
+    @jsii.member(jsii_name="fromDeliveryStreamAttributes") # type: ignore[misc]
     @builtins.classmethod
     def from_delivery_stream_attributes(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         delivery_stream_arn: typing.Optional[builtins.str] = None,
         delivery_stream_name: typing.Optional[builtins.str] = None,
-        role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
     ) -> IDeliveryStream:
         '''(experimental) Import an existing delivery stream from its attributes.
 
         :param scope: -
         :param id: -
         :param delivery_stream_arn: (experimental) The ARN of the delivery stream. At least one of deliveryStreamArn and deliveryStreamName must be provided. Default: - derived from ``deliveryStreamName``.
         :param delivery_stream_name: (experimental) The name of the delivery stream. At least one of deliveryStreamName and deliveryStreamArn must be provided. Default: - derived from ``deliveryStreamArn``.
         :param role: (experimental) The IAM role associated with this delivery stream. Assumed by Kinesis Data Firehose to read from sources and encrypt data server-side. Default: - the imported stream cannot be granted access to other resources as an ``iam.IGrantable``.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__15d1ffa9ef82ad136fc3ac357f1408c9cabf573565d041ea53e380db096eb6c0)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         attrs = DeliveryStreamAttributes(
             delivery_stream_arn=delivery_stream_arn,
             delivery_stream_name=delivery_stream_name,
             role=role,
         )
 
         return typing.cast(IDeliveryStream, jsii.sinvoke(cls, "fromDeliveryStreamAttributes", [scope, id, attrs]))
 
-    @jsii.member(jsii_name="fromDeliveryStreamName")
+    @jsii.member(jsii_name="fromDeliveryStreamName") # type: ignore[misc]
     @builtins.classmethod
     def from_delivery_stream_name(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         delivery_stream_name: builtins.str,
     ) -> IDeliveryStream:
         '''(experimental) Import an existing delivery stream from its name.
 
         :param scope: -
         :param id: -
         :param delivery_stream_name: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__168d683020312f2b15764cdc25a6be82817b2514d1c2b88155f00def1ad9c568)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument delivery_stream_name", value=delivery_stream_name, expected_type=type_hints["delivery_stream_name"])
         return typing.cast(IDeliveryStream, jsii.sinvoke(cls, "fromDeliveryStreamName", [scope, id, delivery_stream_name]))
 
     @jsii.member(jsii_name="grant")
     def grant(
         self,
-        grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
+        grantee: aws_cdk.aws_iam.IGrantable,
         *actions: builtins.str,
-    ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
+    ) -> aws_cdk.aws_iam.Grant:
         '''(experimental) Grant the ``grantee`` identity permissions to perform ``actions``.
 
         :param grantee: -
         :param actions: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__515f94ece05e22db1e06d81218142285fb52fd10e8a6d6ee18155b380109775d)
-            check_type(argname="argument grantee", value=grantee, expected_type=type_hints["grantee"])
-            check_type(argname="argument actions", value=actions, expected_type=typing.Tuple[type_hints["actions"], ...]) # pyright: ignore [reportGeneralTypeIssues]
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.Grant, jsii.invoke(self, "grant", [grantee, *actions]))
+        return typing.cast(aws_cdk.aws_iam.Grant, jsii.invoke(self, "grant", [grantee, *actions]))
 
     @jsii.member(jsii_name="grantPutRecords")
     def grant_put_records(
         self,
-        grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-    ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
+        grantee: aws_cdk.aws_iam.IGrantable,
+    ) -> aws_cdk.aws_iam.Grant:
         '''(experimental) Grant the ``grantee`` identity permissions to perform ``firehose:PutRecord`` and ``firehose:PutRecordBatch`` actions on this delivery stream.
 
         :param grantee: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__00e89f089940bed5c1c643dc6b376b126bd05eeb1447a041d52ce0d28a8908bd)
-            check_type(argname="argument grantee", value=grantee, expected_type=type_hints["grantee"])
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.Grant, jsii.invoke(self, "grantPutRecords", [grantee]))
+        return typing.cast(aws_cdk.aws_iam.Grant, jsii.invoke(self, "grantPutRecords", [grantee]))
 
     @jsii.member(jsii_name="metric")
     def metric(
         self,
         metric_name: builtins.str,
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
         '''(experimental) Return the given named metric for this delivery stream.
 
         :param metric_name: -
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
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9c09c95f82beee7d5e89649a93759d6a7c6cc9c416bb7220f83b2f3463dc3b14)
-            check_type(argname="argument metric_name", value=metric_name, expected_type=type_hints["metric_name"])
-        props = _aws_cdk_aws_cloudwatch_ceddda9d.MetricOptions(
+        props = aws_cdk.aws_cloudwatch.MetricOptions(
             account=account,
             color=color,
             dimensions_map=dimensions_map,
             label=label,
             period=period,
             region=region,
             statistic=statistic,
             unit=unit,
         )
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metric", [metric_name, props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metric", [metric_name, props]))
 
     @jsii.member(jsii_name="metricBackupToS3Bytes")
     def metric_backup_to_s3_bytes(
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
         '''(experimental) Metric for the number of bytes delivered to Amazon S3 for backup over the specified time period.
 
         By default, this metric will be calculated as an average over a period of 5 minutes.
 
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
-        props = _aws_cdk_aws_cloudwatch_ceddda9d.MetricOptions(
+        props = aws_cdk.aws_cloudwatch.MetricOptions(
             account=account,
             color=color,
             dimensions_map=dimensions_map,
             label=label,
             period=period,
             region=region,
             statistic=statistic,
             unit=unit,
         )
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricBackupToS3Bytes", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricBackupToS3Bytes", [props]))
 
     @jsii.member(jsii_name="metricBackupToS3DataFreshness")
     def metric_backup_to_s3_data_freshness(
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
         '''(experimental) Metric for the age (from getting into Kinesis Data Firehose to now) of the oldest record in Kinesis Data Firehose.
 
         Any record older than this age has been delivered to the Amazon S3 bucket for backup.
 
         By default, this metric will be calculated as an average over a period of 5 minutes.
 
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
-        props = _aws_cdk_aws_cloudwatch_ceddda9d.MetricOptions(
+        props = aws_cdk.aws_cloudwatch.MetricOptions(
             account=account,
             color=color,
             dimensions_map=dimensions_map,
             label=label,
             period=period,
             region=region,
             statistic=statistic,
             unit=unit,
         )
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricBackupToS3DataFreshness", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricBackupToS3DataFreshness", [props]))
 
     @jsii.member(jsii_name="metricBackupToS3Records")
     def metric_backup_to_s3_records(
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
         '''(experimental) Metric for the number of records delivered to Amazon S3 for backup over the specified time period.
 
         By default, this metric will be calculated as an average over a period of 5 minutes.
 
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
-        props = _aws_cdk_aws_cloudwatch_ceddda9d.MetricOptions(
+        props = aws_cdk.aws_cloudwatch.MetricOptions(
             account=account,
             color=color,
             dimensions_map=dimensions_map,
             label=label,
             period=period,
             region=region,
             statistic=statistic,
             unit=unit,
         )
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricBackupToS3Records", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricBackupToS3Records", [props]))
 
     @jsii.member(jsii_name="metricIncomingBytes")
     def metric_incoming_bytes(
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
         '''(experimental) Metric for the number of bytes ingested successfully into the delivery stream over the specified time period after throttling.
 
         By default, this metric will be calculated as an average over a period of 5 minutes.
 
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
-        props = _aws_cdk_aws_cloudwatch_ceddda9d.MetricOptions(
+        props = aws_cdk.aws_cloudwatch.MetricOptions(
             account=account,
             color=color,
             dimensions_map=dimensions_map,
             label=label,
             period=period,
             region=region,
             statistic=statistic,
             unit=unit,
         )
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricIncomingBytes", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricIncomingBytes", [props]))
 
     @jsii.member(jsii_name="metricIncomingRecords")
     def metric_incoming_records(
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
         '''(experimental) Metric for the number of records ingested successfully into the delivery stream over the specified time period after throttling.
 
         By default, this metric will be calculated as an average over a period of 5 minutes.
 
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
-        props = _aws_cdk_aws_cloudwatch_ceddda9d.MetricOptions(
+        props = aws_cdk.aws_cloudwatch.MetricOptions(
             account=account,
             color=color,
             dimensions_map=dimensions_map,
             label=label,
             period=period,
             region=region,
             statistic=statistic,
             unit=unit,
         )
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricIncomingRecords", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricIncomingRecords", [props]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="connections")
-    def connections(self) -> _aws_cdk_aws_ec2_ceddda9d.Connections:
+    def connections(self) -> aws_cdk.aws_ec2.Connections:
         '''(experimental) Network connections between Kinesis Data Firehose and other resources, i.e. Redshift cluster.
 
         :stability: experimental
         '''
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.Connections, jsii.get(self, "connections"))
+        return typing.cast(aws_cdk.aws_ec2.Connections, jsii.get(self, "connections"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="deliveryStreamArn")
     def delivery_stream_arn(self) -> builtins.str:
         '''(experimental) The ARN of the delivery stream.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "deliveryStreamArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="deliveryStreamName")
     def delivery_stream_name(self) -> builtins.str:
         '''(experimental) The name of the delivery stream.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "deliveryStreamName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="grantPrincipal")
-    def grant_principal(self) -> _aws_cdk_aws_iam_ceddda9d.IPrincipal:
+    def grant_principal(self) -> aws_cdk.aws_iam.IPrincipal:
         '''(experimental) The principal to grant permissions to.
 
         :stability: experimental
         '''
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.IPrincipal, jsii.get(self, "grantPrincipal"))
+        return typing.cast(aws_cdk.aws_iam.IPrincipal, jsii.get(self, "grantPrincipal"))
 
 
 __all__ = [
     "DataProcessorBindOptions",
     "DataProcessorConfig",
     "DataProcessorIdentifier",
     "DataProcessorProps",
@@ -2772,197 +2861,7 @@
     "IDeliveryStream",
     "IDestination",
     "LambdaFunctionProcessor",
     "StreamEncryption",
 ]
 
 publication.publish()
-
-def _typecheckingstub__fb128eca4e7ba1f83c4f0e58098f008795374fee30ada93711dd3b253dad0ef8(
-    *,
-    role: _aws_cdk_aws_iam_ceddda9d.IRole,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__99d8516a4394f7676eff7b29cec88a391ff919bb6bbda458b6e8e06f6ddb7a88(
-    *,
-    processor_identifier: typing.Union[DataProcessorIdentifier, typing.Dict[builtins.str, typing.Any]],
-    processor_type: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__3c5e177461759fec4dd89a5e4a7730bec0e39ea197243fa5f2eceea512a39f24(
-    *,
-    parameter_name: builtins.str,
-    parameter_value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b6f8aa68afc823d87c695ee05759728c85e4023a37cf01cf765a10be84fbcac8(
-    *,
-    buffer_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    buffer_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
-    retries: typing.Optional[jsii.Number] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__5a349f2444857db9da26d39113740e8ab10e954d7aef8340312a07dcb3ca0c72(
-    *,
-    delivery_stream_arn: typing.Optional[builtins.str] = None,
-    delivery_stream_name: typing.Optional[builtins.str] = None,
-    role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__5b9413f788fdc9578de6565f85eb1d6d397a1047293bb85b71a059af7643ba38(
-    *,
-    destinations: typing.Sequence[IDestination],
-    delivery_stream_name: typing.Optional[builtins.str] = None,
-    encryption: typing.Optional[StreamEncryption] = None,
-    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-    role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-    source_stream: typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.IStream] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__173daa2306128c47572263a530e0a02f73aa7e3f60be737ce497d123e3edc32d(
-    *,
-    dependables: typing.Optional[typing.Sequence[_constructs_77d1e7e8.IDependable]] = None,
-    extended_s3_destination_configuration: typing.Optional[typing.Union[_aws_cdk_aws_kinesisfirehose_ceddda9d.CfnDeliveryStream.ExtendedS3DestinationConfigurationProperty, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__22c1e85da04925f59501768e65d47bdfdedeb6e3e0dfcee70ee80c529df93f3a(
-    scope: _constructs_77d1e7e8.Construct,
-    *,
-    role: _aws_cdk_aws_iam_ceddda9d.IRole,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__4e83b2c41b0be3872a96c9d852da78dc5625213352508d0b4a5e81440d9d1a8e(
-    grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-    *actions: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__ce79dffc4fc87d6b02f31af6954926f1cdb38d458bb0706848609d95b5e62915(
-    grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__52389e5ce1f5828630ba548c0c34e45b5f8dfbc1ad4857c9e91cc7ac36dac99f(
-    metric_name: builtins.str,
-    *,
-    account: typing.Optional[builtins.str] = None,
-    color: typing.Optional[builtins.str] = None,
-    dimensions_map: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-    label: typing.Optional[builtins.str] = None,
-    period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    region: typing.Optional[builtins.str] = None,
-    statistic: typing.Optional[builtins.str] = None,
-    unit: typing.Optional[_aws_cdk_aws_cloudwatch_ceddda9d.Unit] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b51d023ede755a18ed86b3caecd01c91773858417bf2e779e934ccc241569676(
-    scope: _constructs_77d1e7e8.Construct,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__55ad5ddd8cb82f7d48b10e7568eedd0f96f6c1002a8170490a68123a94b247e0(
-    lambda_function: _aws_cdk_aws_lambda_ceddda9d.IFunction,
-    *,
-    buffer_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    buffer_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
-    retries: typing.Optional[jsii.Number] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__d5ab51e341f9a14a9cabc6a1c4031e599b81834c9b42a486091b78758471db6d(
-    _scope: _constructs_77d1e7e8.Construct,
-    *,
-    role: _aws_cdk_aws_iam_ceddda9d.IRole,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__208f5c89209d3c20b3a3c0084efb06d5b736bd75af4a592867db25f4a68945e0(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    destinations: typing.Sequence[IDestination],
-    delivery_stream_name: typing.Optional[builtins.str] = None,
-    encryption: typing.Optional[StreamEncryption] = None,
-    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-    role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-    source_stream: typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.IStream] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__8e9fcc25a75b7a9f5bc9babea310bb6c89fb28bda587f324f1e0fc18ad762f10(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    delivery_stream_arn: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__15d1ffa9ef82ad136fc3ac357f1408c9cabf573565d041ea53e380db096eb6c0(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    delivery_stream_arn: typing.Optional[builtins.str] = None,
-    delivery_stream_name: typing.Optional[builtins.str] = None,
-    role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__168d683020312f2b15764cdc25a6be82817b2514d1c2b88155f00def1ad9c568(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    delivery_stream_name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__515f94ece05e22db1e06d81218142285fb52fd10e8a6d6ee18155b380109775d(
-    grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-    *actions: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__00e89f089940bed5c1c643dc6b376b126bd05eeb1447a041d52ce0d28a8908bd(
-    grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__9c09c95f82beee7d5e89649a93759d6a7c6cc9c416bb7220f83b2f3463dc3b14(
-    metric_name: builtins.str,
-    *,
-    account: typing.Optional[builtins.str] = None,
-    color: typing.Optional[builtins.str] = None,
-    dimensions_map: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-    label: typing.Optional[builtins.str] = None,
-    period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    region: typing.Optional[builtins.str] = None,
-    statistic: typing.Optional[builtins.str] = None,
-    unit: typing.Optional[_aws_cdk_aws_cloudwatch_ceddda9d.Unit] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
```

### Comparing `aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-kinesisfirehose-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::KinesisFirehose
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
 
 # Amazon Kinesis Data Firehose Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -44,15 +44,15 @@
 [Amazon Kinesis Data Firehose](https://docs.aws.amazon.com/firehose/latest/dev/what-is-this-service.html)
 is a service for fully-managed delivery of real-time streaming data to storage services
 such as Amazon S3, Amazon Redshift, Amazon Elasticsearch, Splunk, or any custom HTTP
 endpoint or third-party services such as Datadog, Dynatrace, LogicMonitor, MongoDB, New
 Relic, and Sumo Logic.
 
 Kinesis Data Firehose delivery streams are distinguished from Kinesis data streams in
-their models of consumption. Whereas consumers read from a data stream by actively pulling
+their models of consumtpion. Whereas consumers read from a data stream by actively pulling
 data from the stream, a delivery stream pushes data to its destination on a regular
 cadence. This means that data streams are intended to have consumers that do on-demand
 processing, like AWS Lambda or Amazon EC2. On the other hand, delivery streams are
 intended to have destinations that are sources for offline processing and analytics, such
 as Amazon S3 and Amazon Redshift.
 
 This module is part of the [AWS Cloud Development Kit](https://github.com/aws/aws-cdk)
@@ -99,16 +99,16 @@
     source_stream=source_stream,
     destinations=[destination]
 )
 ```
 
 ### Direct Put
 
-Data must be provided via "direct put", ie., by using a `PutRecord` or
-`PutRecordBatch` API call. There are a number of ways of doing so, such as:
+Data must be provided via "direct put", ie., by using a `PutRecord` or `PutRecordBatch` API call. There are a number of ways of doing
+so, such as:
 
 * Kinesis Agent: a standalone Java application that monitors and delivers files while
   handling file rotation, checkpointing, and retries. See: [Writing to Kinesis Data Firehose Using Kinesis Agent](https://docs.aws.amazon.com/firehose/latest/dev/writing-with-agents.html)
   in the *Kinesis Data Firehose Developer Guide*.
 * AWS SDK: a general purpose solution that allows you to deliver data to a delivery stream
   from anywhere using Java, .NET, Node.js, Python, or Ruby. See: [Writing to Kinesis Data Firehose Using the AWS SDK](https://docs.aws.amazon.com/firehose/latest/dev/writing-with-sdk.html)
   in the *Kinesis Data Firehose Developer Guide*.
@@ -135,100 +135,99 @@
 s3_destination = destinations.S3Bucket(bucket)
 
 firehose.DeliveryStream(self, "Delivery Stream",
     destinations=[s3_destination]
 )
 ```
 
-The S3 destination also supports custom dynamic prefixes. `dataOutputPrefix`
-will be used for files successfully delivered to S3. `errorOutputPrefix` will be added to
-failed records before writing them to S3.
+The S3 destination also supports custom dynamic prefixes. `prefix` will be used for files
+successfully delivered to S3. `errorOutputPrefix` will be added to failed records before
+writing them to S3.
 
 ```python
 # bucket: s3.Bucket
 
 s3_destination = destinations.S3Bucket(bucket,
     data_output_prefix="myFirehose/DeliveredYear=!{timestamp:yyyy}/anyMonth/rand=!{firehose:random-string}",
     error_output_prefix="myFirehoseFailures/!{firehose:error-output-type}/!{timestamp:yyyy}/anyMonth/!{timestamp:dd}"
 )
 ```
 
-See: [Custom S3 Prefixes](https://docs.aws.amazon.com/firehose/latest/dev/s3-prefixes.html)
-in the *Kinesis Data Firehose Developer Guide*.
+See: [Custom S3 Prefixes](https://docs.aws.amazon.com/firehose/latest/dev/s3-prefixes.html) in the *Kinesis Data Firehose Developer Guide*.
 
 ## Server-side Encryption
 
 Enabling server-side encryption (SSE) requires Kinesis Data Firehose to encrypt all data
 sent to delivery stream when it is stored at rest. This means that data is encrypted
 before being written to the service's internal storage layer and decrypted after it is
 received from the internal storage layer. The service manages keys and cryptographic
 operations so that sources and destinations do not need to, as the data is encrypted and
-decrypted at the boundaries of the service (i.e., before the data is delivered to a
+decrypted at the boundaries of the service (ie., before the data is delivered to a
 destination). By default, delivery streams do not have SSE enabled.
 
-The Key Management Service keys (KMS keys) used for SSE can either be AWS-owned or
-customer-managed. AWS-owned KMS keys are created, owned and managed by AWS for use in
-multiple AWS accounts. As a customer, you cannot view, use, track, or manage these keys,
-and you are not charged for their use. On the other hand, customer-managed KMS keys are
-created and owned within your account and managed entirely by you. As a customer, you are
-responsible for managing access, rotation, aliases, and deletion for these keys, and you
-are changed for their use.
-
-See: [AWS KMS keys](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#kms_keys)
+The Key Management Service (KMS) Customer Managed Key (CMK) used for SSE can either be
+AWS-owned or customer-managed. AWS-owned CMKs are keys that an AWS service (in this case
+Kinesis Data Firehose) owns and manages for use in multiple AWS accounts. As a customer,
+you cannot view, use, track, or manage these keys, and you are not charged for their
+use. On the other hand, customer-managed CMKs are keys that are created and owned within
+your account and managed entirely by you. As a customer, you are responsible for managing
+access, rotation, aliases, and deletion for these keys, and you are changed for their
+use. See: [Customer master keys](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#master_keys)
 in the *KMS Developer Guide*.
 
 ```python
 # destination: firehose.IDestination
-# SSE with an customer-managed key that is explicitly specified
+# SSE with an customer-managed CMK that is explicitly specified
 # key: kms.Key
 
 
-# SSE with an AWS-owned key
+# SSE with an AWS-owned CMK
 firehose.DeliveryStream(self, "Delivery Stream AWS Owned",
     encryption=firehose.StreamEncryption.AWS_OWNED,
     destinations=[destination]
 )
-# SSE with an customer-managed key that is created automatically by the CDK
+# SSE with an customer-managed CMK that is created automatically by the CDK
 firehose.DeliveryStream(self, "Delivery Stream Implicit Customer Managed",
     encryption=firehose.StreamEncryption.CUSTOMER_MANAGED,
     destinations=[destination]
 )
 firehose.DeliveryStream(self, "Delivery Stream Explicit Customer Managed",
     encryption_key=key,
     destinations=[destination]
 )
 ```
 
-See: [Data Protection](https://docs.aws.amazon.com/firehose/latest/dev/encryption.html)
-in the *Kinesis Data Firehose Developer Guide*.
+See: [Data Protection](https://docs.aws.amazon.com/firehose/latest/dev/encryption.html) in
+the *Kinesis Data Firehose Developer Guide*.
 
 ## Monitoring
 
 Kinesis Data Firehose is integrated with CloudWatch, so you can monitor the performance of
 your delivery streams via logs and metrics.
 
 ### Logs
 
 Kinesis Data Firehose will send logs to CloudWatch when data transformation or data
 delivery fails. The CDK will enable logging by default and create a CloudWatch LogGroup
 and LogStream for your Delivery Stream.
 
-When you create a destination, you can specify a log group. In this log group, The CDK
-will create log streams where log events will be sent:
+You can provide a specific log group to specify where the CDK will create the log streams
+where log events will be sent:
 
 ```python
 import aws_cdk.aws_logs as logs
 # bucket: s3.Bucket
 
+# destination: firehose.IDestination
+
 
 log_group = logs.LogGroup(self, "Log Group")
 destination = destinations.S3Bucket(bucket,
     log_group=log_group
 )
-
 firehose.DeliveryStream(self, "Delivery Stream",
     destinations=[destination]
 )
 ```
 
 Logging can also be disabled:
 
@@ -261,15 +260,14 @@
 such as `metricIncomingBytes`, and `metricIncomingRecords` (see [`IDeliveryStream`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-kinesisfirehose.IDeliveryStream.html)
 for a full list). CDK also provides a generic `metric` method that can be used to produce
 metric configurations for any metric provided by Kinesis Data Firehose; the configurations
 are pre-populated with the correct dimensions for the delivery stream.
 
 ```python
 import aws_cdk.aws_cloudwatch as cloudwatch
-
 # delivery_stream: firehose.DeliveryStream
 
 
 # Alarm that triggers when the per-second average of incoming bytes exceeds 90% of the current service limit
 incoming_bytes_percent_of_limit = cloudwatch.MathExpression(
     expression="incomingBytes / 300 / bytePerSecLimit",
     using_metrics={
@@ -331,21 +329,20 @@
 ```
 
 See: [Data Delivery Frequency](https://docs.aws.amazon.com/firehose/latest/dev/basic-deliver.html#frequency)
 in the *Kinesis Data Firehose Developer Guide*.
 
 ## Destination Encryption
 
-Your data can be automatically encrypted when it is delivered to S3 as a final or an
-intermediary/backup destination. Kinesis Data Firehose supports Amazon S3 server-side
-encryption with AWS Key Management Service (AWS KMS) for encrypting delivered data in
-Amazon S3. You can choose to not encrypt the data or to encrypt with a key from the list
-of AWS KMS keys that you own. For more information,
-see [Protecting Data Using Server-Side Encryption with AWS KMS–Managed Keys (SSE-KMS)](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingKMSEncryption.html).
-Data is not encrypted by default.
+Your data can be automatically encrypted when it is delivered to S3 as a final or
+an intermediary/backup destination. Kinesis Data Firehose supports Amazon S3 server-side
+encryption with AWS Key Management Service (AWS KMS) for encrypting delivered data
+in Amazon S3. You can choose to not encrypt the data or to encrypt with a key from
+the list of AWS KMS keys that you own. For more information, see [Protecting Data
+Using Server-Side Encryption with AWS KMS–Managed Keys (SSE-KMS)](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingKMSEncryption.html). Data is not encrypted by default.
 
 ```python
 # bucket: s3.Bucket
 # key: kms.Key
 
 destination = destinations.S3Bucket(bucket,
     encryption_key=key
@@ -353,18 +350,18 @@
 firehose.DeliveryStream(self, "Delivery Stream",
     destinations=[destination]
 )
 ```
 
 ## Backup
 
-A delivery stream can be configured to back up data to S3 that it attempted to deliver to
+A delivery stream can be configured to backup data to S3 that it attempted to deliver to
 the configured destination. Backed up data can be all the data that the delivery stream
 attempted to deliver or just data that it failed to deliver (Redshift and S3 destinations
-can only back up all data). CDK can create a new S3 bucket where it will back up data, or
+can only backup all data). CDK can create a new S3 bucket where it will back up data or
 you can provide a bucket where data will be backed up. You can also provide a prefix under
 which your backed-up data will be placed within the bucket. By default, source data is not
 backed up to S3.
 
 ```python
 # Enable backup of all source records (to an S3 bucket created by CDK).
 # bucket: s3.Bucket
@@ -423,26 +420,25 @@
 
 * `recordId` -- the ID of the input record that corresponds the results.
 * `result` -- the status of the transformation of the record: "Ok" (success), "Dropped"
   (not processed intentionally), or "ProcessingFailed" (not processed due to an error).
 * `data` -- the transformed data, Base64-encoded.
 
 The data is buffered up to 1 minute and up to 3 MiB by default before being sent to the
-function, but can be configured using `bufferInterval` and `bufferSize`
-in the processor configuration (see: [Buffering](#buffering)). If the function invocation
-fails due to a network timeout or because of hitting an invocation limit, the invocation
-is retried 3 times by default, but can be configured using `retries` in the processor
-configuration.
+function, but can be configured using `bufferInterval` and `bufferSize` in the processor
+configuration (see: [Buffering](#buffering)). If the function invocation fails due to a
+network timeout or because of hitting an invocation limit, the invocation is retried 3
+times by default, but can be configured using `retries` in the processor configuration.
 
 ```python
 # bucket: s3.Bucket
 # Provide a Lambda function that will transform records before delivery, with custom
 # buffering and retry configuration
 lambda_function = lambda_.Function(self, "Processor",
-    runtime=lambda_.Runtime.NODEJS_14_X,
+    runtime=lambda_.Runtime.NODEJS_12_X,
     handler="index.handler",
     code=lambda_.Code.from_asset(path.join(__dirname, "process-records"))
 )
 lambda_processor = firehose.LambdaFunctionProcessor(lambda_function,
     buffer_interval=Duration.minutes(5),
     buffer_size=Size.mebibytes(5),
     retries=5
@@ -524,14 +520,89 @@
         )
     )]
 )
 
 app.synth()
 ```
 
+!cdk-integ pragma:ignore-assets
+
+```python
+import path as path
+import aws_cdk.aws_kinesisfirehose_alpha as firehose
+import aws_cdk.aws_kms as kms
+import aws_cdk.aws_lambda_nodejs as lambdanodejs
+import aws_cdk.aws_logs as logs
+import aws_cdk.aws_s3 as s3
+import aws_cdk as cdk
+import aws_cdk.aws_kinesisfirehose_destinations_alpha as destinations
+
+app = cdk.App()
+
+stack = cdk.Stack(app, "aws-cdk-firehose-delivery-stream-s3-all-properties")
+
+bucket = s3.Bucket(stack, "Bucket",
+    removal_policy=cdk.RemovalPolicy.DESTROY,
+    auto_delete_objects=True
+)
+
+backup_bucket = s3.Bucket(stack, "BackupBucket",
+    removal_policy=cdk.RemovalPolicy.DESTROY,
+    auto_delete_objects=True
+)
+log_group = logs.LogGroup(stack, "LogGroup",
+    removal_policy=cdk.RemovalPolicy.DESTROY
+)
+
+data_processor_function = lambdanodejs.NodejsFunction(stack, "DataProcessorFunction",
+    entry=path.join(__dirname, "lambda-data-processor.js"),
+    timeout=cdk.Duration.minutes(1)
+)
+
+processor = firehose.LambdaFunctionProcessor(data_processor_function,
+    buffer_interval=cdk.Duration.seconds(60),
+    buffer_size=cdk.Size.mebibytes(1),
+    retries=1
+)
+
+key = kms.Key(stack, "Key",
+    removal_policy=cdk.RemovalPolicy.DESTROY
+)
+
+backup_key = kms.Key(stack, "BackupKey",
+    removal_policy=cdk.RemovalPolicy.DESTROY
+)
+
+firehose.DeliveryStream(stack, "Delivery Stream",
+    destinations=[destinations.S3Bucket(bucket,
+        logging=True,
+        log_group=log_group,
+        processor=processor,
+        compression=destinations.Compression.GZIP,
+        data_output_prefix="regularPrefix",
+        error_output_prefix="errorPrefix",
+        buffering_interval=cdk.Duration.seconds(60),
+        buffering_size=cdk.Size.mebibytes(1),
+        encryption_key=key,
+        s3_backup=destinations.DestinationS3BackupProps(
+            mode=destinations.BackupMode.ALL,
+            bucket=backup_bucket,
+            compression=destinations.Compression.ZIP,
+            data_output_prefix="backupPrefix",
+            error_output_prefix="backupErrorPrefix",
+            buffering_interval=cdk.Duration.seconds(60),
+            buffering_size=cdk.Size.mebibytes(1),
+            encryption_key=backup_key
+        )
+    )]
+)
+
+app.synth()
+```
+
 See: [Data Transformation](https://docs.aws.amazon.com/firehose/latest/dev/data-transformation.html)
 in the *Kinesis Data Firehose Developer Guide*.
 
 ## Specifying an IAM role
 
 The DeliveryStream class automatically creates IAM service roles with all the minimum
 necessary permissions for Kinesis Data Firehose to access the resources referenced by your
@@ -570,15 +641,15 @@
 in the *Kinesis Data Firehose Developer Guide*.
 
 ## Granting application access to a delivery stream
 
 IAM roles, users or groups which need to be able to work with delivery streams should be
 granted IAM permissions.
 
-Any object that implements the `IGrantable` interface (i.e., has an associated principal)
+Any object that implements the `IGrantable` interface (ie., has an associated principal)
 can be granted permissions to a delivery stream by calling:
 
 * `grantPutRecords(principal)` - grants the principal the ability to put records onto the
   delivery stream
 * `grant(principal, ...actions)` - grants the principal permission to a custom set of
   actions
 
@@ -587,16 +658,15 @@
 # delivery_stream: firehose.DeliveryStream
 lambda_role = iam.Role(self, "Role",
     assumed_by=iam.ServicePrincipal("lambda.amazonaws.com")
 )
 delivery_stream.grant_put_records(lambda_role)
 ```
 
-The following write permissions are provided to a service principal by the
-`grantPutRecords()` method:
+The following write permissions are provided to a service principal by the `grantPutRecords()` method:
 
 * `firehose:PutRecord`
 * `firehose:PutRecordBatch`
 
 ## Granting a delivery stream access to a resource
 
 Conversely to the above, Kinesis Data Firehose requires permissions in order for delivery
@@ -618,7 +688,9 @@
 ```
 
 ## Multiple destinations
 
 Though the delivery stream allows specifying an array of destinations, only one
 destination per delivery stream is currently allowed. This limitation is enforced at CDK
 synthesis time and will throw an error.
+
+
```

### Comparing `aws-cdk.aws-kinesisfirehose-alpha-2.84.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/requires.txt
 src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_kinesisfirehose_alpha/__init__.py
 src/aws_cdk/aws_kinesisfirehose_alpha/py.typed
 src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/__init__.py
-src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/aws-kinesisfirehose-alpha@2.84.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/aws-kinesisfirehose-alpha@2.9.0-alpha.0.jsii.tgz
```

