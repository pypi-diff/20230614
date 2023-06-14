# Comparing `tmp/aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0.tar.gz` & `tmp/aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src629398401/src/packages/@aws-cdk/aws-apigatewayv2-integrations-alpha/dist/python/aws-cdk.aws-apigatewayv2-i", last modified: Fri Jun  9 09:55:06 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-apigatewayv2-integrations/dist/python/aws-cdk.aws-apigatewa", last modified: Wed Jan 26 11:22:15 2022, max compression
```

## Comparing `aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0.tar` & `aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:06.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-09 09:54:54.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-09 09:54:54.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-09 09:54:54.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9076 2023-06-09 09:55:06.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8065 2023-06-09 09:54:54.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-09 09:54:54.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 09:55:06.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2023 2023-06-09 09:54:54.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:06.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:06.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:06.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/src/aws_cdk/aws_apigatewayv2_integrations_alpha/
--rw-r--r--   0 root         (0) root         (0)    83171 2023-06-09 09:54:54.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/src/aws_cdk/aws_apigatewayv2_integrations_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:06.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/src/aws_cdk/aws_apigatewayv2_integrations_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      521 2023-06-09 09:54:54.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/src/aws_cdk/aws_apigatewayv2_integrations_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46303 2023-06-09 09:54:54.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/src/aws_cdk/aws_apigatewayv2_integrations_alpha/_jsii/aws-apigatewayv2-integrations-alpha@2.83.1-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:54:54.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/src/aws_cdk/aws_apigatewayv2_integrations_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:06.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9076 2023-06-09 09:55:06.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      711 2023-06-09 09:55:06.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:55:06.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-09 09:55:06.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-09 09:55:06.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:15.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:11.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:11.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:11.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9053 2022-01-26 11:22:15.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8075 2022-01-26 11:22:11.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:11.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:15.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1947 2022-01-26 11:22:11.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:15.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:15.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:15.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_integrations_alpha/
+-rw-r--r--   0 root         (0) root         (0)    63387 2022-01-26 11:22:11.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_integrations_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:15.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_integrations_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      485 2022-01-26 11:22:11.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_integrations_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40697 2022-01-26 11:22:11.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_integrations_alpha/_jsii/aws-apigatewayv2-integrations-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:11.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/src/aws_cdk/aws_apigatewayv2_integrations_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:15.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9053 2022-01-26 11:22:15.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      710 2022-01-26 11:22:15.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:15.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2022-01-26 11:22:15.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:15.000000 aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/LICENSE` & `aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/LICENSE`

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

### Comparing `aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/PKG-INFO` & `aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-apigatewayv2-integrations-alpha
-Version: 2.83.1a0
+Version: 2.9.0a0
 Summary: Integrations for AWS APIGateway V2
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
 
 # AWS APIGatewayv2 Integrations
 
 <!--BEGIN STABILITY BANNER-->---
@@ -88,21 +88,21 @@
 
 HTTP Proxy integrations enables connecting an HTTP API route to a publicly routable HTTP endpoint. When a client
 invokes the route, the API Gateway service forwards the entire request and response between the API Gateway endpoint
 and the integrating HTTP endpoint. More information can be found at [Working with HTTP proxy
 integrations](https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-develop-integrations-http.html).
 
 The following code configures a route `GET /books` with an HTTP proxy integration to an HTTP endpoint
-`get-books-proxy.example.com`.
+`get-books-proxy.myproxy.internal`.
 
 ```python
 from aws_cdk.aws_apigatewayv2_integrations_alpha import HttpUrlIntegration
 
 
-books_integration = HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com")
+books_integration = HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal")
 
 http_api = apigwv2.HttpApi(self, "HttpApi")
 
 http_api.add_routes(
     path="/books",
     methods=[apigwv2.HttpMethod.GET],
     integration=books_integration
@@ -254,7 +254,9 @@
     stage_name="dev",
     auto_deploy=True
 )
 web_socket_api.add_route("sendmessage",
     integration=WebSocketLambdaIntegration("SendMessageIntegration", message_handler)
 )
 ```
