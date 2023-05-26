# Comparing `tmp/langkit-0.0.1b3.tar.gz` & `tmp/langkit-0.0.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langkit-0.0.1b3.tar", max compression
+gzip compressed data, was "langkit-0.0.1b4.tar", max compression
```

## Comparing `langkit-0.0.1b3.tar` & `langkit-0.0.1b4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     2259 2023-05-20 01:38:15.592537 langkit-0.0.1b3/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.1b3/LICENSE
--rw-r--r--   0        0        0      706 2023-05-19 23:22:41.142537 langkit-0.0.1b3/langkit/__init__.py
--rw-r--r--   0        0        0    16284 2023-05-20 01:39:38.002537 langkit-0.0.1b3/langkit/examples/GPT_Intro_to_LangKit.ipynb
--rw-r--r--   0        0        0     1119 2023-05-20 01:19:57.252537 langkit-0.0.1b3/langkit/input_output.py
--rw-r--r--   0        0        0      778 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/pattern_groups.json
--rw-r--r--   0        0        0     2505 2023-05-19 23:24:38.182537 langkit-0.0.1b3/langkit/regexes.py
--rw-r--r--   0        0        0      451 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/sentiment.py
--rw-r--r--   0        0        0      714 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/tests/conftest.py
--rw-r--r--   0        0        0     2201 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/tests/test_input_output.py
--rw-r--r--   0        0        0     2170 2023-05-19 23:26:15.952537 langkit-0.0.1b3/langkit/tests/test_patterns.py
--rw-r--r--   0        0        0     2273 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/tests/test_themes.py
--rw-r--r--   0        0        0     2289 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/textstat.py
--rw-r--r--   0        0        0     8896 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/themes.json
--rw-r--r--   0        0        0      261 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/themes.json.txt
--rw-r--r--   0        0        0     2869 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/themes.py
--rw-r--r--   0        0        0      728 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/toxicity.py
--rw-r--r--   0        0        0      144 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/transformer.py
--rw-r--r--   0        0        0      749 2023-05-23 22:38:43.492537 langkit-0.0.1b3/pyproject.toml
--rw-r--r--   0        0        0     3166 1970-01-01 00:00:00.000000 langkit-0.0.1b3/PKG-INFO
+-rw-r--r--   0        0        0     2259 2023-05-26 20:55:15.988991 langkit-0.0.1b4/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.1b4/LICENSE
+-rw-r--r--   0        0        0      706 2023-05-19 23:22:41.142537 langkit-0.0.1b4/langkit/__init__.py
+-rw-r--r--   0        0        0    16075 2023-05-26 20:49:07.178991 langkit-0.0.1b4/langkit/examples/GPT_Intro_to_LangKit.ipynb
+-rw-r--r--   0        0        0      750 2023-05-26 20:48:57.228991 langkit-0.0.1b4/langkit/injections.py
+-rw-r--r--   0        0        0     1047 2023-05-26 04:00:38.203377 langkit-0.0.1b4/langkit/input_output.py
+-rw-r--r--   0        0        0      778 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/pattern_groups.json
+-rw-r--r--   0        0        0     2962 2023-05-26 20:48:57.228991 langkit-0.0.1b4/langkit/regexes.py
+-rw-r--r--   0        0        0      451 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/sentiment.py
+-rw-r--r--   0        0        0      714 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/tests/conftest.py
+-rw-r--r--   0        0        0     2152 2023-05-26 20:49:07.188991 langkit-0.0.1b4/langkit/tests/test_input_output.py
+-rw-r--r--   0        0        0     2150 2023-05-26 04:00:38.203377 langkit-0.0.1b4/langkit/tests/test_patterns.py
+-rw-r--r--   0        0        0     2273 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/tests/test_themes.py
+-rw-r--r--   0        0        0     3235 2023-05-26 20:48:57.228991 langkit-0.0.1b4/langkit/textstat.py
+-rw-r--r--   0        0        0     8896 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/themes.json
+-rw-r--r--   0        0        0      261 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/themes.json.txt
+-rw-r--r--   0        0        0     2869 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/themes.py
+-rw-r--r--   0        0        0      728 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/toxicity.py
+-rw-r--r--   0        0        0      144 2023-05-19 23:17:27.872537 langkit-0.0.1b4/langkit/transformer.py
+-rw-r--r--   0        0        0      753 2023-05-26 20:54:04.228991 langkit-0.0.1b4/pyproject.toml
+-rw-r--r--   0        0        0     3171 1970-01-01 00:00:00.000000 langkit-0.0.1b4/PKG-INFO
```

### Comparing `langkit-0.0.1b3/DESCRIPTION.md` & `langkit-0.0.1b4/DESCRIPTION.md`

 * *Files 9% similar despite different names*

```diff
@@ -35,14 +35,14 @@
 from whylogs.experimental.core.metrics.udf_metric import generate_udf_schema
 from whylogs.core.schema import DeclarativeSchema
 import whylogs as why
 from langkit.sentiment import *
 from langkit.textstat import *
 
 text_schema = DeclarativeSchema(generate_udf_schema())
