# Comparing `tmp/meta-tags-parser-1.2.1.tar.gz` & `tmp/meta_tags_parser-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta-tags-parser-1.2.1.tar", max compression
+gzip compressed data, was "meta_tags_parser-1.3.0.tar", max compression
```

## Comparing `meta-tags-parser-1.2.1.tar` & `meta_tags_parser-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1052 2022-08-04 22:47:08.398037 meta-tags-parser-1.2.1/LICENSE
--rw-r--r--   0        0        0     7896 2022-08-04 22:47:08.398037 meta-tags-parser-1.2.1/README.md
--rw-r--r--   0        0        0      149 2022-08-04 22:47:08.398037 meta-tags-parser-1.2.1/meta_tags_parser/__init__.py
--rw-r--r--   0        0        0      479 2022-08-04 22:47:08.398037 meta-tags-parser-1.2.1/meta_tags_parser/download.py
--rw-r--r--   0        0        0     5944 2022-08-04 22:47:08.398037 meta-tags-parser-1.2.1/meta_tags_parser/parse.py
--rw-r--r--   0        0        0     1045 2022-08-04 22:47:08.398037 meta-tags-parser-1.2.1/meta_tags_parser/public.py
--rw-r--r--   0        0        0        0 2022-08-04 22:47:08.398037 meta-tags-parser-1.2.1/meta_tags_parser/py.typed
--rw-r--r--   0        0        0     1121 2022-08-04 22:47:08.398037 meta-tags-parser-1.2.1/meta_tags_parser/settings.py
--rw-r--r--   0        0        0     1224 2022-08-04 22:47:08.398037 meta-tags-parser-1.2.1/meta_tags_parser/snippets.py
--rw-r--r--   0        0        0     1295 2022-08-04 22:47:08.398037 meta-tags-parser-1.2.1/meta_tags_parser/structs.py
--rw-r--r--   0        0        0     1573 2022-08-04 22:47:15.386132 meta-tags-parser-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     8848 2022-08-04 22:47:16.230035 meta-tags-parser-1.2.1/setup.py
--rw-r--r--   0        0        0     8659 2022-08-04 22:47:16.230596 meta-tags-parser-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-05-26 22:58:58.987301 meta_tags_parser-1.3.0/LICENSE
+-rw-r--r--   0        0        0     7896 2023-05-26 22:58:58.987301 meta_tags_parser-1.3.0/README.md
+-rw-r--r--   0        0        0      149 2023-05-26 22:58:58.987301 meta_tags_parser-1.3.0/meta_tags_parser/__init__.py
+-rw-r--r--   0        0        0      479 2023-05-26 22:58:58.987301 meta_tags_parser-1.3.0/meta_tags_parser/download.py
+-rw-r--r--   0        0        0     5944 2023-05-26 22:58:58.987301 meta_tags_parser-1.3.0/meta_tags_parser/parse.py
+-rw-r--r--   0        0        0     1045 2023-05-26 22:58:58.987301 meta_tags_parser-1.3.0/meta_tags_parser/public.py
+-rw-r--r--   0        0        0        0 2023-05-26 22:58:58.987301 meta_tags_parser-1.3.0/meta_tags_parser/py.typed
+-rw-r--r--   0        0        0     1121 2023-05-26 22:58:58.987301 meta_tags_parser-1.3.0/meta_tags_parser/settings.py
+-rw-r--r--   0        0        0     1224 2023-05-26 22:58:58.987301 meta_tags_parser-1.3.0/meta_tags_parser/snippets.py
+-rw-r--r--   0        0        0     1361 2023-05-26 22:58:58.987301 meta_tags_parser-1.3.0/meta_tags_parser/structs.py
+-rw-r--r--   0        0        0     1614 2023-05-26 22:59:13.631345 meta_tags_parser-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8710 1970-01-01 00:00:00.000000 meta_tags_parser-1.3.0/PKG-INFO
```

### Comparing `meta-tags-parser-1.2.1/LICENSE` & `meta_tags_parser-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meta-tags-parser-1.2.1/README.md` & `meta_tags_parser-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `meta-tags-parser-1.2.1/meta_tags_parser/parse.py` & `meta_tags_parser-1.3.0/meta_tags_parser/parse.py`

 * *Files identical despite different names*

### Comparing `meta-tags-parser-1.2.1/meta_tags_parser/public.py` & `meta_tags_parser-1.3.0/meta_tags_parser/public.py`

 * *Files identical despite different names*

### Comparing `meta-tags-parser-1.2.1/meta_tags_parser/settings.py` & `meta_tags_parser-1.3.0/meta_tags_parser/settings.py`

 * *Files identical despite different names*

### Comparing `meta-tags-parser-1.2.1/meta_tags_parser/snippets.py` & `meta_tags_parser-1.3.0/meta_tags_parser/snippets.py`

 * *Files identical despite different names*

