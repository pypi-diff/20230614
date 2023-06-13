# Comparing `tmp/huma_signals-0.3.1.tar.gz` & `tmp/huma_signals-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huma_signals-0.3.1.tar", max compression
+gzip compressed data, was "huma_signals-0.4.0.tar", max compression
```

## Comparing `huma_signals-0.3.1.tar` & `huma_signals-0.4.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0    34523 2023-06-09 20:15:53.683031 huma_signals-0.3.1/LICENSE
--rw-r--r--   0        0        0     2162 2023-06-09 20:15:53.683031 huma_signals-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/adapters/__init__.py
--rw-r--r--   0        0        0      586 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/adapters/ethereum_wallet/README.md
--rw-r--r--   0        0        0        0 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/adapters/ethereum_wallet/__init__.py
--rw-r--r--   0        0        0     3088 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/adapters/ethereum_wallet/adapter.py
--rw-r--r--   0        0        0      186 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/adapters/ethereum_wallet/settings.py
--rw-r--r--   0        0        0      586 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/adapters/lending_pools/README.md
--rw-r--r--   0        0        0        0 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/adapters/lending_pools/__init__.py
--rw-r--r--   0        0        0    23699 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json
--rw-r--r--   0        0        0    30632 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json
--rw-r--r--   0        0        0    32155 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json
--rw-r--r--   0        0        0    30290 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json
--rw-r--r--   0        0        0     4533 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/adapters/lending_pools/adapter.py
--rw-r--r--   0        0        0     1938 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/adapters/lending_pools/registry.py
--rw-r--r--   0        0        0      158 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/adapters/lending_pools/settings.py
--rw-r--r--   0        0        0      145 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/adapters/models.py
--rw-r--r--   0        0        0      591 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/adapters/polygon_wallet/README.md
--rw-r--r--   0        0        0        0 2023-06-09 20:15:53.683031 huma_signals-0.3.1/huma_signals/adapters/polygon_wallet/__init__.py
--rw-r--r--   0        0        0     3201 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/adapters/polygon_wallet/adapter.py
--rw-r--r--   0        0        0      222 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/adapters/polygon_wallet/settings.py
--rw-r--r--   0        0        0      576 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/adapters/request_network/README.md
--rw-r--r--   0        0        0        0 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/adapters/request_network/__init__.py
--rw-r--r--   0        0        0     4372 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/adapters/request_network/models.py
--rw-r--r--   0        0        0     5464 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/adapters/request_network/request_invoice_adapter.py
--rw-r--r--   0        0        0     4930 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/adapters/request_network/request_transaction_adapter.py
--rw-r--r--   0        0        0      284 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/adapters/request_network/settings.py
--rw-r--r--   0        0        0        0 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/adapters/superfluid/__init__.py
--rw-r--r--   0        0        0      238 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/adapters/superfluid/settings.py
--rw-r--r--   0        0        0     3587 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/adapters/superfluid/superfluid_adapter.py
--rw-r--r--   0        0        0      436 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/adapters/superfluid/superfluid_models.py
--rw-r--r--   0        0        0        0 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/clients/eth_client/__init__.py
--rw-r--r--   0        0        0     1427 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/clients/eth_client/eth_client.py
--rw-r--r--   0        0        0      673 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/clients/eth_client/eth_types.py
--rw-r--r--   0        0        0        0 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/clients/polygon_client/__init__.py
--rw-r--r--   0        0        0     1503 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/clients/polygon_client/polygon_client.py
--rw-r--r--   0        0        0      685 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/clients/polygon_client/polygon_types.py
--rw-r--r--   0        0        0        0 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/clients/request_client/__init__.py
--rw-r--r--   0        0        0     8129 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/clients/request_client/request_client.py
--rw-r--r--   0        0        0      900 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/clients/request_client/request_types.py
--rw-r--r--   0        0        0        0 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/commons/__init__.py
--rw-r--r--   0        0        0      291 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/commons/chains.py
--rw-r--r--   0        0        0      330 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/commons/datetime_utils.py
--rw-r--r--   0        0        0      227 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/commons/pydantic_utils.py
--rw-r--r--   0        0        0      569 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/commons/string_utils.py
--rw-r--r--   0        0        0     1309 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/commons/tokens.py
--rw-r--r--   0        0        0     1078 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/commons/web3_utils.py
--rw-r--r--   0        0        0      499 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/dotenv/example.env
--rw-r--r--   0        0        0     1157 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/exceptions.py
--rw-r--r--   0        0        0      322 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/models.py
--rw-r--r--   0        0        0        0 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/py.typed
--rw-r--r--   0        0        0     1563 2023-06-09 20:15:53.687031 huma_signals-0.3.1/huma_signals/settings.py
--rw-r--r--   0        0        0     2792 2023-06-09 20:15:53.687031 huma_signals-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 huma_signals-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-13 21:53:22.735692 huma_signals-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2162 2023-06-13 21:53:22.735692 huma_signals-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/__init__.py
+-rw-r--r--   0        0        0      586 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/ethereum_wallet/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/ethereum_wallet/__init__.py
+-rw-r--r--   0        0        0     3088 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/ethereum_wallet/adapter.py
+-rw-r--r--   0        0        0      186 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/ethereum_wallet/settings.py
+-rw-r--r--   0        0        0      586 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/__init__.py
+-rw-r--r--   0        0        0    23699 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json
+-rw-r--r--   0        0        0    30632 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json
+-rw-r--r--   0        0        0    32155 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json
+-rw-r--r--   0        0        0    30290 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json
+-rw-r--r--   0        0        0     4533 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/adapter.py
+-rw-r--r--   0        0        0     1938 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/registry.py
+-rw-r--r--   0        0        0      158 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/settings.py
+-rw-r--r--   0        0        0      145 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/models.py
+-rw-r--r--   0        0        0      591 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/polygon_wallet/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/polygon_wallet/__init__.py
+-rw-r--r--   0        0        0     3201 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/polygon_wallet/adapter.py
+-rw-r--r--   0        0        0      222 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/polygon_wallet/settings.py
+-rw-r--r--   0        0        0      576 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/request_network/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/request_network/__init__.py
+-rw-r--r--   0        0        0     4156 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/request_network/models.py
+-rw-r--r--   0        0        0     5466 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/request_network/request_invoice_adapter.py
+-rw-r--r--   0        0        0     4930 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/request_network/request_transaction_adapter.py
+-rw-r--r--   0        0        0      284 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/request_network/settings.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/superfluid/__init__.py
+-rw-r--r--   0        0        0      238 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/superfluid/settings.py
+-rw-r--r--   0        0        0     4252 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/superfluid/superfluid_adapter.py
+-rw-r--r--   0        0        0      501 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/superfluid/superfluid_models.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/eth_client/__init__.py
+-rw-r--r--   0        0        0     1427 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/eth_client/eth_client.py
+-rw-r--r--   0        0        0      673 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/eth_client/eth_types.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/polygon_client/__init__.py
+-rw-r--r--   0        0        0     1503 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/polygon_client/polygon_client.py
+-rw-r--r--   0        0        0      685 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/polygon_client/polygon_types.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/request_client/__init__.py
+-rw-r--r--   0        0        0     8250 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/request_client/request_client.py
+-rw-r--r--   0        0        0      978 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/request_client/request_types.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/commons/__init__.py
+-rw-r--r--   0        0        0      291 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/commons/chains.py
+-rw-r--r--   0        0        0      330 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/commons/datetime_utils.py
+-rw-r--r--   0        0        0      227 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/commons/pydantic_utils.py
+-rw-r--r--   0        0        0      569 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/commons/string_utils.py
+-rw-r--r--   0        0        0     1309 2023-06-13 21:53:22.739692 huma_signals-0.4.0/huma_signals/commons/tokens.py
+-rw-r--r--   0        0        0     1078 2023-06-13 21:53:22.739692 huma_signals-0.4.0/huma_signals/commons/web3_utils.py
+-rw-r--r--   0        0        0      499 2023-06-13 21:53:22.739692 huma_signals-0.4.0/huma_signals/dotenv/example.env
+-rw-r--r--   0        0        0     1157 2023-06-13 21:53:22.739692 huma_signals-0.4.0/huma_signals/exceptions.py
+-rw-r--r--   0        0        0      322 2023-06-13 21:53:22.739692 huma_signals-0.4.0/huma_signals/models.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:53:22.739692 huma_signals-0.4.0/huma_signals/py.typed
+-rw-r--r--   0        0        0     1563 2023-06-13 21:53:22.739692 huma_signals-0.4.0/huma_signals/settings.py
+-rw-r--r--   0        0        0     2792 2023-06-13 21:53:22.739692 huma_signals-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 huma_signals-0.4.0/PKG-INFO
```

### Comparing `huma_signals-0.3.1/LICENSE` & `huma_signals-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/README.md` & `huma_signals-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/adapters/ethereum_wallet/README.md` & `huma_signals-0.4.0/huma_signals/adapters/ethereum_wallet/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/adapters/ethereum_wallet/adapter.py` & `huma_signals-0.4.0/huma_signals/adapters/ethereum_wallet/adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/adapters/lending_pools/README.md` & `huma_signals-0.4.0/huma_signals/adapters/lending_pools/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json` & `huma_signals-0.4.0/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json` & `huma_signals-0.4.0/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json` & `huma_signals-0.4.0/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json` & `huma_signals-0.4.0/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/adapters/lending_pools/adapter.py` & `huma_signals-0.4.0/huma_signals/adapters/lending_pools/adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/adapters/lending_pools/registry.py` & `huma_signals-0.4.0/huma_signals/adapters/lending_pools/registry.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/adapters/polygon_wallet/README.md` & `huma_signals-0.4.0/huma_signals/adapters/polygon_wallet/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/adapters/polygon_wallet/adapter.py` & `huma_signals-0.4.0/huma_signals/adapters/polygon_wallet/adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/adapters/request_network/README.md` & `huma_signals-0.4.0/huma_signals/adapters/request_network/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/adapters/request_network/models.py` & `huma_signals-0.4.0/huma_signals/adapters/request_network/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,112 +9,108 @@
 
 logger = structlog.get_logger()
 
 
 class RequestInvoiceSignals(models.HumaBaseModel):
     # transactions based features: Payer Quality
     payer_tenure: int = pydantic.Field(
-        ..., description="The number of days since the payer's first transaction"
+        description="The number of days since the payer's first transaction"
     )
     payer_recent: int = pydantic.Field(
-        ..., description="The number of days since the payer's most recent transaction"
+        description="The number of days since the payer's most recent transaction"
     )
     payer_count: int = pydantic.Field(
-        ..., description="The number of transactions the payer has made"
+        description="The number of transactions the payer has made"
     )
     payer_total_amount: int = pydantic.Field(
-        ..., description="The total amount the payer has paid"
+        description="The total amount the payer has paid"
     )
     payer_unique_payees: int = pydantic.Field(
-        ..., description="The number of unique payees the payer has paid"
+        description="The number of unique payees the payer has paid"
     )
 
     # transactions based features: Payee Quality
     payee_tenure: int = pydantic.Field(
-        ..., description="The number of days since the payee's first transaction"
+        description="The number of days since the payee's first transaction"
     )
     payee_recent: int = pydantic.Field(
-        ..., description="The number of days since the payee's most recent transaction"
+        description="The number of days since the payee's most recent transaction"
     )
     payee_count: int = pydantic.Field(
-        ..., description="The number of transactions the payee has made"
+        description="The number of transactions the payee has made"
     )
     payee_total_amount: int = pydantic.Field(
-        ..., description="The total amount the payee has received"
+        description="The total amount the payee has received"
     )
     payee_unique_payers: int = pydantic.Field(
-        ..., description="The number of unique payers the payee has received"
+        description="The number of unique payers the payee has received"
     )
 
     # transactions based features: Pair Quality
     mutual_count: int = pydantic.Field(
-        ..., description="The number of transactions between the payer and payee"
+        description="The number of transactions between the payer and payee"
     )
     mutual_total_amount: int = pydantic.Field(
-        ..., description="The total amount the payer and payee have transacted"
+        description="The total amount the payer and payee have transacted"
     )
 
     # invoice based features
     payee_match_borrower: bool = pydantic.Field(
-        ..., description="Whether the borrower is the invoice's payee"
+        description="Whether the borrower is the invoice's payee"
     )
     payer_match_payee: bool = pydantic.Field(
-        ..., description="Whether the payee is the invoice's payer"
+        description="Whether the payee is the invoice's payer"
     )
     borrower_own_invoice: bool = pydantic.Field(
-        ..., description="Whether the borrower own the invoice NFT token"
+        description="Whether the borrower own the invoice NFT token"
     )
     days_until_due_date: int = pydantic.Field(
-        ..., description="The number of days until the invoice's due date"
+        description="The number of days until the invoice's due date"
     )
     invoice_amount: decimal.Decimal = pydantic.Field(
-        ..., description="The amount of the invoice"
-    )
-
-    # allowlist feature
-    payer_on_allowlist: bool = pydantic.Field(
-        ..., description="Whether the payer is on the allowlist"
+        description="The amount of the invoice"
     )
