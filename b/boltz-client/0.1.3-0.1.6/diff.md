# Comparing `tmp/boltz_client-0.1.3.tar.gz` & `tmp/boltz_client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boltz_client-0.1.3.tar", max compression
+gzip compressed data, was "boltz_client-0.1.6.tar", max compression
```

## Comparing `boltz_client-0.1.3.tar` & `boltz_client-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0      283 2023-01-23 08:41:29.719756 boltz_client-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-01-23 08:41:29.719756 boltz_client-0.1.3/boltz_client/__init__.py
--rw-r--r--   0        0        0     6677 2023-01-23 08:41:29.719756 boltz_client-0.1.3/boltz_client/boltz.py
--rw-r--r--   0        0        0     5776 2023-01-23 08:41:29.719756 boltz_client-0.1.3/boltz_client/cli.py
--rw-r--r--   0        0        0      309 2023-01-23 08:41:29.719756 boltz_client-0.1.3/boltz_client/helpers.py
--rw-r--r--   0        0        0     5477 2023-01-23 08:41:29.719756 boltz_client-0.1.3/boltz_client/mempool.py
--rw-r--r--   0        0        0     2985 2023-01-23 08:41:29.719756 boltz_client-0.1.3/boltz_client/onchain.py
--rw-r--r--   0        0        0        0 2023-01-23 08:41:29.719756 boltz_client-0.1.3/boltz_client/py.typed
--rw-r--r--   0        0        0      931 2023-01-23 08:41:29.719756 boltz_client-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1119 1970-01-01 00:00:00.000000 boltz_client-0.1.3/setup.py
--rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 boltz_client-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      283 2023-05-27 13:32:13.299822 boltz_client-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 13:32:13.299822 boltz_client-0.1.6/boltz_client/__init__.py
+-rw-r--r--   0        0        0     7017 2023-05-27 13:32:13.299822 boltz_client-0.1.6/boltz_client/boltz.py
+-rw-r--r--   0        0        0     6547 2023-05-27 13:32:13.299822 boltz_client-0.1.6/boltz_client/cli.py
+-rw-r--r--   0        0        0      375 2023-05-27 13:32:13.299822 boltz_client-0.1.6/boltz_client/helpers.py
+-rw-r--r--   0        0        0     5342 2023-05-27 13:32:13.299822 boltz_client-0.1.6/boltz_client/mempool.py
+-rw-r--r--   0        0        0     3066 2023-05-27 13:32:13.299822 boltz_client-0.1.6/boltz_client/onchain.py
+-rw-r--r--   0        0        0        0 2023-05-27 13:32:13.299822 boltz_client-0.1.6/boltz_client/py.typed
+-rw-r--r--   0        0        0     1160 2023-05-27 13:32:13.299822 boltz_client-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 boltz_client-0.1.6/PKG-INFO
```

### Comparing `boltz_client-0.1.3/boltz_client/boltz.py` & `boltz_client-0.1.6/boltz_client/boltz.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+""" boltz_client main module """
+
 from dataclasses import dataclass
 from typing import Optional
 
 import httpx
 
 from .helpers import req_wrap
 from .mempool import MempoolClient
@@ -74,20 +76,20 @@
         self.mempool = MempoolClient(self._cfg.mempool_url, self._cfg.mempool_ws_url)
 
     def request(self, funcname, *args, **kwargs) -> dict:
         try:
             return req_wrap(funcname, *args, **kwargs)
         except httpx.RequestError as exc:
             msg = f"unreachable: {exc.request.url!r}."
-            raise BoltzApiException(f"boltz api connection error: {msg}")
+            raise BoltzApiException(f"boltz api connection error: {msg}") from exc
         except httpx.HTTPStatusError as exc:
             if exc.response.status_code == 404:
-                raise BoltzNotFoundException(exc.response.json()["error"])
+                raise BoltzNotFoundException(exc.response.json()["error"]) from exc
             msg = f"{exc.response.status_code} while requesting {exc.request.url!r}. message: {exc.response.json()['error']}"
