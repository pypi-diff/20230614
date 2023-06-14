# Comparing `tmp/aws-cdk.aws-redshift-alpha-2.84.0a0.tar.gz` & `tmp/aws-cdk.aws-redshift-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/aws-redshift-alpha/dist/python/aws-cdk.aws-redshift-alpha-2.84.0a0.tar", last modified: Tue Jun 13 23:47:08 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-redshift/dist/python/aws-cdk.aws-redshift-alpha-2.9.0a0.tar", last modified: Wed Jan 26 11:22:06 2022, max compression
```

## Comparing `aws-cdk.aws-redshift-alpha-2.84.0a0.tar` & `aws-cdk.aws-redshift-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:08.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:57.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:57.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 23:46:57.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    20569 2023-06-13 23:47:08.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    19566 2023-06-13 23:46:57.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:57.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:47:08.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1877 2023-06-13 23:46:57.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:08.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:08.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:08.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/src/aws_cdk/aws_redshift_alpha/
--rw-r--r--   0 root         (0) root         (0)   195266 2023-06-13 23:46:57.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/src/aws_cdk/aws_redshift_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:08.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/src/aws_cdk/aws_redshift_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      443 2023-06-13 23:46:57.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/src/aws_cdk/aws_redshift_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   131947 2023-06-13 23:46:57.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/src/aws_cdk/aws_redshift_alpha/_jsii/aws-redshift-alpha@2.84.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:57.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/src/aws_cdk/aws_redshift_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:08.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/src/aws_cdk.aws_redshift_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    20569 2023-06-13 23:47:08.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/src/aws_cdk.aws_redshift_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      541 2023-06-13 23:47:08.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/src/aws_cdk.aws_redshift_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:47:08.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/src/aws_cdk.aws_redshift_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-13 23:47:08.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/src/aws_cdk.aws_redshift_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:47:08.000000 aws-cdk.aws-redshift-alpha-2.84.0a0/src/aws_cdk.aws_redshift_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:01.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10773 2022-01-26 11:22:06.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9803 2022-01-26 11:22:01.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:06.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1802 2022-01-26 11:22:01.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/src/aws_cdk/aws_redshift_alpha/
+-rw-r--r--   0 root         (0) root         (0)   127876 2022-01-26 11:22:01.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/src/aws_cdk/aws_redshift_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/src/aws_cdk/aws_redshift_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      407 2022-01-26 11:22:01.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/src/aws_cdk/aws_redshift_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    99526 2022-01-26 11:22:01.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/src/aws_cdk/aws_redshift_alpha/_jsii/aws-redshift-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/src/aws_cdk/aws_redshift_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/src/aws_cdk.aws_redshift_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10773 2022-01-26 11:22:06.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/src/aws_cdk.aws_redshift_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      540 2022-01-26 11:22:06.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/src/aws_cdk.aws_redshift_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:06.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/src/aws_cdk.aws_redshift_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:06.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/src/aws_cdk.aws_redshift_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:06.000000 aws-cdk.aws-redshift-alpha-2.9.0a0/src/aws_cdk.aws_redshift_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-redshift-alpha-2.84.0a0/LICENSE` & `aws-cdk.aws-redshift-alpha-2.9.0a0/LICENSE`

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

### Comparing `aws-cdk.aws-redshift-alpha-2.84.0a0/setup.py` & `aws-cdk.aws-redshift-alpha-2.9.0a0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-redshift-alpha",
-    "version": "2.84.0.a0",
+    "version": "2.9.0.a0",
     "description": "The CDK Construct Library for AWS::Redshift",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,43 +22,41 @@
     },
     "packages": [
         "aws_cdk.aws_redshift_alpha",
         "aws_cdk.aws_redshift_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_redshift_alpha._jsii": [
-            "aws-redshift-alpha@2.84.0-alpha.0.jsii.tgz"
+            "aws-redshift-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_redshift_alpha": [
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

### Comparing `aws-cdk.aws-redshift-alpha-2.84.0a0/src/aws_cdk/aws_redshift_alpha/__init__.py` & `aws-cdk.aws-redshift-alpha-2.9.0a0/src/aws_cdk/aws_redshift_alpha/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -36,51 +36,46 @@
 By default, the master password will be generated and stored in AWS Secrets Manager.
 
 A default database named `default_db` will be created in the cluster. To change the name of this database set the `defaultDatabaseName` attribute in the constructor properties.
 
 By default, the cluster will not be publicly accessible.
 Depending on your use case, you can make the cluster publicly accessible with the `publiclyAccessible` property.
 
-## Adding a logging bucket for database audit logging to S3
+## Connecting
 
-Amazon Redshift logs information about connections and user activities in your database. These logs help you to monitor the database for security and troubleshooting purposes, a process called database auditing. To send these logs to an S3 bucket, specify the `loggingProperties` when creating a new cluster.
+To control who can access the cluster, use the `.connections` attribute. Redshift Clusters have
+a default port, so you don't need to specify the port:
 
 ```python
-import aws_cdk.aws_ec2 as ec2
-import aws_cdk.aws_s3 as s3
-
+cluster.connections.allow_default_port_from_any_ipv4("Open to the world")
+```
 
-vpc = ec2.Vpc(self, "Vpc")
-bucket = s3.Bucket.from_bucket_name(self, "bucket", "logging-bucket")
+The endpoint to access your database cluster will be available as the `.clusterEndpoint` attribute:
 
-cluster = Cluster(self, "Redshift",
-    master_user=Login(
-        master_username="admin"
-    ),
-    vpc=vpc,
-    logging_properties=LoggingProperties(
-        logging_bucket=bucket,
-        logging_key_prefix="prefix"
-    )
-)
+```python
+cluster.cluster_endpoint.socket_address
 ```
 
-## Connecting
+## Rotating credentials
 
-To control who can access the cluster, use the `.connections` attribute. Redshift Clusters have
-a default port, so you don't need to specify the port:
+When the master password is generated and stored in AWS Secrets Manager, it can be rotated automatically:
 
 ```python
-cluster.connections.allow_default_port_from_any_ipv4("Open to the world")
+cluster.add_rotation_single_user()
 ```
 
-The endpoint to access your database cluster will be available as the `.clusterEndpoint` attribute:
+The multi user rotation scheme is also available:
 
 ```python
-cluster.cluster_endpoint.socket_address
+import aws_cdk.aws_secretsmanager as secretsmanager
+
+
+cluster.add_rotation_multi_user("MyUser",
+    secret=secretsmanager.Secret.from_secret_name_v2(self, "Imported Secret", "my-secret")
+)
 ```
 
 ## Database Resources
 
 This module allows for the creation of non-CloudFormation database resources such as users
 and tables. This allows you to manage identities, permissions, and stateful resources
 within your Redshift cluster from your CDK application.
@@ -189,53 +184,14 @@
     ],
     cluster=cluster,
     database_name="databaseName",
     sort_style=TableSortStyle.COMPOUND
 )
 ```
 
-Tables and their respective columns can be configured to contain comments:
-
-```python
-Table(self, "Table",
-    table_columns=[Column(name="col1", data_type="varchar(4)", comment="This is a column comment"), Column(name="col2", data_type="float", comment="This is a another column comment")
-    ],
-    cluster=cluster,
-    database_name="databaseName",
-    table_comment="This is a table comment"
-)
-```
-
-Table columns can be configured to use a specific compression encoding:
-
-```python
-from aws_cdk.aws_redshift_alpha import ColumnEncoding
-
-
-Table(self, "Table",
-    table_columns=[Column(name="col1", data_type="varchar(4)", encoding=ColumnEncoding.TEXT32K), Column(name="col2", data_type="float", encoding=ColumnEncoding.DELTA32K)
-    ],
-    cluster=cluster,
-    database_name="databaseName"
-)
-```
-
-Table columns can also contain an `id` attribute, which can allow table columns to be renamed.
-
-**NOTE** To use the `id` attribute, you must also enable the `@aws-cdk/aws-redshift:columnId` feature flag.
-
-```python
-Table(self, "Table",
-    table_columns=[Column(id="col1", name="col1", data_type="varchar(4)"), Column(id="col2", name="col2", data_type="float")
-    ],
-    cluster=cluster,
-    database_name="databaseName"
-)
-```
-
 ### Granting Privileges
 
 You can give a user privileges to perform certain actions on a table by using the
 `Table.grant()` method.
 
 ```python
 user = User(self, "User",
@@ -281,15 +237,15 @@
 ```python
 database_name = "databaseName"
 username = "myuser"
 table_name = "mytable"
 
 user = User.from_user_attributes(self, "User",
     username=username,
-    password=SecretValue.unsafe_plain_text("NOT_FOR_PRODUCTION"),
+    password=SecretValue.plain_text("NOT_FOR_PRODUCTION"),
     cluster=cluster,
     database_name=database_name
 )
 table = Table.from_table_attributes(self, "Table",
     table_name=table_name,
     table_columns=[Column(name="col1", data_type="varchar(4)"), Column(name="col2", data_type="float")],
     cluster=cluster,
@@ -306,270 +262,34 @@
 submitted to the Redshift cluster. In general, application 1 does not know that
 application 2 has also granted this permission and thus cannot decide not to issue the
 revocation. This leads to the undesirable state where application 2 still contains the
 call to `grant` but the user does not have the specified permission.
 
 Note that this does not occur when duplicate privileges are granted within the same
 application, as such privileges are de-duplicated before any SQL query is submitted.
-
-## Rotating credentials
-
-When the master password is generated and stored in AWS Secrets Manager, it can be rotated automatically:
-
-```python
-cluster.add_rotation_single_user()
-```
-
-The multi user rotation scheme is also available:
-
-```python
-user = User(self, "User",
-    cluster=cluster,
-    database_name="databaseName"
-)
-cluster.add_rotation_multi_user("MultiUserRotation",
-    secret=user.secret
-)
-```
-
-## Adding Parameters
-
-You can add a parameter to a parameter group with`ClusterParameterGroup.addParameter()`.
-
-```python
-from aws_cdk.aws_redshift_alpha import ClusterParameterGroup
-
-
-params = ClusterParameterGroup(self, "Params",
-    description="desc",
-    parameters={
-        "require_ssl": "true"
-    }
-)
-
-params.add_parameter("enable_user_activity_logging", "true")
-```
-
-Additionally, you can add a parameter to the cluster's associated parameter group with `Cluster.addToParameterGroup()`. If the cluster does not have an associated parameter group, a new parameter group is created.
-
-```python
-import aws_cdk.aws_ec2 as ec2
-import aws_cdk as cdk
-# vpc: ec2.Vpc
-
-
-cluster = Cluster(self, "Cluster",
-    master_user=Login(
-        master_username="admin",
-        master_password=cdk.SecretValue.unsafe_plain_text("tooshort")
-    ),
-    vpc=vpc
-)
-
-cluster.add_to_parameter_group("enable_user_activity_logging", "true")
-```
-
-## Rebooting for Parameter Updates
-
-In most cases, existing clusters [must be manually rebooted](https://docs.aws.amazon.com/redshift/latest/mgmt/working-with-parameter-groups.html) to apply parameter changes. You can automate parameter related reboots by setting the cluster's `rebootForParameterChanges` property to `true` , or by using `Cluster.enableRebootForParameterChanges()`.
-
-```python
-import aws_cdk.aws_ec2 as ec2
-import aws_cdk as cdk
-# vpc: ec2.Vpc
-
-
-cluster = Cluster(self, "Cluster",
-    master_user=Login(
-        master_username="admin",
-        master_password=cdk.SecretValue.unsafe_plain_text("tooshort")
-    ),
-    vpc=vpc
-)
-
-cluster.add_to_parameter_group("enable_user_activity_logging", "true")
-cluster.enable_reboot_for_parameter_changes()
-```
-
-## Elastic IP
-
-If you configure your cluster to be publicly accessible, you can optionally select an *elastic IP address* to use for the external IP address. An elastic IP address is a static IP address that is associated with your AWS account. You can use an elastic IP address to connect to your cluster from outside the VPC. An elastic IP address gives you the ability to change your underlying configuration without affecting the IP address that clients use to connect to your cluster. This approach can be helpful for situations such as recovery after a failure.
-
-```python
-import aws_cdk.aws_ec2 as ec2
-import aws_cdk as cdk
-# vpc: ec2.Vpc
-
-
-Cluster(self, "Redshift",
-    master_user=Login(
-        master_username="admin",
-        master_password=cdk.SecretValue.unsafe_plain_text("tooshort")
-    ),
-    vpc=vpc,
-    publicly_accessible=True,
-    elastic_ip="10.123.123.255"
-)
-```
-
-If the Cluster is in a VPC and you want to connect to it using the private IP address from within the cluster, it is important to enable *DNS resolution* and *DNS hostnames* in the VPC config. If these parameters would not be set, connections from within the VPC would connect to the elastic IP address and not the private IP address.
-
-```python
-import aws_cdk.aws_ec2 as ec2
-
-vpc = ec2.Vpc(self, "VPC",
-    enable_dns_support=True,
-    enable_dns_hostnames=True
-)
-```
-
-Note that if there is already an existing, public accessible Cluster, which VPC configuration is changed to use *DNS hostnames* and *DNS resolution*, connections still use the elastic IP address until the cluster is resized.
-
-### Elastic IP vs. Cluster node public IP
-
-The elastic IP address is an external IP address for accessing the cluster outside of a VPC. It's not related to the cluster node public IP addresses and private IP addresses that are accessible via the `clusterEndpoint` property. The public and private cluster node IP addresses appear regardless of whether the cluster is publicly accessible or not. They are used only in certain circumstances to configure ingress rules on the remote host. These circumstances occur when you load data from an Amazon EC2 instance or other remote host using a Secure Shell (SSH) connection.
-
-### Attach Elastic IP after Cluster creation
-
-In some cases, you might want to associate the cluster with an elastic IP address or change an elastic IP address that is associated with the cluster. To attach an elastic IP address after the cluster is created, first update the cluster so that it is not publicly accessible, then make it both publicly accessible and add an Elastic IP address in the same operation.
-
-## Enhanced VPC Routing
-
-When you use Amazon Redshift enhanced VPC routing, Amazon Redshift forces all COPY and UNLOAD traffic between your cluster and your data repositories through your virtual private cloud (VPC) based on the Amazon VPC service. By using enhanced VPC routing, you can use standard VPC features, such as VPC security groups, network access control lists (ACLs), VPC endpoints, VPC endpoint policies, internet gateways, and Domain Name System (DNS) servers, as described in the Amazon VPC User Guide. You use these features to tightly manage the flow of data between your Amazon Redshift cluster and other resources. When you use enhanced VPC routing to route traffic through your VPC, you can also use VPC flow logs to monitor COPY and UNLOAD traffic.
-
-```python
-import aws_cdk.aws_ec2 as ec2
-import aws_cdk as cdk
-# vpc: ec2.Vpc
-
-
-Cluster(self, "Redshift",
-    master_user=Login(
-        master_username="admin",
-        master_password=cdk.SecretValue.unsafe_plain_text("tooshort")
-    ),
-    vpc=vpc,
-    enhanced_vpc_routing=True
-)
-```
-
-If enhanced VPC routing is not enabled, Amazon Redshift routes traffic through the internet, including traffic to other services within the AWS network.
-
-## Default IAM role
-
-Some Amazon Redshift features require Amazon Redshift to access other AWS services on your behalf. For your Amazon Redshift clusters to act on your behalf, you supply security credentials to your clusters. The preferred method to supply security credentials is to specify an AWS Identity and Access Management (IAM) role.
-
-When you create an IAM role and set it as the default for the cluster using console, you don't have to provide the IAM role's Amazon Resource Name (ARN) to perform authentication and authorization.
-
-```python
-import aws_cdk.aws_ec2 as ec2
-import aws_cdk.aws_iam as iam
-# vpc: ec2.Vpc
-
-
-default_role = iam.Role(self, "DefaultRole",
-    assumed_by=iam.ServicePrincipal("redshift.amazonaws.com")
-)
-
-Cluster(self, "Redshift",
-    master_user=Login(
-        master_username="admin"
-    ),
-    vpc=vpc,
-    roles=[default_role],
-    default_role=default_role
-)
-```
-
-A default role can also be added to a cluster using the `addDefaultIamRole` method.
-
-```python
-import aws_cdk.aws_ec2 as ec2
-import aws_cdk.aws_iam as iam
-# vpc: ec2.Vpc
-
-
-default_role = iam.Role(self, "DefaultRole",
-    assumed_by=iam.ServicePrincipal("redshift.amazonaws.com")
-)
-
-redshift_cluster = Cluster(self, "Redshift",
-    master_user=Login(
-        master_username="admin"
-    ),
-    vpc=vpc,
-    roles=[default_role]
-)
-
-redshift_cluster.add_default_iam_role(default_role)
-```
-
-## IAM roles
-
-Attaching IAM roles to a Redshift Cluster grants permissions to the Redshift service to perform actions on your behalf.
-
-```python
-import aws_cdk.aws_ec2 as ec2
-import aws_cdk.aws_iam as iam
-# vpc: ec2.Vpc
-
-
-role = iam.Role(self, "Role",
-    assumed_by=iam.ServicePrincipal("redshift.amazonaws.com")
-)
-cluster = Cluster(self, "Redshift",
-    master_user=Login(
-        master_username="admin"
-    ),
-    vpc=vpc,
-    roles=[role]
-)
-```
-
-Additional IAM roles can be attached to a cluster using the `addIamRole` method.
-
-```python
-import aws_cdk.aws_ec2 as ec2
-import aws_cdk.aws_iam as iam
-# vpc: ec2.Vpc
-
-
-role = iam.Role(self, "Role",
-    assumed_by=iam.ServicePrincipal("redshift.amazonaws.com")
-)
-cluster = Cluster(self, "Redshift",
-    master_user=Login(
-        master_username="admin"
-    ),
-    vpc=vpc
-)
-cluster.add_iam_role(role)
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
-import aws_cdk.aws_ec2 as _aws_cdk_aws_ec2_ceddda9d
-import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
-import aws_cdk.aws_kms as _aws_cdk_aws_kms_ceddda9d
-import aws_cdk.aws_s3 as _aws_cdk_aws_s3_ceddda9d
-import aws_cdk.aws_secretsmanager as _aws_cdk_aws_secretsmanager_ceddda9d
-import constructs as _constructs_77d1e7e8
+import aws_cdk
+import aws_cdk.aws_ec2
+import aws_cdk.aws_iam
+import aws_cdk.aws_kms
+import aws_cdk.aws_s3
+import aws_cdk.aws_secretsmanager
+import constructs
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-redshift-alpha.ClusterAttributes",
     jsii_struct_bases=[],
     name_mapping={
         "cluster_endpoint_address": "clusterEndpointAddress",
@@ -581,15 +301,15 @@
 class ClusterAttributes:
     def __init__(
         self,
         *,
         cluster_endpoint_address: builtins.str,
         cluster_endpoint_port: jsii.Number,
         cluster_name: builtins.str,
-        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+        security_groups: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.ISecurityGroup]] = None,
     ) -> None:
         '''(experimental) Properties that describe an existing cluster instance.
 
         :param cluster_endpoint_address: (experimental) Cluster endpoint address.
         :param cluster_endpoint_port: (experimental) Cluster endpoint port.
         :param cluster_name: (experimental) Identifier for the cluster.
         :param security_groups: (experimental) The security groups of the redshift cluster. Default: no security groups will be attached to the import
@@ -611,21 +331,15 @@
                 cluster_endpoint_port=123,
                 cluster_name="clusterName",
             
                 # the properties below are optional
                 security_groups=[security_group]
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__cf5e43f35a05f5c5658f39bc00260eed640e4a1a644169632c3ab77941eded83)
-            check_type(argname="argument cluster_endpoint_address", value=cluster_endpoint_address, expected_type=type_hints["cluster_endpoint_address"])
-            check_type(argname="argument cluster_endpoint_port", value=cluster_endpoint_port, expected_type=type_hints["cluster_endpoint_port"])
-            check_type(argname="argument cluster_name", value=cluster_name, expected_type=type_hints["cluster_name"])
-            check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "cluster_endpoint_address": cluster_endpoint_address,
             "cluster_endpoint_port": cluster_endpoint_port,
             "cluster_name": cluster_name,
         }
         if security_groups is not None:
             self._values["security_groups"] = security_groups
 
@@ -658,23 +372,23 @@
         result = self._values.get("cluster_name")
         assert result is not None, "Required property 'cluster_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def security_groups(
         self,
-    ) -> typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]]:
+    ) -> typing.Optional[typing.List[aws_cdk.aws_ec2.ISecurityGroup]]:
         '''(experimental) The security groups of the redshift cluster.
 
         :default: no security groups will be attached to the import
 
         :stability: experimental
         '''
         result = self._values.get("security_groups")
-        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]], result)
+        return typing.cast(typing.Optional[typing.List[aws_cdk.aws_ec2.ISecurityGroup]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -698,35 +412,32 @@
     ) -> None:
         '''(experimental) Properties for a parameter group.
 
         :param parameters: (experimental) The parameters in this parameter group.
         :param description: (experimental) Description for this parameter group. Default: a CDK generated description
 
         :stability: experimental
-        :exampleMetadata: infused
+        :exampleMetadata: fixture=_generated
 
         Example::
 
-            from aws_cdk.aws_redshift_alpha import ClusterParameterGroup
-            
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.aws_redshift_alpha as redshift_alpha
             
-            params = ClusterParameterGroup(self, "Params",
-                description="desc",
+            cluster_parameter_group_props = redshift_alpha.ClusterParameterGroupProps(
                 parameters={
-                    "require_ssl": "true"
-                }
-            )
+                    "parameters_key": "parameters"
+                },
             
-            params.add_parameter("enable_user_activity_logging", "true")
+                # the properties below are optional
+                description="description"
+            )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__cb07da80fc73b7c25808e76fda84dcebec84019d464cfe8908504bd326b69e87)
-            check_type(argname="argument parameters", value=parameters, expected_type=type_hints["parameters"])
-            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "parameters": parameters,
         }
         if description is not None:
             self._values["description"] = description
 
     @builtins.property
     def parameters(self) -> typing.Mapping[builtins.str, builtins.str]:
