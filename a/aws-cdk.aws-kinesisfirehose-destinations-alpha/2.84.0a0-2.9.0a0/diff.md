# Comparing `tmp/aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0.tar.gz` & `tmp/aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/aws-kinesisfirehose-destinations-alpha/dist/python/aws-cdk.aws-kinesisfire", last modified: Tue Jun 13 23:47:17 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-kinesisfirehose-destinations/dist/python/aws-cdk.aws-kinesi", last modified: Wed Jan 26 11:22:14 2022, max compression
```

## Comparing `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0.tar` & `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:17.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:57.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:47:08.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 23:47:00.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     2185 2023-06-13 23:47:17.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1153 2023-06-13 23:47:08.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:47:08.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:47:17.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2062 2023-06-13 23:47:08.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:17.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:17.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:17.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/
--rw-r--r--   0 root         (0) root         (0)    60963 2023-06-13 23:47:08.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:17.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      530 2023-06-13 23:47:08.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39673 2023-06-13 23:46:57.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/aws-kinesisfirehose-destinations-alpha@2.84.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:47:08.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:17.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2185 2023-06-13 23:47:17.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      741 2023-06-13 23:47:17.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:47:17.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      149 2023-06-13 23:47:17.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:47:17.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:14.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:11.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:11.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:11.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     2152 2022-01-26 11:22:14.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1153 2022-01-26 11:22:11.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:11.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:14.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1986 2022-01-26 11:22:11.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:14.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:14.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:14.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/
+-rw-r--r--   0 root         (0) root         (0)    56190 2022-01-26 11:22:11.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:14.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      494 2022-01-26 11:22:11.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35494 2022-01-26 11:22:11.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/aws-kinesisfirehose-destinations-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:11.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:14.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2152 2022-01-26 11:22:14.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2022-01-26 11:22:14.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:14.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2022-01-26 11:22:14.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:14.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/LICENSE` & `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/LICENSE`

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

### Comparing `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/PKG-INFO` & `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-kinesisfirehose-destinations-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: CDK Destinations Constructs for AWS Kinesis Firehose
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
 
 # Amazon Kinesis Data Firehose Destinations Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -46,7 +46,9 @@
 defining a delivery stream.
 
 See [Amazon Kinesis Data Firehose module README](https://docs.aws.amazon.com/cdk/api/latest/docs/aws-kinesisfirehose-readme.html) for usage examples.
 
 ```python
 import aws_cdk.aws_kinesisfirehose_destinations_alpha as destinations
 ```
+
+
```

### Comparing `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/README.md` & `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/__init__.py` & `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,70 +31,104 @@
 import enum
 import typing
 
 import jsii
 import publication
 import typing_extensions
 
-from typeguard import check_type
-
 from ._jsii import *
 
-import aws_cdk as _aws_cdk_ceddda9d
-import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
-import aws_cdk.aws_kinesisfirehose_alpha as _aws_cdk_aws_kinesisfirehose_alpha_30daaf29
-import aws_cdk.aws_kms as _aws_cdk_aws_kms_ceddda9d
-import aws_cdk.aws_logs as _aws_cdk_aws_logs_ceddda9d
-import aws_cdk.aws_s3 as _aws_cdk_aws_s3_ceddda9d
-import constructs as _constructs_77d1e7e8
+import aws_cdk
+import aws_cdk.aws_iam
+import aws_cdk.aws_kinesisfirehose_alpha
+import aws_cdk.aws_kms
+import aws_cdk.aws_logs
+import aws_cdk.aws_s3
+import constructs
 
 
 @jsii.enum(jsii_type="@aws-cdk/aws-kinesisfirehose-destinations-alpha.BackupMode")
 class BackupMode(enum.Enum):
     '''(experimental) Options for S3 record backup of a delivery stream.
 
     :stability: experimental
-    :exampleMetadata: infused
+    :exampleMetadata: lit=../aws-kinesisfirehose-destinations/test/integ.s3-bucket.lit.ts infused
 
     Example::
 
-        # Enable backup of all source records (to an S3 bucket created by CDK).
-        # bucket: s3.Bucket
-        # Explicitly provide an S3 bucket to which all source records will be backed up.
-        # backup_bucket: s3.Bucket
+        import path as path
+        import aws_cdk.aws_kinesisfirehose_alpha as firehose
+        import aws_cdk.aws_kms as kms
+        import aws_cdk.aws_lambda_nodejs as lambdanodejs
+        import aws_cdk.aws_logs as logs
+        import aws_cdk.aws_s3 as s3
+        import aws_cdk as cdk
+        import aws_cdk.aws_kinesisfirehose_destinations_alpha as destinations
         
-        firehose.DeliveryStream(self, "Delivery Stream Backup All",
-            destinations=[
-                destinations.S3Bucket(bucket,
-                    s3_backup=destinations.DestinationS3BackupProps(
-                        mode=destinations.BackupMode.ALL
-                    )
-                )
-            ]
+        app = cdk.App()
+        
+        stack = cdk.Stack(app, "aws-cdk-firehose-delivery-stream-s3-all-properties")
+        
+        bucket = s3.Bucket(stack, "Bucket",
+            removal_policy=cdk.RemovalPolicy.DESTROY,
+            auto_delete_objects=True
         )
-        firehose.DeliveryStream(self, "Delivery Stream Backup All Explicit Bucket",
-            destinations=[
-                destinations.S3Bucket(bucket,
-                    s3_backup=destinations.DestinationS3BackupProps(
-                        bucket=backup_bucket
-                    )
-                )
-            ]
+        
+        backup_bucket = s3.Bucket(stack, "BackupBucket",
+            removal_policy=cdk.RemovalPolicy.DESTROY,
+            auto_delete_objects=True
         )
-        # Explicitly provide an S3 prefix under which all source records will be backed up.
-        firehose.DeliveryStream(self, "Delivery Stream Backup All Explicit Prefix",
-            destinations=[
-                destinations.S3Bucket(bucket,
-                    s3_backup=destinations.DestinationS3BackupProps(
-                        mode=destinations.BackupMode.ALL,
-                        data_output_prefix="mybackup"
-                    )
+        log_group = logs.LogGroup(stack, "LogGroup",
+            removal_policy=cdk.RemovalPolicy.DESTROY
+        )
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
                 )
-            ]
+            )]
         )
+        
+        app.synth()
     '''
 
     ALL = "ALL"
     '''(experimental) All records are backed up.
 
     :stability: experimental
     '''
@@ -117,18 +151,18 @@
     },
 )
 class CommonDestinationProps:
     def __init__(
         self,
         *,
         logging: typing.Optional[builtins.bool] = None,
-        log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
-        processor: typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDataProcessor] = None,
-        role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-        s3_backup: typing.Optional[typing.Union["DestinationS3BackupProps", typing.Dict[builtins.str, typing.Any]]] = None,
+        log_group: typing.Optional[aws_cdk.aws_logs.ILogGroup] = None,
+        processor: typing.Optional[aws_cdk.aws_kinesisfirehose_alpha.IDataProcessor] = None,
+        role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
+        s3_backup: typing.Optional["DestinationS3BackupProps"] = None,
     ) -> None:
         '''(experimental) Generic properties for defining a delivery stream destination.
 
         :param logging: (experimental) If true, log errors when data transformation or data delivery fails. If ``logGroup`` is provided, this will be implicitly set to ``true``. Default: true - errors are logged.
         :param log_group: (experimental) The CloudWatch log group where log streams will be created to hold error logs. Default: - if ``logging`` is set to ``true``, a log group will be created for you.
         :param processor: (experimental) The data transformation that should be performed on the data before writing to the destination. Default: - no data transformation will occur.
         :param role: (experimental) The IAM role associated with this destination. Assumed by Kinesis Data Firehose to invoke processors and write to destinations Default: - a role will be created with default permissions.
@@ -174,22 +208,15 @@
                     log_group=log_group,
                     mode=kinesisfirehose_destinations_alpha.BackupMode.ALL
                 )
             )
         '''
         if isinstance(s3_backup, dict):
             s3_backup = DestinationS3BackupProps(**s3_backup)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5fbf34f5fd9f20fb9930579dc14faadfa41c4fd4b95d18a03249d155e66990ef)
