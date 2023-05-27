# Comparing `tmp/talk_codebase-0.1.13.tar.gz` & `tmp/talk_codebase-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.13.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.14.tar", max compression
```

## Comparing `talk_codebase-0.1.13.tar` & `talk_codebase-0.1.14.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1234 2023-05-26 18:39:43.575177 talk_codebase-0.1.13/README.md
--rw-r--r--   0        0        0      744 2023-05-26 18:39:43.575177 talk_codebase-0.1.13/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 18:39:43.575177 talk_codebase-0.1.13/talk_codebase/__init__.py
--rw-r--r--   0        0        0     1895 2023-05-26 18:39:43.575177 talk_codebase-0.1.13/talk_codebase/cli.py
--rw-r--r--   0        0        0      517 2023-05-26 18:39:43.575177 talk_codebase-0.1.13/talk_codebase/consts.py
--rw-r--r--   0        0        0     1451 2023-05-26 18:39:43.575177 talk_codebase-0.1.13/talk_codebase/llm.py
--rw-r--r--   0        0        0     1454 2023-05-26 18:39:43.575177 talk_codebase-0.1.13/talk_codebase/utils.py
--rw-r--r--   0        0        0     1974 1970-01-01 00:00:00.000000 talk_codebase-0.1.13/PKG-INFO
+-rw-r--r--   0        0        0     1237 2023-05-27 01:21:38.748767 talk_codebase-0.1.14/README.md
+-rw-r--r--   0        0        0      785 2023-05-27 01:21:38.748767 talk_codebase-0.1.14/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-27 01:21:38.748767 talk_codebase-0.1.14/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     1897 2023-05-27 01:21:38.748767 talk_codebase-0.1.14/talk_codebase/cli.py
+-rw-r--r--   0        0        0      518 2023-05-27 01:21:38.748767 talk_codebase-0.1.14/talk_codebase/consts.py
+-rw-r--r--   0        0        0     1451 2023-05-27 01:21:38.748767 talk_codebase-0.1.14/talk_codebase/llm.py
+-rw-r--r--   0        0        0     1945 2023-05-27 01:21:38.748767 talk_codebase-0.1.14/talk_codebase/utils.py
+-rw-r--r--   0        0        0     2054 1970-01-01 00:00:00.000000 talk_codebase-0.1.14/PKG-INFO
```

### Comparing `talk_codebase-0.1.13/README.md` & `talk_codebase-0.1.14/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 # talk-codebase is a powerful tool for chatting with your codebase
+
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
 
 <p align="center">
   <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/6d92e905-fb1b-4235-857b-e6e19041ad79" width="800" alt="chat">
 </p>
-
+ 
 ## Description
 
-In the chat, you can ask questions about the codebase. AI will answer your questions, and if necessary, it will offer code improvements. This is very convenient when you want to quickly find something in the codebase, but don't want to waste time searching. It is also convenient when you want to improve a specific function, you can ask "How can I improve the function {function name}?" and AI will suggest improvements. Codebase is analyzed using openai.
+In the chat, you can ask questions about the codebase. AI will answer your questions, and if necessary, it will offer
+code improvements. This is very convenient when you want to quickly find something in the codebase, but don't want to
+waste time searching. It is also convenient when you want to improve a specific function, you can ask "How can I improve
+the function {function name}?" and AI will suggest improvements. Codebase is analyzed using openai.
 
 ## Installation
 
 ```bash
 pip install talk-codebase
 ```
 
 ## Usage
 
-talk-codebase works only with files of popular programming languages and additionally with .txt files. All other files will be ignored.
+talk-codebase works only with files of popular programming languages and additionally with .txt files. All other files
+will be ignored.
+
 ```bash
 # Start chatting with your codebase
 talk-codebase chat <directory>
 
 # Configure
 talk-codebase configure
```

### Comparing `talk_codebase-0.1.13/pyproject.toml` & `talk_codebase-0.1.14/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.13"
+version = "0.1.14"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{include = "talk_codebase"}]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-langchain = "^0.0.180"
+langchain = "^0.0.181"
 fire = "^0.5.0"
 openai = "^0.27.7"
 tiktoken = "^0.4.0"
 faiss-cpu = "^1.7.4"
 halo = "^0.0.31"
+urllib3 = "1.26.6"
+gitpython = "^3.1.31"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project.urls]
```

### Comparing `talk_codebase-0.1.13/talk_codebase/cli.py` & `talk_codebase-0.1.14/talk_codebase/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
+
 import fire
 import yaml
+
 from talk_codebase.llm import create_vector_store, send_question
 
 
 def get_config():
     home_dir = os.path.expanduser("~")
     config_path = os.path.join(home_dir, ".config.yaml")
     if os.path.exists(config_path):