@@ -763,184 +474,132 @@
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-redshift-alpha.ClusterProps",
     jsii_struct_bases=[],
     name_mapping={
         "master_user": "masterUser",
         "vpc": "vpc",
-        "classic_resizing": "classicResizing",
         "cluster_name": "clusterName",
         "cluster_type": "clusterType",
         "default_database_name": "defaultDatabaseName",
-        "default_role": "defaultRole",
-        "elastic_ip": "elasticIp",
         "encrypted": "encrypted",
         "encryption_key": "encryptionKey",
-        "enhanced_vpc_routing": "enhancedVpcRouting",
-        "logging_properties": "loggingProperties",
+        "logging_bucket": "loggingBucket",
+        "logging_key_prefix": "loggingKeyPrefix",
         "node_type": "nodeType",
         "number_of_nodes": "numberOfNodes",
         "parameter_group": "parameterGroup",
         "port": "port",
         "preferred_maintenance_window": "preferredMaintenanceWindow",
         "publicly_accessible": "publiclyAccessible",
-        "reboot_for_parameter_changes": "rebootForParameterChanges",
         "removal_policy": "removalPolicy",
         "roles": "roles",
         "security_groups": "securityGroups",
         "subnet_group": "subnetGroup",
         "vpc_subnets": "vpcSubnets",
     },
 )
 class ClusterProps:
     def __init__(
         self,
         *,
-        master_user: typing.Union["Login", typing.Dict[builtins.str, typing.Any]],
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-        classic_resizing: typing.Optional[builtins.bool] = None,
+        master_user: "Login",
+        vpc: aws_cdk.aws_ec2.IVpc,
         cluster_name: typing.Optional[builtins.str] = None,
         cluster_type: typing.Optional["ClusterType"] = None,
         default_database_name: typing.Optional[builtins.str] = None,
-        default_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-        elastic_ip: typing.Optional[builtins.str] = None,
         encrypted: typing.Optional[builtins.bool] = None,
-        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-        enhanced_vpc_routing: typing.Optional[builtins.bool] = None,
-        logging_properties: typing.Optional[typing.Union["LoggingProperties", typing.Dict[builtins.str, typing.Any]]] = None,
+        encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
+        logging_bucket: typing.Optional[aws_cdk.aws_s3.IBucket] = None,
+        logging_key_prefix: typing.Optional[builtins.str] = None,
         node_type: typing.Optional["NodeType"] = None,
         number_of_nodes: typing.Optional[jsii.Number] = None,
         parameter_group: typing.Optional["IClusterParameterGroup"] = None,
         port: typing.Optional[jsii.Number] = None,
         preferred_maintenance_window: typing.Optional[builtins.str] = None,
         publicly_accessible: typing.Optional[builtins.bool] = None,
-        reboot_for_parameter_changes: typing.Optional[builtins.bool] = None,
-        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-        roles: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.IRole]] = None,
-        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+        removal_policy: typing.Optional[aws_cdk.RemovalPolicy] = None,
+        roles: typing.Optional[typing.Sequence[aws_cdk.aws_iam.IRole]] = None,
+        security_groups: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.ISecurityGroup]] = None,
         subnet_group: typing.Optional["IClusterSubnetGroup"] = None,
-        vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        vpc_subnets: typing.Optional[aws_cdk.aws_ec2.SubnetSelection] = None,
     ) -> None:
         '''(experimental) Properties for a new database cluster.
 
         :param master_user: (experimental) Username and password for the administrative user.
         :param vpc: (experimental) The VPC to place the cluster in.
-        :param classic_resizing: (experimental) If this flag is set, the cluster resizing type will be set to classic. When resizing a cluster, classic resizing will always provision a new cluster and transfer the data there. Classic resize takes more time to complete, but it can be useful in cases where the change in node count or the node type to migrate to doesn't fall within the bounds for elastic resize. Default: - Elastic resize type
         :param cluster_name: (experimental) An optional identifier for the cluster. Default: - A name is automatically generated.
-        :param cluster_type: (experimental) Settings for the individual instances that are launched. Default: ``ClusterType.MULTI_NODE``
+        :param cluster_type: (experimental) Settings for the individual instances that are launched. Default: {@link ClusterType.MULTI_NODE}
         :param default_database_name: (experimental) Name of a database which is automatically created inside the cluster. Default: - default_db
-        :param default_role: (experimental) A single AWS Identity and Access Management (IAM) role to be used as the default role for the cluster. The default role must be included in the roles list. Default: - No default role is specified for the cluster.
-        :param elastic_ip: (experimental) The Elastic IP (EIP) address for the cluster. Default: - No Elastic IP
         :param encrypted: (experimental) Whether to enable encryption of data at rest in the cluster. Default: true
         :param encryption_key: (experimental) The KMS key to use for encryption of data at rest. Default: - AWS-managed key, if encryption at rest is enabled
-        :param enhanced_vpc_routing: (experimental) If this flag is set, Amazon Redshift forces all COPY and UNLOAD traffic between your cluster and your data repositories through your virtual private cloud (VPC). Default: - false
-        :param logging_properties: (experimental) Bucket details for log files to be sent to, including prefix. Default: - No logging bucket is used
-        :param node_type: (experimental) The node type to be provisioned for the cluster. Default: ``NodeType.DC2_LARGE``
+        :param logging_bucket: (experimental) Bucket to send logs to. Logging information includes queries and connection attempts, for the specified Amazon Redshift cluster. Default: - No Logs
+        :param logging_key_prefix: (experimental) Prefix used for logging. Default: - no prefix
+        :param node_type: (experimental) The node type to be provisioned for the cluster. Default: {@link NodeType.DC2_LARGE}
         :param number_of_nodes: (experimental) Number of compute nodes in the cluster. Only specify this property for multi-node clusters. Value must be at least 2 and no more than 100. Default: - 2 if ``clusterType`` is ClusterType.MULTI_NODE, undefined otherwise
         :param parameter_group: (experimental) Additional parameters to pass to the database engine https://docs.aws.amazon.com/redshift/latest/mgmt/working-with-parameter-groups.html. Default: - No parameter group.
         :param port: (experimental) What port to listen on. Default: - The default for the engine is used.
         :param preferred_maintenance_window: (experimental) A preferred maintenance window day/time range. Should be specified as a range ddd:hh24:mi-ddd:hh24:mi (24H Clock UTC). Example: 'Sun:23:45-Mon:00:15' Default: - 30-minute window selected at random from an 8-hour block of time for each AWS Region, occurring on a random day of the week.
         :param publicly_accessible: (experimental) Whether to make cluster publicly accessible. Default: false
-        :param reboot_for_parameter_changes: (experimental) If this flag is set, the cluster will be rebooted when changes to the cluster's parameter group that require a restart to apply. Default: false
         :param removal_policy: (experimental) The removal policy to apply when the cluster and its instances are removed from the stack or replaced during an update. Default: RemovalPolicy.RETAIN
-        :param roles: (experimental) A list of AWS Identity and Access Management (IAM) role that can be used by the cluster to access other AWS services. The maximum number of roles to attach to a cluster is subject to a quota. Default: - No role is attached to the cluster.
+        :param roles: (experimental) A list of AWS Identity and Access Management (IAM) role that can be used by the cluster to access other AWS services. Specify a maximum of 10 roles. Default: - No role is attached to the cluster.
         :param security_groups: (experimental) Security group. Default: - a new security group is created.
         :param subnet_group: (experimental) A cluster subnet group to use with this cluster. Default: - a new subnet group will be created.
         :param vpc_subnets: (experimental) Where to place the instances within the VPC. Default: - private subnets
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
             import aws_cdk.aws_ec2 as ec2
-            import aws_cdk as cdk
-            # vpc: ec2.Vpc
             
             
-            cluster = Cluster(self, "Cluster",
+            vpc = ec2.Vpc(self, "Vpc")
+            cluster = Cluster(self, "Redshift",
                 master_user=Login(
-                    master_username="admin",
-                    master_password=cdk.SecretValue.unsafe_plain_text("tooshort")
+                    master_username="admin"
                 ),
                 vpc=vpc
             )
-            
-            cluster.add_to_parameter_group("enable_user_activity_logging", "true")
         '''
         if isinstance(master_user, dict):
             master_user = Login(**master_user)
-        if isinstance(logging_properties, dict):
-            logging_properties = LoggingProperties(**logging_properties)
         if isinstance(vpc_subnets, dict):
