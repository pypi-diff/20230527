# Comparing `tmp/duckduckgo_search-3.5.0.tar.gz` & `tmp/duckduckgo_search-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-3.5.0.tar", last modified: Fri May 26 21:24:18 2023, max compression
+gzip compressed data, was "duckduckgo_search-3.6.0.tar", last modified: Sat May 27 20:49:17 2023, max compression
```

## Comparing `duckduckgo_search-3.5.0.tar` & `duckduckgo_search-3.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:24:18.935401 duckduckgo_search-3.5.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-05-26 21:24:18.935401 duckduckgo_search-3.5.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    14016 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:24:18.935401 duckduckgo_search-3.5.0/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16092 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/duckduckgo_search/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/duckduckgo_search/duckduckgo_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:24:18.935401 duckduckgo_search-3.5.0/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-05-26 21:24:18.000000 duckduckgo_search-3.5.0/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-26 21:24:18.000000 duckduckgo_search-3.5.0/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:24:18.000000 duckduckgo_search-3.5.0/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 21:24:18.000000 duckduckgo_search-3.5.0/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 21:24:18.000000 duckduckgo_search-3.5.0/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 21:24:18.000000 duckduckgo_search-3.5.0/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 21:24:18.935401 duckduckgo_search-3.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:24:18.935401 duckduckgo_search-3.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-26 21:23:58.000000 duckduckgo_search-3.5.0/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:49:17.845033 duckduckgo_search-3.6.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15018 2023-05-27 20:49:17.845033 duckduckgo_search-3.6.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13903 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:49:17.845033 duckduckgo_search-3.6.0/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16030 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/duckduckgo_search/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30492 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/duckduckgo_search/duckduckgo_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:49:17.845033 duckduckgo_search-3.6.0/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15018 2023-05-27 20:49:17.000000 duckduckgo_search-3.6.0/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-27 20:49:17.000000 duckduckgo_search-3.6.0/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 20:49:17.000000 duckduckgo_search-3.6.0/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 20:49:17.000000 duckduckgo_search-3.6.0/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-27 20:49:17.000000 duckduckgo_search-3.6.0/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-27 20:49:17.000000 duckduckgo_search-3.6.0/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 20:49:17.845033 duckduckgo_search-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:49:17.845033 duckduckgo_search-3.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-3.5.0/LICENSE.md` & `duckduckgo_search-3.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.5.0/PKG-INFO` & `duckduckgo_search-3.6.0/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: duckduckgo_search
-Version: 3.5.0
+Name: duckduckgo-search
+Version: 3.6.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,14 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ![Python >= 3.7](https://img.shields.io/badge/python->=3.7-red.svg) [![](https://badgen.net/github/release/deedy5/duckduckgo_search)](https://github.com/deedy5/duckduckgo_search/releases) [![](https://badge.fury.io/py/duckduckgo-search.svg)](https://pypi.org/project/duckduckgo-search)
 # Duckduckgo_search<a name="TOP"></a>
-***_Attention. Versions before v2.9.4 no longer work as of May 12, 2023!_***
 
 Search for words, documents, images, videos, news, maps and text translation using the DuckDuckGo.com search engine. Downloading files and images to a local hard drive.
 
 ## Table of Contents
 * [Install](#install)
 * [CLI version](#cli-version)
 * [Duckduckgo search operators](#duckduckgo-search-operators)
@@ -162,52 +161,50 @@
 </details>
 
 [Go To TOP](#TOP)
 
 ## Using proxy
 If you send too many requests the site blocks ip for up to one minute and DDGS will raise an exception 
 `requests.exceptions.HTTPError: 418 Client Error:  for url: https://duckduckgo.com/`.
-In this case, you need repeat again after a while or to use a proxy. 
+In this case, you need repeat again after a while or to use a proxy ([httpx documentation](https://www.python-httpx.org/advanced)).
 You can set a timeout if the proxy takes a long time to respond (default timeout=10).
 
 *1. The easiest way. Launch the Tor Browser*
 ```python3
 from duckduckgo_search import DDGS
 
 proxies = {
-    "http": "socks5h://localhost:9150",
-    "https": "socks5h://localhost:9150"
+    "all://": "socks5h://localhost:9150",
 }
 ddgs_text_gen = DDGS(proxies=proxies, timeout=20).text("something you need")
 for r in ddgs_text_gen:
-	print(r)
+    print(r)
 ```
 *2. Use any proxy server* (*example with [iproyal residential proxies](https://iproyal.com?r=residential_proxies)*)
 ```python3
 from duckduckgo_search import DDGS
 
 proxies = {
-    "http": "socks5h://user:password@geo.iproyal.com:32325",
-    "https": "socks5h://user:password@geo.iproyal.com:32325",
-    "no_proxy": "localhost,127.0.0.1",
+    "all://": "https://user:password@geo.iproyal.com:32325",
 }
 ddgs_text_gen = DDGS(proxies=proxies, timeout=20).text("something you need")
 for r in ddgs_text_gen:
-	print(r)
+    print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 1. text() - text search by by duckduckgo.com
 ```python
 def text(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
+    backend: str = "api",
 ) -> Iterator[dict]:
     """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
@@ -226,28 +223,28 @@
 from duckduckgo_search import DDGS
 
 ddgs = DDGS()
 
 keywords = 'live free or die'
 ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
-	print(r)
+    print(r)
 
 # Searching for pdf files
 keywords = 'russia filetype:pdf'
 ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
-	print(r)
+    print(r)
 
 # Using lite backend and limit the number of results to 10
 from itertools import islice
 
 ddgs_text_gen = DDGS().text("notes from a dead house", backend="lite")
 for r in islice(ddgs_text_gen, 10):
-	print(r)
+    print(r)
 ```
 
 
 [Go To TOP](#TOP)
 
 ## 2. answers() - instant answers by duckduckgo.com
```

### Comparing `duckduckgo_search-3.5.0/README.md` & `duckduckgo_search-3.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 ![Python >= 3.7](https://img.shields.io/badge/python->=3.7-red.svg) [![](https://badgen.net/github/release/deedy5/duckduckgo_search)](https://github.com/deedy5/duckduckgo_search/releases) [![](https://badge.fury.io/py/duckduckgo-search.svg)](https://pypi.org/project/duckduckgo-search)
 # Duckduckgo_search<a name="TOP"></a>
-***_Attention. Versions before v2.9.4 no longer work as of May 12, 2023!_***
 
 Search for words, documents, images, videos, news, maps and text translation using the DuckDuckGo.com search engine. Downloading files and images to a local hard drive.
 
 ## Table of Contents
 * [Install](#install)
 * [CLI version](#cli-version)
 * [Duckduckgo search operators](#duckduckgo-search-operators)
@@ -137,52 +136,50 @@
 </details>
 
 [Go To TOP](#TOP)
 
 ## Using proxy
 If you send too many requests the site blocks ip for up to one minute and DDGS will raise an exception 
 `requests.exceptions.HTTPError: 418 Client Error:  for url: https://duckduckgo.com/`.
-In this case, you need repeat again after a while or to use a proxy. 
+In this case, you need repeat again after a while or to use a proxy ([httpx documentation](https://www.python-httpx.org/advanced)).
 You can set a timeout if the proxy takes a long time to respond (default timeout=10).
 
 *1. The easiest way. Launch the Tor Browser*
 ```python3
 from duckduckgo_search import DDGS
 
 proxies = {
-    "http": "socks5h://localhost:9150",
-    "https": "socks5h://localhost:9150"
+    "all://": "socks5h://localhost:9150",
 }
 ddgs_text_gen = DDGS(proxies=proxies, timeout=20).text("something you need")
 for r in ddgs_text_gen:
-	print(r)
+    print(r)
 ```
 *2. Use any proxy server* (*example with [iproyal residential proxies](https://iproyal.com?r=residential_proxies)*)
 ```python3
 from duckduckgo_search import DDGS
 
 proxies = {
-    "http": "socks5h://user:password@geo.iproyal.com:32325",
-    "https": "socks5h://user:password@geo.iproyal.com:32325",
-    "no_proxy": "localhost,127.0.0.1",
+    "all://": "https://user:password@geo.iproyal.com:32325",
 }
 ddgs_text_gen = DDGS(proxies=proxies, timeout=20).text("something you need")
 for r in ddgs_text_gen:
-	print(r)
+    print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 1. text() - text search by by duckduckgo.com
 ```python
 def text(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
+    backend: str = "api",
 ) -> Iterator[dict]:
     """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
@@ -201,28 +198,28 @@
 from duckduckgo_search import DDGS
 
 ddgs = DDGS()
 
 keywords = 'live free or die'
 ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
-	print(r)
+    print(r)
 
 # Searching for pdf files
 keywords = 'russia filetype:pdf'
 ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
-	print(r)
+    print(r)
 
 # Using lite backend and limit the number of results to 10
 from itertools import islice
 
 ddgs_text_gen = DDGS().text("notes from a dead house", backend="lite")
 for r in islice(ddgs_text_gen, 10):
-	print(r)
+    print(r)
 ```
 
 
 [Go To TOP](#TOP)
 
 ## 2. answers() - instant answers by duckduckgo.com
```

### Comparing `duckduckgo_search-3.5.0/duckduckgo_search/__init__.py` & `duckduckgo_search-3.6.0/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.5.0/duckduckgo_search/cli.py` & `duckduckgo_search-3.6.0/duckduckgo_search/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from datetime import datetime
 from shutil import copyfileobj
 from urllib.parse import unquote
 
 import click
-import requests
+import httpx
 
 # isort: off
 from .duckduckgo_search import DDGS
 from .version import __version__
 
 # isort: on
 
@@ -88,20 +88,19 @@
 
 
 def download_file(url, dir_path, filename):
     headers = {
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:102.0) Gecko/20100101 Firefox/102.0",
     }
     try:
-        with requests.get(url, headers=headers, stream=True, timeout=10) as resp:
-            resp.raise_for_status()
-            resp.raw.decode_content = True
-            with open(os.path.join(dir_path, filename), "wb") as file:
-                copyfileobj(resp.raw, file)
-            logger.info(f"File downloaded {url}")
+        with open(os.path.join(dir_path, filename), "wb") as file:
+            with httpx.stream("GET", url, headers=headers) as resp:
+                for chunk in resp.iter_bytes():
+                    file.write(chunk)
+        logger.info(f"File downloaded {url}")
     except Exception as ex:
         logger.debug(f"download_file url={url} {type(ex).__name__} {ex}")
 
 
 def download_results(keywords, results, images=False):
     if images:
         path = f"images_{keywords}_{datetime.now():%Y%m%d_%H%M%S}"
```

### Comparing `duckduckgo_search-3.5.0/duckduckgo_search/compat.py` & `duckduckgo_search-3.6.0/duckduckgo_search/compat.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.5.0/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-3.6.0/duckduckgo_search/duckduckgo_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from decimal import Decimal
 from html import unescape
 from itertools import cycle
 from time import sleep
 from typing import Deque, Dict, Iterator, Optional, Set
 from urllib.parse import unquote
 
+import httpx
 import requests
 from lxml import html
-from requests.models import Response
 
 logger = logging.getLogger(__name__)
 
 HEADERS = {
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:102.0) Gecko/20100101 Firefox/102.0",
     "Referer": "https://duckduckgo.com/",
 }
@@ -42,30 +42,38 @@
 
 class DDGS:
     """DuckDuckgo_search class to get search results from duckduckgo.com"""
 
     def __init__(
         self,
         headers: Optional[Dict[str, str]] = None,
-        proxies: Optional[Dict[str, str]] = None,
+        proxies: Optional[Dict] = None,
         timeout: int = 10,
     ) -> None:
-        self._session = requests.Session()
-        self._session.headers.update(headers if headers else HEADERS)
-        self._session.proxies.update(proxies if proxies else {})
-        self._timeout = timeout
+        self._client = httpx.Client(
+            headers=headers if headers else HEADERS,
+            proxies=proxies,
+            timeout=timeout,
+            http2=True,
+        )
+
+    def __enter__(self):
+        return self
 
-    def _get_url(self, method: str, url: str, **kwargs) -> Optional[Response]:
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self._client.close()
+
+    def _get_url(
+        self, method: str, url: str, **kwargs
+    ) -> Optional[httpx._models.Response]:
         for i in range(3):
             try:
-                resp = self._session.request(
-                    method, url, timeout=self._timeout, **kwargs
-                )
-                if self._is_500_in_url(resp.url) or resp.status_code == 202:
-                    raise requests.HTTPError
+                resp = self._client.request(method, url, **kwargs)
+                if self._is_500_in_url(str(resp.url)) or resp.status_code == 202:
+                    raise httpx._exceptions.HTTPError("")
                 resp.raise_for_status()
                 if resp.status_code == 200:
                     return resp
             except Exception as ex:
                 logger.warning(f"_get_url() {url} {type(ex).__name__} {ex}")
                 if i >= 2 or "418" in str(ex):
                     raise ex
@@ -656,15 +664,17 @@
 
         assert keywords, "keywords is mandatory"
 
         payload = {
             "q": keywords,
             "kl": region,
         }
-        resp = self._get_url("GET", "https://duckduckgo.com/ac", params=payload)
+        resp = self._get_url(
+            "GET", "https://duckduckgo.com/ac", params=payload, follow_redirects=True
+        )
         if resp is None:
             return None
         try:
             page_data = resp.json()
             for r in page_data:
                 yield r
         except Exception:
@@ -848,16 +858,15 @@
         payload = {
             "vqd": vqd,
             "query": "translate",
             "from": from_,
             "to": to,
         }
 
-        resp = self._get_url(
-            "POST",
+        resp = requests.post(
             "https://duckduckgo.com/translation.js",
             params=payload,
             data=keywords.encode(),
         )
         if resp is None:
             return None
         try:
```

### Comparing `duckduckgo_search-3.5.0/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-3.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: duckduckgo-search
-Version: 3.5.0
+Name: duckduckgo_search
+Version: 3.6.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,14 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ![Python >= 3.7](https://img.shields.io/badge/python->=3.7-red.svg) [![](https://badgen.net/github/release/deedy5/duckduckgo_search)](https://github.com/deedy5/duckduckgo_search/releases) [![](https://badge.fury.io/py/duckduckgo-search.svg)](https://pypi.org/project/duckduckgo-search)
 # Duckduckgo_search<a name="TOP"></a>
-***_Attention. Versions before v2.9.4 no longer work as of May 12, 2023!_***
 
 Search for words, documents, images, videos, news, maps and text translation using the DuckDuckGo.com search engine. Downloading files and images to a local hard drive.
 
 ## Table of Contents
 * [Install](#install)
 * [CLI version](#cli-version)
 * [Duckduckgo search operators](#duckduckgo-search-operators)
@@ -162,52 +161,50 @@
 </details>
 
 [Go To TOP](#TOP)
 
 ## Using proxy
 If you send too many requests the site blocks ip for up to one minute and DDGS will raise an exception 
 `requests.exceptions.HTTPError: 418 Client Error:  for url: https://duckduckgo.com/`.
-In this case, you need repeat again after a while or to use a proxy. 
+In this case, you need repeat again after a while or to use a proxy ([httpx documentation](https://www.python-httpx.org/advanced)).
 You can set a timeout if the proxy takes a long time to respond (default timeout=10).
 
 *1. The easiest way. Launch the Tor Browser*
 ```python3
 from duckduckgo_search import DDGS
 
 proxies = {
-    "http": "socks5h://localhost:9150",
-    "https": "socks5h://localhost:9150"
+    "all://": "socks5h://localhost:9150",
 }
 ddgs_text_gen = DDGS(proxies=proxies, timeout=20).text("something you need")
 for r in ddgs_text_gen:
-	print(r)
+    print(r)
 ```
 *2. Use any proxy server* (*example with [iproyal residential proxies](https://iproyal.com?r=residential_proxies)*)
 ```python3
 from duckduckgo_search import DDGS
 
 proxies = {
-    "http": "socks5h://user:password@geo.iproyal.com:32325",
-    "https": "socks5h://user:password@geo.iproyal.com:32325",
-    "no_proxy": "localhost,127.0.0.1",
+    "all://": "https://user:password@geo.iproyal.com:32325",
 }
 ddgs_text_gen = DDGS(proxies=proxies, timeout=20).text("something you need")
 for r in ddgs_text_gen:
-	print(r)
+    print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 1. text() - text search by by duckduckgo.com
 ```python
 def text(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
+    backend: str = "api",
 ) -> Iterator[dict]:
     """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
@@ -226,28 +223,28 @@
 from duckduckgo_search import DDGS
 
 ddgs = DDGS()
 
 keywords = 'live free or die'
 ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
-	print(r)
+    print(r)
 
 # Searching for pdf files
 keywords = 'russia filetype:pdf'
 ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
-	print(r)
+    print(r)
 
 # Using lite backend and limit the number of results to 10
 from itertools import islice
 
 ddgs_text_gen = DDGS().text("notes from a dead house", backend="lite")
 for r in islice(ddgs_text_gen, 10):
-	print(r)
+    print(r)
 ```
 
 
 [Go To TOP](#TOP)
 
 ## 2. answers() - instant answers by duckduckgo.com
```

### Comparing `duckduckgo_search-3.5.0/pyproject.toml` & `duckduckgo_search-3.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "click>=8.1.3",
     "lxml>=4.9.2",
+    "httpx[http2]>=0.24.1",
     "requests>=2.31.0",
 ]
 dynamic = ["version"]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/deedy5/duckduckgo_search"
```

### Comparing `duckduckgo_search-3.5.0/tests/test_duckduckgo_search.py` & `duckduckgo_search-3.6.0/tests/test_duckduckgo_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,32 +10,14 @@
     counter = 0
     for i, x in enumerate(results_gen):
         counter += 1
         if i >= 25:
             break
     assert counter >= 25
 
-def test_text_html():
-    results_gen = DDGS().text("cat", backend="html")
-    counter = 0
-    for i, x in enumerate(results_gen):
-        counter += 1
-        if i >= 25:
-            break
-    assert counter >= 25
-
-def test_text_lite():
-    results_gen = DDGS().text("cat", backend="lite")
-    counter = 0
-    for i, x in enumerate(results_gen):
-        counter += 1
-        if i >= 25:
-            break
-    assert counter >= 25
-
 
 def test_images():
     results_gen = DDGS().images("cat")
     counter = 0
     for i, x in enumerate(results_gen):
         counter += 1
         if i >= 150:
```

