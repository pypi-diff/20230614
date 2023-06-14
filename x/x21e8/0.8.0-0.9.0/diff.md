# Comparing `tmp/x21e8-0.8.0.tar.gz` & `tmp/x21e8-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x21e8-0.8.0.tar", max compression
+gzip compressed data, was "x21e8-0.9.0.tar", max compression
```

## Comparing `x21e8-0.8.0.tar` & `x21e8-0.9.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     5126 2023-06-05 07:40:44.116080 x21e8-0.8.0/README.md
--rw-r--r--   0        0        0      794 2023-06-05 07:40:44.124084 x21e8-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/application/__init__.py
--rw-r--r--   0        0        0     6153 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/application/liquid.py
--rw-r--r--   0        0        0        1 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/application/notarize.py
--rw-r--r--   0        0        0     2409 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/application/planetmint.py
--rw-r--r--   0        0        0      398 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/application/rddl.py
--rw-r--r--   0        0        0     1743 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/application/token.py
--rw-r--r--   0        0        0      765 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/config.py
--rw-r--r--   0        0        0     1001 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/main.py
--rw-r--r--   0        0        0        0 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/models/__init__.py
--rw-r--r--   0        0        0      182 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/models/issuing_request.py
--rw-r--r--   0        0        0      188 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/models/nft_asset.py
--rw-r--r--   0        0        0      354 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/models/token_related_accounts.py
--rw-r--r--   0        0        0      494 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/models/transfer.py
--rw-r--r--   0        0        0        0 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/network/__init__.py
--rw-r--r--   0        0        0     2220 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/network/liquid/__init__.py
--rwxr-xr-x   0        0        0    97346 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/network/liquid/util.py
--rw-r--r--   0        0        0     1693 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/routers/assets.py
--rw-r--r--   0        0        0      375 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/routers/config.py
--rw-r--r--   0        0        0     1096 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/routers/data.py
--rw-r--r--   0        0        0     4145 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/routers/machine.py
--rw-r--r--   0        0        0      925 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/routers/seed.py
--rw-r--r--   0        0        0      630 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/routers/utils.py
--rw-r--r--   0        0        0      997 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/routers/wallet.py
--rw-r--r--   0        0        0        0 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/utils/__init__.py
--rw-r--r--   0        0        0      256 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/utils/cointype.py
--rw-r--r--   0        0        0     1035 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/utils/encryption.py
--rw-r--r--   0        0        0     2237 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/utils/storage.py
--rw-r--r--   0        0        0        0 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/wallet/__init__.py
--rw-r--r--   0        0        0      628 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/wallet/base_wallet.py
--rw-r--r--   0        0        0        0 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/wallet/planetmint/__init__.py
--rw-r--r--   0        0        0     2771 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/wallet/planetmint/keymanagement.py
--rw-r--r--   0        0        0     3231 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/wallet/planetmint/keystore.py
--rw-r--r--   0        0        0      720 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/wallet/seed.py
--rw-r--r--   0        0        0     4781 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/wallet/sw_wallet.py
--rw-r--r--   0        0        0     6174 1970-01-01 00:00:00.000000 x21e8-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     5223 2023-06-14 08:34:56.845137 x21e8-0.9.0/README.md
+-rw-r--r--   0        0        0      823 2023-06-14 08:34:56.849137 x21e8-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/application/__init__.py
+-rw-r--r--   0        0        0     6153 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/application/liquid.py
+-rw-r--r--   0        0        0        1 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/application/notarize.py
+-rw-r--r--   0        0        0     2391 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/application/planetmint.py
+-rw-r--r--   0        0        0      398 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/application/rddl.py
+-rw-r--r--   0        0        0     1743 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/application/token.py
+-rw-r--r--   0        0        0      837 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/config.py
+-rw-r--r--   0        0        0     1001 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/main.py
+-rw-r--r--   0        0        0        0 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/models/__init__.py
+-rw-r--r--   0        0        0      182 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/models/issuing_request.py
+-rw-r--r--   0        0        0      188 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/models/nft_asset.py
+-rw-r--r--   0        0        0      354 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/models/token_related_accounts.py
+-rw-r--r--   0        0        0      494 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/models/transfer.py
+-rw-r--r--   0        0        0        0 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/network/__init__.py
+-rw-r--r--   0        0        0     2220 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/network/liquid/__init__.py
+-rwxr-xr-x   0        0        0    97346 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/network/liquid/util.py
+-rw-r--r--   0        0        0     1693 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/routers/assets.py
+-rw-r--r--   0        0        0      375 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/routers/config.py
+-rw-r--r--   0        0        0     1096 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/routers/data.py
+-rw-r--r--   0        0        0     4145 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/routers/machine.py
+-rw-r--r--   0        0        0      925 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/routers/seed.py
+-rw-r--r--   0        0        0      630 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/routers/utils.py
+-rw-r--r--   0        0        0      997 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/routers/wallet.py
+-rw-r--r--   0        0        0        0 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/utils/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/utils/cointype.py
+-rw-r--r--   0        0        0     1123 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/utils/eddsa_auth.py
+-rw-r--r--   0        0        0     1035 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/utils/encryption.py
+-rw-r--r--   0        0        0     2354 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/utils/storage.py
+-rw-r--r--   0        0        0        0 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/wallet/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/wallet/base_wallet.py
+-rw-r--r--   0        0        0        0 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/wallet/planetmint/__init__.py
+-rw-r--r--   0        0        0     2771 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/wallet/planetmint/keymanagement.py
+-rw-r--r--   0        0        0     3231 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/wallet/planetmint/keystore.py
+-rw-r--r--   0        0        0      720 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/wallet/seed.py
+-rw-r--r--   0        0        0     4862 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/wallet/sw_wallet.py
+-rw-r--r--   0        0        0     6322 1970-01-01 00:00:00.000000 x21e8-0.9.0/PKG-INFO
```

### Comparing `x21e8-0.8.0/README.md` & `x21e8-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,24 +41,26 @@
     * RPC URL
     * RPC port
     * RPC user
     * RPC password
 * web3storage token to store data
 * RDDL asset registration endpoint
 * RDDL CID resolver
