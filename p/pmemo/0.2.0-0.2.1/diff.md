# Comparing `tmp/pmemo-0.2.0.tar.gz` & `tmp/pmemo-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmemo-0.2.0.tar", max compression
+gzip compressed data, was "pmemo-0.2.1.tar", max compression
```

## Comparing `pmemo-0.2.0.tar` & `pmemo-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2023-05-27 09:39:35.408709 pmemo-0.2.0/LICENSE
--rw-r--r--   0        0        0     2265 2023-05-27 09:39:35.408709 pmemo-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-27 09:39:35.416710 pmemo-0.2.0/pmemo/__init__.py
--rw-r--r--   0        0        0     4915 2023-05-27 09:39:35.416710 pmemo-0.2.0/pmemo/custom_select.py
--rw-r--r--   0        0        0     3803 2023-05-27 09:39:35.416710 pmemo-0.2.0/pmemo/main.py
--rw-r--r--   0        0        0     5266 2023-05-27 09:39:35.416710 pmemo-0.2.0/pmemo/memo.py
--rw-r--r--   0        0        0     1502 2023-05-27 09:39:35.416710 pmemo-0.2.0/pmemo/openai_completion.py
--rw-r--r--   0        0        0     5352 2023-05-27 09:39:35.416710 pmemo-0.2.0/pmemo/pmemo_editor.py
--rw-r--r--   0        0        0     2415 2023-05-27 09:39:35.416710 pmemo-0.2.0/pmemo/preferences.py
--rw-r--r--   0        0        0      704 2023-05-27 09:39:35.416710 pmemo-0.2.0/pmemo/utils.py
--rw-r--r--   0        0        0      856 2023-05-27 09:39:35.416710 pmemo-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 pmemo-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-27 15:04:11.916826 pmemo-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2265 2023-05-27 15:04:11.916826 pmemo-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 15:04:11.928826 pmemo-0.2.1/pmemo/__init__.py
+-rw-r--r--   0        0        0     4916 2023-05-27 15:04:11.928826 pmemo-0.2.1/pmemo/custom_select.py
+-rw-r--r--   0        0        0     3803 2023-05-27 15:04:11.928826 pmemo-0.2.1/pmemo/main.py
+-rw-r--r--   0        0        0     5266 2023-05-27 15:04:11.928826 pmemo-0.2.1/pmemo/memo.py
+-rw-r--r--   0        0        0     1502 2023-05-27 15:04:11.928826 pmemo-0.2.1/pmemo/openai_completion.py
+-rw-r--r--   0        0        0     5352 2023-05-27 15:04:11.928826 pmemo-0.2.1/pmemo/pmemo_editor.py
+-rw-r--r--   0        0        0     2415 2023-05-27 15:04:11.928826 pmemo-0.2.1/pmemo/preferences.py
+-rw-r--r--   0        0        0      704 2023-05-27 15:04:11.928826 pmemo-0.2.1/pmemo/utils.py
+-rw-r--r--   0        0        0      856 2023-05-27 15:04:11.928826 pmemo-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 pmemo-0.2.1/PKG-INFO
```

### Comparing `pmemo-0.2.0/LICENSE` & `pmemo-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pmemo-0.2.0/README.md` & `pmemo-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pmemo-0.2.0/pmemo/custom_select.py` & `pmemo-0.2.1/pmemo/custom_select.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from functools import partial
 from pathlib import Path
-from typing import Optional, Union
+from typing import Union
 
 from prompt_toolkit.application import Application
 from prompt_toolkit.filters import IsDone
 from prompt_toolkit.formatted_text import AnyFormattedText
 from prompt_toolkit.formatted_text.utils import to_plain_text
 from prompt_toolkit.key_binding import KeyBindings, KeyBindingsBase, merge_key_bindings
 from prompt_toolkit.keys import Keys
 from prompt_toolkit.layout.containers import (
     ConditionalContainer,
     HSplit,
     VSplit,
     Window,
 )
-from prompt_toolkit.layout.controls import DummyControl, FormattedTextControl
+from prompt_toolkit.layout.controls import FormattedTextControl
 from prompt_toolkit.layout.layout import Layout
 from prompt_toolkit.styles import Style
 from prompt_toolkit.widgets import TextArea
 
 from pmemo.utils import error_handler
 
 ITEM_CLASS = "class:item"
@@ -57,17 +57,15 @@
 
     def move_cursor_down(self) -> None:
         self.pointed_at += 1
         self.pointed_at = max(0, min(self.pointed_at, self.choice_count - 1))
 
     def get_pointed_at(self) -> AnyFormattedText:
         self.pointed_at = max(0, min(self.pointed_at, self.choice_count - 1))
-        return (
-            self._fragments[self.pointed_at][1] if self._fragments is not None else None
-        )
+        return self._fragments[self.pointed_at][1] if self._fragments else None
 
     def get_key_bindings(self) -> KeyBindingsBase:
         bindings = KeyBindings()
 
         @bindings.add(Keys.ControlC, eager=True)
         def _(event):
             event.app.exit(exception=KeyboardInterrupt, style="class:aborting")
@@ -119,15 +117,19 @@
         partial(filter_candidates, choices), focusable=True
     )
 
     candidates_display = ConditionalContainer(Window(control), ~IsDone())
 
     def get_memo_content() -> str:
         selected = to_plain_text(control.get_pointed_at()).strip()
-        return choices[selected].read_text() if isinstance(choices, dict) else ""
+        return (
+            choices[selected].read_text()
+            if isinstance(choices, dict) and selected
+            else ""
+        )
 
     preview_control = FormattedTextControl(get_memo_content, focusable=False)
     preview_display = ConditionalContainer(
         Window(
             preview_control,
             height=max(len(choices), max_preview_height),
             wrap_lines=True,
```

### Comparing `pmemo-0.2.0/pmemo/main.py` & `pmemo-0.2.1/pmemo/main.py`

 * *Files identical despite different names*

### Comparing `pmemo-0.2.0/pmemo/memo.py` & `pmemo-0.2.1/pmemo/memo.py`

 * *Files identical despite different names*

### Comparing `pmemo-0.2.0/pmemo/openai_completion.py` & `pmemo-0.2.1/pmemo/openai_completion.py`

 * *Files identical despite different names*

### Comparing `pmemo-0.2.0/pmemo/pmemo_editor.py` & `pmemo-0.2.1/pmemo/pmemo_editor.py`

 * *Files identical despite different names*

### Comparing `pmemo-0.2.0/pmemo/preferences.py` & `pmemo-0.2.1/pmemo/preferences.py`

 * *Files identical despite different names*

### Comparing `pmemo-0.2.0/pmemo/utils.py` & `pmemo-0.2.1/pmemo/utils.py`

 * *Files identical despite different names*

### Comparing `pmemo-0.2.0/pyproject.toml` & `pmemo-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pmemo"
-version = "0.2.0"
+version = "0.2.1"
 description = "Pmemo with ChatGPT is a CUI memo app that enables direct terminal editing without full-screen mode. It integrates OpenAI's ChatGPT, allowing interactive inquiries via the ctrl + o shortcut."
 authors = ["Asugawara <asgasw@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pmemo"}]
 
 [tool.poetry.scripts]
 pm = "pmemo.main:main"
```

### Comparing `pmemo-0.2.0/PKG-INFO` & `pmemo-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmemo
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pmemo with ChatGPT is a CUI memo app that enables direct terminal editing without full-screen mode. It integrates OpenAI's ChatGPT, allowing interactive inquiries via the ctrl + o shortcut.
 Author: Asugawara
 Author-email: asgasw@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

