# Comparing `tmp/aws-cdk.aws-glue-alpha-2.84.0a0.tar.gz` & `tmp/aws-cdk.aws-glue-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/aws-glue-alpha/dist/python/aws-cdk.aws-glue-alpha-2.84.0a0.tar", last modified: Tue Jun 13 23:46:45 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-glue/dist/python/aws-cdk.aws-glue-alpha-2.9.0a0.tar", last modified: Wed Jan 26 11:22:06 2022, max compression
```

## Comparing `aws-cdk.aws-glue-alpha-2.84.0a0.tar` & `aws-cdk.aws-glue-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-glue-alpha-2.84.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:37.000000 aws-cdk.aws-glue-alpha-2.84.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:37.000000 aws-cdk.aws-glue-alpha-2.84.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 23:46:37.000000 aws-cdk.aws-glue-alpha-2.84.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    19986 2023-06-13 23:46:45.000000 aws-cdk.aws-glue-alpha-2.84.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18991 2023-06-13 23:46:37.000000 aws-cdk.aws-glue-alpha-2.84.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:37.000000 aws-cdk.aws-glue-alpha-2.84.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:46:45.000000 aws-cdk.aws-glue-alpha-2.84.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1849 2023-06-13 23:46:37.000000 aws-cdk.aws-glue-alpha-2.84.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-glue-alpha-2.84.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-glue-alpha-2.84.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-glue-alpha-2.84.0a0/src/aws_cdk/aws_glue_alpha/
--rw-r--r--   0 root         (0) root         (0)   397157 2023-06-13 23:46:37.000000 aws-cdk.aws-glue-alpha-2.84.0a0/src/aws_cdk/aws_glue_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-glue-alpha-2.84.0a0/src/aws_cdk/aws_glue_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      435 2023-06-13 23:46:37.000000 aws-cdk.aws-glue-alpha-2.84.0a0/src/aws_cdk/aws_glue_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   152398 2023-06-13 23:46:37.000000 aws-cdk.aws-glue-alpha-2.84.0a0/src/aws_cdk/aws_glue_alpha/_jsii/aws-glue-alpha@2.84.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:37.000000 aws-cdk.aws-glue-alpha-2.84.0a0/src/aws_cdk/aws_glue_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-glue-alpha-2.84.0a0/src/aws_cdk.aws_glue_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19986 2023-06-13 23:46:45.000000 aws-cdk.aws-glue-alpha-2.84.0a0/src/aws_cdk.aws_glue_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      501 2023-06-13 23:46:45.000000 aws-cdk.aws-glue-alpha-2.84.0a0/src/aws_cdk.aws_glue_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:45.000000 aws-cdk.aws-glue-alpha-2.84.0a0/src/aws_cdk.aws_glue_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-13 23:46:45.000000 aws-cdk.aws-glue-alpha-2.84.0a0/src/aws_cdk.aws_glue_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:46:45.000000 aws-cdk.aws-glue-alpha-2.84.0a0/src/aws_cdk.aws_glue_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-glue-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-glue-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-glue-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:01.000000 aws-cdk.aws-glue-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    18455 2022-01-26 11:22:06.000000 aws-cdk.aws-glue-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17493 2022-01-26 11:22:01.000000 aws-cdk.aws-glue-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-glue-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:06.000000 aws-cdk.aws-glue-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1774 2022-01-26 11:22:01.000000 aws-cdk.aws-glue-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-glue-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-glue-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-glue-alpha-2.9.0a0/src/aws_cdk/aws_glue_alpha/
+-rw-r--r--   0 root         (0) root         (0)   304051 2022-01-26 11:22:01.000000 aws-cdk.aws-glue-alpha-2.9.0a0/src/aws_cdk/aws_glue_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-glue-alpha-2.9.0a0/src/aws_cdk/aws_glue_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      399 2022-01-26 11:22:01.000000 aws-cdk.aws-glue-alpha-2.9.0a0/src/aws_cdk/aws_glue_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   128286 2022-01-26 11:22:01.000000 aws-cdk.aws-glue-alpha-2.9.0a0/src/aws_cdk/aws_glue_alpha/_jsii/aws-glue-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-glue-alpha-2.9.0a0/src/aws_cdk/aws_glue_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-glue-alpha-2.9.0a0/src/aws_cdk.aws_glue_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    18455 2022-01-26 11:22:06.000000 aws-cdk.aws-glue-alpha-2.9.0a0/src/aws_cdk.aws_glue_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2022-01-26 11:22:06.000000 aws-cdk.aws-glue-alpha-2.9.0a0/src/aws_cdk.aws_glue_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:06.000000 aws-cdk.aws-glue-alpha-2.9.0a0/src/aws_cdk.aws_glue_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:06.000000 aws-cdk.aws-glue-alpha-2.9.0a0/src/aws_cdk.aws_glue_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:06.000000 aws-cdk.aws-glue-alpha-2.9.0a0/src/aws_cdk.aws_glue_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-glue-alpha-2.84.0a0/LICENSE` & `aws-cdk.aws-glue-alpha-2.9.0a0/LICENSE`

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

### Comparing `aws-cdk.aws-glue-alpha-2.84.0a0/PKG-INFO` & `aws-cdk.aws-glue-alpha-2.9.0a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-glue-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::Glue
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
 
 # AWS Glue Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -62,78 +62,56 @@
 An ETL job processes data in batches using Apache Spark.
 
 ```python
 # bucket: s3.Bucket
 
 glue.Job(self, "ScalaSparkEtlJob",
     executable=glue.JobExecutable.scala_etl(
-        glue_version=glue.GlueVersion.V4_0,
+        glue_version=glue.GlueVersion.V2_0,
         script=glue.Code.from_bucket(bucket, "src/com/example/HelloWorld.scala"),
         class_name="com.example.HelloWorld",
         extra_jars=[glue.Code.from_bucket(bucket, "jars/HelloWorld.jar")]
     ),
-    worker_type=glue.WorkerType.G_8X,
     description="an example Scala ETL job"
 )
 ```
 
 #### Streaming Jobs
 
 A Streaming job is similar to an ETL job, except that it performs ETL on data streams. It uses the Apache Spark Structured Streaming framework. Some Spark job features are not available to streaming ETL jobs.
 
 ```python
 glue.Job(self, "PythonSparkStreamingJob",
     executable=glue.JobExecutable.python_streaming(
-        glue_version=glue.GlueVersion.V4_0,
+        glue_version=glue.GlueVersion.V2_0,
         python_version=glue.PythonVersion.THREE,
         script=glue.Code.from_asset(path.join(__dirname, "job-script/hello_world.py"))
     ),
     description="an example Python Streaming job"
 )
 ```
 
 ### Python Shell Jobs
 
 A Python shell job runs Python scripts as a shell and supports a Python version that depends on the AWS Glue version you are using.
-This can be used to schedule and run tasks that don't require an Apache Spark environment. Currently, three flavors are supported:
-
-* PythonVersion.TWO (2.7; EOL)
-* PythonVersion.THREE (3.6)
-* PythonVersion.THREE_NINE (3.9)
+This can be used to schedule and run tasks that don't require an Apache Spark environment.
 
 ```python
 # bucket: s3.Bucket
 
 glue.Job(self, "PythonShellJob",
     executable=glue.JobExecutable.python_shell(
         glue_version=glue.GlueVersion.V1_0,
         python_version=glue.PythonVersion.THREE,
         script=glue.Code.from_bucket(bucket, "script.py")
     ),
     description="an example Python Shell job"
 )
 ```
 
-### Ray Jobs
-
-These jobs run in a Ray environment managed by AWS Glue.
-
-```python
-glue.Job(self, "RayJob",
-    executable=glue.JobExecutable.python_ray(
-        glue_version=glue.GlueVersion.V4_0,
-        python_version=glue.PythonVersion.THREE_NINE,
-        script=glue.Code.from_asset(path.join(__dirname, "job-script/hello_world.py"))
-    ),
-    worker_type=glue.WorkerType.Z_2X,
-    worker_count=2,
-    description="an example Ray job"
-)
-```
-
 See [documentation](https://docs.aws.amazon.com/glue/latest/dg/add-job.html) for more information on adding jobs in Glue.
 
 ## Connection
 
 A `Connection` allows Glue jobs, crawlers and development endpoints to access certain types of data stores. For example, to create a network connection to connect to a data source within a VPC:
 
 ```python
@@ -145,43 +123,25 @@
     # The security groups granting AWS Glue inbound access to the data source within the VPC
     security_groups=[security_group],
     # The VPC subnet which contains the data source
     subnet=subnet
 )
 ```
 
-For RDS `Connection` by JDBC, it is recommended to manage credentials using AWS Secrets Manager. To use Secret, specify `SECRET_ID` in `properties` like the following code. Note that in this case, the subnet must have a route to the AWS Secrets Manager VPC endpoint or to the AWS Secrets Manager endpoint through a NAT gateway.
-
-```python
-# security_group: ec2.SecurityGroup
-# subnet: ec2.Subnet
-# db: rds.DatabaseCluster
-
-glue.Connection(self, "RdsConnection",
-    type=glue.ConnectionType.JDBC,
-    security_groups=[security_group],
-    subnet=subnet,
-    properties={
-        "JDBC_CONNECTION_URL": f"jdbc:mysql://{db.clusterEndpoint.socketAddress}/databasename",
-        "JDBC_ENFORCE_SSL": "false",
-        "SECRET_ID": db.secret.secret_name
-    }
-)
-```
-
 If you need to use a connection type that doesn't exist as a static member on `ConnectionType`, you can instantiate a `ConnectionType` object, e.g: `new glue.ConnectionType('NEW_TYPE')`.
 
 See [Adding a Connection to Your Data Store](https://docs.aws.amazon.com/glue/latest/dg/populate-add-connection.html) and [Connection Structure](https://docs.aws.amazon.com/glue/latest/dg/aws-glue-api-catalog-connections.html#aws-glue-api-catalog-connections-Connection) documentation for more information on the supported data stores and their configurations.
 
 ## SecurityConfiguration
 
 A `SecurityConfiguration` is a set of security properties that can be used by AWS Glue to encrypt data at rest.
 
 ```python
 glue.SecurityConfiguration(self, "MySecurityConfiguration",
+    security_configuration_name="name",
     cloud_watch_encryption=glue.CloudWatchEncryption(
         mode=glue.CloudWatchEncryptionMode.KMS
     ),
     job_bookmarks_encryption=glue.JobBookmarksEncryption(
         mode=glue.JobBookmarksEncryptionMode.CLIENT_SIDE_KMS
     ),
     s3_encryption=glue.S3Encryption(
@@ -192,40 +152,44 @@
 
 By default, a shared KMS key is created for use with the encryption configurations that require one. You can also supply your own key for each encryption config, for example, for CloudWatch encryption:
 
 ```python
 # key: kms.Key
 
 glue.SecurityConfiguration(self, "MySecurityConfiguration",
+    security_configuration_name="name",
     cloud_watch_encryption=glue.CloudWatchEncryption(
         mode=glue.CloudWatchEncryptionMode.KMS,
         kms_key=key
     )
 )
 ```
 
 See [documentation](https://docs.aws.amazon.com/glue/latest/dg/encryption-security-configuration.html) for more info for Glue encrypting data written by Crawlers, Jobs, and Development Endpoints.
 
 ## Database
 
 A `Database` is a logical grouping of `Tables` in the Glue Catalog.
 
 ```python
-glue.Database(self, "MyDatabase")
+glue.Database(self, "MyDatabase",
+    database_name="my_database"
+)
 ```
 
 ## Table
 
 A Glue table describes a table of data in S3: its structure (column names and types), location of data (S3 objects with a common prefix in a S3 bucket), and format for the files (Json, Avro, Parquet, etc.):
 
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     ), glue.Column(
         name="col2",
         type=glue.Schema.array(glue.Schema.STRING),
         comment="col2 is an array of strings"
@@ -241,14 +205,15 @@
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     bucket=my_bucket,
     s3_prefix="my-table/",
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -260,14 +225,15 @@
 To improve query performance, a table can specify `partitionKeys` on which data is stored and queried separately. For example, you might partition a table by `year` and `month` to optimize queries based on a time window:
 
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     partition_keys=[glue.Column(
         name="year",
         type=glue.Schema.SMALL_INT
@@ -292,14 +258,15 @@
 property:
 
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     partition_keys=[glue.Column(
         name="year",
         type=glue.Schema.SMALL_INT
@@ -322,52 +289,29 @@
 
 my_table.add_partition_index(
     index_name="my-index",
     key_names=["year"]
 )
 ```
 
-### Partition Filtering
-
-If you have a table with a large number of partitions that grows over time, consider using AWS Glue partition indexing and filtering.
-
-```python
-# my_database: glue.Database
-
-glue.Table(self, "MyTable",
-    database=my_database,
-    columns=[glue.Column(
-        name="col1",
-        type=glue.Schema.STRING
-    )],
-    partition_keys=[glue.Column(
-        name="year",
-        type=glue.Schema.SMALL_INT
-    ), glue.Column(
-        name="month",
-        type=glue.Schema.SMALL_INT
-    )],
-    data_format=glue.DataFormat.JSON,
-    enable_partition_filtering=True
-)
-```
-
 ## [Encryption](https://docs.aws.amazon.com/athena/latest/ug/encryption.html)
 
 You can enable encryption on a Table's data:
 
-* [S3Managed](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingServerSideEncryption.html) - (default) Server side encryption (`SSE-S3`) with an Amazon S3-managed key.
+* `Unencrypted` - files are not encrypted. The default encryption setting.
+* [S3Managed](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingServerSideEncryption.html) - Server side encryption (`SSE-S3`) with an Amazon S3-managed key.
 
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.S3_MANAGED,
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -378,27 +322,29 @@
 # my_database: glue.Database
 
 # KMS key is created automatically
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.KMS,
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 
 # with an explicit KMS key
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.KMS,
     encryption_key=kms.Key(self, "MyKey"),
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -408,14 +354,15 @@
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.KMS_MANAGED,
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -426,27 +373,29 @@
 # my_database: glue.Database
 
 # KMS key is created automatically
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.CLIENT_SIDE_KMS,
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 
 # with an explicit KMS key
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.CLIENT_SIDE_KMS,
     encryption_key=kms.Key(self, "MyKey"),
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -479,14 +428,15 @@
             type=glue.Schema.DATE,
             comment="nested comment"
         ]),
         comment="struct<nested_column:date COMMENT 'nested comment'>"
     )],
     # ...
     database=my_database,
+    table_name="my_table",
     data_format=glue.DataFormat.JSON
 )
 ```
 
 ### Primitives
 
 #### Numeric
@@ -526,7 +476,9 @@
 ### Complex
 
 | Name                                	| Type     	| Comments                                                          	|
 |-------------------------------------	|----------	|-------------------------------------------------------------------	|
 | array(itemType: Type)               	| Function 	| An array of some other type                                       	|
 | map(keyType: Type, valueType: Type) 	| Function 	| A map of some primitive key type to any value type                	|
 | struct(collumns: Column[])          	| Function 	| Nested structure containing individually named and typed collumns 	|
+
+
```

### Comparing `aws-cdk.aws-glue-alpha-2.84.0a0/README.md` & `aws-cdk.aws-glue-alpha-2.9.0a0/src/aws_cdk.aws_glue_alpha.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: aws-cdk.aws-glue-alpha
+Version: 2.9.0a0
+Summary: The CDK Construct Library for AWS::Glue
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
 # AWS Glue Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
 
 
 ![cdk-constructs: Experimental](https://img.shields.io/badge/cdk--constructs-experimental-important.svg?style=for-the-badge)
 
@@ -35,78 +62,56 @@
 An ETL job processes data in batches using Apache Spark.
 
 ```python
 # bucket: s3.Bucket
 
 glue.Job(self, "ScalaSparkEtlJob",
     executable=glue.JobExecutable.scala_etl(
-        glue_version=glue.GlueVersion.V4_0,
+        glue_version=glue.GlueVersion.V2_0,
         script=glue.Code.from_bucket(bucket, "src/com/example/HelloWorld.scala"),
         class_name="com.example.HelloWorld",
         extra_jars=[glue.Code.from_bucket(bucket, "jars/HelloWorld.jar")]
     ),
-    worker_type=glue.WorkerType.G_8X,
     description="an example Scala ETL job"
 )
 ```
 
 #### Streaming Jobs
 
 A Streaming job is similar to an ETL job, except that it performs ETL on data streams. It uses the Apache Spark Structured Streaming framework. Some Spark job features are not available to streaming ETL jobs.
 
 ```python
 glue.Job(self, "PythonSparkStreamingJob",
     executable=glue.JobExecutable.python_streaming(
-        glue_version=glue.GlueVersion.V4_0,
+        glue_version=glue.GlueVersion.V2_0,
         python_version=glue.PythonVersion.THREE,
         script=glue.Code.from_asset(path.join(__dirname, "job-script/hello_world.py"))
     ),
     description="an example Python Streaming job"
 )
 ```
 
 ### Python Shell Jobs
 
 A Python shell job runs Python scripts as a shell and supports a Python version that depends on the AWS Glue version you are using.
-This can be used to schedule and run tasks that don't require an Apache Spark environment. Currently, three flavors are supported:
-
-* PythonVersion.TWO (2.7; EOL)
-* PythonVersion.THREE (3.6)
-* PythonVersion.THREE_NINE (3.9)
+This can be used to schedule and run tasks that don't require an Apache Spark environment.
 
 ```python
 # bucket: s3.Bucket
 
 glue.Job(self, "PythonShellJob",
     executable=glue.JobExecutable.python_shell(
         glue_version=glue.GlueVersion.V1_0,
         python_version=glue.PythonVersion.THREE,
         script=glue.Code.from_bucket(bucket, "script.py")
     ),
     description="an example Python Shell job"
 )
 ```
 
-### Ray Jobs
-
-These jobs run in a Ray environment managed by AWS Glue.
-
-```python
-glue.Job(self, "RayJob",
-    executable=glue.JobExecutable.python_ray(
-        glue_version=glue.GlueVersion.V4_0,
-        python_version=glue.PythonVersion.THREE_NINE,
-        script=glue.Code.from_asset(path.join(__dirname, "job-script/hello_world.py"))
-    ),
-    worker_type=glue.WorkerType.Z_2X,
-    worker_count=2,
-    description="an example Ray job"
-)
-```
-
 See [documentation](https://docs.aws.amazon.com/glue/latest/dg/add-job.html) for more information on adding jobs in Glue.
 
 ## Connection
 
 A `Connection` allows Glue jobs, crawlers and development endpoints to access certain types of data stores. For example, to create a network connection to connect to a data source within a VPC:
 
 ```python
@@ -118,43 +123,25 @@
     # The security groups granting AWS Glue inbound access to the data source within the VPC
     security_groups=[security_group],
     # The VPC subnet which contains the data source
     subnet=subnet
 )
 ```
 
-For RDS `Connection` by JDBC, it is recommended to manage credentials using AWS Secrets Manager. To use Secret, specify `SECRET_ID` in `properties` like the following code. Note that in this case, the subnet must have a route to the AWS Secrets Manager VPC endpoint or to the AWS Secrets Manager endpoint through a NAT gateway.
-
-```python
-# security_group: ec2.SecurityGroup
-# subnet: ec2.Subnet
-# db: rds.DatabaseCluster
-
-glue.Connection(self, "RdsConnection",
-    type=glue.ConnectionType.JDBC,
-    security_groups=[security_group],
-    subnet=subnet,
-    properties={
-        "JDBC_CONNECTION_URL": f"jdbc:mysql://{db.clusterEndpoint.socketAddress}/databasename",
-        "JDBC_ENFORCE_SSL": "false",
-        "SECRET_ID": db.secret.secret_name
-    }
-)
-```
-
 If you need to use a connection type that doesn't exist as a static member on `ConnectionType`, you can instantiate a `ConnectionType` object, e.g: `new glue.ConnectionType('NEW_TYPE')`.
 
 See [Adding a Connection to Your Data Store](https://docs.aws.amazon.com/glue/latest/dg/populate-add-connection.html) and [Connection Structure](https://docs.aws.amazon.com/glue/latest/dg/aws-glue-api-catalog-connections.html#aws-glue-api-catalog-connections-Connection) documentation for more information on the supported data stores and their configurations.
 
 ## SecurityConfiguration
 
 A `SecurityConfiguration` is a set of security properties that can be used by AWS Glue to encrypt data at rest.
 
 ```python
 glue.SecurityConfiguration(self, "MySecurityConfiguration",
+    security_configuration_name="name",
     cloud_watch_encryption=glue.CloudWatchEncryption(
         mode=glue.CloudWatchEncryptionMode.KMS
     ),
     job_bookmarks_encryption=glue.JobBookmarksEncryption(
         mode=glue.JobBookmarksEncryptionMode.CLIENT_SIDE_KMS
     ),
     s3_encryption=glue.S3Encryption(
@@ -165,40 +152,44 @@
 
 By default, a shared KMS key is created for use with the encryption configurations that require one. You can also supply your own key for each encryption config, for example, for CloudWatch encryption:
 
 ```python
 # key: kms.Key
 
 glue.SecurityConfiguration(self, "MySecurityConfiguration",
+    security_configuration_name="name",
     cloud_watch_encryption=glue.CloudWatchEncryption(
         mode=glue.CloudWatchEncryptionMode.KMS,
         kms_key=key
     )
 )
 ```
 
 See [documentation](https://docs.aws.amazon.com/glue/latest/dg/encryption-security-configuration.html) for more info for Glue encrypting data written by Crawlers, Jobs, and Development Endpoints.
 
 ## Database
 
 A `Database` is a logical grouping of `Tables` in the Glue Catalog.
 
 ```python
-glue.Database(self, "MyDatabase")
+glue.Database(self, "MyDatabase",
+    database_name="my_database"
+)
 ```
 
 ## Table
 
 A Glue table describes a table of data in S3: its structure (column names and types), location of data (S3 objects with a common prefix in a S3 bucket), and format for the files (Json, Avro, Parquet, etc.):
 
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     ), glue.Column(
         name="col2",
         type=glue.Schema.array(glue.Schema.STRING),
         comment="col2 is an array of strings"
@@ -214,14 +205,15 @@
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     bucket=my_bucket,
     s3_prefix="my-table/",
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -233,14 +225,15 @@
 To improve query performance, a table can specify `partitionKeys` on which data is stored and queried separately. For example, you might partition a table by `year` and `month` to optimize queries based on a time window:
 
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     partition_keys=[glue.Column(
         name="year",
         type=glue.Schema.SMALL_INT
@@ -265,14 +258,15 @@
 property:
 
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     partition_keys=[glue.Column(
         name="year",
         type=glue.Schema.SMALL_INT
@@ -295,52 +289,29 @@
 
 my_table.add_partition_index(
     index_name="my-index",
     key_names=["year"]
 )
 ```
 
-### Partition Filtering
-
-If you have a table with a large number of partitions that grows over time, consider using AWS Glue partition indexing and filtering.
-
-```python
-# my_database: glue.Database
-
-glue.Table(self, "MyTable",
-    database=my_database,
-    columns=[glue.Column(
-        name="col1",
-        type=glue.Schema.STRING
-    )],
-    partition_keys=[glue.Column(
-        name="year",
-        type=glue.Schema.SMALL_INT
-    ), glue.Column(
-        name="month",
-        type=glue.Schema.SMALL_INT
-    )],
-    data_format=glue.DataFormat.JSON,
-    enable_partition_filtering=True
-)
-```
-
 ## [Encryption](https://docs.aws.amazon.com/athena/latest/ug/encryption.html)
 
 You can enable encryption on a Table's data:
 
-* [S3Managed](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingServerSideEncryption.html) - (default) Server side encryption (`SSE-S3`) with an Amazon S3-managed key.
+* `Unencrypted` - files are not encrypted. The default encryption setting.
+* [S3Managed](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingServerSideEncryption.html) - Server side encryption (`SSE-S3`) with an Amazon S3-managed key.
 
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.S3_MANAGED,
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -351,27 +322,29 @@
 # my_database: glue.Database
 
 # KMS key is created automatically
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.KMS,
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 
 # with an explicit KMS key
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.KMS,
     encryption_key=kms.Key(self, "MyKey"),
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -381,14 +354,15 @@
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.KMS_MANAGED,
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -399,27 +373,29 @@
 # my_database: glue.Database
 
 # KMS key is created automatically
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.CLIENT_SIDE_KMS,
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 
 # with an explicit KMS key
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.CLIENT_SIDE_KMS,
     encryption_key=kms.Key(self, "MyKey"),
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -452,14 +428,15 @@
             type=glue.Schema.DATE,
             comment="nested comment"
         ]),
         comment="struct<nested_column:date COMMENT 'nested comment'>"
     )],
     # ...
     database=my_database,
+    table_name="my_table",
     data_format=glue.DataFormat.JSON
 )
 ```
 
 ### Primitives
 
 #### Numeric
@@ -499,7 +476,9 @@
 ### Complex
 
 | Name                                	| Type     	| Comments                                                          	|
 |-------------------------------------	|----------	|-------------------------------------------------------------------	|
 | array(itemType: Type)               	| Function 	| An array of some other type                                       	|
 | map(keyType: Type, valueType: Type) 	| Function 	| A map of some primitive key type to any value type                	|
 | struct(collumns: Column[])          	| Function 	| Nested structure containing individually named and typed collumns 	|
+
+
```