-            check_type(argname="argument logging", value=logging, expected_type=type_hints["logging"])
-            check_type(argname="argument log_group", value=log_group, expected_type=type_hints["log_group"])
-            check_type(argname="argument processor", value=processor, expected_type=type_hints["processor"])
-            check_type(argname="argument role", value=role, expected_type=type_hints["role"])
-            check_type(argname="argument s3_backup", value=s3_backup, expected_type=type_hints["s3_backup"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if logging is not None:
             self._values["logging"] = logging
         if log_group is not None:
             self._values["log_group"] = log_group
         if processor is not None:
             self._values["processor"] = processor
         if role is not None:
@@ -207,49 +234,49 @@
 
         :stability: experimental
         '''
         result = self._values.get("logging")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def log_group(self) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup]:
+    def log_group(self) -> typing.Optional[aws_cdk.aws_logs.ILogGroup]:
         '''(experimental) The CloudWatch log group where log streams will be created to hold error logs.
 
         :default: - if ``logging`` is set to ``true``, a log group will be created for you.
 
         :stability: experimental
         '''
         result = self._values.get("log_group")
-        return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_logs.ILogGroup], result)
 
     @builtins.property
     def processor(
         self,
-    ) -> typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDataProcessor]:
+    ) -> typing.Optional[aws_cdk.aws_kinesisfirehose_alpha.IDataProcessor]:
         '''(experimental) The data transformation that should be performed on the data before writing to the destination.
 
         :default: - no data transformation will occur.
 
         :stability: experimental
         '''
         result = self._values.get("processor")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDataProcessor], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kinesisfirehose_alpha.IDataProcessor], result)
 
     @builtins.property
-    def role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+    def role(self) -> typing.Optional[aws_cdk.aws_iam.IRole]:
         '''(experimental) The IAM role associated with this destination.
 
         Assumed by Kinesis Data Firehose to invoke processors and write to destinations
 
         :default: - a role will be created with default permissions.
 
         :stability: experimental
         '''
         result = self._values.get("role")
-        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_iam.IRole], result)
 
     @builtins.property
     def s3_backup(self) -> typing.Optional["DestinationS3BackupProps"]:
         '''(experimental) The configuration for backing up source records to S3.
 
         :default: - source records will not be backed up to S3.
 
@@ -282,19 +309,19 @@
         "error_output_prefix": "errorOutputPrefix",
     },
 )
 class CommonDestinationS3Props:
     def __init__(
         self,
         *,
-        buffering_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-        buffering_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
+        buffering_interval: typing.Optional[aws_cdk.Duration] = None,
+        buffering_size: typing.Optional[aws_cdk.Size] = None,
         compression: typing.Optional["Compression"] = None,
         data_output_prefix: typing.Optional[builtins.str] = None,
-        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
         error_output_prefix: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Common properties for defining a backup, intermediary, or final S3 destination for a Kinesis Data Firehose delivery stream.
 
         :param buffering_interval: (experimental) The length of time that Firehose buffers incoming data before delivering it to the S3 bucket. Minimum: Duration.seconds(60) Maximum: Duration.seconds(900) Default: Duration.seconds(300)
         :param buffering_size: (experimental) The size of the buffer that Kinesis Data Firehose uses for incoming data before delivering it to the S3 bucket. Minimum: Size.mebibytes(1) Maximum: Size.mebibytes(128) Default: Size.mebibytes(5)
         :param compression: (experimental) The type of compression that Kinesis Data Firehose uses to compress the data that it delivers to the Amazon S3 bucket. The compression formats SNAPPY or ZIP cannot be specified for Amazon Redshift destinations because they are not supported by the Amazon Redshift COPY operation that reads from the S3 bucket. Default: - UNCOMPRESSED
@@ -322,63 +349,55 @@
                 buffering_size=size,
                 compression=compression,
                 data_output_prefix="dataOutputPrefix",
                 encryption_key=key,
                 error_output_prefix="errorOutputPrefix"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e5f701ffebd736052be12e083983d47077a58d65f5f8d0ea947d4c5c024262de)