-results = why.log({"prompt": "hello!", "response": "world!"}, schema=text_schema)
+results = why.log({"prompt": "Hello,", "response": "World!"}, schema=text_schema)
 
 ```
 
 The code above will produce a set of metrics comprised of the default whylogs metrics for text features and all the metrics defined in the imported modules.
 
 More examples are available [here](https://github.com/whylabs/LanguageToolkit/tree/main/langkit/examples).
```

### Comparing `langkit-0.0.1b3/LICENSE` & `langkit-0.0.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b3/langkit/__init__.py` & `langkit-0.0.1b4/langkit/__init__.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b3/langkit/examples/GPT_Intro_to_LangKit.ipynb` & `langkit-0.0.1b4/langkit/examples/GPT_Intro_to_LangKit.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978174603174603%*

 * *Differences: {"'cells'": "{6: {'source': ['%pip install langkit -q']}, 8: {'execution_count': 12}, 9: "*

 * *            "{'source': {insert: [(2, "*

 * *            '\'print(profile_view.get_column("prompt").get_metric("udf").to_summary_dict())\\n\'), '*

 * *            '(3, '*

 * *            '\'print(profile_view.get_column("similarity_all-MiniLM-L6-v2").to_summary_dict())\\n\')], '*

 * *            "delete: [3, 2]}}, 19: {'execution_count': None, 'outputs': []}}"}*

```diff
@@ -61,28 +61,28 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "%pip install langkit==0.0.1b1"
+                "%pip install langkit -q"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "To test the installation worked run the following \"Hello, World!\" example (note the first time you import these langkit modules it will need to download models):"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import whylogs as why\n",
                 "from whylogs.experimental.core.udf_schema import udf_schema\n",
                 "from langkit.input_output import *\n",
                 "from langkit.sentiment import *\n",
@@ -98,16 +98,16 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This verifies that the installation and initialization of models worked, and now this text_schema can be used to profile you LLM. If you are curious what kinds of metrics are gathered you can see a dictionary of the metrics gathered on this Hello, World! example by running something like this:\n",
                 "```python\n",
-                "    print(profile_view.get_column(\"prompt\").get_metric(\"udf\").to_summary_dict())\n",
-                "    print(profile_view.get_column(\"similarity_all-MiniLM-L6-v2\").to_summary_dict())\n",
+                "print(profile_view.get_column(\"prompt\").get_metric(\"udf\").to_summary_dict())\n",
+                "print(profile_view.get_column(\"similarity_all-MiniLM-L6-v2\").to_summary_dict())\n",
                 "```"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -291,28 +291,17 @@
             "metadata": {},
             "source": [
                 "For demonstration, let's use some more archived response/prompts data from Hugging Face, or you can interact with GPT to see how it works in real time if you already have an OpenAI api key."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "(True, 'log-0QApIE2LzK62kU22')"
-                        ]
-                    },
-                    "execution_count": 18,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "from datasets import load_dataset\n",
                 "\n",
                 "from whylogs.api.writer.whylabs import WhyLabsWriter\n",
                 "import whylogs as why\n",
                 "\n",
                 "\n",
```

### Comparing `langkit-0.0.1b3/langkit/input_output.py` & `langkit-0.0.1b4/langkit/input_output.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,18 +17,17 @@
     if transformer_name is None:
         transformer_name = lang_config.transformer_name
     _transformer_model = load_model(transformer_name)
     _transformer_name = transformer_name
 
 
 init()
-_udf_name = _transformer_name or lang_config.transformer_name
 
 
-@register_dataset_udf(["prompt", "response"], f"similarity_{_udf_name.split('/')[-1]}")
+@register_dataset_udf(["prompt", "response"], "response.relevance_to_prompt")
 def similarity_MiniLM_L6_v2(text):
     x = text["prompt"]
     y = text["response"]
     # below assumes text is Dict[str, str], no pandas support
     embedding_1 = _transformer_model.encode(x, convert_to_tensor=True)
     embedding_2 = _transformer_model.encode(y, convert_to_tensor=True)
     similarity = util.pytorch_cos_sim(embedding_1, embedding_2)
```

### Comparing `langkit-0.0.1b3/langkit/pattern_groups.json` & `langkit-0.0.1b4/langkit/pattern_groups.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b3/langkit/regexes.py` & `langkit-0.0.1b4/langkit/regexes.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,36 @@
 import json
 import re
 from logging import getLogger
-from typing import Optional
 
-from whylogs.core.datatypes import String
 from whylogs.experimental.core.metrics.udf_metric import register_metric_udf
