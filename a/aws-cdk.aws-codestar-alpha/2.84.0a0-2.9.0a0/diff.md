# Comparing `tmp/aws-cdk.aws-codestar-alpha-2.84.0a0.tar.gz` & `tmp/aws-cdk.aws-codestar-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/aws-codestar-alpha/dist/python/aws-cdk.aws-codestar-alpha-2.84.0a0.tar", last modified: Tue Jun 13 23:46:45 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-codestar/dist/python/aws-cdk.aws-codestar-alpha-2.9.0a0.tar", last modified: Wed Jan 26 11:22:04 2022, max compression
```

## Comparing `aws-cdk.aws-codestar-alpha-2.84.0a0.tar` & `aws-cdk.aws-codestar-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:37.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:37.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 23:46:37.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     2488 2023-06-13 23:46:45.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1485 2023-06-13 23:46:37.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:37.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:46:45.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1877 2023-06-13 23:46:37.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/src/aws_cdk/aws_codestar_alpha/
--rw-r--r--   0 root         (0) root         (0)    18998 2023-06-13 23:46:37.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/src/aws_cdk/aws_codestar_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/src/aws_cdk/aws_codestar_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      443 2023-06-13 23:46:37.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/src/aws_cdk/aws_codestar_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22514 2023-06-13 23:46:37.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/src/aws_cdk/aws_codestar_alpha/_jsii/aws-codestar-alpha@2.84.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:37.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/src/aws_cdk/aws_codestar_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2488 2023-06-13 23:46:45.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      541 2023-06-13 23:46:45.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:45.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-13 23:46:45.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:46:45.000000 aws-cdk.aws-codestar-alpha-2.84.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:04.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:01.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     2541 2022-01-26 11:22:04.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1571 2022-01-26 11:22:01.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:04.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1802 2022-01-26 11:22:01.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:04.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:04.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:04.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/src/aws_cdk/aws_codestar_alpha/
+-rw-r--r--   0 root         (0) root         (0)    16355 2022-01-26 11:22:01.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/src/aws_cdk/aws_codestar_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:04.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/src/aws_cdk/aws_codestar_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      407 2022-01-26 11:22:01.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/src/aws_cdk/aws_codestar_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19168 2022-01-26 11:22:01.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/src/aws_cdk/aws_codestar_alpha/_jsii/aws-codestar-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/src/aws_cdk/aws_codestar_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:04.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2541 2022-01-26 11:22:04.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      540 2022-01-26 11:22:04.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:04.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:04.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:04.000000 aws-cdk.aws-codestar-alpha-2.9.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-codestar-alpha-2.84.0a0/LICENSE` & `aws-cdk.aws-codestar-alpha-2.9.0a0/LICENSE`

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

### Comparing `aws-cdk.aws-codestar-alpha-2.84.0a0/PKG-INFO` & `aws-cdk.aws-codestar-alpha-2.9.0a0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-codestar-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::CodeStar
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
 
 # AWS::CodeStar Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -42,25 +42,27 @@
 <!--END STABILITY BANNER-->
 
 ## GitHub Repository
 
 To create a new GitHub Repository and commit the assets from S3 bucket into the repository after it is created:
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 import aws_cdk.aws_codestar_alpha as codestar
 import aws_cdk.aws_s3 as s3
 