+    token_id: str = pydantic.Field(description="The ID of the invoice")
 
 
 class RequestTransactionSignals(models.HumaBaseModel):
     # transactions based features: Payer Quality
     payer_tenure: int = pydantic.Field(
-        ..., description="The number of days since the payer's first transaction"
+        description="The number of days since the payer's first transaction"
     )
     payer_recent: int = pydantic.Field(
-        ..., description="The number of days since the payer's most recent transaction"
+        description="The number of days since the payer's most recent transaction"
     )
     payer_count: int = pydantic.Field(
-        ..., description="The number of transactions the payer has made"
+        description="The number of transactions the payer has made"
     )
     payer_total_amount: int = pydantic.Field(
-        ..., description="The total amount the payer has paid"
+        description="The total amount the payer has paid"
     )
     payer_unique_payees: int = pydantic.Field(
-        ..., description="The number of unique payees the payer has paid"
+        description="The number of unique payees the payer has paid"
     )
 
     # transactions based features: Payee Quality
     payee_tenure: int = pydantic.Field(
-        ..., description="The number of days since the payee's first transaction"
+        description="The number of days since the payee's first transaction"
     )
     payee_recent: int = pydantic.Field(
-        ..., description="The number of days since the payee's most recent transaction"
+        description="The number of days since the payee's most recent transaction"
     )
     payee_count: int = pydantic.Field(
-        ..., description="The number of transactions the payee has made"
+        description="The number of transactions the payee has made"
     )
     payee_total_amount: int = pydantic.Field(
-        ..., description="The total amount the payee has received"
+        description="The total amount the payee has received"
     )
     payee_unique_payers: int = pydantic.Field(
-        ..., description="The number of unique payers the payee has received"
+        description="The number of unique payers the payee has received"
     )
 
     # transactions based features: Pair Quality
     mutual_count: int = pydantic.Field(
-        ..., description="The number of transactions between the payer and payee"
+        description="The number of transactions between the payer and payee"
     )
     mutual_total_amount: int = pydantic.Field(
-        ..., description="The total amount the payer and payee have transacted"
+        description="The total amount the payer and payee have transacted"
     )
