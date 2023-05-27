# Comparing `tmp/EdgeGPT-0.6.5.tar.gz` & `tmp/EdgeGPT-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.6.5.tar", last modified: Fri May 26 00:34:45 2023, max compression
+gzip compressed data, was "EdgeGPT-0.6.6.tar", last modified: Sat May 27 06:46:26 2023, max compression
```

## Comparing `EdgeGPT-0.6.5.tar` & `EdgeGPT-0.6.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:34:45.990424 EdgeGPT-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 00:34:15.000000 EdgeGPT-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-26 00:34:45.990424 EdgeGPT-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-05-26 00:34:45.000000 EdgeGPT-0.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-26 00:34:45.990424 EdgeGPT-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-26 00:34:15.000000 EdgeGPT-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:34:45.986425 EdgeGPT-0.6.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:34:45.990424 EdgeGPT-0.6.5/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-26 00:34:45.000000 EdgeGPT-0.6.5/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-26 00:34:45.000000 EdgeGPT-0.6.5/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:34:45.000000 EdgeGPT-0.6.5/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 00:34:45.000000 EdgeGPT-0.6.5/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-26 00:34:45.000000 EdgeGPT-0.6.5/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 00:34:45.000000 EdgeGPT-0.6.5/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    38051 2023-05-26 00:34:15.000000 EdgeGPT-0.6.5/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-26 00:34:15.000000 EdgeGPT-0.6.5/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:46:26.876631 EdgeGPT-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-27 06:45:44.000000 EdgeGPT-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-27 06:46:26.876631 EdgeGPT-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-05-27 06:46:26.000000 EdgeGPT-0.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 06:46:26.876631 EdgeGPT-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-27 06:45:44.000000 EdgeGPT-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:46:26.876631 EdgeGPT-0.6.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:46:26.876631 EdgeGPT-0.6.6/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-27 06:46:26.000000 EdgeGPT-0.6.6/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-27 06:46:26.000000 EdgeGPT-0.6.6/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 06:46:26.000000 EdgeGPT-0.6.6/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-27 06:46:26.000000 EdgeGPT-0.6.6/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-27 06:46:26.000000 EdgeGPT-0.6.6/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-27 06:46:26.000000 EdgeGPT-0.6.6/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    39038 2023-05-27 06:45:44.000000 EdgeGPT-0.6.6/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-27 06:45:44.000000 EdgeGPT-0.6.6/src/ImageGen.py
```

### Comparing `EdgeGPT-0.6.5/LICENSE` & `EdgeGPT-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.6.5/PKG-INFO` & `EdgeGPT-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.6.5
+Version: 0.6.6
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.5 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.6 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.6.5/README.md` & `EdgeGPT-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.6.5/setup.py` & `EdgeGPT-0.6.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.6.5",
+    version="0.6.6",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.6.5/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.6.6/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.6.5
+Version: 0.6.6
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.5 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.6 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.6.5/src/EdgeGPT.py` & `EdgeGPT-0.6.6/src/EdgeGPT.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import ssl
 import sys
 import time
 import uuid
 from enum import Enum
 from pathlib import Path
 from typing import Generator
+
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 from typing import Optional
 from typing import Union
 
@@ -103,57 +104,55 @@
     creative = [
         "nlu_direct_response_filter",
         "deepleo",
         "disable_emoji_spoken_text",
         "responsible_ai_policy_235",
         "enablemm",
         "h3imaginative",
-        "travelansgnd",
+        "cachewriteext",
+        "e2ecachewrite",
+        "nodlcpcwrite",
+        "nointernalsugg",
+        "saharasugg",
+        "enablenewsfc",
         "dv3sugg",
         "clgalileo",
         "gencontentv3",
-        "dv3sugg",
-        "responseos",
-        "e2ecachewrite",
-        "cachewriteext",
-        "nodlcpcwrite",
-        "travelansgnd",
-        "nojbfedge",
     ]
     balanced = [
         "nlu_direct_response_filter",
         "deepleo",
         "disable_emoji_spoken_text",
         "responsible_ai_policy_235",
         "enablemm",
         "galileo",
-        "dv3sugg",
-        "responseos",
-        "e2ecachewrite",
         "cachewriteext",
+        "e2ecachewrite",
         "nodlcpcwrite",
-        "travelansgnd",
-        "nojbfedge",
+        "nointernalsugg",
+        "saharasugg",
+        "enablenewsfc",
+        "dv3sugg",
     ]
     precise = [
         "nlu_direct_response_filter",
         "deepleo",
         "disable_emoji_spoken_text",
         "responsible_ai_policy_235",
         "enablemm",
-        "galileo",
-        "dv3sugg",
-        "responseos",
-        "e2ecachewrite",
+        "h3precise",
         "cachewriteext",
+        "e2ecachewrite",
         "nodlcpcwrite",
-        "travelansgnd",
-        "h3precise",
+        "nointernalsugg",
+        "saharasugg",
+        "enablenewsfc",
+        "dv3sugg",
         "clgalileo",
-        "nojbfedge",
+        "gencontentv3",
     ]
 
 
 CONVERSATION_STYLE_TYPE = Optional[
     Union[ConversationStyle, Literal["creative", "balanced", "precise"]]
 ]
 
