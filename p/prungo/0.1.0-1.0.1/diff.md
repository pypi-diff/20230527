# Comparing `tmp/prungo-0.1.0.tar.gz` & `tmp/prungo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prungo-0.1.0.tar", max compression
+gzip compressed data, was "prungo-1.0.1.tar", max compression
```

## Comparing `prungo-0.1.0.tar` & `prungo-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1523 2023-05-27 13:13:05.781145 prungo-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-05-27 13:13:05.781145 prungo-0.1.0/prungo/__init__.py
--rw-r--r--   0        0        0      622 2023-05-27 14:32:21.243477 prungo-0.1.0/prungo/decorators.py
--rw-r--r--   0        0        0       74 2023-05-27 14:30:25.820358 prungo-0.1.0/prungo/main.py
--rw-r--r--   0        0        0      548 2023-05-27 13:42:12.444074 prungo-0.1.0/prungo/models.py
--rw-r--r--   0        0        0      723 2023-05-27 14:20:13.668280 prungo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       60 2023-05-27 13:13:05.781145 prungo-0.1.0/README.md
--rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 prungo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-05-27 14:48:22.893842 prungo-1.0.1/LICENSE
+-rw-r--r--   0        0        0       58 2023-05-27 14:48:22.893842 prungo-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 14:48:22.893842 prungo-1.0.1/prungo/__init__.py
+-rw-r--r--   0        0        0      599 2023-05-27 14:48:22.893842 prungo-1.0.1/prungo/decorators.py
+-rw-r--r--   0        0        0       71 2023-05-27 14:48:22.893842 prungo-1.0.1/prungo/main.py
+-rw-r--r--   0        0        0      521 2023-05-27 14:48:22.893842 prungo-1.0.1/prungo/models.py
+-rw-r--r--   0        0        0      693 2023-05-27 14:48:46.682072 prungo-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 prungo-1.0.1/setup.py
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 prungo-1.0.1/PKG-INFO
```

### Comparing `prungo-0.1.0/LICENSE` & `prungo-1.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Copyright (c) <year>, <copyright holder>
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of the copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+Copyright (c) <year>, <copyright holder>
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of the copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `prungo-0.1.0/prungo/decorators.py` & `prungo-1.0.1/prungo/decorators.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import logging
-from functools import wraps
-from typing import Callable, ParamSpec, TypeVar
-
-from prungo.models import logger_type
-
-P = ParamSpec("P")
-T = TypeVar("T")
-
-
-def log_call(log: logger_type = logging.getLogger("util"), /):
-    """log to default logger whenever decorated function is called"""
-
-    def decorator(method: Callable[P, T], /):
-        @wraps(method)
-        def func(*args: P.args, **kwargs: P.kwargs):
-            log_text = f" {method.__name__} "
-            log.info(f"{log_text :-^50}")
-            return method(*args, **kwargs)
-
-        return func
-
-    return decorator
+import logging
+from functools import wraps
+from typing import Callable, ParamSpec, TypeVar
+
+from prungo.models import logger_type
+
+P = ParamSpec("P")
+T = TypeVar("T")
+
+
+def log_call(log: logger_type = logging.getLogger("util"), /):
+    """log to default logger whenever decorated function is called"""
+
+    def decorator(method: Callable[P, T], /):
+        @wraps(method)
+        def func(*args: P.args, **kwargs: P.kwargs):
+            log_text = f" {method.__name__} "
+            log.info(f"{log_text :-^50}")
+            return method(*args, **kwargs)
+
+        return func
+
+    return decorator
```

### Comparing `prungo-0.1.0/prungo/models.py` & `prungo-1.0.1/prungo/models.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from typing import Any, Protocol
-
-
-class logger_type(Protocol):
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
-        ...
-
-    def debug(self, text: str) -> None:
-        ...
-
-    def info(self, text: str) -> None:
-        ...
-
-    def warning(self, text: str) -> None:
-        ...
-
-    def error(self, text: str) -> None:
-        ...
-
-    def critical(self, text: str) -> None:
-        ...
-
-    def traceback(self, text: str) -> None:
-        ...
-
-    def contextualise(self, text: str) -> None:
-        ...
+from typing import Any, Protocol
+
+
+class logger_type(Protocol):
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+        ...
+
+    def debug(self, text: str) -> None:
+        ...
+
+    def info(self, text: str) -> None:
+        ...
+
+    def warning(self, text: str) -> None:
+        ...
+
+    def error(self, text: str) -> None:
+        ...
+
+    def critical(self, text: str) -> None:
+        ...
+
+    def traceback(self, text: str) -> None:
+        ...
+
+    def contextualise(self, text: str) -> None:
+        ...
```

### Comparing `prungo-0.1.0/PKG-INFO` & `prungo-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: prungo
-Version: 0.1.0
+Version: 1.0.1
 Summary: A package for basic utility functions/classes
 Home-page: https://github.com/c-prungo/prungo-util
 License: MIT
 Author: c-prungo
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Project-URL: Repository, https://github.com/c-prungo/prungo-util
 Description-Content-Type: text/markdown
 
 # prungo-util
 utility package for importing into projects
```

