# Comparing `tmp/web3client-1.1.8.tar.gz` & `tmp/web3client-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3client-1.1.8.tar", last modified: Wed Apr 19 13:54:00 2023, max compression
+gzip compressed data, was "web3client-1.1.9.tar", last modified: Fri May 19 17:48:31 2023, max compression
```

## Comparing `web3client-1.1.8.tar` & `web3client-1.1.9.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1069 2022-10-13 15:30:24.076003 web3client-1.1.8/LICENSE
--rw-r--r--   0        0        0     2757 2023-04-17 14:56:39.469040 web3client-1.1.8/README.md
--rw-r--r--   0        0        0     1983 2023-04-19 13:53:38.302364 web3client-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.879656 web3client-1.1.8/src/.DS_Store
--rw-r--r--   0        0        0     6148 2023-03-13 02:23:28.884980 web3client-1.1.8/src/web3client/.DS_Store
--rw-r--r--   0        0        0        0 2022-10-18 14:47:37.603558 web3client-1.1.8/src/web3client/__init__.py
--rw-r--r--   0        0        0    11117 2022-10-18 14:47:37.604295 web3client-1.1.8/src/web3client/abi/erc20.json
--rw-r--r--   0        0        0    24640 2023-04-19 12:54:16.926188 web3client-1.1.8/src/web3client/base_client.py
--rw-r--r--   0        0        0     4436 2023-04-19 12:51:51.450776 web3client-1.1.8/src/web3client/erc20_client.py
--rw-r--r--   0        0        0      342 2022-10-19 17:40:52.208885 web3client-1.1.8/src/web3client/exceptions.py
--rw-r--r--   0        0        0        0 2022-10-18 14:47:37.604873 web3client-1.1.8/src/web3client/helpers/__init__.py
--rw-r--r--   0        0        0     1732 2023-02-13 20:06:35.817499 web3client-1.1.8/src/web3client/helpers/debug.py
--rw-r--r--   0        0        0     2438 2022-10-18 14:47:37.605628 web3client-1.1.8/src/web3client/helpers/general.py
--rw-r--r--   0        0        0     1909 2023-04-10 15:26:30.878490 web3client-1.1.8/src/web3client/helpers/websockets.py
--rw-r--r--   0        0        0        0 2022-10-18 14:47:37.601242 web3client-1.1.8/src/web3factory/__init__.py
--rw-r--r--   0        0        0     2190 2023-04-05 13:58:18.268337 web3client-1.1.8/src/web3factory/erc20_tokens.py
--rw-r--r--   0        0        0     1795 2023-04-19 13:52:52.905078 web3client-1.1.8/src/web3factory/factory.py
--rw-r--r--   0        0        0     2770 2023-04-17 14:56:39.482576 web3client-1.1.8/src/web3factory/networks.py
--rw-r--r--   0        0        0      621 2023-02-13 19:47:49.818983 web3client-1.1.8/src/web3factory/types.py
--rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.878800 web3client-1.1.8/tests/.DS_Store
--rw-r--r--   0        0        0        0 2023-02-23 10:04:23.399090 web3client-1.1.8/tests/__init__.py
--rw-r--r--   0        0        0     6148 2023-04-05 16:39:49.642961 web3client-1.1.8/tests/ape/.DS_Store
--rw-r--r--   0        0        0      779 2023-04-06 10:47:11.288879 web3client-1.1.8/tests/ape/.build/SafeMath.json
--rw-r--r--   0        0        0    14895 2023-04-06 10:47:11.290250 web3client-1.1.8/tests/ape/.build/Token.json
--rw-r--r--   0        0        0    20923 2023-04-19 13:53:42.199720 web3client-1.1.8/tests/ape/.build/__local__.json
--rw-r--r--   0        0        0      600 2023-02-23 10:18:28.269673 web3client-1.1.8/tests/ape/contracts/token/SafeMath.sol
--rw-r--r--   0        0        0     4082 2023-02-23 10:18:28.283242 web3client-1.1.8/tests/ape/contracts/token/Token.sol
--rw-r--r--   0        0        0     3529 2023-04-05 16:42:52.576613 web3client-1.1.8/tests/ape/fixtures.py
--rw-r--r--   0        0        0        0 2023-04-05 15:27:07.832128 web3client-1.1.8/tests/ape/scripts/__init__.py
--rw-r--r--   0        0        0      123 2023-04-05 14:37:05.616337 web3client-1.1.8/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-02-23 10:04:38.139397 web3client-1.1.8/tests/web3client/__init__.py
--rw-r--r--   0        0        0     1300 2023-04-06 11:08:05.647477 web3client-1.1.8/tests/web3client/fixtures.py
--rw-r--r--   0        0        0     1417 2023-02-13 20:04:46.649348 web3client-1.1.8/tests/web3client/test_networks.py
--rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 web3client-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-10-13 15:30:24.076003 web3client-1.1.9/LICENSE
+-rw-r--r--   0        0        0     2757 2023-04-17 14:56:39.469040 web3client-1.1.9/README.md
+-rw-r--r--   0        0        0     1983 2023-05-19 17:46:43.515043 web3client-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.879656 web3client-1.1.9/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2023-03-13 02:23:28.884980 web3client-1.1.9/src/web3client/.DS_Store
+-rw-r--r--   0        0        0        0 2022-10-18 14:47:37.603558 web3client-1.1.9/src/web3client/__init__.py
+-rw-r--r--   0        0        0    11117 2022-10-18 14:47:37.604295 web3client-1.1.9/src/web3client/abi/erc20.json
+-rw-r--r--   0        0        0    24910 2023-05-19 17:46:33.696739 web3client-1.1.9/src/web3client/base_client.py
+-rw-r--r--   0        0        0     4436 2023-04-19 12:51:51.450776 web3client-1.1.9/src/web3client/erc20_client.py
+-rw-r--r--   0        0        0      342 2022-10-19 17:40:52.208885 web3client-1.1.9/src/web3client/exceptions.py
+-rw-r--r--   0        0        0        0 2022-10-18 14:47:37.604873 web3client-1.1.9/src/web3client/helpers/__init__.py
+-rw-r--r--   0        0        0     1723 2023-05-19 17:29:22.495116 web3client-1.1.9/src/web3client/helpers/debug.py
+-rw-r--r--   0        0        0     2438 2022-10-18 14:47:37.605628 web3client-1.1.9/src/web3client/helpers/general.py
+-rw-r--r--   0        0        0     1909 2023-04-10 15:26:30.878490 web3client-1.1.9/src/web3client/helpers/websockets.py
+-rw-r--r--   0        0        0        0 2022-10-18 14:47:37.601242 web3client-1.1.9/src/web3factory/__init__.py
+-rw-r--r--   0        0        0     2190 2023-04-05 13:58:18.268337 web3client-1.1.9/src/web3factory/erc20_tokens.py
+-rw-r--r--   0        0        0     1759 2023-05-19 17:32:25.658006 web3client-1.1.9/src/web3factory/factory.py
+-rw-r--r--   0        0        0     2770 2023-04-17 14:56:39.482576 web3client-1.1.9/src/web3factory/networks.py
+-rw-r--r--   0        0        0      621 2023-02-13 19:47:49.818983 web3client-1.1.9/src/web3factory/types.py
+-rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.878800 web3client-1.1.9/tests/.DS_Store
+-rw-r--r--   0        0        0        0 2023-02-23 10:04:23.399090 web3client-1.1.9/tests/__init__.py
+-rw-r--r--   0        0        0     6148 2023-04-05 16:39:49.642961 web3client-1.1.9/tests/ape/.DS_Store
+-rw-r--r--   0        0        0      779 2023-04-06 10:47:11.288879 web3client-1.1.9/tests/ape/.build/SafeMath.json
+-rw-r--r--   0        0        0    14895 2023-04-06 10:47:11.290250 web3client-1.1.9/tests/ape/.build/Token.json
+-rw-r--r--   0        0        0    20923 2023-05-19 17:46:47.921906 web3client-1.1.9/tests/ape/.build/__local__.json
+-rw-r--r--   0        0        0      600 2023-02-23 10:18:28.269673 web3client-1.1.9/tests/ape/contracts/token/SafeMath.sol
+-rw-r--r--   0        0        0     4082 2023-02-23 10:18:28.283242 web3client-1.1.9/tests/ape/contracts/token/Token.sol
+-rw-r--r--   0        0        0     3529 2023-04-05 16:42:52.576613 web3client-1.1.9/tests/ape/fixtures.py
+-rw-r--r--   0        0        0        0 2023-04-05 15:27:07.832128 web3client-1.1.9/tests/ape/scripts/__init__.py
+-rw-r--r--   0        0        0      123 2023-04-05 14:37:05.616337 web3client-1.1.9/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-02-23 10:04:38.139397 web3client-1.1.9/tests/web3client/__init__.py
+-rw-r--r--   0        0        0     3724 2023-05-19 17:38:35.898202 web3client-1.1.9/tests/web3client/fixtures.py
+-rw-r--r--   0        0        0     1417 2023-02-13 20:04:46.649348 web3client-1.1.9/tests/web3client/test_networks.py
+-rw-r--r--   0        0        0     1413 2023-05-19 17:43:20.552735 web3client-1.1.9/tests/web3client/test_sign.py
+-rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 web3client-1.1.9/PKG-INFO
```

### Comparing `web3client-1.1.8/LICENSE` & `web3client-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/README.md` & `web3client-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/pyproject.toml` & `web3client-1.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "web3client"
-version = "1.1.8"
+version = "1.1.9"
 description = "Batteries-included client to interact with blockchains and smart contracts"
 authors = [
     { name = "coccoinomane", email = "coccoinomane@gmail.com" },
 ]
 readme = "README.md"
 keywords = [
     "web3",
```

### Comparing `web3client-1.1.8/src/.DS_Store` & `web3client-1.1.9/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/src/web3client/.DS_Store` & `web3client-1.1.9/src/web3client/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/src/web3client/abi/erc20.json` & `web3client-1.1.9/src/web3client/abi/erc20.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/src/web3client/base_client.py` & `web3client-1.1.9/src/web3client/base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     2. Specialize it by making a subclass. Override the parameters
        to match the desired blockchain and, optionally, contract.
     3. If the blockchain and contract you need to use is supported,
        just use one of the 'make' methods in factory.py.
 
     Attributes
     ----------------------
-    node_uri: str | RPC node to use
+    node_uri: str | RPC node to use.  Set it to None for a uninitialized client.
     chain_id: int = None | ID of the chain
     tx_type: int = 2 | Type of transaction: 1 for pre-EIP-1599, 2 for EIP-1599. More details here > https://docs.infura.io/infura/networks/ethereum/concepts/transaction-types
     private_key: str = None | Private key to use (optional)
     max_priority_fee_in_gwei: float = 1 | Miner's tip, relevant only for type-2 transactions (optional, default is 1)
     upper_limit_for_base_fee_in_gwei: float = inf | Raise an exception if baseFee is larger than this (optional, default is no limit)
     contract_address: Address = None | Address of smart contract (optional)
     abi: dict[str, Any] = None | ABI of smart contract; to generate from a JSON file, use static method get_contract_abi_from_file() (optional)
@@ -83,16 +83,15 @@
     ) -> None:
         # Set attributes
         self.chain_id: int = chain_id
         self.tx_type: int = tx_type
         self.max_priority_fee_in_gwei: float = max_priority_fee_in_gwei
         self.upper_limit_for_base_fee_in_gwei: float = upper_limit_for_base_fee_in_gwei
         # Initialize web3.py provider
