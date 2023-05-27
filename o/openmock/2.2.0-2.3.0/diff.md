# Comparing `tmp/openmock-2.2.0.tar.gz` & `tmp/openmock-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmock-2.2.0.tar", max compression
+gzip compressed data, was "openmock-2.3.0.tar", max compression
```

## Comparing `openmock-2.2.0.tar` & `openmock-2.3.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1081 2023-02-25 16:59:27.795654 openmock-2.2.0/LICENSE
--rw-r--r--   0        0        0      830 2023-02-25 15:59:51.627751 openmock-2.2.0/openmock/__init__.py
--rw-r--r--   0        0        0      121 2023-02-25 14:23:58.983906 openmock-2.2.0/openmock/behaviour/__init__.py
--rw-r--r--   0        0        0      475 2023-02-25 15:44:39.634633 openmock-2.2.0/openmock/behaviour/server_failure.py
--rw-r--r--   0        0        0     1100 2023-02-25 15:44:39.650234 openmock-2.2.0/openmock/fake_cluster.py
--rw-r--r--   0        0        0     1179 2023-02-25 15:44:39.681003 openmock-2.2.0/openmock/fake_indices.py
--rw-r--r--   0        0        0    38912 2023-02-25 16:14:15.578997 openmock-2.2.0/openmock/fake_opensearch.py
--rw-r--r--   0        0        0     2154 2023-02-25 15:57:03.276687 openmock-2.2.0/openmock/normalize_hosts.py
--rw-r--r--   0        0        0      732 2023-02-25 14:23:58.986909 openmock-2.2.0/openmock/utilities/__init__.py
--rw-r--r--   0        0        0      451 2023-02-25 16:14:15.032995 openmock-2.2.0/openmock/utilities/decorator.py
--rw-r--r--   0        0        0     2302 2023-02-25 17:31:20.740524 openmock-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     4946 2023-02-25 16:59:27.826133 openmock-2.2.0/README.md
--rw-r--r--   0        0        0     5881 1970-01-01 00:00:00.000000 openmock-2.2.0/setup.py
--rw-r--r--   0        0        0     6659 1970-01-01 00:00:00.000000 openmock-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-27 19:27:59.010484 openmock-2.3.0/LICENSE
+-rw-r--r--   0        0        0     4946 2023-05-27 19:27:59.010484 openmock-2.3.0/README.md
+-rw-r--r--   0        0        0      830 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/__init__.py
+-rw-r--r--   0        0        0      121 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/behaviour/__init__.py
+-rw-r--r--   0        0        0      475 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/behaviour/server_failure.py
+-rw-r--r--   0        0        0     1100 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/fake_cluster.py
+-rw-r--r--   0        0        0     1179 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/fake_indices.py
+-rw-r--r--   0        0        0    39864 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/fake_opensearch.py
+-rw-r--r--   0        0        0     2154 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/normalize_hosts.py
+-rw-r--r--   0        0        0      732 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/utilities/__init__.py
+-rw-r--r--   0        0        0      451 2023-05-27 19:27:59.010484 openmock-2.3.0/openmock/utilities/decorator.py
+-rw-r--r--   0        0        0     2302 2023-05-27 19:27:59.010484 openmock-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 openmock-2.3.0/PKG-INFO
```

### Comparing `openmock-2.2.0/LICENSE` & `openmock-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openmock-2.2.0/openmock/__init__.py` & `openmock-2.3.0/openmock/__init__.py`

 * *Files identical despite different names*

### Comparing `openmock-2.2.0/openmock/fake_cluster.py` & `openmock-2.3.0/openmock/fake_cluster.py`

 * *Files identical despite different names*

### Comparing `openmock-2.2.0/openmock/fake_indices.py` & `openmock-2.3.0/openmock/fake_indices.py`

 * *Files identical despite different names*

### Comparing `openmock-2.2.0/openmock/fake_opensearch.py` & `openmock-2.3.0/openmock/fake_opensearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from collections import defaultdict
 
 import dateutil.parser
 import ranges
 
 from opensearchpy import OpenSearch
 from opensearchpy.client.utils import query_params
-from opensearchpy.exceptions import NotFoundError, RequestError
+from opensearchpy.exceptions import NotFoundError, RequestError, ConflictError
 from opensearchpy.transport import Transport
 
 from openmock.behaviour.server_failure import server_failure
 from openmock.fake_cluster import FakeClusterClient
 from openmock.fake_indices import FakeIndicesClient
 from openmock.normalize_hosts import _normalize_hosts
 from openmock.utilities import (
@@ -382,14 +382,47 @@
         "routing",
         "timeout",
         "timestamp",
         "ttl",
         "version",
         "version_type",
     )