-
 from . import LangKitConfig
+from whylogs.core.datatypes import TypeMapper, DataType, String
+from typing import Any, List, Optional, Type
 
 diagnostic_logger = getLogger(__name__)
 
 lang_config = LangKitConfig()
 
 
+class AllString(TypeMapper):
+    """Map a dtype (Pandas) or a Python type to a data type."""
+
+    def __init__(self, custom_types: Optional[List[Type[DataType]]] = None):
+        """
+
+        Args:
+            custom_types: List of additional DataType classes that you want to extend.
+        """
+        pass
+
+    def __call__(self, dtype_or_type: Any) -> DataType:
+        return String()
+
+
 class PatternLoader:
     def __init__(self):
         self.config: LangKitConfig = LangKitConfig()
         self.regex_groups = self.load_patterns()
 
     def load_patterns(self):
         json_path = self.config.pattern_file_path
@@ -51,21 +65,20 @@
         self.regex_groups = self.load_patterns()
 
     def get_regex_groups(self):
         return self.regex_groups
 
 
 pattern_loader = PatternLoader()
-
 if pattern_loader.get_regex_groups() is not None:
 
-    @register_metric_udf(col_type=String)
+    @register_metric_udf(col_type=String, type_mapper=AllString())
     def has_patterns(text: str) -> Optional[str]:
         regex_groups = pattern_loader.get_regex_groups()
-        patterns_info = ""
+        patterns_info = None
         if regex_groups:
             for group in regex_groups:
                 for expression in group["expressions"]:
                     if expression.search(text):
                         patterns_info = group["name"]
                         return group["name"]
         return patterns_info
```

### Comparing `langkit-0.0.1b3/langkit/tests/conftest.py` & `langkit-0.0.1b4/langkit/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b3/langkit/tests/test_input_output.py` & `langkit-0.0.1b4/langkit/tests/test_input_output.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 import whylogs as why
 from whylogs.core.metrics import MetricConfig
