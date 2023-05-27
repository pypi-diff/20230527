# Comparing `tmp/pmemo-0.1.0.tar.gz` & `tmp/pmemo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmemo-0.1.0.tar", max compression
+gzip compressed data, was "pmemo-0.2.0.tar", max compression
```

## Comparing `pmemo-0.1.0.tar` & `pmemo-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1065 2023-05-22 02:17:41.871474 pmemo-0.1.0/LICENSE
--rw-r--r--   0        0        0     1317 2023-05-22 02:17:41.871474 pmemo-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-22 02:17:41.875474 pmemo-0.1.0/pmemo/__init__.py
--rw-r--r--   0        0        0     4173 2023-05-22 02:17:41.875474 pmemo-0.1.0/pmemo/custom_select.py
--rw-r--r--   0        0        0     2945 2023-05-22 02:17:41.875474 pmemo-0.1.0/pmemo/main.py
--rw-r--r--   0        0        0     4797 2023-05-22 02:17:41.875474 pmemo-0.1.0/pmemo/memo.py
--rw-r--r--   0        0        0     3803 2023-05-22 02:17:41.875474 pmemo-0.1.0/pmemo/pmemo_editor.py
--rw-r--r--   0        0        0      233 2023-05-22 02:17:41.875474 pmemo-0.1.0/pmemo/utils.py
--rw-r--r--   0        0        0      634 2023-05-22 02:17:41.875474 pmemo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 pmemo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-27 09:39:35.408709 pmemo-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2265 2023-05-27 09:39:35.408709 pmemo-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 09:39:35.416710 pmemo-0.2.0/pmemo/__init__.py
+-rw-r--r--   0        0        0     4915 2023-05-27 09:39:35.416710 pmemo-0.2.0/pmemo/custom_select.py
+-rw-r--r--   0        0        0     3803 2023-05-27 09:39:35.416710 pmemo-0.2.0/pmemo/main.py
+-rw-r--r--   0        0        0     5266 2023-05-27 09:39:35.416710 pmemo-0.2.0/pmemo/memo.py
+-rw-r--r--   0        0        0     1502 2023-05-27 09:39:35.416710 pmemo-0.2.0/pmemo/openai_completion.py
+-rw-r--r--   0        0        0     5352 2023-05-27 09:39:35.416710 pmemo-0.2.0/pmemo/pmemo_editor.py
+-rw-r--r--   0        0        0     2415 2023-05-27 09:39:35.416710 pmemo-0.2.0/pmemo/preferences.py
+-rw-r--r--   0        0        0      704 2023-05-27 09:39:35.416710 pmemo-0.2.0/pmemo/utils.py
+-rw-r--r--   0        0        0      856 2023-05-27 09:39:35.416710 pmemo-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 pmemo-0.2.0/PKG-INFO
```

### Comparing `pmemo-0.1.0/LICENSE` & `pmemo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pmemo-0.1.0/pmemo/custom_select.py` & `pmemo-0.2.0/pmemo/custom_select.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from functools import partial
+from pathlib import Path
+from typing import Optional, Union
 
 from prompt_toolkit.application import Application
 from prompt_toolkit.filters import IsDone
 from prompt_toolkit.formatted_text import AnyFormattedText
 from prompt_toolkit.formatted_text.utils import to_plain_text
 from prompt_toolkit.key_binding import KeyBindings, KeyBindingsBase, merge_key_bindings
 from prompt_toolkit.keys import Keys
-from prompt_toolkit.layout.containers import ConditionalContainer, HSplit, Window
-from prompt_toolkit.layout.controls import FormattedTextControl
+from prompt_toolkit.layout.containers import (
+    ConditionalContainer,
+    HSplit,
+    VSplit,
+    Window,
+)
+from prompt_toolkit.layout.controls import DummyControl, FormattedTextControl
 from prompt_toolkit.layout.layout import Layout
 from prompt_toolkit.styles import Style
 from prompt_toolkit.widgets import TextArea
 
 from pmemo.utils import error_handler
 
 ITEM_CLASS = "class:item"
 SELECTED_CLASS = "class:selected"
-styles = Style([("item", ""), ("selected", "underline bg:#d980ff #ffffff")])
 
 
 class CustomFormattedTextControl(FormattedTextControl):
     def __init__(self, text: AnyFormattedText, *args, **kwargs) -> None:
         super(CustomFormattedTextControl, self).__init__(
             self._convert_callable_text(text), *args, **kwargs
         )
@@ -83,20 +89,22 @@
             bindings
             if self.key_bindings is None
             else merge_key_bindings([bindings, self.key_bindings])
         )
 
 
 @error_handler
-def custom_select(choices: list[str]) -> str:
+def custom_select(
+    choices: Union[list[str], dict[str, Path]], max_preview_height: int = 10
+) -> str:
     """Choose one option from a list of choices while searching with a specified query, similar to using the "peco"
     If the execution is interrupted by a "KeyboardInterrupt" (typically triggered by pressing Ctrl+C), the program will be terminated.
 
     Args:
-        choices (list[str]): list of choices displayed on the terminal.
+        choices (Union[list[str], dict[str, Path]]): list or dict of choices displayed on the terminal.
 
     Returns:
         str: string of the selected choice.
     """
     text_area = TextArea(prompt="QUERY> ", multiline=False)
 
     def filter_candidates(choices):
@@ -109,14 +117,30 @@
 
     control = CustomFormattedTextControl(
         partial(filter_candidates, choices), focusable=True
     )
 
     candidates_display = ConditionalContainer(Window(control), ~IsDone())
 