```

### Comparing `huma_signals-0.3.1/huma_signals/adapters/request_network/request_invoice_adapter.py` & `huma_signals-0.4.0/huma_signals/adapters/request_network/request_invoice_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         **kwargs: Any,
     ) -> models.RequestInvoiceSignals:
         if not web3.Web3.is_address(borrower_wallet_address):
             raise exceptions.InvalidAddressException(
                 f"Invalid borrower wallet address: {borrower_wallet_address}"
             )
 
-        invoice = await self.request_client.get_invoice(invoice_id=receivable_param)
+        invoice = await self.request_client.get_invoice(request_id=receivable_param)
         records = []
         records.extend(
             await self.request_client.get_payments(
                 from_address=invoice.payer, to_address=None
             )
         )
         records.extend(
@@ -115,9 +115,9 @@
             ),
             borrower_own_invoice=(
                 invoice.token_owner.lower() == borrower_wallet_address.lower()
             ),
             payer_match_payee=(invoice.payer.lower() == invoice.payee.lower()),
             days_until_due_date=(invoice.due_date - datetime.datetime.utcnow()).days,
             invoice_amount=invoice.amount,
-            payer_on_allowlist=True,
+            token_id=invoice.token_id,
         )
```

### Comparing `huma_signals-0.3.1/huma_signals/adapters/request_network/request_transaction_adapter.py` & `huma_signals-0.4.0/huma_signals/adapters/request_network/request_transaction_adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/adapters/superfluid/superfluid_adapter.py` & `huma_signals-0.4.0/huma_signals/adapters/superfluid/superfluid_adapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -52,21 +52,35 @@
             borrower_wallet_address,
             payer_wallet_address,
             super_token_address,
         ]:
             if not web3.Web3.is_address(address):
                 raise exceptions.InvalidAddressException(f"Invalid address: {address}")
 