-            raise BoltzApiException(f"boltz api status error: {msg}")
+            raise BoltzApiException(f"boltz api status error: {msg}") from exc
 
     def check_version(self):
         return self.request(
             "get",
             f"{self._cfg.api_url}/version",
             headers={"Content-Type": "application/json"},
         )
@@ -102,15 +104,15 @@
         limits = pair["limits"]
         fees = pair["fees"]
         self.limit_maximal = limits["maximal"]
         self.limit_minimal = limits["minimal"]
         self.fee_percentage = fees["percentage"]
 
     def check_limits(self, amount: int) -> None:
-        valid = amount >= self.limit_minimal and amount <= self.limit_maximal
+        valid = self.limit_minimal <= amount <= self.limit_maximal
         if not valid:
             msg = f"Boltz - swap not in boltz limits, amount: {amount}, min: {self.limit_minimal}, max: {self.limit_maximal}"
             raise BoltzLimitException(msg)
 
     def swap_status(self, boltz_id: str) -> BoltzSwapStatusResponse:
         data = self.request(
             "post",
@@ -135,47 +137,50 @@
         zeroconf: bool = False,
     ):
         lockup_tx = await self.mempool.get_tx_from_address(lockup_address)
 
         if not zeroconf and lockup_tx.status != "confirmed":
             await self.mempool.wait_for_tx_confirmed(lockup_tx.txid)
 
