# Comparing `tmp/scribeauth-1.0.4-py3-none-any.whl.zip` & `tmp/scribeauth-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7623 bytes, number of entries: 9
+Zip file size: 8050 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat       66 b- defN 23-May-17 09:44 scribeauth/__init__.py
 -rw-rw-rw-  2.0 fat      521 b- defN 23-Jun-12 14:20 scribeauth/__main__.py
--rw-rw-rw-  2.0 fat    13230 b- defN 23-Jun-14 09:44 scribeauth/scribeauth.py
+-rw-rw-rw-  2.0 fat    14380 b- defN 23-Jun-14 18:03 scribeauth/scribeauth.py
 -rw-rw-rw-  2.0 fat     1351 b- defN 23-May-15 17:21 scribeauth/scribeauthfederation.py
--rw-rw-rw-  2.0 fat     1097 b- defN 23-Jun-14 09:45 scribeauth-1.0.4.dist-info/LICENSE.md
--rw-rw-rw-  2.0 fat     4400 b- defN 23-Jun-14 09:45 scribeauth-1.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-14 09:45 scribeauth-1.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-14 09:45 scribeauth-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      732 b- defN 23-Jun-14 09:45 scribeauth-1.0.4.dist-info/RECORD
-9 files, 21500 bytes uncompressed, 6359 bytes compressed:  70.4%
+-rw-rw-rw-  2.0 fat     1097 b- defN 23-Jun-14 18:04 scribeauth-1.0.5.dist-info/LICENSE.md
+-rw-rw-rw-  2.0 fat     5073 b- defN 23-Jun-14 18:04 scribeauth-1.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-14 18:04 scribeauth-1.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-14 18:04 scribeauth-1.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      732 b- defN 23-Jun-14 18:04 scribeauth-1.0.5.dist-info/RECORD
+9 files, 23323 bytes uncompressed, 6786 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: scribeauth/scribeauth.py
 Comment: 
 
 Filename: scribeauth/scribeauthfederation.py
 Comment: 
 
-Filename: scribeauth-1.0.4.dist-info/LICENSE.md
+Filename: scribeauth-1.0.5.dist-info/LICENSE.md
 Comment: 
 
-Filename: scribeauth-1.0.4.dist-info/METADATA
+Filename: scribeauth-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: scribeauth-1.0.4.dist-info/WHEEL
+Filename: scribeauth-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: scribeauth-1.0.4.dist-info/top_level.txt
+Filename: scribeauth-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: scribeauth-1.0.4.dist-info/RECORD
+Filename: scribeauth-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## scribeauth/scribeauth.py

```diff
@@ -1,12 +1,15 @@
 from typing import List, TypedDict, Union
 from typing_extensions import Unpack
 import boto3
 import botocore
 from botocore.config import Config
+from botocore.auth import SigV4Auth
+from botocore.awsrequest import AWSRequest
+import botocore.session
 
 
 class Tokens(TypedDict):
     refresh_token: str
     access_token: str
     id_token: str
 
@@ -282,14 +285,43 @@
             return response['Credentials']
         except Exception as err:
             if err.response['Error']['Code'] == 'NotAuthorizedException':
                 raise UnauthorizedException('Could not retrieve federated credentials')
             if err.response['Error']['Code'] == 'TooManyRequestsException':
                 raise TooManyRequestsException('Too many requests. Try again later')
             raise err
+        
+    def get_signature_for_request(self, request: AWSRequest, credentials: Credentials):
+        """A user gets a signature for a request.
+
+        Args
+        ----
+
+        request -- Request to send.
+
+        credentials -- Credentials for the signature creation.
+
+        Returns
+        -------
+        Headers -- Headers containing the signature for the request.
+        """
+        try:
+            session = botocore.session.Session()
+            session.set_credentials(access_key=credentials['AccessKeyId'], secret_key=credentials['SecretKey'], token=credentials['SessionToken'])
+            signer = SigV4Auth(
+                credentials=session.get_credentials(),
+                service_name='execute-api',
+                region_name='eu-west-2')
+            request.context["payload_signing_enabled"] = False
+            signer.add_auth(request=request)
+            prepped = request.prepare()
+            return prepped.headers
+        except Exception as err:
+            raise err
+      
 
     def __get_tokens_with_pair(self, username: str, password: str):
         auth_result = 'AuthenticationResult'
         if username != None and password != None:
             try:
                 response = self.__initiate_auth(username, password)
                 result = response.get(auth_result)
```