-            check_type(argname="argument buffering_interval", value=buffering_interval, expected_type=type_hints["buffering_interval"])
-            check_type(argname="argument buffering_size", value=buffering_size, expected_type=type_hints["buffering_size"])
-            check_type(argname="argument compression", value=compression, expected_type=type_hints["compression"])
-            check_type(argname="argument data_output_prefix", value=data_output_prefix, expected_type=type_hints["data_output_prefix"])
-            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
-            check_type(argname="argument error_output_prefix", value=error_output_prefix, expected_type=type_hints["error_output_prefix"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if buffering_interval is not None:
             self._values["buffering_interval"] = buffering_interval
         if buffering_size is not None:
             self._values["buffering_size"] = buffering_size
         if compression is not None:
             self._values["compression"] = compression
         if data_output_prefix is not None:
             self._values["data_output_prefix"] = data_output_prefix
         if encryption_key is not None:
             self._values["encryption_key"] = encryption_key
         if error_output_prefix is not None:
             self._values["error_output_prefix"] = error_output_prefix
 
     @builtins.property
-    def buffering_interval(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+    def buffering_interval(self) -> typing.Optional[aws_cdk.Duration]:
         '''(experimental) The length of time that Firehose buffers incoming data before delivering it to the S3 bucket.
 
         Minimum: Duration.seconds(60)
         Maximum: Duration.seconds(900)
 
         :default: Duration.seconds(300)
 
         :stability: experimental
         '''
         result = self._values.get("buffering_interval")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
+        return typing.cast(typing.Optional[aws_cdk.Duration], result)
 
     @builtins.property
-    def buffering_size(self) -> typing.Optional[_aws_cdk_ceddda9d.Size]:
+    def buffering_size(self) -> typing.Optional[aws_cdk.Size]:
         '''(experimental) The size of the buffer that Kinesis Data Firehose uses for incoming data before delivering it to the S3 bucket.
 
         Minimum: Size.mebibytes(1)
         Maximum: Size.mebibytes(128)
 
         :default: Size.mebibytes(5)
 
         :stability: experimental
         '''
         result = self._values.get("buffering_size")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Size], result)
+        return typing.cast(typing.Optional[aws_cdk.Size], result)
 
     @builtins.property
     def compression(self) -> typing.Optional["Compression"]:
         '''(experimental) The type of compression that Kinesis Data Firehose uses to compress the data that it delivers to the Amazon S3 bucket.
 
         The compression formats SNAPPY or ZIP cannot be specified for Amazon Redshift
         destinations because they are not supported by the Amazon Redshift COPY operation
@@ -402,23 +421,23 @@
         :see: https://docs.aws.amazon.com/firehose/latest/dev/s3-prefixes.html
         :stability: experimental
         '''
         result = self._values.get("data_output_prefix")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def encryption_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def encryption_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) The AWS KMS key used to encrypt the data that it delivers to your Amazon S3 bucket.
 
         :default: - Data is not encrypted.
 
         :stability: experimental
         '''
         result = self._values.get("encryption_key")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], result)
 
     @builtins.property
     def error_output_prefix(self) -> typing.Optional[builtins.str]:
         '''(experimental) A prefix that Kinesis Data Firehose evaluates and adds to failed records before writing them to S3.
 
         This prefix appears immediately following the bucket name.
 