-            vpc_subnets = _aws_cdk_aws_ec2_ceddda9d.SubnetSelection(**vpc_subnets)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8184b6f381b827fb337da7fe46dcdf07d3411d00c00a966acf72f7524193e365)
-            check_type(argname="argument master_user", value=master_user, expected_type=type_hints["master_user"])
-            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
-            check_type(argname="argument classic_resizing", value=classic_resizing, expected_type=type_hints["classic_resizing"])
-            check_type(argname="argument cluster_name", value=cluster_name, expected_type=type_hints["cluster_name"])
-            check_type(argname="argument cluster_type", value=cluster_type, expected_type=type_hints["cluster_type"])
-            check_type(argname="argument default_database_name", value=default_database_name, expected_type=type_hints["default_database_name"])
-            check_type(argname="argument default_role", value=default_role, expected_type=type_hints["default_role"])
-            check_type(argname="argument elastic_ip", value=elastic_ip, expected_type=type_hints["elastic_ip"])
-            check_type(argname="argument encrypted", value=encrypted, expected_type=type_hints["encrypted"])
-            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
-            check_type(argname="argument enhanced_vpc_routing", value=enhanced_vpc_routing, expected_type=type_hints["enhanced_vpc_routing"])
-            check_type(argname="argument logging_properties", value=logging_properties, expected_type=type_hints["logging_properties"])
-            check_type(argname="argument node_type", value=node_type, expected_type=type_hints["node_type"])
-            check_type(argname="argument number_of_nodes", value=number_of_nodes, expected_type=type_hints["number_of_nodes"])
-            check_type(argname="argument parameter_group", value=parameter_group, expected_type=type_hints["parameter_group"])
-            check_type(argname="argument port", value=port, expected_type=type_hints["port"])
-            check_type(argname="argument preferred_maintenance_window", value=preferred_maintenance_window, expected_type=type_hints["preferred_maintenance_window"])
-            check_type(argname="argument publicly_accessible", value=publicly_accessible, expected_type=type_hints["publicly_accessible"])
-            check_type(argname="argument reboot_for_parameter_changes", value=reboot_for_parameter_changes, expected_type=type_hints["reboot_for_parameter_changes"])
-            check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
-            check_type(argname="argument roles", value=roles, expected_type=type_hints["roles"])
-            check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
-            check_type(argname="argument subnet_group", value=subnet_group, expected_type=type_hints["subnet_group"])
-            check_type(argname="argument vpc_subnets", value=vpc_subnets, expected_type=type_hints["vpc_subnets"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+            vpc_subnets = aws_cdk.aws_ec2.SubnetSelection(**vpc_subnets)
+        self._values: typing.Dict[str, typing.Any] = {
             "master_user": master_user,
             "vpc": vpc,
         }
-        if classic_resizing is not None:
-            self._values["classic_resizing"] = classic_resizing
         if cluster_name is not None:
             self._values["cluster_name"] = cluster_name
         if cluster_type is not None:
             self._values["cluster_type"] = cluster_type
         if default_database_name is not None:
             self._values["default_database_name"] = default_database_name
-        if default_role is not None:
-            self._values["default_role"] = default_role
-        if elastic_ip is not None:
-            self._values["elastic_ip"] = elastic_ip
         if encrypted is not None:
             self._values["encrypted"] = encrypted
         if encryption_key is not None:
             self._values["encryption_key"] = encryption_key
-        if enhanced_vpc_routing is not None:
-            self._values["enhanced_vpc_routing"] = enhanced_vpc_routing
-        if logging_properties is not None:
-            self._values["logging_properties"] = logging_properties
+        if logging_bucket is not None:
+            self._values["logging_bucket"] = logging_bucket
+        if logging_key_prefix is not None:
+            self._values["logging_key_prefix"] = logging_key_prefix
         if node_type is not None:
             self._values["node_type"] = node_type
         if number_of_nodes is not None:
             self._values["number_of_nodes"] = number_of_nodes
         if parameter_group is not None:
             self._values["parameter_group"] = parameter_group
         if port is not None:
             self._values["port"] = port
         if preferred_maintenance_window is not None:
             self._values["preferred_maintenance_window"] = preferred_maintenance_window
         if publicly_accessible is not None:
             self._values["publicly_accessible"] = publicly_accessible
-        if reboot_for_parameter_changes is not None:
-            self._values["reboot_for_parameter_changes"] = reboot_for_parameter_changes
         if removal_policy is not None:
             self._values["removal_policy"] = removal_policy
         if roles is not None:
             self._values["roles"] = roles
         if security_groups is not None:
             self._values["security_groups"] = security_groups
         if subnet_group is not None:
@@ -955,39 +614,22 @@
         :stability: experimental
         '''
         result = self._values.get("master_user")
         assert result is not None, "Required property 'master_user' is missing"
         return typing.cast("Login", result)
 
     @builtins.property
-    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
+    def vpc(self) -> aws_cdk.aws_ec2.IVpc:
         '''(experimental) The VPC to place the cluster in.
 
         :stability: experimental
         '''
         result = self._values.get("vpc")
         assert result is not None, "Required property 'vpc' is missing"
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, result)
-
-    @builtins.property
-    def classic_resizing(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) If this flag is set, the cluster resizing type will be set to classic.
-
-        When resizing a cluster, classic resizing will always provision a new cluster and transfer the data there.
-
-        Classic resize takes more time to complete, but it can be useful in cases where the change in node count or
-        the node type to migrate to doesn't fall within the bounds for elastic resize.
-
-        :default: - Elastic resize type
-
-        :see: https://docs.aws.amazon.com/redshift/latest/mgmt/managing-cluster-operations.html#elastic-resize
-        :stability: experimental
-        '''
-        result = self._values.get("classic_resizing")
-        return typing.cast(typing.Optional[builtins.bool], result)
+        return typing.cast(aws_cdk.aws_ec2.IVpc, result)
 
     @builtins.property
     def cluster_name(self) -> typing.Optional[builtins.str]:
         '''(experimental) An optional identifier for the cluster.
 
         :default: - A name is automatically generated.
 
@@ -996,15 +638,15 @@
         result = self._values.get("cluster_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def cluster_type(self) -> typing.Optional["ClusterType"]:
         '''(experimental) Settings for the individual instances that are launched.
 
-        :default: ``ClusterType.MULTI_NODE``
+        :default: {@link ClusterType.MULTI_NODE}
 
         :stability: experimental
         '''
         result = self._values.get("cluster_type")
         return typing.cast(typing.Optional["ClusterType"], result)
 
     @builtins.property
@@ -1015,88 +657,64 @@
 
         :stability: experimental
         '''
         result = self._values.get("default_database_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def default_role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
-        '''(experimental) A single AWS Identity and Access Management (IAM) role to be used as the default role for the cluster.
-
-        The default role must be included in the roles list.
-
-        :default: - No default role is specified for the cluster.
-
-        :stability: experimental
-        '''
-        result = self._values.get("default_role")
-        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
-
-    @builtins.property
-    def elastic_ip(self) -> typing.Optional[builtins.str]:
-        '''(experimental) The Elastic IP (EIP) address for the cluster.
-
-        :default: - No Elastic IP
-
-        :see: https://docs.aws.amazon.com/redshift/latest/mgmt/managing-clusters-vpc.html
-        :stability: experimental
-        '''
-        result = self._values.get("elastic_ip")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
     def encrypted(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Whether to enable encryption of data at rest in the cluster.
 
         :default: true
 
         :stability: experimental
         '''
         result = self._values.get("encrypted")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def encryption_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def encryption_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) The KMS key to use for encryption of data at rest.
 
         :default: - AWS-managed key, if encryption at rest is enabled
 
         :stability: experimental
         '''
         result = self._values.get("encryption_key")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], result)
 
     @builtins.property
-    def enhanced_vpc_routing(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) If this flag is set, Amazon Redshift forces all COPY and UNLOAD traffic between your cluster and your data repositories through your virtual private cloud (VPC).
+    def logging_bucket(self) -> typing.Optional[aws_cdk.aws_s3.IBucket]:
+        '''(experimental) Bucket to send logs to.
+
+        Logging information includes queries and connection attempts, for the specified Amazon Redshift cluster.
 
-        :default: - false
+        :default: - No Logs
 
-        :see: https://docs.aws.amazon.com/redshift/latest/mgmt/enhanced-vpc-routing.html
         :stability: experimental
         '''
-        result = self._values.get("enhanced_vpc_routing")
-        return typing.cast(typing.Optional[builtins.bool], result)
+        result = self._values.get("logging_bucket")
+        return typing.cast(typing.Optional[aws_cdk.aws_s3.IBucket], result)
 
     @builtins.property
-    def logging_properties(self) -> typing.Optional["LoggingProperties"]:
-        '''(experimental) Bucket details for log files to be sent to, including prefix.
+    def logging_key_prefix(self) -> typing.Optional[builtins.str]:
+        '''(experimental) Prefix used for logging.
 
-        :default: - No logging bucket is used
+        :default: - no prefix
 
         :stability: experimental
         '''
-        result = self._values.get("logging_properties")
-        return typing.cast(typing.Optional["LoggingProperties"], result)
+        result = self._values.get("logging_key_prefix")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def node_type(self) -> typing.Optional["NodeType"]:
         '''(experimental) The node type to be provisioned for the cluster.
 
-        :default: ``NodeType.DC2_LARGE``
+        :default: {@link NodeType.DC2_LARGE}
 
         :stability: experimental
         '''
         result = self._values.get("node_type")
         return typing.cast(typing.Optional["NodeType"], result)
 
     @builtins.property
@@ -1159,82 +777,71 @@
 
         :stability: experimental
         '''
         result = self._values.get("publicly_accessible")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def reboot_for_parameter_changes(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) If this flag is set, the cluster will be rebooted when changes to the cluster's parameter group that require a restart to apply.
-
-        :default: false
-
-        :stability: experimental
-        '''
-        result = self._values.get("reboot_for_parameter_changes")
-        return typing.cast(typing.Optional[builtins.bool], result)
-
-    @builtins.property
-    def removal_policy(self) -> typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy]:
+    def removal_policy(self) -> typing.Optional[aws_cdk.RemovalPolicy]:
         '''(experimental) The removal policy to apply when the cluster and its instances are removed from the stack or replaced during an update.
 
         :default: RemovalPolicy.RETAIN
 
         :stability: experimental
         '''
         result = self._values.get("removal_policy")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy], result)
+        return typing.cast(typing.Optional[aws_cdk.RemovalPolicy], result)
 
     @builtins.property
-    def roles(self) -> typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.IRole]]:
+    def roles(self) -> typing.Optional[typing.List[aws_cdk.aws_iam.IRole]]:
         '''(experimental) A list of AWS Identity and Access Management (IAM) role that can be used by the cluster to access other AWS services.
 
-        The maximum number of roles to attach to a cluster is subject to a quota.
+        Specify a maximum of 10 roles.
 
         :default: - No role is attached to the cluster.
 
         :stability: experimental
         '''
         result = self._values.get("roles")
-        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.IRole]], result)
+        return typing.cast(typing.Optional[typing.List[aws_cdk.aws_iam.IRole]], result)
 
     @builtins.property
     def security_groups(
         self,
-    ) -> typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]]:
+    ) -> typing.Optional[typing.List[aws_cdk.aws_ec2.ISecurityGroup]]:
         '''(experimental) Security group.
 
         :default: - a new security group is created.
 
         :stability: experimental
         '''
         result = self._values.get("security_groups")
-        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]], result)
+        return typing.cast(typing.Optional[typing.List[aws_cdk.aws_ec2.ISecurityGroup]], result)
 
     @builtins.property
     def subnet_group(self) -> typing.Optional["IClusterSubnetGroup"]:
         '''(experimental) A cluster subnet group to use with this cluster.
 
         :default: - a new subnet group will be created.
 
         :stability: experimental
         '''
         result = self._values.get("subnet_group")
         return typing.cast(typing.Optional["IClusterSubnetGroup"], result)
 
     @builtins.property
-    def vpc_subnets(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection]:
+    def vpc_subnets(self) -> typing.Optional[aws_cdk.aws_ec2.SubnetSelection]:
         '''(experimental) Where to place the instances within the VPC.
 
         :default: - private subnets
 
         :stability: experimental
         '''
         result = self._values.get("vpc_subnets")
-        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_ec2.SubnetSelection], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -1255,17 +862,17 @@
     },
 )
 class ClusterSubnetGroupProps:
     def __init__(
         self,
         *,
         description: builtins.str,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-        vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        vpc: aws_cdk.aws_ec2.IVpc,
+        removal_policy: typing.Optional[aws_cdk.RemovalPolicy] = None,
+        vpc_subnets: typing.Optional[aws_cdk.aws_ec2.SubnetSelection] = None,
     ) -> None:
         '''(experimental) Properties for creating a ClusterSubnetGroup.
 
         :param description: (experimental) Description of the subnet group.
         :param vpc: (experimental) The VPC to place the subnet group in.
         :param removal_policy: (experimental) The removal policy to apply when the subnet group are removed from the stack or replaced during an update. Default: RemovalPolicy.RETAIN
         :param vpc_subnets: (experimental) Which subnets within the VPC to associate with this group. Default: - private subnets
@@ -1298,22 +905,16 @@
                     subnet_group_name="subnetGroupName",
                     subnets=[subnet],
                     subnet_type=ec2.SubnetType.PRIVATE_ISOLATED
                 )
             )
         '''
         if isinstance(vpc_subnets, dict):
-            vpc_subnets = _aws_cdk_aws_ec2_ceddda9d.SubnetSelection(**vpc_subnets)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d4e8f5beb5d0b96f6d62d9dc9f2e62c24bedea9a666fc29101e682e182fb215a)
-            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
-            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
-            check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
-            check_type(argname="argument vpc_subnets", value=vpc_subnets, expected_type=type_hints["vpc_subnets"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+            vpc_subnets = aws_cdk.aws_ec2.SubnetSelection(**vpc_subnets)
+        self._values: typing.Dict[str, typing.Any] = {
             "description": description,
             "vpc": vpc,
         }
         if removal_policy is not None:
             self._values["removal_policy"] = removal_policy
         if vpc_subnets is not None:
             self._values["vpc_subnets"] = vpc_subnets
@@ -1325,44 +926,44 @@
         :stability: experimental
         '''
         result = self._values.get("description")
         assert result is not None, "Required property 'description' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
+    def vpc(self) -> aws_cdk.aws_ec2.IVpc:
         '''(experimental) The VPC to place the subnet group in.
 
         :stability: experimental
         '''
         result = self._values.get("vpc")
         assert result is not None, "Required property 'vpc' is missing"
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, result)
+        return typing.cast(aws_cdk.aws_ec2.IVpc, result)
 
     @builtins.property
-    def removal_policy(self) -> typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy]:
+    def removal_policy(self) -> typing.Optional[aws_cdk.RemovalPolicy]:
         '''(experimental) The removal policy to apply when the subnet group are removed from the stack or replaced during an update.
 
         :default: RemovalPolicy.RETAIN
 
         :stability: experimental
         '''
         result = self._values.get("removal_policy")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy], result)
+        return typing.cast(typing.Optional[aws_cdk.RemovalPolicy], result)
 
     @builtins.property
-    def vpc_subnets(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection]:
+    def vpc_subnets(self) -> typing.Optional[aws_cdk.aws_ec2.SubnetSelection]:
         '''(experimental) Which subnets within the VPC to associate with this group.
 
         :default: - private subnets
 
         :stability: experimental
         '''
         result = self._values.get("vpc_subnets")
-        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_ec2.SubnetSelection], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -1372,64 +973,55 @@
         )
 
 
 @jsii.enum(jsii_type="@aws-cdk/aws-redshift-alpha.ClusterType")
 class ClusterType(enum.Enum):
     '''(experimental) What cluster type to use.
 
-    Used by ``ClusterProps.clusterType``
+    Used by {@link ClusterProps.clusterType}
 
     :stability: experimental
     '''
 
     SINGLE_NODE = "SINGLE_NODE"
