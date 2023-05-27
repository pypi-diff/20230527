# Comparing `tmp/talk_codebase-0.1.14.tar.gz` & `tmp/talk_codebase-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.14.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.15.tar", max compression
```

## Comparing `talk_codebase-0.1.14.tar` & `talk_codebase-0.1.15.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1237 2023-05-27 01:21:38.748767 talk_codebase-0.1.14/README.md
--rw-r--r--   0        0        0      785 2023-05-27 01:21:38.748767 talk_codebase-0.1.14/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-27 01:21:38.748767 talk_codebase-0.1.14/talk_codebase/__init__.py
--rw-r--r--   0        0        0     1897 2023-05-27 01:21:38.748767 talk_codebase-0.1.14/talk_codebase/cli.py
--rw-r--r--   0        0        0      518 2023-05-27 01:21:38.748767 talk_codebase-0.1.14/talk_codebase/consts.py
--rw-r--r--   0        0        0     1451 2023-05-27 01:21:38.748767 talk_codebase-0.1.14/talk_codebase/llm.py
--rw-r--r--   0        0        0     1945 2023-05-27 01:21:38.748767 talk_codebase-0.1.14/talk_codebase/utils.py
--rw-r--r--   0        0        0     2054 1970-01-01 00:00:00.000000 talk_codebase-0.1.14/PKG-INFO
+-rw-r--r--   0        0        0     1237 2023-05-27 02:38:14.577253 talk_codebase-0.1.15/README.md
+-rw-r--r--   0        0        0      787 2023-05-27 02:38:14.581253 talk_codebase-0.1.15/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-27 02:38:14.581253 talk_codebase-0.1.15/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     1960 2023-05-27 02:38:14.581253 talk_codebase-0.1.15/talk_codebase/cli.py
+-rw-r--r--   0        0        0      518 2023-05-27 02:38:14.581253 talk_codebase-0.1.15/talk_codebase/consts.py
+-rw-r--r--   0        0        0     1530 2023-05-27 02:38:14.581253 talk_codebase-0.1.15/talk_codebase/llm.py
+-rw-r--r--   0        0        0     1947 2023-05-27 02:38:14.581253 talk_codebase-0.1.15/talk_codebase/utils.py
+-rw-r--r--   0        0        0     2054 1970-01-01 00:00:00.000000 talk_codebase-0.1.15/PKG-INFO
```

### Comparing `talk_codebase-0.1.14/README.md` & `talk_codebase-0.1.15/README.md`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.14/pyproject.toml` & `talk_codebase-0.1.15/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.14"
+version = "0.1.15"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
-packages = [{include = "talk_codebase"}]
+packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 langchain = "^0.0.181"
 fire = "^0.5.0"
 openai = "^0.27.7"
```

### Comparing `talk_codebase-0.1.14/talk_codebase/cli.py` & `talk_codebase-0.1.15/talk_codebase/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,31 +29,35 @@
     api_key = input("🤖 Enter your OpenAI API key: ")
     model_name = input("🤖 Enter your model name (default: gpt-3.5-turbo): ") or "gpt-3.5-turbo"
     config["api_key"] = api_key
     config["model_name"] = model_name
     save_config(config)
 
 
+def loop(vector_store, api_key, model_name):
+    while True:
+        question = input("👉 ")
+        if not question:
+            print("🤖 Please enter a question.")
+            continue
+        if question.lower() in ('exit', 'quit'):
+            break
+        send_question(question, vector_store, api_key, model_name)
+
+
 def chat(root_dir):
     try:
         config = get_config()
         api_key = config.get("api_key")
         model_name = config.get("model_name")
         if not (api_key and model_name):
             configure()
             chat(root_dir)
         vector_store = create_vector_store(root_dir, api_key)
-        while True:
-            question = input("👉 ")
-            if not question:
-                print("🤖 Please enter a question.")
-                continue
-            if question.lower() in ('exit', 'quit'):
-                break
-            send_question(question, vector_store, api_key, model_name)
+        loop(vector_store, api_key, model_name)
     except KeyboardInterrupt:
         print("\n🤖 Bye!")
     except Exception as e:
         if str(e) == "<empty message>":
             print("🤖 Please configure your API key.")
             configure()
             chat(root_dir)
```

### Comparing `talk_codebase-0.1.14/talk_codebase/consts.py` & `talk_codebase-0.1.15/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.14/talk_codebase/llm.py` & `talk_codebase-0.1.15/talk_codebase/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
 from talk_codebase.utils import StreamStdOut, load_files
 
 
 @Halo(text='Creating vector store', spinner='dots')
 def create_vector_store(root_dir, openai_api_key):
     docs = load_files(root_dir)
+    if len(docs) == 0:
+        print("✘ No documents found")
+        exit(0)
     text_splitter = CharacterTextSplitter(chunk_size=1000, chunk_overlap=0)
     texts = text_splitter.split_documents(docs)
 
     embeddings = OpenAIEmbeddings(openai_api_key=openai_api_key)
     db = FAISS.from_documents(texts, embeddings)
 
     return db
```

### Comparing `talk_codebase-0.1.14/talk_codebase/utils.py` & `talk_codebase-0.1.15/talk_codebase/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,27 +5,23 @@
 from halo import Halo
 from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 from langchain.document_loaders import TextLoader
 
 from talk_codebase.consts import EXCLUDE_DIRS, EXCLUDE_FILES, ALLOW_FILES
 
 
-def get_repo():
+def get_repo(root_dir):
     try:
-        return Repo()
+        return Repo(root_dir)
     except:
         return None
 
 
-def has_repo():
-    return get_repo() is not None
-
-
-def is_ignored(path):
-    repo = get_repo()
+def is_ignored(path, root_dir):
+    repo = get_repo(root_dir)
     if repo is None:
         return False
     if not os.path.exists(path):
         return False
     ignored = repo.ignored(path)
     return len(ignored) > 0
 
@@ -43,22 +39,22 @@
         sys.stdout.flush()
 
 
 def load_files(root_dir):
     spinners = Halo(text='Loading files', spinner='dots')
     docs = []
     for dirpath, dirnames, filenames in os.walk(root_dir):
-        if is_ignored(dirpath):
+        if is_ignored(dirpath, root_dir):
             continue
         if any(exclude_dir in dirpath for exclude_dir in EXCLUDE_DIRS):
             continue
         if not filenames:
             continue
         for file in filenames:
-            if is_ignored(os.path.join(dirpath, file)):
+            if is_ignored(os.path.join(dirpath, file), root_dir):
                 continue
             if any(file.endswith(allow_file) for allow_file in ALLOW_FILES) and not any(
                     file == exclude_file for exclude_file in EXCLUDE_FILES):
                 try:
                     loader = TextLoader(os.path.join(dirpath, file), encoding='utf-8')
                     docs.extend(loader.load_and_split())
                 except Exception as e:
```

### Comparing `talk_codebase-0.1.14/PKG-INFO` & `talk_codebase-0.1.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.14
+Version: 0.1.15
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