+    def create(self, index, body, doc_type="_doc", id=None, params=None, headers=None):
+        if self.exists(index, id, doc_type=doc_type, params=params):
+            raise ConflictError(
+                409,
+                "action_request_validation_exception",
+                "Validation Failed: 1: no documents to get;",
+            )
+
+        if index not in self.__documents_dict:
+            self.__documents_dict[index] = []
+
+        if id is None:
+            id = get_random_id()
+
+        self.__documents_dict[index].append(
+            {
+                "_type": doc_type,
+                "_id": id,
+                "_source": body,
+                "_index": index,
+                "_version": 1,
+            }
+        )
+
+        return {
+            "_type": doc_type,
+            "_id": id,
+            "created": True,
+            "_version": 1,
+            "_index": index,
+            "result": "created",
+        }
+
     def index(self, index, body, doc_type="_doc", id=None, params=None, headers=None):
         if index not in self.__documents_dict:
             self.__documents_dict[index] = []
 
         version = 1
 
         result = "created"
```

### Comparing `openmock-2.2.0/openmock/normalize_hosts.py` & `openmock-2.3.0/openmock/normalize_hosts.py`

 * *Files identical despite different names*

### Comparing `openmock-2.2.0/openmock/utilities/__init__.py` & `openmock-2.3.0/openmock/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `openmock-2.2.0/pyproject.toml` & `openmock-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openmock"
-version = "2.2.0"
+version = "2.3.0"
 description = "Python OpenSearch Mock for test purposes"
 authors = ["Marcos Cardoso",
     "Mathew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["opensearch", "mocking", "testing"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/matthewdeanmartin/openmock"
@@ -33,15 +33,15 @@
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/matthewdeanmartin/openmock/issues"
 "Change Log" = "https://github.com/matthewdeanmartin/openmock/blob/main/CHANGES.md"
 
 [tool.poetry.dependencies]
-python = ">=3.6"
+python = ">=3.9"
 opensearch-py = "*"
 python-dateutil = "*"
 
 # Old python had support up to 1.0.0
 # python-ranges  = "1.0.0" # nope!
 python-ranges  = "0.2.1"
```

