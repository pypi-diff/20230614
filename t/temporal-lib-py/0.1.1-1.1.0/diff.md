# Comparing `tmp/temporal_lib_py-0.1.1-py3-none-any.whl.zip` & `tmp/temporal_lib_py-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18751 bytes, number of entries: 12
+Zip file size: 19412 bytes, number of entries: 12
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 temporallib/__init__.py
--rw-r--r--  2.0 unx       75 b- defN 80-Jan-01 00:00 temporallib/auth/__init__.py
--rw-r--r--  2.0 unx     2508 b- defN 80-Jan-01 00:00 temporallib/auth/auth.py
--rw-r--r--  2.0 unx       66 b- defN 80-Jan-01 00:00 temporallib/connection/__init__.py
--rw-r--r--  2.0 unx     3841 b- defN 80-Jan-01 00:00 temporallib/connection/connection.py
+-rw-r--r--  2.0 unx      115 b- defN 80-Jan-01 00:00 temporallib/auth/__init__.py
+-rw-r--r--  2.0 unx     3893 b- defN 80-Jan-01 00:00 temporallib/auth/auth.py
+-rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 temporallib/client/__init__.py
+-rw-r--r--  2.0 unx     3875 b- defN 80-Jan-01 00:00 temporallib/client/client.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 temporallib/encryption/__init__.py
 -rw-r--r--  2.0 unx      853 b- defN 80-Jan-01 00:00 temporallib/encryption/crypt.py
 -rw-r--r--  2.0 unx     2029 b- defN 80-Jan-01 00:00 temporallib/encryption/data_converter.py
--rw-r--r--  2.0 unx    34519 b- defN 80-Jan-01 00:00 temporal_lib_py-0.1.1.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 temporal_lib_py-0.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2629 b- defN 16-Jan-01 00:00 temporal_lib_py-0.1.1.dist-info/METADATA
-?rw-r--r--  2.0 unx     1024 b- defN 16-Jan-01 00:00 temporal_lib_py-0.1.1.dist-info/RECORD
-12 files, 47823 bytes uncompressed, 17009 bytes compressed:  64.4%
+-rw-r--r--  2.0 unx    34519 b- defN 80-Jan-01 00:00 temporal_lib_py-1.1.0.dist-info/LICENSE
+?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 temporal_lib_py-1.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     4172 b- defN 16-Jan-01 00:00 temporal_lib_py-1.1.0.dist-info/METADATA
+?rw-r--r--  2.0 unx     1013 b- defN 16-Jan-01 00:00 temporal_lib_py-1.1.0.dist-info/RECORD
+12 files, 50802 bytes uncompressed, 17694 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -3,35 +3,35 @@
 
 Filename: temporallib/auth/__init__.py
 Comment: 
 
 Filename: temporallib/auth/auth.py
 Comment: 
 
-Filename: temporallib/connection/__init__.py
+Filename: temporallib/client/__init__.py
 Comment: 
 
-Filename: temporallib/connection/connection.py
+Filename: temporallib/client/client.py
 Comment: 
 
 Filename: temporallib/encryption/__init__.py
 Comment: 
 
 Filename: temporallib/encryption/crypt.py
 Comment: 
 
 Filename: temporallib/encryption/data_converter.py
 Comment: 
 
-Filename: temporal_lib_py-0.1.1.dist-info/LICENSE
+Filename: temporal_lib_py-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: temporal_lib_py-0.1.1.dist-info/WHEEL
+Filename: temporal_lib_py-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: temporal_lib_py-0.1.1.dist-info/METADATA
+Filename: temporal_lib_py-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: temporal_lib_py-0.1.1.dist-info/RECORD
+Filename: temporal_lib_py-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## temporallib/auth/__init__.py

```diff
@@ -1 +1 @@
-from temporallib.auth.auth import AuthHeaderProvider, AuthOptions, KeyPair
+from temporallib.auth.auth import AuthHeaderProvider, AuthOptions, MacaroonAuthOptions, GoogleAuthOptions, KeyPair
```