### Comparing `meta-tags-parser-1.2.1/meta_tags_parser/structs.py` & `meta_tags_parser-1.3.0/meta_tags_parser/structs.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     url: str = ""
 
 
 @dataclasses.dataclass
 class SnippetGroup:
     """Groupping for social media."""
 
-    open_graph: SocialMediaSnippet = SocialMediaSnippet()
-    twitter: SocialMediaSnippet = SocialMediaSnippet()
+    open_graph: SocialMediaSnippet = dataclasses.field(default_factory=SocialMediaSnippet)
+    twitter: SocialMediaSnippet = dataclasses.field(default_factory=SocialMediaSnippet)
 
 
 class WhatToParse(enum.IntEnum):
     """Enum for parsing configuration."""
 
     TITLE: int = 0
     BASIC: int = 1
```

### Comparing `meta-tags-parser-1.2.1/pyproject.toml` & `meta_tags_parser-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "meta-tags-parser"
-version = "1.2.1"
+version = "1.3.0"
 description = "Fast and modern meta tags parser (og, twitter, title, description, etc) with snippet support"
 authors = ["Denis Anikin <ad@xfenix.ru>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/xfenix/meta-tags-parser/"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [
     { include = "meta_tags_parser" }
 ]
 
 [tool.poetry.urls]
@@ -23,16 +24,16 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
+pytest-cov = "*"
 Faker = "*"
-pytest-coverage = "*"
 pytest-asyncio = "*"
 pylint = "*"
 mypy = "*"
 pytest-xdist = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `meta-tags-parser-1.2.1/setup.py` & `meta_tags_parser-1.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,228 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: meta-tags-parser
+Version: 1.3.0
+Summary: Fast and modern meta tags parser (og, twitter, title, description, etc) with snippet support
+Home-page: https://github.com/xfenix/meta-tags-parser/
+License: MIT
+Author: Denis Anikin
+Author-email: ad@xfenix.ru
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: httpx
+Project-URL: Documentation, https://github.com/xfenix/meta-tags-parser
+Description-Content-Type: text/markdown
+
+# Meta tags parser
+[![Test, lint, publish](https://github.com/xfenix/meta-tags-parser/actions/workflows/main.yml/badge.svg)](https://github.com/xfenix/meta-tags-parser/actions/workflows/main.yml)
+[![PyPI version](https://badge.fury.io/py/meta-tags-parser.svg)](https://badge.fury.io/py/meta-tags-parser)
+[![Downloads](https://pepy.tech/badge/meta-tags-parser)](https://pepy.tech/project/meta-tags-parser)
+[![codecov](https://codecov.io/gh/xfenix/meta-tags-parser/branch/master/graph/badge.svg)](https://codecov.io/gh/xfenix/meta-tags-parser)
+<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+[![Imports: isort](https://img.shields.io/badge/imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://timothycrosley.github.io/isort/)
+
+Fast, modern, pure python meta tags parser and snippet creator with full support of type annotations, py.typed in basic package and structured output. No jelly dicts, only typed structures!  
+If you want to see what exactly is social media snippets, look at the example:
+![](https://raw.githubusercontent.com/xfenix/meta-tags-parser/master/social-media-snippets.png)
+
+## Requirements
+* Python 3.8+
+* [Httpx](https://www.python-httpx.org/)
+
+## Install
+`pip install meta-tags-parser`
+
+## Usage
+### TL:DR
+1. Parse meta tags from source:
+    ```python
+    from meta_tags_parser import parse_meta_tags_from_source, structs
+
+
+    desired_result: structs.TagsGroup = parse_meta_tags_from_source("""... html source ...""")
+    # desired_result — is what you want
+    ```
+1. Parse meta tags from url:
+    ```python
+    from meta_tags_parser import parse_tags_from_url, parse_tags_from_url_async, structs
+
+
+    desired_result: structs.TagsGroup = parse_tags_from_url("https://xfenix.ru")
+    # and async variant
+    desired_result: structs.TagsGroup = await parse_tags_from_url_async("https://xfenix.ru")
+    # desired_result — is what you want for both cases
+    ```
+1. Parse social media snippet from source:
+    ```python
+    from meta_tags_parser import parse_snippets_from_source, structs
+
+
+    snippet_obj: structs.SnippetGroup = parse_snippets_from_source("""... html source ...""")
+    # snippet_obj — is what you want
+    # access like snippet_obj.open_graph.title, ...
+    ```
+1. Parse social media snippet from url:
+    ```python
+    from meta_tags_parser import parse_snippets_from_url, parse_snippets_from_url_async, structs
+
+
+    snippet_obj: structs.SnippetGroup = parse_snippets_from_url("https://xfenix.ru")
+    # and async variant
+    snippet_obj: structs.SnippetGroup = await parse_snippets_from_url_async("https://xfenix.ru")
+    # snippet_obj — is what you want
+    # access like snippet_obj.open_graph.title, ...
+    ```
+
+**Huge note**: functions `*_from_url` written only for convenience and very error-prone, so any reconnections/error handling — completely on your side.  
+Also, I don't want to add some bloated requirements to achieve robust connections for any users, because they may simply not await any of this from the library. But if you really need this — write me.
+
+### Basic snippets parsing
+Lets say you want extract snippet for twitter from html page:
+```python
+from meta_tags_parser import parse_snippets_from_source, structs
+
+
+my_result: structs.TagsGroup = parse_snippets_from_source("""
+    <meta property="og:card" content="summary_large_image">
+    <meta property="og:url" content="https://github.com/">
+    <meta property="og:title" content="Hello, my friend">
+    <meta property="og:description" content="Content here, yehehe">
+    <meta property="twitter:card" content="summary_large_image">
+    <meta property="twitter:url" content="https://github.com/">
+    <meta property="twitter:title" content="Hello, my friend">
+    <meta property="twitter:description" content="Content here, yehehe">
+""")
+
+print(my_result)
+# What will be printed:
+"""
+SnippetGroup(
+    open_graph=SocialMediaSnippet(
+        title='Hello, my friend',
+        description='Content here, yehehe',
+        image='',
+        url='https://github.com/'
+    ),
+    twitter=SocialMediaSnippet(
+        title='Hello, my friend',
+        description='Content here, yehehe',
+        image='',
+        url='https://github.com/'
+    )
+)
+"""
+# You can access attributes as this
+my_result.open_graph.title
+my_result.twitter.image
+# All fields are necessary and will be always available, even if they have not contain data
+# So no need to worry about attributes exsitence (but you may need to check values)
+```
+
+### Basic meta tags parsing
+Main function is `parse_meta_tags_from_source`. It can be used like this:
+```python
+from meta_tags_parser import parse_meta_tags_from_source, structs
+
+
+my_result: structs.TagsGroup = parse_meta_tags_from_source("""... html source ...""")
+print(my_result)
+
+# What will be printed:
+"""
+structs.TagsGroup(
+    title="...",
+    twitter=[
+        structs.OneMetaTag(
+            name="title", value="Hello",
+            ...
+        )
+    ],
+    open_graph=[
+        structs.OneMetaTag(
+            name="title", value="Hello",
+            ...
+        )
+    ],
+    basic=[
+        structs.OneMetaTag(
+            name="title", value="Hello",
+            ...
+        )
+    ],
+    other=[
+        structs.OneMetaTag(
+            name="article:name", value="Hello",
+            ...
+        )
+    ]
+)
+"""
+```
+As you can see from this example, we are not using any jelly dicts, only structured dataclasses. Lets see another example:
+
+```python
+from meta_tags_parser import parse_meta_tags_from_source, structs
+
+
+my_result: structs.TagsGroup = parse_meta_tags_from_source("""
+    <meta property="twitter:card" content="summary_large_image">
+    <meta property="twitter:url" content="https://github.com/">
+    <meta property="twitter:title" content="Hello, my friend">
+    <meta property="twitter:description" content="Content here, yehehe">
+""")
+
+print(my_result)
+# What will be printed:
+"""
+TagsGroup(
+    title='',
+    basic=[],
+    open_graph=[],
+    twitter=[
+        OneMetaTag(name='card', value='summary_large_image'),
+        OneMetaTag(name='url', value='https://github.com/'),
+        OneMetaTag(name='title', value='Hello, my friend'),
+        OneMetaTag(name='description', value='Content here, yehehe')
+    ],
+    other=[]
+)
+"""
+
+for one_tag in my_result.twitter:
+    if one_tag.name == "title":
+        print(one_tag.value)
+# What will be printed:
+"""
+Hello, my friend
+"""
+```
+
+### If you want to improve speed
+You can specify what you want to parse:
+```python
+from meta_tags_parser import parse_meta_tags_from_source, structs
+
+
+result: structs.TagsGroup = parse_meta_tags_from_source("""... source ...""",
+    what_to_parse=(WhatToParse.TITLE, WhatToParse.BASIC, WhatToParse.OPEN_GRAPH, WhatToParse.TWITTER, WhatToParse.OTHER)
+)
+```
+If you reduce this tuple of parsing requirements it may increase overall parsing speed.
+
+## Important notes
+* Any name in meta tag (name or property attribute) will be lowercased
+* I decided to strip `og:` and `twitter:` from original attributes, and let dataclass structures carry this information. If parser met meta tag with property `og:name`, it will be available in `my_result` variable as one element of list `my_result.open_graph`
+* Title of page (e.g. `<title>Something</title>`) will be available as string `my_result.title` (of course, you recieve `Something`)
+* «Standart» tags like title, description (check full list here [./meta_tags_parser/structs.py](./meta_tags_parser/structs.py) in constant `BASIC_META_TAGS`) will be available as list in `my_result.basic`
+* Other tags will be available as list in `my_result.other` attribute, name of tags will be preserved, unlike `og:`/`twitter:` behaviour
+* If you want structured snippets, use `parse_snippets_from_source` function
 
-packages = \
-['meta_tags_parser']
 
-package_data = \
-{'': ['*']}
+# Changelog
+You can check https://github.com/xfenix/meta-tags-parser/releases/ release page.
 
-install_requires = \
-['httpx']
-
-setup_kwargs = {
-    'name': 'meta-tags-parser',
-    'version': '1.2.1',
-    'description': 'Fast and modern meta tags parser (og, twitter, title, description, etc) with snippet support',
-    'long_description': '# Meta tags parser\n[![Test, lint, publish](https://github.com/xfenix/meta-tags-parser/actions/workflows/main.yml/badge.svg)](https://github.com/xfenix/meta-tags-parser/actions/workflows/main.yml)\n[![PyPI version](https://badge.fury.io/py/meta-tags-parser.svg)](https://badge.fury.io/py/meta-tags-parser)\n[![Downloads](https://pepy.tech/badge/meta-tags-parser)](https://pepy.tech/project/meta-tags-parser)\n[![codecov](https://codecov.io/gh/xfenix/meta-tags-parser/branch/master/graph/badge.svg)](https://codecov.io/gh/xfenix/meta-tags-parser)\n<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>\n[![Imports: isort](https://img.shields.io/badge/imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://timothycrosley.github.io/isort/)\n\nFast, modern, pure python meta tags parser and snippet creator with full support of type annotations, py.typed in basic package and structured output. No jelly dicts, only typed structures!  \nIf you want to see what exactly is social media snippets, look at the example:\n![](https://raw.githubusercontent.com/xfenix/meta-tags-parser/master/social-media-snippets.png)\n\n## Requirements\n* Python 3.8+\n* [Httpx](https://www.python-httpx.org/)\n\n## Install\n`pip install meta-tags-parser`\n\n## Usage\n### TL:DR\n1. Parse meta tags from source:\n    ```python\n    from meta_tags_parser import parse_meta_tags_from_source, structs\n\n\n    desired_result: structs.TagsGroup = parse_meta_tags_from_source("""... html source ...""")\n    # desired_result — is what you want\n    ```\n1. Parse meta tags from url:\n    ```python\n    from meta_tags_parser import parse_tags_from_url, parse_tags_from_url_async, structs\n\n\n    desired_result: structs.TagsGroup = parse_tags_from_url("https://xfenix.ru")\n    # and async variant\n    desired_result: structs.TagsGroup = await parse_tags_from_url_async("https://xfenix.ru")\n    # desired_result — is what you want for both cases\n    ```\n1. Parse social media snippet from source:\n    ```python\n    from meta_tags_parser import parse_snippets_from_source, structs\n\n\n    snippet_obj: structs.SnippetGroup = parse_snippets_from_source("""... html source ...""")\n    # snippet_obj — is what you want\n    # access like snippet_obj.open_graph.title, ...\n    ```\n1. Parse social media snippet from url:\n    ```python\n    from meta_tags_parser import parse_snippets_from_url, parse_snippets_from_url_async, structs\n\n\n    snippet_obj: structs.SnippetGroup = parse_snippets_from_url("https://xfenix.ru")\n    # and async variant\n    snippet_obj: structs.SnippetGroup = await parse_snippets_from_url_async("https://xfenix.ru")\n    # snippet_obj — is what you want\n    # access like snippet_obj.open_graph.title, ...\n    ```\n\n**Huge note**: functions `*_from_url` written only for convenience and very error-prone, so any reconnections/error handling — completely on your side.  \nAlso, I don\'t want to add some bloated requirements to achieve robust connections for any users, because they may simply not await any of this from the library. But if you really need this — write me.\n\n### Basic snippets parsing\nLets say you want extract snippet for twitter from html page:\n```python\nfrom meta_tags_parser import parse_snippets_from_source, structs\n\n\nmy_result: structs.TagsGroup = parse_snippets_from_source("""\n    <meta property="og:card" content="summary_large_image">\n    <meta property="og:url" content="https://github.com/">\n    <meta property="og:title" content="Hello, my friend">\n    <meta property="og:description" content="Content here, yehehe">\n    <meta property="twitter:card" content="summary_large_image">\n    <meta property="twitter:url" content="https://github.com/">\n    <meta property="twitter:title" content="Hello, my friend">\n    <meta property="twitter:description" content="Content here, yehehe">\n""")\n\nprint(my_result)\n# What will be printed:\n"""\nSnippetGroup(\n    open_graph=SocialMediaSnippet(\n        title=\'Hello, my friend\',\n        description=\'Content here, yehehe\',\n        image=\'\',\n        url=\'https://github.com/\'\n    ),\n    twitter=SocialMediaSnippet(\n        title=\'Hello, my friend\',\n        description=\'Content here, yehehe\',\n        image=\'\',\n        url=\'https://github.com/\'\n    )\n)\n"""\n# You can access attributes as this\nmy_result.open_graph.title\nmy_result.twitter.image\n# All fields are necessary and will be always available, even if they have not contain data\n# So no need to worry about attributes exsitence (but you may need to check values)\n```\n\n### Basic meta tags parsing\nMain function is `parse_meta_tags_from_source`. It can be used like this:\n```python\nfrom meta_tags_parser import parse_meta_tags_from_source, structs\n\n\nmy_result: structs.TagsGroup = parse_meta_tags_from_source("""... html source ...""")\nprint(my_result)\n\n# What will be printed:\n"""\nstructs.TagsGroup(\n    title="...",\n    twitter=[\n        structs.OneMetaTag(\n            name="title", value="Hello",\n            ...\n        )\n    ],\n    open_graph=[\n        structs.OneMetaTag(\n            name="title", value="Hello",\n            ...\n        )\n    ],\n    basic=[\n        structs.OneMetaTag(\n            name="title", value="Hello",\n            ...\n        )\n    ],\n    other=[\n        structs.OneMetaTag(\n            name="article:name", value="Hello",\n            ...\n        )\n    ]\n)\n"""\n```\nAs you can see from this example, we are not using any jelly dicts, only structured dataclasses. Lets see another example:\n\n```python\nfrom meta_tags_parser import parse_meta_tags_from_source, structs\n\n\nmy_result: structs.TagsGroup = parse_meta_tags_from_source("""\n    <meta property="twitter:card" content="summary_large_image">\n    <meta property="twitter:url" content="https://github.com/">\n    <meta property="twitter:title" content="Hello, my friend">\n    <meta property="twitter:description" content="Content here, yehehe">\n""")\n\nprint(my_result)\n# What will be printed:\n"""\nTagsGroup(\n    title=\'\',\n    basic=[],\n    open_graph=[],\n    twitter=[\n        OneMetaTag(name=\'card\', value=\'summary_large_image\'),\n        OneMetaTag(name=\'url\', value=\'https://github.com/\'),\n        OneMetaTag(name=\'title\', value=\'Hello, my friend\'),\n        OneMetaTag(name=\'description\', value=\'Content here, yehehe\')\n    ],\n    other=[]\n)\n"""\n\nfor one_tag in my_result.twitter:\n    if one_tag.name == "title":\n        print(one_tag.value)\n# What will be printed:\n"""\nHello, my friend\n"""\n```\n\n### If you want to improve speed\nYou can specify what you want to parse:\n```python\nfrom meta_tags_parser import parse_meta_tags_from_source, structs\n\n\nresult: structs.TagsGroup = parse_meta_tags_from_source("""... source ...""",\n    what_to_parse=(WhatToParse.TITLE, WhatToParse.BASIC, WhatToParse.OPEN_GRAPH, WhatToParse.TWITTER, WhatToParse.OTHER)\n)\n```\nIf you reduce this tuple of parsing requirements it may increase overall parsing speed.\n\n## Important notes\n* Any name in meta tag (name or property attribute) will be lowercased\n* I decided to strip `og:` and `twitter:` from original attributes, and let dataclass structures carry this information. If parser met meta tag with property `og:name`, it will be available in `my_result` variable as one element of list `my_result.open_graph`\n* Title of page (e.g. `<title>Something</title>`) will be available as string `my_result.title` (of course, you recieve `Something`)\n* «Standart» tags like title, description (check full list here [./meta_tags_parser/structs.py](./meta_tags_parser/structs.py) in constant `BASIC_META_TAGS`) will be available as list in `my_result.basic`\n* Other tags will be available as list in `my_result.other` attribute, name of tags will be preserved, unlike `og:`/`twitter:` behaviour\n* If you want structured snippets, use `parse_snippets_from_source` function\n\n\n# Changelog\nYou can check https://github.com/xfenix/meta-tags-parser/releases/ release page.\n',
-    'author': 'Denis Anikin',
-    'author_email': 'ad@xfenix.ru',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/xfenix/meta-tags-parser/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,112 +1,110 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['meta_tags_parser'] package_data = \ {'': ['*']} install_requires = \
-['httpx'] setup_kwargs = { 'name': 'meta-tags-parser', 'version': '1.2.1',
-'description': 'Fast and modern meta tags parser (og, twitter, title,
-description, etc) with snippet support', 'long_description': '# Meta tags
-parser\n[![Test, lint, publish](https://github.com/xfenix/meta-tags-parser/
-actions/workflows/main.yml/badge.svg)](https://github.com/xfenix/meta-tags-
-parser/actions/workflows/main.yml)\n[![PyPI version](https://badge.fury.io/py/
-meta-tags-parser.svg)](https://badge.fury.io/py/meta-tags-parser)\n[!
-[Downloads](https://pepy.tech/badge/meta-tags-parser)](https://pepy.tech/
-project/meta-tags-parser)\n[![codecov](https://codecov.io/gh/xfenix/meta-tags-
-parser/branch/master/graph/badge.svg)](https://codecov.io/gh/xfenix/meta-tags-
-parser)\n[Code_style:_black]\n[![Imports: isort](https://img.shields.io/badge/
-imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
-timothycrosley.github.io/isort/)\n\nFast, modern, pure python meta tags parser
-and snippet creator with full support of type annotations, py.typed in basic
-package and structured output. No jelly dicts, only typed structures! \nIf you
-want to see what exactly is social media snippets, look at the example:\n![]
-(https://raw.githubusercontent.com/xfenix/meta-tags-parser/master/social-media-
-snippets.png)\n\n## Requirements\n* Python 3.8+\n* [Httpx](https://www.python-
-httpx.org/)\n\n## Install\n`pip install meta-tags-parser`\n\n## Usage\n### TL:
-DR\n1. Parse meta tags from source:\n ```python\n from meta_tags_parser import
-parse_meta_tags_from_source, structs\n\n\n desired_result: structs.TagsGroup =
-parse_meta_tags_from_source("""... html source ...""")\n # desired_result â
-is what you want\n ```\n1. Parse meta tags from url:\n ```python\n from
-meta_tags_parser import parse_tags_from_url, parse_tags_from_url_async,
-structs\n\n\n desired_result: structs.TagsGroup = parse_tags_from_url("https://
-xfenix.ru")\n # and async variant\n desired_result: structs.TagsGroup = await
-parse_tags_from_url_async("https://xfenix.ru")\n # desired_result â is what
-you want for both cases\n ```\n1. Parse social media snippet from source:\n
-```python\n from meta_tags_parser import parse_snippets_from_source,
-structs\n\n\n snippet_obj: structs.SnippetGroup = parse_snippets_from_source
-("""... html source ...""")\n # snippet_obj â is what you want\n # access
-like snippet_obj.open_graph.title, ...\n ```\n1. Parse social media snippet
-from url:\n ```python\n from meta_tags_parser import parse_snippets_from_url,
-parse_snippets_from_url_async, structs\n\n\n snippet_obj: structs.SnippetGroup
-= parse_snippets_from_url("https://xfenix.ru")\n # and async variant\n
-snippet_obj: structs.SnippetGroup = await parse_snippets_from_url_async("https:
-//xfenix.ru")\n # snippet_obj â is what you want\n # access like
-snippet_obj.open_graph.title, ...\n ```\n\n**Huge note**: functions
-`*_from_url` written only for convenience and very error-prone, so any
-reconnections/error handling â completely on your side. \nAlso, I don\'t want
-to add some bloated requirements to achieve robust connections for any users,
-because they may simply not await any of this from the library. But if you
-really need this â write me.\n\n### Basic snippets parsing\nLets say you want
-extract snippet for twitter from html page:\n```python\nfrom meta_tags_parser
-import parse_snippets_from_source, structs\n\n\nmy_result: structs.TagsGroup =
-parse_snippets_from_source("""\n
-\n
-\n
-\n
-\n
-\n
-\n
-\n
-\n""")\n\nprint(my_result)\n# What will be printed:\n"""\nSnippetGroup(\n
-open_graph=SocialMediaSnippet(\n title=\'Hello, my friend\',\n
-description=\'Content here, yehehe\',\n image=\'\',\n url=\'https://github.com/
-\'\n ),\n twitter=SocialMediaSnippet(\n title=\'Hello, my friend\',\n
-description=\'Content here, yehehe\',\n image=\'\',\n url=\'https://github.com/
-\'\n )\n)\n"""\n# You can access attributes as
-this\nmy_result.open_graph.title\nmy_result.twitter.image\n# All fields are
-necessary and will be always available, even if they have not contain data\n#
-So no need to worry about attributes exsitence (but you may need to check
-values)\n```\n\n### Basic meta tags parsing\nMain function is
-`parse_meta_tags_from_source`. It can be used like this:\n```python\nfrom
-meta_tags_parser import parse_meta_tags_from_source, structs\n\n\nmy_result:
-structs.TagsGroup = parse_meta_tags_from_source("""... html source
-...""")\nprint(my_result)\n\n# What will be printed:\n"""\nstructs.TagsGroup(\n
-title="...",\n twitter=[\n structs.OneMetaTag(\n name="title", value="Hello",\n
-...\n )\n ],\n open_graph=[\n structs.OneMetaTag(\n name="title",
-value="Hello",\n ...\n )\n ],\n basic=[\n structs.OneMetaTag(\n name="title",
-value="Hello",\n ...\n )\n ],\n other=[\n structs.OneMetaTag(\n name="article:
-name", value="Hello",\n ...\n )\n ]\n)\n"""\n```\nAs you can see from this
-example, we are not using any jelly dicts, only structured dataclasses. Lets
-see another example:\n\n```python\nfrom meta_tags_parser import
-parse_meta_tags_from_source, structs\n\n\nmy_result: structs.TagsGroup =
-parse_meta_tags_from_source("""\n
-\n
-\n
-\n
-\n""")\n\nprint(my_result)\n# What will be printed:\n"""\nTagsGroup(\n
-title=\'\',\n basic=[],\n open_graph=[],\n twitter=[\n OneMetaTag
-(name=\'card\', value=\'summary_large_image\'),\n OneMetaTag(name=\'url\',
-value=\'https://github.com/\'),\n OneMetaTag(name=\'title\', value=\'Hello, my
-friend\'),\n OneMetaTag(name=\'description\', value=\'Content here, yehehe\')\n
-],\n other=[]\n)\n"""\n\nfor one_tag in my_result.twitter:\n if one_tag.name ==
-"title":\n print(one_tag.value)\n# What will be printed:\n"""\nHello, my
-friend\n"""\n```\n\n### If you want to improve speed\nYou can specify what you
-want to parse:\n```python\nfrom meta_tags_parser import
-parse_meta_tags_from_source, structs\n\n\nresult: structs.TagsGroup =
-parse_meta_tags_from_source("""... source ...""",\n what_to_parse=
+Metadata-Version: 2.1 Name: meta-tags-parser Version: 1.3.0 Summary: Fast and
+modern meta tags parser (og, twitter, title, description, etc) with snippet
+support Home-page: https://github.com/xfenix/meta-tags-parser/ License: MIT
+Author: Denis Anikin Author-email: ad@xfenix.ru Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: httpx Project-URL: Documentation, https://github.com/xfenix/
+meta-tags-parser Description-Content-Type: text/markdown # Meta tags parser [!
+[Test, lint, publish](https://github.com/xfenix/meta-tags-parser/actions/
+workflows/main.yml/badge.svg)](https://github.com/xfenix/meta-tags-parser/
+actions/workflows/main.yml) [![PyPI version](https://badge.fury.io/py/meta-
+tags-parser.svg)](https://badge.fury.io/py/meta-tags-parser) [![Downloads]
+(https://pepy.tech/badge/meta-tags-parser)](https://pepy.tech/project/meta-
+tags-parser) [![codecov](https://codecov.io/gh/xfenix/meta-tags-parser/branch/
+master/graph/badge.svg)](https://codecov.io/gh/xfenix/meta-tags-parser) [Code
+style:_black] [![Imports: isort](https://img.shields.io/badge/imports-isort-
+%231674b1?style=flat&labelColor=ef8336)](https://timothycrosley.github.io/
+isort/) Fast, modern, pure python meta tags parser and snippet creator with
+full support of type annotations, py.typed in basic package and structured
+output. No jelly dicts, only typed structures! If you want to see what exactly
+is social media snippets, look at the example: ![](https://
+raw.githubusercontent.com/xfenix/meta-tags-parser/master/social-media-
+snippets.png) ## Requirements * Python 3.8+ * [Httpx](https://www.python-
+httpx.org/) ## Install `pip install meta-tags-parser` ## Usage ### TL:DR 1.
+Parse meta tags from source: ```python from meta_tags_parser import
+parse_meta_tags_from_source, structs desired_result: structs.TagsGroup =
+parse_meta_tags_from_source("""... html source ...""") # desired_result â is
+what you want ``` 1. Parse meta tags from url: ```python from meta_tags_parser
+import parse_tags_from_url, parse_tags_from_url_async, structs desired_result:
+structs.TagsGroup = parse_tags_from_url("https://xfenix.ru") # and async
+variant desired_result: structs.TagsGroup = await parse_tags_from_url_async
+("https://xfenix.ru") # desired_result â is what you want for both cases ```
+1. Parse social media snippet from source: ```python from meta_tags_parser
+import parse_snippets_from_source, structs snippet_obj: structs.SnippetGroup =
+parse_snippets_from_source("""... html source ...""") # snippet_obj â is what
+you want # access like snippet_obj.open_graph.title, ... ``` 1. Parse social
+media snippet from url: ```python from meta_tags_parser import
+parse_snippets_from_url, parse_snippets_from_url_async, structs snippet_obj:
+structs.SnippetGroup = parse_snippets_from_url("https://xfenix.ru") # and async
+variant snippet_obj: structs.SnippetGroup = await parse_snippets_from_url_async
+("https://xfenix.ru") # snippet_obj â is what you want # access like
+snippet_obj.open_graph.title, ... ``` **Huge note**: functions `*_from_url`
+written only for convenience and very error-prone, so any reconnections/error
+handling â completely on your side. Also, I don't want to add some bloated
+requirements to achieve robust connections for any users, because they may
+simply not await any of this from the library. But if you really need this â
+write me. ### Basic snippets parsing Lets say you want extract snippet for
+twitter from html page: ```python from meta_tags_parser import
+parse_snippets_from_source, structs my_result: structs.TagsGroup =
+parse_snippets_from_source("""
+
+
+
+
+
+
+
+ """) print(my_result) # What will be printed: """ SnippetGroup
+( open_graph=SocialMediaSnippet( title='Hello, my friend', description='Content
+here, yehehe', image='', url='https://github.com/' ),
+twitter=SocialMediaSnippet( title='Hello, my friend', description='Content
+here, yehehe', image='', url='https://github.com/' ) ) """ # You can access
+attributes as this my_result.open_graph.title my_result.twitter.image # All
+fields are necessary and will be always available, even if they have not
+contain data # So no need to worry about attributes exsitence (but you may need
+to check values) ``` ### Basic meta tags parsing Main function is
+`parse_meta_tags_from_source`. It can be used like this: ```python from
+meta_tags_parser import parse_meta_tags_from_source, structs my_result:
+structs.TagsGroup = parse_meta_tags_from_source("""... html source ...""")
+print(my_result) # What will be printed: """ structs.TagsGroup( title="...",
+twitter=[ structs.OneMetaTag( name="title", value="Hello", ... ) ], open_graph=
+[ structs.OneMetaTag( name="title", value="Hello", ... ) ], basic=
+[ structs.OneMetaTag( name="title", value="Hello", ... ) ], other=
+[ structs.OneMetaTag( name="article:name", value="Hello", ... ) ] ) """ ``` As
+you can see from this example, we are not using any jelly dicts, only
+structured dataclasses. Lets see another example: ```python from
+meta_tags_parser import parse_meta_tags_from_source, structs my_result:
+structs.TagsGroup = parse_meta_tags_from_source("""
+
+
+
+ """) print(my_result) # What will be printed: """ TagsGroup( title='', basic=
+[], open_graph=[], twitter=[ OneMetaTag(name='card',
+value='summary_large_image'), OneMetaTag(name='url', value='https://github.com/
+'), OneMetaTag(name='title', value='Hello, my friend'), OneMetaTag
+(name='description', value='Content here, yehehe') ], other=[] ) """ for
+one_tag in my_result.twitter: if one_tag.name == "title": print(one_tag.value)
+# What will be printed: """ Hello, my friend """ ``` ### If you want to improve
+speed You can specify what you want to parse: ```python from meta_tags_parser
+import parse_meta_tags_from_source, structs result: structs.TagsGroup =
+parse_meta_tags_from_source("""... source ...""", what_to_parse=
 (WhatToParse.TITLE, WhatToParse.BASIC, WhatToParse.OPEN_GRAPH,
-WhatToParse.TWITTER, WhatToParse.OTHER)\n)\n```\nIf you reduce this tuple of
-parsing requirements it may increase overall parsing speed.\n\n## Important
-notes\n* Any name in meta tag (name or property attribute) will be
-lowercased\n* I decided to strip `og:` and `twitter:` from original attributes,
-and let dataclass structures carry this information. If parser met meta tag
-with property `og:name`, it will be available in `my_result` variable as one
-element of list `my_result.open_graph`\n* Title of page (e.g. `
+WhatToParse.TWITTER, WhatToParse.OTHER) ) ``` If you reduce this tuple of
+parsing requirements it may increase overall parsing speed. ## Important notes
+* Any name in meta tag (name or property attribute) will be lowercased * I
+decided to strip `og:` and `twitter:` from original attributes, and let
+dataclass structures carry this information. If parser met meta tag with
+property `og:name`, it will be available in `my_result` variable as one element
+of list `my_result.open_graph` * Title of page (e.g. `
 `) will be available as string `my_result.title` (of course, you recieve
-`Something`)\n* Â«StandartÂ» tags like title, description (check full list here
+`Something`) * Â«StandartÂ» tags like title, description (check full list here
 [./meta_tags_parser/structs.py](./meta_tags_parser/structs.py) in constant
-`BASIC_META_TAGS`) will be available as list in `my_result.basic`\n* Other tags
+`BASIC_META_TAGS`) will be available as list in `my_result.basic` * Other tags
 will be available as list in `my_result.other` attribute, name of tags will be
-preserved, unlike `og:`/`twitter:` behaviour\n* If you want structured
-snippets, use `parse_snippets_from_source` function\n\n\n# Changelog\nYou can
-check https://github.com/xfenix/meta-tags-parser/releases/ release page.\n',
-'author': 'Denis Anikin', 'author_email': 'ad@xfenix.ru', 'maintainer': None,
-'maintainer_email': None, 'url': 'https://github.com/xfenix/meta-tags-parser/',
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
+preserved, unlike `og:`/`twitter:` behaviour * If you want structured snippets,
+use `parse_snippets_from_source` function # Changelog You can check https://
+github.com/xfenix/meta-tags-parser/releases/ release page.
```

