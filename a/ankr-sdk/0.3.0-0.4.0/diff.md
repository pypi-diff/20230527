# Comparing `tmp/ankr_sdk-0.3.0.tar.gz` & `tmp/ankr_sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ankr_sdk-0.3.0.tar", max compression
+gzip compressed data, was "ankr_sdk-0.4.0.tar", max compression
```

## Comparing `ankr_sdk-0.3.0.tar` & `ankr_sdk-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-03-31 07:01:13.223743 ankr_sdk-0.3.0/LICENSE
--rw-r--r--   0        0        0     4989 2023-03-31 07:01:13.223743 ankr_sdk-0.3.0/README.md
--rw-r--r--   0        0        0      114 2023-03-31 07:01:13.223743 ankr_sdk-0.3.0/ankr/__init__.py
--rw-r--r--   0        0        0     8730 2023-03-31 07:01:13.223743 ankr_sdk-0.3.0/ankr/advanced_apis.py
--rw-r--r--   0        0        0      215 2023-03-31 07:01:13.223743 ankr_sdk-0.3.0/ankr/exceptions.py
--rw-r--r--   0        0        0     4513 2023-03-31 07:01:13.223743 ankr_sdk-0.3.0/ankr/providers.py
--rw-r--r--   0        0        0     8400 2023-03-31 07:01:13.223743 ankr_sdk-0.3.0/ankr/types.py
--rw-r--r--   0        0        0     3395 2023-03-31 07:01:13.223743 ankr_sdk-0.3.0/ankr/web3.py
--rw-r--r--   0        0        0      757 2023-03-31 07:01:13.227743 ankr_sdk-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5819 1970-01-01 00:00:00.000000 ankr_sdk-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-27 12:12:13.747905 ankr_sdk-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5083 2023-05-27 12:12:13.747905 ankr_sdk-0.4.0/README.md
+-rw-r--r--   0        0        0      114 2023-05-27 12:12:13.747905 ankr_sdk-0.4.0/ankr/__init__.py
+-rw-r--r--   0        0        0     8707 2023-05-27 12:12:13.747905 ankr_sdk-0.4.0/ankr/advanced_apis.py
+-rw-r--r--   0        0        0      215 2023-05-27 12:12:13.747905 ankr_sdk-0.4.0/ankr/exceptions.py
+-rw-r--r--   0        0        0     4487 2023-05-27 12:12:13.747905 ankr_sdk-0.4.0/ankr/providers.py
+-rw-r--r--   0        0        0     8400 2023-05-27 12:12:13.747905 ankr_sdk-0.4.0/ankr/types.py
+-rw-r--r--   0        0        0     3378 2023-05-27 12:12:13.747905 ankr_sdk-0.4.0/ankr/web3.py
+-rw-r--r--   0        0        0      757 2023-05-27 12:12:13.751905 ankr_sdk-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5913 1970-01-01 00:00:00.000000 ankr_sdk-0.4.0/PKG-INFO
```

### Comparing `ankr_sdk-0.3.0/LICENSE` & `ankr_sdk-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ankr_sdk-0.3.0/README.md` & `ankr_sdk-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 
 ```bash
 pip install ankr-sdk
 ```
 
 #### 2. Initialize the SDK
 
+_Note: to use Advanced API for free starting from May 29th, 2023 you have to register on the platform._
+
+Get your individual endpoint here https://www.ankr.com/rpc/advanced-api and provide it to the `AnkrWeb3` class.
+
 ```python3
 from ankr import AnkrWeb3
 
-ankr_w3 = AnkrWeb3()
-
-# Or, if you have an Ankr Protocol premium plan
 ankr_w3 = AnkrWeb3("YOUR-TOKEN")
 ```
 
 #### 3. Use the sdk and call one of the supported methods
 
 #### Node's API
 ```python3
@@ -214,11 +215,10 @@
     decode_tx_data=True,
 )
 ````
 
 
 ### About API keys
 
-For now, Ankr is offering _free_ access to these APIs with no request limits i.e. you don't need an API key at this
-time.
+Ankr is offering _free_ access to Advanced API, however you have to register on Ankr platform to access it.
 
-Later on, these APIs will become a part of Ankr Protocol's [Premium Plan](https://www.ankr.com/protocol/plan/).
+Get your individual API Key here https://www.ankr.com/rpc/advanced-api.
```

### Comparing `ankr_sdk-0.3.0/ankr/advanced_apis.py` & `ankr_sdk-0.4.0/ankr/advanced_apis.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from ankr.exceptions import APIError
 from ankr.providers import MultichainHTTPProvider
 
 
 class AnkrMultichainAPI:
     def __init__(
         self,
-        api_key: Optional[str] = None,
+        api_key: str,
         endpoint_uri: Optional[str] = None,
     ) -> None:
-        self.provider = MultichainHTTPProvider(api_key or "", endpoint_uri)
+        self.provider = MultichainHTTPProvider(api_key, endpoint_uri)
 
 
 class AnkrQueryAPI(AnkrMultichainAPI):
     def get_logs(
         self,
         blockchain: types.BlockchainNames,
         from_block: Optional[types.BlockNumber] = None,
```

### Comparing `ankr_sdk-0.3.0/ankr/providers.py` & `ankr_sdk-0.4.0/ankr/providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,20 @@
 TRequestPaginated = TypeVar("TRequestPaginated", bound=types.RPCRequestPaginated)
 TReplyPaginated = TypeVar("TReplyPaginated", bound=types.RPCReplyPaginated)
 
 
 class MultichainHTTPProvider(HTTPProvider):
     def __init__(
         self,
-        api_key: str = "",
+        api_key: str,
         endpoint_uri: Optional[Union[URI, str]] = None,
         request_kwargs: Optional[Any] = None,
         session: Optional[Any] = None,
     ) -> None:
-        if endpoint_uri is None:
-            endpoint_uri = "https://rpc.ankr.com/multichain/"
+        endpoint_uri = endpoint_uri or "https://rpc.ankr.com/multichain/"
         super().__init__(endpoint_uri + api_key, request_kwargs, session)
 
     def make_request(self, method: RPCEndpoint, params: Any) -> RPCResponse:
         response = super().make_request(method, params)
         if response.get("error"):
             raise APIError(response["error"])
         if "result" not in response:
```

### Comparing `ankr_sdk-0.3.0/ankr/types.py` & `ankr_sdk-0.4.0/ankr/types.py`

 * *Files identical despite different names*

### Comparing `ankr_sdk-0.3.0/ankr/web3.py` & `ankr_sdk-0.4.0/ankr/web3.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     nervos: Eth
     optimism: Eth
     polygon: Eth
     syscoin: Eth
 
     def __init__(
         self,
-        api_key: Optional[str] = None,
+        api_key: str,
         request_kwargs: Optional[Any] = None,
         middlewares: Optional[Sequence[Any]] = None,
         modules: Optional[Dict[str, Union[Type[Module], Sequence[Any]]]] = None,
         external_modules: Optional[
             Dict[str, Union[Type[Module], Sequence[Any]]]
         ] = None,
         ens: ENS = cast(ENS, empty),
```

### Comparing `ankr_sdk-0.3.0/pyproject.toml` & `ankr_sdk-0.4.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ankr-sdk"
-version = "0.3.0"
+version = "0.4.0"
 description = "Compact Python library for interacting with Ankr's Advanced APIs."
 authors = ["Roman Fasakhov <romanfasakhov@ankr.com>"]
 license = "MIT License"
 
 homepage = "https://ankr.com/"
 repository = "https://github.com/Ankr-network/ankr-python-sdk"
 keywords = ["ankr", "sdk", "blockchain", "nft"]
@@ -12,21 +12,21 @@
 include = ["LICENSE"]
 
 packages = [{ include = "ankr" }]
 
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-web3 = "^6.0.0"
-pydantic = "^1.10.7"
+web3 = "^6.4.0"
+pydantic = "^1.10.8"
 pyhumps = "^3.8.0"
-typing-extensions = "^4.5.0"
+typing-extensions = "^4.6.2"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.2"
-mypy = "^1.1.1"
+pytest = "^7.3.1"
+mypy = "^1.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ankr_sdk-0.3.0/PKG-INFO` & `ankr_sdk-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: ankr-sdk
-Version: 0.3.0
+Version: 0.4.0
 Summary: Compact Python library for interacting with Ankr's Advanced APIs.
 Home-page: https://ankr.com/
 License: MIT
 Keywords: ankr,sdk,blockchain,nft
 Author: Roman Fasakhov
 Author-email: romanfasakhov@ankr.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
-Requires-Dist: web3 (>=6.0.0,<7.0.0)
+Requires-Dist: typing-extensions (>=4.6.2,<5.0.0)
+Requires-Dist: web3 (>=6.4.0,<7.0.0)
 Project-URL: Repository, https://github.com/Ankr-network/ankr-python-sdk
 Description-Content-Type: text/markdown
 
 # ⚓️ Ankr Python SDK
 
 Compact Python library for interacting with Ankr's [Advanced APIs](https://www.ankr.com/advanced-api/).
 
@@ -30,20 +30,21 @@
 
 ```bash
 pip install ankr-sdk
 ```
 
 #### 2. Initialize the SDK
 
+_Note: to use Advanced API for free starting from May 29th, 2023 you have to register on the platform._
+
+Get your individual endpoint here https://www.ankr.com/rpc/advanced-api and provide it to the `AnkrWeb3` class.
+
 ```python3
 from ankr import AnkrWeb3
 
-ankr_w3 = AnkrWeb3()
-
-# Or, if you have an Ankr Protocol premium plan
 ankr_w3 = AnkrWeb3("YOUR-TOKEN")
 ```
 
 #### 3. Use the sdk and call one of the supported methods
 
 #### Node's API
 ```python3
@@ -236,12 +237,11 @@
     decode_tx_data=True,
 )
 ````
 
 
 ### About API keys
 
-For now, Ankr is offering _free_ access to these APIs with no request limits i.e. you don't need an API key at this
-time.
+Ankr is offering _free_ access to Advanced API, however you have to register on Ankr platform to access it.
 
-Later on, these APIs will become a part of Ankr Protocol's [Premium Plan](https://www.ankr.com/protocol/plan/).
+Get your individual API Key here https://www.ankr.com/rpc/advanced-api.
```

