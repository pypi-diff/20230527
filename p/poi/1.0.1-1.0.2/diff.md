# Comparing `tmp/poi-1.0.1.tar.gz` & `tmp/poi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poi-1.0.1.tar", max compression
+gzip compressed data, was "poi-1.0.2.tar", max compression
```

## Comparing `poi-1.0.1.tar` & `poi-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1066 2023-03-13 03:34:22.084937 poi-1.0.1/LICENSE
--rw-r--r--   0        0        0     1817 2023-03-13 03:34:22.085087 poi-1.0.1/README.md
--rw-r--r--   0        0        0      241 2023-03-13 07:10:37.979782 poi-1.0.1/poi/__init__.py
--rw-r--r--   0        0        0      900 2023-03-13 03:34:22.097492 poi-1.0.1/poi/book.py
--rw-r--r--   0        0        0    13901 2023-03-13 07:10:08.109600 poi-1.0.1/poi/nodes.py
--rw-r--r--   0        0        0        0 2023-03-13 03:34:22.097815 poi-1.0.1/poi/py.typed
--rw-r--r--   0        0        0     1968 2023-03-13 03:34:22.098004 poi-1.0.1/poi/sheet.py
--rw-r--r--   0        0        0      583 2023-03-13 03:34:22.098205 poi-1.0.1/poi/utils.py
--rw-r--r--   0        0        0        0 2023-03-13 03:34:22.098238 poi-1.0.1/poi/visitors/__init__.py
--rw-r--r--   0        0        0      943 2023-03-13 03:34:22.098389 poi-1.0.1/poi/visitors/printer.py
--rw-r--r--   0        0        0     4166 2023-03-13 03:34:22.098702 poi-1.0.1/poi/visitors/writer.py
--rw-r--r--   0        0        0     2363 2023-03-13 03:34:22.098882 poi-1.0.1/poi/writer.py
--rw-r--r--   0        0        0     1235 2023-03-13 07:10:37.980039 poi-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2563 1970-01-01 00:00:00.000000 poi-1.0.1/setup.py
--rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 poi-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-03-13 03:34:22.084937 poi-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1817 2023-03-13 03:34:22.085087 poi-1.0.2/README.md
+-rw-r--r--   0        0        0      241 2023-05-27 12:42:49.733142 poi-1.0.2/poi/__init__.py
+-rw-r--r--   0        0        0      900 2023-03-13 03:34:22.097492 poi-1.0.2/poi/book.py
+-rw-r--r--   0        0        0    13901 2023-03-13 07:10:08.109600 poi-1.0.2/poi/nodes.py
+-rw-r--r--   0        0        0        0 2023-03-13 03:34:22.097815 poi-1.0.2/poi/py.typed
+-rw-r--r--   0        0        0     1968 2023-03-13 03:34:22.098004 poi-1.0.2/poi/sheet.py
+-rw-r--r--   0        0        0      583 2023-03-13 03:34:22.098205 poi-1.0.2/poi/utils.py
+-rw-r--r--   0        0        0        0 2023-03-13 03:34:22.098238 poi-1.0.2/poi/visitors/__init__.py
+-rw-r--r--   0        0        0      943 2023-03-13 03:34:22.098389 poi-1.0.2/poi/visitors/printer.py
+-rw-r--r--   0        0        0     4166 2023-03-13 03:34:22.098702 poi-1.0.2/poi/visitors/writer.py
+-rw-r--r--   0        0        0     2742 2023-05-27 12:42:49.733465 poi-1.0.2/poi/writer.py
+-rw-r--r--   0        0        0     1235 2023-05-27 12:42:49.733781 poi-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2563 1970-01-01 00:00:00.000000 poi-1.0.2/setup.py
+-rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 poi-1.0.2/PKG-INFO
```

### Comparing `poi-1.0.1/LICENSE` & `poi-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poi-1.0.1/README.md` & `poi-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `poi-1.0.1/poi/book.py` & `poi-1.0.2/poi/book.py`

 * *Files identical despite different names*

### Comparing `poi-1.0.1/poi/nodes.py` & `poi-1.0.2/poi/nodes.py`

 * *Files identical despite different names*

### Comparing `poi-1.0.1/poi/sheet.py` & `poi-1.0.2/poi/sheet.py`

 * *Files identical despite different names*

### Comparing `poi-1.0.1/poi/utils.py` & `poi-1.0.2/poi/utils.py`

 * *Files identical despite different names*

### Comparing `poi-1.0.1/poi/visitors/printer.py` & `poi-1.0.2/poi/visitors/printer.py`

 * *Files identical despite different names*

### Comparing `poi-1.0.1/poi/visitors/writer.py` & `poi-1.0.2/poi/visitors/writer.py`

 * *Files identical despite different names*

### Comparing `poi-1.0.1/poi/writer.py` & `poi-1.0.2/poi/writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from __future__ import annotations
 from io import BytesIO
 from typing import Protocol, List, Any, Optional
 
 import xlsxwriter
 from xlsxwriter.format import Format
 from xlsxwriter.worksheet import Worksheet