+
+
```

### Comparing `aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/README.md` & `aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,21 +61,21 @@
 
 HTTP Proxy integrations enables connecting an HTTP API route to a publicly routable HTTP endpoint. When a client
 invokes the route, the API Gateway service forwards the entire request and response between the API Gateway endpoint
 and the integrating HTTP endpoint. More information can be found at [Working with HTTP proxy
 integrations](https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-develop-integrations-http.html).
 
 The following code configures a route `GET /books` with an HTTP proxy integration to an HTTP endpoint
-`get-books-proxy.example.com`.
+`get-books-proxy.myproxy.internal`.
 
 ```python
 from aws_cdk.aws_apigatewayv2_integrations_alpha import HttpUrlIntegration
 
 
-books_integration = HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com")
+books_integration = HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal")
 
 http_api = apigwv2.HttpApi(self, "HttpApi")
 
 http_api.add_routes(
     path="/books",
     methods=[apigwv2.HttpMethod.GET],
     integration=books_integration
```

### Comparing `aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/setup.py` & `aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-apigatewayv2-integrations-alpha",
-    "version": "2.83.1.a0",
+    "version": "2.9.0.a0",
     "description": "Integrations for AWS APIGateway V2",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,44 +22,42 @@
     },
     "packages": [
         "aws_cdk.aws_apigatewayv2_integrations_alpha",
         "aws_cdk.aws_apigatewayv2_integrations_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_apigatewayv2_integrations_alpha._jsii": [
-            "aws-apigatewayv2-integrations-alpha@2.83.1-alpha.0.jsii.tgz"
+            "aws-apigatewayv2-integrations-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_apigatewayv2_integrations_alpha": [
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

### Comparing `aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-apigatewayv2-integrations-alpha
-Version: 2.83.1a0
+Version: 2.9.0a0
 Summary: Integrations for AWS APIGateway V2
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
 
 # AWS APIGatewayv2 Integrations
 
 <!--BEGIN STABILITY BANNER-->---
@@ -88,21 +88,21 @@
 
 HTTP Proxy integrations enables connecting an HTTP API route to a publicly routable HTTP endpoint. When a client
 invokes the route, the API Gateway service forwards the entire request and response between the API Gateway endpoint
 and the integrating HTTP endpoint. More information can be found at [Working with HTTP proxy
 integrations](https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-develop-integrations-http.html).
 
 The following code configures a route `GET /books` with an HTTP proxy integration to an HTTP endpoint
-`get-books-proxy.example.com`.
+`get-books-proxy.myproxy.internal`.
 
 ```python
 from aws_cdk.aws_apigatewayv2_integrations_alpha import HttpUrlIntegration
 
 
-books_integration = HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.example.com")
+books_integration = HttpUrlIntegration("BooksIntegration", "https://get-books-proxy.myproxy.internal")
 
 http_api = apigwv2.HttpApi(self, "HttpApi")
 
 http_api.add_routes(
     path="/books",
     methods=[apigwv2.HttpMethod.GET],
     integration=books_integration
@@ -254,7 +254,9 @@
     stage_name="dev",
     auto_deploy=True
 )
 web_socket_api.add_route("sendmessage",
     integration=WebSocketLambdaIntegration("SendMessageIntegration", message_handler)
 )
 ```
+
+
```

### Comparing `aws-cdk.aws-apigatewayv2-integrations-alpha-2.83.1a0/src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-apigatewayv2-integrations-alpha-2.9.0a0/src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/requires.txt
 src/aws_cdk.aws_apigatewayv2_integrations_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_apigatewayv2_integrations_alpha/__init__.py
 src/aws_cdk/aws_apigatewayv2_integrations_alpha/py.typed
 src/aws_cdk/aws_apigatewayv2_integrations_alpha/_jsii/__init__.py
-src/aws_cdk/aws_apigatewayv2_integrations_alpha/_jsii/aws-apigatewayv2-integrations-alpha@2.83.1-alpha.0.jsii.tgz
+src/aws_cdk/aws_apigatewayv2_integrations_alpha/_jsii/aws-apigatewayv2-integrations-alpha@2.9.0-alpha.0.jsii.tgz
```

