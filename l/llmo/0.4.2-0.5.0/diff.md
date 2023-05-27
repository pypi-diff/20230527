# Comparing `tmp/llmo-0.4.2.tar.gz` & `tmp/llmo-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmo-0.4.2.tar", last modified: Wed May 24 23:07:46 2023, max compression
+gzip compressed data, was "llmo-0.5.0.tar", last modified: Sat May 27 20:01:25 2023, max compression
```

## Comparing `llmo-0.4.2.tar` & `llmo-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.4.2/LICENSE
--rw-r--r--   0        0        0     2373 2023-05-24 23:06:37.762004 llmo-0.4.2/README.md
--rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.4.2/llmo/__init__.py
--rw-r--r--   0        0        0     2961 2023-05-24 03:21:31.439301 llmo-0.4.2/llmo/cli.py
--rw-r--r--   0        0        0      122 2023-05-22 21:51:03.475865 llmo-0.4.2/llmo/constants.py
--rw-r--r--   0        0        0     9793 2023-05-23 03:53:39.625867 llmo-0.4.2/llmo/gui.py
--rw-r--r--   0        0        0      341 2023-05-23 03:17:45.469101 llmo-0.4.2/llmo/layout.css
--rw-r--r--   0        0        0     6481 2023-05-24 21:01:58.190536 llmo-0.4.2/llmo/llms.py
--rw-r--r--   0        0        0     1593 2023-05-23 04:53:16.585981 llmo-0.4.2/llmo/shell_mode.py
--rw-r--r--   0        0        0      722 2023-05-24 23:07:46.252966 llmo-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      838 2023-05-22 22:24:34.139710 llmo-0.4.2/tests/test_openai.py
--rw-r--r--   0        0        0     2749 1970-01-01 00:00:00.000000 llmo-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2374 2023-05-26 15:57:37.255918 llmo-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.5.0/llmo/__init__.py
+-rw-r--r--   0        0        0     2961 2023-05-24 03:21:31.439301 llmo-0.5.0/llmo/cli.py
+-rw-r--r--   0        0        0      122 2023-05-22 21:51:03.475865 llmo-0.5.0/llmo/constants.py
+-rw-r--r--   0        0        0     9835 2023-05-27 19:43:28.486609 llmo-0.5.0/llmo/gui.py
+-rw-r--r--   0        0        0      341 2023-05-23 03:17:45.469101 llmo-0.5.0/llmo/layout.css
+-rw-r--r--   0        0        0     5957 2023-05-27 19:43:28.491411 llmo-0.5.0/llmo/llms.py
+-rw-r--r--   0        0        0     1593 2023-05-23 04:53:16.585981 llmo-0.5.0/llmo/shell_mode.py
+-rw-r--r--   0        0        0      722 2023-05-27 20:01:25.439524 llmo-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      838 2023-05-22 22:24:34.139710 llmo-0.5.0/tests/test_openai.py
+-rw-r--r--   0        0        0     2750 1970-01-01 00:00:00.000000 llmo-0.5.0/PKG-INFO
```

### Comparing `llmo-0.4.2/LICENSE` & `llmo-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmo-0.4.2/README.md` & `llmo-0.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 
 <img src="https://github.com/knowsuchagency/llmo/blob/main/static/mascot.png?raw=true" alt="mascot" style="width: 400px; height: auto;">   
 
 LLMO is the AI pair programming tool that meets you where you are (your terminal) 😉
 
 With the **"staging area"**, you can keep files in the context window without the hassle of copying and pasting every time you make changes to your code.
 
-## Demo
-
-https://github.com/knowsuchagency/llmo/assets/11974795/72419d64-585b-4cd5-a546-2a07de3e6f03
-
 
 ## Features
 
 - Interactive Chat: Enjoy real-time, interactive programming assistance in your terminal.
 - Staging Area: Easily add files to the AI's context to update it about your ongoing coding tasks. No need to copy and paste updates.
 - Model Customization: Choose the OpenAI model that fits your needs.
 - Personality: By default, Elmo loves to make bodybuilding references. This can be turned off through a CLI flag or environment variable.
@@ -28,14 +24,19 @@
 
 The recommended way to install `llmo` is through [pipx][pipx]:
 
 ```bash
 pipx install llmo
 ```
 
