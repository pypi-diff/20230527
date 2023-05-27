# Comparing `tmp/custom_chat_gpt-0.2.2.tar.gz` & `tmp/custom_chat_gpt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_chat_gpt-0.2.2.tar", max compression
+gzip compressed data, was "custom_chat_gpt-0.2.3.tar", max compression
```

## Comparing `custom_chat_gpt-0.2.2.tar` & `custom_chat_gpt-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      221 2023-04-22 14:51:31.930390 custom_chat_gpt-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-04-22 16:59:59.393190 custom_chat_gpt-0.2.2/chat_gpt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 16:59:59.393439 custom_chat_gpt-0.2.2/chat_gpt/commands/__init__.py
--rw-r--r--   0        0        0     1320 2023-04-22 17:06:55.759659 custom_chat_gpt-0.2.2/chat_gpt/commands/chat.py
--rw-r--r--   0        0        0     3267 2023-04-22 17:06:55.759966 custom_chat_gpt-0.2.2/chat_gpt/commands/youtube.py
--rw-r--r--   0        0        0     1385 2023-04-22 16:59:59.394326 custom_chat_gpt-0.2.2/chat_gpt/main.py
--rw-r--r--   0        0        0        0 2023-04-22 16:59:59.394382 custom_chat_gpt-0.2.2/chat_gpt/utils/__init__.py
--rw-r--r--   0        0        0      709 2023-04-22 16:59:59.394662 custom_chat_gpt-0.2.2/chat_gpt/utils/callbacks.py
--rw-r--r--   0        0        0      635 2023-04-22 17:07:24.914852 custom_chat_gpt-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 custom_chat_gpt-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      221 2023-04-22 14:51:31.930390 custom_chat_gpt-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 16:59:59.393190 custom_chat_gpt-0.2.3/chat_gpt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 16:59:59.393439 custom_chat_gpt-0.2.3/chat_gpt/commands/__init__.py
+-rw-r--r--   0        0        0     1557 2023-05-27 14:40:28.579243 custom_chat_gpt-0.2.3/chat_gpt/commands/chat.py
+-rw-r--r--   0        0        0     3267 2023-04-22 17:06:55.759966 custom_chat_gpt-0.2.3/chat_gpt/commands/youtube.py
+-rw-r--r--   0        0        0     1446 2023-05-27 14:41:21.255211 custom_chat_gpt-0.2.3/chat_gpt/main.py
+-rw-r--r--   0        0        0        0 2023-04-22 16:59:59.394382 custom_chat_gpt-0.2.3/chat_gpt/utils/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-27 14:01:46.439509 custom_chat_gpt-0.2.3/chat_gpt/utils/callbacks.py
+-rw-r--r--   0        0        0      670 2023-05-27 14:42:34.412766 custom_chat_gpt-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 custom_chat_gpt-0.2.3/PKG-INFO
```

### Comparing `custom_chat_gpt-0.2.2/chat_gpt/commands/chat.py` & `custom_chat_gpt-0.2.3/chat_gpt/commands/chat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,51 @@
-
-from typing import Any
-from rich.prompt import Prompt
+from langchain.callbacks import CallbackManager
+from langchain.chat_models import ChatOpenAI
+from langchain.schema import BaseMessage
+from langchain.schema import HumanMessage
+from langchain.schema import SystemMessage
 from rich.console import Console
 from rich.live import Live
-from langchain.chat_models import ChatOpenAI
-from langchain.callbacks import CallbackManager
-from langchain.schema import (
-    HumanMessage,
-    SystemMessage,
-    BaseMessage
-)
-from chat_gpt.utils.callbacks import StreamingTerminalCallbackHandler, rich_streaming_display
-
+from rich.prompt import Prompt
 
+from chat_gpt.utils.callbacks import rich_streaming_display
+from chat_gpt.utils.callbacks import StreamingTerminalCallbackHandler
 
-def chat():
 
+def chat(model_name: str):
     console = Console()
 
     messages: list[BaseMessage] = [
-        SystemMessage(content="You’re a helpful programming assistant. Answers the questions as a professional programmer."),
+        SystemMessage(
+            content="You’re a helpful programming assistant. Answers the questions as a professional programmer."
+        ),
     ]
 
     console.print("Starting a chat ...")
     console.print()
