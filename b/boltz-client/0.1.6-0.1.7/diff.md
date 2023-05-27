# Comparing `tmp/boltz_client-0.1.6.tar.gz` & `tmp/boltz_client-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boltz_client-0.1.6.tar", max compression
+gzip compressed data, was "boltz_client-0.1.7.tar", max compression
```

## Comparing `boltz_client-0.1.6.tar` & `boltz_client-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      283 2023-05-27 13:32:13.299822 boltz_client-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-05-27 13:32:13.299822 boltz_client-0.1.6/boltz_client/__init__.py
--rw-r--r--   0        0        0     7017 2023-05-27 13:32:13.299822 boltz_client-0.1.6/boltz_client/boltz.py
--rw-r--r--   0        0        0     6547 2023-05-27 13:32:13.299822 boltz_client-0.1.6/boltz_client/cli.py
--rw-r--r--   0        0        0      375 2023-05-27 13:32:13.299822 boltz_client-0.1.6/boltz_client/helpers.py
--rw-r--r--   0        0        0     5342 2023-05-27 13:32:13.299822 boltz_client-0.1.6/boltz_client/mempool.py
--rw-r--r--   0        0        0     3066 2023-05-27 13:32:13.299822 boltz_client-0.1.6/boltz_client/onchain.py
--rw-r--r--   0        0        0        0 2023-05-27 13:32:13.299822 boltz_client-0.1.6/boltz_client/py.typed
--rw-r--r--   0        0        0     1160 2023-05-27 13:32:13.299822 boltz_client-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 boltz_client-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      283 2023-05-27 15:07:14.934714 boltz_client-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 15:07:14.934714 boltz_client-0.1.7/boltz_client/__init__.py
+-rw-r--r--   0        0        0     7017 2023-05-27 15:07:14.934714 boltz_client-0.1.7/boltz_client/boltz.py
+-rw-r--r--   0        0        0     6547 2023-05-27 15:07:14.934714 boltz_client-0.1.7/boltz_client/cli.py
+-rw-r--r--   0        0        0      375 2023-05-27 15:07:14.934714 boltz_client-0.1.7/boltz_client/helpers.py
+-rw-r--r--   0        0        0     5343 2023-05-27 15:07:14.934714 boltz_client-0.1.7/boltz_client/mempool.py
+-rw-r--r--   0        0        0     3066 2023-05-27 15:07:14.934714 boltz_client-0.1.7/boltz_client/onchain.py
+-rw-r--r--   0        0        0        0 2023-05-27 15:07:14.934714 boltz_client-0.1.7/boltz_client/py.typed
+-rw-r--r--   0        0        0     1160 2023-05-27 15:07:14.938714 boltz_client-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 boltz_client-0.1.7/PKG-INFO
```

### Comparing `boltz_client-0.1.6/boltz_client/boltz.py` & `boltz_client-0.1.7/boltz_client/boltz.py`

 * *Files identical despite different names*

### Comparing `boltz_client-0.1.6/boltz_client/cli.py` & `boltz_client-0.1.7/boltz_client/cli.py`

 * *Files identical despite different names*

### Comparing `boltz_client-0.1.6/boltz_client/mempool.py` & `boltz_client-0.1.7/boltz_client/mempool.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
     def get_fees(self) -> int:
         data = self.request(
             "get",
             f"{self._api_url}/v1/fees/recommended",
             headers={"Content-Type": "application/json"},
         )
-        return int(data["economyFee"])
+        return int(data["halfHourFee"])
 
     def get_blockheight(self) -> int:
         data = self.request(
             "get",
             f"{self._api_url}/blocks/tip/height",
             headers={"Content-Type": "text/plain"},
         )
```

### Comparing `boltz_client-0.1.6/boltz_client/onchain.py` & `boltz_client-0.1.7/boltz_client/onchain.py`

 * *Files identical despite different names*

### Comparing `boltz_client-0.1.6/pyproject.toml` & `boltz_client-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boltz_client"
-version = "0.1.6"
+version = "0.1.7"
 description = "python boltz client"
 license = "MIT"
 authors = ["dni <office@dnilabs.com>"]
 readme = "README.md"
 repository = "https://github.com/dni/boltz-client-python"
 homepage = "https://boltz.exchange"
 packages = [
```

### Comparing `boltz_client-0.1.6/PKG-INFO` & `boltz_client-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boltz-client
-Version: 0.1.6
+Version: 0.1.7
 Summary: python boltz client
 Home-page: https://boltz.exchange
 License: MIT
 Author: dni
 Author-email: office@dnilabs.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

