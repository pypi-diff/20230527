# Comparing `tmp/embedbase_client-0.1.6.tar.gz` & `tmp/embedbase_client-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase_client-0.1.6.tar", max compression
+gzip compressed data, was "embedbase_client-0.1.7.tar", max compression
```

## Comparing `embedbase_client-0.1.6.tar` & `embedbase_client-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/LICENSE
--rw-r--r--   0        0        0     1005 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/README.md
--rw-r--r--   0        0        0      389 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/embedbase_client/__init__.py
--rw-r--r--   0        0        0    16767 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/embedbase_client/async_client.py
--rw-r--r--   0        0        0      913 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/embedbase_client/base.py
--rw-r--r--   0        0        0     1150 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/embedbase_client/errors.py
--rw-r--r--   0        0        0     1717 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/embedbase_client/model.py
--rw-r--r--   0        0        0     3388 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/embedbase_client/split.py
--rw-r--r--   0        0        0    16718 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/embedbase_client/sync_client.py
--rw-r--r--   0        0        0     2051 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/embedbase_client/utils.py
--rw-r--r--   0        0        0     3535 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2102 1970-01-01 00:00:00.000000 embedbase_client-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-27 16:09:15.167635 embedbase_client-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1005 2023-05-27 16:09:15.167635 embedbase_client-0.1.7/README.md
+-rw-r--r--   0        0        0      389 2023-05-27 16:09:15.167635 embedbase_client-0.1.7/embedbase_client/__init__.py
+-rw-r--r--   0        0        0    19402 2023-05-27 16:09:15.167635 embedbase_client-0.1.7/embedbase_client/async_client.py
+-rw-r--r--   0        0        0      913 2023-05-27 16:09:15.167635 embedbase_client-0.1.7/embedbase_client/base.py
+-rw-r--r--   0        0        0     1150 2023-05-27 16:09:15.167635 embedbase_client-0.1.7/embedbase_client/errors.py
+-rw-r--r--   0        0        0     1634 2023-05-27 16:09:15.167635 embedbase_client-0.1.7/embedbase_client/model.py
+-rw-r--r--   0        0        0     3388 2023-05-27 16:09:15.167635 embedbase_client-0.1.7/embedbase_client/split.py
+-rw-r--r--   0        0        0    19336 2023-05-27 16:09:15.167635 embedbase_client-0.1.7/embedbase_client/sync_client.py
+-rw-r--r--   0        0        0     2051 2023-05-27 16:09:15.167635 embedbase_client-0.1.7/embedbase_client/utils.py
+-rw-r--r--   0        0        0     3535 2023-05-27 16:09:15.167635 embedbase_client-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2102 1970-01-01 00:00:00.000000 embedbase_client-0.1.7/PKG-INFO
```

### Comparing `embedbase_client-0.1.6/LICENSE` & `embedbase_client-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.6/README.md` & `embedbase_client-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.6/embedbase_client/async_client.py` & `embedbase_client-0.1.7/embedbase_client/async_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from typing import Any, Dict, List, Optional
 
+import asyncio
+import itertools
 import json
 from dataclasses import dataclass
 
 import httpx
 from embedbase_client.base import BaseClient
 from embedbase_client.errors import EmbedbaseAPIException
 from embedbase_client.model import (
+    AddDocument,
     ClientDatasets,
     Document,
     GenerateOptions,
+    Metadata,
     SearchSimilarity,
 )
+from embedbase_client.split import split_text
 from embedbase_client.utils import CustomAsyncGenerator, async_stream
 
 
 class AsyncSearchBuilder:
     def __init__(
         self, client, dataset: str, query: str, options: Optional[Dict[str, Any]] = None
     ):
@@ -233,14 +238,33 @@
             A list of documents.
 
         Example usage:
             documents = await dataset.list()
         """
         return AsyncListBuilder(self.client, self.dataset)
 
+    async def chunk_and_batch_add(self, documents: List[AddDocument]) -> List[Document]:
+        """
+        Chunk and add multiple documents to the specified dataset in a single batch asynchronously.
+
+        Args:
+            documents: A list of documents.
+
+        Returns:
+            A list of documents.
+
+        Example usage:
+            documents = [
+                {"data": "Python is a programming language.", metadata: {"topic": "programming"}},
+                {"data": "Java is also a programming language.", metadata: {"topic": "programming"}},
+            ]
+            results = await dataset.chunk_and_batch_add(documents)
+        """
+        return await self.client.chunk_and_batch_add(self.dataset, documents)
+
 
 class EmbedbaseAsyncClient(BaseClient):
     def dataset(self, dataset: str) -> AsyncDataset:
         return AsyncDataset(client=self, dataset=dataset)
 
     async def create_context(
         self, dataset: str, query: str, limit: Optional[int] = None
@@ -296,15 +320,15 @@
 
         Example usage:
             results = await embedbase.search("my_dataset", "What is Python?", limit=3)
         """
         return AsyncSearchBuilder(self, dataset, query, {"limit": limit})
 
     async def add(
-        self, dataset: str, document: str, metadata: Optional[Dict[str, Any]] = None
+        self, dataset: str, document: str, metadata: Optional[Metadata] = None
     ) -> Document:
         """
         Add a document to the specified dataset asynchronously.
         Args:
             dataset: The name of the dataset to add the document to.
             document: The document string to add to the dataset.
             metadata: Optional metadata about the document.
@@ -331,15 +355,15 @@
             raise EmbedbaseAPIException(res.text)
 
         if res.status_code != 200:
             raise EmbedbaseAPIException(data.get("error", res.text))
         return Document(**data["results"][0])
 
     async def batch_add(
-        self, dataset: str, documents: List[Dict[str, Any]]
+        self, dataset: str, documents: List[AddDocument]
     ) -> List[Document]:
         """
         Add multiple documents to the specified dataset in a single batch asynchronously.
 
         Args:
             dataset: The name of the dataset to add the documents to.
             documents: A list of documents.