+import json
+import logging
+
+logger = logging.getLogger(__name__)
 
 
 class WorkBook(Protocol):
     def add_format(self, format: dict[str, Any]) -> Format:
         ...
 
     def worksheets(self) -> List[Worksheet]:
@@ -51,23 +55,31 @@
     ) -> None:
         self.workbook = workbook
         self.worksheet = worksheet
         self.global_format = (
             self.workbook.add_format(global_format) if global_format else None
         )
         self.global_format_dict = global_format or {}
+        self.formats = {}
 
     def _calc_format(self, cell_format: Any) -> Any:
-        if cell_format is None:
-            cell_format = self.global_format
+        if not cell_format:
+            return self.global_format
         elif isinstance(cell_format, dict):
-            cell_format = self.workbook.add_format(
-                {**self.global_format_dict, **cell_format}
-            )
-        return cell_format
+            fmt_key = json.dumps(cell_format, sort_keys=True)
+            fmt = self.formats.get(fmt_key)
+            if not fmt:
+                fmt = self.workbook.add_format(
+                    {**self.global_format_dict, **cell_format}
+                )
+                self.formats[fmt_key] = fmt
+            return fmt
+        else:
+            logger.error(f"cell_format must be dict, got {cell_format}")
+            return self.global_format
 
     def _path_args(self, args: Any) -> Any:
         last_arg = args[-1]
         if isinstance(last_arg, dict):
             args = list(args[:-1]) + [self._calc_format(last_arg)]
         return args
```

### Comparing `poi-1.0.1/pyproject.toml` & `poi-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poi"
-version = "1.0.1"
+version = "1.0.2"
 description = "Write Excel XLSX declaratively."
 authors = ["Ryan Wang <hwwangwang@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/baoshishu/poi"
 repository = "https://github.com/baoshishu/poi"
 documentation = "https://baoshishu.github.io/poi/"
```

### Comparing `poi-1.0.1/setup.py` & `poi-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['xlsxwriter>=1.1,<2.0']
 
 setup_kwargs = {
     'name': 'poi',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'Write Excel XLSX declaratively.',
     'long_description': '# Poi: Make creating Excel XLSX files fun again.\n\n![travis](https://travis-ci.org/baoshishu/poi.svg?branch=master)\n\nPoi helps you write Excel sheet in a declarative way, ensuring you have a better Excel writing experience.\n\nIt only supports Python 3.7+.\n\n[Documentation](https://ryanwang520.github.io/poi/)\n\n## Installation\n\n```bash\npip install poi\n```\n\n## Quick start\n\n### Create a sheet object and write to a file.\n\n```python\nfrom poi import Sheet, Cell\nsheet = Sheet(\n    root=Cell("hello world")\n)\n\nsheet.write(\'hello.xlsx\')\n```\n\n![hello](https://github.com/baoshishu/poi/raw/master/docs/assets/hello.png)\n\nSee, it\'s pretty simple and clear.\n\n\n### Sample for rendering a simple table.\n\n```python\nfrom typing import NamedTuple\nfrom datetime import datetime\nimport random\n\nfrom poi import Sheet, Table\n\n\nclass Product(NamedTuple):\n    name: str\n    desc: str\n    price: int\n    created_at: datetime\n    img: str\n\n\ndata = [\n    Product(\n        name=f"prod {i}",\n        desc=f"desc {i}",\n        price=random.randint(1, 100),\n        created_at=datetime.now(),\n        img="./docs/assets/product.jpg",\n    )\n    for i in range(5)\n]\ncolumns = [\n    {\n        "type": "image",\n        "attr": "img",\n        "title": "Product Image",\n        "options": {"x_scale": 0.27, "y_scale": 0.25},\n    },\n    ("name", "Name"),\n    ("desc", "Description"),\n    ("price", "Price"),\n    ("created_at", "Create Time"),\n]\nsheet = Sheet(\n    root=Table(\n        data=data,\n        columns=columns,\n        row_height=80,\n        cell_style={\n            "color: red": lambda record, col: col.attr == "price" and record.price > 50\n        },\n        date_format="yyyy-mm-dd",\n        align="center",\n        border=1,\n    )\n)\nsheet.write("table.xlsx")\n```\n\n![table](https://github.com/baoshishu/poi/raw/master/docs/assets/table.png)\n',
     'author': 'Ryan Wang',
     'author_email': 'hwwangwang@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/baoshishu/poi',
```

### Comparing `poi-1.0.1/PKG-INFO` & `poi-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Write Excel XLSX declaratively.
 Home-page: https://github.com/baoshishu/poi
 License: MIT
 Keywords: xlsx,xlswriter,excel,declarative
 Author: Ryan Wang
 Author-email: hwwangwang@gmail.com
 Requires-Python: >=3.7,<4.0
```

