# Comparing `tmp/aws-cdk.aws-ivs-alpha-2.84.0a0.tar.gz` & `tmp/aws-cdk.aws-ivs-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/aws-ivs-alpha/dist/python/aws-cdk.aws-ivs-alpha-2.84.0a0.tar", last modified: Tue Jun 13 23:47:04 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-ivs/dist/python/aws-cdk.aws-ivs-alpha-2.9.0a0.tar", last modified: Wed Jan 26 11:22:06 2022, max compression
```

## Comparing `aws-cdk.aws-ivs-alpha-2.84.0a0.tar` & `aws-cdk.aws-ivs-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:57.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:57.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 23:46:57.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4208 2023-06-13 23:47:04.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3215 2023-06-13 23:46:57.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:57.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:47:04.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1842 2023-06-13 23:46:57.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/src/aws_cdk/aws_ivs_alpha/
--rw-r--r--   0 root         (0) root         (0)    31477 2023-06-13 23:46:57.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/src/aws_cdk/aws_ivs_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/src/aws_cdk/aws_ivs_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      433 2023-06-13 23:46:57.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/src/aws_cdk/aws_ivs_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32832 2023-06-13 23:46:57.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/src/aws_cdk/aws_ivs_alpha/_jsii/aws-ivs-alpha@2.84.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:57.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/src/aws_cdk/aws_ivs_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/src/aws_cdk.aws_ivs_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4208 2023-06-13 23:47:04.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/src/aws_cdk.aws_ivs_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      491 2023-06-13 23:47:04.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/src/aws_cdk.aws_ivs_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:47:04.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/src/aws_cdk.aws_ivs_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-13 23:47:04.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/src/aws_cdk.aws_ivs_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:47:04.000000 aws-cdk.aws-ivs-alpha-2.84.0a0/src/aws_cdk.aws_ivs_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:01.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4175 2022-01-26 11:22:06.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3215 2022-01-26 11:22:01.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:06.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1767 2022-01-26 11:22:01.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/src/aws_cdk/aws_ivs_alpha/
+-rw-r--r--   0 root         (0) root         (0)    25389 2022-01-26 11:22:01.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/src/aws_cdk/aws_ivs_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/src/aws_cdk/aws_ivs_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      397 2022-01-26 11:22:01.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/src/aws_cdk/aws_ivs_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27646 2022-01-26 11:22:01.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/src/aws_cdk/aws_ivs_alpha/_jsii/aws-ivs-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/src/aws_cdk/aws_ivs_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/src/aws_cdk.aws_ivs_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4175 2022-01-26 11:22:06.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/src/aws_cdk.aws_ivs_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      490 2022-01-26 11:22:06.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/src/aws_cdk.aws_ivs_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:06.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/src/aws_cdk.aws_ivs_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:06.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/src/aws_cdk.aws_ivs_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:06.000000 aws-cdk.aws-ivs-alpha-2.9.0a0/src/aws_cdk.aws_ivs_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-ivs-alpha-2.84.0a0/LICENSE` & `aws-cdk.aws-ivs-alpha-2.9.0a0/LICENSE`

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

### Comparing `aws-cdk.aws-ivs-alpha-2.84.0a0/PKG-INFO` & `aws-cdk.aws-ivs-alpha-2.9.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-ivs-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::IVS
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
 
 # AWS::IVS Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -109,7 +109,9 @@
 Then, when creating a channel, specify the authorized property
 
 ```python
 my_channel = ivs.Channel(self, "Channel",
     authorized=True
 )
 ```
