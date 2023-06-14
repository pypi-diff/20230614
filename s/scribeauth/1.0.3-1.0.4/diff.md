# Comparing `tmp/scribeauth-1.0.3-py3-none-any.whl.zip` & `tmp/scribeauth-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6738 bytes, number of entries: 9
+Zip file size: 7623 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat       66 b- defN 23-May-17 09:44 scribeauth/__init__.py
--rw-rw-rw-  2.0 fat      521 b- defN 22-Jul-27 09:39 scribeauth/__main__.py
--rw-rw-rw-  2.0 fat     8718 b- defN 23-May-17 16:30 scribeauth/scribeauth.py
+-rw-rw-rw-  2.0 fat      521 b- defN 23-Jun-12 14:20 scribeauth/__main__.py
+-rw-rw-rw-  2.0 fat    13230 b- defN 23-Jun-14 09:44 scribeauth/scribeauth.py
 -rw-rw-rw-  2.0 fat     1351 b- defN 23-May-15 17:21 scribeauth/scribeauthfederation.py
--rw-rw-rw-  2.0 fat     1097 b- defN 23-May-22 13:26 scribeauth-1.0.3.dist-info/LICENSE.md
--rw-rw-rw-  2.0 fat     3719 b- defN 23-May-22 13:26 scribeauth-1.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-22 13:26 scribeauth-1.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-May-22 13:26 scribeauth-1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      731 b- defN 23-May-22 13:26 scribeauth-1.0.3.dist-info/RECORD
-9 files, 16306 bytes uncompressed, 5474 bytes compressed:  66.4%
+-rw-rw-rw-  2.0 fat     1097 b- defN 23-Jun-14 09:45 scribeauth-1.0.4.dist-info/LICENSE.md
+-rw-rw-rw-  2.0 fat     4400 b- defN 23-Jun-14 09:45 scribeauth-1.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-14 09:45 scribeauth-1.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-14 09:45 scribeauth-1.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      732 b- defN 23-Jun-14 09:45 scribeauth-1.0.4.dist-info/RECORD
+9 files, 21500 bytes uncompressed, 6359 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: scribeauth/scribeauth.py
 Comment: 
 
 Filename: scribeauth/scribeauthfederation.py
 Comment: 
 
-Filename: scribeauth-1.0.3.dist-info/LICENSE.md
+Filename: scribeauth-1.0.4.dist-info/LICENSE.md
 Comment: 
 
-Filename: scribeauth-1.0.3.dist-info/METADATA
+Filename: scribeauth-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: scribeauth-1.0.3.dist-info/WHEEL
+Filename: scribeauth-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: scribeauth-1.0.3.dist-info/top_level.txt
+Filename: scribeauth-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: scribeauth-1.0.3.dist-info/RECORD
+Filename: scribeauth-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## scribeauth/scribeauth.py

