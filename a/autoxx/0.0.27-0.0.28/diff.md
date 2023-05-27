# Comparing `tmp/autoxx-0.0.27.tar.gz` & `tmp/autoxx-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.27.tar", max compression
+gzip compressed data, was "autoxx-0.0.28.tar", max compression
```

## Comparing `autoxx-0.0.27.tar` & `autoxx-0.0.28.tar`

### file list

```diff
@@ -1,12 +1,19 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.27/README.md
--rw-r--r--   0        0        0     7222 2023-05-24 03:15:10.185371 autoxx-0.0.27/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.27/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    11000 2023-05-24 03:30:40.854436 autoxx-0.0.27/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.27/autoxx/requirements.txt
--rw-r--r--   0        0        0      801 2023-05-23 08:04:17.676812 autoxx-0.0.27/autoxx/setup.py
--rw-r--r--   0        0        0     5352 2023-05-22 11:51:39.068804 autoxx-0.0.27/autoxx/tools/knowledge_base/utils.py
--rw-r--r--   0        0        0      929 2023-05-22 06:15:52.199109 autoxx-0.0.27/autoxx/tools/llm/utils.py
--rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.27/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0     6473 2023-05-23 10:03:19.637350 autoxx-0.0.27/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0      664 2023-05-24 03:30:57.645010 autoxx-0.0.27/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 autoxx-0.0.27/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.28/README.md
+-rw-r--r--   0        0        0     7195 2023-05-27 09:14:52.541250 autoxx-0.0.28/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.28/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.28/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0     6052 2023-05-27 08:29:33.321541 autoxx-0.0.28/autoxx/config/config.py
+-rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.28/autoxx/requirements.txt
+-rw-r--r--   0        0        0      230 2023-05-27 08:43:09.345534 autoxx-0.0.28/autoxx/setup.py
+-rw-r--r--   0        0        0     5315 2023-05-27 10:32:18.140459 autoxx-0.0.28/autoxx/tools/knowledge_base/base.py
+-rw-r--r--   0        0        0      409 2023-05-26 07:39:48.123009 autoxx-0.0.28/autoxx/tools/llm/base.py
+-rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.28/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0    11819 2023-05-27 10:32:41.926545 autoxx-0.0.28/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0     1060 2023-05-27 00:53:33.776643 autoxx-0.0.28/autoxx/utils/base.py
+-rw-r--r--   0        0        0     3198 2023-05-27 10:33:03.387959 autoxx-0.0.28/autoxx/utils/llm.py
+-rw-r--r--   0        0        0     1905 2023-05-26 07:22:28.056438 autoxx-0.0.28/autoxx/utils/openai_models.py
+-rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.28/autoxx/utils/processing_html.py
+-rw-r--r--   0        0        0     5550 2023-05-27 10:33:16.566378 autoxx-0.0.28/autoxx/utils/processing_text.py
+-rw-r--r--   0        0        0     2631 2023-05-27 01:02:06.078829 autoxx-0.0.28/autoxx/utils/token_counter.py
+-rw-r--r--   0        0        0      633 2023-05-27 11:00:15.559904 autoxx-0.0.28/pyproject.toml
+-rw-r--r--   0        0        0      993 1970-01-01 00:00:00.000000 autoxx-0.0.28/PKG-INFO
```

### Comparing `autoxx-0.0.27/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.28/autoxx/agent/babyagi/agi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json, time
 from typing import Dict, List, Dict, Optional
 import logging
 
-from autogpt.llm_utils import create_chat_completion
-from autogpt.config import Config
+from autoxx.tools.llm.base import get_chat_completion
 
 from autoxx.tools.web_search.search import web_search
-from autoxx.tools.llm.utils import llm_uils, create_message
+from autoxx.tools.llm.base import llm_uils
+from autoxx.utils.llm import create_message
 
 
 class AGIExecutor:
     def __init__(self, objective:str, max_tasks_count: Optional[int] = 5):
         if objective is None or len(objective) <= 1:  
             raise ValueError("Must provide an objective")  
 