+
+
```

### Comparing `aws-cdk.aws-ivs-alpha-2.84.0a0/README.md` & `aws-cdk.aws-ivs-alpha-2.9.0a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-ivs-alpha-2.84.0a0/setup.py` & `aws-cdk.aws-ivs-alpha-2.9.0a0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-ivs-alpha",
-    "version": "2.84.0.a0",
+    "version": "2.9.0.a0",
     "description": "The CDK Construct Library for AWS::IVS",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,43 +22,41 @@
     },
     "packages": [
         "aws_cdk.aws_ivs_alpha",
         "aws_cdk.aws_ivs_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_ivs_alpha._jsii": [
-            "aws-ivs-alpha@2.84.0-alpha.0.jsii.tgz"
+            "aws-ivs-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_ivs_alpha": [
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

### Comparing `aws-cdk.aws-ivs-alpha-2.84.0a0/src/aws_cdk/aws_ivs_alpha/__init__.py` & `aws-cdk.aws-ivs-alpha-2.9.0a0/src/aws_cdk/aws_ivs_alpha/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -94,70 +94,62 @@
 import enum
 import typing
 
 import jsii
 import publication
 import typing_extensions
 
-from typeguard import check_type
-
 from ._jsii import *
 
-import aws_cdk as _aws_cdk_ceddda9d
-import constructs as _constructs_77d1e7e8
+import aws_cdk
+import constructs
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-ivs-alpha.ChannelProps",
     jsii_struct_bases=[],
     name_mapping={
         "authorized": "authorized",
-        "channel_name": "channelName",
         "latency_mode": "latencyMode",
+        "name": "name",
         "type": "type",
     },
 )
 class ChannelProps:
     def __init__(
         self,
         *,
         authorized: typing.Optional[builtins.bool] = None,
-        channel_name: typing.Optional[builtins.str] = None,
         latency_mode: typing.Optional["LatencyMode"] = None,
+        name: typing.Optional[builtins.str] = None,
         type: typing.Optional["ChannelType"] = None,
     ) -> None:
         '''(experimental) Properties for creating a new Channel.
 
         :param authorized: (experimental) Whether the channel is authorized. If you wish to make an authorized channel, you will need to ensure that a PlaybackKeyPair has been uploaded to your account as this is used to validate the signed JWT that is required for authorization Default: false
-        :param channel_name: (experimental) A name for the channel. Default: Automatically generated name
         :param latency_mode: (experimental) Channel latency mode. Default: LatencyMode.LOW
+        :param name: (experimental) Channel name. Default: - None
         :param type: (experimental) The channel type, which determines the allowable resolution and bitrate. If you exceed the allowable resolution or bitrate, the stream will disconnect immediately Default: ChannelType.STANDARD
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
             my_channel = ivs.Channel(self, "Channel",
                 authorized=True
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0ebf6a0e98bbd5b88d9676fbe616666a44f837cba80675eade5df1fea22c9d22)
-            check_type(argname="argument authorized", value=authorized, expected_type=type_hints["authorized"])
-            check_type(argname="argument channel_name", value=channel_name, expected_type=type_hints["channel_name"])
-            check_type(argname="argument latency_mode", value=latency_mode, expected_type=type_hints["latency_mode"])
-            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if authorized is not None:
             self._values["authorized"] = authorized
-        if channel_name is not None:
-            self._values["channel_name"] = channel_name
         if latency_mode is not None:
             self._values["latency_mode"] = latency_mode
+        if name is not None:
+            self._values["name"] = name
         if type is not None:
             self._values["type"] = type
 
     @builtins.property
     def authorized(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Whether the channel is authorized.
 
@@ -169,34 +161,34 @@
 
         :stability: experimental
         '''
         result = self._values.get("authorized")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def channel_name(self) -> typing.Optional[builtins.str]:
-        '''(experimental) A name for the channel.
+    def latency_mode(self) -> typing.Optional["LatencyMode"]:
+        '''(experimental) Channel latency mode.
 
-        :default: Automatically generated name
+        :default: LatencyMode.LOW
 
         :stability: experimental
         '''
-        result = self._values.get("channel_name")
-        return typing.cast(typing.Optional[builtins.str], result)
+        result = self._values.get("latency_mode")
+        return typing.cast(typing.Optional["LatencyMode"], result)
 
     @builtins.property
-    def latency_mode(self) -> typing.Optional["LatencyMode"]:
-        '''(experimental) Channel latency mode.
+    def name(self) -> typing.Optional[builtins.str]:
+        '''(experimental) Channel name.
 
-        :default: LatencyMode.LOW
+        :default: - None
 
         :stability: experimental
         '''
-        result = self._values.get("latency_mode")
-        return typing.cast(typing.Optional["LatencyMode"], result)
+        result = self._values.get("name")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def type(self) -> typing.Optional["ChannelType"]:
         '''(experimental) The channel type, which determines the allowable resolution and bitrate.
 
         If you exceed the allowable resolution or bitrate, the stream will disconnect immediately
 
@@ -241,21 +233,21 @@
 
     :see: https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-ivs-channel.html
     :stability: experimental
     '''
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-ivs-alpha.IChannel")
-class IChannel(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class IChannel(aws_cdk.IResource, typing_extensions.Protocol):
     '''(experimental) Represents an IVS Channel.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="channelArn")
     def channel_arn(self) -> builtins.str:
         '''(experimental) The channel ARN.
 
         For example: arn:aws:ivs:us-west-2:123456789012:channel/abcdABCDefgh
 
         :stability: experimental
@@ -271,24 +263,24 @@
 
         :stability: experimental
         '''
         ...
 
 
 class _IChannelProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''(experimental) Represents an IVS Channel.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-ivs-alpha.IChannel"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="channelArn")
     def channel_arn(self) -> builtins.str:
         '''(experimental) The channel ARN.
 
         For example: arn:aws:ivs:us-west-2:123456789012:channel/abcdABCDefgh
 
         :stability: experimental
@@ -300,54 +292,51 @@
     def add_stream_key(self, id: builtins.str) -> "StreamKey":
         '''(experimental) Adds a stream key for this IVS Channel.
 
         :param id: construct ID.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__809e7d60e77d2ede718027f4d99dcf810db3b33f39daebb557b424c6457e2f22)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         return typing.cast("StreamKey", jsii.invoke(self, "addStreamKey", [id]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IChannel).__jsii_proxy_class__ = lambda : _IChannelProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-ivs-alpha.IPlaybackKeyPair")
-class IPlaybackKeyPair(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class IPlaybackKeyPair(aws_cdk.IResource, typing_extensions.Protocol):
     '''(experimental) Represents an IVS Playback Key Pair.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="playbackKeyPairArn")
     def playback_key_pair_arn(self) -> builtins.str:
         '''(experimental) Key-pair ARN.
 
         For example: arn:aws:ivs:us-west-2:693991300569:playback-key/f99cde61-c2b0-4df3-8941-ca7d38acca1a
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _IPlaybackKeyPairProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''(experimental) Represents an IVS Playback Key Pair.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-ivs-alpha.IPlaybackKeyPair"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="playbackKeyPairArn")
     def playback_key_pair_arn(self) -> builtins.str:
         '''(experimental) Key-pair ARN.
 
         For example: arn:aws:ivs:us-west-2:693991300569:playback-key/f99cde61-c2b0-4df3-8941-ca7d38acca1a
 
         :stability: experimental
@@ -356,44 +345,44 @@
         return typing.cast(builtins.str, jsii.get(self, "playbackKeyPairArn"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IPlaybackKeyPair).__jsii_proxy_class__ = lambda : _IPlaybackKeyPairProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-ivs-alpha.IStreamKey")
-class IStreamKey(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class IStreamKey(aws_cdk.IResource, typing_extensions.Protocol):
     '''(experimental) Represents an IVS Stream Key.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="streamKeyArn")
     def stream_key_arn(self) -> builtins.str:
         '''(experimental) The stream-key ARN.
 
         For example: arn:aws:ivs:us-west-2:123456789012:stream-key/g1H2I3j4k5L6
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _IStreamKeyProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''(experimental) Represents an IVS Stream Key.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-ivs-alpha.IStreamKey"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="streamKeyArn")
     def stream_key_arn(self) -> builtins.str:
         '''(experimental) The stream-key ARN.
 
         For example: arn:aws:ivs:us-west-2:123456789012:stream-key/g1H2I3j4k5L6
 
         :stability: experimental
@@ -422,15 +411,15 @@
 
     :stability: experimental
     '''
 
 
 @jsii.implements(IPlaybackKeyPair)
 class PlaybackKeyPair(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-ivs-alpha.PlaybackKeyPair",
 ):
     '''(experimental) A new IVS Playback Key Pair.
 
     :stability: experimental
     :exampleMetadata: infused
@@ -440,51 +429,46 @@
         key_pair = ivs.PlaybackKeyPair(self, "PlaybackKeyPair",
             public_key_material=my_public_key_pem_string
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         public_key_material: builtins.str,
-        playback_key_pair_name: typing.Optional[builtins.str] = None,
+        name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param public_key_material: (experimental) The public portion of a customer-generated key pair.
-        :param playback_key_pair_name: (experimental) An arbitrary string (a nickname) assigned to a playback key pair that helps the customer identify that resource. The value does not need to be unique. Default: Automatically generated name
+        :param name: (experimental) An arbitrary string (a nickname) assigned to a playback key pair that helps the customer identify that resource. The value does not need to be unique. Default: None
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__75931c57bc0ba240c98824ea65da9a0bc0a3bc48be2344ac7b70c03f259e632f)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = PlaybackKeyPairProps(
-            public_key_material=public_key_material,
-            playback_key_pair_name=playback_key_pair_name,
+            public_key_material=public_key_material, name=name
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="playbackKeyPairArn")
     def playback_key_pair_arn(self) -> builtins.str:
         '''(experimental) Key-pair ARN.
 
         For example: arn:aws:ivs:us-west-2:693991300569:playback-key/f99cde61-c2b0-4df3-8941-ca7d38acca1a
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "playbackKeyPairArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="playbackKeyPairFingerprint")
     def playback_key_pair_fingerprint(self) -> builtins.str:
         '''(experimental) Key-pair identifier.
 
         For example: 98:0d:1a:a0:19:96:1e:ea:0a:0a:2c:9a:42:19:2b:e7
 
         :stability: experimental
@@ -492,71 +476,64 @@
         '''
         return typing.cast(builtins.str, jsii.get(self, "playbackKeyPairFingerprint"))
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-ivs-alpha.PlaybackKeyPairProps",
     jsii_struct_bases=[],
-    name_mapping={
-        "public_key_material": "publicKeyMaterial",
-        "playback_key_pair_name": "playbackKeyPairName",
-    },
+    name_mapping={"public_key_material": "publicKeyMaterial", "name": "name"},
 )
 class PlaybackKeyPairProps:
     def __init__(
         self,
         *,
         public_key_material: builtins.str,
-        playback_key_pair_name: typing.Optional[builtins.str] = None,
+        name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Properties for creating a new Playback Key Pair.
 
         :param public_key_material: (experimental) The public portion of a customer-generated key pair.
-        :param playback_key_pair_name: (experimental) An arbitrary string (a nickname) assigned to a playback key pair that helps the customer identify that resource. The value does not need to be unique. Default: Automatically generated name
+        :param name: (experimental) An arbitrary string (a nickname) assigned to a playback key pair that helps the customer identify that resource. The value does not need to be unique. Default: None
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
             key_pair = ivs.PlaybackKeyPair(self, "PlaybackKeyPair",
                 public_key_material=my_public_key_pem_string
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5f26b3314acb516329ef76511a5408ac87ae783446cab3f1be9ed1d0b81fa5b7)
-            check_type(argname="argument public_key_material", value=public_key_material, expected_type=type_hints["public_key_material"])
-            check_type(argname="argument playback_key_pair_name", value=playback_key_pair_name, expected_type=type_hints["playback_key_pair_name"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "public_key_material": public_key_material,
         }
-        if playback_key_pair_name is not None:
-            self._values["playback_key_pair_name"] = playback_key_pair_name
+        if name is not None:
+            self._values["name"] = name
 
     @builtins.property
     def public_key_material(self) -> builtins.str:
         '''(experimental) The public portion of a customer-generated key pair.
 
         :stability: experimental
         '''
         result = self._values.get("public_key_material")
         assert result is not None, "Required property 'public_key_material' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def playback_key_pair_name(self) -> typing.Optional[builtins.str]:
+    def name(self) -> typing.Optional[builtins.str]:
         '''(experimental) An arbitrary string (a nickname) assigned to a playback key pair that helps the customer identify that resource.
 
         The value does not need to be unique.
 
-        :default: Automatically generated name
+        :default: None
 
         :stability: experimental
         '''
-        result = self._values.get("playback_key_pair_name")
+        result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
@@ -565,15 +542,15 @@
         return "PlaybackKeyPairProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.implements(IStreamKey)
 class StreamKey(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-ivs-alpha.StreamKey",
 ):
     '''(experimental) A new IVS Stream Key.
 
     :stability: experimental
     :exampleMetadata: fixture=with-channel infused
@@ -581,46 +558,42 @@
     Example::
 
         my_stream_key = my_channel.add_stream_key("StreamKey")
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         channel: IChannel,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param channel: (experimental) Channel ARN for the stream.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__67fad0f56ffbc15680b0f651250d8bb5cf4dacb899e5c5bbf4abdcfc3ae39632)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = StreamKeyProps(channel=channel)
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="streamKeyArn")
     def stream_key_arn(self) -> builtins.str:
         '''(experimental) The stream-key ARN.
 
         For example: arn:aws:ivs:us-west-2:123456789012:stream-key/g1H2I3j4k5L6
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "streamKeyArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="streamKeyValue")
     def stream_key_value(self) -> builtins.str:
         '''(experimental) The stream-key value.
 
         For example: sk_us-west-2_abcdABCDefgh_567890abcdef
 
         :stability: experimental
@@ -651,18 +624,15 @@
             
             # channel: ivs_alpha.Channel
             
             stream_key_props = ivs_alpha.StreamKeyProps(
                 channel=channel
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__10474702d05a8d909166c4d0ef1de9632d82c17ae609436e3980c1bd4fa2ddb3)
-            check_type(argname="argument channel", value=channel, expected_type=type_hints["channel"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "channel": channel,
         }
 
     @builtins.property
     def channel(self) -> IChannel:
         '''(experimental) Channel ARN for the stream.
 
@@ -682,15 +652,15 @@
         return "StreamKeyProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.implements(IChannel)
 class Channel(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-ivs-alpha.Channel",
 ):
     '''(experimental) A new IVS channel.
 
     :stability: experimental
     :exampleMetadata: infused
@@ -698,105 +668,90 @@
     Example::
 
         my_channel = ivs.Channel(self, "Channel")
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         authorized: typing.Optional[builtins.bool] = None,
-        channel_name: typing.Optional[builtins.str] = None,
         latency_mode: typing.Optional[LatencyMode] = None,
+        name: typing.Optional[builtins.str] = None,
         type: typing.Optional[ChannelType] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param authorized: (experimental) Whether the channel is authorized. If you wish to make an authorized channel, you will need to ensure that a PlaybackKeyPair has been uploaded to your account as this is used to validate the signed JWT that is required for authorization Default: false
-        :param channel_name: (experimental) A name for the channel. Default: Automatically generated name
         :param latency_mode: (experimental) Channel latency mode. Default: LatencyMode.LOW
+        :param name: (experimental) Channel name. Default: - None
         :param type: (experimental) The channel type, which determines the allowable resolution and bitrate. If you exceed the allowable resolution or bitrate, the stream will disconnect immediately Default: ChannelType.STANDARD
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__07139327925dc97a551bbf17c849a0f698e0c9c60d3da3f65f2b3d2bea0e0c50)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = ChannelProps(
-            authorized=authorized,
-            channel_name=channel_name,
-            latency_mode=latency_mode,
-            type=type,
+            authorized=authorized, latency_mode=latency_mode, name=name, type=type
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromChannelArn")
+    @jsii.member(jsii_name="fromChannelArn") # type: ignore[misc]
     @builtins.classmethod
     def from_channel_arn(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         channel_arn: builtins.str,
     ) -> IChannel:
         '''(experimental) Import an existing channel.
 
         :param scope: -
         :param id: -
         :param channel_arn: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5efa416339cc500736f229c9a2b3b3b1143c18d7a26fe2712053e5511d370c5f)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument channel_arn", value=channel_arn, expected_type=type_hints["channel_arn"])
         return typing.cast(IChannel, jsii.sinvoke(cls, "fromChannelArn", [scope, id, channel_arn]))
 
     @jsii.member(jsii_name="addStreamKey")
     def add_stream_key(self, id: builtins.str) -> StreamKey:
         '''(experimental) Adds a stream key for this IVS Channel.
 
         :param id: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__65e1f25de7c3a0e391031082a65ee02865e1f85fe29f43a74bbc59866b95e50a)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         return typing.cast(StreamKey, jsii.invoke(self, "addStreamKey", [id]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="channelArn")
     def channel_arn(self) -> builtins.str:
         '''(experimental) The channel ARN.
 
         For example: arn:aws:ivs:us-west-2:123456789012:channel/abcdABCDefgh
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "channelArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="channelIngestEndpoint")
     def channel_ingest_endpoint(self) -> builtins.str:
         '''(experimental) Channel ingest endpoint, part of the definition of an ingest server, used when you set up streaming software.
 
         For example: a1b2c3d4e5f6.global-contribute.live-video.net
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "channelIngestEndpoint"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="channelPlaybackUrl")
     def channel_playback_url(self) -> builtins.str:
         '''(experimental) Channel playback URL.
 
         For example:
         https://a1b2c3d4e5f6.us-west-2.playback.live-video.net/api/video/v1/us-west-2.123456789012.channel.abcdEFGH.m3u8
 
@@ -817,83 +772,7 @@
     "PlaybackKeyPair",
     "PlaybackKeyPairProps",
     "StreamKey",
     "StreamKeyProps",
 ]
 
 publication.publish()
-
-def _typecheckingstub__0ebf6a0e98bbd5b88d9676fbe616666a44f837cba80675eade5df1fea22c9d22(
-    *,
-    authorized: typing.Optional[builtins.bool] = None,
-    channel_name: typing.Optional[builtins.str] = None,
-    latency_mode: typing.Optional[LatencyMode] = None,
-    type: typing.Optional[ChannelType] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__809e7d60e77d2ede718027f4d99dcf810db3b33f39daebb557b424c6457e2f22(
-    id: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__75931c57bc0ba240c98824ea65da9a0bc0a3bc48be2344ac7b70c03f259e632f(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    public_key_material: builtins.str,
-    playback_key_pair_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__5f26b3314acb516329ef76511a5408ac87ae783446cab3f1be9ed1d0b81fa5b7(
-    *,
-    public_key_material: builtins.str,
-    playback_key_pair_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__67fad0f56ffbc15680b0f651250d8bb5cf4dacb899e5c5bbf4abdcfc3ae39632(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    channel: IChannel,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__10474702d05a8d909166c4d0ef1de9632d82c17ae609436e3980c1bd4fa2ddb3(
-    *,
-    channel: IChannel,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__07139327925dc97a551bbf17c849a0f698e0c9c60d3da3f65f2b3d2bea0e0c50(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    authorized: typing.Optional[builtins.bool] = None,
-    channel_name: typing.Optional[builtins.str] = None,
-    latency_mode: typing.Optional[LatencyMode] = None,
-    type: typing.Optional[ChannelType] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__5efa416339cc500736f229c9a2b3b3b1143c18d7a26fe2712053e5511d370c5f(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    channel_arn: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__65e1f25de7c3a0e391031082a65ee02865e1f85fe29f43a74bbc59866b95e50a(
-    id: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
```

### Comparing `aws-cdk.aws-ivs-alpha-2.84.0a0/src/aws_cdk.aws_ivs_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-ivs-alpha-2.9.0a0/src/aws_cdk.aws_ivs_alpha.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-ivs-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::IVS
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
 
 # AWS::IVS Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -109,7 +109,9 @@
 Then, when creating a channel, specify the authorized property
 
 ```python
 my_channel = ivs.Channel(self, "Channel",
     authorized=True
 )
 ```
+
+
```

