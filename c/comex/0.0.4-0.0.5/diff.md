# Comparing `tmp/comex-0.0.4.tar.gz` & `tmp/comex-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comex-0.0.4.tar", last modified: Tue May 23 15:38:00 2023, max compression
+gzip compressed data, was "comex-0.0.5.tar", last modified: Sat May 27 08:05:31 2023, max compression
```

## Comparing `comex-0.0.4.tar` & `comex-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-23 15:38:00.290000 comex-0.0.4/
--rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-09 06:59:54.000000 comex-0.0.4/LICENSE
--rwxrwxrwx   0 noble      (501) staff       (20)     7952 2023-05-23 15:38:00.290000 comex-0.0.4/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)     7335 2023-05-20 03:38:54.000000 comex-0.0.4/README.md
--rwxrwxrwx   0 noble      (501) staff       (20)     1021 2023-05-23 15:38:00.300000 comex-0.0.4/setup.cfg
--rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-05-09 06:59:54.000000 comex-0.0.4/setup.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-23 15:38:00.290000 comex-0.0.4/src/
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-23 15:38:00.290000 comex-0.0.4/src/comex.egg-info/
--rwxrwxrwx   0 noble      (501) staff       (20)     7952 2023-05-23 15:38:00.000000 comex-0.0.4/src/comex.egg-info/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)      236 2023-05-23 15:38:00.000000 comex-0.0.4/src/comex.egg-info/SOURCES.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-23 15:38:00.000000 comex-0.0.4/src/comex.egg-info/dependency_links.txt
--rwxrwxrwx   0 noble      (501) staff       (20)       40 2023-05-23 15:38:00.000000 comex-0.0.4/src/comex.egg-info/entry_points.txt
--rwxrwxrwx   0 noble      (501) staff       (20)      137 2023-05-23 15:38:00.000000 comex-0.0.4/src/comex.egg-info/requires.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-23 15:38:00.000000 comex-0.0.4/src/comex.egg-info/top_level.txt
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:05:31.020000 comex-0.0.5/
+-rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-09 06:59:54.000000 comex-0.0.5/LICENSE
+-rwxrwxrwx   0 noble      (501) staff       (20)     8106 2023-05-27 08:05:31.020000 comex-0.0.5/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)     7489 2023-05-27 06:29:25.000000 comex-0.0.5/README.md
+-rwxrwxrwx   0 noble      (501) staff       (20)     1021 2023-05-27 08:05:31.020000 comex-0.0.5/setup.cfg
+-rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-05-09 06:59:54.000000 comex-0.0.5/setup.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:05:31.020000 comex-0.0.5/src/
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:05:31.020000 comex-0.0.5/src/comex.egg-info/
+-rwxrwxrwx   0 noble      (501) staff       (20)     8106 2023-05-27 08:05:31.000000 comex-0.0.5/src/comex.egg-info/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)      236 2023-05-27 08:05:31.000000 comex-0.0.5/src/comex.egg-info/SOURCES.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-27 08:05:31.000000 comex-0.0.5/src/comex.egg-info/dependency_links.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)       40 2023-05-27 08:05:31.000000 comex-0.0.5/src/comex.egg-info/entry_points.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)      137 2023-05-27 08:05:31.000000 comex-0.0.5/src/comex.egg-info/requires.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-27 08:05:31.000000 comex-0.0.5/src/comex.egg-info/top_level.txt
```

### Comparing `comex-0.0.4/LICENSE` & `comex-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `comex-0.0.4/PKG-INFO` & `comex-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comex
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generate combined multi-code view graphs
 Home-page: https://github.com/IBM/tree-sitter-codeviews
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -13,15 +13,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Tree Sitter Multi Codeview Generator
 
-Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence model neural networks, graph neural networks, etc). It is also designed to be easily extended to various source code languages. [tree-sitter](https://tree-sitter.github.io/tree-sitter/) is used for parsing which is highly efficient and has support for over 40+ languages. Currently, this repository supports codeviews for Java in over 40 possible combinations of codeviews. It has been structured such that support for other languages can be easily added. If you wish to add support for more languages, please refer to the [contributing](CONTRIBUTING.md) guide.
+Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence model neural networks, graph neural networks, etc). It is also designed to be easily extended to various source code languages. [tree-sitter](https://tree-sitter.github.io/tree-sitter/) is used for parsing which is highly efficient and has support for over 40+ languages. Currently, this repository supports codeviews for Java in over 40 possible combinations of codeviews. It has been structured such that support for other languages can be easily added. If you wish to add support for more languages, please refer to the [contributing](https://github.com/IBM/tree-sitter-codeviews/blob/main/CONTRIBUTING.md) guide.
 
 ## Comex
 `comex` is a rebuild of Tree Sitter Multi Codeview Generator for easier invocation as a Python package. 
 This rebuild also includes a cli interface for easier usage.
 It isolates the logic pertaining to the generation and combination of codeviews to better differentiate tasks involved in the `IBM OSCP Project`.
 
 ### Installation
@@ -96,17 +96,17 @@
 Combined simple AST+CFG+DFG for a simple Java program that finds the maximum among 2 numbers:
 
 <img src="https://github.com/IBM/tree-sitter-codeviews/raw/main/sample.png" >
 
 
 ### Code Organization
 The code is structured in the following way:
-1. For each code-view, first the source code is parsed using the tree-sitter parser and then the various code-views are generated. In the [tree_parser](src/comex/tree_parser) directory, the Parser and ParserDriver is implemented with various funcitonalities commonly required by all code-views. Language-specific features are further developed in the language-specific parsers also placed in this directory.
-2. The [codeviews](src/comex/codeviews) directory contains the core logic for the various codeviews. Each codeview has a driver class and a codeview class, which is further inherited and extended by language in case of code-views that require language-specific implementation.
-3. The [cli.py](src/comex/cli.py) file is the CLI implementation. The drivers can also be directly imported and used like a python package. It is responsible for parsing the source code and generating the codeviews.
+1. For each code-view, first the source code is parsed using the tree-sitter parser and then the various code-views are generated. In the [tree_parser](https://github.com/IBM/tree-sitter-codeviews/tree/main/src/comex/tree_parser) directory, the Parser and ParserDriver is implemented with various funcitonalities commonly required by all code-views. Language-specific features are further developed in the language-specific parsers also placed in this directory.
+2. The [codeviews](https://github.com/IBM/tree-sitter-codeviews/tree/main/src/comex/codeviews) directory contains the core logic for the various codeviews. Each codeview has a driver class and a codeview class, which is further inherited and extended by language in case of code-views that require language-specific implementation.
+3. The [cli.py](https://github.com/IBM/tree-sitter-codeviews/tree/main/src/comex/cli.py) file is the CLI implementation. The drivers can also be directly imported and used like a python package. It is responsible for parsing the source code and generating the codeviews.
 
 ### Testing
 
 The repo is setup to automatically perform CI tests on making pulls to main and development branches.
 To test locally:
 
 Run specific test 
@@ -157,9 +157,8 @@
 
 This tool is based on the ongoing joint research effort between IBM and [Risha Lab](https://rishalab.in/) at [IIT Tirupati](https://www.iittp.ac.in/) to explore the effects of different code representations on code based tasks involving: 
  - [Srikanth Tamilselvam](https://www.linkedin.com/in/srikanth-tamilselvam-913a2ab/)
  - [Sridhar Chimalakonda](https://www.linkedin.com/in/sridharch/)
  - [Alex Mathai](https://www.linkedin.com/in/alex-mathai-403117131/)
  - [Debeshee Das](https://www.linkedin.com/in/debeshee-das/) 
  - [Noble Saji Mathews](https://www.linkedin.com/in/noble-saji-mathews/) 
- - [Kranthi Sedamaki](https://www.linkedin.com/in/kranthisedamaki/) 
- - [Atul Kumar](https://www.linkedin.com/in/atul-kumar-0ba442/) 
+ - [Kranthi Sedamaki](https://www.linkedin.com/in/kranthisedamaki/)
```