-        if node_uri:
-            self.set_provider(node_uri)
+        self.set_provider(node_uri)
         # User account
         if private_key:
             self.set_account(private_key)
         # Initialize the contract
         # TODO: we should be able to load an ABI without a specific address.
         # This might be useful to access the ABI decoding functions of web3.
         # For example, to read events from a tx only the ABI is needed, you
@@ -643,20 +642,26 @@
     def get_provider(node_uri: str) -> Web3:
         """
         Initialize provider (HTTPS & WS supported).
 
         TODO: Support autodetection with empty node_uri
         docs here https://web3py.readthedocs.io/en/stable/providers.html#how-automated-detection-works
         """
-        if node_uri[0:4] == "http":
+        if node_uri is None:
+            return Web3()
+        elif node_uri[0:4] == "http":
             return Web3(Web3.HTTPProvider(node_uri))
         elif node_uri[0:2] == "ws":
             return Web3(Web3.WebsocketProvider(node_uri))
+        elif node_uri[-4:] == ".ipc":
+            return Web3(Web3.IPCProvider(node_uri))
         else:
-            return Web3()
+            raise ValueError(
+                "Node URI not recognized, must start with http, ws or end with .ipc"
+            )
 
     @staticmethod
     def get_gas_spent_in_eth(txReceipt: TxReceipt) -> float:
         """
         Given the transaction receipt, return the ETH that
         was spent in gas to process the transaction
         """