+    def get_memo_content() -> str:
+        selected = to_plain_text(control.get_pointed_at()).strip()
+        return choices[selected].read_text() if isinstance(choices, dict) else ""
+
+    preview_control = FormattedTextControl(get_memo_content, focusable=False)
+    preview_display = ConditionalContainer(
+        Window(
+            preview_control,
+            height=max(len(choices), max_preview_height),
+            wrap_lines=True,
+            ignore_content_width=True,
+        ),
+        ~IsDone(),
+    )
     app: Application[AnyFormattedText] = Application(
-        layout=Layout(HSplit([text_area, candidates_display])),
+        layout=Layout(
+            HSplit([text_area, VSplit([candidates_display, preview_display])])
+        ),
         key_bindings=control.get_key_bindings(),
-        style=styles,
+        style=Style([("item", ""), ("selected", "underline bg:#d980ff #ffffff")]),
         erase_when_done=True,
     )
     return to_plain_text(app.run()).strip()
```

### Comparing `pmemo-0.1.0/pmemo/memo.py` & `pmemo-0.2.0/pmemo/memo.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,82 +3,91 @@
 import hashlib
 import re
 from pathlib import Path
 
 from prompt_toolkit.shortcuts import confirm
 
 RE_CODEBLOCK = re.compile(r"`{3}([^:\s]*):?(.*?)\n([\s\S]+?)`{3}")
-MAX_LENGTH = 30
 LANG_EXT = {"markdown": ".md", "python": ".py", "python3": ".py"}
 DEFAULT_ENCODING = "utf-8"
 
 
-def extract_codeblocks(text: str) -> list[tuple[str, str, str]]:
+def extract_codeblocks(
+    text: str, title_max_length: int = 30
+) -> list[tuple[str, str, str]]:
     """
     Extracts code blocks from the given text and returns a list of tuples representing the code blocks.
 
     Args:
         text (str): The input text from which code blocks are extracted.
+        title_max_length (int): Max length of codeblock's title. Defaults to 30.
 
     Returns:
         list[tuple[str, str, str]]: A list of tuples representing code blocks. Each tuple contains three elements:
                                     - lang (str): The language of the code block.
                                     - blockname (str): The name or identifier of the code block.
                                     - code (str): The actual code contained in the block.
     """
     codeblocks = []
     for lang, blockname, code in RE_CODEBLOCK.findall(text):
         lang = lang.strip() if lang else "python"
         blockname = (
             blockname.strip()
             if blockname.strip()
-            else hashlib.sha256(bytes(code, DEFAULT_ENCODING)).hexdigest()[:MAX_LENGTH]
+            else hashlib.sha256(bytes(code, DEFAULT_ENCODING)).hexdigest()[
+                :title_max_length
+            ]
         )
         blockname = "".join((blockname, LANG_EXT.get(lang, "")))
         codeblocks.append((lang, blockname, code.strip()))
     return codeblocks
 
 
 class Memo:
     """
     Represents a memo with content, title, and file-related operations.
     If the title is not specified, title and file_path depend on the content.
-
-    Attributes:
-        TITLE_MAX_LENGTH (int): The maximum length allowed for a memo title.
     """
 
-    TITLE_MAX_LENGTH: int = 30
-
-    def __init__(self, out_dir: Path, content: str, title: str = ""):
+    def __init__(
+        self, out_dir: Path, content: str, title: str = "", title_max_length: int = 30
+    ):
         """
         Initializes a Memo instance.
 
         Args:
             out_dir (Path): The output directory where the memo will be stored.
             content (str): The content of the memo.
             title (str, optional): The title of the memo. Defaults to an empty string.
+            title_max_length (int): Max length of codeblock's title. Defaults to 30.
         """
         self._out_dir = out_dir
         self._content = content
         self._title = title
+        self._title_max_length = title_max_length
         self._is_edited: bool = False
 
     @classmethod
-    def from_file(cls, file_path: Path) -> Memo:
+    def from_file(cls, file_path: Path, title_max_length: int = 30) -> Memo:
         """
         Creates a Memo instance from a file.
 
         Args:
             file_path (Path): The path to the file.
+            title_max_length (int): Max length of codeblock's title. Defaults to 30.
 
         Returns:
             Memo: A Memo instance created from the file.
         """
-        return cls(file_path.parents[1], file_path.read_text(), file_path.stem)
+        return cls(
+            file_path.parents[1],
+            file_path.read_text(),
+            file_path.stem,
+            title_max_length,
+        )
 
     def edit_content(self, content: str) -> None:
         """
         Edits the content of the memo.
 
         Args:
             content (str): The new content of the memo.
@@ -98,15 +107,17 @@
         If the title is not specified, it is derived from the first line of the content.
 
         Returns:
             str: The title of the memo.
         """
         if not self._title:
             self._title = (
-                self._content.splitlines()[0][: self.TITLE_MAX_LENGTH].replace(" ", "_")
+                self._content.splitlines()[0][: self._title_max_length].replace(
+                    " ", "_"
+                )
                 if self._content
                 else "Untitled"
             )
         return self._title
 
     @property
     def file_path(self) -> Path:
@@ -140,10 +151,12 @@
         Saves the memo to the file system, including associated code blocks.
         """
         if not self._content:
             self._remove()
         elif self._confirm_overwrite():
             self.file_path.write_text(self._content)
 
-            for _, blockname, code in extract_codeblocks(self._content):
+            for _, blockname, code in extract_codeblocks(
+                self._content, self._title_max_length
+            ):
                 codeblock_path = self.file_path.parent / blockname
                 codeblock_path.write_text(code)
```

