# Comparing `tmp/aws-cdk.aws-iot-alpha-2.84.0a0.tar.gz` & `tmp/aws-cdk.aws-iot-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/aws-iot-alpha/dist/python/aws-cdk.aws-iot-alpha-2.84.0a0.tar", last modified: Tue Jun 13 23:47:04 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-iot/dist/python/aws-cdk.aws-iot-alpha-2.9.0a0.tar", last modified: Wed Jan 26 11:22:05 2022, max compression
```

## Comparing `aws-cdk.aws-iot-alpha-2.84.0a0.tar` & `aws-cdk.aws-iot-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-iot-alpha-2.84.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:57.000000 aws-cdk.aws-iot-alpha-2.84.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:57.000000 aws-cdk.aws-iot-alpha-2.84.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 23:46:57.000000 aws-cdk.aws-iot-alpha-2.84.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3845 2023-06-13 23:47:04.000000 aws-cdk.aws-iot-alpha-2.84.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2852 2023-06-13 23:46:57.000000 aws-cdk.aws-iot-alpha-2.84.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:57.000000 aws-cdk.aws-iot-alpha-2.84.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:47:04.000000 aws-cdk.aws-iot-alpha-2.84.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1842 2023-06-13 23:46:57.000000 aws-cdk.aws-iot-alpha-2.84.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-iot-alpha-2.84.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-iot-alpha-2.84.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-iot-alpha-2.84.0a0/src/aws_cdk/aws_iot_alpha/
--rw-r--r--   0 root         (0) root         (0)    38433 2023-06-13 23:46:57.000000 aws-cdk.aws-iot-alpha-2.84.0a0/src/aws_cdk/aws_iot_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-iot-alpha-2.84.0a0/src/aws_cdk/aws_iot_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      433 2023-06-13 23:46:57.000000 aws-cdk.aws-iot-alpha-2.84.0a0/src/aws_cdk/aws_iot_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39906 2023-06-13 23:46:57.000000 aws-cdk.aws-iot-alpha-2.84.0a0/src/aws_cdk/aws_iot_alpha/_jsii/aws-iot-alpha@2.84.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:57.000000 aws-cdk.aws-iot-alpha-2.84.0a0/src/aws_cdk/aws_iot_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-iot-alpha-2.84.0a0/src/aws_cdk.aws_iot_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3845 2023-06-13 23:47:04.000000 aws-cdk.aws-iot-alpha-2.84.0a0/src/aws_cdk.aws_iot_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      491 2023-06-13 23:47:04.000000 aws-cdk.aws-iot-alpha-2.84.0a0/src/aws_cdk.aws_iot_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:47:04.000000 aws-cdk.aws-iot-alpha-2.84.0a0/src/aws_cdk.aws_iot_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-13 23:47:04.000000 aws-cdk.aws-iot-alpha-2.84.0a0/src/aws_cdk.aws_iot_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:47:04.000000 aws-cdk.aws-iot-alpha-2.84.0a0/src/aws_cdk.aws_iot_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-iot-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-iot-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-iot-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:01.000000 aws-cdk.aws-iot-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3969 2022-01-26 11:22:05.000000 aws-cdk.aws-iot-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3009 2022-01-26 11:22:01.000000 aws-cdk.aws-iot-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-iot-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:05.000000 aws-cdk.aws-iot-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1767 2022-01-26 11:22:01.000000 aws-cdk.aws-iot-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-iot-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-iot-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-iot-alpha-2.9.0a0/src/aws_cdk/aws_iot_alpha/
+-rw-r--r--   0 root         (0) root         (0)    31549 2022-01-26 11:22:01.000000 aws-cdk.aws-iot-alpha-2.9.0a0/src/aws_cdk/aws_iot_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-iot-alpha-2.9.0a0/src/aws_cdk/aws_iot_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      397 2022-01-26 11:22:01.000000 aws-cdk.aws-iot-alpha-2.9.0a0/src/aws_cdk/aws_iot_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34511 2022-01-26 11:22:01.000000 aws-cdk.aws-iot-alpha-2.9.0a0/src/aws_cdk/aws_iot_alpha/_jsii/aws-iot-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-iot-alpha-2.9.0a0/src/aws_cdk/aws_iot_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-iot-alpha-2.9.0a0/src/aws_cdk.aws_iot_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3969 2022-01-26 11:22:05.000000 aws-cdk.aws-iot-alpha-2.9.0a0/src/aws_cdk.aws_iot_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      490 2022-01-26 11:22:05.000000 aws-cdk.aws-iot-alpha-2.9.0a0/src/aws_cdk.aws_iot_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:05.000000 aws-cdk.aws-iot-alpha-2.9.0a0/src/aws_cdk.aws_iot_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:05.000000 aws-cdk.aws-iot-alpha-2.9.0a0/src/aws_cdk.aws_iot_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:05.000000 aws-cdk.aws-iot-alpha-2.9.0a0/src/aws_cdk.aws_iot_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-iot-alpha-2.84.0a0/LICENSE` & `aws-cdk.aws-iot-alpha-2.9.0a0/LICENSE`

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

### Comparing `aws-cdk.aws-iot-alpha-2.84.0a0/PKG-INFO` & `aws-cdk.aws-iot-alpha-2.9.0a0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-iot-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::IoT
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
 
 # AWS IoT Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -40,14 +40,28 @@
 
 ---
 <!--END STABILITY BANNER-->
 
 AWS IoT Core lets you connect billions of IoT devices and route trillions of
 messages to AWS services without managing infrastructure.
 