```diff
@@ -1,8 +1,8 @@
-from typing import List, TypedDict
+from typing import List, TypedDict, Union
 from typing_extensions import Unpack
 import boto3
 import botocore
 from botocore.config import Config
 
 
 class Tokens(TypedDict):
@@ -15,14 +15,25 @@
     refresh_token: str
 
 
 class UsernamePassword(TypedDict):
     username: str
     password: str
 
+class Credentials(TypedDict):
+    AccessKeyId: str
+    SecretKey: str
+    SessionToken: str
+    Expiration: str
+
+class PoolConfiguration(TypedDict):
+    client_id: str
+    user_pool_id: str
+    identity_pool_id: str
+
 class UnauthorizedException(Exception):
     """
     Exception raised when a user cannot perform an action.
 
     Possible reasons:
     - Username and/or Password are incorrect.
     - Refresh_token is incorrect.
@@ -35,28 +46,61 @@
 
     Actions that could raise this exception:
     - Changing a Password.
     - Revoke Refresh_token.
     """
     pass
 
+class MissingIdException(Exception):
+    pass
+
+class UnknownException(Exception):
+    pass
+
+def is_complete_credentials(cred: Credentials) -> bool:
+    return 'AccessKeyId' in cred and 'SecretKey' in cred and 'SessionToken' in cred
+
 class ScribeAuth:
-    def __init__(self, client_id: str):
+    def __init__(self, param: Union[Unpack[PoolConfiguration], str]):
         """Construct an authorisation client.
 
         Args
         ----
+        Union[Unpack[PoolConfiguration], str]
+        A parameter that can either be an instance of PoolConfiguration or a string.
+        
+        ---
+
+        PoolConfiguration:
+        ---
+        client_id -- The client ID of the application provided by Scribe.
+        
+        user_pool_id -- The user pool ID provided by Scribe.
+        
+        identity_pool_id -- The identity pool ID provided by Scribe.
+
+        ---
+
+        str:
+        ---
         client_id -- The client ID of the application provided by Scribe.
         """
         config = Config(signature_version=botocore.UNSIGNED)
         self.client_unsigned = boto3.client(
             'cognito-idp', config=config, region_name='eu-west-2')
         self.client_signed = boto3.client(
             'cognito-idp', region_name='eu-west-2')
-        self.client_id = client_id
+        self.fed_client = boto3.client('cognito-identity', region_name='eu-west-2')
+        if isinstance(param, str):
+            self.client_id = param
+        else:
+            self.client_id = param.get('client_id')
+            self.user_pool_id = param.get('user_pool_id')
+            self.identity_pool_id = param.get('identity_pool_id')
+
 
     def change_password(self, username: str, password: str, new_password: str) -> bool: # pragma: no cover
         """Creates a new password for a user.
 
         Args
         ----
         username -- Username (usually an email address).
@@ -67,37 +111,45 @@
         
         Returns
         -------
         bool
         """
         try:
             response_initiate = self.__initiate_auth(username, password)
-        except Exception:
-            raise UnauthorizedException("Username and/or Password are incorrect")
-        challenge_name = response_initiate.get('ChallengeName')
-        if challenge_name == None:
-            try:
-                auth_result = response_initiate.get('AuthenticationResult')
-                access_token = auth_result.get('AccessToken')
-                self.__change_password_cognito(
-                    password, new_password, access_token)
-                return True
-            except Exception:
-                raise TooManyRequestsException("Password has been changed too many times. Try again later")
-        else:
-            session = response_initiate.get("Session")
-            challenge_parameters = response_initiate.get("ChallengeParameters")
-            user_id_SRP = challenge_parameters.get("USER_ID_FOR_SRP")
-            required_attributes = challenge_parameters.get("requiredAttributes")
-            try:
-                self.__respond_to_auth_challenge(
-                    username, new_password, session, user_id_SRP, required_attributes)
-                return True
-            except Exception:
-                raise Exception("InternalServerError: try again later")
+            challenge_name = response_initiate.get('ChallengeName')
+            if challenge_name == None:
+                try:
+                    auth_result = response_initiate.get('AuthenticationResult')
+                    access_token = auth_result.get('AccessToken')
+                    self.__change_password_cognito(
+                        password, new_password, access_token)
+                    return True
+                except Exception as err:
+                    raise err
+            else:
+                if not self.client_id:
+                    raise MissingIdException("Missing client ID")
+                session = response_initiate.get("Session")
+                challenge_parameters = response_initiate.get("ChallengeParameters")
+                user_id_SRP = challenge_parameters.get("USER_ID_FOR_SRP")
+                required_attributes = challenge_parameters.get("requiredAttributes")
+                try:
+                    self.__respond_to_auth_challenge(
+                        username, new_password, session, user_id_SRP, required_attributes)
+                    return True
+                except Exception:
+                    raise Exception("InternalServerError: try again later")
+        except MissingIdException as err:
+            raise err
+        except TooManyRequestsException:
+            raise TooManyRequestsException("Too many requests. Try again later")
+        except Exception as err:
+            if err.response['Error']['Code'] == 'NotAuthorizedException':
+                raise UnauthorizedException("Username and/or Password are incorrect.")
+            raise err
 
     def forgot_password(self, username: str, password: str, confirmation_code: str) -> bool: # pragma: no cover
         """Allows a user to enter a confirmation code sent to their email to reset a forgotten password.
 
         Args
         ----
         username -- Username (usually an email address).
@@ -114,16 +166,19 @@
             self.client_signed.confirm_forgot_password(
                 ClientId=self.client_id,
                 Username=username,
                 ConfirmationCode=confirmation_code,
                 Password=password
             )
             return True
-        except Exception:
-            raise UnauthorizedException("Username, Password and/or Confirmation_code are incorrect. Could not reset password")
+        except Exception as err:
+            if err.response['Error']['Code'] == 'NotAuthorizedException':
+                raise UnauthorizedException("Username, Password and/or Confirmation_code are incorrect. Could not reset password")
+            raise err
+                
 
     def get_tokens(self, **param: Unpack[UsernamePassword] | Unpack[RefreshToken]) -> Tokens:
         """A user gets their tokens (refresh_token, access_token and id_token).
 
         Args
         ----
         username -- Username (usually an email address).
@@ -134,44 +189,21 @@
 
         refresh_token -- Refresh token to use.
         
         Returns
         -------
         Tokens -- Dictionary {"refresh_token": "str", "access_token": "str", "id_token": "str"}
         """
-        auth_result = 'AuthenticationResult'
         refresh_token = param.get('refresh_token')
+        username = param.get('username')
+        password = param.get('password')
         if refresh_token == None:
-            username = param.get('username')
-            password = param.get('password')
-            if username != None and password != None:
-                try:
-                    response = self.__initiate_auth(username, password)
-                    result = response.get(auth_result)
-                    return {
-                        'refresh_token': result.get('RefreshToken'),
-                        'access_token': result.get('AccessToken'),
-                        'id_token': result.get('IdToken')
-                    }
-                except:
-                    raise UnauthorizedException("Username and/or Password are incorrect. Could not get tokens")
-            else:
-                raise UnauthorizedException("Username and/or Password are missing. Could not get tokens")
+            return self.__get_tokens_with_pair(username, password)
         else:
-            try:
-                response = self.__get_tokens_from_refresh(refresh_token)
-                result = response.get(auth_result)
-                return {
-                    'refresh_token': refresh_token,
-                    'access_token': result.get('AccessToken'),
-                    'id_token': result.get('IdToken')
-                }
-            except:
-                raise UnauthorizedException("Refresh_token is incorrect. Could not get tokens")
-
+            return self.__get_tokens_with_refresh(refresh_token)
 
     def revoke_refresh_token(self, refresh_token: str) -> bool:
         """Revokes all of the access tokens generated by the specified refresh token.
         After the token is revoked, the user cannot use the revoked token.
 
         Args
         ----
@@ -186,14 +218,109 @@
         if(status_code == 200):
             return True
         if(status_code == 400): # pragma: no cover
             raise TooManyRequestsException("Too many requests. Try again later")
         else: # pragma: no cover
             raise Exception("InternalServerError: Try again later")
 
+    def get_federated_id(self, id_token: str) -> str:
+        """A user gets their federated id.
+
+        Args
+        ----
+        id_token -- Id token to use.
+
+        Returns
+        -------
+        str
+        """
+        if not self.user_pool_id:
+            raise MissingIdException('Missing user pool ID')
+        if not self.identity_pool_id:
+            raise MissingIdException('Missing federated pool ID')
+        try:
+            response = self.fed_client.get_id(
+                IdentityPoolId=self.identity_pool_id,
+                Logins={
+                    f'cognito-idp.eu-west-2.amazonaws.com/{self.user_pool_id}': id_token
+                }
+            )
+            if not response.get('IdentityId'):
+                raise UnknownException('Could not retrieve federated id')
+            return response.get('IdentityId')
+        except Exception as err:
+            if err.response['Error']['Code'] == 'NotAuthorizedException':
+                raise UnauthorizedException('Could not retrieve federated id')
+            if err.response['Error']['Code'] == 'TooManyRequestsException':
+                raise TooManyRequestsException('Too many requests. Try again later')
+            raise err
+    
+
+    def get_federated_credentials(self, id: str, id_token:str) -> Credentials:
+        """A user gets their federated credentials (AccessKeyId, SecretKey and SessionToken).
+
+        Args
+        ----
+        id -- Federated id.
+
+        id_token -- Id token to use.
+
+        Returns
+        -------
+        Credentials -- Dictionary {"AccessKeyId": "str", "SecretKey": "str", "SessionToken": "str", "Expiration": "str"}
+        """
+        if not self.user_pool_id:
+            raise MissingIdException('Missing user pool ID')
+        try:
+            response = self.fed_client.get_credentials_for_identity(
+                IdentityId=id,
+                Logins={
+                    f'cognito-idp.eu-west-2.amazonaws.com/{self.user_pool_id}': id_token
+                }
+            )
+            if not is_complete_credentials(response['Credentials']):
+                raise UnknownException('Could not retrieve federated credentials')
+            return response['Credentials']
+        except Exception as err:
+            if err.response['Error']['Code'] == 'NotAuthorizedException':
+                raise UnauthorizedException('Could not retrieve federated credentials')
+            if err.response['Error']['Code'] == 'TooManyRequestsException':
+                raise TooManyRequestsException('Too many requests. Try again later')
+            raise err
+
+    def __get_tokens_with_pair(self, username: str, password: str):
+        auth_result = 'AuthenticationResult'
+        if username != None and password != None:
+            try:
+                response = self.__initiate_auth(username, password)
+                result = response.get(auth_result)
+                return {
+                    'refresh_token': result.get('RefreshToken'),
+                    'access_token': result.get('AccessToken'),
+                    'id_token': result.get('IdToken')
+                }
+            except:
+                raise UnauthorizedException("Username and/or Password are incorrect. Could not get tokens")
+        else:
+            raise UnauthorizedException("Username and/or Password are missing. Could not get tokens")
+       
+    def __get_tokens_with_refresh(self, refresh_token: str):
+        try:
+            auth_result = 'AuthenticationResult'
+            response = self.client_signed.initiate_auth(ClientId=self.client_id, AuthFlow='REFRESH_TOKEN', AuthParameters={'REFRESH_TOKEN': refresh_token})
+            result = response.get(auth_result)
+            return {
+                'refresh_token': refresh_token,
+                'access_token': result.get('AccessToken'),
+                'id_token': result.get('IdToken')
+            }
+        except:
+            raise UnauthorizedException("Refresh_token is incorrect. Could not get tokens")
+
+
     def __initiate_auth(self, username: str, password: str):
         response = self.client_signed.initiate_auth(
             ClientId=self.client_id,
             AuthFlow='USER_PASSWORD_AUTH',
             AuthParameters={
                 'USERNAME': username,
                 'PASSWORD': password})
@@ -209,21 +336,14 @@
                 "requiredAttributes": required_attributes,
                 "USERNAME": username,
                 "NEW_PASSWORD": new_password
             },
         )
         return response
 
-    def __get_tokens_from_refresh(self, refresh_token: str):
-        response = self.client_signed.initiate_auth(
-            ClientId=self.client_id,
-            AuthFlow='REFRESH_TOKEN',
-            AuthParameters={'REFRESH_TOKEN': refresh_token})
-        return response
-
     def __change_password_cognito(self, password: str, new_password: str, access_token: str): # pragma: no cover
         response = self.client_signed.change_password(
             PreviousPassword=password,
             ProposedPassword=new_password,
             AccessToken=access_token)
         return response
```

## Comparing `scribeauth-1.0.3.dist-info/LICENSE.md` & `scribeauth-1.0.4.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `scribeauth-1.0.3.dist-info/METADATA` & `scribeauth-1.0.4.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,124 @@
-Metadata-Version: 2.1
-Name: scribeauth
-Version: 1.0.3
-Summary: Library to authenticate to Scribe's platform
-Home-page: https://github.com/ScribeLabsAI/ScribeAuth
-Author: Ailin Venerus
-Author-email: ailin@scribelabs.ai
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
-This library requires Python >= 3.10 that supports typings.
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
+Metadata-Version: 2.1
+Name: scribeauth
+Version: 1.0.4
+Summary: Library to authenticate to Scribe's platform
+Home-page: https://github.com/ScribeLabsAI/ScribeAuth
+Author: Ailin Venerus
+Author-email: ailin@scribelabs.ai
+License: UNKNOWN
+Platform: UNKNOWN
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
+
+
```