## Comparing `scribeauth-1.0.4.dist-info/LICENSE.md` & `scribeauth-1.0.5.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `scribeauth-1.0.4.dist-info/METADATA` & `scribeauth-1.0.5.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,124 +1,130 @@
-Metadata-Version: 2.1
-Name: scribeauth
-Version: 1.0.4
-Summary: Library to authenticate to Scribe's platform
-Home-page: https://github.com/ScribeLabsAI/ScribeAuth
-Author: Ailin Venerus
-Author-email: ailin@scribelabs.ai
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Security
-Classifier: Typing :: Typed
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: boto3
-Requires-Dist: typing-extensions
-
-# Scribe Auth
-
-Most calls to Scribe's API require authentication and authorization. This library simplifies this process.
-
-You first need a Scribe account and a client ID. Both can be requested at support[atsign]scribelabs[dotsign]ai or through Intercom on https://platform.scribelabs.ai if you already have a Scribe account.
-
-This library interacts directly with our authentication provider [AWS Cognito](https://aws.amazon.com/cognito/) meaning that your username and password never transit through our servers.
-
-## Installation
-
-```bash
-pip install scribeauth
-```
-
-This library requires Python >= 3.10 that supports typing.
-
-## Methods
-
-### 1. Changing password
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth(client_id)
-access.change_password('username', 'password', 'new_password')
-```
-
-### 2. Recovering an account in case of forgotten password
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth(client_id)
-access.forgot_password('username', 'password', 'confirmation_code')
-```
-
-### 3. Get or generate tokens
-
-##### With username and password
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth(client_id)
-access.get_tokens(username='username', password='password')
-```
-
-##### With refresh token
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth(client_id)
-access.get_tokens(refresh_token='refresh_token')
-```
-
-### 4. Revoking a refresh token
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth(client_id)
-access.revoke_refresh_token('refresh_token')
-```
-
-### 5. Getting federated id
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth({'client_id': your_client_id, 'user_pool_id': your_user_pool_id, 'identity_pool_id': your_identity_pool_id})
-access.get_federated_id('your_id_token')
-```
-
-### 6. Getting federated credentials
-
-```python
-from scribeauth import ScribeAuth
-access = ScribeAuth({'client_id': your_client_id, 'user_pool_id': your_user_pool_id, 'identity_pool_id': your_identity_pool_id})
-access.get_federated_credentials('your_federated_id', 'your_id_token')
-```
-
-## Flow
-
-- If you never have accessed your Scribe account, it probably still contains the temporary password we generated for you. You can change it directly on the [platform](https://platform.scribelabs.ai) or with the `change_password` method. You won't be able to access anything else until the temporary password has been changed.
-
-- Once the account is up and running, you can request new tokens with `get_tokens`. You will initially have to provide your username and password. The access and id tokens are valid for up to 30 minutes. The refresh token is valid for 30 days.
-
-- While you have a valid refresh token, you can request fresh access and id tokens with `get_tokens` but using the refresh token this time, so you're not sending your username and password over the wire anymore.
-
-- In case you suspect that your refresh token has been leaked, you can revoke it with `revoke_token`. This will also invalidate any access/id token that has been issued with it. In order to get a new one, you'll need to use your username and password again.
-
-- You can get your federated id by using `get_federated_id` and providing your id token. The federated id will allow you to use `get_federated_credentials` to get an access key id, secret key and session token.
-
-## Command line
-
-You can also use the package as follows for quick access to tokens:
-
-```bash
-python -m scribeauth --client_id clientid --username username --password password
-```
-
----
-
-To flag an issue, open a ticket on [Github](https://github.com/ScribeLabsAI/ScribeAuth/issues) and contact us on Intercom through the platform.
-
-
+Metadata-Version: 2.1
+Name: scribeauth
+Version: 1.0.5
+Summary: Library to authenticate to Scribe's platform
+Home-page: https://github.com/ScribeLabsAI/ScribeAuth
+Author: Ailin Venerus
+Author-email: ailin@scribelabs.ai
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Security
+Classifier: Typing :: Typed
+Requires-Python: >=3.10.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: boto3
+Requires-Dist: typing-extensions
+
+# Scribe Auth
+
+Most calls to Scribe's API require authentication and authorization. This library simplifies this process.
+
+You first need a Scribe account and a client ID. Both can be requested at support[atsign]scribelabs[dotsign]ai or through Intercom on https://platform.scribelabs.ai if you already have a Scribe account.
+
+This library interacts directly with our authentication provider [AWS Cognito](https://aws.amazon.com/cognito/) meaning that your username and password never transit through our servers.
+
+## Installation
+
+```bash
+pip install scribeauth
+```
+
+This library requires Python >= 3.10 that supports typing.
+
+## Methods
+
+### 1. Changing password
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth(client_id)
+access.change_password('username', 'password', 'new_password')
+```
+
+### 2. Recovering an account in case of forgotten password
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth(client_id)
+access.forgot_password('username', 'password', 'confirmation_code')
+```
+
+### 3. Get or generate tokens
+
+##### With username and password
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth(client_id)
+access.get_tokens(username='username', password='password')
+```
+
+##### With refresh token
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth(client_id)
+access.get_tokens(refresh_token='refresh_token')
+```
+
+### 4. Revoking a refresh token
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth(client_id)
+access.revoke_refresh_token('refresh_token')
+```
+
+### 5. Getting federated id
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth({'client_id': your_client_id, 'user_pool_id': your_user_pool_id, 'identity_pool_id': your_identity_pool_id})
+access.get_federated_id('your_id_token')
+```
+
+### 6. Getting federated credentials
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth({'client_id': your_client_id, 'user_pool_id': your_user_pool_id, 'identity_pool_id': your_identity_pool_id})
+access.get_federated_credentials('your_federated_id', 'your_id_token')
+```
+
+### 7. Getting signature for request
+
+```python
+from scribeauth import ScribeAuth
+access = ScribeAuth({'client_id': your_client_id, 'user_pool_id': your_user_pool_id, 'identity_pool_id': your_identity_pool_id})
+access.get_signature_for_request(request='your_request', credentials='your_federated_credentials')
+```
+
+## Flow
+
+- If you never have accessed your Scribe account, it probably still contains the temporary password we generated for you. You can change it directly on the [platform](https://platform.scribelabs.ai) or with the `change_password` method. You won't be able to access anything else until the temporary password has been changed.
+
+- Once the account is up and running, you can request new tokens with `get_tokens`. You will initially have to provide your username and password. The access and id tokens are valid for up to 30 minutes. The refresh token is valid for 30 days.
+
+- While you have a valid refresh token, you can request fresh access and id tokens with `get_tokens` but using the refresh token this time, so you're not sending your username and password over the wire anymore.
+
+- In case you suspect that your refresh token has been leaked, you can revoke it with `revoke_token`. This will also invalidate any access/id token that has been issued with it. In order to get a new one, you'll need to use your username and password again.
+
+- You can get your federated id by using `get_federated_id` and providing your id token. The federated id will allow you to use `get_federated_credentials` to get an access key id, secret key and session token.
+
+- Every API call to be made to Scribe's API Gateway needs to have a signature. You can get the signature for your request by using `get_signature_for_request`. Provide the request you'll be using and your credentials (use `get_federated_credentials` to get them).
+
+## Command line
+
+You can also use the package as follows for quick access to tokens:
+
+```bash
+python -m scribeauth --client_id clientid --username username --password password
+```
+
+---
+
+To flag an issue, open a ticket on [Github](https://github.com/ScribeLabsAI/ScribeAuth/issues) and contact us on Intercom through the platform.
```