-    '''(experimental) single-node cluster, the ``ClusterProps.numberOfNodes`` parameter is not required.
+    '''(experimental) single-node cluster, the {@link ClusterProps.numberOfNodes} parameter is not required.
 
     :stability: experimental
     '''
     MULTI_NODE = "MULTI_NODE"
-    '''(experimental) multi-node cluster, set the amount of nodes using ``ClusterProps.numberOfNodes`` parameter.
+    '''(experimental) multi-node cluster, set the amount of nodes using {@link ClusterProps.numberOfNodes} parameter.
 
     :stability: experimental
     '''
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-redshift-alpha.Column",
     jsii_struct_bases=[],
     name_mapping={
         "data_type": "dataType",
         "name": "name",
-        "comment": "comment",
         "dist_key": "distKey",
-        "encoding": "encoding",
-        "id": "id",
         "sort_key": "sortKey",
     },
 )
 class Column:
     def __init__(
         self,
         *,
         data_type: builtins.str,
         name: builtins.str,
-        comment: typing.Optional[builtins.str] = None,
         dist_key: typing.Optional[builtins.bool] = None,
-        encoding: typing.Optional["ColumnEncoding"] = None,
-        id: typing.Optional[builtins.str] = None,
         sort_key: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''(experimental) A column in a Redshift table.
 
         :param data_type: (experimental) The data type of the column.
-        :param name: (experimental) The name of the column. This will appear on Amazon Redshift.
-        :param comment: (experimental) A comment to attach to the column. Default: - no comment
+        :param name: (experimental) The name of the column.
         :param dist_key: (experimental) Boolean value that indicates whether the column is to be configured as DISTKEY. Default: - column is not DISTKEY
-        :param encoding: (experimental) The encoding to use for the column. Default: - Amazon Redshift determines the encoding based on the data type.
-        :param id: (experimental) The unique identifier of the column. This is not the name of the column, and renaming this identifier will cause a new column to be created and the old column to be dropped. **NOTE** - This field will be set, however, only by setting the ``@aws-cdk/aws-redshift:columnId`` feature flag will this field be used. Default: - the column name is used as the identifier
         :param sort_key: (experimental) Boolean value that indicates whether the column is to be configured as SORTKEY. Default: - column is not a SORTKEY
 
         :stability: experimental
         :exampleMetadata: fixture=_generated
 
         Example::
 
@@ -1438,42 +1030,24 @@
             import aws_cdk.aws_redshift_alpha as redshift_alpha
             
             column = redshift_alpha.Column(
                 data_type="dataType",
                 name="name",
             
                 # the properties below are optional
-                comment="comment",
                 dist_key=False,
-                encoding=redshift_alpha.ColumnEncoding.AUTO,
-                id="id",
                 sort_key=False
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__32216f4dee559bc797af2f48171aa04cf72e7a5ff7495657331f2098b799968d)
-            check_type(argname="argument data_type", value=data_type, expected_type=type_hints["data_type"])
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
-            check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
-            check_type(argname="argument dist_key", value=dist_key, expected_type=type_hints["dist_key"])
-            check_type(argname="argument encoding", value=encoding, expected_type=type_hints["encoding"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument sort_key", value=sort_key, expected_type=type_hints["sort_key"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "data_type": data_type,
             "name": name,
         }
-        if comment is not None:
-            self._values["comment"] = comment
         if dist_key is not None:
             self._values["dist_key"] = dist_key
-        if encoding is not None:
-            self._values["encoding"] = encoding
-        if id is not None:
-            self._values["id"] = id
         if sort_key is not None:
             self._values["sort_key"] = sort_key
 
     @builtins.property
     def data_type(self) -> builtins.str:
         '''(experimental) The data type of the column.
 
@@ -1483,71 +1057,32 @@
         assert result is not None, "Required property 'data_type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''(experimental) The name of the column.
 
-        This will appear on Amazon Redshift.
-
         :stability: experimental
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def comment(self) -> typing.Optional[builtins.str]:
-        '''(experimental) A comment to attach to the column.
-
-        :default: - no comment
-
-        :stability: experimental
-        '''
-        result = self._values.get("comment")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
     def dist_key(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Boolean value that indicates whether the column is to be configured as DISTKEY.
 
         :default: - column is not DISTKEY
 
         :stability: experimental
         '''
         result = self._values.get("dist_key")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def encoding(self) -> typing.Optional["ColumnEncoding"]:
-        '''(experimental) The encoding to use for the column.
-
-        :default: - Amazon Redshift determines the encoding based on the data type.
-
-        :stability: experimental
-        '''
-        result = self._values.get("encoding")
-        return typing.cast(typing.Optional["ColumnEncoding"], result)
-
-    @builtins.property
-    def id(self) -> typing.Optional[builtins.str]:
-        '''(experimental) The unique identifier of the column.
-
-        This is not the name of the column, and renaming this identifier will cause a new column to be created and the old column to be dropped.
-
-        **NOTE** - This field will be set, however, only by setting the ``@aws-cdk/aws-redshift:columnId`` feature flag will this field be used.
-
-        :default: - the column name is used as the identifier
-
-        :stability: experimental
-        '''
-        result = self._values.get("id")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
     def sort_key(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Boolean value that indicates whether the column is to be configured as SORTKEY.
 
         :default: - column is not a SORTKEY
 
         :stability: experimental
         '''
@@ -1562,132 +1097,14 @@
 
     def __repr__(self) -> str:
         return "Column(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-@jsii.enum(jsii_type="@aws-cdk/aws-redshift-alpha.ColumnEncoding")
-class ColumnEncoding(enum.Enum):
-    '''(experimental) The compression encoding of a column.
-
-    :see: https://docs.aws.amazon.com/redshift/latest/dg/c_Compression_encodings.html
-    :stability: experimental
-    :exampleMetadata: fixture=cluster infused
-
-    Example::
-
-        from aws_cdk.aws_redshift_alpha import ColumnEncoding
-        
-        
-        Table(self, "Table",
-            table_columns=[Column(name="col1", data_type="varchar(4)", encoding=ColumnEncoding.TEXT32K), Column(name="col2", data_type="float", encoding=ColumnEncoding.DELTA32K)
-            ],
-            cluster=cluster,
-            database_name="databaseName"
-        )
-    '''
-
-    AUTO = "AUTO"
-    '''(experimental) Amazon Redshift assigns an optimal encoding based on the column data.
-
-    This is the default.
-
-    :stability: experimental
-    '''
-    RAW = "RAW"
-    '''(experimental) The column is not compressed.
-
-    :see: https://docs.aws.amazon.com/redshift/latest/dg/c_Raw_encoding.html
-    :stability: experimental
-    '''
-    AZ64 = "AZ64"
-    '''(experimental) The column is compressed using the AZ64 algorithm.
-
-    :see: https://docs.aws.amazon.com/redshift/latest/dg/az64-encoding.html
-    :stability: experimental
-    '''
-    BYTEDICT = "BYTEDICT"
-    '''(experimental) The column is compressed using a separate dictionary for each block column value on disk.
-
-    :see: https://docs.aws.amazon.com/redshift/latest/dg/c_Byte_dictionary_encoding.html
-    :stability: experimental
-    '''
-    DELTA = "DELTA"
-    '''(experimental) The column is compressed based on the difference between values in the column.
-
-    This records differences as 1-byte values.
-
-    :see: https://docs.aws.amazon.com/redshift/latest/dg/c_Delta_encoding.html
-    :stability: experimental
-    '''
-    DELTA32K = "DELTA32K"
-    '''(experimental) The column is compressed based on the difference between values in the column.
-
-    This records differences as 2-byte values.
-
-    :see: https://docs.aws.amazon.com/redshift/latest/dg/c_Delta_encoding.html
-    :stability: experimental
-    '''
-    LZO = "LZO"
-    '''(experimental) The column is compressed using the LZO algorithm.
-
-    :see: https://docs.aws.amazon.com/redshift/latest/dg/lzo-encoding.html
-    :stability: experimental
-    '''
-    MOSTLY8 = "MOSTLY8"
-    '''(experimental) The column is compressed to a smaller storage size than the original data type.
-
-    The compressed storage size is 1 byte.
-
-    :see: https://docs.aws.amazon.com/redshift/latest/dg/c_MostlyN_encoding.html
-    :stability: experimental
-    '''
-    MOSTLY16 = "MOSTLY16"
-    '''(experimental) The column is compressed to a smaller storage size than the original data type.
-
-    The compressed storage size is 2 bytes.
-
-    :see: https://docs.aws.amazon.com/redshift/latest/dg/c_MostlyN_encoding.html
-    :stability: experimental
-    '''
-    MOSTLY32 = "MOSTLY32"
-    '''(experimental) The column is compressed to a smaller storage size than the original data type.
-
-    The compressed storage size is 4 bytes.
-
-    :see: https://docs.aws.amazon.com/redshift/latest/dg/c_MostlyN_encoding.html
-    :stability: experimental
-    '''
-    RUNLENGTH = "RUNLENGTH"
-    '''(experimental) The column is compressed by recording the number of occurrences of each value in the column.
-
-    :see: https://docs.aws.amazon.com/redshift/latest/dg/c_Runlength_encoding.html
-    :stability: experimental
-    '''
-    TEXT255 = "TEXT255"
-    '''(experimental) The column is compressed by recording the first 245 unique words and then using a 1-byte index to represent each word.
-
-    :see: https://docs.aws.amazon.com/redshift/latest/dg/c_Text255_encoding.html
-    :stability: experimental
-    '''
-    TEXT32K = "TEXT32K"
-    '''(experimental) The column is compressed by recording the first 32K unique words and then using a 2-byte index to represent each word.
-
-    :see: https://docs.aws.amazon.com/redshift/latest/dg/c_Text255_encoding.html
-    :stability: experimental
-    '''
-    ZSTD = "ZSTD"
-    '''(experimental) The column is compressed using the ZSTD algorithm.
-
-    :see: https://docs.aws.amazon.com/redshift/latest/dg/zstd-encoding.html
-    :stability: experimental
-    '''
-
-
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-redshift-alpha.DatabaseOptions",
     jsii_struct_bases=[],
     name_mapping={
         "cluster": "cluster",
         "database_name": "databaseName",
         "admin_user": "adminUser",
@@ -1695,15 +1112,15 @@
 )
 class DatabaseOptions:
     def __init__(
         self,
         *,
         cluster: "ICluster",
         database_name: builtins.str,
-        admin_user: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
+        admin_user: typing.Optional[aws_cdk.aws_secretsmanager.ISecret] = None,
     ) -> None:
         '''(experimental) Properties for accessing a Redshift database.
 
         :param cluster: (experimental) The cluster containing the database.
         :param database_name: (experimental) The name of the database.
         :param admin_user: (experimental) The secret containing credentials to a Redshift user with administrator privileges. Secret JSON schema: ``{ username: string; password: string }``. Default: - the admin secret is taken from the cluster
 
@@ -1724,20 +1141,15 @@
                 cluster=cluster,
                 database_name="databaseName",
             
                 # the properties below are optional
                 admin_user=secret
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6fe4c22044df6e55f8af7e726bd1ff39590ed6b0ad6f13efc5dcf977502c0b7b)
-            check_type(argname="argument cluster", value=cluster, expected_type=type_hints["cluster"])
-            check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
-            check_type(argname="argument admin_user", value=admin_user, expected_type=type_hints["admin_user"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "cluster": cluster,
             "database_name": database_name,
         }
         if admin_user is not None:
             self._values["admin_user"] = admin_user
 
     @builtins.property
@@ -1757,42 +1169,40 @@
         :stability: experimental
         '''
         result = self._values.get("database_name")
         assert result is not None, "Required property 'database_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def admin_user(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret]:
+    def admin_user(self) -> typing.Optional[aws_cdk.aws_secretsmanager.ISecret]:
         '''(experimental) The secret containing credentials to a Redshift user with administrator privileges.
 
         Secret JSON schema: ``{ username: string; password: string }``.
 
         :default: - the admin secret is taken from the cluster
 
         :stability: experimental
         '''
         result = self._values.get("admin_user")
-        return typing.cast(typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_secretsmanager.ISecret], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
         return "DatabaseOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 class DatabaseSecret(
-    _aws_cdk_aws_secretsmanager_ceddda9d.Secret,
+    aws_cdk.aws_secretsmanager.Secret,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-redshift-alpha.DatabaseSecret",
 ):
     '''(experimental) A database secret.
 
     :stability: experimental
     :resource: AWS::SecretsManager::Secret
@@ -1813,32 +1223,28 @@
             # the properties below are optional
             encryption_key=key
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         username: builtins.str,
-        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param username: (experimental) The username.
         :param encryption_key: (experimental) The KMS key to use to encrypt the secret. Default: default master key
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__984b48cb3b4940dc6b6d9cdce4c356224668b8a25e815f08a9d2475010ddc7f7)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = DatabaseSecretProps(username=username, encryption_key=encryption_key)
 
         jsii.create(self.__class__, self, [scope, id, props])
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-redshift-alpha.DatabaseSecretProps",
@@ -1846,15 +1252,15 @@
     name_mapping={"username": "username", "encryption_key": "encryptionKey"},
 )
 class DatabaseSecretProps:
     def __init__(
         self,
         *,
         username: builtins.str,
-        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
     ) -> None:
         '''(experimental) Construction properties for a DatabaseSecret.
 
         :param username: (experimental) The username.
         :param encryption_key: (experimental) The KMS key to use to encrypt the secret. Default: default master key
 
         :stability: experimental
@@ -1872,19 +1278,15 @@
             database_secret_props = redshift_alpha.DatabaseSecretProps(
                 username="username",
             
                 # the properties below are optional
                 encryption_key=key
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6c5db30f831b907067d91296ccc68bfe4767f2efe09ae877fe203adb5df73e42)
-            check_type(argname="argument username", value=username, expected_type=type_hints["username"])
-            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "username": username,
         }
         if encryption_key is not None:
             self._values["encryption_key"] = encryption_key
 
     @builtins.property
     def username(self) -> builtins.str:
@@ -1893,23 +1295,23 @@
         :stability: experimental
         '''
         result = self._values.get("username")
         assert result is not None, "Required property 'username' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def encryption_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def encryption_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) The KMS key to use to encrypt the secret.
 
         :default: default master key
 
         :stability: experimental
         '''
         result = self._values.get("encryption_key")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -1942,240 +1344,236 @@
     def __init__(self, address: builtins.str, port: jsii.Number) -> None:
         '''
         :param address: -
         :param port: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9156a39d8268aff7d98d3e261bceea1730546d85f7f12d19efdada7e91b09890)
-            check_type(argname="argument address", value=address, expected_type=type_hints["address"])
-            check_type(argname="argument port", value=port, expected_type=type_hints["port"])
         jsii.create(self.__class__, self, [address, port])
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="hostname")
     def hostname(self) -> builtins.str:
         '''(experimental) The hostname of the endpoint.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "hostname"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="port")
     def port(self) -> jsii.Number:
         '''(experimental) The port of the endpoint.
 
         :stability: experimental
         '''
         return typing.cast(jsii.Number, jsii.get(self, "port"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="socketAddress")
     def socket_address(self) -> builtins.str:
         '''(experimental) The combination of "HOSTNAME:PORT" for this endpoint.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "socketAddress"))
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-redshift-alpha.ICluster")
 class ICluster(
-    _aws_cdk_ceddda9d.IResource,
-    _aws_cdk_aws_ec2_ceddda9d.IConnectable,
-    _aws_cdk_aws_secretsmanager_ceddda9d.ISecretAttachmentTarget,
+    aws_cdk.IResource,
+    aws_cdk.aws_ec2.IConnectable,
+    aws_cdk.aws_secretsmanager.ISecretAttachmentTarget,
     typing_extensions.Protocol,
 ):
     '''(experimental) Create a Redshift Cluster with a given number of nodes.
 
-    Implemented by ``Cluster`` via ``ClusterBase``.
+    Implemented by {@link Cluster} via {@link ClusterBase}.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterEndpoint")
     def cluster_endpoint(self) -> Endpoint:
         '''(experimental) The endpoint to use for read/write operations.
 
         :stability: experimental
         :attribute: EndpointAddress,EndpointPort
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterName")
     def cluster_name(self) -> builtins.str:
         '''(experimental) Name of the cluster.
 
         :stability: experimental
         :attribute: ClusterName
         '''
         ...
 
 
 class _IClusterProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
-    jsii.proxy_for(_aws_cdk_aws_ec2_ceddda9d.IConnectable), # type: ignore[misc]
-    jsii.proxy_for(_aws_cdk_aws_secretsmanager_ceddda9d.ISecretAttachmentTarget), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.aws_ec2.IConnectable), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.aws_secretsmanager.ISecretAttachmentTarget), # type: ignore[misc]
 ):
     '''(experimental) Create a Redshift Cluster with a given number of nodes.
 
-    Implemented by ``Cluster`` via ``ClusterBase``.
+    Implemented by {@link Cluster} via {@link ClusterBase}.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-redshift-alpha.ICluster"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterEndpoint")
     def cluster_endpoint(self) -> Endpoint:
         '''(experimental) The endpoint to use for read/write operations.
 
         :stability: experimental
         :attribute: EndpointAddress,EndpointPort
         '''
         return typing.cast(Endpoint, jsii.get(self, "clusterEndpoint"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterName")
     def cluster_name(self) -> builtins.str:
         '''(experimental) Name of the cluster.
 
         :stability: experimental
         :attribute: ClusterName
         '''
         return typing.cast(builtins.str, jsii.get(self, "clusterName"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, ICluster).__jsii_proxy_class__ = lambda : _IClusterProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-redshift-alpha.IClusterParameterGroup")
-class IClusterParameterGroup(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class IClusterParameterGroup(aws_cdk.IResource, typing_extensions.Protocol):
     '''(experimental) A parameter group.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterParameterGroupName")
     def cluster_parameter_group_name(self) -> builtins.str:
         '''(experimental) The name of this parameter group.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _IClusterParameterGroupProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''(experimental) A parameter group.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-redshift-alpha.IClusterParameterGroup"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterParameterGroupName")
     def cluster_parameter_group_name(self) -> builtins.str:
         '''(experimental) The name of this parameter group.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "clusterParameterGroupName"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IClusterParameterGroup).__jsii_proxy_class__ = lambda : _IClusterParameterGroupProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-redshift-alpha.IClusterSubnetGroup")
-class IClusterSubnetGroup(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class IClusterSubnetGroup(aws_cdk.IResource, typing_extensions.Protocol):
     '''(experimental) Interface for a cluster subnet group.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterSubnetGroupName")
     def cluster_subnet_group_name(self) -> builtins.str:
         '''(experimental) The name of the cluster subnet group.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _IClusterSubnetGroupProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''(experimental) Interface for a cluster subnet group.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-redshift-alpha.IClusterSubnetGroup"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterSubnetGroupName")
     def cluster_subnet_group_name(self) -> builtins.str:
         '''(experimental) The name of the cluster subnet group.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "clusterSubnetGroupName"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IClusterSubnetGroup).__jsii_proxy_class__ = lambda : _IClusterSubnetGroupProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-redshift-alpha.ITable")
-class ITable(_constructs_77d1e7e8.IConstruct, typing_extensions.Protocol):
+class ITable(constructs.IConstruct, typing_extensions.Protocol):
     '''(experimental) Represents a table in a Redshift database.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="cluster")
     def cluster(self) -> ICluster:
         '''(experimental) The cluster where the table is located.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="databaseName")
     def database_name(self) -> builtins.str:
         '''(experimental) The name of the database where the table is located.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="tableColumns")
     def table_columns(self) -> typing.List[Column]:
         '''(experimental) The columns of the table.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="tableName")
     def table_name(self) -> builtins.str:
         '''(experimental) Name of the table.
 
         :stability: experimental
         '''
         ...
@@ -2189,51 +1587,51 @@
 
         :stability: experimental
         '''
         ...
 
 
 class _ITableProxy(
-    jsii.proxy_for(_constructs_77d1e7e8.IConstruct), # type: ignore[misc]
+    jsii.proxy_for(constructs.IConstruct) # type: ignore[misc]
 ):
     '''(experimental) Represents a table in a Redshift database.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-redshift-alpha.ITable"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="cluster")
     def cluster(self) -> ICluster:
         '''(experimental) The cluster where the table is located.
 
         :stability: experimental
         '''
         return typing.cast(ICluster, jsii.get(self, "cluster"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="databaseName")
     def database_name(self) -> builtins.str:
         '''(experimental) The name of the database where the table is located.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "databaseName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="tableColumns")
     def table_columns(self) -> typing.List[Column]:
         '''(experimental) The columns of the table.
 
         :stability: experimental
         '''
         return typing.cast(typing.List[Column], jsii.get(self, "tableColumns"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="tableName")
     def table_name(self) -> builtins.str:
         '''(experimental) Name of the table.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "tableName"))
@@ -2243,59 +1641,55 @@
         '''(experimental) Grant a user privilege to access this table.
 
         :param user: -
         :param actions: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__febfab9a8c6f0c1f081d5f0f1dd5fb2ba403be29fbe7dcef6e4fffb955b09c77)
-            check_type(argname="argument user", value=user, expected_type=type_hints["user"])
-            check_type(argname="argument actions", value=actions, expected_type=typing.Tuple[type_hints["actions"], ...]) # pyright: ignore [reportGeneralTypeIssues]
         return typing.cast(None, jsii.invoke(self, "grant", [user, *actions]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, ITable).__jsii_proxy_class__ = lambda : _ITableProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-redshift-alpha.IUser")
-class IUser(_constructs_77d1e7e8.IConstruct, typing_extensions.Protocol):
+class IUser(constructs.IConstruct, typing_extensions.Protocol):
     '''(experimental) Represents a user in a Redshift database.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="cluster")
     def cluster(self) -> ICluster:
         '''(experimental) The cluster where the table is located.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="databaseName")
     def database_name(self) -> builtins.str:
         '''(experimental) The name of the database where the table is located.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="password")
-    def password(self) -> _aws_cdk_ceddda9d.SecretValue:
+    def password(self) -> aws_cdk.SecretValue:
         '''(experimental) The password of the user.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="username")
     def username(self) -> builtins.str:
         '''(experimental) The name of the user.
 
         :stability: experimental
         '''
         ...
@@ -2309,51 +1703,51 @@
 
         :stability: experimental
         '''
         ...
 
 
 class _IUserProxy(
-    jsii.proxy_for(_constructs_77d1e7e8.IConstruct), # type: ignore[misc]
+    jsii.proxy_for(constructs.IConstruct) # type: ignore[misc]
 ):
     '''(experimental) Represents a user in a Redshift database.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-redshift-alpha.IUser"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="cluster")
     def cluster(self) -> ICluster:
         '''(experimental) The cluster where the table is located.
 
         :stability: experimental
         '''
         return typing.cast(ICluster, jsii.get(self, "cluster"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="databaseName")
     def database_name(self) -> builtins.str:
         '''(experimental) The name of the database where the table is located.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "databaseName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="password")
-    def password(self) -> _aws_cdk_ceddda9d.SecretValue:
+    def password(self) -> aws_cdk.SecretValue:
         '''(experimental) The password of the user.
 
         :stability: experimental
         '''
-        return typing.cast(_aws_cdk_ceddda9d.SecretValue, jsii.get(self, "password"))
+        return typing.cast(aws_cdk.SecretValue, jsii.get(self, "password"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="username")
     def username(self) -> builtins.str:
         '''(experimental) The name of the user.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "username"))