+## Demo
+
+https://github.com/knowsuchagency/llmo/assets/11974795/72419d64-585b-4cd5-a546-2a07de3e6f03
+
+
 ## Usage
 
 ```bash
 llmo --help
 # you can also use the shorthand
 lm
```

### Comparing `llmo-0.4.2/llmo/cli.py` & `llmo-0.5.0/llmo/cli.py`

 * *Files identical despite different names*

### Comparing `llmo-0.4.2/llmo/gui.py` & `llmo-0.5.0/llmo/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 from llmo.constants import MODELS
 from llmo.llms import OpenAI
 
 
 class LLMInterface(Protocol):
     has_personality: bool
 
+    def reset(self) -> None:
+        ...
+
     def submit(self, prompt: str, files: Iterable[Path] = None) -> str:
         ...
 
     async def asubmit(self, prompt: str, files: Iterable[Path] = None):
         ...
 
     def add_personality(self) -> None:
```

### Comparing `llmo-0.4.2/llmo/llms.py` & `llmo-0.5.0/llmo/llms.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,89 +47,91 @@
     )
     personality_prompt: str = (
         "You love creatine and bodybuilding "
         "and go out of your way to insert creative, bodybuilding, and /r/swoleacceptance references in your responses."
     )
     max_tokens: int = None
 
-    @property
-    def has_personality(self):
-        return self.personality_prompt in self.system_prompt
-
-    def add_personality(self):
-        self.system_prompt = self._initial_system_prompt + " " + self.personality_prompt
-
-    def remove_personality(self):
-        self.system_prompt = self._initial_system_prompt
-
     def __post_init__(self):
         self._initial_system_prompt = self.system_prompt
         if self.api_key:
             openai.api_key = self.api_key
 
-    def reset(self):
-        self.messages = deque()
-
-    def remove_file_messages(self):
+    def _remove_file_messages(self):
         temp_messages = copy(self.messages)
         for msg in temp_messages:
             if (
                 msg["role"] == "user"
                 and msg["content"].startswith("`")
                 and msg["content"].endswith("```")
             ):
                 self.messages.remove(msg)
                 return True
         return False
 
-    def truncate_old_messages(self):
+    def _truncate_old_messages(self):
         """Truncate old messages to stay under the character limit."""
         if self.max_tokens is not None:
             estimated_tokens = sum(
                 len(m["content"]) / ESTIMATED_CHAR_PER_TOKEN for m in self.messages
             )
             while estimated_tokens > self.max_tokens:
                 # Try to remove file messages first
-                if not self.remove_file_messages():
+                if not self._remove_file_messages():
                     # If no file messages to remove, remove the oldest message
                     removed_message = self.messages.popleft()
                 else:
                     # If a file message was removed, continue to the next iteration
                     continue
 
                 estimated_tokens -= (
                     len(removed_message["content"]) / ESTIMATED_CHAR_PER_TOKEN
                 )
 
-    @retry_openai_call
-    async def asubmit(self, prompt: str, files: Iterable[Path] = None):
-        """
-        Submit a prompt to the OpenAI API and asynchronously yield tokens.
-
-        If files are provided, they will be added to the prompt as part of the submission.
-        """
+    async def _prepare_messages(self, files, prompt):
         for file in files or []:
             # remove any existing messages with the same file content
             temp_messages = copy(self.messages)
             for msg in temp_messages:
                 if msg["role"] == "user" and msg["content"].startswith(f"`{file}`"):
                     self.messages.remove(msg)
             # add file content to messages
             self.messages.append(
                 {"role": "user", "content": f"`{file}`\n```{file.read_text()}```"}
             )
         self.messages.append({"role": "user", "content": prompt})
-
-        self.truncate_old_messages()
-
+        self._truncate_old_messages()
         system_message = SystemMessage(
             role="system",
             content=self.system_prompt,
         )
         messages = [system_message, *self.messages]
