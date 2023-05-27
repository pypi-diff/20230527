# Comparing `tmp/talk_codebase-0.1.16.tar.gz` & `tmp/talk_codebase-0.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.16.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.17.tar", max compression
```

## Comparing `talk_codebase-0.1.16.tar` & `talk_codebase-0.1.17.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1237 2023-05-27 14:14:29.673279 talk_codebase-0.1.16/README.md
--rw-r--r--   0        0        0      811 2023-05-27 14:14:29.673279 talk_codebase-0.1.16/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-27 14:14:29.673279 talk_codebase-0.1.16/talk_codebase/__init__.py
--rw-r--r--   0        0        0     1960 2023-05-27 14:14:29.673279 talk_codebase-0.1.16/talk_codebase/cli.py
--rw-r--r--   0        0        0      518 2023-05-27 14:14:29.673279 talk_codebase-0.1.16/talk_codebase/consts.py
--rw-r--r--   0        0        0     2149 2023-05-27 14:14:29.673279 talk_codebase-0.1.16/talk_codebase/llm.py
--rw-r--r--   0        0        0     1947 2023-05-27 14:14:29.677279 talk_codebase-0.1.16/talk_codebase/utils.py
--rw-r--r--   0        0        0     2099 1970-01-01 00:00:00.000000 talk_codebase-0.1.16/PKG-INFO
+-rw-r--r--   0        0        0     1236 2023-05-27 14:30:36.778215 talk_codebase-0.1.17/README.md
+-rw-r--r--   0        0        0      811 2023-05-27 14:30:36.778215 talk_codebase-0.1.17/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-27 14:30:36.778215 talk_codebase-0.1.17/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     1960 2023-05-27 14:30:36.778215 talk_codebase-0.1.17/talk_codebase/cli.py
+-rw-r--r--   0        0        0      518 2023-05-27 14:30:36.778215 talk_codebase-0.1.17/talk_codebase/consts.py
+-rw-r--r--   0        0        0     2318 2023-05-27 14:30:36.778215 talk_codebase-0.1.17/talk_codebase/llm.py
+-rw-r--r--   0        0        0     1947 2023-05-27 14:30:36.778215 talk_codebase-0.1.17/talk_codebase/utils.py
+-rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 talk_codebase-0.1.17/PKG-INFO
```

### Comparing `talk_codebase-0.1.16/README.md` & `talk_codebase-0.1.17/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # talk-codebase is a powerful tool for chatting with your codebase
 
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
 
 <p align="center">
-  <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/6d92e905-fb1b-4235-857b-e6e19041ad79" width="800" alt="chat">
+  <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b5d338f9-14a5-417b-9690-83f5cd66facf" width="800" alt="chat">
 </p>
- 
+
 ## Description
 
 In the chat, you can ask questions about the codebase. AI will answer your questions, and if necessary, it will offer
 code improvements. This is very convenient when you want to quickly find something in the codebase, but don't want to
 waste time searching. It is also convenient when you want to improve a specific function, you can ask "How can I improve
 the function {function name}?" and AI will suggest improvements. Codebase is analyzed using openai.
```

### Comparing `talk_codebase-0.1.16/pyproject.toml` & `talk_codebase-0.1.17/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.16"
+version = "0.1.17"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.16/talk_codebase/cli.py` & `talk_codebase-0.1.17/talk_codebase/cli.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.16/talk_codebase/consts.py` & `talk_codebase-0.1.17/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.16/talk_codebase/llm.py` & `talk_codebase-0.1.17/talk_codebase/llm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 
 import questionary
 import tiktoken
+from halo import Halo
 from langchain import FAISS
 from langchain.callbacks.manager import CallbackManager
 from langchain.chains import ConversationalRetrievalChain
 from langchain.chat_models import ChatOpenAI
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.text_splitter import CharacterTextSplitter
 
@@ -38,16 +39,18 @@
             {"name": "No", "value": False},
         ]
     ).ask()
 
     if not approve:
         exit(0)
 
+    spinners = Halo(text='Creating vector store', spinner='dots').start()
     embeddings = OpenAIEmbeddings(openai_api_key=openai_api_key)
     db = FAISS.from_documents(texts, embeddings)
+    spinners.succeed(f"Created vector store with {len(docs)} documents")
 
     return db
 
 
 def send_question(question, vector_store, openai_api_key, model_name):
     model = ChatOpenAI(model_name=model_name, openai_api_key=openai_api_key, streaming=True,
                        callback_manager=CallbackManager([StreamStdOut()]))
```

### Comparing `talk_codebase-0.1.16/talk_codebase/utils.py` & `talk_codebase-0.1.17/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.16/PKG-INFO` & `talk_codebase-0.1.17/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.16
+Version: 0.1.17
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -22,17 +22,17 @@
 Description-Content-Type: text/markdown
 
 # talk-codebase is a powerful tool for chatting with your codebase
 
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
 
 <p align="center">
-  <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/6d92e905-fb1b-4235-857b-e6e19041ad79" width="800" alt="chat">
+  <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b5d338f9-14a5-417b-9690-83f5cd66facf" width="800" alt="chat">
 </p>
- 
+
 ## Description
 
 In the chat, you can ask questions about the codebase. AI will answer your questions, and if necessary, it will offer
 code improvements. This is very convenient when you want to quickly find something in the codebase, but don't want to
 waste time searching. It is also convenient when you want to improve a specific function, you can ask "How can I improve
 the function {function name}?" and AI will suggest improvements. Codebase is analyzed using openai.
```