@@ -449,15 +473,15 @@
             prompt (str): The text prompt to send to the API for generating responses.
             options (dict, optional): Options for the generation process, including history.
                                     Defaults to None.
 
         Returns:
             CustomAsyncGenerator[str, None, None]: An asynchronous generator that yields generated text data in chunks.
         """
-        url = (options and options.get("url")) or f"https://app.embedbase.xyz/api/chat"
+        url = (options and options.get("url")) or "https://app.embedbase.xyz/api/chat"
 
         options = options or {
             "history": [],
         }
 
         system = ""
         if options.get("history"):
@@ -477,7 +501,58 @@
             url,
             json.dumps(
                 {"prompt": prompt, "system": system, "history": options["history"]}
             ),
             self.headers,
         )
         return CustomAsyncGenerator(async_gen)
+
+    async def chunk_and_batch_add(
+        self, dataset: str, documents: List[AddDocument]
+    ) -> List[Document]:
+        """
+        Chunk and add multiple documents to the specified dataset in a single batch asynchronously.
+
+        Args:
+            dataset: The name of the dataset to add the documents to.
+            documents: A list of documents.
+
+        Returns:
+            A list of documents.
+
+        Example usage:
+            documents = [
+                {"data": "Python is a programming language.", metadata: {"topic": "programming"}},
+                {"data": "Java is also a programming language.", metadata: {"topic": "programming"}},
+            ]
+            results = await embedbase.batch_add("my_dataset", documents)
+        """
+        chunks = []
+        for document_index, document in enumerate(documents):
+            for chunk_index, chunk in enumerate(split_text(document["data"])):
+                chunks.append(
+                    {
+                        "data": chunk.chunk,
+                        "metadata": {
+                            **document["metadata"],
+                            "documentIndex": document_index,
+                            "chunkIndex": chunk_index,
+                            "chunkStart": chunk.start,
+                            "chunkEnd": chunk.end,
+                        },
+                    }
+                )
+
+        parallel_batch_size = 100
+
+        def batch_chunks(l, n):
+            for i in range(0, len(l), n):
+                yield l[i : i + n]
+
+        results = await asyncio.gather(
+            *[
+                self.batch_add(dataset, batch)
+                for batch in batch_chunks(chunks, parallel_batch_size)
+            ]
+        )
+
+        return list(itertools.chain.from_iterable(results))
```

### Comparing `embedbase_client-0.1.6/embedbase_client/base.py` & `embedbase_client-0.1.7/embedbase_client/base.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.6/embedbase_client/errors.py` & `embedbase_client-0.1.7/embedbase_client/errors.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.6/embedbase_client/model.py` & `embedbase_client-0.1.7/embedbase_client/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Any, Dict, List, Optional
+
 from pydantic import BaseModel, Extra
 
 
 class Metadata(BaseModel):
     path: Optional[str]
 
     def __getitem__(self, key: str) -> Any:
@@ -35,22 +36,17 @@
 
 
 class ClientDatasets:
     dataset_id: str
     documents_count: int
 
 
-class ClientAddData(BaseModel):
-    id: Optional[str]
-    status: str
-
-
-class BatchAddDocument(BaseModel):
+class AddDocument(BaseModel):
     data: str
-    metadata: Optional[Dict[str, Any]]
+    metadata: Optional[Metadata]
 
 
 class SearchSimilarity(Document):
     similarity: float
 
 
 class SearchData(BaseModel):
@@ -67,15 +63,14 @@
 
 
 class AddData(BaseModel):
     results: Optional[List[AddDataResult]]
     error: Optional[str]
 
 
-
 class Chat(BaseModel):
     role: str
     content: str
 
 
 class GenerateOptions(BaseModel):
     history: List[Chat]
```

### Comparing `embedbase_client-0.1.6/embedbase_client/split.py` & `embedbase_client-0.1.7/embedbase_client/split.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.6/embedbase_client/sync_client.py` & `embedbase_client-0.1.7/embedbase_client/sync_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from typing import Any, Dict, Generator, List, Optional
 
+import itertools
 import json
 from dataclasses import dataclass
+from multiprocessing.pool import ThreadPool
 
 import requests
 from embedbase_client.base import BaseClient
 from embedbase_client.errors import EmbedbaseAPIException
 from embedbase_client.model import (
+    AddDocument,
     ClientDatasets,
     Document,
     GenerateOptions,
     Metadata,
     SearchSimilarity,
 )
+from embedbase_client.split import split_text
 from embedbase_client.utils import sync_stream
 
 
 class SyncSearchBuilder:
     def __init__(
         self,
         client: BaseClient,
@@ -233,14 +237,33 @@
             A list of document IDs and metadata.
 
         Example usage:
             documents = dataset.list()
         """
         return SyncListBuilder(self.client, self.dataset, {})
 