### Comparing `aws-cdk.aws-glue-alpha-2.84.0a0/setup.py` & `aws-cdk.aws-glue-alpha-2.9.0a0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-glue-alpha",
-    "version": "2.84.0.a0",
+    "version": "2.9.0.a0",
     "description": "The CDK Construct Library for AWS::Glue",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,43 +22,41 @@
     },
     "packages": [
         "aws_cdk.aws_glue_alpha",
         "aws_cdk.aws_glue_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_glue_alpha._jsii": [
-            "aws-glue-alpha@2.84.0-alpha.0.jsii.tgz"
+            "aws-glue-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_glue_alpha": [
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

### Comparing `aws-cdk.aws-glue-alpha-2.84.0a0/src/aws_cdk/aws_glue_alpha/__init__.py` & `aws-cdk.aws-glue-alpha-2.9.0a0/src/aws_cdk/aws_glue_alpha/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -36,78 +36,56 @@
 An ETL job processes data in batches using Apache Spark.
 
 ```python
 # bucket: s3.Bucket
 
 glue.Job(self, "ScalaSparkEtlJob",
     executable=glue.JobExecutable.scala_etl(
-        glue_version=glue.GlueVersion.V4_0,
+        glue_version=glue.GlueVersion.V2_0,
         script=glue.Code.from_bucket(bucket, "src/com/example/HelloWorld.scala"),
         class_name="com.example.HelloWorld",
         extra_jars=[glue.Code.from_bucket(bucket, "jars/HelloWorld.jar")]
     ),
-    worker_type=glue.WorkerType.G_8X,
     description="an example Scala ETL job"
 )
 ```
 
 #### Streaming Jobs
 
 A Streaming job is similar to an ETL job, except that it performs ETL on data streams. It uses the Apache Spark Structured Streaming framework. Some Spark job features are not available to streaming ETL jobs.
 
 ```python
 glue.Job(self, "PythonSparkStreamingJob",
     executable=glue.JobExecutable.python_streaming(
-        glue_version=glue.GlueVersion.V4_0,
+        glue_version=glue.GlueVersion.V2_0,
         python_version=glue.PythonVersion.THREE,
         script=glue.Code.from_asset(path.join(__dirname, "job-script/hello_world.py"))
     ),
     description="an example Python Streaming job"
 )
 ```
 
 ### Python Shell Jobs
 
 A Python shell job runs Python scripts as a shell and supports a Python version that depends on the AWS Glue version you are using.
-This can be used to schedule and run tasks that don't require an Apache Spark environment. Currently, three flavors are supported:
-
-* PythonVersion.TWO (2.7; EOL)
-* PythonVersion.THREE (3.6)
-* PythonVersion.THREE_NINE (3.9)
+This can be used to schedule and run tasks that don't require an Apache Spark environment.
 
 ```python
 # bucket: s3.Bucket
 
 glue.Job(self, "PythonShellJob",
     executable=glue.JobExecutable.python_shell(
         glue_version=glue.GlueVersion.V1_0,
         python_version=glue.PythonVersion.THREE,
         script=glue.Code.from_bucket(bucket, "script.py")
     ),
     description="an example Python Shell job"
 )
 ```
 
-### Ray Jobs
-
-These jobs run in a Ray environment managed by AWS Glue.
-
-```python
-glue.Job(self, "RayJob",
-    executable=glue.JobExecutable.python_ray(
-        glue_version=glue.GlueVersion.V4_0,
-        python_version=glue.PythonVersion.THREE_NINE,
-        script=glue.Code.from_asset(path.join(__dirname, "job-script/hello_world.py"))
-    ),
-    worker_type=glue.WorkerType.Z_2X,
-    worker_count=2,
-    description="an example Ray job"
-)
-```
-
 See [documentation](https://docs.aws.amazon.com/glue/latest/dg/add-job.html) for more information on adding jobs in Glue.
 
 ## Connection
 
 A `Connection` allows Glue jobs, crawlers and development endpoints to access certain types of data stores. For example, to create a network connection to connect to a data source within a VPC:
 
 ```python
@@ -119,43 +97,25 @@
     # The security groups granting AWS Glue inbound access to the data source within the VPC
     security_groups=[security_group],
     # The VPC subnet which contains the data source
     subnet=subnet
 )
 ```
 
-For RDS `Connection` by JDBC, it is recommended to manage credentials using AWS Secrets Manager. To use Secret, specify `SECRET_ID` in `properties` like the following code. Note that in this case, the subnet must have a route to the AWS Secrets Manager VPC endpoint or to the AWS Secrets Manager endpoint through a NAT gateway.
-
-```python
-# security_group: ec2.SecurityGroup
-# subnet: ec2.Subnet
-# db: rds.DatabaseCluster
-
-glue.Connection(self, "RdsConnection",
-    type=glue.ConnectionType.JDBC,
-    security_groups=[security_group],
-    subnet=subnet,
-    properties={
-        "JDBC_CONNECTION_URL": f"jdbc:mysql://{db.clusterEndpoint.socketAddress}/databasename",
-        "JDBC_ENFORCE_SSL": "false",
-        "SECRET_ID": db.secret.secret_name
-    }
-)
-```
-
 If you need to use a connection type that doesn't exist as a static member on `ConnectionType`, you can instantiate a `ConnectionType` object, e.g: `new glue.ConnectionType('NEW_TYPE')`.
 
 See [Adding a Connection to Your Data Store](https://docs.aws.amazon.com/glue/latest/dg/populate-add-connection.html) and [Connection Structure](https://docs.aws.amazon.com/glue/latest/dg/aws-glue-api-catalog-connections.html#aws-glue-api-catalog-connections-Connection) documentation for more information on the supported data stores and their configurations.
 
 ## SecurityConfiguration
 
 A `SecurityConfiguration` is a set of security properties that can be used by AWS Glue to encrypt data at rest.
 
 ```python
 glue.SecurityConfiguration(self, "MySecurityConfiguration",
+    security_configuration_name="name",
     cloud_watch_encryption=glue.CloudWatchEncryption(
         mode=glue.CloudWatchEncryptionMode.KMS
     ),
     job_bookmarks_encryption=glue.JobBookmarksEncryption(
         mode=glue.JobBookmarksEncryptionMode.CLIENT_SIDE_KMS
     ),
     s3_encryption=glue.S3Encryption(
@@ -166,40 +126,44 @@
 
 By default, a shared KMS key is created for use with the encryption configurations that require one. You can also supply your own key for each encryption config, for example, for CloudWatch encryption:
 
 ```python
 # key: kms.Key
 
 glue.SecurityConfiguration(self, "MySecurityConfiguration",
+    security_configuration_name="name",
     cloud_watch_encryption=glue.CloudWatchEncryption(
         mode=glue.CloudWatchEncryptionMode.KMS,
         kms_key=key
     )
 )
 ```
 
 See [documentation](https://docs.aws.amazon.com/glue/latest/dg/encryption-security-configuration.html) for more info for Glue encrypting data written by Crawlers, Jobs, and Development Endpoints.
 
 ## Database
 
 A `Database` is a logical grouping of `Tables` in the Glue Catalog.
 
 ```python
-glue.Database(self, "MyDatabase")
+glue.Database(self, "MyDatabase",
+    database_name="my_database"
+)
 ```
 
 ## Table
 
 A Glue table describes a table of data in S3: its structure (column names and types), location of data (S3 objects with a common prefix in a S3 bucket), and format for the files (Json, Avro, Parquet, etc.):
 
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     ), glue.Column(
         name="col2",
         type=glue.Schema.array(glue.Schema.STRING),
         comment="col2 is an array of strings"
@@ -215,14 +179,15 @@
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     bucket=my_bucket,
     s3_prefix="my-table/",
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -234,14 +199,15 @@
 To improve query performance, a table can specify `partitionKeys` on which data is stored and queried separately. For example, you might partition a table by `year` and `month` to optimize queries based on a time window:
 
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     partition_keys=[glue.Column(
         name="year",
         type=glue.Schema.SMALL_INT
@@ -266,14 +232,15 @@
 property:
 
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     partition_keys=[glue.Column(
         name="year",
         type=glue.Schema.SMALL_INT
@@ -296,52 +263,29 @@
 
 my_table.add_partition_index(
     index_name="my-index",
     key_names=["year"]
 )
 ```
 
-### Partition Filtering
-
-If you have a table with a large number of partitions that grows over time, consider using AWS Glue partition indexing and filtering.
-
-```python
-# my_database: glue.Database
-
-glue.Table(self, "MyTable",
-    database=my_database,
-    columns=[glue.Column(
-        name="col1",
-        type=glue.Schema.STRING
-    )],
-    partition_keys=[glue.Column(
-        name="year",
-        type=glue.Schema.SMALL_INT
-    ), glue.Column(
-        name="month",
-        type=glue.Schema.SMALL_INT
-    )],
-    data_format=glue.DataFormat.JSON,
-    enable_partition_filtering=True
-)
-```
-
 ## [Encryption](https://docs.aws.amazon.com/athena/latest/ug/encryption.html)
 
 You can enable encryption on a Table's data:
 
-* [S3Managed](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingServerSideEncryption.html) - (default) Server side encryption (`SSE-S3`) with an Amazon S3-managed key.
+* `Unencrypted` - files are not encrypted. The default encryption setting.
+* [S3Managed](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingServerSideEncryption.html) - Server side encryption (`SSE-S3`) with an Amazon S3-managed key.
 
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.S3_MANAGED,
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -352,27 +296,29 @@
 # my_database: glue.Database
 
 # KMS key is created automatically
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.KMS,
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 
 # with an explicit KMS key
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.KMS,
     encryption_key=kms.Key(self, "MyKey"),
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -382,14 +328,15 @@
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.KMS_MANAGED,
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -400,27 +347,29 @@
 # my_database: glue.Database
 
 # KMS key is created automatically
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.CLIENT_SIDE_KMS,
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 
 # with an explicit KMS key
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.CLIENT_SIDE_KMS,
     encryption_key=kms.Key(self, "MyKey"),
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -453,14 +402,15 @@
             type=glue.Schema.DATE,
             comment="nested comment"
         ]),
         comment="struct<nested_column:date COMMENT 'nested comment'>"
     )],
     # ...
     database=my_database,
+    table_name="my_table",
     data_format=glue.DataFormat.JSON
 )
 ```
 
 ### Primitives
 
 #### Numeric
@@ -511,28 +461,26 @@
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
-import aws_cdk.aws_events as _aws_cdk_aws_events_ceddda9d
-import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
-import aws_cdk.aws_kms as _aws_cdk_aws_kms_ceddda9d
-import aws_cdk.aws_logs as _aws_cdk_aws_logs_ceddda9d
-import aws_cdk.aws_s3 as _aws_cdk_aws_s3_ceddda9d
-import aws_cdk.aws_s3_assets as _aws_cdk_aws_s3_assets_ceddda9d
-import constructs as _constructs_77d1e7e8
+import aws_cdk
+import aws_cdk.aws_cloudwatch
+import aws_cdk.aws_ec2
+import aws_cdk.aws_events
+import aws_cdk.aws_iam
+import aws_cdk.aws_kms
+import aws_cdk.aws_logs
+import aws_cdk.aws_s3
+import aws_cdk.aws_s3_assets
+import constructs
 
 
 class ClassificationString(
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-glue-alpha.ClassificationString",
 ):
     '''(experimental) Classification string given to tables with this data format.
@@ -552,74 +500,71 @@
 
     def __init__(self, value: builtins.str) -> None:
         '''
         :param value: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2bfce587a58c2deea97e71eeab8754a97692804f6d43271eda89c6257eaebdfc)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.create(self.__class__, self, [value])
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="AVRO")
     def AVRO(cls) -> "ClassificationString":
         '''
         :see: https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-format.html#aws-glue-programming-etl-format-avro
         :stability: experimental
         '''
         return typing.cast("ClassificationString", jsii.sget(cls, "AVRO"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="CSV")
     def CSV(cls) -> "ClassificationString":
         '''
         :see: https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-format.html#aws-glue-programming-etl-format-csv
         :stability: experimental
         '''
         return typing.cast("ClassificationString", jsii.sget(cls, "CSV"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="JSON")
     def JSON(cls) -> "ClassificationString":
         '''
         :see: https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-format.html#aws-glue-programming-etl-format-json
         :stability: experimental
         '''
         return typing.cast("ClassificationString", jsii.sget(cls, "JSON"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="ORC")
     def ORC(cls) -> "ClassificationString":
         '''
         :see: https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-format.html#aws-glue-programming-etl-format-orc
         :stability: experimental
         '''
         return typing.cast("ClassificationString", jsii.sget(cls, "ORC"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="PARQUET")
     def PARQUET(cls) -> "ClassificationString":
         '''
         :see: https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-format.html#aws-glue-programming-etl-format-parquet
         :stability: experimental
         '''
         return typing.cast("ClassificationString", jsii.sget(cls, "PARQUET"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="XML")
     def XML(cls) -> "ClassificationString":
         '''
         :see: https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-format.html#aws-glue-programming-etl-format-xml
         :stability: experimental
         '''
         return typing.cast("ClassificationString", jsii.sget(cls, "XML"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="value")
     def value(self) -> builtins.str:
         '''
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "value"))
 
@@ -630,43 +575,40 @@
     name_mapping={"mode": "mode", "kms_key": "kmsKey"},
 )
 class CloudWatchEncryption:
     def __init__(
         self,
         *,
         mode: "CloudWatchEncryptionMode",
-        kms_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        kms_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
     ) -> None:
         '''(experimental) CloudWatch Logs encryption configuration.
 
         :param mode: (experimental) Encryption mode.
         :param kms_key: (experimental) The KMS key to be used to encrypt the data. Default: A key will be created if one is not provided.
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
             glue.SecurityConfiguration(self, "MySecurityConfiguration",
+                security_configuration_name="name",
                 cloud_watch_encryption=glue.CloudWatchEncryption(
                     mode=glue.CloudWatchEncryptionMode.KMS
                 ),
                 job_bookmarks_encryption=glue.JobBookmarksEncryption(
                     mode=glue.JobBookmarksEncryptionMode.CLIENT_SIDE_KMS
                 ),
                 s3_encryption=glue.S3Encryption(
                     mode=glue.S3EncryptionMode.KMS
                 )
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ceec14d1d7029d8fb7df76e4abb14bc79250421d85a9584f0271d9e7c4f4ef3f)
-            check_type(argname="argument mode", value=mode, expected_type=type_hints["mode"])
-            check_type(argname="argument kms_key", value=kms_key, expected_type=type_hints["kms_key"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "mode": mode,
         }
         if kms_key is not None:
             self._values["kms_key"] = kms_key
 
     @builtins.property
     def mode(self) -> "CloudWatchEncryptionMode":
@@ -675,23 +617,23 @@
         :stability: experimental
         '''
         result = self._values.get("mode")
         assert result is not None, "Required property 'mode' is missing"
         return typing.cast("CloudWatchEncryptionMode", result)
 
     @builtins.property
-    def kms_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def kms_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) The KMS key to be used to encrypt the data.
 
         :default: A key will be created if one is not provided.
 
         :stability: experimental
         '''
         result = self._values.get("kms_key")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -708,14 +650,15 @@
     :see: https://docs.aws.amazon.com/glue/latest/webapi/API_CloudWatchEncryption.html#Glue-Type-CloudWatchEncryption-CloudWatchEncryptionMode
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
         glue.SecurityConfiguration(self, "MySecurityConfiguration",
+            security_configuration_name="name",
             cloud_watch_encryption=glue.CloudWatchEncryption(
                 mode=glue.CloudWatchEncryptionMode.KMS
             ),
             job_bookmarks_encryption=glue.JobBookmarksEncryption(
                 mode=glue.JobBookmarksEncryptionMode.CLIENT_SIDE_KMS
             ),
             s3_encryption=glue.S3Encryption(
@@ -736,101 +679,89 @@
     '''(experimental) Represents a Glue Job's Code assets (an asset can be a scripts, a jar, a python file or any other file).
 
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
-        glue.Job(self, "PythonSparkStreamingJob",
-            executable=glue.JobExecutable.python_streaming(
-                glue_version=glue.GlueVersion.V4_0,
+        # bucket: s3.Bucket
+        
+        glue.Job(self, "PythonShellJob",
+            executable=glue.JobExecutable.python_shell(
+                glue_version=glue.GlueVersion.V1_0,
                 python_version=glue.PythonVersion.THREE,
-                script=glue.Code.from_asset(path.join(__dirname, "job-script/hello_world.py"))
+                script=glue.Code.from_bucket(bucket, "script.py")
             ),
-            description="an example Python Streaming job"
+            description="an example Python Shell job"
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
         path: builtins.str,
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
         '''(experimental) Job code from a local disk path.
 
         :param path: code file (not a directory).
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
-            type_hints = typing.get_type_hints(_typecheckingstub__cd7e88ca82e81ea6700503f28d9e5352c4a86e264d00afb35e761e591a7e0e24)
-            check_type(argname="argument path", value=path, expected_type=type_hints["path"])
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
 
         return typing.cast("AssetCode", jsii.sinvoke(cls, "fromAsset", [path, options]))
 
-    @jsii.member(jsii_name="fromBucket")
+    @jsii.member(jsii_name="fromBucket") # type: ignore[misc]
     @builtins.classmethod
-    def from_bucket(
-        cls,
-        bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
-        key: builtins.str,
-    ) -> "S3Code":
+    def from_bucket(cls, bucket: aws_cdk.aws_s3.IBucket, key: builtins.str) -> "S3Code":
         '''(experimental) Job code as an S3 object.
 
         :param bucket: The S3 bucket.
         :param key: The object key.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d23f6002340150960cebd70816482874d96a0de7d52265f1fcd0ab459eea2a61)
-            check_type(argname="argument bucket", value=bucket, expected_type=type_hints["bucket"])
-            check_type(argname="argument key", value=key, expected_type=type_hints["key"])
         return typing.cast("S3Code", jsii.sinvoke(cls, "fromBucket", [bucket, key]))
 
-    @jsii.member(jsii_name="bind")
+    @jsii.member(jsii_name="bind") # type: ignore[misc]
     @abc.abstractmethod
     def bind(
         self,
-        scope: _constructs_77d1e7e8.Construct,
-        grantable: _aws_cdk_aws_iam_ceddda9d.IGrantable,
+        scope: constructs.Construct,
+        grantable: aws_cdk.aws_iam.IGrantable,
     ) -> "CodeConfig":
         '''(experimental) Called when the Job is initialized to allow this object to bind.
 
         :param scope: -
         :param grantable: -
 
         :stability: experimental
@@ -838,45 +769,37 @@
         ...
 
 
 class _CodeProxy(Code):
     @jsii.member(jsii_name="bind")
     def bind(
         self,
-        scope: _constructs_77d1e7e8.Construct,
-        grantable: _aws_cdk_aws_iam_ceddda9d.IGrantable,
+        scope: constructs.Construct,
+        grantable: aws_cdk.aws_iam.IGrantable,
     ) -> "CodeConfig":
         '''(experimental) Called when the Job is initialized to allow this object to bind.
 
         :param scope: -
         :param grantable: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7b88388256be44082f9ce622ac393616c31af36dc246d0cb6ea3eb8e78b31dc1)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument grantable", value=grantable, expected_type=type_hints["grantable"])
         return typing.cast("CodeConfig", jsii.invoke(self, "bind", [scope, grantable]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the abstract class
 typing.cast(typing.Any, Code).__jsii_proxy_class__ = lambda : _CodeProxy
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-glue-alpha.CodeConfig",
     jsii_struct_bases=[],
     name_mapping={"s3_location": "s3Location"},
 )
 class CodeConfig:
-    def __init__(
-        self,
-        *,
-        s3_location: typing.Union[_aws_cdk_aws_s3_ceddda9d.Location, typing.Dict[builtins.str, typing.Any]],
-    ) -> None:
+    def __init__(self, *, s3_location: aws_cdk.aws_s3.Location) -> None:
         '''(experimental) Result of binding ``Code`` into a ``Job``.
 
         :param s3_location: (experimental) The location of the code in S3.
 
         :stability: experimental
         :exampleMetadata: fixture=_generated
 
@@ -893,31 +816,28 @@
             
                     # the properties below are optional
                     object_version="objectVersion"
                 )
             )
         '''
         if isinstance(s3_location, dict):
-            s3_location = _aws_cdk_aws_s3_ceddda9d.Location(**s3_location)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7667596ec33fb86df61ee9e5603a0bed57aa6e48e3795e84685966147e79b05e)
-            check_type(argname="argument s3_location", value=s3_location, expected_type=type_hints["s3_location"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+            s3_location = aws_cdk.aws_s3.Location(**s3_location)
+        self._values: typing.Dict[str, typing.Any] = {
             "s3_location": s3_location,
         }
 
     @builtins.property
-    def s3_location(self) -> _aws_cdk_aws_s3_ceddda9d.Location:
+    def s3_location(self) -> aws_cdk.aws_s3.Location:
         '''(experimental) The location of the code in S3.
 
         :stability: experimental
         '''
         result = self._values.get("s3_location")
         assert result is not None, "Required property 's3_location' is missing"
-        return typing.cast(_aws_cdk_aws_s3_ceddda9d.Location, result)
+        return typing.cast(aws_cdk.aws_s3.Location, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -933,15 +853,15 @@
     name_mapping={"name": "name", "type": "type", "comment": "comment"},
 )
 class Column:
     def __init__(
         self,
         *,
         name: builtins.str,
-        type: typing.Union["Type", typing.Dict[builtins.str, typing.Any]],
+        type: "Type",
         comment: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) A column of a table.
 
         :param name: (experimental) Name of the column.
         :param type: (experimental) Type of the column.
         :param comment: (experimental) Coment describing the column. Default: none
@@ -964,20 +884,15 @@
             
                 # the properties below are optional
                 comment="comment"
             )
         '''
         if isinstance(type, dict):
             type = Type(**type)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__043c8b76c78332fa2f7a0e1444ad14734d788355c87767ffb0dd0aac9a19fbdf)
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
-            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
-            check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "name": name,
             "type": type,
         }
         if comment is not None:
             self._values["comment"] = comment
 
     @builtins.property
@@ -1039,16 +954,16 @@
     def __init__(
         self,
         *,
         connection_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         match_criteria: typing.Optional[typing.Sequence[builtins.str]] = None,
         properties: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-        subnet: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISubnet] = None,
+        security_groups: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.ISecurityGroup]] = None,
+        subnet: typing.Optional[aws_cdk.aws_ec2.ISubnet] = None,
     ) -> None:
         '''(experimental) Base Connection Options.
 
         :param connection_name: (experimental) The name of the connection. Default: cloudformation generated name
         :param description: (experimental) The description of the connection. Default: no description
         :param match_criteria: (experimental) A list of criteria that can be used in selecting this connection. This is useful for filtering the results of https://awscli.amazonaws.com/v2/documentation/api/latest/reference/glue/get-connections.html Default: no match criteria
         :param properties: (experimental) Key-Value pairs that define parameters for the connection. Default: empty properties
@@ -1075,23 +990,15 @@
                 properties={
                     "properties_key": "properties"
                 },
                 security_groups=[security_group],
                 subnet=subnet
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a1670baf78db937cd3601a16badd87755f3fc525b8fd6a352d45c2bc3994b494)
-            check_type(argname="argument connection_name", value=connection_name, expected_type=type_hints["connection_name"])
-            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
-            check_type(argname="argument match_criteria", value=match_criteria, expected_type=type_hints["match_criteria"])
-            check_type(argname="argument properties", value=properties, expected_type=type_hints["properties"])
-            check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
-            check_type(argname="argument subnet", value=subnet, expected_type=type_hints["subnet"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if connection_name is not None:
             self._values["connection_name"] = connection_name
         if description is not None:
             self._values["description"] = description
         if match_criteria is not None:
             self._values["match_criteria"] = match_criteria
         if properties is not None:
@@ -1147,36 +1054,36 @@
         '''
         result = self._values.get("properties")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def security_groups(
         self,
-    ) -> typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]]:
+    ) -> typing.Optional[typing.List[aws_cdk.aws_ec2.ISecurityGroup]]:
         '''(experimental) The list of security groups needed to successfully make this connection e.g. to successfully connect to VPC.
 
         :default: no security group
 
         :stability: experimental
         '''
         result = self._values.get("security_groups")
-        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]], result)
+        return typing.cast(typing.Optional[typing.List[aws_cdk.aws_ec2.ISecurityGroup]], result)
 
     @builtins.property
-    def subnet(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISubnet]:
+    def subnet(self) -> typing.Optional[aws_cdk.aws_ec2.ISubnet]:
         '''(experimental) The VPC subnet to connect to resources within a VPC.
 
         See more at https://docs.aws.amazon.com/glue/latest/dg/start-connecting.html.
 
         :default: no subnet
 
         :stability: experimental
         '''
         result = self._values.get("subnet")
-        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISubnet], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_ec2.ISubnet], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -1203,19 +1110,19 @@
     def __init__(
         self,
         *,
         connection_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         match_criteria: typing.Optional[typing.Sequence[builtins.str]] = None,
         properties: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-        subnet: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISubnet] = None,
+        security_groups: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.ISecurityGroup]] = None,
+        subnet: typing.Optional[aws_cdk.aws_ec2.ISubnet] = None,
         type: "ConnectionType",
     ) -> None:
-        '''(experimental) Construction properties for ``Connection``.
+        '''(experimental) Construction properties for {@link Connection}.
 
         :param connection_name: (experimental) The name of the connection. Default: cloudformation generated name
         :param description: (experimental) The description of the connection. Default: no description
         :param match_criteria: (experimental) A list of criteria that can be used in selecting this connection. This is useful for filtering the results of https://awscli.amazonaws.com/v2/documentation/api/latest/reference/glue/get-connections.html Default: no match criteria
         :param properties: (experimental) Key-Value pairs that define parameters for the connection. Default: empty properties
         :param security_groups: (experimental) The list of security groups needed to successfully make this connection e.g. to successfully connect to VPC. Default: no security group
         :param subnet: (experimental) The VPC subnet to connect to resources within a VPC. See more at https://docs.aws.amazon.com/glue/latest/dg/start-connecting.html. Default: no subnet
@@ -1233,24 +1140,15 @@
                 type=glue.ConnectionType.NETWORK,
                 # The security groups granting AWS Glue inbound access to the data source within the VPC
                 security_groups=[security_group],
                 # The VPC subnet which contains the data source
                 subnet=subnet
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d3fa037db6ada98c73a1d8889753f75c2f3c7513c8a41daf149dc5769cdb83e8)
-            check_type(argname="argument connection_name", value=connection_name, expected_type=type_hints["connection_name"])
-            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
-            check_type(argname="argument match_criteria", value=match_criteria, expected_type=type_hints["match_criteria"])
-            check_type(argname="argument properties", value=properties, expected_type=type_hints["properties"])
-            check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
-            check_type(argname="argument subnet", value=subnet, expected_type=type_hints["subnet"])
-            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "type": type,
         }
         if connection_name is not None:
             self._values["connection_name"] = connection_name
         if description is not None:
             self._values["description"] = description
         if match_criteria is not None:
@@ -1308,36 +1206,36 @@
         '''
         result = self._values.get("properties")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def security_groups(
         self,
-    ) -> typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]]:
+    ) -> typing.Optional[typing.List[aws_cdk.aws_ec2.ISecurityGroup]]:
         '''(experimental) The list of security groups needed to successfully make this connection e.g. to successfully connect to VPC.
 
         :default: no security group
 
         :stability: experimental
         '''
         result = self._values.get("security_groups")
-        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]], result)
+        return typing.cast(typing.Optional[typing.List[aws_cdk.aws_ec2.ISecurityGroup]], result)
 
     @builtins.property
-    def subnet(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISubnet]:
+    def subnet(self) -> typing.Optional[aws_cdk.aws_ec2.ISubnet]:
         '''(experimental) The VPC subnet to connect to resources within a VPC.
 
         See more at https://docs.aws.amazon.com/glue/latest/dg/start-connecting.html.
 
         :default: no subnet
 
         :stability: experimental
         '''
         result = self._values.get("subnet")
-        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISubnet], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_ec2.ISubnet], result)
 
     @builtins.property
     def type(self) -> "ConnectionType":
         '''(experimental) The type of the connection.
 
         :stability: experimental
         '''
@@ -1385,64 +1283,61 @@
 
     def __init__(self, name: builtins.str) -> None:
         '''
         :param name: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b1f57c94567ffb3d89cdd8c9cd2b37bd37decd390b53c9bfdadd569dc797aa3f)
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         jsii.create(self.__class__, self, [name])
 
     @jsii.member(jsii_name="toString")
     def to_string(self) -> builtins.str:
         '''(experimental) The connection type name as expected by Connection resource.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.invoke(self, "toString", []))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="JDBC")
     def JDBC(cls) -> "ConnectionType":
         '''(experimental) Designates a connection to a database through Java Database Connectivity (JDBC).
 
         :stability: experimental
         '''
         return typing.cast("ConnectionType", jsii.sget(cls, "JDBC"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="KAFKA")
     def KAFKA(cls) -> "ConnectionType":
         '''(experimental) Designates a connection to an Apache Kafka streaming platform.
 
         :stability: experimental
         '''
         return typing.cast("ConnectionType", jsii.sget(cls, "KAFKA"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="MONGODB")
     def MONGODB(cls) -> "ConnectionType":
         '''(experimental) Designates a connection to a MongoDB document database.
 
         :stability: experimental
         '''
         return typing.cast("ConnectionType", jsii.sget(cls, "MONGODB"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="NETWORK")
     def NETWORK(cls) -> "ConnectionType":
         '''(experimental) Designates a network connection to a data source within an Amazon Virtual Private Cloud environment (Amazon VPC).
 
         :stability: experimental
         '''
         return typing.cast("ConnectionType", jsii.sget(cls, "NETWORK"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         '''(experimental) The name of this ConnectionType, as expected by Connection resource.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "name"))
@@ -1461,15 +1356,15 @@
 )
 class ContinuousLoggingProps:
     def __init__(
         self,
         *,
         enabled: builtins.bool,
         conversion_pattern: typing.Optional[builtins.str] = None,
-        log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
+        log_group: typing.Optional[aws_cdk.aws_logs.ILogGroup] = None,
         log_stream_prefix: typing.Optional[builtins.str] = None,
         quiet: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''(experimental) Properties for enabling Continuous Logging for Glue Jobs.
 
         :param enabled: (experimental) Enable continouous logging.
         :param conversion_pattern: (experimental) Apply the provided conversion pattern. This is a Log4j Conversion Pattern to customize driver and executor logs. Default: ``%d{yy/MM/dd HH:mm:ss} %p %c{1}: %m%n``
@@ -1496,22 +1391,15 @@
                 # the properties below are optional
                 conversion_pattern="conversionPattern",
                 log_group=log_group,
                 log_stream_prefix="logStreamPrefix",
                 quiet=False
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6be4bb41017f52f2aa453e36400fa3a47b2e6bf3a87cf64d46e0345d6f22428b)
-            check_type(argname="argument enabled", value=enabled, expected_type=type_hints["enabled"])
-            check_type(argname="argument conversion_pattern", value=conversion_pattern, expected_type=type_hints["conversion_pattern"])
-            check_type(argname="argument log_group", value=log_group, expected_type=type_hints["log_group"])
-            check_type(argname="argument log_stream_prefix", value=log_stream_prefix, expected_type=type_hints["log_stream_prefix"])
-            check_type(argname="argument quiet", value=quiet, expected_type=type_hints["quiet"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "enabled": enabled,
         }
         if conversion_pattern is not None:
             self._values["conversion_pattern"] = conversion_pattern
         if log_group is not None:
             self._values["log_group"] = log_group
         if log_stream_prefix is not None:
@@ -1539,23 +1427,23 @@
 
         :stability: experimental
         '''
         result = self._values.get("conversion_pattern")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def log_group(self) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup]:
+    def log_group(self) -> typing.Optional[aws_cdk.aws_logs.ILogGroup]:
         '''(experimental) Specify a custom CloudWatch log group name.
 
         :default: - a log group is created with name ``/aws-glue/jobs/logs-v2/``.
 
         :stability: experimental
         '''
         result = self._values.get("log_group")
-        return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_logs.ILogGroup], result)
 
     @builtins.property
     def log_stream_prefix(self) -> typing.Optional[builtins.str]:
         '''(experimental) Specify a custom CloudWatch log stream prefix.
 
         :default: - the job run ID.
 
@@ -1598,14 +1486,15 @@
 
     Example::
 
         # my_database: glue.Database
         
         glue.Table(self, "MyTable",
             database=my_database,
+            table_name="my_table",
             columns=[glue.Column(
                 name="col1",
                 type=glue.Schema.STRING
             )],
             partition_keys=[glue.Column(
                 name="year",
                 type=glue.Schema.SMALL_INT
@@ -1638,136 +1527,136 @@
             output_format=output_format,
             serialization_library=serialization_library,
             classification_string=classification_string,
         )
 
         jsii.create(self.__class__, self, [props])
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="APACHE_LOGS")
     def APACHE_LOGS(cls) -> "DataFormat":
         '''(experimental) DataFormat for Apache Web Server Logs.
 
         Also works for CloudFront logs
 
         :see: https://docs.aws.amazon.com/athena/latest/ug/apache.html
         :stability: experimental
         '''
         return typing.cast("DataFormat", jsii.sget(cls, "APACHE_LOGS"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="AVRO")
     def AVRO(cls) -> "DataFormat":
         '''(experimental) DataFormat for Apache Avro.
 
         :see: https://docs.aws.amazon.com/athena/latest/ug/avro.html
         :stability: experimental
         '''
         return typing.cast("DataFormat", jsii.sget(cls, "AVRO"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="CLOUDTRAIL_LOGS")
     def CLOUDTRAIL_LOGS(cls) -> "DataFormat":
         '''(experimental) DataFormat for CloudTrail logs stored on S3.
 
         :see: https://docs.aws.amazon.com/athena/latest/ug/cloudtrail.html
         :stability: experimental
         '''
         return typing.cast("DataFormat", jsii.sget(cls, "CLOUDTRAIL_LOGS"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="CSV")
     def CSV(cls) -> "DataFormat":
         '''(experimental) DataFormat for CSV Files.
 
         :see: https://docs.aws.amazon.com/athena/latest/ug/csv.html
         :stability: experimental
         '''
         return typing.cast("DataFormat", jsii.sget(cls, "CSV"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="JSON")
     def JSON(cls) -> "DataFormat":
         '''(experimental) Stored as plain text files in JSON format.
 
         Uses OpenX Json SerDe for serialization and deseralization.
 
         :see: https://docs.aws.amazon.com/athena/latest/ug/json.html
         :stability: experimental
         '''
         return typing.cast("DataFormat", jsii.sget(cls, "JSON"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="LOGSTASH")
     def LOGSTASH(cls) -> "DataFormat":
         '''(experimental) DataFormat for Logstash Logs, using the GROK SerDe.
 
         :see: https://docs.aws.amazon.com/athena/latest/ug/grok.html
         :stability: experimental
         '''
         return typing.cast("DataFormat", jsii.sget(cls, "LOGSTASH"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="ORC")
     def ORC(cls) -> "DataFormat":
         '''(experimental) DataFormat for Apache ORC (Optimized Row Columnar).
 
         :see: https://docs.aws.amazon.com/athena/latest/ug/orc.html
         :stability: experimental
         '''
         return typing.cast("DataFormat", jsii.sget(cls, "ORC"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="PARQUET")
     def PARQUET(cls) -> "DataFormat":
         '''(experimental) DataFormat for Apache Parquet.
 
         :see: https://docs.aws.amazon.com/athena/latest/ug/parquet.html
         :stability: experimental
         '''
         return typing.cast("DataFormat", jsii.sget(cls, "PARQUET"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="TSV")
     def TSV(cls) -> "DataFormat":
         '''(experimental) DataFormat for TSV (Tab-Separated Values).
 
         :see: https://docs.aws.amazon.com/athena/latest/ug/lazy-simple-serde.html
         :stability: experimental
         '''
         return typing.cast("DataFormat", jsii.sget(cls, "TSV"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="inputFormat")
     def input_format(self) -> "InputFormat":
         '''(experimental) ``InputFormat`` for this data format.
 
         :stability: experimental
         '''
         return typing.cast("InputFormat", jsii.get(self, "inputFormat"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="outputFormat")
     def output_format(self) -> "OutputFormat":
         '''(experimental) ``OutputFormat`` for this data format.
 
         :stability: experimental
         '''
         return typing.cast("OutputFormat", jsii.get(self, "outputFormat"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="serializationLibrary")
     def serialization_library(self) -> "SerializationLibrary":
         '''(experimental) Serialization library for this data format.
 
         :stability: experimental
         '''
         return typing.cast("SerializationLibrary", jsii.get(self, "serializationLibrary"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="classificationString")
     def classification_string(self) -> typing.Optional[ClassificationString]:
         '''(experimental) Classification string given to tables with this data format.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[ClassificationString], jsii.get(self, "classificationString"))
@@ -1818,21 +1707,15 @@
                 output_format=output_format,
                 serialization_library=serialization_library,
             
                 # the properties below are optional
                 classification_string=classification_string
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f5302ed9f621270e44cf453ed62f78ee39e66f12961a87e084ec3d874438a19f)
-            check_type(argname="argument input_format", value=input_format, expected_type=type_hints["input_format"])
-            check_type(argname="argument output_format", value=output_format, expected_type=type_hints["output_format"])
-            check_type(argname="argument serialization_library", value=serialization_library, expected_type=type_hints["serialization_library"])
-            check_type(argname="argument classification_string", value=classification_string, expected_type=type_hints["classification_string"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "input_format": input_format,
             "output_format": output_format,
             "serialization_library": serialization_library,
         }
         if classification_string is not None:
             self._values["classification_string"] = classification_string
 
@@ -1894,55 +1777,45 @@
     jsii_struct_bases=[],
     name_mapping={"database_name": "databaseName", "location_uri": "locationUri"},
 )
 class DatabaseProps:
     def __init__(
         self,
         *,
-        database_name: typing.Optional[builtins.str] = None,
+        database_name: builtins.str,
         location_uri: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param database_name: (experimental) The name of the database. Default: - generated by CDK.
+        :param database_name: (experimental) The name of the database.
         :param location_uri: (experimental) The location of the database (for example, an HDFS path). Default: undefined. This field is optional in AWS::Glue::Database DatabaseInput
 
         :stability: experimental
-        :exampleMetadata: fixture=_generated
+        :exampleMetadata: infused
 
         Example::
 
-            # The code below shows an example of how to instantiate this type.
-            # The values are placeholders you should change.
-            import aws_cdk.aws_glue_alpha as glue_alpha
-            
-            database_props = glue_alpha.DatabaseProps(
-                database_name="databaseName",
-                location_uri="locationUri"
+            glue.Database(self, "MyDatabase",
+                database_name="my_database"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d07df31a9d41958f45422a1d7914c5016d66ed0e46a7e97ab37e2dd3d42ecf38)
-            check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
-            check_type(argname="argument location_uri", value=location_uri, expected_type=type_hints["location_uri"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
-        if database_name is not None:
-            self._values["database_name"] = database_name
+        self._values: typing.Dict[str, typing.Any] = {
+            "database_name": database_name,
+        }
         if location_uri is not None:
             self._values["location_uri"] = location_uri
 
     @builtins.property
-    def database_name(self) -> typing.Optional[builtins.str]:
+    def database_name(self) -> builtins.str:
         '''(experimental) The name of the database.
 
-        :default: - generated by CDK.
-
         :stability: experimental
         '''
         result = self._values.get("database_name")
-        return typing.cast(typing.Optional[builtins.str], result)
+        assert result is not None, "Required property 'database_name' is missing"
+        return typing.cast(builtins.str, result)
 
     @builtins.property
     def location_uri(self) -> typing.Optional[builtins.str]:
         '''(experimental) The location of the database (for example, an HDFS path).
 
         :default: undefined. This field is optional in AWS::Glue::Database DatabaseInput
 
@@ -1977,273 +1850,259 @@
     If you need to use a GlueVersion that doesn't exist as a static member, you
     can instantiate a ``GlueVersion`` object, e.g: ``GlueVersion.of('1.5')``.
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
-        glue.Job(self, "PythonSparkStreamingJob",
-            executable=glue.JobExecutable.python_streaming(
-                glue_version=glue.GlueVersion.V4_0,
+        # bucket: s3.Bucket
+        
+        glue.Job(self, "PythonShellJob",
+            executable=glue.JobExecutable.python_shell(
+                glue_version=glue.GlueVersion.V1_0,
                 python_version=glue.PythonVersion.THREE,
-                script=glue.Code.from_asset(path.join(__dirname, "job-script/hello_world.py"))
+                script=glue.Code.from_bucket(bucket, "script.py")
             ),
-            description="an example Python Streaming job"
+            description="an example Python Shell job"
         )
     '''
 
-    @jsii.member(jsii_name="of")
+    @jsii.member(jsii_name="of") # type: ignore[misc]
     @builtins.classmethod
     def of(cls, version: builtins.str) -> "GlueVersion":
         '''(experimental) Custom Glue version.
 
         :param version: custom version.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1bf24e914c5a2058c5a8ba633944792fe46a62d0d67ae96056f15edaf764112b)
-            check_type(argname="argument version", value=version, expected_type=type_hints["version"])
         return typing.cast("GlueVersion", jsii.sinvoke(cls, "of", [version]))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V0_9")
     def V0_9(cls) -> "GlueVersion":
         '''(experimental) Glue version using Spark 2.2.1 and Python 2.7.
 
         :stability: experimental
         '''
         return typing.cast("GlueVersion", jsii.sget(cls, "V0_9"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V1_0")
     def V1_0(cls) -> "GlueVersion":
         '''(experimental) Glue version using Spark 2.4.3, Python 2.7 and Python 3.6.
 
         :stability: experimental
         '''
         return typing.cast("GlueVersion", jsii.sget(cls, "V1_0"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V2_0")
     def V2_0(cls) -> "GlueVersion":
         '''(experimental) Glue version using Spark 2.4.3 and Python 3.7.
 
         :stability: experimental
         '''
         return typing.cast("GlueVersion", jsii.sget(cls, "V2_0"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="V3_0")
     def V3_0(cls) -> "GlueVersion":
         '''(experimental) Glue version using Spark 3.1.1 and Python 3.7.
 
         :stability: experimental
         '''
         return typing.cast("GlueVersion", jsii.sget(cls, "V3_0"))
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V4_0")
-    def V4_0(cls) -> "GlueVersion":
-        '''(experimental) Glue version using Spark 3.3.0 and Python 3.10.
-
-        :stability: experimental
-        '''
-        return typing.cast("GlueVersion", jsii.sget(cls, "V4_0"))
-
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         '''(experimental) The name of this GlueVersion, as expected by Job resource.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "name"))
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-glue-alpha.IConnection")
-class IConnection(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
-    '''(experimental) Interface representing a created or an imported ``Connection``.
+class IConnection(aws_cdk.IResource, typing_extensions.Protocol):
+    '''(experimental) Interface representing a created or an imported {@link Connection}.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="connectionArn")
     def connection_arn(self) -> builtins.str:
         '''(experimental) The ARN of the connection.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="connectionName")
     def connection_name(self) -> builtins.str:
         '''(experimental) The name of the connection.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _IConnectionProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
-    '''(experimental) Interface representing a created or an imported ``Connection``.
+    '''(experimental) Interface representing a created or an imported {@link Connection}.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-glue-alpha.IConnection"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="connectionArn")
     def connection_arn(self) -> builtins.str:
         '''(experimental) The ARN of the connection.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "connectionArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="connectionName")
     def connection_name(self) -> builtins.str:
         '''(experimental) The name of the connection.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "connectionName"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IConnection).__jsii_proxy_class__ = lambda : _IConnectionProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-glue-alpha.IDatabase")
-class IDatabase(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class IDatabase(aws_cdk.IResource, typing_extensions.Protocol):
     '''
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="catalogArn")
     def catalog_arn(self) -> builtins.str:
         '''(experimental) The ARN of the catalog.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="catalogId")
     def catalog_id(self) -> builtins.str:
         '''(experimental) The catalog id of the database (usually, the AWS account id).
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="databaseArn")
     def database_arn(self) -> builtins.str:
         '''(experimental) The ARN of the database.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="databaseName")
     def database_name(self) -> builtins.str:
         '''(experimental) The name of the database.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _IDatabaseProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-glue-alpha.IDatabase"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="catalogArn")
     def catalog_arn(self) -> builtins.str:
         '''(experimental) The ARN of the catalog.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "catalogArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="catalogId")
     def catalog_id(self) -> builtins.str:
         '''(experimental) The catalog id of the database (usually, the AWS account id).
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "catalogId"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="databaseArn")
     def database_arn(self) -> builtins.str:
         '''(experimental) The ARN of the database.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "databaseArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="databaseName")
     def database_name(self) -> builtins.str:
         '''(experimental) The name of the database.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "databaseName"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IDatabase).__jsii_proxy_class__ = lambda : _IDatabaseProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-glue-alpha.IJob")
-class IJob(
-    _aws_cdk_ceddda9d.IResource,
-    _aws_cdk_aws_iam_ceddda9d.IGrantable,
-    typing_extensions.Protocol,
-):
-    '''(experimental) Interface representing a created or an imported ``Job``.
+class IJob(aws_cdk.IResource, aws_cdk.aws_iam.IGrantable, typing_extensions.Protocol):
+    '''(experimental) Interface representing a created or an imported {@link Job}.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="jobArn")
     def job_arn(self) -> builtins.str:
         '''(experimental) The ARN of the job.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="jobName")
     def job_name(self) -> builtins.str:
         '''(experimental) The name of the job.
 
         :stability: experimental
         :attribute: true
         '''
@@ -2255,30 +2114,30 @@
         metric_name: builtins.str,
         type: "MetricType",
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
         '''(experimental) Create a CloudWatch metric.
 
         :param metric_name: name of the metric typically prefixed with ``glue.driver.``, ``glue.<executorId>.`` or ``glue.ALL.``.
         :param type: the metric type.
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
 
         :see: https://docs.aws.amazon.com/glue/latest/dg/monitoring-awsglue-with-cloudwatch-metrics.html
         :stability: experimental
         '''
         ...
 
@@ -2286,240 +2145,230 @@
     def metric_failure(
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
         '''(experimental) Create a CloudWatch Metric indicating job failure.
 
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
 
     @jsii.member(jsii_name="metricSuccess")
     def metric_success(
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
         '''(experimental) Create a CloudWatch Metric indicating job success.
 
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
 
     @jsii.member(jsii_name="metricTimeout")
     def metric_timeout(
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
         '''(experimental) Create a CloudWatch Metric indicating job timeout.
 
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
 
     @jsii.member(jsii_name="onEvent")
     def on_event(
         self,
         id: builtins.str,
         *,
-        target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-        cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
         description: typing.Optional[builtins.str] = None,
-        event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
+        event_pattern: typing.Optional[aws_cdk.aws_events.EventPattern] = None,
         rule_name: typing.Optional[builtins.str] = None,
-    ) -> _aws_cdk_aws_events_ceddda9d.Rule:
+        target: typing.Optional[aws_cdk.aws_events.IRuleTarget] = None,
+    ) -> aws_cdk.aws_events.Rule:
         '''(experimental) Defines a CloudWatch event rule triggered when something happens with this job.
 
         :param id: -
-        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
-        :param cross_stack_scope: The scope to use if the source of the rule and its target are in different Stacks (but in the same account & region). This helps dealing with cycles that often arise in these situations. Default: - none (the main scope will be used, even for cross-stack Events)
         :param description: A description of the rule's purpose. Default: - No description
         :param event_pattern: Additional restrictions for the event to route to the specified target. The method that generates the rule probably imposes some type of event filtering. The filtering implied by what you pass here is added on top of that filtering. Default: - No additional filtering based on an event pattern.
         :param rule_name: A name for the rule. Default: AWS CloudFormation generates a unique physical ID.
+        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/EventTypes.html#glue-event-types
         :stability: experimental
         '''
         ...
 
     @jsii.member(jsii_name="onFailure")
     def on_failure(
         self,
         id: builtins.str,
         *,
-        target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-        cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
         description: typing.Optional[builtins.str] = None,
-        event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
+        event_pattern: typing.Optional[aws_cdk.aws_events.EventPattern] = None,
         rule_name: typing.Optional[builtins.str] = None,
-    ) -> _aws_cdk_aws_events_ceddda9d.Rule:
+        target: typing.Optional[aws_cdk.aws_events.IRuleTarget] = None,
+    ) -> aws_cdk.aws_events.Rule:
         '''(experimental) Defines a CloudWatch event rule triggered when this job moves to the FAILED state.
 
         :param id: -
-        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
-        :param cross_stack_scope: The scope to use if the source of the rule and its target are in different Stacks (but in the same account & region). This helps dealing with cycles that often arise in these situations. Default: - none (the main scope will be used, even for cross-stack Events)
         :param description: A description of the rule's purpose. Default: - No description
         :param event_pattern: Additional restrictions for the event to route to the specified target. The method that generates the rule probably imposes some type of event filtering. The filtering implied by what you pass here is added on top of that filtering. Default: - No additional filtering based on an event pattern.
         :param rule_name: A name for the rule. Default: AWS CloudFormation generates a unique physical ID.
+        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/EventTypes.html#glue-event-types
         :stability: experimental
         '''
         ...
 
     @jsii.member(jsii_name="onStateChange")
     def on_state_change(
         self,
         id: builtins.str,
         job_state: "JobState",
         *,
-        target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-        cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
         description: typing.Optional[builtins.str] = None,
-        event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
+        event_pattern: typing.Optional[aws_cdk.aws_events.EventPattern] = None,
         rule_name: typing.Optional[builtins.str] = None,
-    ) -> _aws_cdk_aws_events_ceddda9d.Rule:
+        target: typing.Optional[aws_cdk.aws_events.IRuleTarget] = None,
+    ) -> aws_cdk.aws_events.Rule:
         '''(experimental) Defines a CloudWatch event rule triggered when this job moves to the input jobState.
 
         :param id: -
         :param job_state: -
-        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
-        :param cross_stack_scope: The scope to use if the source of the rule and its target are in different Stacks (but in the same account & region). This helps dealing with cycles that often arise in these situations. Default: - none (the main scope will be used, even for cross-stack Events)
         :param description: A description of the rule's purpose. Default: - No description
         :param event_pattern: Additional restrictions for the event to route to the specified target. The method that generates the rule probably imposes some type of event filtering. The filtering implied by what you pass here is added on top of that filtering. Default: - No additional filtering based on an event pattern.
         :param rule_name: A name for the rule. Default: AWS CloudFormation generates a unique physical ID.
+        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/EventTypes.html#glue-event-types
         :stability: experimental
         '''
         ...
 
     @jsii.member(jsii_name="onSuccess")
     def on_success(
         self,
         id: builtins.str,
         *,
-        target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-        cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
         description: typing.Optional[builtins.str] = None,
-        event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
+        event_pattern: typing.Optional[aws_cdk.aws_events.EventPattern] = None,
         rule_name: typing.Optional[builtins.str] = None,
-    ) -> _aws_cdk_aws_events_ceddda9d.Rule:
+        target: typing.Optional[aws_cdk.aws_events.IRuleTarget] = None,
+    ) -> aws_cdk.aws_events.Rule:
         '''(experimental) Defines a CloudWatch event rule triggered when this job moves to the SUCCEEDED state.
 
         :param id: -
-        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
-        :param cross_stack_scope: The scope to use if the source of the rule and its target are in different Stacks (but in the same account & region). This helps dealing with cycles that often arise in these situations. Default: - none (the main scope will be used, even for cross-stack Events)
         :param description: A description of the rule's purpose. Default: - No description
         :param event_pattern: Additional restrictions for the event to route to the specified target. The method that generates the rule probably imposes some type of event filtering. The filtering implied by what you pass here is added on top of that filtering. Default: - No additional filtering based on an event pattern.
         :param rule_name: A name for the rule. Default: AWS CloudFormation generates a unique physical ID.
+        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/EventTypes.html#glue-event-types
         :stability: experimental
         '''
         ...
 
     @jsii.member(jsii_name="onTimeout")
     def on_timeout(
         self,
         id: builtins.str,
         *,
-        target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-        cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
         description: typing.Optional[builtins.str] = None,
-        event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
+        event_pattern: typing.Optional[aws_cdk.aws_events.EventPattern] = None,
         rule_name: typing.Optional[builtins.str] = None,
-    ) -> _aws_cdk_aws_events_ceddda9d.Rule:
+        target: typing.Optional[aws_cdk.aws_events.IRuleTarget] = None,
+    ) -> aws_cdk.aws_events.Rule:
         '''(experimental) Defines a CloudWatch event rule triggered when this job moves to the TIMEOUT state.
 
         :param id: -
-        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
-        :param cross_stack_scope: The scope to use if the source of the rule and its target are in different Stacks (but in the same account & region). This helps dealing with cycles that often arise in these situations. Default: - none (the main scope will be used, even for cross-stack Events)
         :param description: A description of the rule's purpose. Default: - No description
         :param event_pattern: Additional restrictions for the event to route to the specified target. The method that generates the rule probably imposes some type of event filtering. The filtering implied by what you pass here is added on top of that filtering. Default: - No additional filtering based on an event pattern.
         :param rule_name: A name for the rule. Default: AWS CloudFormation generates a unique physical ID.
+        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/EventTypes.html#glue-event-types
         :stability: experimental
         '''
         ...
 
 
 class _IJobProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
-    jsii.proxy_for(_aws_cdk_aws_iam_ceddda9d.IGrantable), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.aws_iam.IGrantable), # type: ignore[misc]
 ):
-    '''(experimental) Interface representing a created or an imported ``Job``.
+    '''(experimental) Interface representing a created or an imported {@link Job}.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-glue-alpha.IJob"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="jobArn")
     def job_arn(self) -> builtins.str:
         '''(experimental) The ARN of the job.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "jobArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="jobName")
     def job_name(self) -> builtins.str:
         '''(experimental) The name of the job.
 
         :stability: experimental
         :attribute: true
         '''
@@ -2531,442 +2380,407 @@
         metric_name: builtins.str,
         type: "MetricType",
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
         '''(experimental) Create a CloudWatch metric.
 
         :param metric_name: name of the metric typically prefixed with ``glue.driver.``, ``glue.<executorId>.`` or ``glue.ALL.``.
         :param type: the metric type.
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
 
         :see: https://docs.aws.amazon.com/glue/latest/dg/monitoring-awsglue-with-cloudwatch-metrics.html
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__79f8eb7ba0850dad06f49887b6323e6019fa48cdf967d96e579591ff36e61765)
-            check_type(argname="argument metric_name", value=metric_name, expected_type=type_hints["metric_name"])
-            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metric", [metric_name, type, props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metric", [metric_name, type, props]))
 
     @jsii.member(jsii_name="metricFailure")
     def metric_failure(
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
         '''(experimental) Create a CloudWatch Metric indicating job failure.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricFailure", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricFailure", [props]))
 
     @jsii.member(jsii_name="metricSuccess")
     def metric_success(
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
         '''(experimental) Create a CloudWatch Metric indicating job success.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricSuccess", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricSuccess", [props]))
 
     @jsii.member(jsii_name="metricTimeout")
     def metric_timeout(
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
         '''(experimental) Create a CloudWatch Metric indicating job timeout.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricTimeout", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricTimeout", [props]))
 
     @jsii.member(jsii_name="onEvent")
     def on_event(
         self,
         id: builtins.str,
         *,
-        target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-        cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
         description: typing.Optional[builtins.str] = None,
-        event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
+        event_pattern: typing.Optional[aws_cdk.aws_events.EventPattern] = None,
         rule_name: typing.Optional[builtins.str] = None,
-    ) -> _aws_cdk_aws_events_ceddda9d.Rule:
+        target: typing.Optional[aws_cdk.aws_events.IRuleTarget] = None,
+    ) -> aws_cdk.aws_events.Rule:
         '''(experimental) Defines a CloudWatch event rule triggered when something happens with this job.
 
         :param id: -
-        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
-        :param cross_stack_scope: The scope to use if the source of the rule and its target are in different Stacks (but in the same account & region). This helps dealing with cycles that often arise in these situations. Default: - none (the main scope will be used, even for cross-stack Events)
         :param description: A description of the rule's purpose. Default: - No description
         :param event_pattern: Additional restrictions for the event to route to the specified target. The method that generates the rule probably imposes some type of event filtering. The filtering implied by what you pass here is added on top of that filtering. Default: - No additional filtering based on an event pattern.
         :param rule_name: A name for the rule. Default: AWS CloudFormation generates a unique physical ID.
+        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/EventTypes.html#glue-event-types
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4e9bb641a392e36442ae2624591822707bc3af7603043bcb85c82e6dde0aedff)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        options = _aws_cdk_aws_events_ceddda9d.OnEventOptions(
-            target=target,
-            cross_stack_scope=cross_stack_scope,
+        options = aws_cdk.aws_events.OnEventOptions(
             description=description,
             event_pattern=event_pattern,
             rule_name=rule_name,
+            target=target,
         )
 
-        return typing.cast(_aws_cdk_aws_events_ceddda9d.Rule, jsii.invoke(self, "onEvent", [id, options]))
+        return typing.cast(aws_cdk.aws_events.Rule, jsii.invoke(self, "onEvent", [id, options]))
 
     @jsii.member(jsii_name="onFailure")
     def on_failure(
         self,
         id: builtins.str,
         *,
-        target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-        cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
         description: typing.Optional[builtins.str] = None,
-        event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
+        event_pattern: typing.Optional[aws_cdk.aws_events.EventPattern] = None,
         rule_name: typing.Optional[builtins.str] = None,
-    ) -> _aws_cdk_aws_events_ceddda9d.Rule:
+        target: typing.Optional[aws_cdk.aws_events.IRuleTarget] = None,
+    ) -> aws_cdk.aws_events.Rule:
         '''(experimental) Defines a CloudWatch event rule triggered when this job moves to the FAILED state.
 
         :param id: -
-        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
-        :param cross_stack_scope: The scope to use if the source of the rule and its target are in different Stacks (but in the same account & region). This helps dealing with cycles that often arise in these situations. Default: - none (the main scope will be used, even for cross-stack Events)
         :param description: A description of the rule's purpose. Default: - No description
         :param event_pattern: Additional restrictions for the event to route to the specified target. The method that generates the rule probably imposes some type of event filtering. The filtering implied by what you pass here is added on top of that filtering. Default: - No additional filtering based on an event pattern.
         :param rule_name: A name for the rule. Default: AWS CloudFormation generates a unique physical ID.
+        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/EventTypes.html#glue-event-types
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__192bf1eecc268b3f759e65151917fb49666d5a0144c2df120f2dd72e3fd5e4f4)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        options = _aws_cdk_aws_events_ceddda9d.OnEventOptions(
-            target=target,
-            cross_stack_scope=cross_stack_scope,
+        options = aws_cdk.aws_events.OnEventOptions(
             description=description,
             event_pattern=event_pattern,
             rule_name=rule_name,
+            target=target,
         )
 
-        return typing.cast(_aws_cdk_aws_events_ceddda9d.Rule, jsii.invoke(self, "onFailure", [id, options]))
+        return typing.cast(aws_cdk.aws_events.Rule, jsii.invoke(self, "onFailure", [id, options]))
 
     @jsii.member(jsii_name="onStateChange")
     def on_state_change(
         self,
         id: builtins.str,
         job_state: "JobState",
         *,
-        target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-        cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
         description: typing.Optional[builtins.str] = None,
-        event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
+        event_pattern: typing.Optional[aws_cdk.aws_events.EventPattern] = None,
         rule_name: typing.Optional[builtins.str] = None,
-    ) -> _aws_cdk_aws_events_ceddda9d.Rule:
+        target: typing.Optional[aws_cdk.aws_events.IRuleTarget] = None,
+    ) -> aws_cdk.aws_events.Rule:
         '''(experimental) Defines a CloudWatch event rule triggered when this job moves to the input jobState.
 
         :param id: -
         :param job_state: -
-        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
-        :param cross_stack_scope: The scope to use if the source of the rule and its target are in different Stacks (but in the same account & region). This helps dealing with cycles that often arise in these situations. Default: - none (the main scope will be used, even for cross-stack Events)
         :param description: A description of the rule's purpose. Default: - No description
         :param event_pattern: Additional restrictions for the event to route to the specified target. The method that generates the rule probably imposes some type of event filtering. The filtering implied by what you pass here is added on top of that filtering. Default: - No additional filtering based on an event pattern.
         :param rule_name: A name for the rule. Default: AWS CloudFormation generates a unique physical ID.
+        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/EventTypes.html#glue-event-types
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__bab9c989bad00c9e92013f90e2646073cc90125f09e75268ec3f2999a69b9b8d)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument job_state", value=job_state, expected_type=type_hints["job_state"])
-        options = _aws_cdk_aws_events_ceddda9d.OnEventOptions(
-            target=target,
-            cross_stack_scope=cross_stack_scope,
+        options = aws_cdk.aws_events.OnEventOptions(
             description=description,
             event_pattern=event_pattern,
             rule_name=rule_name,
+            target=target,
         )
 
-        return typing.cast(_aws_cdk_aws_events_ceddda9d.Rule, jsii.invoke(self, "onStateChange", [id, job_state, options]))
+        return typing.cast(aws_cdk.aws_events.Rule, jsii.invoke(self, "onStateChange", [id, job_state, options]))
 
     @jsii.member(jsii_name="onSuccess")
     def on_success(
         self,
         id: builtins.str,
         *,
-        target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-        cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
         description: typing.Optional[builtins.str] = None,
-        event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
+        event_pattern: typing.Optional[aws_cdk.aws_events.EventPattern] = None,
         rule_name: typing.Optional[builtins.str] = None,
-    ) -> _aws_cdk_aws_events_ceddda9d.Rule:
+        target: typing.Optional[aws_cdk.aws_events.IRuleTarget] = None,
+    ) -> aws_cdk.aws_events.Rule:
         '''(experimental) Defines a CloudWatch event rule triggered when this job moves to the SUCCEEDED state.
 
         :param id: -
-        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
-        :param cross_stack_scope: The scope to use if the source of the rule and its target are in different Stacks (but in the same account & region). This helps dealing with cycles that often arise in these situations. Default: - none (the main scope will be used, even for cross-stack Events)
         :param description: A description of the rule's purpose. Default: - No description
         :param event_pattern: Additional restrictions for the event to route to the specified target. The method that generates the rule probably imposes some type of event filtering. The filtering implied by what you pass here is added on top of that filtering. Default: - No additional filtering based on an event pattern.
         :param rule_name: A name for the rule. Default: AWS CloudFormation generates a unique physical ID.
+        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/EventTypes.html#glue-event-types
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5b62843a9fea91eb93e6bf7bcd95a76fc790b72a6a7ae7024cf486b3fd9d20f7)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        options = _aws_cdk_aws_events_ceddda9d.OnEventOptions(
-            target=target,
-            cross_stack_scope=cross_stack_scope,
+        options = aws_cdk.aws_events.OnEventOptions(
             description=description,
             event_pattern=event_pattern,
             rule_name=rule_name,
+            target=target,
         )
 
-        return typing.cast(_aws_cdk_aws_events_ceddda9d.Rule, jsii.invoke(self, "onSuccess", [id, options]))
+        return typing.cast(aws_cdk.aws_events.Rule, jsii.invoke(self, "onSuccess", [id, options]))
 
     @jsii.member(jsii_name="onTimeout")
     def on_timeout(
         self,
         id: builtins.str,
         *,
-        target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-        cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
         description: typing.Optional[builtins.str] = None,
-        event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
+        event_pattern: typing.Optional[aws_cdk.aws_events.EventPattern] = None,
         rule_name: typing.Optional[builtins.str] = None,
-    ) -> _aws_cdk_aws_events_ceddda9d.Rule:
+        target: typing.Optional[aws_cdk.aws_events.IRuleTarget] = None,
+    ) -> aws_cdk.aws_events.Rule:
         '''(experimental) Defines a CloudWatch event rule triggered when this job moves to the TIMEOUT state.
 
         :param id: -
-        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
-        :param cross_stack_scope: The scope to use if the source of the rule and its target are in different Stacks (but in the same account & region). This helps dealing with cycles that often arise in these situations. Default: - none (the main scope will be used, even for cross-stack Events)
         :param description: A description of the rule's purpose. Default: - No description
         :param event_pattern: Additional restrictions for the event to route to the specified target. The method that generates the rule probably imposes some type of event filtering. The filtering implied by what you pass here is added on top of that filtering. Default: - No additional filtering based on an event pattern.
         :param rule_name: A name for the rule. Default: AWS CloudFormation generates a unique physical ID.
+        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/EventTypes.html#glue-event-types
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b1fcdc972ccb29fe1572e8970cb83faccd76d7cee7f09ed3f5c9571bca7a886d)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        options = _aws_cdk_aws_events_ceddda9d.OnEventOptions(
-            target=target,
-            cross_stack_scope=cross_stack_scope,
+        options = aws_cdk.aws_events.OnEventOptions(
             description=description,
             event_pattern=event_pattern,
             rule_name=rule_name,
+            target=target,
         )
 
-        return typing.cast(_aws_cdk_aws_events_ceddda9d.Rule, jsii.invoke(self, "onTimeout", [id, options]))
+        return typing.cast(aws_cdk.aws_events.Rule, jsii.invoke(self, "onTimeout", [id, options]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IJob).__jsii_proxy_class__ = lambda : _IJobProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-glue-alpha.ISecurityConfiguration")
-class ISecurityConfiguration(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
-    '''(experimental) Interface representing a created or an imported ``SecurityConfiguration``.
+class ISecurityConfiguration(aws_cdk.IResource, typing_extensions.Protocol):
+    '''(experimental) Interface representing a created or an imported {@link SecurityConfiguration}.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="securityConfigurationName")
     def security_configuration_name(self) -> builtins.str:
         '''(experimental) The name of the security configuration.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _ISecurityConfigurationProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
-    '''(experimental) Interface representing a created or an imported ``SecurityConfiguration``.
+    '''(experimental) Interface representing a created or an imported {@link SecurityConfiguration}.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-glue-alpha.ISecurityConfiguration"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="securityConfigurationName")
     def security_configuration_name(self) -> builtins.str:
         '''(experimental) The name of the security configuration.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "securityConfigurationName"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, ISecurityConfiguration).__jsii_proxy_class__ = lambda : _ISecurityConfigurationProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-glue-alpha.ITable")
-class ITable(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class ITable(aws_cdk.IResource, typing_extensions.Protocol):
     '''
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="tableArn")
     def table_arn(self) -> builtins.str:
         '''
         :stability: experimental
         :attribute: true
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="tableName")
     def table_name(self) -> builtins.str:
         '''
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _ITableProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-glue-alpha.ITable"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="tableArn")
     def table_arn(self) -> builtins.str:
         '''
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "tableArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="tableName")
     def table_name(self) -> builtins.str:
         '''
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "tableName"))
@@ -2995,158 +2809,153 @@
 
     def __init__(self, class_name: builtins.str) -> None:
         '''
         :param class_name: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__697ee4e4007ce058f39e7fc610b2c0c4457bbd6008e9287406b18505ed299434)
-            check_type(argname="argument class_name", value=class_name, expected_type=type_hints["class_name"])
         jsii.create(self.__class__, self, [class_name])
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="AVRO")
     def AVRO(cls) -> "InputFormat":
         '''(experimental) InputFormat for Avro files.
 
-        :see: https://svn.apache.org/repos/infra/websites/production/hive/content/javadocs/r3.1.3/api/org/apache/hadoop/hive/ql/io/avro/AvroContainerInputFormat.html
+        :see: https://hive.apache.org/javadocs/r1.2.2/api/org/apache/hadoop/hive/ql/io/avro/AvroContainerInputFormat.html
         :stability: experimental
         '''
         return typing.cast("InputFormat", jsii.sget(cls, "AVRO"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="CLOUDTRAIL")
     def CLOUDTRAIL(cls) -> "InputFormat":
         '''(experimental) InputFormat for Cloudtrail Logs.
 
         :see: https://docs.aws.amazon.com/athena/latest/ug/cloudtrail.html
         :stability: experimental
         '''
         return typing.cast("InputFormat", jsii.sget(cls, "CLOUDTRAIL"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="ORC")
     def ORC(cls) -> "InputFormat":
         '''(experimental) InputFormat for Orc files.
 
-        :see: https://svn.apache.org/repos/infra/websites/production/hive/content/javadocs/r3.1.3/api/org/apache/hadoop/hive/ql/io/orc/OrcInputFormat.html
+        :see: https://hive.apache.org/javadocs/r1.2.2/api/org/apache/hadoop/hive/ql/io/orc/OrcInputFormat.html
         :stability: experimental
         '''
         return typing.cast("InputFormat", jsii.sget(cls, "ORC"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="PARQUET")
     def PARQUET(cls) -> "InputFormat":
         '''(experimental) InputFormat for Parquet files.
 
-        :see: https://svn.apache.org/repos/infra/websites/production/hive/content/javadocs/r3.1.3/api/org/apache/hadoop/hive/ql/io/parquet/MapredParquetInputFormat.html
+        :see: https://hive.apache.org/javadocs/r1.2.2/api/org/apache/hadoop/hive/ql/io/parquet/MapredParquetInputFormat.html
         :stability: experimental
         '''
         return typing.cast("InputFormat", jsii.sget(cls, "PARQUET"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="TEXT")
     def TEXT(cls) -> "InputFormat":
         '''(experimental) An InputFormat for plain text files.
 
         Files are broken into lines. Either linefeed or
         carriage-return are used to signal end of line. Keys are the position in the file, and
         values are the line of text.
         JSON & CSV files are examples of this InputFormat
 
         :see: https://hadoop.apache.org/docs/stable/api/org/apache/hadoop/mapred/TextInputFormat.html
         :stability: experimental
         '''
         return typing.cast("InputFormat", jsii.sget(cls, "TEXT"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="className")
     def class_name(self) -> builtins.str:
         '''
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "className"))
 
 
 @jsii.implements(IJob)
 class Job(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-glue-alpha.Job",
 ):
     '''(experimental) A Glue Job.
 
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
-        glue.Job(self, "PythonSparkStreamingJob",
-            executable=glue.JobExecutable.python_streaming(
-                glue_version=glue.GlueVersion.V4_0,
+        # bucket: s3.Bucket
+        
+        glue.Job(self, "PythonShellJob",
+            executable=glue.JobExecutable.python_shell(
+                glue_version=glue.GlueVersion.V1_0,
                 python_version=glue.PythonVersion.THREE,
-                script=glue.Code.from_asset(path.join(__dirname, "job-script/hello_world.py"))
+                script=glue.Code.from_bucket(bucket, "script.py")
             ),
-            description="an example Python Streaming job"
+            description="an example Python Shell job"
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         executable: "JobExecutable",
         connections: typing.Optional[typing.Sequence[IConnection]] = None,
-        continuous_logging: typing.Optional[typing.Union[ContinuousLoggingProps, typing.Dict[builtins.str, typing.Any]]] = None,
+        continuous_logging: typing.Optional[ContinuousLoggingProps] = None,
         default_arguments: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         description: typing.Optional[builtins.str] = None,
         enable_profiling_metrics: typing.Optional[builtins.bool] = None,
         job_name: typing.Optional[builtins.str] = None,
         max_capacity: typing.Optional[jsii.Number] = None,
         max_concurrent_runs: typing.Optional[jsii.Number] = None,
         max_retries: typing.Optional[jsii.Number] = None,
-        notify_delay_after: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-        role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        notify_delay_after: typing.Optional[aws_cdk.Duration] = None,
+        role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
         security_configuration: typing.Optional[ISecurityConfiguration] = None,
-        spark_ui: typing.Optional[typing.Union["SparkUIProps", typing.Dict[builtins.str, typing.Any]]] = None,
+        spark_ui: typing.Optional["SparkUIProps"] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-        timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        timeout: typing.Optional[aws_cdk.Duration] = None,
         worker_count: typing.Optional[jsii.Number] = None,
         worker_type: typing.Optional["WorkerType"] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param executable: (experimental) The job's executable properties.
-        :param connections: (experimental) The ``Connection``s used for this job. Connections are used to connect to other AWS Service or resources within a VPC. Default: [] - no connections are added to the job
+        :param connections: (experimental) The {@link Connection}s used for this job. Connections are used to connect to other AWS Service or resources within a VPC. Default: [] - no connections are added to the job
         :param continuous_logging: (experimental) Enables continuous logging with the specified props. Default: - continuous logging is disabled.
         :param default_arguments: (experimental) The default arguments for this job, specified as name-value pairs. Default: - no arguments
         :param description: (experimental) The description of the job. Default: - no value
         :param enable_profiling_metrics: (experimental) Enables the collection of metrics for job profiling. Default: - no profiling metrics emitted.
         :param job_name: (experimental) The name of the job. Default: - a name is automatically generated
         :param max_capacity: (experimental) The number of AWS Glue data processing units (DPUs) that can be allocated when this job runs. Cannot be used for Glue version 2.0 and later - workerType and workerCount should be used instead. Default: - 10 when job type is Apache Spark ETL or streaming, 0.0625 when job type is Python shell
         :param max_concurrent_runs: (experimental) The maximum number of concurrent runs allowed for the job. An error is returned when this threshold is reached. The maximum value you can specify is controlled by a service limit. Default: 1
         :param max_retries: (experimental) The maximum number of times to retry this job after a job run fails. Default: 0
         :param notify_delay_after: (experimental) The number of minutes to wait after a job run starts, before sending a job run delay notification. Default: - no delay notifications
         :param role: (experimental) The IAM role assumed by Glue to run this job. If providing a custom role, it needs to trust the Glue service principal (glue.amazonaws.com) and be granted sufficient permissions. Default: - a role is automatically generated
-        :param security_configuration: (experimental) The ``SecurityConfiguration`` to use for this job. Default: - no security configuration.
+        :param security_configuration: (experimental) The {@link SecurityConfiguration} to use for this job. Default: - no security configuration.
         :param spark_ui: (experimental) Enables the Spark UI debugging and monitoring with the specified props. Default: - Spark UI debugging and monitoring is disabled.
         :param tags: (experimental) The tags to add to the resources on which the job runs. Default: {} - no tags
         :param timeout: (experimental) The maximum time that a job run can consume resources before it is terminated and enters TIMEOUT status. Default: cdk.Duration.hours(48)
-        :param worker_count: (experimental) The number of workers of a defined ``WorkerType`` that are allocated when a job runs. Default: - differs based on specific Glue version/worker type
+        :param worker_count: (experimental) The number of workers of a defined {@link WorkerType} that are allocated when a job runs. Default: - differs based on specific Glue version/worker type
         :param worker_type: (experimental) The type of predefined worker that is allocated when a job runs. Default: - differs based on specific Glue version
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e6176c370f308e8911be636fb1acf643512dbe9ca58823d8267644ab7efc406c)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = JobProps(
             executable=executable,
             connections=connections,
             continuous_logging=continuous_logging,
             default_arguments=default_arguments,
             description=description,
             enable_profiling_metrics=enable_profiling_metrics,
@@ -3162,428 +2971,389 @@
             timeout=timeout,
             worker_count=worker_count,
             worker_type=worker_type,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromJobAttributes")
+    @jsii.member(jsii_name="fromJobAttributes") # type: ignore[misc]
     @builtins.classmethod
     def from_job_attributes(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         job_name: builtins.str,
-        role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
     ) -> IJob:
         '''(experimental) Creates a Glue Job.
 
         :param scope: The scope creating construct (usually ``this``).
         :param id: The construct's id.
         :param job_name: (experimental) The name of the job.
         :param role: (experimental) The IAM role assumed by Glue to run this job. Default: - undefined
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__cd8db6c08c7bba32e81d8cda162918f634f3065c707bdd1ddfb404e329994882)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         attrs = JobAttributes(job_name=job_name, role=role)
 
         return typing.cast(IJob, jsii.sinvoke(cls, "fromJobAttributes", [scope, id, attrs]))
 
     @jsii.member(jsii_name="metric")
     def metric(
         self,
         metric_name: builtins.str,
         type: "MetricType",
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
         '''(experimental) Create a CloudWatch metric.
 
         :param metric_name: name of the metric typically prefixed with ``glue.driver.``, ``glue.<executorId>.`` or ``glue.ALL.``.
         :param type: the metric type.
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
 
         :see: https://docs.aws.amazon.com/glue/latest/dg/monitoring-awsglue-with-cloudwatch-metrics.html
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c143c24940c0f180cf99d417380821b95c0287b9b01c42df4f74c6e7959a56b8)
-            check_type(argname="argument metric_name", value=metric_name, expected_type=type_hints["metric_name"])
-            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metric", [metric_name, type, props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metric", [metric_name, type, props]))
 
     @jsii.member(jsii_name="metricFailure")
     def metric_failure(
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
         '''(experimental) Return a CloudWatch Metric indicating job failure.
 
         This metric is based on the Rule returned by no-args onFailure() call.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricFailure", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricFailure", [props]))
 
     @jsii.member(jsii_name="metricSuccess")
     def metric_success(
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
         '''(experimental) Return a CloudWatch Metric indicating job success.
 
         This metric is based on the Rule returned by no-args onSuccess() call.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricSuccess", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricSuccess", [props]))
 
     @jsii.member(jsii_name="metricTimeout")
     def metric_timeout(
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
         '''(experimental) Return a CloudWatch Metric indicating job timeout.
 
         This metric is based on the Rule returned by no-args onTimeout() call.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricTimeout", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricTimeout", [props]))
 
     @jsii.member(jsii_name="onEvent")
     def on_event(
         self,
         id: builtins.str,
         *,
-        target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-        cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
         description: typing.Optional[builtins.str] = None,
-        event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
+        event_pattern: typing.Optional[aws_cdk.aws_events.EventPattern] = None,
         rule_name: typing.Optional[builtins.str] = None,
-    ) -> _aws_cdk_aws_events_ceddda9d.Rule:
+        target: typing.Optional[aws_cdk.aws_events.IRuleTarget] = None,
+    ) -> aws_cdk.aws_events.Rule:
         '''(experimental) Create a CloudWatch Event Rule for this Glue Job when it's in a given state.
 
         :param id: construct id.
-        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
-        :param cross_stack_scope: The scope to use if the source of the rule and its target are in different Stacks (but in the same account & region). This helps dealing with cycles that often arise in these situations. Default: - none (the main scope will be used, even for cross-stack Events)
         :param description: A description of the rule's purpose. Default: - No description
         :param event_pattern: Additional restrictions for the event to route to the specified target. The method that generates the rule probably imposes some type of event filtering. The filtering implied by what you pass here is added on top of that filtering. Default: - No additional filtering based on an event pattern.
         :param rule_name: A name for the rule. Default: AWS CloudFormation generates a unique physical ID.
+        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/EventTypes.html#glue-event-types
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1d8262e07cdf8942bd30cd21bf9d73a8b85e3b2683e99b4f40ed03fbf49b57ac)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        options = _aws_cdk_aws_events_ceddda9d.OnEventOptions(
-            target=target,
-            cross_stack_scope=cross_stack_scope,
+        options = aws_cdk.aws_events.OnEventOptions(
             description=description,
             event_pattern=event_pattern,
             rule_name=rule_name,
+            target=target,
         )
 
-        return typing.cast(_aws_cdk_aws_events_ceddda9d.Rule, jsii.invoke(self, "onEvent", [id, options]))
+        return typing.cast(aws_cdk.aws_events.Rule, jsii.invoke(self, "onEvent", [id, options]))
 
     @jsii.member(jsii_name="onFailure")
     def on_failure(
         self,
         id: builtins.str,
         *,
-        target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-        cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
         description: typing.Optional[builtins.str] = None,
-        event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
+        event_pattern: typing.Optional[aws_cdk.aws_events.EventPattern] = None,
         rule_name: typing.Optional[builtins.str] = None,
-    ) -> _aws_cdk_aws_events_ceddda9d.Rule:
+        target: typing.Optional[aws_cdk.aws_events.IRuleTarget] = None,
+    ) -> aws_cdk.aws_events.Rule:
         '''(experimental) Return a CloudWatch Event Rule matching FAILED state.
 
         :param id: construct id.
-        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
-        :param cross_stack_scope: The scope to use if the source of the rule and its target are in different Stacks (but in the same account & region). This helps dealing with cycles that often arise in these situations. Default: - none (the main scope will be used, even for cross-stack Events)
         :param description: A description of the rule's purpose. Default: - No description
         :param event_pattern: Additional restrictions for the event to route to the specified target. The method that generates the rule probably imposes some type of event filtering. The filtering implied by what you pass here is added on top of that filtering. Default: - No additional filtering based on an event pattern.
         :param rule_name: A name for the rule. Default: AWS CloudFormation generates a unique physical ID.
+        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a8a1d8b4180629a6e1364fed24a3f246786b2d528b0ef21dda37098ac2af2c9a)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        options = _aws_cdk_aws_events_ceddda9d.OnEventOptions(
-            target=target,
-            cross_stack_scope=cross_stack_scope,
+        options = aws_cdk.aws_events.OnEventOptions(
             description=description,
             event_pattern=event_pattern,
             rule_name=rule_name,
+            target=target,
         )
 
-        return typing.cast(_aws_cdk_aws_events_ceddda9d.Rule, jsii.invoke(self, "onFailure", [id, options]))
+        return typing.cast(aws_cdk.aws_events.Rule, jsii.invoke(self, "onFailure", [id, options]))
 
     @jsii.member(jsii_name="onStateChange")
     def on_state_change(
         self,
         id: builtins.str,
         job_state: "JobState",
         *,
-        target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-        cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
         description: typing.Optional[builtins.str] = None,
-        event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
+        event_pattern: typing.Optional[aws_cdk.aws_events.EventPattern] = None,
         rule_name: typing.Optional[builtins.str] = None,
-    ) -> _aws_cdk_aws_events_ceddda9d.Rule:
+        target: typing.Optional[aws_cdk.aws_events.IRuleTarget] = None,
+    ) -> aws_cdk.aws_events.Rule:
         '''(experimental) Create a CloudWatch Event Rule for the transition into the input jobState.
 
         :param id: construct id.
         :param job_state: the job state.
-        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
-        :param cross_stack_scope: The scope to use if the source of the rule and its target are in different Stacks (but in the same account & region). This helps dealing with cycles that often arise in these situations. Default: - none (the main scope will be used, even for cross-stack Events)
         :param description: A description of the rule's purpose. Default: - No description
         :param event_pattern: Additional restrictions for the event to route to the specified target. The method that generates the rule probably imposes some type of event filtering. The filtering implied by what you pass here is added on top of that filtering. Default: - No additional filtering based on an event pattern.
         :param rule_name: A name for the rule. Default: AWS CloudFormation generates a unique physical ID.
+        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0546c2bad534dee21310d2705463267023bd2bd40cd093c29b95dccda7c69228)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument job_state", value=job_state, expected_type=type_hints["job_state"])
-        options = _aws_cdk_aws_events_ceddda9d.OnEventOptions(
-            target=target,
-            cross_stack_scope=cross_stack_scope,
+        options = aws_cdk.aws_events.OnEventOptions(
             description=description,
             event_pattern=event_pattern,
             rule_name=rule_name,
+            target=target,
         )
 
-        return typing.cast(_aws_cdk_aws_events_ceddda9d.Rule, jsii.invoke(self, "onStateChange", [id, job_state, options]))
+        return typing.cast(aws_cdk.aws_events.Rule, jsii.invoke(self, "onStateChange", [id, job_state, options]))
 
     @jsii.member(jsii_name="onSuccess")
     def on_success(
         self,
         id: builtins.str,
         *,
-        target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-        cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
         description: typing.Optional[builtins.str] = None,
-        event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
+        event_pattern: typing.Optional[aws_cdk.aws_events.EventPattern] = None,
         rule_name: typing.Optional[builtins.str] = None,
-    ) -> _aws_cdk_aws_events_ceddda9d.Rule:
+        target: typing.Optional[aws_cdk.aws_events.IRuleTarget] = None,
+    ) -> aws_cdk.aws_events.Rule:
         '''(experimental) Create a CloudWatch Event Rule matching JobState.SUCCEEDED.
 
         :param id: construct id.
-        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
-        :param cross_stack_scope: The scope to use if the source of the rule and its target are in different Stacks (but in the same account & region). This helps dealing with cycles that often arise in these situations. Default: - none (the main scope will be used, even for cross-stack Events)
         :param description: A description of the rule's purpose. Default: - No description
         :param event_pattern: Additional restrictions for the event to route to the specified target. The method that generates the rule probably imposes some type of event filtering. The filtering implied by what you pass here is added on top of that filtering. Default: - No additional filtering based on an event pattern.
         :param rule_name: A name for the rule. Default: AWS CloudFormation generates a unique physical ID.
+        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b8390e01882a245ed021fa1f65648219d84b9932b1c593026055b61fe2c56a85)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        options = _aws_cdk_aws_events_ceddda9d.OnEventOptions(
-            target=target,
-            cross_stack_scope=cross_stack_scope,
+        options = aws_cdk.aws_events.OnEventOptions(
             description=description,
             event_pattern=event_pattern,
             rule_name=rule_name,
+            target=target,
         )
 
-        return typing.cast(_aws_cdk_aws_events_ceddda9d.Rule, jsii.invoke(self, "onSuccess", [id, options]))
+        return typing.cast(aws_cdk.aws_events.Rule, jsii.invoke(self, "onSuccess", [id, options]))
 
     @jsii.member(jsii_name="onTimeout")
     def on_timeout(
         self,
         id: builtins.str,
         *,
-        target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-        cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
         description: typing.Optional[builtins.str] = None,
-        event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
+        event_pattern: typing.Optional[aws_cdk.aws_events.EventPattern] = None,
         rule_name: typing.Optional[builtins.str] = None,
-    ) -> _aws_cdk_aws_events_ceddda9d.Rule:
+        target: typing.Optional[aws_cdk.aws_events.IRuleTarget] = None,
+    ) -> aws_cdk.aws_events.Rule:
         '''(experimental) Return a CloudWatch Event Rule matching TIMEOUT state.
 
         :param id: construct id.
-        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
-        :param cross_stack_scope: The scope to use if the source of the rule and its target are in different Stacks (but in the same account & region). This helps dealing with cycles that often arise in these situations. Default: - none (the main scope will be used, even for cross-stack Events)
         :param description: A description of the rule's purpose. Default: - No description
         :param event_pattern: Additional restrictions for the event to route to the specified target. The method that generates the rule probably imposes some type of event filtering. The filtering implied by what you pass here is added on top of that filtering. Default: - No additional filtering based on an event pattern.
         :param rule_name: A name for the rule. Default: AWS CloudFormation generates a unique physical ID.
+        :param target: The target to register for the event. Default: - No target is added to the rule. Use ``addTarget()`` to add a target.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b061eb382ce02e7e8798f77ad4abe593f170f59b9df192c9e6c5fb3de7901a33)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        options = _aws_cdk_aws_events_ceddda9d.OnEventOptions(
-            target=target,
-            cross_stack_scope=cross_stack_scope,
+        options = aws_cdk.aws_events.OnEventOptions(
             description=description,
             event_pattern=event_pattern,
             rule_name=rule_name,
+            target=target,
         )
 
-        return typing.cast(_aws_cdk_aws_events_ceddda9d.Rule, jsii.invoke(self, "onTimeout", [id, options]))
+        return typing.cast(aws_cdk.aws_events.Rule, jsii.invoke(self, "onTimeout", [id, options]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="grantPrincipal")
-    def grant_principal(self) -> _aws_cdk_aws_iam_ceddda9d.IPrincipal:
+    def grant_principal(self) -> aws_cdk.aws_iam.IPrincipal:
         '''(experimental) The principal this Glue Job is running as.
 
         :stability: experimental
         '''
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.IPrincipal, jsii.get(self, "grantPrincipal"))
+        return typing.cast(aws_cdk.aws_iam.IPrincipal, jsii.get(self, "grantPrincipal"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="jobArn")
     def job_arn(self) -> builtins.str:
         '''(experimental) The ARN of the job.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "jobArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="jobName")
     def job_name(self) -> builtins.str:
         '''(experimental) The name of the job.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "jobName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="role")
-    def role(self) -> _aws_cdk_aws_iam_ceddda9d.IRole:
+    def role(self) -> aws_cdk.aws_iam.IRole:
         '''(experimental) The IAM role Glue assumes to run this job.
 
         :stability: experimental
         '''
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.IRole, jsii.get(self, "role"))
+        return typing.cast(aws_cdk.aws_iam.IRole, jsii.get(self, "role"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="sparkUILoggingLocation")
     def spark_ui_logging_location(self) -> typing.Optional["SparkUILoggingLocation"]:
         '''(experimental) The Spark UI logs location if Spark UI monitoring and debugging is enabled.
 
         :see: https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-glue-arguments.html
         :stability: experimental
         '''
@@ -3596,17 +3366,17 @@
     name_mapping={"job_name": "jobName", "role": "role"},
 )
 class JobAttributes:
     def __init__(
         self,
         *,
         job_name: builtins.str,
-        role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
     ) -> None:
-        '''(experimental) Attributes for importing ``Job``.
+        '''(experimental) Attributes for importing {@link Job}.
 
         :param job_name: (experimental) The name of the job.
         :param role: (experimental) The IAM role assumed by Glue to run this job. Default: - undefined
 
         :stability: experimental
         :exampleMetadata: fixture=_generated
 
@@ -3622,19 +3392,15 @@
             job_attributes = glue_alpha.JobAttributes(
                 job_name="jobName",
             
                 # the properties below are optional
                 role=role
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2f1f5ae0406d4aaf443249ea9377b38a10b1814ed1f9c1fb9f0cbc5f489fd89e)
-            check_type(argname="argument job_name", value=job_name, expected_type=type_hints["job_name"])
-            check_type(argname="argument role", value=role, expected_type=type_hints["role"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "job_name": job_name,
         }
         if role is not None:
             self._values["role"] = role
 
     @builtins.property
     def job_name(self) -> builtins.str:
@@ -3643,23 +3409,23 @@
         :stability: experimental
         '''
         result = self._values.get("job_name")
         assert result is not None, "Required property 'job_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+    def role(self) -> typing.Optional[aws_cdk.aws_iam.IRole]:
         '''(experimental) The IAM role assumed by Glue to run this job.
 
         :default: - undefined
 
         :stability: experimental
         '''
         result = self._values.get("role")
-        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_iam.IRole], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -3675,43 +3441,40 @@
     name_mapping={"mode": "mode", "kms_key": "kmsKey"},
 )
 class JobBookmarksEncryption:
     def __init__(
         self,
         *,
         mode: "JobBookmarksEncryptionMode",
-        kms_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        kms_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
     ) -> None:
         '''(experimental) Job bookmarks encryption configuration.
 
         :param mode: (experimental) Encryption mode.
         :param kms_key: (experimental) The KMS key to be used to encrypt the data. Default: A key will be created if one is not provided.
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
             glue.SecurityConfiguration(self, "MySecurityConfiguration",
+                security_configuration_name="name",
                 cloud_watch_encryption=glue.CloudWatchEncryption(
                     mode=glue.CloudWatchEncryptionMode.KMS
                 ),
                 job_bookmarks_encryption=glue.JobBookmarksEncryption(
                     mode=glue.JobBookmarksEncryptionMode.CLIENT_SIDE_KMS
                 ),
                 s3_encryption=glue.S3Encryption(
                     mode=glue.S3EncryptionMode.KMS
                 )
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__61a555ea81acfe554401802d7d44d70d3e1a6f96890ffbc28283fadb7ea81f9e)
-            check_type(argname="argument mode", value=mode, expected_type=type_hints["mode"])
-            check_type(argname="argument kms_key", value=kms_key, expected_type=type_hints["kms_key"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "mode": mode,
         }
         if kms_key is not None:
             self._values["kms_key"] = kms_key
 
     @builtins.property
     def mode(self) -> "JobBookmarksEncryptionMode":
@@ -3720,23 +3483,23 @@
         :stability: experimental
         '''
         result = self._values.get("mode")
         assert result is not None, "Required property 'mode' is missing"
         return typing.cast("JobBookmarksEncryptionMode", result)
 
     @builtins.property
-    def kms_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def kms_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) The KMS key to be used to encrypt the data.
 
         :default: A key will be created if one is not provided.
 
         :stability: experimental
         '''
         result = self._values.get("kms_key")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -3753,14 +3516,15 @@
     :see: https://docs.aws.amazon.com/glue/latest/webapi/API_JobBookmarksEncryption.html#Glue-Type-JobBookmarksEncryption-JobBookmarksEncryptionMode
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
         glue.SecurityConfiguration(self, "MySecurityConfiguration",
+            security_configuration_name="name",
             cloud_watch_encryption=glue.CloudWatchEncryption(
                 mode=glue.CloudWatchEncryptionMode.KMS
             ),
             job_bookmarks_encryption=glue.JobBookmarksEncryption(
                 mode=glue.JobBookmarksEncryptionMode.CLIENT_SIDE_KMS
             ),
             s3_encryption=glue.S3Encryption(
@@ -3784,25 +3548,27 @@
     '''(experimental) The executable properties related to the Glue job's GlueVersion, JobType and code.
 
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
-        glue.Job(self, "PythonSparkStreamingJob",
-            executable=glue.JobExecutable.python_streaming(
-                glue_version=glue.GlueVersion.V4_0,
+        # bucket: s3.Bucket
+        
+        glue.Job(self, "PythonShellJob",
+            executable=glue.JobExecutable.python_shell(
+                glue_version=glue.GlueVersion.V1_0,
                 python_version=glue.PythonVersion.THREE,
-                script=glue.Code.from_asset(path.join(__dirname, "job-script/hello_world.py"))
+                script=glue.Code.from_bucket(bucket, "script.py")
             ),
-            description="an example Python Streaming job"
+            description="an example Python Shell job"
         )
     '''
 
-    @jsii.member(jsii_name="of")
+    @jsii.member(jsii_name="of") # type: ignore[misc]
     @builtins.classmethod
     def of(
         cls,
         *,
         glue_version: GlueVersion,
         language: "JobLanguage",
         script: Code,
@@ -3840,15 +3606,15 @@
             extra_jars_first=extra_jars_first,
             extra_python_files=extra_python_files,
             python_version=python_version,
         )
 
         return typing.cast("JobExecutable", jsii.sinvoke(cls, "of", [config]))
 
-    @jsii.member(jsii_name="pythonEtl")
+    @jsii.member(jsii_name="pythonEtl") # type: ignore[misc]
     @builtins.classmethod
     def python_etl(
         cls,
         *,
         glue_version: GlueVersion,
         python_version: "PythonVersion",
         script: Code,
@@ -3877,46 +3643,15 @@
             extra_jars=extra_jars,
             extra_jars_first=extra_jars_first,
             extra_python_files=extra_python_files,
         )
 
         return typing.cast("JobExecutable", jsii.sinvoke(cls, "pythonEtl", [props]))
 
-    @jsii.member(jsii_name="pythonRay")
-    @builtins.classmethod
-    def python_ray(
-        cls,
-        *,
-        glue_version: GlueVersion,
-        python_version: "PythonVersion",
-        script: Code,
-        extra_files: typing.Optional[typing.Sequence[Code]] = None,
-        extra_python_files: typing.Optional[typing.Sequence[Code]] = None,
-    ) -> "JobExecutable":
-        '''(experimental) Create Python executable props for Ray jobs.
-
-        :param glue_version: (experimental) Glue version.
-        :param python_version: (experimental) The Python version to use.
-        :param script: (experimental) The script that executes a job.
-        :param extra_files: (experimental) Additional files, such as configuration files that AWS Glue copies to the working directory of your script before executing it. Only individual files are supported, directories are not supported. Default: [] - no extra files are copied to the working directory
-        :param extra_python_files: (experimental) Additional Python files that AWS Glue adds to the Python path before executing your script. Only individual files are supported, directories are not supported. Default: - no extra python files and argument is not set
-
-        :stability: experimental
-        '''
-        props = PythonRayExecutableProps(
-            glue_version=glue_version,
-            python_version=python_version,
-            script=script,
-            extra_files=extra_files,
-            extra_python_files=extra_python_files,
-        )
-
-        return typing.cast("JobExecutable", jsii.sinvoke(cls, "pythonRay", [props]))
-
-    @jsii.member(jsii_name="pythonShell")
+    @jsii.member(jsii_name="pythonShell") # type: ignore[misc]
     @builtins.classmethod
     def python_shell(
         cls,
         *,
         glue_version: GlueVersion,
         python_version: "PythonVersion",
         script: Code,
@@ -3939,15 +3674,15 @@
             script=script,
             extra_files=extra_files,
             extra_python_files=extra_python_files,
         )
 
         return typing.cast("JobExecutable", jsii.sinvoke(cls, "pythonShell", [props]))
 
-    @jsii.member(jsii_name="pythonStreaming")
+    @jsii.member(jsii_name="pythonStreaming") # type: ignore[misc]
     @builtins.classmethod
     def python_streaming(
         cls,
         *,
         glue_version: GlueVersion,
         python_version: "PythonVersion",
         script: Code,
@@ -3976,15 +3711,15 @@
             extra_jars=extra_jars,
             extra_jars_first=extra_jars_first,
             extra_python_files=extra_python_files,
         )
 
         return typing.cast("JobExecutable", jsii.sinvoke(cls, "pythonStreaming", [props]))
 
-    @jsii.member(jsii_name="scalaEtl")
+    @jsii.member(jsii_name="scalaEtl") # type: ignore[misc]
     @builtins.classmethod
     def scala_etl(
         cls,
         *,
         class_name: builtins.str,
         glue_version: GlueVersion,
         script: Code,
@@ -4010,15 +3745,15 @@
             extra_files=extra_files,
             extra_jars=extra_jars,
             extra_jars_first=extra_jars_first,
         )
 
         return typing.cast("JobExecutable", jsii.sinvoke(cls, "scalaEtl", [props]))
 
-    @jsii.member(jsii_name="scalaStreaming")
+    @jsii.member(jsii_name="scalaStreaming") # type: ignore[misc]
     @builtins.classmethod
     def scala_streaming(
         cls,
         *,
         class_name: builtins.str,
         glue_version: GlueVersion,
         script: Code,
@@ -4125,27 +3860,15 @@
                 extra_files=[code],
                 extra_jars=[code],
                 extra_jars_first=False,
                 extra_python_files=[code],
                 python_version=glue_alpha.PythonVersion.TWO
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__629e6b8d2f364b0c0cfaa00ca6e06725f3d280ad7a2366cf5df8f63e472fea40)
-            check_type(argname="argument glue_version", value=glue_version, expected_type=type_hints["glue_version"])
-            check_type(argname="argument language", value=language, expected_type=type_hints["language"])
-            check_type(argname="argument script", value=script, expected_type=type_hints["script"])
-            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
-            check_type(argname="argument class_name", value=class_name, expected_type=type_hints["class_name"])
-            check_type(argname="argument extra_files", value=extra_files, expected_type=type_hints["extra_files"])
-            check_type(argname="argument extra_jars", value=extra_jars, expected_type=type_hints["extra_jars"])
-            check_type(argname="argument extra_jars_first", value=extra_jars_first, expected_type=type_hints["extra_jars_first"])
-            check_type(argname="argument extra_python_files", value=extra_python_files, expected_type=type_hints["extra_python_files"])
-            check_type(argname="argument python_version", value=python_version, expected_type=type_hints["python_version"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "glue_version": glue_version,
             "language": language,
             "script": script,
             "type": type,
         }
         if class_name is not None:
             self._values["class_name"] = class_name
@@ -4332,91 +4055,73 @@
 )
 class JobProps:
     def __init__(
         self,
         *,
         executable: JobExecutable,
         connections: typing.Optional[typing.Sequence[IConnection]] = None,
-        continuous_logging: typing.Optional[typing.Union[ContinuousLoggingProps, typing.Dict[builtins.str, typing.Any]]] = None,
+        continuous_logging: typing.Optional[ContinuousLoggingProps] = None,
         default_arguments: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         description: typing.Optional[builtins.str] = None,
         enable_profiling_metrics: typing.Optional[builtins.bool] = None,
         job_name: typing.Optional[builtins.str] = None,
         max_capacity: typing.Optional[jsii.Number] = None,
         max_concurrent_runs: typing.Optional[jsii.Number] = None,
         max_retries: typing.Optional[jsii.Number] = None,
-        notify_delay_after: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-        role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        notify_delay_after: typing.Optional[aws_cdk.Duration] = None,
+        role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
         security_configuration: typing.Optional[ISecurityConfiguration] = None,
-        spark_ui: typing.Optional[typing.Union["SparkUIProps", typing.Dict[builtins.str, typing.Any]]] = None,
+        spark_ui: typing.Optional["SparkUIProps"] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-        timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        timeout: typing.Optional[aws_cdk.Duration] = None,
         worker_count: typing.Optional[jsii.Number] = None,
         worker_type: typing.Optional["WorkerType"] = None,
     ) -> None:
-        '''(experimental) Construction properties for ``Job``.
+        '''(experimental) Construction properties for {@link Job}.
 
         :param executable: (experimental) The job's executable properties.
-        :param connections: (experimental) The ``Connection``s used for this job. Connections are used to connect to other AWS Service or resources within a VPC. Default: [] - no connections are added to the job
+        :param connections: (experimental) The {@link Connection}s used for this job. Connections are used to connect to other AWS Service or resources within a VPC. Default: [] - no connections are added to the job
         :param continuous_logging: (experimental) Enables continuous logging with the specified props. Default: - continuous logging is disabled.
         :param default_arguments: (experimental) The default arguments for this job, specified as name-value pairs. Default: - no arguments
         :param description: (experimental) The description of the job. Default: - no value
         :param enable_profiling_metrics: (experimental) Enables the collection of metrics for job profiling. Default: - no profiling metrics emitted.
         :param job_name: (experimental) The name of the job. Default: - a name is automatically generated
         :param max_capacity: (experimental) The number of AWS Glue data processing units (DPUs) that can be allocated when this job runs. Cannot be used for Glue version 2.0 and later - workerType and workerCount should be used instead. Default: - 10 when job type is Apache Spark ETL or streaming, 0.0625 when job type is Python shell
         :param max_concurrent_runs: (experimental) The maximum number of concurrent runs allowed for the job. An error is returned when this threshold is reached. The maximum value you can specify is controlled by a service limit. Default: 1
         :param max_retries: (experimental) The maximum number of times to retry this job after a job run fails. Default: 0
         :param notify_delay_after: (experimental) The number of minutes to wait after a job run starts, before sending a job run delay notification. Default: - no delay notifications
         :param role: (experimental) The IAM role assumed by Glue to run this job. If providing a custom role, it needs to trust the Glue service principal (glue.amazonaws.com) and be granted sufficient permissions. Default: - a role is automatically generated
-        :param security_configuration: (experimental) The ``SecurityConfiguration`` to use for this job. Default: - no security configuration.
+        :param security_configuration: (experimental) The {@link SecurityConfiguration} to use for this job. Default: - no security configuration.
         :param spark_ui: (experimental) Enables the Spark UI debugging and monitoring with the specified props. Default: - Spark UI debugging and monitoring is disabled.
         :param tags: (experimental) The tags to add to the resources on which the job runs. Default: {} - no tags
         :param timeout: (experimental) The maximum time that a job run can consume resources before it is terminated and enters TIMEOUT status. Default: cdk.Duration.hours(48)
-        :param worker_count: (experimental) The number of workers of a defined ``WorkerType`` that are allocated when a job runs. Default: - differs based on specific Glue version/worker type
+        :param worker_count: (experimental) The number of workers of a defined {@link WorkerType} that are allocated when a job runs. Default: - differs based on specific Glue version/worker type
         :param worker_type: (experimental) The type of predefined worker that is allocated when a job runs. Default: - differs based on specific Glue version
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
-            glue.Job(self, "PythonSparkStreamingJob",
-                executable=glue.JobExecutable.python_streaming(
-                    glue_version=glue.GlueVersion.V4_0,
+            # bucket: s3.Bucket
+            
+            glue.Job(self, "PythonShellJob",
+                executable=glue.JobExecutable.python_shell(
+                    glue_version=glue.GlueVersion.V1_0,
                     python_version=glue.PythonVersion.THREE,
-                    script=glue.Code.from_asset(path.join(__dirname, "job-script/hello_world.py"))
+                    script=glue.Code.from_bucket(bucket, "script.py")
                 ),
-                description="an example Python Streaming job"
+                description="an example Python Shell job"
             )
         '''
         if isinstance(continuous_logging, dict):
             continuous_logging = ContinuousLoggingProps(**continuous_logging)
         if isinstance(spark_ui, dict):
             spark_ui = SparkUIProps(**spark_ui)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9f47dc7b3a9514a79f7f82e52c4441b82161dce2eb5b67f22211660776beaa70)
-            check_type(argname="argument executable", value=executable, expected_type=type_hints["executable"])
-            check_type(argname="argument connections", value=connections, expected_type=type_hints["connections"])
-            check_type(argname="argument continuous_logging", value=continuous_logging, expected_type=type_hints["continuous_logging"])
-            check_type(argname="argument default_arguments", value=default_arguments, expected_type=type_hints["default_arguments"])
-            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
-            check_type(argname="argument enable_profiling_metrics", value=enable_profiling_metrics, expected_type=type_hints["enable_profiling_metrics"])
-            check_type(argname="argument job_name", value=job_name, expected_type=type_hints["job_name"])
-            check_type(argname="argument max_capacity", value=max_capacity, expected_type=type_hints["max_capacity"])
-            check_type(argname="argument max_concurrent_runs", value=max_concurrent_runs, expected_type=type_hints["max_concurrent_runs"])
-            check_type(argname="argument max_retries", value=max_retries, expected_type=type_hints["max_retries"])
-            check_type(argname="argument notify_delay_after", value=notify_delay_after, expected_type=type_hints["notify_delay_after"])
-            check_type(argname="argument role", value=role, expected_type=type_hints["role"])
-            check_type(argname="argument security_configuration", value=security_configuration, expected_type=type_hints["security_configuration"])
-            check_type(argname="argument spark_ui", value=spark_ui, expected_type=type_hints["spark_ui"])
-            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
-            check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
-            check_type(argname="argument worker_count", value=worker_count, expected_type=type_hints["worker_count"])
-            check_type(argname="argument worker_type", value=worker_type, expected_type=type_hints["worker_type"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "executable": executable,
         }
         if connections is not None:
             self._values["connections"] = connections
         if continuous_logging is not None:
             self._values["continuous_logging"] = continuous_logging
         if default_arguments is not None:
@@ -4458,15 +4163,15 @@
         '''
         result = self._values.get("executable")
         assert result is not None, "Required property 'executable' is missing"
         return typing.cast(JobExecutable, result)
 
     @builtins.property
     def connections(self) -> typing.Optional[typing.List[IConnection]]:
-        '''(experimental) The ``Connection``s used for this job.
+        '''(experimental) The {@link Connection}s used for this job.
 
         Connections are used to connect to other AWS Service or resources within a VPC.
 
         :default: [] - no connections are added to the job
 
         :stability: experimental
         '''
@@ -4567,41 +4272,41 @@
 
         :stability: experimental
         '''
         result = self._values.get("max_retries")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
-    def notify_delay_after(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+    def notify_delay_after(self) -> typing.Optional[aws_cdk.Duration]:
         '''(experimental) The number of minutes to wait after a job run starts, before sending a job run delay notification.
 
         :default: - no delay notifications
 
         :stability: experimental
         '''
         result = self._values.get("notify_delay_after")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
+        return typing.cast(typing.Optional[aws_cdk.Duration], result)
 
     @builtins.property
-    def role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+    def role(self) -> typing.Optional[aws_cdk.aws_iam.IRole]:
         '''(experimental) The IAM role assumed by Glue to run this job.
 
         If providing a custom role, it needs to trust the Glue service principal (glue.amazonaws.com) and be granted sufficient permissions.
 
         :default: - a role is automatically generated
 
         :see: https://docs.aws.amazon.com/glue/latest/dg/getting-started-access.html
         :stability: experimental
         '''
         result = self._values.get("role")
-        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_iam.IRole], result)
 
     @builtins.property
     def security_configuration(self) -> typing.Optional[ISecurityConfiguration]:
-        '''(experimental) The ``SecurityConfiguration`` to use for this job.
+        '''(experimental) The {@link SecurityConfiguration} to use for this job.
 
         :default: - no security configuration.
 
         :stability: experimental
         '''
         result = self._values.get("security_configuration")
         return typing.cast(typing.Optional[ISecurityConfiguration], result)
@@ -4626,27 +4331,27 @@
 
         :stability: experimental
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
-    def timeout(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+    def timeout(self) -> typing.Optional[aws_cdk.Duration]:
         '''(experimental) The maximum time that a job run can consume resources before it is terminated and enters TIMEOUT status.
 
         :default: cdk.Duration.hours(48)
 
         :stability: experimental
         '''
         result = self._values.get("timeout")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
+        return typing.cast(typing.Optional[aws_cdk.Duration], result)
 
     @builtins.property
     def worker_count(self) -> typing.Optional[jsii.Number]:
-        '''(experimental) The number of workers of a defined ``WorkerType`` that are allocated when a job runs.
+        '''(experimental) The number of workers of a defined {@link WorkerType} that are allocated when a job runs.
 
         :default: - differs based on specific Glue version/worker type
 
         :stability: experimental
         '''
         result = self._values.get("worker_count")
         return typing.cast(typing.Optional[jsii.Number], result)
@@ -4733,65 +4438,53 @@
         # The code below shows an example of how to instantiate this type.
         # The values are placeholders you should change.
         import aws_cdk.aws_glue_alpha as glue_alpha
         
         job_type = glue_alpha.JobType.ETL
     '''
 
-    @jsii.member(jsii_name="of")
+    @jsii.member(jsii_name="of") # type: ignore[misc]
     @builtins.classmethod
     def of(cls, name: builtins.str) -> "JobType":
         '''(experimental) Custom type name.
 
         :param name: type name.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0683afe40f10e5c8c02ac80ffb25aca1e5830884e6b5e539accb9e36df90257d)
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         return typing.cast("JobType", jsii.sinvoke(cls, "of", [name]))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="ETL")
     def ETL(cls) -> "JobType":
-        '''(experimental) Command for running a Glue Spark job.
+        '''(experimental) Command for running a Glue ETL job.
 
         :stability: experimental
         '''
         return typing.cast("JobType", jsii.sget(cls, "ETL"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="PYTHON_SHELL")
     def PYTHON_SHELL(cls) -> "JobType":
         '''(experimental) Command for running a Glue python shell job.
 
         :stability: experimental
         '''
         return typing.cast("JobType", jsii.sget(cls, "PYTHON_SHELL"))
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="RAY")
-    def RAY(cls) -> "JobType":
-        '''(experimental) Command for running a Glue Ray job.
-
-        :stability: experimental
-        '''
-        return typing.cast("JobType", jsii.sget(cls, "RAY"))
-
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="STREAMING")
     def STREAMING(cls) -> "JobType":
-        '''(experimental) Command for running a Glue Spark streaming job.
+        '''(experimental) Command for running a Glue streaming job.
 
         :stability: experimental
         '''
         return typing.cast("JobType", jsii.sget(cls, "STREAMING"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         '''(experimental) The name of this JobType, as expected by Job resource.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "name"))
@@ -4837,60 +4530,57 @@
 
     def __init__(self, class_name: builtins.str) -> None:
         '''
         :param class_name: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8952681a040fc7931f48438a2e01cd3c2bed40202b6f32cd606344a5ea10e810)
-            check_type(argname="argument class_name", value=class_name, expected_type=type_hints["class_name"])
         jsii.create(self.__class__, self, [class_name])
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="AVRO")
     def AVRO(cls) -> InputFormat:
         '''(experimental) OutputFormat for Avro files.
 
-        :see: https://svn.apache.org/repos/infra/websites/production/hive/content/javadocs/r3.1.3/api/org/apache/hadoop/hive/ql/io/avro/AvroContainerOutputFormat.html
+        :see: https://hive.apache.org/javadocs/r1.2.2/api/org/apache/hadoop/hive/ql/io/avro/AvroContainerOutputFormat.html
         :stability: experimental
         '''
         return typing.cast(InputFormat, jsii.sget(cls, "AVRO"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="HIVE_IGNORE_KEY_TEXT")
     def HIVE_IGNORE_KEY_TEXT(cls) -> "OutputFormat":
         '''(experimental) Writes text data with a null key (value only).
 
-        :see: https://svn.apache.org/repos/infra/websites/production/hive/content/javadocs/r3.1.3/api/org/apache/hadoop/hive/ql/io/HiveIgnoreKeyTextOutputFormat.html
+        :see: https://hive.apache.org/javadocs/r2.2.0/api/org/apache/hadoop/hive/ql/io/HiveIgnoreKeyTextOutputFormat.html
         :stability: experimental
         '''
         return typing.cast("OutputFormat", jsii.sget(cls, "HIVE_IGNORE_KEY_TEXT"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="ORC")
     def ORC(cls) -> InputFormat:
         '''(experimental) OutputFormat for Orc files.
 
-        :see: https://svn.apache.org/repos/infra/websites/production/hive/content/javadocs/r3.1.3/api/org/apache/hadoop/hive/ql/io/orc/OrcOutputFormat.html
+        :see: https://hive.apache.org/javadocs/r1.2.2/api/org/apache/hadoop/hive/ql/io/orc/OrcOutputFormat.html
         :stability: experimental
         '''
         return typing.cast(InputFormat, jsii.sget(cls, "ORC"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="PARQUET")
     def PARQUET(cls) -> "OutputFormat":
         '''(experimental) OutputFormat for Parquet files.
 
-        :see: https://svn.apache.org/repos/infra/websites/production/hive/content/javadocs/r3.1.3/api/org/apache/hadoop/hive/ql/io/parquet/MapredParquetOutputFormat.html
+        :see: https://hive.apache.org/javadocs/r1.2.2/api/org/apache/hadoop/hive/ql/io/parquet/MapredParquetOutputFormat.html
         :stability: experimental
         '''
         return typing.cast("OutputFormat", jsii.sget(cls, "PARQUET"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="className")
     def class_name(self) -> builtins.str:
         '''
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "className"))
 
@@ -4920,19 +4610,15 @@
             # my_table: glue.Table
             
             my_table.add_partition_index(
                 index_name="my-index",
                 key_names=["year"]
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__854153aaeace5af7af75594677e850d114f911156b5cd93d50a01feeff4a76a8)
-            check_type(argname="argument key_names", value=key_names, expected_type=type_hints["key_names"])
-            check_type(argname="argument index_name", value=index_name, expected_type=type_hints["index_name"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "key_names": key_names,
         }
         if index_name is not None:
             self._values["index_name"] = index_name
 
     @builtins.property
     def key_names(self) -> typing.List[builtins.str]:
@@ -4967,147 +4653,14 @@
     def __repr__(self) -> str:
         return "PartitionIndex(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="@aws-cdk/aws-glue-alpha.PythonRayExecutableProps",
-    jsii_struct_bases=[],
-    name_mapping={
-        "glue_version": "glueVersion",
-        "python_version": "pythonVersion",
-        "script": "script",
-        "extra_files": "extraFiles",
-        "extra_python_files": "extraPythonFiles",
-    },
-)
-class PythonRayExecutableProps:
-    def __init__(
-        self,
-        *,
-        glue_version: GlueVersion,
-        python_version: "PythonVersion",
-        script: Code,
-        extra_files: typing.Optional[typing.Sequence[Code]] = None,
-        extra_python_files: typing.Optional[typing.Sequence[Code]] = None,
-    ) -> None:
-        '''(experimental) Props for creating a Python Ray job executable.
-
-        :param glue_version: (experimental) Glue version.
-        :param python_version: (experimental) The Python version to use.
-        :param script: (experimental) The script that executes a job.
-        :param extra_files: (experimental) Additional files, such as configuration files that AWS Glue copies to the working directory of your script before executing it. Only individual files are supported, directories are not supported. Default: [] - no extra files are copied to the working directory
-        :param extra_python_files: (experimental) Additional Python files that AWS Glue adds to the Python path before executing your script. Only individual files are supported, directories are not supported. Default: - no extra python files and argument is not set
-
-        :stability: experimental
-        :exampleMetadata: infused
-
-        Example::
-
-            glue.Job(self, "RayJob",
-                executable=glue.JobExecutable.python_ray(
-                    glue_version=glue.GlueVersion.V4_0,
-                    python_version=glue.PythonVersion.THREE_NINE,
-                    script=glue.Code.from_asset(path.join(__dirname, "job-script/hello_world.py"))
-                ),
-                worker_type=glue.WorkerType.Z_2X,
-                worker_count=2,
-                description="an example Ray job"
-            )
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__96728d115db88df2280e8997d67958a9b8d05214b04966c306fbf00f84a6324f)
-            check_type(argname="argument glue_version", value=glue_version, expected_type=type_hints["glue_version"])
-            check_type(argname="argument python_version", value=python_version, expected_type=type_hints["python_version"])
-            check_type(argname="argument script", value=script, expected_type=type_hints["script"])
-            check_type(argname="argument extra_files", value=extra_files, expected_type=type_hints["extra_files"])
-            check_type(argname="argument extra_python_files", value=extra_python_files, expected_type=type_hints["extra_python_files"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
-            "glue_version": glue_version,
-            "python_version": python_version,
-            "script": script,
-        }
-        if extra_files is not None:
-            self._values["extra_files"] = extra_files
-        if extra_python_files is not None:
-            self._values["extra_python_files"] = extra_python_files
-
-    @builtins.property
-    def glue_version(self) -> GlueVersion:
-        '''(experimental) Glue version.
-
-        :see: https://docs.aws.amazon.com/glue/latest/dg/release-notes.html
-        :stability: experimental
-        '''
-        result = self._values.get("glue_version")
-        assert result is not None, "Required property 'glue_version' is missing"
-        return typing.cast(GlueVersion, result)
-
-    @builtins.property
-    def python_version(self) -> "PythonVersion":
-        '''(experimental) The Python version to use.
-
-        :stability: experimental
-        '''
-        result = self._values.get("python_version")
-        assert result is not None, "Required property 'python_version' is missing"
-        return typing.cast("PythonVersion", result)
-
-    @builtins.property
-    def script(self) -> Code:
-        '''(experimental) The script that executes a job.
-
-        :stability: experimental
-        '''
-        result = self._values.get("script")
-        assert result is not None, "Required property 'script' is missing"
-        return typing.cast(Code, result)
-
-    @builtins.property
-    def extra_files(self) -> typing.Optional[typing.List[Code]]:
-        '''(experimental) Additional files, such as configuration files that AWS Glue copies to the working directory of your script before executing it.
-
-        Only individual files are supported, directories are not supported.
-
-        :default: [] - no extra files are copied to the working directory
-
-        :see: ``--extra-files`` in https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-glue-arguments.html
-        :stability: experimental
-        '''
-        result = self._values.get("extra_files")
-        return typing.cast(typing.Optional[typing.List[Code]], result)
-
-    @builtins.property
-    def extra_python_files(self) -> typing.Optional[typing.List[Code]]:
-        '''(experimental) Additional Python files that AWS Glue adds to the Python path before executing your script.
-
-        Only individual files are supported, directories are not supported.
-
-        :default: - no extra python files and argument is not set
-
-        :see: ``--extra-py-files`` in https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-glue-arguments.html
-        :stability: experimental
-        '''
-        result = self._values.get("extra_python_files")
-        return typing.cast(typing.Optional[typing.List[Code]], result)
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "PythonRayExecutableProps(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
-
-@jsii.data_type(
     jsii_type="@aws-cdk/aws-glue-alpha.PythonShellExecutableProps",
     jsii_struct_bases=[],
     name_mapping={
         "glue_version": "glueVersion",
         "python_version": "pythonVersion",
         "script": "script",
         "extra_files": "extraFiles",
@@ -5144,22 +4697,15 @@
                     glue_version=glue.GlueVersion.V1_0,
                     python_version=glue.PythonVersion.THREE,
                     script=glue.Code.from_bucket(bucket, "script.py")
                 ),
                 description="an example Python Shell job"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__787eb0d11407cb3ae6ba15f28cff4370dd45126f9ce4e2ab093edba7a3b628e8)
-            check_type(argname="argument glue_version", value=glue_version, expected_type=type_hints["glue_version"])
-            check_type(argname="argument python_version", value=python_version, expected_type=type_hints["python_version"])
-            check_type(argname="argument script", value=script, expected_type=type_hints["script"])
-            check_type(argname="argument extra_files", value=extra_files, expected_type=type_hints["extra_files"])
-            check_type(argname="argument extra_python_files", value=extra_python_files, expected_type=type_hints["extra_python_files"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "glue_version": glue_version,
             "python_version": python_version,
             "script": script,
         }
         if extra_files is not None:
             self._values["extra_files"] = extra_files
         if extra_python_files is not None:
@@ -5274,31 +4820,22 @@
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
             glue.Job(self, "PythonSparkStreamingJob",
                 executable=glue.JobExecutable.python_streaming(
-                    glue_version=glue.GlueVersion.V4_0,
+                    glue_version=glue.GlueVersion.V2_0,
                     python_version=glue.PythonVersion.THREE,
                     script=glue.Code.from_asset(path.join(__dirname, "job-script/hello_world.py"))
                 ),
                 description="an example Python Streaming job"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2e0bf4f1c4314f36fa21cf1fde861d972bb36e11678ce6f78e9dab93055f9ed4)
-            check_type(argname="argument glue_version", value=glue_version, expected_type=type_hints["glue_version"])
-            check_type(argname="argument python_version", value=python_version, expected_type=type_hints["python_version"])
-            check_type(argname="argument script", value=script, expected_type=type_hints["script"])
-            check_type(argname="argument extra_files", value=extra_files, expected_type=type_hints["extra_files"])
-            check_type(argname="argument extra_jars", value=extra_jars, expected_type=type_hints["extra_jars"])
-            check_type(argname="argument extra_jars_first", value=extra_jars_first, expected_type=type_hints["extra_jars_first"])
-            check_type(argname="argument extra_python_files", value=extra_python_files, expected_type=type_hints["extra_python_files"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "glue_version": glue_version,
             "python_version": python_version,
             "script": script,
         }
         if extra_files is not None:
             self._values["extra_files"] = extra_files
         if extra_jars is not None:
@@ -5410,15 +4947,15 @@
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
         glue.Job(self, "PythonSparkStreamingJob",
             executable=glue.JobExecutable.python_streaming(
-                glue_version=glue.GlueVersion.V4_0,
+                glue_version=glue.GlueVersion.V2_0,
                 python_version=glue.PythonVersion.THREE,
                 script=glue.Code.from_asset(path.join(__dirname, "job-script/hello_world.py"))
             ),
             description="an example Python Streaming job"
         )
     '''
 
@@ -5428,19 +4965,14 @@
     :stability: experimental
     '''
     THREE = "THREE"
     '''(experimental) Python 3 (the exact version depends on GlueVersion and JobCommand used).
 
     :stability: experimental
     '''
-    THREE_NINE = "THREE_NINE"
-    '''(experimental) Python 3.9 (the exact version depends on GlueVersion and JobCommand used).
-
-    :stability: experimental
-    '''
 
 
 class S3Code(Code, metaclass=jsii.JSIIMeta, jsii_type="@aws-cdk/aws-glue-alpha.S3Code"):
     '''(experimental) Glue job Code from an S3 bucket.
 
     :stability: experimental
     :exampleMetadata: fixture=_generated
@@ -5453,90 +4985,75 @@
         from aws_cdk import aws_s3 as s3
         
         # bucket: s3.Bucket
         
         s3_code = glue_alpha.S3Code(bucket, "key")
     '''
 
-    def __init__(
-        self,
-        bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
-        key: builtins.str,
-    ) -> None:
+    def __init__(self, bucket: aws_cdk.aws_s3.IBucket, key: builtins.str) -> None:
         '''
         :param bucket: -
         :param key: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f7854e17fe796bdc5dc10fe3c8febb691186728550ca107493a43fc6979cafee)
-            check_type(argname="argument bucket", value=bucket, expected_type=type_hints["bucket"])
-            check_type(argname="argument key", value=key, expected_type=type_hints["key"])
         jsii.create(self.__class__, self, [bucket, key])
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
-        _scope: _constructs_77d1e7e8.Construct,
-        grantable: _aws_cdk_aws_iam_ceddda9d.IGrantable,
+        _scope: constructs.Construct,
+        grantable: aws_cdk.aws_iam.IGrantable,
     ) -> CodeConfig:
         '''(experimental) Called when the Job is initialized to allow this object to bind.
 
         :param _scope: -
         :param grantable: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__18fa6b6bc6e19007515f753b3e849efd4b7a16720ea785b0e155f20075d71602)
-            check_type(argname="argument _scope", value=_scope, expected_type=type_hints["_scope"])
-            check_type(argname="argument grantable", value=grantable, expected_type=type_hints["grantable"])
         return typing.cast(CodeConfig, jsii.invoke(self, "bind", [_scope, grantable]))
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-glue-alpha.S3Encryption",
     jsii_struct_bases=[],
     name_mapping={"mode": "mode", "kms_key": "kmsKey"},
 )
 class S3Encryption:
     def __init__(
         self,
         *,
         mode: "S3EncryptionMode",
-        kms_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        kms_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
     ) -> None:
         '''(experimental) S3 encryption configuration.
 
         :param mode: (experimental) Encryption mode.
         :param kms_key: (experimental) The KMS key to be used to encrypt the data. Default: no kms key if mode = S3_MANAGED. A key will be created if one is not provided and mode = KMS.
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
             glue.SecurityConfiguration(self, "MySecurityConfiguration",
+                security_configuration_name="name",
                 cloud_watch_encryption=glue.CloudWatchEncryption(
                     mode=glue.CloudWatchEncryptionMode.KMS
                 ),
                 job_bookmarks_encryption=glue.JobBookmarksEncryption(
                     mode=glue.JobBookmarksEncryptionMode.CLIENT_SIDE_KMS
                 ),
                 s3_encryption=glue.S3Encryption(
                     mode=glue.S3EncryptionMode.KMS
                 )
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d972222b3b5c087e70a7ab859853e97f1579eeee2ede763d551c41d4076f740e)
-            check_type(argname="argument mode", value=mode, expected_type=type_hints["mode"])
-            check_type(argname="argument kms_key", value=kms_key, expected_type=type_hints["kms_key"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "mode": mode,
         }
         if kms_key is not None:
             self._values["kms_key"] = kms_key
 
     @builtins.property
     def mode(self) -> "S3EncryptionMode":
@@ -5545,23 +5062,23 @@
         :stability: experimental
         '''
         result = self._values.get("mode")
         assert result is not None, "Required property 'mode' is missing"
         return typing.cast("S3EncryptionMode", result)
 
     @builtins.property
-    def kms_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def kms_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) The KMS key to be used to encrypt the data.
 
         :default: no kms key if mode = S3_MANAGED. A key will be created if one is not provided and mode = KMS.
 
         :stability: experimental
         '''
         result = self._values.get("kms_key")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -5578,14 +5095,15 @@
     :see: https://docs.aws.amazon.com/glue/latest/webapi/API_S3Encryption.html#Glue-Type-S3Encryption-S3EncryptionMode
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
         glue.SecurityConfiguration(self, "MySecurityConfiguration",
+            security_configuration_name="name",
             cloud_watch_encryption=glue.CloudWatchEncryption(
                 mode=glue.CloudWatchEncryptionMode.KMS
             ),
             job_bookmarks_encryption=glue.JobBookmarksEncryption(
                 mode=glue.JobBookmarksEncryptionMode.CLIENT_SIDE_KMS
             ),
             s3_encryption=glue.S3Encryption(
@@ -5645,32 +5163,23 @@
 
         Example::
 
             # bucket: s3.Bucket
             
             glue.Job(self, "ScalaSparkEtlJob",
                 executable=glue.JobExecutable.scala_etl(
-                    glue_version=glue.GlueVersion.V4_0,
+                    glue_version=glue.GlueVersion.V2_0,
                     script=glue.Code.from_bucket(bucket, "src/com/example/HelloWorld.scala"),
                     class_name="com.example.HelloWorld",
                     extra_jars=[glue.Code.from_bucket(bucket, "jars/HelloWorld.jar")]
                 ),
-                worker_type=glue.WorkerType.G_8X,
                 description="an example Scala ETL job"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a8895a1f83a364cc50cc706b326361b090931a87ba5ad2c1f9a0747bf6c0f7e7)
-            check_type(argname="argument class_name", value=class_name, expected_type=type_hints["class_name"])
-            check_type(argname="argument glue_version", value=glue_version, expected_type=type_hints["glue_version"])
-            check_type(argname="argument script", value=script, expected_type=type_hints["script"])
-            check_type(argname="argument extra_files", value=extra_files, expected_type=type_hints["extra_files"])
-            check_type(argname="argument extra_jars", value=extra_jars, expected_type=type_hints["extra_jars"])
-            check_type(argname="argument extra_jars_first", value=extra_jars_first, expected_type=type_hints["extra_jars_first"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "class_name": class_name,
             "glue_version": glue_version,
             "script": script,
         }
         if extra_files is not None:
             self._values["extra_files"] = extra_files
         if extra_jars is not None:
@@ -5768,14 +5277,15 @@
 
     Example::
 
         # my_database: glue.Database
         
         glue.Table(self, "MyTable",
             database=my_database,
+            table_name="my_table",
             columns=[glue.Column(
                 name="col1",
                 type=glue.Schema.STRING
             )],
             partition_keys=[glue.Column(
                 name="year",
                 type=glue.Schema.SMALL_INT
@@ -5789,15 +5299,15 @@
 
     def __init__(self) -> None:
         '''
         :stability: experimental
         '''
         jsii.create(self.__class__, self, [])
 
-    @jsii.member(jsii_name="array")
+    @jsii.member(jsii_name="array") # type: ignore[misc]
     @builtins.classmethod
     def array(
         cls,
         *,
         input_string: builtins.str,
         is_primitive: builtins.bool,
     ) -> "Type":
@@ -5808,29 +5318,26 @@
 
         :stability: experimental
         '''
         item_type = Type(input_string=input_string, is_primitive=is_primitive)
 
         return typing.cast("Type", jsii.sinvoke(cls, "array", [item_type]))
 
-    @jsii.member(jsii_name="char")
+    @jsii.member(jsii_name="char") # type: ignore[misc]
     @builtins.classmethod
     def char(cls, length: jsii.Number) -> "Type":
         '''(experimental) Fixed length character data, with a specified length between 1 and 255.
 
         :param length: length between 1 and 255.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d4b92f46741e45dc5d5e256fe3738d53a8878b40fc430d149eec6fdbfe167229)
-            check_type(argname="argument length", value=length, expected_type=type_hints["length"])
         return typing.cast("Type", jsii.sinvoke(cls, "char", [length]))
 
-    @jsii.member(jsii_name="decimal")
+    @jsii.member(jsii_name="decimal") # type: ignore[misc]
     @builtins.classmethod
     def decimal(
         cls,
         precision: jsii.Number,
         scale: typing.Optional[jsii.Number] = None,
     ) -> "Type":
         '''(experimental) Creates a decimal type.
@@ -5838,174 +5345,158 @@
         TODO: Bounds
 
         :param precision: the total number of digits.
         :param scale: the number of digits in fractional part, the default is 0.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fcdd8f07d6d5e4e87f54cd2104a8605a571a6abede0b42465e2352b51723b900)
-            check_type(argname="argument precision", value=precision, expected_type=type_hints["precision"])
-            check_type(argname="argument scale", value=scale, expected_type=type_hints["scale"])
         return typing.cast("Type", jsii.sinvoke(cls, "decimal", [precision, scale]))
 
-    @jsii.member(jsii_name="map")
+    @jsii.member(jsii_name="map") # type: ignore[misc]
     @builtins.classmethod
     def map(
         cls,
-        key_type: typing.Union["Type", typing.Dict[builtins.str, typing.Any]],
+        key_type: "Type",
         *,
         input_string: builtins.str,
         is_primitive: builtins.bool,
     ) -> "Type":
         '''(experimental) Creates a map of some primitive key type to some value type.
 
         :param key_type: type of key, must be a primitive.
         :param input_string: (experimental) Glue InputString for this type.
         :param is_primitive: (experimental) Indicates whether this type is a primitive data type.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fc04f65c508e37fca936dfd67a8b4a0f84a73b9ef9c446edcd34f17c738c8dae)
-            check_type(argname="argument key_type", value=key_type, expected_type=type_hints["key_type"])
         value_type = Type(input_string=input_string, is_primitive=is_primitive)
 
         return typing.cast("Type", jsii.sinvoke(cls, "map", [key_type, value_type]))
 
-    @jsii.member(jsii_name="struct")
+    @jsii.member(jsii_name="struct") # type: ignore[misc]
     @builtins.classmethod
-    def struct(
-        cls,
-        columns: typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]],
-    ) -> "Type":
+    def struct(cls, columns: typing.Sequence[Column]) -> "Type":
         '''(experimental) Creates a nested structure containing individually named and typed columns.
 
         :param columns: the columns of the structure.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__33f94b4c838eb0e3d03de4da6b4f3fe8e873ef98895fb940645c459801c4bb50)
-            check_type(argname="argument columns", value=columns, expected_type=type_hints["columns"])
         return typing.cast("Type", jsii.sinvoke(cls, "struct", [columns]))
 
-    @jsii.member(jsii_name="varchar")
+    @jsii.member(jsii_name="varchar") # type: ignore[misc]
     @builtins.classmethod
     def varchar(cls, length: jsii.Number) -> "Type":
         '''(experimental) Variable length character data, with a specified length between 1 and 65535.
 
         :param length: length between 1 and 65535.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0ba18137b7dd32100f635af375c8586adc2f9824c4ccd0a1b01168f5ba757da4)
-            check_type(argname="argument length", value=length, expected_type=type_hints["length"])
         return typing.cast("Type", jsii.sinvoke(cls, "varchar", [length]))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="BIG_INT")
     def BIG_INT(cls) -> "Type":
         '''(experimental) A 64-bit signed INTEGER in two’s complement format, with a minimum value of -2^63 and a maximum value of 2^63-1.
 
         :stability: experimental
         '''
         return typing.cast("Type", jsii.sget(cls, "BIG_INT"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="BINARY")
     def BINARY(cls) -> "Type":
         '''
         :stability: experimental
         '''
         return typing.cast("Type", jsii.sget(cls, "BINARY"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="BOOLEAN")
     def BOOLEAN(cls) -> "Type":
         '''
         :stability: experimental
         '''
         return typing.cast("Type", jsii.sget(cls, "BOOLEAN"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="DATE")
     def DATE(cls) -> "Type":
         '''(experimental) Date type.
 
         :stability: experimental
         '''
         return typing.cast("Type", jsii.sget(cls, "DATE"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="DOUBLE")
     def DOUBLE(cls) -> "Type":
         '''
         :stability: experimental
         '''
         return typing.cast("Type", jsii.sget(cls, "DOUBLE"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="FLOAT")
     def FLOAT(cls) -> "Type":
         '''
         :stability: experimental
         '''
         return typing.cast("Type", jsii.sget(cls, "FLOAT"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="INTEGER")
     def INTEGER(cls) -> "Type":
         '''(experimental) A 32-bit signed INTEGER in two’s complement format, with a minimum value of -2^31 and a maximum value of 2^31-1.
 
         :stability: experimental
         '''
         return typing.cast("Type", jsii.sget(cls, "INTEGER"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="SMALL_INT")
     def SMALL_INT(cls) -> "Type":
         '''(experimental) A 16-bit signed INTEGER in two’s complement format, with a minimum value of -2^15 and a maximum value of 2^15-1.
 
         :stability: experimental
         '''
         return typing.cast("Type", jsii.sget(cls, "SMALL_INT"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="STRING")
     def STRING(cls) -> "Type":
         '''(experimental) Arbitrary-length string type.
 
         :stability: experimental
         '''
         return typing.cast("Type", jsii.sget(cls, "STRING"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="TIMESTAMP")
     def TIMESTAMP(cls) -> "Type":
         '''(experimental) Timestamp type (date and time).
 
         :stability: experimental
         '''
         return typing.cast("Type", jsii.sget(cls, "TIMESTAMP"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="TINY_INT")
     def TINY_INT(cls) -> "Type":
         '''(experimental) A 8-bit signed INTEGER in two’s complement format, with a minimum value of -2^7 and a maximum value of 2^7-1.
 
         :stability: experimental
         '''
         return typing.cast("Type", jsii.sget(cls, "TINY_INT"))
 
 
 @jsii.implements(ISecurityConfiguration)
 class SecurityConfiguration(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-glue-alpha.SecurityConfiguration",
 ):
     '''(experimental) A security configuration is a set of security properties that can be used by AWS Glue to encrypt data at rest.
 
     The following scenarios show some of the ways that you can use a security configuration.
 
@@ -6016,156 +5507,145 @@
 
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
         glue.SecurityConfiguration(self, "MySecurityConfiguration",
+            security_configuration_name="name",
             cloud_watch_encryption=glue.CloudWatchEncryption(
                 mode=glue.CloudWatchEncryptionMode.KMS
             ),
             job_bookmarks_encryption=glue.JobBookmarksEncryption(
                 mode=glue.JobBookmarksEncryptionMode.CLIENT_SIDE_KMS
             ),
             s3_encryption=glue.S3Encryption(
                 mode=glue.S3EncryptionMode.KMS
             )
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
-        cloud_watch_encryption: typing.Optional[typing.Union[CloudWatchEncryption, typing.Dict[builtins.str, typing.Any]]] = None,
-        job_bookmarks_encryption: typing.Optional[typing.Union[JobBookmarksEncryption, typing.Dict[builtins.str, typing.Any]]] = None,
-        s3_encryption: typing.Optional[typing.Union[S3Encryption, typing.Dict[builtins.str, typing.Any]]] = None,
-        security_configuration_name: typing.Optional[builtins.str] = None,
+        security_configuration_name: builtins.str,
+        cloud_watch_encryption: typing.Optional[CloudWatchEncryption] = None,
+        job_bookmarks_encryption: typing.Optional[JobBookmarksEncryption] = None,
+        s3_encryption: typing.Optional[S3Encryption] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
+        :param security_configuration_name: (experimental) The name of the security configuration.
         :param cloud_watch_encryption: (experimental) The encryption configuration for Amazon CloudWatch Logs. Default: no cloudwatch logs encryption.
         :param job_bookmarks_encryption: (experimental) The encryption configuration for Glue Job Bookmarks. Default: no job bookmarks encryption.
         :param s3_encryption: (experimental) The encryption configuration for Amazon Simple Storage Service (Amazon S3) data. Default: no s3 encryption.
-        :param security_configuration_name: (experimental) The name of the security configuration. Default: - generated by CDK.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__cd628a6199f5b5fb7644771f78b6cc6d9230e3c38bba0463810d192bceb52e8d)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = SecurityConfigurationProps(
+            security_configuration_name=security_configuration_name,
             cloud_watch_encryption=cloud_watch_encryption,
             job_bookmarks_encryption=job_bookmarks_encryption,
             s3_encryption=s3_encryption,
-            security_configuration_name=security_configuration_name,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromSecurityConfigurationName")
+    @jsii.member(jsii_name="fromSecurityConfigurationName") # type: ignore[misc]
     @builtins.classmethod
     def from_security_configuration_name(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         security_configuration_name: builtins.str,
     ) -> ISecurityConfiguration:
         '''(experimental) Creates a Connection construct that represents an external security configuration.
 
         :param scope: The scope creating construct (usually ``this``).
         :param id: The construct's id.
         :param security_configuration_name: name of external security configuration.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4a85db96fd444625c46f4574190ecd86214bed327c2f826ee3294853f69a42b6)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument security_configuration_name", value=security_configuration_name, expected_type=type_hints["security_configuration_name"])
         return typing.cast(ISecurityConfiguration, jsii.sinvoke(cls, "fromSecurityConfigurationName", [scope, id, security_configuration_name]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="securityConfigurationName")
     def security_configuration_name(self) -> builtins.str:
         '''(experimental) The name of the security configuration.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "securityConfigurationName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="cloudWatchEncryptionKey")
-    def cloud_watch_encryption_key(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def cloud_watch_encryption_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) The KMS key used in CloudWatch encryption if it requires a kms key.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], jsii.get(self, "cloudWatchEncryptionKey"))
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], jsii.get(self, "cloudWatchEncryptionKey"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="jobBookmarksEncryptionKey")
-    def job_bookmarks_encryption_key(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def job_bookmarks_encryption_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) The KMS key used in job bookmarks encryption if it requires a kms key.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], jsii.get(self, "jobBookmarksEncryptionKey"))
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], jsii.get(self, "jobBookmarksEncryptionKey"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="s3EncryptionKey")
-    def s3_encryption_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def s3_encryption_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) The KMS key used in S3 encryption if it requires a kms key.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], jsii.get(self, "s3EncryptionKey"))
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], jsii.get(self, "s3EncryptionKey"))
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-glue-alpha.SecurityConfigurationProps",
     jsii_struct_bases=[],
     name_mapping={
+        "security_configuration_name": "securityConfigurationName",
         "cloud_watch_encryption": "cloudWatchEncryption",
         "job_bookmarks_encryption": "jobBookmarksEncryption",
         "s3_encryption": "s3Encryption",
-        "security_configuration_name": "securityConfigurationName",
     },
 )
 class SecurityConfigurationProps:
     def __init__(
         self,
         *,
-        cloud_watch_encryption: typing.Optional[typing.Union[CloudWatchEncryption, typing.Dict[builtins.str, typing.Any]]] = None,
-        job_bookmarks_encryption: typing.Optional[typing.Union[JobBookmarksEncryption, typing.Dict[builtins.str, typing.Any]]] = None,
-        s3_encryption: typing.Optional[typing.Union[S3Encryption, typing.Dict[builtins.str, typing.Any]]] = None,
-        security_configuration_name: typing.Optional[builtins.str] = None,
+        security_configuration_name: builtins.str,
+        cloud_watch_encryption: typing.Optional[CloudWatchEncryption] = None,
+        job_bookmarks_encryption: typing.Optional[JobBookmarksEncryption] = None,
+        s3_encryption: typing.Optional[S3Encryption] = None,
     ) -> None:
-        '''(experimental) Constructions properties of ``SecurityConfiguration``.
+        '''(experimental) Constructions properties of {@link SecurityConfiguration}.
 
+        :param security_configuration_name: (experimental) The name of the security configuration.
         :param cloud_watch_encryption: (experimental) The encryption configuration for Amazon CloudWatch Logs. Default: no cloudwatch logs encryption.
         :param job_bookmarks_encryption: (experimental) The encryption configuration for Glue Job Bookmarks. Default: no job bookmarks encryption.
         :param s3_encryption: (experimental) The encryption configuration for Amazon Simple Storage Service (Amazon S3) data. Default: no s3 encryption.
-        :param security_configuration_name: (experimental) The name of the security configuration. Default: - generated by CDK.
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
             glue.SecurityConfiguration(self, "MySecurityConfiguration",
+                security_configuration_name="name",
                 cloud_watch_encryption=glue.CloudWatchEncryption(
                     mode=glue.CloudWatchEncryptionMode.KMS
                 ),
                 job_bookmarks_encryption=glue.JobBookmarksEncryption(
                     mode=glue.JobBookmarksEncryptionMode.CLIENT_SIDE_KMS
                 ),
                 s3_encryption=glue.S3Encryption(
@@ -6175,29 +5655,33 @@
         '''
         if isinstance(cloud_watch_encryption, dict):
             cloud_watch_encryption = CloudWatchEncryption(**cloud_watch_encryption)
         if isinstance(job_bookmarks_encryption, dict):
             job_bookmarks_encryption = JobBookmarksEncryption(**job_bookmarks_encryption)
         if isinstance(s3_encryption, dict):
             s3_encryption = S3Encryption(**s3_encryption)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3b8dd2838cd56b87c144ac347e4b66a78dd0c85a6196f1282adce12bd2e94f36)
-            check_type(argname="argument cloud_watch_encryption", value=cloud_watch_encryption, expected_type=type_hints["cloud_watch_encryption"])
-            check_type(argname="argument job_bookmarks_encryption", value=job_bookmarks_encryption, expected_type=type_hints["job_bookmarks_encryption"])
-            check_type(argname="argument s3_encryption", value=s3_encryption, expected_type=type_hints["s3_encryption"])
-            check_type(argname="argument security_configuration_name", value=security_configuration_name, expected_type=type_hints["security_configuration_name"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {
+            "security_configuration_name": security_configuration_name,
+        }
         if cloud_watch_encryption is not None:
             self._values["cloud_watch_encryption"] = cloud_watch_encryption
         if job_bookmarks_encryption is not None:
             self._values["job_bookmarks_encryption"] = job_bookmarks_encryption
         if s3_encryption is not None:
             self._values["s3_encryption"] = s3_encryption
-        if security_configuration_name is not None:
-            self._values["security_configuration_name"] = security_configuration_name
+
+    @builtins.property
+    def security_configuration_name(self) -> builtins.str:
+        '''(experimental) The name of the security configuration.
+
+        :stability: experimental
+        '''
+        result = self._values.get("security_configuration_name")
+        assert result is not None, "Required property 'security_configuration_name' is missing"
+        return typing.cast(builtins.str, result)
 
     @builtins.property
     def cloud_watch_encryption(self) -> typing.Optional[CloudWatchEncryption]:
         '''(experimental) The encryption configuration for Amazon CloudWatch Logs.
 
         :default: no cloudwatch logs encryption.
 
@@ -6224,25 +5708,14 @@
         :default: no s3 encryption.
 
         :stability: experimental
         '''
         result = self._values.get("s3_encryption")
         return typing.cast(typing.Optional[S3Encryption], result)
 
-    @builtins.property
-    def security_configuration_name(self) -> typing.Optional[builtins.str]:
-        '''(experimental) The name of the security configuration.
-
-        :default: - generated by CDK.
-
-        :stability: experimental
-        '''
-        result = self._values.get("security_configuration_name")
-        return typing.cast(typing.Optional[builtins.str], result)
-
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -6272,110 +5745,107 @@
 
     def __init__(self, class_name: builtins.str) -> None:
         '''
         :param class_name: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__44b6eea0230610f203e5d4ed1dbd871c9ecc76a60681d0500a51e2d3815f193e)
-            check_type(argname="argument class_name", value=class_name, expected_type=type_hints["class_name"])
         jsii.create(self.__class__, self, [class_name])
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="AVRO")
     def AVRO(cls) -> "SerializationLibrary":
         '''
-        :see: https://svn.apache.org/repos/infra/websites/production/hive/content/javadocs/r3.1.3/api/org/apache/hadoop/hive/serde2/avro/AvroSerDe.html
+        :see: https://hive.apache.org/javadocs/r1.2.2/api/org/apache/hadoop/hive/serde2/avro/AvroSerDe.html
         :stability: experimental
         '''
         return typing.cast("SerializationLibrary", jsii.sget(cls, "AVRO"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="CLOUDTRAIL")
     def CLOUDTRAIL(cls) -> "SerializationLibrary":
         '''
         :see: https://docs.aws.amazon.com/athena/latest/ug/cloudtrail.html
         :stability: experimental
         '''
         return typing.cast("SerializationLibrary", jsii.sget(cls, "CLOUDTRAIL"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="GROK")
     def GROK(cls) -> "SerializationLibrary":
         '''
         :see: https://docs.aws.amazon.com/athena/latest/ug/grok.html
         :stability: experimental
         '''
         return typing.cast("SerializationLibrary", jsii.sget(cls, "GROK"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="HIVE_JSON")
     def HIVE_JSON(cls) -> "SerializationLibrary":
         '''
-        :see: https://svn.apache.org/repos/infra/websites/production/hive/content/javadocs/r3.1.3/api/org/apache/hive/hcatalog/data/JsonSerDe.html
+        :see: https://hive.apache.org/javadocs/r1.2.2/api/org/apache/hive/hcatalog/data/JsonSerDe.html
         :stability: experimental
         '''
         return typing.cast("SerializationLibrary", jsii.sget(cls, "HIVE_JSON"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="LAZY_SIMPLE")
     def LAZY_SIMPLE(cls) -> "SerializationLibrary":
         '''
-        :see: https://svn.apache.org/repos/infra/websites/production/hive/content/javadocs/r3.1.3/api/org/apache/hadoop/hive/serde2/lazy/LazySimpleSerDe.html
+        :see: https://hive.apache.org/javadocs/r1.2.2/api/org/apache/hadoop/hive/serde2/lazy/LazySimpleSerDe.html
         :stability: experimental
         '''
         return typing.cast("SerializationLibrary", jsii.sget(cls, "LAZY_SIMPLE"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="OPEN_CSV")
     def OPEN_CSV(cls) -> "SerializationLibrary":
         '''
-        :see: https://svn.apache.org/repos/infra/websites/production/hive/content/javadocs/r3.1.3/api/org/apache/hadoop/hive/serde2/OpenCSVSerde.html
+        :see: https://hive.apache.org/javadocs/r1.2.2/api/org/apache/hadoop/hive/serde2/OpenCSVSerde.html
         :stability: experimental
         '''
         return typing.cast("SerializationLibrary", jsii.sget(cls, "OPEN_CSV"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="OPENX_JSON")
     def OPENX_JSON(cls) -> "SerializationLibrary":
         '''
         :see: https://github.com/rcongiu/Hive-JSON-Serde
         :stability: experimental
         '''
         return typing.cast("SerializationLibrary", jsii.sget(cls, "OPENX_JSON"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="ORC")
     def ORC(cls) -> "SerializationLibrary":
         '''
-        :see: https://svn.apache.org/repos/infra/websites/production/hive/content/javadocs/r3.1.3/api/org/apache/hadoop/hive/ql/io/orc/OrcSerde.html
+        :see: https://hive.apache.org/javadocs/r1.2.2/api/org/apache/hadoop/hive/ql/io/orc/OrcSerde.html
         :stability: experimental
         '''
         return typing.cast("SerializationLibrary", jsii.sget(cls, "ORC"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="PARQUET")
     def PARQUET(cls) -> "SerializationLibrary":
         '''
-        :see: https://svn.apache.org/repos/infra/websites/production/hive/content/javadocs/r3.1.3/api/org/apache/hadoop/hive/ql/io/parquet/serde/ParquetHiveSerDe.html
+        :see: https://hive.apache.org/javadocs/r1.2.2/api/org/apache/hadoop/hive/ql/io/parquet/serde/ParquetHiveSerDe.html
         :stability: experimental
         '''
         return typing.cast("SerializationLibrary", jsii.sget(cls, "PARQUET"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="REGEXP")
     def REGEXP(cls) -> "SerializationLibrary":
         '''
-        :see: https://svn.apache.org/repos/infra/websites/production/hive/content/javadocs/r3.1.3/api/org/apache/hadoop/hive/serde2/RegexSerDe.html
+        :see: https://hive.apache.org/javadocs/r1.2.2/api/org/apache/hadoop/hive/serde2/RegexSerDe.html
         :stability: experimental
         '''
         return typing.cast("SerializationLibrary", jsii.sget(cls, "REGEXP"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="className")
     def class_name(self) -> builtins.str:
         '''
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "className"))
 
@@ -6385,15 +5855,15 @@
     jsii_struct_bases=[],
     name_mapping={"bucket": "bucket", "prefix": "prefix"},
 )
 class SparkUILoggingLocation:
     def __init__(
         self,
         *,
-        bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        bucket: aws_cdk.aws_s3.IBucket,
         prefix: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) The Spark UI logging location.
 
         :param bucket: (experimental) The bucket where the Glue job stores the logs.
         :param prefix: (experimental) The path inside the bucket (objects prefix) where the Glue job stores the logs. Default: '/' - the logs will be written at the root of the bucket
 
@@ -6413,33 +5883,29 @@
             spark_uILogging_location = glue_alpha.SparkUILoggingLocation(
                 bucket=bucket,
             
                 # the properties below are optional
                 prefix="prefix"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5697eede3034b2366456fa6abdccec9640fd76f2916540c3a178d004e5cd680a)
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
         '''(experimental) The bucket where the Glue job stores the logs.
 
         :stability: experimental
         '''
         result = self._values.get("bucket")
         assert result is not None, "Required property 'bucket' is missing"
-        return typing.cast(_aws_cdk_aws_s3_ceddda9d.IBucket, result)
+        return typing.cast(aws_cdk.aws_s3.IBucket, result)
 
     @builtins.property
     def prefix(self) -> typing.Optional[builtins.str]:
         '''(experimental) The path inside the bucket (objects prefix) where the Glue job stores the logs.
 
         :default: '/' - the logs will be written at the root of the bucket
 
@@ -6466,15 +5932,15 @@
     name_mapping={"enabled": "enabled", "bucket": "bucket", "prefix": "prefix"},
 )
 class SparkUIProps:
     def __init__(
         self,
         *,
         enabled: builtins.bool,
-        bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
+        bucket: typing.Optional[aws_cdk.aws_s3.IBucket] = None,
         prefix: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Properties for enabling Spark UI monitoring feature for Spark-based Glue jobs.
 
         :param enabled: (experimental) Enable Spark UI.
         :param bucket: (experimental) The bucket where the Glue job stores the logs. Default: a new bucket will be created.
         :param prefix: (experimental) The path inside the bucket (objects prefix) where the Glue job stores the logs. Default: '/' - the logs will be written at the root of the bucket
@@ -6496,20 +5962,15 @@
                 enabled=False,
             
                 # the properties below are optional
                 bucket=bucket,
                 prefix="prefix"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c613959b2bc20f05aa8f4578d26e870c2d4044aaaee1a5248ed0ddf8d4b75776)
-            check_type(argname="argument enabled", value=enabled, expected_type=type_hints["enabled"])
-            check_type(argname="argument bucket", value=bucket, expected_type=type_hints["bucket"])
-            check_type(argname="argument prefix", value=prefix, expected_type=type_hints["prefix"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "enabled": enabled,
         }
         if bucket is not None:
             self._values["bucket"] = bucket
         if prefix is not None:
             self._values["prefix"] = prefix
 
@@ -6520,23 +5981,23 @@
         :stability: experimental
         '''
         result = self._values.get("enabled")
         assert result is not None, "Required property 'enabled' is missing"
         return typing.cast(builtins.bool, result)
 
     @builtins.property
-    def bucket(self) -> typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket]:
+    def bucket(self) -> typing.Optional[aws_cdk.aws_s3.IBucket]:
         '''(experimental) The bucket where the Glue job stores the logs.
 
         :default: a new bucket will be created.
 
         :stability: experimental
         '''
         result = self._values.get("bucket")
-        return typing.cast(typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_s3.IBucket], result)
 
     @builtins.property
     def prefix(self) -> typing.Optional[builtins.str]:
         '''(experimental) The path inside the bucket (objects prefix) where the Glue job stores the logs.
 
         :default: '/' - the logs will be written at the root of the bucket
 
@@ -6555,29 +6016,30 @@
         return "SparkUIProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.implements(ITable)
 class Table(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-glue-alpha.Table",
 ):
     '''(experimental) A Glue table.
 
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
         # my_database: glue.Database
         
         glue.Table(self, "MyTable",
             database=my_database,
+            table_name="my_table",
             columns=[glue.Column(
                 name="col1",
                 type=glue.Schema.STRING
             )],
             partition_keys=[glue.Column(
                 name="year",
                 type=glue.Schema.SMALL_INT
@@ -6587,120 +6049,104 @@
             )],
             data_format=glue.DataFormat.JSON
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
-        columns: typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]],
+        columns: typing.Sequence[Column],
         database: IDatabase,
         data_format: DataFormat,
-        bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
+        table_name: builtins.str,
+        bucket: typing.Optional[aws_cdk.aws_s3.IBucket] = None,
         compressed: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
-        enable_partition_filtering: typing.Optional[builtins.bool] = None,
         encryption: typing.Optional["TableEncryption"] = None,
-        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-        partition_indexes: typing.Optional[typing.Sequence[typing.Union[PartitionIndex, typing.Dict[builtins.str, typing.Any]]]] = None,
-        partition_keys: typing.Optional[typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]]] = None,
+        encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
+        partition_indexes: typing.Optional[typing.Sequence[PartitionIndex]] = None,
+        partition_keys: typing.Optional[typing.Sequence[Column]] = None,
         s3_prefix: typing.Optional[builtins.str] = None,
         stored_as_sub_directories: typing.Optional[builtins.bool] = None,
-        table_name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param columns: (experimental) Columns of the table.
         :param database: (experimental) Database in which to store the table.
         :param data_format: (experimental) Storage type of the table's data.
+        :param table_name: (experimental) Name of the table.
         :param bucket: (experimental) S3 bucket in which to store data. Default: one is created for you
         :param compressed: (experimental) Indicates whether the table's data is compressed or not. Default: false
         :param description: (experimental) Description of the table. Default: generated
-        :param enable_partition_filtering: (experimental) Enables partition filtering. Default: - The parameter is not defined
-        :param encryption: (experimental) The kind of encryption to secure the data with. You can only provide this option if you are not explicitly passing in a bucket. If you choose ``SSE-KMS``, you *can* provide an un-managed KMS key with ``encryptionKey``. If you choose ``CSE-KMS``, you *must* provide an un-managed KMS key with ``encryptionKey``. Default: BucketEncryption.S3_MANAGED
+        :param encryption: (experimental) The kind of encryption to secure the data with. You can only provide this option if you are not explicitly passing in a bucket. If you choose ``SSE-KMS``, you *can* provide an un-managed KMS key with ``encryptionKey``. If you choose ``CSE-KMS``, you *must* provide an un-managed KMS key with ``encryptionKey``. Default: Unencrypted
         :param encryption_key: (experimental) External KMS key to use for bucket encryption. The ``encryption`` property must be ``SSE-KMS`` or ``CSE-KMS``. Default: key is managed by KMS.
         :param partition_indexes: (experimental) Partition indexes on the table. A maximum of 3 indexes are allowed on a table. Keys in the index must be part of the table's partition keys. Default: table has no partition indexes
         :param partition_keys: (experimental) Partition columns of the table. Default: table is not partitioned
         :param s3_prefix: (experimental) S3 prefix under which table objects are stored. Default: - No prefix. The data will be stored under the root of the bucket.
         :param stored_as_sub_directories: (experimental) Indicates whether the table data is stored in subdirectories. Default: false
-        :param table_name: (experimental) Name of the table. Default: - generated by CDK.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1146b20665153f742431bb500cb6e71362a22d8446ea9e132183e7be255411a3)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = TableProps(
             columns=columns,
             database=database,
             data_format=data_format,
+            table_name=table_name,
             bucket=bucket,
             compressed=compressed,
             description=description,
-            enable_partition_filtering=enable_partition_filtering,
             encryption=encryption,
             encryption_key=encryption_key,
             partition_indexes=partition_indexes,
             partition_keys=partition_keys,
             s3_prefix=s3_prefix,
             stored_as_sub_directories=stored_as_sub_directories,
-            table_name=table_name,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromTableArn")
+    @jsii.member(jsii_name="fromTableArn") # type: ignore[misc]
     @builtins.classmethod
     def from_table_arn(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         table_arn: builtins.str,
     ) -> ITable:
         '''
         :param scope: -
         :param id: -
         :param table_arn: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d2352656fb7b43cf3eb4a2aded8ee671361ffac4262eb238ffab674bdd5f1a43)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument table_arn", value=table_arn, expected_type=type_hints["table_arn"])
         return typing.cast(ITable, jsii.sinvoke(cls, "fromTableArn", [scope, id, table_arn]))
 
-    @jsii.member(jsii_name="fromTableAttributes")
+    @jsii.member(jsii_name="fromTableAttributes") # type: ignore[misc]
     @builtins.classmethod
     def from_table_attributes(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         table_arn: builtins.str,
         table_name: builtins.str,
     ) -> ITable:
         '''(experimental) Creates a Table construct that represents an external table.
 
         :param scope: The scope creating construct (usually ``this``).
         :param id: The construct's id.
         :param table_arn: 
         :param table_name: 
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__878a448eb32afe3f25973ce417c7da6d24066f7505ef5d1d41def8846459f1b2)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         attrs = TableAttributes(table_arn=table_arn, table_name=table_name)
 
         return typing.cast(ITable, jsii.sinvoke(cls, "fromTableAttributes", [scope, id, attrs]))
 
     @jsii.member(jsii_name="addPartitionIndex")
     def add_partition_index(
         self,
@@ -6723,201 +6169,178 @@
         index = PartitionIndex(key_names=key_names, index_name=index_name)
 
         return typing.cast(None, jsii.invoke(self, "addPartitionIndex", [index]))
 
     @jsii.member(jsii_name="grant")
     def grant(
         self,
-        grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
+        grantee: aws_cdk.aws_iam.IGrantable,
         actions: typing.Sequence[builtins.str],
-    ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
+    ) -> aws_cdk.aws_iam.Grant:
         '''(experimental) Grant the given identity custom permissions.
 
         :param grantee: -
         :param actions: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f4dfffa03e116904994394edf6d8a0cdb045dd643bd15f4851fffe2fcf3bb2c3)
-            check_type(argname="argument grantee", value=grantee, expected_type=type_hints["grantee"])
-            check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.Grant, jsii.invoke(self, "grant", [grantee, actions]))
+        return typing.cast(aws_cdk.aws_iam.Grant, jsii.invoke(self, "grant", [grantee, actions]))
 
     @jsii.member(jsii_name="grantRead")
-    def grant_read(
-        self,
-        grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-    ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
+    def grant_read(self, grantee: aws_cdk.aws_iam.IGrantable) -> aws_cdk.aws_iam.Grant:
         '''(experimental) Grant read permissions to the table and the underlying data stored in S3 to an IAM principal.
 
         :param grantee: the principal.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__178f51e9e12bf57dd3c2087ba05f992d088117836781e3d3ef35f50b93703bca)
-            check_type(argname="argument grantee", value=grantee, expected_type=type_hints["grantee"])
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.Grant, jsii.invoke(self, "grantRead", [grantee]))
+        return typing.cast(aws_cdk.aws_iam.Grant, jsii.invoke(self, "grantRead", [grantee]))
 
     @jsii.member(jsii_name="grantReadWrite")
     def grant_read_write(
         self,
-        grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-    ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
+        grantee: aws_cdk.aws_iam.IGrantable,
+    ) -> aws_cdk.aws_iam.Grant:
         '''(experimental) Grant read and write permissions to the table and the underlying data stored in S3 to an IAM principal.
 
         :param grantee: the principal.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3391fac8ac01ce95e4ae79063fb3652de1e9903f2059cae076fd5afb03ff397c)
-            check_type(argname="argument grantee", value=grantee, expected_type=type_hints["grantee"])
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.Grant, jsii.invoke(self, "grantReadWrite", [grantee]))
+        return typing.cast(aws_cdk.aws_iam.Grant, jsii.invoke(self, "grantReadWrite", [grantee]))
 
     @jsii.member(jsii_name="grantToUnderlyingResources")
     def grant_to_underlying_resources(
         self,
-        grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
+        grantee: aws_cdk.aws_iam.IGrantable,
         actions: typing.Sequence[builtins.str],
-    ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
+    ) -> aws_cdk.aws_iam.Grant:
         '''(experimental) Grant the given identity custom permissions to ALL underlying resources of the table.
 
         Permissions will be granted to the catalog, the database, and the table.
 
         :param grantee: -
         :param actions: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__63977272bab021689f3d71478f4c82752becd7b3d056de397295124ae552de69)
-            check_type(argname="argument grantee", value=grantee, expected_type=type_hints["grantee"])
-            check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.Grant, jsii.invoke(self, "grantToUnderlyingResources", [grantee, actions]))
+        return typing.cast(aws_cdk.aws_iam.Grant, jsii.invoke(self, "grantToUnderlyingResources", [grantee, actions]))
 
     @jsii.member(jsii_name="grantWrite")
-    def grant_write(
-        self,
-        grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-    ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
+    def grant_write(self, grantee: aws_cdk.aws_iam.IGrantable) -> aws_cdk.aws_iam.Grant:
         '''(experimental) Grant write permissions to the table and the underlying data stored in S3 to an IAM principal.
 
         :param grantee: the principal.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__57f6a44bd614de20527ea17e5e1d0bc11b21928cc61ce42b64421f9c1005f4d6)
-            check_type(argname="argument grantee", value=grantee, expected_type=type_hints["grantee"])
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.Grant, jsii.invoke(self, "grantWrite", [grantee]))
+        return typing.cast(aws_cdk.aws_iam.Grant, jsii.invoke(self, "grantWrite", [grantee]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="bucket")
-    def bucket(self) -> _aws_cdk_aws_s3_ceddda9d.IBucket:
+    def bucket(self) -> aws_cdk.aws_s3.IBucket:
         '''(experimental) S3 bucket in which the table's data resides.
 
         :stability: experimental
         '''
-        return typing.cast(_aws_cdk_aws_s3_ceddda9d.IBucket, jsii.get(self, "bucket"))
+        return typing.cast(aws_cdk.aws_s3.IBucket, jsii.get(self, "bucket"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="columns")
     def columns(self) -> typing.List[Column]:
         '''(experimental) This table's columns.
 
         :stability: experimental
         '''
         return typing.cast(typing.List[Column], jsii.get(self, "columns"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="compressed")
     def compressed(self) -> builtins.bool:
         '''(experimental) Indicates whether the table's data is compressed or not.
 
         :stability: experimental
         '''
         return typing.cast(builtins.bool, jsii.get(self, "compressed"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="database")
     def database(self) -> IDatabase:
         '''(experimental) Database this table belongs to.
 
         :stability: experimental
         '''
         return typing.cast(IDatabase, jsii.get(self, "database"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="dataFormat")
     def data_format(self) -> DataFormat:
         '''(experimental) Format of this table's data files.
 
         :stability: experimental
         '''
         return typing.cast(DataFormat, jsii.get(self, "dataFormat"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="encryption")
     def encryption(self) -> "TableEncryption":
         '''(experimental) The type of encryption enabled for the table.
 
         :stability: experimental
         '''
         return typing.cast("TableEncryption", jsii.get(self, "encryption"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="s3Prefix")
     def s3_prefix(self) -> builtins.str:
         '''(experimental) S3 Key Prefix under which this table's files are stored in S3.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "s3Prefix"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="tableArn")
     def table_arn(self) -> builtins.str:
         '''(experimental) ARN of this table.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "tableArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="tableName")
     def table_name(self) -> builtins.str:
         '''(experimental) Name of this table.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "tableName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="encryptionKey")
-    def encryption_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def encryption_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) The KMS key used to secure the data if ``encryption`` is set to ``CSE-KMS`` or ``SSE-KMS``.
 
         Otherwise, ``undefined``.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], jsii.get(self, "encryptionKey"))
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], jsii.get(self, "encryptionKey"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="partitionIndexes")
     def partition_indexes(self) -> typing.Optional[typing.List[PartitionIndex]]:
         '''(experimental) This table's partition indexes.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[typing.List[PartitionIndex]], jsii.get(self, "partitionIndexes"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="partitionKeys")
     def partition_keys(self) -> typing.Optional[typing.List[Column]]:
         '''(experimental) This table's partition keys if the table is partitioned.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[typing.List[Column]], jsii.get(self, "partitionKeys"))
@@ -6944,19 +6367,15 @@
             import aws_cdk.aws_glue_alpha as glue_alpha
             
             table_attributes = glue_alpha.TableAttributes(
                 table_arn="tableArn",
                 table_name="tableName"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b9a76a75ff6c3a793e7e5f24f77665e06ab62ec467008c0ae0a13c2537b6003d)
-            check_type(argname="argument table_arn", value=table_arn, expected_type=type_hints["table_arn"])
-            check_type(argname="argument table_name", value=table_name, expected_type=type_hints["table_name"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "table_arn": table_arn,
             "table_name": table_name,
         }
 
     @builtins.property
     def table_arn(self) -> builtins.str:
         '''
@@ -6999,22 +6418,27 @@
 
         # my_database: glue.Database
         
         glue.Table(self, "MyTable",
             encryption=glue.TableEncryption.S3_MANAGED,
             # ...
             database=my_database,
+            table_name="my_table",
             columns=[glue.Column(
                 name="col1",
                 type=glue.Schema.STRING
             )],
             data_format=glue.DataFormat.JSON
         )
     '''
 
+    UNENCRYPTED = "UNENCRYPTED"
+    '''
+    :stability: experimental
+    '''
     S3_MANAGED = "S3_MANAGED"
     '''(experimental) Server side encryption (SSE) with an Amazon S3-managed key.
 
     :see: https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingServerSideEncryption.html
     :stability: experimental
     '''
     KMS = "KMS"
@@ -7039,128 +6463,107 @@
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-glue-alpha.TableProps",
     jsii_struct_bases=[],
     name_mapping={
         "columns": "columns",
         "database": "database",
         "data_format": "dataFormat",
+        "table_name": "tableName",
         "bucket": "bucket",
         "compressed": "compressed",
         "description": "description",
-        "enable_partition_filtering": "enablePartitionFiltering",
         "encryption": "encryption",
         "encryption_key": "encryptionKey",
         "partition_indexes": "partitionIndexes",
         "partition_keys": "partitionKeys",
         "s3_prefix": "s3Prefix",
         "stored_as_sub_directories": "storedAsSubDirectories",
-        "table_name": "tableName",
     },
 )
 class TableProps:
     def __init__(
         self,
         *,
-        columns: typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]],
+        columns: typing.Sequence[Column],
         database: IDatabase,
         data_format: DataFormat,
-        bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
+        table_name: builtins.str,
+        bucket: typing.Optional[aws_cdk.aws_s3.IBucket] = None,
         compressed: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
-        enable_partition_filtering: typing.Optional[builtins.bool] = None,
         encryption: typing.Optional[TableEncryption] = None,
-        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-        partition_indexes: typing.Optional[typing.Sequence[typing.Union[PartitionIndex, typing.Dict[builtins.str, typing.Any]]]] = None,
-        partition_keys: typing.Optional[typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]]] = None,
+        encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
+        partition_indexes: typing.Optional[typing.Sequence[PartitionIndex]] = None,
+        partition_keys: typing.Optional[typing.Sequence[Column]] = None,
         s3_prefix: typing.Optional[builtins.str] = None,
         stored_as_sub_directories: typing.Optional[builtins.bool] = None,
-        table_name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param columns: (experimental) Columns of the table.
         :param database: (experimental) Database in which to store the table.
         :param data_format: (experimental) Storage type of the table's data.
+        :param table_name: (experimental) Name of the table.
         :param bucket: (experimental) S3 bucket in which to store data. Default: one is created for you
         :param compressed: (experimental) Indicates whether the table's data is compressed or not. Default: false
         :param description: (experimental) Description of the table. Default: generated
-        :param enable_partition_filtering: (experimental) Enables partition filtering. Default: - The parameter is not defined
-        :param encryption: (experimental) The kind of encryption to secure the data with. You can only provide this option if you are not explicitly passing in a bucket. If you choose ``SSE-KMS``, you *can* provide an un-managed KMS key with ``encryptionKey``. If you choose ``CSE-KMS``, you *must* provide an un-managed KMS key with ``encryptionKey``. Default: BucketEncryption.S3_MANAGED
+        :param encryption: (experimental) The kind of encryption to secure the data with. You can only provide this option if you are not explicitly passing in a bucket. If you choose ``SSE-KMS``, you *can* provide an un-managed KMS key with ``encryptionKey``. If you choose ``CSE-KMS``, you *must* provide an un-managed KMS key with ``encryptionKey``. Default: Unencrypted
         :param encryption_key: (experimental) External KMS key to use for bucket encryption. The ``encryption`` property must be ``SSE-KMS`` or ``CSE-KMS``. Default: key is managed by KMS.
         :param partition_indexes: (experimental) Partition indexes on the table. A maximum of 3 indexes are allowed on a table. Keys in the index must be part of the table's partition keys. Default: table has no partition indexes
         :param partition_keys: (experimental) Partition columns of the table. Default: table is not partitioned
         :param s3_prefix: (experimental) S3 prefix under which table objects are stored. Default: - No prefix. The data will be stored under the root of the bucket.
         :param stored_as_sub_directories: (experimental) Indicates whether the table data is stored in subdirectories. Default: false
-        :param table_name: (experimental) Name of the table. Default: - generated by CDK.
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
             # my_database: glue.Database
             
             glue.Table(self, "MyTable",
                 database=my_database,
+                table_name="my_table",
                 columns=[glue.Column(
                     name="col1",
                     type=glue.Schema.STRING
                 )],
                 partition_keys=[glue.Column(
                     name="year",
                     type=glue.Schema.SMALL_INT
                 ), glue.Column(
                     name="month",
                     type=glue.Schema.SMALL_INT
                 )],
                 data_format=glue.DataFormat.JSON
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0336d5abace2b9645857eae2fba5aa1c4bbb0db1762c5d5031d2f8c64019d606)
-            check_type(argname="argument columns", value=columns, expected_type=type_hints["columns"])
-            check_type(argname="argument database", value=database, expected_type=type_hints["database"])
-            check_type(argname="argument data_format", value=data_format, expected_type=type_hints["data_format"])
-            check_type(argname="argument bucket", value=bucket, expected_type=type_hints["bucket"])
-            check_type(argname="argument compressed", value=compressed, expected_type=type_hints["compressed"])
-            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
-            check_type(argname="argument enable_partition_filtering", value=enable_partition_filtering, expected_type=type_hints["enable_partition_filtering"])
-            check_type(argname="argument encryption", value=encryption, expected_type=type_hints["encryption"])
-            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
-            check_type(argname="argument partition_indexes", value=partition_indexes, expected_type=type_hints["partition_indexes"])
-            check_type(argname="argument partition_keys", value=partition_keys, expected_type=type_hints["partition_keys"])
-            check_type(argname="argument s3_prefix", value=s3_prefix, expected_type=type_hints["s3_prefix"])
-            check_type(argname="argument stored_as_sub_directories", value=stored_as_sub_directories, expected_type=type_hints["stored_as_sub_directories"])
-            check_type(argname="argument table_name", value=table_name, expected_type=type_hints["table_name"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "columns": columns,
             "database": database,
             "data_format": data_format,
+            "table_name": table_name,
         }
         if bucket is not None:
             self._values["bucket"] = bucket
         if compressed is not None:
             self._values["compressed"] = compressed
         if description is not None:
             self._values["description"] = description
-        if enable_partition_filtering is not None:
-            self._values["enable_partition_filtering"] = enable_partition_filtering
         if encryption is not None:
             self._values["encryption"] = encryption
         if encryption_key is not None:
             self._values["encryption_key"] = encryption_key
         if partition_indexes is not None:
             self._values["partition_indexes"] = partition_indexes
         if partition_keys is not None:
             self._values["partition_keys"] = partition_keys
         if s3_prefix is not None:
             self._values["s3_prefix"] = s3_prefix
         if stored_as_sub_directories is not None:
             self._values["stored_as_sub_directories"] = stored_as_sub_directories
-        if table_name is not None:
-            self._values["table_name"] = table_name
 
     @builtins.property
     def columns(self) -> typing.List[Column]:
         '''(experimental) Columns of the table.
 
         :stability: experimental
         '''
@@ -7185,23 +6588,33 @@
         :stability: experimental
         '''
         result = self._values.get("data_format")
         assert result is not None, "Required property 'data_format' is missing"
         return typing.cast(DataFormat, result)
 
     @builtins.property
-    def bucket(self) -> typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket]:
+    def table_name(self) -> builtins.str:
+        '''(experimental) Name of the table.
+
+        :stability: experimental
+        '''
+        result = self._values.get("table_name")
+        assert result is not None, "Required property 'table_name' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def bucket(self) -> typing.Optional[aws_cdk.aws_s3.IBucket]:
         '''(experimental) S3 bucket in which to store data.
 
         :default: one is created for you
 
         :stability: experimental
         '''
         result = self._values.get("bucket")
-        return typing.cast(typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_s3.IBucket], result)
 
     @builtins.property
     def compressed(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Indicates whether the table's data is compressed or not.
 
         :default: false
 
@@ -7218,53 +6631,41 @@
 
         :stability: experimental
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def enable_partition_filtering(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Enables partition filtering.
-
-        :default: - The parameter is not defined
-
-        :see: https://docs.aws.amazon.com/athena/latest/ug/glue-best-practices.html#glue-best-practices-partition-index
-        :stability: experimental
-        '''
-        result = self._values.get("enable_partition_filtering")
-        return typing.cast(typing.Optional[builtins.bool], result)
-
-    @builtins.property
     def encryption(self) -> typing.Optional[TableEncryption]:
         '''(experimental) The kind of encryption to secure the data with.
 
         You can only provide this option if you are not explicitly passing in a bucket.
 
         If you choose ``SSE-KMS``, you *can* provide an un-managed KMS key with ``encryptionKey``.
         If you choose ``CSE-KMS``, you *must* provide an un-managed KMS key with ``encryptionKey``.
 
-        :default: BucketEncryption.S3_MANAGED
+        :default: Unencrypted
 
         :stability: experimental
         '''
         result = self._values.get("encryption")
         return typing.cast(typing.Optional[TableEncryption], result)
 
     @builtins.property
-    def encryption_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def encryption_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) External KMS key to use for bucket encryption.
 
         The ``encryption`` property must be ``SSE-KMS`` or ``CSE-KMS``.
 
         :default: key is managed by KMS.
 
         :stability: experimental
         '''
         result = self._values.get("encryption_key")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], result)
 
     @builtins.property
     def partition_indexes(self) -> typing.Optional[typing.List[PartitionIndex]]:
         '''(experimental) Partition indexes on the table.
 
         A maximum of 3 indexes
         are allowed on a table. Keys in the index must be part
@@ -7306,25 +6707,14 @@
         :default: false
 
         :stability: experimental
         '''
         result = self._values.get("stored_as_sub_directories")
         return typing.cast(typing.Optional[builtins.bool], result)
 
-    @builtins.property
-    def table_name(self) -> typing.Optional[builtins.str]:
-        '''(experimental) Name of the table.
-
-        :default: - generated by CDK.
-
-        :stability: experimental
-        '''
-        result = self._values.get("table_name")
-        return typing.cast(typing.Optional[builtins.str], result)
-
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -7355,33 +6745,30 @@
 
         Example::
 
             # my_database: glue.Database
             
             glue.Table(self, "MyTable",
                 database=my_database,
+                table_name="my_table",
                 columns=[glue.Column(
                     name="col1",
                     type=glue.Schema.STRING
                 )],
                 partition_keys=[glue.Column(
                     name="year",
                     type=glue.Schema.SMALL_INT
                 ), glue.Column(
                     name="month",
                     type=glue.Schema.SMALL_INT
                 )],
                 data_format=glue.DataFormat.JSON
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c5fb0ad30c447263aceddf4b77f71aec991966bf6e2dc3a181ff400914c16d85)
-            check_type(argname="argument input_string", value=input_string, expected_type=type_hints["input_string"])
-            check_type(argname="argument is_primitive", value=is_primitive, expected_type=type_hints["is_primitive"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "input_string": input_string,
             "is_primitive": is_primitive,
         }
 
     @builtins.property
     def input_string(self) -> builtins.str:
         '''(experimental) Glue InputString for this type.
@@ -7420,120 +6807,68 @@
 ):
     '''(experimental) The type of predefined worker that is allocated when a job runs.
 
     If you need to use a WorkerType that doesn't exist as a static member, you
     can instantiate a ``WorkerType`` object, e.g: ``WorkerType.of('other type')``.
 
     :stability: experimental
-    :exampleMetadata: infused
+    :exampleMetadata: fixture=_generated
 
     Example::
 
-        # bucket: s3.Bucket
+        # The code below shows an example of how to instantiate this type.
+        # The values are placeholders you should change.
+        import aws_cdk.aws_glue_alpha as glue_alpha
         
-        glue.Job(self, "ScalaSparkEtlJob",
-            executable=glue.JobExecutable.scala_etl(
-                glue_version=glue.GlueVersion.V4_0,
-                script=glue.Code.from_bucket(bucket, "src/com/example/HelloWorld.scala"),
-                class_name="com.example.HelloWorld",
-                extra_jars=[glue.Code.from_bucket(bucket, "jars/HelloWorld.jar")]
-            ),
-            worker_type=glue.WorkerType.G_8X,
-            description="an example Scala ETL job"
-        )
+        worker_type = glue_alpha.WorkerType.G_1X
     '''
 
-    @jsii.member(jsii_name="of")
+    @jsii.member(jsii_name="of") # type: ignore[misc]
     @builtins.classmethod
     def of(cls, worker_type: builtins.str) -> "WorkerType":
         '''(experimental) Custom worker type.
 
         :param worker_type: custom worker type.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__217f80c6bee3c0db54c77a2a2bd0aa17178f371ff924355e6d6d4576a10d15c0)
-            check_type(argname="argument worker_type", value=worker_type, expected_type=type_hints["worker_type"])
         return typing.cast("WorkerType", jsii.sinvoke(cls, "of", [worker_type]))
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="G_025X")
-    def G_025_X(cls) -> "WorkerType":
-        '''(experimental) Each worker maps to 0.25 DPU (2 vCPU, 4 GB of memory, 64 GB disk), and provides 1 executor per worker. Suitable for low volume streaming jobs.
-
-        :stability: experimental
-        '''
-        return typing.cast("WorkerType", jsii.sget(cls, "G_025X"))
-
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="G_1X")
     def G_1_X(cls) -> "WorkerType":
         '''(experimental) Each worker maps to 1 DPU (4 vCPU, 16 GB of memory, 64 GB disk), and provides 1 executor per worker.
 
         Suitable for memory-intensive jobs.
 
         :stability: experimental
         '''
         return typing.cast("WorkerType", jsii.sget(cls, "G_1X"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="G_2X")
     def G_2_X(cls) -> "WorkerType":
         '''(experimental) Each worker maps to 2 DPU (8 vCPU, 32 GB of memory, 128 GB disk), and provides 1 executor per worker.
 
         Suitable for memory-intensive jobs.
 
         :stability: experimental
         '''
         return typing.cast("WorkerType", jsii.sget(cls, "G_2X"))
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="G_4X")
-    def G_4_X(cls) -> "WorkerType":
-        '''(experimental) Each worker maps to 4 DPU (16 vCPU, 64 GB of memory, 256 GB disk), and provides 1 executor per worker.
-
-        We recommend this worker type for jobs whose workloads contain your most demanding transforms, aggregations, joins, and queries. This worker type is available only for AWS Glue version 3.0 or later jobs.
-
-        :stability: experimental
-        '''
-        return typing.cast("WorkerType", jsii.sget(cls, "G_4X"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="G_8X")
-    def G_8_X(cls) -> "WorkerType":
-        '''(experimental) Each worker maps to 8 DPU (32 vCPU, 128 GB of memory, 512 GB disk), and provides 1 executor per worker.
-
-        We recommend this worker type for jobs whose workloads contain your most demanding transforms, aggregations, joins, and queries. This worker type is available only for AWS Glue version 3.0 or later jobs.
-
-        :stability: experimental
-        '''
-        return typing.cast("WorkerType", jsii.sget(cls, "G_8X"))
-
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="STANDARD")
     def STANDARD(cls) -> "WorkerType":
         '''(experimental) Each worker provides 4 vCPU, 16 GB of memory and a 50GB disk, and 2 executors per worker.
 
         :stability: experimental
         '''
         return typing.cast("WorkerType", jsii.sget(cls, "STANDARD"))
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="Z_2X")
-    def Z_2_X(cls) -> "WorkerType":
-        '''(experimental) Each worker maps to 2 high-memory DPU [M-DPU] (8 vCPU, 64 GB of memory, 128 GB disk).
-
-        Supported in Ray jobs.
-
-        :stability: experimental
-        '''
-        return typing.cast("WorkerType", jsii.sget(cls, "Z_2X"))
-
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         '''(experimental) The name of this WorkerType, as expected by Job resource.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "name"))
@@ -7564,108 +6899,94 @@
         asset_code = glue_alpha.AssetCode("path",
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
         path: builtins.str,
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
         :param path: The path to the Code file.
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
-            type_hints = typing.get_type_hints(_typecheckingstub__8659d1457c6b7393d9d7559014d5e5cf2fae91cdf81e1dcc8f010bdd5e6159d6)
-            check_type(argname="argument path", value=path, expected_type=type_hints["path"])
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
 
         jsii.create(self.__class__, self, [path, options])
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
-        scope: _constructs_77d1e7e8.Construct,
-        grantable: _aws_cdk_aws_iam_ceddda9d.IGrantable,
+        scope: constructs.Construct,
+        grantable: aws_cdk.aws_iam.IGrantable,
     ) -> CodeConfig:
         '''(experimental) Called when the Job is initialized to allow this object to bind.
 
         :param scope: -
         :param grantable: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__02569161383966e61e7748be2a2760721daf0107762bdf02e3d7b51459e0adda)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument grantable", value=grantable, expected_type=type_hints["grantable"])
         return typing.cast(CodeConfig, jsii.invoke(self, "bind", [scope, grantable]))
 
 
 @jsii.implements(IConnection)
 class Connection(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-glue-alpha.Connection",
 ):
     '''(experimental) An AWS Glue connection to a data source.
 
     :stability: experimental
     :exampleMetadata: infused
@@ -7682,233 +7003,208 @@
             # The VPC subnet which contains the data source
             subnet=subnet
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         type: ConnectionType,
         connection_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         match_criteria: typing.Optional[typing.Sequence[builtins.str]] = None,
         properties: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-        subnet: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISubnet] = None,
+        security_groups: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.ISecurityGroup]] = None,
+        subnet: typing.Optional[aws_cdk.aws_ec2.ISubnet] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param type: (experimental) The type of the connection.
         :param connection_name: (experimental) The name of the connection. Default: cloudformation generated name
         :param description: (experimental) The description of the connection. Default: no description
         :param match_criteria: (experimental) A list of criteria that can be used in selecting this connection. This is useful for filtering the results of https://awscli.amazonaws.com/v2/documentation/api/latest/reference/glue/get-connections.html Default: no match criteria
         :param properties: (experimental) Key-Value pairs that define parameters for the connection. Default: empty properties
         :param security_groups: (experimental) The list of security groups needed to successfully make this connection e.g. to successfully connect to VPC. Default: no security group
         :param subnet: (experimental) The VPC subnet to connect to resources within a VPC. See more at https://docs.aws.amazon.com/glue/latest/dg/start-connecting.html. Default: no subnet
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9e49faf739a72a3e5056a9506838a646b867a4b6b78cad2fc0eb56a8a3a4d314)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = ConnectionProps(
             type=type,
             connection_name=connection_name,
             description=description,
             match_criteria=match_criteria,
             properties=properties,
             security_groups=security_groups,
             subnet=subnet,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromConnectionArn")
+    @jsii.member(jsii_name="fromConnectionArn") # type: ignore[misc]
     @builtins.classmethod
     def from_connection_arn(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         connection_arn: builtins.str,
     ) -> IConnection:
         '''(experimental) Creates a Connection construct that represents an external connection.
 
         :param scope: The scope creating construct (usually ``this``).
         :param id: The construct's id.
         :param connection_arn: arn of external connection.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0a3a56fcf056a17ac1a36f3aeea6a054c7367495dbcff654385c491f79a8de6e)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument connection_arn", value=connection_arn, expected_type=type_hints["connection_arn"])
         return typing.cast(IConnection, jsii.sinvoke(cls, "fromConnectionArn", [scope, id, connection_arn]))
 
-    @jsii.member(jsii_name="fromConnectionName")
+    @jsii.member(jsii_name="fromConnectionName") # type: ignore[misc]
     @builtins.classmethod
     def from_connection_name(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         connection_name: builtins.str,
     ) -> IConnection:
         '''(experimental) Creates a Connection construct that represents an external connection.
 
         :param scope: The scope creating construct (usually ``this``).
         :param id: The construct's id.
         :param connection_name: name of external connection.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2376990bb2b0fdc1652696730260ad95accfa020e78a7421e67836ad9c49c867)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument connection_name", value=connection_name, expected_type=type_hints["connection_name"])
         return typing.cast(IConnection, jsii.sinvoke(cls, "fromConnectionName", [scope, id, connection_name]))
 
     @jsii.member(jsii_name="addProperty")
     def add_property(self, key: builtins.str, value: builtins.str) -> None:
         '''(experimental) Add additional connection parameters.
 
         :param key: parameter key.
         :param value: parameter value.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__664a10af42e73be7ad7fc6b49fd43b23cdb7750d16ad9c795923ec494e582778)
-            check_type(argname="argument key", value=key, expected_type=type_hints["key"])
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast(None, jsii.invoke(self, "addProperty", [key, value]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="connectionArn")
     def connection_arn(self) -> builtins.str:
         '''(experimental) The ARN of the connection.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "connectionArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="connectionName")
     def connection_name(self) -> builtins.str:
         '''(experimental) The name of the connection.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "connectionName"))
 
 
 @jsii.implements(IDatabase)
 class Database(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-glue-alpha.Database",
 ):
     '''(experimental) A Glue database.
 
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
-        glue.Database(self, "MyDatabase")
+        glue.Database(self, "MyDatabase",
+            database_name="my_database"
+        )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
-        database_name: typing.Optional[builtins.str] = None,
+        database_name: builtins.str,
         location_uri: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
-        :param database_name: (experimental) The name of the database. Default: - generated by CDK.
+        :param database_name: (experimental) The name of the database.
         :param location_uri: (experimental) The location of the database (for example, an HDFS path). Default: undefined. This field is optional in AWS::Glue::Database DatabaseInput
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2f4b410df1b0bf1116ce03c0e8a707776efd2f03da87fd718bf64b6a4964b2cd)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = DatabaseProps(database_name=database_name, location_uri=location_uri)
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromDatabaseArn")
+    @jsii.member(jsii_name="fromDatabaseArn") # type: ignore[misc]
     @builtins.classmethod
     def from_database_arn(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         database_arn: builtins.str,
     ) -> IDatabase:
         '''
         :param scope: -
         :param id: -
         :param database_arn: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6b20be4513bbaa9c562fcfb165fa327a8e6c6d38a0b15481eca8493b9b5a7b8d)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument database_arn", value=database_arn, expected_type=type_hints["database_arn"])
         return typing.cast(IDatabase, jsii.sinvoke(cls, "fromDatabaseArn", [scope, id, database_arn]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="catalogArn")
     def catalog_arn(self) -> builtins.str:
         '''(experimental) ARN of the Glue catalog in which this database is stored.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "catalogArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="catalogId")
     def catalog_id(self) -> builtins.str:
         '''(experimental) The catalog id of the database (usually, the AWS account id).
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "catalogId"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="databaseArn")
     def database_arn(self) -> builtins.str:
         '''(experimental) ARN of this database.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "databaseArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="databaseName")
     def database_name(self) -> builtins.str:
         '''(experimental) Name of this database.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "databaseName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="locationUri")
     def location_uri(self) -> typing.Optional[builtins.str]:
         '''(experimental) Location URI of this database.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "locationUri"))
@@ -7947,15 +7243,14 @@
     "JobLanguage",
     "JobProps",
     "JobState",
     "JobType",
     "MetricType",
     "OutputFormat",
     "PartitionIndex",
-    "PythonRayExecutableProps",
     "PythonShellExecutableProps",
     "PythonSparkJobExecutableProps",
     "PythonVersion",
     "S3Code",
     "S3Encryption",
     "S3EncryptionMode",
     "ScalaJobExecutableProps",
@@ -7970,752 +7265,7 @@
     "TableEncryption",
     "TableProps",
     "Type",
     "WorkerType",
 ]
 
 publication.publish()
-
-def _typecheckingstub__2bfce587a58c2deea97e71eeab8754a97692804f6d43271eda89c6257eaebdfc(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__ceec14d1d7029d8fb7df76e4abb14bc79250421d85a9584f0271d9e7c4f4ef3f(
-    *,
-    mode: CloudWatchEncryptionMode,
-    kms_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__cd7e88ca82e81ea6700503f28d9e5352c4a86e264d00afb35e761e591a7e0e24(
-    path: builtins.str,
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
-def _typecheckingstub__d23f6002340150960cebd70816482874d96a0de7d52265f1fcd0ab459eea2a61(
-    bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
-    key: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__7b88388256be44082f9ce622ac393616c31af36dc246d0cb6ea3eb8e78b31dc1(
-    scope: _constructs_77d1e7e8.Construct,
-    grantable: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__7667596ec33fb86df61ee9e5603a0bed57aa6e48e3795e84685966147e79b05e(
-    *,
-    s3_location: typing.Union[_aws_cdk_aws_s3_ceddda9d.Location, typing.Dict[builtins.str, typing.Any]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__043c8b76c78332fa2f7a0e1444ad14734d788355c87767ffb0dd0aac9a19fbdf(
-    *,
-    name: builtins.str,
-    type: typing.Union[Type, typing.Dict[builtins.str, typing.Any]],
-    comment: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a1670baf78db937cd3601a16badd87755f3fc525b8fd6a352d45c2bc3994b494(
-    *,
-    connection_name: typing.Optional[builtins.str] = None,
-    description: typing.Optional[builtins.str] = None,
-    match_criteria: typing.Optional[typing.Sequence[builtins.str]] = None,
-    properties: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-    subnet: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISubnet] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__d3fa037db6ada98c73a1d8889753f75c2f3c7513c8a41daf149dc5769cdb83e8(
-    *,
-    connection_name: typing.Optional[builtins.str] = None,
-    description: typing.Optional[builtins.str] = None,
-    match_criteria: typing.Optional[typing.Sequence[builtins.str]] = None,
-    properties: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-    subnet: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISubnet] = None,
-    type: ConnectionType,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b1f57c94567ffb3d89cdd8c9cd2b37bd37decd390b53c9bfdadd569dc797aa3f(
-    name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__6be4bb41017f52f2aa453e36400fa3a47b2e6bf3a87cf64d46e0345d6f22428b(
-    *,
-    enabled: builtins.bool,
-    conversion_pattern: typing.Optional[builtins.str] = None,
-    log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
-    log_stream_prefix: typing.Optional[builtins.str] = None,
-    quiet: typing.Optional[builtins.bool] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__f5302ed9f621270e44cf453ed62f78ee39e66f12961a87e084ec3d874438a19f(
-    *,
-    input_format: InputFormat,
-    output_format: OutputFormat,
-    serialization_library: SerializationLibrary,
-    classification_string: typing.Optional[ClassificationString] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__d07df31a9d41958f45422a1d7914c5016d66ed0e46a7e97ab37e2dd3d42ecf38(
-    *,
-    database_name: typing.Optional[builtins.str] = None,
-    location_uri: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__1bf24e914c5a2058c5a8ba633944792fe46a62d0d67ae96056f15edaf764112b(
-    version: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__79f8eb7ba0850dad06f49887b6323e6019fa48cdf967d96e579591ff36e61765(
-    metric_name: builtins.str,
-    type: MetricType,
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
-def _typecheckingstub__4e9bb641a392e36442ae2624591822707bc3af7603043bcb85c82e6dde0aedff(
-    id: builtins.str,
-    *,
-    target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-    cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
-    description: typing.Optional[builtins.str] = None,
-    event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
-    rule_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__192bf1eecc268b3f759e65151917fb49666d5a0144c2df120f2dd72e3fd5e4f4(
-    id: builtins.str,
-    *,
-    target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-    cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
-    description: typing.Optional[builtins.str] = None,
-    event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
-    rule_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__bab9c989bad00c9e92013f90e2646073cc90125f09e75268ec3f2999a69b9b8d(
-    id: builtins.str,
-    job_state: JobState,
-    *,
-    target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-    cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
-    description: typing.Optional[builtins.str] = None,
-    event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
-    rule_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__5b62843a9fea91eb93e6bf7bcd95a76fc790b72a6a7ae7024cf486b3fd9d20f7(
-    id: builtins.str,
-    *,
-    target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-    cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
-    description: typing.Optional[builtins.str] = None,
-    event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
-    rule_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b1fcdc972ccb29fe1572e8970cb83faccd76d7cee7f09ed3f5c9571bca7a886d(
-    id: builtins.str,
-    *,
-    target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-    cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
-    description: typing.Optional[builtins.str] = None,
-    event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
-    rule_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__697ee4e4007ce058f39e7fc610b2c0c4457bbd6008e9287406b18505ed299434(
-    class_name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e6176c370f308e8911be636fb1acf643512dbe9ca58823d8267644ab7efc406c(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    executable: JobExecutable,
-    connections: typing.Optional[typing.Sequence[IConnection]] = None,
-    continuous_logging: typing.Optional[typing.Union[ContinuousLoggingProps, typing.Dict[builtins.str, typing.Any]]] = None,
-    default_arguments: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-    description: typing.Optional[builtins.str] = None,
-    enable_profiling_metrics: typing.Optional[builtins.bool] = None,
-    job_name: typing.Optional[builtins.str] = None,
-    max_capacity: typing.Optional[jsii.Number] = None,
-    max_concurrent_runs: typing.Optional[jsii.Number] = None,
-    max_retries: typing.Optional[jsii.Number] = None,
-    notify_delay_after: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-    security_configuration: typing.Optional[ISecurityConfiguration] = None,
-    spark_ui: typing.Optional[typing.Union[SparkUIProps, typing.Dict[builtins.str, typing.Any]]] = None,
-    tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-    timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    worker_count: typing.Optional[jsii.Number] = None,
-    worker_type: typing.Optional[WorkerType] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__cd8db6c08c7bba32e81d8cda162918f634f3065c707bdd1ddfb404e329994882(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    job_name: builtins.str,
-    role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__c143c24940c0f180cf99d417380821b95c0287b9b01c42df4f74c6e7959a56b8(
-    metric_name: builtins.str,
-    type: MetricType,
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
-def _typecheckingstub__1d8262e07cdf8942bd30cd21bf9d73a8b85e3b2683e99b4f40ed03fbf49b57ac(
-    id: builtins.str,
-    *,
-    target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-    cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
-    description: typing.Optional[builtins.str] = None,
-    event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
-    rule_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a8a1d8b4180629a6e1364fed24a3f246786b2d528b0ef21dda37098ac2af2c9a(
-    id: builtins.str,
-    *,
-    target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-    cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
-    description: typing.Optional[builtins.str] = None,
-    event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
-    rule_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0546c2bad534dee21310d2705463267023bd2bd40cd093c29b95dccda7c69228(
-    id: builtins.str,
-    job_state: JobState,
-    *,
-    target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-    cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
-    description: typing.Optional[builtins.str] = None,
-    event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
-    rule_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b8390e01882a245ed021fa1f65648219d84b9932b1c593026055b61fe2c56a85(
-    id: builtins.str,
-    *,
-    target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-    cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
-    description: typing.Optional[builtins.str] = None,
-    event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
-    rule_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b061eb382ce02e7e8798f77ad4abe593f170f59b9df192c9e6c5fb3de7901a33(
-    id: builtins.str,
-    *,
-    target: typing.Optional[_aws_cdk_aws_events_ceddda9d.IRuleTarget] = None,
-    cross_stack_scope: typing.Optional[_constructs_77d1e7e8.Construct] = None,
-    description: typing.Optional[builtins.str] = None,
-    event_pattern: typing.Optional[typing.Union[_aws_cdk_aws_events_ceddda9d.EventPattern, typing.Dict[builtins.str, typing.Any]]] = None,
-    rule_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__2f1f5ae0406d4aaf443249ea9377b38a10b1814ed1f9c1fb9f0cbc5f489fd89e(
-    *,
-    job_name: builtins.str,
-    role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__61a555ea81acfe554401802d7d44d70d3e1a6f96890ffbc28283fadb7ea81f9e(
-    *,
-    mode: JobBookmarksEncryptionMode,
-    kms_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__629e6b8d2f364b0c0cfaa00ca6e06725f3d280ad7a2366cf5df8f63e472fea40(
-    *,
-    glue_version: GlueVersion,
-    language: JobLanguage,
-    script: Code,
-    type: JobType,
-    class_name: typing.Optional[builtins.str] = None,
-    extra_files: typing.Optional[typing.Sequence[Code]] = None,
-    extra_jars: typing.Optional[typing.Sequence[Code]] = None,
-    extra_jars_first: typing.Optional[builtins.bool] = None,
-    extra_python_files: typing.Optional[typing.Sequence[Code]] = None,
-    python_version: typing.Optional[PythonVersion] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__9f47dc7b3a9514a79f7f82e52c4441b82161dce2eb5b67f22211660776beaa70(
-    *,
-    executable: JobExecutable,
-    connections: typing.Optional[typing.Sequence[IConnection]] = None,
-    continuous_logging: typing.Optional[typing.Union[ContinuousLoggingProps, typing.Dict[builtins.str, typing.Any]]] = None,
-    default_arguments: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-    description: typing.Optional[builtins.str] = None,
-    enable_profiling_metrics: typing.Optional[builtins.bool] = None,
-    job_name: typing.Optional[builtins.str] = None,
-    max_capacity: typing.Optional[jsii.Number] = None,
-    max_concurrent_runs: typing.Optional[jsii.Number] = None,
-    max_retries: typing.Optional[jsii.Number] = None,
-    notify_delay_after: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-    security_configuration: typing.Optional[ISecurityConfiguration] = None,
-    spark_ui: typing.Optional[typing.Union[SparkUIProps, typing.Dict[builtins.str, typing.Any]]] = None,
-    tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-    timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    worker_count: typing.Optional[jsii.Number] = None,
-    worker_type: typing.Optional[WorkerType] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0683afe40f10e5c8c02ac80ffb25aca1e5830884e6b5e539accb9e36df90257d(
-    name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__8952681a040fc7931f48438a2e01cd3c2bed40202b6f32cd606344a5ea10e810(
-    class_name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__854153aaeace5af7af75594677e850d114f911156b5cd93d50a01feeff4a76a8(
-    *,
-    key_names: typing.Sequence[builtins.str],
-    index_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__96728d115db88df2280e8997d67958a9b8d05214b04966c306fbf00f84a6324f(
-    *,
-    glue_version: GlueVersion,
-    python_version: PythonVersion,
-    script: Code,
-    extra_files: typing.Optional[typing.Sequence[Code]] = None,
-    extra_python_files: typing.Optional[typing.Sequence[Code]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__787eb0d11407cb3ae6ba15f28cff4370dd45126f9ce4e2ab093edba7a3b628e8(
-    *,
-    glue_version: GlueVersion,
-    python_version: PythonVersion,
-    script: Code,
-    extra_files: typing.Optional[typing.Sequence[Code]] = None,
-    extra_python_files: typing.Optional[typing.Sequence[Code]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__2e0bf4f1c4314f36fa21cf1fde861d972bb36e11678ce6f78e9dab93055f9ed4(
-    *,
-    glue_version: GlueVersion,
-    python_version: PythonVersion,
-    script: Code,
-    extra_files: typing.Optional[typing.Sequence[Code]] = None,
-    extra_jars: typing.Optional[typing.Sequence[Code]] = None,
-    extra_jars_first: typing.Optional[builtins.bool] = None,
-    extra_python_files: typing.Optional[typing.Sequence[Code]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__f7854e17fe796bdc5dc10fe3c8febb691186728550ca107493a43fc6979cafee(
-    bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
-    key: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__18fa6b6bc6e19007515f753b3e849efd4b7a16720ea785b0e155f20075d71602(
-    _scope: _constructs_77d1e7e8.Construct,
-    grantable: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__d972222b3b5c087e70a7ab859853e97f1579eeee2ede763d551c41d4076f740e(
-    *,
-    mode: S3EncryptionMode,
-    kms_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a8895a1f83a364cc50cc706b326361b090931a87ba5ad2c1f9a0747bf6c0f7e7(
-    *,
-    class_name: builtins.str,
-    glue_version: GlueVersion,
-    script: Code,
-    extra_files: typing.Optional[typing.Sequence[Code]] = None,
-    extra_jars: typing.Optional[typing.Sequence[Code]] = None,
-    extra_jars_first: typing.Optional[builtins.bool] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__d4b92f46741e45dc5d5e256fe3738d53a8878b40fc430d149eec6fdbfe167229(
-    length: jsii.Number,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__fcdd8f07d6d5e4e87f54cd2104a8605a571a6abede0b42465e2352b51723b900(
-    precision: jsii.Number,
-    scale: typing.Optional[jsii.Number] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__fc04f65c508e37fca936dfd67a8b4a0f84a73b9ef9c446edcd34f17c738c8dae(
-    key_type: typing.Union[Type, typing.Dict[builtins.str, typing.Any]],
-    *,
-    input_string: builtins.str,
-    is_primitive: builtins.bool,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__33f94b4c838eb0e3d03de4da6b4f3fe8e873ef98895fb940645c459801c4bb50(
-    columns: typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0ba18137b7dd32100f635af375c8586adc2f9824c4ccd0a1b01168f5ba757da4(
-    length: jsii.Number,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__cd628a6199f5b5fb7644771f78b6cc6d9230e3c38bba0463810d192bceb52e8d(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    cloud_watch_encryption: typing.Optional[typing.Union[CloudWatchEncryption, typing.Dict[builtins.str, typing.Any]]] = None,
-    job_bookmarks_encryption: typing.Optional[typing.Union[JobBookmarksEncryption, typing.Dict[builtins.str, typing.Any]]] = None,
-    s3_encryption: typing.Optional[typing.Union[S3Encryption, typing.Dict[builtins.str, typing.Any]]] = None,
-    security_configuration_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__4a85db96fd444625c46f4574190ecd86214bed327c2f826ee3294853f69a42b6(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    security_configuration_name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__3b8dd2838cd56b87c144ac347e4b66a78dd0c85a6196f1282adce12bd2e94f36(
-    *,
-    cloud_watch_encryption: typing.Optional[typing.Union[CloudWatchEncryption, typing.Dict[builtins.str, typing.Any]]] = None,
-    job_bookmarks_encryption: typing.Optional[typing.Union[JobBookmarksEncryption, typing.Dict[builtins.str, typing.Any]]] = None,
-    s3_encryption: typing.Optional[typing.Union[S3Encryption, typing.Dict[builtins.str, typing.Any]]] = None,
-    security_configuration_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__44b6eea0230610f203e5d4ed1dbd871c9ecc76a60681d0500a51e2d3815f193e(
-    class_name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__5697eede3034b2366456fa6abdccec9640fd76f2916540c3a178d004e5cd680a(
-    *,
-    bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
-    prefix: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__c613959b2bc20f05aa8f4578d26e870c2d4044aaaee1a5248ed0ddf8d4b75776(
-    *,
-    enabled: builtins.bool,
-    bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
-    prefix: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__1146b20665153f742431bb500cb6e71362a22d8446ea9e132183e7be255411a3(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    columns: typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]],
-    database: IDatabase,
-    data_format: DataFormat,
-    bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
-    compressed: typing.Optional[builtins.bool] = None,
-    description: typing.Optional[builtins.str] = None,
-    enable_partition_filtering: typing.Optional[builtins.bool] = None,
-    encryption: typing.Optional[TableEncryption] = None,
-    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-    partition_indexes: typing.Optional[typing.Sequence[typing.Union[PartitionIndex, typing.Dict[builtins.str, typing.Any]]]] = None,
-    partition_keys: typing.Optional[typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]]] = None,
-    s3_prefix: typing.Optional[builtins.str] = None,
-    stored_as_sub_directories: typing.Optional[builtins.bool] = None,
-    table_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__d2352656fb7b43cf3eb4a2aded8ee671361ffac4262eb238ffab674bdd5f1a43(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    table_arn: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__878a448eb32afe3f25973ce417c7da6d24066f7505ef5d1d41def8846459f1b2(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    table_arn: builtins.str,
-    table_name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__f4dfffa03e116904994394edf6d8a0cdb045dd643bd15f4851fffe2fcf3bb2c3(
-    grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-    actions: typing.Sequence[builtins.str],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__178f51e9e12bf57dd3c2087ba05f992d088117836781e3d3ef35f50b93703bca(
-    grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__3391fac8ac01ce95e4ae79063fb3652de1e9903f2059cae076fd5afb03ff397c(
-    grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__63977272bab021689f3d71478f4c82752becd7b3d056de397295124ae552de69(
-    grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-    actions: typing.Sequence[builtins.str],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__57f6a44bd614de20527ea17e5e1d0bc11b21928cc61ce42b64421f9c1005f4d6(
-    grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b9a76a75ff6c3a793e7e5f24f77665e06ab62ec467008c0ae0a13c2537b6003d(
-    *,
-    table_arn: builtins.str,
-    table_name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0336d5abace2b9645857eae2fba5aa1c4bbb0db1762c5d5031d2f8c64019d606(
-    *,
-    columns: typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]],
-    database: IDatabase,
-    data_format: DataFormat,
-    bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
-    compressed: typing.Optional[builtins.bool] = None,
-    description: typing.Optional[builtins.str] = None,
-    enable_partition_filtering: typing.Optional[builtins.bool] = None,
-    encryption: typing.Optional[TableEncryption] = None,
-    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-    partition_indexes: typing.Optional[typing.Sequence[typing.Union[PartitionIndex, typing.Dict[builtins.str, typing.Any]]]] = None,
-    partition_keys: typing.Optional[typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]]] = None,
-    s3_prefix: typing.Optional[builtins.str] = None,
-    stored_as_sub_directories: typing.Optional[builtins.bool] = None,
-    table_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__c5fb0ad30c447263aceddf4b77f71aec991966bf6e2dc3a181ff400914c16d85(
-    *,
-    input_string: builtins.str,
-    is_primitive: builtins.bool,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__217f80c6bee3c0db54c77a2a2bd0aa17178f371ff924355e6d6d4576a10d15c0(
-    worker_type: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__8659d1457c6b7393d9d7559014d5e5cf2fae91cdf81e1dcc8f010bdd5e6159d6(
-    path: builtins.str,
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
-def _typecheckingstub__02569161383966e61e7748be2a2760721daf0107762bdf02e3d7b51459e0adda(
-    scope: _constructs_77d1e7e8.Construct,
-    grantable: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__9e49faf739a72a3e5056a9506838a646b867a4b6b78cad2fc0eb56a8a3a4d314(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    type: ConnectionType,
-    connection_name: typing.Optional[builtins.str] = None,
-    description: typing.Optional[builtins.str] = None,
-    match_criteria: typing.Optional[typing.Sequence[builtins.str]] = None,
-    properties: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-    subnet: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ISubnet] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0a3a56fcf056a17ac1a36f3aeea6a054c7367495dbcff654385c491f79a8de6e(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    connection_arn: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__2376990bb2b0fdc1652696730260ad95accfa020e78a7421e67836ad9c49c867(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    connection_name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__664a10af42e73be7ad7fc6b49fd43b23cdb7750d16ad9c795923ec494e582778(
-    key: builtins.str,
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__2f4b410df1b0bf1116ce03c0e8a707776efd2f03da87fd718bf64b6a4964b2cd(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    database_name: typing.Optional[builtins.str] = None,
-    location_uri: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__6b20be4513bbaa9c562fcfb165fa327a8e6c6d38a0b15481eca8493b9b5a7b8d(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    database_arn: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
```

