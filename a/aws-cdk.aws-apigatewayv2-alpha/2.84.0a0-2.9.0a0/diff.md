# Comparing `tmp/aws-cdk.aws-apigatewayv2-alpha-2.84.0a0.tar.gz` & `tmp/aws-cdk.aws-apigatewayv2-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/aws-apigatewayv2-alpha/dist/python/aws-cdk.aws-apigatewayv2-alpha-2.84.0a0", last modified: Tue Jun 13 23:46:43 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-apigatewayv2/dist/python/aws-cdk.aws-apigatewayv2-alpha-2.9", last modified: Wed Jan 26 11:22:05 2022, max compression
```

## Comparing `aws-cdk.aws-apigatewayv2-alpha-2.84.0a0.tar` & `aws-cdk.aws-apigatewayv2-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:43.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:37.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:37.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 23:46:37.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    19711 2023-06-13 23:46:43.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18700 2023-06-13 23:46:37.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:37.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:46:43.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1905 2023-06-13 23:46:37.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:43.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:43.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:43.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/src/aws_cdk/aws_apigatewayv2_alpha/
--rw-r--r--   0 root         (0) root         (0)   561673 2023-06-13 23:46:37.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/src/aws_cdk/aws_apigatewayv2_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:43.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/src/aws_cdk/aws_apigatewayv2_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      451 2023-06-13 23:46:37.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/src/aws_cdk/aws_apigatewayv2_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   166066 2023-06-13 23:46:37.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/src/aws_cdk/aws_apigatewayv2_alpha/_jsii/aws-apigatewayv2-alpha@2.84.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:37.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/src/aws_cdk/aws_apigatewayv2_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:43.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/src/aws_cdk.aws_apigatewayv2_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19711 2023-06-13 23:46:43.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/src/aws_cdk.aws_apigatewayv2_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      581 2023-06-13 23:46:43.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/src/aws_cdk.aws_apigatewayv2_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:43.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/src/aws_cdk.aws_apigatewayv2_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-13 23:46:43.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/src/aws_cdk.aws_apigatewayv2_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:46:43.000000 aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/src/aws_cdk.aws_apigatewayv2_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:01.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    19438 2022-01-26 11:22:05.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18460 2022-01-26 11:22:01.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:05.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1830 2022-01-26 11:22:01.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_alpha/
+-rw-r--r--   0 root         (0) root         (0)   440857 2022-01-26 11:22:01.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      415 2022-01-26 11:22:01.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   144195 2022-01-26 11:22:01.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_alpha/_jsii/aws-apigatewayv2-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19438 2022-01-26 11:22:05.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2022-01-26 11:22:05.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:05.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:05.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:05.000000 aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/LICENSE` & `aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/LICENSE`

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

### Comparing `aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/PKG-INFO` & `aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-apigatewayv2-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::APIGatewayv2
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
 
 # AWS::APIGatewayv2 Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -93,20 +93,21 @@
 [Configuring integrations](https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-develop-integrations.html).
 
 Integrations are available at the `aws-apigatewayv2-integrations` module and more information is available in that module.
 As an early example, the following code snippet configures a route `GET /books` with an HTTP proxy integration all
 configures all other HTTP method calls to `/books` to a lambda proxy.
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 from aws_cdk.aws_apigatewayv2_integrations_alpha import HttpUrlIntegration, HttpLambdaIntegration
 
 # books_default_fn: lambda.Function
 
 