@@ -2363,159 +1757,59 @@
         '''(experimental) Grant this user privilege to access a table.
 
         :param table: -
         :param actions: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__482349d4a650668e65613cc4cb7308f07f28faff85e9f7754c08cde21ac2e7fb)
-            check_type(argname="argument table", value=table, expected_type=type_hints["table"])
-            check_type(argname="argument actions", value=actions, expected_type=typing.Tuple[type_hints["actions"], ...]) # pyright: ignore [reportGeneralTypeIssues]
         return typing.cast(None, jsii.invoke(self, "addTablePrivileges", [table, *actions]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IUser).__jsii_proxy_class__ = lambda : _IUserProxy
 
 
 @jsii.data_type(
-    jsii_type="@aws-cdk/aws-redshift-alpha.LoggingProperties",
-    jsii_struct_bases=[],
-    name_mapping={
-        "logging_bucket": "loggingBucket",
-        "logging_key_prefix": "loggingKeyPrefix",
-    },
-)
-class LoggingProperties:
-    def __init__(
-        self,
-        *,
-        logging_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
-        logging_key_prefix: builtins.str,
-    ) -> None:
-        '''(experimental) Logging bucket and S3 prefix combination.
-
-        :param logging_bucket: (experimental) Bucket to send logs to. Logging information includes queries and connection attempts, for the specified Amazon Redshift cluster.
-        :param logging_key_prefix: (experimental) Prefix used for logging.
-
-        :stability: experimental
-        :exampleMetadata: infused
-
-        Example::
-
-            import aws_cdk.aws_ec2 as ec2
-            import aws_cdk.aws_s3 as s3
-            
-            
-            vpc = ec2.Vpc(self, "Vpc")
-            bucket = s3.Bucket.from_bucket_name(self, "bucket", "logging-bucket")
-            
-            cluster = Cluster(self, "Redshift",
-                master_user=Login(
-                    master_username="admin"
-                ),
-                vpc=vpc,
-                logging_properties=LoggingProperties(
-                    logging_bucket=bucket,
-                    logging_key_prefix="prefix"
-                )
-            )
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__31bfca026b86708f38bf1964cd5ab577729657ca2c1adbb4f4c27e417cbd7b99)
-            check_type(argname="argument logging_bucket", value=logging_bucket, expected_type=type_hints["logging_bucket"])
-            check_type(argname="argument logging_key_prefix", value=logging_key_prefix, expected_type=type_hints["logging_key_prefix"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
-            "logging_bucket": logging_bucket,
-            "logging_key_prefix": logging_key_prefix,
-        }
-
-    @builtins.property
-    def logging_bucket(self) -> _aws_cdk_aws_s3_ceddda9d.IBucket:
-        '''(experimental) Bucket to send logs to.
-
-        Logging information includes queries and connection attempts, for the specified Amazon Redshift cluster.
-
-        :stability: experimental
-        '''
-        result = self._values.get("logging_bucket")
-        assert result is not None, "Required property 'logging_bucket' is missing"
-        return typing.cast(_aws_cdk_aws_s3_ceddda9d.IBucket, result)
-
-    @builtins.property
-    def logging_key_prefix(self) -> builtins.str:
-        '''(experimental) Prefix used for logging.
-
-        :stability: experimental
-        '''
-        result = self._values.get("logging_key_prefix")
-        assert result is not None, "Required property 'logging_key_prefix' is missing"
-        return typing.cast(builtins.str, result)
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "LoggingProperties(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
-
-@jsii.data_type(
     jsii_type="@aws-cdk/aws-redshift-alpha.Login",
     jsii_struct_bases=[],
     name_mapping={
         "master_username": "masterUsername",
         "encryption_key": "encryptionKey",
         "master_password": "masterPassword",
     },
 )
 class Login:
     def __init__(
         self,
         *,
         master_username: builtins.str,
-        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-        master_password: typing.Optional[_aws_cdk_ceddda9d.SecretValue] = None,
+        encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
+        master_password: typing.Optional[aws_cdk.SecretValue] = None,
     ) -> None:
         '''(experimental) Username and password combination.
 
         :param master_username: (experimental) Username.
         :param encryption_key: (experimental) KMS encryption key to encrypt the generated secret. Default: default master key
         :param master_password: (experimental) Password. Do not put passwords in your CDK code directly. Default: a Secrets Manager generated password
 
         :stability: experimental
-        :exampleMetadata: infused
+        :exampleMetadata: fixture=cluster infused
 
         Example::
 
-            import aws_cdk.aws_ec2 as ec2
-            import aws_cdk as cdk
-            # vpc: ec2.Vpc
+            import aws_cdk.aws_kms as kms
             
             
-            Cluster(self, "Redshift",
-                master_user=Login(
-                    master_username="admin",
-                    master_password=cdk.SecretValue.unsafe_plain_text("tooshort")
-                ),
-                vpc=vpc,
-                publicly_accessible=True,
-                elastic_ip="10.123.123.255"
+            encryption_key = kms.Key(self, "Key")
+            User(self, "User",
+                encryption_key=encryption_key,
+                cluster=cluster,
+                database_name="databaseName"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f290e69c40e3c1e3b75f41243f96283d1619e3967c3b2bd3458c974e11b7f430)
-            check_type(argname="argument master_username", value=master_username, expected_type=type_hints["master_username"])
-            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
-            check_type(argname="argument master_password", value=master_password, expected_type=type_hints["master_password"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "master_username": master_username,
         }
         if encryption_key is not None:
             self._values["encryption_key"] = encryption_key
         if master_password is not None:
             self._values["master_password"] = master_password
 
@@ -2526,36 +1820,36 @@
         :stability: experimental
         '''
         result = self._values.get("master_username")
         assert result is not None, "Required property 'master_username' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def encryption_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def encryption_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) KMS encryption key to encrypt the generated secret.
 
         :default: default master key
 
         :stability: experimental
         '''
         result = self._values.get("encryption_key")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], result)
 
     @builtins.property
-    def master_password(self) -> typing.Optional[_aws_cdk_ceddda9d.SecretValue]:
+    def master_password(self) -> typing.Optional[aws_cdk.SecretValue]:
         '''(experimental) Password.
 
         Do not put passwords in your CDK code directly.
 
         :default: a Secrets Manager generated password
 
         :stability: experimental
         '''
         result = self._values.get("master_password")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.SecretValue], result)
+        return typing.cast(typing.Optional[aws_cdk.SecretValue], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -2563,15 +1857,15 @@
         return "Login(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.enum(jsii_type="@aws-cdk/aws-redshift-alpha.NodeType")
 class NodeType(enum.Enum):
-    '''(experimental) Possible Node Types to use in the cluster used for defining ``ClusterProps.nodeType``.
+    '''(experimental) Possible Node Types to use in the cluster used for defining {@link ClusterProps.nodeType}.
 
     :stability: experimental
     '''
 
     DS2_XLARGE = "DS2_XLARGE"
     '''(experimental) ds2.xlarge.
 
@@ -2624,77 +1918,72 @@
     jsii_struct_bases=[],
     name_mapping={"secret": "secret", "automatically_after": "automaticallyAfter"},
 )
 class RotationMultiUserOptions:
     def __init__(
         self,
         *,
-        secret: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
-        automatically_after: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        secret: aws_cdk.aws_secretsmanager.ISecret,
+        automatically_after: typing.Optional[aws_cdk.Duration] = None,
     ) -> None:
         '''(experimental) Options to add the multi user rotation.
 
         :param secret: (experimental) The secret to rotate. It must be a JSON string with the following format:: { "engine": <required: database engine>, "host": <required: instance host name>, "username": <required: username>, "password": <required: password>, "dbname": <optional: database name>, "port": <optional: if not specified, default port will be used>, "masterarn": <required: the arn of the master secret which will be used to create users/change passwords> }
         :param automatically_after: (experimental) Specifies the number of days after the previous rotation before Secrets Manager triggers the next automatic rotation. Default: Duration.days(30)
 
         :stability: experimental
         :exampleMetadata: fixture=cluster infused
 
         Example::
 
-            user = User(self, "User",
-                cluster=cluster,
-                database_name="databaseName"
-            )
-            cluster.add_rotation_multi_user("MultiUserRotation",
-                secret=user.secret
+            import aws_cdk.aws_secretsmanager as secretsmanager
+            
+            
+            cluster.add_rotation_multi_user("MyUser",
+                secret=secretsmanager.Secret.from_secret_name_v2(self, "Imported Secret", "my-secret")
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e8ff1dc8f069ed8db9a6c9c88c8b732a109f9c9198fa3b3df5acbb57173d041d)
-            check_type(argname="argument secret", value=secret, expected_type=type_hints["secret"])
-            check_type(argname="argument automatically_after", value=automatically_after, expected_type=type_hints["automatically_after"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "secret": secret,
         }
         if automatically_after is not None:
             self._values["automatically_after"] = automatically_after
 
     @builtins.property
-    def secret(self) -> _aws_cdk_aws_secretsmanager_ceddda9d.ISecret:
+    def secret(self) -> aws_cdk.aws_secretsmanager.ISecret:
         '''(experimental) The secret to rotate.
 
         It must be a JSON string with the following format::
 
            {
-             "engine": <required: database engine>,
-             "host": <required: instance host name>,
-             "username": <required: username>,
-             "password": <required: password>,
-             "dbname": <optional: database name>,
-             "port": <optional: if not specified, default port will be used>,
-             "masterarn": <required: the arn of the master secret which will be used to create users/change passwords>
+              "engine": <required: database engine>,
+              "host": <required: instance host name>,
+              "username": <required: username>,
+              "password": <required: password>,
+              "dbname": <optional: database name>,
+              "port": <optional: if not specified, default port will be used>,
+              "masterarn": <required: the arn of the master secret which will be used to create users/change passwords>
            }
 
         :stability: experimental
         '''
         result = self._values.get("secret")
         assert result is not None, "Required property 'secret' is missing"
-        return typing.cast(_aws_cdk_aws_secretsmanager_ceddda9d.ISecret, result)
+        return typing.cast(aws_cdk.aws_secretsmanager.ISecret, result)
 
     @builtins.property
-    def automatically_after(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+    def automatically_after(self) -> typing.Optional[aws_cdk.Duration]:
         '''(experimental) Specifies the number of days after the previous rotation before Secrets Manager triggers the next automatic rotation.
 
         :default: Duration.days(30)
 
         :stability: experimental
         '''
         result = self._values.get("automatically_after")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
+        return typing.cast(typing.Optional[aws_cdk.Duration], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -2702,15 +1991,15 @@
         return "RotationMultiUserOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.implements(ITable)
 class Table(
-    _constructs_77d1e7e8.Construct,
+    constructs.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-redshift-alpha.Table",
 ):
     '''(experimental) A table in a Redshift cluster.
 
     :stability: experimental
     :exampleMetadata: fixture=cluster infused
@@ -2724,98 +2013,87 @@
             database_name="databaseName",
             dist_style=TableDistStyle.KEY
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
-        table_columns: typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]],
+        table_columns: typing.Sequence[Column],
         dist_style: typing.Optional["TableDistStyle"] = None,
-        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+        removal_policy: typing.Optional[aws_cdk.RemovalPolicy] = None,
         sort_style: typing.Optional["TableSortStyle"] = None,
-        table_comment: typing.Optional[builtins.str] = None,
         table_name: typing.Optional[builtins.str] = None,
         cluster: ICluster,
         database_name: builtins.str,
-        admin_user: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
+        admin_user: typing.Optional[aws_cdk.aws_secretsmanager.ISecret] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param table_columns: (experimental) The columns of the table.
         :param dist_style: (experimental) The distribution style of the table. Default: TableDistStyle.AUTO
         :param removal_policy: (experimental) The policy to apply when this resource is removed from the application. Default: cdk.RemovalPolicy.Retain
         :param sort_style: (experimental) The sort style of the table. Default: TableSortStyle.AUTO if no sort key is specified, TableSortStyle.COMPOUND if a sort key is specified
-        :param table_comment: (experimental) A comment to attach to the table. Default: - no comment
         :param table_name: (experimental) The name of the table. Default: - a name is generated
         :param cluster: (experimental) The cluster containing the database.
         :param database_name: (experimental) The name of the database.
         :param admin_user: (experimental) The secret containing credentials to a Redshift user with administrator privileges. Secret JSON schema: ``{ username: string; password: string }``. Default: - the admin secret is taken from the cluster
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f5bb5cdc9b9d71db081569ce1699ad72f4cda1e74e44ad08c8dfcaa831d2ecfb)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = TableProps(
             table_columns=table_columns,
             dist_style=dist_style,
             removal_policy=removal_policy,
             sort_style=sort_style,
-            table_comment=table_comment,
             table_name=table_name,
             cluster=cluster,
             database_name=database_name,
             admin_user=admin_user,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromTableAttributes")
+    @jsii.member(jsii_name="fromTableAttributes") # type: ignore[misc]
     @builtins.classmethod
     def from_table_attributes(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         cluster: ICluster,
         database_name: builtins.str,
-        table_columns: typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]],
+        table_columns: typing.Sequence[Column],
         table_name: builtins.str,
     ) -> ITable:
         '''(experimental) Specify a Redshift table using a table name and schema that already exists.
 
         :param scope: -
         :param id: -
         :param cluster: (experimental) The cluster where the table is located.
         :param database_name: (experimental) The name of the database where the table is located.
         :param table_columns: (experimental) The columns of the table.
         :param table_name: (experimental) Name of the table.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c588c15b59523c46188be2ed268598c40457a45f5ae6af6ee90f43398b2a87c6)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         attrs = TableAttributes(
             cluster=cluster,
             database_name=database_name,
             table_columns=table_columns,
             table_name=table_name,
         )
 
         return typing.cast(ITable, jsii.sinvoke(cls, "fromTableAttributes", [scope, id, attrs]))
 
     @jsii.member(jsii_name="applyRemovalPolicy")
-    def apply_removal_policy(self, policy: _aws_cdk_ceddda9d.RemovalPolicy) -> None:
+    def apply_removal_policy(self, policy: aws_cdk.RemovalPolicy) -> None:
         '''(experimental) Apply the given removal policy to this resource.
 
         The Removal Policy controls what happens to this resource when it stops
         being managed by CloudFormation, either because you've removed it from the
         CDK application or because you've made a change that requires the resource
         to be replaced.
 
@@ -2824,62 +2102,55 @@
 
         This resource is retained by default.
 
         :param policy: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7a2559de86af99b035e3551696efbd323c09454e4966d219dbac73eb0ecbbc26)
-            check_type(argname="argument policy", value=policy, expected_type=type_hints["policy"])
         return typing.cast(None, jsii.invoke(self, "applyRemovalPolicy", [policy]))
 
     @jsii.member(jsii_name="grant")
     def grant(self, user: IUser, *actions: "TableAction") -> None:
         '''(experimental) Grant a user privilege to access this table.
 
         :param user: -
         :param actions: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2cedd8e4ce5ed742b7998abe8c2f47aca8c358cbec88a746c68669950dbfcf79)
-            check_type(argname="argument user", value=user, expected_type=type_hints["user"])
-            check_type(argname="argument actions", value=actions, expected_type=typing.Tuple[type_hints["actions"], ...]) # pyright: ignore [reportGeneralTypeIssues]
         return typing.cast(None, jsii.invoke(self, "grant", [user, *actions]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="cluster")
     def cluster(self) -> ICluster:
         '''(experimental) The cluster where the table is located.
 
         :stability: experimental
         '''
         return typing.cast(ICluster, jsii.get(self, "cluster"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="databaseName")
     def database_name(self) -> builtins.str:
         '''(experimental) The name of the database where the table is located.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "databaseName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="tableColumns")
     def table_columns(self) -> typing.List[Column]:
         '''(experimental) The columns of the table.
 
         :stability: experimental
         '''
         return typing.cast(typing.List[Column], jsii.get(self, "tableColumns"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="tableName")
     def table_name(self) -> builtins.str:
         '''(experimental) Name of the table.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "tableName"))
@@ -2962,15 +2233,15 @@
 )
 class TableAttributes:
     def __init__(
         self,
         *,
         cluster: ICluster,
         database_name: builtins.str,
-        table_columns: typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]],
+        table_columns: typing.Sequence[Column],
         table_name: builtins.str,
     ) -> None:
         '''(experimental) A full specification of a Redshift table that can be used to import it fluently into the CDK application.
 
         :param cluster: (experimental) The cluster where the table is located.
         :param database_name: (experimental) The name of the database where the table is located.
         :param table_columns: (experimental) The columns of the table.
@@ -2983,33 +2254,27 @@
 
             database_name = "databaseName"
             username = "myuser"
             table_name = "mytable"
             
             user = User.from_user_attributes(self, "User",
                 username=username,
-                password=SecretValue.unsafe_plain_text("NOT_FOR_PRODUCTION"),
+                password=SecretValue.plain_text("NOT_FOR_PRODUCTION"),
                 cluster=cluster,
                 database_name=database_name
             )
             table = Table.from_table_attributes(self, "Table",
                 table_name=table_name,
                 table_columns=[Column(name="col1", data_type="varchar(4)"), Column(name="col2", data_type="float")],
                 cluster=cluster,
                 database_name="databaseName"
             )
             table.grant(user, TableAction.INSERT)
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a72be394d5e035726f67dcce82f498875671e673396787b30bed1cb67dd061c8)
-            check_type(argname="argument cluster", value=cluster, expected_type=type_hints["cluster"])
-            check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
-            check_type(argname="argument table_columns", value=table_columns, expected_type=type_hints["table_columns"])
-            check_type(argname="argument table_name", value=table_name, expected_type=type_hints["table_name"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "cluster": cluster,
             "database_name": database_name,
             "table_columns": table_columns,
             "table_name": table_name,
         }
 
     @builtins.property
@@ -3111,42 +2376,39 @@
         "cluster": "cluster",
         "database_name": "databaseName",
         "admin_user": "adminUser",
         "table_columns": "tableColumns",
         "dist_style": "distStyle",
         "removal_policy": "removalPolicy",
         "sort_style": "sortStyle",
-        "table_comment": "tableComment",
         "table_name": "tableName",
     },
 )
 class TableProps(DatabaseOptions):
     def __init__(
         self,
         *,
         cluster: ICluster,
         database_name: builtins.str,
-        admin_user: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
-        table_columns: typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]],
+        admin_user: typing.Optional[aws_cdk.aws_secretsmanager.ISecret] = None,
+        table_columns: typing.Sequence[Column],
         dist_style: typing.Optional[TableDistStyle] = None,
-        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+        removal_policy: typing.Optional[aws_cdk.RemovalPolicy] = None,
         sort_style: typing.Optional["TableSortStyle"] = None,
-        table_comment: typing.Optional[builtins.str] = None,
         table_name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Properties for configuring a Redshift table.
 
         :param cluster: (experimental) The cluster containing the database.
         :param database_name: (experimental) The name of the database.
         :param admin_user: (experimental) The secret containing credentials to a Redshift user with administrator privileges. Secret JSON schema: ``{ username: string; password: string }``. Default: - the admin secret is taken from the cluster
         :param table_columns: (experimental) The columns of the table.
         :param dist_style: (experimental) The distribution style of the table. Default: TableDistStyle.AUTO
         :param removal_policy: (experimental) The policy to apply when this resource is removed from the application. Default: cdk.RemovalPolicy.Retain
         :param sort_style: (experimental) The sort style of the table. Default: TableSortStyle.AUTO if no sort key is specified, TableSortStyle.COMPOUND if a sort key is specified
-        :param table_comment: (experimental) A comment to attach to the table. Default: - no comment
         :param table_name: (experimental) The name of the table. Default: - a name is generated
 
         :stability: experimental
         :exampleMetadata: fixture=cluster infused
 
         Example::
 
@@ -3154,40 +2416,27 @@
                 table_columns=[Column(name="col1", data_type="varchar(4)", dist_key=True), Column(name="col2", data_type="float")
                 ],
                 cluster=cluster,
                 database_name="databaseName",
                 dist_style=TableDistStyle.KEY
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2d4444361722818dd5438346bad361ad93c2f629efde6c384600398f4b5051b2)
-            check_type(argname="argument cluster", value=cluster, expected_type=type_hints["cluster"])
-            check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
-            check_type(argname="argument admin_user", value=admin_user, expected_type=type_hints["admin_user"])
-            check_type(argname="argument table_columns", value=table_columns, expected_type=type_hints["table_columns"])
-            check_type(argname="argument dist_style", value=dist_style, expected_type=type_hints["dist_style"])
-            check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
-            check_type(argname="argument sort_style", value=sort_style, expected_type=type_hints["sort_style"])
-            check_type(argname="argument table_comment", value=table_comment, expected_type=type_hints["table_comment"])
-            check_type(argname="argument table_name", value=table_name, expected_type=type_hints["table_name"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "cluster": cluster,
             "database_name": database_name,
             "table_columns": table_columns,
         }
         if admin_user is not None:
             self._values["admin_user"] = admin_user
         if dist_style is not None:
             self._values["dist_style"] = dist_style
         if removal_policy is not None:
             self._values["removal_policy"] = removal_policy
         if sort_style is not None:
             self._values["sort_style"] = sort_style
-        if table_comment is not None:
-            self._values["table_comment"] = table_comment
         if table_name is not None:
             self._values["table_name"] = table_name
 
     @builtins.property
     def cluster(self) -> ICluster:
         '''(experimental) The cluster containing the database.
 
