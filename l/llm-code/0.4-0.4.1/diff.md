# Comparing `tmp/llm_code-0.4.tar.gz` & `tmp/llm_code-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_code-0.4.tar", max compression
+gzip compressed data, was "llm_code-0.4.1.tar", max compression
```

## Comparing `llm_code-0.4.tar` & `llm_code-0.4.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-05-19 17:43:32.824715 llm_code-0.4/LICENSE
--rw-r--r--   0        0        0     2933 2023-05-21 18:28:27.298503 llm_code-0.4/README.md
--rw-r--r--   0        0        0       75 2023-05-21 18:28:27.298792 llm_code-0.4/llm_code/__init__.py
--rw-r--r--   0        0        0     1938 2023-05-22 20:59:37.527156 llm_code-0.4/llm_code/db.py
--rw-r--r--   0        0        0     4382 2023-05-22 20:59:37.527939 llm_code-0.4/llm_code/llm_code.py
--rw-r--r--   0        0        0     3293 2023-05-19 22:57:07.356159 llm_code-0.4/llm_code/templates.py
--rw-r--r--   0        0        0      161 2023-05-19 18:26:22.445515 llm_code-0.4/prompts/coding/system.toml
--rw-r--r--   0        0        0      613 2023-05-19 18:23:27.578834 llm_code-0.4/prompts/coding/user/input.toml
--rw-r--r--   0        0        0      396 2023-05-19 18:19:43.905655 llm_code-0.4/prompts/coding/user/simple.toml
--rw-r--r--   0        0        0     1155 2023-05-22 20:59:37.530387 llm_code-0.4/pyproject.toml
--rw-r--r--   0        0        0     3909 1970-01-01 00:00:00.000000 llm_code-0.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-19 17:20:49.716226 llm_code-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4655 2023-05-23 04:05:15.622745 llm_code-0.4.1/README.md
+-rw-r--r--   0        0        0       75 2023-05-21 03:18:50.955110 llm_code-0.4.1/llm_code/__init__.py
+-rw-r--r--   0        0        0     1938 2023-05-23 04:05:15.623074 llm_code-0.4.1/llm_code/db.py
+-rw-r--r--   0        0        0     4405 2023-05-26 23:31:51.216868 llm_code-0.4.1/llm_code/llm_code.py
+-rw-r--r--   0        0        0     3293 2023-05-21 02:14:00.115437 llm_code-0.4.1/llm_code/templates.py
+-rw-r--r--   0        0        0      161 2023-05-21 02:14:00.117237 llm_code-0.4.1/prompts/coding/system.toml
+-rw-r--r--   0        0        0      613 2023-05-21 02:14:00.117511 llm_code-0.4.1/prompts/coding/user/input.toml
+-rw-r--r--   0        0        0      396 2023-05-21 02:14:00.117693 llm_code-0.4.1/prompts/coding/user/simple.toml
+-rw-r--r--   0        0        0     1157 2023-05-26 23:36:43.181569 llm_code-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5633 1970-01-01 00:00:00.000000 llm_code-0.4.1/PKG-INFO
```

### Comparing `llm_code-0.4/LICENSE` & `llm_code-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_code-0.4/llm_code/db.py` & `llm_code-0.4.1/llm_code/db.py`

 * *Files identical despite different names*

### Comparing `llm_code-0.4/llm_code/llm_code.py` & `llm_code-0.4.1/llm_code/llm_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 import click
 import openai
 from pydantic import BaseSettings
 from rich.console import Console
 from rich.syntax import Syntax
 
 from llm_code import __version__, db
-
-from .templates import Message, TemplateLibrary
+from llm_code.templates import Message, TemplateLibrary
 
 
 class Settings(BaseSettings):
     openai_api_key: str = ""
     model: str = "gpt-3.5-turbo"
     temperature: float = 0.8
     max_tokens: int = 1000
@@ -73,21 +72,21 @@
     console = Console()
 
     if version:
         console.print(f"[bold green]llm_code[/] version {__version__}")
         sys.exit(0)
 
     settings = Settings()
+    if not settings.openai_api_key:
+        raise click.UsageError("OPENAI_API_KEY must be set.")
+
     if gpt_4:
         settings.model = "gpt-4"
     init_db(settings.config_dir)
 
-    if not settings.openai_api_key:
-        raise click.UsageError("OPENAI_API_KEY must be set.")
-
     instructions = " ".join(instructions)
     if not instructions:
         raise click.UsageError("Please provide some instructions.")
 
     library = load_templates(settings.config_dir) or load_templates(
         Path(__file__).parent.parent
     )
@@ -128,15 +127,15 @@
             output_tokens=response.usage["completion_tokens"],  # type: ignore
         )
     else:
         message = cached_response
 
     code = message.code()
     if code:
-        console.print(Syntax(code.code, code.lang))
+        console.print(Syntax(code.code, code.lang), soft_wrap=True)
     else:
         console.print(f"No code found in message: \n\n{message.content}")
         sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `llm_code-0.4/llm_code/templates.py` & `llm_code-0.4.1/llm_code/templates.py`

 * *Files identical despite different names*

### Comparing `llm_code-0.4/prompts/coding/user/input.toml` & `llm_code-0.4.1/prompts/coding/user/input.toml`

 * *Files identical despite different names*

### Comparing `llm_code-0.4/pyproject.toml` & `llm_code-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-code"
-version = "0.4"
+version = "0.4.1"
 description = "An OpenAI LLM based CLI coding assistant."
 authors = ["Rushabh Doshi <radoshi+pypi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "llm_code" }]
 homepage = "https://github.com/radoshi/llm-code"
 repository = "https://github.com/radoshi/llm-code"
```

### Comparing `llm_code-0.4/PKG-INFO` & `llm_code-0.4.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: llm-code
-Version: 0.4
-Summary: An OpenAI LLM based CLI coding assistant.
-Home-page: https://github.com/radoshi/llm-code
-License: MIT
-Keywords: openai,llm,cli,coding,assistant
-Author: Rushabh Doshi
-Author-email: radoshi+pypi@gmail.com
-Requires-Python: >=3.11,<4.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Code Generators
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: openai (>=0.27.6,<0.28.0)
-Requires-Dist: pydantic[dotenv] (>=1.10.7,<2.0.0)
-Requires-Dist: rich (>=13.3.5,<14.0.0)
-Requires-Dist: sqlalchemy (>=2.0.15,<3.0.0)
-Requires-Dist: tomli (>=2.0.1,<3.0.0)
-Project-URL: Repository, https://github.com/radoshi/llm-code
-Description-Content-Type: text/markdown
-
 # llm-code
 
 ![PyPi](https://img.shields.io/pypi/v/llm-code?color=green)
 [![Coverage Status](https://coveralls.io/repos/github/radoshi/llm-code/badge.svg?branch=main)](https://coveralls.io/github/radoshi/llm-code?branch=main)
 
 ---
 
@@ -82,21 +56,64 @@
 ```bash
 llm-code --help
 ```
 
 ```
 Usage: llm-code [OPTIONS] [INSTRUCTIONS]...
 
-  Ask for code completion from OpenAI's chat models.
+  Coding assistant using OpenAI's chat models.
+
+  Requires OPENAI_API_KEY as an environment variable. Alternately, you can set
+  it in ~/.llm_code/env.
 
 Options:
   -i, --inputs TEXT  Glob of input files.
+  -nc, --no-cache    Don't use cache.
+  -4, --gpt-4        Use GPT-4.
+  --version          Show version.
   --help             Show this message and exit.
 ```
 
+## Changing OpenAI parameters
+
+Any of the OpenAI parameters can be changed using environment variables. GPT-4 is one exception: you can also set it using `-4` for convenience.
+
+```bash
+export MAX_TOKENS=2000
+export TEMPERATURE=0.5
+export MODEL=gpt-4
+```
+
+or
+
+```bash
+llm-code -4 ...
+```
+
+## Caching
+
+A common usage pattern is to examine the output of a model and either accept it, or continue to play around with the prompts. When "accepting" the output, a common thing is to append it to a file, or copy it to the clipboard (using `pbcopy` on a mac, for example.). To facilitate this workflow of inspection and acceptance, `llm-code` caches the output of the model in a local sqlite database. This allows you to replay the same query without having to hit the OpenAI API.
+
+```bash
+llm-code 'write a function that takes a list of numbers and returns the sum of the numbers in python. Add type hints.'
+```
+
+Following this, assuming you like the output:
+
+```bash
+llm-code 'write a function that takes a list of numbers and returns the sum of the numbers in python. Add type hints.' > sum.py
+```
+
+## Database
+
+Borrowing simonw's excellent idea of logging things to a local sqlite, as demonstrated in [`llm`](https://github.com/simonw/llm), `llm-code` also logs all queries to a local sqlite database. This is useful for a few reasons:
+
+1. It allows you to replay the same query without having to hit the OpenAI API.
+2. It allows you to see what queries you've made in the past with responses, and number of tokens used.
+
 ## Examples
 
 Simple hello world.
 
 ```bash
 llm-code write hello world in rust
 ```
@@ -157,12 +174,11 @@
     assert sum_numbers([1, 2, 3]) == 6
     assert sum_numbers([-1, 0, 1]) == 0
     assert sum_numbers([]) == 0
 ```
 
 ## TODO
 
-- [ ] Add a simple cache to replay the same query.
+- [X] Add a simple cache to replay the same query.
+- [X] Add logging to a local sqllite db.
 - [ ] Add an `--exec` option to execute the generated code.
 - [ ] Add a `--stats` option to output token counts.
-- [ ] Add logging to a local sqllite db.
-
```

