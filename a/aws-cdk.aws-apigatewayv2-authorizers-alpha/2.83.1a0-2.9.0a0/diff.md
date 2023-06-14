# Comparing `tmp/aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0.tar.gz` & `tmp/aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src629398401/src/packages/@aws-cdk/aws-apigatewayv2-authorizers-alpha/dist/python/aws-cdk.aws-apigatewayv2-au", last modified: Fri Jun  9 09:55:25 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-apigatewayv2-authorizers/dist/python/aws-cdk.aws-apigateway", last modified: Wed Jan 26 11:22:21 2022, max compression
```

## Comparing `aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0.tar` & `aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:25.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-09 09:55:15.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-09 09:55:15.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-09 09:55:15.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11682 2023-06-09 09:55:25.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10673 2023-06-09 09:55:15.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-09 09:55:15.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 09:55:25.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2016 2023-06-09 09:55:15.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:25.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:25.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:25.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/src/aws_cdk/aws_apigatewayv2_authorizers_alpha/
--rw-r--r--   0 root         (0) root         (0)    54178 2023-06-09 09:55:15.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/src/aws_cdk/aws_apigatewayv2_authorizers_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:25.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/src/aws_cdk/aws_apigatewayv2_authorizers_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-09 09:55:15.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/src/aws_cdk/aws_apigatewayv2_authorizers_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45566 2023-06-09 09:55:15.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/src/aws_cdk/aws_apigatewayv2_authorizers_alpha/_jsii/aws-apigatewayv2-authorizers-alpha@2.83.1-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:55:15.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/src/aws_cdk/aws_apigatewayv2_authorizers_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:25.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11682 2023-06-09 09:55:25.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      701 2023-06-09 09:55:25.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:55:25.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-09 09:55:25.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-09 09:55:25.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:21.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:18.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:18.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:18.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10627 2022-01-26 11:22:21.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9651 2022-01-26 11:22:18.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:18.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:21.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1940 2022-01-26 11:22:18.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:21.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:21.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:21.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_authorizers_alpha/
+-rw-r--r--   0 root         (0) root         (0)    43110 2022-01-26 11:22:18.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_authorizers_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:21.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_authorizers_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      483 2022-01-26 11:22:18.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_authorizers_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36953 2022-01-26 11:22:18.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_authorizers_alpha/_jsii/aws-apigatewayv2-authorizers-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:18.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_authorizers_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:21.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10627 2022-01-26 11:22:21.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      700 2022-01-26 11:22:21.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:21.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2022-01-26 11:22:21.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:21.000000 aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/LICENSE` & `aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/LICENSE`

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

### Comparing `aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/PKG-INFO` & `aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-apigatewayv2-authorizers-alpha
-Version: 2.83.1a0
+Version: 2.9.0a0
 Summary: Authorizers for AWS APIGateway V2
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
 
 # AWS APIGatewayv2 Authorizers
 
 <!--BEGIN STABILITY BANNER-->---