## temporallib/auth/auth.py

```diff
@@ -6,68 +6,104 @@
 from typing import Mapping
 
 import requests
 from macaroonbakery import bakery, httpbakery
 from macaroonbakery.bakery import Macaroon, b64decode, macaroon_to_dict
 from macaroonbakery.httpbakery.agent import Agent, AgentInteractor, AuthInfo
 
+from google.oauth2 import service_account
+from typing import Union
+from dataclasses import asdict
 
 @dataclass
-class AuthOptions:
+class MacaroonAuthOptions:
     """
     Defines the parameters for authenticating with Candid.
     """
-
     macaroon_url: str
     username: str
     keys: KeyPair
-
+    
+@dataclass
+class GoogleAuthOptions:
+    """
+    Defines the parameters for authenticating with Google IAM.
+    """
+    type: str
+    project_id: str
+    private_key_id: str
+    private_key: str
+    client_email: str
+    client_id: str
+    auth_uri: str
+    token_uri: str
+    auth_provider_x509_cert_url: str
+    client_x509_cert_url: str
 
 @dataclass
 class KeyPair:
     """
     A structure for storing agent the key pair.
     """
-
     private: str
     public: str = None
 
+@dataclass
+class AuthOptions:
+    provider: str
+    config: Union[MacaroonAuthOptions, GoogleAuthOptions]
 
 class AuthHeaderProvider:
     """
     A class to provide the authorization headers to the Temporal client.
     """
 
-    def __init__(self, cfg: AuthOptions):
-        self.cfg = cfg
+    def __init__(self, auth: AuthOptions):
+        self.auth = auth
+
+    def get_headers(self) -> Mapping[str,str]:
+        if not self.auth.provider:
+            raise TemporalError("auth provider must be specified")
+
+        if self.auth.provider == "candid":
+            return self.get_macaroon_headers()
+        if self.auth.provider == "google":
+            return self.get_google_iam_headers()
+        raise TemporalError("auth provider not supported. please specify candid or google.")
+
+    def get_google_iam_headers(self) -> Mapping[str, str]:
+        auth_dict = asdict(self.auth.config)
+        credentials = service_account.Credentials.from_service_account_info(auth_dict, scopes=['email', 'profile', 'openid', 'https://www.googleapis.com/auth/admin.directory.group.readonly'])
+
+        return {"authorization": f"Bearer {credentials.token}"}
 
-    def get_headers(self) -> Mapping[str, str]:
+    def get_macaroon_headers(self) -> Mapping[str, str]:
         """
         Retrieves the macaroon from Temporal server, discharges it and returns the according header.
         :return: A header entry for the authorization field
         """
         # get the macaroon from temporal server
-        resp = requests.get(self.cfg.macaroon_url)
+        resp = requests.get(self.auth.config.macaroon_url)
         if resp.status_code != 200:
             raise TemporalError(
-                f"error reaching the macaroon server ({self.cfg.macaroon_url})"
+                f"error reaching the macaroon server ({self.auth.config.macaroon_url})"
                 f" response code - {resp.status_code}"
             )
 
         # decode and extract candid url
         mc_serialized = b64decode(resp.text)
         macaroon = Macaroon.deserialize_json(mc_serialized)
         if len(macaroon.macaroon.caveats) == 0:
             raise TemporalError(f"retrieved macaroon is missing caveats")
         auth_url = macaroon.macaroon.caveats[0].location
 
         # set up bakery agent and connection
         auth_info = AuthInfo(
-            key=bakery.PrivateKey.deserialize(self.cfg.keys.private),
-            agents=[Agent(url=auth_url, username=self.cfg.username)],
+            key=bakery.PrivateKey.deserialize(self.auth.config.keys.private),
+            agents=[Agent(url=auth_url, username=self.auth.config.username)],
         )
         client = httpbakery.Client(interaction_methods=[AgentInteractor(auth_info)])
 
         # discharge macaroon
         ms = bakery.discharge_all(macaroon, client.acquire_discharge, client.key)
 
         # convert it to byte and encode
```