+* RDDL Authentication service to be able to authenticate with EdDSA to RDDL services
 
 The configuration is set via environment variables such as
 * LQD_RPC_PORT
 * LQD_RPC_USER
 * LQD_RPC_PASSWORD
 * LQD_RPC_HOST
 * PLNTMNT_ENDPOINT
 * WEB3STORAGE_TOKEN
 * RDDL_ASSET_REG_ENDPOINT
 * CID_RESOLVER
+* RDDL_AUTH
 
 Alternatively, the variables can be defined within the ```.env``` file of the project. A example ```env.example``` file can be adjusted and copied to ```.env```.
 
 ## Service Execution
 ```bash
 uvicorn --log-level debug --reload x21e8.main:app
 ```
```

### Comparing `x21e8-0.8.0/pyproject.toml` & `x21e8-0.9.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "x21e8"
-version = "0.8.0"
+version = "0.9.0"
 description = "x21e8 service to manage RDDL network identities on TrustAnchors and workflows."
 authors = ["Firat Berk Cakar <firat@riddleandcode.com>", "Jürgen Eckel <juergen@riddleandcode.com"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 TrezorCryptoTestRc = "*" 
@@ -16,15 +16,16 @@
 mypy = "^0.982"
 python-decouple = "^3.6"
 pysha3 = "^1.0.2"
 python-rapidjson = ">1.0.0"
 python-rapidjson-schema = "0.1.1"
 multiformats = "^0.2.1"
 uvicorn = "^0.19.0"
-planetmint-driver = "0.18.2"
+planetmint-driver = "^0.18.2"
+typing-extensions = "4.5.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `x21e8-0.8.0/x21e8/application/liquid.py` & `x21e8-0.9.0/x21e8/application/liquid.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.8.0/x21e8/application/planetmint.py` & `x21e8-0.9.0/x21e8/application/planetmint.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import json
 import ast
 
 
 def create_cid_based_asset(cid: str, wallet: BaseWallet):
     plntmnt = Planetmint(PLNTMNT_ENDPOINT)
     pubkey = wallet.get_planetmint_pubkey()
-    print(pubkey)
     tx = plntmnt.transactions.prepare(
         operation="CREATE",
         signers=[base58.b58encode(pubkey).decode()],
         assets=[{"data": cid}],
     )
 
     signed_tx = fulfill_with_signing_delegation(tx, wallet.planetmint_sign_digest)
```

### Comparing `x21e8-0.8.0/x21e8/application/token.py` & `x21e8-0.9.0/x21e8/application/token.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.8.0/x21e8/config.py` & `x21e8-0.9.0/x21e8/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,7 +6,8 @@
 LQD_RPC_HOST: str = config("LQD_RPC_HOST", default="localhost")
 LQD_RPC_ENDPOINT_SCHEMA: str = config("LQD_RPC_SCHEMA", default="http")
 PLNTMNT_ENDPOINT = config("PLNTMNT_ENDPOINT", default="http://localhost:9984")
 WEB3STORAGE_TOKEN = config("WEB3STORAGE_TOKEN")
 CID_RESOLVER = config("CID_RESOLVER", default="https://cid-resolver.rddl.io")
 RDDL_ASSET_REG_ENDPOINT = config("RDDL_ASSET_REG_ENDPOINT", default="http://lab.r3c.network:8090/register_asset")
 LIQUID_REGISTRATION_DOMAIN = config("LIQUID_REGISTRATION_DOMAIN", default="lab.r3c.network")
+RDDL_AUTH = config("RDDL_AUTH", default="https://cid-resolver.rddl.io")
```

### Comparing `x21e8-0.8.0/x21e8/main.py` & `x21e8-0.9.0/x21e8/main.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.8.0/x21e8/network/liquid/__init__.py` & `x21e8-0.9.0/x21e8/network/liquid/__init__.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.8.0/x21e8/network/liquid/util.py` & `x21e8-0.9.0/x21e8/network/liquid/util.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.8.0/x21e8/routers/assets.py` & `x21e8-0.9.0/x21e8/routers/assets.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.8.0/x21e8/routers/data.py` & `x21e8-0.9.0/x21e8/routers/data.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.8.0/x21e8/routers/machine.py` & `x21e8-0.9.0/x21e8/routers/machine.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.8.0/x21e8/routers/seed.py` & `x21e8-0.9.0/x21e8/routers/seed.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.8.0/x21e8/routers/utils.py` & `x21e8-0.9.0/x21e8/routers/utils.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.8.0/x21e8/routers/wallet.py` & `x21e8-0.9.0/x21e8/routers/wallet.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.8.0/x21e8/utils/encryption.py` & `x21e8-0.9.0/x21e8/utils/encryption.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.8.0/x21e8/utils/storage.py` & `x21e8-0.9.0/x21e8/utils/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-import json
 import urllib3
 import w3storage
 from urllib.request import urlopen
 from multiformats import CID, multihash
-
+from x21e8.utils.eddsa_auth import get_jwt_token
 from x21e8.config import WEB3STORAGE_TOKEN, CID_RESOLVER
 from x21e8.utils.encryption import encrypt_bytes, decrypt_2_bytes
 
 ENCODING = "utf-8"
 
 w3s = w3storage.API(token=WEB3STORAGE_TOKEN)
 
 
 def get_ipfs_link(cid: str):
     return "https://" + cid + ".ipfs.w3s.link"
 
 
 def register_cid_url(cid: str, url: str):
     http = urllib3.PoolManager()
+    token = get_jwt_token()
     cid_resp = http.request(
-        "POST", CID_RESOLVER + "/entry?cid=" + cid + "&url=" + url, headers={"Content-Type": "application/json"}
+        "POST",
+        CID_RESOLVER + "/entry?cid=" + cid + "&url=" + url,
+        headers={"Content-Type": "application/json", "Authorization": f"Bearer {token}"},
     )
     return cid_resp
 
 
 def decryption_layer(data, decrypt_data: bool = False):
     if decrypt_data:
         print(f"encrypted : {data}")
```

### Comparing `x21e8-0.8.0/x21e8/wallet/base_wallet.py` & `x21e8-0.9.0/x21e8/wallet/base_wallet.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.8.0/x21e8/wallet/planetmint/keymanagement.py` & `x21e8-0.9.0/x21e8/wallet/planetmint/keymanagement.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.8.0/x21e8/wallet/planetmint/keystore.py` & `x21e8-0.9.0/x21e8/wallet/planetmint/keystore.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.8.0/x21e8/wallet/seed.py` & `x21e8-0.9.0/x21e8/wallet/seed.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.8.0/x21e8/wallet/sw_wallet.py` & `x21e8-0.9.0/x21e8/wallet/sw_wallet.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,17 +16,20 @@
         self.public_key = None
         self.planetmint_address = None
         self.liquid_address = None
         self.liquid_derived_key = None
         self._init_wallet()
 
     def planetmint_sign_digest(self, input, message: bytes):
-        cc_key = Ed25519SigningKey(self.private_key, "bytes")
-        signature = cc_key.sign(message, encoding="bytes")
-        return signature  # signature matches signature from other schemes
+        return self.planetmint_sign_challenge(message, encoding="bytes")
+
+    def planetmint_sign_challenge(self, challenge, encoding="base58"):
+        sk = Ed25519SigningKey(self.private_key, "bytes")
+        signature = sk.sign(challenge, encoding)
+        return signature
 
     def liquid_sign_digest(self, message: bytes):
         pass
 
     def get_liquid_pubkey(self) -> bytes:
         return self.liquid_address
```

### Comparing `x21e8-0.8.0/PKG-INFO` & `x21e8-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: x21e8
-Version: 0.8.0
+Version: 0.9.0
 Summary: x21e8 service to manage RDDL network identities on TrustAnchors and workflows.
 Author: Firat Berk Cakar
 Author-email: firat@riddleandcode.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: TrezorCryptoTestRc
 Requires-Dist: bitcoin-utils (>=0.5.6,<0.6.0)
 Requires-Dist: fastapi (>=0.85.0,<0.86.0)
 Requires-Dist: mnemonic (>=0.20,<0.21)
 Requires-Dist: multiformats (>=0.2.1,<0.3.0)
 Requires-Dist: mypy (>=0.982,<0.983)
-Requires-Dist: planetmint-driver (==0.18.2)
+Requires-Dist: planetmint-driver (>=0.18.2,<0.19.0)
 Requires-Dist: pysha3 (>=1.0.2,<2.0.0)
 Requires-Dist: python-decouple (>=3.6,<4.0)
 Requires-Dist: python-rapidjson (>1.0.0)
 Requires-Dist: python-rapidjson-schema (==0.1.1)
 Requires-Dist: requests (>2.20.0)
+Requires-Dist: typing-extensions (==4.5.0)
 Requires-Dist: uvicorn (>=0.19.0,<0.20.0)
 Requires-Dist: w3storage (>=0.0.1,<0.0.2)
 Description-Content-Type: text/markdown
 
 # 0x21e8 RDDL Interaction Service
 
 The 0x21e8 service is usually installed and executed on RDDL compatible hardware wallets (HW-03). The service utilizes the hardware wallet and enables the HW-03 devices to interact with the RDDL network (Planetmint and liquid). 
@@ -68,24 +69,26 @@
     * RPC URL
     * RPC port
     * RPC user
     * RPC password
 * web3storage token to store data
 * RDDL asset registration endpoint
 * RDDL CID resolver
+* RDDL Authentication service to be able to authenticate with EdDSA to RDDL services
 
 The configuration is set via environment variables such as
 * LQD_RPC_PORT
 * LQD_RPC_USER
 * LQD_RPC_PASSWORD
 * LQD_RPC_HOST
 * PLNTMNT_ENDPOINT
 * WEB3STORAGE_TOKEN
 * RDDL_ASSET_REG_ENDPOINT
 * CID_RESOLVER
+* RDDL_AUTH
 
 Alternatively, the variables can be defined within the ```.env``` file of the project. A example ```env.example``` file can be adjusted and copied to ```.env```.
 
 ## Service Execution
 ```bash
 uvicorn --log-level debug --reload x21e8.main:app
 ```
```