@@ -52,15 +52,14 @@
 
     * [User Pool Authorizer](#user-pool-authorizer)
   * [Lambda Authorizers](#lambda-authorizers)
   * [IAM Authorizers](#iam-authorizers)
 * [WebSocket APIs](#websocket-apis)
 
   * [Lambda Authorizer](#lambda-authorizer)
-  * [IAM Authorizers](#iam-authorizer)
 
 ## Introduction
 
 API Gateway supports multiple mechanisms for controlling and managing access to your HTTP API. They are mainly
 classified into Lambda Authorizers, JWT authorizers and standard AWS IAM roles and policies. More information is
 available at [Controlling and managing access to an HTTP
 API](https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-access-control.html).
@@ -114,34 +113,34 @@
 
 api = apigwv2.HttpApi(self, "HttpApi",
     default_authorizer=authorizer,
     default_authorization_scopes=["read:books"]
 )
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     methods=[apigwv2.HttpMethod.GET]
 )
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIdIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIdIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books/{id}",
     methods=[apigwv2.HttpMethod.GET]
 )
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     methods=[apigwv2.HttpMethod.POST],
     authorization_scopes=["write:books"]
 )
 
 api.add_routes(
-    integration=HttpUrlIntegration("LoginIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("LoginIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/login",
     methods=[apigwv2.HttpMethod.POST],
     authorizer=apigwv2.HttpNoneAuthorizer()
 )
 ```
 
 ### JWT Authorizers
@@ -169,15 +168,15 @@
 authorizer = HttpJwtAuthorizer("BooksAuthorizer", issuer,
     jwt_audience=["3131231"]
 )
 
 api = apigwv2.HttpApi(self, "HttpApi")
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     authorizer=authorizer
 )
 ```
 
 #### User Pool Authorizer
 
@@ -196,15 +195,15 @@
 user_pool = cognito.UserPool(self, "UserPool")
 
 authorizer = HttpUserPoolAuthorizer("BooksAuthorizer", user_pool)
 
 api = apigwv2.HttpApi(self, "HttpApi")
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     authorizer=authorizer
 )
 ```
 
 ### Lambda Authorizers
 
@@ -223,15 +222,15 @@
 authorizer = HttpLambdaAuthorizer("BooksAuthorizer", auth_handler,
     response_types=[HttpLambdaResponseType.SIMPLE]
 )
 
 api = apigwv2.HttpApi(self, "HttpApi")
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     authorizer=authorizer
 )
 ```
 
 ### IAM Authorizers
 
@@ -247,15 +246,15 @@
 authorizer = HttpIamAuthorizer()
 
 http_api = apigwv2.HttpApi(self, "HttpApi",
     default_authorizer=authorizer
 )
 
 routes = http_api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books/{book}"
 )
 
 routes[0].grant_invoke(principal)
 ```
 
 ## WebSocket APIs
@@ -285,45 +284,8 @@
     connect_route_options=apigwv2.WebSocketRouteOptions(
         integration=integration,
         authorizer=authorizer
     )
 )
 ```
 
-### IAM Authorizer
 
-IAM authorizers can be used to allow identity-based access to your WebSocket API.
-
-```python
-from aws_cdk.aws_apigatewayv2_authorizers_alpha import WebSocketIamAuthorizer
-from aws_cdk.aws_apigatewayv2_integrations_alpha import WebSocketLambdaIntegration
-
-# This function handles your connect route
-# connect_handler: lambda.Function
-
-
-web_socket_api = apigwv2.WebSocketApi(self, "WebSocketApi")
-
-web_socket_api.add_route("$connect",
-    integration=WebSocketLambdaIntegration("Integration", connect_handler),
-    authorizer=WebSocketIamAuthorizer()
-)
-
-# Create an IAM user (identity)
-user = iam.User(self, "User")
-
-web_socket_arn = Stack.of(self).format_arn(
-    service="execute-api",
-    resource=web_socket_api.api_id
-)
-
-# Grant access to the IAM user
-user.attach_inline_policy(iam.Policy(self, "AllowInvoke",
-    statements=[
-        iam.PolicyStatement(
-            actions=["execute-api:Invoke"],
-            effect=iam.Effect.ALLOW,
-            resources=[web_socket_arn]
-        )
-    ]
-))
-```
```

### Comparing `aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/README.md` & `aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
     * [User Pool Authorizer](#user-pool-authorizer)
   * [Lambda Authorizers](#lambda-authorizers)
   * [IAM Authorizers](#iam-authorizers)
 * [WebSocket APIs](#websocket-apis)
 
   * [Lambda Authorizer](#lambda-authorizer)
-  * [IAM Authorizers](#iam-authorizer)
 
 ## Introduction
 
 API Gateway supports multiple mechanisms for controlling and managing access to your HTTP API. They are mainly
 classified into Lambda Authorizers, JWT authorizers and standard AWS IAM roles and policies. More information is
 available at [Controlling and managing access to an HTTP
 API](https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-access-control.html).
@@ -87,34 +86,34 @@
 
 api = apigwv2.HttpApi(self, "HttpApi",
     default_authorizer=authorizer,
     default_authorization_scopes=["read:books"]
 )
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     methods=[apigwv2.HttpMethod.GET]
 )
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIdIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIdIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books/{id}",
     methods=[apigwv2.HttpMethod.GET]
 )
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     methods=[apigwv2.HttpMethod.POST],
     authorization_scopes=["write:books"]
 )
 
 api.add_routes(
-    integration=HttpUrlIntegration("LoginIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("LoginIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/login",
     methods=[apigwv2.HttpMethod.POST],
     authorizer=apigwv2.HttpNoneAuthorizer()
 )
 ```
 
 ### JWT Authorizers
@@ -142,15 +141,15 @@
 authorizer = HttpJwtAuthorizer("BooksAuthorizer", issuer,
     jwt_audience=["3131231"]
 )
 
 api = apigwv2.HttpApi(self, "HttpApi")
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     authorizer=authorizer
 )
 ```
 
 #### User Pool Authorizer
 
@@ -169,15 +168,15 @@
 user_pool = cognito.UserPool(self, "UserPool")
 
 authorizer = HttpUserPoolAuthorizer("BooksAuthorizer", user_pool)
 
 api = apigwv2.HttpApi(self, "HttpApi")
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     authorizer=authorizer
 )
 ```
 
 ### Lambda Authorizers
 
@@ -196,15 +195,15 @@
 authorizer = HttpLambdaAuthorizer("BooksAuthorizer", auth_handler,
     response_types=[HttpLambdaResponseType.SIMPLE]
 )
 
 api = apigwv2.HttpApi(self, "HttpApi")
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     authorizer=authorizer
 )
 ```
 
 ### IAM Authorizers
 
@@ -220,15 +219,15 @@
 authorizer = HttpIamAuthorizer()
 
 http_api = apigwv2.HttpApi(self, "HttpApi",
     default_authorizer=authorizer
 )
 
 routes = http_api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books/{book}"
 )
 
 routes[0].grant_invoke(principal)
 ```
 
 ## WebSocket APIs
@@ -257,46 +256,7 @@
 apigwv2.WebSocketApi(self, "WebSocketApi",
     connect_route_options=apigwv2.WebSocketRouteOptions(
         integration=integration,
         authorizer=authorizer
     )
 )
 ```
-
-### IAM Authorizer
-
-IAM authorizers can be used to allow identity-based access to your WebSocket API.
-
-```python
-from aws_cdk.aws_apigatewayv2_authorizers_alpha import WebSocketIamAuthorizer
-from aws_cdk.aws_apigatewayv2_integrations_alpha import WebSocketLambdaIntegration
-
-# This function handles your connect route
-# connect_handler: lambda.Function
-
-
-web_socket_api = apigwv2.WebSocketApi(self, "WebSocketApi")
-
-web_socket_api.add_route("$connect",
-    integration=WebSocketLambdaIntegration("Integration", connect_handler),
-    authorizer=WebSocketIamAuthorizer()
-)
-
-# Create an IAM user (identity)
-user = iam.User(self, "User")
-
-web_socket_arn = Stack.of(self).format_arn(
-    service="execute-api",
-    resource=web_socket_api.api_id
-)
-
-# Grant access to the IAM user
-user.attach_inline_policy(iam.Policy(self, "AllowInvoke",
-    statements=[
-        iam.PolicyStatement(
-            actions=["execute-api:Invoke"],
-            effect=iam.Effect.ALLOW,
-            resources=[web_socket_arn]
-        )
-    ]
-))
-```
```

### Comparing `aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/setup.py` & `aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-apigatewayv2-authorizers-alpha",
-    "version": "2.83.1.a0",
+    "version": "2.9.0.a0",
     "description": "Authorizers for AWS APIGateway V2",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,44 +22,42 @@
     },
     "packages": [
         "aws_cdk.aws_apigatewayv2_authorizers_alpha",
         "aws_cdk.aws_apigatewayv2_authorizers_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_apigatewayv2_authorizers_alpha._jsii": [
-            "aws-apigatewayv2-authorizers-alpha@2.83.1-alpha.0.jsii.tgz"
+            "aws-apigatewayv2-authorizers-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_apigatewayv2_authorizers_alpha": [
             "py.typed"
         ]
     },
-    "python_requires": "~=3.7",
+    "python_requires": ">=3.6",
     "install_requires": [
-        "aws-cdk-lib==2.83.1",
-        "aws-cdk.aws-apigatewayv2-alpha==2.83.1.a0",
+        "aws-cdk-lib>=2.9.0, <3.0.0",
+        "aws-cdk.aws-apigatewayv2-alpha==2.9.0.a0",
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

### Comparing `aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/src/aws_cdk/aws_apigatewayv2_authorizers_alpha/__init__.py` & `aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_authorizers_alpha/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
     * [User Pool Authorizer](#user-pool-authorizer)
   * [Lambda Authorizers](#lambda-authorizers)
   * [IAM Authorizers](#iam-authorizers)
 * [WebSocket APIs](#websocket-apis)
 
   * [Lambda Authorizer](#lambda-authorizer)
-  * [IAM Authorizers](#iam-authorizer)
 
 ## Introduction
 
 API Gateway supports multiple mechanisms for controlling and managing access to your HTTP API. They are mainly
 classified into Lambda Authorizers, JWT authorizers and standard AWS IAM roles and policies. More information is
 available at [Controlling and managing access to an HTTP
 API](https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-access-control.html).
@@ -88,34 +87,34 @@
 
 api = apigwv2.HttpApi(self, "HttpApi",
     default_authorizer=authorizer,
     default_authorization_scopes=["read:books"]
 )
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     methods=[apigwv2.HttpMethod.GET]
 )
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIdIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIdIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books/{id}",
     methods=[apigwv2.HttpMethod.GET]
 )
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     methods=[apigwv2.HttpMethod.POST],
     authorization_scopes=["write:books"]
 )
 
 api.add_routes(
-    integration=HttpUrlIntegration("LoginIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("LoginIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/login",
     methods=[apigwv2.HttpMethod.POST],
     authorizer=apigwv2.HttpNoneAuthorizer()
 )
 ```
 
 ### JWT Authorizers
@@ -143,15 +142,15 @@
 authorizer = HttpJwtAuthorizer("BooksAuthorizer", issuer,
     jwt_audience=["3131231"]
 )
 
 api = apigwv2.HttpApi(self, "HttpApi")
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     authorizer=authorizer
 )
 ```
 
 #### User Pool Authorizer
 
@@ -170,15 +169,15 @@
 user_pool = cognito.UserPool(self, "UserPool")
 
 authorizer = HttpUserPoolAuthorizer("BooksAuthorizer", user_pool)
 
 api = apigwv2.HttpApi(self, "HttpApi")
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     authorizer=authorizer
 )
 ```
 
 ### Lambda Authorizers
 
@@ -197,15 +196,15 @@
 authorizer = HttpLambdaAuthorizer("BooksAuthorizer", auth_handler,
     response_types=[HttpLambdaResponseType.SIMPLE]
 )
 
 api = apigwv2.HttpApi(self, "HttpApi")
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     authorizer=authorizer
 )
 ```
 
 ### IAM Authorizers
 
@@ -221,15 +220,15 @@
 authorizer = HttpIamAuthorizer()
 
 http_api = apigwv2.HttpApi(self, "HttpApi",
     default_authorizer=authorizer
 )
 
 routes = http_api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books/{book}"
 )
 
 routes[0].grant_invoke(principal)
 ```
 
 ## WebSocket APIs
@@ -258,76 +257,35 @@
 apigwv2.WebSocketApi(self, "WebSocketApi",
     connect_route_options=apigwv2.WebSocketRouteOptions(
         integration=integration,
         authorizer=authorizer
     )
 )
 ```
-
-### IAM Authorizer
-
-IAM authorizers can be used to allow identity-based access to your WebSocket API.
-
-```python
-from aws_cdk.aws_apigatewayv2_authorizers_alpha import WebSocketIamAuthorizer
-from aws_cdk.aws_apigatewayv2_integrations_alpha import WebSocketLambdaIntegration
-
-# This function handles your connect route
-# connect_handler: lambda.Function
-
-
-web_socket_api = apigwv2.WebSocketApi(self, "WebSocketApi")
-
-web_socket_api.add_route("$connect",
-    integration=WebSocketLambdaIntegration("Integration", connect_handler),
-    authorizer=WebSocketIamAuthorizer()
-)
-
-# Create an IAM user (identity)
-user = iam.User(self, "User")
-
-web_socket_arn = Stack.of(self).format_arn(
-    service="execute-api",
-    resource=web_socket_api.api_id
-)
-
-# Grant access to the IAM user
-user.attach_inline_policy(iam.Policy(self, "AllowInvoke",
-    statements=[
-        iam.PolicyStatement(
-            actions=["execute-api:Invoke"],
-            effect=iam.Effect.ALLOW,
-            resources=[web_socket_arn]
-        )
-    ]
-))
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
-import aws_cdk.aws_apigatewayv2_alpha as _aws_cdk_aws_apigatewayv2_alpha_050969fe
-import aws_cdk.aws_cognito as _aws_cdk_aws_cognito_ceddda9d
-import aws_cdk.aws_lambda as _aws_cdk_aws_lambda_ceddda9d
-import constructs as _constructs_77d1e7e8
+import aws_cdk
+import aws_cdk.aws_apigatewayv2_alpha
+import aws_cdk.aws_cognito
+import aws_cdk.aws_lambda
+import constructs
 
 
-@jsii.implements(_aws_cdk_aws_apigatewayv2_alpha_050969fe.IHttpRouteAuthorizer)
+@jsii.implements(aws_cdk.aws_apigatewayv2_alpha.IHttpRouteAuthorizer)
 class HttpIamAuthorizer(
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-authorizers-alpha.HttpIamAuthorizer",
 ):
     '''(experimental) Authorize HTTP API Routes with IAM.
 
     :stability: experimental
@@ -344,15 +302,15 @@
         authorizer = HttpIamAuthorizer()
         
         http_api = apigwv2.HttpApi(self, "HttpApi",
             default_authorizer=authorizer
         )
         
         routes = http_api.add_routes(
-            integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+            integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
             path="/books/{book}"
         )
         
         routes[0].grant_invoke(principal)
     '''
 
     def __init__(self) -> None:
@@ -361,32 +319,32 @@
         '''
         jsii.create(self.__class__, self, [])
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
         *,
-        route: _aws_cdk_aws_apigatewayv2_alpha_050969fe.IHttpRoute,
-        scope: _constructs_77d1e7e8.Construct,
-    ) -> _aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpRouteAuthorizerConfig:
-        '''(experimental) Bind this authorizer to a specified Http route.
+        route: aws_cdk.aws_apigatewayv2_alpha.IHttpRoute,
+        scope: constructs.Construct,
+    ) -> aws_cdk.aws_apigatewayv2_alpha.HttpRouteAuthorizerConfig:
+        '''(experimental) (experimental) Bind this authorizer to a specified Http route.
 
         :param route: (experimental) The route to which the authorizer is being bound.
         :param scope: (experimental) The scope for any constructs created as part of the bind.
 
         :stability: experimental
         '''
-        _options = _aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpRouteAuthorizerBindOptions(
+        _options = aws_cdk.aws_apigatewayv2_alpha.HttpRouteAuthorizerBindOptions(
             route=route, scope=scope
         )
 
-        return typing.cast(_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpRouteAuthorizerConfig, jsii.invoke(self, "bind", [_options]))
+        return typing.cast(aws_cdk.aws_apigatewayv2_alpha.HttpRouteAuthorizerConfig, jsii.invoke(self, "bind", [_options]))
 
 
-@jsii.implements(_aws_cdk_aws_apigatewayv2_alpha_050969fe.IHttpRouteAuthorizer)
+@jsii.implements(aws_cdk.aws_apigatewayv2_alpha.IHttpRouteAuthorizer)
 class HttpJwtAuthorizer(
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-authorizers-alpha.HttpJwtAuthorizer",
 ):
     '''(experimental) Authorize Http Api routes on whether the requester is registered as part of an AWS Cognito user pool.
 
     :stability: experimental
@@ -402,15 +360,15 @@
         authorizer = HttpJwtAuthorizer("BooksAuthorizer", issuer,
             jwt_audience=["3131231"]
         )
         
         api = apigwv2.HttpApi(self, "HttpApi")
         
         api.add_routes(
-            integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+            integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
             path="/books",
             authorizer=authorizer
         )
     '''
 
     def __init__(
         self,
@@ -427,45 +385,41 @@
         :param jwt_issuer: The base domain of the identity provider that issues JWT.
         :param jwt_audience: (experimental) A list of the intended recipients of the JWT. A valid JWT must provide an aud that matches at least one entry in this list.
         :param authorizer_name: (experimental) The name of the authorizer. Default: - same value as ``id`` passed in the constructor
         :param identity_source: (experimental) The identity source for which authorization is requested. Default: ['$request.header.Authorization']
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fd7e477eedbddb612666258aa8e25ffee558e7f117660edf3a32774dc570644a)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument jwt_issuer", value=jwt_issuer, expected_type=type_hints["jwt_issuer"])
         props = HttpJwtAuthorizerProps(
             jwt_audience=jwt_audience,
             authorizer_name=authorizer_name,
             identity_source=identity_source,
         )
 
         jsii.create(self.__class__, self, [id, jwt_issuer, props])
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
         *,
-        route: _aws_cdk_aws_apigatewayv2_alpha_050969fe.IHttpRoute,
-        scope: _constructs_77d1e7e8.Construct,
-    ) -> _aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpRouteAuthorizerConfig:
-        '''(experimental) Bind this authorizer to a specified Http route.
+        route: aws_cdk.aws_apigatewayv2_alpha.IHttpRoute,
+        scope: constructs.Construct,
+    ) -> aws_cdk.aws_apigatewayv2_alpha.HttpRouteAuthorizerConfig:
+        '''(experimental) (experimental) Bind this authorizer to a specified Http route.
 
         :param route: (experimental) The route to which the authorizer is being bound.
         :param scope: (experimental) The scope for any constructs created as part of the bind.
 
         :stability: experimental
         '''
-        options = _aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpRouteAuthorizerBindOptions(
+        options = aws_cdk.aws_apigatewayv2_alpha.HttpRouteAuthorizerBindOptions(
             route=route, scope=scope
         )
 
-        return typing.cast(_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpRouteAuthorizerConfig, jsii.invoke(self, "bind", [options]))
+        return typing.cast(aws_cdk.aws_apigatewayv2_alpha.HttpRouteAuthorizerConfig, jsii.invoke(self, "bind", [options]))
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-apigatewayv2-authorizers-alpha.HttpJwtAuthorizerProps",
     jsii_struct_bases=[],
     name_mapping={
         "jwt_audience": "jwtAudience",
@@ -500,25 +454,20 @@
             authorizer = HttpJwtAuthorizer("BooksAuthorizer", issuer,
                 jwt_audience=["3131231"]
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
-            type_hints = typing.get_type_hints(_typecheckingstub__fe3ac9440c16507631949d98ec581bf0b61f90002e7b14fd7a99c168b4219825)
-            check_type(argname="argument jwt_audience", value=jwt_audience, expected_type=type_hints["jwt_audience"])
-            check_type(argname="argument authorizer_name", value=authorizer_name, expected_type=type_hints["authorizer_name"])
-            check_type(argname="argument identity_source", value=identity_source, expected_type=type_hints["identity_source"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "jwt_audience": jwt_audience,
         }
         if authorizer_name is not None:
             self._values["authorizer_name"] = authorizer_name
         if identity_source is not None:
             self._values["identity_source"] = identity_source
 
@@ -564,15 +513,15 @@
 
     def __repr__(self) -> str:
         return "HttpJwtAuthorizerProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-@jsii.implements(_aws_cdk_aws_apigatewayv2_alpha_050969fe.IHttpRouteAuthorizer)
+@jsii.implements(aws_cdk.aws_apigatewayv2_alpha.IHttpRouteAuthorizer)
 class HttpLambdaAuthorizer(
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-authorizers-alpha.HttpLambdaAuthorizer",
 ):
     '''(experimental) Authorize Http Api routes via a lambda function.
 
     :stability: experimental
@@ -590,73 +539,69 @@
         authorizer = HttpLambdaAuthorizer("BooksAuthorizer", auth_handler,
             response_types=[HttpLambdaResponseType.SIMPLE]
         )
         
         api = apigwv2.HttpApi(self, "HttpApi")
         
         api.add_routes(
-            integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+            integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
             path="/books",
             authorizer=authorizer
         )
     '''
 
     def __init__(
         self,
         id: builtins.str,
-        handler: _aws_cdk_aws_lambda_ceddda9d.IFunction,
+        handler: aws_cdk.aws_lambda.IFunction,
         *,
         authorizer_name: typing.Optional[builtins.str] = None,
         identity_source: typing.Optional[typing.Sequence[builtins.str]] = None,
         response_types: typing.Optional[typing.Sequence["HttpLambdaResponseType"]] = None,
-        results_cache_ttl: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        results_cache_ttl: typing.Optional[aws_cdk.Duration] = None,
     ) -> None:
         '''(experimental) Initialize a lambda authorizer to be bound with HTTP route.
 
         :param id: The id of the underlying construct.
         :param handler: -
         :param authorizer_name: (experimental) Friendly authorizer name. Default: - same value as ``id`` passed in the constructor.
         :param identity_source: (experimental) The identity source for which authorization is requested. Default: ['$request.header.Authorization']
         :param response_types: (experimental) The types of responses the lambda can return. If HttpLambdaResponseType.SIMPLE is included then response format 2.0 will be used. Default: [HttpLambdaResponseType.IAM]
         :param results_cache_ttl: (experimental) How long APIGateway should cache the results. Max 1 hour. Disable caching by setting this to ``Duration.seconds(0)``. Default: Duration.minutes(5)
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7e42d3d343b93ad060d80dddb5e5a74cbe97da9d96944dc42a0cda74ed3f38e6)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument handler", value=handler, expected_type=type_hints["handler"])
         props = HttpLambdaAuthorizerProps(
             authorizer_name=authorizer_name,
             identity_source=identity_source,
             response_types=response_types,
             results_cache_ttl=results_cache_ttl,
         )
 
         jsii.create(self.__class__, self, [id, handler, props])
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
         *,
-        route: _aws_cdk_aws_apigatewayv2_alpha_050969fe.IHttpRoute,
-        scope: _constructs_77d1e7e8.Construct,
-    ) -> _aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpRouteAuthorizerConfig:
-        '''(experimental) Bind this authorizer to a specified Http route.
+        route: aws_cdk.aws_apigatewayv2_alpha.IHttpRoute,
+        scope: constructs.Construct,
+    ) -> aws_cdk.aws_apigatewayv2_alpha.HttpRouteAuthorizerConfig:
+        '''(experimental) (experimental) Bind this authorizer to a specified Http route.
 
         :param route: (experimental) The route to which the authorizer is being bound.
         :param scope: (experimental) The scope for any constructs created as part of the bind.
 
         :stability: experimental
         '''
-        options = _aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpRouteAuthorizerBindOptions(
+        options = aws_cdk.aws_apigatewayv2_alpha.HttpRouteAuthorizerBindOptions(
             route=route, scope=scope
         )
 
-        return typing.cast(_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpRouteAuthorizerConfig, jsii.invoke(self, "bind", [options]))
+        return typing.cast(aws_cdk.aws_apigatewayv2_alpha.HttpRouteAuthorizerConfig, jsii.invoke(self, "bind", [options]))
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-apigatewayv2-authorizers-alpha.HttpLambdaAuthorizerProps",
     jsii_struct_bases=[],
     name_mapping={
         "authorizer_name": "authorizerName",
@@ -668,15 +613,15 @@
 class HttpLambdaAuthorizerProps:
     def __init__(
         self,
         *,
         authorizer_name: typing.Optional[builtins.str] = None,
         identity_source: typing.Optional[typing.Sequence[builtins.str]] = None,
         response_types: typing.Optional[typing.Sequence["HttpLambdaResponseType"]] = None,
-        results_cache_ttl: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        results_cache_ttl: typing.Optional[aws_cdk.Duration] = None,
     ) -> None:
         '''(experimental) Properties to initialize HttpTokenAuthorizer.
 
         :param authorizer_name: (experimental) Friendly authorizer name. Default: - same value as ``id`` passed in the constructor.
         :param identity_source: (experimental) The identity source for which authorization is requested. Default: ['$request.header.Authorization']
         :param response_types: (experimental) The types of responses the lambda can return. If HttpLambdaResponseType.SIMPLE is included then response format 2.0 will be used. Default: [HttpLambdaResponseType.IAM]
         :param results_cache_ttl: (experimental) How long APIGateway should cache the results. Max 1 hour. Disable caching by setting this to ``Duration.seconds(0)``. Default: Duration.minutes(5)
@@ -696,26 +641,20 @@
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
-            type_hints = typing.get_type_hints(_typecheckingstub__7922e845c6214a013523af13f680c0ed1fd920d1b18193d6e81eb9a1e52f0e3a)
-            check_type(argname="argument authorizer_name", value=authorizer_name, expected_type=type_hints["authorizer_name"])
-            check_type(argname="argument identity_source", value=identity_source, expected_type=type_hints["identity_source"])
-            check_type(argname="argument response_types", value=response_types, expected_type=type_hints["response_types"])
-            check_type(argname="argument results_cache_ttl", value=results_cache_ttl, expected_type=type_hints["results_cache_ttl"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if authorizer_name is not None:
             self._values["authorizer_name"] = authorizer_name
         if identity_source is not None:
             self._values["identity_source"] = identity_source
         if response_types is not None:
             self._values["response_types"] = response_types
         if results_cache_ttl is not None:
@@ -755,26 +694,26 @@
         :see: https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-lambda-authorizer.html#http-api-lambda-authorizer.payload-format-response
         :stability: experimental
         '''
         result = self._values.get("response_types")
         return typing.cast(typing.Optional[typing.List["HttpLambdaResponseType"]], result)
 
     @builtins.property
-    def results_cache_ttl(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+    def results_cache_ttl(self) -> typing.Optional[aws_cdk.Duration]:
         '''(experimental) How long APIGateway should cache the results.
 
         Max 1 hour.
         Disable caching by setting this to ``Duration.seconds(0)``.
 
         :default: Duration.minutes(5)
 
         :stability: experimental
         '''
         result = self._values.get("results_cache_ttl")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
+        return typing.cast(typing.Optional[aws_cdk.Duration], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -801,15 +740,15 @@
     IAM = "IAM"
     '''(experimental) Returns an IAM Policy.
 
     :stability: experimental
     '''
 
 
-@jsii.implements(_aws_cdk_aws_apigatewayv2_alpha_050969fe.IHttpRouteAuthorizer)
+@jsii.implements(aws_cdk.aws_apigatewayv2_alpha.IHttpRouteAuthorizer)
 class HttpUserPoolAuthorizer(
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-authorizers-alpha.HttpUserPoolAuthorizer",
 ):
     '''(experimental) Authorize Http Api routes on whether the requester is registered as part of an AWS Cognito user pool.
 
     :stability: experimental
@@ -825,73 +764,69 @@
         user_pool = cognito.UserPool(self, "UserPool")
         
         authorizer = HttpUserPoolAuthorizer("BooksAuthorizer", user_pool)
         
         api = apigwv2.HttpApi(self, "HttpApi")
         
         api.add_routes(
-            integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+            integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
             path="/books",
             authorizer=authorizer
         )
     '''
 
     def __init__(
         self,
         id: builtins.str,
-        pool: _aws_cdk_aws_cognito_ceddda9d.IUserPool,
+        pool: aws_cdk.aws_cognito.IUserPool,
         *,
         authorizer_name: typing.Optional[builtins.str] = None,
         identity_source: typing.Optional[typing.Sequence[builtins.str]] = None,
-        user_pool_clients: typing.Optional[typing.Sequence[_aws_cdk_aws_cognito_ceddda9d.IUserPoolClient]] = None,
+        user_pool_clients: typing.Optional[typing.Sequence[aws_cdk.aws_cognito.IUserPoolClient]] = None,
         user_pool_region: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Initialize a Cognito user pool authorizer to be bound with HTTP route.
 
         :param id: The id of the underlying construct.
         :param pool: The user pool to use for authorization.
         :param authorizer_name: (experimental) Friendly name of the authorizer. Default: - same value as ``id`` passed in the constructor
         :param identity_source: (experimental) The identity source for which authorization is requested. Default: ['$request.header.Authorization']
         :param user_pool_clients: (experimental) The user pool clients that should be used to authorize requests with the user pool. Default: - a new client will be created for the given user pool
         :param user_pool_region: (experimental) The AWS region in which the user pool is present. Default: - same region as the Route the authorizer is attached to.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__84cb6a1dac867ab33174b63daa8a384a2e178b1ed0c49e901511f25a5a928583)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument pool", value=pool, expected_type=type_hints["pool"])
         props = HttpUserPoolAuthorizerProps(
             authorizer_name=authorizer_name,
             identity_source=identity_source,
             user_pool_clients=user_pool_clients,
             user_pool_region=user_pool_region,
         )
 
         jsii.create(self.__class__, self, [id, pool, props])
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
         *,
-        route: _aws_cdk_aws_apigatewayv2_alpha_050969fe.IHttpRoute,
-        scope: _constructs_77d1e7e8.Construct,
-    ) -> _aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpRouteAuthorizerConfig:
-        '''(experimental) Bind this authorizer to a specified Http route.
+        route: aws_cdk.aws_apigatewayv2_alpha.IHttpRoute,
+        scope: constructs.Construct,
+    ) -> aws_cdk.aws_apigatewayv2_alpha.HttpRouteAuthorizerConfig:
+        '''(experimental) (experimental) Bind this authorizer to a specified Http route.
 
         :param route: (experimental) The route to which the authorizer is being bound.
         :param scope: (experimental) The scope for any constructs created as part of the bind.
 
         :stability: experimental
         '''
-        options = _aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpRouteAuthorizerBindOptions(
+        options = aws_cdk.aws_apigatewayv2_alpha.HttpRouteAuthorizerBindOptions(
             route=route, scope=scope
         )
 
-        return typing.cast(_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpRouteAuthorizerConfig, jsii.invoke(self, "bind", [options]))
+        return typing.cast(aws_cdk.aws_apigatewayv2_alpha.HttpRouteAuthorizerConfig, jsii.invoke(self, "bind", [options]))
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-apigatewayv2-authorizers-alpha.HttpUserPoolAuthorizerProps",
     jsii_struct_bases=[],
     name_mapping={
         "authorizer_name": "authorizerName",
@@ -902,15 +837,15 @@
 )
 class HttpUserPoolAuthorizerProps:
     def __init__(
         self,
         *,
         authorizer_name: typing.Optional[builtins.str] = None,
         identity_source: typing.Optional[typing.Sequence[builtins.str]] = None,
-        user_pool_clients: typing.Optional[typing.Sequence[_aws_cdk_aws_cognito_ceddda9d.IUserPoolClient]] = None,
+        user_pool_clients: typing.Optional[typing.Sequence[aws_cdk.aws_cognito.IUserPoolClient]] = None,
         user_pool_region: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Properties to initialize HttpUserPoolAuthorizer.
 
         :param authorizer_name: (experimental) Friendly name of the authorizer. Default: - same value as ``id`` passed in the constructor
         :param identity_source: (experimental) The identity source for which authorization is requested. Default: ['$request.header.Authorization']
         :param user_pool_clients: (experimental) The user pool clients that should be used to authorize requests with the user pool. Default: - a new client will be created for the given user pool
@@ -931,21 +866,15 @@
             http_user_pool_authorizer_props = apigatewayv2_authorizers_alpha.HttpUserPoolAuthorizerProps(
                 authorizer_name="authorizerName",
                 identity_source=["identitySource"],
                 user_pool_clients=[user_pool_client],
                 user_pool_region="userPoolRegion"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__012cb35afcb2f89a14d2c6d5d63d40f8e00f6e28c5dddd9440b9ccd952953a66)
-            check_type(argname="argument authorizer_name", value=authorizer_name, expected_type=type_hints["authorizer_name"])
-            check_type(argname="argument identity_source", value=identity_source, expected_type=type_hints["identity_source"])
-            check_type(argname="argument user_pool_clients", value=user_pool_clients, expected_type=type_hints["user_pool_clients"])
-            check_type(argname="argument user_pool_region", value=user_pool_region, expected_type=type_hints["user_pool_region"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if authorizer_name is not None:
             self._values["authorizer_name"] = authorizer_name
         if identity_source is not None:
             self._values["identity_source"] = identity_source
         if user_pool_clients is not None:
             self._values["user_pool_clients"] = user_pool_clients
         if user_pool_region is not None:
@@ -972,23 +901,23 @@
         '''
         result = self._values.get("identity_source")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def user_pool_clients(
         self,
-    ) -> typing.Optional[typing.List[_aws_cdk_aws_cognito_ceddda9d.IUserPoolClient]]:
+    ) -> typing.Optional[typing.List[aws_cdk.aws_cognito.IUserPoolClient]]:
         '''(experimental) The user pool clients that should be used to authorize requests with the user pool.
 
         :default: - a new client will be created for the given user pool
 
         :stability: experimental
         '''
         result = self._values.get("user_pool_clients")
-        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_cognito_ceddda9d.IUserPoolClient]], result)
+        return typing.cast(typing.Optional[typing.List[aws_cdk.aws_cognito.IUserPoolClient]], result)
 
     @builtins.property
     def user_pool_region(self) -> typing.Optional[builtins.str]:
         '''(experimental) The AWS region in which the user pool is present.
 
         :default: - same region as the Route the authorizer is attached to.
 
@@ -1005,88 +934,15 @@
 
     def __repr__(self) -> str:
         return "HttpUserPoolAuthorizerProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-@jsii.implements(_aws_cdk_aws_apigatewayv2_alpha_050969fe.IWebSocketRouteAuthorizer)
-class WebSocketIamAuthorizer(
-    metaclass=jsii.JSIIMeta,
-    jsii_type="@aws-cdk/aws-apigatewayv2-authorizers-alpha.WebSocketIamAuthorizer",
-):
-    '''(experimental) Authorize WebSocket API Routes with IAM.
-
-    :stability: experimental
-    :exampleMetadata: infused
-
-    Example::
-
-        from aws_cdk.aws_apigatewayv2_authorizers_alpha import WebSocketIamAuthorizer
-        from aws_cdk.aws_apigatewayv2_integrations_alpha import WebSocketLambdaIntegration
-        
-        # This function handles your connect route
-        # connect_handler: lambda.Function
-        
-        
-        web_socket_api = apigwv2.WebSocketApi(self, "WebSocketApi")
-        
-        web_socket_api.add_route("$connect",
-            integration=WebSocketLambdaIntegration("Integration", connect_handler),
-            authorizer=WebSocketIamAuthorizer()
-        )
-        
-        # Create an IAM user (identity)
-        user = iam.User(self, "User")
-        
-        web_socket_arn = Stack.of(self).format_arn(
-            service="execute-api",
-            resource=web_socket_api.api_id
-        )
-        
-        # Grant access to the IAM user
-        user.attach_inline_policy(iam.Policy(self, "AllowInvoke",
-            statements=[
-                iam.PolicyStatement(
-                    actions=["execute-api:Invoke"],
-                    effect=iam.Effect.ALLOW,
-                    resources=[web_socket_arn]
-                )
-            ]
-        ))
-    '''
-
-    def __init__(self) -> None:
-        '''
-        :stability: experimental
-        '''
-        jsii.create(self.__class__, self, [])
-
-    @jsii.member(jsii_name="bind")
-    def bind(
-        self,
-        *,
-        route: _aws_cdk_aws_apigatewayv2_alpha_050969fe.IWebSocketRoute,
-        scope: _constructs_77d1e7e8.Construct,
-    ) -> _aws_cdk_aws_apigatewayv2_alpha_050969fe.WebSocketRouteAuthorizerConfig:
-        '''(experimental) Bind this authorizer to a specified WebSocket route.
-
-        :param route: (experimental) The route to which the authorizer is being bound.
-        :param scope: (experimental) The scope for any constructs created as part of the bind.
-
-        :stability: experimental
-        '''
-        _options = _aws_cdk_aws_apigatewayv2_alpha_050969fe.WebSocketRouteAuthorizerBindOptions(
-            route=route, scope=scope
-        )
-
-        return typing.cast(_aws_cdk_aws_apigatewayv2_alpha_050969fe.WebSocketRouteAuthorizerConfig, jsii.invoke(self, "bind", [_options]))
-
-
-@jsii.implements(_aws_cdk_aws_apigatewayv2_alpha_050969fe.IWebSocketRouteAuthorizer)
+@jsii.implements(aws_cdk.aws_apigatewayv2_alpha.IWebSocketRouteAuthorizer)
 class WebSocketLambdaAuthorizer(
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-apigatewayv2-authorizers-alpha.WebSocketLambdaAuthorizer",
 ):
     '''(experimental) Authorize WebSocket Api routes via a lambda function.
 
     :stability: experimental
@@ -1115,56 +971,52 @@
             )
         )
     '''
 
     def __init__(
         self,
         id: builtins.str,
-        handler: _aws_cdk_aws_lambda_ceddda9d.IFunction,
+        handler: aws_cdk.aws_lambda.IFunction,
         *,
         authorizer_name: typing.Optional[builtins.str] = None,
         identity_source: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
         :param id: -
         :param handler: -
         :param authorizer_name: (experimental) The name of the authorizer. Default: - same value as ``id`` passed in the constructor.
         :param identity_source: (experimental) The identity source for which authorization is requested. Request parameter match ``'route.request.querystring|header.[a-zA-z0-9._-]+'``. Staged variable match ``'stageVariables.[a-zA-Z0-9._-]+'``. Context parameter match ``'context.[a-zA-Z0-9._-]+'``. Default: ['route.request.header.Authorization']
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b0d2c747a0bfd922859066f8058bdb2ec535f9d20c1e5ae4c4e836c9aa3de5af)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument handler", value=handler, expected_type=type_hints["handler"])
         props = WebSocketLambdaAuthorizerProps(
             authorizer_name=authorizer_name, identity_source=identity_source
         )
 
         jsii.create(self.__class__, self, [id, handler, props])
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
         *,
-        route: _aws_cdk_aws_apigatewayv2_alpha_050969fe.IWebSocketRoute,
-        scope: _constructs_77d1e7e8.Construct,
-    ) -> _aws_cdk_aws_apigatewayv2_alpha_050969fe.WebSocketRouteAuthorizerConfig:
-        '''(experimental) Bind this authorizer to a specified WebSocket route.
+        route: aws_cdk.aws_apigatewayv2_alpha.IWebSocketRoute,
+        scope: constructs.Construct,
+    ) -> aws_cdk.aws_apigatewayv2_alpha.WebSocketRouteAuthorizerConfig:
+        '''(experimental) (experimental) Bind this authorizer to a specified WebSocket route.
 
         :param route: (experimental) The route to which the authorizer is being bound.
         :param scope: (experimental) The scope for any constructs created as part of the bind.
 
         :stability: experimental
         '''
-        options = _aws_cdk_aws_apigatewayv2_alpha_050969fe.WebSocketRouteAuthorizerBindOptions(
+        options = aws_cdk.aws_apigatewayv2_alpha.WebSocketRouteAuthorizerBindOptions(
             route=route, scope=scope
         )
 
-        return typing.cast(_aws_cdk_aws_apigatewayv2_alpha_050969fe.WebSocketRouteAuthorizerConfig, jsii.invoke(self, "bind", [options]))
+        return typing.cast(aws_cdk.aws_apigatewayv2_alpha.WebSocketRouteAuthorizerConfig, jsii.invoke(self, "bind", [options]))
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-apigatewayv2-authorizers-alpha.WebSocketLambdaAuthorizerProps",
     jsii_struct_bases=[],
     name_mapping={
         "authorizer_name": "authorizerName",
@@ -1193,19 +1045,15 @@
             import aws_cdk.aws_apigatewayv2_authorizers_alpha as apigatewayv2_authorizers_alpha
             
             web_socket_lambda_authorizer_props = apigatewayv2_authorizers_alpha.WebSocketLambdaAuthorizerProps(
                 authorizer_name="authorizerName",
                 identity_source=["identitySource"]
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e54d622dee3bbcf9b78941971356ff9a02536b0cd379ff02839c013e7f717f26)
-            check_type(argname="argument authorizer_name", value=authorizer_name, expected_type=type_hints["authorizer_name"])
-            check_type(argname="argument identity_source", value=identity_source, expected_type=type_hints["identity_source"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if authorizer_name is not None:
             self._values["authorizer_name"] = authorizer_name
         if identity_source is not None:
             self._values["identity_source"] = identity_source
 
     @builtins.property
     def authorizer_name(self) -> typing.Optional[builtins.str]:
@@ -1250,95 +1098,12 @@
     "HttpJwtAuthorizer",
     "HttpJwtAuthorizerProps",
     "HttpLambdaAuthorizer",
     "HttpLambdaAuthorizerProps",
     "HttpLambdaResponseType",
     "HttpUserPoolAuthorizer",
     "HttpUserPoolAuthorizerProps",
-    "WebSocketIamAuthorizer",
     "WebSocketLambdaAuthorizer",
     "WebSocketLambdaAuthorizerProps",
 ]
 
 publication.publish()
-
-def _typecheckingstub__fd7e477eedbddb612666258aa8e25ffee558e7f117660edf3a32774dc570644a(
-    id: builtins.str,
-    jwt_issuer: builtins.str,
-    *,
-    jwt_audience: typing.Sequence[builtins.str],
-    authorizer_name: typing.Optional[builtins.str] = None,
-    identity_source: typing.Optional[typing.Sequence[builtins.str]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__fe3ac9440c16507631949d98ec581bf0b61f90002e7b14fd7a99c168b4219825(
-    *,
-    jwt_audience: typing.Sequence[builtins.str],
-    authorizer_name: typing.Optional[builtins.str] = None,
-    identity_source: typing.Optional[typing.Sequence[builtins.str]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__7e42d3d343b93ad060d80dddb5e5a74cbe97da9d96944dc42a0cda74ed3f38e6(
-    id: builtins.str,
-    handler: _aws_cdk_aws_lambda_ceddda9d.IFunction,
-    *,
-    authorizer_name: typing.Optional[builtins.str] = None,
-    identity_source: typing.Optional[typing.Sequence[builtins.str]] = None,
-    response_types: typing.Optional[typing.Sequence[HttpLambdaResponseType]] = None,
-    results_cache_ttl: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__7922e845c6214a013523af13f680c0ed1fd920d1b18193d6e81eb9a1e52f0e3a(
-    *,
-    authorizer_name: typing.Optional[builtins.str] = None,
-    identity_source: typing.Optional[typing.Sequence[builtins.str]] = None,
-    response_types: typing.Optional[typing.Sequence[HttpLambdaResponseType]] = None,
-    results_cache_ttl: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__84cb6a1dac867ab33174b63daa8a384a2e178b1ed0c49e901511f25a5a928583(
-    id: builtins.str,
-    pool: _aws_cdk_aws_cognito_ceddda9d.IUserPool,
-    *,
-    authorizer_name: typing.Optional[builtins.str] = None,
-    identity_source: typing.Optional[typing.Sequence[builtins.str]] = None,
-    user_pool_clients: typing.Optional[typing.Sequence[_aws_cdk_aws_cognito_ceddda9d.IUserPoolClient]] = None,
-    user_pool_region: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__012cb35afcb2f89a14d2c6d5d63d40f8e00f6e28c5dddd9440b9ccd952953a66(
-    *,
-    authorizer_name: typing.Optional[builtins.str] = None,
-    identity_source: typing.Optional[typing.Sequence[builtins.str]] = None,
-    user_pool_clients: typing.Optional[typing.Sequence[_aws_cdk_aws_cognito_ceddda9d.IUserPoolClient]] = None,
-    user_pool_region: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b0d2c747a0bfd922859066f8058bdb2ec535f9d20c1e5ae4c4e836c9aa3de5af(
-    id: builtins.str,
-    handler: _aws_cdk_aws_lambda_ceddda9d.IFunction,
-    *,
-    authorizer_name: typing.Optional[builtins.str] = None,
-    identity_source: typing.Optional[typing.Sequence[builtins.str]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e54d622dee3bbcf9b78941971356ff9a02536b0cd379ff02839c013e7f717f26(
-    *,
-    authorizer_name: typing.Optional[builtins.str] = None,
-    identity_source: typing.Optional[typing.Sequence[builtins.str]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
```

### Comparing `aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-apigatewayv2-authorizers-alpha
-Version: 2.83.1a0
+Version: 2.9.0a0
 Summary: Authorizers for AWS APIGateway V2
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
 
 # AWS APIGatewayv2 Authorizers
 
 <!--BEGIN STABILITY BANNER-->---
@@ -52,15 +52,14 @@
 
     * [User Pool Authorizer](#user-pool-authorizer)
   * [Lambda Authorizers](#lambda-authorizers)
   * [IAM Authorizers](#iam-authorizers)
 * [WebSocket APIs](#websocket-apis)
 
   * [Lambda Authorizer](#lambda-authorizer)
-  * [IAM Authorizers](#iam-authorizer)
 
 ## Introduction
 
 API Gateway supports multiple mechanisms for controlling and managing access to your HTTP API. They are mainly
 classified into Lambda Authorizers, JWT authorizers and standard AWS IAM roles and policies. More information is
 available at [Controlling and managing access to an HTTP
 API](https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-access-control.html).
@@ -114,34 +113,34 @@
 
 api = apigwv2.HttpApi(self, "HttpApi",
     default_authorizer=authorizer,
     default_authorization_scopes=["read:books"]
 )
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     methods=[apigwv2.HttpMethod.GET]
 )
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIdIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIdIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books/{id}",
     methods=[apigwv2.HttpMethod.GET]
 )
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     methods=[apigwv2.HttpMethod.POST],
     authorization_scopes=["write:books"]
 )
 
 api.add_routes(
-    integration=HttpUrlIntegration("LoginIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("LoginIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/login",
     methods=[apigwv2.HttpMethod.POST],
     authorizer=apigwv2.HttpNoneAuthorizer()
 )
 ```
 
 ### JWT Authorizers
@@ -169,15 +168,15 @@
 authorizer = HttpJwtAuthorizer("BooksAuthorizer", issuer,
     jwt_audience=["3131231"]
 )
 
 api = apigwv2.HttpApi(self, "HttpApi")
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     authorizer=authorizer
 )
 ```
 
 #### User Pool Authorizer
 
@@ -196,15 +195,15 @@
 user_pool = cognito.UserPool(self, "UserPool")
 
 authorizer = HttpUserPoolAuthorizer("BooksAuthorizer", user_pool)
 
 api = apigwv2.HttpApi(self, "HttpApi")
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     authorizer=authorizer
 )
 ```
 
 ### Lambda Authorizers
 
@@ -223,15 +222,15 @@
 authorizer = HttpLambdaAuthorizer("BooksAuthorizer", auth_handler,
     response_types=[HttpLambdaResponseType.SIMPLE]
 )
 
 api = apigwv2.HttpApi(self, "HttpApi")
 
 api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books",
     authorizer=authorizer
 )
 ```
 
 ### IAM Authorizers
 
@@ -247,15 +246,15 @@
 authorizer = HttpIamAuthorizer()
 
 http_api = apigwv2.HttpApi(self, "HttpApi",
     default_authorizer=authorizer
 )
 
 routes = http_api.add_routes(
-    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com"),
+    integration=HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal"),
     path="/books/{book}"
 )
 
 routes[0].grant_invoke(principal)
 ```
 
 ## WebSocket APIs
@@ -285,45 +284,8 @@
     connect_route_options=apigwv2.WebSocketRouteOptions(
         integration=integration,
         authorizer=authorizer
     )
 )
 ```
 
-### IAM Authorizer
 
-IAM authorizers can be used to allow identity-based access to your WebSocket API.
-
-```python
-from aws_cdk.aws_apigatewayv2_authorizers_alpha import WebSocketIamAuthorizer
-from aws_cdk.aws_apigatewayv2_integrations_alpha import WebSocketLambdaIntegration
-
-# This function handles your connect route
-# connect_handler: lambda.Function
-
-
-web_socket_api = apigwv2.WebSocketApi(self, "WebSocketApi")
-
-web_socket_api.add_route("$connect",
-    integration=WebSocketLambdaIntegration("Integration", connect_handler),
-    authorizer=WebSocketIamAuthorizer()
-)
-
-# Create an IAM user (identity)
-user = iam.User(self, "User")
-
-web_socket_arn = Stack.of(self).format_arn(
-    service="execute-api",
-    resource=web_socket_api.api_id
-)
-
-# Grant access to the IAM user
-user.attach_inline_policy(iam.Policy(self, "AllowInvoke",
-    statements=[
-        iam.PolicyStatement(
-            actions=["execute-api:Invoke"],
-            effect=iam.Effect.ALLOW,
-            resources=[web_socket_arn]
-        )
-    ]
-))
-```
```

### Comparing `aws-cdk.aws-apigatewayv2-authorizers-alpha-2.83.1a0/src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-apigatewayv2-authorizers-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/requires.txt
 src/aws_cdk.aws_apigatewayv2_authorizers_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_apigatewayv2_authorizers_alpha/__init__.py
 src/aws_cdk/aws_apigatewayv2_authorizers_alpha/py.typed
 src/aws_cdk/aws_apigatewayv2_authorizers_alpha/_jsii/__init__.py
-src/aws_cdk/aws_apigatewayv2_authorizers_alpha/_jsii/aws-apigatewayv2-authorizers-alpha@2.83.1-alpha.0.jsii.tgz
+src/aws_cdk/aws_apigatewayv2_authorizers_alpha/_jsii/aws-apigatewayv2-authorizers-alpha@2.9.0-alpha.0.jsii.tgz
```

