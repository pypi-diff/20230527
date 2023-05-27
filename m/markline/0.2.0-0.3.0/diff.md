# Comparing `tmp/markline-0.2.0.tar.gz` & `tmp/markline-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markline-0.2.0.tar", max compression
+gzip compressed data, was "markline-0.3.0.tar", max compression
```

## Comparing `markline-0.2.0.tar` & `markline-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1069 2022-09-22 13:01:34.022832 markline-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     1398 2022-09-22 13:01:34.022832 markline-0.2.0/README.md
--rw-r--r--   0        0        0    27610 2022-09-22 13:01:34.026831 markline-0.2.0/markline/__init__.py
--rw-r--r--   0        0        0      598 2022-09-22 13:01:34.026831 markline-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2207 1970-01-01 00:00:00.000000 markline-0.2.0/setup.py
--rw-r--r--   0        0        0     2148 1970-01-01 00:00:00.000000 markline-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-27 10:24:23.478139 markline-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     1398 2023-05-27 10:24:23.478139 markline-0.3.0/README.md
+-rw-r--r--   0        0        0    27809 2023-05-27 10:24:23.478139 markline-0.3.0/markline/__init__.py
+-rw-r--r--   0        0        0      604 2023-05-27 10:24:23.478139 markline-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2106 1970-01-01 00:00:00.000000 markline-0.3.0/PKG-INFO
```

### Comparing `markline-0.2.0/LICENSE.md` & `markline-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `markline-0.2.0/README.md` & `markline-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `markline-0.2.0/markline/__init__.py` & `markline-0.3.0/markline/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 import copy
 import importlib.util
 import re
 from builtins import slice
 from collections import Counter
 from datetime import datetime
+from html import unescape
 from select import select
 from typing import Callable, List, NamedTuple, Union
 
 import httpx