+        sender_address = payer_wallet_address.lower()
+        receiver_address = borrower_wallet_address.lower()
+        token_address = super_token_address.lower()
         current_stream = await self._get_current_stream(
-            sender_address=payer_wallet_address.lower(),
-            receiver_address=borrower_wallet_address.lower(),
-            token_address=super_token_address.lower(),
+            sender_address=sender_address,
+            receiver_address=receiver_address,
+            token_address=token_address,
         )
+        # Pylint doesn't recognize the `@combomethod` decorator that makes a method
+        # callable as a class method.
+        stream_id = web3.Web3.solidity_keccak(  # pylint: disable=no-value-for-parameter
+            abi_types=["address", "address", "address"],
+            values=[
+                web3.Web3.to_checksum_address(token_address),
+                web3.Web3.to_checksum_address(sender_address),
+                web3.Web3.to_checksum_address(receiver_address),
+            ],
+        ).hex()
         return superfluid_models.SuperfluidSignals(
             current_flow_rate=current_stream.current_flow_rate,
+            stream_id=stream_id,
         )
 
     async def _get_current_stream(
         self, sender_address: str, receiver_address: str, token_address: str
     ) -> superfluid_models.SuperfluidStream:
         try:
             async with httpx.AsyncClient() as client:
```

### Comparing `huma_signals-0.3.1/huma_signals/clients/eth_client/eth_client.py` & `huma_signals-0.4.0/huma_signals/clients/eth_client/eth_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/clients/eth_client/eth_types.py` & `huma_signals-0.4.0/huma_signals/clients/eth_client/eth_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/clients/polygon_client/polygon_client.py` & `huma_signals-0.4.0/huma_signals/clients/polygon_client/polygon_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/clients/polygon_client/polygon_types.py` & `huma_signals-0.4.0/huma_signals/clients/polygon_client/polygon_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/clients/request_client/request_client.py` & `huma_signals-0.4.0/huma_signals/clients/request_client/request_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     async def get_payments(
         self,
         from_address: str | None,
         to_address: str | None,
     ) -> list[dict[str, Any]]:
         pass
 