-from whylogs.experimental.core.udf_schema import generate_udf_dataset_schema
+from whylogs.experimental.core.udf_schema import udf_schema
 
 
 @pytest.fixture
 def interactions():
     interactions_list = [
         {"prompt": "P"},
         {"response": "I"},
@@ -32,20 +32,20 @@
 
     return True
 
 
 @pytest.mark.load
 def test_similarity(interactions):
     # default input col is "prompt" and output col is "response".
-    from langkit import input_output as lkio
+    from langkit import input_output as lkio  # noqa
 
-    schema = generate_udf_dataset_schema(default_config=MetricConfig(fi_disabled=True))
+    schema = udf_schema(default_config=MetricConfig(fi_disabled=True))
     for i, interaction in enumerate(interactions):
         result = why.log(interaction, schema=schema)
-        column_name = f"similarity_{lkio._transformer_name.split('/')[-1]}"
+        column_name = "response.relevance_to_prompt"
         if {"prompt", "response"}.issubset(set(interaction.keys())):
             similarity_median = (
                 result.view()
                 .get_column(column_name)
                 .get_metric("distribution")
                 .to_summary_dict()["median"]
             )
```

### Comparing `langkit-0.0.1b3/langkit/tests/test_patterns.py` & `langkit-0.0.1b4/langkit/tests/test_patterns.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,18 +60,17 @@
 
     result = why.log(ptt_df, schema=udf_metric_schema())
     fi_input_list = result.view().to_pandas()[
         "udf/has_patterns:frequent_items/frequent_strings"
     ]["input"]
     if not user_defined_json:
         group_names = {
-            "",
             "credit card number",
             "email address",
             "SSN",
             "phone number",
             "mailing address",
         }
     else:
-        group_names = {"custom_group", ""}
+        group_names = {"custom_group"}
 
     assert set([x.value for x in fi_input_list]) == group_names
```

### Comparing `langkit-0.0.1b3/langkit/tests/test_themes.py` & `langkit-0.0.1b4/langkit/tests/test_themes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b3/langkit/textstat.py` & `langkit-0.0.1b4/langkit/textstat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import textstat
 from whylogs.core.datatypes import String
 from whylogs.experimental.core.metrics.udf_metric import register_metric_udf
 
+# score metrics
+
 
 @register_metric_udf(col_type=String)
 def flesch_kincaid_grade(text: str) -> float:
     return textstat.textstat.flesch_kincaid_grade(text)
 
 
 @register_metric_udf(col_type=String)
@@ -30,19 +32,14 @@
 
 @register_metric_udf(col_type=String)
 def dale_chall_readability_score(text: str) -> float:
     return textstat.textstat.dale_chall_readability_score(text)
 
 
 @register_metric_udf(col_type=String)
-def difficult_words(text: str) -> float:
-    return textstat.textstat.difficult_words(text)
-
-
-@register_metric_udf(col_type=String)
 def linsear_write_formula(text: str) -> float:
     return textstat.textstat.linsear_write_formula(text)
 
 
 @register_metric_udf(col_type=String)
 def gunning_fog(text: str) -> float:
     return textstat.textstat.gunning_fog(text)
@@ -77,7 +74,50 @@
 def gulpease_index(text: str) -> float:
     return textstat.textstat.gulpease_index(text)
 
 
 @register_metric_udf(col_type=String)
 def osman(text: str) -> float:
     return textstat.textstat.osman(text)
+
+
+# count metrics
+
+
+@register_metric_udf(col_type=String)
+def syllable_count(text: str) -> float:
+    return textstat.textstat.syllable_count(text)
+
+
+@register_metric_udf(col_type=String)
+def lexicon_count(text: str) -> float:
+    return textstat.textstat.lexicon_count(text)
+
+
+@register_metric_udf(col_type=String)
+def sentence_count(text: str) -> float:
+    return textstat.textstat.sentence_count(text)
+
+
+@register_metric_udf(col_type=String)
+def character_count(text: str) -> float:
+    return textstat.textstat.char_count(text)
+
+
+@register_metric_udf(col_type=String)
+def letter_count(text: str) -> float:
+    return textstat.textstat.letter_count(text)
+
+
+@register_metric_udf(col_type=String)
+def polysyllable_count(text: str) -> float:
+    return textstat.textstat.polysyllabcount(text)
+
+
+@register_metric_udf(col_type=String)
+def monosyllable_count(text: str) -> float:
+    return textstat.textstat.monosyllabcount(text)
+
+
+@register_metric_udf(col_type=String)
+def difficult_words(text: str) -> float:
+    return textstat.textstat.difficult_words(text)
```

### Comparing `langkit-0.0.1b3/langkit/themes.json` & `langkit-0.0.1b4/langkit/themes.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b3/langkit/themes.py` & `langkit-0.0.1b4/langkit/themes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b3/langkit/toxicity.py` & `langkit-0.0.1b4/langkit/toxicity.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b3/pyproject.toml` & `langkit-0.0.1b4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "langkit"
-version = "0.0.1b3"
+version = "0.0.1b4"
 description = "A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs"
 authors = ["WhyLabs.ai <langkit@whylabs.ai>"]
 license = "Apache-2.0"
 readme = "DESCRIPTION.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
-whylogs = {version = ">=1.1.42.dev3, <=1.1.42.dev4"}
+whylogs = {version = "1.1.43.dev0"}
 textstat = "^0.7.3"
 sentence-transformers = "^2.2.2"
 nltk = "^3.8.1"
 pandas = "*"
 datasets = "*"
 
 # optional dependencies
@@ -23,13 +23,16 @@
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.23.0"
 pytest = "^7.3.1"
 
 
 [tool.poetry.extras]
-io = ["torch"]
+all = [
+    "torch",
+    "openai"
+]
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `langkit-0.0.1b3/PKG-INFO` & `langkit-0.0.1b4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: langkit
-Version: 0.0.1b3
+Version: 0.0.1b4
 Summary: A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: langkit@whylabs.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: io
+Provides-Extra: all
 Requires-Dist: datasets
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
-Requires-Dist: openai
+Requires-Dist: openai ; extra == "all"
 Requires-Dist: pandas
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: textstat (>=0.7.3,<0.8.0)
-Requires-Dist: torch ; extra == "io"
-Requires-Dist: whylogs (>=1.1.42.dev3,<=1.1.42.dev4)
+Requires-Dist: torch ; extra == "all"
+Requires-Dist: whylogs (==1.1.43.dev0)
 Description-Content-Type: text/markdown
 
 # LangKit
 
 **LangKit** is an open-source text metrics toolkit for monitoring language models. It offers an array of methods for extracting relevant signals from the input and/or output text, which are compatible with the open-source data logging library [whylogs](https://whylogs.readthedocs.io/en/latest).
 
 The generated profiles can be visualized and monitored in the [WhyLabs platform](https://whylabs.ai/) or they can be further analyzed by the user on their own accord.
@@ -60,15 +60,15 @@
 from whylogs.experimental.core.metrics.udf_metric import generate_udf_schema
 from whylogs.core.schema import DeclarativeSchema
 import whylogs as why
 from langkit.sentiment import *
 from langkit.textstat import *
 
 text_schema = DeclarativeSchema(generate_udf_schema())
-results = why.log({"prompt": "hello!", "response": "world!"}, schema=text_schema)
+results = why.log({"prompt": "Hello,", "response": "World!"}, schema=text_schema)
 
 ```
 
 The code above will produce a set of metrics comprised of the default whylogs metrics for text features and all the metrics defined in the imported modules.
 
 More examples are available [here](https://github.com/whylabs/LanguageToolkit/tree/main/langkit/examples).
```

