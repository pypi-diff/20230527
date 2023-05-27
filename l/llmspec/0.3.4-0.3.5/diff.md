# Comparing `tmp/llmspec-0.3.4.tar.gz` & `tmp/llmspec-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmspec-0.3.4.tar", last modified: Thu May 25 09:33:28 2023, max compression
+gzip compressed data, was "llmspec-0.3.5.tar", last modified: Sat May 27 03:52:30 2023, max compression
```

## Comparing `llmspec-0.3.4.tar` & `llmspec-0.3.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11098 2023-05-25 09:33:16.788003 llmspec-0.3.4/LICENSE
--rw-r--r--   0        0        0       33 2023-05-25 09:33:16.788003 llmspec-0.3.4/README.md
--rw-r--r--   0        0        0      649 2023-05-25 09:33:16.788003 llmspec-0.3.4/llmspec/__init__.py
--rw-r--r--   0        0        0    10702 2023-05-25 09:33:16.788003 llmspec-0.3.4/llmspec/llmspec.py
--rw-r--r--   0        0        0      215 2023-05-25 09:33:16.788003 llmspec-0.3.4/llmspec/mixins.py
--rw-r--r--   0        0        0       54 2023-05-25 09:33:16.788003 llmspec-0.3.4/llmspec/types.py
--rw-r--r--   0        0        0     1097 2023-05-25 09:33:28.556393 llmspec-0.3.4/pyproject.toml
--rw-r--r--   0        0        0       34 2023-05-25 09:33:16.788003 llmspec-0.3.4/tests/dummy_test.py
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 llmspec-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    11098 2023-05-27 03:52:21.586964 llmspec-0.3.5/LICENSE
+-rw-r--r--   0        0        0       33 2023-05-27 03:52:21.586964 llmspec-0.3.5/README.md
+-rw-r--r--   0        0        0      687 2023-05-27 03:52:21.586964 llmspec-0.3.5/llmspec/__init__.py
+-rw-r--r--   0        0        0    12393 2023-05-27 03:52:21.586964 llmspec-0.3.5/llmspec/llmspec.py
+-rw-r--r--   0        0        0      215 2023-05-27 03:52:21.586964 llmspec-0.3.5/llmspec/mixins.py
+-rw-r--r--   0        0        0       54 2023-05-27 03:52:21.586964 llmspec-0.3.5/llmspec/types.py
+-rw-r--r--   0        0        0     1130 2023-05-27 03:52:30.735068 llmspec-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-27 03:52:21.590964 llmspec-0.3.5/tests/dummy_test.py
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 llmspec-0.3.5/PKG-INFO
```

### Comparing `llmspec-0.3.4/LICENSE` & `llmspec-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llmspec-0.3.4/llmspec/__init__.py` & `llmspec-0.3.5/llmspec/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from llmspec.llmspec import (
     ChatChoice,
     ChatCompletionRequest,
     ChatMessage,
+    ChatResponse,
     CompletionChoice,
     CompletionResponse,
     EmbeddingData,
     EmbeddingRequest,
     EmbeddingResponse,
     ErrorResponse,
     LanguageModels,
@@ -15,14 +16,15 @@
     TokenUsage,
 )
 
 __all__ = [
     "LanguageModels",
     "LLMSpec",
     "ChatMessage",
+    "ChatResponse",
     "ChatCompletionRequest",
     "ChatChoice",
     "CompletionResponse",
     "CompletionChoice",
     "PromptCompletionRequest",
     "EmbeddingRequest",
     "EmbeddingResponse",
```

### Comparing `llmspec-0.3.4/pyproject.toml` & `llmspec-0.3.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "msgspec>=0.15.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "0.3.4"
+version = "0.3.5"
 
 [project.license]
 text = "Apache-2.0"
 
 [build-system]
 requires = [
     "pdm-backend",
@@ -62,9 +62,12 @@
     "B",
     "I",
     "SIM",
     "TID",
     "PL",
 ]
 
+[tool.ruff.pylint]
+max-args = 7
+
 [tool.black]
 line-length = 88
```

