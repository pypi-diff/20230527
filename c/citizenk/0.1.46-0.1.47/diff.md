# Comparing `tmp/citizenk-0.1.46.tar.gz` & `tmp/citizenk-0.1.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.46.tar", max compression
+gzip compressed data, was "citizenk-0.1.47.tar", max compression
```

## Comparing `citizenk-0.1.46.tar` & `citizenk-0.1.47.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      382 2023-05-01 17:44:32.309329 citizenk-0.1.46/citizenk/__init__.py
--rw-r--r--   0        0        0     8805 2023-05-06 18:47:13.206357 citizenk-0.1.46/citizenk/agent.py
--rw-r--r--   0        0        0    20655 2023-05-06 18:23:30.532087 citizenk-0.1.46/citizenk/citizenk.py
--rw-r--r--   0        0        0    20928 2023-04-30 10:29:36.713916 citizenk-0.1.46/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.46/citizenk/murmur2.py
--rw-r--r--   0        0        0     5453 2023-05-06 18:31:26.831757 citizenk-0.1.46/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.46/citizenk/utils.py
--rw-r--r--   0        0        0     1521 2023-05-06 18:47:20.808397 citizenk-0.1.46/pyproject.toml
--rw-r--r--   0        0        0      863 2023-05-06 18:47:38.270075 citizenk-0.1.46/setup.py
--rw-r--r--   0        0        0     1076 2023-05-06 18:47:38.270341 citizenk-0.1.46/PKG-INFO
+-rw-r--r--   0        0        0    18767 2023-05-27 09:09:22.290086 citizenk-0.1.47/README.md
+-rw-r--r--   0        0        0      382 2023-05-25 17:44:44.985810 citizenk-0.1.47/citizenk/__init__.py
+-rw-r--r--   0        0        0     8805 2023-05-25 17:44:44.985906 citizenk-0.1.47/citizenk/agent.py
+-rw-r--r--   0        0        0    20655 2023-05-25 17:44:44.986069 citizenk-0.1.47/citizenk/citizenk.py
+-rw-r--r--   0        0        0    20928 2023-05-25 17:44:44.986229 citizenk-0.1.47/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-05-25 17:44:44.986302 citizenk-0.1.47/citizenk/murmur2.py
+-rw-r--r--   0        0        0     5448 2023-05-25 17:44:44.986393 citizenk-0.1.47/citizenk/topic.py
+-rw-r--r--   0        0        0      413 2023-05-25 17:44:44.986451 citizenk-0.1.47/citizenk/utils.py
+-rw-r--r--   0        0        0     1542 2023-05-27 09:08:35.537133 citizenk-0.1.47/pyproject.toml
+-rw-r--r--   0        0        0    20075 2023-05-27 09:09:22.827184 citizenk-0.1.47/setup.py
+-rw-r--r--   0        0        0    19885 2023-05-27 09:09:22.828151 citizenk-0.1.47/PKG-INFO
```

### Comparing `citizenk-0.1.46/citizenk/agent.py` & `citizenk-0.1.47/citizenk/agent.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.46/citizenk/citizenk.py` & `citizenk-0.1.47/citizenk/citizenk.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.46/citizenk/kafka_adapter.py` & `citizenk-0.1.47/citizenk/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.46/citizenk/murmur2.py` & `citizenk-0.1.47/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.46/citizenk/topic.py` & `citizenk-0.1.47/citizenk/topic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import logging
 from enum import Enum
-from typing import TYPE_CHECKING, Any, Callable, Dict, List
+from typing import TYPE_CHECKING, Any, Callable
 
 from confluent_kafka.schema_registry import Schema, SchemaRegistryClient
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel, ValidationError
 
 from .utils import CitizenKError, annotate_function
 
@@ -51,22 +51,22 @@
         self.replica_count = None
         if self.app.auto_generate_apis:
             self._generate_apis()
 
         # Register topic schema
         self.manage_schema()
 
-    def info(self, lags: Dict[str,int]={}, assignments: Dict[str,List[int]]={}):
+    def info(self, lags: dict[str, int] = {}, assignments: dict[str, list[int]] = {}):
         topic_info = {
             "name": self.name,
             "dir": self.topic_dir.name,
             "value": self.value_type.__name__,
             "subject": self.subject_name,
             "partitions": self.partition_count,
-            "replicas": self.replica_count
+            "replicas": self.replica_count,
         }
         if self.name in lags:
             topic_info["lag"] = lags[self.name]
         if self.name in assignments:
             topic_info["assignments"] = assignments[self.name]
         return topic_info
```

### Comparing `citizenk-0.1.46/pyproject.toml` & `citizenk-0.1.47/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.46"
+version = "0.1.47"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi"]
+readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Development Status :: 4 - Beta",
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
```