+        return messages
+
+    @property
+    def has_personality(self):
+        return self.personality_prompt in self.system_prompt
+
+    def add_personality(self):
+        self.system_prompt = self._initial_system_prompt + " " + self.personality_prompt
+
+    def remove_personality(self):
+        self.system_prompt = self._initial_system_prompt
+
+    def reset(self):
+        self.messages = deque()
+
+    @retry_openai_call
+    async def asubmit(self, prompt: str, files: Iterable[Path] = None):
+        """
+        Submit a prompt to the OpenAI API and asynchronously yield tokens.
+
+        If files are provided, they will be added to the prompt as part of the submission.
+        """
+        messages = await self._prepare_messages(files, prompt)
 
         events = openai.ChatCompletion.create(
             messages=messages,
             model=self.model,
             temperature=self.temperature,
             stream=True,
         )
@@ -157,32 +159,15 @@
     @retry_openai_call
     def submit(self, prompt: str, files: Iterable[Path] = None):
         """
         Submit a prompt to the OpenAI API and return the response.
 
         If files are provided, they will be added to the prompt as part of the submission.
         """
-        for file in files or []:
-            # remove any existing messages with the same file content
-            temp_messages = copy(self.messages)
-            for msg in temp_messages:
-                if msg["role"] == "user" and msg["content"].startswith(f"`{file}`"):
-                    self.messages.remove(msg)
-            self.messages.append(
-                {"role": "user", "content": f"`{file}`\n```{file.read_text()}```"}
-            )
-        self.messages.append({"role": "user", "content": prompt})
-
-        self.truncate_old_messages()
-
-        system_message = SystemMessage(
-            role="system",
-            content=self.system_prompt,
-        )
-        messages = [system_message, *self.messages]
+        messages = self._prepare_messages(files, prompt)
 
         assistant_message = openai.ChatCompletion.create(
             messages=messages,
             model=self.model,
             temperature=self.temperature,
         )["choices"][0]["message"]
```

### Comparing `llmo-0.4.2/llmo/shell_mode.py` & `llmo-0.5.0/llmo/shell_mode.py`

 * *Files identical despite different names*

### Comparing `llmo-0.4.2/pyproject.toml` & `llmo-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmo"
-version = "0.4.2"
+version = "0.5.0"
 description = "AI pair programmer"
 authors = [
     { name = "Stephan Fitzpatrick", email = "stephan@knowsuchagency.com" },
 ]
 dependencies = [
     "textual>=0.26.0",
     "openai>=0.27.6",
```

### Comparing `llmo-0.4.2/tests/test_openai.py` & `llmo-0.5.0/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `llmo-0.4.2/PKG-INFO` & `llmo-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmo
-Version: 0.4.2
+Version: 0.5.0
 Summary: AI pair programmer
 Author-Email: Stephan Fitzpatrick <stephan@knowsuchagency.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/knowsuchagency/llmo
 Requires-Python: >=3.10
 Requires-Dist: textual>=0.26.0
 Requires-Dist: openai>=0.27.6
@@ -21,18 +21,14 @@
 
 <img src="https://github.com/knowsuchagency/llmo/blob/main/static/mascot.png?raw=true" alt="mascot" style="width: 400px; height: auto;">   
 
 LLMO is the AI pair programming tool that meets you where you are (your terminal) 😉
 
 With the **"staging area"**, you can keep files in the context window without the hassle of copying and pasting every time you make changes to your code.
 
-## Demo
-
-https://github.com/knowsuchagency/llmo/assets/11974795/72419d64-585b-4cd5-a546-2a07de3e6f03
-
 
 ## Features
 
 - Interactive Chat: Enjoy real-time, interactive programming assistance in your terminal.
 - Staging Area: Easily add files to the AI's context to update it about your ongoing coding tasks. No need to copy and paste updates.
 - Model Customization: Choose the OpenAI model that fits your needs.
 - Personality: By default, Elmo loves to make bodybuilding references. This can be turned off through a CLI flag or environment variable.
@@ -41,14 +37,19 @@
 
 The recommended way to install `llmo` is through [pipx][pipx]:
 
 ```bash
 pipx install llmo
 ```
 
+## Demo
+
+https://github.com/knowsuchagency/llmo/assets/11974795/72419d64-585b-4cd5-a546-2a07de3e6f03
+
+
 ## Usage
 
 ```bash
 llmo --help
 # you can also use the shorthand
 lm
```