-
-codestar.GitHubRepository(self, "GitHubRepo",
+codestar.GitHubRepository(stack, "GitHubRepo",
     owner="aws",
     repository_name="aws-cdk",
-    access_token=SecretValue.secrets_manager("my-github-token",
+    access_token=cdk.SecretValue.secrets_manager("my-github-token",
         json_field="token"
     ),
-    contents_bucket=s3.Bucket.from_bucket_name(self, "Bucket", "bucket-name"),
+    contents_bucket=s3.Bucket.from_bucket_name(stack, "Bucket", "bucket-name"),
     contents_key="import.zip"
 )
 ```
 
 ## Update or Delete the GitHubRepository
 
 At this moment, updates to the `GitHubRepository` are not supported and the repository will not be deleted upon the deletion of the CloudFormation stack. You will need to update or delete the GitHub repository manually.
+
+
```

### Comparing `aws-cdk.aws-codestar-alpha-2.84.0a0/README.md` & `aws-cdk.aws-codestar-alpha-2.9.0a0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 <!--END STABILITY BANNER-->
 
 ## GitHub Repository
 
 To create a new GitHub Repository and commit the assets from S3 bucket into the repository after it is created:
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 import aws_cdk.aws_codestar_alpha as codestar
 import aws_cdk.aws_s3 as s3
 
-
-codestar.GitHubRepository(self, "GitHubRepo",
+codestar.GitHubRepository(stack, "GitHubRepo",
     owner="aws",
     repository_name="aws-cdk",
-    access_token=SecretValue.secrets_manager("my-github-token",
+    access_token=cdk.SecretValue.secrets_manager("my-github-token",
         json_field="token"
     ),
-    contents_bucket=s3.Bucket.from_bucket_name(self, "Bucket", "bucket-name"),
+    contents_bucket=s3.Bucket.from_bucket_name(stack, "Bucket", "bucket-name"),
     contents_key="import.zip"
 )
 ```
 
 ## Update or Delete the GitHubRepository
 
 At this moment, updates to the `GitHubRepository` are not supported and the repository will not be deleted upon the deletion of the CloudFormation stack. You will need to update or delete the GitHub repository manually.
```

### Comparing `aws-cdk.aws-codestar-alpha-2.84.0a0/setup.py` & `aws-cdk.aws-codestar-alpha-2.9.0a0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-codestar-alpha",
-    "version": "2.84.0.a0",
+    "version": "2.9.0.a0",
     "description": "The CDK Construct Library for AWS::CodeStar",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,43 +22,41 @@
     },
     "packages": [
         "aws_cdk.aws_codestar_alpha",
         "aws_cdk.aws_codestar_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_codestar_alpha._jsii": [
-            "aws-codestar-alpha@2.84.0-alpha.0.jsii.tgz"
+            "aws-codestar-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_codestar_alpha": [
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

### Comparing `aws-cdk.aws-codestar-alpha-2.84.0a0/src/aws_cdk/aws_codestar_alpha/__init__.py` & `aws-cdk.aws-codestar-alpha-2.9.0a0/src/aws_cdk/aws_codestar_alpha/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 <!--END STABILITY BANNER-->
 
 ## GitHub Repository
 
 To create a new GitHub Repository and commit the assets from S3 bucket into the repository after it is created:
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 import aws_cdk.aws_codestar_alpha as codestar
 import aws_cdk.aws_s3 as s3
 
-
-codestar.GitHubRepository(self, "GitHubRepo",
+codestar.GitHubRepository(stack, "GitHubRepo",
     owner="aws",
     repository_name="aws-cdk",
-    access_token=SecretValue.secrets_manager("my-github-token",
+    access_token=cdk.SecretValue.secrets_manager("my-github-token",
         json_field="token"
     ),
-    contents_bucket=s3.Bucket.from_bucket_name(self, "Bucket", "bucket-name"),
+    contents_bucket=s3.Bucket.from_bucket_name(stack, "Bucket", "bucket-name"),
     contents_key="import.zip"
 )
 ```
 
 ## Update or Delete the GitHubRepository
 
 At this moment, updates to the `GitHubRepository` are not supported and the repository will not be deleted upon the deletion of the CloudFormation stack. You will need to update or delete the GitHub repository manually.
@@ -45,21 +45,19 @@
 import enum
 import typing
 
 import jsii
 import publication
 import typing_extensions
 
-from typeguard import check_type
-
 from ._jsii import *
 
-import aws_cdk as _aws_cdk_ceddda9d
-import aws_cdk.aws_s3 as _aws_cdk_aws_s3_ceddda9d
-import constructs as _constructs_77d1e7e8
+import aws_cdk
+import aws_cdk.aws_s3
+import constructs
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-codestar-alpha.GitHubRepositoryProps",
     jsii_struct_bases=[],
     name_mapping={
         "access_token": "accessToken",
@@ -73,25 +71,25 @@
         "visibility": "visibility",
     },
 )
 class GitHubRepositoryProps:
     def __init__(
         self,
         *,
-        access_token: _aws_cdk_ceddda9d.SecretValue,
-        contents_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        access_token: aws_cdk.SecretValue,
+        contents_bucket: aws_cdk.aws_s3.IBucket,
         contents_key: builtins.str,
         owner: builtins.str,
         repository_name: builtins.str,
         contents_s3_version: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         enable_issues: typing.Optional[builtins.bool] = None,
         visibility: typing.Optional["RepositoryVisibility"] = None,
     ) -> None:
-        '''(experimental) Construction properties of ``GitHubRepository``.
+        '''(experimental) Construction properties of {@link GitHubRepository}.
 
         :param access_token: (experimental) The GitHub user's personal access token for the GitHub repository.
         :param contents_bucket: (experimental) The name of the Amazon S3 bucket that contains the ZIP file with the content to be committed to the new repository.
         :param contents_key: (experimental) The S3 object key or file name for the ZIP file.
         :param owner: (experimental) The GitHub user name for the owner of the GitHub repository to be created. If this repository should be owned by a GitHub organization, provide its name
         :param repository_name: (experimental) The name of the repository you want to create in GitHub with AWS CloudFormation stack creation.
         :param contents_s3_version: (experimental) The object version of the ZIP file, if versioning is enabled for the Amazon S3 bucket. Default: - not specified
@@ -100,40 +98,29 @@
         :param visibility: (experimental) Indicates whether the GitHub repository is a private repository. If so, you choose who can see and commit to this repository. Default: RepositoryVisibility.PUBLIC
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
+            # Example automatically generated from non-compiling source. May contain errors.
             import aws_cdk.aws_codestar_alpha as codestar
             import aws_cdk.aws_s3 as s3
             
-            
-            codestar.GitHubRepository(self, "GitHubRepo",
+            codestar.GitHubRepository(stack, "GitHubRepo",
                 owner="aws",
                 repository_name="aws-cdk",
-                access_token=SecretValue.secrets_manager("my-github-token",
+                access_token=cdk.SecretValue.secrets_manager("my-github-token",
                     json_field="token"
                 ),
-                contents_bucket=s3.Bucket.from_bucket_name(self, "Bucket", "bucket-name"),
+                contents_bucket=s3.Bucket.from_bucket_name(stack, "Bucket", "bucket-name"),
                 contents_key="import.zip"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c848afd2b589eccc9fe7fdbeff1681e2af3dab8477fed31f0d8bfb02ca05e0df)
-            check_type(argname="argument access_token", value=access_token, expected_type=type_hints["access_token"])
-            check_type(argname="argument contents_bucket", value=contents_bucket, expected_type=type_hints["contents_bucket"])
-            check_type(argname="argument contents_key", value=contents_key, expected_type=type_hints["contents_key"])
-            check_type(argname="argument owner", value=owner, expected_type=type_hints["owner"])
-            check_type(argname="argument repository_name", value=repository_name, expected_type=type_hints["repository_name"])
-            check_type(argname="argument contents_s3_version", value=contents_s3_version, expected_type=type_hints["contents_s3_version"])
-            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
-            check_type(argname="argument enable_issues", value=enable_issues, expected_type=type_hints["enable_issues"])
-            check_type(argname="argument visibility", value=visibility, expected_type=type_hints["visibility"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "access_token": access_token,
             "contents_bucket": contents_bucket,
             "contents_key": contents_key,
             "owner": owner,
             "repository_name": repository_name,
         }
         if contents_s3_version is not None:
@@ -142,32 +129,32 @@
             self._values["description"] = description
         if enable_issues is not None:
             self._values["enable_issues"] = enable_issues
         if visibility is not None:
             self._values["visibility"] = visibility
 
     @builtins.property
-    def access_token(self) -> _aws_cdk_ceddda9d.SecretValue:
+    def access_token(self) -> aws_cdk.SecretValue:
         '''(experimental) The GitHub user's personal access token for the GitHub repository.
 
         :stability: experimental
         '''
         result = self._values.get("access_token")
         assert result is not None, "Required property 'access_token' is missing"
-        return typing.cast(_aws_cdk_ceddda9d.SecretValue, result)
+        return typing.cast(aws_cdk.SecretValue, result)
 
     @builtins.property
-    def contents_bucket(self) -> _aws_cdk_aws_s3_ceddda9d.IBucket:
+    def contents_bucket(self) -> aws_cdk.aws_s3.IBucket:
         '''(experimental) The name of the Amazon S3 bucket that contains the ZIP file with the content to be committed to the new repository.
 
         :stability: experimental
         '''
         result = self._values.get("contents_bucket")
         assert result is not None, "Required property 'contents_bucket' is missing"
-        return typing.cast(_aws_cdk_aws_s3_ceddda9d.IBucket, result)
+        return typing.cast(aws_cdk.aws_s3.IBucket, result)
 
     @builtins.property
     def contents_key(self) -> builtins.str:
         '''(experimental) The S3 object key or file name for the ZIP file.
 
         :stability: experimental
         '''
@@ -260,59 +247,59 @@
     def __repr__(self) -> str:
         return "GitHubRepositoryProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-codestar-alpha.IGitHubRepository")
-class IGitHubRepository(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class IGitHubRepository(aws_cdk.IResource, typing_extensions.Protocol):
     '''(experimental) GitHubRepository resource interface.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="owner")
     def owner(self) -> builtins.str:
         '''(experimental) the repository owner.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="repo")
     def repo(self) -> builtins.str:
         '''(experimental) the repository name.
 
         :stability: experimental
         '''
         ...
 
 
 class _IGitHubRepositoryProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''(experimental) GitHubRepository resource interface.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-codestar-alpha.IGitHubRepository"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="owner")
     def owner(self) -> builtins.str:
         '''(experimental) the repository owner.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "owner"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="repo")
     def repo(self) -> builtins.str:
         '''(experimental) the repository name.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "repo"))
@@ -338,47 +325,47 @@
 
     :stability: experimental
     '''
 
 
 @jsii.implements(IGitHubRepository)
 class GitHubRepository(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-codestar-alpha.GitHubRepository",
 ):
     '''(experimental) The GitHubRepository resource.
 
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
+        # Example automatically generated from non-compiling source. May contain errors.
         import aws_cdk.aws_codestar_alpha as codestar
         import aws_cdk.aws_s3 as s3
         
-        
-        codestar.GitHubRepository(self, "GitHubRepo",
+        codestar.GitHubRepository(stack, "GitHubRepo",
             owner="aws",
             repository_name="aws-cdk",
-            access_token=SecretValue.secrets_manager("my-github-token",
+            access_token=cdk.SecretValue.secrets_manager("my-github-token",
                 json_field="token"
             ),
-            contents_bucket=s3.Bucket.from_bucket_name(self, "Bucket", "bucket-name"),
+            contents_bucket=s3.Bucket.from_bucket_name(stack, "Bucket", "bucket-name"),
             contents_key="import.zip"
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
-        access_token: _aws_cdk_ceddda9d.SecretValue,
-        contents_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        access_token: aws_cdk.SecretValue,
+        contents_bucket: aws_cdk.aws_s3.IBucket,
         contents_key: builtins.str,
         owner: builtins.str,
         repository_name: builtins.str,
         contents_s3_version: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         enable_issues: typing.Optional[builtins.bool] = None,
         visibility: typing.Optional[RepositoryVisibility] = None,
@@ -394,42 +381,38 @@
         :param contents_s3_version: (experimental) The object version of the ZIP file, if versioning is enabled for the Amazon S3 bucket. Default: - not specified
         :param description: (experimental) A comment or description about the new repository. This description is displayed in GitHub after the repository is created. Default: - no description
         :param enable_issues: (experimental) Indicates whether to enable issues for the GitHub repository. You can use GitHub issues to track information and bugs for your repository. Default: true
         :param visibility: (experimental) Indicates whether the GitHub repository is a private repository. If so, you choose who can see and commit to this repository. Default: RepositoryVisibility.PUBLIC
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9532a574e633c6d68e3daa0a175cb9309cb6a09badef5107c2a79a31d721ba10)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = GitHubRepositoryProps(
             access_token=access_token,
             contents_bucket=contents_bucket,
             contents_key=contents_key,
             owner=owner,
             repository_name=repository_name,
             contents_s3_version=contents_s3_version,
             description=description,
             enable_issues=enable_issues,
             visibility=visibility,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="owner")
     def owner(self) -> builtins.str:
         '''(experimental) the repository owner.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "owner"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="repo")
     def repo(self) -> builtins.str:
         '''(experimental) the repository name.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "repo"))
@@ -439,39 +422,7 @@
     "GitHubRepository",
     "GitHubRepositoryProps",
     "IGitHubRepository",
     "RepositoryVisibility",
 ]
 
 publication.publish()
-
-def _typecheckingstub__c848afd2b589eccc9fe7fdbeff1681e2af3dab8477fed31f0d8bfb02ca05e0df(
-    *,
-    access_token: _aws_cdk_ceddda9d.SecretValue,
-    contents_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
-    contents_key: builtins.str,
-    owner: builtins.str,
-    repository_name: builtins.str,
-    contents_s3_version: typing.Optional[builtins.str] = None,
-    description: typing.Optional[builtins.str] = None,
-    enable_issues: typing.Optional[builtins.bool] = None,
-    visibility: typing.Optional[RepositoryVisibility] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__9532a574e633c6d68e3daa0a175cb9309cb6a09badef5107c2a79a31d721ba10(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    access_token: _aws_cdk_ceddda9d.SecretValue,
-    contents_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
-    contents_key: builtins.str,
-    owner: builtins.str,
-    repository_name: builtins.str,
-    contents_s3_version: typing.Optional[builtins.str] = None,
-    description: typing.Optional[builtins.str] = None,
-    enable_issues: typing.Optional[builtins.bool] = None,
-    visibility: typing.Optional[RepositoryVisibility] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
```

### Comparing `aws-cdk.aws-codestar-alpha-2.84.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-codestar-alpha-2.9.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-codestar-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::CodeStar
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
 
 # AWS::CodeStar Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -42,25 +42,27 @@
 <!--END STABILITY BANNER-->
 
 ## GitHub Repository
 
 To create a new GitHub Repository and commit the assets from S3 bucket into the repository after it is created:
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 import aws_cdk.aws_codestar_alpha as codestar
 import aws_cdk.aws_s3 as s3
 
-
-codestar.GitHubRepository(self, "GitHubRepo",
+codestar.GitHubRepository(stack, "GitHubRepo",
     owner="aws",
     repository_name="aws-cdk",
-    access_token=SecretValue.secrets_manager("my-github-token",
+    access_token=cdk.SecretValue.secrets_manager("my-github-token",
         json_field="token"
     ),
-    contents_bucket=s3.Bucket.from_bucket_name(self, "Bucket", "bucket-name"),
+    contents_bucket=s3.Bucket.from_bucket_name(stack, "Bucket", "bucket-name"),
     contents_key="import.zip"
 )
 ```
 
 ## Update or Delete the GitHubRepository
 
 At this moment, updates to the `GitHubRepository` are not supported and the repository will not be deleted upon the deletion of the CloudFormation stack. You will need to update or delete the GitHub repository manually.
+
+
```

### Comparing `aws-cdk.aws-codestar-alpha-2.84.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-codestar-alpha-2.9.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_codestar_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_codestar_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_codestar_alpha.egg-info/requires.txt
 src/aws_cdk.aws_codestar_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_codestar_alpha/__init__.py
 src/aws_cdk/aws_codestar_alpha/py.typed
 src/aws_cdk/aws_codestar_alpha/_jsii/__init__.py
-src/aws_cdk/aws_codestar_alpha/_jsii/aws-codestar-alpha@2.84.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_codestar_alpha/_jsii/aws-codestar-alpha@2.9.0-alpha.0.jsii.tgz
```