### Comparing `openmock-2.2.0/README.md` & `openmock-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `openmock-2.2.0/setup.py` & `openmock-2.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,233 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: openmock
+Version: 2.3.0
+Summary: Python OpenSearch Mock for test purposes
+Home-page: https://github.com/matthewdeanmartin/openmock
+License: MIT
+Keywords: opensearch,mocking,testing
+Author: Marcos Cardoso
+Requires-Python: >=3.9
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: opensearch-py
+Requires-Dist: python-dateutil
+Requires-Dist: python-ranges (==0.2.1)
+Project-URL: Bug Tracker, https://github.com/matthewdeanmartin/openmock/issues
+Project-URL: Change Log, https://github.com/matthewdeanmartin/openmock/blob/main/CHANGES.md
+Project-URL: Documentation, https://github.com/matthewdeanmartin/openmock
+Project-URL: Repository, https://github.com/matthewdeanmartin/openmock
+Description-Content-Type: text/markdown
+
+# Openmock
+
+Mock/fake of opensearch library, allows you to mock opensearch-py
+
+Fork of Python Elasticsearch(TM) Mock. Sometimes the developers who work with elasticsearch (TM),
+don't really have any input in choice of host and need to get work done.
+
+![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/openmock) [![Downloads](https://pepy.tech/badge/openmock/month)](https://pepy.tech/project/openmock/month)
+
+## Installation
+
+```shell
+pip install openmock
+```
+
+## Usage
+
+To use Openmock, decorate your test method with **@openmock** decorator:
+
+```python
+from unittest import TestCase
+
+from openmock import openmock
+
+
+class TestClass(TestCase):
+
+    @openmock
+    def test_should_return_something_from_opensearch(self):
+        self.assertIsNotNone(some_function_that_uses_opensearch())
+```
+
+### Custom Behaviours
+
+You can also force the behaviour of the OpenSearch instance by importing the `openmock.behaviour` module:
+
+```python
+from unittest import TestCase
+
+from openmock import behaviour
+
+
+class TestClass(TestCase):
+
+    ...
+
+    def test_should_return_internal_server_error_when_simulate_server_error_is_true(self):
+        behaviour.server_failure.enable()
+        ...
+        behaviour.server_failure.disable()
+```
+
+You can also disable all behaviours by calling `behaviour.disable_all()` (Consider put this in your `def tearDown(self)` method)
+
+#### Available Behaviours
+
+* `server_failure`: Will make all calls to OpenSearch returns the following error message:
+    ```python
+    {
+        'status_code': 500,
+        'error': 'Internal Server Error'
+    }
+    ```
+
+## Code example
+
+Let's say you have a prod code snippet like this one:
+
+```python
+import opensearchpy
+
+class FooService:
+
+    def __init__(self):
+        self.es = opensearchpy.OpenSearch(hosts=[{'host': 'localhost', 'port': 9200}])
+
+    def create(self, index, body):
+        es_object = self.es.index(index, body)
+        return es_object.get('_id')
+
+    def read(self, index, id):
+        es_object = self.es.get(index, id)
+        return es_object.get('_source')
+
+```
+
+Then you should be able to test this class by mocking OpenSearch using the following test class:
+
+```python
+from unittest import TestCase
+from openmock import openmock
+from foo.bar import FooService
+
+class FooServiceTest(TestCase):
+
+    @openmock
+    def should_create_and_read_object(self):
+        # Variables used to test
+        index = 'test-index'
+        expected_document = {
+            'foo': 'bar'
+        }
+
+        # Instantiate service
+        service = FooService()
+
+        # Index document on OpenSearch
+        id = service.create(index, expected_document)
+        self.assertIsNotNone(id)
+
+        # Retrive document from OpenSearch
+        document = service.read(index, id)
+        self.assertEquals(expected_document, document)
+
+```
+
+## Notes:
+
+- The mocked **search** method returns **all available documents** indexed on the index with the requested document type.
+- The mocked **suggest** method returns the exactly suggestions dictionary passed as body serialized in OpenSearch.suggest response. **Attention:** If the term is an *int*, the suggestion will be ```python term + 1```. If not, the suggestion will be formatted as ```python {0}_suggestion.format(term) ```.
+Example:
+	- **Suggestion Body**:
+	```python
+    suggestion_body = {
+        'suggestion-string': {
+            'text': 'test_text',
+            'term': {
+                'field': 'string'
+            }
+        },
+        'suggestion-id': {
+            'text': 1234567,
+            'term': {
+                'field': 'id'
+            }
+        }
+    }
+    ```
+    - **Suggestion Response**:
+    ```python
+    {
+        'suggestion-string': [
+            {
+                'text': 'test_text',
+                'length': 1,
+                'options': [
+                    {
+                        'text': 'test_text_suggestion',
+                        'freq': 1,
+                        'score': 1.0
+                    }
+                ],
+                'offset': 0
+            }
+        ],
+        'suggestion-id': [
+            {
+                'text': 1234567,
+                'length': 1,
+                'options': [
+                    {
+                        'text': 1234568,
+                        'freq': 1,
+                        'score': 1.0
+                    }
+                ],
+                'offset': 0
+            }
+        ],
+    }
+    ```
+
+## Testing
+
+Preferred for testing one version of python.
+```bash
+pytest test
+```
+
+Won't catch pytest tests.
+```bash
+python -m unittest
+```
+
+We are trying to support a full matrix of openmock versions and python versions 3.6+. This is slow.
+```bash
+tox
+```
+
+## Changelog
+
+#### 2.1.0:
+- Update function (Thanks!)
+- tox runs against full matrix
+- Range queries (Thanks!)
 
-packages = \
-['openmock', 'openmock.behaviour', 'openmock.utilities']
+#### 2.0.0:
+- Fork from elasticmock
 
-package_data = \
-{'': ['*']}
+## License
+MIT with normalize_host.py being Apache 2 from Elasticsearch.
 
-install_requires = \
-['opensearch-py', 'python-dateutil', 'python-ranges==0.2.1']
-
-setup_kwargs = {
-    'name': 'openmock',
-    'version': '2.2.0',
-    'description': 'Python OpenSearch Mock for test purposes',
-    'long_description': "# Openmock\n\nMock/fake of opensearch library, allows you to mock opensearch-py\n\nFork of Python Elasticsearch(TM) Mock. Sometimes the developers who work with elasticsearch (TM),\ndon't really have any input in choice of host and need to get work done.\n\n![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/openmock) [![Downloads](https://pepy.tech/badge/openmock/month)](https://pepy.tech/project/openmock/month)\n\n## Installation\n\n```shell\npip install openmock\n```\n\n## Usage\n\nTo use Openmock, decorate your test method with **@openmock** decorator:\n\n```python\nfrom unittest import TestCase\n\nfrom openmock import openmock\n\n\nclass TestClass(TestCase):\n\n    @openmock\n    def test_should_return_something_from_opensearch(self):\n        self.assertIsNotNone(some_function_that_uses_opensearch())\n```\n\n### Custom Behaviours\n\nYou can also force the behaviour of the OpenSearch instance by importing the `openmock.behaviour` module:\n\n```python\nfrom unittest import TestCase\n\nfrom openmock import behaviour\n\n\nclass TestClass(TestCase):\n\n    ...\n\n    def test_should_return_internal_server_error_when_simulate_server_error_is_true(self):\n        behaviour.server_failure.enable()\n        ...\n        behaviour.server_failure.disable()\n```\n\nYou can also disable all behaviours by calling `behaviour.disable_all()` (Consider put this in your `def tearDown(self)` method)\n\n#### Available Behaviours\n\n* `server_failure`: Will make all calls to OpenSearch returns the following error message:\n    ```python\n    {\n        'status_code': 500,\n        'error': 'Internal Server Error'\n    }\n    ```\n\n## Code example\n\nLet's say you have a prod code snippet like this one:\n\n```python\nimport opensearchpy\n\nclass FooService:\n\n    def __init__(self):\n        self.es = opensearchpy.OpenSearch(hosts=[{'host': 'localhost', 'port': 9200}])\n\n    def create(self, index, body):\n        es_object = self.es.index(index, body)\n        return es_object.get('_id')\n\n    def read(self, index, id):\n        es_object = self.es.get(index, id)\n        return es_object.get('_source')\n\n```\n\nThen you should be able to test this class by mocking OpenSearch using the following test class:\n\n```python\nfrom unittest import TestCase\nfrom openmock import openmock\nfrom foo.bar import FooService\n\nclass FooServiceTest(TestCase):\n\n    @openmock\n    def should_create_and_read_object(self):\n        # Variables used to test\n        index = 'test-index'\n        expected_document = {\n            'foo': 'bar'\n        }\n\n        # Instantiate service\n        service = FooService()\n\n        # Index document on OpenSearch\n        id = service.create(index, expected_document)\n        self.assertIsNotNone(id)\n\n        # Retrive document from OpenSearch\n        document = service.read(index, id)\n        self.assertEquals(expected_document, document)\n\n```\n\n## Notes:\n\n- The mocked **search** method returns **all available documents** indexed on the index with the requested document type.\n- The mocked **suggest** method returns the exactly suggestions dictionary passed as body serialized in OpenSearch.suggest response. **Attention:** If the term is an *int*, the suggestion will be ```python term + 1```. If not, the suggestion will be formatted as ```python {0}_suggestion.format(term) ```.\nExample:\n\t- **Suggestion Body**:\n\t```python\n    suggestion_body = {\n        'suggestion-string': {\n            'text': 'test_text',\n            'term': {\n                'field': 'string'\n            }\n        },\n        'suggestion-id': {\n            'text': 1234567,\n            'term': {\n                'field': 'id'\n            }\n        }\n    }\n    ```\n    - **Suggestion Response**:\n    ```python\n    {\n        'suggestion-string': [\n            {\n                'text': 'test_text',\n                'length': 1,\n                'options': [\n                    {\n                        'text': 'test_text_suggestion',\n                        'freq': 1,\n                        'score': 1.0\n                    }\n                ],\n                'offset': 0\n            }\n        ],\n        'suggestion-id': [\n            {\n                'text': 1234567,\n                'length': 1,\n                'options': [\n                    {\n                        'text': 1234568,\n                        'freq': 1,\n                        'score': 1.0\n                    }\n                ],\n                'offset': 0\n            }\n        ],\n    }\n    ```\n\n## Testing\n\nPreferred for testing one version of python.\n```bash\npytest test\n```\n\nWon't catch pytest tests.\n```bash\npython -m unittest\n```\n\nWe are trying to support a full matrix of openmock versions and python versions 3.6+. This is slow.\n```bash\ntox\n```\n\n## Changelog\n\n#### 2.1.0:\n- Update function (Thanks!)\n- tox runs against full matrix\n- Range queries (Thanks!)\n\n#### 2.0.0:\n- Fork from elasticmock\n\n## License\nMIT with normalize_host.py being Apache 2 from Elasticsearch.\n",
-    'author': 'Marcos Cardoso',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/matthewdeanmartin/openmock',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6',
-}
-
-
-setup(**setup_kwargs)
```