+## Installation
+
+Install the module:
+
+```console
+$ npm i @aws-cdk/aws-iot
+```
+
+Import it into your code:
+
+```python
+import aws_cdk.aws_iot_alpha as iot
+```
+
 ## `TopicRule`
 
 Create a topic rule that give your devices the ability to interact with AWS services.
 You can create a topic rule with an action that invoke the Lambda action as following:
 
 ```python
 func = lambda_.Function(self, "MyFunction",
@@ -100,7 +114,9 @@
 iot.TopicRule(self, "TopicRule",
     sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id, timestamp() as timestamp FROM 'device/+/data'"),
     enabled=False
 )
 ```
 
 See also [@aws-cdk/aws-iot-actions](https://docs.aws.amazon.com/cdk/api/latest/docs/aws-iot-actions-readme.html) for other actions.
+
+
```

### Comparing `aws-cdk.aws-iot-alpha-2.84.0a0/README.md` & `aws-cdk.aws-iot-alpha-2.9.0a0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,28 @@
 
 ---
 <!--END STABILITY BANNER-->
 
 AWS IoT Core lets you connect billions of IoT devices and route trillions of
 messages to AWS services without managing infrastructure.
 
+## Installation
+
+Install the module:
+
+```console
+$ npm i @aws-cdk/aws-iot
+```
+
+Import it into your code:
+
+```python
+import aws_cdk.aws_iot_alpha as iot
+```
+
 ## `TopicRule`
 
 Create a topic rule that give your devices the ability to interact with AWS services.
 You can create a topic rule with an action that invoke the Lambda action as following:
 
 ```python
 func = lambda_.Function(self, "MyFunction",
```

### Comparing `aws-cdk.aws-iot-alpha-2.84.0a0/setup.py` & `aws-cdk.aws-iot-alpha-2.9.0a0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-iot-alpha",
-    "version": "2.84.0.a0",
+    "version": "2.9.0.a0",
     "description": "The CDK Construct Library for AWS::IoT",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,43 +22,41 @@
     },
     "packages": [
         "aws_cdk.aws_iot_alpha",
         "aws_cdk.aws_iot_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_iot_alpha._jsii": [
-            "aws-iot-alpha@2.84.0-alpha.0.jsii.tgz"
+            "aws-iot-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_iot_alpha": [
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

### Comparing `aws-cdk.aws-iot-alpha-2.84.0a0/src/aws_cdk/aws_iot_alpha/__init__.py` & `aws-cdk.aws-iot-alpha-2.9.0a0/src/aws_cdk/aws_iot_alpha/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,28 @@
 
 ---
 <!--END STABILITY BANNER-->
 
 AWS IoT Core lets you connect billions of IoT devices and route trillions of
 messages to AWS services without managing infrastructure.
 
+## Installation
+
+Install the module:
+
+```console
+$ npm i @aws-cdk/aws-iot
+```
+
+Import it into your code:
+
+```python
+import aws_cdk.aws_iot_alpha as iot
+```
+
 ## `TopicRule`
 
 Create a topic rule that give your devices the ability to interact with AWS services.
 You can create a topic rule with an action that invoke the Lambda action as following:
 
 ```python
 func = lambda_.Function(self, "MyFunction",
@@ -85,33 +99,31 @@
 import enum
 import typing
 
 import jsii
 import publication
 import typing_extensions
 
-from typeguard import check_type
-
 from ._jsii import *
 
-import aws_cdk as _aws_cdk_ceddda9d
-import aws_cdk.aws_iot as _aws_cdk_aws_iot_ceddda9d
-import constructs as _constructs_77d1e7e8
+import aws_cdk
+import aws_cdk.aws_iot
+import constructs
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-iot-alpha.ActionConfig",
     jsii_struct_bases=[],
     name_mapping={"configuration": "configuration"},
 )
 class ActionConfig:
     def __init__(
         self,
         *,
-        configuration: typing.Union[_aws_cdk_aws_iot_ceddda9d.CfnTopicRule.ActionProperty, typing.Dict[builtins.str, typing.Any]],
+        configuration: aws_cdk.aws_iot.CfnTopicRule.ActionProperty,
     ) -> None:
         '''(experimental) Properties for an topic rule action.
 
         :param configuration: (experimental) The configuration for this action.
 
         :stability: experimental
         :exampleMetadata: fixture=_generated
@@ -128,18 +140,15 @@
                         alarm_name="alarmName",
                         role_arn="roleArn",
                         state_reason="stateReason",
                         state_value="stateValue"
                     ),
                     cloudwatch_logs=CloudwatchLogsActionProperty(
                         log_group_name="logGroupName",
-                        role_arn="roleArn",
-            
-                        # the properties below are optional
-                        batch_mode=False
+                        role_arn="roleArn"
                     ),
                     cloudwatch_metric=CloudwatchMetricActionProperty(
                         metric_name="metricName",
                         metric_namespace="metricNamespace",
                         metric_unit="metricUnit",
                         metric_value="metricValue",
                         role_arn="roleArn",
@@ -258,52 +267,26 @@
             
                         # the properties below are optional
                         partition_key="partitionKey"
                     ),
                     lambda_=LambdaActionProperty(
                         function_arn="functionArn"
                     ),
-                    location=LocationActionProperty(
-                        device_id="deviceId",
-                        latitude="latitude",
-                        longitude="longitude",
-                        role_arn="roleArn",
-                        tracker_name="trackerName",
-            
-                        # the properties below are optional
-                        timestamp=TimestampProperty(
-                            value="value",
-            
-                            # the properties below are optional
-                            unit="unit"
-                        )
-                    ),
                     open_search=OpenSearchActionProperty(
                         endpoint="endpoint",
                         id="id",
                         index="index",
                         role_arn="roleArn",
                         type="type"
                     ),
                     republish=RepublishActionProperty(
                         role_arn="roleArn",
                         topic="topic",
             
                         # the properties below are optional
-                        headers=RepublishActionHeadersProperty(
-                            content_type="contentType",
-                            correlation_data="correlationData",
-                            message_expiry="messageExpiry",
-                            payload_format_indicator="payloadFormatIndicator",
-                            response_topic="responseTopic",
-                            user_properties=[UserPropertyProperty(
-                                key="key",
-                                value="value"
-                            )]
-                        ),
                         qos=123
                     ),
                     s3=S3ActionProperty(
                         bucket_name="bucketName",
                         key="key",
                         role_arn="roleArn",
             
@@ -337,40 +320,38 @@
                             name="name",
                             value="value"
                         )],
                         role_arn="roleArn",
                         table_name="tableName",
             
                         # the properties below are optional
+                        batch_mode=False,
                         timestamp=TimestreamTimestampProperty(
                             unit="unit",
                             value="value"
                         )
                     )
                 )
             )
         '''
         if isinstance(configuration, dict):
-            configuration = _aws_cdk_aws_iot_ceddda9d.CfnTopicRule.ActionProperty(**configuration)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__db72c5f97249b79d721bcd6a87436f822fe27caf16ccc0ae7aaa3671a54e7e5f)
-            check_type(argname="argument configuration", value=configuration, expected_type=type_hints["configuration"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+            configuration = aws_cdk.aws_iot.CfnTopicRule.ActionProperty(**configuration)
+        self._values: typing.Dict[str, typing.Any] = {
             "configuration": configuration,
         }
 
     @builtins.property
-    def configuration(self) -> _aws_cdk_aws_iot_ceddda9d.CfnTopicRule.ActionProperty:
+    def configuration(self) -> aws_cdk.aws_iot.CfnTopicRule.ActionProperty:
         '''(experimental) The configuration for this action.
 
         :stability: experimental
         '''
         result = self._values.get("configuration")
         assert result is not None, "Required property 'configuration' is missing"
-        return typing.cast(_aws_cdk_aws_iot_ceddda9d.CfnTopicRule.ActionProperty, result)
+        return typing.cast(aws_cdk.aws_iot.CfnTopicRule.ActionProperty, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -383,79 +364,96 @@
 @jsii.interface(jsii_type="@aws-cdk/aws-iot-alpha.IAction")
 class IAction(typing_extensions.Protocol):
     '''(experimental) An abstract action for TopicRule.
 
     :stability: experimental
     '''
 
-    pass
+    @jsii.member(jsii_name="bind")
+    def bind(self, topic_rule: "ITopicRule") -> ActionConfig:
+        '''(experimental) Returns the topic rule action specification.
+
+        :param topic_rule: The TopicRule that would trigger this action.
+
+        :stability: experimental
+        '''
+        ...
 
 
 class _IActionProxy:
     '''(experimental) An abstract action for TopicRule.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-iot-alpha.IAction"
-    pass
+
+    @jsii.member(jsii_name="bind")
+    def bind(self, topic_rule: "ITopicRule") -> ActionConfig:
+        '''(experimental) Returns the topic rule action specification.
+
+        :param topic_rule: The TopicRule that would trigger this action.
+
+        :stability: experimental
+        '''
+        return typing.cast(ActionConfig, jsii.invoke(self, "bind", [topic_rule]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IAction).__jsii_proxy_class__ = lambda : _IActionProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-iot-alpha.ITopicRule")
-class ITopicRule(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class ITopicRule(aws_cdk.IResource, typing_extensions.Protocol):
     '''(experimental) Represents an AWS IoT Rule.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="topicRuleArn")
     def topic_rule_arn(self) -> builtins.str:
         '''(experimental) The value of the topic rule Amazon Resource Name (ARN), such as arn:aws:iot:us-east-2:123456789012:rule/rule_name.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="topicRuleName")
     def topic_rule_name(self) -> builtins.str:
         '''(experimental) The name topic rule.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _ITopicRuleProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''(experimental) Represents an AWS IoT Rule.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-iot-alpha.ITopicRule"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="topicRuleArn")
     def topic_rule_arn(self) -> builtins.str:
         '''(experimental) The value of the topic rule Amazon Resource Name (ARN), such as arn:aws:iot:us-east-2:123456789012:rule/rule_name.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "topicRuleArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="topicRuleName")
     def topic_rule_name(self) -> builtins.str:
         '''(experimental) The name topic rule.
 
         :stability: experimental
         :attribute: true
         '''
@@ -472,124 +470,109 @@
     '''(experimental) Defines AWS IoT SQL.
 
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
-        import aws_cdk.aws_sns as sns
-        
+        bucket = s3.Bucket(self, "MyBucket")
         
-        topic = sns.Topic(self, "MyTopic")
-        
-        topic_rule = iot.TopicRule(self, "TopicRule",
-            sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id, year, month, day FROM 'device/+/data'"),
+        iot.TopicRule(self, "TopicRule",
+            sql=iot.IotSql.from_string_as_ver20160323("SELECT * FROM 'device/+/data'"),
             actions=[
-                actions.SnsTopicAction(topic,
-                    message_format=actions.SnsActionMessageFormat.JSON
+                actions.S3PutObjectAction(bucket,
+                    access_control=s3.BucketAccessControl.PUBLIC_READ
                 )
             ]
         )
     '''
 
     def __init__(self) -> None:
         '''
         :stability: experimental
         '''
         jsii.create(self.__class__, self, [])
 
-    @jsii.member(jsii_name="fromStringAsVer20151008")
+    @jsii.member(jsii_name="fromStringAsVer20151008") # type: ignore[misc]
     @builtins.classmethod
     def from_string_as_ver20151008(cls, sql: builtins.str) -> "IotSql":
         '''(experimental) Uses the original SQL version built on 2015-10-08.
 
         :param sql: The actual SQL-like syntax query.
 
         :return: Instance of IotSql
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__40b60afd6a89f56eb454ee327bd143df85ea1ea9518d995f338ac85c6f9172ef)
-            check_type(argname="argument sql", value=sql, expected_type=type_hints["sql"])
         return typing.cast("IotSql", jsii.sinvoke(cls, "fromStringAsVer20151008", [sql]))
 
-    @jsii.member(jsii_name="fromStringAsVer20160323")
+    @jsii.member(jsii_name="fromStringAsVer20160323") # type: ignore[misc]
     @builtins.classmethod
     def from_string_as_ver20160323(cls, sql: builtins.str) -> "IotSql":
         '''(experimental) Uses the SQL version built on 2016-03-23.
 
         :param sql: The actual SQL-like syntax query.
 
         :return: Instance of IotSql
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__246c805677b75001ec2445224c8ee29056b92709ee8d3bb168587a48bc5d0fb5)
-            check_type(argname="argument sql", value=sql, expected_type=type_hints["sql"])
         return typing.cast("IotSql", jsii.sinvoke(cls, "fromStringAsVer20160323", [sql]))
 
-    @jsii.member(jsii_name="fromStringAsVerNewestUnstable")
+    @jsii.member(jsii_name="fromStringAsVerNewestUnstable") # type: ignore[misc]
     @builtins.classmethod
     def from_string_as_ver_newest_unstable(cls, sql: builtins.str) -> "IotSql":
         '''(experimental) Uses the most recent beta SQL version.
 
         If you use this version, it might
         introduce breaking changes to your rules.
 
         :param sql: The actual SQL-like syntax query.
 
         :return: Instance of IotSql
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__715467063ed924cc91a9fa5b60c44d4b1b82edbc8eb085d68321fd0014a32067)
-            check_type(argname="argument sql", value=sql, expected_type=type_hints["sql"])
         return typing.cast("IotSql", jsii.sinvoke(cls, "fromStringAsVerNewestUnstable", [sql]))
 
-    @jsii.member(jsii_name="bind")
+    @jsii.member(jsii_name="bind") # type: ignore[misc]
     @abc.abstractmethod
-    def bind(self, scope: _constructs_77d1e7e8.Construct) -> "IotSqlConfig":
+    def bind(self, scope: constructs.Construct) -> "IotSqlConfig":
         '''(experimental) Returns the IoT SQL configuration.
 
         :param scope: -
 
         :stability: experimental
         '''
         ...
 
 
 class _IotSqlProxy(IotSql):
     @jsii.member(jsii_name="bind")
-    def bind(self, scope: _constructs_77d1e7e8.Construct) -> "IotSqlConfig":
+    def bind(self, scope: constructs.Construct) -> "IotSqlConfig":
         '''(experimental) Returns the IoT SQL configuration.
 
         :param scope: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7d3862c5242014e403c7a2af3ffcf5d3a77ce6e5376d651493716a5b5061bd9a)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
         return typing.cast("IotSqlConfig", jsii.invoke(self, "bind", [scope]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the abstract class
 typing.cast(typing.Any, IotSql).__jsii_proxy_class__ = lambda : _IotSqlProxy
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-iot-alpha.IotSqlConfig",
     jsii_struct_bases=[],
     name_mapping={"aws_iot_sql_version": "awsIotSqlVersion", "sql": "sql"},
 )
 class IotSqlConfig:
     def __init__(self, *, aws_iot_sql_version: builtins.str, sql: builtins.str) -> None:
-        '''(experimental) The type returned from the ``bind()`` method in ``IotSql``.
+        '''(experimental) The type returned from the ``bind()`` method in {@link IotSql}.
 
         :param aws_iot_sql_version: (experimental) The version of the SQL rules engine to use when evaluating the rule.
         :param sql: (experimental) The SQL statement used to query the topic.
 
         :stability: experimental
         :exampleMetadata: fixture=_generated
 
@@ -600,19 +583,15 @@
             import aws_cdk.aws_iot_alpha as iot_alpha
             
             iot_sql_config = iot_alpha.IotSqlConfig(
                 aws_iot_sql_version="awsIotSqlVersion",
                 sql="sql"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__887fb9654c4aa0ba71be51a8acf671f0dc89cdb21899f13ebce575d2da566e05)
-            check_type(argname="argument aws_iot_sql_version", value=aws_iot_sql_version, expected_type=type_hints["aws_iot_sql_version"])
-            check_type(argname="argument sql", value=sql, expected_type=type_hints["sql"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "aws_iot_sql_version": aws_iot_sql_version,
             "sql": sql,
         }
 
     @builtins.property
     def aws_iot_sql_version(self) -> builtins.str:
         '''(experimental) The version of the SQL rules engine to use when evaluating the rule.
@@ -643,43 +622,40 @@
         return "IotSqlConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.implements(ITopicRule)
 class TopicRule(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-iot-alpha.TopicRule",
 ):
     '''(experimental) Defines an AWS IoT Rule in this stack.
 
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
-        import aws_cdk.aws_sns as sns
-        
+        bucket = s3.Bucket(self, "MyBucket")
         
-        topic = sns.Topic(self, "MyTopic")
-        
-        topic_rule = iot.TopicRule(self, "TopicRule",
-            sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id, year, month, day FROM 'device/+/data'"),
+        iot.TopicRule(self, "TopicRule",
+            sql=iot.IotSql.from_string_as_ver20160323("SELECT * FROM 'device/+/data'"),
             actions=[
-                actions.SnsTopicAction(topic,
-                    message_format=actions.SnsActionMessageFormat.JSON
+                actions.S3PutObjectAction(bucket,
+                    access_control=s3.BucketAccessControl.PUBLIC_READ
                 )
             ]
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         sql: IotSql,
         actions: typing.Optional[typing.Sequence[IAction]] = None,
         description: typing.Optional[builtins.str] = None,
         enabled: typing.Optional[builtins.bool] = None,
         error_action: typing.Optional[IAction] = None,
@@ -693,76 +669,64 @@
         :param description: (experimental) A textual description of the topic rule. Default: None
         :param enabled: (experimental) Specifies whether the rule is enabled. Default: true
         :param error_action: (experimental) The action AWS IoT performs when it is unable to perform a rule's action. Default: - no action will be performed
         :param topic_rule_name: (experimental) The name of the topic rule. Default: None
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5629ae4086674af1b4cd4c3b55a1d2cd04d194fe7dd7d9a1a08478dc69d9ac5f)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = TopicRuleProps(
             sql=sql,
             actions=actions,
             description=description,
             enabled=enabled,
             error_action=error_action,
             topic_rule_name=topic_rule_name,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromTopicRuleArn")
+    @jsii.member(jsii_name="fromTopicRuleArn") # type: ignore[misc]
     @builtins.classmethod
     def from_topic_rule_arn(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         topic_rule_arn: builtins.str,
     ) -> ITopicRule:
         '''(experimental) Import an existing AWS IoT Rule provided an ARN.
 
         :param scope: The parent creating construct (usually ``this``).
         :param id: The construct's name.
         :param topic_rule_arn: AWS IoT Rule ARN (i.e. arn:aws:iot:::rule/MyRule).
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__92a02640c49b9d9e3824df915f05b77c597b5dfd5d900377ada5b2b60b004bbf)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument topic_rule_arn", value=topic_rule_arn, expected_type=type_hints["topic_rule_arn"])
         return typing.cast(ITopicRule, jsii.sinvoke(cls, "fromTopicRuleArn", [scope, id, topic_rule_arn]))
 
     @jsii.member(jsii_name="addAction")
     def add_action(self, action: IAction) -> None:
         '''(experimental) Add a action to the topic rule.
 
         :param action: the action to associate with the topic rule.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4e6d84c555ae6d88e9f422f5418183ec42014991c6a48af643a3d0341a35a73a)
-            check_type(argname="argument action", value=action, expected_type=type_hints["action"])
         return typing.cast(None, jsii.invoke(self, "addAction", [action]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="topicRuleArn")
     def topic_rule_arn(self) -> builtins.str:
         '''(experimental) Arn of this topic rule.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "topicRuleArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="topicRuleName")
     def topic_rule_name(self) -> builtins.str:
         '''(experimental) Name of this topic rule.
 
         :stability: experimental
         :attribute: true
         '''
@@ -802,37 +766,26 @@
         :param topic_rule_name: (experimental) The name of the topic rule. Default: None
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
-            import aws_cdk.aws_sns as sns
+            bucket = s3.Bucket(self, "MyBucket")
             
-            
-            topic = sns.Topic(self, "MyTopic")
-            
-            topic_rule = iot.TopicRule(self, "TopicRule",
-                sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id, year, month, day FROM 'device/+/data'"),
+            iot.TopicRule(self, "TopicRule",
+                sql=iot.IotSql.from_string_as_ver20160323("SELECT * FROM 'device/+/data'"),
                 actions=[
-                    actions.SnsTopicAction(topic,
-                        message_format=actions.SnsActionMessageFormat.JSON
+                    actions.S3PutObjectAction(bucket,
+                        access_control=s3.BucketAccessControl.PUBLIC_READ
                     )
                 ]
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__590edde80b67943632c721759786da252d24ea6e116cd451e3e93bb968888414)
-            check_type(argname="argument sql", value=sql, expected_type=type_hints["sql"])
-            check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
-            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
-            check_type(argname="argument enabled", value=enabled, expected_type=type_hints["enabled"])
-            check_type(argname="argument error_action", value=error_action, expected_type=type_hints["error_action"])
-            check_type(argname="argument topic_rule_name", value=topic_rule_name, expected_type=type_hints["topic_rule_name"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "sql": sql,
         }
         if actions is not None:
             self._values["actions"] = actions
         if description is not None:
             self._values["description"] = description
         if enabled is not None:
@@ -927,86 +880,7 @@
     "IotSql",
     "IotSqlConfig",
     "TopicRule",
     "TopicRuleProps",
 ]
 
 publication.publish()
-
-def _typecheckingstub__db72c5f97249b79d721bcd6a87436f822fe27caf16ccc0ae7aaa3671a54e7e5f(
-    *,
-    configuration: typing.Union[_aws_cdk_aws_iot_ceddda9d.CfnTopicRule.ActionProperty, typing.Dict[builtins.str, typing.Any]],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__40b60afd6a89f56eb454ee327bd143df85ea1ea9518d995f338ac85c6f9172ef(
-    sql: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__246c805677b75001ec2445224c8ee29056b92709ee8d3bb168587a48bc5d0fb5(
-    sql: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__715467063ed924cc91a9fa5b60c44d4b1b82edbc8eb085d68321fd0014a32067(
-    sql: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__7d3862c5242014e403c7a2af3ffcf5d3a77ce6e5376d651493716a5b5061bd9a(
-    scope: _constructs_77d1e7e8.Construct,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__887fb9654c4aa0ba71be51a8acf671f0dc89cdb21899f13ebce575d2da566e05(
-    *,
-    aws_iot_sql_version: builtins.str,
-    sql: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__5629ae4086674af1b4cd4c3b55a1d2cd04d194fe7dd7d9a1a08478dc69d9ac5f(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    sql: IotSql,
-    actions: typing.Optional[typing.Sequence[IAction]] = None,
-    description: typing.Optional[builtins.str] = None,
-    enabled: typing.Optional[builtins.bool] = None,
-    error_action: typing.Optional[IAction] = None,
-    topic_rule_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__92a02640c49b9d9e3824df915f05b77c597b5dfd5d900377ada5b2b60b004bbf(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    topic_rule_arn: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__4e6d84c555ae6d88e9f422f5418183ec42014991c6a48af643a3d0341a35a73a(
-    action: IAction,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__590edde80b67943632c721759786da252d24ea6e116cd451e3e93bb968888414(
-    *,
-    sql: IotSql,
-    actions: typing.Optional[typing.Sequence[IAction]] = None,
-    description: typing.Optional[builtins.str] = None,
-    enabled: typing.Optional[builtins.bool] = None,
-    error_action: typing.Optional[IAction] = None,
-    topic_rule_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
```

### Comparing `aws-cdk.aws-iot-alpha-2.84.0a0/src/aws_cdk.aws_iot_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-iot-alpha-2.9.0a0/src/aws_cdk.aws_iot_alpha.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-iot-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::IoT
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
 
 # AWS IoT Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -40,14 +40,28 @@
 
 ---
 <!--END STABILITY BANNER-->
 
 AWS IoT Core lets you connect billions of IoT devices and route trillions of
 messages to AWS services without managing infrastructure.
 
+## Installation
+
+Install the module:
+
+```console
+$ npm i @aws-cdk/aws-iot
+```
+
+Import it into your code:
+
+```python
+import aws_cdk.aws_iot_alpha as iot
+```
+
 ## `TopicRule`
 
 Create a topic rule that give your devices the ability to interact with AWS services.
 You can create a topic rule with an action that invoke the Lambda action as following:
 
 ```python
 func = lambda_.Function(self, "MyFunction",
@@ -100,7 +114,9 @@
 iot.TopicRule(self, "TopicRule",
     sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id, timestamp() as timestamp FROM 'device/+/data'"),
     enabled=False
 )
 ```
 
 See also [@aws-cdk/aws-iot-actions](https://docs.aws.amazon.com/cdk/api/latest/docs/aws-iot-actions-readme.html) for other actions.
+
+
```

