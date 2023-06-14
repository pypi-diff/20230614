# Comparing `tmp/aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0.tar.gz` & `tmp/aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/aws-cognito-identitypool-alpha/dist/python/aws-cdk.aws-cognito-identitypoo", last modified: Tue Jun 13 23:46:43 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-cognito-identitypool/dist/python/aws-cdk.aws-cognito-identi", last modified: Wed Jan 26 11:22:05 2022, max compression
```

## Comparing `aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0.tar` & `aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:43.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:37.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:37.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      112 2023-06-13 23:46:37.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    18196 2023-06-13 23:46:43.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17167 2023-06-13 23:46:37.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:37.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:46:43.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1963 2023-06-13 23:46:37.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:43.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:43.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:43.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/src/aws_cdk/aws_cognito_identitypool_alpha/
--rw-r--r--   0 root         (0) root         (0)   132767 2023-06-13 23:46:37.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/src/aws_cdk/aws_cognito_identitypool_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:43.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/src/aws_cdk/aws_cognito_identitypool_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      467 2023-06-13 23:46:37.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/src/aws_cdk/aws_cognito_identitypool_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69184 2023-06-13 23:46:37.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/src/aws_cdk/aws_cognito_identitypool_alpha/_jsii/aws-cognito-identitypool-alpha@2.84.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:37.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/src/aws_cdk/aws_cognito_identitypool_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:43.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18196 2023-06-13 23:46:43.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      661 2023-06-13 23:46:43.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:43.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-13 23:46:43.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:46:43.000000 aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      112 2022-01-26 11:22:01.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    17544 2022-01-26 11:22:05.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16548 2022-01-26 11:22:01.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:05.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-01-26 11:22:01.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/src/aws_cdk/aws_cognito_identitypool_alpha/
+-rw-r--r--   0 root         (0) root         (0)   111650 2022-01-26 11:22:01.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/src/aws_cdk/aws_cognito_identitypool_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/src/aws_cdk/aws_cognito_identitypool_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      431 2022-01-26 11:22:01.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/src/aws_cdk/aws_cognito_identitypool_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58756 2022-01-26 11:22:01.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/src/aws_cdk/aws_cognito_identitypool_alpha/_jsii/aws-cognito-identitypool-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/src/aws_cdk/aws_cognito_identitypool_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17544 2022-01-26 11:22:05.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      660 2022-01-26 11:22:05.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:05.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:05.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:05.000000 aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/LICENSE` & `aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/LICENSE`

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

### Comparing `aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/PKG-INFO` & `aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-cognito-identitypool-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::Cognito Identity Pools
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
 
 # Amazon Cognito Identity Pool Construct Library
 
 > **Identity Pools are in a separate module while the API is being stabilized. Once we stabilize the module, they will**