-get_books_integration = HttpUrlIntegration("GetBooksIntegration", "https://get-books-proxy.example.com")
+get_books_integration = HttpUrlIntegration("GetBooksIntegration", "https://get-books-proxy.myproxy.internal")
 books_default_integration = HttpLambdaIntegration("BooksIntegration", books_default_fn)
 
 http_api = apigwv2.HttpApi(self, "HttpApi")
 
 http_api.add_routes(
     path="/books",
     methods=[apigwv2.HttpMethod.GET],
@@ -279,30 +280,29 @@
 ```
 
 ### Mutual TLS (mTLS)
 
 Mutual TLS can be configured to limit access to your API based by using client certificates instead of (or as an extension of) using authorization headers.
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 import aws_cdk.aws_s3 as s3
-import aws_cdk.aws_certificatemanager as acm
-# bucket: s3.Bucket
-
 
 cert_arn = "arn:aws:acm:us-east-1:111111111111:certificate"
 domain_name = "example.com"
+bucket = s3.Bucket.from_bucket_name(stack, "TrustStoreBucket", ...)
 
-apigwv2.DomainName(self, "DomainName",
+DomainName(stack, "DomainName",
     domain_name=domain_name,
-    certificate=acm.Certificate.from_certificate_arn(self, "cert", cert_arn),
-    mtls=apigwv2.MTLSConfig(
-        bucket=bucket,
-        key="someca.pem",
-        version="version"
-    )
+    certificate=Certificate.from_certificate_arn(stack, "cert", cert_arn),
+    mtls={
+        "bucket": bucket,
+        "key": "someca.pem",
+        "version": "version"
+    }
 )
 ```
 
 Instructions for configuring your trust store can be found [here](https://aws.amazon.com/blogs/compute/introducing-mutual-tls-authentication-for-amazon-api-gateway/)
 
 ### Managing access to HTTP APIs
 
@@ -428,52 +428,32 @@
 
 web_socket_api = apigwv2.WebSocketApi(self, "mywsapi")
 web_socket_api.add_route("sendmessage",
     integration=WebSocketLambdaIntegration("SendMessageIntegration", message_handler)
 )
 ```
 
-To add a route that can return a result:
-
-```python
-from aws_cdk.aws_apigatewayv2_integrations_alpha import WebSocketLambdaIntegration
-
-# message_handler: lambda.Function
-
-web_socket_api = apigwv2.WebSocketApi(self, "mywsapi")
-web_socket_api.add_route("sendmessage",
-    integration=WebSocketLambdaIntegration("SendMessageIntegration", message_handler),
-    return_response=True
-)
-```
-
-To import an existing WebSocketApi:
-
-```python
-web_socket_api = apigwv2.WebSocketApi.from_web_socket_api_attributes(self, "mywsapi", web_socket_id="api-1234")
-```
-
 ### Manage Connections Permission
 
 Grant permission to use API Gateway Management API of a WebSocket API by calling the `grantManageConnections` API.
 You can use Management API to send a callback message to a connected client, get connection information, or disconnect the client. Learn more at [Use @connections commands in your backend service](https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-how-to-call-websocket-api-connections.html).
 
 ```python
-# fn: lambda.Function
+# Example automatically generated from non-compiling source. May contain errors.
+lambda_ = lambda_.Function(self, "lambda")
 
-
-web_socket_api = apigwv2.WebSocketApi(self, "mywsapi")
-stage = apigwv2.WebSocketStage(self, "mystage",
+web_socket_api = WebSocketApi(stack, "mywsapi")
+stage = WebSocketStage(stack, "mystage",
     web_socket_api=web_socket_api,
     stage_name="dev"
 )
 # per stage permission
-stage.grant_management_api_access(fn)
+stage.grant_manage_connections(lambda_)
 # for all the stages permission
-web_socket_api.grant_manage_connections(fn)
+web_socket_api.grant_manage_connections(lambda_)
 ```
 
 ### Managing access to WebSocket APIs
 
 API Gateway supports multiple mechanisms for [controlling and managing access to a WebSocket API](https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-websocket-api-control-access.html) through authorizers.
 
 These authorizers can be found in the [APIGatewayV2-Authorizers](https://docs.aws.amazon.com/cdk/api/latest/docs/aws-apigatewayv2-authorizers-readme.html) constructs library.
@@ -481,11 +461,14 @@
 ### API Keys
 
 Websocket APIs also support usage of API Keys. An API Key is a key that is used to grant access to an API. These are useful for controlling and tracking access to an API, when used together with [usage plans](https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-api-usage-plans.html). These together allow you to configure controls around API access such as quotas and throttling, along with per-API Key metrics on usage.
 
 To require an API Key when accessing the Websocket API:
 
 ```python
-web_socket_api = apigwv2.WebSocketApi(self, "mywsapi",
-    api_key_selection_expression=apigwv2.WebSocketApiKeySelectionExpression.HEADER_X_API_KEY
+# Example automatically generated from non-compiling source. May contain errors.
+web_socket_api = WebSocketApi(stack, "mywsapi",
+    api_key_selection_expression=WebSocketApiKeySelectionExpression.HEADER_X_API_KEY
 )
 ```
+
+
```

### Comparing `aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/README.md` & `aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -66,20 +66,21 @@
 [Configuring integrations](https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-develop-integrations.html).
 
 Integrations are available at the `aws-apigatewayv2-integrations` module and more information is available in that module.
 As an early example, the following code snippet configures a route `GET /books` with an HTTP proxy integration all
 configures all other HTTP method calls to `/books` to a lambda proxy.
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 from aws_cdk.aws_apigatewayv2_integrations_alpha import HttpUrlIntegration, HttpLambdaIntegration
 
 # books_default_fn: lambda.Function
 
 
-get_books_integration = HttpUrlIntegration("GetBooksIntegration", "https://get-books-proxy.example.com")
+get_books_integration = HttpUrlIntegration("GetBooksIntegration", "https://get-books-proxy.myproxy.internal")
 books_default_integration = HttpLambdaIntegration("BooksIntegration", books_default_fn)
 
 http_api = apigwv2.HttpApi(self, "HttpApi")
 
 http_api.add_routes(
     path="/books",
     methods=[apigwv2.HttpMethod.GET],
@@ -252,30 +253,29 @@
 ```
 
 ### Mutual TLS (mTLS)
 
 Mutual TLS can be configured to limit access to your API based by using client certificates instead of (or as an extension of) using authorization headers.
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 import aws_cdk.aws_s3 as s3
-import aws_cdk.aws_certificatemanager as acm
-# bucket: s3.Bucket
-
 
 cert_arn = "arn:aws:acm:us-east-1:111111111111:certificate"
 domain_name = "example.com"
+bucket = s3.Bucket.from_bucket_name(stack, "TrustStoreBucket", ...)
 
-apigwv2.DomainName(self, "DomainName",
+DomainName(stack, "DomainName",
     domain_name=domain_name,
-    certificate=acm.Certificate.from_certificate_arn(self, "cert", cert_arn),
-    mtls=apigwv2.MTLSConfig(
-        bucket=bucket,
-        key="someca.pem",
-        version="version"
-    )
+    certificate=Certificate.from_certificate_arn(stack, "cert", cert_arn),
+    mtls={
+        "bucket": bucket,
+        "key": "someca.pem",
+        "version": "version"
+    }
 )
 ```
 
 Instructions for configuring your trust store can be found [here](https://aws.amazon.com/blogs/compute/introducing-mutual-tls-authentication-for-amazon-api-gateway/)
 
 ### Managing access to HTTP APIs
 
@@ -401,52 +401,32 @@
 
 web_socket_api = apigwv2.WebSocketApi(self, "mywsapi")
 web_socket_api.add_route("sendmessage",
     integration=WebSocketLambdaIntegration("SendMessageIntegration", message_handler)
 )
 ```
 
-To add a route that can return a result:
-
-```python
-from aws_cdk.aws_apigatewayv2_integrations_alpha import WebSocketLambdaIntegration
-
-# message_handler: lambda.Function
-
-web_socket_api = apigwv2.WebSocketApi(self, "mywsapi")
-web_socket_api.add_route("sendmessage",
-    integration=WebSocketLambdaIntegration("SendMessageIntegration", message_handler),
-    return_response=True
-)
-```
-
-To import an existing WebSocketApi:
-
-```python
-web_socket_api = apigwv2.WebSocketApi.from_web_socket_api_attributes(self, "mywsapi", web_socket_id="api-1234")
-```
-
 ### Manage Connections Permission
 
 Grant permission to use API Gateway Management API of a WebSocket API by calling the `grantManageConnections` API.
 You can use Management API to send a callback message to a connected client, get connection information, or disconnect the client. Learn more at [Use @connections commands in your backend service](https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-how-to-call-websocket-api-connections.html).
 
 ```python
-# fn: lambda.Function
-
+# Example automatically generated from non-compiling source. May contain errors.
+lambda_ = lambda_.Function(self, "lambda")
 
-web_socket_api = apigwv2.WebSocketApi(self, "mywsapi")
-stage = apigwv2.WebSocketStage(self, "mystage",
+web_socket_api = WebSocketApi(stack, "mywsapi")
+stage = WebSocketStage(stack, "mystage",
     web_socket_api=web_socket_api,
     stage_name="dev"
 )
 # per stage permission
-stage.grant_management_api_access(fn)
+stage.grant_manage_connections(lambda_)
 # for all the stages permission
-web_socket_api.grant_manage_connections(fn)
+web_socket_api.grant_manage_connections(lambda_)
 ```
 
 ### Managing access to WebSocket APIs
 
 API Gateway supports multiple mechanisms for [controlling and managing access to a WebSocket API](https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-websocket-api-control-access.html) through authorizers.
 
 These authorizers can be found in the [APIGatewayV2-Authorizers](https://docs.aws.amazon.com/cdk/api/latest/docs/aws-apigatewayv2-authorizers-readme.html) constructs library.
@@ -454,11 +434,12 @@
 ### API Keys
 
 Websocket APIs also support usage of API Keys. An API Key is a key that is used to grant access to an API. These are useful for controlling and tracking access to an API, when used together with [usage plans](https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-api-usage-plans.html). These together allow you to configure controls around API access such as quotas and throttling, along with per-API Key metrics on usage.
 
 To require an API Key when accessing the Websocket API:
 
 ```python
-web_socket_api = apigwv2.WebSocketApi(self, "mywsapi",
-    api_key_selection_expression=apigwv2.WebSocketApiKeySelectionExpression.HEADER_X_API_KEY
+# Example automatically generated from non-compiling source. May contain errors.
+web_socket_api = WebSocketApi(stack, "mywsapi",
+    api_key_selection_expression=WebSocketApiKeySelectionExpression.HEADER_X_API_KEY
 )
 ```
```

### Comparing `aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/setup.py` & `aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-apigatewayv2-alpha",
-    "version": "2.84.0.a0",
+    "version": "2.9.0.a0",
     "description": "The CDK Construct Library for AWS::APIGatewayv2",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,43 +22,41 @@
     },
     "packages": [
         "aws_cdk.aws_apigatewayv2_alpha",
         "aws_cdk.aws_apigatewayv2_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_apigatewayv2_alpha._jsii": [
-            "aws-apigatewayv2-alpha@2.84.0-alpha.0.jsii.tgz"
+            "aws-apigatewayv2-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_apigatewayv2_alpha": [
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

### Comparing `aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/src/aws_cdk/aws_apigatewayv2_alpha/__init__.py` & `aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_alpha/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -67,20 +67,21 @@
 [Configuring integrations](https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-develop-integrations.html).
 
 Integrations are available at the `aws-apigatewayv2-integrations` module and more information is available in that module.
 As an early example, the following code snippet configures a route `GET /books` with an HTTP proxy integration all
 configures all other HTTP method calls to `/books` to a lambda proxy.
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 from aws_cdk.aws_apigatewayv2_integrations_alpha import HttpUrlIntegration, HttpLambdaIntegration
 
 # books_default_fn: lambda.Function
 
 
-get_books_integration = HttpUrlIntegration("GetBooksIntegration", "https://get-books-proxy.example.com")
+get_books_integration = HttpUrlIntegration("GetBooksIntegration", "https://get-books-proxy.myproxy.internal")
 books_default_integration = HttpLambdaIntegration("BooksIntegration", books_default_fn)
 
 http_api = apigwv2.HttpApi(self, "HttpApi")
 
 http_api.add_routes(
     path="/books",
     methods=[apigwv2.HttpMethod.GET],
@@ -253,30 +254,29 @@
 ```
 
 ### Mutual TLS (mTLS)
 
 Mutual TLS can be configured to limit access to your API based by using client certificates instead of (or as an extension of) using authorization headers.
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 import aws_cdk.aws_s3 as s3
-import aws_cdk.aws_certificatemanager as acm
-# bucket: s3.Bucket
-
 
 cert_arn = "arn:aws:acm:us-east-1:111111111111:certificate"
 domain_name = "example.com"
+bucket = s3.Bucket.from_bucket_name(stack, "TrustStoreBucket", ...)
 
-apigwv2.DomainName(self, "DomainName",
+DomainName(stack, "DomainName",
     domain_name=domain_name,
-    certificate=acm.Certificate.from_certificate_arn(self, "cert", cert_arn),
-    mtls=apigwv2.MTLSConfig(
-        bucket=bucket,
-        key="someca.pem",
-        version="version"
-    )
+    certificate=Certificate.from_certificate_arn(stack, "cert", cert_arn),
+    mtls={
+        "bucket": bucket,
+        "key": "someca.pem",
+        "version": "version"
+    }
 )
 ```
 
 Instructions for configuring your trust store can be found [here](https://aws.amazon.com/blogs/compute/introducing-mutual-tls-authentication-for-amazon-api-gateway/)
 
 ### Managing access to HTTP APIs
 
@@ -402,52 +402,32 @@
 
 web_socket_api = apigwv2.WebSocketApi(self, "mywsapi")
 web_socket_api.add_route("sendmessage",
     integration=WebSocketLambdaIntegration("SendMessageIntegration", message_handler)
 )
 ```
 
-To add a route that can return a result:
-
-```python
-from aws_cdk.aws_apigatewayv2_integrations_alpha import WebSocketLambdaIntegration
-
-# message_handler: lambda.Function
-
-web_socket_api = apigwv2.WebSocketApi(self, "mywsapi")
-web_socket_api.add_route("sendmessage",
-    integration=WebSocketLambdaIntegration("SendMessageIntegration", message_handler),
-    return_response=True
-)
-```
-
-To import an existing WebSocketApi:
-
-```python
-web_socket_api = apigwv2.WebSocketApi.from_web_socket_api_attributes(self, "mywsapi", web_socket_id="api-1234")
-```
-
 ### Manage Connections Permission
 
 Grant permission to use API Gateway Management API of a WebSocket API by calling the `grantManageConnections` API.
 You can use Management API to send a callback message to a connected client, get connection information, or disconnect the client. Learn more at [Use @connections commands in your backend service](https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-how-to-call-websocket-api-connections.html).
 
 ```python
-# fn: lambda.Function
-
+# Example automatically generated from non-compiling source. May contain errors.
+lambda_ = lambda_.Function(self, "lambda")
 
-web_socket_api = apigwv2.WebSocketApi(self, "mywsapi")
-stage = apigwv2.WebSocketStage(self, "mystage",
+web_socket_api = WebSocketApi(stack, "mywsapi")
+stage = WebSocketStage(stack, "mystage",
     web_socket_api=web_socket_api,
     stage_name="dev"
 )
 # per stage permission
-stage.grant_management_api_access(fn)
+stage.grant_manage_connections(lambda_)
 # for all the stages permission
-web_socket_api.grant_manage_connections(fn)
+web_socket_api.grant_manage_connections(lambda_)
 ```
 
 ### Managing access to WebSocket APIs
 
 API Gateway supports multiple mechanisms for [controlling and managing access to a WebSocket API](https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-websocket-api-control-access.html) through authorizers.
 
 These authorizers can be found in the [APIGatewayV2-Authorizers](https://docs.aws.amazon.com/cdk/api/latest/docs/aws-apigatewayv2-authorizers-readme.html) constructs library.
@@ -455,40 +435,39 @@
 ### API Keys
 
 Websocket APIs also support usage of API Keys. An API Key is a key that is used to grant access to an API. These are useful for controlling and tracking access to an API, when used together with [usage plans](https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-api-usage-plans.html). These together allow you to configure controls around API access such as quotas and throttling, along with per-API Key metrics on usage.
 
 To require an API Key when accessing the Websocket API:
 
 ```python
-web_socket_api = apigwv2.WebSocketApi(self, "mywsapi",
-    api_key_selection_expression=apigwv2.WebSocketApiKeySelectionExpression.HEADER_X_API_KEY
+# Example automatically generated from non-compiling source. May contain errors.
+web_socket_api = WebSocketApi(stack, "mywsapi",
+    api_key_selection_expression=WebSocketApiKeySelectionExpression.HEADER_X_API_KEY
 )
 ```
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
-import aws_cdk.aws_certificatemanager as _aws_cdk_aws_certificatemanager_ceddda9d
-import aws_cdk.aws_cloudwatch as _aws_cdk_aws_cloudwatch_ceddda9d
-import aws_cdk.aws_ec2 as _aws_cdk_aws_ec2_ceddda9d
-import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
-import aws_cdk.aws_s3 as _aws_cdk_aws_s3_ceddda9d
-import constructs as _constructs_77d1e7e8
+import aws_cdk
+import aws_cdk.aws_certificatemanager
+import aws_cdk.aws_cloudwatch
+import aws_cdk.aws_ec2
+import aws_cdk.aws_iam
+import aws_cdk.aws_s3
+import constructs
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.ApiMappingAttributes",
     jsii_struct_bases=[],
     name_mapping={"api_mapping_id": "apiMappingId"},
 )
@@ -507,18 +486,15 @@
             # The values are placeholders you should change.
             import aws_cdk.aws_apigatewayv2_alpha as apigatewayv2_alpha
             
             api_mapping_attributes = apigatewayv2_alpha.ApiMappingAttributes(
                 api_mapping_id="apiMappingId"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__742c0d28ff28876a0bc0d1152ef7b3343151f193a0e128ba64a6cbc4509c8f05)
-            check_type(argname="argument api_mapping_id", value=api_mapping_id, expected_type=type_hints["api_mapping_id"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "api_mapping_id": api_mapping_id,
         }
 
     @builtins.property
     def api_mapping_id(self) -> builtins.str:
         '''(experimental) The API mapping ID.
 
@@ -584,21 +560,15 @@
                 domain_name=domain_name,
             
                 # the properties below are optional
                 api_mapping_key="apiMappingKey",
                 stage=stage
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__75ffb83f83ec42f2a0382885c05d069ecb32c50d82d796df38b991d84782ded6)
-            check_type(argname="argument api", value=api, expected_type=type_hints["api"])
-            check_type(argname="argument domain_name", value=domain_name, expected_type=type_hints["domain_name"])
-            check_type(argname="argument api_mapping_key", value=api_mapping_key, expected_type=type_hints["api_mapping_key"])
-            check_type(argname="argument stage", value=stage, expected_type=type_hints["stage"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "api": api,
             "domain_name": domain_name,
         }
         if api_mapping_key is not None:
             self._values["api_mapping_key"] = api_mapping_key
         if stage is not None:
             self._values["stage"] = stage
@@ -703,18 +673,15 @@
             
             # http_route_integration: apigatewayv2_alpha.HttpRouteIntegration
             
             batch_http_route_options = apigatewayv2_alpha.BatchHttpRouteOptions(
                 integration=http_route_integration
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__dd6be8693e2cd2875856654344853bc620de9c6dd3e82fbd384cba9b5468a36d)
-            check_type(argname="argument integration", value=integration, expected_type=type_hints["integration"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "integration": integration,
         }
 
     @builtins.property
     def integration(self) -> "HttpRouteIntegration":
         '''(experimental) The integration to be configured on this route.
 
@@ -815,15 +782,15 @@
         self,
         *,
         allow_credentials: typing.Optional[builtins.bool] = None,
         allow_headers: typing.Optional[typing.Sequence[builtins.str]] = None,
         allow_methods: typing.Optional[typing.Sequence[CorsHttpMethod]] = None,
         allow_origins: typing.Optional[typing.Sequence[builtins.str]] = None,
         expose_headers: typing.Optional[typing.Sequence[builtins.str]] = None,
-        max_age: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        max_age: typing.Optional[aws_cdk.Duration] = None,
     ) -> None:
         '''(experimental) Options for the CORS Configuration.
 
         :param allow_credentials: (experimental) Specifies whether credentials are included in the CORS request. Default: false
         :param allow_headers: (experimental) Represents a collection of allowed headers. Default: - No Headers are allowed.
         :param allow_methods: (experimental) Represents a collection of allowed HTTP methods. Default: - No Methods are allowed.
         :param allow_origins: (experimental) Represents a collection of allowed origins. Default: - No Origins are allowed.
@@ -841,23 +808,15 @@
                     allow_methods=[apigwv2.CorsHttpMethod.GET, apigwv2.CorsHttpMethod.HEAD, apigwv2.CorsHttpMethod.OPTIONS, apigwv2.CorsHttpMethod.POST
                     ],
                     allow_origins=["*"],
                     max_age=Duration.days(10)
                 )
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a8623074d52aadb0b4dc416f52273d5e1695739d7da72a818e4a16b0988313fa)
-            check_type(argname="argument allow_credentials", value=allow_credentials, expected_type=type_hints["allow_credentials"])
-            check_type(argname="argument allow_headers", value=allow_headers, expected_type=type_hints["allow_headers"])
-            check_type(argname="argument allow_methods", value=allow_methods, expected_type=type_hints["allow_methods"])
-            check_type(argname="argument allow_origins", value=allow_origins, expected_type=type_hints["allow_origins"])
-            check_type(argname="argument expose_headers", value=expose_headers, expected_type=type_hints["expose_headers"])
-            check_type(argname="argument max_age", value=max_age, expected_type=type_hints["max_age"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if allow_credentials is not None:
             self._values["allow_credentials"] = allow_credentials
         if allow_headers is not None:
             self._values["allow_headers"] = allow_headers
         if allow_methods is not None:
             self._values["allow_methods"] = allow_methods
         if allow_origins is not None:
@@ -919,23 +878,23 @@
 
         :stability: experimental
         '''
         result = self._values.get("expose_headers")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
-    def max_age(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+    def max_age(self) -> typing.Optional[aws_cdk.Duration]:
         '''(experimental) The duration that the browser should cache preflight request results.
 
         :default: Duration.seconds(0)
 
         :stability: experimental
         '''
         result = self._values.get("max_age")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
+        return typing.cast(typing.Optional[aws_cdk.Duration], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -978,19 +937,15 @@
                 # https://${dn.domainName}/demo goes to apiDemo $default stage
                 default_domain_mapping=apigwv2.DomainMappingOptions(
                     domain_name=dn,
                     mapping_key="demo"
                 )
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b9c022929eefc93f95859e1c88a0b0f15538c5b557fbe539653100b894c61520)
-            check_type(argname="argument domain_name", value=domain_name, expected_type=type_hints["domain_name"])
-            check_type(argname="argument mapping_key", value=mapping_key, expected_type=type_hints["mapping_key"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "domain_name": domain_name,
         }
         if mapping_key is not None:
             self._values["mapping_key"] = mapping_key
 
     @builtins.property
     def domain_name(self) -> "IDomainName":
@@ -1061,20 +1016,15 @@
             
             domain_name_attributes = apigatewayv2_alpha.DomainNameAttributes(
                 name="name",
                 regional_domain_name="regionalDomainName",
                 regional_hosted_zone_id="regionalHostedZoneId"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e3a28ea7d17c0cb32594b624176b2b5339560671719297d538c51a793079d6f8)
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
-            check_type(argname="argument regional_domain_name", value=regional_domain_name, expected_type=type_hints["regional_domain_name"])
-            check_type(argname="argument regional_hosted_zone_id", value=regional_hosted_zone_id, expected_type=type_hints["regional_hosted_zone_id"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "name": name,
             "regional_domain_name": regional_domain_name,
             "regional_hosted_zone_id": regional_hosted_zone_id,
         }
 
     @builtins.property
     def name(self) -> builtins.str:
@@ -1129,18 +1079,18 @@
         "security_policy": "securityPolicy",
     },
 )
 class EndpointOptions:
     def __init__(
         self,
         *,
-        certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
+        certificate: aws_cdk.aws_certificatemanager.ICertificate,
         certificate_name: typing.Optional[builtins.str] = None,
         endpoint_type: typing.Optional["EndpointType"] = None,
-        ownership_certificate: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
+        ownership_certificate: typing.Optional[aws_cdk.aws_certificatemanager.ICertificate] = None,
         security_policy: typing.Optional["SecurityPolicy"] = None,
     ) -> None:
         '''(experimental) properties for creating a domain name endpoint.
 
         :param certificate: (experimental) The ACM certificate for this domain name. Certificate can be both ACM issued or imported.
         :param certificate_name: (experimental) The user-friendly name of the certificate that will be used by the endpoint for this domain name. Default: - No friendly certificate name
         :param endpoint_type: (experimental) The type of endpoint for this DomainName. Default: EndpointType.REGIONAL
@@ -1165,44 +1115,37 @@
                 # the properties below are optional
                 certificate_name="certificateName",
                 endpoint_type=apigatewayv2_alpha.EndpointType.EDGE,
                 ownership_certificate=certificate,
                 security_policy=apigatewayv2_alpha.SecurityPolicy.TLS_1_0
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0a18b13421aac912723b2ab35f8a14b008971c520719c36b6764e8ff2bd43194)
-            check_type(argname="argument certificate", value=certificate, expected_type=type_hints["certificate"])
-            check_type(argname="argument certificate_name", value=certificate_name, expected_type=type_hints["certificate_name"])
-            check_type(argname="argument endpoint_type", value=endpoint_type, expected_type=type_hints["endpoint_type"])
-            check_type(argname="argument ownership_certificate", value=ownership_certificate, expected_type=type_hints["ownership_certificate"])
-            check_type(argname="argument security_policy", value=security_policy, expected_type=type_hints["security_policy"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "certificate": certificate,
         }
         if certificate_name is not None:
             self._values["certificate_name"] = certificate_name
         if endpoint_type is not None:
             self._values["endpoint_type"] = endpoint_type
         if ownership_certificate is not None:
             self._values["ownership_certificate"] = ownership_certificate
         if security_policy is not None:
             self._values["security_policy"] = security_policy
 
     @builtins.property
-    def certificate(self) -> _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate:
+    def certificate(self) -> aws_cdk.aws_certificatemanager.ICertificate:
         '''(experimental) The ACM certificate for this domain name.
 
         Certificate can be both ACM issued or imported.
 
         :stability: experimental
         '''
         result = self._values.get("certificate")
         assert result is not None, "Required property 'certificate' is missing"
-        return typing.cast(_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate, result)
+        return typing.cast(aws_cdk.aws_certificatemanager.ICertificate, result)
 
     @builtins.property
     def certificate_name(self) -> typing.Optional[builtins.str]:
         '''(experimental) The user-friendly name of the certificate that will be used by the endpoint for this domain name.
 
         :default: - No friendly certificate name
 
@@ -1221,27 +1164,27 @@
         '''
         result = self._values.get("endpoint_type")
         return typing.cast(typing.Optional["EndpointType"], result)
 
     @builtins.property
     def ownership_certificate(
         self,
-    ) -> typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate]:
+    ) -> typing.Optional[aws_cdk.aws_certificatemanager.ICertificate]:
         '''(experimental) A public certificate issued by ACM to validate that you own a custom domain.
 
         This parameter is required
         only when you configure mutual TLS authentication and you specify an ACM imported or private CA certificate
         for ``certificate``. The ownership certificate validates that you have permissions to use the domain name.
 
         :default: - only required when configuring mTLS
 
         :stability: experimental
         '''
         result = self._values.get("ownership_certificate")
-        return typing.cast(typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_certificatemanager.ICertificate], result)
 
     @builtins.property
     def security_policy(self) -> typing.Optional["SecurityPolicy"]:
         '''(experimental) The Transport Layer Security (TLS) version + cipher suite for this domain name.
 
         :default: SecurityPolicy.TLS_1_2
 
@@ -1305,18 +1248,15 @@
             # The values are placeholders you should change.
             import aws_cdk.aws_apigatewayv2_alpha as apigatewayv2_alpha
             
             grant_invoke_options = apigatewayv2_alpha.GrantInvokeOptions(
                 http_methods=[apigatewayv2_alpha.HttpMethod.ANY]
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a82686daa9fd8d0f3123464a3edac12340e9f588999872022e157589c9935c8a)
-            check_type(argname="argument http_methods", value=http_methods, expected_type=type_hints["http_methods"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if http_methods is not None:
             self._values["http_methods"] = http_methods
 
     @builtins.property
     def http_methods(self) -> typing.Optional[typing.List["HttpMethod"]]:
         '''(experimental) The HTTP methods to allow.
 
@@ -1368,19 +1308,15 @@
             http_api_attributes = apigatewayv2_alpha.HttpApiAttributes(
                 http_api_id="httpApiId",
             
                 # the properties below are optional
                 api_endpoint="apiEndpoint"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ca86693c779a127085f398e4f4b28effbcaffb7b0e4c3586085ba8720c18c3b6)
-            check_type(argname="argument http_api_id", value=http_api_id, expected_type=type_hints["http_api_id"])
-            check_type(argname="argument api_endpoint", value=api_endpoint, expected_type=type_hints["api_endpoint"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "http_api_id": http_api_id,
         }
         if api_endpoint is not None:
             self._values["api_endpoint"] = api_endpoint
 
     @builtins.property
     def http_api_id(self) -> builtins.str:
@@ -1431,19 +1367,19 @@
     },
 )
 class HttpApiProps:
     def __init__(
         self,
         *,
         api_name: typing.Optional[builtins.str] = None,
-        cors_preflight: typing.Optional[typing.Union[CorsPreflightOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        cors_preflight: typing.Optional[CorsPreflightOptions] = None,
         create_default_stage: typing.Optional[builtins.bool] = None,
         default_authorization_scopes: typing.Optional[typing.Sequence[builtins.str]] = None,
         default_authorizer: typing.Optional["IHttpRouteAuthorizer"] = None,
-        default_domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        default_domain_mapping: typing.Optional[DomainMappingOptions] = None,
         default_integration: typing.Optional["HttpRouteIntegration"] = None,
         description: typing.Optional[builtins.str] = None,
         disable_execute_api_endpoint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''(experimental) Properties to initialize an instance of ``HttpApi``.
 
         :param api_name: (experimental) Name for the HTTP API resource. Default: - id of the HttpApi construct.
@@ -1476,26 +1412,15 @@
                 )
             )
         '''
         if isinstance(cors_preflight, dict):
             cors_preflight = CorsPreflightOptions(**cors_preflight)
         if isinstance(default_domain_mapping, dict):
             default_domain_mapping = DomainMappingOptions(**default_domain_mapping)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__61f68792e068176f35bfd5b9b8d36c51601ad6882e6aa3ce1c951683b5d199d2)
-            check_type(argname="argument api_name", value=api_name, expected_type=type_hints["api_name"])
-            check_type(argname="argument cors_preflight", value=cors_preflight, expected_type=type_hints["cors_preflight"])
-            check_type(argname="argument create_default_stage", value=create_default_stage, expected_type=type_hints["create_default_stage"])
-            check_type(argname="argument default_authorization_scopes", value=default_authorization_scopes, expected_type=type_hints["default_authorization_scopes"])
-            check_type(argname="argument default_authorizer", value=default_authorizer, expected_type=type_hints["default_authorizer"])
-            check_type(argname="argument default_domain_mapping", value=default_domain_mapping, expected_type=type_hints["default_domain_mapping"])
-            check_type(argname="argument default_integration", value=default_integration, expected_type=type_hints["default_integration"])
-            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
-            check_type(argname="argument disable_execute_api_endpoint", value=disable_execute_api_endpoint, expected_type=type_hints["disable_execute_api_endpoint"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if api_name is not None:
             self._values["api_name"] = api_name
         if cors_preflight is not None:
             self._values["cors_preflight"] = cors_preflight
         if create_default_stage is not None:
             self._values["create_default_stage"] = create_default_stage
         if default_authorization_scopes is not None:
@@ -1659,19 +1584,15 @@
             import aws_cdk.aws_apigatewayv2_alpha as apigatewayv2_alpha
             
             http_authorizer_attributes = apigatewayv2_alpha.HttpAuthorizerAttributes(
                 authorizer_id="authorizerId",
                 authorizer_type="authorizerType"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e213cc5ff1a6a50f727adfa1a93746afabbb568dc170da0d58f5c5f6b4a65877)
-            check_type(argname="argument authorizer_id", value=authorizer_id, expected_type=type_hints["authorizer_id"])
-            check_type(argname="argument authorizer_type", value=authorizer_type, expected_type=type_hints["authorizer_type"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "authorizer_id": authorizer_id,
             "authorizer_type": authorizer_type,
         }
 
     @builtins.property
     def authorizer_id(self) -> builtins.str:
         '''(experimental) Id of the Authorizer.
@@ -1735,15 +1656,15 @@
         type: "HttpAuthorizerType",
         authorizer_name: typing.Optional[builtins.str] = None,
         authorizer_uri: typing.Optional[builtins.str] = None,
         enable_simple_responses: typing.Optional[builtins.bool] = None,
         jwt_audience: typing.Optional[typing.Sequence[builtins.str]] = None,
         jwt_issuer: typing.Optional[builtins.str] = None,
         payload_format_version: typing.Optional[AuthorizerPayloadVersion] = None,
-        results_cache_ttl: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        results_cache_ttl: typing.Optional[aws_cdk.Duration] = None,
     ) -> None:
         '''(experimental) Properties to initialize an instance of ``HttpAuthorizer``.
 
         :param http_api: (experimental) HTTP Api to attach the authorizer to.
         :param identity_source: (experimental) The identity source for which authorization is requested.
         :param type: (experimental) The type of authorizer.
         :param authorizer_name: (experimental) Name of the authorizer. Default: - id of the HttpAuthorizer construct.
@@ -1777,27 +1698,15 @@
                 enable_simple_responses=False,
                 jwt_audience=["jwtAudience"],
                 jwt_issuer="jwtIssuer",
                 payload_format_version=apigatewayv2_alpha.AuthorizerPayloadVersion.VERSION_1_0,
                 results_cache_ttl=cdk.Duration.minutes(30)
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__270c2096601be45fba89ecb508234f5870eaabd6d21813bc090ce9b1a459264d)
-            check_type(argname="argument http_api", value=http_api, expected_type=type_hints["http_api"])
-            check_type(argname="argument identity_source", value=identity_source, expected_type=type_hints["identity_source"])
-            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
-            check_type(argname="argument authorizer_name", value=authorizer_name, expected_type=type_hints["authorizer_name"])
-            check_type(argname="argument authorizer_uri", value=authorizer_uri, expected_type=type_hints["authorizer_uri"])
-            check_type(argname="argument enable_simple_responses", value=enable_simple_responses, expected_type=type_hints["enable_simple_responses"])
-            check_type(argname="argument jwt_audience", value=jwt_audience, expected_type=type_hints["jwt_audience"])
-            check_type(argname="argument jwt_issuer", value=jwt_issuer, expected_type=type_hints["jwt_issuer"])
-            check_type(argname="argument payload_format_version", value=payload_format_version, expected_type=type_hints["payload_format_version"])
-            check_type(argname="argument results_cache_ttl", value=results_cache_ttl, expected_type=type_hints["results_cache_ttl"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "http_api": http_api,
             "identity_source": identity_source,
             "type": type,
         }
         if authorizer_name is not None:
             self._values["authorizer_name"] = authorizer_name
         if authorizer_uri is not None:
@@ -1913,25 +1822,25 @@
 
         :stability: experimental
         '''
         result = self._values.get("payload_format_version")
         return typing.cast(typing.Optional[AuthorizerPayloadVersion], result)
 
     @builtins.property
-    def results_cache_ttl(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+    def results_cache_ttl(self) -> typing.Optional[aws_cdk.Duration]:
         '''(experimental) How long APIGateway should cache the results.
 
         Max 1 hour.
 
         :default: - API Gateway will not cache authorizer responses
 
         :stability: experimental
         '''
         result = self._values.get("results_cache_ttl")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
+        return typing.cast(typing.Optional[aws_cdk.Duration], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -2057,28 +1966,15 @@
                 integration_uri="integrationUri",
                 method=apigatewayv2_alpha.HttpMethod.ANY,
                 parameter_mapping=parameter_mapping,
                 payload_format_version=payload_format_version,
                 secure_server_name="secureServerName"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0e70b5fc9ef16c84251eedf90fb9f4578a5231e285c86d485055a9875610b863)
-            check_type(argname="argument http_api", value=http_api, expected_type=type_hints["http_api"])
-            check_type(argname="argument integration_type", value=integration_type, expected_type=type_hints["integration_type"])
-            check_type(argname="argument connection_id", value=connection_id, expected_type=type_hints["connection_id"])
-            check_type(argname="argument connection_type", value=connection_type, expected_type=type_hints["connection_type"])
-            check_type(argname="argument credentials", value=credentials, expected_type=type_hints["credentials"])
-            check_type(argname="argument integration_subtype", value=integration_subtype, expected_type=type_hints["integration_subtype"])
-            check_type(argname="argument integration_uri", value=integration_uri, expected_type=type_hints["integration_uri"])
-            check_type(argname="argument method", value=method, expected_type=type_hints["method"])
-            check_type(argname="argument parameter_mapping", value=parameter_mapping, expected_type=type_hints["parameter_mapping"])
-            check_type(argname="argument payload_format_version", value=payload_format_version, expected_type=type_hints["payload_format_version"])
-            check_type(argname="argument secure_server_name", value=secure_server_name, expected_type=type_hints["secure_server_name"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "http_api": http_api,
             "integration_type": integration_type,
         }
         if connection_id is not None:
             self._values["connection_id"] = connection_id
         if connection_type is not None:
             self._values["connection_type"] = connection_type
@@ -2332,20 +2228,21 @@
     '''(experimental) Supported HTTP methods.
 
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
+        # Example automatically generated from non-compiling source. May contain errors.
         from aws_cdk.aws_apigatewayv2_integrations_alpha import HttpUrlIntegration, HttpLambdaIntegration
         
         # books_default_fn: lambda.Function
         
         
-        get_books_integration = HttpUrlIntegration("GetBooksIntegration", "https://get-books-proxy.example.com")
+        get_books_integration = HttpUrlIntegration("GetBooksIntegration", "https://get-books-proxy.myproxy.internal")
         books_default_integration = HttpLambdaIntegration("BooksIntegration", books_default_fn)
         
         http_api = apigwv2.HttpApi(self, "HttpApi")
         
         http_api.add_routes(
             path="/books",
             methods=[apigwv2.HttpMethod.GET],
@@ -2402,20 +2299,15 @@
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.HttpRouteAuthorizerBindOptions",
     jsii_struct_bases=[],
     name_mapping={"route": "route", "scope": "scope"},
 )
 class HttpRouteAuthorizerBindOptions:
-    def __init__(
-        self,
-        *,
-        route: "IHttpRoute",
-        scope: _constructs_77d1e7e8.Construct,
-    ) -> None:
+    def __init__(self, *, route: "IHttpRoute", scope: constructs.Construct) -> None:
         '''(experimental) Input to the bind() operation, that binds an authorizer to a route.
 
         :param route: (experimental) The route to which the authorizer is being bound.
         :param scope: (experimental) The scope for any constructs created as part of the bind.
 
         :stability: experimental
         :exampleMetadata: fixture=_generated
@@ -2431,19 +2323,15 @@
             # http_route: apigatewayv2_alpha.HttpRoute
             
             http_route_authorizer_bind_options = apigatewayv2_alpha.HttpRouteAuthorizerBindOptions(
                 route=http_route,
                 scope=construct
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__327eab42c70e54708c05239cc92e1d413d8f439a24b6448c6de2d0f2d4df7521)
-            check_type(argname="argument route", value=route, expected_type=type_hints["route"])
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "route": route,
             "scope": scope,
         }
 
     @builtins.property
     def route(self) -> "IHttpRoute":
         '''(experimental) The route to which the authorizer is being bound.
@@ -2451,22 +2339,22 @@
         :stability: experimental
         '''
         result = self._values.get("route")
         assert result is not None, "Required property 'route' is missing"
         return typing.cast("IHttpRoute", result)
 
     @builtins.property
-    def scope(self) -> _constructs_77d1e7e8.Construct:
+    def scope(self) -> constructs.Construct:
         '''(experimental) The scope for any constructs created as part of the bind.
 
         :stability: experimental
         '''
         result = self._values.get("scope")
         assert result is not None, "Required property 'scope' is missing"
-        return typing.cast(_constructs_77d1e7e8.Construct, result)
+        return typing.cast(constructs.Construct, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -2512,20 +2400,15 @@
                 authorization_type="authorizationType",
             
                 # the properties below are optional
                 authorization_scopes=["authorizationScopes"],
                 authorizer_id="authorizerId"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__23fa1130cc8cec3f96c4c7be76f4fde0189dfa2fd6410ede8be1c8e24a88a0f2)
-            check_type(argname="argument authorization_type", value=authorization_type, expected_type=type_hints["authorization_type"])
-            check_type(argname="argument authorization_scopes", value=authorization_scopes, expected_type=type_hints["authorization_scopes"])
-            check_type(argname="argument authorizer_id", value=authorizer_id, expected_type=type_hints["authorizer_id"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "authorization_type": authorization_type,
         }
         if authorization_scopes is not None:
             self._values["authorization_scopes"] = authorization_scopes
         if authorizer_id is not None:
             self._values["authorizer_id"] = authorizer_id
 
@@ -2610,69 +2493,41 @@
     def __init__(self, id: builtins.str) -> None:
         '''(experimental) Initialize an integration for a route on http api.
 
         :param id: id of the underlying ``HttpIntegration`` construct.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0d2d16b160325ee41bba7780d2678d810d12da5f663f886f5c8a810a06c66fef)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         jsii.create(self.__class__, self, [id])
 
-    @jsii.member(jsii_name="bind")
+    @jsii.member(jsii_name="bind") # type: ignore[misc]
     @abc.abstractmethod
     def bind(
         self,
         *,
         route: "IHttpRoute",
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
     ) -> "HttpRouteIntegrationConfig":
         '''(experimental) Bind this integration to the route.
 
         :param route: (experimental) The route to which this is being bound.
         :param scope: (experimental) The current scope in which the bind is occurring. If the ``HttpRouteIntegration`` being bound creates additional constructs, this will be used as their parent scope.
 
         :stability: experimental
         '''
         ...
 
-    @jsii.member(jsii_name="completeBind")
-    def _complete_bind(
-        self,
-        *,
-        route: "IHttpRoute",
-        scope: _constructs_77d1e7e8.Construct,
-    ) -> None:
-        '''(experimental) Complete the binding of the integration to the route.
-
-        In some cases, there is
-        some additional work to do, such as adding permissions for the API to access
-        the target. This work is necessary whether the integration has just been
-        created for this route or it is an existing one, previously created for other
-        routes. In most cases, however, concrete implementations do not need to
-        override this method.
-
-        :param route: (experimental) The route to which this is being bound.
-        :param scope: (experimental) The current scope in which the bind is occurring. If the ``HttpRouteIntegration`` being bound creates additional constructs, this will be used as their parent scope.
-
-        :stability: experimental
-        '''
-        _options = HttpRouteIntegrationBindOptions(route=route, scope=scope)
-
-        return typing.cast(None, jsii.invoke(self, "completeBind", [_options]))
-
 
 class _HttpRouteIntegrationProxy(HttpRouteIntegration):
     @jsii.member(jsii_name="bind")
     def bind(
         self,
         *,
         route: "IHttpRoute",
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
     ) -> "HttpRouteIntegrationConfig":
         '''(experimental) Bind this integration to the route.
 
         :param route: (experimental) The route to which this is being bound.
         :param scope: (experimental) The current scope in which the bind is occurring. If the ``HttpRouteIntegration`` being bound creates additional constructs, this will be used as their parent scope.
 
         :stability: experimental
@@ -2687,20 +2542,15 @@
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.HttpRouteIntegrationBindOptions",
     jsii_struct_bases=[],
     name_mapping={"route": "route", "scope": "scope"},
 )
 class HttpRouteIntegrationBindOptions:
-    def __init__(
-        self,
-        *,
-        route: "IHttpRoute",
-        scope: _constructs_77d1e7e8.Construct,
-    ) -> None:
+    def __init__(self, *, route: "IHttpRoute", scope: constructs.Construct) -> None:
         '''(experimental) Options to the HttpRouteIntegration during its bind operation.
 
         :param route: (experimental) The route to which this is being bound.
         :param scope: (experimental) The current scope in which the bind is occurring. If the ``HttpRouteIntegration`` being bound creates additional constructs, this will be used as their parent scope.
 
         :stability: experimental
         :exampleMetadata: fixture=_generated
@@ -2716,19 +2566,15 @@
             # http_route: apigatewayv2_alpha.HttpRoute
             
             http_route_integration_bind_options = apigatewayv2_alpha.HttpRouteIntegrationBindOptions(
                 route=http_route,
                 scope=construct
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fee001518b0d0335530b5174be6d0d04745ad94a5bffe05a6d9007712a52eb52)
-            check_type(argname="argument route", value=route, expected_type=type_hints["route"])
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "route": route,
             "scope": scope,
         }
 
     @builtins.property
     def route(self) -> "IHttpRoute":
         '''(experimental) The route to which this is being bound.
@@ -2736,25 +2582,25 @@
         :stability: experimental
         '''
         result = self._values.get("route")
         assert result is not None, "Required property 'route' is missing"
         return typing.cast("IHttpRoute", result)
 
     @builtins.property
-    def scope(self) -> _constructs_77d1e7e8.Construct:
+    def scope(self) -> constructs.Construct:
         '''(experimental) The current scope in which the bind is occurring.
 
         If the ``HttpRouteIntegration`` being bound creates additional constructs,
         this will be used as their parent scope.
 
         :stability: experimental
         '''
         result = self._values.get("scope")
         assert result is not None, "Required property 'scope' is missing"
-        return typing.cast(_constructs_77d1e7e8.Construct, result)
+        return typing.cast(constructs.Construct, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -2832,27 +2678,15 @@
                 method=apigatewayv2_alpha.HttpMethod.ANY,
                 parameter_mapping=parameter_mapping,
                 secure_server_name="secureServerName",
                 subtype=apigatewayv2_alpha.HttpIntegrationSubtype.EVENTBRIDGE_PUT_EVENTS,
                 uri="uri"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8d07656a3841a48dd4643d0e10742dee8735d4fa1b6dec4e77afe67a3c12f2dd)
-            check_type(argname="argument payload_format_version", value=payload_format_version, expected_type=type_hints["payload_format_version"])
-            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
-            check_type(argname="argument connection_id", value=connection_id, expected_type=type_hints["connection_id"])
-            check_type(argname="argument connection_type", value=connection_type, expected_type=type_hints["connection_type"])
-            check_type(argname="argument credentials", value=credentials, expected_type=type_hints["credentials"])
-            check_type(argname="argument method", value=method, expected_type=type_hints["method"])
-            check_type(argname="argument parameter_mapping", value=parameter_mapping, expected_type=type_hints["parameter_mapping"])
-            check_type(argname="argument secure_server_name", value=secure_server_name, expected_type=type_hints["secure_server_name"])
-            check_type(argname="argument subtype", value=subtype, expected_type=type_hints["subtype"])
-            check_type(argname="argument uri", value=uri, expected_type=type_hints["uri"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "payload_format_version": payload_format_version,
             "type": type,
         }
         if connection_id is not None:
             self._values["connection_id"] = connection_id
         if connection_type is not None:
             self._values["connection_type"] = connection_type
@@ -3014,62 +2848,58 @@
         # The code below shows an example of how to instantiate this type.
         # The values are placeholders you should change.
         import aws_cdk.aws_apigatewayv2_alpha as apigatewayv2_alpha
         
         http_route_key = apigatewayv2_alpha.HttpRouteKey.with("path", apigatewayv2_alpha.HttpMethod.ANY)
     '''
 
-    @jsii.member(jsii_name="with")
+    @jsii.member(jsii_name="with") # type: ignore[misc]
     @builtins.classmethod
     def with_(
         cls,
         path: builtins.str,
         method: typing.Optional[HttpMethod] = None,
     ) -> "HttpRouteKey":
         '''(experimental) Create a route key with the combination of the path and the method.
 
         :param path: -
         :param method: default is 'ANY'.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__757949aa83516e4dc3de82eaf70c9ec58058087715b274d9a080b33530b01213)
-            check_type(argname="argument path", value=path, expected_type=type_hints["path"])
-            check_type(argname="argument method", value=method, expected_type=type_hints["method"])
         return typing.cast("HttpRouteKey", jsii.sinvoke(cls, "with", [path, method]))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="DEFAULT")
     def DEFAULT(cls) -> "HttpRouteKey":
         '''(experimental) The catch-all route of the API, i.e., when no other routes match.
 
         :stability: experimental
         '''
         return typing.cast("HttpRouteKey", jsii.sget(cls, "DEFAULT"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="key")
     def key(self) -> builtins.str:
         '''(experimental) The key to the RouteKey as recognized by APIGateway.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "key"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="method")
     def method(self) -> HttpMethod:
         '''(experimental) The method of the route.
 
         :stability: experimental
         '''
         return typing.cast(HttpMethod, jsii.get(self, "method"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="path")
     def path(self) -> typing.Optional[builtins.str]:
         '''(experimental) The path part of this RouteKey.
 
         Returns ``undefined`` when ``RouteKey.DEFAULT`` is used.
 
         :stability: experimental
@@ -3126,22 +2956,15 @@
                 route_key=http_route_key,
             
                 # the properties below are optional
                 authorization_scopes=["authorizationScopes"],
                 authorizer=http_route_authorizer
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a43a4a903025b4c98824c40d09ba7a3ec865a0a5902fb4f311846b446c460133)
-            check_type(argname="argument integration", value=integration, expected_type=type_hints["integration"])
-            check_type(argname="argument http_api", value=http_api, expected_type=type_hints["http_api"])
-            check_type(argname="argument route_key", value=route_key, expected_type=type_hints["route_key"])
-            check_type(argname="argument authorization_scopes", value=authorization_scopes, expected_type=type_hints["authorization_scopes"])
-            check_type(argname="argument authorizer", value=authorizer, expected_type=type_hints["authorizer"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "integration": integration,
             "http_api": http_api,
             "route_key": route_key,
         }
         if authorization_scopes is not None:
             self._values["authorization_scopes"] = authorization_scopes
         if authorizer is not None:
@@ -3212,31 +3035,31 @@
     def __repr__(self) -> str:
         return "HttpRouteProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-apigatewayv2-alpha.IApi")
-class IApi(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class IApi(aws_cdk.IResource, typing_extensions.Protocol):
     '''(experimental) Represents a API Gateway HTTP/WebSocket API.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="apiEndpoint")
     def api_endpoint(self) -> builtins.str:
         '''(experimental) The default endpoint for an API.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="apiId")
     def api_id(self) -> builtins.str:
         '''(experimental) The identifier of this API Gateway API.
 
         :stability: experimental
         :attribute: true
         '''
@@ -3247,59 +3070,59 @@
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
         '''(experimental) Return the given named metric for this Api Gateway.
 
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
 
         :default: - average over 5 minutes
 
         :stability: experimental
         '''
         ...
 
 
 class _IApiProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''(experimental) Represents a API Gateway HTTP/WebSocket API.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IApi"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="apiEndpoint")
     def api_endpoint(self) -> builtins.str:
         '''(experimental) The default endpoint for an API.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "apiEndpoint"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="apiId")
     def api_id(self) -> builtins.str:
         '''(experimental) The identifier of this API Gateway API.
 
         :stability: experimental
         :attribute: true
         '''
@@ -3310,212 +3133,209 @@
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
         '''(experimental) Return the given named metric for this Api Gateway.
 
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
 
         :default: - average over 5 minutes
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c475fcfbd8ec2d43f9f067afa8d49c21d334d5c85f25834be833f0c107d99e8e)
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
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IApi).__jsii_proxy_class__ = lambda : _IApiProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-apigatewayv2-alpha.IApiMapping")
-class IApiMapping(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class IApiMapping(aws_cdk.IResource, typing_extensions.Protocol):
     '''(experimental) Represents an ApiGatewayV2 ApiMapping resource.
 
     :see: https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-apigatewayv2-apimapping.html
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="apiMappingId")
     def api_mapping_id(self) -> builtins.str:
         '''(experimental) ID of the api mapping.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _IApiMappingProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''(experimental) Represents an ApiGatewayV2 ApiMapping resource.
 
     :see: https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-apigatewayv2-apimapping.html
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IApiMapping"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="apiMappingId")
     def api_mapping_id(self) -> builtins.str:
         '''(experimental) ID of the api mapping.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "apiMappingId"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IApiMapping).__jsii_proxy_class__ = lambda : _IApiMappingProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-apigatewayv2-alpha.IAuthorizer")
-class IAuthorizer(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class IAuthorizer(aws_cdk.IResource, typing_extensions.Protocol):
     '''(experimental) Represents an Authorizer.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="authorizerId")
     def authorizer_id(self) -> builtins.str:
         '''(experimental) Id of the Authorizer.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _IAuthorizerProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''(experimental) Represents an Authorizer.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IAuthorizer"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="authorizerId")
     def authorizer_id(self) -> builtins.str:
         '''(experimental) Id of the Authorizer.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "authorizerId"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IAuthorizer).__jsii_proxy_class__ = lambda : _IAuthorizerProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-apigatewayv2-alpha.IDomainName")
-class IDomainName(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class IDomainName(aws_cdk.IResource, typing_extensions.Protocol):
     '''(experimental) Represents an APIGatewayV2 DomainName.
 
     :see: https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-apigatewayv2-domainname.html
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         '''(experimental) The custom domain name.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="regionalDomainName")
     def regional_domain_name(self) -> builtins.str:
         '''(experimental) The domain name associated with the regional endpoint for this custom domain name.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="regionalHostedZoneId")
     def regional_hosted_zone_id(self) -> builtins.str:
         '''(experimental) The region-specific Amazon Route 53 Hosted Zone ID of the regional endpoint.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _IDomainNameProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''(experimental) Represents an APIGatewayV2 DomainName.
 
     :see: https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-apigatewayv2-domainname.html
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IDomainName"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         '''(experimental) The custom domain name.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "name"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="regionalDomainName")
     def regional_domain_name(self) -> builtins.str:
         '''(experimental) The domain name associated with the regional endpoint for this custom domain name.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "regionalDomainName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="regionalHostedZoneId")
     def regional_hosted_zone_id(self) -> builtins.str:
         '''(experimental) The region-specific Amazon Route 53 Hosted Zone ID of the regional endpoint.
 
         :stability: experimental
         :attribute: true
         '''
@@ -3528,15 +3348,15 @@
 @jsii.interface(jsii_type="@aws-cdk/aws-apigatewayv2-alpha.IHttpApi")
 class IHttpApi(IApi, typing_extensions.Protocol):
     '''(experimental) Represents an HTTP API.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="httpApiId")
     def http_api_id(self) -> builtins.str:
         '''(deprecated) The identifier of this API Gateway HTTP API.
 
         :deprecated: - use apiId instead
 
         :stability: deprecated
@@ -3544,17 +3364,17 @@
         '''
         ...
 
     @jsii.member(jsii_name="addVpcLink")
     def add_vpc_link(
         self,
         *,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-        subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        vpc: aws_cdk.aws_ec2.IVpc,
+        security_groups: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.ISecurityGroup]] = None,
+        subnets: typing.Optional[aws_cdk.aws_ec2.SubnetSelection] = None,
         vpc_link_name: typing.Optional[builtins.str] = None,
     ) -> "VpcLink":
         '''(experimental) Add a new VpcLink.
 
         :param vpc: (experimental) The VPC in which the private resources reside.
         :param security_groups: (experimental) A list of security groups for the VPC link. Default: - no security groups. Use ``addSecurityGroups`` to add security groups
         :param subnets: (experimental) A list of subnets for the VPC link. Default: - private subnets of the provided VPC. Use ``addSubnets`` to add more subnets
@@ -3568,28 +3388,28 @@
     def metric_client_error(
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
         '''(experimental) Metric for the number of client-side errors captured in a given period.
 
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
 
         :default: - sum over 5 minutes
 
         :stability: experimental
         '''
         ...
@@ -3598,28 +3418,28 @@
     def metric_count(
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
         '''(experimental) Metric for the total number API requests in a given period.
 
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
 
         :default: - SampleCount over 5 minutes
 
         :stability: experimental
         '''
         ...
@@ -3628,28 +3448,28 @@
     def metric_data_processed(
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
         '''(experimental) Metric for the amount of data processed in bytes.
 
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
 
         :default: - sum over 5 minutes
 
         :stability: experimental
         '''
         ...
@@ -3658,28 +3478,28 @@
     def metric_integration_latency(
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
         '''(experimental) Metric for the time between when API Gateway relays a request to the backend and when it receives a response from the backend.
 
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
 
         :default: - no statistic
 
         :stability: experimental
         '''
         ...
@@ -3688,30 +3508,30 @@
     def metric_latency(
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
         '''(experimental) The time between when API Gateway receives a request from a client and when it returns a response to the client.
 
         The latency includes the integration latency and other API Gateway overhead.
 
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
 
         :default: - no statistic
 
         :stability: experimental
         '''
         ...
@@ -3720,48 +3540,48 @@
     def metric_server_error(
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
         '''(experimental) Metric for the number of server-side errors captured in a given period.
 
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
 
         :default: - sum over 5 minutes
 
         :stability: experimental
         '''
         ...
 
 
 class _IHttpApiProxy(
-    jsii.proxy_for(IApi), # type: ignore[misc]
+    jsii.proxy_for(IApi) # type: ignore[misc]
 ):
     '''(experimental) Represents an HTTP API.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IHttpApi"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="httpApiId")
     def http_api_id(self) -> builtins.str:
         '''(deprecated) The identifier of this API Gateway HTTP API.
 
         :deprecated: - use apiId instead
 
         :stability: deprecated
@@ -3769,17 +3589,17 @@
         '''
         return typing.cast(builtins.str, jsii.get(self, "httpApiId"))
 
     @jsii.member(jsii_name="addVpcLink")
     def add_vpc_link(
         self,
         *,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-        subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        vpc: aws_cdk.aws_ec2.IVpc,
+        security_groups: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.ISecurityGroup]] = None,
+        subnets: typing.Optional[aws_cdk.aws_ec2.SubnetSelection] = None,
         vpc_link_name: typing.Optional[builtins.str] = None,
     ) -> "VpcLink":
         '''(experimental) Add a new VpcLink.
 
         :param vpc: (experimental) The VPC in which the private resources reside.
         :param security_groups: (experimental) A list of security groups for the VPC link. Default: - no security groups. Use ``addSecurityGroups`` to add security groups
         :param subnets: (experimental) A list of subnets for the VPC link. Default: - private subnets of the provided VPC. Use ``addSubnets`` to add more subnets
@@ -3800,253 +3620,253 @@
     def metric_client_error(
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
         '''(experimental) Metric for the number of client-side errors captured in a given period.
 
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
 
         :default: - sum over 5 minutes
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricClientError", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricClientError", [props]))
 
     @jsii.member(jsii_name="metricCount")
     def metric_count(
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
         '''(experimental) Metric for the total number API requests in a given period.
 
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
 
         :default: - SampleCount over 5 minutes
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricCount", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricCount", [props]))
 
     @jsii.member(jsii_name="metricDataProcessed")
     def metric_data_processed(
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
         '''(experimental) Metric for the amount of data processed in bytes.
 
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
 
         :default: - sum over 5 minutes
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricDataProcessed", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricDataProcessed", [props]))
 
     @jsii.member(jsii_name="metricIntegrationLatency")
     def metric_integration_latency(
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
         '''(experimental) Metric for the time between when API Gateway relays a request to the backend and when it receives a response from the backend.
 
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
 
         :default: - no statistic
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricIntegrationLatency", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricIntegrationLatency", [props]))
 
     @jsii.member(jsii_name="metricLatency")
     def metric_latency(
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
         '''(experimental) The time between when API Gateway receives a request from a client and when it returns a response to the client.
 
         The latency includes the integration latency and other API Gateway overhead.
 
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
 
         :default: - no statistic
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricLatency", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricLatency", [props]))
 
     @jsii.member(jsii_name="metricServerError")
     def metric_server_error(
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
         '''(experimental) Metric for the number of server-side errors captured in a given period.
 
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
 
         :default: - sum over 5 minutes
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricServerError", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricServerError", [props]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IHttpApi).__jsii_proxy_class__ = lambda : _IHttpApiProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-apigatewayv2-alpha.IHttpAuthorizer")
 class IHttpAuthorizer(IAuthorizer, typing_extensions.Protocol):
@@ -4055,15 +3875,15 @@
     :stability: experimental
     '''
 
     pass
 
 
 class _IHttpAuthorizerProxy(
-    jsii.proxy_for(IAuthorizer), # type: ignore[misc]
+    jsii.proxy_for(IAuthorizer) # type: ignore[misc]
 ):
     '''(experimental) An authorizer for HTTP APIs.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IHttpAuthorizer"
@@ -4081,15 +3901,15 @@
     '''
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
         *,
         route: "IHttpRoute",
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
     ) -> HttpRouteAuthorizerConfig:
         '''(experimental) Bind this authorizer to a specified Http route.
 
         :param route: (experimental) The route to which the authorizer is being bound.
         :param scope: (experimental) The scope for any constructs created as part of the bind.
 
         :stability: experimental
@@ -4106,15 +3926,15 @@
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IHttpRouteAuthorizer"
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
         *,
         route: "IHttpRoute",
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
     ) -> HttpRouteAuthorizerConfig:
         '''(experimental) Bind this authorizer to a specified Http route.
 
         :param route: (experimental) The route to which the authorizer is being bound.
         :param scope: (experimental) The scope for any constructs created as part of the bind.
 
         :stability: experimental
@@ -4124,42 +3944,42 @@
         return typing.cast(HttpRouteAuthorizerConfig, jsii.invoke(self, "bind", [options]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IHttpRouteAuthorizer).__jsii_proxy_class__ = lambda : _IHttpRouteAuthorizerProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-apigatewayv2-alpha.IIntegration")
-class IIntegration(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class IIntegration(aws_cdk.IResource, typing_extensions.Protocol):
     '''(experimental) Represents an integration to an API Route.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="integrationId")
     def integration_id(self) -> builtins.str:
         '''(experimental) Id of the integration.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _IIntegrationProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''(experimental) Represents an integration to an API Route.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IIntegration"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="integrationId")
     def integration_id(self) -> builtins.str:
         '''(experimental) Id of the integration.
 
         :stability: experimental
         :attribute: true
         '''
@@ -4172,15 +3992,15 @@
 @jsii.interface(jsii_type="@aws-cdk/aws-apigatewayv2-alpha.IMappingValue")
 class IMappingValue(typing_extensions.Protocol):
     '''(experimental) Represents a Mapping Value.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="value")
     def value(self) -> builtins.str:
         '''(experimental) Represents a Mapping Value.
 
         :stability: experimental
         '''
         ...
@@ -4190,89 +4010,89 @@
     '''(experimental) Represents a Mapping Value.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IMappingValue"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="value")
     def value(self) -> builtins.str:
         '''(experimental) Represents a Mapping Value.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "value"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IMappingValue).__jsii_proxy_class__ = lambda : _IMappingValueProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-apigatewayv2-alpha.IRoute")
-class IRoute(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class IRoute(aws_cdk.IResource, typing_extensions.Protocol):
     '''(experimental) Represents a route.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="routeId")
     def route_id(self) -> builtins.str:
         '''(experimental) Id of the Route.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _IRouteProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''(experimental) Represents a route.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IRoute"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="routeId")
     def route_id(self) -> builtins.str:
         '''(experimental) Id of the Route.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "routeId"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IRoute).__jsii_proxy_class__ = lambda : _IRouteProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-apigatewayv2-alpha.IStage")
-class IStage(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class IStage(aws_cdk.IResource, typing_extensions.Protocol):
     '''(experimental) Represents a Stage.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="stageName")
     def stage_name(self) -> builtins.str:
         '''(experimental) The name of the stage;
 
         its primary identifier.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="url")
     def url(self) -> builtins.str:
         '''(experimental) The URL to this stage.
 
         :stability: experimental
         '''
         ...
@@ -4282,61 +4102,61 @@
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
         '''(experimental) Return the given named metric for this HTTP Api Gateway Stage.
 
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
 
         :default: - average over 5 minutes
 
         :stability: experimental
         '''
         ...
 
 
 class _IStageProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''(experimental) Represents a Stage.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IStage"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="stageName")
     def stage_name(self) -> builtins.str:
         '''(experimental) The name of the stage;
 
         its primary identifier.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "stageName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="url")
     def url(self) -> builtins.str:
         '''(experimental) The URL to this stage.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "url"))
@@ -4346,102 +4166,99 @@
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
         '''(experimental) Return the given named metric for this HTTP Api Gateway Stage.
 
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
 
         :default: - average over 5 minutes
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d6eea31b2ea3d8439d0d065d266b0097b8fd2775bebde3b5b7cfc484683aa34a)
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
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IStage).__jsii_proxy_class__ = lambda : _IStageProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-apigatewayv2-alpha.IVpcLink")
-class IVpcLink(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class IVpcLink(aws_cdk.IResource, typing_extensions.Protocol):
     '''(experimental) Represents an API Gateway VpcLink.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="vpc")
-    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
+    def vpc(self) -> aws_cdk.aws_ec2.IVpc:
         '''(experimental) The VPC to which this VPC Link is associated with.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="vpcLinkId")
     def vpc_link_id(self) -> builtins.str:
         '''(experimental) Physical ID of the VpcLink resource.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _IVpcLinkProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''(experimental) Represents an API Gateway VpcLink.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IVpcLink"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="vpc")
-    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
+    def vpc(self) -> aws_cdk.aws_ec2.IVpc:
         '''(experimental) The VPC to which this VPC Link is associated with.
 
         :stability: experimental
         '''
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, jsii.get(self, "vpc"))
+        return typing.cast(aws_cdk.aws_ec2.IVpc, jsii.get(self, "vpc"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="vpcLinkId")
     def vpc_link_id(self) -> builtins.str:
         '''(experimental) Physical ID of the VpcLink resource.
 
         :stability: experimental
         :attribute: true
         '''
@@ -4458,15 +4275,15 @@
     :stability: experimental
     '''
 
     pass
 
 
 class _IWebSocketApiProxy(
-    jsii.proxy_for(IApi), # type: ignore[misc]
+    jsii.proxy_for(IApi) # type: ignore[misc]
 ):
     '''(experimental) Represents a WebSocket API.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IWebSocketApi"
@@ -4483,15 +4300,15 @@
     :stability: experimental
     '''
 
     pass
 
 
 class _IWebSocketAuthorizerProxy(
-    jsii.proxy_for(IAuthorizer), # type: ignore[misc]
+    jsii.proxy_for(IAuthorizer) # type: ignore[misc]
 ):
     '''(experimental) An authorizer for WebSocket APIs.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IWebSocketAuthorizer"
@@ -4504,35 +4321,35 @@
 @jsii.interface(jsii_type="@aws-cdk/aws-apigatewayv2-alpha.IWebSocketIntegration")
 class IWebSocketIntegration(IIntegration, typing_extensions.Protocol):
     '''(experimental) Represents an Integration for an WebSocket API.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="webSocketApi")
     def web_socket_api(self) -> IWebSocketApi:
         '''(experimental) The WebSocket API associated with this integration.
 
         :stability: experimental
         '''
         ...
 
 
 class _IWebSocketIntegrationProxy(
-    jsii.proxy_for(IIntegration), # type: ignore[misc]
+    jsii.proxy_for(IIntegration) # type: ignore[misc]
 ):
     '''(experimental) Represents an Integration for an WebSocket API.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IWebSocketIntegration"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="webSocketApi")
     def web_socket_api(self) -> IWebSocketApi:
         '''(experimental) The WebSocket API associated with this integration.
 
         :stability: experimental
         '''
         return typing.cast(IWebSocketApi, jsii.get(self, "webSocketApi"))
@@ -4544,55 +4361,55 @@
 @jsii.interface(jsii_type="@aws-cdk/aws-apigatewayv2-alpha.IWebSocketRoute")
 class IWebSocketRoute(IRoute, typing_extensions.Protocol):
     '''(experimental) Represents a Route for an WebSocket API.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="routeKey")
     def route_key(self) -> builtins.str:
         '''(experimental) The key to this route.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="webSocketApi")
     def web_socket_api(self) -> IWebSocketApi:
         '''(experimental) The WebSocket API associated with this route.
 
         :stability: experimental
         '''
         ...
 
 
 class _IWebSocketRouteProxy(
-    jsii.proxy_for(IRoute), # type: ignore[misc]
+    jsii.proxy_for(IRoute) # type: ignore[misc]
 ):
     '''(experimental) Represents a Route for an WebSocket API.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IWebSocketRoute"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="routeKey")
     def route_key(self) -> builtins.str:
         '''(experimental) The key to this route.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "routeKey"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="webSocketApi")
     def web_socket_api(self) -> IWebSocketApi:
         '''(experimental) The WebSocket API associated with this route.
 
         :stability: experimental
         '''
         return typing.cast(IWebSocketApi, jsii.get(self, "webSocketApi"))
@@ -4609,15 +4426,15 @@
     '''
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
         *,
         route: IWebSocketRoute,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
     ) -> "WebSocketRouteAuthorizerConfig":
         '''(experimental) Bind this authorizer to a specified WebSocket route.
 
         :param route: (experimental) The route to which the authorizer is being bound.
         :param scope: (experimental) The scope for any constructs created as part of the bind.
 
         :stability: experimental
@@ -4634,15 +4451,15 @@
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IWebSocketRouteAuthorizer"
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
         *,
         route: IWebSocketRoute,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
     ) -> "WebSocketRouteAuthorizerConfig":
         '''(experimental) Bind this authorizer to a specified WebSocket route.
 
         :param route: (experimental) The route to which the authorizer is being bound.
         :param scope: (experimental) The scope for any constructs created as part of the bind.
 
         :stability: experimental
@@ -4658,57 +4475,57 @@
 @jsii.interface(jsii_type="@aws-cdk/aws-apigatewayv2-alpha.IWebSocketStage")
 class IWebSocketStage(IStage, typing_extensions.Protocol):
     '''(experimental) Represents the WebSocketStage.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="api")
     def api(self) -> IWebSocketApi:
         '''(experimental) The API this stage is associated to.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="callbackUrl")
     def callback_url(self) -> builtins.str:
         '''(experimental) The callback URL to this stage.
 
         You can use the callback URL to send messages to the client from the backend system.
         https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-basic-concept.html
         https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-how-to-call-websocket-api-connections.html
 
         :stability: experimental
         '''
         ...
 
 
 class _IWebSocketStageProxy(
-    jsii.proxy_for(IStage), # type: ignore[misc]
+    jsii.proxy_for(IStage) # type: ignore[misc]
 ):
     '''(experimental) Represents the WebSocketStage.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IWebSocketStage"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="api")
     def api(self) -> IWebSocketApi:
         '''(experimental) The API this stage is associated to.
 
         :stability: experimental
         '''
         return typing.cast(IWebSocketApi, jsii.get(self, "api"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="callbackUrl")
     def callback_url(self) -> builtins.str:
         '''(experimental) The callback URL to this stage.
 
         You can use the callback URL to send messages to the client from the backend system.
         https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-basic-concept.html
         https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-how-to-call-websocket-api-connections.html
@@ -4744,53 +4561,47 @@
 
     def __init__(self) -> None:
         '''
         :stability: experimental
         '''
         jsii.create(self.__class__, self, [])
 
-    @jsii.member(jsii_name="fromRole")
+    @jsii.member(jsii_name="fromRole") # type: ignore[misc]
     @builtins.classmethod
-    def from_role(
-        cls,
-        role: _aws_cdk_aws_iam_ceddda9d.IRole,
-    ) -> "IntegrationCredentials":
+    def from_role(cls, role: aws_cdk.aws_iam.IRole) -> "IntegrationCredentials":
         '''(experimental) Use the specified role for integration requests.
 
         :param role: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__102c1a776427fd4c0938e5abf575144e45fdb236c63258f1da261499f33717f0)
-            check_type(argname="argument role", value=role, expected_type=type_hints["role"])
         return typing.cast("IntegrationCredentials", jsii.sinvoke(cls, "fromRole", [role]))
 
-    @jsii.member(jsii_name="useCallerIdentity")
+    @jsii.member(jsii_name="useCallerIdentity") # type: ignore[misc]
     @builtins.classmethod
     def use_caller_identity(cls) -> "IntegrationCredentials":
         '''(experimental) Use the calling user's identity to call the integration.
 
         :stability: experimental
         '''
         return typing.cast("IntegrationCredentials", jsii.sinvoke(cls, "useCallerIdentity", []))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="credentialsArn")
     @abc.abstractmethod
     def credentials_arn(self) -> builtins.str:
         '''(experimental) The ARN of the credentials.
 
         :stability: experimental
         '''
         ...
 
 
 class _IntegrationCredentialsProxy(IntegrationCredentials):
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="credentialsArn")
     def credentials_arn(self) -> builtins.str:
         '''(experimental) The ARN of the credentials.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "credentialsArn"))
@@ -4804,68 +4615,60 @@
     jsii_struct_bases=[],
     name_mapping={"bucket": "bucket", "key": "key", "version": "version"},
 )
 class MTLSConfig:
     def __init__(
         self,
         *,
-        bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        bucket: aws_cdk.aws_s3.IBucket,
         key: builtins.str,
         version: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) The mTLS authentication configuration for a custom domain name.
 
         :param bucket: (experimental) The bucket that the trust store is hosted in.
         :param key: (experimental) The key in S3 to look at for the trust store.
         :param version: (experimental) The version of the S3 object that contains your truststore. To specify a version, you must have versioning enabled for the S3 bucket. Default: - latest version
 
         :stability: experimental
-        :exampleMetadata: infused
+        :exampleMetadata: fixture=_generated
 
         Example::
 
-            import aws_cdk.aws_s3 as s3
-            import aws_cdk.aws_certificatemanager as acm
-            # bucket: s3.Bucket
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.aws_apigatewayv2_alpha as apigatewayv2_alpha
+            from aws_cdk import aws_s3 as s3
             
+            # bucket: s3.Bucket
             
-            cert_arn = "arn:aws:acm:us-east-1:111111111111:certificate"
-            domain_name = "example.com"
+            m_tLSConfig = apigatewayv2_alpha.MTLSConfig(
+                bucket=bucket,
+                key="key",
             
-            apigwv2.DomainName(self, "DomainName",
-                domain_name=domain_name,
-                certificate=acm.Certificate.from_certificate_arn(self, "cert", cert_arn),
-                mtls=apigwv2.MTLSConfig(
-                    bucket=bucket,
-                    key="someca.pem",
-                    version="version"
-                )
+                # the properties below are optional
+                version="version"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__38e19f865daecac4e9c0b7840b549ee7e3e17328107146b6aeed11be416a4830)
-            check_type(argname="argument bucket", value=bucket, expected_type=type_hints["bucket"])
-            check_type(argname="argument key", value=key, expected_type=type_hints["key"])
-            check_type(argname="argument version", value=version, expected_type=type_hints["version"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "bucket": bucket,
             "key": key,
         }
         if version is not None:
             self._values["version"] = version
 
     @builtins.property
-    def bucket(self) -> _aws_cdk_aws_s3_ceddda9d.IBucket:
+    def bucket(self) -> aws_cdk.aws_s3.IBucket:
         '''(experimental) The bucket that the trust store is hosted in.
 
         :stability: experimental
         '''
         result = self._values.get("bucket")
         assert result is not None, "Required property 'bucket' is missing"
-        return typing.cast(_aws_cdk_aws_s3_ceddda9d.IBucket, result)
+        return typing.cast(aws_cdk.aws_s3.IBucket, result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''(experimental) The key in S3 to look at for the trust store.
 
         :stability: experimental
         '''
@@ -4924,140 +4727,116 @@
                 parameter_mapping=apigwv2.ParameterMapping().append_header("header2", apigwv2.MappingValue.request_header("header1")).remove_header("header1")
             )
         )
     '''
 
     def __init__(self, value: builtins.str) -> None:
         '''
-        :param value: Represents a Mapping Value.
+        :param value: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__214070b3203c10af4bde0b28ed256ac9a4d24597f026dd0b0cc830dd88c3212d)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.create(self.__class__, self, [value])
 
-    @jsii.member(jsii_name="contextVariable")
+    @jsii.member(jsii_name="contextVariable") # type: ignore[misc]
     @builtins.classmethod
     def context_variable(cls, variable_name: builtins.str) -> "MappingValue":
         '''(experimental) Creates a context variable mapping value.
 
         :param variable_name: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4af933305aeacd390d336f32a5829afa054de657121385d6ec7753a9ea26d601)
-            check_type(argname="argument variable_name", value=variable_name, expected_type=type_hints["variable_name"])
         return typing.cast("MappingValue", jsii.sinvoke(cls, "contextVariable", [variable_name]))
 
-    @jsii.member(jsii_name="custom")
+    @jsii.member(jsii_name="custom") # type: ignore[misc]
     @builtins.classmethod
     def custom(cls, value: builtins.str) -> "MappingValue":
         '''(experimental) Creates a custom mapping value.
 
         :param value: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4ea57d3eb4bcfb04e995828dff02ab6f0787305f407450d33b5272726fe121ba)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast("MappingValue", jsii.sinvoke(cls, "custom", [value]))
 
-    @jsii.member(jsii_name="requestBody")
+    @jsii.member(jsii_name="requestBody") # type: ignore[misc]
     @builtins.classmethod
     def request_body(cls, name: builtins.str) -> "MappingValue":
         '''(experimental) Creates a request body mapping value.
 
         :param name: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fd491365abe2954925b1f433ba7521a56e4bbc0bcdfddd61b667ca4f13903681)
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         return typing.cast("MappingValue", jsii.sinvoke(cls, "requestBody", [name]))
 
-    @jsii.member(jsii_name="requestHeader")
+    @jsii.member(jsii_name="requestHeader") # type: ignore[misc]
     @builtins.classmethod
     def request_header(cls, name: builtins.str) -> "MappingValue":
         '''(experimental) Creates a header mapping value.
 
         :param name: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e720451078130f0098a0b48416451612a00e6befa0c802ff75a2b864085649a5)
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         return typing.cast("MappingValue", jsii.sinvoke(cls, "requestHeader", [name]))
 
-    @jsii.member(jsii_name="requestPath")
+    @jsii.member(jsii_name="requestPath") # type: ignore[misc]
     @builtins.classmethod
     def request_path(cls) -> "MappingValue":
         '''(experimental) Creates a request path mapping value.
 
         :stability: experimental
         '''
         return typing.cast("MappingValue", jsii.sinvoke(cls, "requestPath", []))
 
-    @jsii.member(jsii_name="requestPathParam")
+    @jsii.member(jsii_name="requestPathParam") # type: ignore[misc]
     @builtins.classmethod
     def request_path_param(cls, name: builtins.str) -> "MappingValue":
         '''(experimental) Creates a request path parameter mapping value.
 
         :param name: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__69c384039069eb05e230de4bc9ac53925e0d361bd038ed0a3b02e073b1525c71)
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         return typing.cast("MappingValue", jsii.sinvoke(cls, "requestPathParam", [name]))
 
-    @jsii.member(jsii_name="requestQueryString")
+    @jsii.member(jsii_name="requestQueryString") # type: ignore[misc]
     @builtins.classmethod
     def request_query_string(cls, name: builtins.str) -> "MappingValue":
         '''(experimental) Creates a query string mapping value.
 
         :param name: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b36b16773b8a1c554f9a57b9e3d7a3722f155a3d65b1a10b4204ac3f1740616a)
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         return typing.cast("MappingValue", jsii.sinvoke(cls, "requestQueryString", [name]))
 
-    @jsii.member(jsii_name="stageVariable")
+    @jsii.member(jsii_name="stageVariable") # type: ignore[misc]
     @builtins.classmethod
     def stage_variable(cls, variable_name: builtins.str) -> "MappingValue":
         '''(experimental) Creates a stage variable mapping value.
 
         :param variable_name: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b3602fe53f550a6f339115089310b50937eb494d182495b9b3787a639c5dcaed)
-            check_type(argname="argument variable_name", value=variable_name, expected_type=type_hints["variable_name"])
         return typing.cast("MappingValue", jsii.sinvoke(cls, "stageVariable", [variable_name]))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="NONE")
     def NONE(cls) -> "MappingValue":
         '''(experimental) Creates an empty mapping value.
 
         :stability: experimental
         '''
         return typing.cast("MappingValue", jsii.sget(cls, "NONE"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="value")
     def value(self) -> builtins.str:
         '''(experimental) Represents a Mapping Value.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "value"))
@@ -5092,29 +4871,26 @@
 
     def __init__(self) -> None:
         '''
         :stability: experimental
         '''
         jsii.create(self.__class__, self, [])
 
-    @jsii.member(jsii_name="fromObject")
+    @jsii.member(jsii_name="fromObject") # type: ignore[misc]
     @builtins.classmethod
     def from_object(
         cls,
         obj: typing.Mapping[builtins.str, MappingValue],
     ) -> "ParameterMapping":
         '''(experimental) Creates a mapping from an object.
 
         :param obj: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c8181ef9cc8308f9477f0a1caad591787ed40d80e9353a4ab806411f93450058)
-            check_type(argname="argument obj", value=obj, expected_type=type_hints["obj"])
         return typing.cast("ParameterMapping", jsii.sinvoke(cls, "fromObject", [obj]))
 
     @jsii.member(jsii_name="appendHeader")
     def append_header(
         self,
         name: builtins.str,
         value: MappingValue,
@@ -5122,18 +4898,14 @@
         '''(experimental) Creates a mapping to append a header.
 
         :param name: -
         :param value: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__56ae57cc9968fa2fd30ad1d66784260b0e784ac1e0ae80923fa737f9a8ada22a)
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast("ParameterMapping", jsii.invoke(self, "appendHeader", [name, value]))
 
     @jsii.member(jsii_name="appendQueryString")
     def append_query_string(
         self,
         name: builtins.str,
         value: MappingValue,
@@ -5141,33 +4913,25 @@
         '''(experimental) Creates a mapping to append a query string.
 
         :param name: -
         :param value: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4f855f9472042f201eb931ccc90ac6f72c3684fdf5485ee6979662f843ed27cc)
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast("ParameterMapping", jsii.invoke(self, "appendQueryString", [name, value]))
 
     @jsii.member(jsii_name="custom")
     def custom(self, key: builtins.str, value: builtins.str) -> "ParameterMapping":
         '''(experimental) Creates a custom mapping.
 
         :param key: -
         :param value: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ea27856048c8e84cddc832b14d9115403f2b80ce39008d1d2a456c126be689c6)
-            check_type(argname="argument key", value=key, expected_type=type_hints["key"])
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast("ParameterMapping", jsii.invoke(self, "custom", [key, value]))
 
     @jsii.member(jsii_name="overwriteHeader")
     def overwrite_header(
         self,
         name: builtins.str,
         value: MappingValue,
@@ -5175,31 +4939,24 @@
         '''(experimental) Creates a mapping to overwrite a header.
 
         :param name: -
         :param value: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0bbf5124407bf24ea9fa7d17aa1565a5ed9210655f4f602da854ad14a24db0d5)
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast("ParameterMapping", jsii.invoke(self, "overwriteHeader", [name, value]))
 
     @jsii.member(jsii_name="overwritePath")
     def overwrite_path(self, value: MappingValue) -> "ParameterMapping":
         '''(experimental) Creates a mapping to overwrite a path.
 
         :param value: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3969677f031f21644ed17215886d65e2445e67dcf22241b2a6150248c6192f36)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast("ParameterMapping", jsii.invoke(self, "overwritePath", [value]))
 
     @jsii.member(jsii_name="overwriteQueryString")
     def overwrite_query_string(
         self,
         name: builtins.str,
         value: MappingValue,
@@ -5207,47 +4964,37 @@
         '''(experimental) Creates a mapping to overwrite a querystring.
 
         :param name: -
         :param value: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e75c515536f95796a2a8f985b00f7829f0664a04b9a30bed03ea9ad1ce892d91)
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast("ParameterMapping", jsii.invoke(self, "overwriteQueryString", [name, value]))
 
     @jsii.member(jsii_name="removeHeader")
     def remove_header(self, name: builtins.str) -> "ParameterMapping":
         '''(experimental) Creates a mapping to remove a header.
 
         :param name: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__48411845428e2e72182038805ca1f55aa523a254158b3148ec49d4ee874decc5)
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         return typing.cast("ParameterMapping", jsii.invoke(self, "removeHeader", [name]))
 
     @jsii.member(jsii_name="removeQueryString")
     def remove_query_string(self, name: builtins.str) -> "ParameterMapping":
         '''(experimental) Creates a mapping to remove a querystring.
 
         :param name: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__46e584a752980831919a8156516ab93f44fb1a783b5798270ff450fdc6bc50d2)
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         return typing.cast("ParameterMapping", jsii.invoke(self, "removeQueryString", [name]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="mappings")
     def mappings(self) -> typing.Mapping[builtins.str, builtins.str]:
         '''(experimental) Represents all created parameter mappings.
 
         :stability: experimental
         '''
         return typing.cast(typing.Mapping[builtins.str, builtins.str], jsii.get(self, "mappings"))
@@ -5268,49 +5015,46 @@
         # The code below shows an example of how to instantiate this type.
         # The values are placeholders you should change.
         import aws_cdk.aws_apigatewayv2_alpha as apigatewayv2_alpha
         
         payload_format_version = apigatewayv2_alpha.PayloadFormatVersion.custom("version")
     '''
 
-    @jsii.member(jsii_name="custom")
+    @jsii.member(jsii_name="custom") # type: ignore[misc]
     @builtins.classmethod
     def custom(cls, version: builtins.str) -> "PayloadFormatVersion":
         '''(experimental) A custom payload version.
 
         Typically used if there is a version number that the CDK doesn't support yet
 
         :param version: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__650e7e8cf5095b5caf036d1cdfea61cdc50d05db4e0b82311e5988ab562c7508)
-            check_type(argname="argument version", value=version, expected_type=type_hints["version"])
         return typing.cast("PayloadFormatVersion", jsii.sinvoke(cls, "custom", [version]))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="VERSION_1_0")
     def VERSION_1_0(cls) -> "PayloadFormatVersion":
         '''(experimental) Version 1.0.
 
         :stability: experimental
         '''
         return typing.cast("PayloadFormatVersion", jsii.sget(cls, "VERSION_1_0"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="VERSION_2_0")
     def VERSION_2_0(cls) -> "PayloadFormatVersion":
         '''(experimental) Version 2.0.
 
         :stability: experimental
         '''
         return typing.cast("PayloadFormatVersion", jsii.sget(cls, "VERSION_2_0"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="version")
     def version(self) -> builtins.str:
         '''(experimental) version as a string.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "version"))
@@ -5355,18 +5099,15 @@
             # The values are placeholders you should change.
             import aws_cdk.aws_apigatewayv2_alpha as apigatewayv2_alpha
             
             stage_attributes = apigatewayv2_alpha.StageAttributes(
                 stage_name="stageName"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b7bc86d60b044b6ce8b75e1e701218c18bc2ca9ef7cc2a9667e4858066891f46)
-            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "stage_name": stage_name,
         }
 
     @builtins.property
     def stage_name(self) -> builtins.str:
         '''(experimental) The name of the stage.
 
@@ -5387,35 +5128,29 @@
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.StageOptions",
     jsii_struct_bases=[],
-    name_mapping={
-        "auto_deploy": "autoDeploy",
-        "domain_mapping": "domainMapping",
-        "throttle": "throttle",
-    },
+    name_mapping={"auto_deploy": "autoDeploy", "domain_mapping": "domainMapping"},
 )
 class StageOptions:
     def __init__(
         self,
         *,
         auto_deploy: typing.Optional[builtins.bool] = None,
-        domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-        throttle: typing.Optional[typing.Union["ThrottleSettings", typing.Dict[builtins.str, typing.Any]]] = None,
+        domain_mapping: typing.Optional[DomainMappingOptions] = None,
     ) -> None:
         '''(experimental) Options required to create a new stage.
 
         Options that are common between HTTP and Websocket APIs.
 
         :param auto_deploy: (experimental) Whether updates to an API automatically trigger a new deployment. Default: false
         :param domain_mapping: (experimental) The options for custom domain and api mapping. Default: - no custom domain and api mapping configuration
-        :param throttle: (experimental) Throttle settings for the routes of this stage. Default: - no throttling configuration
 
         :stability: experimental
         :exampleMetadata: fixture=_generated
 
         Example::
 
             # The code below shows an example of how to instantiate this type.
@@ -5427,37 +5162,24 @@
             stage_options = apigatewayv2_alpha.StageOptions(
                 auto_deploy=False,
                 domain_mapping=apigatewayv2_alpha.DomainMappingOptions(
                     domain_name=domain_name,
             
                     # the properties below are optional
                     mapping_key="mappingKey"
-                ),
-                throttle=apigatewayv2_alpha.ThrottleSettings(
-                    burst_limit=123,
-                    rate_limit=123
                 )
             )
         '''
         if isinstance(domain_mapping, dict):
             domain_mapping = DomainMappingOptions(**domain_mapping)
-        if isinstance(throttle, dict):
-            throttle = ThrottleSettings(**throttle)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a32c0806cbd09e57e1b6cb67e4b59ac7fdd424ef31f824f2caeda822945dbf65)
-            check_type(argname="argument auto_deploy", value=auto_deploy, expected_type=type_hints["auto_deploy"])
-            check_type(argname="argument domain_mapping", value=domain_mapping, expected_type=type_hints["domain_mapping"])
-            check_type(argname="argument throttle", value=throttle, expected_type=type_hints["throttle"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if auto_deploy is not None:
             self._values["auto_deploy"] = auto_deploy
         if domain_mapping is not None:
             self._values["domain_mapping"] = domain_mapping
-        if throttle is not None:
-            self._values["throttle"] = throttle
 
     @builtins.property
     def auto_deploy(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Whether updates to an API automatically trigger a new deployment.
 
         :default: false
 
@@ -5473,115 +5195,29 @@
         :default: - no custom domain and api mapping configuration
 
         :stability: experimental
         '''
         result = self._values.get("domain_mapping")
         return typing.cast(typing.Optional[DomainMappingOptions], result)
 
-    @builtins.property
-    def throttle(self) -> typing.Optional["ThrottleSettings"]:
-        '''(experimental) Throttle settings for the routes of this stage.
-
-        :default: - no throttling configuration
-
-        :stability: experimental
-        '''
-        result = self._values.get("throttle")
-        return typing.cast(typing.Optional["ThrottleSettings"], result)
-
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
         return "StageOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-@jsii.data_type(
-    jsii_type="@aws-cdk/aws-apigatewayv2-alpha.ThrottleSettings",
-    jsii_struct_bases=[],
-    name_mapping={"burst_limit": "burstLimit", "rate_limit": "rateLimit"},
-)
-class ThrottleSettings:
-    def __init__(
-        self,
-        *,
-        burst_limit: typing.Optional[jsii.Number] = None,
-        rate_limit: typing.Optional[jsii.Number] = None,
-    ) -> None:
-        '''(experimental) Container for defining throttling parameters to API stages.
-
-        :param burst_limit: (experimental) The maximum API request rate limit over a time ranging from one to a few seconds. Default: none
-        :param rate_limit: (experimental) The API request steady-state rate limit (average requests per second over an extended period of time). Default: none
-
-        :stability: experimental
-        :exampleMetadata: fixture=_generated
-
-        Example::
-
-            # The code below shows an example of how to instantiate this type.
-            # The values are placeholders you should change.
-            import aws_cdk.aws_apigatewayv2_alpha as apigatewayv2_alpha
-            
-            throttle_settings = apigatewayv2_alpha.ThrottleSettings(
-                burst_limit=123,
-                rate_limit=123
-            )
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4ad556ef4d84d522901264cb64a96b656171558870186a72f596567dc19746a2)
-            check_type(argname="argument burst_limit", value=burst_limit, expected_type=type_hints["burst_limit"])
-            check_type(argname="argument rate_limit", value=rate_limit, expected_type=type_hints["rate_limit"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
-        if burst_limit is not None:
-            self._values["burst_limit"] = burst_limit
-        if rate_limit is not None:
-            self._values["rate_limit"] = rate_limit
-
-    @builtins.property
-    def burst_limit(self) -> typing.Optional[jsii.Number]:
-        '''(experimental) The maximum API request rate limit over a time ranging from one to a few seconds.
-
-        :default: none
-
-        :stability: experimental
-        '''
-        result = self._values.get("burst_limit")
-        return typing.cast(typing.Optional[jsii.Number], result)
-
-    @builtins.property
-    def rate_limit(self) -> typing.Optional[jsii.Number]:
-        '''(experimental) The API request steady-state rate limit (average requests per second over an extended period of time).
-
-        :default: none
-
-        :stability: experimental
-        '''
-        result = self._values.get("rate_limit")
-        return typing.cast(typing.Optional[jsii.Number], result)
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "ThrottleSettings(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
-
 @jsii.implements(IVpcLink)
 class VpcLink(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.VpcLink",
 ):
     '''(experimental) Define a new VPC Link Specifies an API Gateway VPC link for a HTTP API to access resources in an Amazon Virtual Private Cloud (VPC).
 
     :stability: experimental
     :exampleMetadata: infused
@@ -5593,111 +5229,94 @@
         
         vpc = ec2.Vpc(self, "VPC")
         vpc_link = apigwv2.VpcLink(self, "VpcLink", vpc=vpc)
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-        subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        vpc: aws_cdk.aws_ec2.IVpc,
+        security_groups: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.ISecurityGroup]] = None,
+        subnets: typing.Optional[aws_cdk.aws_ec2.SubnetSelection] = None,
         vpc_link_name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param vpc: (experimental) The VPC in which the private resources reside.
         :param security_groups: (experimental) A list of security groups for the VPC link. Default: - no security groups. Use ``addSecurityGroups`` to add security groups
         :param subnets: (experimental) A list of subnets for the VPC link. Default: - private subnets of the provided VPC. Use ``addSubnets`` to add more subnets
         :param vpc_link_name: (experimental) The name used to label and identify the VPC link. Default: - automatically generated name
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a7e5cf8ebb393b1b711349f32ce6a5d91c23aa92cb3f1a5fb324d1ace8fa39e5)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = VpcLinkProps(
             vpc=vpc,
             security_groups=security_groups,
             subnets=subnets,
             vpc_link_name=vpc_link_name,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromVpcLinkAttributes")
+    @jsii.member(jsii_name="fromVpcLinkAttributes") # type: ignore[misc]
     @builtins.classmethod
     def from_vpc_link_attributes(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
+        vpc: aws_cdk.aws_ec2.IVpc,
         vpc_link_id: builtins.str,
     ) -> IVpcLink:
         '''(experimental) Import a VPC Link by specifying its attributes.
 
         :param scope: -
         :param id: -
         :param vpc: (experimental) The VPC to which this VPC link is associated with.
         :param vpc_link_id: (experimental) The VPC Link id.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d1b73cd3902808dcd9cedbbb002791b3c0b71ecf07dc9ee537153e45a37de0b7)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         attrs = VpcLinkAttributes(vpc=vpc, vpc_link_id=vpc_link_id)
 
         return typing.cast(IVpcLink, jsii.sinvoke(cls, "fromVpcLinkAttributes", [scope, id, attrs]))
 
     @jsii.member(jsii_name="addSecurityGroups")
-    def add_security_groups(
-        self,
-        *groups: _aws_cdk_aws_ec2_ceddda9d.ISecurityGroup,
-    ) -> None:
+    def add_security_groups(self, *groups: aws_cdk.aws_ec2.ISecurityGroup) -> None:
         '''(experimental) Adds the provided security groups to the vpc link.
 
         :param groups: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fb1536c4a56444b87ed12cf12ec84dcad1aeea01af7e687ab6bc5440355e7e11)
-            check_type(argname="argument groups", value=groups, expected_type=typing.Tuple[type_hints["groups"], ...]) # pyright: ignore [reportGeneralTypeIssues]
         return typing.cast(None, jsii.invoke(self, "addSecurityGroups", [*groups]))
 
     @jsii.member(jsii_name="addSubnets")
-    def add_subnets(self, *subnets: _aws_cdk_aws_ec2_ceddda9d.ISubnet) -> None:
+    def add_subnets(self, *subnets: aws_cdk.aws_ec2.ISubnet) -> None:
         '''(experimental) Adds the provided subnets to the vpc link.
 
         :param subnets: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0b26d604e4ca1a2688579e0987cdb68ab389de0e4b8cb68e274ece105bdd03cf)
-            check_type(argname="argument subnets", value=subnets, expected_type=typing.Tuple[type_hints["subnets"], ...]) # pyright: ignore [reportGeneralTypeIssues]
         return typing.cast(None, jsii.invoke(self, "addSubnets", [*subnets]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="vpc")
-    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
+    def vpc(self) -> aws_cdk.aws_ec2.IVpc:
         '''(experimental) The VPC to which this VPC Link is associated with.
 
         :stability: experimental
         '''
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, jsii.get(self, "vpc"))
+        return typing.cast(aws_cdk.aws_ec2.IVpc, jsii.get(self, "vpc"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="vpcLinkId")
     def vpc_link_id(self) -> builtins.str:
         '''(experimental) Physical ID of the VpcLink resource.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "vpcLinkId"))
@@ -5705,20 +5324,15 @@
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.VpcLinkAttributes",
     jsii_struct_bases=[],
     name_mapping={"vpc": "vpc", "vpc_link_id": "vpcLinkId"},
 )
 class VpcLinkAttributes:
-    def __init__(
-        self,
-        *,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-        vpc_link_id: builtins.str,
-    ) -> None:
+    def __init__(self, *, vpc: aws_cdk.aws_ec2.IVpc, vpc_link_id: builtins.str) -> None:
         '''(experimental) Attributes when importing a new VpcLink.
 
         :param vpc: (experimental) The VPC to which this VPC link is associated with.
         :param vpc_link_id: (experimental) The VPC Link id.
 
         :stability: experimental
         :exampleMetadata: infused
@@ -5730,32 +5344,28 @@
             # vpc: ec2.Vpc
             
             awesome_link = apigwv2.VpcLink.from_vpc_link_attributes(self, "awesome-vpc-link",
                 vpc_link_id="us-east-1_oiuR12Abd",
                 vpc=vpc
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b806190a5cb732ad4de67d21bd895caa64bb12248a0d0ab31634597e02c8057e)
-            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
-            check_type(argname="argument vpc_link_id", value=vpc_link_id, expected_type=type_hints["vpc_link_id"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "vpc": vpc,
             "vpc_link_id": vpc_link_id,
         }
 
     @builtins.property
-    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
+    def vpc(self) -> aws_cdk.aws_ec2.IVpc:
         '''(experimental) The VPC to which this VPC link is associated with.
 
         :stability: experimental
         '''
         result = self._values.get("vpc")
         assert result is not None, "Required property 'vpc' is missing"
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, result)
+        return typing.cast(aws_cdk.aws_ec2.IVpc, result)
 
     @builtins.property
     def vpc_link_id(self) -> builtins.str:
         '''(experimental) The VPC Link id.
 
         :stability: experimental
         '''
@@ -5785,17 +5395,17 @@
         "vpc_link_name": "vpcLinkName",
     },
 )
 class VpcLinkProps:
     def __init__(
         self,
         *,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-        subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        vpc: aws_cdk.aws_ec2.IVpc,
+        security_groups: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.ISecurityGroup]] = None,
+        subnets: typing.Optional[aws_cdk.aws_ec2.SubnetSelection] = None,
         vpc_link_name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Properties for a VpcLink.
 
         :param vpc: (experimental) The VPC in which the private resources reside.
         :param security_groups: (experimental) A list of security groups for the VPC link. Default: - no security groups. Use ``addSecurityGroups`` to add security groups
         :param subnets: (experimental) A list of subnets for the VPC link. Default: - private subnets of the provided VPC. Use ``addSubnets`` to add more subnets
@@ -5809,64 +5419,58 @@
             import aws_cdk.aws_ec2 as ec2
             
             
             vpc = ec2.Vpc(self, "VPC")
             vpc_link = apigwv2.VpcLink(self, "VpcLink", vpc=vpc)
         '''
         if isinstance(subnets, dict):
-            subnets = _aws_cdk_aws_ec2_ceddda9d.SubnetSelection(**subnets)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9aed9118f19188de6967aa0373708cfcd4ffb3d828b567d6cbc01404c7aa6581)
-            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
-            check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
-            check_type(argname="argument subnets", value=subnets, expected_type=type_hints["subnets"])
-            check_type(argname="argument vpc_link_name", value=vpc_link_name, expected_type=type_hints["vpc_link_name"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+            subnets = aws_cdk.aws_ec2.SubnetSelection(**subnets)
+        self._values: typing.Dict[str, typing.Any] = {
             "vpc": vpc,
         }
         if security_groups is not None:
             self._values["security_groups"] = security_groups
         if subnets is not None:
             self._values["subnets"] = subnets
         if vpc_link_name is not None:
             self._values["vpc_link_name"] = vpc_link_name
 
     @builtins.property
-    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
+    def vpc(self) -> aws_cdk.aws_ec2.IVpc:
         '''(experimental) The VPC in which the private resources reside.
 
         :stability: experimental
         '''
         result = self._values.get("vpc")
         assert result is not None, "Required property 'vpc' is missing"
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, result)
+        return typing.cast(aws_cdk.aws_ec2.IVpc, result)
 
     @builtins.property
     def security_groups(
         self,
-    ) -> typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]]:
+    ) -> typing.Optional[typing.List[aws_cdk.aws_ec2.ISecurityGroup]]:
         '''(experimental) A list of security groups for the VPC link.
 
         :default: - no security groups. Use ``addSecurityGroups`` to add security groups
 
         :stability: experimental
         '''
         result = self._values.get("security_groups")
-        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]], result)
+        return typing.cast(typing.Optional[typing.List[aws_cdk.aws_ec2.ISecurityGroup]], result)
 
     @builtins.property
-    def subnets(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection]:
+    def subnets(self) -> typing.Optional[aws_cdk.aws_ec2.SubnetSelection]:
         '''(experimental) A list of subnets for the VPC link.
 
         :default: - private subnets of the provided VPC. Use ``addSubnets`` to add more subnets
 
         :stability: experimental
         '''
         result = self._values.get("subnets")
-        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_ec2.SubnetSelection], result)
 
     @builtins.property
     def vpc_link_name(self) -> typing.Optional[builtins.str]:
         '''(experimental) The name used to label and identify the VPC link.
 
         :default: - automatically generated name
 
@@ -5885,23 +5489,23 @@
         return "VpcLinkProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.implements(IWebSocketApi, IApi)
 class WebSocketApi(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.WebSocketApi",
 ):
     '''(experimental) Create a new API Gateway WebSocket API endpoint.
 
     :stability: experimental
-    :resource: AWS::ApiGatewayV2::Api
     :exampleMetadata: infused
+    :resource: AWS::ApiGatewayV2::Api
 
     Example::
 
         from aws_cdk.aws_apigatewayv2_integrations_alpha import WebSocketLambdaIntegration
         
         # message_handler: lambda.Function
         
@@ -5915,23 +5519,23 @@
         web_socket_api.add_route("sendmessage",
             integration=WebSocketLambdaIntegration("SendMessageIntegration", message_handler)
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         api_key_selection_expression: typing.Optional["WebSocketApiKeySelectionExpression"] = None,
         api_name: typing.Optional[builtins.str] = None,
-        connect_route_options: typing.Optional[typing.Union["WebSocketRouteOptions", typing.Dict[builtins.str, typing.Any]]] = None,
-        default_route_options: typing.Optional[typing.Union["WebSocketRouteOptions", typing.Dict[builtins.str, typing.Any]]] = None,
+        connect_route_options: typing.Optional["WebSocketRouteOptions"] = None,
+        default_route_options: typing.Optional["WebSocketRouteOptions"] = None,
         description: typing.Optional[builtins.str] = None,
-        disconnect_route_options: typing.Optional[typing.Union["WebSocketRouteOptions", typing.Dict[builtins.str, typing.Any]]] = None,
+        disconnect_route_options: typing.Optional["WebSocketRouteOptions"] = None,
         route_selection_expression: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param api_key_selection_expression: (experimental) An API key selection expression. Providing this option will require an API Key be provided to access the API. Default: - Key is not required to access these APIs
         :param api_name: (experimental) Name for the WebSocket API resource. Default: - id of the WebSocketApi construct.
@@ -5939,293 +5543,177 @@
         :param default_route_options: (experimental) Options to configure a '$default' route. Default: - no '$default' route configured
         :param description: (experimental) The description of the API. Default: - none
         :param disconnect_route_options: (experimental) Options to configure a '$disconnect' route. Default: - no '$disconnect' route configured
         :param route_selection_expression: (experimental) The route selection expression for the API. Default: '$request.body.action'
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1178cce7f52c6ba72b835087f977643630d7f0c2665b967ecfee0bfe59093cb6)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = WebSocketApiProps(
             api_key_selection_expression=api_key_selection_expression,
             api_name=api_name,
             connect_route_options=connect_route_options,
             default_route_options=default_route_options,
             description=description,
             disconnect_route_options=disconnect_route_options,
             route_selection_expression=route_selection_expression,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromWebSocketApiAttributes")
-    @builtins.classmethod
-    def from_web_socket_api_attributes(
-        cls,
-        scope: _constructs_77d1e7e8.Construct,
-        id: builtins.str,
-        *,
-        web_socket_id: builtins.str,
-        api_endpoint: typing.Optional[builtins.str] = None,
-    ) -> IWebSocketApi:
-        '''(experimental) Import an existing WebSocket API into this CDK app.
-
-        :param scope: -
-        :param id: -
-        :param web_socket_id: (experimental) The identifier of the WebSocketApi.
-        :param api_endpoint: (experimental) The endpoint URL of the WebSocketApi. Default: - throw san error if apiEndpoint is accessed.
-
-        :stability: experimental
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__53d1a9fe1fdf41c0b5a739761d4875fb19c206a09c26c51425f989503e6b976b)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        attrs = WebSocketApiAttributes(
-            web_socket_id=web_socket_id, api_endpoint=api_endpoint
-        )
-
-        return typing.cast(IWebSocketApi, jsii.sinvoke(cls, "fromWebSocketApiAttributes", [scope, id, attrs]))
-
     @jsii.member(jsii_name="addRoute")
     def add_route(
         self,
         route_key: builtins.str,
         *,
         integration: "WebSocketRouteIntegration",
         authorizer: typing.Optional[IWebSocketRouteAuthorizer] = None,
-        return_response: typing.Optional[builtins.bool] = None,
     ) -> "WebSocketRoute":
         '''(experimental) Add a new route.
 
         :param route_key: -
         :param integration: (experimental) The integration to be configured on this route.
         :param authorizer: (experimental) The authorize to this route. You can only set authorizer to a $connect route. Default: - No Authorizer
-        :param return_response: (experimental) Should the route send a response to the client. Default: false
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b3fea69a2469b346680a0c3465ad0d8edf75af46ec799894b3faabfa5c26ec77)
-            check_type(argname="argument route_key", value=route_key, expected_type=type_hints["route_key"])
-        options = WebSocketRouteOptions(
-            integration=integration,
-            authorizer=authorizer,
-            return_response=return_response,
-        )
+        options = WebSocketRouteOptions(integration=integration, authorizer=authorizer)
 
         return typing.cast("WebSocketRoute", jsii.invoke(self, "addRoute", [route_key, options]))
 
     @jsii.member(jsii_name="grantManageConnections")
     def grant_manage_connections(
         self,
-        identity: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-    ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
+        identity: aws_cdk.aws_iam.IGrantable,
+    ) -> aws_cdk.aws_iam.Grant:
         '''(experimental) Grant access to the API Gateway management API for this WebSocket API to an IAM principal (Role/Group/User).
 
         :param identity: The principal.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3519e657dc5ef6b61e34eb3fc9f6d114f2ebbf762f5ca278412f276b78b73bd7)
-            check_type(argname="argument identity", value=identity, expected_type=type_hints["identity"])
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.Grant, jsii.invoke(self, "grantManageConnections", [identity]))
+        return typing.cast(aws_cdk.aws_iam.Grant, jsii.invoke(self, "grantManageConnections", [identity]))
 
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
         '''(experimental) Return the given named metric for this Api Gateway.
 
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
-            type_hints = typing.get_type_hints(_typecheckingstub__25c26b71a707cd073d476cfe86d40884d0adc369830b3b667bfcc8d3d5069fe3)
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
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="apiEndpoint")
     def api_endpoint(self) -> builtins.str:
         '''(experimental) The default endpoint for an API.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "apiEndpoint"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="apiId")
     def api_id(self) -> builtins.str:
         '''(experimental) The identifier of this API Gateway API.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "apiId"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="webSocketApiName")
     def web_socket_api_name(self) -> typing.Optional[builtins.str]:
         '''(experimental) A human friendly name for this WebSocket API.
 
         Note that this is different from ``webSocketApiId``.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "webSocketApiName"))
 
 
-@jsii.data_type(
-    jsii_type="@aws-cdk/aws-apigatewayv2-alpha.WebSocketApiAttributes",
-    jsii_struct_bases=[],
-    name_mapping={"web_socket_id": "webSocketId", "api_endpoint": "apiEndpoint"},
-)
-class WebSocketApiAttributes:
-    def __init__(
-        self,
-        *,
-        web_socket_id: builtins.str,
-        api_endpoint: typing.Optional[builtins.str] = None,
-    ) -> None:
-        '''(experimental) Attributes for importing a WebSocketApi into the CDK.
-
-        :param web_socket_id: (experimental) The identifier of the WebSocketApi.
-        :param api_endpoint: (experimental) The endpoint URL of the WebSocketApi. Default: - throw san error if apiEndpoint is accessed.
-
-        :stability: experimental
-        :exampleMetadata: infused
-
-        Example::
-
-            web_socket_api = apigwv2.WebSocketApi.from_web_socket_api_attributes(self, "mywsapi", web_socket_id="api-1234")
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ae0c8df0ca0e715101942e90c3ba6802a24a7d17b7ccaf420c2de7498d0f3110)
-            check_type(argname="argument web_socket_id", value=web_socket_id, expected_type=type_hints["web_socket_id"])
-            check_type(argname="argument api_endpoint", value=api_endpoint, expected_type=type_hints["api_endpoint"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
-            "web_socket_id": web_socket_id,
-        }
-        if api_endpoint is not None:
-            self._values["api_endpoint"] = api_endpoint
-
-    @builtins.property
-    def web_socket_id(self) -> builtins.str:
-        '''(experimental) The identifier of the WebSocketApi.
-
-        :stability: experimental
-        '''
-        result = self._values.get("web_socket_id")
-        assert result is not None, "Required property 'web_socket_id' is missing"
-        return typing.cast(builtins.str, result)
-
-    @builtins.property
-    def api_endpoint(self) -> typing.Optional[builtins.str]:
-        '''(experimental) The endpoint URL of the WebSocketApi.
-
-        :default: - throw san error if apiEndpoint is accessed.
-
-        :stability: experimental
-        '''
-        result = self._values.get("api_endpoint")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "WebSocketApiAttributes(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
-
 class WebSocketApiKeySelectionExpression(
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.WebSocketApiKeySelectionExpression",
 ):
     '''(experimental) Represents the currently available API Key Selection Expressions.
 
     :stability: experimental
-    :exampleMetadata: infused
+    :exampleMetadata: fixture=_generated
 
     Example::
 
-        web_socket_api = apigwv2.WebSocketApi(self, "mywsapi",
-            api_key_selection_expression=apigwv2.WebSocketApiKeySelectionExpression.HEADER_X_API_KEY
-        )
+        # The code below shows an example of how to instantiate this type.
+        # The values are placeholders you should change.
+        import aws_cdk.aws_apigatewayv2_alpha as apigatewayv2_alpha
+        
+        web_socket_api_key_selection_expression = apigatewayv2_alpha.WebSocketApiKeySelectionExpression("customApiKeySelector")
     '''
 
     def __init__(self, custom_api_key_selector: builtins.str) -> None:
         '''
         :param custom_api_key_selector: The expression used by API Gateway.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__34791e0880629c49a9f044c4e76a43e531d8704f81a7f9c57e446e0f8af0541c)
-            check_type(argname="argument custom_api_key_selector", value=custom_api_key_selector, expected_type=type_hints["custom_api_key_selector"])
         jsii.create(self.__class__, self, [custom_api_key_selector])
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="AUTHORIZER_USAGE_IDENTIFIER_KEY")
     def AUTHORIZER_USAGE_IDENTIFIER_KEY(cls) -> "WebSocketApiKeySelectionExpression":
         '''(experimental) The API will extract the key value from the ``usageIdentifierKey`` attribute in the ``context`` map, returned by the Lambda Authorizer.
 
         See https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-lambda-authorizer-output.html
 
         :stability: experimental
         '''
         return typing.cast("WebSocketApiKeySelectionExpression", jsii.sget(cls, "AUTHORIZER_USAGE_IDENTIFIER_KEY"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="HEADER_X_API_KEY")
     def HEADER_X_API_KEY(cls) -> "WebSocketApiKeySelectionExpression":
         '''(experimental) The API will extract the key value from the ``x-api-key`` header in the user request.
 
         :stability: experimental
         '''
         return typing.cast("WebSocketApiKeySelectionExpression", jsii.sget(cls, "HEADER_X_API_KEY"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="customApiKeySelector")
     def custom_api_key_selector(self) -> builtins.str:
         '''(experimental) The expression used by API Gateway.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "customApiKeySelector"))
@@ -6246,18 +5734,18 @@
 )
 class WebSocketApiProps:
     def __init__(
         self,
         *,
         api_key_selection_expression: typing.Optional[WebSocketApiKeySelectionExpression] = None,
         api_name: typing.Optional[builtins.str] = None,
-        connect_route_options: typing.Optional[typing.Union["WebSocketRouteOptions", typing.Dict[builtins.str, typing.Any]]] = None,
-        default_route_options: typing.Optional[typing.Union["WebSocketRouteOptions", typing.Dict[builtins.str, typing.Any]]] = None,
+        connect_route_options: typing.Optional["WebSocketRouteOptions"] = None,
+        default_route_options: typing.Optional["WebSocketRouteOptions"] = None,
         description: typing.Optional[builtins.str] = None,
-        disconnect_route_options: typing.Optional[typing.Union["WebSocketRouteOptions", typing.Dict[builtins.str, typing.Any]]] = None,
+        disconnect_route_options: typing.Optional["WebSocketRouteOptions"] = None,
         route_selection_expression: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Props for WebSocket API.
 
         :param api_key_selection_expression: (experimental) An API key selection expression. Providing this option will require an API Key be provided to access the API. Default: - Key is not required to access these APIs
         :param api_name: (experimental) Name for the WebSocket API resource. Default: - id of the WebSocketApi construct.
         :param connect_route_options: (experimental) Options to configure a '$connect' route. Default: - no '$connect' route configured
@@ -6267,51 +5755,40 @@
         :param route_selection_expression: (experimental) The route selection expression for the API. Default: '$request.body.action'
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
-            from aws_cdk.aws_apigatewayv2_authorizers_alpha import WebSocketLambdaAuthorizer
             from aws_cdk.aws_apigatewayv2_integrations_alpha import WebSocketLambdaIntegration
             
-            # This function handles your auth logic
-            # auth_handler: lambda.Function
+            # connect_handler: lambda.Function
+            # disconnect_handler: lambda.Function
+            # default_handler: lambda.Function
             
-            # This function handles your WebSocket requests
-            # handler: lambda.Function
             
+            web_socket_api = apigwv2.WebSocketApi(self, "mywsapi",
+                connect_route_options=apigwv2.WebSocketRouteOptions(integration=WebSocketLambdaIntegration("ConnectIntegration", connect_handler)),
+                disconnect_route_options=apigwv2.WebSocketRouteOptions(integration=WebSocketLambdaIntegration("DisconnectIntegration", disconnect_handler)),
+                default_route_options=apigwv2.WebSocketRouteOptions(integration=WebSocketLambdaIntegration("DefaultIntegration", default_handler))
+            )
             
-            authorizer = WebSocketLambdaAuthorizer("Authorizer", auth_handler)
-            
-            integration = WebSocketLambdaIntegration("Integration", handler)
-            
-            apigwv2.WebSocketApi(self, "WebSocketApi",
-                connect_route_options=apigwv2.WebSocketRouteOptions(
-                    integration=integration,
-                    authorizer=authorizer
-                )
+            apigwv2.WebSocketStage(self, "mystage",
+                web_socket_api=web_socket_api,
+                stage_name="dev",
+                auto_deploy=True
             )
         '''
         if isinstance(connect_route_options, dict):
             connect_route_options = WebSocketRouteOptions(**connect_route_options)
         if isinstance(default_route_options, dict):
             default_route_options = WebSocketRouteOptions(**default_route_options)
         if isinstance(disconnect_route_options, dict):
             disconnect_route_options = WebSocketRouteOptions(**disconnect_route_options)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__92cd23b712e91b17d8d403f5d44376505198f2e4d79f2370e3ce6a05ea6ddc2a)
-            check_type(argname="argument api_key_selection_expression", value=api_key_selection_expression, expected_type=type_hints["api_key_selection_expression"])
-            check_type(argname="argument api_name", value=api_name, expected_type=type_hints["api_name"])
-            check_type(argname="argument connect_route_options", value=connect_route_options, expected_type=type_hints["connect_route_options"])
-            check_type(argname="argument default_route_options", value=default_route_options, expected_type=type_hints["default_route_options"])
-            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
-            check_type(argname="argument disconnect_route_options", value=disconnect_route_options, expected_type=type_hints["disconnect_route_options"])
-            check_type(argname="argument route_selection_expression", value=route_selection_expression, expected_type=type_hints["route_selection_expression"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if api_key_selection_expression is not None:
             self._values["api_key_selection_expression"] = api_key_selection_expression
         if api_name is not None:
             self._values["api_name"] = api_name
         if connect_route_options is not None:
             self._values["connect_route_options"] = connect_route_options
         if default_route_options is not None:
@@ -6414,15 +5891,15 @@
         return "WebSocketApiProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.implements(IWebSocketAuthorizer)
 class WebSocketAuthorizer(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.WebSocketAuthorizer",
 ):
     '''(experimental) An authorizer for WebSocket Apis.
 
     :stability: experimental
     :resource: AWS::ApiGatewayV2::Authorizer
@@ -6445,15 +5922,15 @@
             authorizer_name="authorizerName",
             authorizer_uri="authorizerUri"
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         identity_source: typing.Sequence[builtins.str],
         type: "WebSocketAuthorizerType",
         web_socket_api: IWebSocketApi,
         authorizer_name: typing.Optional[builtins.str] = None,
         authorizer_uri: typing.Optional[builtins.str] = None,
@@ -6465,58 +5942,50 @@
         :param type: (experimental) The type of authorizer.
         :param web_socket_api: (experimental) WebSocket Api to attach the authorizer to.
         :param authorizer_name: (experimental) Name of the authorizer. Default: - id of the WebSocketAuthorizer construct.
         :param authorizer_uri: (experimental) The authorizer's Uniform Resource Identifier (URI). For REQUEST authorizers, this must be a well-formed Lambda function URI. Default: - required for Request authorizer types
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f24f7e7421170c9759c052f1d385a1f7e94dbd5eb18e0b47be9cab3ee8826990)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = WebSocketAuthorizerProps(
             identity_source=identity_source,
             type=type,
             web_socket_api=web_socket_api,
             authorizer_name=authorizer_name,
             authorizer_uri=authorizer_uri,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromWebSocketAuthorizerAttributes")
+    @jsii.member(jsii_name="fromWebSocketAuthorizerAttributes") # type: ignore[misc]
     @builtins.classmethod
     def from_web_socket_authorizer_attributes(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         authorizer_id: builtins.str,
         authorizer_type: builtins.str,
     ) -> IWebSocketRouteAuthorizer:
         '''(experimental) Import an existing WebSocket Authorizer into this CDK app.
 
         :param scope: -
         :param id: -
         :param authorizer_id: (experimental) Id of the Authorizer.
         :param authorizer_type: (experimental) Type of authorizer. Possible values are: - CUSTOM - Lambda Authorizer - NONE - No Authorization
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e383ace2ee0471b5314c8dcb5e8b4c903443f7f45d06e85ce1160c2494ade7c3)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         attrs = WebSocketAuthorizerAttributes(
             authorizer_id=authorizer_id, authorizer_type=authorizer_type
         )
 
         return typing.cast(IWebSocketRouteAuthorizer, jsii.sinvoke(cls, "fromWebSocketAuthorizerAttributes", [scope, id, attrs]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="authorizerId")
     def authorizer_id(self) -> builtins.str:
         '''(experimental) Id of the Authorizer.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "authorizerId"))
@@ -6552,19 +6021,15 @@
             import aws_cdk.aws_apigatewayv2_alpha as apigatewayv2_alpha
             
             web_socket_authorizer_attributes = apigatewayv2_alpha.WebSocketAuthorizerAttributes(
                 authorizer_id="authorizerId",
                 authorizer_type="authorizerType"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ec6cd687f35d4560bc6ed8b97968247261b8e88313cf6380b0c261222b1d373c)
-            check_type(argname="argument authorizer_id", value=authorizer_id, expected_type=type_hints["authorizer_id"])
-            check_type(argname="argument authorizer_type", value=authorizer_type, expected_type=type_hints["authorizer_type"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "authorizer_id": authorizer_id,
             "authorizer_type": authorizer_type,
         }
 
     @builtins.property
     def authorizer_id(self) -> builtins.str:
         '''(experimental) Id of the Authorizer.
@@ -6648,22 +6113,15 @@
                 web_socket_api=web_socket_api,
             
                 # the properties below are optional
                 authorizer_name="authorizerName",
                 authorizer_uri="authorizerUri"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e02c909494ad68823621decb1cf4f3c9d5a9383ba2429deace659f406a376cde)
-            check_type(argname="argument identity_source", value=identity_source, expected_type=type_hints["identity_source"])
-            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
-            check_type(argname="argument web_socket_api", value=web_socket_api, expected_type=type_hints["web_socket_api"])
-            check_type(argname="argument authorizer_name", value=authorizer_name, expected_type=type_hints["authorizer_name"])
-            check_type(argname="argument authorizer_uri", value=authorizer_uri, expected_type=type_hints["authorizer_uri"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "identity_source": identity_source,
             "type": type,
             "web_socket_api": web_socket_api,
         }
         if authorizer_name is not None:
             self._values["authorizer_name"] = authorizer_name
         if authorizer_uri is not None:
@@ -6744,24 +6202,19 @@
     '''
 
     LAMBDA = "LAMBDA"
     '''(experimental) Lambda Authorizer.
 
     :stability: experimental
     '''
-    IAM = "IAM"
-    '''(experimental) IAM Authorizer.
-
-    :stability: experimental
-    '''
 
 
 @jsii.implements(IWebSocketIntegration)
 class WebSocketIntegration(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.WebSocketIntegration",
 ):
     '''(experimental) The integration for an API route.
 
     :stability: experimental
     :resource: AWS::ApiGatewayV2::Integration
@@ -6780,15 +6233,15 @@
             integration_uri="integrationUri",
             web_socket_api=web_socket_api
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         integration_type: "WebSocketIntegrationType",
         integration_uri: builtins.str,
         web_socket_api: IWebSocketApi,
     ) -> None:
         '''
@@ -6796,36 +6249,32 @@
         :param id: -
         :param integration_type: (experimental) Integration type.
         :param integration_uri: (experimental) Integration URI.
         :param web_socket_api: (experimental) The WebSocket API to which this integration should be bound.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__870fc94d82010681246ecba710a6ed2fbd784a22488897490747220c5a9bb1a9)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = WebSocketIntegrationProps(
             integration_type=integration_type,
             integration_uri=integration_uri,
             web_socket_api=web_socket_api,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="integrationId")
     def integration_id(self) -> builtins.str:
         '''(experimental) Id of the integration.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "integrationId"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="webSocketApi")
     def web_socket_api(self) -> IWebSocketApi:
         '''(experimental) The WebSocket API associated with this integration.
 
         :stability: experimental
         '''
         return typing.cast(IWebSocketApi, jsii.get(self, "webSocketApi"))
@@ -6867,20 +6316,15 @@
             
             web_socket_integration_props = apigatewayv2_alpha.WebSocketIntegrationProps(
                 integration_type=apigatewayv2_alpha.WebSocketIntegrationType.AWS_PROXY,
                 integration_uri="integrationUri",
                 web_socket_api=web_socket_api
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__809d7a61872d8b86104362e83bf279e0275cab4ee56d78bb981f42a476435905)
-            check_type(argname="argument integration_type", value=integration_type, expected_type=type_hints["integration_type"])
-            check_type(argname="argument integration_uri", value=integration_uri, expected_type=type_hints["integration_uri"])
-            check_type(argname="argument web_socket_api", value=web_socket_api, expected_type=type_hints["web_socket_api"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "integration_type": integration_type,
             "integration_uri": integration_uri,
             "web_socket_api": web_socket_api,
         }
 
     @builtins.property
     def integration_type(self) -> "WebSocketIntegrationType":
@@ -6969,31 +6413,31 @@
         jsii.create(self.__class__, self, [])
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
         *,
         route: IWebSocketRoute,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
     ) -> "WebSocketRouteAuthorizerConfig":
         '''(experimental) Bind this authorizer to a specified WebSocket route.
 
         :param route: (experimental) The route to which the authorizer is being bound.
         :param scope: (experimental) The scope for any constructs created as part of the bind.
 
         :stability: experimental
         '''
-        _options = WebSocketRouteAuthorizerBindOptions(route=route, scope=scope)
+        _ = WebSocketRouteAuthorizerBindOptions(route=route, scope=scope)
 
-        return typing.cast("WebSocketRouteAuthorizerConfig", jsii.invoke(self, "bind", [_options]))
+        return typing.cast("WebSocketRouteAuthorizerConfig", jsii.invoke(self, "bind", [_]))
 
 
 @jsii.implements(IWebSocketRoute)
 class WebSocketRoute(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.WebSocketRoute",
 ):
     '''(experimental) Route class that creates the Route for API Gateway WebSocket API.
 
     :stability: experimental
     :resource: AWS::ApiGatewayV2::Route
@@ -7012,86 +6456,78 @@
         web_socket_route = apigatewayv2_alpha.WebSocketRoute(self, "MyWebSocketRoute",
             integration=web_socket_route_integration,
             route_key="routeKey",
             web_socket_api=web_socket_api,
         
             # the properties below are optional
             api_key_required=False,
-            authorizer=web_socket_route_authorizer,
-            return_response=False
+            authorizer=web_socket_route_authorizer
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         route_key: builtins.str,
         web_socket_api: IWebSocketApi,
         api_key_required: typing.Optional[builtins.bool] = None,
         integration: "WebSocketRouteIntegration",
         authorizer: typing.Optional[IWebSocketRouteAuthorizer] = None,
-        return_response: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param route_key: (experimental) The key to this route.
         :param web_socket_api: (experimental) The API the route is associated with.
         :param api_key_required: (experimental) Whether the route requires an API Key to be provided. Default: false
         :param integration: (experimental) The integration to be configured on this route.
         :param authorizer: (experimental) The authorize to this route. You can only set authorizer to a $connect route. Default: - No Authorizer
-        :param return_response: (experimental) Should the route send a response to the client. Default: false
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__89ed8dea5fd2abdd3d7348cec8375728ea8c56911ab73c2e7661f42936a36951)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = WebSocketRouteProps(
             route_key=route_key,
             web_socket_api=web_socket_api,
             api_key_required=api_key_required,
             integration=integration,
             authorizer=authorizer,
-            return_response=return_response,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="routeId")
     def route_id(self) -> builtins.str:
         '''(experimental) Id of the Route.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "routeId"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="routeKey")
     def route_key(self) -> builtins.str:
         '''(experimental) The key to this route.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "routeKey"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="webSocketApi")
     def web_socket_api(self) -> IWebSocketApi:
         '''(experimental) The WebSocket API associated with this route.
 
         :stability: experimental
         '''
         return typing.cast(IWebSocketApi, jsii.get(self, "webSocketApi"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="integrationResponseId")
     def integration_response_id(self) -> typing.Optional[builtins.str]:
         '''(experimental) Integration response ID.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "integrationResponseId"))
@@ -7099,20 +6535,15 @@
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.WebSocketRouteAuthorizerBindOptions",
     jsii_struct_bases=[],
     name_mapping={"route": "route", "scope": "scope"},
 )
 class WebSocketRouteAuthorizerBindOptions:
-    def __init__(
-        self,
-        *,
-        route: IWebSocketRoute,
-        scope: _constructs_77d1e7e8.Construct,
-    ) -> None:
+    def __init__(self, *, route: IWebSocketRoute, scope: constructs.Construct) -> None:
         '''(experimental) Input to the bind() operation, that binds an authorizer to a route.
 
         :param route: (experimental) The route to which the authorizer is being bound.
         :param scope: (experimental) The scope for any constructs created as part of the bind.
 
         :stability: experimental
         :exampleMetadata: fixture=_generated
@@ -7128,19 +6559,15 @@
             # web_socket_route: apigatewayv2_alpha.WebSocketRoute
             
             web_socket_route_authorizer_bind_options = apigatewayv2_alpha.WebSocketRouteAuthorizerBindOptions(
                 route=web_socket_route,
                 scope=construct
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fccd4465748920ec078ce3c095e6d5997201164b60c9937b341677d4bed18d2d)
-            check_type(argname="argument route", value=route, expected_type=type_hints["route"])
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "route": route,
             "scope": scope,
         }
 
     @builtins.property
     def route(self) -> IWebSocketRoute:
         '''(experimental) The route to which the authorizer is being bound.
@@ -7148,22 +6575,22 @@
         :stability: experimental
         '''
         result = self._values.get("route")
         assert result is not None, "Required property 'route' is missing"
         return typing.cast(IWebSocketRoute, result)
 
     @builtins.property
-    def scope(self) -> _constructs_77d1e7e8.Construct:
+    def scope(self) -> constructs.Construct:
         '''(experimental) The scope for any constructs created as part of the bind.
 
         :stability: experimental
         '''
         result = self._values.get("scope")
         assert result is not None, "Required property 'scope' is missing"
-        return typing.cast(_constructs_77d1e7e8.Construct, result)
+        return typing.cast(constructs.Construct, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -7205,19 +6632,15 @@
             web_socket_route_authorizer_config = apigatewayv2_alpha.WebSocketRouteAuthorizerConfig(
                 authorization_type="authorizationType",
             
                 # the properties below are optional
                 authorizer_id="authorizerId"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__31b7978ca3879b28e59655ad191a6a2a4b1f15e48c662e792f29609537418e7b)
-            check_type(argname="argument authorization_type", value=authorization_type, expected_type=type_hints["authorization_type"])
-            check_type(argname="argument authorizer_id", value=authorizer_id, expected_type=type_hints["authorizer_id"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "authorization_type": authorization_type,
         }
         if authorizer_id is not None:
             self._values["authorizer_id"] = authorizer_id
 
     @builtins.property
     def authorization_type(self) -> builtins.str:
@@ -7287,26 +6710,23 @@
     def __init__(self, id: builtins.str) -> None:
         '''(experimental) Initialize an integration for a route on websocket api.
 
         :param id: id of the underlying ``WebSocketIntegration`` construct.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c197ca72497cd4c42d540f6e0560e6883980b3d825f1228e227525877aff3ac4)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         jsii.create(self.__class__, self, [id])
 
-    @jsii.member(jsii_name="bind")
+    @jsii.member(jsii_name="bind") # type: ignore[misc]
     @abc.abstractmethod
     def bind(
         self,
         *,
         route: IWebSocketRoute,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
     ) -> "WebSocketRouteIntegrationConfig":
         '''(experimental) Bind this integration to the route.
 
         :param route: (experimental) The route to which this is being bound.
         :param scope: (experimental) The current scope in which the bind is occurring. If the ``WebSocketRouteIntegration`` being bound creates additional constructs, this will be used as their parent scope.
 
         :stability: experimental
@@ -7316,15 +6736,15 @@
 
 class _WebSocketRouteIntegrationProxy(WebSocketRouteIntegration):
     @jsii.member(jsii_name="bind")
     def bind(
         self,
         *,
         route: IWebSocketRoute,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
     ) -> "WebSocketRouteIntegrationConfig":
         '''(experimental) Bind this integration to the route.
 
         :param route: (experimental) The route to which this is being bound.
         :param scope: (experimental) The current scope in which the bind is occurring. If the ``WebSocketRouteIntegration`` being bound creates additional constructs, this will be used as their parent scope.
 
         :stability: experimental
@@ -7339,20 +6759,15 @@
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.WebSocketRouteIntegrationBindOptions",
     jsii_struct_bases=[],
     name_mapping={"route": "route", "scope": "scope"},
 )
 class WebSocketRouteIntegrationBindOptions:
-    def __init__(
-        self,
-        *,
-        route: IWebSocketRoute,
-        scope: _constructs_77d1e7e8.Construct,
-    ) -> None:
+    def __init__(self, *, route: IWebSocketRoute, scope: constructs.Construct) -> None:
         '''(experimental) Options to the WebSocketRouteIntegration during its bind operation.
 
         :param route: (experimental) The route to which this is being bound.
         :param scope: (experimental) The current scope in which the bind is occurring. If the ``WebSocketRouteIntegration`` being bound creates additional constructs, this will be used as their parent scope.
 
         :stability: experimental
         :exampleMetadata: fixture=_generated
@@ -7368,19 +6783,15 @@
             # web_socket_route: apigatewayv2_alpha.WebSocketRoute
             
             web_socket_route_integration_bind_options = apigatewayv2_alpha.WebSocketRouteIntegrationBindOptions(
                 route=web_socket_route,
                 scope=construct
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a9af6c9ac36dba4ed1e02e99de4fc973a26bd4423e8609681f9bddbf43144cd7)
-            check_type(argname="argument route", value=route, expected_type=type_hints["route"])
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "route": route,
             "scope": scope,
         }
 
     @builtins.property
     def route(self) -> IWebSocketRoute:
         '''(experimental) The route to which this is being bound.
@@ -7388,25 +6799,25 @@
         :stability: experimental
         '''
         result = self._values.get("route")
         assert result is not None, "Required property 'route' is missing"
         return typing.cast(IWebSocketRoute, result)
 
     @builtins.property
-    def scope(self) -> _constructs_77d1e7e8.Construct:
+    def scope(self) -> constructs.Construct:
         '''(experimental) The current scope in which the bind is occurring.
 
         If the ``WebSocketRouteIntegration`` being bound creates additional constructs,
         this will be used as their parent scope.
 
         :stability: experimental
         '''
         result = self._values.get("scope")
         assert result is not None, "Required property 'scope' is missing"
-        return typing.cast(_constructs_77d1e7e8.Construct, result)
+        return typing.cast(constructs.Construct, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -7438,19 +6849,15 @@
             import aws_cdk.aws_apigatewayv2_alpha as apigatewayv2_alpha
             
             web_socket_route_integration_config = apigatewayv2_alpha.WebSocketRouteIntegrationConfig(
                 type=apigatewayv2_alpha.WebSocketIntegrationType.AWS_PROXY,
                 uri="uri"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d9151ff6a777a4992f010dc6dd1747375682b7a6c0d45bfbda07ab180448bf7f)
-            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
-            check_type(argname="argument uri", value=uri, expected_type=type_hints["uri"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "type": type,
             "uri": uri,
         }
 
     @builtins.property
     def type(self) -> WebSocketIntegrationType:
         '''(experimental) Integration type.
@@ -7482,33 +6889,27 @@
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.WebSocketRouteOptions",
     jsii_struct_bases=[],
-    name_mapping={
-        "integration": "integration",
-        "authorizer": "authorizer",
-        "return_response": "returnResponse",
-    },
+    name_mapping={"integration": "integration", "authorizer": "authorizer"},
 )
 class WebSocketRouteOptions:
     def __init__(
         self,
         *,
         integration: WebSocketRouteIntegration,
         authorizer: typing.Optional[IWebSocketRouteAuthorizer] = None,
-        return_response: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''(experimental) Options used to add route to the API.
 
         :param integration: (experimental) The integration to be configured on this route.
         :param authorizer: (experimental) The authorize to this route. You can only set authorizer to a $connect route. Default: - No Authorizer
-        :param return_response: (experimental) Should the route send a response to the client. Default: false
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
             from aws_cdk.aws_apigatewayv2_integrations_alpha import WebSocketLambdaIntegration
@@ -7522,26 +6923,19 @@
                 stage_name="dev",
                 auto_deploy=True
             )
             web_socket_api.add_route("sendmessage",
                 integration=WebSocketLambdaIntegration("SendMessageIntegration", message_handler)
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__015136d7cb99d78ecaebab742d43a14edcb81e619d7967b3b64eaf687c0d9ee3)
-            check_type(argname="argument integration", value=integration, expected_type=type_hints["integration"])
-            check_type(argname="argument authorizer", value=authorizer, expected_type=type_hints["authorizer"])
-            check_type(argname="argument return_response", value=return_response, expected_type=type_hints["return_response"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "integration": integration,
         }
         if authorizer is not None:
             self._values["authorizer"] = authorizer
-        if return_response is not None:
-            self._values["return_response"] = return_response
 
     @builtins.property
     def integration(self) -> WebSocketRouteIntegration:
         '''(experimental) The integration to be configured on this route.
 
         :stability: experimental
         '''
@@ -7558,25 +6952,14 @@
         :default: - No Authorizer
 
         :stability: experimental
         '''
         result = self._values.get("authorizer")
         return typing.cast(typing.Optional[IWebSocketRouteAuthorizer], result)
 
-    @builtins.property
-    def return_response(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Should the route send a response to the client.
-
-        :default: false
-
-        :stability: experimental
-        '''
-        result = self._values.get("return_response")
-        return typing.cast(typing.Optional[builtins.bool], result)
-
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -7587,36 +6970,33 @@
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.WebSocketRouteProps",
     jsii_struct_bases=[WebSocketRouteOptions],
     name_mapping={
         "integration": "integration",
         "authorizer": "authorizer",
-        "return_response": "returnResponse",
         "route_key": "routeKey",
         "web_socket_api": "webSocketApi",
         "api_key_required": "apiKeyRequired",
     },
 )
 class WebSocketRouteProps(WebSocketRouteOptions):
     def __init__(
         self,
         *,
         integration: WebSocketRouteIntegration,
         authorizer: typing.Optional[IWebSocketRouteAuthorizer] = None,
-        return_response: typing.Optional[builtins.bool] = None,
         route_key: builtins.str,
         web_socket_api: IWebSocketApi,
         api_key_required: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''(experimental) Properties to initialize a new Route.
 
         :param integration: (experimental) The integration to be configured on this route.
         :param authorizer: (experimental) The authorize to this route. You can only set authorizer to a $connect route. Default: - No Authorizer
-        :param return_response: (experimental) Should the route send a response to the client. Default: false
         :param route_key: (experimental) The key to this route.
         :param web_socket_api: (experimental) The API the route is associated with.
         :param api_key_required: (experimental) Whether the route requires an API Key to be provided. Default: false
 
         :stability: experimental
         :exampleMetadata: fixture=_generated
 
@@ -7633,35 +7013,24 @@
             web_socket_route_props = apigatewayv2_alpha.WebSocketRouteProps(
                 integration=web_socket_route_integration,
                 route_key="routeKey",
                 web_socket_api=web_socket_api,
             
                 # the properties below are optional
                 api_key_required=False,
-                authorizer=web_socket_route_authorizer,
-                return_response=False
+                authorizer=web_socket_route_authorizer
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__16bac6f0c09166c97608a842bf64940ba77c4a2c9803f76985adfdc50657856b)
-            check_type(argname="argument integration", value=integration, expected_type=type_hints["integration"])
-            check_type(argname="argument authorizer", value=authorizer, expected_type=type_hints["authorizer"])
-            check_type(argname="argument return_response", value=return_response, expected_type=type_hints["return_response"])
-            check_type(argname="argument route_key", value=route_key, expected_type=type_hints["route_key"])
-            check_type(argname="argument web_socket_api", value=web_socket_api, expected_type=type_hints["web_socket_api"])
-            check_type(argname="argument api_key_required", value=api_key_required, expected_type=type_hints["api_key_required"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "integration": integration,
             "route_key": route_key,
             "web_socket_api": web_socket_api,
         }
         if authorizer is not None:
             self._values["authorizer"] = authorizer
-        if return_response is not None:
-            self._values["return_response"] = return_response
         if api_key_required is not None:
             self._values["api_key_required"] = api_key_required
 
     @builtins.property
     def integration(self) -> WebSocketRouteIntegration:
         '''(experimental) The integration to be configured on this route.
 
@@ -7681,25 +7050,14 @@
 
         :stability: experimental
         '''
         result = self._values.get("authorizer")
         return typing.cast(typing.Optional[IWebSocketRouteAuthorizer], result)
 
     @builtins.property
-    def return_response(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Should the route send a response to the client.
-
-        :default: false
-
-        :stability: experimental
-        '''
-        result = self._values.get("return_response")
-        return typing.cast(typing.Optional[builtins.bool], result)
-
-    @builtins.property
     def route_key(self) -> builtins.str:
         '''(experimental) The key to this route.
 
         :stability: experimental
         '''
         result = self._values.get("route_key")
         assert result is not None, "Required property 'route_key' is missing"
@@ -7736,203 +7094,190 @@
         return "WebSocketRouteProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.implements(IWebSocketStage, IStage)
 class WebSocketStage(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.WebSocketStage",
 ):
     '''(experimental) Represents a stage where an instance of the API is deployed.
 
     :stability: experimental
-    :resource: AWS::ApiGatewayV2::Stage
     :exampleMetadata: infused
+    :resource: AWS::ApiGatewayV2::Stage
 
     Example::
 
         from aws_cdk.aws_apigatewayv2_integrations_alpha import WebSocketLambdaIntegration
         
-        # message_handler: lambda.Function
+        # connect_handler: lambda.Function
+        # disconnect_handler: lambda.Function
+        # default_handler: lambda.Function
         
         
-        web_socket_api = apigwv2.WebSocketApi(self, "mywsapi")
+        web_socket_api = apigwv2.WebSocketApi(self, "mywsapi",
+            connect_route_options=apigwv2.WebSocketRouteOptions(integration=WebSocketLambdaIntegration("ConnectIntegration", connect_handler)),
+            disconnect_route_options=apigwv2.WebSocketRouteOptions(integration=WebSocketLambdaIntegration("DisconnectIntegration", disconnect_handler)),
+            default_route_options=apigwv2.WebSocketRouteOptions(integration=WebSocketLambdaIntegration("DefaultIntegration", default_handler))
+        )
+        
         apigwv2.WebSocketStage(self, "mystage",
             web_socket_api=web_socket_api,
             stage_name="dev",
             auto_deploy=True
         )
-        web_socket_api.add_route("sendmessage",
-            integration=WebSocketLambdaIntegration("SendMessageIntegration", message_handler)
-        )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         stage_name: builtins.str,
         web_socket_api: IWebSocketApi,
         auto_deploy: typing.Optional[builtins.bool] = None,
-        domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-        throttle: typing.Optional[typing.Union[ThrottleSettings, typing.Dict[builtins.str, typing.Any]]] = None,
+        domain_mapping: typing.Optional[DomainMappingOptions] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param stage_name: (experimental) The name of the stage.
         :param web_socket_api: (experimental) The WebSocket API to which this stage is associated.
         :param auto_deploy: (experimental) Whether updates to an API automatically trigger a new deployment. Default: false
         :param domain_mapping: (experimental) The options for custom domain and api mapping. Default: - no custom domain and api mapping configuration
-        :param throttle: (experimental) Throttle settings for the routes of this stage. Default: - no throttling configuration
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__48af0e7d3ce9ece527270c25928990cf8b605f1e3585927c1afcc3ffef087cf6)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = WebSocketStageProps(
             stage_name=stage_name,
             web_socket_api=web_socket_api,
             auto_deploy=auto_deploy,
             domain_mapping=domain_mapping,
-            throttle=throttle,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromWebSocketStageAttributes")
+    @jsii.member(jsii_name="fromWebSocketStageAttributes") # type: ignore[misc]
     @builtins.classmethod
     def from_web_socket_stage_attributes(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         api: IWebSocketApi,
         stage_name: builtins.str,
     ) -> IWebSocketStage:
         '''(experimental) Import an existing stage into this CDK app.
 
         :param scope: -
         :param id: -
         :param api: (experimental) The API to which this stage is associated.
         :param stage_name: (experimental) The name of the stage.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__96d2e4a524a0487b6a3e41257302724f03ec2dea315215c2348c1e882d82a509)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         attrs = WebSocketStageAttributes(api=api, stage_name=stage_name)
 
         return typing.cast(IWebSocketStage, jsii.sinvoke(cls, "fromWebSocketStageAttributes", [scope, id, attrs]))
 
     @jsii.member(jsii_name="grantManagementApiAccess")
     def grant_management_api_access(
         self,
-        identity: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-    ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
+        identity: aws_cdk.aws_iam.IGrantable,
+    ) -> aws_cdk.aws_iam.Grant:
         '''(experimental) Grant access to the API Gateway management API for this WebSocket API Stage to an IAM principal (Role/Group/User).
 
         :param identity: The principal.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__385987aac133337ee8f5f880408bf66af8f3e3a5651bc827a3bc5af110334a17)
-            check_type(argname="argument identity", value=identity, expected_type=type_hints["identity"])
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.Grant, jsii.invoke(self, "grantManagementApiAccess", [identity]))
+        return typing.cast(aws_cdk.aws_iam.Grant, jsii.invoke(self, "grantManagementApiAccess", [identity]))
 
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
         '''(experimental) Return the given named metric for this HTTP Api Gateway Stage.
 
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
-            type_hints = typing.get_type_hints(_typecheckingstub__b080276ad15c8223193f7ed4fefbc76be9f47841814221e9a4dee06286100c93)
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
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="api")
     def api(self) -> IWebSocketApi:
         '''(experimental) The API this stage is associated to.
 
         :stability: experimental
         '''
         return typing.cast(IWebSocketApi, jsii.get(self, "api"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="baseApi")
     def _base_api(self) -> IApi:
         '''
         :stability: experimental
         '''
         return typing.cast(IApi, jsii.get(self, "baseApi"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="callbackUrl")
     def callback_url(self) -> builtins.str:
         '''(experimental) The callback URL to this stage.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "callbackUrl"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="stageName")
     def stage_name(self) -> builtins.str:
         '''(experimental) The name of the stage;
 
         its primary identifier.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "stageName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="url")
     def url(self) -> builtins.str:
         '''(experimental) The websocket URL to this stage.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "url"))
@@ -7962,19 +7307,15 @@
             # web_socket_api: apigatewayv2_alpha.WebSocketApi
             
             web_socket_stage_attributes = apigatewayv2_alpha.WebSocketStageAttributes(
                 api=web_socket_api,
                 stage_name="stageName"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3e391865a4ae4984a049207c6b5c3768117999fb528b5847ca1a6c7c35d2f82b)
-            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
-            check_type(argname="argument api", value=api, expected_type=type_hints["api"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "stage_name": stage_name,
             "api": api,
         }
 
     @builtins.property
     def stage_name(self) -> builtins.str:
         '''(experimental) The name of the stage.
@@ -8009,78 +7350,68 @@
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.WebSocketStageProps",
     jsii_struct_bases=[StageOptions],
     name_mapping={
         "auto_deploy": "autoDeploy",
         "domain_mapping": "domainMapping",
-        "throttle": "throttle",
         "stage_name": "stageName",
         "web_socket_api": "webSocketApi",
     },
 )
 class WebSocketStageProps(StageOptions):
     def __init__(
         self,
         *,
         auto_deploy: typing.Optional[builtins.bool] = None,
-        domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-        throttle: typing.Optional[typing.Union[ThrottleSettings, typing.Dict[builtins.str, typing.Any]]] = None,
+        domain_mapping: typing.Optional[DomainMappingOptions] = None,
         stage_name: builtins.str,
         web_socket_api: IWebSocketApi,
     ) -> None:
         '''(experimental) Properties to initialize an instance of ``WebSocketStage``.
 
         :param auto_deploy: (experimental) Whether updates to an API automatically trigger a new deployment. Default: false
         :param domain_mapping: (experimental) The options for custom domain and api mapping. Default: - no custom domain and api mapping configuration
-        :param throttle: (experimental) Throttle settings for the routes of this stage. Default: - no throttling configuration
         :param stage_name: (experimental) The name of the stage.
         :param web_socket_api: (experimental) The WebSocket API to which this stage is associated.
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
             from aws_cdk.aws_apigatewayv2_integrations_alpha import WebSocketLambdaIntegration
             
-            # message_handler: lambda.Function
+            # connect_handler: lambda.Function
+            # disconnect_handler: lambda.Function
+            # default_handler: lambda.Function
             
             
-            web_socket_api = apigwv2.WebSocketApi(self, "mywsapi")
+            web_socket_api = apigwv2.WebSocketApi(self, "mywsapi",
+                connect_route_options=apigwv2.WebSocketRouteOptions(integration=WebSocketLambdaIntegration("ConnectIntegration", connect_handler)),
+                disconnect_route_options=apigwv2.WebSocketRouteOptions(integration=WebSocketLambdaIntegration("DisconnectIntegration", disconnect_handler)),
+                default_route_options=apigwv2.WebSocketRouteOptions(integration=WebSocketLambdaIntegration("DefaultIntegration", default_handler))
+            )
+            
             apigwv2.WebSocketStage(self, "mystage",
                 web_socket_api=web_socket_api,
                 stage_name="dev",
                 auto_deploy=True
             )
-            web_socket_api.add_route("sendmessage",
-                integration=WebSocketLambdaIntegration("SendMessageIntegration", message_handler)
-            )
         '''
         if isinstance(domain_mapping, dict):
             domain_mapping = DomainMappingOptions(**domain_mapping)
-        if isinstance(throttle, dict):
-            throttle = ThrottleSettings(**throttle)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__782ab449d8fa4cf0a46fbab6526bdc241efef3893414586af02c8f715748ee2a)
-            check_type(argname="argument auto_deploy", value=auto_deploy, expected_type=type_hints["auto_deploy"])
-            check_type(argname="argument domain_mapping", value=domain_mapping, expected_type=type_hints["domain_mapping"])
-            check_type(argname="argument throttle", value=throttle, expected_type=type_hints["throttle"])
-            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
-            check_type(argname="argument web_socket_api", value=web_socket_api, expected_type=type_hints["web_socket_api"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "stage_name": stage_name,
             "web_socket_api": web_socket_api,
         }
         if auto_deploy is not None:
             self._values["auto_deploy"] = auto_deploy
         if domain_mapping is not None:
             self._values["domain_mapping"] = domain_mapping
-        if throttle is not None:
-            self._values["throttle"] = throttle
 
     @builtins.property
     def auto_deploy(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Whether updates to an API automatically trigger a new deployment.
 
         :default: false
 
@@ -8097,25 +7428,14 @@
 
         :stability: experimental
         '''
         result = self._values.get("domain_mapping")
         return typing.cast(typing.Optional[DomainMappingOptions], result)
 
     @builtins.property
-    def throttle(self) -> typing.Optional[ThrottleSettings]:
-        '''(experimental) Throttle settings for the routes of this stage.
-
-        :default: - no throttling configuration
-
-        :stability: experimental
-        '''
-        result = self._values.get("throttle")
-        return typing.cast(typing.Optional[ThrottleSettings], result)
-
-    @builtins.property
     def stage_name(self) -> builtins.str:
         '''(experimental) The name of the stage.
 
         :stability: experimental
         '''
         result = self._values.get("stage_name")
         assert result is not None, "Required property 'stage_name' is missing"
@@ -8187,27 +7507,20 @@
             authorizer = HttpLambdaAuthorizer("BooksAuthorizer", auth_handler,
                 response_types=[HttpLambdaResponseType.SIMPLE]
             )
             
             api = apigwv2.HttpApi(self, "HttpApi")
             
             api.add_routes(
-                integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+                integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
                 path="/books",
                 authorizer=authorizer
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ca8141f667bdde01ab0100d57a58a21f4b9acc231a1bbfb55a1925c258a680c6)
-            check_type(argname="argument integration", value=integration, expected_type=type_hints["integration"])
-            check_type(argname="argument path", value=path, expected_type=type_hints["path"])
-            check_type(argname="argument authorization_scopes", value=authorization_scopes, expected_type=type_hints["authorization_scopes"])
-            check_type(argname="argument authorizer", value=authorizer, expected_type=type_hints["authorizer"])
-            check_type(argname="argument methods", value=methods, expected_type=type_hints["methods"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "integration": integration,
             "path": path,
         }
         if authorization_scopes is not None:
             self._values["authorization_scopes"] = authorization_scopes
         if authorizer is not None:
             self._values["authorizer"] = authorizer
@@ -8282,15 +7595,15 @@
         return "AddRoutesOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.implements(IApiMapping)
 class ApiMapping(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.ApiMapping",
 ):
     '''(experimental) Create a new API mapping for API Gateway API endpoint.
 
     :stability: experimental
     :resource: AWS::ApiGatewayV2::ApiMapping
@@ -8314,15 +7627,15 @@
             api_mapping_key="apiMappingKey",
             stage=stage
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         api: IApi,
         domain_name: IDomainName,
         api_mapping_key: typing.Optional[builtins.str] = None,
         stage: typing.Optional[IStage] = None,
     ) -> None:
@@ -8332,83 +7645,75 @@
         :param api: (experimental) The Api to which this mapping is applied.
         :param domain_name: (experimental) custom domain name of the mapping target.
         :param api_mapping_key: (experimental) Api mapping key. The path where this stage should be mapped to on the domain Default: - undefined for the root path mapping.
         :param stage: (experimental) stage for the ApiMapping resource required for WebSocket API defaults to default stage of an HTTP API. Default: - Default stage of the passed API for HTTP API, required for WebSocket API
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__cbff8656b4f6706b46963d8d04c49514410f8af75cfeb33a4c2fe1a07e9f33ac)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = ApiMappingProps(
             api=api,
             domain_name=domain_name,
             api_mapping_key=api_mapping_key,
             stage=stage,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromApiMappingAttributes")
+    @jsii.member(jsii_name="fromApiMappingAttributes") # type: ignore[misc]
     @builtins.classmethod
     def from_api_mapping_attributes(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         api_mapping_id: builtins.str,
     ) -> IApiMapping:
         '''(experimental) import from API ID.
 
         :param scope: -
         :param id: -
         :param api_mapping_id: (experimental) The API mapping ID.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a142e4a61436ea624a748446cb739233abd5326d66a7e1a91f9c88642f61ca94)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         attrs = ApiMappingAttributes(api_mapping_id=api_mapping_id)
 
         return typing.cast(IApiMapping, jsii.sinvoke(cls, "fromApiMappingAttributes", [scope, id, attrs]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="apiMappingId")
     def api_mapping_id(self) -> builtins.str:
         '''(experimental) ID of the API Mapping.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "apiMappingId"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="domainName")
     def domain_name(self) -> IDomainName:
         '''(experimental) API domain name.
 
         :stability: experimental
         '''
         return typing.cast(IDomainName, jsii.get(self, "domainName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="mappingKey")
     def mapping_key(self) -> typing.Optional[builtins.str]:
         '''(experimental) API Mapping key.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "mappingKey"))
 
 
 @jsii.implements(IDomainName)
 class DomainName(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.DomainName",
 ):
     '''(experimental) Custom domain resource for the API.
 
     :stability: experimental
     :exampleMetadata: infused
@@ -8436,23 +7741,23 @@
                 mapping_key="foo"
             )
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         domain_name: builtins.str,
-        mtls: typing.Optional[typing.Union[MTLSConfig, typing.Dict[builtins.str, typing.Any]]] = None,
-        certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
+        mtls: typing.Optional[MTLSConfig] = None,
+        certificate: aws_cdk.aws_certificatemanager.ICertificate,
         certificate_name: typing.Optional[builtins.str] = None,
         endpoint_type: typing.Optional[EndpointType] = None,
-        ownership_certificate: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
+        ownership_certificate: typing.Optional[aws_cdk.aws_certificatemanager.ICertificate] = None,
         security_policy: typing.Optional[SecurityPolicy] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param domain_name: (experimental) The custom domain name.
         :param mtls: (experimental) The mutual TLS authentication configuration for a custom domain name. Default: - mTLS is not configured.
@@ -8460,35 +7765,31 @@
         :param certificate_name: (experimental) The user-friendly name of the certificate that will be used by the endpoint for this domain name. Default: - No friendly certificate name
         :param endpoint_type: (experimental) The type of endpoint for this DomainName. Default: EndpointType.REGIONAL
         :param ownership_certificate: (experimental) A public certificate issued by ACM to validate that you own a custom domain. This parameter is required only when you configure mutual TLS authentication and you specify an ACM imported or private CA certificate for ``certificate``. The ownership certificate validates that you have permissions to use the domain name. Default: - only required when configuring mTLS
         :param security_policy: (experimental) The Transport Layer Security (TLS) version + cipher suite for this domain name. Default: SecurityPolicy.TLS_1_2
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b9d717e977e1b3688e10b96a28c290636a0c8ffb230b0e32f751c93cfed6ae39)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = DomainNameProps(
             domain_name=domain_name,
             mtls=mtls,
             certificate=certificate,
             certificate_name=certificate_name,
             endpoint_type=endpoint_type,
             ownership_certificate=ownership_certificate,
             security_policy=security_policy,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromDomainNameAttributes")
+    @jsii.member(jsii_name="fromDomainNameAttributes") # type: ignore[misc]
     @builtins.classmethod
     def from_domain_name_attributes(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
         regional_domain_name: builtins.str,
         regional_hosted_zone_id: builtins.str,
     ) -> IDomainName:
         '''(experimental) Import from attributes.
@@ -8497,34 +7798,30 @@
         :param id: -
         :param name: (experimental) domain name string.
         :param regional_domain_name: (experimental) The domain name associated with the regional endpoint for this custom domain name.
         :param regional_hosted_zone_id: (experimental) The region-specific Amazon Route 53 Hosted Zone ID of the regional endpoint.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a75b51d5333f983b1ad28c7723855075bb1accd439fd505ecabd1a569a79bab5)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         attrs = DomainNameAttributes(
             name=name,
             regional_domain_name=regional_domain_name,
             regional_hosted_zone_id=regional_hosted_zone_id,
         )
 
         return typing.cast(IDomainName, jsii.sinvoke(cls, "fromDomainNameAttributes", [scope, id, attrs]))
 
     @jsii.member(jsii_name="addEndpoint")
     def add_endpoint(
         self,
         *,
-        certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
+        certificate: aws_cdk.aws_certificatemanager.ICertificate,
         certificate_name: typing.Optional[builtins.str] = None,
         endpoint_type: typing.Optional[EndpointType] = None,
-        ownership_certificate: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
+        ownership_certificate: typing.Optional[aws_cdk.aws_certificatemanager.ICertificate] = None,
         security_policy: typing.Optional[SecurityPolicy] = None,
     ) -> None:
         '''(experimental) Adds an endpoint to a domain name.
 
         :param certificate: (experimental) The ACM certificate for this domain name. Certificate can be both ACM issued or imported.
         :param certificate_name: (experimental) The user-friendly name of the certificate that will be used by the endpoint for this domain name. Default: - No friendly certificate name
         :param endpoint_type: (experimental) The type of endpoint for this DomainName. Default: EndpointType.REGIONAL
@@ -8539,33 +7836,33 @@
             endpoint_type=endpoint_type,
             ownership_certificate=ownership_certificate,
             security_policy=security_policy,
         )
 
         return typing.cast(None, jsii.invoke(self, "addEndpoint", [options]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         '''(experimental) The custom domain name.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "name"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="regionalDomainName")
     def regional_domain_name(self) -> builtins.str:
         '''(experimental) The domain name associated with the regional endpoint for this custom domain name.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "regionalDomainName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="regionalHostedZoneId")
     def regional_hosted_zone_id(self) -> builtins.str:
         '''(experimental) The region-specific Amazon Route 53 Hosted Zone ID of the regional endpoint.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "regionalHostedZoneId"))
@@ -8584,21 +7881,21 @@
         "mtls": "mtls",
     },
 )
 class DomainNameProps(EndpointOptions):
     def __init__(
         self,
         *,
-        certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
+        certificate: aws_cdk.aws_certificatemanager.ICertificate,
         certificate_name: typing.Optional[builtins.str] = None,
         endpoint_type: typing.Optional[EndpointType] = None,
-        ownership_certificate: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
+        ownership_certificate: typing.Optional[aws_cdk.aws_certificatemanager.ICertificate] = None,
         security_policy: typing.Optional[SecurityPolicy] = None,
         domain_name: builtins.str,
-        mtls: typing.Optional[typing.Union[MTLSConfig, typing.Dict[builtins.str, typing.Any]]] = None,
+        mtls: typing.Optional[MTLSConfig] = None,
     ) -> None:
         '''(experimental) properties used for creating the DomainName.
 
         :param certificate: (experimental) The ACM certificate for this domain name. Certificate can be both ACM issued or imported.
         :param certificate_name: (experimental) The user-friendly name of the certificate that will be used by the endpoint for this domain name. Default: - No friendly certificate name
         :param endpoint_type: (experimental) The type of endpoint for this DomainName. Default: EndpointType.REGIONAL
         :param ownership_certificate: (experimental) A public certificate issued by ACM to validate that you own a custom domain. This parameter is required only when you configure mutual TLS authentication and you specify an ACM imported or private CA certificate for ``certificate``. The ownership certificate validates that you have permissions to use the domain name. Default: - only required when configuring mTLS
@@ -8631,24 +7928,15 @@
                     domain_name=dn,
                     mapping_key="foo"
                 )
             )
         '''
         if isinstance(mtls, dict):
             mtls = MTLSConfig(**mtls)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__698fe2808c79855db0ec402620f39e09a615424a13b6af162379044207a388e5)
-            check_type(argname="argument certificate", value=certificate, expected_type=type_hints["certificate"])
-            check_type(argname="argument certificate_name", value=certificate_name, expected_type=type_hints["certificate_name"])
-            check_type(argname="argument endpoint_type", value=endpoint_type, expected_type=type_hints["endpoint_type"])
-            check_type(argname="argument ownership_certificate", value=ownership_certificate, expected_type=type_hints["ownership_certificate"])
-            check_type(argname="argument security_policy", value=security_policy, expected_type=type_hints["security_policy"])
-            check_type(argname="argument domain_name", value=domain_name, expected_type=type_hints["domain_name"])
-            check_type(argname="argument mtls", value=mtls, expected_type=type_hints["mtls"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "certificate": certificate,
             "domain_name": domain_name,
         }
         if certificate_name is not None:
             self._values["certificate_name"] = certificate_name
         if endpoint_type is not None:
             self._values["endpoint_type"] = endpoint_type
@@ -8656,24 +7944,24 @@
             self._values["ownership_certificate"] = ownership_certificate
         if security_policy is not None:
             self._values["security_policy"] = security_policy
         if mtls is not None:
             self._values["mtls"] = mtls
 
     @builtins.property
-    def certificate(self) -> _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate:
+    def certificate(self) -> aws_cdk.aws_certificatemanager.ICertificate:
         '''(experimental) The ACM certificate for this domain name.
 
         Certificate can be both ACM issued or imported.
 
         :stability: experimental
         '''
         result = self._values.get("certificate")
         assert result is not None, "Required property 'certificate' is missing"
-        return typing.cast(_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate, result)
+        return typing.cast(aws_cdk.aws_certificatemanager.ICertificate, result)
 
     @builtins.property
     def certificate_name(self) -> typing.Optional[builtins.str]:
         '''(experimental) The user-friendly name of the certificate that will be used by the endpoint for this domain name.
 
         :default: - No friendly certificate name
 
@@ -8692,27 +7980,27 @@
         '''
         result = self._values.get("endpoint_type")
         return typing.cast(typing.Optional[EndpointType], result)
 
     @builtins.property
     def ownership_certificate(
         self,
-    ) -> typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate]:
+    ) -> typing.Optional[aws_cdk.aws_certificatemanager.ICertificate]:
         '''(experimental) A public certificate issued by ACM to validate that you own a custom domain.
 
         This parameter is required
         only when you configure mutual TLS authentication and you specify an ACM imported or private CA certificate
         for ``certificate``. The ownership certificate validates that you have permissions to use the domain name.
 
         :default: - only required when configuring mTLS
 
         :stability: experimental
         '''
         result = self._values.get("ownership_certificate")
-        return typing.cast(typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_certificatemanager.ICertificate], result)
 
     @builtins.property
     def security_policy(self) -> typing.Optional[SecurityPolicy]:
         '''(experimental) The Transport Layer Security (TLS) version + cipher suite for this domain name.
 
         :default: SecurityPolicy.TLS_1_2
 
@@ -8752,23 +8040,23 @@
         return "DomainNameProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.implements(IHttpApi, IApi)
 class HttpApi(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.HttpApi",
 ):
     '''(experimental) Create a new API Gateway HTTP API endpoint.
 
     :stability: experimental
-    :resource: AWS::ApiGatewayV2::Api
     :exampleMetadata: infused
+    :resource: AWS::ApiGatewayV2::Api
 
     Example::
 
         from aws_cdk.aws_apigatewayv2_integrations_alpha import HttpLambdaIntegration
         
         # books_default_fn: lambda.Function
         
@@ -8781,23 +8069,23 @@
             methods=[apigwv2.HttpMethod.GET],
             integration=books_integration
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         api_name: typing.Optional[builtins.str] = None,
-        cors_preflight: typing.Optional[typing.Union[CorsPreflightOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        cors_preflight: typing.Optional[CorsPreflightOptions] = None,
         create_default_stage: typing.Optional[builtins.bool] = None,
         default_authorization_scopes: typing.Optional[typing.Sequence[builtins.str]] = None,
         default_authorizer: typing.Optional[IHttpRouteAuthorizer] = None,
-        default_domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        default_domain_mapping: typing.Optional[DomainMappingOptions] = None,
         default_integration: typing.Optional[HttpRouteIntegration] = None,
         description: typing.Optional[builtins.str] = None,
         disable_execute_api_endpoint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
@@ -8809,55 +8097,47 @@
         :param default_domain_mapping: (experimental) Configure a custom domain with the API mapping resource to the HTTP API. Default: - no default domain mapping configured. meaningless if ``createDefaultStage`` is ``false``.
         :param default_integration: (experimental) An integration that will be configured on the catch-all route ($default). Default: - none
         :param description: (experimental) The description of the API. Default: - none
         :param disable_execute_api_endpoint: (experimental) Specifies whether clients can invoke your API using the default endpoint. By default, clients can invoke your API with the default ``https://{api_id}.execute-api.{region}.amazonaws.com`` endpoint. Enable this if you would like clients to use your custom domain name. Default: false execute-api endpoint enabled.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d5003409414773984b85252451580f75369de42c80978f161fece7261c553c54)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = HttpApiProps(
             api_name=api_name,
             cors_preflight=cors_preflight,
             create_default_stage=create_default_stage,
             default_authorization_scopes=default_authorization_scopes,
             default_authorizer=default_authorizer,
             default_domain_mapping=default_domain_mapping,
             default_integration=default_integration,
             description=description,
             disable_execute_api_endpoint=disable_execute_api_endpoint,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromHttpApiAttributes")
+    @jsii.member(jsii_name="fromHttpApiAttributes") # type: ignore[misc]
     @builtins.classmethod
     def from_http_api_attributes(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         http_api_id: builtins.str,
         api_endpoint: typing.Optional[builtins.str] = None,
     ) -> IHttpApi:
         '''(experimental) Import an existing HTTP API into this CDK app.
 
         :param scope: -
         :param id: -
         :param http_api_id: (experimental) The identifier of the HttpApi.
         :param api_endpoint: (experimental) The endpoint URL of the HttpApi. Default: - throws an error if apiEndpoint is accessed.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ecd315f15fe552c95da2ac31778a118bb3415d560941e8d18e9c71e631481225)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         attrs = HttpApiAttributes(http_api_id=http_api_id, api_endpoint=api_endpoint)
 
         return typing.cast(IHttpApi, jsii.sinvoke(cls, "fromHttpApiAttributes", [scope, id, attrs]))
 
     @jsii.member(jsii_name="addRoutes")
     def add_routes(
         self,
@@ -8894,46 +8174,40 @@
     @jsii.member(jsii_name="addStage")
     def add_stage(
         self,
         id: builtins.str,
         *,
         stage_name: typing.Optional[builtins.str] = None,
         auto_deploy: typing.Optional[builtins.bool] = None,
-        domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-        throttle: typing.Optional[typing.Union[ThrottleSettings, typing.Dict[builtins.str, typing.Any]]] = None,
+        domain_mapping: typing.Optional[DomainMappingOptions] = None,
     ) -> "HttpStage":
         '''(experimental) Add a new stage.
 
         :param id: -
         :param stage_name: (experimental) The name of the stage. See ``StageName`` class for more details. Default: '$default' the default stage of the API. This stage will have the URL at the root of the API endpoint.
         :param auto_deploy: (experimental) Whether updates to an API automatically trigger a new deployment. Default: false
         :param domain_mapping: (experimental) The options for custom domain and api mapping. Default: - no custom domain and api mapping configuration
-        :param throttle: (experimental) Throttle settings for the routes of this stage. Default: - no throttling configuration
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2bab5e6089f6e913d418934d66da25f8a39159ad3bd9f9f115cbcde831da78e0)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         options = HttpStageOptions(
             stage_name=stage_name,
             auto_deploy=auto_deploy,
             domain_mapping=domain_mapping,
-            throttle=throttle,
         )
 
         return typing.cast("HttpStage", jsii.invoke(self, "addStage", [id, options]))
 
     @jsii.member(jsii_name="addVpcLink")
     def add_vpc_link(
         self,
         *,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-        subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        vpc: aws_cdk.aws_ec2.IVpc,
+        security_groups: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.ISecurityGroup]] = None,
+        subnets: typing.Optional[aws_cdk.aws_ec2.SubnetSelection] = None,
         vpc_link_name: typing.Optional[builtins.str] = None,
     ) -> VpcLink:
         '''(experimental) Add a new VpcLink.
 
         :param vpc: (experimental) The VPC in which the private resources reside.
         :param security_groups: (experimental) A list of security groups for the VPC link. Default: - no security groups. Use ``addSecurityGroups`` to add security groups
         :param subnets: (experimental) A list of subnets for the VPC link. Default: - private subnets of the provided VPC. Use ``addSubnets`` to add more subnets
@@ -8955,356 +8229,353 @@
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
         '''(experimental) Return the given named metric for this Api Gateway.
 
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
-            type_hints = typing.get_type_hints(_typecheckingstub__a7709e3cbcd45c7d4a9b816ad94388873b7fd0558ca6fdcb427f2d5ca6e8df6a)
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
 
     @jsii.member(jsii_name="metricClientError")
     def metric_client_error(
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
         '''(experimental) Metric for the number of client-side errors captured in a given period.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricClientError", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricClientError", [props]))
 
     @jsii.member(jsii_name="metricCount")
     def metric_count(
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
         '''(experimental) Metric for the total number API requests in a given period.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricCount", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricCount", [props]))
 
     @jsii.member(jsii_name="metricDataProcessed")
     def metric_data_processed(
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
         '''(experimental) Metric for the amount of data processed in bytes.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricDataProcessed", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricDataProcessed", [props]))
 
     @jsii.member(jsii_name="metricIntegrationLatency")
     def metric_integration_latency(
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
         '''(experimental) Metric for the time between when API Gateway relays a request to the backend and when it receives a response from the backend.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricIntegrationLatency", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricIntegrationLatency", [props]))
 
     @jsii.member(jsii_name="metricLatency")
     def metric_latency(
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
         '''(experimental) The time between when API Gateway receives a request from a client and when it returns a response to the client.
 
         The latency includes the integration latency and other API Gateway overhead.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricLatency", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricLatency", [props]))
 
     @jsii.member(jsii_name="metricServerError")
     def metric_server_error(
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
         '''(experimental) Metric for the number of server-side errors captured in a given period.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricServerError", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricServerError", [props]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="apiEndpoint")
     def api_endpoint(self) -> builtins.str:
         '''(experimental) Get the default endpoint for this API.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "apiEndpoint"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="apiId")
     def api_id(self) -> builtins.str:
         '''(experimental) The identifier of this API Gateway API.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "apiId"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="httpApiId")
     def http_api_id(self) -> builtins.str:
         '''(experimental) The identifier of this API Gateway HTTP API.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "httpApiId"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="defaultStage")
     def default_stage(self) -> typing.Optional["IHttpStage"]:
         '''(experimental) The default stage of this API.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional["IHttpStage"], jsii.get(self, "defaultStage"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="disableExecuteApiEndpoint")
     def disable_execute_api_endpoint(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Specifies whether clients can invoke this HTTP API by using the default execute-api endpoint.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "disableExecuteApiEndpoint"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="httpApiName")
     def http_api_name(self) -> typing.Optional[builtins.str]:
         '''(experimental) A human friendly name for this HTTP API.
 
         Note that this is different from ``httpApiId``.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "httpApiName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="url")
     def url(self) -> typing.Optional[builtins.str]:
         '''(experimental) Get the URL to the default stage of this API.
 
         Returns ``undefined`` if ``createDefaultStage`` is unset.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "url"))
 
 
 @jsii.implements(IHttpAuthorizer)
 class HttpAuthorizer(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.HttpAuthorizer",
 ):
     '''(experimental) An authorizer for Http Apis.
 
     :stability: experimental
     :resource: AWS::ApiGatewayV2::Authorizer
@@ -9333,27 +8604,27 @@
             payload_format_version=apigatewayv2_alpha.AuthorizerPayloadVersion.VERSION_1_0,
             results_cache_ttl=cdk.Duration.minutes(30)
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         http_api: IHttpApi,
         identity_source: typing.Sequence[builtins.str],
         type: HttpAuthorizerType,
         authorizer_name: typing.Optional[builtins.str] = None,
         authorizer_uri: typing.Optional[builtins.str] = None,
         enable_simple_responses: typing.Optional[builtins.bool] = None,
         jwt_audience: typing.Optional[typing.Sequence[builtins.str]] = None,
         jwt_issuer: typing.Optional[builtins.str] = None,
         payload_format_version: typing.Optional[AuthorizerPayloadVersion] = None,
-        results_cache_ttl: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        results_cache_ttl: typing.Optional[aws_cdk.Duration] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param http_api: (experimental) HTTP Api to attach the authorizer to.
         :param identity_source: (experimental) The identity source for which authorization is requested.
         :param type: (experimental) The type of authorizer.
@@ -9363,18 +8634,14 @@
         :param jwt_audience: (experimental) A list of the intended recipients of the JWT. A valid JWT must provide an aud that matches at least one entry in this list. Default: - required for JWT authorizer typess.
         :param jwt_issuer: (experimental) The base domain of the identity provider that issues JWT. Default: - required for JWT authorizer types.
         :param payload_format_version: (experimental) Specifies the format of the payload sent to an HTTP API Lambda authorizer. Default: AuthorizerPayloadVersion.VERSION_2_0 if the authorizer type is HttpAuthorizerType.LAMBDA
         :param results_cache_ttl: (experimental) How long APIGateway should cache the results. Max 1 hour. Default: - API Gateway will not cache authorizer responses
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__03f7fb4792b9161dda177d8df2f5bc58091a4f546c4ca11ee18afaa4e0bf5e28)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = HttpAuthorizerProps(
             http_api=http_api,
             identity_source=identity_source,
             type=type,
             authorizer_name=authorizer_name,
             authorizer_uri=authorizer_uri,
             enable_simple_responses=enable_simple_responses,
@@ -9382,44 +8649,40 @@
             jwt_issuer=jwt_issuer,
             payload_format_version=payload_format_version,
             results_cache_ttl=results_cache_ttl,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromHttpAuthorizerAttributes")
+    @jsii.member(jsii_name="fromHttpAuthorizerAttributes") # type: ignore[misc]
     @builtins.classmethod
     def from_http_authorizer_attributes(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         authorizer_id: builtins.str,
         authorizer_type: builtins.str,
     ) -> IHttpRouteAuthorizer:
         '''(experimental) Import an existing HTTP Authorizer into this CDK app.
 
         :param scope: -
         :param id: -
         :param authorizer_id: (experimental) Id of the Authorizer.
         :param authorizer_type: (experimental) Type of authorizer. Possible values are: - JWT - JSON Web Token Authorizer - CUSTOM - Lambda Authorizer - NONE - No Authorization
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__efb4a2f65822f686a6ffa7ada308b84e89325054661df552cb9bc6286414ff5b)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         attrs = HttpAuthorizerAttributes(
             authorizer_id=authorizer_id, authorizer_type=authorizer_type
         )
 
         return typing.cast(IHttpRouteAuthorizer, jsii.sinvoke(cls, "fromHttpAuthorizerAttributes", [scope, id, attrs]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="authorizerId")
     def authorizer_id(self) -> builtins.str:
         '''(experimental) Id of the Authorizer.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "authorizerId"))
@@ -9448,34 +8711,34 @@
         
         api = apigwv2.HttpApi(self, "HttpApi",
             default_authorizer=authorizer,
             default_authorization_scopes=["read:books"]
         )
         
         api.add_routes(
-            integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+            integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
             path="/books",
             methods=[apigwv2.HttpMethod.GET]
         )
         
         api.add_routes(
-            integration=HttpUrlIntegration("BooksIdIntegration", "https://get-books-proxy.example.com"),
+            integration=HttpUrlIntegration("BooksIdIntegration", "https://get-books-proxy.myproxy.internal"),
             path="/books/{id}",
             methods=[apigwv2.HttpMethod.GET]
         )
         
         api.add_routes(
-            integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+            integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
             path="/books",
             methods=[apigwv2.HttpMethod.POST],
             authorization_scopes=["write:books"]
         )
         
         api.add_routes(
-            integration=HttpUrlIntegration("LoginIntegration", "https://get-books-proxy.example.com"),
+            integration=HttpUrlIntegration("LoginIntegration", "https://get-books-proxy.myproxy.internal"),
             path="/login",
             methods=[apigwv2.HttpMethod.POST],
             authorizer=apigwv2.HttpNoneAuthorizer()
         )
     '''
 
     def __init__(self) -> None:
@@ -9485,26 +8748,26 @@
         jsii.create(self.__class__, self, [])
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
         *,
         route: "IHttpRoute",
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
     ) -> HttpRouteAuthorizerConfig:
         '''(experimental) Bind this authorizer to a specified Http route.
 
         :param route: (experimental) The route to which the authorizer is being bound.
         :param scope: (experimental) The scope for any constructs created as part of the bind.
 
         :stability: experimental
         '''
-        _options = HttpRouteAuthorizerBindOptions(route=route, scope=scope)
+        _ = HttpRouteAuthorizerBindOptions(route=route, scope=scope)
 
-        return typing.cast(HttpRouteAuthorizerConfig, jsii.invoke(self, "bind", [_options]))
+        return typing.cast(HttpRouteAuthorizerConfig, jsii.invoke(self, "bind", [_]))
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.HttpStageAttributes",
     jsii_struct_bases=[StageAttributes],
     name_mapping={"stage_name": "stageName", "api": "api"},
 )
@@ -9527,19 +8790,15 @@
             # http_api: apigatewayv2_alpha.HttpApi
             
             http_stage_attributes = apigatewayv2_alpha.HttpStageAttributes(
                 api=http_api,
                 stage_name="stageName"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__68b934e47d5c501cf4c24923fe5b089fdb197a5624c649d8f83e58305cd890d5)
-            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
-            check_type(argname="argument api", value=api, expected_type=type_hints["api"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "stage_name": stage_name,
             "api": api,
         }
 
     @builtins.property
     def stage_name(self) -> builtins.str:
         '''(experimental) The name of the stage.
@@ -9574,32 +8833,29 @@
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.HttpStageOptions",
     jsii_struct_bases=[StageOptions],
     name_mapping={
         "auto_deploy": "autoDeploy",
         "domain_mapping": "domainMapping",
-        "throttle": "throttle",
         "stage_name": "stageName",
     },
 )
 class HttpStageOptions(StageOptions):
     def __init__(
         self,
         *,
         auto_deploy: typing.Optional[builtins.bool] = None,
-        domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-        throttle: typing.Optional[typing.Union[ThrottleSettings, typing.Dict[builtins.str, typing.Any]]] = None,
+        domain_mapping: typing.Optional[DomainMappingOptions] = None,
         stage_name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) The options to create a new Stage for an HTTP API.
 
         :param auto_deploy: (experimental) Whether updates to an API automatically trigger a new deployment. Default: false
         :param domain_mapping: (experimental) The options for custom domain and api mapping. Default: - no custom domain and api mapping configuration
-        :param throttle: (experimental) Throttle settings for the routes of this stage. Default: - no throttling configuration
         :param stage_name: (experimental) The name of the stage. See ``StageName`` class for more details. Default: '$default' the default stage of the API. This stage will have the URL at the root of the API endpoint.
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
@@ -9615,29 +8871,19 @@
                     domain_name=dn,
                     mapping_key="bar"
                 )
             )
         '''
         if isinstance(domain_mapping, dict):
             domain_mapping = DomainMappingOptions(**domain_mapping)
-        if isinstance(throttle, dict):
-            throttle = ThrottleSettings(**throttle)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6e64c35e906d5449f8f7b3901603109565a527cbb27318f310243b054419c4a7)
-            check_type(argname="argument auto_deploy", value=auto_deploy, expected_type=type_hints["auto_deploy"])
-            check_type(argname="argument domain_mapping", value=domain_mapping, expected_type=type_hints["domain_mapping"])
-            check_type(argname="argument throttle", value=throttle, expected_type=type_hints["throttle"])
-            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if auto_deploy is not None:
             self._values["auto_deploy"] = auto_deploy
         if domain_mapping is not None:
             self._values["domain_mapping"] = domain_mapping
-        if throttle is not None:
-            self._values["throttle"] = throttle
         if stage_name is not None:
             self._values["stage_name"] = stage_name
 
     @builtins.property
     def auto_deploy(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Whether updates to an API automatically trigger a new deployment.
 
@@ -9656,25 +8902,14 @@
 
         :stability: experimental
         '''
         result = self._values.get("domain_mapping")
         return typing.cast(typing.Optional[DomainMappingOptions], result)
 
     @builtins.property
-    def throttle(self) -> typing.Optional[ThrottleSettings]:
-        '''(experimental) Throttle settings for the routes of this stage.
-
-        :default: - no throttling configuration
-
-        :stability: experimental
-        '''
-        result = self._values.get("throttle")
-        return typing.cast(typing.Optional[ThrottleSettings], result)
-
-    @builtins.property
     def stage_name(self) -> typing.Optional[builtins.str]:
         '''(experimental) The name of the stage.
 
         See ``StageName`` class for more details.
 
         :default: '$default' the default stage of the API. This stage will have the URL at the root of the API endpoint.
 
@@ -9697,34 +8932,31 @@
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.HttpStageProps",
     jsii_struct_bases=[HttpStageOptions],
     name_mapping={
         "auto_deploy": "autoDeploy",
         "domain_mapping": "domainMapping",
-        "throttle": "throttle",
         "stage_name": "stageName",
         "http_api": "httpApi",
     },
 )
 class HttpStageProps(HttpStageOptions):
     def __init__(
         self,
         *,
         auto_deploy: typing.Optional[builtins.bool] = None,
-        domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-        throttle: typing.Optional[typing.Union[ThrottleSettings, typing.Dict[builtins.str, typing.Any]]] = None,
+        domain_mapping: typing.Optional[DomainMappingOptions] = None,
         stage_name: typing.Optional[builtins.str] = None,
         http_api: IHttpApi,
     ) -> None:
         '''(experimental) Properties to initialize an instance of ``HttpStage``.
 
         :param auto_deploy: (experimental) Whether updates to an API automatically trigger a new deployment. Default: false
         :param domain_mapping: (experimental) The options for custom domain and api mapping. Default: - no custom domain and api mapping configuration
-        :param throttle: (experimental) Throttle settings for the routes of this stage. Default: - no throttling configuration
         :param stage_name: (experimental) The name of the stage. See ``StageName`` class for more details. Default: '$default' the default stage of the API. This stage will have the URL at the root of the API endpoint.
         :param http_api: (experimental) The HTTP API to which this stage is associated.
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
@@ -9735,32 +8967,21 @@
             apigwv2.HttpStage(self, "Stage",
                 http_api=api,
                 stage_name="beta"
             )
         '''
         if isinstance(domain_mapping, dict):
             domain_mapping = DomainMappingOptions(**domain_mapping)
-        if isinstance(throttle, dict):
-            throttle = ThrottleSettings(**throttle)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__925560a3ec43c8b350658e7729b7c093c0eb2dc51b442b9b5877c46ec328fbb4)
-            check_type(argname="argument auto_deploy", value=auto_deploy, expected_type=type_hints["auto_deploy"])
-            check_type(argname="argument domain_mapping", value=domain_mapping, expected_type=type_hints["domain_mapping"])
-            check_type(argname="argument throttle", value=throttle, expected_type=type_hints["throttle"])
-            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
-            check_type(argname="argument http_api", value=http_api, expected_type=type_hints["http_api"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "http_api": http_api,
         }
         if auto_deploy is not None:
             self._values["auto_deploy"] = auto_deploy
         if domain_mapping is not None:
             self._values["domain_mapping"] = domain_mapping
-        if throttle is not None:
-            self._values["throttle"] = throttle
         if stage_name is not None:
             self._values["stage_name"] = stage_name
 
     @builtins.property
     def auto_deploy(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Whether updates to an API automatically trigger a new deployment.
 
@@ -9779,25 +9000,14 @@
 
         :stability: experimental
         '''
         result = self._values.get("domain_mapping")
         return typing.cast(typing.Optional[DomainMappingOptions], result)
 
     @builtins.property
-    def throttle(self) -> typing.Optional[ThrottleSettings]:
-        '''(experimental) Throttle settings for the routes of this stage.
-
-        :default: - no throttling configuration
-
-        :stability: experimental
-        '''
-        result = self._values.get("throttle")
-        return typing.cast(typing.Optional[ThrottleSettings], result)
-
-    @builtins.property
     def stage_name(self) -> typing.Optional[builtins.str]:
         '''(experimental) The name of the stage.
 
         See ``StageName`` class for more details.
 
         :default: '$default' the default stage of the API. This stage will have the URL at the root of the API endpoint.
 
@@ -9831,35 +9041,35 @@
 @jsii.interface(jsii_type="@aws-cdk/aws-apigatewayv2-alpha.IHttpIntegration")
 class IHttpIntegration(IIntegration, typing_extensions.Protocol):
     '''(experimental) Represents an Integration for an HTTP API.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="httpApi")
     def http_api(self) -> IHttpApi:
         '''(experimental) The HTTP API associated with this integration.
 
         :stability: experimental
         '''
         ...
 
 
 class _IHttpIntegrationProxy(
-    jsii.proxy_for(IIntegration), # type: ignore[misc]
+    jsii.proxy_for(IIntegration) # type: ignore[misc]
 ):
     '''(experimental) Represents an Integration for an HTTP API.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IHttpIntegration"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="httpApi")
     def http_api(self) -> IHttpApi:
         '''(experimental) The HTTP API associated with this integration.
 
         :stability: experimental
         '''
         return typing.cast(IHttpApi, jsii.get(self, "httpApi"))
@@ -9871,145 +9081,142 @@
 @jsii.interface(jsii_type="@aws-cdk/aws-apigatewayv2-alpha.IHttpRoute")
 class IHttpRoute(IRoute, typing_extensions.Protocol):
     '''(experimental) Represents a Route for an HTTP API.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="httpApi")
     def http_api(self) -> IHttpApi:
         '''(experimental) The HTTP API associated with this route.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="routeArn")
     def route_arn(self) -> builtins.str:
         '''(experimental) Returns the arn of the route.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="path")
     def path(self) -> typing.Optional[builtins.str]:
         '''(experimental) Returns the path component of this HTTP route, ``undefined`` if the path is the catch-all route.
 
         :stability: experimental
         '''
         ...
 
     @jsii.member(jsii_name="grantInvoke")
     def grant_invoke(
         self,
-        grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
+        grantee: aws_cdk.aws_iam.IGrantable,
         *,
         http_methods: typing.Optional[typing.Sequence[HttpMethod]] = None,
-    ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
+    ) -> aws_cdk.aws_iam.Grant:
         '''(experimental) Grant access to invoke the route.
 
         This method requires that the authorizer of the route is undefined or is
         an ``HttpIamAuthorizer``.
 
         :param grantee: -
         :param http_methods: (experimental) The HTTP methods to allow. Default: - the HttpMethod of the route
 
         :stability: experimental
         '''
         ...
 
 
 class _IHttpRouteProxy(
-    jsii.proxy_for(IRoute), # type: ignore[misc]
+    jsii.proxy_for(IRoute) # type: ignore[misc]
 ):
     '''(experimental) Represents a Route for an HTTP API.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IHttpRoute"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="httpApi")
     def http_api(self) -> IHttpApi:
         '''(experimental) The HTTP API associated with this route.
 
         :stability: experimental
         '''
         return typing.cast(IHttpApi, jsii.get(self, "httpApi"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="routeArn")
     def route_arn(self) -> builtins.str:
         '''(experimental) Returns the arn of the route.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "routeArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="path")
     def path(self) -> typing.Optional[builtins.str]:
         '''(experimental) Returns the path component of this HTTP route, ``undefined`` if the path is the catch-all route.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "path"))
 
     @jsii.member(jsii_name="grantInvoke")
     def grant_invoke(
         self,
-        grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
+        grantee: aws_cdk.aws_iam.IGrantable,
         *,
         http_methods: typing.Optional[typing.Sequence[HttpMethod]] = None,
-    ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
+    ) -> aws_cdk.aws_iam.Grant:
         '''(experimental) Grant access to invoke the route.
 
         This method requires that the authorizer of the route is undefined or is
         an ``HttpIamAuthorizer``.
 
         :param grantee: -
         :param http_methods: (experimental) The HTTP methods to allow. Default: - the HttpMethod of the route
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e68d78a6fdd2cf02aa0a9db3e16ddc620002125429503856eb2206ca6638a462)
-            check_type(argname="argument grantee", value=grantee, expected_type=type_hints["grantee"])
         options = GrantInvokeOptions(http_methods=http_methods)
 
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.Grant, jsii.invoke(self, "grantInvoke", [grantee, options]))
+        return typing.cast(aws_cdk.aws_iam.Grant, jsii.invoke(self, "grantInvoke", [grantee, options]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IHttpRoute).__jsii_proxy_class__ = lambda : _IHttpRouteProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-apigatewayv2-alpha.IHttpStage")
 class IHttpStage(IStage, typing_extensions.Protocol):
     '''(experimental) Represents the HttpStage.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="api")
     def api(self) -> IHttpApi:
         '''(experimental) The API this stage is associated to.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="domainUrl")
     def domain_url(self) -> builtins.str:
         '''(experimental) The custom domain URL to this stage.
 
         :stability: experimental
         '''
         ...
@@ -10018,28 +9225,28 @@
     def metric_client_error(
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
         '''(experimental) Metric for the number of client-side errors captured in a given period.
 
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
 
         :default: - sum over 5 minutes
 
         :stability: experimental
         '''
         ...
@@ -10048,28 +9255,28 @@
     def metric_count(
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
         '''(experimental) Metric for the total number API requests in a given period.
 
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
 
         :default: - SampleCount over 5 minutes
 
         :stability: experimental
         '''
         ...
@@ -10078,28 +9285,28 @@
     def metric_data_processed(
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
         '''(experimental) Metric for the amount of data processed in bytes.
 
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
 
         :default: - sum over 5 minutes
 
         :stability: experimental
         '''
         ...
@@ -10108,28 +9315,28 @@
     def metric_integration_latency(
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
         '''(experimental) Metric for the time between when API Gateway relays a request to the backend and when it receives a response from the backend.
 
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
 
         :default: - no statistic
 
         :stability: experimental
         '''
         ...
@@ -10138,30 +9345,30 @@
     def metric_latency(
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
         '''(experimental) The time between when API Gateway receives a request from a client and when it returns a response to the client.
 
         The latency includes the integration latency and other API Gateway overhead.
 
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
 
         :default: - no statistic
 
         :stability: experimental
         '''
         ...
@@ -10170,57 +9377,57 @@
     def metric_server_error(
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
         '''(experimental) Metric for the number of server-side errors captured in a given period.
 
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
 
         :default: - sum over 5 minutes
 
         :stability: experimental
         '''
         ...
 
 
 class _IHttpStageProxy(
-    jsii.proxy_for(IStage), # type: ignore[misc]
+    jsii.proxy_for(IStage) # type: ignore[misc]
 ):
     '''(experimental) Represents the HttpStage.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-apigatewayv2-alpha.IHttpStage"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="api")
     def api(self) -> IHttpApi:
         '''(experimental) The API this stage is associated to.
 
         :stability: experimental
         '''
         return typing.cast(IHttpApi, jsii.get(self, "api"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="domainUrl")
     def domain_url(self) -> builtins.str:
         '''(experimental) The custom domain URL to this stage.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "domainUrl"))
@@ -10229,261 +9436,261 @@
     def metric_client_error(
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
         '''(experimental) Metric for the number of client-side errors captured in a given period.
 
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
 
         :default: - sum over 5 minutes
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricClientError", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricClientError", [props]))
 
     @jsii.member(jsii_name="metricCount")
     def metric_count(
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
         '''(experimental) Metric for the total number API requests in a given period.
 
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
 
         :default: - SampleCount over 5 minutes
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricCount", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricCount", [props]))
 
     @jsii.member(jsii_name="metricDataProcessed")
     def metric_data_processed(
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
         '''(experimental) Metric for the amount of data processed in bytes.
 
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
 
         :default: - sum over 5 minutes
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricDataProcessed", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricDataProcessed", [props]))
 
     @jsii.member(jsii_name="metricIntegrationLatency")
     def metric_integration_latency(
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
         '''(experimental) Metric for the time between when API Gateway relays a request to the backend and when it receives a response from the backend.
 
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
 
         :default: - no statistic
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricIntegrationLatency", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricIntegrationLatency", [props]))
 
     @jsii.member(jsii_name="metricLatency")
     def metric_latency(
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
         '''(experimental) The time between when API Gateway receives a request from a client and when it returns a response to the client.
 
         The latency includes the integration latency and other API Gateway overhead.
 
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
 
         :default: - no statistic
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricLatency", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricLatency", [props]))
 
     @jsii.member(jsii_name="metricServerError")
     def metric_server_error(
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
         '''(experimental) Metric for the number of server-side errors captured in a given period.
 
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
 
         :default: - sum over 5 minutes
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricServerError", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricServerError", [props]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IHttpStage).__jsii_proxy_class__ = lambda : _IHttpStageProxy
 
 
 @jsii.implements(IHttpIntegration)
 class HttpIntegration(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.HttpIntegration",
 ):
     '''(experimental) The integration for an API route.
 
     :stability: experimental
     :resource: AWS::ApiGatewayV2::Integration
@@ -10515,15 +9722,15 @@
             payload_format_version=payload_format_version,
             secure_server_name="secureServerName"
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         http_api: IHttpApi,
         integration_type: HttpIntegrationType,
         connection_id: typing.Optional[builtins.str] = None,
         connection_type: typing.Optional[HttpConnectionType] = None,
         credentials: typing.Optional[IntegrationCredentials] = None,
@@ -10547,18 +9754,14 @@
         :param method: (experimental) The HTTP method to use when calling the underlying HTTP proxy. Default: - none. required if the integration type is ``HttpIntegrationType.HTTP_PROXY``.
         :param parameter_mapping: (experimental) Specifies how to transform HTTP requests before sending them to the backend. Default: undefined requests are sent to the backend unmodified
         :param payload_format_version: (experimental) The version of the payload format. Default: - defaults to latest in the case of HttpIntegrationType.AWS_PROXY`, irrelevant otherwise.
         :param secure_server_name: (experimental) Specifies the TLS configuration for a private integration. Default: undefined private integration traffic will use HTTP protocol
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3de74d25b3d7d1e17696a2da7bd0666d13d0467eed87993389dc688e2ffcf281)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = HttpIntegrationProps(
             http_api=http_api,
             integration_type=integration_type,
             connection_id=connection_id,
             connection_type=connection_type,
             credentials=credentials,
             integration_subtype=integration_subtype,
@@ -10567,36 +9770,36 @@
             parameter_mapping=parameter_mapping,
             payload_format_version=payload_format_version,
             secure_server_name=secure_server_name,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="httpApi")
     def http_api(self) -> IHttpApi:
         '''(experimental) The HTTP API associated with this integration.
 
         :stability: experimental
         '''
         return typing.cast(IHttpApi, jsii.get(self, "httpApi"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="integrationId")
     def integration_id(self) -> builtins.str:
         '''(experimental) Id of the integration.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "integrationId"))
 
 
 @jsii.implements(IHttpRoute)
 class HttpRoute(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.HttpRoute",
 ):
     '''(experimental) Route class that creates the Route for API Gateway HTTP API.
 
     :stability: experimental
     :resource: AWS::ApiGatewayV2::Route
@@ -10622,15 +9825,15 @@
             authorization_scopes=["authorizationScopes"],
             authorizer=http_route_authorizer
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         http_api: IHttpApi,
         route_key: HttpRouteKey,
         authorization_scopes: typing.Optional[typing.Sequence[builtins.str]] = None,
         authorizer: typing.Optional[IHttpRouteAuthorizer] = None,
         integration: HttpRouteIntegration,
@@ -10642,493 +9845,472 @@
         :param route_key: (experimental) The key to this route. This is a combination of an HTTP method and an HTTP path.
         :param authorization_scopes: (experimental) The list of OIDC scopes to include in the authorization. These scopes will be merged with the scopes from the attached authorizer Default: - no additional authorization scopes
         :param authorizer: (experimental) Authorizer for a WebSocket API or an HTTP API. Default: - No authorizer
         :param integration: (experimental) The integration to be configured on this route.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d456143a18e04fab72c125ff49f83adf6625ae62b417322c1724ded4c91eeb7d)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = HttpRouteProps(
             http_api=http_api,
             route_key=route_key,
             authorization_scopes=authorization_scopes,
             authorizer=authorizer,
             integration=integration,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @jsii.member(jsii_name="grantInvoke")
     def grant_invoke(
         self,
-        grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
+        grantee: aws_cdk.aws_iam.IGrantable,
         *,
         http_methods: typing.Optional[typing.Sequence[HttpMethod]] = None,
-    ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
+    ) -> aws_cdk.aws_iam.Grant:
         '''(experimental) Grant access to invoke the route.
 
         This method requires that the authorizer of the route is undefined or is
         an ``HttpIamAuthorizer``.
 
         :param grantee: -
         :param http_methods: (experimental) The HTTP methods to allow. Default: - the HttpMethod of the route
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__53257a740a0bf9e3076f5e9960cdc2b0c474378d558e854838154ba2bd8034cf)
-            check_type(argname="argument grantee", value=grantee, expected_type=type_hints["grantee"])
         options = GrantInvokeOptions(http_methods=http_methods)
 
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.Grant, jsii.invoke(self, "grantInvoke", [grantee, options]))
+        return typing.cast(aws_cdk.aws_iam.Grant, jsii.invoke(self, "grantInvoke", [grantee, options]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="httpApi")
     def http_api(self) -> IHttpApi:
         '''(experimental) The HTTP API associated with this route.
 
         :stability: experimental
         '''
         return typing.cast(IHttpApi, jsii.get(self, "httpApi"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="routeArn")
     def route_arn(self) -> builtins.str:
         '''(experimental) Returns the arn of the route.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "routeArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="routeId")
     def route_id(self) -> builtins.str:
         '''(experimental) Id of the Route.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "routeId"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="path")
     def path(self) -> typing.Optional[builtins.str]:
         '''(experimental) Returns the path component of this HTTP route, ``undefined`` if the path is the catch-all route.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "path"))
 
 
 @jsii.implements(IHttpStage, IStage)
 class HttpStage(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-alpha.HttpStage",
 ):
     '''(experimental) Represents a stage where an instance of the API is deployed.
 
     :stability: experimental
-    :resource: AWS::ApiGatewayV2::Stage
     :exampleMetadata: infused
+    :resource: AWS::ApiGatewayV2::Stage
 
     Example::
 
         # api: apigwv2.HttpApi
         
         
         apigwv2.HttpStage(self, "Stage",
             http_api=api,
             stage_name="beta"
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         http_api: IHttpApi,
         stage_name: typing.Optional[builtins.str] = None,
         auto_deploy: typing.Optional[builtins.bool] = None,
-        domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-        throttle: typing.Optional[typing.Union[ThrottleSettings, typing.Dict[builtins.str, typing.Any]]] = None,
+        domain_mapping: typing.Optional[DomainMappingOptions] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param http_api: (experimental) The HTTP API to which this stage is associated.
         :param stage_name: (experimental) The name of the stage. See ``StageName`` class for more details. Default: '$default' the default stage of the API. This stage will have the URL at the root of the API endpoint.
         :param auto_deploy: (experimental) Whether updates to an API automatically trigger a new deployment. Default: false
         :param domain_mapping: (experimental) The options for custom domain and api mapping. Default: - no custom domain and api mapping configuration
-        :param throttle: (experimental) Throttle settings for the routes of this stage. Default: - no throttling configuration
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ed92fb335fa6855175afbb033d45447922cc6911de5d516e1c4dd76351a72aa1)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = HttpStageProps(
             http_api=http_api,
             stage_name=stage_name,
             auto_deploy=auto_deploy,
             domain_mapping=domain_mapping,
-            throttle=throttle,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromHttpStageAttributes")
+    @jsii.member(jsii_name="fromHttpStageAttributes") # type: ignore[misc]
     @builtins.classmethod
     def from_http_stage_attributes(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         api: IHttpApi,
         stage_name: builtins.str,
     ) -> IHttpStage:
         '''(experimental) Import an existing stage into this CDK app.
 
         :param scope: -
         :param id: -
         :param api: (experimental) The API to which this stage is associated.
         :param stage_name: (experimental) The name of the stage.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__456b0db547449fda45bdfda459b2a51921656ff642e3c234362965315dbd5cd5)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         attrs = HttpStageAttributes(api=api, stage_name=stage_name)
 
         return typing.cast(IHttpStage, jsii.sinvoke(cls, "fromHttpStageAttributes", [scope, id, attrs]))
 
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
         '''(experimental) Return the given named metric for this HTTP Api Gateway Stage.
 
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
-            type_hints = typing.get_type_hints(_typecheckingstub__13222b5ec0bde39f747497ef32fa2559d2b7146ce09903ba475536fb3869b080)
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
 
     @jsii.member(jsii_name="metricClientError")
     def metric_client_error(
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
         '''(experimental) Metric for the number of client-side errors captured in a given period.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricClientError", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricClientError", [props]))
 
     @jsii.member(jsii_name="metricCount")
     def metric_count(
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
         '''(experimental) Metric for the total number API requests in a given period.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricCount", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricCount", [props]))
 
     @jsii.member(jsii_name="metricDataProcessed")
     def metric_data_processed(
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
         '''(experimental) Metric for the amount of data processed in bytes.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricDataProcessed", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricDataProcessed", [props]))
 
     @jsii.member(jsii_name="metricIntegrationLatency")
     def metric_integration_latency(
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
         '''(experimental) Metric for the time between when API Gateway relays a request to the backend and when it receives a response from the backend.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricIntegrationLatency", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricIntegrationLatency", [props]))
 
     @jsii.member(jsii_name="metricLatency")
     def metric_latency(
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
         '''(experimental) The time between when API Gateway receives a request from a client and when it returns a response to the client.
 
         The latency includes the integration latency and other API Gateway overhead.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricLatency", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricLatency", [props]))
 
     @jsii.member(jsii_name="metricServerError")
     def metric_server_error(
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
         '''(experimental) Metric for the number of server-side errors captured in a given period.
 
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
 
-        return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.Metric, jsii.invoke(self, "metricServerError", [props]))
+        return typing.cast(aws_cdk.aws_cloudwatch.Metric, jsii.invoke(self, "metricServerError", [props]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="api")
     def api(self) -> IHttpApi:
         '''(experimental) The API this stage is associated to.
 
         :stability: experimental
         '''
         return typing.cast(IHttpApi, jsii.get(self, "api"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="baseApi")
     def _base_api(self) -> IApi:
         '''
         :stability: experimental
         '''
         return typing.cast(IApi, jsii.get(self, "baseApi"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="domainUrl")
     def domain_url(self) -> builtins.str:
         '''(experimental) The custom domain URL to this stage.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "domainUrl"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="stageName")
     def stage_name(self) -> builtins.str:
         '''(experimental) The name of the stage;
 
         its primary identifier.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "stageName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="url")
     def url(self) -> builtins.str:
         '''(experimental) The URL to this stage.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "url"))
@@ -11201,20 +10383,18 @@
     "MTLSConfig",
     "MappingValue",
     "ParameterMapping",
     "PayloadFormatVersion",
     "SecurityPolicy",
     "StageAttributes",
     "StageOptions",
-    "ThrottleSettings",
     "VpcLink",
     "VpcLinkAttributes",
     "VpcLinkProps",
     "WebSocketApi",
-    "WebSocketApiAttributes",
     "WebSocketApiKeySelectionExpression",
     "WebSocketApiProps",
     "WebSocketAuthorizer",
     "WebSocketAuthorizerAttributes",
     "WebSocketAuthorizerProps",
     "WebSocketAuthorizerType",
     "WebSocketIntegration",
@@ -11231,989 +10411,7 @@
     "WebSocketRouteProps",
     "WebSocketStage",
     "WebSocketStageAttributes",
     "WebSocketStageProps",
 ]
 
 publication.publish()
-
-def _typecheckingstub__742c0d28ff28876a0bc0d1152ef7b3343151f193a0e128ba64a6cbc4509c8f05(
-    *,
-    api_mapping_id: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__75ffb83f83ec42f2a0382885c05d069ecb32c50d82d796df38b991d84782ded6(
-    *,
-    api: IApi,
-    domain_name: IDomainName,
-    api_mapping_key: typing.Optional[builtins.str] = None,
-    stage: typing.Optional[IStage] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__dd6be8693e2cd2875856654344853bc620de9c6dd3e82fbd384cba9b5468a36d(
-    *,
-    integration: HttpRouteIntegration,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a8623074d52aadb0b4dc416f52273d5e1695739d7da72a818e4a16b0988313fa(
-    *,
-    allow_credentials: typing.Optional[builtins.bool] = None,
-    allow_headers: typing.Optional[typing.Sequence[builtins.str]] = None,
-    allow_methods: typing.Optional[typing.Sequence[CorsHttpMethod]] = None,
-    allow_origins: typing.Optional[typing.Sequence[builtins.str]] = None,
-    expose_headers: typing.Optional[typing.Sequence[builtins.str]] = None,
-    max_age: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b9c022929eefc93f95859e1c88a0b0f15538c5b557fbe539653100b894c61520(
-    *,
-    domain_name: IDomainName,
-    mapping_key: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e3a28ea7d17c0cb32594b624176b2b5339560671719297d538c51a793079d6f8(
-    *,
-    name: builtins.str,
-    regional_domain_name: builtins.str,
-    regional_hosted_zone_id: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0a18b13421aac912723b2ab35f8a14b008971c520719c36b6764e8ff2bd43194(
-    *,
-    certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
-    certificate_name: typing.Optional[builtins.str] = None,
-    endpoint_type: typing.Optional[EndpointType] = None,
-    ownership_certificate: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
-    security_policy: typing.Optional[SecurityPolicy] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a82686daa9fd8d0f3123464a3edac12340e9f588999872022e157589c9935c8a(
-    *,
-    http_methods: typing.Optional[typing.Sequence[HttpMethod]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__ca86693c779a127085f398e4f4b28effbcaffb7b0e4c3586085ba8720c18c3b6(
-    *,
-    http_api_id: builtins.str,
-    api_endpoint: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__61f68792e068176f35bfd5b9b8d36c51601ad6882e6aa3ce1c951683b5d199d2(
-    *,
-    api_name: typing.Optional[builtins.str] = None,
-    cors_preflight: typing.Optional[typing.Union[CorsPreflightOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    create_default_stage: typing.Optional[builtins.bool] = None,
-    default_authorization_scopes: typing.Optional[typing.Sequence[builtins.str]] = None,
-    default_authorizer: typing.Optional[IHttpRouteAuthorizer] = None,
-    default_domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    default_integration: typing.Optional[HttpRouteIntegration] = None,
-    description: typing.Optional[builtins.str] = None,
-    disable_execute_api_endpoint: typing.Optional[builtins.bool] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e213cc5ff1a6a50f727adfa1a93746afabbb568dc170da0d58f5c5f6b4a65877(
-    *,
-    authorizer_id: builtins.str,
-    authorizer_type: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__270c2096601be45fba89ecb508234f5870eaabd6d21813bc090ce9b1a459264d(
-    *,
-    http_api: IHttpApi,
-    identity_source: typing.Sequence[builtins.str],
-    type: HttpAuthorizerType,
-    authorizer_name: typing.Optional[builtins.str] = None,
-    authorizer_uri: typing.Optional[builtins.str] = None,
-    enable_simple_responses: typing.Optional[builtins.bool] = None,
-    jwt_audience: typing.Optional[typing.Sequence[builtins.str]] = None,
-    jwt_issuer: typing.Optional[builtins.str] = None,
-    payload_format_version: typing.Optional[AuthorizerPayloadVersion] = None,
-    results_cache_ttl: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0e70b5fc9ef16c84251eedf90fb9f4578a5231e285c86d485055a9875610b863(
-    *,
-    http_api: IHttpApi,
-    integration_type: HttpIntegrationType,
-    connection_id: typing.Optional[builtins.str] = None,
-    connection_type: typing.Optional[HttpConnectionType] = None,
-    credentials: typing.Optional[IntegrationCredentials] = None,
-    integration_subtype: typing.Optional[HttpIntegrationSubtype] = None,
-    integration_uri: typing.Optional[builtins.str] = None,
-    method: typing.Optional[HttpMethod] = None,
-    parameter_mapping: typing.Optional[ParameterMapping] = None,
-    payload_format_version: typing.Optional[PayloadFormatVersion] = None,
-    secure_server_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__327eab42c70e54708c05239cc92e1d413d8f439a24b6448c6de2d0f2d4df7521(
-    *,
-    route: IHttpRoute,
-    scope: _constructs_77d1e7e8.Construct,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__23fa1130cc8cec3f96c4c7be76f4fde0189dfa2fd6410ede8be1c8e24a88a0f2(
-    *,
-    authorization_type: builtins.str,
-    authorization_scopes: typing.Optional[typing.Sequence[builtins.str]] = None,
-    authorizer_id: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0d2d16b160325ee41bba7780d2678d810d12da5f663f886f5c8a810a06c66fef(
-    id: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__fee001518b0d0335530b5174be6d0d04745ad94a5bffe05a6d9007712a52eb52(
-    *,
-    route: IHttpRoute,
-    scope: _constructs_77d1e7e8.Construct,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__8d07656a3841a48dd4643d0e10742dee8735d4fa1b6dec4e77afe67a3c12f2dd(
-    *,
-    payload_format_version: PayloadFormatVersion,
-    type: HttpIntegrationType,
-    connection_id: typing.Optional[builtins.str] = None,
-    connection_type: typing.Optional[HttpConnectionType] = None,
-    credentials: typing.Optional[IntegrationCredentials] = None,
-    method: typing.Optional[HttpMethod] = None,
-    parameter_mapping: typing.Optional[ParameterMapping] = None,
-    secure_server_name: typing.Optional[builtins.str] = None,
-    subtype: typing.Optional[HttpIntegrationSubtype] = None,
-    uri: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__757949aa83516e4dc3de82eaf70c9ec58058087715b274d9a080b33530b01213(
-    path: builtins.str,
-    method: typing.Optional[HttpMethod] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a43a4a903025b4c98824c40d09ba7a3ec865a0a5902fb4f311846b446c460133(
-    *,
-    integration: HttpRouteIntegration,
-    http_api: IHttpApi,
-    route_key: HttpRouteKey,
-    authorization_scopes: typing.Optional[typing.Sequence[builtins.str]] = None,
-    authorizer: typing.Optional[IHttpRouteAuthorizer] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__c475fcfbd8ec2d43f9f067afa8d49c21d334d5c85f25834be833f0c107d99e8e(
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
-def _typecheckingstub__d6eea31b2ea3d8439d0d065d266b0097b8fd2775bebde3b5b7cfc484683aa34a(
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
-def _typecheckingstub__102c1a776427fd4c0938e5abf575144e45fdb236c63258f1da261499f33717f0(
-    role: _aws_cdk_aws_iam_ceddda9d.IRole,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__38e19f865daecac4e9c0b7840b549ee7e3e17328107146b6aeed11be416a4830(
-    *,
-    bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
-    key: builtins.str,
-    version: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__214070b3203c10af4bde0b28ed256ac9a4d24597f026dd0b0cc830dd88c3212d(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__4af933305aeacd390d336f32a5829afa054de657121385d6ec7753a9ea26d601(
-    variable_name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__4ea57d3eb4bcfb04e995828dff02ab6f0787305f407450d33b5272726fe121ba(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__fd491365abe2954925b1f433ba7521a56e4bbc0bcdfddd61b667ca4f13903681(
-    name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e720451078130f0098a0b48416451612a00e6befa0c802ff75a2b864085649a5(
-    name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__69c384039069eb05e230de4bc9ac53925e0d361bd038ed0a3b02e073b1525c71(
-    name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b36b16773b8a1c554f9a57b9e3d7a3722f155a3d65b1a10b4204ac3f1740616a(
-    name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b3602fe53f550a6f339115089310b50937eb494d182495b9b3787a639c5dcaed(
-    variable_name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__c8181ef9cc8308f9477f0a1caad591787ed40d80e9353a4ab806411f93450058(
-    obj: typing.Mapping[builtins.str, MappingValue],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__56ae57cc9968fa2fd30ad1d66784260b0e784ac1e0ae80923fa737f9a8ada22a(
-    name: builtins.str,
-    value: MappingValue,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__4f855f9472042f201eb931ccc90ac6f72c3684fdf5485ee6979662f843ed27cc(
-    name: builtins.str,
-    value: MappingValue,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__ea27856048c8e84cddc832b14d9115403f2b80ce39008d1d2a456c126be689c6(
-    key: builtins.str,
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0bbf5124407bf24ea9fa7d17aa1565a5ed9210655f4f602da854ad14a24db0d5(
-    name: builtins.str,
-    value: MappingValue,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__3969677f031f21644ed17215886d65e2445e67dcf22241b2a6150248c6192f36(
-    value: MappingValue,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e75c515536f95796a2a8f985b00f7829f0664a04b9a30bed03ea9ad1ce892d91(
-    name: builtins.str,
-    value: MappingValue,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__48411845428e2e72182038805ca1f55aa523a254158b3148ec49d4ee874decc5(
-    name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__46e584a752980831919a8156516ab93f44fb1a783b5798270ff450fdc6bc50d2(
-    name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__650e7e8cf5095b5caf036d1cdfea61cdc50d05db4e0b82311e5988ab562c7508(
-    version: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b7bc86d60b044b6ce8b75e1e701218c18bc2ca9ef7cc2a9667e4858066891f46(
-    *,
-    stage_name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a32c0806cbd09e57e1b6cb67e4b59ac7fdd424ef31f824f2caeda822945dbf65(
-    *,
-    auto_deploy: typing.Optional[builtins.bool] = None,
-    domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    throttle: typing.Optional[typing.Union[ThrottleSettings, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__4ad556ef4d84d522901264cb64a96b656171558870186a72f596567dc19746a2(
-    *,
-    burst_limit: typing.Optional[jsii.Number] = None,
-    rate_limit: typing.Optional[jsii.Number] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a7e5cf8ebb393b1b711349f32ce6a5d91c23aa92cb3f1a5fb324d1ace8fa39e5(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-    subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
-    vpc_link_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__d1b73cd3902808dcd9cedbbb002791b3c0b71ecf07dc9ee537153e45a37de0b7(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-    vpc_link_id: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__fb1536c4a56444b87ed12cf12ec84dcad1aeea01af7e687ab6bc5440355e7e11(
-    *groups: _aws_cdk_aws_ec2_ceddda9d.ISecurityGroup,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0b26d604e4ca1a2688579e0987cdb68ab389de0e4b8cb68e274ece105bdd03cf(
-    *subnets: _aws_cdk_aws_ec2_ceddda9d.ISubnet,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b806190a5cb732ad4de67d21bd895caa64bb12248a0d0ab31634597e02c8057e(
-    *,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-    vpc_link_id: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__9aed9118f19188de6967aa0373708cfcd4ffb3d828b567d6cbc01404c7aa6581(
-    *,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
-    subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
-    vpc_link_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__1178cce7f52c6ba72b835087f977643630d7f0c2665b967ecfee0bfe59093cb6(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    api_key_selection_expression: typing.Optional[WebSocketApiKeySelectionExpression] = None,
-    api_name: typing.Optional[builtins.str] = None,
-    connect_route_options: typing.Optional[typing.Union[WebSocketRouteOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    default_route_options: typing.Optional[typing.Union[WebSocketRouteOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    description: typing.Optional[builtins.str] = None,
-    disconnect_route_options: typing.Optional[typing.Union[WebSocketRouteOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    route_selection_expression: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__53d1a9fe1fdf41c0b5a739761d4875fb19c206a09c26c51425f989503e6b976b(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    web_socket_id: builtins.str,
-    api_endpoint: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b3fea69a2469b346680a0c3465ad0d8edf75af46ec799894b3faabfa5c26ec77(
-    route_key: builtins.str,
-    *,
-    integration: WebSocketRouteIntegration,
-    authorizer: typing.Optional[IWebSocketRouteAuthorizer] = None,
-    return_response: typing.Optional[builtins.bool] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__3519e657dc5ef6b61e34eb3fc9f6d114f2ebbf762f5ca278412f276b78b73bd7(
-    identity: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__25c26b71a707cd073d476cfe86d40884d0adc369830b3b667bfcc8d3d5069fe3(
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
-def _typecheckingstub__ae0c8df0ca0e715101942e90c3ba6802a24a7d17b7ccaf420c2de7498d0f3110(
-    *,
-    web_socket_id: builtins.str,
-    api_endpoint: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__34791e0880629c49a9f044c4e76a43e531d8704f81a7f9c57e446e0f8af0541c(
-    custom_api_key_selector: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__92cd23b712e91b17d8d403f5d44376505198f2e4d79f2370e3ce6a05ea6ddc2a(
-    *,
-    api_key_selection_expression: typing.Optional[WebSocketApiKeySelectionExpression] = None,
-    api_name: typing.Optional[builtins.str] = None,
-    connect_route_options: typing.Optional[typing.Union[WebSocketRouteOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    default_route_options: typing.Optional[typing.Union[WebSocketRouteOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    description: typing.Optional[builtins.str] = None,
-    disconnect_route_options: typing.Optional[typing.Union[WebSocketRouteOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    route_selection_expression: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__f24f7e7421170c9759c052f1d385a1f7e94dbd5eb18e0b47be9cab3ee8826990(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    identity_source: typing.Sequence[builtins.str],
-    type: WebSocketAuthorizerType,
-    web_socket_api: IWebSocketApi,
-    authorizer_name: typing.Optional[builtins.str] = None,
-    authorizer_uri: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e383ace2ee0471b5314c8dcb5e8b4c903443f7f45d06e85ce1160c2494ade7c3(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    authorizer_id: builtins.str,
-    authorizer_type: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__ec6cd687f35d4560bc6ed8b97968247261b8e88313cf6380b0c261222b1d373c(
-    *,
-    authorizer_id: builtins.str,
-    authorizer_type: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e02c909494ad68823621decb1cf4f3c9d5a9383ba2429deace659f406a376cde(
-    *,
-    identity_source: typing.Sequence[builtins.str],
-    type: WebSocketAuthorizerType,
-    web_socket_api: IWebSocketApi,
-    authorizer_name: typing.Optional[builtins.str] = None,
-    authorizer_uri: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__870fc94d82010681246ecba710a6ed2fbd784a22488897490747220c5a9bb1a9(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    integration_type: WebSocketIntegrationType,
-    integration_uri: builtins.str,
-    web_socket_api: IWebSocketApi,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__809d7a61872d8b86104362e83bf279e0275cab4ee56d78bb981f42a476435905(
-    *,
-    integration_type: WebSocketIntegrationType,
-    integration_uri: builtins.str,
-    web_socket_api: IWebSocketApi,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__89ed8dea5fd2abdd3d7348cec8375728ea8c56911ab73c2e7661f42936a36951(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    route_key: builtins.str,
-    web_socket_api: IWebSocketApi,
-    api_key_required: typing.Optional[builtins.bool] = None,
-    integration: WebSocketRouteIntegration,
-    authorizer: typing.Optional[IWebSocketRouteAuthorizer] = None,
-    return_response: typing.Optional[builtins.bool] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__fccd4465748920ec078ce3c095e6d5997201164b60c9937b341677d4bed18d2d(
-    *,
-    route: IWebSocketRoute,
-    scope: _constructs_77d1e7e8.Construct,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__31b7978ca3879b28e59655ad191a6a2a4b1f15e48c662e792f29609537418e7b(
-    *,
-    authorization_type: builtins.str,
-    authorizer_id: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__c197ca72497cd4c42d540f6e0560e6883980b3d825f1228e227525877aff3ac4(
-    id: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a9af6c9ac36dba4ed1e02e99de4fc973a26bd4423e8609681f9bddbf43144cd7(
-    *,
-    route: IWebSocketRoute,
-    scope: _constructs_77d1e7e8.Construct,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__d9151ff6a777a4992f010dc6dd1747375682b7a6c0d45bfbda07ab180448bf7f(
-    *,
-    type: WebSocketIntegrationType,
-    uri: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__015136d7cb99d78ecaebab742d43a14edcb81e619d7967b3b64eaf687c0d9ee3(
-    *,
-    integration: WebSocketRouteIntegration,
-    authorizer: typing.Optional[IWebSocketRouteAuthorizer] = None,
-    return_response: typing.Optional[builtins.bool] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__16bac6f0c09166c97608a842bf64940ba77c4a2c9803f76985adfdc50657856b(
-    *,
-    integration: WebSocketRouteIntegration,
-    authorizer: typing.Optional[IWebSocketRouteAuthorizer] = None,
-    return_response: typing.Optional[builtins.bool] = None,
-    route_key: builtins.str,
-    web_socket_api: IWebSocketApi,
-    api_key_required: typing.Optional[builtins.bool] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__48af0e7d3ce9ece527270c25928990cf8b605f1e3585927c1afcc3ffef087cf6(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    stage_name: builtins.str,
-    web_socket_api: IWebSocketApi,
-    auto_deploy: typing.Optional[builtins.bool] = None,
-    domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    throttle: typing.Optional[typing.Union[ThrottleSettings, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__96d2e4a524a0487b6a3e41257302724f03ec2dea315215c2348c1e882d82a509(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    api: IWebSocketApi,
-    stage_name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__385987aac133337ee8f5f880408bf66af8f3e3a5651bc827a3bc5af110334a17(
-    identity: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b080276ad15c8223193f7ed4fefbc76be9f47841814221e9a4dee06286100c93(
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
-def _typecheckingstub__3e391865a4ae4984a049207c6b5c3768117999fb528b5847ca1a6c7c35d2f82b(
-    *,
-    stage_name: builtins.str,
-    api: IWebSocketApi,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__782ab449d8fa4cf0a46fbab6526bdc241efef3893414586af02c8f715748ee2a(
-    *,
-    auto_deploy: typing.Optional[builtins.bool] = None,
-    domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    throttle: typing.Optional[typing.Union[ThrottleSettings, typing.Dict[builtins.str, typing.Any]]] = None,
-    stage_name: builtins.str,
-    web_socket_api: IWebSocketApi,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__ca8141f667bdde01ab0100d57a58a21f4b9acc231a1bbfb55a1925c258a680c6(
-    *,
-    integration: HttpRouteIntegration,
-    path: builtins.str,
-    authorization_scopes: typing.Optional[typing.Sequence[builtins.str]] = None,
-    authorizer: typing.Optional[IHttpRouteAuthorizer] = None,
-    methods: typing.Optional[typing.Sequence[HttpMethod]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__cbff8656b4f6706b46963d8d04c49514410f8af75cfeb33a4c2fe1a07e9f33ac(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    api: IApi,
-    domain_name: IDomainName,
-    api_mapping_key: typing.Optional[builtins.str] = None,
-    stage: typing.Optional[IStage] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a142e4a61436ea624a748446cb739233abd5326d66a7e1a91f9c88642f61ca94(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    api_mapping_id: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b9d717e977e1b3688e10b96a28c290636a0c8ffb230b0e32f751c93cfed6ae39(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    domain_name: builtins.str,
-    mtls: typing.Optional[typing.Union[MTLSConfig, typing.Dict[builtins.str, typing.Any]]] = None,
-    certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
-    certificate_name: typing.Optional[builtins.str] = None,
-    endpoint_type: typing.Optional[EndpointType] = None,
-    ownership_certificate: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
-    security_policy: typing.Optional[SecurityPolicy] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a75b51d5333f983b1ad28c7723855075bb1accd439fd505ecabd1a569a79bab5(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    name: builtins.str,
-    regional_domain_name: builtins.str,
-    regional_hosted_zone_id: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__698fe2808c79855db0ec402620f39e09a615424a13b6af162379044207a388e5(
-    *,
-    certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
-    certificate_name: typing.Optional[builtins.str] = None,
-    endpoint_type: typing.Optional[EndpointType] = None,
-    ownership_certificate: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
-    security_policy: typing.Optional[SecurityPolicy] = None,
-    domain_name: builtins.str,
-    mtls: typing.Optional[typing.Union[MTLSConfig, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__d5003409414773984b85252451580f75369de42c80978f161fece7261c553c54(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    api_name: typing.Optional[builtins.str] = None,
-    cors_preflight: typing.Optional[typing.Union[CorsPreflightOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    create_default_stage: typing.Optional[builtins.bool] = None,
-    default_authorization_scopes: typing.Optional[typing.Sequence[builtins.str]] = None,
-    default_authorizer: typing.Optional[IHttpRouteAuthorizer] = None,
-    default_domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    default_integration: typing.Optional[HttpRouteIntegration] = None,
-    description: typing.Optional[builtins.str] = None,
-    disable_execute_api_endpoint: typing.Optional[builtins.bool] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__ecd315f15fe552c95da2ac31778a118bb3415d560941e8d18e9c71e631481225(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    http_api_id: builtins.str,
-    api_endpoint: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__2bab5e6089f6e913d418934d66da25f8a39159ad3bd9f9f115cbcde831da78e0(
-    id: builtins.str,
-    *,
-    stage_name: typing.Optional[builtins.str] = None,
-    auto_deploy: typing.Optional[builtins.bool] = None,
-    domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    throttle: typing.Optional[typing.Union[ThrottleSettings, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a7709e3cbcd45c7d4a9b816ad94388873b7fd0558ca6fdcb427f2d5ca6e8df6a(
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
-def _typecheckingstub__03f7fb4792b9161dda177d8df2f5bc58091a4f546c4ca11ee18afaa4e0bf5e28(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    http_api: IHttpApi,
-    identity_source: typing.Sequence[builtins.str],
-    type: HttpAuthorizerType,
-    authorizer_name: typing.Optional[builtins.str] = None,
-    authorizer_uri: typing.Optional[builtins.str] = None,
-    enable_simple_responses: typing.Optional[builtins.bool] = None,
-    jwt_audience: typing.Optional[typing.Sequence[builtins.str]] = None,
-    jwt_issuer: typing.Optional[builtins.str] = None,
-    payload_format_version: typing.Optional[AuthorizerPayloadVersion] = None,
-    results_cache_ttl: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__efb4a2f65822f686a6ffa7ada308b84e89325054661df552cb9bc6286414ff5b(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    authorizer_id: builtins.str,
-    authorizer_type: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__68b934e47d5c501cf4c24923fe5b089fdb197a5624c649d8f83e58305cd890d5(
-    *,
-    stage_name: builtins.str,
-    api: IHttpApi,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__6e64c35e906d5449f8f7b3901603109565a527cbb27318f310243b054419c4a7(
-    *,
-    auto_deploy: typing.Optional[builtins.bool] = None,
-    domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    throttle: typing.Optional[typing.Union[ThrottleSettings, typing.Dict[builtins.str, typing.Any]]] = None,
-    stage_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__925560a3ec43c8b350658e7729b7c093c0eb2dc51b442b9b5877c46ec328fbb4(
-    *,
-    auto_deploy: typing.Optional[builtins.bool] = None,
-    domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    throttle: typing.Optional[typing.Union[ThrottleSettings, typing.Dict[builtins.str, typing.Any]]] = None,
-    stage_name: typing.Optional[builtins.str] = None,
-    http_api: IHttpApi,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e68d78a6fdd2cf02aa0a9db3e16ddc620002125429503856eb2206ca6638a462(
-    grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-    *,
-    http_methods: typing.Optional[typing.Sequence[HttpMethod]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__3de74d25b3d7d1e17696a2da7bd0666d13d0467eed87993389dc688e2ffcf281(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    http_api: IHttpApi,
-    integration_type: HttpIntegrationType,
-    connection_id: typing.Optional[builtins.str] = None,
-    connection_type: typing.Optional[HttpConnectionType] = None,
-    credentials: typing.Optional[IntegrationCredentials] = None,
-    integration_subtype: typing.Optional[HttpIntegrationSubtype] = None,
-    integration_uri: typing.Optional[builtins.str] = None,
-    method: typing.Optional[HttpMethod] = None,
-    parameter_mapping: typing.Optional[ParameterMapping] = None,
-    payload_format_version: typing.Optional[PayloadFormatVersion] = None,
-    secure_server_name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__d456143a18e04fab72c125ff49f83adf6625ae62b417322c1724ded4c91eeb7d(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    http_api: IHttpApi,
-    route_key: HttpRouteKey,
-    authorization_scopes: typing.Optional[typing.Sequence[builtins.str]] = None,
-    authorizer: typing.Optional[IHttpRouteAuthorizer] = None,
-    integration: HttpRouteIntegration,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__53257a740a0bf9e3076f5e9960cdc2b0c474378d558e854838154ba2bd8034cf(
-    grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
-    *,
-    http_methods: typing.Optional[typing.Sequence[HttpMethod]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__ed92fb335fa6855175afbb033d45447922cc6911de5d516e1c4dd76351a72aa1(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    http_api: IHttpApi,
-    stage_name: typing.Optional[builtins.str] = None,
-    auto_deploy: typing.Optional[builtins.bool] = None,
-    domain_mapping: typing.Optional[typing.Union[DomainMappingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    throttle: typing.Optional[typing.Union[ThrottleSettings, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__456b0db547449fda45bdfda459b2a51921656ff642e3c234362965315dbd5cd5(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    api: IHttpApi,
-    stage_name: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__13222b5ec0bde39f747497ef32fa2559d2b7146ce09903ba475536fb3869b080(
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

### Comparing `aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/src/aws_cdk.aws_apigatewayv2_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_alpha.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-apigatewayv2-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::APIGatewayv2
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
 
 # AWS::APIGatewayv2 Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -93,20 +93,21 @@
 [Configuring integrations](https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-develop-integrations.html).
 
 Integrations are available at the `aws-apigatewayv2-integrations` module and more information is available in that module.
 As an early example, the following code snippet configures a route `GET /books` with an HTTP proxy integration all
 configures all other HTTP method calls to `/books` to a lambda proxy.
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 from aws_cdk.aws_apigatewayv2_integrations_alpha import HttpUrlIntegration, HttpLambdaIntegration
 
 # books_default_fn: lambda.Function
 
 
-get_books_integration = HttpUrlIntegration("GetBooksIntegration", "https://get-books-proxy.example.com")
+get_books_integration = HttpUrlIntegration("GetBooksIntegration", "https://get-books-proxy.myproxy.internal")
 books_default_integration = HttpLambdaIntegration("BooksIntegration", books_default_fn)
 
 http_api = apigwv2.HttpApi(self, "HttpApi")
 
 http_api.add_routes(
     path="/books",
     methods=[apigwv2.HttpMethod.GET],
@@ -279,30 +280,29 @@
 ```
 
 ### Mutual TLS (mTLS)
 
 Mutual TLS can be configured to limit access to your API based by using client certificates instead of (or as an extension of) using authorization headers.
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 import aws_cdk.aws_s3 as s3
-import aws_cdk.aws_certificatemanager as acm
-# bucket: s3.Bucket
-
 
 cert_arn = "arn:aws:acm:us-east-1:111111111111:certificate"
 domain_name = "example.com"
+bucket = s3.Bucket.from_bucket_name(stack, "TrustStoreBucket", ...)
 
-apigwv2.DomainName(self, "DomainName",
+DomainName(stack, "DomainName",
     domain_name=domain_name,
-    certificate=acm.Certificate.from_certificate_arn(self, "cert", cert_arn),
-    mtls=apigwv2.MTLSConfig(
-        bucket=bucket,
-        key="someca.pem",
-        version="version"
-    )
+    certificate=Certificate.from_certificate_arn(stack, "cert", cert_arn),
+    mtls={
+        "bucket": bucket,
+        "key": "someca.pem",
+        "version": "version"
+    }
 )
 ```
 
 Instructions for configuring your trust store can be found [here](https://aws.amazon.com/blogs/compute/introducing-mutual-tls-authentication-for-amazon-api-gateway/)
 
 ### Managing access to HTTP APIs
 
@@ -428,52 +428,32 @@
 
 web_socket_api = apigwv2.WebSocketApi(self, "mywsapi")
 web_socket_api.add_route("sendmessage",
     integration=WebSocketLambdaIntegration("SendMessageIntegration", message_handler)
 )
 ```
 
-To add a route that can return a result:
-
-```python
-from aws_cdk.aws_apigatewayv2_integrations_alpha import WebSocketLambdaIntegration
-
-# message_handler: lambda.Function
-
-web_socket_api = apigwv2.WebSocketApi(self, "mywsapi")
-web_socket_api.add_route("sendmessage",
-    integration=WebSocketLambdaIntegration("SendMessageIntegration", message_handler),
-    return_response=True
-)
-```
-
-To import an existing WebSocketApi:
-
-```python
-web_socket_api = apigwv2.WebSocketApi.from_web_socket_api_attributes(self, "mywsapi", web_socket_id="api-1234")
-```
-
 ### Manage Connections Permission
 
 Grant permission to use API Gateway Management API of a WebSocket API by calling the `grantManageConnections` API.
 You can use Management API to send a callback message to a connected client, get connection information, or disconnect the client. Learn more at [Use @connections commands in your backend service](https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-how-to-call-websocket-api-connections.html).
 
 ```python
-# fn: lambda.Function
+# Example automatically generated from non-compiling source. May contain errors.
+lambda_ = lambda_.Function(self, "lambda")
 
-
-web_socket_api = apigwv2.WebSocketApi(self, "mywsapi")
-stage = apigwv2.WebSocketStage(self, "mystage",
+web_socket_api = WebSocketApi(stack, "mywsapi")
+stage = WebSocketStage(stack, "mystage",
     web_socket_api=web_socket_api,
     stage_name="dev"
 )
 # per stage permission
-stage.grant_management_api_access(fn)
+stage.grant_manage_connections(lambda_)
 # for all the stages permission
-web_socket_api.grant_manage_connections(fn)
+web_socket_api.grant_manage_connections(lambda_)
 ```
 
 ### Managing access to WebSocket APIs
 
 API Gateway supports multiple mechanisms for [controlling and managing access to a WebSocket API](https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-websocket-api-control-access.html) through authorizers.
 
 These authorizers can be found in the [APIGatewayV2-Authorizers](https://docs.aws.amazon.com/cdk/api/latest/docs/aws-apigatewayv2-authorizers-readme.html) constructs library.
@@ -481,11 +461,14 @@
 ### API Keys
 
 Websocket APIs also support usage of API Keys. An API Key is a key that is used to grant access to an API. These are useful for controlling and tracking access to an API, when used together with [usage plans](https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-api-usage-plans.html). These together allow you to configure controls around API access such as quotas and throttling, along with per-API Key metrics on usage.
 
 To require an API Key when accessing the Websocket API:
 
 ```python
-web_socket_api = apigwv2.WebSocketApi(self, "mywsapi",
-    api_key_selection_expression=apigwv2.WebSocketApiKeySelectionExpression.HEADER_X_API_KEY
+# Example automatically generated from non-compiling source. May contain errors.
+web_socket_api = WebSocketApi(stack, "mywsapi",
+    api_key_selection_expression=WebSocketApiKeySelectionExpression.HEADER_X_API_KEY
 )
 ```
+
+
```

### Comparing `aws-cdk.aws-apigatewayv2-alpha-2.84.0a0/src/aws_cdk.aws_apigatewayv2_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-apigatewayv2-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_alpha.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_apigatewayv2_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_apigatewayv2_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_apigatewayv2_alpha.egg-info/requires.txt
 src/aws_cdk.aws_apigatewayv2_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_apigatewayv2_alpha/__init__.py
 src/aws_cdk/aws_apigatewayv2_alpha/py.typed
 src/aws_cdk/aws_apigatewayv2_alpha/_jsii/__init__.py
-src/aws_cdk/aws_apigatewayv2_alpha/_jsii/aws-apigatewayv2-alpha@2.84.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_apigatewayv2_alpha/_jsii/aws-apigatewayv2-alpha@2.9.0-alpha.0.jsii.tgz
```

