# Comparing `tmp/quivr-0.3.3.tar.gz` & `tmp/quivr-0.3.4.tar.gz`

## Comparing `quivr-0.3.3.tar` & `quivr-0.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/__version__.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/attributes.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/concat.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/defragment.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/errors.py
--rw-r--r--   0        0        0    25837 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/fields.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/indexing.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/matrix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/py.typed
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/schemagraph.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/streaming.py
--rw-r--r--   0        0        0    27450 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/tables.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/validators.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.3.3/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.3.3/LICENSE
--rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 quivr-0.3.3/README.md
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 quivr-0.3.3/pyproject.toml
--rw-r--r--   0        0        0    11097 2020-02-02 00:00:00.000000 quivr-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/__version__.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/attributes.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/concat.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/defragment.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/errors.py
+-rw-r--r--   0        0        0    25951 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/fields.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/indexing.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/py.typed
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/schemagraph.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/streaming.py
+-rw-r--r--   0        0        0    27561 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/tables.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/validators.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.3.4/LICENSE
+-rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 quivr-0.3.4/README.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 quivr-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0    11136 2020-02-02 00:00:00.000000 quivr-0.3.4/PKG-INFO
```

### Comparing `quivr-0.3.3/quivr/__init__.py` & `quivr-0.3.4/quivr/__init__.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.3/quivr/attributes.py` & `quivr-0.3.4/quivr/attributes.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.3/quivr/concat.py` & `quivr-0.3.4/quivr/concat.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.3/quivr/fields.py` & `quivr-0.3.4/quivr/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from typing import TYPE_CHECKING, Generic, Optional, TypeAlias, TypeVar, Union
+import sys
+if sys.version_info < (3, 10):
+    from typing_extensions import TypeAlias
+else:
+    from typing import TypeAlias
+from typing import TYPE_CHECKING, Generic, Optional, TypeVar, Union
 
 import pyarrow as pa
 
 from . import validators
 
 if TYPE_CHECKING:
     from .tables import Table
```

### Comparing `quivr-0.3.3/quivr/indexing.py` & `quivr-0.3.4/quivr/indexing.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.3/quivr/matrix.py` & `quivr-0.3.4/quivr/matrix.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.3/quivr/schemagraph.py` & `quivr-0.3.4/quivr/schemagraph.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.3/quivr/tables.py` & `quivr-0.3.4/quivr/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 import os
 import warnings
 from io import IOBase
-from typing import Any, ClassVar, Optional, Self, Union
+import sys
+
+if sys.version_info < (3, 11):
+    from typing_extensions import Self
+else:
+    from typing import Self
+
+from typing import Any, ClassVar, Optional, Union
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.csv
 import pyarrow.feather
```

### Comparing `quivr-0.3.3/quivr/validators.py` & `quivr-0.3.4/quivr/validators.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.3/LICENSE` & `quivr-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.3.3/README.md` & `quivr-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `quivr-0.3.3/pyproject.toml` & `quivr-0.3.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 [project]
 name = "quivr"
 description = "Container library for working with tabular Arrow data"
 readme = "README.md"
 authors = [
    { name = "Spencer Nelson", email = "spencer@spencerwnelson.com" }
 ]
-requires-python = ">= 3.11"
+requires-python = ">= 3.9"
 dependencies = [
   "pandas",
   "pyarrow",
   "numpy",
   "mmh3",
+  "typing_extensions>=4.0.0"
 ]
 dynamic = [ "version" ]
 
 [project.urls]
 Source = "https://github.com/spenczar/quivr"
 
 [tool.hatch.build.targets.sdist]
@@ -35,14 +36,28 @@
   "mypy",
   "pandas-stubs",
   "pytest",
   "pytest-benchmark",
   "ruff",
 ]
 
+[tool.hatch.envs.py310]
+python = "3.10"
+dependencies = [
+  "pytest",
+  "pytest-benchmark",
+]
+
+[tool.hatch.envs.py39]
+python = "3.9"
+dependencies = [
+  "pytest",
+  "pytest-benchmark",
+]
+
 [tool.hatch.envs.default.scripts]
 check = [
   "lint",
   "typecheck",
   "test",
 ]
 fix = [
```

### Comparing `quivr-0.3.3/PKG-INFO` & `quivr-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: quivr
-Version: 0.3.3
+Version: 0.3.4
 Summary: Container library for working with tabular Arrow data
 Project-URL: Source, https://github.com/spenczar/quivr
 Author-email: Spencer Nelson <spencer@spencerwnelson.com>
 License-File: LICENSE
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Requires-Dist: mmh3
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyarrow
+Requires-Dist: typing-extensions>=4.0.0
 Description-Content-Type: text/markdown
 
 # quivr
 
 Quivr is a Python library which provides great containers for Arrow data.
 
 Quivr's `Table`s are like DataFrames, but with strict schemas to
```