@@ -43,17 +43,17 @@
             f"Do not create any summarizing steps outside of the last step.\n"
             f"The task list output format is as follows: "
             "[{\"id\": 1, \"task\": \"Untapped Capital\", \"tool\": \"web-search\", \"dependent_task_ids\": [], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}, {\"id\": 2, \"task\": \"Consider additional insights that can be reasoned from the results of...\", \"tool\": \"text-completion\", \"dependent_task_ids\": [1], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}].\n"
             f"Ensure the output can be parsed by Python json.loads.\n task list="
         )
 
         messages = create_message(prompt)
-        response = create_chat_completion(
-            model=Config().smart_llm_model,
+        response = get_chat_completion(
             messages=messages,
+            model="gpt-4"
         )
 
         new_tasks = json.loads(response)
         task_list = []
         for new_task in new_tasks:
             task_id_counter += 1
             new_task.update({"id": task_id_counter})
```

### Comparing `autoxx-0.0.27/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.28/autoxx/agent/babyagi/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.27/autoxx/agent/react/agent.py` & `autoxx-0.0.28/autoxx/agent/react/agent.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from langchain.prompts import StringPromptTemplate
 from langchain import LLMChain
 from langchain.chat_models import ChatOpenAI
 from langchain.schema import AgentAction, AgentFinish, OutputParserException
 from langchain.tools.base import BaseTool
 from langchain.agents.tools import InvalidTool
 
-from autogpt.config import Config
-from autoxx.tools.llm.utils import llm_uils
+from autoxx.config.config import GlobalConfig
+from autoxx.tools.llm.base import llm_uils
 
 
 # Set up the base template
 template = """Answer the following questions as best you can. You have access to the following tools:
 
 {tools}
 
@@ -81,40 +81,32 @@
         # Return the action and action input
         return AgentAction(tool=action, tool_input=action_input.strip(" ").strip('"'), log=llm_output)
 
     
 def setup_planner(tools: List[Tool], model: str = "gpt-3.5-turbo") -> BaseSingleActionAgent:
     tool_names = [tool.name for tool in tools]
     output_parser = CustomOutputParser()
-    config = Config()
+    config = GlobalConfig().get()
 
     prompt = CustomPromptTemplate(
         template=template,
         tools=tools,
         # This omits the `agent_scratchpad`, `tools`, and `tool_names` variables because those are generated dynamically
         # This includes the `intermediate_steps` variable because that is needed
         input_variables=["input", "intermediate_steps"]
     )
 
-    if model == config.fast_llm_model:
-        llm = ChatOpenAI(temperature=0, model_name=config.fast_llm_model, model_kwargs={
-                "api_key": config.openai_api_key,
-                "api_base": config.openai_api_base,
-                "api_type": config.openai_api_type,
-                "api_version": config.openai_api_version,
-                "deployment_id": config.get_azure_deployment_id_for_model(config.fast_llm_model),
-            })
-    elif model == config.smart_llm_model:
-         llm = ChatOpenAI(temperature=0, model_name=config.smart_llm_model, model_kwargs={
-                "api_key": config.openai_api_key,
-                "api_base": config.openai_api_base,
-                "api_type": config.openai_api_type,
-                "api_version": config.openai_api_version,
-                "deployment_id": config.get_azure_deployment_id_for_model(config.smart_llm_model),
-            })
+    model_config = config.get_llm_model_config(model)
+    llm = ChatOpenAI(temperature=0, model_name=model_config.model, model_kwargs={
+        "api_key": model_config.api_key,
+        "api_base": model_config.api_base,
+        "api_type": model_config.api_type,
+        "api_version": model_config.api_version,
+        "deployment_id": model_config.api_deployment_id,
+    })
 
     # LLM chain consisting of the LLM and a prompt
     llm_chain = LLMChain(llm=llm, prompt=prompt)
     return LLMSingleActionAgent(
         llm_chain=llm_chain, 
         output_parser=output_parser,
         stop=["\nObservation:"],
```

### Comparing `autoxx-0.0.27/autoxx/tools/knowledge_base/utils.py` & `autoxx-0.0.28/autoxx/tools/knowledge_base/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import pinecone
 import os
 from langchain.chat_models import ChatOpenAI
-from autogpt.config import Config
+from autoxx.config.config import GlobalConfig
 from llama_index.embeddings.openai import OpenAIEmbedding
 
 from llama_index import (LLMPredictor,
                         ServiceContext,
                         StorageContext)
 from llama_index.indices.loading import load_index_from_storage
 from llama_index.storage.docstore import MongoDocumentStore
 from llama_index.storage.index_store import MongoIndexStore
 from llama_index.vector_stores import PineconeVectorStore
 from llama_index.readers.schema.base import Document
-from typing import List, Dict
+from typing import List
 from llama_index.node_parser import SimpleNodeParser
 from llama_index.langchain_helpers.text_splitter import TokenTextSplitter
 from llama_index.callbacks.base import CallbackManager
 
 class knowleage_bot:
 
-    def __init__(self, corpus:str, model:str = "gpt-3.5-turbo"):
+    def __init__(self, corpus:str, model:str = "gpt-3.5-turbo", embedding_model: str="text-embedding-ada-002"):
         self.corpus = corpus
         self.model = model
+        self.embedding_model = embedding_model
         mongodb_dbname = self.corpus
 
         mongodb_password = os.getenv("MONGODB_PASSWORD")
         assert mongodb_password is not None, "Please set MONGODB_PASSWORD environment variable"
         mongodb_user = os.getenv("MONGODB_USER") or "raga"
-        mongodb_url = f"mongodb+srv://{mongodb_user}:{mongodb_password}@cluster0.spj0g.mongodb.net/?retryWrites=true&w=majority"
+        mongodb_host = os.getenv("MONGODB_HOST") or "cluster0.spj0g.mongodb.net"
+        mongodb_url = f"mongodb+srv://{mongodb_user}:{mongodb_password}@{mongodb_host}/?retryWrites=true&w=majority"
 
         # create mongodb docstore, indexstore
         self.docstore = MongoDocumentStore.from_uri(uri=mongodb_url, db_name=mongodb_dbname)
         self.index_store = MongoIndexStore.from_uri(uri=mongodb_url, db_name=mongodb_dbname)
         pinecone_api_key = os.getenv("PINECONE_API_KEY")
         assert pinecone_api_key is not None, "Please set PINECONE_API_KEY environment variable"
         pinecone_environment =  os.getenv("PINECONE_ENVIRONMENT") or "us-central1-gcp"
@@ -43,39 +45,35 @@
 
         storage_context = StorageContext.from_defaults(
             docstore=self.docstore,
             index_store=self.index_store,
             vector_store=self.vector_store,
         )
 
-        config = Config()
-        if config.use_azure:
-            llm = ChatOpenAI(model_name= config.fast_llm_model, model_kwargs={
-                "api_key": config.openai_api_key,
-                "api_base": config.openai_api_base,
-                "api_type": config.openai_api_type,
-                "api_version": config.openai_api_version,
-                "deployment_id": config.get_azure_deployment_id_for_model(config.fast_llm_model),
-            })
-            llm_predictor_chatgpt = LLMPredictor(
-                llm=llm
-            )
-            embed_model = OpenAIEmbedding(
-                deployment_name=config.get_azure_deployment_id_for_model("text-embedding-ada-002"),
-                api_key=config.openai_api_key,
-                api_base=config.openai_api_base,
-                api_type=config.openai_api_type,
-                api_version=config.openai_api_version,
-            )
-        else:
-            print(config.use_azure, config.openai_api_key)
-            llm_predictor_chatgpt = LLMPredictor(
-                llm=ChatOpenAI(temperature=0, model_name="gpt-3.5-turbo")
-            )
-            embed_model = OpenAIEmbedding()
+        config = GlobalConfig().get()
+        llm_model_config = config.get_llm_model_config(self.model)
+        llm = ChatOpenAI(model_name= llm_model_config.model, model_kwargs={
+            "api_key": llm_model_config.api_key,
+            "api_base": llm_model_config.api_base,
+            "api_type": llm_model_config.api_type,
+            "api_version": llm_model_config.api_version,
+            "deployment_id": llm_model_config.api_deployment_id,
+        })
+        llm_predictor_chatgpt = LLMPredictor(
+            llm=llm
+        )
+        embed_model_config = config.get_embedding_model_config(self.embedding_model)
+        embed_model = OpenAIEmbedding(
+            deployment_name=embed_model_config.api_deployment_id,
+            api_key=embed_model_config.api_key,
+            api_base=embed_model_config.api_base,
+            api_type=embed_model_config.api_type,
+            api_version=embed_model_config.api_version,
+        )
+       
         service_context = ServiceContext.from_defaults(
             llm_predictor=llm_predictor_chatgpt, chunk_size_limit=1024, embed_model=embed_model,
             node_parser=SimpleNodeParser(
                 text_splitter=TokenTextSplitter(
                     callback_manager=CallbackManager([]),
                     chunk_size = 2048,
             ))
```

### Comparing `autoxx-0.0.27/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.28/autoxx/tools/web_search/js/overlay.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -14,16 +14,16 @@
     justifyContent: 'center',
     alignItems: 'center',
 });
 const textContent = document.createElement('div');
 Object.assign(textContent.style, {
     textAlign: 'center',
 });
-textContent.textContent = 'AutoGPT Analyzing Page';
+textContent.textContent = 'Analyzing Page';
 overlay.appendChild(textContent);
 document.body.append(overlay);
 document.body.style.overflow = 'hidden';
 let dotCount = 0;
 setInterval(() => {
-    textContent.textContent = 'AutoGPT Analyzing Page' + '.'.repeat(dotCount);
+    textContent.textContent = 'Analyzing Page' + '.'.repeat(dotCount);
     dotCount = (dotCount + 1) % 4;
 }, 1000);
```

### Comparing `autoxx-0.0.27/pyproject.toml` & `autoxx-0.0.28/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.27"
+version = "0.0.28"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pinecone-client = "2.2.1"
-agpt = "0.2.2"
 selenium = "4.9.0"
 openai = "0.27.6"
-auto_gpt_plugin_template = "0.0.3"
 colorama = "0.4.6"
 python-dotenv = "1.0.0"
 bs4 = "0.0.1"
 webdriver_manager = "3.8.6"
 tiktoken = "0.3.3"
 playsound = "1.2.2"
 gTTS = "2.3.1"
 orjson = "3.8.10"
 spacy = ">=3.0.0,<4.0.0"
 llama-index = "^0.6.9"
 google-api-python-client = "^2.86.0"
+pymongo = "^4.3.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `autoxx-0.0.27/PKG-INFO` & `autoxx-0.0.28/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.27
+Version: 0.0.28
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: agpt (==0.2.2)
-Requires-Dist: auto_gpt_plugin_template (==0.0.3)
 Requires-Dist: bs4 (==0.0.1)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: gTTS (==2.3.1)
 Requires-Dist: google-api-python-client (>=2.86.0,<3.0.0)
 Requires-Dist: llama-index (>=0.6.9,<0.7.0)
 Requires-Dist: openai (==0.27.6)
 Requires-Dist: orjson (==3.8.10)
 Requires-Dist: pinecone-client (==2.2.1)
 Requires-Dist: playsound (==1.2.2)
+Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: selenium (==4.9.0)
 Requires-Dist: spacy (>=3.0.0,<4.0.0)
 Requires-Dist: tiktoken (==0.3.3)
 Requires-Dist: webdriver_manager (==3.8.6)
 Description-Content-Type: text/markdown
```