### Comparing `comex-0.0.4/README.md` & `comex-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Tree Sitter Multi Codeview Generator
 
-Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence model neural networks, graph neural networks, etc). It is also designed to be easily extended to various source code languages. [tree-sitter](https://tree-sitter.github.io/tree-sitter/) is used for parsing which is highly efficient and has support for over 40+ languages. Currently, this repository supports codeviews for Java in over 40 possible combinations of codeviews. It has been structured such that support for other languages can be easily added. If you wish to add support for more languages, please refer to the [contributing](CONTRIBUTING.md) guide.
+Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence model neural networks, graph neural networks, etc). It is also designed to be easily extended to various source code languages. [tree-sitter](https://tree-sitter.github.io/tree-sitter/) is used for parsing which is highly efficient and has support for over 40+ languages. Currently, this repository supports codeviews for Java in over 40 possible combinations of codeviews. It has been structured such that support for other languages can be easily added. If you wish to add support for more languages, please refer to the [contributing](https://github.com/IBM/tree-sitter-codeviews/blob/main/CONTRIBUTING.md) guide.
 
 ## Comex
 `comex` is a rebuild of Tree Sitter Multi Codeview Generator for easier invocation as a Python package. 
 This rebuild also includes a cli interface for easier usage.
 It isolates the logic pertaining to the generation and combination of codeviews to better differentiate tasks involved in the `IBM OSCP Project`.
 
 ### Installation
@@ -79,17 +79,17 @@
 Combined simple AST+CFG+DFG for a simple Java program that finds the maximum among 2 numbers:
 
 <img src="https://github.com/IBM/tree-sitter-codeviews/raw/main/sample.png" >
 
 
 ### Code Organization
 The code is structured in the following way:
-1. For each code-view, first the source code is parsed using the tree-sitter parser and then the various code-views are generated. In the [tree_parser](src/comex/tree_parser) directory, the Parser and ParserDriver is implemented with various funcitonalities commonly required by all code-views. Language-specific features are further developed in the language-specific parsers also placed in this directory.
-2. The [codeviews](src/comex/codeviews) directory contains the core logic for the various codeviews. Each codeview has a driver class and a codeview class, which is further inherited and extended by language in case of code-views that require language-specific implementation.
-3. The [cli.py](src/comex/cli.py) file is the CLI implementation. The drivers can also be directly imported and used like a python package. It is responsible for parsing the source code and generating the codeviews.
+1. For each code-view, first the source code is parsed using the tree-sitter parser and then the various code-views are generated. In the [tree_parser](https://github.com/IBM/tree-sitter-codeviews/tree/main/src/comex/tree_parser) directory, the Parser and ParserDriver is implemented with various funcitonalities commonly required by all code-views. Language-specific features are further developed in the language-specific parsers also placed in this directory.
+2. The [codeviews](https://github.com/IBM/tree-sitter-codeviews/tree/main/src/comex/codeviews) directory contains the core logic for the various codeviews. Each codeview has a driver class and a codeview class, which is further inherited and extended by language in case of code-views that require language-specific implementation.
+3. The [cli.py](https://github.com/IBM/tree-sitter-codeviews/tree/main/src/comex/cli.py) file is the CLI implementation. The drivers can also be directly imported and used like a python package. It is responsible for parsing the source code and generating the codeviews.
 
 ### Testing
 
 The repo is setup to automatically perform CI tests on making pulls to main and development branches.
 To test locally:
 
 Run specific test 
@@ -140,9 +140,8 @@
 
 This tool is based on the ongoing joint research effort between IBM and [Risha Lab](https://rishalab.in/) at [IIT Tirupati](https://www.iittp.ac.in/) to explore the effects of different code representations on code based tasks involving: 
  - [Srikanth Tamilselvam](https://www.linkedin.com/in/srikanth-tamilselvam-913a2ab/)
  - [Sridhar Chimalakonda](https://www.linkedin.com/in/sridharch/)
  - [Alex Mathai](https://www.linkedin.com/in/alex-mathai-403117131/)
  - [Debeshee Das](https://www.linkedin.com/in/debeshee-das/) 
  - [Noble Saji Mathews](https://www.linkedin.com/in/noble-saji-mathews/) 
- - [Kranthi Sedamaki](https://www.linkedin.com/in/kranthisedamaki/) 
- - [Atul Kumar](https://www.linkedin.com/in/atul-kumar-0ba442/) 
+ - [Kranthi Sedamaki](https://www.linkedin.com/in/kranthisedamaki/)
```

### Comparing `comex-0.0.4/setup.cfg` & `comex-0.0.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = comex
-version = 0.0.4
+version = 0.0.5
 description = Generate combined multi-code view graphs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/IBM/tree-sitter-codeviews
 license = Apache-2.0
 license_file = LICENSE
 classifiers =
```

### Comparing `comex-0.0.4/src/comex.egg-info/PKG-INFO` & `comex-0.0.5/src/comex.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comex
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generate combined multi-code view graphs
 Home-page: https://github.com/IBM/tree-sitter-codeviews
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -13,15 +13,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Tree Sitter Multi Codeview Generator
 
-Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence model neural networks, graph neural networks, etc). It is also designed to be easily extended to various source code languages. [tree-sitter](https://tree-sitter.github.io/tree-sitter/) is used for parsing which is highly efficient and has support for over 40+ languages. Currently, this repository supports codeviews for Java in over 40 possible combinations of codeviews. It has been structured such that support for other languages can be easily added. If you wish to add support for more languages, please refer to the [contributing](CONTRIBUTING.md) guide.
+Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence model neural networks, graph neural networks, etc). It is also designed to be easily extended to various source code languages. [tree-sitter](https://tree-sitter.github.io/tree-sitter/) is used for parsing which is highly efficient and has support for over 40+ languages. Currently, this repository supports codeviews for Java in over 40 possible combinations of codeviews. It has been structured such that support for other languages can be easily added. If you wish to add support for more languages, please refer to the [contributing](https://github.com/IBM/tree-sitter-codeviews/blob/main/CONTRIBUTING.md) guide.
 
 ## Comex
 `comex` is a rebuild of Tree Sitter Multi Codeview Generator for easier invocation as a Python package. 
 This rebuild also includes a cli interface for easier usage.
 It isolates the logic pertaining to the generation and combination of codeviews to better differentiate tasks involved in the `IBM OSCP Project`.
 
 ### Installation
@@ -96,17 +96,17 @@
 Combined simple AST+CFG+DFG for a simple Java program that finds the maximum among 2 numbers:
 
 <img src="https://github.com/IBM/tree-sitter-codeviews/raw/main/sample.png" >
 
 
 ### Code Organization
 The code is structured in the following way:
-1. For each code-view, first the source code is parsed using the tree-sitter parser and then the various code-views are generated. In the [tree_parser](src/comex/tree_parser) directory, the Parser and ParserDriver is implemented with various funcitonalities commonly required by all code-views. Language-specific features are further developed in the language-specific parsers also placed in this directory.
-2. The [codeviews](src/comex/codeviews) directory contains the core logic for the various codeviews. Each codeview has a driver class and a codeview class, which is further inherited and extended by language in case of code-views that require language-specific implementation.
-3. The [cli.py](src/comex/cli.py) file is the CLI implementation. The drivers can also be directly imported and used like a python package. It is responsible for parsing the source code and generating the codeviews.
+1. For each code-view, first the source code is parsed using the tree-sitter parser and then the various code-views are generated. In the [tree_parser](https://github.com/IBM/tree-sitter-codeviews/tree/main/src/comex/tree_parser) directory, the Parser and ParserDriver is implemented with various funcitonalities commonly required by all code-views. Language-specific features are further developed in the language-specific parsers also placed in this directory.
+2. The [codeviews](https://github.com/IBM/tree-sitter-codeviews/tree/main/src/comex/codeviews) directory contains the core logic for the various codeviews. Each codeview has a driver class and a codeview class, which is further inherited and extended by language in case of code-views that require language-specific implementation.
+3. The [cli.py](https://github.com/IBM/tree-sitter-codeviews/tree/main/src/comex/cli.py) file is the CLI implementation. The drivers can also be directly imported and used like a python package. It is responsible for parsing the source code and generating the codeviews.
 
 ### Testing
 
 The repo is setup to automatically perform CI tests on making pulls to main and development branches.
 To test locally:
 
 Run specific test 
@@ -157,9 +157,8 @@
 
 This tool is based on the ongoing joint research effort between IBM and [Risha Lab](https://rishalab.in/) at [IIT Tirupati](https://www.iittp.ac.in/) to explore the effects of different code representations on code based tasks involving: 
  - [Srikanth Tamilselvam](https://www.linkedin.com/in/srikanth-tamilselvam-913a2ab/)
  - [Sridhar Chimalakonda](https://www.linkedin.com/in/sridharch/)
  - [Alex Mathai](https://www.linkedin.com/in/alex-mathai-403117131/)
  - [Debeshee Das](https://www.linkedin.com/in/debeshee-das/) 
  - [Noble Saji Mathews](https://www.linkedin.com/in/noble-saji-mathews/) 
- - [Kranthi Sedamaki](https://www.linkedin.com/in/kranthisedamaki/) 
- - [Atul Kumar](https://www.linkedin.com/in/atul-kumar-0ba442/) 
+ - [Kranthi Sedamaki](https://www.linkedin.com/in/kranthisedamaki/)
```