```

### Comparing `web3client-1.1.8/src/web3client/erc20_client.py` & `web3client-1.1.9/src/web3client/erc20_client.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/src/web3client/helpers/debug.py` & `web3client-1.1.9/src/web3client/helpers/debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
     Get a transaction receipt and print it, together with
     the tx cost
     """
     print(">>> TX SENT!")
     print("Hash = " + txHash)
     print("Waiting for transaction to finalize...")
-    tx_receipt = client.get_transaction_receipt(txHash)
+    tx_receipt = client.get_tx_receipt(txHash)
     print(">>> TX IS ON THE BLOCKCHAIN :-)")
     pprint.pprint(tx_receipt)
     print(">>> ETH SPENT")
     print(BaseClient.get_gas_spent_in_eth(tx_receipt))
 
 
 def pprintAttributeDict(
```

### Comparing `web3client-1.1.8/src/web3client/helpers/general.py` & `web3client-1.1.9/src/web3client/helpers/general.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/src/web3client/helpers/websockets.py` & `web3client-1.1.9/src/web3client/helpers/websockets.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/src/web3factory/erc20_tokens.py` & `web3client-1.1.9/src/web3factory/erc20_tokens.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/src/web3factory/factory.py` & `web3client-1.1.9/src/web3factory/factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from typing import Any, Type, cast
 
-from eth_typing import Address
-
 from web3client.base_client import BaseClient
 from web3client.erc20_client import Erc20Client
 from web3factory.erc20_tokens import get_token_config
 from web3factory.networks import get_network_config, pick_first_rpc
 from web3factory.types import NetworkName, TokenName
 
 
@@ -27,15 +25,15 @@
     client.set_middlewares(networkConfig.get("middlewares", []))
     return client
 
 
 def make_erc20_client(
     networkName: NetworkName,
     node_uri: str = None,
-    token_address: Address = None,
+    token_address: str = None,
     token_name: TokenName = None,
     **clientArgs: Any,
 ) -> Erc20Client:
     """
     Return a brand new client configured for the given blockchain
     and preloaded with the ERC20 token ABI.