@@ -52,18 +52,14 @@
 a third party such as Facebook, Amazon, Google or Apple.
 
 The other main component in Amazon Cognito is [user pools](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-identity-pools.html). User Pools are user directories that provide sign-up and
 sign-in options for your app users.
 
 This module is part of the [AWS Cloud Development Kit](https://github.com/aws/aws-cdk) project.
 
-```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPool, UserPoolAuthenticationProvider
-```
-
 ## Table of Contents
 
 * [Identity Pools](#identity-pools)
 
   * [Authenticated and Unauthenticated Identities](#authenticated-and-unauthenticated-identities)
   * [Authentication Providers](#authentication-providers)
 
@@ -94,53 +90,52 @@
 identities, and a default role for unauthenticated identities. Absent other overriding rules (see below), these are the
 roles that will be assumed by the corresponding users in the authentication process.
 
 A basic Identity Pool with minimal configuration has no required props, with default authenticated (user) and
 unauthenticated (guest) roles applied to the identity pool:
 
 ```python
-IdentityPool(self, "myIdentityPool")
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myIdentityPool")
 ```
 
 By default, both the authenticated and unauthenticated roles will have no permissions attached. Grant permissions
 to roles using the public `authenticatedRole` and `unauthenticatedRole` properties:
 
 ```python
-import aws_cdk.aws_dynamodb as dynamodb
-# table: dynamodb.Table
-
-
-identity_pool = IdentityPool(self, "myIdentityPool")
+# Example automatically generated from non-compiling source. May contain errors.
+identity_pool = cognito.IdentityPool(self, "myIdentityPool")
+table = dynamodb.Table(self, "MyTable")
 
 # Grant permissions to authenticated users
 table.grant_read_write_data(identity_pool.authenticated_role)
 # Grant permissions to unauthenticated guest users
-table.grant_read_data(identity_pool.unauthenticated_role)
+table.grant_read(identity_pool.unauthenticated_role)
 
 # Or add policy statements straight to the role
-identity_pool.authenticated_role.add_to_principal_policy(iam.PolicyStatement(
-    effect=iam.Effect.ALLOW,
+identity_pool.authenticated_role.add_to_principal_policy(PolicyStatement(
+    effect=Effect.ALLOW,
     actions=["dynamodb:*"],
     resources=["*"]
 ))
 ```
 
 The default roles can also be supplied in `IdentityPoolProps`:
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 stack = Stack()
-authenticated_role = iam.Role(self, "authRole",
-    assumed_by=iam.ServicePrincipal("service.amazonaws.com")
+authenticated_role = Role(stack, "authRole",
+    assumed_by=ServicePrincipal("service.amazonaws.com")
 )
-unauthenticated_role = iam.Role(self, "unauthRole",
-    assumed_by=iam.ServicePrincipal("service.amazonaws.com")
+unauthenticated_role = Role(stack, "unauthRole",
+    assumed_by=ServicePrincipal("service.amazonaws.com")
 )
-identity_pool = IdentityPool(self, "TestIdentityPoolActions",
-    authenticated_role=authenticated_role,
-    unauthenticated_role=unauthenticated_role
+identity_pool = IdentityPool(stack, "TestIdentityPoolActions",
+    authenticated_role=authenticated_role, unauthenticated_role=unauthenticated_role
 )
 ```
 
 ### Authentication Providers
 
 Authenticated identities belong to users who are authenticated by a public login provider (Amazon Cognito user pools,
 Login with Amazon, Sign in with Apple, Facebook, Google, SAML, or any OpenID Connect Providers) or a developer provider
@@ -152,34 +147,34 @@
 #### User Pool Authentication Provider
 
 In order to attach a user pool to an identity pool as an authentication provider, the identity pool needs properties
 from both the user pool and the user pool client. For this reason identity pools use a `UserPoolAuthenticationProvider`
 to gather the necessary properties from the user pool constructs.
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 user_pool = cognito.UserPool(self, "Pool")
 
-IdentityPool(self, "myidentitypool",
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    authentication_providers=IdentityPoolAuthenticationProviders(
-        user_pools=[UserPoolAuthenticationProvider(user_pool=user_pool)]
-    )
+    authentication_providers={
+        "user_pools": [UserPoolAuthenticationProvider(user_pool=user_pool)]
+    }
 )
 ```
 
 User pools can also be associated with an identity pool after instantiation. The Identity Pool's `addUserPoolAuthentication` method
 returns the User Pool Client that has been created:
 
 ```python
-# identity_pool: IdentityPool
-
+# Example automatically generated from non-compiling source. May contain errors.
 user_pool = cognito.UserPool(self, "Pool")
-user_pool_client = identity_pool.add_user_pool_authentication(UserPoolAuthenticationProvider(
-    user_pool=user_pool
-))
+user_pool_client = identity_pool.add_user_pool_authentication(
+    user_pools=[UserPoolAuthenticationProvider(user_pool=user_pool)]
+)
 ```
 
 #### Server Side Token Check
 
 With the `IdentityPool` CDK Construct, by default the pool is configured to check with the integrated user pools to
 make sure that the user has not been globally signed out or deleted before the identity pool provides an OIDC token or
 AWS credentials for the user.
@@ -187,49 +182,51 @@
 If the user is signed out or deleted, the identity pool will return a 400 Not Authorized error. This setting can be
 disabled, however, in several ways.
 
 Setting `disableServerSideTokenCheck` to true will change the default behavior to no server side token check. Learn
 more [here](https://docs.aws.amazon.com/cognitoidentity/latest/APIReference/API_CognitoIdentityProvider.html#CognitoIdentity-Type-CognitoIdentityProvider-ServerSideTokenCheck):
 
 ```python
-# identity_pool: IdentityPool
-
+# Example automatically generated from non-compiling source. May contain errors.
 user_pool = cognito.UserPool(self, "Pool")
-identity_pool.add_user_pool_authentication(UserPoolAuthenticationProvider(
-    user_pool=user_pool,
-    disable_server_side_token_check=True
-))
+identity_pool.add_user_pool_authentication(
+    user_pool=UserPoolAuthenticationProvider(
+        user_pool=user_pool,
+        disable_server_side_token_check=True
+    )
+)
 ```
 
 #### Associating an External Provider Directly
 
 One or more [external identity providers](https://docs.aws.amazon.com/cognito/latest/developerguide/external-identity-providers.html) can be associated with an identity pool directly using
 `authenticationProviders`:
 
 ```python
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    authentication_providers=IdentityPoolAuthenticationProviders(
-        amazon=IdentityPoolAmazonLoginProvider(
-            app_id="amzn1.application.12312k3j234j13rjiwuenf"
-        ),
-        facebook=IdentityPoolFacebookLoginProvider(
-            app_id="1234567890123"
-        ),
-        google=IdentityPoolGoogleLoginProvider(
-            client_id="12345678012.apps.googleusercontent.com"
-        ),
-        apple=IdentityPoolAppleLoginProvider(
-            services_id="com.myappleapp.auth"
-        ),
-        twitter=IdentityPoolTwitterLoginProvider(
-            consumer_key="my-twitter-id",
-            consumer_secret="my-twitter-secret"
-        )
-    )
+    authentication_providers={
+        "amazon": {
+            "app_id": "amzn1.application.12312k3j234j13rjiwuenf"
+        },
+        "facebook": {
+            "app_id": "1234567890123"
+        },
+        "google": {
+            "client_id": "12345678012.apps.googleusercontent.com"
+        },
+        "apple": {
+            "services_id": "com.myappleapp.auth"
+        },
+        "twitter": {
+            "consumer_key": "my-twitter-id",
+            "consumer_secret": "my-twitter-secret"
+        }
+    }
 )
 ```
 
 To associate more than one provider of the same type with the identity pool, use User
 Pools, OpenIdConnect, or SAML. Only one provider per external service can be attached directly to the identity pool.
 
 #### OpenId Connect and Saml
@@ -240,182 +237,143 @@
 
 An identity provider that supports [Security Assertion Markup Language 2.0 (SAML 2.0)](https://docs.aws.amazon.com/cognito/latest/developerguide/saml-identity-provider.html) can be used to provide a simple
 onboarding flow for users. The SAML-supporting identity provider specifies the IAM roles that can be assumed by users
 so that different users can be granted different sets of permissions. Associating an OpenId Connect or Saml provider
 with an identity pool:
 
 ```python
-# open_id_connect_provider: iam.OpenIdConnectProvider
-# saml_provider: iam.SamlProvider
-
+# Example automatically generated from non-compiling source. May contain errors.
+open_id_connect_provider = iam.OpenIdConnectProvider(self, "my-openid-connect-provider", ...)
+saml_provider = iam.SamlProvider(self, "my-saml-provider", ...)
 
-IdentityPool(self, "myidentitypool",
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    authentication_providers=IdentityPoolAuthenticationProviders(
-        open_id_connect_providers=[open_id_connect_provider],
-        saml_providers=[saml_provider]
-    )
+    authentication_providers={
+        "open_id_connect_provider": open_id_connect_provider,
+        "saml_provider": saml_provider
+    }
 )
 ```
 
 #### Custom Providers
 
 The identity pool's behavior can be customized further using custom [developer authenticated identities](https://docs.aws.amazon.com/cognito/latest/developerguide/developer-authenticated-identities.html).
 With developer authenticated identities, users can be registered and authenticated via an existing authentication
 process while still using Amazon Cognito to synchronize user data and access AWS resources.
 
 Like the supported external providers, though, only one custom provider can be directly associated with the identity
 pool.
 
 ```python
-# open_id_connect_provider: iam.OpenIdConnectProvider
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    authentication_providers=IdentityPoolAuthenticationProviders(
-        google=IdentityPoolGoogleLoginProvider(
-            client_id="12345678012.apps.googleusercontent.com"
-        ),
-        open_id_connect_providers=[open_id_connect_provider],
-        custom_provider="my-custom-provider.example.com"
-    )
+    authentication_providers={
+        "google": "12345678012.apps.googleusercontent.com",
+        "open_id_connect_provider": open_id_connect_provider,
+        "custom_provider": "my-custom-provider.example.com"
+    }
 )
 ```
 
 ### Role Mapping
 
 In addition to setting default roles for authenticated and unauthenticated users, identity pools can also be used to
 define rules to choose the role for each user based on claims in the user's ID token by using Role Mapping. When using
 role mapping, it's important to be aware of some of the permissions the role will need. An in depth
 review of roles and role mapping can be found [here](https://docs.aws.amazon.com/cognito/latest/developerguide/role-based-access-control.html).
 
 Using a [token-based approach](https://docs.aws.amazon.com/cognito/latest/developerguide/role-based-access-control.html#using-tokens-to-assign-roles-to-users) to role mapping will allow mapped roles to be passed through the `cognito:roles` or
 `cognito:preferred_role` claims from the identity provider:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl
-
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    role_mappings=[IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.AMAZON,
-        use_token=True
-    )]
+    role_mappings=[{
+        "provider_url": IdentityPoolProviderUrl.AMAZON,
+        "use_token": True
+    }]
 )
 ```
 
-Using a rule-based approach to role mapping allows roles to be assigned based on custom claims passed from the identity provider:
+Using a rule-based approach to role mapping allows roles to be assigned based on custom claims passed from the identity  provider:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl, RoleMappingMatchType
-
-# admin_role: iam.Role
-# non_admin_role: iam.Role
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
     # Assign specific roles to users based on whether or not the custom admin claim is passed from the identity provider
-    role_mappings=[IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.AMAZON,
-        rules=[RoleMappingRule(
-            claim="custom:admin",
-            claim_value="admin",
-            mapped_role=admin_role
-        ), RoleMappingRule(
-            claim="custom:admin",
-            claim_value="admin",
-            match_type=RoleMappingMatchType.NOTEQUAL,
-            mapped_role=non_admin_role
-        )
+    role_mappings=[{
+        "provider_url": IdentityPoolProviderUrl.AMAZON,
+        "rules": [{
+            "claim": "custom:admin",
+            "claim_value": "admin",
+            "mapped_role": admin_role
+        }, {
+            "claim": "custom:admin",
+            "claim_value": "admin",
+            "match_type": RoleMappingMatchType.NOTEQUAL,
+            "mapped_role": non_admin_role
+        }
         ]
-    )]
+    }]
 )
 ```
 
 Role mappings can also be added after instantiation with the Identity Pool's `addRoleMappings` method:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolRoleMapping
-
-# identity_pool: IdentityPool
-# my_added_role_mapping1: IdentityPoolRoleMapping
-# my_added_role_mapping2: IdentityPoolRoleMapping
-# my_added_role_mapping3: IdentityPoolRoleMapping
-
-
+# Example automatically generated from non-compiling source. May contain errors.
 identity_pool.add_role_mappings(my_added_role_mapping1, my_added_role_mapping2, my_added_role_mapping3)
 ```
 
 #### Provider Urls
 
 Role mappings must be associated with the url of an Identity Provider which can be supplied
 `IdentityPoolProviderUrl`. Supported Providers have static Urls that can be used:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl
-
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    role_mappings=[IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.FACEBOOK,
-        use_token=True
-    )]
+    role_mappings=[{
+        "provider_url": IdentityPoolProviderUrl.FACEBOOK,
+        "use_token": True
+    }]
 )
 ```
 
 For identity providers that don't have static Urls, a custom Url or User Pool Client Url can be supplied:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl
-
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    role_mappings=[IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.user_pool("cognito-idp.my-idp-region.amazonaws.com/my-idp-region_abcdefghi:app_client_id"),
-        use_token=True
-    ), IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.custom("my-custom-provider.com"),
-        use_token=True
-    )
+    role_mappings=[{
+        "provider_url": IdentityPoolProviderUrl.user_pool("cognito-idp.my-idp-region.amazonaws.com/my-idp-region_abcdefghi:app_client_id"),
+        "use_token": True
+    }, {
+        "provider_url": IdentityPoolProviderUrl.custom("my-custom-provider.com"),
+        "use_token": True
+    }
     ]
 )
 ```
 
-If a provider URL is a CDK Token, as it will be if you are trying to use a previously defined Cognito User Pool, you will need to also provide a mappingKey.
-This is because by default, the key in the Cloudformation role mapping hash is the providerUrl, and Cloudformation map keys must be concrete strings, they
-cannot be references. For example:
-
-```python
-from aws_cdk.aws_cognito import UserPool
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl
-
-# user_pool: UserPool
-
-IdentityPool(self, "myidentitypool",
-    identity_pool_name="myidentitypool",
-    role_mappings=[IdentityPoolRoleMapping(
-        mapping_key="cognito",
-        provider_url=IdentityPoolProviderUrl.user_pool(user_pool.user_pool_provider_url),
-        use_token=True
-    )]
-)
-```
-
 See [here](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-cognito-identitypoolroleattachment-rolemapping.html#cfn-cognito-identitypoolroleattachment-rolemapping-identityprovider) for more information.
 
 ### Authentication Flow
 
 Identity Pool [Authentication Flow](https://docs.aws.amazon.com/cognito/latest/developerguide/authentication-flow.html) defaults to the enhanced, simplified flow. The Classic (basic) Authentication Flow
 can also be implemented using `allowClassicFlow`:
 
 ```python
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
     allow_classic_flow=True
 )
 ```
 
 ### Cognito Sync
 
@@ -425,10 +383,13 @@
 
 ### Importing Identity Pools
 
 You can import existing identity pools into your stack using Identity Pool static methods with the Identity Pool Id or
 Arn:
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 IdentityPool.from_identity_pool_id(self, "my-imported-identity-pool", "us-east-1:dj2823ryiwuhef937")
 IdentityPool.from_identity_pool_arn(self, "my-imported-identity-pool", "arn:aws:cognito-identity:us-east-1:123456789012:identitypool/us-east-1:dj2823ryiwuhef937")
 ```
+
+
```

### Comparing `aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/README.md` & `aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -25,18 +25,14 @@
 a third party such as Facebook, Amazon, Google or Apple.
 
 The other main component in Amazon Cognito is [user pools](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-identity-pools.html). User Pools are user directories that provide sign-up and
 sign-in options for your app users.
 
 This module is part of the [AWS Cloud Development Kit](https://github.com/aws/aws-cdk) project.
 
-```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPool, UserPoolAuthenticationProvider
-```
-
 ## Table of Contents
 
 * [Identity Pools](#identity-pools)
 
   * [Authenticated and Unauthenticated Identities](#authenticated-and-unauthenticated-identities)
   * [Authentication Providers](#authentication-providers)
 
@@ -67,53 +63,52 @@
 identities, and a default role for unauthenticated identities. Absent other overriding rules (see below), these are the
 roles that will be assumed by the corresponding users in the authentication process.
 
 A basic Identity Pool with minimal configuration has no required props, with default authenticated (user) and
 unauthenticated (guest) roles applied to the identity pool:
 
 ```python
-IdentityPool(self, "myIdentityPool")
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myIdentityPool")
 ```
 
 By default, both the authenticated and unauthenticated roles will have no permissions attached. Grant permissions
 to roles using the public `authenticatedRole` and `unauthenticatedRole` properties:
 
 ```python
-import aws_cdk.aws_dynamodb as dynamodb
-# table: dynamodb.Table
-
-
-identity_pool = IdentityPool(self, "myIdentityPool")
+# Example automatically generated from non-compiling source. May contain errors.
+identity_pool = cognito.IdentityPool(self, "myIdentityPool")
+table = dynamodb.Table(self, "MyTable")
 
 # Grant permissions to authenticated users
 table.grant_read_write_data(identity_pool.authenticated_role)
 # Grant permissions to unauthenticated guest users
-table.grant_read_data(identity_pool.unauthenticated_role)
+table.grant_read(identity_pool.unauthenticated_role)
 
 # Or add policy statements straight to the role
-identity_pool.authenticated_role.add_to_principal_policy(iam.PolicyStatement(
-    effect=iam.Effect.ALLOW,
+identity_pool.authenticated_role.add_to_principal_policy(PolicyStatement(
+    effect=Effect.ALLOW,
     actions=["dynamodb:*"],
     resources=["*"]
 ))
 ```
 
 The default roles can also be supplied in `IdentityPoolProps`:
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 stack = Stack()
-authenticated_role = iam.Role(self, "authRole",
-    assumed_by=iam.ServicePrincipal("service.amazonaws.com")
+authenticated_role = Role(stack, "authRole",
+    assumed_by=ServicePrincipal("service.amazonaws.com")
 )
-unauthenticated_role = iam.Role(self, "unauthRole",
-    assumed_by=iam.ServicePrincipal("service.amazonaws.com")
+unauthenticated_role = Role(stack, "unauthRole",
+    assumed_by=ServicePrincipal("service.amazonaws.com")
 )
-identity_pool = IdentityPool(self, "TestIdentityPoolActions",
-    authenticated_role=authenticated_role,
-    unauthenticated_role=unauthenticated_role
+identity_pool = IdentityPool(stack, "TestIdentityPoolActions",
+    authenticated_role=authenticated_role, unauthenticated_role=unauthenticated_role
 )
 ```
 
 ### Authentication Providers
 
 Authenticated identities belong to users who are authenticated by a public login provider (Amazon Cognito user pools,
 Login with Amazon, Sign in with Apple, Facebook, Google, SAML, or any OpenID Connect Providers) or a developer provider
@@ -125,34 +120,34 @@
 #### User Pool Authentication Provider
 
 In order to attach a user pool to an identity pool as an authentication provider, the identity pool needs properties
 from both the user pool and the user pool client. For this reason identity pools use a `UserPoolAuthenticationProvider`
 to gather the necessary properties from the user pool constructs.
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 user_pool = cognito.UserPool(self, "Pool")
 
-IdentityPool(self, "myidentitypool",
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    authentication_providers=IdentityPoolAuthenticationProviders(
-        user_pools=[UserPoolAuthenticationProvider(user_pool=user_pool)]
-    )
+    authentication_providers={
+        "user_pools": [UserPoolAuthenticationProvider(user_pool=user_pool)]
+    }
 )
 ```
 
 User pools can also be associated with an identity pool after instantiation. The Identity Pool's `addUserPoolAuthentication` method
 returns the User Pool Client that has been created:
 
 ```python
-# identity_pool: IdentityPool
-
+# Example automatically generated from non-compiling source. May contain errors.
 user_pool = cognito.UserPool(self, "Pool")
-user_pool_client = identity_pool.add_user_pool_authentication(UserPoolAuthenticationProvider(
-    user_pool=user_pool
-))
+user_pool_client = identity_pool.add_user_pool_authentication(
+    user_pools=[UserPoolAuthenticationProvider(user_pool=user_pool)]
+)
 ```
 
 #### Server Side Token Check
 
 With the `IdentityPool` CDK Construct, by default the pool is configured to check with the integrated user pools to
 make sure that the user has not been globally signed out or deleted before the identity pool provides an OIDC token or
 AWS credentials for the user.
@@ -160,49 +155,51 @@
 If the user is signed out or deleted, the identity pool will return a 400 Not Authorized error. This setting can be
 disabled, however, in several ways.
 
 Setting `disableServerSideTokenCheck` to true will change the default behavior to no server side token check. Learn
 more [here](https://docs.aws.amazon.com/cognitoidentity/latest/APIReference/API_CognitoIdentityProvider.html#CognitoIdentity-Type-CognitoIdentityProvider-ServerSideTokenCheck):
 
 ```python
-# identity_pool: IdentityPool
-
+# Example automatically generated from non-compiling source. May contain errors.
 user_pool = cognito.UserPool(self, "Pool")
-identity_pool.add_user_pool_authentication(UserPoolAuthenticationProvider(
-    user_pool=user_pool,
-    disable_server_side_token_check=True
-))
+identity_pool.add_user_pool_authentication(
+    user_pool=UserPoolAuthenticationProvider(
+        user_pool=user_pool,
+        disable_server_side_token_check=True
+    )
+)
 ```
 
 #### Associating an External Provider Directly
 
 One or more [external identity providers](https://docs.aws.amazon.com/cognito/latest/developerguide/external-identity-providers.html) can be associated with an identity pool directly using
 `authenticationProviders`:
 
 ```python
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    authentication_providers=IdentityPoolAuthenticationProviders(
-        amazon=IdentityPoolAmazonLoginProvider(
-            app_id="amzn1.application.12312k3j234j13rjiwuenf"
-        ),
-        facebook=IdentityPoolFacebookLoginProvider(
-            app_id="1234567890123"
-        ),
-        google=IdentityPoolGoogleLoginProvider(
-            client_id="12345678012.apps.googleusercontent.com"
-        ),
-        apple=IdentityPoolAppleLoginProvider(
-            services_id="com.myappleapp.auth"
-        ),
-        twitter=IdentityPoolTwitterLoginProvider(
-            consumer_key="my-twitter-id",
-            consumer_secret="my-twitter-secret"
-        )
-    )
+    authentication_providers={
+        "amazon": {
+            "app_id": "amzn1.application.12312k3j234j13rjiwuenf"
+        },
+        "facebook": {
+            "app_id": "1234567890123"
+        },
+        "google": {
+            "client_id": "12345678012.apps.googleusercontent.com"
+        },
+        "apple": {
+            "services_id": "com.myappleapp.auth"
+        },
+        "twitter": {
+            "consumer_key": "my-twitter-id",
+            "consumer_secret": "my-twitter-secret"
+        }
+    }
 )
 ```
 
 To associate more than one provider of the same type with the identity pool, use User
 Pools, OpenIdConnect, or SAML. Only one provider per external service can be attached directly to the identity pool.
 
 #### OpenId Connect and Saml
@@ -213,182 +210,143 @@
 
 An identity provider that supports [Security Assertion Markup Language 2.0 (SAML 2.0)](https://docs.aws.amazon.com/cognito/latest/developerguide/saml-identity-provider.html) can be used to provide a simple
 onboarding flow for users. The SAML-supporting identity provider specifies the IAM roles that can be assumed by users
 so that different users can be granted different sets of permissions. Associating an OpenId Connect or Saml provider
 with an identity pool:
 
 ```python
-# open_id_connect_provider: iam.OpenIdConnectProvider
-# saml_provider: iam.SamlProvider
-
+# Example automatically generated from non-compiling source. May contain errors.
+open_id_connect_provider = iam.OpenIdConnectProvider(self, "my-openid-connect-provider", ...)
+saml_provider = iam.SamlProvider(self, "my-saml-provider", ...)
 
-IdentityPool(self, "myidentitypool",
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    authentication_providers=IdentityPoolAuthenticationProviders(
-        open_id_connect_providers=[open_id_connect_provider],
-        saml_providers=[saml_provider]
-    )
+    authentication_providers={
+        "open_id_connect_provider": open_id_connect_provider,
+        "saml_provider": saml_provider
+    }
 )
 ```
 
 #### Custom Providers
 
 The identity pool's behavior can be customized further using custom [developer authenticated identities](https://docs.aws.amazon.com/cognito/latest/developerguide/developer-authenticated-identities.html).
 With developer authenticated identities, users can be registered and authenticated via an existing authentication
 process while still using Amazon Cognito to synchronize user data and access AWS resources.
 
 Like the supported external providers, though, only one custom provider can be directly associated with the identity
 pool.
 
 ```python
-# open_id_connect_provider: iam.OpenIdConnectProvider
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    authentication_providers=IdentityPoolAuthenticationProviders(
-        google=IdentityPoolGoogleLoginProvider(
-            client_id="12345678012.apps.googleusercontent.com"
-        ),
-        open_id_connect_providers=[open_id_connect_provider],
-        custom_provider="my-custom-provider.example.com"
-    )
+    authentication_providers={
+        "google": "12345678012.apps.googleusercontent.com",
+        "open_id_connect_provider": open_id_connect_provider,
+        "custom_provider": "my-custom-provider.example.com"
+    }
 )
 ```
 
 ### Role Mapping
 
 In addition to setting default roles for authenticated and unauthenticated users, identity pools can also be used to
 define rules to choose the role for each user based on claims in the user's ID token by using Role Mapping. When using
 role mapping, it's important to be aware of some of the permissions the role will need. An in depth
 review of roles and role mapping can be found [here](https://docs.aws.amazon.com/cognito/latest/developerguide/role-based-access-control.html).
 
 Using a [token-based approach](https://docs.aws.amazon.com/cognito/latest/developerguide/role-based-access-control.html#using-tokens-to-assign-roles-to-users) to role mapping will allow mapped roles to be passed through the `cognito:roles` or
 `cognito:preferred_role` claims from the identity provider:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl
-
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    role_mappings=[IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.AMAZON,
-        use_token=True
-    )]
+    role_mappings=[{
+        "provider_url": IdentityPoolProviderUrl.AMAZON,
+        "use_token": True
+    }]
 )
 ```
 
-Using a rule-based approach to role mapping allows roles to be assigned based on custom claims passed from the identity provider:
+Using a rule-based approach to role mapping allows roles to be assigned based on custom claims passed from the identity  provider:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl, RoleMappingMatchType
-
-# admin_role: iam.Role
-# non_admin_role: iam.Role
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
     # Assign specific roles to users based on whether or not the custom admin claim is passed from the identity provider
-    role_mappings=[IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.AMAZON,
-        rules=[RoleMappingRule(
-            claim="custom:admin",
-            claim_value="admin",
-            mapped_role=admin_role
-        ), RoleMappingRule(
-            claim="custom:admin",
-            claim_value="admin",
-            match_type=RoleMappingMatchType.NOTEQUAL,
-            mapped_role=non_admin_role
-        )
+    role_mappings=[{
+        "provider_url": IdentityPoolProviderUrl.AMAZON,
+        "rules": [{
+            "claim": "custom:admin",
+            "claim_value": "admin",
+            "mapped_role": admin_role
+        }, {
+            "claim": "custom:admin",
+            "claim_value": "admin",
+            "match_type": RoleMappingMatchType.NOTEQUAL,
+            "mapped_role": non_admin_role
+        }
         ]
-    )]
+    }]
 )
 ```
 
 Role mappings can also be added after instantiation with the Identity Pool's `addRoleMappings` method:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolRoleMapping
-
-# identity_pool: IdentityPool
-# my_added_role_mapping1: IdentityPoolRoleMapping
-# my_added_role_mapping2: IdentityPoolRoleMapping
-# my_added_role_mapping3: IdentityPoolRoleMapping
-
-
+# Example automatically generated from non-compiling source. May contain errors.
 identity_pool.add_role_mappings(my_added_role_mapping1, my_added_role_mapping2, my_added_role_mapping3)
 ```
 
 #### Provider Urls
 
 Role mappings must be associated with the url of an Identity Provider which can be supplied
 `IdentityPoolProviderUrl`. Supported Providers have static Urls that can be used:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl
-
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    role_mappings=[IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.FACEBOOK,
-        use_token=True
-    )]
+    role_mappings=[{
+        "provider_url": IdentityPoolProviderUrl.FACEBOOK,
+        "use_token": True
+    }]
 )
 ```
 
 For identity providers that don't have static Urls, a custom Url or User Pool Client Url can be supplied:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl
-
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    role_mappings=[IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.user_pool("cognito-idp.my-idp-region.amazonaws.com/my-idp-region_abcdefghi:app_client_id"),
-        use_token=True
-    ), IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.custom("my-custom-provider.com"),
-        use_token=True
-    )
+    role_mappings=[{
+        "provider_url": IdentityPoolProviderUrl.user_pool("cognito-idp.my-idp-region.amazonaws.com/my-idp-region_abcdefghi:app_client_id"),
+        "use_token": True
+    }, {
+        "provider_url": IdentityPoolProviderUrl.custom("my-custom-provider.com"),
+        "use_token": True
+    }
     ]
 )
 ```
 
-If a provider URL is a CDK Token, as it will be if you are trying to use a previously defined Cognito User Pool, you will need to also provide a mappingKey.
-This is because by default, the key in the Cloudformation role mapping hash is the providerUrl, and Cloudformation map keys must be concrete strings, they
-cannot be references. For example:
-
-```python
-from aws_cdk.aws_cognito import UserPool
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl
-
-# user_pool: UserPool
-
-IdentityPool(self, "myidentitypool",
-    identity_pool_name="myidentitypool",
-    role_mappings=[IdentityPoolRoleMapping(
-        mapping_key="cognito",
-        provider_url=IdentityPoolProviderUrl.user_pool(user_pool.user_pool_provider_url),
-        use_token=True
-    )]
-)
-```
-
 See [here](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-cognito-identitypoolroleattachment-rolemapping.html#cfn-cognito-identitypoolroleattachment-rolemapping-identityprovider) for more information.
 
 ### Authentication Flow
 
 Identity Pool [Authentication Flow](https://docs.aws.amazon.com/cognito/latest/developerguide/authentication-flow.html) defaults to the enhanced, simplified flow. The Classic (basic) Authentication Flow
 can also be implemented using `allowClassicFlow`:
 
 ```python
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
     allow_classic_flow=True
 )
 ```
 
 ### Cognito Sync
 
@@ -398,10 +356,11 @@
 
 ### Importing Identity Pools
 
 You can import existing identity pools into your stack using Identity Pool static methods with the Identity Pool Id or
 Arn:
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 IdentityPool.from_identity_pool_id(self, "my-imported-identity-pool", "us-east-1:dj2823ryiwuhef937")
 IdentityPool.from_identity_pool_arn(self, "my-imported-identity-pool", "arn:aws:cognito-identity:us-east-1:123456789012:identitypool/us-east-1:dj2823ryiwuhef937")
 ```
```

### Comparing `aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/setup.py` & `aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-cognito-identitypool-alpha",
-    "version": "2.84.0.a0",
+    "version": "2.9.0.a0",
     "description": "The CDK Construct Library for AWS::Cognito Identity Pools",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,43 +22,41 @@
     },
     "packages": [
         "aws_cdk.aws_cognito_identitypool_alpha",
         "aws_cdk.aws_cognito_identitypool_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_cognito_identitypool_alpha._jsii": [
-            "aws-cognito-identitypool-alpha@2.84.0-alpha.0.jsii.tgz"
+            "aws-cognito-identitypool-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_cognito_identitypool_alpha": [
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

### Comparing `aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/src/aws_cdk/aws_cognito_identitypool_alpha/__init__.py` & `aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/src/aws_cdk/aws_cognito_identitypool_alpha/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,18 +26,14 @@
 a third party such as Facebook, Amazon, Google or Apple.
 
 The other main component in Amazon Cognito is [user pools](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-identity-pools.html). User Pools are user directories that provide sign-up and
 sign-in options for your app users.
 
 This module is part of the [AWS Cloud Development Kit](https://github.com/aws/aws-cdk) project.
 
-```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPool, UserPoolAuthenticationProvider
-```
-
 ## Table of Contents
 
 * [Identity Pools](#identity-pools)
 
   * [Authenticated and Unauthenticated Identities](#authenticated-and-unauthenticated-identities)
   * [Authentication Providers](#authentication-providers)
 
@@ -68,53 +64,52 @@
 identities, and a default role for unauthenticated identities. Absent other overriding rules (see below), these are the
 roles that will be assumed by the corresponding users in the authentication process.
 
 A basic Identity Pool with minimal configuration has no required props, with default authenticated (user) and
 unauthenticated (guest) roles applied to the identity pool:
 
 ```python
-IdentityPool(self, "myIdentityPool")
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myIdentityPool")
 ```
 
 By default, both the authenticated and unauthenticated roles will have no permissions attached. Grant permissions
 to roles using the public `authenticatedRole` and `unauthenticatedRole` properties:
 
 ```python
-import aws_cdk.aws_dynamodb as dynamodb
-# table: dynamodb.Table
-
-
-identity_pool = IdentityPool(self, "myIdentityPool")
+# Example automatically generated from non-compiling source. May contain errors.
+identity_pool = cognito.IdentityPool(self, "myIdentityPool")
+table = dynamodb.Table(self, "MyTable")
 
 # Grant permissions to authenticated users
 table.grant_read_write_data(identity_pool.authenticated_role)
 # Grant permissions to unauthenticated guest users
-table.grant_read_data(identity_pool.unauthenticated_role)
+table.grant_read(identity_pool.unauthenticated_role)
 
 # Or add policy statements straight to the role
-identity_pool.authenticated_role.add_to_principal_policy(iam.PolicyStatement(
-    effect=iam.Effect.ALLOW,
+identity_pool.authenticated_role.add_to_principal_policy(PolicyStatement(
+    effect=Effect.ALLOW,
     actions=["dynamodb:*"],
     resources=["*"]
 ))
 ```
 
 The default roles can also be supplied in `IdentityPoolProps`:
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 stack = Stack()
-authenticated_role = iam.Role(self, "authRole",
-    assumed_by=iam.ServicePrincipal("service.amazonaws.com")
+authenticated_role = Role(stack, "authRole",
+    assumed_by=ServicePrincipal("service.amazonaws.com")
 )
-unauthenticated_role = iam.Role(self, "unauthRole",
-    assumed_by=iam.ServicePrincipal("service.amazonaws.com")
+unauthenticated_role = Role(stack, "unauthRole",
+    assumed_by=ServicePrincipal("service.amazonaws.com")
 )
-identity_pool = IdentityPool(self, "TestIdentityPoolActions",
-    authenticated_role=authenticated_role,
-    unauthenticated_role=unauthenticated_role
+identity_pool = IdentityPool(stack, "TestIdentityPoolActions",
+    authenticated_role=authenticated_role, unauthenticated_role=unauthenticated_role
 )
 ```
 
 ### Authentication Providers
 
 Authenticated identities belong to users who are authenticated by a public login provider (Amazon Cognito user pools,
 Login with Amazon, Sign in with Apple, Facebook, Google, SAML, or any OpenID Connect Providers) or a developer provider
@@ -126,34 +121,34 @@
 #### User Pool Authentication Provider
 
 In order to attach a user pool to an identity pool as an authentication provider, the identity pool needs properties
 from both the user pool and the user pool client. For this reason identity pools use a `UserPoolAuthenticationProvider`
 to gather the necessary properties from the user pool constructs.
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 user_pool = cognito.UserPool(self, "Pool")
 
-IdentityPool(self, "myidentitypool",
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    authentication_providers=IdentityPoolAuthenticationProviders(
-        user_pools=[UserPoolAuthenticationProvider(user_pool=user_pool)]
-    )
+    authentication_providers={
+        "user_pools": [UserPoolAuthenticationProvider(user_pool=user_pool)]
+    }
 )
 ```
 
 User pools can also be associated with an identity pool after instantiation. The Identity Pool's `addUserPoolAuthentication` method
 returns the User Pool Client that has been created:
 
 ```python
-# identity_pool: IdentityPool
-
+# Example automatically generated from non-compiling source. May contain errors.
 user_pool = cognito.UserPool(self, "Pool")
-user_pool_client = identity_pool.add_user_pool_authentication(UserPoolAuthenticationProvider(
-    user_pool=user_pool
-))
+user_pool_client = identity_pool.add_user_pool_authentication(
+    user_pools=[UserPoolAuthenticationProvider(user_pool=user_pool)]
+)
 ```
 
 #### Server Side Token Check
 
 With the `IdentityPool` CDK Construct, by default the pool is configured to check with the integrated user pools to
 make sure that the user has not been globally signed out or deleted before the identity pool provides an OIDC token or
 AWS credentials for the user.
@@ -161,49 +156,51 @@
 If the user is signed out or deleted, the identity pool will return a 400 Not Authorized error. This setting can be
 disabled, however, in several ways.
 
 Setting `disableServerSideTokenCheck` to true will change the default behavior to no server side token check. Learn
 more [here](https://docs.aws.amazon.com/cognitoidentity/latest/APIReference/API_CognitoIdentityProvider.html#CognitoIdentity-Type-CognitoIdentityProvider-ServerSideTokenCheck):
 
 ```python
-# identity_pool: IdentityPool
-
+# Example automatically generated from non-compiling source. May contain errors.
 user_pool = cognito.UserPool(self, "Pool")
-identity_pool.add_user_pool_authentication(UserPoolAuthenticationProvider(
-    user_pool=user_pool,
-    disable_server_side_token_check=True
-))
+identity_pool.add_user_pool_authentication(
+    user_pool=UserPoolAuthenticationProvider(
+        user_pool=user_pool,
+        disable_server_side_token_check=True
+    )
+)
 ```
 
 #### Associating an External Provider Directly
 
 One or more [external identity providers](https://docs.aws.amazon.com/cognito/latest/developerguide/external-identity-providers.html) can be associated with an identity pool directly using
 `authenticationProviders`:
 
 ```python
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    authentication_providers=IdentityPoolAuthenticationProviders(
-        amazon=IdentityPoolAmazonLoginProvider(
-            app_id="amzn1.application.12312k3j234j13rjiwuenf"
-        ),
-        facebook=IdentityPoolFacebookLoginProvider(
-            app_id="1234567890123"
-        ),
-        google=IdentityPoolGoogleLoginProvider(
-            client_id="12345678012.apps.googleusercontent.com"
-        ),
-        apple=IdentityPoolAppleLoginProvider(
-            services_id="com.myappleapp.auth"
-        ),
-        twitter=IdentityPoolTwitterLoginProvider(
-            consumer_key="my-twitter-id",
-            consumer_secret="my-twitter-secret"
-        )
-    )
+    authentication_providers={
+        "amazon": {
+            "app_id": "amzn1.application.12312k3j234j13rjiwuenf"
+        },
+        "facebook": {
+            "app_id": "1234567890123"
+        },
+        "google": {
+            "client_id": "12345678012.apps.googleusercontent.com"
+        },
+        "apple": {
+            "services_id": "com.myappleapp.auth"
+        },
+        "twitter": {
+            "consumer_key": "my-twitter-id",
+            "consumer_secret": "my-twitter-secret"
+        }
+    }
 )
 ```
 
 To associate more than one provider of the same type with the identity pool, use User
 Pools, OpenIdConnect, or SAML. Only one provider per external service can be attached directly to the identity pool.
 
 #### OpenId Connect and Saml
@@ -214,182 +211,143 @@
 
 An identity provider that supports [Security Assertion Markup Language 2.0 (SAML 2.0)](https://docs.aws.amazon.com/cognito/latest/developerguide/saml-identity-provider.html) can be used to provide a simple
 onboarding flow for users. The SAML-supporting identity provider specifies the IAM roles that can be assumed by users
 so that different users can be granted different sets of permissions. Associating an OpenId Connect or Saml provider
 with an identity pool:
 
 ```python
-# open_id_connect_provider: iam.OpenIdConnectProvider
-# saml_provider: iam.SamlProvider
+# Example automatically generated from non-compiling source. May contain errors.
+open_id_connect_provider = iam.OpenIdConnectProvider(self, "my-openid-connect-provider", ...)
+saml_provider = iam.SamlProvider(self, "my-saml-provider", ...)
 
-
-IdentityPool(self, "myidentitypool",
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    authentication_providers=IdentityPoolAuthenticationProviders(
-        open_id_connect_providers=[open_id_connect_provider],
-        saml_providers=[saml_provider]
-    )
+    authentication_providers={
+        "open_id_connect_provider": open_id_connect_provider,
+        "saml_provider": saml_provider
+    }
 )
 ```
 
 #### Custom Providers
 
 The identity pool's behavior can be customized further using custom [developer authenticated identities](https://docs.aws.amazon.com/cognito/latest/developerguide/developer-authenticated-identities.html).
 With developer authenticated identities, users can be registered and authenticated via an existing authentication
 process while still using Amazon Cognito to synchronize user data and access AWS resources.
 
 Like the supported external providers, though, only one custom provider can be directly associated with the identity
 pool.
 
 ```python
-# open_id_connect_provider: iam.OpenIdConnectProvider
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    authentication_providers=IdentityPoolAuthenticationProviders(
-        google=IdentityPoolGoogleLoginProvider(
-            client_id="12345678012.apps.googleusercontent.com"
-        ),
-        open_id_connect_providers=[open_id_connect_provider],
-        custom_provider="my-custom-provider.example.com"
-    )
+    authentication_providers={
+        "google": "12345678012.apps.googleusercontent.com",
+        "open_id_connect_provider": open_id_connect_provider,
+        "custom_provider": "my-custom-provider.example.com"
+    }
 )
 ```
 
 ### Role Mapping
 
 In addition to setting default roles for authenticated and unauthenticated users, identity pools can also be used to
 define rules to choose the role for each user based on claims in the user's ID token by using Role Mapping. When using
 role mapping, it's important to be aware of some of the permissions the role will need. An in depth
 review of roles and role mapping can be found [here](https://docs.aws.amazon.com/cognito/latest/developerguide/role-based-access-control.html).
 
 Using a [token-based approach](https://docs.aws.amazon.com/cognito/latest/developerguide/role-based-access-control.html#using-tokens-to-assign-roles-to-users) to role mapping will allow mapped roles to be passed through the `cognito:roles` or
 `cognito:preferred_role` claims from the identity provider:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl
-
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    role_mappings=[IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.AMAZON,
-        use_token=True
-    )]
+    role_mappings=[{
+        "provider_url": IdentityPoolProviderUrl.AMAZON,
+        "use_token": True
+    }]
 )
 ```
 
-Using a rule-based approach to role mapping allows roles to be assigned based on custom claims passed from the identity provider:
+Using a rule-based approach to role mapping allows roles to be assigned based on custom claims passed from the identity  provider:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl, RoleMappingMatchType
-
-# admin_role: iam.Role
-# non_admin_role: iam.Role
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
     # Assign specific roles to users based on whether or not the custom admin claim is passed from the identity provider
-    role_mappings=[IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.AMAZON,
-        rules=[RoleMappingRule(
-            claim="custom:admin",
-            claim_value="admin",
-            mapped_role=admin_role
-        ), RoleMappingRule(
-            claim="custom:admin",
-            claim_value="admin",
-            match_type=RoleMappingMatchType.NOTEQUAL,
-            mapped_role=non_admin_role
-        )
+    role_mappings=[{
+        "provider_url": IdentityPoolProviderUrl.AMAZON,
+        "rules": [{
+            "claim": "custom:admin",
+            "claim_value": "admin",
+            "mapped_role": admin_role
+        }, {
+            "claim": "custom:admin",
+            "claim_value": "admin",
+            "match_type": RoleMappingMatchType.NOTEQUAL,
+            "mapped_role": non_admin_role
+        }
         ]
-    )]
+    }]
 )
 ```
 
 Role mappings can also be added after instantiation with the Identity Pool's `addRoleMappings` method:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolRoleMapping
-
-# identity_pool: IdentityPool
-# my_added_role_mapping1: IdentityPoolRoleMapping
-# my_added_role_mapping2: IdentityPoolRoleMapping
-# my_added_role_mapping3: IdentityPoolRoleMapping
-
-
+# Example automatically generated from non-compiling source. May contain errors.
 identity_pool.add_role_mappings(my_added_role_mapping1, my_added_role_mapping2, my_added_role_mapping3)
 ```
 
 #### Provider Urls
 
 Role mappings must be associated with the url of an Identity Provider which can be supplied
 `IdentityPoolProviderUrl`. Supported Providers have static Urls that can be used:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl
-
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    role_mappings=[IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.FACEBOOK,
-        use_token=True
-    )]
+    role_mappings=[{
+        "provider_url": IdentityPoolProviderUrl.FACEBOOK,
+        "use_token": True
+    }]
 )
 ```
 
 For identity providers that don't have static Urls, a custom Url or User Pool Client Url can be supplied:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl
-
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    role_mappings=[IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.user_pool("cognito-idp.my-idp-region.amazonaws.com/my-idp-region_abcdefghi:app_client_id"),
-        use_token=True
-    ), IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.custom("my-custom-provider.com"),
-        use_token=True
-    )
+    role_mappings=[{
+        "provider_url": IdentityPoolProviderUrl.user_pool("cognito-idp.my-idp-region.amazonaws.com/my-idp-region_abcdefghi:app_client_id"),
+        "use_token": True
+    }, {
+        "provider_url": IdentityPoolProviderUrl.custom("my-custom-provider.com"),
+        "use_token": True
+    }
     ]
 )
 ```
 
-If a provider URL is a CDK Token, as it will be if you are trying to use a previously defined Cognito User Pool, you will need to also provide a mappingKey.
-This is because by default, the key in the Cloudformation role mapping hash is the providerUrl, and Cloudformation map keys must be concrete strings, they
-cannot be references. For example:
-
-```python
-from aws_cdk.aws_cognito import UserPool
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl
-
-# user_pool: UserPool
-
-IdentityPool(self, "myidentitypool",
-    identity_pool_name="myidentitypool",
-    role_mappings=[IdentityPoolRoleMapping(
-        mapping_key="cognito",
-        provider_url=IdentityPoolProviderUrl.user_pool(user_pool.user_pool_provider_url),
-        use_token=True
-    )]
-)
-```
-
 See [here](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-cognito-identitypoolroleattachment-rolemapping.html#cfn-cognito-identitypoolroleattachment-rolemapping-identityprovider) for more information.
 
 ### Authentication Flow
 
 Identity Pool [Authentication Flow](https://docs.aws.amazon.com/cognito/latest/developerguide/authentication-flow.html) defaults to the enhanced, simplified flow. The Classic (basic) Authentication Flow
 can also be implemented using `allowClassicFlow`:
 
 ```python
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
     allow_classic_flow=True
 )
 ```
 
 ### Cognito Sync
 
@@ -399,107 +357,106 @@
 
 ### Importing Identity Pools
 
 You can import existing identity pools into your stack using Identity Pool static methods with the Identity Pool Id or
 Arn:
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 IdentityPool.from_identity_pool_id(self, "my-imported-identity-pool", "us-east-1:dj2823ryiwuhef937")
 IdentityPool.from_identity_pool_arn(self, "my-imported-identity-pool", "arn:aws:cognito-identity:us-east-1:123456789012:identitypool/us-east-1:dj2823ryiwuhef937")
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
-import aws_cdk.aws_cognito as _aws_cdk_aws_cognito_ceddda9d
-import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
-import constructs as _constructs_77d1e7e8
+import aws_cdk
+import aws_cdk.aws_cognito
+import aws_cdk.aws_iam
+import constructs
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-cognito-identitypool-alpha.IIdentityPool")
-class IIdentityPool(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+class IIdentityPool(aws_cdk.IResource, typing_extensions.Protocol):
     '''(experimental) Represents a Cognito IdentityPool.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="identityPoolArn")
     def identity_pool_arn(self) -> builtins.str:
         '''(experimental) The ARN of the Identity Pool.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="identityPoolId")
     def identity_pool_id(self) -> builtins.str:
         '''(experimental) The id of the Identity Pool in the format REGION:GUID.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="identityPoolName")
     def identity_pool_name(self) -> builtins.str:
         '''(experimental) Name of the Identity Pool.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _IIdentityPoolProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''(experimental) Represents a Cognito IdentityPool.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-cognito-identitypool-alpha.IIdentityPool"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="identityPoolArn")
     def identity_pool_arn(self) -> builtins.str:
         '''(experimental) The ARN of the Identity Pool.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "identityPoolArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="identityPoolId")
     def identity_pool_id(self) -> builtins.str:
         '''(experimental) The id of the Identity Pool in the format REGION:GUID.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "identityPoolId"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="identityPoolName")
     def identity_pool_name(self) -> builtins.str:
         '''(experimental) Name of the Identity Pool.
 
         :stability: experimental
         :attribute: true
         '''
@@ -508,44 +465,41 @@
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IIdentityPool).__jsii_proxy_class__ = lambda : _IIdentityPoolProxy
 
 
 @jsii.interface(
     jsii_type="@aws-cdk/aws-cognito-identitypool-alpha.IIdentityPoolRoleAttachment"
 )
-class IIdentityPoolRoleAttachment(
-    _aws_cdk_ceddda9d.IResource,
-    typing_extensions.Protocol,
-):
+class IIdentityPoolRoleAttachment(aws_cdk.IResource, typing_extensions.Protocol):
     '''(experimental) Represents an Identity Pool Role Attachment.
 
     :stability: experimental
     '''
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="identityPoolId")
     def identity_pool_id(self) -> builtins.str:
         '''(experimental) Id of the Attachments Underlying Identity Pool.
 
         :stability: experimental
         '''
         ...
 
 
 class _IIdentityPoolRoleAttachmentProxy(
-    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
 ):
     '''(experimental) Represents an Identity Pool Role Attachment.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-cognito-identitypool-alpha.IIdentityPoolRoleAttachment"
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="identityPoolId")
     def identity_pool_id(self) -> builtins.str:
         '''(experimental) Id of the Attachments Underlying Identity Pool.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "identityPoolId"))
@@ -565,15 +519,15 @@
 
     :stability: experimental
     '''
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         identity_pool: IIdentityPool,
     ) -> "UserPoolAuthenticationProviderBindConfig":
         '''(experimental) The method called when a given User Pool Authentication Provider is added (for the first time) to an Identity Pool.
 
         :param scope: -
         :param identity_pool: -
 
@@ -592,272 +546,278 @@
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-cognito-identitypool-alpha.IUserPoolAuthenticationProvider"
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         identity_pool: IIdentityPool,
     ) -> "UserPoolAuthenticationProviderBindConfig":
         '''(experimental) The method called when a given User Pool Authentication Provider is added (for the first time) to an Identity Pool.
 
         :param scope: -
         :param identity_pool: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__07632ef1025feb6e05894b02941c351317dc03c46357f2c76f22433d4b28396c)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument identity_pool", value=identity_pool, expected_type=type_hints["identity_pool"])
         options = UserPoolAuthenticationProviderBindOptions()
 
         return typing.cast("UserPoolAuthenticationProviderBindConfig", jsii.invoke(self, "bind", [scope, identity_pool, options]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IUserPoolAuthenticationProvider).__jsii_proxy_class__ = lambda : _IUserPoolAuthenticationProviderProxy
 
 
 @jsii.implements(IIdentityPool)
 class IdentityPool(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-cognito-identitypool-alpha.IdentityPool",
 ):
     '''(experimental) Define a Cognito Identity Pool.
 
     :stability: experimental
     :resource: AWS::Cognito::IdentityPool
-    :exampleMetadata: infused
+    :exampleMetadata: fixture=_generated
 
     Example::
 
+        # The code below shows an example of how to instantiate this type.
+        # The values are placeholders you should change.
+        import aws_cdk.aws_cognito_identitypool_alpha as cognito_identitypool_alpha
+        from aws_cdk import aws_iam as iam
+        
+        # identity_pool_provider_url: cognito_identitypool_alpha.IdentityPoolProviderUrl
         # open_id_connect_provider: iam.OpenIdConnectProvider
+        # role: iam.Role
+        # saml_provider: iam.SamlProvider
+        # user_pool_authentication_provider: cognito_identitypool_alpha.UserPoolAuthenticationProvider
         
-        IdentityPool(self, "myidentitypool",
-            identity_pool_name="myidentitypool",
-            authentication_providers=IdentityPoolAuthenticationProviders(
-                google=IdentityPoolGoogleLoginProvider(
-                    client_id="12345678012.apps.googleusercontent.com"
+        identity_pool = cognito_identitypool_alpha.IdentityPool(self, "MyIdentityPool",
+            allow_classic_flow=False,
+            allow_unauthenticated_identities=False,
+            authenticated_role=role,
+            authentication_providers=cognito_identitypool_alpha.IdentityPoolAuthenticationProviders(
+                amazon=cognito_identitypool_alpha.IdentityPoolAmazonLoginProvider(
+                    app_id="appId"
+                ),
+                apple=cognito_identitypool_alpha.IdentityPoolAppleLoginProvider(
+                    services_id="servicesId"
+                ),
+                custom_provider="customProvider",
+                digits=cognito_identitypool_alpha.IdentityPoolDigitsLoginProvider(
+                    consumer_key="consumerKey",
+                    consumer_secret="consumerSecret"
+                ),
+                facebook=cognito_identitypool_alpha.IdentityPoolFacebookLoginProvider(
+                    app_id="appId"
+                ),
+                google=cognito_identitypool_alpha.IdentityPoolGoogleLoginProvider(
+                    client_id="clientId"
                 ),
                 open_id_connect_providers=[open_id_connect_provider],
-                custom_provider="my-custom-provider.example.com"
-            )
+                saml_providers=[saml_provider],
+                twitter=cognito_identitypool_alpha.IdentityPoolTwitterLoginProvider(
+                    consumer_key="consumerKey",
+                    consumer_secret="consumerSecret"
+                ),
+                user_pools=[user_pool_authentication_provider]
+            ),
+            identity_pool_name="identityPoolName",
+            role_mappings=[cognito_identitypool_alpha.IdentityPoolRoleMapping(
+                provider_url=identity_pool_provider_url,
+        
+                # the properties below are optional
+                resolve_ambiguous_roles=False,
+                rules=[cognito_identitypool_alpha.RoleMappingRule(
+                    claim="claim",
+                    claim_value="claimValue",
+                    mapped_role=role,
+        
+                    # the properties below are optional
+                    match_type=cognito_identitypool_alpha.RoleMappingMatchType.EQUALS
+                )],
+                use_token=False
+            )],
+            unauthenticated_role=role
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         allow_classic_flow: typing.Optional[builtins.bool] = None,
         allow_unauthenticated_identities: typing.Optional[builtins.bool] = None,
-        authenticated_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-        authentication_providers: typing.Optional[typing.Union["IdentityPoolAuthenticationProviders", typing.Dict[builtins.str, typing.Any]]] = None,
+        authenticated_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
+        authentication_providers: typing.Optional["IdentityPoolAuthenticationProviders"] = None,
         identity_pool_name: typing.Optional[builtins.str] = None,
-        role_mappings: typing.Optional[typing.Sequence[typing.Union["IdentityPoolRoleMapping", typing.Dict[builtins.str, typing.Any]]]] = None,
-        unauthenticated_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        role_mappings: typing.Optional[typing.Sequence["IdentityPoolRoleMapping"]] = None,
+        unauthenticated_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param allow_classic_flow: (experimental) Enables the Basic (Classic) authentication flow. Default: - Classic Flow not allowed
         :param allow_unauthenticated_identities: (experimental) Wwhether the identity pool supports unauthenticated logins. Default: - false
         :param authenticated_role: (experimental) The Default Role to be assumed by Authenticated Users. Default: - A Default Authenticated Role will be added
         :param authentication_providers: (experimental) Authentication providers for using in identity pool. Default: - No Authentication Providers passed directly to Identity Pool
         :param identity_pool_name: (experimental) The name of the Identity Pool. Default: - automatically generated name by CloudFormation at deploy time
         :param role_mappings: (experimental) Rules for mapping roles to users. Default: - no Role Mappings
         :param unauthenticated_role: (experimental) The Default Role to be assumed by Unauthenticated Users. Default: - A Default Unauthenticated Role will be added
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__af2f072d5cac259fbc65a0c4a6a8cb785ff9ebcf2da91f9184be84a22820a980)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = IdentityPoolProps(
             allow_classic_flow=allow_classic_flow,
             allow_unauthenticated_identities=allow_unauthenticated_identities,
             authenticated_role=authenticated_role,
             authentication_providers=authentication_providers,
             identity_pool_name=identity_pool_name,
             role_mappings=role_mappings,
             unauthenticated_role=unauthenticated_role,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromIdentityPoolArn")
+    @jsii.member(jsii_name="fromIdentityPoolArn") # type: ignore[misc]
     @builtins.classmethod
     def from_identity_pool_arn(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         identity_pool_arn: builtins.str,
     ) -> IIdentityPool:
         '''(experimental) Import an existing Identity Pool from its Arn.
 
         :param scope: -
         :param id: -
         :param identity_pool_arn: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a95e191d26141b46fee8d2cdcabc0803b18860942f1a248701db0dae81123def)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument identity_pool_arn", value=identity_pool_arn, expected_type=type_hints["identity_pool_arn"])
         return typing.cast(IIdentityPool, jsii.sinvoke(cls, "fromIdentityPoolArn", [scope, id, identity_pool_arn]))
 
-    @jsii.member(jsii_name="fromIdentityPoolId")
+    @jsii.member(jsii_name="fromIdentityPoolId") # type: ignore[misc]
     @builtins.classmethod
     def from_identity_pool_id(
         cls,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         identity_pool_id: builtins.str,
     ) -> IIdentityPool:
         '''(experimental) Import an existing Identity Pool from its id.
 
         :param scope: -
         :param id: -
         :param identity_pool_id: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b5abb9f2926d1e1f17a15fd6b4211f8951279c31ec22f381103f75200b458fa1)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument identity_pool_id", value=identity_pool_id, expected_type=type_hints["identity_pool_id"])
         return typing.cast(IIdentityPool, jsii.sinvoke(cls, "fromIdentityPoolId", [scope, id, identity_pool_id]))
 
     @jsii.member(jsii_name="addRoleMappings")
     def add_role_mappings(self, *role_mappings: "IdentityPoolRoleMapping") -> None:
         '''(experimental) Adds Role Mappings to Identity Pool.
 
         :param role_mappings: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__79c997ed6a533e453fd1b182579d72149933074796ba9e81e6eee7479bbb0ea9)
-            check_type(argname="argument role_mappings", value=role_mappings, expected_type=typing.Tuple[type_hints["role_mappings"], ...]) # pyright: ignore [reportGeneralTypeIssues]
         return typing.cast(None, jsii.invoke(self, "addRoleMappings", [*role_mappings]))
 
     @jsii.member(jsii_name="addUserPoolAuthentication")
     def add_user_pool_authentication(
         self,
         user_pool: IUserPoolAuthenticationProvider,
     ) -> None:
         '''(experimental) Add a User Pool to the IdentityPool and configure User Pool Client to handle identities.
 
         :param user_pool: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fbd9ea8a4c738095932e3cf624c6eb098117704692279323d27952d6b2df0e00)
-            check_type(argname="argument user_pool", value=user_pool, expected_type=type_hints["user_pool"])
         return typing.cast(None, jsii.invoke(self, "addUserPoolAuthentication", [user_pool]))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="authenticatedRole")
-    def authenticated_role(self) -> _aws_cdk_aws_iam_ceddda9d.IRole:
+    def authenticated_role(self) -> aws_cdk.aws_iam.IRole:
         '''(experimental) Default role for authenticated users.
 
         :stability: experimental
         '''
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.IRole, jsii.get(self, "authenticatedRole"))
+        return typing.cast(aws_cdk.aws_iam.IRole, jsii.get(self, "authenticatedRole"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="identityPoolArn")
     def identity_pool_arn(self) -> builtins.str:
         '''(experimental) The ARN of the Identity Pool.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "identityPoolArn"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="identityPoolId")
     def identity_pool_id(self) -> builtins.str:
         '''(experimental) The id of the Identity Pool in the format REGION:GUID.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "identityPoolId"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="identityPoolName")
     def identity_pool_name(self) -> builtins.str:
         '''(experimental) The name of the Identity Pool.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "identityPoolName"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="unauthenticatedRole")
-    def unauthenticated_role(self) -> _aws_cdk_aws_iam_ceddda9d.IRole:
+    def unauthenticated_role(self) -> aws_cdk.aws_iam.IRole:
         '''(experimental) Default role for unauthenticated users.
 
         :stability: experimental
         '''
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.IRole, jsii.get(self, "unauthenticatedRole"))
+        return typing.cast(aws_cdk.aws_iam.IRole, jsii.get(self, "unauthenticatedRole"))
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-cognito-identitypool-alpha.IdentityPoolAmazonLoginProvider",
     jsii_struct_bases=[],
     name_mapping={"app_id": "appId"},
 )
 class IdentityPoolAmazonLoginProvider:
     def __init__(self, *, app_id: builtins.str) -> None:
         '''(experimental) Login Provider for Identity Federation using Amazon Credentials.
 
         :param app_id: (experimental) App Id for Amazon Identity Federation.
 
         :stability: experimental
-        :exampleMetadata: infused
+        :exampleMetadata: fixture=_generated
 
         Example::
 
-            IdentityPool(self, "myidentitypool",
-                identity_pool_name="myidentitypool",
-                authentication_providers=IdentityPoolAuthenticationProviders(
-                    amazon=IdentityPoolAmazonLoginProvider(
-                        app_id="amzn1.application.12312k3j234j13rjiwuenf"
-                    ),
-                    facebook=IdentityPoolFacebookLoginProvider(
-                        app_id="1234567890123"
-                    ),
-                    google=IdentityPoolGoogleLoginProvider(
-                        client_id="12345678012.apps.googleusercontent.com"
-                    ),
-                    apple=IdentityPoolAppleLoginProvider(
-                        services_id="com.myappleapp.auth"
-                    ),
-                    twitter=IdentityPoolTwitterLoginProvider(
-                        consumer_key="my-twitter-id",
-                        consumer_secret="my-twitter-secret"
-                    )
-                )
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.aws_cognito_identitypool_alpha as cognito_identitypool_alpha
+            
+            identity_pool_amazon_login_provider = cognito_identitypool_alpha.IdentityPoolAmazonLoginProvider(
+                app_id="appId"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b9e283aa49d3946357252123279fe3e514c02786d6dbaf36c03180cb06444fd8)
-            check_type(argname="argument app_id", value=app_id, expected_type=type_hints["app_id"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "app_id": app_id,
         }
 
     @builtins.property
     def app_id(self) -> builtins.str:
         '''(experimental) App Id for Amazon Identity Federation.
 
@@ -887,44 +847,27 @@
 class IdentityPoolAppleLoginProvider:
     def __init__(self, *, services_id: builtins.str) -> None:
         '''(experimental) Login Provider for Identity Federation using Apple Credentials.
 
         :param services_id: (experimental) App Id for Apple Identity Federation.
 
         :stability: experimental
-        :exampleMetadata: infused
+        :exampleMetadata: fixture=_generated
 
         Example::
 
-            IdentityPool(self, "myidentitypool",
-                identity_pool_name="myidentitypool",
-                authentication_providers=IdentityPoolAuthenticationProviders(
-                    amazon=IdentityPoolAmazonLoginProvider(
-                        app_id="amzn1.application.12312k3j234j13rjiwuenf"
-                    ),
-                    facebook=IdentityPoolFacebookLoginProvider(
-                        app_id="1234567890123"
-                    ),
-                    google=IdentityPoolGoogleLoginProvider(
-                        client_id="12345678012.apps.googleusercontent.com"
-                    ),
-                    apple=IdentityPoolAppleLoginProvider(
-                        services_id="com.myappleapp.auth"
-                    ),
-                    twitter=IdentityPoolTwitterLoginProvider(
-                        consumer_key="my-twitter-id",
-                        consumer_secret="my-twitter-secret"
-                    )
-                )
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.aws_cognito_identitypool_alpha as cognito_identitypool_alpha
+            
+            identity_pool_apple_login_provider = cognito_identitypool_alpha.IdentityPoolAppleLoginProvider(
+                services_id="servicesId"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e7c9040769cdc703f1660cd3e3da515a34764b5e7c1c0fe8e072609ef85af66f)
-            check_type(argname="argument services_id", value=services_id, expected_type=type_hints["services_id"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "services_id": services_id,
         }
 
     @builtins.property
     def services_id(self) -> builtins.str:
         '''(experimental) App Id for Apple Identity Federation.
 
@@ -954,44 +897,27 @@
 class IdentityPoolFacebookLoginProvider:
     def __init__(self, *, app_id: builtins.str) -> None:
         '''(experimental) Login Provider for Identity Federation using Facebook Credentials.
 
         :param app_id: (experimental) App Id for Facebook Identity Federation.
 
         :stability: experimental
-        :exampleMetadata: infused
+        :exampleMetadata: fixture=_generated
 
         Example::
 
-            IdentityPool(self, "myidentitypool",
-                identity_pool_name="myidentitypool",
-                authentication_providers=IdentityPoolAuthenticationProviders(
-                    amazon=IdentityPoolAmazonLoginProvider(
-                        app_id="amzn1.application.12312k3j234j13rjiwuenf"
-                    ),
-                    facebook=IdentityPoolFacebookLoginProvider(
-                        app_id="1234567890123"
-                    ),
-                    google=IdentityPoolGoogleLoginProvider(
-                        client_id="12345678012.apps.googleusercontent.com"
-                    ),
-                    apple=IdentityPoolAppleLoginProvider(
-                        services_id="com.myappleapp.auth"
-                    ),
-                    twitter=IdentityPoolTwitterLoginProvider(
-                        consumer_key="my-twitter-id",
-                        consumer_secret="my-twitter-secret"
-                    )
-                )
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.aws_cognito_identitypool_alpha as cognito_identitypool_alpha
+            
+            identity_pool_facebook_login_provider = cognito_identitypool_alpha.IdentityPoolFacebookLoginProvider(
+                app_id="appId"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__553a6105b1cc099f5bb05790fda107ae2e28e4a5891f7d4400f19cddf53e926e)
-            check_type(argname="argument app_id", value=app_id, expected_type=type_hints["app_id"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "app_id": app_id,
         }
 
     @builtins.property
     def app_id(self) -> builtins.str:
         '''(experimental) App Id for Facebook Identity Federation.
 
@@ -1021,44 +947,27 @@
 class IdentityPoolGoogleLoginProvider:
     def __init__(self, *, client_id: builtins.str) -> None:
         '''(experimental) Login Provider for Identity Federation using Google Credentials.
 
         :param client_id: (experimental) App Id for Google Identity Federation.
 
         :stability: experimental
-        :exampleMetadata: infused
+        :exampleMetadata: fixture=_generated
 
         Example::
 
-            IdentityPool(self, "myidentitypool",
-                identity_pool_name="myidentitypool",
-                authentication_providers=IdentityPoolAuthenticationProviders(
-                    amazon=IdentityPoolAmazonLoginProvider(
-                        app_id="amzn1.application.12312k3j234j13rjiwuenf"
-                    ),
-                    facebook=IdentityPoolFacebookLoginProvider(
-                        app_id="1234567890123"
-                    ),
-                    google=IdentityPoolGoogleLoginProvider(
-                        client_id="12345678012.apps.googleusercontent.com"
-                    ),
-                    apple=IdentityPoolAppleLoginProvider(
-                        services_id="com.myappleapp.auth"
-                    ),
-                    twitter=IdentityPoolTwitterLoginProvider(
-                        consumer_key="my-twitter-id",
-                        consumer_secret="my-twitter-secret"
-                    )
-                )
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.aws_cognito_identitypool_alpha as cognito_identitypool_alpha
+            
+            identity_pool_google_login_provider = cognito_identitypool_alpha.IdentityPoolGoogleLoginProvider(
+                client_id="clientId"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__dc7d7863b86c1b6983201a7e628ab0bb505b6719534f708df8a6c31427dbb5bb)
-            check_type(argname="argument client_id", value=client_id, expected_type=type_hints["client_id"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "client_id": client_id,
         }
 
     @builtins.property
     def client_id(self) -> builtins.str:
         '''(experimental) App Id for Google Identity Federation.
 
@@ -1095,60 +1004,98 @@
 )
 class IdentityPoolProps:
     def __init__(
         self,
         *,
         allow_classic_flow: typing.Optional[builtins.bool] = None,
         allow_unauthenticated_identities: typing.Optional[builtins.bool] = None,
-        authenticated_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-        authentication_providers: typing.Optional[typing.Union["IdentityPoolAuthenticationProviders", typing.Dict[builtins.str, typing.Any]]] = None,
+        authenticated_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
+        authentication_providers: typing.Optional["IdentityPoolAuthenticationProviders"] = None,
         identity_pool_name: typing.Optional[builtins.str] = None,
-        role_mappings: typing.Optional[typing.Sequence[typing.Union["IdentityPoolRoleMapping", typing.Dict[builtins.str, typing.Any]]]] = None,
-        unauthenticated_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        role_mappings: typing.Optional[typing.Sequence["IdentityPoolRoleMapping"]] = None,
+        unauthenticated_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
     ) -> None:
         '''(experimental) Props for the IdentityPool construct.
 
         :param allow_classic_flow: (experimental) Enables the Basic (Classic) authentication flow. Default: - Classic Flow not allowed
         :param allow_unauthenticated_identities: (experimental) Wwhether the identity pool supports unauthenticated logins. Default: - false
         :param authenticated_role: (experimental) The Default Role to be assumed by Authenticated Users. Default: - A Default Authenticated Role will be added
         :param authentication_providers: (experimental) Authentication providers for using in identity pool. Default: - No Authentication Providers passed directly to Identity Pool
         :param identity_pool_name: (experimental) The name of the Identity Pool. Default: - automatically generated name by CloudFormation at deploy time
         :param role_mappings: (experimental) Rules for mapping roles to users. Default: - no Role Mappings
         :param unauthenticated_role: (experimental) The Default Role to be assumed by Unauthenticated Users. Default: - A Default Unauthenticated Role will be added
 
         :stability: experimental
-        :exampleMetadata: infused
+        :exampleMetadata: fixture=_generated
 
         Example::
 
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.aws_cognito_identitypool_alpha as cognito_identitypool_alpha
+            from aws_cdk import aws_iam as iam
+            
+            # identity_pool_provider_url: cognito_identitypool_alpha.IdentityPoolProviderUrl
             # open_id_connect_provider: iam.OpenIdConnectProvider
+            # role: iam.Role
+            # saml_provider: iam.SamlProvider
+            # user_pool_authentication_provider: cognito_identitypool_alpha.UserPoolAuthenticationProvider
             
-            IdentityPool(self, "myidentitypool",
-                identity_pool_name="myidentitypool",
-                authentication_providers=IdentityPoolAuthenticationProviders(
-                    google=IdentityPoolGoogleLoginProvider(
-                        client_id="12345678012.apps.googleusercontent.com"
+            identity_pool_props = cognito_identitypool_alpha.IdentityPoolProps(
+                allow_classic_flow=False,
+                allow_unauthenticated_identities=False,
+                authenticated_role=role,
+                authentication_providers=cognito_identitypool_alpha.IdentityPoolAuthenticationProviders(
+                    amazon=cognito_identitypool_alpha.IdentityPoolAmazonLoginProvider(
+                        app_id="appId"
+                    ),
+                    apple=cognito_identitypool_alpha.IdentityPoolAppleLoginProvider(
+                        services_id="servicesId"
+                    ),
+                    custom_provider="customProvider",
+                    digits=cognito_identitypool_alpha.IdentityPoolDigitsLoginProvider(
+                        consumer_key="consumerKey",
+                        consumer_secret="consumerSecret"
+                    ),
+                    facebook=cognito_identitypool_alpha.IdentityPoolFacebookLoginProvider(
+                        app_id="appId"
+                    ),
+                    google=cognito_identitypool_alpha.IdentityPoolGoogleLoginProvider(
+                        client_id="clientId"
                     ),
                     open_id_connect_providers=[open_id_connect_provider],
-                    custom_provider="my-custom-provider.example.com"
-                )
+                    saml_providers=[saml_provider],
+                    twitter=cognito_identitypool_alpha.IdentityPoolTwitterLoginProvider(
+                        consumer_key="consumerKey",
+                        consumer_secret="consumerSecret"
+                    ),
+                    user_pools=[user_pool_authentication_provider]
+                ),
+                identity_pool_name="identityPoolName",
+                role_mappings=[cognito_identitypool_alpha.IdentityPoolRoleMapping(
+                    provider_url=identity_pool_provider_url,
+            
+                    # the properties below are optional
+                    resolve_ambiguous_roles=False,
+                    rules=[cognito_identitypool_alpha.RoleMappingRule(
+                        claim="claim",
+                        claim_value="claimValue",
+                        mapped_role=role,
+            
+                        # the properties below are optional
+                        match_type=cognito_identitypool_alpha.RoleMappingMatchType.EQUALS
+                    )],
+                    use_token=False
+                )],
+                unauthenticated_role=role
             )
         '''
         if isinstance(authentication_providers, dict):
             authentication_providers = IdentityPoolAuthenticationProviders(**authentication_providers)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__67b8242ca2e55a1962a36ef0e9c4b94eae811b93839b5e265f5743512e5ca12b)
-            check_type(argname="argument allow_classic_flow", value=allow_classic_flow, expected_type=type_hints["allow_classic_flow"])
-            check_type(argname="argument allow_unauthenticated_identities", value=allow_unauthenticated_identities, expected_type=type_hints["allow_unauthenticated_identities"])
-            check_type(argname="argument authenticated_role", value=authenticated_role, expected_type=type_hints["authenticated_role"])
-            check_type(argname="argument authentication_providers", value=authentication_providers, expected_type=type_hints["authentication_providers"])
-            check_type(argname="argument identity_pool_name", value=identity_pool_name, expected_type=type_hints["identity_pool_name"])
-            check_type(argname="argument role_mappings", value=role_mappings, expected_type=type_hints["role_mappings"])
-            check_type(argname="argument unauthenticated_role", value=unauthenticated_role, expected_type=type_hints["unauthenticated_role"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if allow_classic_flow is not None:
             self._values["allow_classic_flow"] = allow_classic_flow
         if allow_unauthenticated_identities is not None:
             self._values["allow_unauthenticated_identities"] = allow_unauthenticated_identities
         if authenticated_role is not None:
             self._values["authenticated_role"] = authenticated_role
         if authentication_providers is not None:
@@ -1179,23 +1126,23 @@
 
         :stability: experimental
         '''
         result = self._values.get("allow_unauthenticated_identities")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def authenticated_role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+    def authenticated_role(self) -> typing.Optional[aws_cdk.aws_iam.IRole]:
         '''(experimental) The Default Role to be assumed by Authenticated Users.
 
         :default: - A Default Authenticated Role will be added
 
         :stability: experimental
         '''
         result = self._values.get("authenticated_role")
-        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_iam.IRole], result)
 
     @builtins.property
     def authentication_providers(
         self,
     ) -> typing.Optional["IdentityPoolAuthenticationProviders"]:
         '''(experimental) Authentication providers for using in identity pool.
 
@@ -1225,23 +1172,23 @@
 
         :stability: experimental
         '''
         result = self._values.get("role_mappings")
         return typing.cast(typing.Optional[typing.List["IdentityPoolRoleMapping"]], result)
 
     @builtins.property
-    def unauthenticated_role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+    def unauthenticated_role(self) -> typing.Optional[aws_cdk.aws_iam.IRole]:
         '''(experimental) The Default Role to be assumed by Unauthenticated Users.
 
         :default: - A Default Unauthenticated Role will be added
 
         :stability: experimental
         '''
         result = self._values.get("unauthenticated_role")
-        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_iam.IRole], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -1315,166 +1262,142 @@
 class IdentityPoolProviderUrl(
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-cognito-identitypool-alpha.IdentityPoolProviderUrl",
 ):
     '''(experimental) Keys for Login Providers - correspond to client id's of respective federation identity providers.
 
     :stability: experimental
-    :exampleMetadata: infused
+    :exampleMetadata: fixture=_generated
 
     Example::
 
-        from aws_cdk.aws_cognito import UserPool
-        from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl
-        
-        # user_pool: UserPool
+        # The code below shows an example of how to instantiate this type.
+        # The values are placeholders you should change.
+        import aws_cdk.aws_cognito_identitypool_alpha as cognito_identitypool_alpha
         
-        IdentityPool(self, "myidentitypool",
-            identity_pool_name="myidentitypool",
-            role_mappings=[IdentityPoolRoleMapping(
-                mapping_key="cognito",
-                provider_url=IdentityPoolProviderUrl.user_pool(user_pool.user_pool_provider_url),
-                use_token=True
-            )]
-        )
+        identity_pool_provider_url = cognito_identitypool_alpha.IdentityPoolProviderUrl.custom("url")
     '''
 
     def __init__(self, type: IdentityPoolProviderType, value: builtins.str) -> None:
         '''
         :param type: type of Provider Url.
         :param value: value of Provider Url.
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__423f3af9588f321b47a169a44fe143eb961b0377418e1736dde381403db8730e)
-            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.create(self.__class__, self, [type, value])
 
-    @jsii.member(jsii_name="custom")
+    @jsii.member(jsii_name="custom") # type: ignore[misc]
     @builtins.classmethod
     def custom(cls, url: builtins.str) -> "IdentityPoolProviderUrl":
         '''(experimental) Custom Provider Url.
 
         :param url: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__aba4eac2376a67f469d725ea627955e1696d934a6d0601d7e4873d8b2b48d749)
-            check_type(argname="argument url", value=url, expected_type=type_hints["url"])
         return typing.cast("IdentityPoolProviderUrl", jsii.sinvoke(cls, "custom", [url]))
 
-    @jsii.member(jsii_name="openId")
+    @jsii.member(jsii_name="openId") # type: ignore[misc]
     @builtins.classmethod
     def open_id(cls, url: builtins.str) -> "IdentityPoolProviderUrl":
         '''(experimental) OpenId Provider Url.
 
         :param url: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3d161a44d12cc621bec8346b7a54def25199238af1ee02be289568c2abb4aed2)
-            check_type(argname="argument url", value=url, expected_type=type_hints["url"])
         return typing.cast("IdentityPoolProviderUrl", jsii.sinvoke(cls, "openId", [url]))
 
-    @jsii.member(jsii_name="saml")
+    @jsii.member(jsii_name="saml") # type: ignore[misc]
     @builtins.classmethod
     def saml(cls, url: builtins.str) -> "IdentityPoolProviderUrl":
         '''(experimental) Saml Provider Url.
 
         :param url: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0cbf2fc0f2dbf61ab8ba7e761e45e78a8d5d3bbfa64ccc8f8d93bff656c1a825)
-            check_type(argname="argument url", value=url, expected_type=type_hints["url"])
         return typing.cast("IdentityPoolProviderUrl", jsii.sinvoke(cls, "saml", [url]))
 
-    @jsii.member(jsii_name="userPool")
+    @jsii.member(jsii_name="userPool") # type: ignore[misc]
     @builtins.classmethod
     def user_pool(cls, url: builtins.str) -> "IdentityPoolProviderUrl":
         '''(experimental) User Pool Provider Url.
 
         :param url: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7531b9fff4293227d6e5c746c9e82a2d3b5164eaf82e984877f422ff7de768c9)
-            check_type(argname="argument url", value=url, expected_type=type_hints["url"])
         return typing.cast("IdentityPoolProviderUrl", jsii.sinvoke(cls, "userPool", [url]))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="AMAZON")
     def AMAZON(cls) -> "IdentityPoolProviderUrl":
         '''(experimental) Amazon Provider Url.
 
         :stability: experimental
         '''
         return typing.cast("IdentityPoolProviderUrl", jsii.sget(cls, "AMAZON"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="APPLE")
     def APPLE(cls) -> "IdentityPoolProviderUrl":
         '''(experimental) Apple Provider Url.
 
         :stability: experimental
         '''
         return typing.cast("IdentityPoolProviderUrl", jsii.sget(cls, "APPLE"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="DIGITS")
     def DIGITS(cls) -> "IdentityPoolProviderUrl":
         '''(experimental) Digits Provider Url.
 
         :stability: experimental
         '''
         return typing.cast("IdentityPoolProviderUrl", jsii.sget(cls, "DIGITS"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="FACEBOOK")
     def FACEBOOK(cls) -> "IdentityPoolProviderUrl":
         '''(experimental) Facebook Provider Url.
 
         :stability: experimental
         '''
         return typing.cast("IdentityPoolProviderUrl", jsii.sget(cls, "FACEBOOK"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="GOOGLE")
     def GOOGLE(cls) -> "IdentityPoolProviderUrl":
         '''(experimental) Google Provider Url.
 
         :stability: experimental
         '''
         return typing.cast("IdentityPoolProviderUrl", jsii.sget(cls, "GOOGLE"))
 
-    @jsii.python.classproperty
+    @jsii.python.classproperty # type: ignore[misc]
     @jsii.member(jsii_name="TWITTER")
     def TWITTER(cls) -> "IdentityPoolProviderUrl":
         '''(experimental) Twitter Provider Url.
 
         :stability: experimental
         '''
         return typing.cast("IdentityPoolProviderUrl", jsii.sget(cls, "TWITTER"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="type")
     def type(self) -> IdentityPoolProviderType:
         '''(experimental) type of Provider Url.
 
         :stability: experimental
         '''
         return typing.cast(IdentityPoolProviderType, jsii.get(self, "type"))
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="value")
     def value(self) -> builtins.str:
         '''(experimental) value of Provider Url.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "value"))
@@ -1492,20 +1415,20 @@
         "twitter": "twitter",
     },
 )
 class IdentityPoolProviders:
     def __init__(
         self,
         *,
-        amazon: typing.Optional[typing.Union[IdentityPoolAmazonLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-        apple: typing.Optional[typing.Union[IdentityPoolAppleLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-        digits: typing.Optional[typing.Union["IdentityPoolDigitsLoginProvider", typing.Dict[builtins.str, typing.Any]]] = None,
-        facebook: typing.Optional[typing.Union[IdentityPoolFacebookLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-        google: typing.Optional[typing.Union[IdentityPoolGoogleLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-        twitter: typing.Optional[typing.Union["IdentityPoolTwitterLoginProvider", typing.Dict[builtins.str, typing.Any]]] = None,
+        amazon: typing.Optional[IdentityPoolAmazonLoginProvider] = None,
+        apple: typing.Optional[IdentityPoolAppleLoginProvider] = None,
+        digits: typing.Optional["IdentityPoolDigitsLoginProvider"] = None,
+        facebook: typing.Optional[IdentityPoolFacebookLoginProvider] = None,
+        google: typing.Optional[IdentityPoolGoogleLoginProvider] = None,
+        twitter: typing.Optional["IdentityPoolTwitterLoginProvider"] = None,
     ) -> None:
         '''(experimental) External Identity Providers To Connect to User Pools and Identity Pools.
 
         :param amazon: (experimental) App Id for Amazon Identity Federation. Default: - No Amazon Authentication Provider used without OpenIdConnect or a User Pool
         :param apple: (experimental) Services Id for Apple Identity Federation. Default: - No Apple Authentication Provider used without OpenIdConnect or a User Pool
         :param digits: (experimental) Consumer Key and Secret for Digits Identity Federation. Default: - No Digits Authentication Provider used without OpenIdConnect or a User Pool
         :param facebook: (experimental) App Id for Facebook Identity Federation. Default: - No Facebook Authentication Provider used without OpenIdConnect or a User Pool
@@ -1552,23 +1475,15 @@
             digits = IdentityPoolDigitsLoginProvider(**digits)
         if isinstance(facebook, dict):
             facebook = IdentityPoolFacebookLoginProvider(**facebook)
         if isinstance(google, dict):
             google = IdentityPoolGoogleLoginProvider(**google)
         if isinstance(twitter, dict):
             twitter = IdentityPoolTwitterLoginProvider(**twitter)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6da31bad5d5f044fd941ec5cc9821499624050d72b9556e6891a7a76644b8330)
-            check_type(argname="argument amazon", value=amazon, expected_type=type_hints["amazon"])
-            check_type(argname="argument apple", value=apple, expected_type=type_hints["apple"])
-            check_type(argname="argument digits", value=digits, expected_type=type_hints["digits"])
-            check_type(argname="argument facebook", value=facebook, expected_type=type_hints["facebook"])
-            check_type(argname="argument google", value=google, expected_type=type_hints["google"])
-            check_type(argname="argument twitter", value=twitter, expected_type=type_hints["twitter"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if amazon is not None:
             self._values["amazon"] = amazon
         if apple is not None:
             self._values["apple"] = apple
         if digits is not None:
             self._values["digits"] = digits
         if facebook is not None:
@@ -1654,15 +1569,15 @@
         return "IdentityPoolProviders(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.implements(IIdentityPoolRoleAttachment)
 class IdentityPoolRoleAttachment(
-    _aws_cdk_ceddda9d.Resource,
+    aws_cdk.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-cognito-identitypool-alpha.IdentityPoolRoleAttachment",
 ):
     '''(experimental) Defines an Identity Pool Role Attachment.
 
     :stability: experimental
     :resource: AWS::Cognito::IdentityPoolRoleAttachment
@@ -1684,15 +1599,14 @@
         
             # the properties below are optional
             authenticated_role=role,
             role_mappings=[cognito_identitypool_alpha.IdentityPoolRoleMapping(
                 provider_url=identity_pool_provider_url,
         
                 # the properties below are optional
-                mapping_key="mappingKey",
                 resolve_ambiguous_roles=False,
                 rules=[cognito_identitypool_alpha.RoleMappingRule(
                     claim="claim",
                     claim_value="claimValue",
                     mapped_role=role,
         
                     # the properties below are optional
@@ -1702,46 +1616,42 @@
             )],
             unauthenticated_role=role
         )
     '''
 
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         identity_pool: IIdentityPool,
-        authenticated_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-        role_mappings: typing.Optional[typing.Sequence[typing.Union["IdentityPoolRoleMapping", typing.Dict[builtins.str, typing.Any]]]] = None,
-        unauthenticated_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        authenticated_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
+        role_mappings: typing.Optional[typing.Sequence["IdentityPoolRoleMapping"]] = None,
+        unauthenticated_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param identity_pool: (experimental) Id of the Attachments Underlying Identity Pool.
         :param authenticated_role: (experimental) Default Authenticated (User) Role. Default: - No default authenticated role will be added
         :param role_mappings: (experimental) Rules for mapping roles to users. Default: - no Role Mappings
         :param unauthenticated_role: (experimental) Default Unauthenticated (Guest) Role. Default: - No default unauthenticated role will be added
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a165e7b7d8cd676948cb9b98c9ae060e6da6931de2231f73fb8bfe09c571e8f3)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = IdentityPoolRoleAttachmentProps(
             identity_pool=identity_pool,
             authenticated_role=authenticated_role,
             role_mappings=role_mappings,
             unauthenticated_role=unauthenticated_role,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @builtins.property
+    @builtins.property # type: ignore[misc]
     @jsii.member(jsii_name="identityPoolId")
     def identity_pool_id(self) -> builtins.str:
         '''(experimental) Id of the underlying identity pool.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "identityPoolId"))
@@ -1758,17 +1668,17 @@
     },
 )
 class IdentityPoolRoleAttachmentProps:
     def __init__(
         self,
         *,
         identity_pool: IIdentityPool,
-        authenticated_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-        role_mappings: typing.Optional[typing.Sequence[typing.Union["IdentityPoolRoleMapping", typing.Dict[builtins.str, typing.Any]]]] = None,
-        unauthenticated_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        authenticated_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
+        role_mappings: typing.Optional[typing.Sequence["IdentityPoolRoleMapping"]] = None,
+        unauthenticated_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
     ) -> None:
         '''(experimental) Props for an Identity Pool Role Attachment.
 
         :param identity_pool: (experimental) Id of the Attachments Underlying Identity Pool.
         :param authenticated_role: (experimental) Default Authenticated (User) Role. Default: - No default authenticated role will be added
         :param role_mappings: (experimental) Rules for mapping roles to users. Default: - no Role Mappings
         :param unauthenticated_role: (experimental) Default Unauthenticated (Guest) Role. Default: - No default unauthenticated role will be added
@@ -1792,36 +1702,29 @@
             
                 # the properties below are optional
                 authenticated_role=role,
                 role_mappings=[cognito_identitypool_alpha.IdentityPoolRoleMapping(
                     provider_url=identity_pool_provider_url,
             
                     # the properties below are optional
-                    mapping_key="mappingKey",
                     resolve_ambiguous_roles=False,
                     rules=[cognito_identitypool_alpha.RoleMappingRule(
                         claim="claim",
                         claim_value="claimValue",
                         mapped_role=role,
             
                         # the properties below are optional
                         match_type=cognito_identitypool_alpha.RoleMappingMatchType.EQUALS
                     )],
                     use_token=False
                 )],
                 unauthenticated_role=role
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__275eb74a4a88284000b15066daef659c73082e99224df6491b0465af179ac6b4)
-            check_type(argname="argument identity_pool", value=identity_pool, expected_type=type_hints["identity_pool"])
-            check_type(argname="argument authenticated_role", value=authenticated_role, expected_type=type_hints["authenticated_role"])
-            check_type(argname="argument role_mappings", value=role_mappings, expected_type=type_hints["role_mappings"])
-            check_type(argname="argument unauthenticated_role", value=unauthenticated_role, expected_type=type_hints["unauthenticated_role"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "identity_pool": identity_pool,
         }
         if authenticated_role is not None:
             self._values["authenticated_role"] = authenticated_role
         if role_mappings is not None:
             self._values["role_mappings"] = role_mappings
         if unauthenticated_role is not None:
@@ -1834,45 +1737,45 @@
         :stability: experimental
         '''
         result = self._values.get("identity_pool")
         assert result is not None, "Required property 'identity_pool' is missing"
         return typing.cast(IIdentityPool, result)
 
     @builtins.property
-    def authenticated_role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+    def authenticated_role(self) -> typing.Optional[aws_cdk.aws_iam.IRole]:
         '''(experimental) Default Authenticated (User) Role.
 
         :default: - No default authenticated role will be added
 
         :stability: experimental
         '''
         result = self._values.get("authenticated_role")
-        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_iam.IRole], result)
 
     @builtins.property
     def role_mappings(self) -> typing.Optional[typing.List["IdentityPoolRoleMapping"]]:
         '''(experimental) Rules for mapping roles to users.
 
         :default: - no Role Mappings
 
         :stability: experimental
         '''
         result = self._values.get("role_mappings")
         return typing.cast(typing.Optional[typing.List["IdentityPoolRoleMapping"]], result)
 
     @builtins.property
-    def unauthenticated_role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+    def unauthenticated_role(self) -> typing.Optional[aws_cdk.aws_iam.IRole]:
         '''(experimental) Default Unauthenticated (Guest) Role.
 
         :default: - No default unauthenticated role will be added
 
         :stability: experimental
         '''
         result = self._values.get("unauthenticated_role")
-        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_iam.IRole], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -1883,66 +1786,68 @@
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-cognito-identitypool-alpha.IdentityPoolRoleMapping",
     jsii_struct_bases=[],
     name_mapping={
         "provider_url": "providerUrl",
-        "mapping_key": "mappingKey",
         "resolve_ambiguous_roles": "resolveAmbiguousRoles",
         "rules": "rules",
         "use_token": "useToken",
     },
 )
 class IdentityPoolRoleMapping:
     def __init__(
         self,
         *,
         provider_url: IdentityPoolProviderUrl,
-        mapping_key: typing.Optional[builtins.str] = None,
         resolve_ambiguous_roles: typing.Optional[builtins.bool] = None,
-        rules: typing.Optional[typing.Sequence[typing.Union["RoleMappingRule", typing.Dict[builtins.str, typing.Any]]]] = None,
+        rules: typing.Optional[typing.Sequence["RoleMappingRule"]] = None,
         use_token: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''(experimental) Map roles to users in the identity pool based on claims from the Identity Provider.
 
         :param provider_url: (experimental) The url of the provider of for which the role is mapped.
-        :param mapping_key: (experimental) The key used for the role mapping in the role mapping hash. Required if the providerUrl is a token. Default: - the provided providerUrl
         :param resolve_ambiguous_roles: (experimental) Allow for role assumption when results of role mapping are ambiguous. Default: false - Ambiguous role resolutions will lead to requester being denied
         :param rules: (experimental) The claim and value that must be matched in order to assume the role. Required if useToken is false Default: - No Rule Mapping Rule
         :param use_token: (experimental) If true then mapped roles must be passed through the cognito:roles or cognito:preferred_role claims from identity provider. Default: false
 
         :see: https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-cognito-identitypoolroleattachment.html
         :stability: experimental
-        :exampleMetadata: infused
+        :exampleMetadata: fixture=_generated
 
         Example::
 
-            from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolRoleMapping
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.aws_cognito_identitypool_alpha as cognito_identitypool_alpha
+            from aws_cdk import aws_iam as iam
+            
+            # identity_pool_provider_url: cognito_identitypool_alpha.IdentityPoolProviderUrl
+            # role: iam.Role
             
-            # identity_pool: IdentityPool
-            # my_added_role_mapping1: IdentityPoolRoleMapping
-            # my_added_role_mapping2: IdentityPoolRoleMapping
-            # my_added_role_mapping3: IdentityPoolRoleMapping
-            
-            
-            identity_pool.add_role_mappings(my_added_role_mapping1, my_added_role_mapping2, my_added_role_mapping3)
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__650ad537013ada6fb730b758a9cc04e3e889c73469adb530187b60e65137d653)
-            check_type(argname="argument provider_url", value=provider_url, expected_type=type_hints["provider_url"])
-            check_type(argname="argument mapping_key", value=mapping_key, expected_type=type_hints["mapping_key"])
-            check_type(argname="argument resolve_ambiguous_roles", value=resolve_ambiguous_roles, expected_type=type_hints["resolve_ambiguous_roles"])
-            check_type(argname="argument rules", value=rules, expected_type=type_hints["rules"])
-            check_type(argname="argument use_token", value=use_token, expected_type=type_hints["use_token"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+            identity_pool_role_mapping = cognito_identitypool_alpha.IdentityPoolRoleMapping(
+                provider_url=identity_pool_provider_url,
+            
+                # the properties below are optional
+                resolve_ambiguous_roles=False,
+                rules=[cognito_identitypool_alpha.RoleMappingRule(
+                    claim="claim",
+                    claim_value="claimValue",
+                    mapped_role=role,
+            
+                    # the properties below are optional
+                    match_type=cognito_identitypool_alpha.RoleMappingMatchType.EQUALS
+                )],
+                use_token=False
+            )
+        '''
+        self._values: typing.Dict[str, typing.Any] = {
             "provider_url": provider_url,
         }
-        if mapping_key is not None:
-            self._values["mapping_key"] = mapping_key
         if resolve_ambiguous_roles is not None:
             self._values["resolve_ambiguous_roles"] = resolve_ambiguous_roles
         if rules is not None:
             self._values["rules"] = rules
         if use_token is not None:
             self._values["use_token"] = use_token
 
@@ -1953,27 +1858,14 @@
         :stability: experimental
         '''
         result = self._values.get("provider_url")
         assert result is not None, "Required property 'provider_url' is missing"
         return typing.cast(IdentityPoolProviderUrl, result)
 
     @builtins.property
-    def mapping_key(self) -> typing.Optional[builtins.str]:
-        '''(experimental) The key used for the role mapping in the role mapping hash.
-
-        Required if the providerUrl is a token.
-
-        :default: - the provided providerUrl
-
-        :stability: experimental
-        '''
-        result = self._values.get("mapping_key")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
     def resolve_ambiguous_roles(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Allow for role assumption when results of role mapping are ambiguous.
 
         :default: false - Ambiguous role resolutions will lead to requester being denied
 
         :stability: experimental
         '''
@@ -2031,45 +1923,28 @@
     ) -> None:
         '''(experimental) Login Provider for Identity Federation using Twitter Credentials.
 
         :param consumer_key: (experimental) App Id for Twitter Identity Federation.
         :param consumer_secret: (experimental) App Secret for Twitter Identity Federation.
 
         :stability: experimental
-        :exampleMetadata: infused
+        :exampleMetadata: fixture=_generated
 
         Example::
 
-            IdentityPool(self, "myidentitypool",
-                identity_pool_name="myidentitypool",
-                authentication_providers=IdentityPoolAuthenticationProviders(
-                    amazon=IdentityPoolAmazonLoginProvider(
-                        app_id="amzn1.application.12312k3j234j13rjiwuenf"
-                    ),
-                    facebook=IdentityPoolFacebookLoginProvider(
-                        app_id="1234567890123"
-                    ),
-                    google=IdentityPoolGoogleLoginProvider(
-                        client_id="12345678012.apps.googleusercontent.com"
-                    ),
-                    apple=IdentityPoolAppleLoginProvider(
-                        services_id="com.myappleapp.auth"
-                    ),
-                    twitter=IdentityPoolTwitterLoginProvider(
-                        consumer_key="my-twitter-id",
-                        consumer_secret="my-twitter-secret"
-                    )
-                )
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.aws_cognito_identitypool_alpha as cognito_identitypool_alpha
+            
+            identity_pool_twitter_login_provider = cognito_identitypool_alpha.IdentityPoolTwitterLoginProvider(
+                consumer_key="consumerKey",
+                consumer_secret="consumerSecret"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f91153aca8aea767279ad014c0a8369ca2e36afc6e9b02f0111bc64f713b104f)
-            check_type(argname="argument consumer_key", value=consumer_key, expected_type=type_hints["consumer_key"])
-            check_type(argname="argument consumer_secret", value=consumer_secret, expected_type=type_hints["consumer_secret"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "consumer_key": consumer_key,
             "consumer_secret": consumer_secret,
         }
 
     @builtins.property
     def consumer_key(self) -> builtins.str:
         '''(experimental) App Id for Twitter Identity Federation.
@@ -2103,41 +1978,14 @@
 
 
 @jsii.enum(jsii_type="@aws-cdk/aws-cognito-identitypool-alpha.RoleMappingMatchType")
 class RoleMappingMatchType(enum.Enum):
     '''(experimental) Types of matches allowed for Role Mapping.
 
     :stability: experimental
-    :exampleMetadata: infused
-
-    Example::
-
-        from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl, RoleMappingMatchType
-        
-        # admin_role: iam.Role
-        # non_admin_role: iam.Role
-        
-        IdentityPool(self, "myidentitypool",
-            identity_pool_name="myidentitypool",
-            # Assign specific roles to users based on whether or not the custom admin claim is passed from the identity provider
-            role_mappings=[IdentityPoolRoleMapping(
-                provider_url=IdentityPoolProviderUrl.AMAZON,
-                rules=[RoleMappingRule(
-                    claim="custom:admin",
-                    claim_value="admin",
-                    mapped_role=admin_role
-                ), RoleMappingRule(
-                    claim="custom:admin",
-                    claim_value="admin",
-                    match_type=RoleMappingMatchType.NOTEQUAL,
-                    mapped_role=non_admin_role
-                )
-                ]
-            )]
-        )
     '''
 
     EQUALS = "EQUALS"
     '''(experimental) The Claim from the token must equal the given value in order for a match.
 
     :stability: experimental
     '''
@@ -2170,15 +2018,15 @@
 )
 class RoleMappingRule:
     def __init__(
         self,
         *,
         claim: builtins.str,
         claim_value: builtins.str,
-        mapped_role: _aws_cdk_aws_iam_ceddda9d.IRole,
+        mapped_role: aws_cdk.aws_iam.IRole,
         match_type: typing.Optional[RoleMappingMatchType] = None,
     ) -> None:
         '''(experimental) Represents an Identity Pool Role Attachment Role Mapping Rule.
 
         :param claim: (experimental) The key sent in the token by the federated identity provider.
         :param claim_value: (experimental) The value of the claim that must be matched.
         :param mapped_role: (experimental) The Role to be assumed when Claim Value is matched.
@@ -2201,21 +2049,15 @@
                 claim_value="claimValue",
                 mapped_role=role,
             
                 # the properties below are optional
                 match_type=cognito_identitypool_alpha.RoleMappingMatchType.EQUALS
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__77869f331952f425fa372fe2f927e6224793554cefa649c244780e367abe94a9)
-            check_type(argname="argument claim", value=claim, expected_type=type_hints["claim"])
-            check_type(argname="argument claim_value", value=claim_value, expected_type=type_hints["claim_value"])
-            check_type(argname="argument mapped_role", value=mapped_role, expected_type=type_hints["mapped_role"])
-            check_type(argname="argument match_type", value=match_type, expected_type=type_hints["match_type"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "claim": claim,
             "claim_value": claim_value,
             "mapped_role": mapped_role,
         }
         if match_type is not None:
             self._values["match_type"] = match_type
 
@@ -2236,22 +2078,22 @@
         :stability: experimental
         '''
         result = self._values.get("claim_value")
         assert result is not None, "Required property 'claim_value' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def mapped_role(self) -> _aws_cdk_aws_iam_ceddda9d.IRole:
+    def mapped_role(self) -> aws_cdk.aws_iam.IRole:
         '''(experimental) The Role to be assumed when Claim Value is matched.
 
         :stability: experimental
         '''
         result = self._values.get("mapped_role")
         assert result is not None, "Required property 'mapped_role' is missing"
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.IRole, result)
+        return typing.cast(aws_cdk.aws_iam.IRole, result)
 
     @builtins.property
     def match_type(self) -> typing.Optional[RoleMappingMatchType]:
         '''(experimental) How to match with the Claim value.
 
         :default: RoleMappingMatchType.EQUALS
 
@@ -2276,33 +2118,41 @@
 class UserPoolAuthenticationProvider(
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-cognito-identitypool-alpha.UserPoolAuthenticationProvider",
 ):
     '''(experimental) Defines a User Pool Authentication Provider.
 
     :stability: experimental
-    :exampleMetadata: infused
+    :exampleMetadata: fixture=_generated
 
     Example::
 
-        # identity_pool: IdentityPool
+        # The code below shows an example of how to instantiate this type.
+        # The values are placeholders you should change.
+        import aws_cdk.aws_cognito_identitypool_alpha as cognito_identitypool_alpha
+        from aws_cdk import aws_cognito as cognito
         
-        user_pool = cognito.UserPool(self, "Pool")
-        identity_pool.add_user_pool_authentication(UserPoolAuthenticationProvider(
+        # user_pool: cognito.UserPool
+        # user_pool_client: cognito.UserPoolClient
+        
+        user_pool_authentication_provider = cognito_identitypool_alpha.UserPoolAuthenticationProvider(
             user_pool=user_pool,
-            disable_server_side_token_check=True
-        ))
+        
+            # the properties below are optional
+            disable_server_side_token_check=False,
+            user_pool_client=user_pool_client
+        )
     '''
 
     def __init__(
         self,
         *,
-        user_pool: _aws_cdk_aws_cognito_ceddda9d.IUserPool,
+        user_pool: aws_cdk.aws_cognito.IUserPool,
         disable_server_side_token_check: typing.Optional[builtins.bool] = None,
-        user_pool_client: typing.Optional[_aws_cdk_aws_cognito_ceddda9d.IUserPoolClient] = None,
+        user_pool_client: typing.Optional[aws_cdk.aws_cognito.IUserPoolClient] = None,
     ) -> None:
         '''
         :param user_pool: (experimental) The User Pool of the Associated Identity Providers.
         :param disable_server_side_token_check: (experimental) Setting this to true turns off identity pool checks for this user pool to make sure the user has not been globally signed out or deleted before the identity pool provides an OIDC token or AWS credentials for the user. Default: false
         :param user_pool_client: (experimental) The User Pool Client for the provided User Pool. Default: - A default user pool client will be added to User Pool
 
         :stability: experimental
@@ -2314,28 +2164,24 @@
         )
 
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="bind")
     def bind(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         identity_pool: IIdentityPool,
     ) -> "UserPoolAuthenticationProviderBindConfig":
         '''(experimental) The method called when a given User Pool Authentication Provider is added (for the first time) to an Identity Pool.
 
         :param scope: -
         :param identity_pool: -
 
         :stability: experimental
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e3c3e4f47b37f4d3265edfa6c7ad01b5c1409a21b5450216878fdce228df9f72)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument identity_pool", value=identity_pool, expected_type=type_hints["identity_pool"])
         _options = UserPoolAuthenticationProviderBindOptions()
 
         return typing.cast("UserPoolAuthenticationProviderBindConfig", jsii.invoke(self, "bind", [scope, identity_pool, _options]))
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-cognito-identitypool-alpha.UserPoolAuthenticationProviderBindConfig",
@@ -2371,20 +2217,15 @@
             
             user_pool_authentication_provider_bind_config = cognito_identitypool_alpha.UserPoolAuthenticationProviderBindConfig(
                 client_id="clientId",
                 provider_name="providerName",
                 server_side_token_check=False
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f7b8fa9dab857d092fcc38b5be232ff1c0998d006d07c8ef726d2a6530e5df52)
-            check_type(argname="argument client_id", value=client_id, expected_type=type_hints["client_id"])
-            check_type(argname="argument provider_name", value=provider_name, expected_type=type_hints["provider_name"])
-            check_type(argname="argument server_side_token_check", value=server_side_token_check, expected_type=type_hints["server_side_token_check"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "client_id": client_id,
             "provider_name": provider_name,
             "server_side_token_check": server_side_token_check,
         }
 
     @builtins.property
     def client_id(self) -> builtins.str:
@@ -2444,15 +2285,15 @@
 
             # The code below shows an example of how to instantiate this type.
             # The values are placeholders you should change.
             import aws_cdk.aws_cognito_identitypool_alpha as cognito_identitypool_alpha
             
             user_pool_authentication_provider_bind_options = cognito_identitypool_alpha.UserPoolAuthenticationProviderBindOptions()
         '''
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -2471,84 +2312,85 @@
         "user_pool_client": "userPoolClient",
     },
 )
 class UserPoolAuthenticationProviderProps:
     def __init__(
         self,
         *,
-        user_pool: _aws_cdk_aws_cognito_ceddda9d.IUserPool,
+        user_pool: aws_cdk.aws_cognito.IUserPool,
         disable_server_side_token_check: typing.Optional[builtins.bool] = None,
-        user_pool_client: typing.Optional[_aws_cdk_aws_cognito_ceddda9d.IUserPoolClient] = None,
+        user_pool_client: typing.Optional[aws_cdk.aws_cognito.IUserPoolClient] = None,
     ) -> None:
         '''(experimental) Props for the User Pool Authentication Provider.
 
         :param user_pool: (experimental) The User Pool of the Associated Identity Providers.
         :param disable_server_side_token_check: (experimental) Setting this to true turns off identity pool checks for this user pool to make sure the user has not been globally signed out or deleted before the identity pool provides an OIDC token or AWS credentials for the user. Default: false
         :param user_pool_client: (experimental) The User Pool Client for the provided User Pool. Default: - A default user pool client will be added to User Pool
 
         :stability: experimental
-        :exampleMetadata: infused
+        :exampleMetadata: fixture=_generated
 
         Example::
 
-            # identity_pool: IdentityPool
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.aws_cognito_identitypool_alpha as cognito_identitypool_alpha
+            from aws_cdk import aws_cognito as cognito
             
-            user_pool = cognito.UserPool(self, "Pool")
-            identity_pool.add_user_pool_authentication(UserPoolAuthenticationProvider(
+            # user_pool: cognito.UserPool
+            # user_pool_client: cognito.UserPoolClient
+            
+            user_pool_authentication_provider_props = cognito_identitypool_alpha.UserPoolAuthenticationProviderProps(
                 user_pool=user_pool,
-                disable_server_side_token_check=True
-            ))
+            
+                # the properties below are optional
+                disable_server_side_token_check=False,
+                user_pool_client=user_pool_client
+            )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__cdefc66d6c0c410084a508326629a8119aadc43267abbb8e697b3b9be03f9561)
-            check_type(argname="argument user_pool", value=user_pool, expected_type=type_hints["user_pool"])
-            check_type(argname="argument disable_server_side_token_check", value=disable_server_side_token_check, expected_type=type_hints["disable_server_side_token_check"])
-            check_type(argname="argument user_pool_client", value=user_pool_client, expected_type=type_hints["user_pool_client"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "user_pool": user_pool,
         }
         if disable_server_side_token_check is not None:
             self._values["disable_server_side_token_check"] = disable_server_side_token_check
         if user_pool_client is not None:
             self._values["user_pool_client"] = user_pool_client
 
     @builtins.property
-    def user_pool(self) -> _aws_cdk_aws_cognito_ceddda9d.IUserPool:
+    def user_pool(self) -> aws_cdk.aws_cognito.IUserPool:
         '''(experimental) The User Pool of the Associated Identity Providers.
 
         :stability: experimental
         '''
         result = self._values.get("user_pool")
         assert result is not None, "Required property 'user_pool' is missing"
-        return typing.cast(_aws_cdk_aws_cognito_ceddda9d.IUserPool, result)
+        return typing.cast(aws_cdk.aws_cognito.IUserPool, result)
 
     @builtins.property
     def disable_server_side_token_check(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Setting this to true turns off identity pool checks for this user pool to make sure the user has not been globally signed out or deleted before the identity pool provides an OIDC token or AWS credentials for the user.
 
         :default: false
 
         :see: https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-cognito-identitypool-cognitoidentityprovider.html
         :stability: experimental
         '''
         result = self._values.get("disable_server_side_token_check")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def user_pool_client(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_cognito_ceddda9d.IUserPoolClient]:
+    def user_pool_client(self) -> typing.Optional[aws_cdk.aws_cognito.IUserPoolClient]:
         '''(experimental) The User Pool Client for the provided User Pool.
 
         :default: - A default user pool client will be added to User Pool
 
         :stability: experimental
         '''
         result = self._values.get("user_pool_client")
-        return typing.cast(typing.Optional[_aws_cdk_aws_cognito_ceddda9d.IUserPoolClient], result)
+        return typing.cast(typing.Optional[aws_cdk.aws_cognito.IUserPoolClient], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -2574,23 +2416,23 @@
         "user_pools": "userPools",
     },
 )
 class IdentityPoolAuthenticationProviders(IdentityPoolProviders):
     def __init__(
         self,
         *,
-        amazon: typing.Optional[typing.Union[IdentityPoolAmazonLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-        apple: typing.Optional[typing.Union[IdentityPoolAppleLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-        digits: typing.Optional[typing.Union["IdentityPoolDigitsLoginProvider", typing.Dict[builtins.str, typing.Any]]] = None,
-        facebook: typing.Optional[typing.Union[IdentityPoolFacebookLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-        google: typing.Optional[typing.Union[IdentityPoolGoogleLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-        twitter: typing.Optional[typing.Union[IdentityPoolTwitterLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
+        amazon: typing.Optional[IdentityPoolAmazonLoginProvider] = None,
+        apple: typing.Optional[IdentityPoolAppleLoginProvider] = None,
+        digits: typing.Optional["IdentityPoolDigitsLoginProvider"] = None,
+        facebook: typing.Optional[IdentityPoolFacebookLoginProvider] = None,
+        google: typing.Optional[IdentityPoolGoogleLoginProvider] = None,
+        twitter: typing.Optional[IdentityPoolTwitterLoginProvider] = None,
         custom_provider: typing.Optional[builtins.str] = None,
-        open_id_connect_providers: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.IOpenIdConnectProvider]] = None,
-        saml_providers: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.ISamlProvider]] = None,
+        open_id_connect_providers: typing.Optional[typing.Sequence[aws_cdk.aws_iam.IOpenIdConnectProvider]] = None,
+        saml_providers: typing.Optional[typing.Sequence[aws_cdk.aws_iam.ISamlProvider]] = None,
         user_pools: typing.Optional[typing.Sequence[IUserPoolAuthenticationProvider]] = None,
     ) -> None:
         '''(experimental) Authentication providers for using in identity pool.
 
         :param amazon: (experimental) App Id for Amazon Identity Federation. Default: - No Amazon Authentication Provider used without OpenIdConnect or a User Pool
         :param apple: (experimental) Services Id for Apple Identity Federation. Default: - No Apple Authentication Provider used without OpenIdConnect or a User Pool
         :param digits: (experimental) Consumer Key and Secret for Digits Identity Federation. Default: - No Digits Authentication Provider used without OpenIdConnect or a User Pool
@@ -2600,56 +2442,67 @@
         :param custom_provider: (experimental) The Developer Provider Name to associate with this Identity Pool. Default: - no Custom Provider
         :param open_id_connect_providers: (experimental) The OpenIdConnect Provider associated with this Identity Pool. Default: - no OpenIdConnectProvider
         :param saml_providers: (experimental) The Security Assertion Markup Language Provider associated with this Identity Pool. Default: - no SamlProvider
         :param user_pools: (experimental) The User Pool Authentication Providers associated with this Identity Pool. Default: - no User Pools Associated
 
         :see: https://docs.aws.amazon.com/cognito/latest/developerguide/external-identity-providers.html
         :stability: experimental
-        :exampleMetadata: infused
+        :exampleMetadata: fixture=_generated
 
         Example::
 
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.aws_cognito_identitypool_alpha as cognito_identitypool_alpha
+            from aws_cdk import aws_iam as iam
+            
             # open_id_connect_provider: iam.OpenIdConnectProvider
+            # saml_provider: iam.SamlProvider
+            # user_pool_authentication_provider: cognito_identitypool_alpha.UserPoolAuthenticationProvider
             
-            IdentityPool(self, "myidentitypool",
-                identity_pool_name="myidentitypool",
-                authentication_providers=IdentityPoolAuthenticationProviders(
-                    google=IdentityPoolGoogleLoginProvider(
-                        client_id="12345678012.apps.googleusercontent.com"
-                    ),
-                    open_id_connect_providers=[open_id_connect_provider],
-                    custom_provider="my-custom-provider.example.com"
-                )
+            identity_pool_authentication_providers = cognito_identitypool_alpha.IdentityPoolAuthenticationProviders(
+                amazon=cognito_identitypool_alpha.IdentityPoolAmazonLoginProvider(
+                    app_id="appId"
+                ),
+                apple=cognito_identitypool_alpha.IdentityPoolAppleLoginProvider(
+                    services_id="servicesId"
+                ),
+                custom_provider="customProvider",
+                digits=cognito_identitypool_alpha.IdentityPoolDigitsLoginProvider(
+                    consumer_key="consumerKey",
+                    consumer_secret="consumerSecret"
+                ),
+                facebook=cognito_identitypool_alpha.IdentityPoolFacebookLoginProvider(
+                    app_id="appId"
+                ),
+                google=cognito_identitypool_alpha.IdentityPoolGoogleLoginProvider(
+                    client_id="clientId"
+                ),
+                open_id_connect_providers=[open_id_connect_provider],
+                saml_providers=[saml_provider],
+                twitter=cognito_identitypool_alpha.IdentityPoolTwitterLoginProvider(
+                    consumer_key="consumerKey",
+                    consumer_secret="consumerSecret"
+                ),
+                user_pools=[user_pool_authentication_provider]
             )
         '''
         if isinstance(amazon, dict):
             amazon = IdentityPoolAmazonLoginProvider(**amazon)
         if isinstance(apple, dict):
             apple = IdentityPoolAppleLoginProvider(**apple)
         if isinstance(digits, dict):
             digits = IdentityPoolDigitsLoginProvider(**digits)
         if isinstance(facebook, dict):
             facebook = IdentityPoolFacebookLoginProvider(**facebook)
         if isinstance(google, dict):
             google = IdentityPoolGoogleLoginProvider(**google)
         if isinstance(twitter, dict):
             twitter = IdentityPoolTwitterLoginProvider(**twitter)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2e83f8914cae586eb38cf0016d133dd934c291cad25f28b936d459ade0c5d887)
-            check_type(argname="argument amazon", value=amazon, expected_type=type_hints["amazon"])
-            check_type(argname="argument apple", value=apple, expected_type=type_hints["apple"])
-            check_type(argname="argument digits", value=digits, expected_type=type_hints["digits"])
-            check_type(argname="argument facebook", value=facebook, expected_type=type_hints["facebook"])
-            check_type(argname="argument google", value=google, expected_type=type_hints["google"])
-            check_type(argname="argument twitter", value=twitter, expected_type=type_hints["twitter"])
-            check_type(argname="argument custom_provider", value=custom_provider, expected_type=type_hints["custom_provider"])
-            check_type(argname="argument open_id_connect_providers", value=open_id_connect_providers, expected_type=type_hints["open_id_connect_providers"])
-            check_type(argname="argument saml_providers", value=saml_providers, expected_type=type_hints["saml_providers"])
-            check_type(argname="argument user_pools", value=user_pools, expected_type=type_hints["user_pools"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if amazon is not None:
             self._values["amazon"] = amazon
         if apple is not None:
             self._values["apple"] = apple
         if digits is not None:
             self._values["digits"] = digits
         if facebook is not None:
@@ -2743,36 +2596,36 @@
         '''
         result = self._values.get("custom_provider")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def open_id_connect_providers(
         self,
-    ) -> typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.IOpenIdConnectProvider]]:
+    ) -> typing.Optional[typing.List[aws_cdk.aws_iam.IOpenIdConnectProvider]]:
         '''(experimental) The OpenIdConnect Provider associated with this Identity Pool.
 
         :default: - no OpenIdConnectProvider
 
         :stability: experimental
         '''
         result = self._values.get("open_id_connect_providers")
-        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.IOpenIdConnectProvider]], result)
+        return typing.cast(typing.Optional[typing.List[aws_cdk.aws_iam.IOpenIdConnectProvider]], result)
 
     @builtins.property
     def saml_providers(
         self,
-    ) -> typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.ISamlProvider]]:
+    ) -> typing.Optional[typing.List[aws_cdk.aws_iam.ISamlProvider]]:
         '''(experimental) The Security Assertion Markup Language Provider associated with this Identity Pool.
 
         :default: - no SamlProvider
 
         :stability: experimental
         '''
         result = self._values.get("saml_providers")
-        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.ISamlProvider]], result)
+        return typing.cast(typing.Optional[typing.List[aws_cdk.aws_iam.ISamlProvider]], result)
 
     @builtins.property
     def user_pools(
         self,
     ) -> typing.Optional[typing.List[IUserPoolAuthenticationProvider]]:
         '''(experimental) The User Pool Authentication Providers associated with this Identity Pool.
 
@@ -2822,19 +2675,15 @@
             import aws_cdk.aws_cognito_identitypool_alpha as cognito_identitypool_alpha
             
             identity_pool_digits_login_provider = cognito_identitypool_alpha.IdentityPoolDigitsLoginProvider(
                 consumer_key="consumerKey",
                 consumer_secret="consumerSecret"
             )
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__acb7b8a984ce1029f7726d4404e76a0e87a2a50e6222dd49f78200cdc1a4f0e8)
-            check_type(argname="argument consumer_key", value=consumer_key, expected_type=type_hints["consumer_key"])
-            check_type(argname="argument consumer_secret", value=consumer_secret, expected_type=type_hints["consumer_secret"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "consumer_key": consumer_key,
             "consumer_secret": consumer_secret,
         }
 
     @builtins.property
     def consumer_key(self) -> builtins.str:
         '''(experimental) App Id for Twitter Identity Federation.
@@ -2891,241 +2740,7 @@
     "UserPoolAuthenticationProvider",
     "UserPoolAuthenticationProviderBindConfig",
     "UserPoolAuthenticationProviderBindOptions",
     "UserPoolAuthenticationProviderProps",
 ]
 
 publication.publish()
-
-def _typecheckingstub__07632ef1025feb6e05894b02941c351317dc03c46357f2c76f22433d4b28396c(
-    scope: _constructs_77d1e7e8.Construct,
-    identity_pool: IIdentityPool,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__af2f072d5cac259fbc65a0c4a6a8cb785ff9ebcf2da91f9184be84a22820a980(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    allow_classic_flow: typing.Optional[builtins.bool] = None,
-    allow_unauthenticated_identities: typing.Optional[builtins.bool] = None,
-    authenticated_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-    authentication_providers: typing.Optional[typing.Union[IdentityPoolAuthenticationProviders, typing.Dict[builtins.str, typing.Any]]] = None,
-    identity_pool_name: typing.Optional[builtins.str] = None,
-    role_mappings: typing.Optional[typing.Sequence[typing.Union[IdentityPoolRoleMapping, typing.Dict[builtins.str, typing.Any]]]] = None,
-    unauthenticated_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a95e191d26141b46fee8d2cdcabc0803b18860942f1a248701db0dae81123def(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    identity_pool_arn: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b5abb9f2926d1e1f17a15fd6b4211f8951279c31ec22f381103f75200b458fa1(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    identity_pool_id: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__79c997ed6a533e453fd1b182579d72149933074796ba9e81e6eee7479bbb0ea9(
-    *role_mappings: IdentityPoolRoleMapping,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__fbd9ea8a4c738095932e3cf624c6eb098117704692279323d27952d6b2df0e00(
-    user_pool: IUserPoolAuthenticationProvider,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__b9e283aa49d3946357252123279fe3e514c02786d6dbaf36c03180cb06444fd8(
-    *,
-    app_id: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e7c9040769cdc703f1660cd3e3da515a34764b5e7c1c0fe8e072609ef85af66f(
-    *,
-    services_id: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__553a6105b1cc099f5bb05790fda107ae2e28e4a5891f7d4400f19cddf53e926e(
-    *,
-    app_id: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__dc7d7863b86c1b6983201a7e628ab0bb505b6719534f708df8a6c31427dbb5bb(
-    *,
-    client_id: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__67b8242ca2e55a1962a36ef0e9c4b94eae811b93839b5e265f5743512e5ca12b(
-    *,
-    allow_classic_flow: typing.Optional[builtins.bool] = None,
-    allow_unauthenticated_identities: typing.Optional[builtins.bool] = None,
-    authenticated_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-    authentication_providers: typing.Optional[typing.Union[IdentityPoolAuthenticationProviders, typing.Dict[builtins.str, typing.Any]]] = None,
-    identity_pool_name: typing.Optional[builtins.str] = None,
-    role_mappings: typing.Optional[typing.Sequence[typing.Union[IdentityPoolRoleMapping, typing.Dict[builtins.str, typing.Any]]]] = None,
-    unauthenticated_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__423f3af9588f321b47a169a44fe143eb961b0377418e1736dde381403db8730e(
-    type: IdentityPoolProviderType,
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__aba4eac2376a67f469d725ea627955e1696d934a6d0601d7e4873d8b2b48d749(
-    url: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__3d161a44d12cc621bec8346b7a54def25199238af1ee02be289568c2abb4aed2(
-    url: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0cbf2fc0f2dbf61ab8ba7e761e45e78a8d5d3bbfa64ccc8f8d93bff656c1a825(
-    url: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__7531b9fff4293227d6e5c746c9e82a2d3b5164eaf82e984877f422ff7de768c9(
-    url: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__6da31bad5d5f044fd941ec5cc9821499624050d72b9556e6891a7a76644b8330(
-    *,
-    amazon: typing.Optional[typing.Union[IdentityPoolAmazonLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-    apple: typing.Optional[typing.Union[IdentityPoolAppleLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-    digits: typing.Optional[typing.Union[IdentityPoolDigitsLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-    facebook: typing.Optional[typing.Union[IdentityPoolFacebookLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-    google: typing.Optional[typing.Union[IdentityPoolGoogleLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-    twitter: typing.Optional[typing.Union[IdentityPoolTwitterLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__a165e7b7d8cd676948cb9b98c9ae060e6da6931de2231f73fb8bfe09c571e8f3(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    identity_pool: IIdentityPool,
-    authenticated_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-    role_mappings: typing.Optional[typing.Sequence[typing.Union[IdentityPoolRoleMapping, typing.Dict[builtins.str, typing.Any]]]] = None,
-    unauthenticated_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__275eb74a4a88284000b15066daef659c73082e99224df6491b0465af179ac6b4(
-    *,
-    identity_pool: IIdentityPool,
-    authenticated_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-    role_mappings: typing.Optional[typing.Sequence[typing.Union[IdentityPoolRoleMapping, typing.Dict[builtins.str, typing.Any]]]] = None,
-    unauthenticated_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__650ad537013ada6fb730b758a9cc04e3e889c73469adb530187b60e65137d653(
-    *,
-    provider_url: IdentityPoolProviderUrl,
-    mapping_key: typing.Optional[builtins.str] = None,
-    resolve_ambiguous_roles: typing.Optional[builtins.bool] = None,
-    rules: typing.Optional[typing.Sequence[typing.Union[RoleMappingRule, typing.Dict[builtins.str, typing.Any]]]] = None,
-    use_token: typing.Optional[builtins.bool] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__f91153aca8aea767279ad014c0a8369ca2e36afc6e9b02f0111bc64f713b104f(
-    *,
-    consumer_key: builtins.str,
-    consumer_secret: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__77869f331952f425fa372fe2f927e6224793554cefa649c244780e367abe94a9(
-    *,
-    claim: builtins.str,
-    claim_value: builtins.str,
-    mapped_role: _aws_cdk_aws_iam_ceddda9d.IRole,
-    match_type: typing.Optional[RoleMappingMatchType] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e3c3e4f47b37f4d3265edfa6c7ad01b5c1409a21b5450216878fdce228df9f72(
-    scope: _constructs_77d1e7e8.Construct,
-    identity_pool: IIdentityPool,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__f7b8fa9dab857d092fcc38b5be232ff1c0998d006d07c8ef726d2a6530e5df52(
-    *,
-    client_id: builtins.str,
-    provider_name: builtins.str,
-    server_side_token_check: builtins.bool,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__cdefc66d6c0c410084a508326629a8119aadc43267abbb8e697b3b9be03f9561(
-    *,
-    user_pool: _aws_cdk_aws_cognito_ceddda9d.IUserPool,
-    disable_server_side_token_check: typing.Optional[builtins.bool] = None,
-    user_pool_client: typing.Optional[_aws_cdk_aws_cognito_ceddda9d.IUserPoolClient] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__2e83f8914cae586eb38cf0016d133dd934c291cad25f28b936d459ade0c5d887(
-    *,
-    amazon: typing.Optional[typing.Union[IdentityPoolAmazonLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-    apple: typing.Optional[typing.Union[IdentityPoolAppleLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-    digits: typing.Optional[typing.Union[IdentityPoolDigitsLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-    facebook: typing.Optional[typing.Union[IdentityPoolFacebookLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-    google: typing.Optional[typing.Union[IdentityPoolGoogleLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-    twitter: typing.Optional[typing.Union[IdentityPoolTwitterLoginProvider, typing.Dict[builtins.str, typing.Any]]] = None,
-    custom_provider: typing.Optional[builtins.str] = None,
-    open_id_connect_providers: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.IOpenIdConnectProvider]] = None,
-    saml_providers: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.ISamlProvider]] = None,
-    user_pools: typing.Optional[typing.Sequence[IUserPoolAuthenticationProvider]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__acb7b8a984ce1029f7726d4404e76a0e87a2a50e6222dd49f78200cdc1a4f0e8(
-    *,
-    consumer_key: builtins.str,
-    consumer_secret: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
```

### Comparing `aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-cognito-identitypool-alpha
-Version: 2.84.0a0
+Version: 2.9.0a0
 Summary: The CDK Construct Library for AWS::Cognito Identity Pools
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
 
 # Amazon Cognito Identity Pool Construct Library
 
 > **Identity Pools are in a separate module while the API is being stabilized. Once we stabilize the module, they will**
@@ -52,18 +52,14 @@
 a third party such as Facebook, Amazon, Google or Apple.
 
 The other main component in Amazon Cognito is [user pools](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-identity-pools.html). User Pools are user directories that provide sign-up and
 sign-in options for your app users.
 
 This module is part of the [AWS Cloud Development Kit](https://github.com/aws/aws-cdk) project.
 
-```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPool, UserPoolAuthenticationProvider
-```
-
 ## Table of Contents
 
 * [Identity Pools](#identity-pools)
 
   * [Authenticated and Unauthenticated Identities](#authenticated-and-unauthenticated-identities)
   * [Authentication Providers](#authentication-providers)
 
@@ -94,53 +90,52 @@
 identities, and a default role for unauthenticated identities. Absent other overriding rules (see below), these are the
 roles that will be assumed by the corresponding users in the authentication process.
 
 A basic Identity Pool with minimal configuration has no required props, with default authenticated (user) and
 unauthenticated (guest) roles applied to the identity pool:
 
 ```python
-IdentityPool(self, "myIdentityPool")
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myIdentityPool")
 ```
 
 By default, both the authenticated and unauthenticated roles will have no permissions attached. Grant permissions
 to roles using the public `authenticatedRole` and `unauthenticatedRole` properties:
 
 ```python
-import aws_cdk.aws_dynamodb as dynamodb
-# table: dynamodb.Table
-
-
-identity_pool = IdentityPool(self, "myIdentityPool")
+# Example automatically generated from non-compiling source. May contain errors.
+identity_pool = cognito.IdentityPool(self, "myIdentityPool")
+table = dynamodb.Table(self, "MyTable")
 
 # Grant permissions to authenticated users
 table.grant_read_write_data(identity_pool.authenticated_role)
 # Grant permissions to unauthenticated guest users
-table.grant_read_data(identity_pool.unauthenticated_role)
+table.grant_read(identity_pool.unauthenticated_role)
 
 # Or add policy statements straight to the role
-identity_pool.authenticated_role.add_to_principal_policy(iam.PolicyStatement(
-    effect=iam.Effect.ALLOW,
+identity_pool.authenticated_role.add_to_principal_policy(PolicyStatement(
+    effect=Effect.ALLOW,
     actions=["dynamodb:*"],
     resources=["*"]
 ))
 ```
 
 The default roles can also be supplied in `IdentityPoolProps`:
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 stack = Stack()
-authenticated_role = iam.Role(self, "authRole",
-    assumed_by=iam.ServicePrincipal("service.amazonaws.com")
+authenticated_role = Role(stack, "authRole",
+    assumed_by=ServicePrincipal("service.amazonaws.com")
 )
-unauthenticated_role = iam.Role(self, "unauthRole",
-    assumed_by=iam.ServicePrincipal("service.amazonaws.com")
+unauthenticated_role = Role(stack, "unauthRole",
+    assumed_by=ServicePrincipal("service.amazonaws.com")
 )
-identity_pool = IdentityPool(self, "TestIdentityPoolActions",
-    authenticated_role=authenticated_role,
-    unauthenticated_role=unauthenticated_role
+identity_pool = IdentityPool(stack, "TestIdentityPoolActions",
+    authenticated_role=authenticated_role, unauthenticated_role=unauthenticated_role
 )
 ```
 
 ### Authentication Providers
 
 Authenticated identities belong to users who are authenticated by a public login provider (Amazon Cognito user pools,
 Login with Amazon, Sign in with Apple, Facebook, Google, SAML, or any OpenID Connect Providers) or a developer provider
@@ -152,34 +147,34 @@
 #### User Pool Authentication Provider
 
 In order to attach a user pool to an identity pool as an authentication provider, the identity pool needs properties
 from both the user pool and the user pool client. For this reason identity pools use a `UserPoolAuthenticationProvider`
 to gather the necessary properties from the user pool constructs.
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 user_pool = cognito.UserPool(self, "Pool")
 
-IdentityPool(self, "myidentitypool",
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    authentication_providers=IdentityPoolAuthenticationProviders(
-        user_pools=[UserPoolAuthenticationProvider(user_pool=user_pool)]
-    )
+    authentication_providers={
+        "user_pools": [UserPoolAuthenticationProvider(user_pool=user_pool)]
+    }
 )
 ```
 
 User pools can also be associated with an identity pool after instantiation. The Identity Pool's `addUserPoolAuthentication` method
 returns the User Pool Client that has been created:
 
 ```python
-# identity_pool: IdentityPool
-
+# Example automatically generated from non-compiling source. May contain errors.
 user_pool = cognito.UserPool(self, "Pool")
-user_pool_client = identity_pool.add_user_pool_authentication(UserPoolAuthenticationProvider(
-    user_pool=user_pool
-))
+user_pool_client = identity_pool.add_user_pool_authentication(
+    user_pools=[UserPoolAuthenticationProvider(user_pool=user_pool)]
+)
 ```
 
 #### Server Side Token Check
 
 With the `IdentityPool` CDK Construct, by default the pool is configured to check with the integrated user pools to
 make sure that the user has not been globally signed out or deleted before the identity pool provides an OIDC token or
 AWS credentials for the user.
@@ -187,49 +182,51 @@
 If the user is signed out or deleted, the identity pool will return a 400 Not Authorized error. This setting can be
 disabled, however, in several ways.
 
 Setting `disableServerSideTokenCheck` to true will change the default behavior to no server side token check. Learn
 more [here](https://docs.aws.amazon.com/cognitoidentity/latest/APIReference/API_CognitoIdentityProvider.html#CognitoIdentity-Type-CognitoIdentityProvider-ServerSideTokenCheck):
 
 ```python
-# identity_pool: IdentityPool
-
+# Example automatically generated from non-compiling source. May contain errors.
 user_pool = cognito.UserPool(self, "Pool")
-identity_pool.add_user_pool_authentication(UserPoolAuthenticationProvider(
-    user_pool=user_pool,
-    disable_server_side_token_check=True
-))
+identity_pool.add_user_pool_authentication(
+    user_pool=UserPoolAuthenticationProvider(
+        user_pool=user_pool,
+        disable_server_side_token_check=True
+    )
+)
 ```
 
 #### Associating an External Provider Directly
 
 One or more [external identity providers](https://docs.aws.amazon.com/cognito/latest/developerguide/external-identity-providers.html) can be associated with an identity pool directly using
 `authenticationProviders`:
 
 ```python
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    authentication_providers=IdentityPoolAuthenticationProviders(
-        amazon=IdentityPoolAmazonLoginProvider(
-            app_id="amzn1.application.12312k3j234j13rjiwuenf"
-        ),
-        facebook=IdentityPoolFacebookLoginProvider(
-            app_id="1234567890123"
-        ),
-        google=IdentityPoolGoogleLoginProvider(
-            client_id="12345678012.apps.googleusercontent.com"
-        ),
-        apple=IdentityPoolAppleLoginProvider(
-            services_id="com.myappleapp.auth"
-        ),
-        twitter=IdentityPoolTwitterLoginProvider(
-            consumer_key="my-twitter-id",
-            consumer_secret="my-twitter-secret"
-        )
-    )
+    authentication_providers={
+        "amazon": {
+            "app_id": "amzn1.application.12312k3j234j13rjiwuenf"
+        },
+        "facebook": {
+            "app_id": "1234567890123"
+        },
+        "google": {
+            "client_id": "12345678012.apps.googleusercontent.com"
+        },
+        "apple": {
+            "services_id": "com.myappleapp.auth"
+        },
+        "twitter": {
+            "consumer_key": "my-twitter-id",
+            "consumer_secret": "my-twitter-secret"
+        }
+    }
 )
 ```
 
 To associate more than one provider of the same type with the identity pool, use User
 Pools, OpenIdConnect, or SAML. Only one provider per external service can be attached directly to the identity pool.
 
 #### OpenId Connect and Saml
@@ -240,182 +237,143 @@
 
 An identity provider that supports [Security Assertion Markup Language 2.0 (SAML 2.0)](https://docs.aws.amazon.com/cognito/latest/developerguide/saml-identity-provider.html) can be used to provide a simple
 onboarding flow for users. The SAML-supporting identity provider specifies the IAM roles that can be assumed by users
 so that different users can be granted different sets of permissions. Associating an OpenId Connect or Saml provider
 with an identity pool:
 
 ```python
-# open_id_connect_provider: iam.OpenIdConnectProvider
-# saml_provider: iam.SamlProvider
-
+# Example automatically generated from non-compiling source. May contain errors.
+open_id_connect_provider = iam.OpenIdConnectProvider(self, "my-openid-connect-provider", ...)
+saml_provider = iam.SamlProvider(self, "my-saml-provider", ...)
 
-IdentityPool(self, "myidentitypool",
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    authentication_providers=IdentityPoolAuthenticationProviders(
-        open_id_connect_providers=[open_id_connect_provider],
-        saml_providers=[saml_provider]
-    )
+    authentication_providers={
+        "open_id_connect_provider": open_id_connect_provider,
+        "saml_provider": saml_provider
+    }
 )
 ```
 
 #### Custom Providers
 
 The identity pool's behavior can be customized further using custom [developer authenticated identities](https://docs.aws.amazon.com/cognito/latest/developerguide/developer-authenticated-identities.html).
 With developer authenticated identities, users can be registered and authenticated via an existing authentication
 process while still using Amazon Cognito to synchronize user data and access AWS resources.
 
 Like the supported external providers, though, only one custom provider can be directly associated with the identity
 pool.
 
 ```python
-# open_id_connect_provider: iam.OpenIdConnectProvider
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    authentication_providers=IdentityPoolAuthenticationProviders(
-        google=IdentityPoolGoogleLoginProvider(
-            client_id="12345678012.apps.googleusercontent.com"
-        ),
-        open_id_connect_providers=[open_id_connect_provider],
-        custom_provider="my-custom-provider.example.com"
-    )
+    authentication_providers={
+        "google": "12345678012.apps.googleusercontent.com",
+        "open_id_connect_provider": open_id_connect_provider,
+        "custom_provider": "my-custom-provider.example.com"
+    }
 )
 ```
 
 ### Role Mapping
 
 In addition to setting default roles for authenticated and unauthenticated users, identity pools can also be used to
 define rules to choose the role for each user based on claims in the user's ID token by using Role Mapping. When using
 role mapping, it's important to be aware of some of the permissions the role will need. An in depth
 review of roles and role mapping can be found [here](https://docs.aws.amazon.com/cognito/latest/developerguide/role-based-access-control.html).
 
 Using a [token-based approach](https://docs.aws.amazon.com/cognito/latest/developerguide/role-based-access-control.html#using-tokens-to-assign-roles-to-users) to role mapping will allow mapped roles to be passed through the `cognito:roles` or
 `cognito:preferred_role` claims from the identity provider:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl
-
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    role_mappings=[IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.AMAZON,
-        use_token=True
-    )]
+    role_mappings=[{
+        "provider_url": IdentityPoolProviderUrl.AMAZON,
+        "use_token": True
+    }]
 )
 ```
 
-Using a rule-based approach to role mapping allows roles to be assigned based on custom claims passed from the identity provider:
+Using a rule-based approach to role mapping allows roles to be assigned based on custom claims passed from the identity  provider:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl, RoleMappingMatchType
-
-# admin_role: iam.Role
-# non_admin_role: iam.Role
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
     # Assign specific roles to users based on whether or not the custom admin claim is passed from the identity provider
-    role_mappings=[IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.AMAZON,
-        rules=[RoleMappingRule(
-            claim="custom:admin",
-            claim_value="admin",
-            mapped_role=admin_role
-        ), RoleMappingRule(
-            claim="custom:admin",
-            claim_value="admin",
-            match_type=RoleMappingMatchType.NOTEQUAL,
-            mapped_role=non_admin_role
-        )
+    role_mappings=[{
+        "provider_url": IdentityPoolProviderUrl.AMAZON,
+        "rules": [{
+            "claim": "custom:admin",
+            "claim_value": "admin",
+            "mapped_role": admin_role
+        }, {
+            "claim": "custom:admin",
+            "claim_value": "admin",
+            "match_type": RoleMappingMatchType.NOTEQUAL,
+            "mapped_role": non_admin_role
+        }
         ]
-    )]
+    }]
 )
 ```
 
 Role mappings can also be added after instantiation with the Identity Pool's `addRoleMappings` method:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolRoleMapping
-
-# identity_pool: IdentityPool
-# my_added_role_mapping1: IdentityPoolRoleMapping
-# my_added_role_mapping2: IdentityPoolRoleMapping
-# my_added_role_mapping3: IdentityPoolRoleMapping
-
-
+# Example automatically generated from non-compiling source. May contain errors.
 identity_pool.add_role_mappings(my_added_role_mapping1, my_added_role_mapping2, my_added_role_mapping3)
 ```
 
 #### Provider Urls
 
 Role mappings must be associated with the url of an Identity Provider which can be supplied
 `IdentityPoolProviderUrl`. Supported Providers have static Urls that can be used:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl
-
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    role_mappings=[IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.FACEBOOK,
-        use_token=True
-    )]
+    role_mappings=[{
+        "provider_url": IdentityPoolProviderUrl.FACEBOOK,
+        "use_token": True
+    }]
 )
 ```
 
 For identity providers that don't have static Urls, a custom Url or User Pool Client Url can be supplied:
 
 ```python
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl
-
-
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
-    role_mappings=[IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.user_pool("cognito-idp.my-idp-region.amazonaws.com/my-idp-region_abcdefghi:app_client_id"),
-        use_token=True
-    ), IdentityPoolRoleMapping(
-        provider_url=IdentityPoolProviderUrl.custom("my-custom-provider.com"),
-        use_token=True
-    )
+    role_mappings=[{
+        "provider_url": IdentityPoolProviderUrl.user_pool("cognito-idp.my-idp-region.amazonaws.com/my-idp-region_abcdefghi:app_client_id"),
+        "use_token": True
+    }, {
+        "provider_url": IdentityPoolProviderUrl.custom("my-custom-provider.com"),
+        "use_token": True
+    }
     ]
 )
 ```
 
-If a provider URL is a CDK Token, as it will be if you are trying to use a previously defined Cognito User Pool, you will need to also provide a mappingKey.
-This is because by default, the key in the Cloudformation role mapping hash is the providerUrl, and Cloudformation map keys must be concrete strings, they
-cannot be references. For example:
-
-```python
-from aws_cdk.aws_cognito import UserPool
-from aws_cdk.aws_cognito_identitypool_alpha import IdentityPoolProviderUrl
-
-# user_pool: UserPool
-
-IdentityPool(self, "myidentitypool",
-    identity_pool_name="myidentitypool",
-    role_mappings=[IdentityPoolRoleMapping(
-        mapping_key="cognito",
-        provider_url=IdentityPoolProviderUrl.user_pool(user_pool.user_pool_provider_url),
-        use_token=True
-    )]
-)
-```
-
 See [here](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-cognito-identitypoolroleattachment-rolemapping.html#cfn-cognito-identitypoolroleattachment-rolemapping-identityprovider) for more information.
 
 ### Authentication Flow
 
 Identity Pool [Authentication Flow](https://docs.aws.amazon.com/cognito/latest/developerguide/authentication-flow.html) defaults to the enhanced, simplified flow. The Classic (basic) Authentication Flow
 can also be implemented using `allowClassicFlow`:
 
 ```python
-IdentityPool(self, "myidentitypool",
+# Example automatically generated from non-compiling source. May contain errors.
+cognito.IdentityPool(self, "myidentitypool",
     identity_pool_name="myidentitypool",
     allow_classic_flow=True
 )
 ```
 
 ### Cognito Sync
 
@@ -425,10 +383,13 @@
 
 ### Importing Identity Pools
 
 You can import existing identity pools into your stack using Identity Pool static methods with the Identity Pool Id or
 Arn:
 
 ```python
+# Example automatically generated from non-compiling source. May contain errors.
 IdentityPool.from_identity_pool_id(self, "my-imported-identity-pool", "us-east-1:dj2823ryiwuhef937")
 IdentityPool.from_identity_pool_arn(self, "my-imported-identity-pool", "arn:aws:cognito-identity:us-east-1:123456789012:identitypool/us-east-1:dj2823ryiwuhef937")
 ```
+
+
```

### Comparing `aws-cdk.aws-cognito-identitypool-alpha-2.84.0a0/src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-cognito-identitypool-alpha-2.9.0a0/src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/requires.txt
 src/aws_cdk.aws_cognito_identitypool_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_cognito_identitypool_alpha/__init__.py
 src/aws_cdk/aws_cognito_identitypool_alpha/py.typed
 src/aws_cdk/aws_cognito_identitypool_alpha/_jsii/__init__.py
-src/aws_cdk/aws_cognito_identitypool_alpha/_jsii/aws-cognito-identitypool-alpha@2.84.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_cognito_identitypool_alpha/_jsii/aws-cognito-identitypool-alpha@2.9.0-alpha.0.jsii.tgz
```