-    async def get_invoice(self, invoice_id: str) -> request_types.Invoice:
+    async def get_invoice(self, request_id: str) -> request_types.Invoice:
         pass
 
     @classmethod
     def enrich_payments_data(
         cls, payments_raw_df: pd.DataFrame, chain: chains.Chain
     ) -> pd.DataFrame:
         """
@@ -167,18 +167,18 @@
         except Exception as e:
             message = f"Error fetching payments: {e}"
             logger.exception(message)
             raise exceptions.RequestException(message=message) from e
 
         return payments
 
-    async def get_invoice(self, invoice_id: str) -> request_types.Invoice:
+    async def get_invoice(self, request_id: str) -> request_types.Invoice:
         try:
             async with httpx.AsyncClient(base_url=self.invoice_api_url) as client:
-                resp = await client.get(f"?id={invoice_id}")
+                resp = await client.get(f"?id={request_id}")
                 resp.raise_for_status()
                 invoice_info = resp.json()
                 if not web3.Web3.is_address(invoice_info["owner"]):
                     raise exceptions.InvalidAddressException(
                         f"Invoice's owner is not a valid address: {invoice_info['owner']}"
                     )
                 if not web3.Web3.is_address(invoice_info["payer"]):
@@ -193,25 +193,27 @@
                 return request_types.Invoice(
                     token_owner=invoice_info["owner"].lower(),
                     currency=invoice_info.get("currencyInfo").get("symbol"),
                     amount=decimal.Decimal(invoice_info["expectedAmount"]),
                     status="",
                     payer=invoice_info["payer"].lower(),
                     payee=invoice_info["payee"].lower(),
+                    # TODO(jiatu): do we need to add tz info here?
                     creation_date=datetime.datetime.fromtimestamp(
                         invoice_info["creationDate"]
                     ),
                     # TODO: Figure out way to get real due date
                     due_date=datetime.datetime.fromtimestamp(
                         invoice_info["creationDate"]
                     )
                     + datetime.timedelta(days=30),
+                    token_id=invoice_info["tokenId"],
                 )
         except httpx.HTTPStatusError as e:
             logger.exception(
                 f"Request Network API returned status code {e.response.status_code}",
                 base_url=self.invoice_api_url,
-                receivable_param=invoice_id,
+                receivable_param=request_id,
             )
             raise exceptions.RequestException(
                 f"Request Network API returned status code {e.response.status_code}",
             ) from e
```

### Comparing `huma_signals-0.3.1/huma_signals/clients/request_client/request_types.py` & `huma_signals-0.4.0/huma_signals/clients/request_client/request_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import pydantic
 
 from huma_signals import models
 
 
 class Invoice(models.HumaBaseModel):
+    token_id: str = pydantic.Field(description="The ID of the invoice token")
     token_owner: str = pydantic.Field(description="The address of the token owner")
     currency: str = pydantic.Field(
         description="The currency of the invoice (e.g. USDC, ETH, etc.)"
     )
     amount: decimal.Decimal = pydantic.Field(
         description="The amount of the invoice (e.g. 100)"
     )
```

### Comparing `huma_signals-0.3.1/huma_signals/commons/string_utils.py` & `huma_signals-0.4.0/huma_signals/commons/string_utils.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/commons/tokens.py` & `huma_signals-0.4.0/huma_signals/commons/tokens.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/commons/web3_utils.py` & `huma_signals-0.4.0/huma_signals/commons/web3_utils.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/exceptions.py` & `huma_signals-0.4.0/huma_signals/exceptions.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/huma_signals/settings.py` & `huma_signals-0.4.0/huma_signals/settings.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.3.1/pyproject.toml` & `huma_signals-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "huma-signals"
-version = "0.3.1"
+version = "0.4.0"
 description = "Enables access to high-quality signals about a borrower's income, assets, and liabilities."
 authors = ["Jiatu Liu <jiatu@huma.finance>", "Ji Peng <ji@huma.finance>"]
 license = "AGPL v3"
 readme = "README.md"
 packages = [{include = "huma_signals"}]
 homepage = "https://github.com/00labs/huma-signals/"
 documentation = "https://docs.huma.finance/developer-guidelines/decentralized_signal_portfolio"
```

### Comparing `huma_signals-0.3.1/PKG-INFO` & `huma_signals-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huma-signals
-Version: 0.3.1
+Version: 0.4.0
 Summary: Enables access to high-quality signals about a borrower's income, assets, and liabilities.
 Home-page: https://github.com/00labs/huma-signals/
 License: AGPL v3
 Author: Jiatu Liu
 Author-email: jiatu@huma.finance
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: huma-signals Version: 0.3.1 Summary: Enables access
+Metadata-Version: 2.1 Name: huma-signals Version: 0.4.0 Summary: Enables access
 to high-quality signals about a borrower's income, assets, and liabilities.
 Home-page: https://github.com/00labs/huma-signals/ License: AGPL v3 Author:
 Jiatu Liu Author-email: jiatu@huma.finance Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: aiofiles (>=22.1.0,<23.0.0) Requires-Dist: httpx
 (>=0.24.0,<0.25.0) Requires-Dist: orjson (>=3.8.5,<4.0.0) Requires-Dist: pandas
```

