# Comparing `tmp/pipen_annotate-0.7.1.tar.gz` & `tmp/pipen_annotate-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_annotate-0.7.1.tar", max compression
+gzip compressed data, was "pipen_annotate-0.7.2.tar", max compression
```

## Comparing `pipen_annotate-0.7.1.tar` & `pipen_annotate-0.7.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-04-14 19:24:27.332493 pipen_annotate-0.7.1/LICENSE
--rw-r--r--   0        0        0     1592 2023-04-14 19:24:27.332493 pipen_annotate-0.7.1/README.md
--rw-r--r--   0        0        0      108 2023-04-14 19:24:27.332493 pipen_annotate-0.7.1/pipen_annotate/__init__.py
--rw-r--r--   0        0        0     5914 2023-04-14 19:24:27.332493 pipen_annotate-0.7.1/pipen_annotate/annotate.py
--rw-r--r--   0        0        0    10972 2023-04-14 19:24:27.332493 pipen_annotate-0.7.1/pipen_annotate/sections.py
--rw-r--r--   0        0        0      958 2023-04-14 19:24:27.332493 pipen_annotate-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 pipen_annotate-0.7.1/setup.py
--rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 pipen_annotate-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-27 06:04:20.588439 pipen_annotate-0.7.2/LICENSE
+-rw-r--r--   0        0        0     1592 2023-05-27 06:04:20.588439 pipen_annotate-0.7.2/README.md
+-rw-r--r--   0        0        0      108 2023-05-27 06:04:20.588439 pipen_annotate-0.7.2/pipen_annotate/__init__.py
+-rw-r--r--   0        0        0     5914 2023-05-27 06:04:20.588439 pipen_annotate-0.7.2/pipen_annotate/annotate.py
+-rw-r--r--   0        0        0    11076 2023-05-27 06:04:20.588439 pipen_annotate-0.7.2/pipen_annotate/sections.py
+-rw-r--r--   0        0        0      958 2023-05-27 06:04:20.588439 pipen_annotate-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 pipen_annotate-0.7.2/setup.py
+-rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 pipen_annotate-0.7.2/PKG-INFO
```

### Comparing `pipen_annotate-0.7.1/LICENSE` & `pipen_annotate-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pipen_annotate-0.7.1/README.md` & `pipen_annotate-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pipen_annotate-0.7.1/pipen_annotate/annotate.py` & `pipen_annotate-0.7.2/pipen_annotate/annotate.py`

 * *Files identical despite different names*

### Comparing `pipen_annotate-0.7.1/pipen_annotate/sections.py` & `pipen_annotate-0.7.2/pipen_annotate/sections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
-from typing import List, MutableMapping
+from typing import List, Mapping, MutableMapping
 
 import re
 import textwrap
 import warnings
 
 from diot import Diot, OrderedDiot
 from pipen.defaults import ProcInputType
@@ -173,14 +173,29 @@
             )
             # continue
 
         if "default" not in parsed[key].attrs:
             parsed[key].attrs["default"] = value
 
 
+def _update_terms(base: Mapping, other: Mapping) -> None:
+    """Update the terms of base with the other terms."""
+    base = base.copy()
+    for key, value in other.items():
+        if key not in base:
+            base[key] = value
+        else:
+            if value.help:
+                base[key].help = value.help
+            base[key].attrs.update(value.attrs)
+            _update_terms(base[key].terms, value.terms)
+
+    return base
+
+
 class Section(ABC):
 
     def __init__(self, cls, name) -> None:
         self.name = name
         self._cls = cls
         self._lines: List[str] = []
 
@@ -256,27 +271,15 @@
     @classmethod
     def update_parsed(
         cls,
         base: str | List[str] | MutableMapping,
         other: str | List[str] | MutableMapping,
     ) -> str | List[str] | MutableMapping:
         """Update the parsed result with the other result."""
-        base = base.copy()
-        # arg, Diot(attrs, terms, help)
-        for key, value in other.items():
-            if key not in base:
-                base[key] = value
-                continue
-
-            base[key].attrs.update(value.attrs)
-            base[key].terms.update(value.terms)
-            if value.help:
-                base[key].help = value.help
-
-        return base
+        return _update_terms(base, other)
 
 
 class SectionInput(SectionItems):
 
     def parse(self) -> str | Diot | List[str]:
         parsed = super().parse()
         input_keys = self._cls.input
```

### Comparing `pipen_annotate-0.7.1/pyproject.toml` & `pipen_annotate-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-annotate"
-version = "0.7.1"
+version = "0.7.2"
 description = "Use docstring to annotate pipen processes"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.build]
 generate-setup-file = true
```

### Comparing `pipen_annotate-0.7.1/setup.py` & `pipen_annotate-0.7.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pipen>=0.9,<0.10']
 
 setup_kwargs = {
     'name': 'pipen-annotate',
-    'version': '0.7.1',
+    'version': '0.7.2',
     'description': 'Use docstring to annotate pipen processes',
     'long_description': '# pipen-annotate\n\nUse docstring to annotate [pipen](https://github.com/pwwang/pipen) processes\n\n## Installation\n\n```shell\npip install -U pipen-annotate\n```\n\n## Usage\n\n```python\nfrom pprint import pprint\nfrom pipen import Proc\nfrom pipen_annotate import annotate\n\n\nclass Process(Proc):\n    """Short description\n\n    Long description\n\n    Input:\n        infile: An input file\n        invar: An input variable\n\n    Output:\n        outfile: The output file\n\n    Envs:\n        ncores: Number of cores\n    """\n    input = "infile:file, invar"\n    output = "outfile:file:output.txt"\n    args = {\'ncores\': 1}\n\nannotated = annotate(Process)\n# prints:\n{\'Envs\': {\'ncores\': {\'attrs\': OrderedDiot([(\'default\', 1)]),\n                     \'help\': \'Number of cores\',\n                     \'terms\': OrderedDiot([])}},\n \'Input\': {\'infile\': {\'attrs\': {\'action\': \'extend\',\n                                \'itype\': \'file\',\n                                \'nargs\': \'+\'},\n                      \'help\': \'An input file\',\n                      \'terms\': OrderedDiot([])},\n           \'invar\': {\'attrs\': {\'action\': \'extend\',\n                               \'itype\': \'var\',\n                               \'nargs\': \'+\'},\n                     \'help\': \'An input variable\',\n                     \'terms\': OrderedDiot([])}},\n \'Output\': {\'outfile\': {\'attrs\': {\'default\': \'output.txt\',\n                                  \'otype\': \'file\'},\n                        \'help\': \'The output file\',\n                        \'terms\': OrderedDiot([])}},\n \'Summary\': {\'long\': \'Long description\\n\',\n             \'short\': \'Short description\'}}\n```\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pipen_annotate-0.7.1/PKG-INFO` & `pipen_annotate-0.7.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-annotate
-Version: 0.7.1
+Version: 0.7.2
 Summary: Use docstring to annotate pipen processes
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