-import pandoc
+import pypandoc
 import pytz
 from bs4 import BeautifulSoup, element
 from furl import furl
 
 DEFAULT_META_ARRAYS = [
     "article:author",
     "article:tag",
@@ -130,29 +131,28 @@
     """
     spec = importlib.util.find_spec(package_name)
     if spec is None:
         return False
     return True
 
 
-def unshorten_url(url: str, headers: dict = {}) -> str:
+def unshorten_url(url: str, client: httpx.Client = httpx.Client()) -> str:
     """Unshorten a URL by following redirects, useful for short
     URLs used in social media.
     A HEAD request is used to avoid downloading the entire page.
     The httpx session recycles connections across redirects.
 
     Args:
         url (str): A URL to unshorten.
-        headers (dict, optional): Headers for the httpx session.
-            Defaults to {}.
+        client (httpx.Client, optional): httpx.Client for the session.
+            Defaults to httpx.Client().
 
     Returns:
         str: URL of the final destination.
     """
-    client = httpx.Client()
     request = client.build_request("GET", url)
     while request is not None:
         response = client.send(request)
         request = response.next_request
     return str(response.url)
 
 
@@ -168,30 +168,30 @@
     return furl(url).remove(query=True).tostr()
 
 
 def prepare_url(
     url: str,
     unshorten: bool = True,
     trim: bool = True,
-    headers: dict = {},
+    client: httpx.Client = httpx.Client(),
 ) -> str:
     """Prepare a URL for content extraction.
 
     Args:
         url (str): URL to prepare.
         unshorten (bool, optional): Unshorten the URL. Defaults to True.
         trim (bool, optional): Unshorten the URL. Defaults to True.
-        headers (dict, optional): Headers for the httpx session.
-            Defaults to {}.
+        client (httpx.Client, optional): httpx.Client for the session.
+            Defaults to httpx.Client().
 
     Returns:
         str: Prepared URL.
     """
     if unshorten:
-        url = unshorten_url(url, headers)
+        url = unshorten_url(url, client)
     if trim:
         url = trim_url(url)
     return url
 
 
 def coalesce(*args):
     """Return the first non-null value in a list of arguments."""
@@ -258,31 +258,35 @@
     ts_utc = ts.replace(tzinfo=pytz.utc)
     if zone == "utc":
         return ts_utc
     tz = pytz.timezone(zone)
     return ts_utc.astimezone(tz)
 
 
-def download_media(url: str, filename: str = None) -> str:
+def download_media(
+    url: str,
+    filename: str = None,
+    client: httpx.Client = httpx.Client(),
+) -> str:
     """Download a file from a URL and save it to a path.
     Useful for downloading images and other media where the
     file format is provided in the Content-Type response header.
 
     If no filename is provided, the filename is derived from the URL stem
     and the file extension is extracted from the Content-Type header.
 
     Args:
         url (str): URL of the file to download.
         filename (str, optional): filename to save the file as. Defaults to None.
 
     Returns:
         str: filename of the downloaded file.
     """
-    response = httpx.get(url)
-    assert response.status_code == 200, response.text
+    response = client.get(url)
+    assert response.status_code == httpx.codes.OK, response.text
     if not filename:
         name = furl(url).path.segments[-1]
         media_type = response.headers.get("Content-Type").split("/")[1]
         # TODO support extension aliases like "jpg" for "jpeg"
         if name.endswith("." + media_type):
             filename = name
         else:
@@ -393,15 +397,16 @@
     The `draft` attribute is a copy of `original` that can be modified by a pipeline
     of steps and exported to markdown or HTML.
 
     Args:
     url (str): URL to prepare and fetch content from.
     unshorten (bool, optional): Unshorten the URL. Defaults to True.
     trim (bool, optional): Unshorten the URL. Defaults to True.
-    headers (dict, optional): Headers for the httpx session. Defaults to {}.
+    client (httpx.Client, optional): httpx.Client for the session.
+        Defaults to httpx.Client().
     meta_arrays (list, optional): List of meta tags to be converted to arrays. Defaults to None.
         See the gather_meta() docstring for more details on meta_arrays.
 
     Properties:
     original (BeautifulSoup): The original HTML content of the URL.
     draft (BeautifulSoup): HTML content of the URL to be processed for export.
     meta (dict): Metadata extracted from the original HTML content.
@@ -411,26 +416,26 @@
     def __init__(
         self,
         url: str = None,
         filepath: str = None,
         parser: str = "lxml",
         unshorten: bool = True,
         trim: bool = True,
-        headers: dict = {},
+        client: httpx.Client = httpx.Client(),
         meta_arrays: list = [],
     ):
         if not any((url, filepath)):
             raise ValueError("One of URL or filepath must be provided.")
         if all((url, filepath)):
             raise ValueError("Only one of URL or filepath can be provided.")
         if filepath:
             self.url = filepath
         if url:
-            self.headers = headers
-            url = prepare_url(url, unshorten, trim, self.headers)
+            self.client = client
+            url = prepare_url(url, unshorten, trim, self.client)
             self.url = url
         self.original = self.fetch_content(url=url, parser=parser, filepath=filepath)
         self.draft = copy.copy(self.original)
         self.meta_arrays = meta_arrays
         self.meta = self.gather_meta()
         self.properties = self.set_properties()
 
@@ -458,15 +463,15 @@
             BeautifulSoup: BeautifulSoup object of the HTML content.
         """
         if parser == "lxml" and not package_available("lxml"):
             parser = "html.parser"
         if filepath:
             with open(filepath, "r") as f:
                 return BeautifulSoup(f.read(), parser)
-        response = httpx.get(url, headers=self.headers)
+        response = self.client.get(url)
         return BeautifulSoup(response.content, parser)
 
     def gather_meta(self, counts: bool = False) -> dict:
         """Extract metadata from the <meta> tags within HTML content.
         Some metadata is extracted as arrays, e.g. article:tag, where
         multiple <meta> tags with the same property are present on the page.
 
@@ -732,16 +737,20 @@
             output_options (List[str], optional): A list of Pandoc write options.
                 Defaults to ["--wrap=none"]. See available options:
                 https://pandoc.org/MANUAL.html#options
 
         Returns:
             str: Pandoc formatted output.
         """
-        doc = pandoc.read(self.draft.prettify(), format=input_format)
-        return pandoc.write(doc, format=output_format, options=output_options)
+        return pypandoc.convert_text(
+            source=self.draft.prettify(),
+            format=input_format,
+            to="md",
+            extra_args=output_options,
+        )
 
     def to_html(self, filepath: str = None) -> str:
         """Render the draft as HTML.
         If a filepath is provided, the HTML content is written to the file.
 
         Returns:
             str: HTML content.
```

### Comparing `markline-0.2.0/pyproject.toml` & `markline-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "markline"
-version = "0.2.0"
+version = "0.3.0"
 description = "Convert Markup to Markdown with a transformation pipeline."
 authors = ["Hugh Cameron <hescameron+githubprojects@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/hughcameron/markline"
 repository = "https://github.com/hughcameron/markline"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
-beautifulsoup4 = "^4.11.1"
-pandoc = "^2.2"
+python = "^3.10.6"
+beautifulsoup4 = "^4.12.2"
 furl = "^2.1.3"
-httpx = "^0.23.0"
+httpx = "^0.24.1"
+pypandoc = "^1.11"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `markline-0.2.0/PKG-INFO` & `markline-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: markline
-Version: 0.2.0
+Version: 0.3.0
 Summary: Convert Markup to Markdown with a transformation pipeline.
 Home-page: https://github.com/hughcameron/markline
 License: MIT
 Author: Hugh Cameron
 Author-email: hescameron+githubprojects@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10.6,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: furl (>=2.1.3,<3.0.0)
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: pandoc (>=2.2,<3.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: pypandoc (>=1.11,<2.0)
 Project-URL: Repository, https://github.com/hughcameron/markline
 Description-Content-Type: text/markdown
 
 # <img src="img/markline.svg" width="200">
 
 **Markline** converts HTML to Markdown and supports transformation methods borrowed from data engineering concepts. The goal of this project is to provide a simple API that renders HTML to Markdown for note management applications such as [Logseq](https://logseq.com).
```