### Comparing `aws-cdk.aws-glue-alpha-2.84.0a0/src/aws_cdk.aws_glue_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-glue-alpha-2.9.0a0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: aws-cdk.aws-glue-alpha
-Version: 2.84.0a0
-Summary: The CDK Construct Library for AWS::Glue
-Home-page: https://github.com/aws/aws-cdk
-Author: Amazon Web Services
-License: Apache-2.0
-Project-URL: Source, https://github.com/aws/aws-cdk.git
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: JavaScript
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Typing :: Typed
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved
-Classifier: Framework :: AWS CDK
-Classifier: Framework :: AWS CDK :: 2
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: NOTICE
-
 # AWS Glue Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
 
 
 ![cdk-constructs: Experimental](https://img.shields.io/badge/cdk--constructs-experimental-important.svg?style=for-the-badge)
 
@@ -62,78 +35,56 @@
 An ETL job processes data in batches using Apache Spark.
 
 ```python
 # bucket: s3.Bucket
 
 glue.Job(self, "ScalaSparkEtlJob",
     executable=glue.JobExecutable.scala_etl(
-        glue_version=glue.GlueVersion.V4_0,
+        glue_version=glue.GlueVersion.V2_0,
         script=glue.Code.from_bucket(bucket, "src/com/example/HelloWorld.scala"),
         class_name="com.example.HelloWorld",
         extra_jars=[glue.Code.from_bucket(bucket, "jars/HelloWorld.jar")]
     ),
-    worker_type=glue.WorkerType.G_8X,
     description="an example Scala ETL job"
 )
 ```
 
 #### Streaming Jobs
 
 A Streaming job is similar to an ETL job, except that it performs ETL on data streams. It uses the Apache Spark Structured Streaming framework. Some Spark job features are not available to streaming ETL jobs.
 
 ```python
 glue.Job(self, "PythonSparkStreamingJob",
     executable=glue.JobExecutable.python_streaming(
-        glue_version=glue.GlueVersion.V4_0,
+        glue_version=glue.GlueVersion.V2_0,
         python_version=glue.PythonVersion.THREE,
         script=glue.Code.from_asset(path.join(__dirname, "job-script/hello_world.py"))
     ),
     description="an example Python Streaming job"
 )
 ```
 
 ### Python Shell Jobs
 
 A Python shell job runs Python scripts as a shell and supports a Python version that depends on the AWS Glue version you are using.
-This can be used to schedule and run tasks that don't require an Apache Spark environment. Currently, three flavors are supported:
-
-* PythonVersion.TWO (2.7; EOL)
-* PythonVersion.THREE (3.6)
-* PythonVersion.THREE_NINE (3.9)
+This can be used to schedule and run tasks that don't require an Apache Spark environment.
 
 ```python
 # bucket: s3.Bucket
 
 glue.Job(self, "PythonShellJob",
     executable=glue.JobExecutable.python_shell(
         glue_version=glue.GlueVersion.V1_0,
         python_version=glue.PythonVersion.THREE,
         script=glue.Code.from_bucket(bucket, "script.py")
     ),
     description="an example Python Shell job"
 )
 ```
 
-### Ray Jobs
-
-These jobs run in a Ray environment managed by AWS Glue.
-
-```python
-glue.Job(self, "RayJob",
-    executable=glue.JobExecutable.python_ray(
-        glue_version=glue.GlueVersion.V4_0,
-        python_version=glue.PythonVersion.THREE_NINE,
-        script=glue.Code.from_asset(path.join(__dirname, "job-script/hello_world.py"))
-    ),
-    worker_type=glue.WorkerType.Z_2X,
-    worker_count=2,
-    description="an example Ray job"
-)
-```
-
 See [documentation](https://docs.aws.amazon.com/glue/latest/dg/add-job.html) for more information on adding jobs in Glue.
 
 ## Connection
 
 A `Connection` allows Glue jobs, crawlers and development endpoints to access certain types of data stores. For example, to create a network connection to connect to a data source within a VPC:
 
 ```python
@@ -145,43 +96,25 @@
     # The security groups granting AWS Glue inbound access to the data source within the VPC
     security_groups=[security_group],
     # The VPC subnet which contains the data source
     subnet=subnet
 )
 ```
 
-For RDS `Connection` by JDBC, it is recommended to manage credentials using AWS Secrets Manager. To use Secret, specify `SECRET_ID` in `properties` like the following code. Note that in this case, the subnet must have a route to the AWS Secrets Manager VPC endpoint or to the AWS Secrets Manager endpoint through a NAT gateway.
-
-```python
-# security_group: ec2.SecurityGroup
-# subnet: ec2.Subnet
-# db: rds.DatabaseCluster
-
-glue.Connection(self, "RdsConnection",
-    type=glue.ConnectionType.JDBC,
-    security_groups=[security_group],
-    subnet=subnet,
-    properties={
-        "JDBC_CONNECTION_URL": f"jdbc:mysql://{db.clusterEndpoint.socketAddress}/databasename",
-        "JDBC_ENFORCE_SSL": "false",
-        "SECRET_ID": db.secret.secret_name
-    }
-)
-```
-
 If you need to use a connection type that doesn't exist as a static member on `ConnectionType`, you can instantiate a `ConnectionType` object, e.g: `new glue.ConnectionType('NEW_TYPE')`.
 
 See [Adding a Connection to Your Data Store](https://docs.aws.amazon.com/glue/latest/dg/populate-add-connection.html) and [Connection Structure](https://docs.aws.amazon.com/glue/latest/dg/aws-glue-api-catalog-connections.html#aws-glue-api-catalog-connections-Connection) documentation for more information on the supported data stores and their configurations.
 
 ## SecurityConfiguration
 
 A `SecurityConfiguration` is a set of security properties that can be used by AWS Glue to encrypt data at rest.
 
 ```python
 glue.SecurityConfiguration(self, "MySecurityConfiguration",
+    security_configuration_name="name",
     cloud_watch_encryption=glue.CloudWatchEncryption(
         mode=glue.CloudWatchEncryptionMode.KMS
     ),
     job_bookmarks_encryption=glue.JobBookmarksEncryption(
         mode=glue.JobBookmarksEncryptionMode.CLIENT_SIDE_KMS
     ),
     s3_encryption=glue.S3Encryption(
@@ -192,40 +125,44 @@
 
 By default, a shared KMS key is created for use with the encryption configurations that require one. You can also supply your own key for each encryption config, for example, for CloudWatch encryption:
 
 ```python
 # key: kms.Key
 
 glue.SecurityConfiguration(self, "MySecurityConfiguration",
+    security_configuration_name="name",
     cloud_watch_encryption=glue.CloudWatchEncryption(
         mode=glue.CloudWatchEncryptionMode.KMS,
         kms_key=key
     )
 )
 ```
 
 See [documentation](https://docs.aws.amazon.com/glue/latest/dg/encryption-security-configuration.html) for more info for Glue encrypting data written by Crawlers, Jobs, and Development Endpoints.
 
 ## Database
 
 A `Database` is a logical grouping of `Tables` in the Glue Catalog.
 
 ```python
-glue.Database(self, "MyDatabase")
+glue.Database(self, "MyDatabase",
+    database_name="my_database"
+)
 ```
 
 ## Table
 
 A Glue table describes a table of data in S3: its structure (column names and types), location of data (S3 objects with a common prefix in a S3 bucket), and format for the files (Json, Avro, Parquet, etc.):
 
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     ), glue.Column(
         name="col2",
         type=glue.Schema.array(glue.Schema.STRING),
         comment="col2 is an array of strings"
@@ -241,14 +178,15 @@
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     bucket=my_bucket,
     s3_prefix="my-table/",
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -260,14 +198,15 @@
 To improve query performance, a table can specify `partitionKeys` on which data is stored and queried separately. For example, you might partition a table by `year` and `month` to optimize queries based on a time window:
 
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     partition_keys=[glue.Column(
         name="year",
         type=glue.Schema.SMALL_INT
@@ -292,14 +231,15 @@
 property:
 
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     partition_keys=[glue.Column(
         name="year",
         type=glue.Schema.SMALL_INT
@@ -322,52 +262,29 @@
 
 my_table.add_partition_index(
     index_name="my-index",
     key_names=["year"]
 )
 ```
 
-### Partition Filtering
-
-If you have a table with a large number of partitions that grows over time, consider using AWS Glue partition indexing and filtering.
-
-```python
-# my_database: glue.Database
-
-glue.Table(self, "MyTable",
-    database=my_database,
-    columns=[glue.Column(
-        name="col1",
-        type=glue.Schema.STRING
-    )],
-    partition_keys=[glue.Column(
-        name="year",
-        type=glue.Schema.SMALL_INT
-    ), glue.Column(
-        name="month",
-        type=glue.Schema.SMALL_INT
-    )],
-    data_format=glue.DataFormat.JSON,
-    enable_partition_filtering=True
-)
-```
-
 ## [Encryption](https://docs.aws.amazon.com/athena/latest/ug/encryption.html)
 
 You can enable encryption on a Table's data:
 
-* [S3Managed](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingServerSideEncryption.html) - (default) Server side encryption (`SSE-S3`) with an Amazon S3-managed key.
+* `Unencrypted` - files are not encrypted. The default encryption setting.
+* [S3Managed](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingServerSideEncryption.html) - Server side encryption (`SSE-S3`) with an Amazon S3-managed key.
 
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.S3_MANAGED,
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -378,27 +295,29 @@
 # my_database: glue.Database
 
 # KMS key is created automatically
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.KMS,
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 
 # with an explicit KMS key
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.KMS,
     encryption_key=kms.Key(self, "MyKey"),
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -408,14 +327,15 @@
 ```python
 # my_database: glue.Database
 
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.KMS_MANAGED,
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -426,27 +346,29 @@
 # my_database: glue.Database
 
 # KMS key is created automatically
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.CLIENT_SIDE_KMS,
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 
 # with an explicit KMS key
 glue.Table(self, "MyTable",
     encryption=glue.TableEncryption.CLIENT_SIDE_KMS,
     encryption_key=kms.Key(self, "MyKey"),
     # ...
     database=my_database,
+    table_name="my_table",
     columns=[glue.Column(
         name="col1",
         type=glue.Schema.STRING
     )],
     data_format=glue.DataFormat.JSON
 )
 ```
@@ -479,14 +401,15 @@
             type=glue.Schema.DATE,
             comment="nested comment"
         ]),
         comment="struct<nested_column:date COMMENT 'nested comment'>"
     )],
     # ...
     database=my_database,
+    table_name="my_table",
     data_format=glue.DataFormat.JSON
 )
 ```
 
 ### Primitives
 
 #### Numeric
```