+    def chunk_and_batch_add(self, documents: List[AddDocument]) -> List[Document]:
+        """
+        Chunk and add multiple documents to the specified dataset in a single batch.
+
+        Args:
+            documents: A list of documents.
+
+        Returns:
+            A list of documents.
+
+        Example usage:
+            documents = [
+                {"data": "Python is a programming language.", metadata: {"topic": "programming"}},
+                {"data": "Java is also a programming language.", metadata: {"topic": "programming"}},
+            ]
+            results = dataset.chunk_and_batch_add(documents)
+        """
+        return self.client.chunk_and_batch_add(self.dataset, documents)
+
 
 class EmbedbaseClient(BaseClient):
     def __init__(
         self,
         embedbase_url: str = "https://api.embedbase.xyz",
         embedbase_key: Optional[str] = None,
         fastapi_app: Optional[Any] = None,
@@ -353,17 +376,15 @@
 
         data = res.json()
 
         return Document(
             **data["results"][0],
         )
 
-    def batch_add(
-        self, dataset: str, documents: List[Dict[str, Any]]
-    ) -> List[Document]:
+    def batch_add(self, dataset: str, documents: List[AddDocument]) -> List[Document]:
         """
         Add multiple documents to the specified dataset in a single batch.
 
         Args:
             dataset: The name of the dataset to add the documents to.
             documents: A list of documents.
 
@@ -472,15 +493,15 @@
             prompt (str): The text prompt to send to the API for generating responses.
             options (dict, optional): Options for the generation process, including history.
                                     Defaults to None.
 
         Returns:
             Generator[str, None, None]: A synchronous generator that yields generated text data in chunks.
         """
-        url = (options and options.get("url")) or f"https://app.embedbase.xyz/api/chat"
+        url = (options and options.get("url")) or "https://app.embedbase.xyz/api/chat"
 
         options = options or {
             "history": [],
         }
 
         system = ""
         if options.get("history"):
@@ -500,7 +521,59 @@
             url,
             json.dumps(
                 {"prompt": prompt, "system": system, "history": options["history"]}
             ),
             self.headers,
             self.timeout,
         )
+
+    def chunk_and_batch_add(
+        self, dataset: str, documents: List[AddDocument]
+    ) -> List[Document]:
+        """
+        Add multiple documents to the specified dataset in a single batch asynchronously.
+
+        Args:
+            dataset: The name of the dataset to add the documents to.
+            documents: A list of documents.
+
+        Returns:
+            A list of documents.
+
+        Example usage:
+            documents = [
+                {"data": "Python is a programming language.", metadata: {"topic": "programming"}},
+                {"data": "Java is also a programming language.", metadata: {"topic": "programming"}},
+            ]
+            results = await embedbase.batch_add("my_dataset", documents)
+        """
+        chunks = []
+        for document_index, document in enumerate(documents):
+            for chunk_index, chunk in enumerate(split_text(document["data"])):
+                chunks.append(
+                    {
+                        "data": chunk.chunk,
+                        "metadata": {
+                            **document["metadata"],
+                            "documentIndex": document_index,
+                            "chunkIndex": chunk_index,
+                            "chunkStart": chunk.start,
+                            "chunkEnd": chunk.end,
+                        },
+                    }
+                )
+
+        parallel_batch_size = 100
+
+        def batch_chunks(l, n):
+            for i in range(0, len(l), n):
+                yield l[i : i + n]
+
+        results = []
+
+        def add_batch(batch):
+            results.append(self.batch_add(dataset, batch))
+
+        with ThreadPool() as pool:
+            pool.map(add_batch, batch_chunks(chunks, parallel_batch_size))
+
+        return list(itertools.chain.from_iterable(results))
```

### Comparing `embedbase_client-0.1.6/embedbase_client/utils.py` & `embedbase_client-0.1.7/embedbase_client/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.6/pyproject.toml` & `embedbase_client-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase-client"
-version = "0.1.6"
+version = "0.1.7"
 description = "Python client for Embedbase"
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py"
 homepage = "https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py"
```

### Comparing `embedbase_client-0.1.6/PKG-INFO` & `embedbase_client-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase-client
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python client for Embedbase
 Home-page: https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embedbase-client Version: 0.1.6 Summary: Python
+Metadata-Version: 2.1 Name: embedbase-client Version: 0.1.7 Summary: Python
 client for Embedbase Home-page: https://github.com/different-ai/embedbase/tree/
 main/sdk/embedbase-py License: MIT Keywords: embeddings,machine
 learning,artificial intelligence,llm Author: Different AI Author-email:
 louis@embedbase.xyz Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