@@ -445,80 +464,138 @@
 class Compression(
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-kinesisfirehose-destinations-alpha.Compression",
 ):
     '''(experimental) Possible compression options Kinesis Data Firehose can use to compress data on delivery.
 
     :stability: experimental
-    :exampleMetadata: infused
+    :exampleMetadata: lit=../aws-kinesisfirehose-destinations/test/integ.s3-bucket.lit.ts infused
 
     Example::
 
-        # Compress data delivered to S3 using Snappy
-        # bucket: s3.Bucket
+        import path as path
+        import aws_cdk.aws_kinesisfirehose_alpha as firehose
+        import aws_cdk.aws_kms as kms
+        import aws_cdk.aws_lambda_nodejs as lambdanodejs
+        import aws_cdk.aws_logs as logs
+        import aws_cdk.aws_s3 as s3
+        import aws_cdk as cdk
+        import aws_cdk.aws_kinesisfirehose_destinations_alpha as destinations
         
-        s3_destination = destinations.S3Bucket(bucket,
-            compression=destinations.Compression.SNAPPY
+        app = cdk.App()
+        
+        stack = cdk.Stack(app, "aws-cdk-firehose-delivery-stream-s3-all-properties")
+        
+        bucket = s3.Bucket(stack, "Bucket",
+            removal_policy=cdk.RemovalPolicy.DESTROY,
+            auto_delete_objects=True
         )
-        firehose.DeliveryStream(self, "Delivery Stream",
-            destinations=[s3_destination]
+        
+        backup_bucket = s3.Bucket(stack, "BackupBucket",
+            removal_policy=cdk.RemovalPolicy.DESTROY,
+            auto_delete_objects=True
+        )
+        log_group = logs.LogGroup(stack, "LogGroup",
+            removal_policy=cdk.RemovalPolicy.DESTROY
+        )
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
 
-    @jsii.member(jsii_name="of")
+    @jsii.member(jsii_name="of") # type: ignore[misc]
     @builtins.classmethod
     def of(cls, value: builtins.str) -> "Compression":
         '''(experimental) Creates a new Compression instance with a custom value.
 
         :param value: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e108c47faf6b9e464aa8e9a66ffd014aedc1e9b63a2ba129a4fc0c3b14bf13bb)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast("Compression", jsii.sinvoke(cls, "of", [value]))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="GZIP")
     def GZIP(cls) -> "Compression":
         '''(experimental) gzip.
 
         :stability: experimental
         '''
         return typing.cast("Compression", jsii.sget(cls, "GZIP"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="HADOOP_SNAPPY")
     def HADOOP_SNAPPY(cls) -> "Compression":
         '''(experimental) Hadoop-compatible Snappy.
 
         :stability: experimental
         '''
         return typing.cast("Compression", jsii.sget(cls, "HADOOP_SNAPPY"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="SNAPPY")
     def SNAPPY(cls) -> "Compression":
         '''(experimental) Snappy.
 
         :stability: experimental
         '''
         return typing.cast("Compression", jsii.sget(cls, "SNAPPY"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="ZIP")
     def ZIP(cls) -> "Compression":
         '''(experimental) ZIP.
 
         :stability: experimental
         '''
         return typing.cast("Compression", jsii.sget(cls, "ZIP"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="value")
     def value(self) -> builtins.str:
         '''(experimental) the string value of the Compression.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "value"))
@@ -540,23 +617,23 @@
         "mode": "mode",
     },
 )
 class DestinationS3BackupProps(CommonDestinationS3Props):
     def __init__(
         self,
         *,
-        buffering_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-        buffering_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
+        buffering_interval: typing.Optional[aws_cdk.Duration] = None,
+        buffering_size: typing.Optional[aws_cdk.Size] = None,
         compression: typing.Optional[Compression] = None,
         data_output_prefix: typing.Optional[builtins.str] = None,
-        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
         error_output_prefix: typing.Optional[builtins.str] = None,
-        bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
+        bucket: typing.Optional[aws_cdk.aws_s3.IBucket] = None,
         logging: typing.Optional[builtins.bool] = None,
-        log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
+        log_group: typing.Optional[aws_cdk.aws_logs.ILogGroup] = None,
         mode: typing.Optional[BackupMode] = None,
     ) -> None:
         '''(experimental) Properties for defining an S3 backup destination.
 
         S3 backup is available for all destinations, regardless of whether the final destination is S3 or not.
 
         :param buffering_interval: (experimental) The length of time that Firehose buffers incoming data before delivering it to the S3 bucket. Minimum: Duration.seconds(60) Maximum: Duration.seconds(900) Default: Duration.seconds(300)
@@ -567,66 +644,90 @@
         :param error_output_prefix: (experimental) A prefix that Kinesis Data Firehose evaluates and adds to failed records before writing them to S3. This prefix appears immediately following the bucket name. Default: "YYYY/MM/DD/HH"
         :param bucket: (experimental) The S3 bucket that will store data and failed records. Default: - If ``mode`` is set to ``BackupMode.ALL`` or ``BackupMode.FAILED``, a bucket will be created for you.
         :param logging: (experimental) If true, log errors when data transformation or data delivery fails. If ``logGroup`` is provided, this will be implicitly set to ``true``. Default: true - errors are logged.
         :param log_group: (experimental) The CloudWatch log group where log streams will be created to hold error logs. Default: - if ``logging`` is set to ``true``, a log group will be created for you.
         :param mode: (experimental) Indicates the mode by which incoming records should be backed up to S3, if any. If ``bucket`` is provided, this will be implicitly set to ``BackupMode.ALL``. Default: - If ``bucket`` is provided, the default will be ``BackupMode.ALL``. Otherwise, source records are not backed up to S3.
 
         :stability: experimental
-        :exampleMetadata: infused
+        :exampleMetadata: lit=../aws-kinesisfirehose-destinations/test/integ.s3-bucket.lit.ts infused
 
         Example::
 
-            # Enable backup of all source records (to an S3 bucket created by CDK).
-            # bucket: s3.Bucket
-            # Explicitly provide an S3 bucket to which all source records will be backed up.
-            # backup_bucket: s3.Bucket
+            import path as path
+            import aws_cdk.aws_kinesisfirehose_alpha as firehose
+            import aws_cdk.aws_kms as kms
+            import aws_cdk.aws_lambda_nodejs as lambdanodejs
+            import aws_cdk.aws_logs as logs
+            import aws_cdk.aws_s3 as s3
+            import aws_cdk as cdk
+            import aws_cdk.aws_kinesisfirehose_destinations_alpha as destinations
             
-            firehose.DeliveryStream(self, "Delivery Stream Backup All",
-                destinations=[
-                    destinations.S3Bucket(bucket,
-                        s3_backup=destinations.DestinationS3BackupProps(
-                            mode=destinations.BackupMode.ALL
-                        )
-                    )
-                ]
+            app = cdk.App()
+            
+            stack = cdk.Stack(app, "aws-cdk-firehose-delivery-stream-s3-all-properties")
+            
+            bucket = s3.Bucket(stack, "Bucket",
+                removal_policy=cdk.RemovalPolicy.DESTROY,
+                auto_delete_objects=True
             )
-            firehose.DeliveryStream(self, "Delivery Stream Backup All Explicit Bucket",
-                destinations=[
-                    destinations.S3Bucket(bucket,
-                        s3_backup=destinations.DestinationS3BackupProps(
-                            bucket=backup_bucket
-                        )
-                    )
-                ]
+            
+            backup_bucket = s3.Bucket(stack, "BackupBucket",
+                removal_policy=cdk.RemovalPolicy.DESTROY,
+                auto_delete_objects=True
+            )
+            log_group = logs.LogGroup(stack, "LogGroup",
+                removal_policy=cdk.RemovalPolicy.DESTROY
+            )
+            
+            data_processor_function = lambdanodejs.NodejsFunction(stack, "DataProcessorFunction",
+                entry=path.join(__dirname, "lambda-data-processor.js"),
+                timeout=cdk.Duration.minutes(1)
+            )
+            
+            processor = firehose.LambdaFunctionProcessor(data_processor_function,
+                buffer_interval=cdk.Duration.seconds(60),
+                buffer_size=cdk.Size.mebibytes(1),
+                retries=1
             )
-            # Explicitly provide an S3 prefix under which all source records will be backed up.
-            firehose.DeliveryStream(self, "Delivery Stream Backup All Explicit Prefix",
-                destinations=[
-                    destinations.S3Bucket(bucket,
-                        s3_backup=destinations.DestinationS3BackupProps(
-                            mode=destinations.BackupMode.ALL,
-                            data_output_prefix="mybackup"
-                        )
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
                     )
-                ]
+                )]
             )
+            
+            app.synth()
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__30f259649e1b40856d1c00eafb1cce1841fecdcf04d620b61fa0dba28186c0c0)
-            check_type(argname="argument buffering_interval", value=buffering_interval, expected_type=type_hints["buffering_interval"])
-            check_type(argname="argument buffering_size", value=buffering_size, expected_type=type_hints["buffering_size"])
-            check_type(argname="argument compression", value=compression, expected_type=type_hints["compression"])
-            check_type(argname="argument data_output_prefix", value=data_output_prefix, expected_type=type_hints["data_output_prefix"])
-            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
-            check_type(argname="argument error_output_prefix", value=error_output_prefix, expected_type=type_hints["error_output_prefix"])
-            check_type(argname="argument bucket", value=bucket, expected_type=type_hints["bucket"])
-            check_type(argname="argument logging", value=logging, expected_type=type_hints["logging"])
-            check_type(argname="argument log_group", value=log_group, expected_type=type_hints["log_group"])
-            check_type(argname="argument mode", value=mode, expected_type=type_hints["mode"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if buffering_interval is not None:
             self._values["buffering_interval"] = buffering_interval
         if buffering_size is not None:
             self._values["buffering_size"] = buffering_size
         if compression is not None:
             self._values["compression"] = compression
         if data_output_prefix is not None:
@@ -641,40 +742,40 @@
             self._values["logging"] = logging
         if log_group is not None:
             self._values["log_group"] = log_group
         if mode is not None:
             self._values["mode"] = mode
 
     @builtins.property
-    def buffering_interval(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+    def buffering_interval(self) -> typing.Optional[aws_cdk.Duration]:
         '''(experimental) The length of time that Firehose buffers incoming data before delivering it to the S3 bucket.
 
         Minimum: Duration.seconds(60)
         Maximum: Duration.seconds(900)
 
         :default: Duration.seconds(300)
 
         :stability: experimental
         '''
         result = self._values.get("buffering_interval")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
+        return typing.cast(typing.Optional[aws_cdk.Duration], result)
 
     @builtins.property
-    def buffering_size(self) -> typing.Optional[_aws_cdk_ceddda9d.Size]:
+    def buffering_size(self) -> typing.Optional[aws_cdk.Size]:
         '''(experimental) The size of the buffer that Kinesis Data Firehose uses for incoming data before delivering it to the S3 bucket.
 
         Minimum: Size.mebibytes(1)
         Maximum: Size.mebibytes(128)
 
         :default: Size.mebibytes(5)
 
         :stability: experimental
         '''
         result = self._values.get("buffering_size")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Size], result)
+        return typing.cast(typing.Optional[aws_cdk.Size], result)
 
     @builtins.property
     def compression(self) -> typing.Optional[Compression]:
         '''(experimental) The type of compression that Kinesis Data Firehose uses to compress the data that it delivers to the Amazon S3 bucket.
 
         The compression formats SNAPPY or ZIP cannot be specified for Amazon Redshift
         destinations because they are not supported by the Amazon Redshift COPY operation
@@ -698,23 +799,23 @@
         :see: https://docs.aws.amazon.com/firehose/latest/dev/s3-prefixes.html
         :stability: experimental
         '''
         result = self._values.get("data_output_prefix")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def encryption_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def encryption_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) The AWS KMS key used to encrypt the data that it delivers to your Amazon S3 bucket.
 
         :default: - Data is not encrypted.
 
         :stability: experimental
         '''
         result = self._values.get("encryption_key")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], result)
 
     @builtins.property
     def error_output_prefix(self) -> typing.Optional[builtins.str]:
         '''(experimental) A prefix that Kinesis Data Firehose evaluates and adds to failed records before writing them to S3.
 
         This prefix appears immediately following the bucket name.
 
@@ -723,23 +824,23 @@
         :see: https://docs.aws.amazon.com/firehose/latest/dev/s3-prefixes.html
         :stability: experimental
         '''
         result = self._values.get("error_output_prefix")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def bucket(self) -> typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket]:
+    def bucket(self) -> typing.Optional[aws_cdk.aws_s3.IBucket]:
         '''(experimental) The S3 bucket that will store data and failed records.
 
         :default: - If ``mode`` is set to ``BackupMode.ALL`` or ``BackupMode.FAILED``, a bucket will be created for you.
 
         :stability: experimental
         '''
         result = self._values.get("bucket")
-        return typing.cast(typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_s3.IBucket], result)
 
     @builtins.property
     def logging(self) -> typing.Optional[builtins.bool]:
         '''(experimental) If true, log errors when data transformation or data delivery fails.
 
         If ``logGroup`` is provided, this will be implicitly set to ``true``.
 
@@ -747,23 +848,23 @@
 
         :stability: experimental
         '''
         result = self._values.get("logging")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def log_group(self) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup]:
+    def log_group(self) -> typing.Optional[aws_cdk.aws_logs.ILogGroup]:
         '''(experimental) The CloudWatch log group where log streams will be created to hold error logs.
 
         :default: - if ``logging`` is set to ``true``, a log group will be created for you.
 
         :stability: experimental
         '''
         result = self._values.get("log_group")
-        return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_logs.ILogGroup], result)
 
     @builtins.property
     def mode(self) -> typing.Optional[BackupMode]:
         '''(experimental) Indicates the mode by which incoming records should be backed up to S3, if any.
 
         If ``bucket`` is provided, this will be implicitly set to ``BackupMode.ALL``.
 
@@ -785,61 +886,62 @@
 
     def __repr__(self) -> str:
         return "DestinationS3BackupProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-@jsii.implements(_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDestination)
+@jsii.implements(aws_cdk.aws_kinesisfirehose_alpha.IDestination)
 class S3Bucket(
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-kinesisfirehose-destinations-alpha.S3Bucket",
 ):
     '''(experimental) An S3 bucket destination for data from a Kinesis Data Firehose delivery stream.
 
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
-        import aws_cdk.aws_kinesisfirehose_alpha as firehose
-        import aws_cdk.aws_kinesisfirehose_destinations_alpha as destinations
-        
-        
-        bucket = s3.Bucket(self, "MyBucket")
-        stream = firehose.DeliveryStream(self, "MyStream",
-            destinations=[destinations.S3Bucket(bucket)]
+        # bucket: s3.Bucket
+        # Provide a Lambda function that will transform records before delivery, with custom
+        # buffering and retry configuration
+        lambda_function = lambda_.Function(self, "Processor",
+            runtime=lambda_.Runtime.NODEJS_12_X,
+            handler="index.handler",
+            code=lambda_.Code.from_asset(path.join(__dirname, "process-records"))
         )
-        
-        topic_rule = iot.TopicRule(self, "TopicRule",
-            sql=iot.IotSql.from_string_as_ver20160323("SELECT * FROM 'device/+/data'"),
-            actions=[
-                actions.FirehosePutRecordAction(stream,
-                    batch_mode=True,
-                    record_separator=actions.FirehoseRecordSeparator.NEWLINE
-                )
-            ]
+        lambda_processor = firehose.LambdaFunctionProcessor(lambda_function,
+            buffer_interval=Duration.minutes(5),
+            buffer_size=Size.mebibytes(5),
+            retries=5
+        )
+        s3_destination = destinations.S3Bucket(bucket,
+            processor=lambda_processor
+        )
+        firehose.DeliveryStream(self, "Delivery Stream",
+            destinations=[s3_destination]
         )
     '''
 
     def __init__(
         self,
-        bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        bucket: aws_cdk.aws_s3.IBucket,
         *,
-        buffering_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-        buffering_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
+        buffering_interval: typing.Optional[aws_cdk.Duration] = None,
+        buffering_size: typing.Optional[aws_cdk.Size] = None,
         compression: typing.Optional[Compression] = None,
         data_output_prefix: typing.Optional[builtins.str] = None,
-        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
         error_output_prefix: typing.Optional[builtins.str] = None,
         logging: typing.Optional[builtins.bool] = None,
-        log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
-        processor: typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDataProcessor] = None,
-        role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-        s3_backup: typing.Optional[typing.Union[DestinationS3BackupProps, typing.Dict[builtins.str, typing.Any]]] = None,
+        log_group: typing.Optional[aws_cdk.aws_logs.ILogGroup] = None,
+        processor: typing.Optional[aws_cdk.aws_kinesisfirehose_alpha.IDataProcessor] = None,
+        role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
+        s3_backup: typing.Optional[DestinationS3BackupProps] = None,
     ) -> None:
         '''
         :param bucket: -
         :param buffering_interval: (experimental) The length of time that Firehose buffers incoming data before delivering it to the S3 bucket. Minimum: Duration.seconds(60) Maximum: Duration.seconds(900) Default: Duration.seconds(300)
         :param buffering_size: (experimental) The size of the buffer that Kinesis Data Firehose uses for incoming data before delivering it to the S3 bucket. Minimum: Size.mebibytes(1) Maximum: Size.mebibytes(128) Default: Size.mebibytes(5)
         :param compression: (experimental) The type of compression that Kinesis Data Firehose uses to compress the data that it delivers to the Amazon S3 bucket. The compression formats SNAPPY or ZIP cannot be specified for Amazon Redshift destinations because they are not supported by the Amazon Redshift COPY operation that reads from the S3 bucket. Default: - UNCOMPRESSED
         :param data_output_prefix: (experimental) A prefix that Kinesis Data Firehose evaluates and adds to records before writing them to S3. This prefix appears immediately following the bucket name. Default: "YYYY/MM/DD/HH"
@@ -849,17 +951,14 @@
         :param log_group: (experimental) The CloudWatch log group where log streams will be created to hold error logs. Default: - if ``logging`` is set to ``true``, a log group will be created for you.
         :param processor: (experimental) The data transformation that should be performed on the data before writing to the destination. Default: - no data transformation will occur.
         :param role: (experimental) The IAM role associated with this destination. Assumed by Kinesis Data Firehose to invoke processors and write to destinations Default: - a role will be created with default permissions.
         :param s3_backup: (experimental) The configuration for backing up source records to S3. Default: - source records will not be backed up to S3.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fe5ecd705abd98d6ae1981009987f3ed192f69f3f1e4484dfa7f074faf45e2f0)
-            check_type(argname="argument bucket", value=bucket, expected_type=type_hints["bucket"])
         props = S3BucketProps(
             buffering_interval=buffering_interval,
             buffering_size=buffering_size,
             compression=compression,
             data_output_prefix=data_output_prefix,
             encryption_key=encryption_key,
             error_output_prefix=error_output_prefix,
@@ -871,30 +970,27 @@
         )
 
         jsii.create(self.__class__, self, [bucket, props])
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
-        scope: _constructs_77d1e7e8.Construct,
-    ) -> _aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DestinationConfig:
-        '''(experimental) Binds this destination to the Kinesis Data Firehose delivery stream.
+        scope: constructs.Construct,
+    ) -> aws_cdk.aws_kinesisfirehose_alpha.DestinationConfig:
+        '''(experimental) (experimental) Binds this destination to the Kinesis Data Firehose delivery stream.
 
         Implementers should use this method to bind resources to the stack and initialize values using the provided stream.
 
         :param scope: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7ef57681cdd36f8cd198608780e9bd1ba808f38c351f3aa6968c6410a4ce0e15)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-        _options = _aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DestinationBindOptions()
+        _options = aws_cdk.aws_kinesisfirehose_alpha.DestinationBindOptions()
 
-        return typing.cast(_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DestinationConfig, jsii.invoke(self, "bind", [scope, _options]))
+        return typing.cast(aws_cdk.aws_kinesisfirehose_alpha.DestinationConfig, jsii.invoke(self, "bind", [scope, _options]))
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-kinesisfirehose-destinations-alpha.S3BucketProps",
     jsii_struct_bases=[CommonDestinationS3Props, CommonDestinationProps],
     name_mapping={
         "buffering_interval": "bufferingInterval",
@@ -910,25 +1006,25 @@
         "s3_backup": "s3Backup",
     },
 )
 class S3BucketProps(CommonDestinationS3Props, CommonDestinationProps):
     def __init__(
         self,
         *,
-        buffering_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-        buffering_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
+        buffering_interval: typing.Optional[aws_cdk.Duration] = None,
+        buffering_size: typing.Optional[aws_cdk.Size] = None,
         compression: typing.Optional[Compression] = None,
         data_output_prefix: typing.Optional[builtins.str] = None,
-        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
         error_output_prefix: typing.Optional[builtins.str] = None,
         logging: typing.Optional[builtins.bool] = None,
-        log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
-        processor: typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDataProcessor] = None,
-        role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-        s3_backup: typing.Optional[typing.Union[DestinationS3BackupProps, typing.Dict[builtins.str, typing.Any]]] = None,
+        log_group: typing.Optional[aws_cdk.aws_logs.ILogGroup] = None,
+        processor: typing.Optional[aws_cdk.aws_kinesisfirehose_alpha.IDataProcessor] = None,
+        role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
+        s3_backup: typing.Optional[DestinationS3BackupProps] = None,
     ) -> None:
         '''(experimental) Props for defining an S3 destination of a Kinesis Data Firehose delivery stream.
 
         :param buffering_interval: (experimental) The length of time that Firehose buffers incoming data before delivering it to the S3 bucket. Minimum: Duration.seconds(60) Maximum: Duration.seconds(900) Default: Duration.seconds(300)
         :param buffering_size: (experimental) The size of the buffer that Kinesis Data Firehose uses for incoming data before delivering it to the S3 bucket. Minimum: Size.mebibytes(1) Maximum: Size.mebibytes(128) Default: Size.mebibytes(5)
         :param compression: (experimental) The type of compression that Kinesis Data Firehose uses to compress the data that it delivers to the Amazon S3 bucket. The compression formats SNAPPY or ZIP cannot be specified for Amazon Redshift destinations because they are not supported by the Amazon Redshift COPY operation that reads from the S3 bucket. Default: - UNCOMPRESSED
         :param data_output_prefix: (experimental) A prefix that Kinesis Data Firehose evaluates and adds to records before writing them to S3. This prefix appears immediately following the bucket name. Default: "YYYY/MM/DD/HH"
@@ -945,15 +1041,15 @@
 
         Example::
 
             # bucket: s3.Bucket
             # Provide a Lambda function that will transform records before delivery, with custom
             # buffering and retry configuration
             lambda_function = lambda_.Function(self, "Processor",
-                runtime=lambda_.Runtime.NODEJS_14_X,
+                runtime=lambda_.Runtime.NODEJS_12_X,
                 handler="index.handler",
                 code=lambda_.Code.from_asset(path.join(__dirname, "process-records"))
             )
             lambda_processor = firehose.LambdaFunctionProcessor(lambda_function,
                 buffer_interval=Duration.minutes(5),
                 buffer_size=Size.mebibytes(5),
                 retries=5
@@ -963,28 +1059,15 @@
             )
             firehose.DeliveryStream(self, "Delivery Stream",
                 destinations=[s3_destination]
             )
         '''
         if isinstance(s3_backup, dict):
             s3_backup = DestinationS3BackupProps(**s3_backup)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7f66c30b3ff0515262c7b17582f885e7605828274db0d3352d72b5ee8ace4cd7)
-            check_type(argname="argument buffering_interval", value=buffering_interval, expected_type=type_hints["buffering_interval"])
-            check_type(argname="argument buffering_size", value=buffering_size, expected_type=type_hints["buffering_size"])
-            check_type(argname="argument compression", value=compression, expected_type=type_hints["compression"])
-            check_type(argname="argument data_output_prefix", value=data_output_prefix, expected_type=type_hints["data_output_prefix"])
-            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
-            check_type(argname="argument error_output_prefix", value=error_output_prefix, expected_type=type_hints["error_output_prefix"])
-            check_type(argname="argument logging", value=logging, expected_type=type_hints["logging"])
-            check_type(argname="argument log_group", value=log_group, expected_type=type_hints["log_group"])
-            check_type(argname="argument processor", value=processor, expected_type=type_hints["processor"])
-            check_type(argname="argument role", value=role, expected_type=type_hints["role"])
-            check_type(argname="argument s3_backup", value=s3_backup, expected_type=type_hints["s3_backup"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if buffering_interval is not None:
             self._values["buffering_interval"] = buffering_interval
         if buffering_size is not None:
             self._values["buffering_size"] = buffering_size
         if compression is not None:
             self._values["compression"] = compression
         if data_output_prefix is not None:
@@ -1001,40 +1084,40 @@
             self._values["processor"] = processor
         if role is not None:
             self._values["role"] = role
         if s3_backup is not None:
             self._values["s3_backup"] = s3_backup
 
     @builtins.property
-    def buffering_interval(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+    def buffering_interval(self) -> typing.Optional[aws_cdk.Duration]:
         '''(experimental) The length of time that Firehose buffers incoming data before delivering it to the S3 bucket.
 
         Minimum: Duration.seconds(60)
         Maximum: Duration.seconds(900)
 
         :default: Duration.seconds(300)
 
         :stability: experimental
         '''
         result = self._values.get("buffering_interval")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
+        return typing.cast(typing.Optional[aws_cdk.Duration], result)
 
     @builtins.property
-    def buffering_size(self) -> typing.Optional[_aws_cdk_ceddda9d.Size]:
+    def buffering_size(self) -> typing.Optional[aws_cdk.Size]:
         '''(experimental) The size of the buffer that Kinesis Data Firehose uses for incoming data before delivering it to the S3 bucket.
 
         Minimum: Size.mebibytes(1)
         Maximum: Size.mebibytes(128)
 
         :default: Size.mebibytes(5)
 
         :stability: experimental
         '''
         result = self._values.get("buffering_size")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Size], result)
+        return typing.cast(typing.Optional[aws_cdk.Size], result)
 
     @builtins.property
     def compression(self) -> typing.Optional[Compression]:
         '''(experimental) The type of compression that Kinesis Data Firehose uses to compress the data that it delivers to the Amazon S3 bucket.
 
         The compression formats SNAPPY or ZIP cannot be specified for Amazon Redshift
         destinations because they are not supported by the Amazon Redshift COPY operation
@@ -1058,23 +1141,23 @@
         :see: https://docs.aws.amazon.com/firehose/latest/dev/s3-prefixes.html
         :stability: experimental
         '''
         result = self._values.get("data_output_prefix")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def encryption_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def encryption_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) The AWS KMS key used to encrypt the data that it delivers to your Amazon S3 bucket.
 
         :default: - Data is not encrypted.
 
         :stability: experimental
         '''
         result = self._values.get("encryption_key")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], result)
 
     @builtins.property
     def error_output_prefix(self) -> typing.Optional[builtins.str]:
         '''(experimental) A prefix that Kinesis Data Firehose evaluates and adds to failed records before writing them to S3.
 
         This prefix appears immediately following the bucket name.
 
@@ -1096,49 +1179,49 @@
 
         :stability: experimental
         '''
         result = self._values.get("logging")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def log_group(self) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup]:
+    def log_group(self) -> typing.Optional[aws_cdk.aws_logs.ILogGroup]:
         '''(experimental) The CloudWatch log group where log streams will be created to hold error logs.
 
         :default: - if ``logging`` is set to ``true``, a log group will be created for you.
 
         :stability: experimental
         '''
         result = self._values.get("log_group")
-        return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_logs.ILogGroup], result)
 
     @builtins.property
     def processor(
         self,
-    ) -> typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDataProcessor]:
+    ) -> typing.Optional[aws_cdk.aws_kinesisfirehose_alpha.IDataProcessor]:
         '''(experimental) The data transformation that should be performed on the data before writing to the destination.
 
         :default: - no data transformation will occur.
 
         :stability: experimental
         '''
         result = self._values.get("processor")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDataProcessor], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kinesisfirehose_alpha.IDataProcessor], result)
 
     @builtins.property
-    def role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+    def role(self) -> typing.Optional[aws_cdk.aws_iam.IRole]:
         '''(experimental) The IAM role associated with this destination.
 
         Assumed by Kinesis Data Firehose to invoke processors and write to destinations
 
         :default: - a role will be created with default permissions.
 
         :stability: experimental
         '''
         result = self._values.get("role")
-        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_iam.IRole], result)
 
     @builtins.property
     def s3_backup(self) -> typing.Optional[DestinationS3BackupProps]:
         '''(experimental) The configuration for backing up source records to S3.
 
         :default: - source records will not be backed up to S3.
 
@@ -1166,93 +1249,7 @@
     "Compression",
     "DestinationS3BackupProps",
     "S3Bucket",
     "S3BucketProps",
 ]
 
 publication.publish()
-
-def _typecheckingstub__5fbf34f5fd9f20fb9930579dc14faadfa41c4fd4b95d18a03249d155e66990ef(
-    *,
-    logging: typing.Optional[builtins.bool] = None,
-    log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
-    processor: typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDataProcessor] = None,
-    role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-    s3_backup: typing.Optional[typing.Union[DestinationS3BackupProps, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e5f701ffebd736052be12e083983d47077a58d65f5f8d0ea947d4c5c024262de(
-    *,
-    buffering_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    buffering_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
-    compression: typing.Optional[Compression] = None,
-    data_output_prefix: typing.Optional[builtins.str] = None,
-    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-    error_output_prefix: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e108c47faf6b9e464aa8e9a66ffd014aedc1e9b63a2ba129a4fc0c3b14bf13bb(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__30f259649e1b40856d1c00eafb1cce1841fecdcf04d620b61fa0dba28186c0c0(
-    *,
-    buffering_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    buffering_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
-    compression: typing.Optional[Compression] = None,
-    data_output_prefix: typing.Optional[builtins.str] = None,
-    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-    error_output_prefix: typing.Optional[builtins.str] = None,
-    bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
-    logging: typing.Optional[builtins.bool] = None,
-    log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
-    mode: typing.Optional[BackupMode] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__fe5ecd705abd98d6ae1981009987f3ed192f69f3f1e4484dfa7f074faf45e2f0(
-    bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
-    *,
-    buffering_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    buffering_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
-    compression: typing.Optional[Compression] = None,
-    data_output_prefix: typing.Optional[builtins.str] = None,
-    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-    error_output_prefix: typing.Optional[builtins.str] = None,
-    logging: typing.Optional[builtins.bool] = None,
-    log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
-    processor: typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDataProcessor] = None,
-    role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-    s3_backup: typing.Optional[typing.Union[DestinationS3BackupProps, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__7ef57681cdd36f8cd198608780e9bd1ba808f38c351f3aa6968c6410a4ce0e15(
-    scope: _constructs_77d1e7e8.Construct,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__7f66c30b3ff0515262c7b17582f885e7605828274db0d3352d72b5ee8ace4cd7(
-    *,
-    buffering_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    buffering_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
-    compression: typing.Optional[Compression] = None,
-    data_output_prefix: typing.Optional[builtins.str] = None,
-    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-    error_output_prefix: typing.Optional[builtins.str] = None,
-    logging: typing.Optional[builtins.bool] = None,
-    log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
-    processor: typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDataProcessor] = None,
-    role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-    s3_backup: typing.Optional[typing.Union[DestinationS3BackupProps, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
```

### Comparing `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-kinesisfirehose-destinations-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: CDK Destinations Constructs for AWS Kinesis Firehose
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
 
 # Amazon Kinesis Data Firehose Destinations Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -46,7 +46,9 @@
 defining a delivery stream.
 
 See [Amazon Kinesis Data Firehose module README](https://docs.aws.amazon.com/cdk/api/latest/docs/aws-kinesisfirehose-readme.html) for usage examples.
 
 ```python
 import aws_cdk.aws_kinesisfirehose_destinations_alpha as destinations
 ```
+
+
```

### Comparing `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.84.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.9.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/requires.txt
 src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_kinesisfirehose_destinations_alpha/__init__.py
 src/aws_cdk/aws_kinesisfirehose_destinations_alpha/py.typed
 src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/__init__.py
-src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/aws-kinesisfirehose-destinations-alpha@2.84.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/aws-kinesisfirehose-destinations-alpha@2.9.0-alpha.0.jsii.tgz
```

