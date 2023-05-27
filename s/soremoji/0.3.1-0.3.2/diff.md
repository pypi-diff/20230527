# Comparing `tmp/soremoji-0.3.1.tar.gz` & `tmp/soremoji-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soremoji-0.3.1.tar", max compression
+gzip compressed data, was "soremoji-0.3.2.tar", max compression
```

## Comparing `soremoji-0.3.1.tar` & `soremoji-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-05-13 11:46:17.757243 soremoji-0.3.1/LICENSE
--rw-r--r--   0        0        0     5411 2023-05-13 11:46:17.757243 soremoji-0.3.1/README.md
--rw-r--r--   0        0        0      369 2023-05-13 11:46:17.757243 soremoji-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      114 2023-05-13 11:46:17.757243 soremoji-0.3.1/soremoji/__init__.py
--rw-r--r--   0        0        0     1441 2023-05-13 11:46:17.757243 soremoji-0.3.1/soremoji/cli.py
--rw-r--r--   0        0        0     1575 2023-05-13 11:46:17.757243 soremoji-0.3.1/soremoji/command.py
--rw-r--r--   0        0        0     7195 2023-05-13 11:46:17.757243 soremoji-0.3.1/soremoji/emoji.py
--rw-r--r--   0        0        0     1824 2023-05-13 11:46:17.757243 soremoji-0.3.1/soremoji/feature.py
--rw-r--r--   0        0        0     5932 1970-01-01 00:00:00.000000 soremoji-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-27 04:26:10.606137 soremoji-0.3.2/LICENSE
+-rw-r--r--   0        0        0     5411 2023-05-27 04:26:10.606137 soremoji-0.3.2/README.md
+-rw-r--r--   0        0        0      369 2023-05-27 04:26:10.606137 soremoji-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-05-27 04:26:10.606137 soremoji-0.3.2/soremoji/__init__.py
+-rw-r--r--   0        0        0       60 2023-05-27 04:26:10.606137 soremoji-0.3.2/soremoji/__main__.py
+-rw-r--r--   0        0        0     1475 2023-05-27 04:26:10.606137 soremoji-0.3.2/soremoji/cli.py
+-rw-r--r--   0        0        0     1575 2023-05-27 04:26:10.606137 soremoji-0.3.2/soremoji/command.py
+-rw-r--r--   0        0        0     7195 2023-05-27 04:26:10.606137 soremoji-0.3.2/soremoji/emoticon.py
+-rw-r--r--   0        0        0     1825 2023-05-27 04:26:10.606137 soremoji-0.3.2/soremoji/feature.py
+-rw-r--r--   0        0        0     5932 1970-01-01 00:00:00.000000 soremoji-0.3.2/PKG-INFO
```

### Comparing `soremoji-0.3.1/LICENSE` & `soremoji-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soremoji-0.3.1/README.md` & `soremoji-0.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   - repo: https://github.com/psf/black
     rev: 22.6.0
     hooks:
       - id: black
         stages: [commit]
 
   - repo: https://github.com/netsora/soremoji
-    rev: 0.3.1
+    rev: 0.3.2
     hooks:
       - id: soremoji
         stages: [pre-commit-msg]
 ```
 
 ## 使用
```

### Comparing `soremoji-0.3.1/soremoji/cli.py` & `soremoji-0.3.2/soremoji/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from argparse import REMAINDER, ArgumentParser
 from typing import Any, Callable, List, Optional
 
-from .command import (
+from command import (
     handle_commit,
     handle_hook,
     handle_list,
     handle_no_subcommand,
     handle_search,
 )
 
-parser = ArgumentParser("soremoji", description="Simple gitmoji cli written in python")
+parser = ArgumentParser("soremoji", description="Simple gitmoji-cli written in python")
 parser.set_defaults(func=handle_no_subcommand)
 _subparsers = parser.add_subparsers(title="subcommands")
 
-# hook
+# hook / 钩子
 hook_parser = _subparsers.add_parser("hook", help="Run as a git hook.")
 hook_parser.add_argument("commit_msg_file", help="Path to the commit message file")
 hook_parser.set_defaults(func=handle_hook)
 
-# commit
-commit_parser = _subparsers.add_parser("commit", help="Start to commit changes.")
+# commit / 提交
+commit_parser = _subparsers.add_parser("commit", help="Start to commit changes")
 commit_parser.add_argument("-e", "--emoji", help="Emoji to use")
 commit_parser.add_argument("-m", "--message", help="Commit message")
 commit_parser.add_argument(
     "--", nargs=REMAINDER, help="Argument to pass to the git", dest="args"
 )
 commit_parser.set_defaults(func=handle_commit)
 
-# list
+# list / 列表
 list_parser = _subparsers.add_parser("list", help="List all available emoji.")
 list_parser.set_defaults(func=handle_list)
 
-# search
+# search / 搜索
 search_parser = _subparsers.add_parser("search", help="Search for an emoji.")
 search_parser.set_defaults(func=handle_search)
 
 
 def main(argv: Optional[List[str]] = None):
     result = parser.parse_args(argv)
     result = vars(result)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `soremoji-0.3.1/soremoji/command.py` & `soremoji-0.3.2/soremoji/command.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import contextlib
 import shlex
 import subprocess
 from pathlib import Path
 from typing import Callable, List, Optional
 
+from emoticon import EMOJIS
+from feature import prompt, prompt_emoji
 from sorampt import CancelledError, Choice, ListPrompt
 
-from .emoji import EMOJIS
-from .feature import prompt, prompt_emoji
-
 
 def handle_no_subcommand(**_):
     with contextlib.suppress(CancelledError):
         result = ListPrompt[Callable[..., None]](
             "What do you want to do?",
             [
                 Choice("Start to commit changes", handle_commit),
```

### Comparing `soremoji-0.3.1/soremoji/emoji.py` & `soremoji-0.3.2/soremoji/emoticon.py`

 * *Files identical despite different names*

### Comparing `soremoji-0.3.1/soremoji/feature.py` & `soremoji-0.3.2/soremoji/feature.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import contextlib
 import re
 from dataclasses import dataclass
 from typing import Optional, cast
 
+from emoticon import EMOJIS, Emoji
 from sorampt import Choice, InputPrompt, ListPrompt
 
-from .emoji import EMOJIS, Emoji
-
 MESSAGE_REGEX = re.compile(r"^:(?P<emoji>\w+):(?P<message>[\s\S]+)$")
 
 
 @dataclass
 class Message:
     emoji: Optional[Emoji] = None
     content: Optional[str] = None
```

### Comparing `soremoji-0.3.1/PKG-INFO` & `soremoji-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soremoji
-Version: 0.3.1
+Version: 0.3.2
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
-    rev: 0.3.1
+    rev: 0.3.2
     hooks:
       - id: soremoji
         stages: [pre-commit-msg]
 ```
 
 ## 使用
```

