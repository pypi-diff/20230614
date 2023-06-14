# Comparing `tmp/algokit_utils-1.2.0b9-py3-none-any.whl.zip` & `tmp/algokit_utils-1.3.0b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 36613 bytes, number of entries: 16
--rw-r--r--  2.0 unx     4091 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
+Zip file size: 36703 bytes, number of entries: 16
+-rw-r--r--  2.0 unx     4159 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     4410 b- defN 80-Jan-01 00:00 algokit_utils/_ensure_funded.py
 -rw-r--r--  2.0 unx     2841 b- defN 80-Jan-01 00:00 algokit_utils/_simulate_315_compat.py
 -rw-r--r--  2.0 unx     3569 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7364 b- defN 80-Jan-01 00:00 algokit_utils/account.py
 -rw-r--r--  2.0 unx    56488 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
--rw-r--r--  2.0 unx    34168 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
+-rw-r--r--  2.0 unx    34650 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     2550 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
 -rw-r--r--  2.0 unx     6319 b- defN 80-Jan-01 00:00 algokit_utils/models.py
--rw-r--r--  2.0 unx     4857 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
+-rw-r--r--  2.0 unx     5267 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b9.dist-info/LICENSE
--rw-r--r--  2.0 unx     2072 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b9.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b9.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1357 b- defN 16-Jan-01 00:00 algokit_utils-1.2.0b9.dist-info/RECORD
-16 files, 138716 bytes uncompressed, 34371 bytes compressed:  75.2%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.3.0b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2072 b- defN 80-Jan-01 00:00 algokit_utils-1.3.0b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.3.0b1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1357 b- defN 16-Jan-01 00:00 algokit_utils-1.3.0b1.dist-info/RECORD
+16 files, 139676 bytes uncompressed, 34461 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.2.0b9.dist-info/LICENSE
+Filename: algokit_utils-1.3.0b1.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.2.0b9.dist-info/METADATA
+Filename: algokit_utils-1.3.0b1.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.2.0b9.dist-info/WHEEL
+Filename: algokit_utils-1.3.0b1.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.2.0b9.dist-info/RECORD
+Filename: algokit_utils-1.3.0b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/__init__.py

```diff
@@ -79,14 +79,16 @@
     get_algod_client,
     get_algonode_config,
     get_default_localnet_config,
     get_indexer_client,
     get_kmd_client_from_algod_client,
     get_purestake_config,
     is_localnet,
+    is_mainnet,
+    is_testnet,
 )
 
 __all__ = [
     "create_kmd_wallet_account",
     "get_account_from_mnemonic",
     "get_or_create_kmd_wallet_account",
     "get_localnet_default_account",
@@ -151,12 +153,14 @@
     "get_algod_client",
     "get_algonode_config",
     "get_default_localnet_config",
     "get_indexer_client",
     "get_kmd_client_from_algod_client",
     "get_purestake_config",
     "is_localnet",
+    "is_mainnet",
+    "is_testnet",
     "EnsureBalanceParameters",
     "TransferParameters",
     "ensure_funded",
     "transfer",
 ]
```

## algokit_utils/deploy.py

```diff
@@ -485,24 +485,27 @@
 
     Fail = 0
     """Fail the deployment"""
     UpdateApp = 1
     """Update the Application with the new approval and clear programs"""
     ReplaceApp = 2
     """Create a new Application and delete the old Application in a single transaction"""
-    # TODO: AppendApp
+    AppendApp = 3
+    """Create a new application"""
 
 
 class OnSchemaBreak(Enum):
     """Action to take if an Application's schema has breaking changes"""
 
     Fail = 0
     """Fail the deployment"""
     ReplaceApp = 2
     """Create a new Application and delete the old Application in a single transaction"""
+    AppendApp = 3
+    """Create a new Application"""
 
 
 class OperationPerformed(Enum):
     """Describes the actions taken during deployment"""
 
     Nothing = 0
     """An existing Application was found"""
@@ -653,14 +656,18 @@
         assert isinstance(self.existing_app_metadata_or_reference, AppMetaData)
         if self.on_schema_break == OnSchemaBreak.Fail:
             raise DeploymentFailedError(
                 "Schema break detected and on_schema_break=OnSchemaBreak.Fail, stopping deployment. "
                 "If you want to try deleting and recreating the app then "
                 "re-run with on_schema_break=OnSchemaBreak.ReplaceApp"
             )
+        if self.on_schema_break == OnSchemaBreak.AppendApp:
+            logger.info("Schema break detected and on_schema_break=AppendApp, will attempt to create new app")
+            return self._create_app()
+
         if self.existing_app_metadata_or_reference.deletable:
             logger.info(
                 "App is deletable and on_schema_break=ReplaceApp, will attempt to create new app and delete old app"
             )
         elif self.existing_app_metadata_or_reference.deletable is False:
             logger.warning(
                 "App is not deletable but on_schema_break=ReplaceApp, "
@@ -675,15 +682,18 @@
     def _deploy_update(self) -> DeployResponse:
         assert isinstance(self.existing_app_metadata_or_reference, AppMetaData)
         if self.on_update == OnUpdate.Fail:
             raise DeploymentFailedError(
                 "Update detected and on_update=Fail, stopping deployment. "
                 "If you want to try updating the app then re-run with on_update=UpdateApp"
             )
-        if self.existing_app_metadata_or_reference.updatable and self.on_update == OnUpdate.UpdateApp:
+        if self.on_update == OnUpdate.AppendApp:
+            logger.info("Update detected and on_update=AppendApp, will attempt to create new app")
+            return self._create_app()
+        elif self.existing_app_metadata_or_reference.updatable and self.on_update == OnUpdate.UpdateApp:
             logger.info("App is updatable and on_update=UpdateApp, will update app")
             return self._update_app()
         elif self.existing_app_metadata_or_reference.updatable and self.on_update == OnUpdate.ReplaceApp:
             logger.warning(
                 "App is updatable but on_update=ReplaceApp, will attempt to create new app and delete old app"
             )
             return self._create_and_delete_app()
```

