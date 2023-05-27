# Comparing `tmp/dxsp-2.5.1.tar.gz` & `tmp/dxsp-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.5.1.tar", max compression
+gzip compressed data, was "dxsp-2.5.2.tar", max compression
```

## Comparing `dxsp-2.5.1.tar` & `dxsp-2.5.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-26 20:52:25.218305 dxsp-2.5.1/LICENSE
--rw-r--r--   0        0        0     2439 2023-05-26 20:52:25.218305 dxsp-2.5.1/README.md
--rw-r--r--   0        0        0       86 2023-05-26 20:52:25.966339 dxsp-2.5.1/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-26 20:52:25.218305 dxsp-2.5.1/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-26 20:52:25.218305 dxsp-2.5.1/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-26 20:52:25.218305 dxsp-2.5.1/dxsp/config.py
--rw-r--r--   0        0        0     3500 2023-05-26 20:52:25.218305 dxsp-2.5.1/dxsp/default_settings.toml
--rw-r--r--   0        0        0    20467 2023-05-26 20:52:25.218305 dxsp-2.5.1/dxsp/main.py
--rw-r--r--   0        0        0     1973 2023-05-26 20:52:25.966339 dxsp-2.5.1/pyproject.toml
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-27 10:41:54.117657 dxsp-2.5.2/LICENSE
+-rw-r--r--   0        0        0     2439 2023-05-27 10:41:54.117657 dxsp-2.5.2/README.md
+-rw-r--r--   0        0        0       86 2023-05-27 10:41:54.961660 dxsp-2.5.2/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-27 10:41:54.117657 dxsp-2.5.2/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-27 10:41:54.117657 dxsp-2.5.2/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      390 2023-05-27 10:41:54.117657 dxsp-2.5.2/dxsp/config.py
+-rw-r--r--   0        0        0     3548 2023-05-27 10:41:54.117657 dxsp-2.5.2/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    20785 2023-05-27 10:41:54.117657 dxsp-2.5.2/dxsp/main.py
+-rw-r--r--   0        0        0     1973 2023-05-27 10:41:54.961660 dxsp-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.5.2/PKG-INFO
```

### Comparing `dxsp-2.5.1/LICENSE` & `dxsp-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.5.1/README.md` & `dxsp-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.5.1/dxsp/assets/blockchains.py` & `dxsp-2.5.2/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.5.1/dxsp/default_settings.toml` & `dxsp-2.5.2/dxsp/default_settings.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 loglevel = "INFO"
 headers = {User-Agent= 'Mozilla/5.0'}
 #📝tokenlist
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 #📝trading setup
-trading_quote_ccy = "USDT"
+trading_asset = "USDT"
 trading_risk_amount = 10 # 10% of the position
 dex_trading_slippage = 2 # 2 % slippage
 #user settings
-dex_wallet_address = "" #this is an example
-dex_private_key = "" #this is an example
+dex_wallet_address = "0x1234567890123456789012345678901234567890" #this is an example
+dex_private_key = "0xdeadbeef" #this is an example
 #chain_1 #see below for other chain ids or use https://chainlist.org to overwrite settings
 dex_chain_id = 1
 dex_protocol_type = "uniswap_v2" #0x | 1inch | uniswap_v3
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_block_explorer_url = "https://api.etherscan.io/api?"
 dex_block_explorer_api =  "798437294880920392"  #this is an example
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D" #UNI_V2
```

### Comparing `dxsp-2.5.1/dxsp/main.py` & `dxsp-2.5.2/dxsp/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,33 +29,34 @@
             self.logger.error(f"connectivity failed {e}")
             return
 
         self.protocol_type = settings.dex_protocol_type
         self.chain_id = settings.dex_chain_id
         self.wallet_address = self.w3.to_checksum_address(
             settings.dex_wallet_address)
-        self.account = str(self.chain_id) + " - "+str(self.wallet_address[-8])
+        self.account = str(self.chain_id) + " - "+str(self.wallet_address[-8:])
         self.private_key = settings.dex_private_key
 
         try:
             self.cg = CoinGeckoAPI()
             asset_platforms = self.cg.get_asset_platforms()
             output_dict = next(
-                x for x in asset_platforms if x["chain_identifier"] == int(self.chain_id)
+                x for x in asset_platforms
+                if x["chain_identifier"] == int(self.chain_id)
             )
             self.cg_platform = output_dict["id"]
             self.logger.debug(f"cg_platform {self.cg_platform}")
         except Exception as e:
             self.logger.error(f"CG: {e}")
 
     async def get_quote(self, symbol):
         self.logger.debug("get_quote")
 
         asset_in_address = await self.search_contract(symbol)
-        asset_out_symbol = settings.trading_quote_ccy
+        asset_out_symbol = settings.trading_asset
         asset_out_address = await self.search_contract(asset_out_symbol)
 
         if asset_out_address is None:
             self.logger.warning("No valid contract")
             return
 
         try:
@@ -76,46 +77,54 @@
             return
 
     async def get_swap(
         self, asset_out_symbol: str, asset_in_symbol: str, amount: int
     ) -> None:
         """Main swap function"""
         try:
-            asset_out_address = await self.search_contract(asset_out_symbol)
-            asset_out_contract = await self.get_token_contract(asset_out_symbol)
+            asset_out_address = await self.search_contract(
+                asset_out_symbol)
+            asset_out_contract = await self.get_token_contract(
+                asset_out_symbol)
             if asset_out_contract is None:
                 raise ValueError("No contract identified")
-            asset_out_balance = await self.get_token_balance(asset_out_symbol)
+            asset_out_balance = await self.get_token_balance(
+                asset_out_symbol)
             if asset_out_balance in (0, None):
                 raise ValueError("No Money")
 
             asset_in_address = await self.search_contract(asset_in_symbol)
             if asset_in_address is None:
                 return
 
             asset_out_decimals = asset_out_contract.functions.decimals().call()
             asset_out_amount = amount * 10 ** asset_out_decimals
-            asset_out_amount_converted = self.w3.to_wei(asset_out_amount, "ether")
+            asset_out_amount_converted = self.w3.to_wei(
+                asset_out_amount, "ether")
 
-            order_amount = int(asset_out_amount_converted * (settings.dex_trading_slippage / 100))
+            order_amount = int(asset_out_amount_converted * (
+                settings.dex_trading_slippage / 100))
 
             if await self.get_approve(asset_out_symbol) is None:
                 return
 
             swap_order = None
             if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
-                swap_order = await self.get_swap_uniswap(asset_out_address, asset_in_address, order_amount)
+                swap_order = await self.get_swap_uniswap(
+                    asset_out_address, asset_in_address, order_amount)
             elif self.protocol_type == "0x":
-                swap_order = await self.get_0x_quote(asset_out_address, asset_in_address, order_amount)
+                swap_order = await self.get_0x_quote(
+                    asset_out_address, asset_in_address, order_amount)
                 await self.get_sign(swap_order)
 
             if swap_order:
                 signed_order = await self.get_sign(swap_order)
                 order_hash = str(self.w3.to_hex(signed_order))
-                order_hash_details = self.w3.wait_for_transaction_receipt(order_hash, timeout=120, poll_latency=0.1)
+                order_hash_details = self.w3.wait_for_transaction_receipt(
+                    order_hash, timeout=120, poll_latency=0.1)
                 if order_hash_details["status"] == 1:
                     await self.get_confirmation(order_hash)
 
         except Exception as e:
             self.logger.error("Error in get_swap: %s", e)
             return e
 
@@ -147,31 +156,35 @@
         """Execute swap function."""
         action = order_params.get('action')
         instrument = order_params.get('instrument')
         quantity = order_params.get('quantity', 1)
 
         try:
             if action == "BUY":
-                asset_out_symbol = settings.trading_quote_ccy
+                asset_out_symbol = settings.trading_asset
                 asset_in_symbol = instrument
             else:
                 asset_out_symbol = instrument
-                asset_in_symbol = settings.trading_quote_ccy
+                asset_in_symbol = settings.trading_asset
 
             try:
-                asset_out_contract = await self.get_token_contract(asset_out_symbol)
+                asset_out_contract = await self.get_token_contract(
+                    asset_out_symbol)
                 asset_out_decimals = asset_out_contract.functions.decimals().call() or 18
             except Exception as e:
                 self.logger.error("execute_order decimals: %s", e)
                 asset_out_decimals = 18
 
             asset_out_balance = await self.get_token_balance(asset_out_symbol)
 
             # Amount to risk percentage - DEFAULT OPTION is 10%
-            asset_out_amount = (asset_out_balance / (settings.trading_risk_amount ** asset_out_decimals)) * (float(quantity) / 100)
+            asset_out_amount = (
+                asset_out_balance /
+                (settings.trading_risk_amount ** asset_out_decimals)) * (
+                    float(quantity) / 100)
 
             order = await self.get_swap(
                 asset_out_symbol,
                 asset_in_symbol,
                 asset_out_amount
             )
             if order:
@@ -332,18 +345,20 @@
     async def get_sign(self, transaction):
         try:
             if self.protocol_type in ['uniswap_v2', 'uniswap_v3']:
                 transaction_params = {
                     'from': self.wallet_address,
                     'gas': await self.get_gas(transaction),
                     'gasPrice': await self.get_gas_price(),
-                    'nonce': self.w3.eth.get_transaction_count(self.wallet_address),
+                    'nonce': self.w3.eth.get_transaction_count(
+                        self.wallet_address),
                 }
                 transaction = transaction.build_transaction(transaction_params)
