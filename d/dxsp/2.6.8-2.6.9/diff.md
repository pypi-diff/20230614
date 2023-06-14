# Comparing `tmp/dxsp-2.6.8.tar.gz` & `tmp/dxsp-2.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.6.8.tar", max compression
+gzip compressed data, was "dxsp-2.6.9.tar", max compression
```

## Comparing `dxsp-2.6.8.tar` & `dxsp-2.6.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-08 15:15:07.664281 dxsp-2.6.8/LICENSE
--rw-r--r--   0        0        0     2348 2023-06-08 15:15:07.664281 dxsp-2.6.8/README.md
--rw-r--r--   0        0        0       86 2023-06-08 15:15:28.893762 dxsp-2.6.8/dxsp/__init__.py
--rw-r--r--   0        0        0      387 2023-06-08 15:15:07.664281 dxsp-2.6.8/dxsp/config.py
--rw-r--r--   0        0        0     3679 2023-06-08 15:15:07.664281 dxsp-2.6.8/dxsp/default_settings.toml
--rw-r--r--   0        0        0    18964 2023-06-08 15:15:07.664281 dxsp-2.6.8/dxsp/main.py
--rw-r--r--   0        0        0     1542 2023-06-08 15:15:28.893762 dxsp-2.6.8/pyproject.toml
--rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dxsp-2.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-11 11:51:34.177079 dxsp-2.6.9/LICENSE
+-rw-r--r--   0        0        0     2348 2023-06-11 11:51:34.177079 dxsp-2.6.9/README.md
+-rw-r--r--   0        0        0       86 2023-06-11 11:51:55.705159 dxsp-2.6.9/dxsp/__init__.py
+-rw-r--r--   0        0        0      387 2023-06-11 11:51:34.177079 dxsp-2.6.9/dxsp/config.py
+-rw-r--r--   0        0        0     3699 2023-06-11 11:51:34.177079 dxsp-2.6.9/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    18704 2023-06-11 11:51:34.177079 dxsp-2.6.9/dxsp/main.py
+-rw-r--r--   0        0        0     1552 2023-06-11 11:51:55.705159 dxsp-2.6.9/pyproject.toml
+-rw-r--r--   0        0        0     3154 1970-01-01 00:00:00.000000 dxsp-2.6.9/PKG-INFO
```

### Comparing `dxsp-2.6.8/LICENSE` & `dxsp-2.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.8/README.md` & `dxsp-2.6.9/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.8/dxsp/default_settings.toml` & `dxsp-2.6.9/dxsp/default_settings.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 [default]
+dxsp_enabled = true
 loglevel = "INFO"
 headers = {User-Agent= 'Mozilla/5.0'}
 #📝tokenlist
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 #📝trading setup
```

### Comparing `dxsp-2.6.8/dxsp/main.py` & `dxsp-2.6.9/dxsp/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         except Exception as error:
             raise error
 
         self.protocol_type = settings.dex_protocol_type
         self.chain_id = settings.dex_chain_id
         self.wallet_address = self.w3.to_checksum_address(
             settings.dex_wallet_address)
-        self.account = str(self.chain_id) + " - "+str(self.wallet_address[-8:])
+        self.account = f"{str(self.chain_id)} - {str(self.wallet_address[-8:])}"
         self.private_key = settings.dex_private_key
 
         self.cg = CoinGeckoAPI()
 
     async def execute_order(self, order_params):
         """Execute swap function."""
         action = order_params.get('action')
@@ -136,19 +136,20 @@
 
 
     async def router(self):
         try:
             router_abi = await self.get_abi(settings.dex_router_contract_addr)
             if router_abi is None:
                 router_abi = await self.get(settings.dex_router_abi_url)
-            router = self.w3.eth.contract(
+            return self.w3.eth.contract(
                 address=self.w3.to_checksum_address(
-                    settings.dex_router_contract_addr),
-                abi=router_abi)
-            return router
+                    settings.dex_router_contract_addr
+                ),
+                abi=router_abi,
+            )
         except Exception as error:
             raise error
 
     async def get_name(self):
         try:
             return settings.dex_router_contract_addr[-8:]
         except Exception as error:
@@ -184,16 +185,15 @@
                     'gasPrice': await self.get_gas_price(),
                     'nonce': self.w3.eth.get_transaction_count(
                         self.wallet_address),
                 }
                 transaction = transaction.build_transaction(transaction_params)
             signed = self.w3.eth.account.sign_transaction(
                 transaction, self.private_key)
-            tx_hash = self.w3.eth.send_raw_transaction(signed.rawTransaction)
-            return tx_hash
+            return self.w3.eth.send_raw_transaction(signed.rawTransaction)
         except Exception as error:
             raise error
 
     async def get_abi(self, address):
         if not settings.dex_block_explorer_api:
             self.logger.warning("No block_explorer_api.")
             return None
@@ -231,46 +231,42 @@
         return None
 
     async def get_confirmation(self, order_hash):
         """Returns trade confirmation."""
         try:
             receipt = self.w3.eth.get_transaction(order_hash)
             block = self.w3.eth.get_block(receipt["blockNumber"])
-            trade = {
+            return {
                 "timestamp": block["timestamp"],
                 "id": receipt["blockHash"],
                 "instrument": receipt["to"],
                 "contract": receipt["to"],
                 "amount": receipt["value"],
                 "price": receipt["value"],  # To be determined.
                 "fee": receipt["gas"],
                 "confirmation": (
                     f"➕ Size: {round(receipt['value'], 4)}\n"
                     f"⚫️ Entry: {round(receipt['value'], 4)}\n"
                     f"ℹ️ {receipt['blockHash']}\n"
                     f"🗓️ {block['timestamp']}"
                 ),
             }
-            return trade
         except Exception as error:
             raise error
 
 
     async def get_gas(self, transaction):
         """get gas estimate"""
         gas_limit = self.w3.eth.estimate_gas(transaction) * 1.25
         return int(self.w3.to_wei(gas_limit, 'wei'))
 
 
     async def get_gas_price(self):
         """search get gas price"""
-        gas_price = round(self.w3.from_wei(
-            self.w3.eth.generate_gas_price(),
-            'gwei'), 2)
-        return gas_price
+        return round(self.w3.from_wei(self.w3.eth.generate_gas_price(), 'gwei'), 2)
 
 ### ------✍️ CONTRACT ---------
     async def search_contract(self, token):
         """search a contract function"""
         self.logger.debug("search_contract")
 
         try:
@@ -303,16 +299,15 @@
     async def search_cg_platform(self):
         """search coingecko platform"""
         asset_platforms = self.cg.get_asset_platforms()
         output_dict = next(
             x for x in asset_platforms
             if x["chain_identifier"] == int(self.chain_id)
         )
-        cg_platform = output_dict["id"] or None
-        return cg_platform
+        return output_dict["id"] or None
 
     async def search_cg(self, token):
         """search coingecko"""
         try:
             search_results = self.cg.search(query=token)
             search_dict = search_results['coins']
             filtered_dict = [x for x in search_dict if
@@ -375,18 +370,15 @@
         if not contract:
             return 0
         return contract.functions.balanceOf(self.wallet_address).call()
 
     async def get_token_decimals(self, token_symbol: str) -> Optional[int]:
         """Get token decimals"""
         contract = await self.get_token_contract(token_symbol)
-        if not contract:
-            return 18
-        token_decimals = contract.functions.decimals().call() or 18
-        return token_decimals
+        return 18 if not contract else contract.functions.decimals().call() or 18
 
     async def get_account_balance(self):
         try:
             account_balance = self.w3.eth.get_balance(
                 self.w3.to_checksum_address(self.wallet_address))
             account_balance = self.w3.from_wei(account_balance, 'ether')
             trading_asset_balance = await self.get_trading_asset_balance()
@@ -433,62 +425,63 @@
                 quoter = await self.quoter()
                 sqrtPriceLimitX96 = 0
                 fee = 3000
                 quote = quoter.functions.quoteExactInputSingle(
                     asset_in_address,
                     asset_out_address,
                     fee, amount, sqrtPriceLimitX96).call()
-            return ("🦄 " + quote + " " +
-                    settings.trading_asset)
+            return f"🦄 {quote} {settings.trading_asset}"
         except Exception as e:
             raise e
 
     async def get_approve_uniswap(self, symbol):
         try:
             contract = await self.get_token_contract(symbol)
             approved_amount = self.w3.to_wei(2 ** 64 - 1, 'ether')
             owner_address = self.w3.to_checksum_address(self.wallet_address)
             dex_router_address = self.w3.to_checksum_address(settings.dex_router_contract_addr)
             allowance = contract.functions.allowance(owner_address, dex_router_address).call()
             self.logger.debug("allowance %s", allowance)
             if allowance == 0:
                 approval_tx = contract.functions.approve(dex_router_address, approved_amount)
                 approval_tx_hash = await self.get_sign(approval_tx)
-                approval_receipt = self.w3.eth.wait_for_transaction_receipt(
-                    approval_tx_hash, timeout=120, poll_latency=0.1)
-                return approval_receipt
+                return self.w3.eth.wait_for_transaction_receipt(
+                    approval_tx_hash, timeout=120, poll_latency=0.1
+                )
         except Exception as e:
             raise e
 
 
     async def get_swap_uniswap(self, asset_out_address, asset_in_address, amount):
         try:
             path = [self.w3.to_checksum_address(asset_out_address),
                     self.w3.to_checksum_address(asset_in_address)]
             deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
             router_instance = await self.router()
             min_amount = self.get_quote_uniswap(
                 asset_in_address, asset_out_address, amount)[0]
 
             if self.protocol_type == "uniswap_v2":
-                swap_order = router_instance.functions.swapExactTokensForTokens(
-                    int(amount), int(min_amount), tuple(path),
-                    self.wallet_address, deadline)
-                return swap_order
+                return router_instance.functions.swapExactTokensForTokens(
+                    int(amount),
+                    int(min_amount),
+                    tuple(path),
+                    self.wallet_address,
+                    deadline,
+                )
             elif self.protocol_type == "uniswap_v3":
                 return None
         except Exception as e:
             raise e
 
 # 0️⃣x
     async def get_0x_quote(self, buy_address, sell_address, amount=1):
         try:
             out_amount = self.w3.to_wei(amount, 'ether')
-            url = (settings.dex_0x_url + "/swap/v1/quote?buyToken=" + str(buy_address) +
-                "&sellToken=" + str(sell_address) + "&buyAmount=" + str(out_amount))
+            url = f"{settings.dex_0x_url}/swap/v1/quote?buyToken={str(buy_address)}&sellToken={str(sell_address)}&buyAmount={str(out_amount)}"
             headers = {"0x-api-key": settings.dex_0x_api_key}
             response = await self.get(url, params=None, headers=headers)
             print(response)
             if response:
                 return round(float(response['guaranteedPrice']), 3)
         except Exception as e:
             raise e
```

### Comparing `dxsp-2.6.8/pyproject.toml` & `dxsp-2.6.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.6.8"
+version = "2.6.9"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
 
 [tool.poetry.urls]
 "Changelog" =  "https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/dxsp/discussions"
 "Issues" =  "https://github.com/mraniki/dxsp/issues"
 
 [tool.poetry.dependencies]
-python = "^3.10"
-asyncio = "*"
-dynaconf = "*"
+python = "^3.10.0"
+dynaconf = "^3.1.12"
 web3 = "^6.4.0"
-pycoingecko = "*"
+pycoingecko = "^3.1.0"
 
 [tool.poetry.dev-dependencies]
-python-semantic-release = "*"
-pytest = "*"
+python-semantic-release = "^7.34.3"
+pytest = "^7.0.0"
 pytest-cov = "*"
 pytest-asyncio = "*"
 pytest-mock = "*"
 
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
```

### Comparing `dxsp-2.6.8/PKG-INFO` & `dxsp-2.6.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.6.8
+Version: 2.6.9
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: asyncio
-Requires-Dist: dynaconf
-Requires-Dist: pycoingecko
+Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
+Requires-Dist: pycoingecko (>=3.1.0,<4.0.0)
 Requires-Dist: web3 (>=6.4.0,<7.0.0)
 Project-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/dxsp/issues
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions
 Description-Content-Type: text/markdown
 
 # DXSP (DeX SwaP)
```