@@ -3204,27 +2453,25 @@
         :stability: experimental
         '''
         result = self._values.get("database_name")
         assert result is not None, "Required property 'database_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def admin_user(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret]:
+    def admin_user(self) -> typing.Optional[aws_cdk.aws_secretsmanager.ISecret]:
         '''(experimental) The secret containing credentials to a Redshift user with administrator privileges.
 
         Secret JSON schema: ``{ username: string; password: string }``.
 
         :default: - the admin secret is taken from the cluster
 
         :stability: experimental
         '''
         result = self._values.get("admin_user")
-        return typing.cast(typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_secretsmanager.ISecret], result)
 
     @builtins.property
     def table_columns(self) -> typing.List[Column]:
         '''(experimental) The columns of the table.
 
         :stability: experimental
         '''
@@ -3240,47 +2487,36 @@
 
         :stability: experimental
         '''
         result = self._values.get("dist_style")
         return typing.cast(typing.Optional[TableDistStyle], result)
 
     @builtins.property
-    def removal_policy(self) -> typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy]:
+    def removal_policy(self) -> typing.Optional[aws_cdk.RemovalPolicy]:
         '''(experimental) The policy to apply when this resource is removed from the application.
 
         :default: cdk.RemovalPolicy.Retain
 
         :stability: experimental
         '''
         result = self._values.get("removal_policy")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy], result)
+        return typing.cast(typing.Optional[aws_cdk.RemovalPolicy], result)
 
     @builtins.property
     def sort_style(self) -> typing.Optional["TableSortStyle"]:
         '''(experimental) The sort style of the table.
 
         :default: TableSortStyle.AUTO if no sort key is specified, TableSortStyle.COMPOUND if a sort key is specified
 
         :stability: experimental
         '''
         result = self._values.get("sort_style")
         return typing.cast(typing.Optional["TableSortStyle"], result)
 
     @builtins.property
-    def table_comment(self) -> typing.Optional[builtins.str]:
-        '''(experimental) A comment to attach to the table.
-
-        :default: - no comment
-
-        :stability: experimental
-        '''
-        result = self._values.get("table_comment")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
     def table_name(self) -> typing.Optional[builtins.str]:
         '''(experimental) The name of the table.
 
         :default: - a name is generated
 
         :stability: experimental
         '''
@@ -3332,102 +2568,96 @@
 
     :stability: experimental
     '''
 
 
 @jsii.implements(IUser)
 class User(
-    _constructs_77d1e7e8.Construct,
+    constructs.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-redshift-alpha.User",
 ):
     '''(experimental) A user in a Redshift cluster.
 
     :stability: experimental
     :exampleMetadata: fixture=cluster infused
 
     Example::
 
-        user = User(self, "User",
+        import aws_cdk.aws_kms as kms
+        
+        
+        encryption_key = kms.Key(self, "Key")
+        User(self, "User",
+            encryption_key=encryption_key,
             cluster=cluster,
             database_name="databaseName"
         )
-        cluster.add_rotation_multi_user("MultiUserRotation",
-            secret=user.secret
-        )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
-        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+        encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
+        removal_policy: typing.Optional[aws_cdk.RemovalPolicy] = None,
         username: typing.Optional[builtins.str] = None,
         cluster: ICluster,
         database_name: builtins.str,
-        admin_user: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
+        admin_user: typing.Optional[aws_cdk.aws_secretsmanager.ISecret] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param encryption_key: (experimental) KMS key to encrypt the generated secret. Default: - the default AWS managed key is used
         :param removal_policy: (experimental) The policy to apply when this resource is removed from the application. Default: cdk.RemovalPolicy.Destroy
         :param username: (experimental) The name of the user. For valid values, see: https://docs.aws.amazon.com/redshift/latest/dg/r_names.html Default: - a name is generated
         :param cluster: (experimental) The cluster containing the database.
         :param database_name: (experimental) The name of the database.
         :param admin_user: (experimental) The secret containing credentials to a Redshift user with administrator privileges. Secret JSON schema: ``{ username: string; password: string }``. Default: - the admin secret is taken from the cluster
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__684a841e4fc7788170b0197fb7931e6c62bd55d596af8e0196b42df62e434ea4)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = UserProps(
             encryption_key=encryption_key,
             removal_policy=removal_policy,
             username=username,
             cluster=cluster,
             database_name=database_name,
             admin_user=admin_user,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromUserAttributes")
+    @jsii.member(jsii_name="fromUserAttributes") # type: ignore[misc]
     @builtins.classmethod
     def from_user_attributes(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
-        password: _aws_cdk_ceddda9d.SecretValue,
+        password: aws_cdk.SecretValue,
         username: builtins.str,
         cluster: ICluster,
         database_name: builtins.str,
-        admin_user: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
+        admin_user: typing.Optional[aws_cdk.aws_secretsmanager.ISecret] = None,
     ) -> IUser:
         '''(experimental) Specify a Redshift user using credentials that already exist.
 
         :param scope: -
         :param id: -
         :param password: (experimental) The password of the user. Do not put passwords in CDK code directly.
         :param username: (experimental) The name of the user.
         :param cluster: (experimental) The cluster containing the database.
         :param database_name: (experimental) The name of the database.
         :param admin_user: (experimental) The secret containing credentials to a Redshift user with administrator privileges. Secret JSON schema: ``{ username: string; password: string }``. Default: - the admin secret is taken from the cluster
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__483704cbd1ddd53dbc57f757961a2e3d53ae948da0d8d8f8e8d50b847958dfd6)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         attrs = UserAttributes(
             password=password,
             username=username,
             cluster=cluster,
             database_name=database_name,
             admin_user=admin_user,
         )
@@ -3439,22 +2669,18 @@
         '''(experimental) Grant this user privilege to access a table.
 
         :param table: -
         :param actions: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9c310d0b8092d0aef06348ff2e68c7aa7577648c18e7656284f491091331d877)
-            check_type(argname="argument table", value=table, expected_type=type_hints["table"])
-            check_type(argname="argument actions", value=actions, expected_type=typing.Tuple[type_hints["actions"], ...]) # pyright: ignore [reportGeneralTypeIssues]
         return typing.cast(None, jsii.invoke(self, "addTablePrivileges", [table, *actions]))
 
     @jsii.member(jsii_name="applyRemovalPolicy")
-    def apply_removal_policy(self, policy: _aws_cdk_ceddda9d.RemovalPolicy) -> None:
+    def apply_removal_policy(self, policy: aws_cdk.RemovalPolicy) -> None:
         '''(experimental) Apply the given removal policy to this resource.
 
         The Removal Policy controls what happens to this resource when it stops
         being managed by CloudFormation, either because you've removed it from the
         CDK application or because you've made a change that requires the resource
         to be replaced.
 
@@ -3463,78 +2689,62 @@
 
         This resource is destroyed by default.
 
         :param policy: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e783176cde66b005bd7a48047c42d2daa161b7fbf0608fd8c280193b160dc7f9)
-            check_type(argname="argument policy", value=policy, expected_type=type_hints["policy"])
         return typing.cast(None, jsii.invoke(self, "applyRemovalPolicy", [policy]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="cluster")
     def cluster(self) -> ICluster:
         '''(experimental) The cluster where the table is located.
 
         :stability: experimental
         '''
         return typing.cast(ICluster, jsii.get(self, "cluster"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="databaseName")
     def database_name(self) -> builtins.str:
         '''(experimental) The name of the database where the table is located.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "databaseName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="password")
-    def password(self) -> _aws_cdk_ceddda9d.SecretValue:
+    def password(self) -> aws_cdk.SecretValue:
         '''(experimental) The password of the user.
 
         :stability: experimental
         '''
-        return typing.cast(_aws_cdk_ceddda9d.SecretValue, jsii.get(self, "password"))
+        return typing.cast(aws_cdk.SecretValue, jsii.get(self, "password"))
 
-    @builtins.property
-    @jsii.member(jsii_name="secret")
-    def secret(self) -> _aws_cdk_aws_secretsmanager_ceddda9d.ISecret:
-        '''(experimental) The Secrets Manager secret of the user.
-
-        :stability: experimental
-        :attribute: true
-        '''
-        return typing.cast(_aws_cdk_aws_secretsmanager_ceddda9d.ISecret, jsii.get(self, "secret"))
-
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="username")
     def username(self) -> builtins.str:
         '''(experimental) The name of the user.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "username"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="databaseProps")
     def _database_props(self) -> DatabaseOptions:
         '''
         :stability: experimental
         '''
         return typing.cast(DatabaseOptions, jsii.get(self, "databaseProps"))
 
     @_database_props.setter
     def _database_props(self, value: DatabaseOptions) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__215d4d48a362ca590c122ef61d7450d160371decc86d4e5977bce6a23d0ca17f)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "databaseProps", value)
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-redshift-alpha.UserAttributes",
     jsii_struct_bases=[DatabaseOptions],
     name_mapping={
@@ -3547,16 +2757,16 @@
 )
 class UserAttributes(DatabaseOptions):
     def __init__(
         self,
         *,
         cluster: ICluster,
         database_name: builtins.str,
-        admin_user: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
-        password: _aws_cdk_ceddda9d.SecretValue,
+        admin_user: typing.Optional[aws_cdk.aws_secretsmanager.ISecret] = None,
+        password: aws_cdk.SecretValue,
         username: builtins.str,
     ) -> None:
         '''(experimental) A full specification of a Redshift user that can be used to import it fluently into the CDK application.
 
         :param cluster: (experimental) The cluster containing the database.
         :param database_name: (experimental) The name of the database.
         :param admin_user: (experimental) The secret containing credentials to a Redshift user with administrator privileges. Secret JSON schema: ``{ username: string; password: string }``. Default: - the admin secret is taken from the cluster
@@ -3570,34 +2780,27 @@
 
             database_name = "databaseName"
             username = "myuser"
             table_name = "mytable"
             
             user = User.from_user_attributes(self, "User",
                 username=username,
-                password=SecretValue.unsafe_plain_text("NOT_FOR_PRODUCTION"),
+                password=SecretValue.plain_text("NOT_FOR_PRODUCTION"),
                 cluster=cluster,
                 database_name=database_name
             )
             table = Table.from_table_attributes(self, "Table",
                 table_name=table_name,
                 table_columns=[Column(name="col1", data_type="varchar(4)"), Column(name="col2", data_type="float")],
                 cluster=cluster,
                 database_name="databaseName"
             )
             table.grant(user, TableAction.INSERT)
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__939764949bce87bd8dcf6ede326ec239f6dd7c2b716dbb9e552964fdc8d62557)
-            check_type(argname="argument cluster", value=cluster, expected_type=type_hints["cluster"])
-            check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
-            check_type(argname="argument admin_user", value=admin_user, expected_type=type_hints["admin_user"])
-            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
-            check_type(argname="argument username", value=username, expected_type=type_hints["username"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "cluster": cluster,
             "database_name": database_name,
             "password": password,
             "username": username,
         }
         if admin_user is not None:
             self._values["admin_user"] = admin_user
@@ -3619,39 +2822,37 @@
         :stability: experimental
         '''
         result = self._values.get("database_name")
         assert result is not None, "Required property 'database_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def admin_user(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret]:
+    def admin_user(self) -> typing.Optional[aws_cdk.aws_secretsmanager.ISecret]:
         '''(experimental) The secret containing credentials to a Redshift user with administrator privileges.
 
         Secret JSON schema: ``{ username: string; password: string }``.
 
         :default: - the admin secret is taken from the cluster
 
         :stability: experimental
         '''
         result = self._values.get("admin_user")
-        return typing.cast(typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_secretsmanager.ISecret], result)
 
     @builtins.property
-    def password(self) -> _aws_cdk_ceddda9d.SecretValue:
+    def password(self) -> aws_cdk.SecretValue:
         '''(experimental) The password of the user.
 
         Do not put passwords in CDK code directly.
 
         :stability: experimental
         '''
         result = self._values.get("password")
         assert result is not None, "Required property 'password' is missing"
-        return typing.cast(_aws_cdk_ceddda9d.SecretValue, result)
+        return typing.cast(aws_cdk.SecretValue, result)
 
     @builtins.property
     def username(self) -> builtins.str:
         '''(experimental) The name of the user.
 
         :stability: experimental
         '''
@@ -3685,17 +2886,17 @@
 )
 class UserProps(DatabaseOptions):
     def __init__(
         self,
         *,
         cluster: ICluster,
         database_name: builtins.str,
-        admin_user: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
-        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+        admin_user: typing.Optional[aws_cdk.aws_secretsmanager.ISecret] = None,
+        encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
+        removal_policy: typing.Optional[aws_cdk.RemovalPolicy] = None,
         username: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Properties for configuring a Redshift user.
 
         :param cluster: (experimental) The cluster containing the database.
         :param database_name: (experimental) The name of the database.
         :param admin_user: (experimental) The secret containing credentials to a Redshift user with administrator privileges. Secret JSON schema: ``{ username: string; password: string }``. Default: - the admin secret is taken from the cluster
@@ -3704,31 +2905,25 @@
         :param username: (experimental) The name of the user. For valid values, see: https://docs.aws.amazon.com/redshift/latest/dg/r_names.html Default: - a name is generated
 
         :stability: experimental
         :exampleMetadata: fixture=cluster infused
 
         Example::
 
-            user = User(self, "User",
+            import aws_cdk.aws_kms as kms
+            
+            
+            encryption_key = kms.Key(self, "Key")
+            User(self, "User",
+                encryption_key=encryption_key,
                 cluster=cluster,
                 database_name="databaseName"
             )
-            cluster.add_rotation_multi_user("MultiUserRotation",
-                secret=user.secret
-            )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0daf47fb2a97e4e73621e19347c149764ca3c3592695c3501419bf0d6e79cbd2)
-            check_type(argname="argument cluster", value=cluster, expected_type=type_hints["cluster"])
-            check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
-            check_type(argname="argument admin_user", value=admin_user, expected_type=type_hints["admin_user"])
-            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
-            check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
-            check_type(argname="argument username", value=username, expected_type=type_hints["username"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "cluster": cluster,
             "database_name": database_name,
         }
         if admin_user is not None:
             self._values["admin_user"] = admin_user
         if encryption_key is not None:
             self._values["encryption_key"] = encryption_key
@@ -3754,49 +2949,47 @@
         :stability: experimental
         '''
         result = self._values.get("database_name")
         assert result is not None, "Required property 'database_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def admin_user(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret]:
+    def admin_user(self) -> typing.Optional[aws_cdk.aws_secretsmanager.ISecret]:
         '''(experimental) The secret containing credentials to a Redshift user with administrator privileges.
 
         Secret JSON schema: ``{ username: string; password: string }``.
 
         :default: - the admin secret is taken from the cluster
 
         :stability: experimental
         '''
         result = self._values.get("admin_user")
-        return typing.cast(typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_secretsmanager.ISecret], result)
 
     @builtins.property
-    def encryption_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+    def encryption_key(self) -> typing.Optional[aws_cdk.aws_kms.IKey]:
         '''(experimental) KMS key to encrypt the generated secret.
 
         :default: - the default AWS managed key is used
 
         :stability: experimental
         '''
         result = self._values.get("encryption_key")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_kms.IKey], result)
 
     @builtins.property