```

### Comparing `talk_codebase-0.1.13/talk_codebase/consts.py` & `talk_codebase-0.1.14/talk_codebase/consts.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 EXCLUDE_DIRS = ['__pycache__', '.venv', '.git', '.idea', 'venv', 'env', 'node_modules', 'dist', 'build', '.vscode',
                 '.github', '.gitlab']
 ALLOW_FILES = ['.txt', '.js', '.mjs', '.ts', '.tsx', '.css', '.scss', '.less', '.html', '.htm', '.json', '.py',
                '.java', '.c', '.cpp', '.cs', '.go', '.php', '.rb', '.rs', '.swift', '.kt', '.scala', '.m', '.h',
                '.sh', '.pl', '.pm', '.lua', '.sql']
-EXCLUDE_FILES = ['requirements.txt', 'package.json', 'package-lock.json', 'yarn.lock']
+EXCLUDE_FILES = ['requirements.txt', 'package.json', 'package-lock.json', 'yarn.lock']
```

### Comparing `talk_codebase-0.1.13/talk_codebase/llm.py` & `talk_codebase-0.1.14/talk_codebase/llm.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 
+from halo import Halo
 from langchain import FAISS
 from langchain.callbacks.manager import CallbackManager
 from langchain.chains import ConversationalRetrievalChain
 from langchain.chat_models import ChatOpenAI
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.text_splitter import CharacterTextSplitter
-from halo import Halo
 
 from talk_codebase.utils import StreamStdOut, load_files
 
 
 @Halo(text='Creating vector store', spinner='dots')
 def create_vector_store(root_dir, openai_api_key):
     docs = load_files(root_dir)
```

### Comparing `talk_codebase-0.1.13/talk_codebase/utils.py` & `talk_codebase-0.1.14/talk_codebase/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,39 @@
 import os
 import sys
 
+from git import Repo
+from halo import Halo
 from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 from langchain.document_loaders import TextLoader
-from halo import Halo
 
 from talk_codebase.consts import EXCLUDE_DIRS, EXCLUDE_FILES, ALLOW_FILES
 
 
+def get_repo():
+    try:
+        return Repo()
+    except:
+        return None
+
+
+def has_repo():
+    return get_repo() is not None
+
+
+def is_ignored(path):
+    repo = get_repo()
+    if repo is None:
+        return False
+    if not os.path.exists(path):
+        return False
+    ignored = repo.ignored(path)
+    return len(ignored) > 0
+
+
 class StreamStdOut(StreamingStdOutCallbackHandler):
     def on_llm_new_token(self, token: str, **kwargs) -> None:
         sys.stdout.write(token)
         sys.stdout.flush()
 
     def on_llm_start(self, serialized, prompts, **kwargs):
         sys.stdout.write("🤖 ")
@@ -21,19 +43,23 @@
         sys.stdout.flush()
 
 
 def load_files(root_dir):
     spinners = Halo(text='Loading files', spinner='dots')
     docs = []
     for dirpath, dirnames, filenames in os.walk(root_dir):
+        if is_ignored(dirpath):
+            continue
         if any(exclude_dir in dirpath for exclude_dir in EXCLUDE_DIRS):
             continue
         if not filenames:
             continue
         for file in filenames:
+            if is_ignored(os.path.join(dirpath, file)):
+                continue
             if any(file.endswith(allow_file) for allow_file in ALLOW_FILES) and not any(
                     file == exclude_file for exclude_file in EXCLUDE_FILES):
                 try:
                     loader = TextLoader(os.path.join(dirpath, file), encoding='utf-8')
                     docs.extend(loader.load_and_split())
                 except Exception as e:
                     print(f"Error loading file {file}: {e}")
```

### Comparing `talk_codebase-0.1.13/PKG-INFO` & `talk_codebase-0.1.14/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.13
+Version: 0.1.14
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
+Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
-Requires-Dist: langchain (>=0.0.180,<0.0.181)
+Requires-Dist: langchain (>=0.0.181,<0.0.182)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
+Requires-Dist: urllib3 (==1.26.6)
 Description-Content-Type: text/markdown
 
 # talk-codebase is a powerful tool for chatting with your codebase
+
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
 
 <p align="center">
   <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/6d92e905-fb1b-4235-857b-e6e19041ad79" width="800" alt="chat">
 </p>
-
+ 
 ## Description
 
-In the chat, you can ask questions about the codebase. AI will answer your questions, and if necessary, it will offer code improvements. This is very convenient when you want to quickly find something in the codebase, but don't want to waste time searching. It is also convenient when you want to improve a specific function, you can ask "How can I improve the function {function name}?" and AI will suggest improvements. Codebase is analyzed using openai.
+In the chat, you can ask questions about the codebase. AI will answer your questions, and if necessary, it will offer
+code improvements. This is very convenient when you want to quickly find something in the codebase, but don't want to
+waste time searching. It is also convenient when you want to improve a specific function, you can ask "How can I improve
+the function {function name}?" and AI will suggest improvements. Codebase is analyzed using openai.
 
 ## Installation
 
 ```bash
 pip install talk-codebase
 ```
 
 ## Usage
 
-talk-codebase works only with files of popular programming languages and additionally with .txt files. All other files will be ignored.
+talk-codebase works only with files of popular programming languages and additionally with .txt files. All other files
+will be ignored.
+
 ```bash
 # Start chatting with your codebase
 talk-codebase chat <directory>
 
 # Configure
 talk-codebase configure
```