## algokit_utils/network_clients.py

```diff
@@ -12,14 +12,16 @@
     "get_algod_client",
     "get_algonode_config",
     "get_default_localnet_config",
     "get_indexer_client",
     "get_kmd_client_from_algod_client",
     "get_purestake_config",
     "is_localnet",
+    "is_mainnet",
+    "is_testnet",
 ]
 
 _PURE_STAKE_HOST = "purestake.io"
 
 
 @dataclasses.dataclass
 class AlgoClientConfig:
@@ -78,14 +80,26 @@
 
 def is_localnet(client: AlgodClient) -> bool:
     """Returns True if client genesis is `devnet-v1` or `sandnet-v1`"""
     params = client.suggested_params()
     return params.gen in ["devnet-v1", "sandnet-v1", "dockernet-v1"]
 
 
+def is_mainnet(client: AlgodClient) -> bool:
+    """Returns True if client genesis is `mainnet-v1`"""
+    params = client.suggested_params()
+    return bool(params.gen == "mainnet-v1")
+
+
+def is_testnet(client: AlgodClient) -> bool:
+    """Returns True if client genesis is `testnet-v1`"""
+    params = client.suggested_params()
+    return bool(params.gen == "testnet-v1")
+
+
 def get_kmd_client_from_algod_client(client: AlgodClient) -> KMDClient:
     """Returns an {py:class}`algosdk.kmd.KMDClient` from supplied `client`
 
     Will use the same address as provided `client` but on port specified by `KMD_PORT` environment variable,
     or 4002 by default"""
     # We can only use Kmd on the LocalNet otherwise it's not exposed so this makes some assumptions
     # (e.g. same token and server as algod and port 4002 by default)
```

## Comparing `algokit_utils-1.2.0b9.dist-info/LICENSE` & `algokit_utils-1.3.0b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.2.0b9.dist-info/METADATA` & `algokit_utils-1.3.0b1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.2.0b9
+Version: 1.3.0b1
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_utils-1.2.0b9.dist-info/RECORD` & `algokit_utils-1.3.0b1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-algokit_utils/__init__.py,sha256=wuh-p9PubCj9Bj2tpxP3tQ5qZPs_nUHzB16BHi9Aq2c,4091
+algokit_utils/__init__.py,sha256=Ko-gEPeER-Ho8lRU_a6k5SsV3mTfZa6CP1I9dmZjQvk,4159
 algokit_utils/_ensure_funded.py,sha256=DjwGnCC_6USLQV5wIMJZRVQFlQ1uLrGDMxRF471atsQ,4410
 algokit_utils/_simulate_315_compat.py,sha256=9qCsNnKa1FXYfCccMFiE0mGEcZJiBuPmUy7ZRvvUSqU,2841
 algokit_utils/_transfer.py,sha256=K8TMoaFcZE74xZ1rhp1De0Ri4mg8vs8pu-iJLOa5WoE,3569
 algokit_utils/account.py,sha256=UIuOQZe28pQxjEP9TzhtYlOU20tUdzzS-nIIZM9Bp6Y,7364
 algokit_utils/application_client.py,sha256=k3eTyhY3zyfpajHffo1uJ2u1C0vlYPmdALl5jmgH1WM,56488
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
-algokit_utils/deploy.py,sha256=UmVlJ-0vo91EjPXRC1EjkFBh5frJ0R4nCnlyZABhcRg,34168
+algokit_utils/deploy.py,sha256=sY6u0T39DuF6oLpal0eJAc76EmjPWdoCPk2OSKGccnM,34650
 algokit_utils/logic_error.py,sha256=8O_4rJ1t57JEG81ucRNih2ojc1-EOm2fVxW6m-1ZXI8,2550
 algokit_utils/models.py,sha256=75tWWa3W-37Om3YgkcuKiuHAGzMkFIJ9U-eHO29RPi4,6319
-algokit_utils/network_clients.py,sha256=dq8yyTLKtyb9yG3tsXV-eZLF3iqMaFWs9kNWm1V4CdU,4857
+algokit_utils/network_clients.py,sha256=KmuSHG2kSdJfo9W4pIB_4RjnBL2yMQNGlF54lxXTnsQ,5267
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.2.0b9.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.2.0b9.dist-info/METADATA,sha256=P25jThT9yhEQKp6_dlmpaY7hUiLQrOrRgPzbyf9S9GA,2072
-algokit_utils-1.2.0b9.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-algokit_utils-1.2.0b9.dist-info/RECORD,,
+algokit_utils-1.3.0b1.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.3.0b1.dist-info/METADATA,sha256=75vQhThgjoQUr2xDl-t--FnVEl9bHz7kAs7LS4jVwns,2072
+algokit_utils-1.3.0b1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+algokit_utils-1.3.0b1.dist-info/RECORD,,
```