-    def removal_policy(self) -> typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy]:
+    def removal_policy(self) -> typing.Optional[aws_cdk.RemovalPolicy]:
         '''(experimental) The policy to apply when this resource is removed from the application.
 
         :default: cdk.RemovalPolicy.Destroy
 
         :stability: experimental
         '''
         result = self._values.get("removal_policy")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy], result)
+        return typing.cast(typing.Optional[aws_cdk.RemovalPolicy], result)
 
     @builtins.property
     def username(self) -> typing.Optional[builtins.str]:
         '''(experimental) The name of the user.
 
         For valid values, see: https://docs.aws.amazon.com/redshift/latest/dg/r_names.html
 
@@ -3817,442 +3010,310 @@
         return "UserProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.implements(ICluster)
 class Cluster(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-redshift-alpha.Cluster",
 ):
     '''(experimental) Create a Redshift cluster a given number of nodes.
 
     :stability: experimental
-    :resource: AWS::Redshift::Cluster
     :exampleMetadata: infused
+    :resource: AWS::Redshift::Cluster
 
     Example::
 
         import aws_cdk.aws_ec2 as ec2
-        import aws_cdk as cdk
-        # vpc: ec2.Vpc
         
         
-        cluster = Cluster(self, "Cluster",
+        vpc = ec2.Vpc(self, "Vpc")
+        cluster = Cluster(self, "Redshift",
             master_user=Login(
-                master_username="admin",
-                master_password=cdk.SecretValue.unsafe_plain_text("tooshort")
+                master_username="admin"
             ),
             vpc=vpc
         )
-        
-        cluster.add_to_parameter_group("enable_user_activity_logging", "true")
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
-        master_user: typing.Union[Login, typing.Dict[builtins.str, typing.Any]],
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-        classic_resizing: typing.Optional[builtins.bool] = None,
+        master_user: Login,
+        vpc: aws_cdk.aws_ec2.IVpc,
         cluster_name: typing.Optional[builtins.str] = None,
         cluster_type: typing.Optional[ClusterType] = None,
         default_database_name: typing.Optional[builtins.str] = None,
-        default_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-        elastic_ip: typing.Optional[builtins.str] = None,
         encrypted: typing.Optional[builtins.bool] = None,
-        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-        enhanced_vpc_routing: typing.Optional[builtins.bool] = None,
-        logging_properties: typing.Optional[typing.Union[LoggingProperties, typing.Dict[builtins.str, typing.Any]]] = None,
+        encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
+        logging_bucket: typing.Optional[aws_cdk.aws_s3.IBucket] = None,
+        logging_key_prefix: typing.Optional[builtins.str] = None,
         node_type: typing.Optional[NodeType] = None,
         number_of_nodes: typing.Optional[jsii.Number] = None,
         parameter_group: typing.Optional[IClusterParameterGroup] = None,
         port: typing.Optional[jsii.Number] = None,
         preferred_maintenance_window: typing.Optional[builtins.str] = None,
         publicly_accessible: typing.Optional[builtins.bool] = None,
-        reboot_for_parameter_changes: typing.Optional[builtins.bool] = None,
-        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-        roles: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.IRole]] = None,
-        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+        removal_policy: typing.Optional[aws_cdk.RemovalPolicy] = None,
+        roles: typing.Optional[typing.Sequence[aws_cdk.aws_iam.IRole]] = None,
+        security_groups: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.ISecurityGroup]] = None,
         subnet_group: typing.Optional[IClusterSubnetGroup] = None,
-        vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        vpc_subnets: typing.Optional[aws_cdk.aws_ec2.SubnetSelection] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param master_user: (experimental) Username and password for the administrative user.
         :param vpc: (experimental) The VPC to place the cluster in.
-        :param classic_resizing: (experimental) If this flag is set, the cluster resizing type will be set to classic. When resizing a cluster, classic resizing will always provision a new cluster and transfer the data there. Classic resize takes more time to complete, but it can be useful in cases where the change in node count or the node type to migrate to doesn't fall within the bounds for elastic resize. Default: - Elastic resize type
         :param cluster_name: (experimental) An optional identifier for the cluster. Default: - A name is automatically generated.
-        :param cluster_type: (experimental) Settings for the individual instances that are launched. Default: ``ClusterType.MULTI_NODE``
+        :param cluster_type: (experimental) Settings for the individual instances that are launched. Default: {@link ClusterType.MULTI_NODE}
         :param default_database_name: (experimental) Name of a database which is automatically created inside the cluster. Default: - default_db
-        :param default_role: (experimental) A single AWS Identity and Access Management (IAM) role to be used as the default role for the cluster. The default role must be included in the roles list. Default: - No default role is specified for the cluster.
-        :param elastic_ip: (experimental) The Elastic IP (EIP) address for the cluster. Default: - No Elastic IP
         :param encrypted: (experimental) Whether to enable encryption of data at rest in the cluster. Default: true
         :param encryption_key: (experimental) The KMS key to use for encryption of data at rest. Default: - AWS-managed key, if encryption at rest is enabled
-        :param enhanced_vpc_routing: (experimental) If this flag is set, Amazon Redshift forces all COPY and UNLOAD traffic between your cluster and your data repositories through your virtual private cloud (VPC). Default: - false
-        :param logging_properties: (experimental) Bucket details for log files to be sent to, including prefix. Default: - No logging bucket is used
-        :param node_type: (experimental) The node type to be provisioned for the cluster. Default: ``NodeType.DC2_LARGE``
+        :param logging_bucket: (experimental) Bucket to send logs to. Logging information includes queries and connection attempts, for the specified Amazon Redshift cluster. Default: - No Logs
+        :param logging_key_prefix: (experimental) Prefix used for logging. Default: - no prefix
+        :param node_type: (experimental) The node type to be provisioned for the cluster. Default: {@link NodeType.DC2_LARGE}
         :param number_of_nodes: (experimental) Number of compute nodes in the cluster. Only specify this property for multi-node clusters. Value must be at least 2 and no more than 100. Default: - 2 if ``clusterType`` is ClusterType.MULTI_NODE, undefined otherwise
         :param parameter_group: (experimental) Additional parameters to pass to the database engine https://docs.aws.amazon.com/redshift/latest/mgmt/working-with-parameter-groups.html. Default: - No parameter group.
         :param port: (experimental) What port to listen on. Default: - The default for the engine is used.
         :param preferred_maintenance_window: (experimental) A preferred maintenance window day/time range. Should be specified as a range ddd:hh24:mi-ddd:hh24:mi (24H Clock UTC). Example: 'Sun:23:45-Mon:00:15' Default: - 30-minute window selected at random from an 8-hour block of time for each AWS Region, occurring on a random day of the week.
         :param publicly_accessible: (experimental) Whether to make cluster publicly accessible. Default: false
-        :param reboot_for_parameter_changes: (experimental) If this flag is set, the cluster will be rebooted when changes to the cluster's parameter group that require a restart to apply. Default: false
         :param removal_policy: (experimental) The removal policy to apply when the cluster and its instances are removed from the stack or replaced during an update. Default: RemovalPolicy.RETAIN
-        :param roles: (experimental) A list of AWS Identity and Access Management (IAM) role that can be used by the cluster to access other AWS services. The maximum number of roles to attach to a cluster is subject to a quota. Default: - No role is attached to the cluster.
+        :param roles: (experimental) A list of AWS Identity and Access Management (IAM) role that can be used by the cluster to access other AWS services. Specify a maximum of 10 roles. Default: - No role is attached to the cluster.
         :param security_groups: (experimental) Security group. Default: - a new security group is created.
         :param subnet_group: (experimental) A cluster subnet group to use with this cluster. Default: - a new subnet group will be created.
         :param vpc_subnets: (experimental) Where to place the instances within the VPC. Default: - private subnets
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fccc3c17caf7412d05e4b1ec5aea8d78637d84be2037a887553088f51a674513)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = ClusterProps(
             master_user=master_user,
             vpc=vpc,
-            classic_resizing=classic_resizing,
             cluster_name=cluster_name,
             cluster_type=cluster_type,
             default_database_name=default_database_name,
-            default_role=default_role,
-            elastic_ip=elastic_ip,
             encrypted=encrypted,
             encryption_key=encryption_key,
-            enhanced_vpc_routing=enhanced_vpc_routing,
-            logging_properties=logging_properties,
+            logging_bucket=logging_bucket,
+            logging_key_prefix=logging_key_prefix,
             node_type=node_type,
             number_of_nodes=number_of_nodes,
             parameter_group=parameter_group,
             port=port,
             preferred_maintenance_window=preferred_maintenance_window,
             publicly_accessible=publicly_accessible,
-            reboot_for_parameter_changes=reboot_for_parameter_changes,
             removal_policy=removal_policy,
             roles=roles,
             security_groups=security_groups,
             subnet_group=subnet_group,
             vpc_subnets=vpc_subnets,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromClusterAttributes")
+    @jsii.member(jsii_name="fromClusterAttributes") # type: ignore[misc]
     @builtins.classmethod
     def from_cluster_attributes(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         cluster_endpoint_address: builtins.str,
         cluster_endpoint_port: jsii.Number,
         cluster_name: builtins.str,
-        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+        security_groups: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.ISecurityGroup]] = None,
     ) -> ICluster:
         '''(experimental) Import an existing DatabaseCluster from properties.
 
         :param scope: -
         :param id: -
         :param cluster_endpoint_address: (experimental) Cluster endpoint address.
         :param cluster_endpoint_port: (experimental) Cluster endpoint port.
         :param cluster_name: (experimental) Identifier for the cluster.
         :param security_groups: (experimental) The security groups of the redshift cluster. Default: no security groups will be attached to the import
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__21ba4e3b26d03c0e24d31e65cc9ad3e3adffc0a316cca0f1c80b868747b641b2)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         attrs = ClusterAttributes(
             cluster_endpoint_address=cluster_endpoint_address,
             cluster_endpoint_port=cluster_endpoint_port,
             cluster_name=cluster_name,
             security_groups=security_groups,
         )
 
         return typing.cast(ICluster, jsii.sinvoke(cls, "fromClusterAttributes", [scope, id, attrs]))
 
-    @jsii.member(jsii_name="addDefaultIamRole")
-    def add_default_iam_role(
-        self,
-        default_iam_role: _aws_cdk_aws_iam_ceddda9d.IRole,
-    ) -> None:
-        '''(experimental) Adds default IAM role to cluster.
-
-        The default IAM role must be already associated to the cluster to be added as the default role.
-
-        :param default_iam_role: the IAM role to be set as the default role.
-
-        :stability: experimental
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e07a26bd82e310420fcc9e019333d0a421ad69226414d3d89695ba030672cf77)
-            check_type(argname="argument default_iam_role", value=default_iam_role, expected_type=type_hints["default_iam_role"])
-        return typing.cast(None, jsii.invoke(self, "addDefaultIamRole", [default_iam_role]))
-
-    @jsii.member(jsii_name="addIamRole")
-    def add_iam_role(self, role: _aws_cdk_aws_iam_ceddda9d.IRole) -> None:
-        '''(experimental) Adds a role to the cluster.
-
-        :param role: the role to add.
-
-        :stability: experimental
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8c84ca95ecc8ee9dcc12d23909c7d13bd1e99a1ef01903453c13c9a022f119d3)
-            check_type(argname="argument role", value=role, expected_type=type_hints["role"])
-        return typing.cast(None, jsii.invoke(self, "addIamRole", [role]))
-
     @jsii.member(jsii_name="addRotationMultiUser")
     def add_rotation_multi_user(
         self,
         id: builtins.str,
         *,
-        secret: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
-        automatically_after: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    ) -> _aws_cdk_aws_secretsmanager_ceddda9d.SecretRotation:
+        secret: aws_cdk.aws_secretsmanager.ISecret,
+        automatically_after: typing.Optional[aws_cdk.Duration] = None,
+    ) -> aws_cdk.aws_secretsmanager.SecretRotation:
         '''(experimental) Adds the multi user rotation to this cluster.
 
         :param id: -
         :param secret: (experimental) The secret to rotate. It must be a JSON string with the following format:: { "engine": <required: database engine>, "host": <required: instance host name>, "username": <required: username>, "password": <required: password>, "dbname": <optional: database name>, "port": <optional: if not specified, default port will be used>, "masterarn": <required: the arn of the master secret which will be used to create users/change passwords> }
         :param automatically_after: (experimental) Specifies the number of days after the previous rotation before Secrets Manager triggers the next automatic rotation. Default: Duration.days(30)
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__bf4dc0f78d44545700f0b343e8999f023e1bab7d4f4c865c93cee1f830e805c6)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         options = RotationMultiUserOptions(
             secret=secret, automatically_after=automatically_after
         )
 
-        return typing.cast(_aws_cdk_aws_secretsmanager_ceddda9d.SecretRotation, jsii.invoke(self, "addRotationMultiUser", [id, options]))
+        return typing.cast(aws_cdk.aws_secretsmanager.SecretRotation, jsii.invoke(self, "addRotationMultiUser", [id, options]))
 
     @jsii.member(jsii_name="addRotationSingleUser")
     def add_rotation_single_user(
         self,
-        automatically_after: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-    ) -> _aws_cdk_aws_secretsmanager_ceddda9d.SecretRotation:
+        automatically_after: typing.Optional[aws_cdk.Duration] = None,
+    ) -> aws_cdk.aws_secretsmanager.SecretRotation:
         '''(experimental) Adds the single user rotation of the master password to this cluster.
 
         :param automatically_after: Specifies the number of days after the previous rotation before Secrets Manager triggers the next automatic rotation.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__03bb70e95fdd5ebb0b8ad627b50473d40ac5415a6c45f903e9795e6077987222)
-            check_type(argname="argument automatically_after", value=automatically_after, expected_type=type_hints["automatically_after"])
-        return typing.cast(_aws_cdk_aws_secretsmanager_ceddda9d.SecretRotation, jsii.invoke(self, "addRotationSingleUser", [automatically_after]))
-
-    @jsii.member(jsii_name="addToParameterGroup")
-    def add_to_parameter_group(self, name: builtins.str, value: builtins.str) -> None:
-        '''(experimental) Adds a parameter to the Clusters' parameter group.
-
-        :param name: the parameter name.
-        :param value: the parameter name.
-
-        :stability: experimental
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__385a4ef011525dfc9ad9bd24539b599b93556e101525f1c7a782b6fd5572e5dd)
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        return typing.cast(None, jsii.invoke(self, "addToParameterGroup", [name, value]))
+        return typing.cast(aws_cdk.aws_secretsmanager.SecretRotation, jsii.invoke(self, "addRotationSingleUser", [automatically_after]))
 
     @jsii.member(jsii_name="asSecretAttachmentTarget")
     def as_secret_attachment_target(
         self,
-    ) -> _aws_cdk_aws_secretsmanager_ceddda9d.SecretAttachmentTargetProps:
+    ) -> aws_cdk.aws_secretsmanager.SecretAttachmentTargetProps:
         '''(experimental) Renders the secret attachment target specifications.
 
         :stability: experimental
         '''
-        return typing.cast(_aws_cdk_aws_secretsmanager_ceddda9d.SecretAttachmentTargetProps, jsii.invoke(self, "asSecretAttachmentTarget", []))
-
-    @jsii.member(jsii_name="enableRebootForParameterChanges")
-    def enable_reboot_for_parameter_changes(self) -> None:
-        '''(experimental) Enables automatic cluster rebooting when changes to the cluster's parameter group require a restart to apply.
-
-        :stability: experimental
-        '''
-        return typing.cast(None, jsii.invoke(self, "enableRebootForParameterChanges", []))
+        return typing.cast(aws_cdk.aws_secretsmanager.SecretAttachmentTargetProps, jsii.invoke(self, "asSecretAttachmentTarget", []))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterEndpoint")
     def cluster_endpoint(self) -> Endpoint:
         '''(experimental) The endpoint to use for read/write operations.
 
         :stability: experimental
         '''
         return typing.cast(Endpoint, jsii.get(self, "clusterEndpoint"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterName")
     def cluster_name(self) -> builtins.str:
         '''(experimental) Identifier of the cluster.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "clusterName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="connections")
-    def connections(self) -> _aws_cdk_aws_ec2_ceddda9d.Connections:
+    def connections(self) -> aws_cdk.aws_ec2.Connections:
         '''(experimental) Access to the network connections.
 
         :stability: experimental
         '''
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.Connections, jsii.get(self, "connections"))
+        return typing.cast(aws_cdk.aws_ec2.Connections, jsii.get(self, "connections"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="secret")
-    def secret(self) -> typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret]:
+    def secret(self) -> typing.Optional[aws_cdk.aws_secretsmanager.ISecret]:
         '''(experimental) The secret attached to this cluster.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret], jsii.get(self, "secret"))