-    
+
     while True:
         content = Prompt.ask("[red][b]User [b/]")
         console.print()
         messages.append(HumanMessage(content=content))
 
         stream_manager = CallbackManager(
-            [StreamingTerminalCallbackHandler(output_callback= lambda x: rich_streaming_display(x, live_chat))]
+            [
+                StreamingTerminalCallbackHandler(
+                    output_callback=lambda x: rich_streaming_display(x, live_chat)
+                )
+            ]
+        )
+        chat = ChatOpenAI(
+            model_name=model_name,
+            temperature=0,
+            streaming=True,
+            callback_manager=stream_manager,
+            verbose=True,
         )
-        chat = ChatOpenAI(temperature=0, streaming=True, callback_manager=stream_manager, verbose=True)
 
         console.print("[blue][b]Assistant :[/b][/blue]")
         with Live(console=console, refresh_per_second=2) as live_chat:
             ai_response = chat(messages)
-        
+
         messages.append(ai_response)
         console.print()
```

### Comparing `custom_chat_gpt-0.2.2/chat_gpt/commands/youtube.py` & `custom_chat_gpt-0.2.3/chat_gpt/commands/youtube.py`

 * *Files identical despite different names*

### Comparing `custom_chat_gpt-0.2.2/chat_gpt/main.py` & `custom_chat_gpt-0.2.3/chat_gpt/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,63 @@
-
 import os
 import sys
+
 import openai
 import typer
 from rich.console import Console
 from youtube_transcript_api import TranscriptsDisabled
+
 from chat_gpt.commands.chat import chat
 from chat_gpt.commands.youtube import chat_with_yt_video
 
 app = typer.Typer()
 
 console = Console()
 
-openai.api_key = os.environ.get('OPENAI_API_KEY')
+openai.api_key = os.environ.get("OPENAI_API_KEY")
+
 if openai.api_key is None:
-    console.print('[red]Please set the OPENAI_API_KEY environment variable.')
-    exit(1)  
+    console.print("[red]Please set the OPENAI_API_KEY environment variable.")
+    exit(1)
+
 
-    
 @app.command("chat")
-def start():
+def start(model_name: str = "gpt-3.5-turbo"):
     """
     Start conversation with our assistant
     """
     try:
-        chat()
+        chat(model_name)
     except KeyboardInterrupt:
         try:
             sys.exit(130)
         except SystemExit:
             os._exit(130)
 
 
 @app.command()
-def youtube(url: str, language: str = 'en'):
+def youtube(url: str, language: str = "en"):
     """
     Start conversation with our assistant using a youtube video transcript
     """
 
     try:
         chat_with_yt_video(url, language)
     except TranscriptsDisabled as e:
-        console.print("\n[red]Transcripts are disabled for this video or the video you're trying to extract doesn't exist.")
+        console.print(
+            "\n[red]Transcripts are disabled for this video or the video you're trying to extract doesn't exist."
+        )
         console.print(e)
     except KeyboardInterrupt:
         try:
             sys.exit(130)
         except SystemExit:
             os._exit(130)
 
 
-
 @app.callback()
 def callback():
     """
     CLI which allows you to chat with our lovely assistant.
 
     Possible to chat with gpt-3.5 or with a youtube video transcript.
-    """
+    """
```

### Comparing `custom_chat_gpt-0.2.2/pyproject.toml` & `custom_chat_gpt-0.2.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "custom-chat-gpt"
-version = "0.2.2"
+version = "0.2.3"
 description = "Use chapgpt from your terminal"
 authors = ["RomainEconomics <jouhameau.romain@gmail.com>"]
 readme = "README.md"
 packages = [{include = "chat_gpt"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
@@ -22,7 +22,10 @@
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.22.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+max_length_line = 119
```

### Comparing `custom_chat_gpt-0.2.2/PKG-INFO` & `custom_chat_gpt-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-chat-gpt
-Version: 0.2.2
+Version: 0.2.3
 Summary: Use chapgpt from your terminal
 Author: RomainEconomics
 Author-email: jouhameau.romain@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

