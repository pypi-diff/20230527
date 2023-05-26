# Comparing `tmp/itkwasm_compress_stringify-0.4.5.tar.gz` & `tmp/itkwasm_compress_stringify-0.5.0.tar.gz`

## Comparing `itkwasm_compress_stringify-0.4.5.tar` & `itkwasm_compress_stringify-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/docs/Makefile
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/docs/conf.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/docs/make.bat
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/docs/requirements.txt
--rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/docs/_static/favicon.png
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/docs/_static/logo.svg
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/_version.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/compress_stringify.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/compress_stringify_async.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/parse_string_decompress.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/parse_string_decompress_async.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/test/test_compress_stringify_emscripten.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/test/test_compress_stringify_wasi.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/.gitignore
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/README.md
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/docs/Makefile
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/docs/conf.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/docs/make.bat
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/docs/requirements.txt
+-rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/docs/_static/favicon.png
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/docs/_static/logo.svg
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/_version.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/compress_stringify.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/compress_stringify_async.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/parse_string_decompress.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/parse_string_decompress_async.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/test/test_compress_stringify_emscripten.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/test/test_compress_stringify_wasi.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/.gitignore
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/README.md
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/PKG-INFO
```

### Comparing `itkwasm_compress_stringify-0.4.5/docs/Makefile` & `itkwasm_compress_stringify-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.4.5/docs/conf.py` & `itkwasm_compress_stringify-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.4.5/docs/make.bat` & `itkwasm_compress_stringify-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.4.5/docs/_static/favicon.png` & `itkwasm_compress_stringify-0.5.0/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.4.5/docs/_static/logo.svg` & `itkwasm_compress_stringify-0.5.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/compress_stringify.py` & `itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/compress_stringify_async.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Generated file. Do not edit.
 
-from typing import Optional
+import os
+from typing import Dict, Tuple, Optional, List
 
 from itkwasm import (
     environment_dispatch,
     BinaryStream,
 )
 
-def compress_stringify(
+async def compress_stringify_async(
     input: bytes,
     stringify: bool = False,
     compression_level: int = 3,
     data_url_prefix: str = "data:base64,",
 ) -> bytes:
     """Given a binary, compress and optionally base64 encode.
 
@@ -26,10 +27,10 @@
 
     :param data_url_prefix: dataURL prefix
     :type  data_url_prefix: str
 
     :return: Output compressed binary
     :rtype:  bytes
     """
-    func = environment_dispatch("itkwasm_compress_stringify", "compress_stringify")
-    output = func(input, stringify=stringify, compression_level=compression_level, data_url_prefix=data_url_prefix)
+    func = environment_dispatch("itkwasm_compress_stringify", "compress_stringify_async")
+    output = await func(input, stringify=stringify, compression_level=compression_level, data_url_prefix=data_url_prefix)
     return output
```

### Comparing `itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/compress_stringify_async.py` & `itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/compress_stringify.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Generated file. Do not edit.
 
-from typing import Optional
+import os
+from typing import Dict, Tuple, Optional, List
 
 from itkwasm import (
     environment_dispatch,
     BinaryStream,
 )
 
-async def compress_stringify_async(
+def compress_stringify(
     input: bytes,
     stringify: bool = False,
     compression_level: int = 3,
     data_url_prefix: str = "data:base64,",
 ) -> bytes:
     """Given a binary, compress and optionally base64 encode.
 
@@ -26,10 +27,10 @@
 
     :param data_url_prefix: dataURL prefix
     :type  data_url_prefix: str
 
     :return: Output compressed binary
     :rtype:  bytes
     """
-    func = environment_dispatch("itkwasm_compress_stringify", "compress_stringify_async")
-    output = await func(input, stringify=stringify, compression_level=compression_level, data_url_prefix=data_url_prefix)
+    func = environment_dispatch("itkwasm_compress_stringify", "compress_stringify")
+    output = func(input, stringify=stringify, compression_level=compression_level, data_url_prefix=data_url_prefix)
     return output
```

### Comparing `itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/parse_string_decompress.py` & `itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/parse_string_decompress.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Generated file. Do not edit.
 
-from typing import Optional
+import os
+from typing import Dict, Tuple, Optional, List
 
 from itkwasm import (
     environment_dispatch,
     BinaryStream,
 )
 
 def parse_string_decompress(
```

### Comparing `itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/parse_string_decompress_async.py` & `itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/parse_string_decompress_async.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Generated file. Do not edit.
 
-from typing import Optional
+import os
+from typing import Dict, Tuple, Optional, List
 
 from itkwasm import (
     environment_dispatch,
     BinaryStream,
 )
 
 async def parse_string_decompress_async(
```

### Comparing `itkwasm_compress_stringify-0.4.5/test/test_compress_stringify_emscripten.py` & `itkwasm_compress_stringify-0.5.0/test/test_compress_stringify_emscripten.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.4.5/test/test_compress_stringify_wasi.py` & `itkwasm_compress_stringify-0.5.0/test/test_compress_stringify_wasi.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.4.5/pyproject.toml` & `itkwasm_compress_stringify-0.5.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -29,19 +29,24 @@
   "webassembly",
   "wasi",
   "emscripten",
 ]
 
 requires-python = ">=3.7"
 dependencies = [
-    "itkwasm >= 1.0.b97",
+    "itkwasm >= 1.0.b105",
     "itkwasm-compress-stringify-wasi; sys_platform != \"emscripten\"",
     "itkwasm-compress-stringify-emscripten; sys_platform == \"emscripten\"",
 ]
 
+[project.urls]
+Home = "https://itk-wasm-compress-stringify-python-docs.on.fleek.co"
+Source = "https://github.com/InsightSoftwareConsortium/itk-wasm"
+Issues = "https://github.com/InsightSoftwareConsortium/itk-wasm/issues"
+
 [tool.hatch.version]
 path = "itkwasm_compress_stringify/_version.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-pyodide",
```

### Comparing `itkwasm_compress_stringify-0.4.5/PKG-INFO` & `itkwasm_compress_stringify-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 Metadata-Version: 2.1
 Name: itkwasm-compress-stringify
-Version: 0.4.5
+Version: 0.5.0
+Project-URL: Home, https://itk-wasm-compress-stringify-python-docs.on.fleek.co
+Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
+Project-URL: Issues, https://github.com/InsightSoftwareConsortium/itk-wasm/issues
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
 Classifier: Environment :: WebAssembly :: Emscripten
 Classifier: Environment :: WebAssembly :: WASI
 Classifier: Intended Audience :: Developers
@@ -17,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: itkwasm-compress-stringify-emscripten; sys_platform == 'emscripten'
 Requires-Dist: itkwasm-compress-stringify-wasi; sys_platform != 'emscripten'
-Requires-Dist: itkwasm>=1.0.b97
+Requires-Dist: itkwasm>=1.0.b105
 Description-Content-Type: text/markdown
 
 # itkwasm-compress-stringify
 
 [![PyPI version](https://badge.fury.io/py/itkwasm-compress-stringify.svg)](https://badge.fury.io/py/itkwasm-compress-stringify)
 
 Zstandard compression and decompression and base64 encoding and decoding in WebAssembly.
```