-
-    @builtins.property
-    @jsii.member(jsii_name="parameterGroup")
-    def _parameter_group(self) -> typing.Optional[IClusterParameterGroup]:
-        '''(experimental) The cluster's parameter group.
-
-        :stability: experimental
-        '''
-        return typing.cast(typing.Optional[IClusterParameterGroup], jsii.get(self, "parameterGroup"))
-
-    @_parameter_group.setter
-    def _parameter_group(self, value: typing.Optional[IClusterParameterGroup]) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2c00f21b389b078f00b9e115501d7de9d004e75c209153d409b6968d062b1b36)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "parameterGroup", value)
+        return typing.cast(typing.Optional[aws_cdk.aws_secretsmanager.ISecret], jsii.get(self, "secret"))
 
 
 @jsii.implements(IClusterParameterGroup)
 class ClusterParameterGroup(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-redshift-alpha.ClusterParameterGroup",
 ):
     '''(experimental) A cluster parameter group.
 
     :stability: experimental
     :resource: AWS::Redshift::ClusterParameterGroup
-    :exampleMetadata: infused
+    :exampleMetadata: fixture=_generated
 
     Example::
 
-        from aws_cdk.aws_redshift_alpha import ClusterParameterGroup
-        
+        # The code below shows an example of how to instantiate this type.
+        # The values are placeholders you should change.
+        import aws_cdk.aws_redshift_alpha as redshift_alpha
         
-        params = ClusterParameterGroup(self, "Params",
-            description="desc",
+        cluster_parameter_group = redshift_alpha.ClusterParameterGroup(self, "MyClusterParameterGroup",
             parameters={
-                "require_ssl": "true"
-            }
-        )
+                "parameters_key": "parameters"
+            },
         
-        params.add_parameter("enable_user_activity_logging", "true")
+            # the properties below are optional
+            description="description"
+        )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         parameters: typing.Mapping[builtins.str, builtins.str],
         description: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param parameters: (experimental) The parameters in this parameter group.
         :param description: (experimental) Description for this parameter group. Default: a CDK generated description
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__80dbeaae7ee868dc2230702ef3076156af6847871ef2c2eb597bfde0e375aaf9)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = ClusterParameterGroupProps(
             parameters=parameters, description=description
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromClusterParameterGroupName")
+    @jsii.member(jsii_name="fromClusterParameterGroupName") # type: ignore[misc]
     @builtins.classmethod
     def from_cluster_parameter_group_name(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         cluster_parameter_group_name: builtins.str,
     ) -> IClusterParameterGroup:
         '''(experimental) Imports a parameter group.
 
         :param scope: -
         :param id: -
         :param cluster_parameter_group_name: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__21b8bc608c922439ec081fe8fb6d01595015b6b8871356bcf580d553b2414bbd)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument cluster_parameter_group_name", value=cluster_parameter_group_name, expected_type=type_hints["cluster_parameter_group_name"])
         return typing.cast(IClusterParameterGroup, jsii.sinvoke(cls, "fromClusterParameterGroupName", [scope, id, cluster_parameter_group_name]))
 
-    @jsii.member(jsii_name="addParameter")
-    def add_parameter(self, name: builtins.str, value: builtins.str) -> None:
-        '''(experimental) Adds a parameter to the parameter group.
-
-        :param name: the parameter name.
-        :param value: the parameter name.
-
-        :stability: experimental
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1b52f6296bee4a32ac8e0a689f5aaf7f963573580c0a50a36e73ab367ef30972)
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        return typing.cast(None, jsii.invoke(self, "addParameter", [name, value]))
-
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterParameterGroupName")
     def cluster_parameter_group_name(self) -> builtins.str:
         '''(experimental) The name of the parameter group.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "clusterParameterGroupName"))
 
-    @builtins.property
-    @jsii.member(jsii_name="parameters")
-    def parameters(self) -> typing.Mapping[builtins.str, builtins.str]:
-        '''(experimental) The parameters in the parameter group.
-
-        :stability: experimental
-        '''
-        return typing.cast(typing.Mapping[builtins.str, builtins.str], jsii.get(self, "parameters"))
-
 
 @jsii.implements(IClusterSubnetGroup)
 class ClusterSubnetGroup(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-redshift-alpha.ClusterSubnetGroup",
 ):
     '''(experimental) Class for creating a Redshift cluster subnet group.
 
     :stability: experimental
     :resource: AWS::Redshift::ClusterSubnetGroup
@@ -4285,69 +3346,60 @@
                 subnet_type=ec2.SubnetType.PRIVATE_ISOLATED
             )
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         description: builtins.str,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-        vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        vpc: aws_cdk.aws_ec2.IVpc,
+        removal_policy: typing.Optional[aws_cdk.RemovalPolicy] = None,
+        vpc_subnets: typing.Optional[aws_cdk.aws_ec2.SubnetSelection] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param description: (experimental) Description of the subnet group.
         :param vpc: (experimental) The VPC to place the subnet group in.
         :param removal_policy: (experimental) The removal policy to apply when the subnet group are removed from the stack or replaced during an update. Default: RemovalPolicy.RETAIN
         :param vpc_subnets: (experimental) Which subnets within the VPC to associate with this group. Default: - private subnets
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__79715a97708d01deffdb6c0c2d2b81d1557e42dd639377201ff24e05b2d61e31)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = ClusterSubnetGroupProps(
             description=description,
             vpc=vpc,
             removal_policy=removal_policy,
             vpc_subnets=vpc_subnets,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromClusterSubnetGroupName")
+    @jsii.member(jsii_name="fromClusterSubnetGroupName") # type: ignore[misc]
     @builtins.classmethod
     def from_cluster_subnet_group_name(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         cluster_subnet_group_name: builtins.str,
     ) -> IClusterSubnetGroup:
         '''(experimental) Imports an existing subnet group by name.
 
         :param scope: -
         :param id: -
         :param cluster_subnet_group_name: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__97ed1ec988c1a6d07ef8bd188169b6e2968b52d6809c0d69c1300f758e2539dc)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument cluster_subnet_group_name", value=cluster_subnet_group_name, expected_type=type_hints["cluster_subnet_group_name"])
         return typing.cast(IClusterSubnetGroup, jsii.sinvoke(cls, "fromClusterSubnetGroupName", [scope, id, cluster_subnet_group_name]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="clusterSubnetGroupName")
     def cluster_subnet_group_name(self) -> builtins.str:
         '''(experimental) The name of the cluster subnet group.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "clusterSubnetGroupName"))
@@ -4359,25 +3411,23 @@
     "ClusterParameterGroup",
     "ClusterParameterGroupProps",
     "ClusterProps",
     "ClusterSubnetGroup",
     "ClusterSubnetGroupProps",
     "ClusterType",
     "Column",
-    "ColumnEncoding",
     "DatabaseOptions",
     "DatabaseSecret",
     "DatabaseSecretProps",
     "Endpoint",
     "ICluster",
     "IClusterParameterGroup",
     "IClusterSubnetGroup",
     "ITable",
     "IUser",
-    "LoggingProperties",
     "Login",
     "NodeType",
     "RotationMultiUserOptions",
     "Table",
     "TableAction",
     "TableAttributes",
     "TableDistStyle",
@@ -4385,416 +3435,7 @@
     "TableSortStyle",
     "User",
     "UserAttributes",
     "UserProps",
 ]
 
 publication.publish()
-
-def _typecheckingstub__cf5e43f35a05f5c5658f39bc00260eed640e4a1a644169632c3ab77941eded83(
-    *,
-    cluster_endpoint_address: builtins.str,
-    cluster_endpoint_port: jsii.Number,
-    cluster_name: builtins.str,
-    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__cb07da80fc73b7c25808e76fda84dcebec84019d464cfe8908504bd326b69e87(
-    *,
-    parameters: typing.Mapping[builtins.str, builtins.str],
-    description: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__8184b6f381b827fb337da7fe46dcdf07d3411d00c00a966acf72f7524193e365(
-    *,
-    master_user: typing.Union[Login, typing.Dict[builtins.str, typing.Any]],
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-    classic_resizing: typing.Optional[builtins.bool] = None,
-    cluster_name: typing.Optional[builtins.str] = None,
-    cluster_type: typing.Optional[ClusterType] = None,
-    default_database_name: typing.Optional[builtins.str] = None,
-    default_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-    elastic_ip: typing.Optional[builtins.str] = None,
-    encrypted: typing.Optional[builtins.bool] = None,
-    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-    enhanced_vpc_routing: typing.Optional[builtins.bool] = None,
-    logging_properties: typing.Optional[typing.Union[LoggingProperties, typing.Dict[builtins.str, typing.Any]]] = None,
-    node_type: typing.Optional[NodeType] = None,
-    number_of_nodes: typing.Optional[jsii.Number] = None,
-    parameter_group: typing.Optional[IClusterParameterGroup] = None,
-    port: typing.Optional[jsii.Number] = None,
-    preferred_maintenance_window: typing.Optional[builtins.str] = None,
-    publicly_accessible: typing.Optional[builtins.bool] = None,
-    reboot_for_parameter_changes: typing.Optional[builtins.bool] = None,
-    removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-    roles: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.IRole]] = None,
-    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-    subnet_group: typing.Optional[IClusterSubnetGroup] = None,
-    vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__d4e8f5beb5d0b96f6d62d9dc9f2e62c24bedea9a666fc29101e682e182fb215a(
-    *,
-    description: builtins.str,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-    removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-    vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__32216f4dee559bc797af2f48171aa04cf72e7a5ff7495657331f2098b799968d(
-    *,
-    data_type: builtins.str,
-    name: builtins.str,
-    comment: typing.Optional[builtins.str] = None,
-    dist_key: typing.Optional[builtins.bool] = None,
-    encoding: typing.Optional[ColumnEncoding] = None,
-    id: typing.Optional[builtins.str] = None,
-    sort_key: typing.Optional[builtins.bool] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__6fe4c22044df6e55f8af7e726bd1ff39590ed6b0ad6f13efc5dcf977502c0b7b(
-    *,
-    cluster: ICluster,
-    database_name: builtins.str,
-    admin_user: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__984b48cb3b4940dc6b6d9cdce4c356224668b8a25e815f08a9d2475010ddc7f7(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    username: builtins.str,
-    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__6c5db30f831b907067d91296ccc68bfe4767f2efe09ae877fe203adb5df73e42(
-    *,
-    username: builtins.str,
-    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__9156a39d8268aff7d98d3e261bceea1730546d85f7f12d19efdada7e91b09890(
-    address: builtins.str,
-    port: jsii.Number,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__febfab9a8c6f0c1f081d5f0f1dd5fb2ba403be29fbe7dcef6e4fffb955b09c77(
-    user: IUser,
-    *actions: TableAction,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__482349d4a650668e65613cc4cb7308f07f28faff85e9f7754c08cde21ac2e7fb(
-    table: ITable,
-    *actions: TableAction,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__31bfca026b86708f38bf1964cd5ab577729657ca2c1adbb4f4c27e417cbd7b99(
-    *,
-    logging_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
-    logging_key_prefix: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__f290e69c40e3c1e3b75f41243f96283d1619e3967c3b2bd3458c974e11b7f430(
-    *,
-    master_username: builtins.str,
-    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-    master_password: typing.Optional[_aws_cdk_ceddda9d.SecretValue] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e8ff1dc8f069ed8db9a6c9c88c8b732a109f9c9198fa3b3df5acbb57173d041d(
-    *,
-    secret: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
-    automatically_after: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__f5bb5cdc9b9d71db081569ce1699ad72f4cda1e74e44ad08c8dfcaa831d2ecfb(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    table_columns: typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]],
-    dist_style: typing.Optional[TableDistStyle] = None,
-    removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-    sort_style: typing.Optional[TableSortStyle] = None,
-    table_comment: typing.Optional[builtins.str] = None,
-    table_name: typing.Optional[builtins.str] = None,
-    cluster: ICluster,
-    database_name: builtins.str,
-    admin_user: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__c588c15b59523c46188be2ed268598c40457a45f5ae6af6ee90f43398b2a87c6(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    cluster: ICluster,
-    database_name: builtins.str,
-    table_columns: typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]],
-    table_name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__7a2559de86af99b035e3551696efbd323c09454e4966d219dbac73eb0ecbbc26(
-    policy: _aws_cdk_ceddda9d.RemovalPolicy,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__2cedd8e4ce5ed742b7998abe8c2f47aca8c358cbec88a746c68669950dbfcf79(
-    user: IUser,
-    *actions: TableAction,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a72be394d5e035726f67dcce82f498875671e673396787b30bed1cb67dd061c8(
-    *,
-    cluster: ICluster,
-    database_name: builtins.str,
-    table_columns: typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]],
-    table_name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__2d4444361722818dd5438346bad361ad93c2f629efde6c384600398f4b5051b2(
-    *,
-    cluster: ICluster,
-    database_name: builtins.str,
-    admin_user: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
-    table_columns: typing.Sequence[typing.Union[Column, typing.Dict[builtins.str, typing.Any]]],
-    dist_style: typing.Optional[TableDistStyle] = None,
-    removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-    sort_style: typing.Optional[TableSortStyle] = None,
-    table_comment: typing.Optional[builtins.str] = None,
-    table_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__684a841e4fc7788170b0197fb7931e6c62bd55d596af8e0196b42df62e434ea4(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-    removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-    username: typing.Optional[builtins.str] = None,
-    cluster: ICluster,
-    database_name: builtins.str,
-    admin_user: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__483704cbd1ddd53dbc57f757961a2e3d53ae948da0d8d8f8e8d50b847958dfd6(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    password: _aws_cdk_ceddda9d.SecretValue,
-    username: builtins.str,
-    cluster: ICluster,
-    database_name: builtins.str,
-    admin_user: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__9c310d0b8092d0aef06348ff2e68c7aa7577648c18e7656284f491091331d877(
-    table: ITable,
-    *actions: TableAction,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e783176cde66b005bd7a48047c42d2daa161b7fbf0608fd8c280193b160dc7f9(
-    policy: _aws_cdk_ceddda9d.RemovalPolicy,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__215d4d48a362ca590c122ef61d7450d160371decc86d4e5977bce6a23d0ca17f(
-    value: DatabaseOptions,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__939764949bce87bd8dcf6ede326ec239f6dd7c2b716dbb9e552964fdc8d62557(
-    *,
-    cluster: ICluster,
-    database_name: builtins.str,
-    admin_user: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
-    password: _aws_cdk_ceddda9d.SecretValue,
-    username: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0daf47fb2a97e4e73621e19347c149764ca3c3592695c3501419bf0d6e79cbd2(
-    *,
-    cluster: ICluster,
-    database_name: builtins.str,
-    admin_user: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
-    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-    removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-    username: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__fccc3c17caf7412d05e4b1ec5aea8d78637d84be2037a887553088f51a674513(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    master_user: typing.Union[Login, typing.Dict[builtins.str, typing.Any]],
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-    classic_resizing: typing.Optional[builtins.bool] = None,
-    cluster_name: typing.Optional[builtins.str] = None,
-    cluster_type: typing.Optional[ClusterType] = None,
-    default_database_name: typing.Optional[builtins.str] = None,
-    default_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-    elastic_ip: typing.Optional[builtins.str] = None,
-    encrypted: typing.Optional[builtins.bool] = None,
-    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-    enhanced_vpc_routing: typing.Optional[builtins.bool] = None,
-    logging_properties: typing.Optional[typing.Union[LoggingProperties, typing.Dict[builtins.str, typing.Any]]] = None,
-    node_type: typing.Optional[NodeType] = None,
-    number_of_nodes: typing.Optional[jsii.Number] = None,
-    parameter_group: typing.Optional[IClusterParameterGroup] = None,
-    port: typing.Optional[jsii.Number] = None,
-    preferred_maintenance_window: typing.Optional[builtins.str] = None,
-    publicly_accessible: typing.Optional[builtins.bool] = None,
-    reboot_for_parameter_changes: typing.Optional[builtins.bool] = None,
-    removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-    roles: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.IRole]] = None,
-    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-    subnet_group: typing.Optional[IClusterSubnetGroup] = None,
-    vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__21ba4e3b26d03c0e24d31e65cc9ad3e3adffc0a316cca0f1c80b868747b641b2(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    cluster_endpoint_address: builtins.str,
-    cluster_endpoint_port: jsii.Number,
-    cluster_name: builtins.str,
-    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e07a26bd82e310420fcc9e019333d0a421ad69226414d3d89695ba030672cf77(
-    default_iam_role: _aws_cdk_aws_iam_ceddda9d.IRole,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__8c84ca95ecc8ee9dcc12d23909c7d13bd1e99a1ef01903453c13c9a022f119d3(
-    role: _aws_cdk_aws_iam_ceddda9d.IRole,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__bf4dc0f78d44545700f0b343e8999f023e1bab7d4f4c865c93cee1f830e805c6(
-    id: builtins.str,
-    *,
-    secret: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
-    automatically_after: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__03bb70e95fdd5ebb0b8ad627b50473d40ac5415a6c45f903e9795e6077987222(
-    automatically_after: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__385a4ef011525dfc9ad9bd24539b599b93556e101525f1c7a782b6fd5572e5dd(
-    name: builtins.str,
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__2c00f21b389b078f00b9e115501d7de9d004e75c209153d409b6968d062b1b36(
-    value: typing.Optional[IClusterParameterGroup],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__80dbeaae7ee868dc2230702ef3076156af6847871ef2c2eb597bfde0e375aaf9(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    parameters: typing.Mapping[builtins.str, builtins.str],
-    description: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__21b8bc608c922439ec081fe8fb6d01595015b6b8871356bcf580d553b2414bbd(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    cluster_parameter_group_name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__1b52f6296bee4a32ac8e0a689f5aaf7f963573580c0a50a36e73ab367ef30972(
-    name: builtins.str,
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__79715a97708d01deffdb6c0c2d2b81d1557e42dd639377201ff24e05b2d61e31(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    description: builtins.str,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-    removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-    vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__97ed1ec988c1a6d07ef8bd188169b6e2968b52d6809c0d69c1300f758e2539dc(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    cluster_subnet_group_name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
```

### Comparing `aws-cdk.aws-redshift-alpha-2.84.0a0/src/aws_cdk.aws_redshift_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-redshift-alpha-2.9.0a0/src/aws_cdk.aws_redshift_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_redshift_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_redshift_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_redshift_alpha.egg-info/requires.txt
 src/aws_cdk.aws_redshift_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_redshift_alpha/__init__.py
 src/aws_cdk/aws_redshift_alpha/py.typed
 src/aws_cdk/aws_redshift_alpha/_jsii/__init__.py
-src/aws_cdk/aws_redshift_alpha/_jsii/aws-redshift-alpha@2.84.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_redshift_alpha/_jsii/aws-redshift-alpha@2.9.0-alpha.0.jsii.tgz
```