-            signed = self.w3.eth.account.sign_transaction(transaction, settings.dex_private_key)
+            signed = self.w3.eth.account.sign_transaction(
+                transaction, self.private_key)
             tx_hash = self.w3.eth.send_raw_transaction(signed.rawTransaction)
             return tx_hash
         except (ValueError, TypeError, KeyError) as e:
             self.logger.error("Failed to sign transaction: %s", e)
             raise
         except Exception as e:
             self.logger.error("Failed to sign transaction: %s", e)
@@ -370,15 +385,16 @@
             "module": "contract",
             "action": "getabi",
             "address": address,
             "apikey": settings.dex_block_explorer_api
         }
 
         try:
-            resp = await self._get(url=settings.dex_block_explorer_url, params=params)
+            resp = await self._get(
+                url=settings.dex_block_explorer_url, params=params)
             if resp['status'] == "1":
                 self.logger.debug("ABI found %s", resp)
                 return resp["result"]
             else:
                 self.logger.warning("No ABI identified")
                 return None
         except Exception as e:
@@ -397,30 +413,31 @@
 
     async def get_account_balance(self):
         try:
             account_balance = self.w3.eth.get_balance(
                 self.w3.to_checksum_address(self.wallet_address))
             account_balance = self.w3.from_wei(account_balance, 'ether')
             try:
-                trading_quote_ccy_balance = await self.get_trading_quote_ccy_balance()
-                if trading_quote_ccy_balance:
-                    account_balance += f"💵{trading_quote_ccy_balance}"
+                trading_asset_balance = await self.get_trading_asset_balance()
+                if trading_asset_balance:
+                    account_balance += f"💵{trading_asset_balance}"
             except Exception:
                 pass
 
             return round(account_balance, 5)
 
         except Exception as e:
             self.logger.error(f"get_account_balance: {e}")
             return 0
 
-    async def get_trading_quote_ccy_balance(self):
+    async def get_trading_asset_balance(self):
         try:
-            trading_quote_ccy_balance = await self.get_token_balance(settings.trading_quote_ccy)
-            return trading_quote_ccy_balance if trading_quote_ccy_balance else 0
+            trading_asset_balance = await self.get_token_balance(
+                settings.trading_asset)
+            return trading_asset_balance if trading_asset_balance else 0
         except Exception:
             return 0
 
     async def get_account_position(self):
         return 0
 
     async def get_account_margin(self):
@@ -449,30 +466,31 @@
                 sqrtPriceLimitX96 = 0
                 fee = 3000
                 quote = quoter.functions.quoteExactInputSingle(
                     asset_in_address,
                     asset_out_address,
                     fee, amount, sqrtPriceLimitX96).call()
             return ("🦄 " + quote + " " +
-                    settings.trading_quote_ccy)
+                    settings.trading_asset)
         except Exception as e:
             self.logger.error("get_quote_uniswap %s", e)
             return
 
     async def get_approve_uniswap(self, symbol):
         try:
             contract = await self.get_token_contract(symbol)
             approved_amount = self.w3.to_wei(2**64-1, 'ether')
             approval_check = contract.functions.allowance(
                 self.w3.to_checksum_address(self.wallet_address),
                 self.w3.to_checksum_address(settings.dex_router_contract_addr)
             ).call()
             if approval_check == 0:
                 approval_transaction = contract.functions.approve(
-                    self.w3.to_checksum_address(settings.dex_router_contract_addr),
+                    self.w3.to_checksum_address(
+                        settings.dex_router_contract_addr),
                     approved_amount)
                 approval_txHash = await self.get_sign(approval_transaction)
                 approval_txHash_complete = self.w3.eth.wait_for_transaction_receipt(
                     approval_txHash, timeout=120, poll_latency=0.1)
                 return approval_txHash_complete
         except Exception as e:
             self.logger.error("Error in get_approve_uniswap: %s", e)
@@ -480,19 +498,21 @@
 
     async def get_swap_uniswap(self, asset_out_address, asset_in_address, amount):
         try:
             path = [self.w3.to_checksum_address(asset_out_address),
                     self.w3.to_checksum_address(asset_in_address)]
             deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
             router_instance = await self.router()
-            min_amount = self.get_quote_uniswap(asset_in_address, asset_out_address, amount)[0]
+            min_amount = self.get_quote_uniswap(
+                asset_in_address, asset_out_address, amount)[0]
 
             if self.protocol_type == "uniswap_v2":
                 swap_order = router_instance.functions.swapExactTokensForTokens(
-                    int(amount), int(min_amount), tuple(path), self.wallet_address, deadline)
+                    int(amount), int(min_amount), tuple(path),
+                    self.wallet_address, deadline)
                 return swap_order
             elif self.protocol_type == "uniswap_v3":
                 return None
         except Exception as e:
             self.logger.error(f"Error in get_swap_uniswap: {e}")
 
 # 0️⃣x
```

### Comparing `dxsp-2.5.1/pyproject.toml` & `dxsp-2.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.5.1"
+version = "2.5.2"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.5.1/PKG-INFO` & `dxsp-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.5.1
+Version: 2.5.2
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

