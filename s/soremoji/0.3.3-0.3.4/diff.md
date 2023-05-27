# Comparing `tmp/soremoji-0.3.3.tar.gz` & `tmp/soremoji-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soremoji-0.3.3.tar", max compression
+gzip compressed data, was "soremoji-0.3.4.tar", max compression
```

## Comparing `soremoji-0.3.3.tar` & `soremoji-0.3.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-05-27 05:02:29.029871 soremoji-0.3.3/LICENSE
--rw-r--r--   0        0        0     5411 2023-05-27 05:02:29.029871 soremoji-0.3.3/README.md
--rw-r--r--   0        0        0      726 2023-05-27 05:02:29.029871 soremoji-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      111 2023-05-27 05:02:29.029871 soremoji-0.3.3/soremoji/__init__.py
--rw-r--r--   0        0        0       60 2023-05-27 05:02:29.029871 soremoji-0.3.3/soremoji/__main__.py
--rw-r--r--   0        0        0     1475 2023-05-27 05:02:29.029871 soremoji-0.3.3/soremoji/cli.py
--rw-r--r--   0        0        0     1575 2023-05-27 05:02:29.029871 soremoji-0.3.3/soremoji/command.py
--rw-r--r--   0        0        0     7195 2023-05-27 05:02:29.029871 soremoji-0.3.3/soremoji/emoticon.py
--rw-r--r--   0        0        0     1825 2023-05-27 05:02:29.029871 soremoji-0.3.3/soremoji/feature.py
--rw-r--r--   0        0        0     5932 1970-01-01 00:00:00.000000 soremoji-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-27 05:10:50.331228 soremoji-0.3.4/LICENSE
+-rw-r--r--   0        0        0     5411 2023-05-27 05:10:50.331228 soremoji-0.3.4/README.md
+-rw-r--r--   0        0        0      726 2023-05-27 05:10:50.331228 soremoji-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-05-27 05:10:50.331228 soremoji-0.3.4/soremoji/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-27 05:10:50.331228 soremoji-0.3.4/soremoji/__main__.py
+-rw-r--r--   0        0        0     1476 2023-05-27 05:10:50.331228 soremoji-0.3.4/soremoji/cli.py
+-rw-r--r--   0        0        0     1578 2023-05-27 05:10:50.331228 soremoji-0.3.4/soremoji/command.py
+-rw-r--r--   0        0        0     7195 2023-05-27 05:10:50.331228 soremoji-0.3.4/soremoji/emoticon.py
+-rw-r--r--   0        0        0     1827 2023-05-27 05:10:50.331228 soremoji-0.3.4/soremoji/feature.py
+-rw-r--r--   0        0        0     5932 1970-01-01 00:00:00.000000 soremoji-0.3.4/PKG-INFO
```

### Comparing `soremoji-0.3.3/LICENSE` & `soremoji-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `soremoji-0.3.3/README.md` & `soremoji-0.3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   - repo: https://github.com/psf/black
     rev: 22.6.0
     hooks:
       - id: black
         stages: [commit]
 
   - repo: https://github.com/netsora/soremoji
-    rev: 0.3.3
+    rev: 0.3.4
     hooks:
       - id: soremoji
         stages: [pre-commit-msg]
 ```
 
 ## 使用
```

### Comparing `soremoji-0.3.3/pyproject.toml` & `soremoji-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "soremoji"
-version = "0.3.3"
+version = "0.3.4"
 description = "自维护的 gitmoji-cli，做了部分更改"
 authors = ["mute. <mute231010@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `soremoji-0.3.3/soremoji/cli.py` & `soremoji-0.3.4/soremoji/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from argparse import REMAINDER, ArgumentParser
-from typing import Any, Callable, List, Optional
+from typing import Any, List, Callable, Optional
 
-from command import (
-    handle_commit,
+from .command import (
     handle_hook,
     handle_list,
-    handle_no_subcommand,
+    handle_commit,
     handle_search,
+    handle_no_subcommand,
 )
 
 parser = ArgumentParser("soremoji", description="Simple gitmoji-cli written in python")
 parser.set_defaults(func=handle_no_subcommand)
 _subparsers = parser.add_subparsers(title="subcommands")
 
 # hook / 钩子
```

### Comparing `soremoji-0.3.3/soremoji/command.py` & `soremoji-0.3.4/soremoji/command.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import contextlib
 import shlex
+import contextlib
 import subprocess
 from pathlib import Path
-from typing import Callable, List, Optional
+from typing import List, Callable, Optional
+
+from sorampt import Choice, ListPrompt, CancelledError
 
-from emoticon import EMOJIS
-from feature import prompt, prompt_emoji
-from sorampt import CancelledError, Choice, ListPrompt
+from .emoticon import EMOJIS
+from .feature import prompt, prompt_emoji
 
 
 def handle_no_subcommand(**_):
     with contextlib.suppress(CancelledError):
         result = ListPrompt[Callable[..., None]](
             "What do you want to do?",
             [
```

### Comparing `soremoji-0.3.3/soremoji/emoticon.py` & `soremoji-0.3.4/soremoji/emoticon.py`

 * *Files identical despite different names*

### Comparing `soremoji-0.3.3/soremoji/feature.py` & `soremoji-0.3.4/soremoji/feature.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import contextlib
 import re
+import contextlib
 from dataclasses import dataclass
 from typing import Optional, cast
 
-from emoticon import EMOJIS, Emoji
-from sorampt import Choice, InputPrompt, ListPrompt
+from sorampt import Choice, ListPrompt, InputPrompt
+
+from .emoticon import EMOJIS, Emoji
 
 MESSAGE_REGEX = re.compile(r"^:(?P<emoji>\w+):(?P<message>[\s\S]+)$")
 
 
 @dataclass
 class Message:
     emoji: Optional[Emoji] = None
```

### Comparing `soremoji-0.3.3/PKG-INFO` & `soremoji-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soremoji
-Version: 0.3.3
+Version: 0.3.4
 Summary: 自维护的 gitmoji-cli，做了部分更改
 License: MIT
 Author: mute.
 Author-email: mute231010@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -39,15 +39,15 @@
   - repo: https://github.com/psf/black
     rev: 22.6.0
     hooks:
       - id: black
         stages: [commit]
 
   - repo: https://github.com/netsora/soremoji
-    rev: 0.3.3
+    rev: 0.3.4
     hooks:
       - id: soremoji
         stages: [pre-commit-msg]
 ```
 
 ## 使用
```