## Comparing `temporallib/connection/connection.py` & `temporallib/client/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 from dataclasses import dataclass
 from typing import Callable, Iterable, Mapping, Optional, Union
 
 from temporalio.client import Client as TemporalClient
 from temporalio.client import Interceptor, OutboundInterceptor
 from temporalio.common import QueryRejectCondition
 from temporalio.converter import DataConverter, default
-from temporalio.workflow_service import RetryConfig, TLSConfig
+from temporalio.service import TLSConfig, RetryConfig
 
-from temporallib.auth import AuthHeaderProvider, AuthOptions
+from temporallib.auth import AuthHeaderProvider, AuthOptions, MacaroonAuthOptions, GoogleAuthOptions
 from temporallib.encryption import EncryptionOptions, EncryptionPayloadCodec
+from typing import Union
 
 
 @dataclass
 class Options:
     """
     Defines the options to pass to the connect method in order to add authentication and parameter encryption
     """
@@ -24,15 +25,15 @@
     queue: str
     namespace: str
     encryption: EncryptionOptions = None
     tls_root_cas: str = None
     auth: AuthOptions = None
 
 
-class Connection:
+class Client:
     """
     A class which wraps the :class:`temporalio.client.Client` class
     """
 
     @staticmethod
     async def connect(
         client_opt: Options,
@@ -40,42 +41,42 @@
         data_converter: DataConverter = default(),
         interceptors: Iterable[
             Union[Interceptor, Callable[[OutboundInterceptor], OutboundInterceptor]]
         ] = None,
         default_workflow_query_reject_condition: Optional[QueryRejectCondition] = None,
         tls: Union[bool, TLSConfig] = False,
         retry_config: Optional[RetryConfig] = None,
-        static_headers: Mapping[str, str] = None,
+        rpc_metadata: Mapping[str, str] = None,
         identity: Optional[str] = None,
     ) -> TemporalClient:
         """
         A method which wraps the temporal :func:`temporalio.client.Client.connect` method by adding
         authorization headers and encrypting payloads.
         :param client_opt: the additional options for authorization and encryption
         :param data_converter: pass through to `Client.connect` if encryption not enabled in client_opt
         :param interceptors: pass through parameter to `Client.connect()`
         :param default_workflow_query_reject_condition: pass through parameter to `Client.connect()`
         :param tls: pass through parameter to `Client.connect()` if tls certificate not specified in client_opt
         :param retry_config: pass through parameter to `Client.connect()`
-        :param static_headers: pass through parameter to `Client.connect()` if authentication not enabled in client_opt
+        :param rpc_metadata: pass through parameter to `Client.connect()` if authentication not enabled in client_opt
         :param identity: pass through parameter to `Client.connect()`
         :return: temporal client used to send or retrieve tasks
         """
         if interceptors is None:
             interceptors = []
 
-        if static_headers is None:
-            static_headers = {}
+        if rpc_metadata is None:
+            rpc_metadata = {}
 
         namespace = client_opt.namespace or "default"
 
         if client_opt.auth:
             auth_header_provider = AuthHeaderProvider(client_opt.auth)
-            static_headers = dict(static_headers)
-            static_headers.update(auth_header_provider.get_headers())
+            rpc_metadata = dict(rpc_metadata)
+            rpc_metadata.update(auth_header_provider.get_headers())
 
         if client_opt.encryption:
             encryption_codec = EncryptionPayloadCodec(client_opt.encryption.key)
             data_converter = dataclasses.replace(
                 data_converter, payload_codec=encryption_codec
             )
 
@@ -88,10 +89,10 @@
             client_opt.host,
             namespace=namespace,
             data_converter=data_converter,
             interceptors=interceptors,
             default_workflow_query_reject_condition=default_workflow_query_reject_condition,
             tls=tls,
             retry_config=retry_config,
-            static_headers=static_headers,
+            rpc_metadata=rpc_metadata,
             identity=identity,
         )
```

## Comparing `temporal_lib_py-0.1.1.dist-info/LICENSE` & `temporal_lib_py-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