-        txid, tx = create_claim_tx(
+        txid, transaction = create_claim_tx(
             lockup_tx=lockup_tx,
             receive_address=receive_address,
             privkey_wif=privkey_wif,
             redeem_script_hex=redeem_script_hex,
             preimage_hex=preimage_hex,
+            fees=self.mempool.get_fee_estimation(),
         )
 
-        self.mempool.send_onchain_tx(tx)
+        self.mempool.send_onchain_tx(transaction)
         return txid
 
     async def refund_swap(
         self,
         privkey_wif: str,
         lockup_address: str,
         receive_address: str,
         redeem_script_hex: str,
         timeout_block_height: int,
     ) -> str:
         self.mempool.check_block_height(timeout_block_height)
         lockup_tx = await self.mempool.get_tx_from_address(lockup_address)
-        txid, tx = create_refund_tx(
+        txid, transaction = create_refund_tx(
             lockup_tx=lockup_tx,
             privkey_wif=privkey_wif,
             receive_address=receive_address,
             redeem_script_hex=redeem_script_hex,
             timeout_block_height=timeout_block_height,
+            fees=self.mempool.get_fee_estimation(),
         )
 
-        self.mempool.send_onchain_tx(tx)
+        self.mempool.send_onchain_tx(transaction)
         return txid
 
     def create_swap(self, payment_request: str) -> tuple[str, BoltzSwapResponse]:
+        """create swap and return private key and boltz response"""
         refund_privkey_wif, refund_pubkey_hex = create_key_pair(self._cfg.network)
         data = self.request(
             "post",
             f"{self._cfg.api_url}/createswap",
             json={
                 "type": "submarine",
                 "pairId": "BTC/BTC",
@@ -187,14 +192,15 @@
             headers={"Content-Type": "application/json"},
         )
         return refund_privkey_wif, BoltzSwapResponse(**data)
 
     def create_reverse_swap(
         self, amount: int = 0
     ) -> tuple[str, str, BoltzReverseSwapResponse]:
+        """create reverse swap and return privkey, preimage and boltz response"""
         self.check_limits(amount)
         claim_privkey_wif, claim_pubkey_hex = create_key_pair(self._cfg.network)
         preimage_hex, preimage_hash = create_preimage()
         data = self.request(
             "post",
             f"{self._cfg.api_url}/createswap",
             json={
```

### Comparing `boltz_client-0.1.3/boltz_client/cli.py` & `boltz_client-0.1.6/boltz_client/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+""" boltz_client CLI """
+
 import asyncio
 import sys
 
 import click
 
 from boltz_client.boltz import BoltzClient, BoltzConfig
 
@@ -40,14 +42,23 @@
     click.echo()
     click.echo(f"refund privkey in wif: {refund_privkey_wif}")
     click.echo(f"redeem_script_hex: {swap.redeemScript}")
     click.echo()
     click.echo(f"onchain address: {swap.address}")
     click.echo(f"expected amount: {swap.expectedAmount}")
     click.echo(f"bip21 address: {swap.bip21}")
+    click.echo(f"timeout block height: {swap.timeoutBlockHeight}")
+
+    click.echo()
+    click.echo("run this command if you need to refund:")
+    click.echo("CHANGE YOUR_RECEIVEADDRESS to your onchain address!!!")
+    click.echo(
+        f"boltz refund-swap {refund_privkey_wif} {swap.address} YOUR_RECEIVEADDRESS "
+        f"{swap.redeemScript} {swap.timeoutBlockHeight}"
+    )
 
 
 @click.command()
 @click.argument("privkey_wif", type=str)
 @click.argument("lockup_address", type=str)
 @click.argument("receive_address", type=str)
 @click.argument("redeem_script_hex", type=str)
@@ -68,15 +79,15 @@
             privkey_wif,
             lockup_address,
             receive_address,
             redeem_script_hex,
             timeout_block_height,
         )
     )
-    click.echo(f"swap refunded!")
+    click.echo("swap refunded!")
     click.echo(f"TXID: {txid}")
 
 
 @click.command()
 @click.argument("sats", type=int)
 def create_reverse_swap(sats: int):
     """
@@ -96,14 +107,22 @@
     click.echo(
         f"mempool.space url: {config.mempool_url.replace('/api', '')}/address/{swap.lockupAddress}"
     )
     click.echo()
     click.echo("invoice:")
     click.echo(swap.invoice)
 
+    click.echo()
+    click.echo("run this command after you see the lockup transaction:")
+    click.echo("CHANGE YOUR_RECEIVEADDRESS to your onchain address!!!")
+    click.echo(
+        f"boltz claim-reverse-swap {swap.lockupAddress} YOUR_RECEIVEADDRESS "
+        f"{claim_privkey_wif} {preimage_hex} {swap.redeemScript}"
+    )
+
 
 @click.command()
 @click.argument("receive_address", type=str)
 @click.argument("sats", type=int)
 @click.argument("zeroconf", type=bool, default=False)
 def create_reverse_swap_and_claim(
     receive_address: str, sats: int, zeroconf: bool = False
@@ -139,15 +158,15 @@
             claim_privkey_wif,
             preimage_hex,
             swap.redeemScript,
             zeroconf,
         )
     )
 
-    click.echo(f"reverse swap claimed!")
+    click.echo("reverse swap claimed!")
     click.echo(f"TXID: {txid}")
 
 
 @click.command()
 @click.argument("lockup_address", type=str)
 @click.argument("receive_address", type=str)
 @click.argument("privkey_wif", type=str)
@@ -174,33 +193,34 @@
             privkey_wif,
             preimage_hex,
             redeem_script_hex,
             zeroconf,
         )
     )
 
-    click.echo(f"reverse swap claimed!")
+    click.echo("reverse swap claimed!")
     click.echo(f"TXID: {txid}")
 
 
 @click.command()
-@click.argument("id", type=str)
-def swap_status(id):
+@click.argument("swap_id", type=str)
+def swap_status(swap_id):
     """
     get swap status
     retrieves the status of your boltz swap from the api
 
     ID is the id of your boltz swap
     """
     client = BoltzClient(config)
-    data = client.swap_status(id)
+    data = client.swap_status(swap_id)
     click.echo(data)
 
 
 def main():
+    """main function"""
     command_group.add_command(swap_status)
     command_group.add_command(create_swap)
     command_group.add_command(refund_swap)
     command_group.add_command(create_reverse_swap)
     command_group.add_command(create_reverse_swap_and_claim)
     command_group.add_command(claim_reverse_swap)
     command_group()
```

### Comparing `boltz_client-0.1.3/boltz_client/mempool.py` & `boltz_client-0.1.6/boltz_client/mempool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+""" boltz_client mempool module """
+
 import asyncio
 import json
 from dataclasses import dataclass
 from typing import Optional
 
 import httpx
-import websockets
+from websockets.client import connect
+from websockets.exceptions import ConnectionClosed
 
 from .helpers import req_wrap
 
 
 @dataclass
 class LockupData:
     status: str
@@ -33,35 +36,33 @@
         self.get_blockheight()
 
     def request(self, funcname, *args, **kwargs) -> dict:
         try:
             return req_wrap(funcname, *args, **kwargs)
         except httpx.RequestError as exc:
             msg = f"unreachable: {exc.request.url!r}."
-            raise MempoolApiException(f"mempool api connection error: {msg}")
+            raise MempoolApiException(f"mempool api connection error: {msg}") from exc
         except httpx.HTTPStatusError as exc:
             msg = f"{exc.response.status_code} while requesting {exc.request.url!r}. message: {exc.response.text}"
-            raise MempoolApiException(f"mempool api status error: {msg}")
+            raise MempoolApiException(f"mempool api status error: {msg}") from exc
 
     async def wait_for_websocket_message(self, send, message_key):
-        async for websocket in websockets.connect(self._ws_url):  # type: ignore
+        async for websocket in connect(self._ws_url):
             try:
-                # await websocket.send(json.dumps({"action": "init"}))
-                # await websocket.send(json.dumps({"action": "want", "data": ["blocks", "mempool-blocks"]}))
                 await websocket.send(json.dumps({"action": "want", "data": ["blocks"]}))
                 await websocket.send(json.dumps(send))
                 async for raw in websocket:
                     message = json.loads(raw)
                     if message_key in message:
                         return message.get(message_key)
-            except websockets.ConnectionClosed:  # type: ignore
+            except ConnectionClosed:
                 continue
 
     async def wait_for_one_websocket_message(self, send):
-        async with websockets.connect(self._ws_url) as websocket:  # type: ignore
+        async with connect(self._ws_url) as websocket:
             await websocket.send(
                 json.dumps({"action": "want", "data": ["blocks", "mempool-blocks"]})
             )
             await websocket.send(json.dumps(send))
             raw = await asyncio.wait_for(websocket.recv(), timeout=10)
             return json.loads(raw) if raw else None
```

### Comparing `boltz_client-0.1.3/boltz_client/onchain.py` & `boltz_client-0.1.6/boltz_client/onchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+""" boltz_client onchain module """
+
 import os
 from hashlib import sha256
 from typing import Optional
 
 from embit import ec, script
 from embit.networks import NETWORKS
 from embit.transaction import SIGHASH, Transaction, TransactionInput, TransactionOutput
@@ -25,52 +27,56 @@
 
 def create_refund_tx(
     privkey_wif: str,
     receive_address: str,
     redeem_script_hex: str,
     timeout_block_height: int,
     lockup_tx: LockupData,
+    fees: int,
 ) -> tuple[str, str]:
     # encrypt redeemscript to script_sig
     rs = bytes([34]) + bytes([0]) + bytes([32])
     rs += sha256(bytes.fromhex(redeem_script_hex)).digest()
     script_sig = script.Script(data=rs)
     return create_onchain_tx(
         sequence=0xFFFFFFFE,
         redeem_script_hex=redeem_script_hex,
         privkey_wif=privkey_wif,
         lockup_tx=lockup_tx,
         receive_address=receive_address,
         timeout_block_height=timeout_block_height,
         script_sig=script_sig,
+        fees=fees,
     )
 
 
 def create_claim_tx(
     preimage_hex: str,
     privkey_wif: str,
     receive_address: str,
     redeem_script_hex: str,
     lockup_tx: LockupData,
+    fees: int,
 ) -> tuple[str, str]:
     return create_onchain_tx(
         preimage_hex=preimage_hex,
         lockup_tx=lockup_tx,
         receive_address=receive_address,
         privkey_wif=privkey_wif,
         redeem_script_hex=redeem_script_hex,
+        fees=fees,
     )
 
 
 def create_onchain_tx(
     lockup_tx: LockupData,
     receive_address: str,
     privkey_wif: str,
     redeem_script_hex: str,
-    fees: int = 1000,
+    fees: int,
     sequence: int = 0xFFFFFFFF,
     timeout_block_height: int = 0,
     preimage_hex: str = "",
     script_sig: Optional[script.Script] = None,
 ) -> tuple[str, str]:
 
     vin = TransactionInput(
@@ -84,19 +90,20 @@
     if timeout_block_height > 0:
         tx.locktime = timeout_block_height
 
     if script_sig:
         tx.vin[0].script_sig = script_sig
 
     # hashing redeemscript
-    s = script.Script(data=bytes.fromhex(redeem_script_hex))
-    h = tx.sighash_segwit(0, s, lockup_tx.vout_amount)
+
+    h = tx.sighash_segwit(
+        0, script.Script(data=bytes.fromhex(redeem_script_hex)), lockup_tx.vout_amount
+    )
 
     # sign the redeemscript hash
-    privkey = ec.PrivateKey.from_wif(privkey_wif)
-    sig = privkey.sign(h).serialize() + bytes([SIGHASH.ALL])
+    sig = ec.PrivateKey.from_wif(privkey_wif).sign(h).serialize() + bytes([SIGHASH.ALL])
 
     # put the witness into the input
     witness_items = [sig, bytes.fromhex(preimage_hex), bytes.fromhex(redeem_script_hex)]
     tx.vin[0].witness = script.Witness(items=witness_items)
 
     return bytes.hex(tx.txid()), bytes.hex(tx.serialize())
```

### Comparing `boltz_client-0.1.3/pyproject.toml` & `boltz_client-0.1.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 [tool.poetry]
 name = "boltz_client"
-version = "0.1.3"
+version = "0.1.6"
 description = "python boltz client"
 license = "MIT"
 authors = ["dni <office@dnilabs.com>"]
 readme = "README.md"
 repository = "https://github.com/dni/boltz-client-python"
 homepage = "https://boltz.exchange"
 packages = [
   {include = "boltz_client"},
   {include = "boltz_client/py.typed"},
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10 | ^3.9 | ^3.8 | ^3.7"
+python = "^3.10 | ^3.9"
 httpx = ">=0.23"
 embit = ">=0.4"
 click = ">=8"
 websockets = ">=10"
 
 [tool.poetry.group.dev.dependencies]
 pytest-asyncio = "^0.20.3"
 isort = "^5.10.1"
 pytest = "^7.1.2"
 black = "^22.6.0"
 mypy = "^0.971"
+pylint = "^2.15.10"
+flake8 = "^6.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 boltz = "boltz_client.cli:main"
@@ -41,7 +43,19 @@
 files = "boltz_client"
 
 [tool.pytest.ini_options]
 log_level = "INFO"
 testpaths = [
   "tests"
 ]
+
+[tool.pylint.format]
+max-line-length = 125
+
+[tool.pylint.'MESSAGES CONTROL']
+disable = [
+  "fixme",
+  "invalid-name",
+  "too-many-arguments",
+  "missing-function-docstring",
+  "missing-class-docstring"
+]
```

### Comparing `boltz_client-0.1.3/PKG-INFO` & `boltz_client-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: boltz-client
-Version: 0.1.3
+Version: 0.1.6
 Summary: python boltz client
 Home-page: https://boltz.exchange
 License: MIT
 Author: dni
 Author-email: office@dnilabs.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8)
 Requires-Dist: embit (>=0.4)
 Requires-Dist: httpx (>=0.23)
 Requires-Dist: websockets (>=10)
```