```

### Comparing `web3client-1.1.8/src/web3factory/networks.py` & `web3client-1.1.9/src/web3factory/networks.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/src/web3factory/types.py` & `web3client-1.1.9/src/web3factory/types.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/tests/.DS_Store` & `web3client-1.1.9/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/tests/ape/.DS_Store` & `web3client-1.1.9/tests/ape/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/tests/ape/.build/SafeMath.json` & `web3client-1.1.9/tests/ape/.build/SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/tests/ape/.build/Token.json` & `web3client-1.1.9/tests/ape/.build/Token.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/tests/ape/.build/__local__.json` & `web3client-1.1.9/tests/ape/.build/__local__.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/tests/ape/contracts/token/SafeMath.sol` & `web3client-1.1.9/tests/ape/contracts/token/SafeMath.sol`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/tests/ape/contracts/token/Token.sol` & `web3client-1.1.9/tests/ape/contracts/token/Token.sol`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/tests/ape/fixtures.py` & `web3client-1.1.9/tests/ape/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.8/tests/web3client/fixtures.py` & `web3client-1.1.9/tests/web3client/test_networks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,39 @@
 from typing import Dict
 
-import pytest
-
 from web3client.base_client import BaseClient
-from web3factory.factory import make_client
-from web3factory.networks import supported_networks
-
-
-@pytest.fixture()
-def rpcs() -> Dict[str, str]:
-    """
-    Let's use difrerent RPCs for tests, in case the regular ones
-    are throttled
-    """
-    return {
-        "eth": "https://mainnet.infura.io/v3/db0e363aad2f43ee8a2f259733721512",
-    }
-
-
-@pytest.fixture()
-def address() -> str:
-    return "0x3A8c8833Abe2e8454F59574A2A18b9bA8A28Ea4F"
-
-
-@pytest.fixture()
-def private_key() -> str:
-    return "53caa63985c6089c84be07e3f42d5d7ebd47a8a097835ede937d4c5e1f1021dd"
-
-
-@pytest.fixture()
-def networks_clients(rpcs: Dict[str, str]) -> Dict[str, BaseClient]:
-    """
-    Ready-to-use clients, indexed by network name, no signer
-    """
-    clients = {}
-    for network in supported_networks:
-        name = network["name"]
-        node_uri = rpcs.get(name)
-        clients[name] = make_client(name, node_uri)
-    return clients
-
-
-@pytest.fixture()
-def eth_client() -> BaseClient:
-    return make_client("eth")
-
-
-@pytest.fixture()
-def bnb_client() -> BaseClient:
-    return make_client("bnb")
 
 
-@pytest.fixture()
-def bnb_ws_client() -> BaseClient:
-    return make_client("bnb", node_uri="wss://dex.binance.org/api/ws")
+def test_get_nonce(address: str, networks_clients: Dict[str, BaseClient]) -> None:
+    for network, client in networks_clients.items():
+        nonce = client.get_nonce(address)
+        assert type(nonce) is int
+        assert nonce >= 0
+
+
+def test_get_latest_block(networks_clients: Dict[str, BaseClient]) -> None:
+    for network, client in networks_clients.items():
+        block = client.get_latest_block()
+        assert type(block.get("number")) is int
+        assert block.get("number") >= 0
+        assert type(block.get("size")) is int
+        assert block.get("size") >= 0
+        assert type(block.get("difficulty")) is int
+        assert block.get("difficulty") >= 0
+        assert type(block.get("transactions")) is list
+
+
+def test_get_eth_balance(address: str, networks_clients: Dict[str, BaseClient]) -> None:
+    for network, client in networks_clients.items():
+        balance = client.get_balance_in_wei(address)
+        assert type(balance) is int
+        assert balance >= 0
+
+
+def test_get_sign_message(
+    private_key: str, networks_clients: Dict[str, BaseClient]
+) -> None:
+    msg = "Hello world!"
+    for network, client in networks_clients.items():
+        client.set_account(private_key=private_key)
+        signed_message = client.sign_message(msg)
+        assert client.is_message_signed_by_me(msg, signed_message)
```

### Comparing `web3client-1.1.8/PKG-INFO` & `web3client-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3client
-Version: 1.1.8
+Version: 1.1.9
 Summary: Batteries-included client to interact with blockchains and smart contracts
 License: MIT
 Keywords: web3,blockchain,ethereum,evm
 Author-email: coccoinomane <coccoinomane@gmail.com>
 Requires-Python: >=3.9,<3.11
 Project-URL: homepage, https://github.com/coccoinomane/web3client
 Project-URL: repository, https://github.com/coccoinomane/web3client
```

