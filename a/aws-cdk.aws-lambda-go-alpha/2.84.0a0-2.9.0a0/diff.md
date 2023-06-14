# Comparing `tmp/aws-cdk.aws-lambda-go-alpha-2.84.0a0.tar.gz` & `tmp/aws-cdk.aws-lambda-go-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/aws-lambda-go-alpha/dist/python/aws-cdk.aws-lambda-go-alpha-2.84.0a0.tar", last modified: Tue Jun 13 23:46:45 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-lambda-go/dist/python/aws-cdk.aws-lambda-go-alpha-2.9.0a0.t", last modified: Wed Jan 26 11:22:07 2022, max compression
```

## Comparing `aws-cdk.aws-lambda-go-alpha-2.84.0a0.tar` & `aws-cdk.aws-lambda-go-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:37.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:37.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 23:46:37.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11798 2023-06-13 23:46:45.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10787 2023-06-13 23:46:37.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:37.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:46:45.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1890 2023-06-13 23:46:37.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/src/aws_cdk/aws_lambda_go_alpha/
--rw-r--r--   0 root         (0) root         (0)   110265 2023-06-13 23:46:37.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/src/aws_cdk/aws_lambda_go_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/src/aws_cdk/aws_lambda_go_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-13 23:46:37.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/src/aws_cdk/aws_lambda_go_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46113 2023-06-13 23:46:37.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/src/aws_cdk/aws_lambda_go_alpha/_jsii/aws-lambda-go-alpha@2.84.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:37.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/src/aws_cdk/aws_lambda_go_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/src/aws_cdk.aws_lambda_go_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11798 2023-06-13 23:46:45.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/src/aws_cdk.aws_lambda_go_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-13 23:46:45.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/src/aws_cdk.aws_lambda_go_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:45.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/src/aws_cdk.aws_lambda_go_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-13 23:46:45.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/src/aws_cdk.aws_lambda_go_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:46:45.000000 aws-cdk.aws-lambda-go-alpha-2.84.0a0/src/aws_cdk.aws_lambda_go_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10507 2022-01-26 11:22:07.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9529 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:07.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1815 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/src/aws_cdk/aws_lambda_go_alpha/
+-rw-r--r--   0 root         (0) root         (0)    73080 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/src/aws_cdk/aws_lambda_go_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/src/aws_cdk/aws_lambda_go_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      409 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/src/aws_cdk/aws_lambda_go_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38075 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/src/aws_cdk/aws_lambda_go_alpha/_jsii/aws-lambda-go-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/src/aws_cdk/aws_lambda_go_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/src/aws_cdk.aws_lambda_go_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10507 2022-01-26 11:22:07.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/src/aws_cdk.aws_lambda_go_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      550 2022-01-26 11:22:07.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/src/aws_cdk.aws_lambda_go_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:07.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/src/aws_cdk.aws_lambda_go_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:07.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/src/aws_cdk.aws_lambda_go_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:07.000000 aws-cdk.aws-lambda-go-alpha-2.9.0a0/src/aws_cdk.aws_lambda_go_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-lambda-go-alpha-2.84.0a0/LICENSE` & `aws-cdk.aws-lambda-go-alpha-2.9.0a0/LICENSE`

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

### Comparing `aws-cdk.aws-lambda-go-alpha-2.84.0a0/PKG-INFO` & `aws-cdk.aws-lambda-go-alpha-2.9.0a0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-lambda-go-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS Lambda in Golang
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
 
 # Amazon Lambda Golang Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -50,15 +50,15 @@
 using a Go version >= 1.11 and is using [Go modules](https://golang.org/ref/mod).
 
 ## Go Function
 
 Define a `GoFunction`:
 
 ```python
-go.GoFunction(self, "handler",
+lambda_.GoFunction(self, "handler",
     entry="app/cmd/api"
 )
 ```
 
 By default, if `entry` points to a directory, then the construct will assume there is a Go entry file (i.e. `main.go`).
 Let's look at an example Go project:
 
@@ -121,30 +121,30 @@
 
 1. You are using vendoring (indicated by the presence of a `vendor` folder)
    In this case `go build` will be run with `-mod=vendor` set
 2. You are not using vendoring (indicated by the absence of a `vendor` folder)
    If you are not vendoring then `go build` will be run without `-mod=vendor`
    since the default behavior is to download dependencies
 
-All other properties of `lambda.Function` are supported, see also the [AWS Lambda construct library](https://github.com/aws/aws-cdk/tree/main/packages/%40aws-cdk/aws-lambda).
+All other properties of `lambda.Function` are supported, see also the [AWS Lambda construct library](https://github.com/aws/aws-cdk/tree/master/packages/%40aws-cdk/aws-lambda).
 
 ## Environment
 
 By default the following environment variables are set for you:
 
 * `GOOS=linux`
 * `GOARCH`: based on the target architecture of the Lambda function
 * `GO111MODULE=on`
 
 Use the `environment` prop to define additional environment variables when go runs:
 
 ```python
-go.GoFunction(self, "handler",
+lambda_.GoFunction(self, "handler",
     entry="app/cmd/api",
-    bundling=go.BundlingOptions(
+    bundling=lambda.BundlingOptions(
         environment={
             "HELLO": "WORLD"
         }
     )
 )
 ```
 
@@ -159,82 +159,54 @@
 ## Docker
 
 To force bundling in a docker container even if `Go` is available in your environment, set the `forceDockerBundling` prop to `true`. This is useful if you want to make sure that your function is built in a consistent Lambda compatible environment.
 
 Use the `buildArgs` prop to pass build arguments when building the bundling image:
 
 ```python
-go.GoFunction(self, "handler",
+lambda_.GoFunction(self, "handler",
     entry="app/cmd/api",
-    bundling=go.BundlingOptions(
+    bundling=lambda.BundlingOptions(
         build_args={
             "HTTPS_PROXY": "https://127.0.0.1:3001"
         }
     )
 )
 ```
 
 Use the `bundling.dockerImage` prop to use a custom bundling image:
 
 ```python
-go.GoFunction(self, "handler",
+lambda_.GoFunction(self, "handler",
     entry="app/cmd/api",
-    bundling=go.BundlingOptions(
+    bundling=lambda.BundlingOptions(
         docker_image=DockerImage.from_build("/path/to/Dockerfile")
     )
 )
 ```
 
 Use the `bundling.goBuildFlags` prop to pass additional build flags to `go build`:
 
 ```python
-go.GoFunction(self, "handler",
+lambda_.GoFunction(self, "handler",
     entry="app/cmd/api",
-    bundling=go.BundlingOptions(
+    bundling=lambda.BundlingOptions(
         go_build_flags=["-ldflags \"-s -w\""]
     )
 )
 ```
 
-By default this construct doesn't use any Go module proxies. This is contrary to
-a standard Go installation, which would use the Google proxy by default. To
-recreate that behavior, do the following:
-
-```python
-go.GoFunction(self, "GoFunction",
-    entry="app/cmd/api",
-    bundling=go.BundlingOptions(
-        go_proxies=[go.GoFunction.GOOGLE_GOPROXY, "direct"]
-    )
-)
-```
-
-You can set additional Docker options to configure the build environment:
-
-```python
-go.GoFunction(self, "GoFunction",
-    entry="app/cmd/api",
-    bundling=go.BundlingOptions(
-        network="host",
-        security_opt="no-new-privileges",
-        user="user:group",
-        volumes_from=["777f7dc92da7"],
-        volumes=[DockerVolume(host_path="/host-path", container_path="/container-path")]
-    )
-)
-```
-
 ## Command hooks
 
 It is  possible to run additional commands by specifying the `commandHooks` prop:
 
 ```text
 // This example only available in TypeScript
 // Run additional commands on a GoFunction via `commandHooks` property
-new go.GoFunction(this, 'handler', {
+new lambda.GoFunction(this, 'handler', {
   bundling: {
     commandHooks: {
       // run tests
       beforeBundling(inputDir: string): string[] {
         return ['go test ./cmd/api -v'];
       },
       // ...
@@ -259,15 +231,15 @@
 
 Depending on how you structure your Golang application, you may want to change the `assetHashType` parameter.
 By default this parameter is set to `AssetHashType.OUTPUT` which means that the CDK will calculate the asset hash
 (and determine whether or not your code has changed) based on the Golang executable that is created.
 
 If you specify `AssetHashType.SOURCE`, the CDK will calculate the asset hash by looking at the folder
 that contains your `go.mod` file. If you are deploying a single Lambda function, or you want to redeploy
-all of your functions if anything changes, then `AssetHashType.SOURCE` will probably work.
+all of your functions if anything changes, then `AssetHashType.SOURCE` will probaby work.
 
 For example, if my app looked like this:
 
 ```bash
 lamda-app
 ├── cmd
 │   └── api
@@ -280,15 +252,15 @@
 ```
 
 With this structure I would provide the `entry` as `cmd/api` which means that the CDK
 will determine that the protect root is `lambda-app` (it contains the `go.mod` file).
 Since I only have a single Lambda function, and any update to files within the `lambda-app` directory
 should trigger a new deploy, I could specify `AssetHashType.SOURCE`.
 
-On the other hand, if I had a project that deployed multiple Lambda functions, for example:
+On the other hand, if I had a project that deployed mmultiple Lambda functions, for example:
 
 ```bash
 lamda-app
 ├── cmd
 │   ├── api
 │   │   └── main.go
 │   └── anotherApi
@@ -305,20 +277,8 @@
 Then I would most likely want `AssetHashType.OUTPUT`. With `OUTPUT`
 the CDK will only recognize changes if the Golang executable has changed,
 and Go only includes dependencies that are used in the executable. So in this case
 if `cmd/api` used the `auth` & `middleware` packages, but `cmd/anotherApi` did not, then
 an update to `auth` or `middleware` would only trigger an update to the `cmd/api` Lambda
 Function.
 
-## Docker based bundling in complex Docker configurations
-
-By default the input and output of Docker based bundling is handled via bind mounts.
-In situtations where this does not work, like Docker-in-Docker setups or when using a remote Docker socket, you can configure an alternative, but slower, variant that also works in these situations.
 
-```python
-go.GoFunction(self, "GoFunction",
-    entry="app/cmd/api",
-    bundling=go.BundlingOptions(
-        bundling_file_access=BundlingFileAccess.VOLUME_COPY
-    )
-)
-```
```

### Comparing `aws-cdk.aws-lambda-go-alpha-2.84.0a0/README.md` & `aws-cdk.aws-lambda-go-alpha-2.9.0a0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 using a Go version >= 1.11 and is using [Go modules](https://golang.org/ref/mod).
 
 ## Go Function
 
 Define a `GoFunction`:
 
 ```python
-go.GoFunction(self, "handler",
+lambda_.GoFunction(self, "handler",
     entry="app/cmd/api"
 )
 ```
 
 By default, if `entry` points to a directory, then the construct will assume there is a Go entry file (i.e. `main.go`).
 Let's look at an example Go project:
 
@@ -94,30 +94,30 @@
 
 1. You are using vendoring (indicated by the presence of a `vendor` folder)
    In this case `go build` will be run with `-mod=vendor` set
 2. You are not using vendoring (indicated by the absence of a `vendor` folder)
    If you are not vendoring then `go build` will be run without `-mod=vendor`
    since the default behavior is to download dependencies
 
-All other properties of `lambda.Function` are supported, see also the [AWS Lambda construct library](https://github.com/aws/aws-cdk/tree/main/packages/%40aws-cdk/aws-lambda).
+All other properties of `lambda.Function` are supported, see also the [AWS Lambda construct library](https://github.com/aws/aws-cdk/tree/master/packages/%40aws-cdk/aws-lambda).
 
 ## Environment
 
 By default the following environment variables are set for you:
 
 * `GOOS=linux`
 * `GOARCH`: based on the target architecture of the Lambda function
 * `GO111MODULE=on`
 
 Use the `environment` prop to define additional environment variables when go runs:
 
 ```python
-go.GoFunction(self, "handler",
+lambda_.GoFunction(self, "handler",
     entry="app/cmd/api",
-    bundling=go.BundlingOptions(
+    bundling=lambda.BundlingOptions(
         environment={
             "HELLO": "WORLD"
         }
     )
 )
 ```
 
@@ -132,82 +132,54 @@
 ## Docker
 
 To force bundling in a docker container even if `Go` is available in your environment, set the `forceDockerBundling` prop to `true`. This is useful if you want to make sure that your function is built in a consistent Lambda compatible environment.
 
 Use the `buildArgs` prop to pass build arguments when building the bundling image:
 
 ```python
-go.GoFunction(self, "handler",
+lambda_.GoFunction(self, "handler",
     entry="app/cmd/api",
-    bundling=go.BundlingOptions(
+    bundling=lambda.BundlingOptions(
         build_args={
             "HTTPS_PROXY": "https://127.0.0.1:3001"
         }
     )
 )
 ```
 
 Use the `bundling.dockerImage` prop to use a custom bundling image:
 
 ```python
-go.GoFunction(self, "handler",
+lambda_.GoFunction(self, "handler",
     entry="app/cmd/api",
-    bundling=go.BundlingOptions(
+    bundling=lambda.BundlingOptions(
         docker_image=DockerImage.from_build("/path/to/Dockerfile")
     )
 )
 ```
 
 Use the `bundling.goBuildFlags` prop to pass additional build flags to `go build`:
 
 ```python
-go.GoFunction(self, "handler",
+lambda_.GoFunction(self, "handler",
     entry="app/cmd/api",
-    bundling=go.BundlingOptions(
+    bundling=lambda.BundlingOptions(
         go_build_flags=["-ldflags \"-s -w\""]
     )
 )
 ```
 
-By default this construct doesn't use any Go module proxies. This is contrary to
-a standard Go installation, which would use the Google proxy by default. To
-recreate that behavior, do the following:
-
-```python
-go.GoFunction(self, "GoFunction",
-    entry="app/cmd/api",
-    bundling=go.BundlingOptions(
-        go_proxies=[go.GoFunction.GOOGLE_GOPROXY, "direct"]
-    )
-)
-```
-
-You can set additional Docker options to configure the build environment:
-
-```python
-go.GoFunction(self, "GoFunction",
-    entry="app/cmd/api",
-    bundling=go.BundlingOptions(
-        network="host",
-        security_opt="no-new-privileges",
-        user="user:group",
-        volumes_from=["777f7dc92da7"],
-        volumes=[DockerVolume(host_path="/host-path", container_path="/container-path")]
-    )
-)
-```
-
 ## Command hooks
 
 It is  possible to run additional commands by specifying the `commandHooks` prop:
 
 ```text
 // This example only available in TypeScript
 // Run additional commands on a GoFunction via `commandHooks` property
-new go.GoFunction(this, 'handler', {
+new lambda.GoFunction(this, 'handler', {
   bundling: {
     commandHooks: {
       // run tests
       beforeBundling(inputDir: string): string[] {
         return ['go test ./cmd/api -v'];
       },
       // ...
@@ -232,15 +204,15 @@
 
 Depending on how you structure your Golang application, you may want to change the `assetHashType` parameter.
 By default this parameter is set to `AssetHashType.OUTPUT` which means that the CDK will calculate the asset hash
 (and determine whether or not your code has changed) based on the Golang executable that is created.
 
 If you specify `AssetHashType.SOURCE`, the CDK will calculate the asset hash by looking at the folder
 that contains your `go.mod` file. If you are deploying a single Lambda function, or you want to redeploy
-all of your functions if anything changes, then `AssetHashType.SOURCE` will probably work.
+all of your functions if anything changes, then `AssetHashType.SOURCE` will probaby work.
 
 For example, if my app looked like this:
 
 ```bash
 lamda-app
 ├── cmd
 │   └── api
@@ -253,15 +225,15 @@
 ```
 
 With this structure I would provide the `entry` as `cmd/api` which means that the CDK
 will determine that the protect root is `lambda-app` (it contains the `go.mod` file).
 Since I only have a single Lambda function, and any update to files within the `lambda-app` directory
 should trigger a new deploy, I could specify `AssetHashType.SOURCE`.
 
-On the other hand, if I had a project that deployed multiple Lambda functions, for example:
+On the other hand, if I had a project that deployed mmultiple Lambda functions, for example:
 
 ```bash
 lamda-app
 ├── cmd
 │   ├── api
 │   │   └── main.go
 │   └── anotherApi
@@ -277,21 +249,7 @@
 
 Then I would most likely want `AssetHashType.OUTPUT`. With `OUTPUT`
 the CDK will only recognize changes if the Golang executable has changed,
 and Go only includes dependencies that are used in the executable. So in this case
 if `cmd/api` used the `auth` & `middleware` packages, but `cmd/anotherApi` did not, then
 an update to `auth` or `middleware` would only trigger an update to the `cmd/api` Lambda
 Function.
-
-## Docker based bundling in complex Docker configurations
-
-By default the input and output of Docker based bundling is handled via bind mounts.
-In situtations where this does not work, like Docker-in-Docker setups or when using a remote Docker socket, you can configure an alternative, but slower, variant that also works in these situations.
-
-```python
-go.GoFunction(self, "GoFunction",
-    entry="app/cmd/api",
-    bundling=go.BundlingOptions(
-        bundling_file_access=BundlingFileAccess.VOLUME_COPY
-    )
-)
-```
```

### Comparing `aws-cdk.aws-lambda-go-alpha-2.84.0a0/setup.py` & `aws-cdk.aws-lambda-go-alpha-2.9.0a0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-lambda-go-alpha",
-    "version": "2.84.0.a0",
+    "version": "2.9.0.a0",
     "description": "The CDK Construct Library for AWS Lambda in Golang",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,43 +22,41 @@
     },
     "packages": [
         "aws_cdk.aws_lambda_go_alpha",
         "aws_cdk.aws_lambda_go_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_lambda_go_alpha._jsii": [
-            "aws-lambda-go-alpha@2.84.0-alpha.0.jsii.tgz"
+            "aws-lambda-go-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_lambda_go_alpha": [
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

### Comparing `aws-cdk.aws-lambda-go-alpha-2.84.0a0/src/aws_cdk.aws_lambda_go_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-lambda-go-alpha-2.9.0a0/src/aws_cdk.aws_lambda_go_alpha.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-lambda-go-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS Lambda in Golang
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
 
 # Amazon Lambda Golang Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -50,15 +50,15 @@
 using a Go version >= 1.11 and is using [Go modules](https://golang.org/ref/mod).
 
 ## Go Function
 
 Define a `GoFunction`:
 
 ```python
-go.GoFunction(self, "handler",
+lambda_.GoFunction(self, "handler",
     entry="app/cmd/api"
 )
 ```
 
 By default, if `entry` points to a directory, then the construct will assume there is a Go entry file (i.e. `main.go`).
 Let's look at an example Go project:
 
@@ -121,30 +121,30 @@
 
 1. You are using vendoring (indicated by the presence of a `vendor` folder)
    In this case `go build` will be run with `-mod=vendor` set
 2. You are not using vendoring (indicated by the absence of a `vendor` folder)
    If you are not vendoring then `go build` will be run without `-mod=vendor`
    since the default behavior is to download dependencies
 
-All other properties of `lambda.Function` are supported, see also the [AWS Lambda construct library](https://github.com/aws/aws-cdk/tree/main/packages/%40aws-cdk/aws-lambda).
+All other properties of `lambda.Function` are supported, see also the [AWS Lambda construct library](https://github.com/aws/aws-cdk/tree/master/packages/%40aws-cdk/aws-lambda).
 
 ## Environment
 
 By default the following environment variables are set for you:
 
 * `GOOS=linux`
 * `GOARCH`: based on the target architecture of the Lambda function
 * `GO111MODULE=on`
 
 Use the `environment` prop to define additional environment variables when go runs:
 
 ```python
-go.GoFunction(self, "handler",
+lambda_.GoFunction(self, "handler",
     entry="app/cmd/api",
-    bundling=go.BundlingOptions(
+    bundling=lambda.BundlingOptions(
         environment={
             "HELLO": "WORLD"
         }
     )
 )
 ```
 
@@ -159,82 +159,54 @@
 ## Docker
 
 To force bundling in a docker container even if `Go` is available in your environment, set the `forceDockerBundling` prop to `true`. This is useful if you want to make sure that your function is built in a consistent Lambda compatible environment.
 
 Use the `buildArgs` prop to pass build arguments when building the bundling image:
 
 ```python
-go.GoFunction(self, "handler",
+lambda_.GoFunction(self, "handler",
     entry="app/cmd/api",
-    bundling=go.BundlingOptions(
+    bundling=lambda.BundlingOptions(
         build_args={
             "HTTPS_PROXY": "https://127.0.0.1:3001"
         }
     )
 )
 ```
 
 Use the `bundling.dockerImage` prop to use a custom bundling image:
 
 ```python
-go.GoFunction(self, "handler",
+lambda_.GoFunction(self, "handler",
     entry="app/cmd/api",
-    bundling=go.BundlingOptions(
+    bundling=lambda.BundlingOptions(
         docker_image=DockerImage.from_build("/path/to/Dockerfile")
     )
 )
 ```
 
 Use the `bundling.goBuildFlags` prop to pass additional build flags to `go build`:
 
 ```python
-go.GoFunction(self, "handler",
+lambda_.GoFunction(self, "handler",
     entry="app/cmd/api",
-    bundling=go.BundlingOptions(
+    bundling=lambda.BundlingOptions(
         go_build_flags=["-ldflags \"-s -w\""]
     )
 )
 ```
 
-By default this construct doesn't use any Go module proxies. This is contrary to
-a standard Go installation, which would use the Google proxy by default. To
-recreate that behavior, do the following:
-
-```python
-go.GoFunction(self, "GoFunction",
-    entry="app/cmd/api",
-    bundling=go.BundlingOptions(
-        go_proxies=[go.GoFunction.GOOGLE_GOPROXY, "direct"]
-    )
-)
-```
-
-You can set additional Docker options to configure the build environment:
-
-```python
-go.GoFunction(self, "GoFunction",
-    entry="app/cmd/api",
-    bundling=go.BundlingOptions(
-        network="host",
-        security_opt="no-new-privileges",
-        user="user:group",
-        volumes_from=["777f7dc92da7"],
-        volumes=[DockerVolume(host_path="/host-path", container_path="/container-path")]
-    )
-)
-```
-
 ## Command hooks
 
 It is  possible to run additional commands by specifying the `commandHooks` prop:
 
 ```text
 // This example only available in TypeScript
 // Run additional commands on a GoFunction via `commandHooks` property
-new go.GoFunction(this, 'handler', {
+new lambda.GoFunction(this, 'handler', {
   bundling: {
     commandHooks: {
       // run tests
       beforeBundling(inputDir: string): string[] {
         return ['go test ./cmd/api -v'];
       },
       // ...
@@ -259,15 +231,15 @@
 
 Depending on how you structure your Golang application, you may want to change the `assetHashType` parameter.
 By default this parameter is set to `AssetHashType.OUTPUT` which means that the CDK will calculate the asset hash
 (and determine whether or not your code has changed) based on the Golang executable that is created.
 
 If you specify `AssetHashType.SOURCE`, the CDK will calculate the asset hash by looking at the folder
 that contains your `go.mod` file. If you are deploying a single Lambda function, or you want to redeploy
-all of your functions if anything changes, then `AssetHashType.SOURCE` will probably work.
+all of your functions if anything changes, then `AssetHashType.SOURCE` will probaby work.
 
 For example, if my app looked like this:
 
 ```bash
 lamda-app
 ├── cmd
 │   └── api
@@ -280,15 +252,15 @@
 ```
 
 With this structure I would provide the `entry` as `cmd/api` which means that the CDK
 will determine that the protect root is `lambda-app` (it contains the `go.mod` file).
 Since I only have a single Lambda function, and any update to files within the `lambda-app` directory
 should trigger a new deploy, I could specify `AssetHashType.SOURCE`.
 
-On the other hand, if I had a project that deployed multiple Lambda functions, for example:
+On the other hand, if I had a project that deployed mmultiple Lambda functions, for example:
 
 ```bash
 lamda-app
 ├── cmd
 │   ├── api
 │   │   └── main.go
 │   └── anotherApi
@@ -305,20 +277,8 @@
 Then I would most likely want `AssetHashType.OUTPUT`. With `OUTPUT`
 the CDK will only recognize changes if the Golang executable has changed,
 and Go only includes dependencies that are used in the executable. So in this case
 if `cmd/api` used the `auth` & `middleware` packages, but `cmd/anotherApi` did not, then
 an update to `auth` or `middleware` would only trigger an update to the `cmd/api` Lambda
 Function.
 
-## Docker based bundling in complex Docker configurations
-
-By default the input and output of Docker based bundling is handled via bind mounts.
-In situtations where this does not work, like Docker-in-Docker setups or when using a remote Docker socket, you can configure an alternative, but slower, variant that also works in these situations.
 
-```python
-go.GoFunction(self, "GoFunction",
-    entry="app/cmd/api",
-    bundling=go.BundlingOptions(
-        bundling_file_access=BundlingFileAccess.VOLUME_COPY
-    )
-)
-```
```

### Comparing `aws-cdk.aws-lambda-go-alpha-2.84.0a0/src/aws_cdk.aws_lambda_go_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-lambda-go-alpha-2.9.0a0/src/aws_cdk.aws_lambda_go_alpha.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_lambda_go_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_lambda_go_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_lambda_go_alpha.egg-info/requires.txt
 src/aws_cdk.aws_lambda_go_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_lambda_go_alpha/__init__.py
 src/aws_cdk/aws_lambda_go_alpha/py.typed
 src/aws_cdk/aws_lambda_go_alpha/_jsii/__init__.py
-src/aws_cdk/aws_lambda_go_alpha/_jsii/aws-lambda-go-alpha@2.84.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_lambda_go_alpha/_jsii/aws-lambda-go-alpha@2.9.0-alpha.0.jsii.tgz
```