@@ -735,14 +734,21 @@
 
     return PromptSession(key_bindings=kb, history=InMemoryHistory())
 
 
 def _create_completer(commands: list, pattern_str: str = "$"):
     return WordCompleter(words=commands, pattern=re.compile(pattern_str))
 
+def _create_history_logger(f):
+    def logger(*args, **kwargs):
+        tmp = sys.stdout
+        sys.stdout = f
+        print(*args, **kwargs, flush=True)
+        sys.stdout = tmp
+    return logger
 
 async def async_main(args: argparse.Namespace) -> None:
     """
     Main function
     """
     print("Initializing...")
     print("Enter `alt+enter` or `escape+enter` to send a message")
@@ -751,27 +757,36 @@
     if args.cookie_file:
         cookies = json.loads(open(args.cookie_file, encoding="utf-8").read())
     bot = await Chatbot.create(proxy=args.proxy, cookies=cookies)
     session = _create_session()
     completer = _create_completer(["!help", "!exit", "!reset"])
     initial_prompt = args.prompt
 
+    # Log chat history
+    def p_hist():
+        pass
+    if args.history_file:
+        f = open(args.history_file, 'a+')
+        p_hist = _create_history_logger(f)
+
     while True:
         print("\nYou:")
+        p_hist("\nYou:")
         if initial_prompt:
             question = initial_prompt
             print(question)
             initial_prompt = None
         else:
             question = (
                 input()
                 if args.enter_once
                 else await _get_input_async(session=session, completer=completer)
             )
         print()
+        p_hist(question + "\n")
         if question == "!exit":
             break
         if question == "!help":
             print(
                 """
             !help - Show this help message
             !exit - Exit the program
@@ -779,35 +794,40 @@
             """,
             )
             continue
         if question == "!reset":
             await bot.reset()
             continue
         print("Bot:")
+        p_hist("Bot:")
         if args.no_stream:
-            print(
-                (
+            response=(
                     await bot.ask(
                         prompt=question,
                         conversation_style=args.style,
                         wss_link=args.wss_link,
                     )
-                )["item"]["messages"][1]["adaptiveCards"][0]["body"][0]["text"],
-            )
+                )["item"]["messages"][1]["adaptiveCards"][0]["body"][0]["text"]
+            print(response)
+            p_hist(response)
         else:
             wrote = 0
             if args.rich:
                 md = Markdown("")
                 with Live(md, auto_refresh=False) as live:
                     async for final, response in bot.ask_stream(
                         prompt=question,
                         conversation_style=args.style,
                         wss_link=args.wss_link,
                     ):
                         if not final:
+                            if not wrote:
+                                p_hist(response, end="")
+                            else:
+                                p_hist(response[wrote:], end="")
                             if wrote > len(response):
                                 print(md)
                                 print(Markdown("***Bing revoked the response.***"))
                             wrote = len(response)
                             md = Markdown(response)
                             live.update(md, refresh=True)
             else:
@@ -815,18 +835,23 @@
                     prompt=question,
                     conversation_style=args.style,
                     wss_link=args.wss_link,
                 ):
                     if not final:
                         if not wrote:
                             print(response, end="", flush=True)
+                            p_hist(response, end="")
                         else:
                             print(response[wrote:], end="", flush=True)
+                            p_hist(response[wrote:], end="")
                         wrote = len(response)
                 print()
+                p_hist()
+    if args.history_file:
+        f.close()
     await bot.close()
 
 
 def main() -> None:
     print(
         """
         EdgeGPT - A demo of reverse engineering the Bing GPT chatbot
@@ -868,14 +893,21 @@
     parser.add_argument(
         "--cookie-file",
         type=str,
         default="",
         required=False,
         help="path to cookie file",
     )
+    parser.add_argument(
+        "--history-file",
+        type=str,
+        default="",
+        required=False,
+        help="path to history file",
+    )
     args = parser.parse_args()
     asyncio.run(async_main(args))
 
 
 class Cookie:
     """
     Convenience class for Bing Cookie files, data, and configuration. This Class
```

