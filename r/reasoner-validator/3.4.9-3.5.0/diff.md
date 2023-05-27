# Comparing `tmp/reasoner_validator-3.4.9.tar.gz` & `tmp/reasoner_validator-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.4.9.tar", max compression
+gzip compressed data, was "reasoner_validator-3.5.0.tar", max compression
```

## Comparing `reasoner_validator-3.4.9.tar` & `reasoner_validator-3.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1153 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/LICENSE
--rw-r--r--   0        0        0    10735 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/README.md
--rw-r--r--   0        0        0      131 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/Makefile
--rw-r--r--   0        0        0     2288 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/conf.py
--rw-r--r--   0        0        0    12701 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/index.rst
--rw-r--r--   0        0        0      795 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/make.bat
--rw-r--r--   0        0        0      136 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    30645 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     1788 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/pyproject.toml
--rw-r--r--   0        0        0    18017 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    41636 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    30438 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0    19593 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4032 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0     5845 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    12518 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0     5115 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      517 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/tests/README.md
--rw-r--r--   0        0        0        0 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/tests/__init__.py
--rw-r--r--   0        0        0    86089 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    27505 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/tests/test_response_validator.py
--rw-r--r--   0        0        0     2722 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/tests/test_semver.py
--rw-r--r--   0        0        0     8795 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/tests/test_validate.py
--rw-r--r--   0        0        0    17440 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/tests/test_validation_report.py
--rw-r--r--   0        0        0    12606 1970-01-01 00:00:00.000000 reasoner_validator-3.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/LICENSE
+-rw-r--r--   0        0        0    12066 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/README.md
+-rw-r--r--   0        0        0      131 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/Makefile
+-rw-r--r--   0        0        0     2288 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/conf.py
+-rw-r--r--   0        0        0    18216 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    36012 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2056 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0    20298 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    59678 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    39221 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0    26512 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4350 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0     6837 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    13781 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0     9165 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0        0 2023-05-27 00:11:15.712252 reasoner_validator-3.5.0/tests/__init__.py
+-rw-r--r--   0        0        0   102228 2023-05-27 00:11:15.712252 reasoner_validator-3.5.0/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    31906 2023-05-27 00:11:15.712252 reasoner_validator-3.5.0/tests/test_response_validator.py
+-rw-r--r--   0        0        0     4546 2023-05-27 00:11:15.712252 reasoner_validator-3.5.0/tests/test_semver.py
+-rw-r--r--   0        0        0    26567 2023-05-27 00:11:15.712252 reasoner_validator-3.5.0/tests/test_validate.py
+-rw-r--r--   0        0        0    19017 2023-05-27 00:11:15.712252 reasoner_validator-3.5.0/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2068 2023-05-27 00:11:15.712252 reasoner_validator-3.5.0/tests/test_workflows.py
+-rw-r--r--   0        0        0    14105 1970-01-01 00:00:00.000000 reasoner_validator-3.5.0/PKG-INFO
```

### Comparing `reasoner_validator-3.4.9/LICENSE` & `reasoner_validator-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.9/README.md` & `reasoner_validator-3.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Reasoner Validator
 
 [![Pyversions](https://img.shields.io/pypi/pyversions/reasoner-validator)](https://pypi.python.org/pypi/reasoner-validator)
-[![pypi](https://github.com/NCATSTranslator/reasoner-validator/workflows/pypi/badge.svg)](https://pypi.org/project/reasoner-validator/)
+[![Publish Python Package](https://github.com/NCATSTranslator/reasoner-validator/actions/workflows/pypi_publish.yml/badge.svg)](https://pypi.org/project/reasoner-validator/)
+[![Sphinx Documentation](https://github.com/NCATSTranslator/reasoner-validator/actions/workflows/doc_pages.yml/badge.svg)](https://github.com/NCATSTranslator/reasoner-validator/actions/workflows/doc_pages.yml)
+[![Run tests](https://github.com/NCATSTranslator/reasoner-validator/actions/workflows/test.yml/badge.svg)](https://github.com/NCATSTranslator/reasoner-validator/actions/workflows/test.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
 
 This package provides software methods to Translator components (e.g. Knowledge Providers and Autonomous Relay Agents) using *any version* of the
 [Translator Reasoner API (TRAPI)](https://github.com/NCATSTranslator/ReasonerAPI/blob/master/README.md) and the [Biolink Model](https://github.com/biolink/biolink-model/blob/master/README.md).
 
 See [the full documentation](https://ncatstranslator.github.io/reasoner-validator/) and [the contributor guidelines](https://github.com/NCATSTranslator/reasoner-validator/blob/master/.github/CONTRIBUTING.md).
 
@@ -13,44 +15,83 @@
 
 ## Python Dependency
 
 The Reasoner Validator now requires Python 3.9 or later (some library dependencies now force this).
 
 ## Installing the Module
 
-The module may be installed directly from pypi.org.
+The module may be installed directly from pypi.org using (Python 3) `pip` or `pip3`, namely:
 
 ```bash
 pip install reasoner-validator
 ```
 
+If you want to install it with the extra dependencies for using it as a web service, you can use:
+
+```bash
+pip install "reasoner-validator[web]"
+```
+
 ## Installing and working with the module locally from source
 
 As of release 3.1.6, this project uses the [poetry dependency management](https://python-poetry.org) tool to orchestrate its installation and dependencies.
 
 After [installing poetry](https://python-poetry.org/docs/#installation) and cloning the project, the poetry installation may be run:
 
 ```bash
 git clone https://github.com/NCATSTranslator/reasoner-validator.git
 cd reasoner-validator
 poetry install
 ```
 
+To develop this package, install with all extras dependencies using:
+
+```bash
+poetry install --all-extras
+```
+
 ## Running Validation against an ARS UUID Result(*)
 
-A local script **`ars_uuid_result_test_runner.py`** is available to run TRAPI Response validation against a UUID indexed query result of the Biomedical Knowledge Translator "Autonomous Relay System" (ARS).
+A local script **`ars_uuid_result_test_runner.py`** is available to run TRAPI Response validation against a 
+UUID indexed query result of the Biomedical Knowledge Translator "Autonomous Relay System" (ARS).
 
 For usage, type:
 
 ```bash
 ./ars_uuid_result_test_runner.py --help
 ```
 
 (*) Thank you Eric Deutsch for the prototype of this script
 
+## Running tests
+
+To run the test locally install with the `dev` dependencies group if not already done:
+
+```bash
+poetry install --extras dev
+```
+
+Run the tests with coverage report:
+
+```bash
+poetry run pytest --cov
+```
+
+Run the tests with detailed coverage report in a HTML page:
+
+```bash
+poetry run pytest --cov --cov-report html
+```
+
+Serve the report on http://localhost:3000:
+
+```bash
+python -m http.server 3000 --directory ./htmlcov
+```
+
 ## Building the Documentation Locally
 
 All paths here are relative to the root project directory.
 
 First install the documentation-specific dependencies.
 
 ```bash
@@ -79,36 +120,42 @@
 
 ### API
 
 The web service has a single POST endpoint `/validate` taking a simple JSON request body, as follows:
 
 ```json
 {
-  "trapi_version": "1.3.0",
-  "biolink_version": "3.2.1",
+  "trapi_version": "1.4.0-beta",
+  "biolink_version": "3.2.6",
   "sources": {
     "ara_source": "infores:aragorn",
     "kp_source": "infores:panther",
     "kp_source_type": "primary"
   },
   "strict_validation": true,
-  "message": {...}
+  "response": {<some full JSON object of a TRAPI query Response...>}
 }
 ```
 
 The request body consists of JSON data structure with two top level tag:
 
 - An **optional** `trapi_version` tag can be given a value of the TRAPI version against which the message will be validated, expressed as a SemVer string (defaults to 'latest' if omitted; partial SemVer strings are resolved to their 'latest' minor and patch releases). 
 - An **optional** `biolink_version` tag can be given a value of the Biolink Model version against which the message knowledge graph semantic contents will be validated, expressed as a SemVer string (defaults to 'latest' Biolink Model Toolkit supported version, if omitted). 
 - An **optional** `sources` with an object dictionary (example shown) specifying the ARA and KP sources involved in the TRAPI call (specified by infores CURIE) and the expected KP provenance source type, i.e. 'primary' implies that the KP is tagged as a 'biolink:primary_knowledge_source'. Optional in that the root "sources" or any of the subsidiary tags may be omitted (default to None)
 - An **optional** `strict_validation` flag (default: None or 'false'). If 'true' then follow strict validation rules, such as treating as 'error' states the use of `category`, `predicate` and `attribute_type_id` that are of type `abstract` or `mixin`  as errors. 
-- A **mandatory** `message` tag should have as its value the complete TRAPI **Message** JSON data structure to be validated (see example below).
+- A **mandatory** `message` tag should have as its value the complete JSON TRAPI **Response** to be validated (See the example below)
 
 ### Running the Web Service Directly
 
+First install the web-specific dependencies.
+
+```bash
+poetry install --extras web
+```
+
 The service may be run directly as a Python module. The web services module may be directly run, as follows. 
 
 ```shell
 python -m api.main
 ```
 
 Note that [poetry automatically uses any existing virtual environment](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment), but you can otherwise also enter the one that is created by poetry by default:
@@ -119,15 +166,15 @@
 exit  # exit the poetry shell
 ```
 
 Go to  http://localhost/docs to see the service documentation and to use the simple UI to input TRAPI messages for validation.
 
 ### Typical Output
 
-As an example of the kind of output to expect, if one posts the following JSON message data to the **/validate** endpoint:
+As an example of the kind of output to expect, if one posts the following TRAPI Response JSON data structure to the **/validate** endpoint:
 
 ```json
 {
   "trapi_version": "1.3.0",
   "biolink_version": "3.2.1",
   "response": {
       "message": {
```

### Comparing `reasoner_validator-3.4.9/docs/Makefile` & `reasoner_validator-3.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.9/docs/conf.py` & `reasoner_validator-3.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.9/docs/index.rst` & `reasoner_validator-3.5.0/docs/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -16,110 +16,179 @@
 As Pypi Package
 ---------------
 
 .. code-block:: bash
 
   pip install reasoner-validator
 
+will install the package from Pypi.org.
+
 From Github
 -----------
 
+Checkout then setup dependencies and the standard virtual environment using poetry, as follows:
+
 .. code-block:: bash
 
     git checkout https://github.com/NCATSTranslator/reasoner-validator.git
     cd reasoner-validator
-    pip install -e .
+    poetry install
+
+You can optionally, `use a tool like pyenv to set your local shell Python version to a 3.9 release <https://python-poetry.org/docs/managing-environments/>`_  prior to the poetry installation.
 
 Basic Programmatic Usage
 ========================
 
 Unlike earlier release of the reasoner-validator package, the current (major release 3.*.*) wraps validation in a general Python class object, 'ValidatorReporter' which is subclassed into various validator types (TRAPI Schema, Biolink, etc.).
 
-Top level programmatic validation of a TRAPI Response uses a TRAPIResponseValidator class wrapper as follows:
+Top level programmatic validation of a TRAPI Response uses a TRAPIResponseValidator class wrapper as follows (sample script):
 
 .. code-block:: python
 
+    #!/usr/bin/env python
+    from typing import Optional, List, Dict
     from reasoner_validator import TRAPIResponseValidator
 
+    SAMPLE_RESPONSE = {
+      "message": {
+        "query_graph": {
+            "nodes": {
+                "type-2 diabetes": {"ids": ["MONDO:0005148"]},
+                "drug": {"categories": ["biolink:Drug"]}
+            },
+            "edges": {
+                "treats": {"subject": "drug", "predicates": ["biolink:treats"], "object": "type-2 diabetes"}
+            }
+        },
+        "knowledge_graph": {
+            "nodes": {
+                "MONDO:0005148": {"name": "type-2 diabetes"},
+                "CHEBI:6801": {"name": "metformin", "categories": ["biolink:Drug"]}
+            },
+            "edges": {
+                "df87ff82": {"subject": "CHEBI:6801", "predicate": "biolink:treats", "object": "MONDO:0005148"}
+            }
+        },
+        "results": [
+            {
+                "node_bindings": {
+                    "type-2 diabetes": [{"id": "MONDO:0005148"}],
+                    "drug": [{"id": "CHEBI:6801"}]
+                },
+                "edge_bindings": {
+                    "treats": [{"id": "df87ff82"}]
+                }
+            }
+        ]
+    }
+
+    }
     validator = TRAPIResponseValidator(
-        trapi_version="1.3.0",
+        trapi_version="1.4.0",
 
         # If omit or set the Biolink Model version parameter to None,
         # then the current Biolink Model Toolkit default release applies
-        biolink_version="3.0.3",
+        biolink_version="3.2.6",
 
         # 'sources' are set to trigger checking of expected edge knowledge source provenance
         sources={
                 "ara_source": "infores:molepro",
                 "kp_source": "infores:hmdb",
                 "kp_source_type": "primary"
         },
-        # Optional flag: if omitted or set to 'None', we let the system decide the
+        # Optional flag: if omitted or set to 'False', we let the system decide the
         # default validation strictness by validation context unless we override it here
-        strict_validation=None
+        strict_validation=False
     )
 
     # Unlike earlier release of the package, validation methods do NOT throw an exception,
     # but rather, return validation outcomes as a dictionary of validation messsages
     # Here, the 'message' parameter here is just the Python equivalent dictionary of the
     # TRAPI.Message JSON schema model component of the TRAPI Response (not the full TRAPI Response...yet)
-    validator.check_compliance_of_trapi_response(message=...)
 
-    # Messages are retrieved from the validator object as follows:
-    messages: Dict[str, List[Dict[str,str]]] = validator.get_messages()
+    # this method validates a complete TRAPI Response JSON result
+    validator.check_compliance_of_trapi_response(response=SAMPLE_RESPONSE)
 
+    # Messages are retrieved from the validator object as follows:
+    messages: Dict[
+                str,  # message type (errors|warnings|information)
+                Dict[
+                    str,  # message 'code' as indexing key
+                    # Dictionary of 'identifier' indexed messages with parameters
+                    # (Maybe None, if code doesn't have any additional parameters)
+                    Optional[
+                        Dict[
+                            str,  # key is the message-unique template 'identifier' value of parameterized messages
+                            Optional[
+                                List[
+                                    # Each reported message adds a dictionary of such parameters
+                                    # to the list here; these are not guaranteed to be unique
+                                    Dict[str, str]
+                                ]
+                            ]
+                        ]
+                    ]
+                ]
+            ] = validator.get_messages()
+
+    # this method dumps a human readable text report of
+    # the validation messages (default) to stdout
+    # See the method signature for options that
+    # allow customization of the text format.
+    validator.dump()
 
 The 'messages' returned are partitioned into 'information', 'warning' and 'error' messages
 in a dictionary looking something like the following (as an example):
 
 .. code-block:: python
 
     messages: Dict[str, List[Dict[str,str]]] = {
         "information": {
-            "info.excluded": [
-                {  # parameters for one distinct message
-                    "edge_id": "(ZFIN:ZDB-GENE-060825-345$biolink:Gene)--[biolink:active_in]->(GO:0042645$biolink:CellularComponent)",
+            "info.excluded": {
+                # the uniquely discriminating 'identifier' here is the edge_id
+                "(ZFIN:ZDB-GENE-060825-345$biolink:Gene)--[biolink:active_in]->(GO:0042645$biolink:CellularComponent)": None
+                # messages with only a contextual identifier may have no additional parameters
                 },
                 {...}  # another message (same code type)
-            ],
-            "info.compliant": []  # parameterless messages don't have distinct instances
+            ,
+            "info.compliant": None  # parameterless messages don't have distinct instances
              # other 'info' code-indexed messages
         },
         "warnings": {
-            "warning.edge.predicate.non_canonical": [
-                {
-                    "context": "Query Graph",
+            "warning.edge.predicate.non_canonical": {
+                # the uniquely discriminating 'identifier' here is the is the predicate term
+                "biolink:participates_in":
+                {   # the secondary context is the 'edge_id'
                     "edge_id": "a--['biolink:participates_in']->b",
-                    "predicate": "biolink:participates_in"
                 },
-                {...}  # another message (same code type)
+                {...}  # another predicate indexed message (same code type)
 
-            ],
-            "warning.trapi.response.status.unknown" [
-                {
-                    "status": "some status message",
-                }
-            ],
+            },
+            "warning.trapi.response.status.unknown" {
+                "500": None  # unexpected http status code returned
+            },
             # other 'warning' code-indexed messages
          },
         "errors": {
-            "error.trapi.request.invalid": [
+            "error.trapi.request.invalid": {
+                # subject node descriptor is the 'identifier'
+                "CHEBI:37565[biolink:SmallMolecule]":
                 {
-                    "context": "raise_subject_entity() test predicate CHEBI:37565[biolink:SmallMolecule]",
+                    "test": "raise_subject_entity"
                     "reason": "has no 'is_a' parent since it is either not an ontology term or does not map onto a parent ontology term."
                 },
                 {...} # another message (same code type)
-            ],
+            },
             # other 'error' code-indexed messages
         }
     }
 
 
 Every message has a 'code' and optional context-specific parameters which correspond to
-named fields in the Python string templates found in the `reasoner_validator package 'codes.yaml' file <https://github.com/NCATSTranslator/reasoner-validator/blob/master/reasoner_validator/codes.yaml>`_ file.
+named fields in the Python string templates found in the `reasoner_validator package 'codes.yaml' file <https://github.com/NCATSTranslator/reasoner-validator/blob/master/reasoner_validator/codes.yaml>`_.
 
 Python API
 ----------
 .. toctree::
    :maxdepth: 2
 
    TRAPI Response Validation <reasoner_validator>
@@ -143,115 +212,170 @@
 ---------------
 
 The web service has a single POST endpoint `/validate` taking a simple JSON request body, as follows:
 
 .. code-block:: json
 
     {
-      "trapi_version": "1.3.0",
-      "biolink_version": "3.0.3",
-      "sources": {
-        "ara_source": "infores:aragorn",
-        "kp_source": "infores:panther",
-        "kp_source_type": "primary"
-      },
-      "strict_validation": true,
-      "message": {"some message"}
+        # If the TRAPI version is omitted or set to None, then the 'latest' TRAPI version is used.
+
+        # Note: for TRAPI releases from 1.4.0 onwards, the Response message will state the assumed 'schema_version'.
+        # This modifies slightly the interpretation of this parameter, as follows:
+        # If the following trapi_version parameter is given, then it overrides the TRAPI Response 'schema_version';
+        # Otherwise, the TRAPI Response 'schema_version' (not 'latest') becomes the default validation version.
+
+        trapi_version="1.4.0",
+
+        # If the Biolink Model version is omitted or set to None, then the current Biolink Model Toolkit is used.
+
+        # Note: for TRAPI releases from 1.4.0 onwards, the Response message will state the assumed 'biolink_version'.
+        # This modifies slightly the interpretation of this parameter, as follows:
+        # If the 'biolink_version' given here is assumed, which overrides the TRAPI Response stated 'biolink_version';
+        # Otherwise, the TRAPI Response stated 'biolink_version' (not BMT) becomes the default validation version.
+
+        biolink_version="3.2.6",
+
+        "sources": {
+            "ara_source": "infores:aragorn",
+            "kp_source": "infores:panther",
+            "kp_source_type": "primary"
+        },
+        "strict_validation": true,
+        "response": {"some TRAPI Response JSON - see below"}
     }
 
 
 The request body consists of JSON data structure with two top level tag:
 
 * An **optional** `trapi_version` tag can be given a value of the TRAPI version against which the message will be validated, expressed as a SemVer string (defaults to 'latest' if omitted; partial SemVer strings are resolved to their 'latest' minor and patch releases).
 * An **optional** `biolink_version` tag can be given a value of the Biolink Model version against which the message knowledge graph semantic contents will be validated, expressed as a SemVer string (defaults to 'latest' Biolink Model Toolkit supported version, if omitted).
 * An **optional** `sources` with an object dictionary (example shown) specifying the ARA and KP sources involved in the TRAPI call (specified by infores CURIE) and the expected KP provenance source type, i.e. 'primary' implies that the KP is tagged as a 'biolink:primary_knowledge_source'. Optional in that the root "sources" or any of the subsidiary tags may be omitted (default to None)
 * An **optional** `strict_validation` flag (default: None or 'false'). If 'true' then follow strict validation rules, such as treating as 'error' states the use of `category`, `predicate` and `attribute_type_id` that are of type `abstract` or `mixin`  as errors.
-* A **mandatory** `message` tag should have as its value the complete TRAPI **Message** JSON data structure to be validated (see example below).
+* A **mandatory** `response` tag should have as its value the complete TRAPI **Response** JSON data structure to be validated (see example below).
 
 Running the Web Service Directly
 --------------------------------
 
-The service may be run directly as a python module. It is suggested that a virtual environment first be created (using virtualenv, conda, within your IDE, or equivalent).  Then, certain Python dependencies need to be installed, as follows:
+The service may be run directly as a Python module after certain dependencies are installed using poetry, as follows:
 
 .. code-block:: bash
 
-    pip install -r requirements-service.txt
-
+    poetry install
 
 The module may afterwards be run, as follows:
 
 .. code-block:: bash
 
     python -m api.main
 
+Run on your local machine, an OpenAPI web service form may now be viewed at http://localhost/docs/
 
 Typical Output
 --------------
 
-As an example of the kind of output to expect, if one posts the following JSON message data to the **/validate** endpoint:
+As an example of the kind of output to expect, if one posts the following TRAPI Response JSON data as input to the **/validate** endpoint:
 
 .. code-block:: json
 
     {
-      "trapi_version": "1.3.0",
-      "biolink_version": "3.0.3",
-      "message": {
-        "query_graph": {
-            "nodes": {
-                "type-2 diabetes": {"ids": ["MONDO:0005148"]},
-                "drug": {"categories": ["biolink:Drug"]}
+        "schema_version": "1.4.0",
+        "biolink_version": "3.2.6",
+        "message": {
+            "query_graph": {
+                "nodes": {
+                    "type-2 diabetes": {"ids": ["MONDO:0005148"]},
+                    "drug": {"categories": ["biolink:Drug"]}
+                },
+                "edges": {
+                    "treats": {"subject": "drug", "predicates": ["biolink:treats"], "object": "type-2 diabetes"}
+                }
             },
-            "edges": {
-                "treats": {"subject": "drug", "predicates": ["biolink:treats"], "object": "type-2 diabetes"}
-            }
-        },
-        "knowledge_graph": {
-            "nodes": {
-                "MONDO:0005148": {"name": "type-2 diabetes"},
-                "CHEBI:6801": {"name": "metformin", "categories": ["biolink:Drug"]}
+            "knowledge_graph": {
+                "nodes": {
+                    "MONDO:0005148": {"name": "type-2 diabetes"},
+                    "CHEBI:6801": {"name": "metformin", "categories": ["biolink:Drug"]}
+                },
+                "edges": {
+                    "df87ff82": {
+                        "subject": "CHEBI:6801",
+                        "predicate": "biolink:treats",
+                        "object": "MONDO:0005148",
+                        "sources": [
+                           {
+                               "resource_id": "infores:aragorn",
+                               "resource_role": "primary_knowledge_source"
+                           },
+                           {
+                               "resource_id": "infores:chebi",
+                               "resource_role": "primary_knowledge_source"
+                           }
+                        ]
+                    }
+                }
             },
-            "edges": {
-                "df87ff82": {"subject": "CHEBI:6801", "predicate": "biolink:treats", "object": "MONDO:0005148"}
-            }
+            "results": [
+                {
+                    "node_bindings": {
+                        "type-2 diabetes": [{"id": "MONDO:0005148"}],
+                        "drug": [{"id": "CHEBI:6801"}]
+                    },
+                    "analyses": [
+                        {
+                            "resource_id": "infores:aragorn",
+                            "edge_bindings": {
+                                    "treats": [{"id": "df87ff82"}]
+                            }
+                        }
+                    ]
+                }
+            ]
         },
-        "results": [
+        "workflow": [
             {
-                "node_bindings": {
-                    "type-2 diabetes": [{"id": "MONDO:0005148"}],
-                    "drug": [{"id": "CHEBI:6801"}]
-                },
-                "edge_bindings": {
-                    "treats": [{"id": "df87ff82"}]
-                }
+                "id": "lookup"
             }
         ]
-      }
     }
 
-one should typically get a response body like the following JSON validation result back:
+then, one should typically get a response body like the following JSON validation result back:
 
 .. code-block:: json
 
     {
-      "trapi_version": "1.3.0",
-      "biolink_version": "3.0.3",
-      "report": [
-        {
-          "code": "warning.node.unmapped_prefix",
-          "node_id": "CHEBI:6801",
-          "categories": "['biolink:Drug']"
-        },
-        {
-          "code": "error.node.missing_categories",
-          "node_id": "MONDO:0005148"
+      "trapi_version": "v1.4.0",
+      "biolink_version": "3.2.6",
+      "messages": {
+        "errors": {
+          "error.knowledge_graph.node.category.missing": {
+            "MONDO:0005148": [
+              {
+                "context": "Knowledge Graph"
+              }
+            ]
+          }
         },
-        {
-          "code": "error.edge.attribute.missing"
-        }
-      ]
+        "warnings": {
+          "warning.knowledge_graph.node.id.unmapped_prefix": {
+            "CHEBI:6801": [
+              {
+                "categories": "['biolink:Drug']"
+              }
+            ]
+          },
+          "warning.knowledge_graph.edge.provenance.kp.missing": {
+            "infores:panther": [
+              {
+                "kp_source_type": "biolink:primary_knowledge_source",
+                "identedge_idifier": "CHEBI:6801--biolink:treats->MONDO:0005148"
+              }
+            ]
+          }
+        },
+        "information": {}
+      }
     }
 
 Validation Code Definitions
 ===========================
 
 The validation message codes issued by the validation software is formally indexed in a single file called codes.yaml.
```

### Comparing `reasoner_validator-3.4.9/docs/make.bat` & `reasoner_validator-3.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.9/docs/validation_codes_dictionary.md` & `reasoner_validator-3.5.0/docs/validation_codes_dictionary.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,112 +1,96 @@
 # Validation Codes Dictionary
 
 ## Information
 
 ### info.excluded
 
-**Message:** User excluded S-P-O triple '{identifier}' or all test case S-P-O triples from resource test location.
+**Message:** All test case S-P-O triples from resource test location, or specific user excluded S-P-O triples
+
+**Context:** identifier
 
 **Description:** Check the JSON KP test edge data file for specific 'exclude_tests' directives, either global to the file, or on specific edges.
 
 ### info.compliant
 
-**Message:** Biolink Model-compliant TRAPI Message.
+**Message:** Biolink Model-compliant TRAPI Message
 
 **Description:** Specified TRAPI message completely satisfies the target TRAPI schema and Biolink Model semantics for specified releases of these standards.
 
-### info.input_edge.node.category.abstract
-
-**Message:** '{identifier}' is abstract.
-
-**Description:** Input Edge data can have 'abstract' category classes.
-
-### info.input_edge.node.category.mixin
-
-**Message:** '{identifier}' is a mixin.
-
-**Description:** Input Edge data can have 'mixin' category classes.
-
 ### info.input_edge.predicate.abstract
 
-**Message:** '{identifier}' is abstract.
-
-**Description:** Input Edge data can have 'abstract' predicates.
-
-### info.input_edge.predicate.mixin
-
-**Message:** '{identifier}' is a mixin.
-
-**Description:** Input Edge data can have 'mixin' predicates.
+**Message:** Edge has an 'abstract' predicate
 
-### info.query_graph.node.category.abstract
+**Context:** edge_id, identifier
 
-**Message:** '{identifier}' is abstract.
+**Description:** Input edge data can have 'abstract' predicates, when the mode of validation is 'non-strict'.
 
-**Description:** TRAPI Message Query Graphs can have 'abstract' category classes.
+### info.input_edge.predicate.mixin
 
-### info.query_graph.node.category.mixin
+**Message:** Edge has an 'mixin' predicate
 
-**Message:** '{identifier}' is a mixin.
+**Context:** edge_id, identifier
 
-**Description:** TRAPI Message Query Graphs can have 'mixin' category classes.
+**Description:** Input edge data can have 'mixin' predicates, when the mode of validation is 'non-strict'.
 
 ### info.query_graph.edge.predicate.abstract
 
-**Message:** '{identifier}' is abstract.
-
-**Description:** TRAPI Messages in Query Graphs can have 'mixin' predicates.
-
-### info.query_graph.edge.predicate.mixin
-
-**Message:** '{identifier}' is a mixin.
-
-**Description:** TRAPI Messages in Query Graphs can have 'mixin' predicates.
+**Message:** Edge has an 'abstract' predicate
 
-### info.knowledge_graph.node.category.abstract
+**Context:** edge_id, identifier
 
-**Message:** '{identifier}' is abstract.
+**Description:** TRAPI Messages in Query Graphs can have 'abstract' predicates, when the mode of validation is 'non-strict'.
 
-**Description:** TRAPI Messages in Knowledge Graphs can have 'abstract' category classes when the mode of validation is 'non-strict'..
+### info.query_graph.edge.predicate.mixin
 
-### info.knowledge_graph.node.category.mixin
+**Message:** Edge has an 'mixin' predicate
 
-**Message:** '{identifier}' is a mixin!
+**Context:** edge_id, identifier
 
-**Description:** TRAPI Messages in Knowledge Graphs can have 'mixin' category classes when the mode of validation is 'non-strict'..
+**Description:** TRAPI Messages in Query Graphs can have 'mixin' predicates, when the mode of validation is 'non-strict'.
 
 ### info.knowledge_graph.edge.predicate.abstract
 
-**Message:** '{identifier}' is abstract.
+**Message:** Edge has an 'abstract' predicate
+
+**Context:** edge_id, identifier
 
-**Description:** TRAPI Messages in Knowledge Graphs can have 'abstract' predicates when the mode of validation is 'non-strict'.
+**Description:** TRAPI Messages in Knowledge Graphs can have 'abstract' predicates, when the mode of validation is 'non-strict'.
 
 ### info.knowledge_graph.edge.predicate.mixin
 
-**Message:** '{identifier}' is mixin.
+**Message:** Edge has an 'mixin' predicate
+
+**Context:** edge_id, identifier
 
-**Description:** TRAPI Messages in Knowledge Graphs can have 'mixin' predicates when the mode of validation is 'non-strict'.
+**Description:** TRAPI Messages in Knowledge Graphs can have 'mixin' predicates, when the mode of validation is 'non-strict'.
 
 ### info.knowledge_graph.edge.attribute.type_id.abstract
 
-**Message:** '{identifier}' is abstract.
+**Message:** Edge has an 'abstract' attribute_type_id
 
-**Description:** TRAPI Messages in Knowledge Graphs can have 'abstract' attribute type identifiers when the mode of validation is 'non-strict'.
+**Context:** edge_id, identifier
+
+**Description:** TRAPI Messages in Knowledge Graphs can have 'abstract' attribute type identifiers, when the mode of validation is 'non-strict'.
 
 ### info.knowledge_graph.edge.attribute.type_id.mixin
 
-**Message:** '{identifier}' is mixin.
+**Message:** Edge has an 'mixin' attribute_type_id
+
+**Context:** edge_id, identifier
 
-**Description:** TRAPI Messages in Knowledge Graphs can have 'mixin' attribute type identifiers when the mode of validation is 'non-strict'.
+**Description:** TRAPI Messages in Knowledge Graphs can have 'mixin' attribute type identifiers, when the mode of validation is 'non-strict'.
 
 ## Warning
 
 ### warning.trapi.response.status.unknown
 
-**Message:** TRAPI Response status code '{identifier}' is unrecognized?
+**Message:** TRAPI Response has unrecognized status code
+
+**Context:** identifier
 
 **Description:** The TRAPI Response status code should be one of a standardized set of short codes, e.g. Success, QueryNotTraversable, KPsNotAvailable
 
 ### warning.trapi.response.workflow.runner_parameters.null
 
 **Message:** TRAPI Response.workflow.runner_parameters property is missing?
 
@@ -116,15 +100,17 @@
 
 **Message:** TRAPI Response.workflow.parameters property is missing?
 
 **Description:** If a 'parameters' property value is given for a workflow step specification, it should not be null. This field will be ignored?
 
 ### warning.graph.empty
 
-**Message:** {identifier} data is empty?
+**Message:** Empty graph
+
+**Context:** identifier
 
 **Description:** An empty graph in this particular context is allowed but merits a boundary response warning?
 
 ### warning.response.knowledge_graph.empty
 
 **Message:** Response returned an empty Message Knowledge Graph?
 
@@ -134,161 +120,209 @@
 
 **Message:** Response returned empty Message.results?
 
 **Description:** Empty Results is allowed but merits a boundary response warning?
 
 ### warning.input_edge.node.category.deprecated
 
-**Message:** '{identifier}' is deprecated?
+**Message:** Node category had deprecated category
+
+**Context:** node_id, identifier
+
+**Description:** Node category is deprecated in the current model, to be removed in the future. Review Biolink Model for suitable replacement?
+
+### warning.input_edge.node.category.not_concrete
+
+**Message:** Node has unknown, abstract or mixin category
+
+**Context:** node_id, identifier
 
-**Description:** Input data node category is deprecated in the current model, to be removed in the future. Review Biolink Model for suitable replacement?
+**Description:** Node category may be unknown, abstract or a mixin in the current model. TRAPI Responses using this edge may not resolve any Knowledge Graph nodes with this category. Review Biolink Model for 'concrete' replacement?
 
 ### warning.input_edge.node.id.unmapped_to_category
 
-**Message:** '{identifier}' has identifiers {unmapped_ids} unmapped to the target categories: {categories}?
+**Message:** Node identifier found unmapped to target categories for node
+
+**Context:** identifier, unmapped_ids, categories
 
 **Description:** The namespaces of Biolink model node of specified category may be incomplete with respect to identifiers being used in input edge data?
 
 ### warning.input_edge.predicate.deprecated
 
-**Message:** '{identifier}' is deprecated?
+**Message:** Edge has deprecated predicate
+
+**Context:** identifier
 
 **Description:** Input data edge predicate is deprecated in the current model, to be removed in the future. Review Biolink Model for a suitable replacement?
 
 ### warning.input_edge.predicate.non_canonical
 
-**Message:** Input data edge '{identifier}' predicate '{predicate}' is non-canonical?
+**Message:** Edge has non-canonical predicate
+
+**Context:** edge_id, identifier
 
 **Description:** A predicate selected for use as input data should preferably be tagged as 'canonical' in the specified Biolink Model release?
 
-### warning.query_graph.node.ids.unmapped_to_categories
+### warning.query_graph.node.category.deprecated
+
+**Message:** Node has deprecated category
+
+**Context:** node_id, identifier
+
+**Description:** Node category is deprecated in the current model, to be removed in the future. Review Biolink Model for suitable replacement?
 
-**Message:** '{identifier}' has identifiers {unmapped_ids} unmapped to the target categories: {categories}?
+### warning.query_graph.node.ids.unmapped_prefix
 
-**Description:** The namespaces of Biolink model node of specified categories may be incomplete with respect to identifiers being used in the query graph?
+**Message:** Node identifiers found unmapped to target categories for node
+
+**Context:** identifier, unmapped_ids, categories
+
+**Description:** One or more node CURIE identifier namespaces are not found among any 'id_prefix' slot values in specified categories in the validating Biolink Model version?
 
 ### warning.query_graph.edge.predicate.deprecated
 
-**Message:** '{identifier}' is deprecated?
+**Message:** Edge has deprecated predicate
+
+**Context:** identifier
 
-**Description:** Query graph edge predicate is deprecated in the current model, to be removed in the future. Review Biolink Model for a suitable replacement?
+**Description:** Edge predicate is deprecated in the current model, to be removed in the future. Review Biolink Model for a suitable replacement?
 
 ### warning.query_graph.edge.predicate.non_canonical
 
-**Message:** Query graph edge '{identifier}' predicate '{predicate}' is non-canonical?
+**Message:** Edge has non-canonical predicate
+
+**Context:** edge_id, identifier
 
 **Description:** A predicate selected for use in a query graph should preferably be tagged as 'canonical' in the specified Biolink Model release?
 
 ### warning.knowledge_graph.node.category.deprecated
 
-**Message:** '{identifier}' is deprecated?
-
-**Description:** Knowledge graph node category is deprecated in the current model, to be removed in the future. Review Biolink Model for a suitable replacement?
+**Message:** Node has deprecated category
 
-### warning.knowledge_graph.node.unmapped_prefix
+**Context:** node_id, identifier
 
-**Message:** '{identifier}' is unmapped to the target categories '{categories}'?
+**Description:** Node category is deprecated in the current model, to be removed in the future. Review Biolink Model for a suitable replacement?
 
-**Description:** ID Namespaces of nodes of specified categories may be incomplete with respect to Biolink Model version being used in the knowledge graph?
+### warning.knowledge_graph.node.id.unmapped_prefix
 
-### warning.knowledge_graph.node.id.unmapped_to_category
+**Message:** Node identifier found unmapped to target categories for node
 
-**Message:** {context} node identifier '{identifier}' is unmapped to '{category}'?
+**Context:** identifier, categories
 
-**Description:** ID Namespaces of nodes of specified categories may be incomplete with respect to Biolink Model version being used in the knowledge graph?
+**Description:** Node CURIE identifier namespace not found among any 'id_prefix' slot values in specified categories in the validating Biolink Model version?
 
 ### warning.knowledge_graph.edge.predicate.deprecated
 
-**Message:** '{identifier}' is deprecated?
-
-**Description:** Knowledge graph edge predicate is deprecated in the current model, to be removed in the future. Review Biolink Model for a suitable replacement?
+**Message:** Edge has deprecated predicate
 
-### warning.knowledge_graph.edge.predicate.non_canonical
+**Context:** identifier
 
-**Message:** Knowledge Graph '{identifier}' predicate '{predicate}' is non-canonical?
+**Description:** Edge predicate is deprecated in the current model, to be removed in the future. Review Biolink Model for a suitable replacement?
 
-**Description:** A predicate selected for use in a knowledge graph should preferably be tagged as 'canonical' in the specified Biolink Model release?
+### warning.knowledge_graph.edge.predicate.non_canonical
 
-### warning.knowledge_graph.edge.qualifiers.empty
+**Message:** Edge has non-canonical predicate
 
-**Message:** Edge qualifiers 
+**Context:** edge_id, identifier
 
-**Description:** Knowledge graph edge attributes should record the infores identifier of their knowledge source provenance with respect to ARA.
+**Description:** A predicate selected for use in a knowledge graph should preferably be tagged as 'canonical' in the specified Biolink Model release?
 
 ### warning.knowledge_graph.edge.attribute.type_id.not_association_slot
 
-**Message:** Edge '{identifier}' attribute_type_id '{attribute_type_id}' not a biolink:association_slot?
+**Message:** Edge has an attribute_type_id that is not an association slot
+
+**Context:** edge_id, identifier
 
-**Description:** Knowledge graph edge 'attribute_type_id' value should generally be a term defined within the biolink:association_slot hierarchy.
+**Description:** Edge 'attribute_type_id' value should generally be a term defined within the biolink:association_slot hierarchy.
 
 ### warning.knowledge_graph.edge.attribute.type_id.non_biolink_prefix
 
-**Message:** Edge '{identifier}' attribute_type_id '{attribute_type_id}' has a non-Biolink CURIE prefix mapped to Biolink.
+**Message:** Edge has an attribute_type_id that has a non-Biolink CURIE prefix mapped to Biolink
+
+**Context:** edge_id, identifier
 
 **Description:** Non-Biolink CURIEs are tolerated, but not preferred, as term value for the attribute_type_id properties of edge attributes.
 
 ### warning.knowledge_graph.edge.attribute.type_id.unknown_prefix
 
-**Message:** Edge '{identifier}' attribute_type_id '{attribute_type_id}' has a CURIE prefix namespace unknown to Biolink!
+**Message:** Edge has an attribute_type_id that has a CURIE prefix namespace unknown to Biolink
+
+**Context:** edge_id, identifier
 
 **Description:** The namespaces of 'attribute_type_id' terms may be incomplete with respect to Biolink Model version being used in the knowledge graph.
 
 ### warning.knowledge_graph.edge.attribute.type_id.deprecated
 
-**Message:** '{identifier}' is deprecated?
+**Message:** Edge has a deprecated attribute_type_id
+
+**Context:** identifier
 
-**Description:** Knowledge graph edge 'attribute_type_id' is deprecated in current model, to be removed in the future. Review Biolink Model for replacement.
+**Description:** Edge 'attribute_type_id' is deprecated in current model, to be removed in the future. Review Biolink Model for replacement.
 
 ### warning.knowledge_graph.edge.provenance.multiple_primary
 
-**Message:** Edge '{identifier}' has recorded multiple 'primary' knowledge sources: '{sources}'?
+**Message:** Edge has recorded multiple 'primary' knowledge sources
+
+**Context:** identifier, sources
 
-**Description:** Knowledge graph edge attributes should record only a single primary knowledge source provenance attribute value.
+**Description:** Edge attributes should record only a single primary knowledge source provenance attribute value.
 
 ### warning.knowledge_graph.edge.provenance.ara.missing
 
-**Message:** Edge '{identifier}' is missing ARA knowledge source provenance '{ara_source}'?
+**Message:** Edge is missing ARA knowledge source provenance
 
-**Description:** Knowledge graph edge attributes ARAs should record the infores identifier of their knowledge source provenance with respect to ARA.
+**Context:** edge_id, identifier
+
+**Description:** Edge attributes ARAs should record the Infores identifier of their knowledge source provenance with respect to ARA.
 
 ### warning.knowledge_graph.edge.provenance.kp.missing
 
-**Message:** Edge '{identifier}' attribute values are missing expected Knowledge Provider '{kp_source}' '{kp_source_type}' provenance?
+**Message:** Edge attribute values are missing expected Knowledge Provider provenance
+
+**Context:** edge_id, identifier, kp_source_type
 
-**Description:** Knowledge graph edge attributes of ARAs and KPs should record the infores identifier of their knowledge source provenance with respect to KP.
+**Description:** Edge attributes of ARAs and KPs should record the infores identifier of their knowledge source provenance with respect to KP.
 
 ## Error
 
 ### error.non_compliant
 
-**Message:** S-P-O statement '{identifier}' is not compliant to Biolink Model {biolink_release}
+**Message:** S-P-O statement is not compliant to Biolink Model release
+
+**Context:** identifier, biolink_release
 
 **Description:** This knowledge statement is not compliant to the specified release of the Biolink Model. Review associated messages for underlying cause!
 
 ### error.trapi.validation
 
-**Message:** TRAPI {identifier} schema exception: '{exception}'!
+**Message:** Schema validation exception
+
+**Context:** identifier, reason
 
 **Description:** TRAPI query attempt triggered an abnormal server exception as noted.
 
 ### error.trapi.request.invalid
 
-**Message:** {identifier} could not generate a valid TRAPI query request object because {reason}!
+**Message:** Test could not generate a valid TRAPI query request object using identified element
+
+**Context:** identifier, test, reason
 
-**Description:** TRAPI query message could not be prepared for the indicated reason, thus query was not attempted.
+**Description:** Specified TRAPI query unit 'test' query could not be prepared for the indicated reason, using the identified Biolink starting element.
 
 ### error.trapi.response.empty
 
 **Message:** TRAPI Response is missing!
 
 **Description:** TRAPI Response to be validated should not be totally empty but should have a Message body.
 
 ### error.trapi.response.unexpected_http_code
 
-**Message:** TRAPI Response has an unexpected HTTP status code: '{status_code}'!
+**Message:** TRAPI Response has an unexpected HTTP status code
+
+**Context:** identifier
 
 **Description:** TRAPI query attempt returned an abnormal (non-200) server HTTP status code as noted.
 
 ### error.trapi.response.message.empty
 
 **Message:** TRAPI Response missing its Message!
 
@@ -310,15 +344,17 @@
 
 **Message:** TRAPI Message is missing its Knowledge Graph component!
 
 **Description:** TRAPI response should generally have a TRAPI request message Knowledge Graph key value in its reply.
 
 ### error.trapi.response.knowledge_graph.missing_expected_edge
 
-**Message:** TRAPI Response Message is missing an expected edge '{identifier}' in its Knowledge Graph!
+**Message:** Knowledge Graph of TRAPI Response Message is missing expected Edge
+
+**Context:** identifier
 
 **Description:** The given TRAPI Response is expected to return specific edge(s) relating to the original (test edge?) data used to prepare the TRAPI Request!
 
 ### error.trapi.response.results.missing
 
 **Message:** TRAPI Message is missing its Results component!
 
@@ -328,203 +364,267 @@
 
 **Message:** Response returned a non-array Message.Results!
 
 **Description:** TRAPI Message.Results must be an array data type (even if empty)
 
 ### error.trapi.response.results.missing_bindings
 
-**Message:** Neither the input id '{identifier}' nor resolved aliases were returned in the Result object IDs for node '{output_node_binding}' binding!
+**Message:** Result object IDs for output node binding did not return the original identifier nor aliases for input id
+
+**Context:** identifier, output_node_binding
 
 **Description:** TRAPI Message.Results cannot resolve its reported identifier mappings to the original query.
 
 ### error.input_edge.node.category.missing
 
-**Message:** Input edge node '{identifier}' is missing its category!
+**Message:** Category missing for node
 
-**Description:** Category value must be specified in an input test data edge!
+**Context:** identifier
 
-### error.input_edge.node.category.unknown
+**Description:** Category value must be specified in an input test data edge!
 
-**Message:** Input edge node '{identifier}' has unknown category '{category}'!
+### error.input_edge.node.category.not_a_category
 
-**Description:** Category specified in input test data edge node is not recorded in specified version of Biolink. Replace with a known category!
+**Message:** Asserted category is not a proper category class for node
 
-### error.input_edge.node.category.abstract
+**Context:** node_id, identifier
 
-**Message:** '{identifier}' is abstract!
+**Description:** Category specified in input test data edge node is not recorded as a category term in specified version of Biolink. Replace with a known category!
 
-**Description:** Category specified in input test data edge node is 'abstract' in specified version of Biolink. Replace with a concrete category!
+### error.input_edge.node.category.unknown
 
-### error.input_edge.node.category.mixin
+**Message:** Node has unknown category
 
-**Message:** '{identifier}' is a mixin!
+**Context:** node_id, identifier
 
-**Description:** Category specified in input test data edge node is a 'mixin' in specified version of Biolink. Replace with a concrete category!
+**Description:** Category specified in input test data edge node is not a model element recorded in specified version of Biolink. Replace with a known category!
 
 ### error.input_edge.node.id.missing
 
-**Message:** {identifier} node identifier is missing!
+**Message:** Node identifier is missing for node
+
+**Context:** identifier
 
 **Description:** Input test data edge data needs to have a specific node identifier for testing!
 
 ### error.input_edge.predicate.missing
 
-**Message:** Input test data edge '{identifier}' predicate is missing or empty!
+**Message:** Edge has missing or empty predicate
+
+**Context:** identifier
 
 **Description:** Input test edge data needs to have a specific edge predicate for testing!
 
 ### error.input_edge.predicate.unknown
 
-**Message:** '{identifier}' is unknown predicate!
+**Message:** Edge has unknown predicate
+
+**Context:** edge_id, identifier
 
 **Description:** Predicate specified in input test data edge is not recorded in specified version of Biolink. Replace with a known predicate!
 
 ### error.input_edge.predicate.abstract
 
-**Message:** '{identifier}' is abstract predicate!
+**Message:** Edge is not permitted to have 'abstract' predicate
 
-**Description:** Input Edge data validation is currently strict: predicates cannot be 'abstract'. Replace with a concrete predicate!
+**Context:** edge_id, identifier
+
+**Description:** Edge data validation is currently strict: predicates cannot be 'abstract'! Replace with a concrete predicate.
 
 ### error.input_edge.predicate.mixin
 
-**Message:** '{identifier}' is a mixin predicate!
+**Message:** Edge is not permitted to have an 'mixin' predicate
+
+**Context:** edge_id, identifier
 
-**Description:** Input Edge data validation is currently strict: predicates cannot be of type 'mixin'. Replace with a concrete predicate!
+**Description:** Edge data validation is currently strict: predicates cannot be of type 'mixin'! Replace with a concrete predicate.
 
 ### error.input_edge.predicate.invalid
 
-**Message:** Edge '{identifier}' predicate '{predicate}' is invalid!
+**Message:** Edge has invalid predicate
+
+**Context:** edge_id, identifier
 
 **Description:** Predicate specified in Input Edge is not defined as a predicate in specified version of Biolink. Replace with a proper predicate!
 
-### error.query_graph.node.category.unknown
+### error.query_graph.node.category.missing
+
+**Message:** Category is missing from node
 
-**Message:** '{identifier}' is unknown!
+**Context:** identifier
 
-**Description:** Category specified in Query Graph node is not recorded in specified version of Biolink. Replace with a defined category!
+**Description:** Category value must be specified in an query graph edge!
 
-### error.query_graph.node.category.abstract
+### error.query_graph.node.category.not_a_category
 
-**Message:** '{identifier}' is abstract!
+**Message:** Node has invalid category
 
-**Description:** 'Abstract' category from specified version of Biolink is specified in Query Graph node. Replace with a concrete category!
+**Context:** node_id, identifier
 
-### error.query_graph.node.category.mixin
+**Description:** Category specified in query graph edge node is not recorded as a category term in specified version of Biolink. Replace with a known category!
 
-**Message:** '{identifier}' is a mixin!
+### error.query_graph.node.category.unknown
 
-**Description:** 'Mixin' category from specified version of Biolink is specified in Query Graph node. Replace with a concrete category!
+**Message:** Node has unknown category
+
+**Context:** node_id, identifier
+
+**Description:** Category specified in query graph edge node is not a model element recorded in specified version of Biolink. Replace with a known category!
 
 ### error.query_graph.node.ids.not_array
 
-**Message:** Node '{identifier}.ids' slot value is not an array!
+**Message:** The 'ids' property value is not an array in node
+
+**Context:** identifier
 
-**Description:** Value of 'ids' slot in Query Graph node must be an array data type (even if empty)!
+**Description:** Value of 'ids' property in Query Graph node must be an array data type (even if empty)!
 
 ### error.query_graph.node.categories.not_array
 
-**Message:** Node '{identifier}.categories' slot value is not an array!
+**Message:** The 'categories' property value is not an array in node
 
-**Description:** Value of 'categories' slot in Query Graph node must be an array data type (even if empty)!
+**Context:** identifier
+
+**Description:** Value of 'categories' property in Query Graph node must be an array data type (even if empty)!
 
 ### error.query_graph.node.is_set.not_boolean
 
-**Message:** Node '{identifier}.is_set' slot is not a boolean value!
+**Message:** The 'is_set' property is not a boolean value in node
+
+**Context:** identifier
 
 **Description:** The 'is_set' field in node of Query Graph, if present, must be a boolean value!
 
 ### error.query_graph.edge.subject.missing
 
-**Message:** Edge '{identifier}' has a missing or empty 'subject' slot value!
+**Message:** The 'subject' property value is missing or empty in Edge
+
+**Context:** identifier
 
-**Description:** Query graph edge must have a 'subject' key with a non-empty associated value!
+**Description:** Edge must have a 'subject' key with a non-empty associated value!
 
 ### error.query_graph.edge.subject.missing_from_nodes
 
-**Message:** Edge 'subject' id '{object_id}' is missing from the nodes catalog!
+**Message:** The nodes catalog of query graph for missing the subject id recorded on Edge
+
+**Context:** edge_id, identifier
 
 **Description:** Every 'subject' identifier of every edge in a Query Graph must also be recorded in the list of nodes for that graph!
 
 ### error.query_graph.edge.object.missing
 
-**Message:** Edge '{identifier}' has a missing or empty 'object' slot value!
+**Message:** The 'object' property value is missing or empty in Edge
+
+**Context:** identifier
 
-**Description:** Query graph edge must have a 'object' key with a non-empty associated value!
+**Description:** Edge must have a 'object' key with a non-empty associated value!
 
 ### error.query_graph.edge.object.missing_from_nodes
 
-**Message:** Edge 'object' id '{object_id}' is missing from the nodes catalog!
+**Message:** The nodes catalog of query graph for missing the object id recorded on Edge
+
+**Context:** edge_id, identifier
 
 **Description:** Every 'object' identifier of every edge in a Query Graph must also be recorded in the list of nodes for that graph!
 
 ### error.query_graph.edge.predicate.missing
 
-**Message:** Edge '{identifier}' predicate is missing or empty!
+**Message:** Predicate is missing or empty for Edge
+
+**Context:** identifier
 
 **Description:** The predicate of Query Graph edge needs to specified using a 'predicate' key with an array list of one or more predicates!
 
 ### error.query_graph.edge.predicate.unknown
 
-**Message:** Edge '{identifier}' predicate '{predicate}' is unknown!
+**Message:** Edge has unknown predicate
+
+**Context:** edge_id, identifier
 
 **Description:** Predicate specified in Query Graph edge is not defined in specified version of Biolink. Replace with a defined predicate!
 
 ### error.query_graph.edge.predicate.not_array
 
-**Message:** Edge '{identifier}' predicate slot value is not an array!
+**Message:** Predicate property value is not an array for Edge
+
+**Context:** identifier
 
-**Description:** Value of 'predicate' slot value in Query Graph must be an array data type!
+**Description:** Value of 'predicate' property value in Query Graph must be an array data type!
 
 ### error.query_graph.edge.predicate.empty_array
 
-**Message:** Edge '{identifier}' predicate slot value is an empty array!
+**Message:** Predicate property value is an empty array for Edge
 
-**Description:** Value of 'predicate' array slot value in Query Graph must contain one or more predicates!
+**Context:** identifier
+
+**Description:** Value of 'predicate' array property value in Query Graph must contain one or more predicates!
 
 ### error.query_graph.edge.predicate.abstract
 
-**Message:** '{identifier}' is abstract!
+**Message:** Edge is not permitted to have an 'abstract' predicate
+
+**Context:** edge_id, identifier
 
-**Description:** Query Graph data validation is currently strict: cannot have 'abstract' predicates!
+**Description:** Query Graph data validation is currently strict: cannot have 'abstract' predicates! Replace with a concrete predicate.
 
 ### error.query_graph.edge.predicate.mixin
 
-**Message:** '{identifier}' is a mixin!
+**Message:** Edge is not permitted to have an 'mixin' predicate
+
+**Context:** edge_id, identifier
 
-**Description:** Query Graph data validation is currently strict: cannot have 'mixin' predicates!
+**Description:** Query Graph data validation is currently strict: cannot have 'mixin' predicates! Replace with a concrete predicate.
 
 ### error.query_graph.edge.predicate.invalid
 
-**Message:** Edge '{identifier}' predicate '{predicate}' is invalid!
+**Message:** Edge has invalid predicate
+
+**Context:** edge_id, identifier
 
 **Description:** Predicate specified in Query Graph edge is not defined as a predicate in specified version of Biolink. Replace with a proper predicate!
 
 ### error.query_graph.edge.attribute_constraints.not_array
 
-**Message:** Edge '{identifier}' attribute_constraints property value is not an array!
+**Message:** Attribute_constraints property value is not an array for Edge
+
+**Context:** identifier
 
-**Description:** Value of 'attribute_constraints' slot value in a Query Graph must be an array data type!
+**Description:** Value of 'attribute_constraints' property value in a Query Graph must be an array data type!
 
 ### error.query_graph.edge.qualifier_constraints.qualifier_set.empty
 
-**Message:** Edge '{identifier}' qualifier_set property value is empty!
+**Message:** Qualifier_set property value is empty for Edge
+
+**Context:** identifier
 
 **Description:** Value of a 'qualifier_constraints.qualifier_set' property in a Query Graph must not be non-empty array!
 
 ### error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.type_id.unknown
 
-**Message:** Edge '{identifier}' qualifier type_id '{qualifier_type_id}' is unknown!
+**Message:** Edge has unknown qualifier_type_id
+
+**Context:** edge_id, identifier
 
 **Description:** A qualifier qualifier_type_id must be defined in the specified version of Biolink!
 
-### error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.value.unresolved
+### error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.value.not_a_predicate
 
-**Message:** Edge '{identifier}' qualifier_value '{qualifier_value}' for '{qualifier_type_id}' cannot be resolved!
+**Message:** Qualifier_type_id 'biolink:qualified_predicate' for edge has a qualifier_value which is not a Biolink predicate.
 
-**Description:** A 'qualifier_value' for the specified 'qualifier_type_id' of a qualifier likely could not be resolved without knowledge of the edge category!
+**Context:** identifier, qualifier_value
+
+**Description:** The 'qualifier_value' for 'biolink:qualified_predicate' should be a Biolink predicate term!
+
+### error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.invalid
+
+**Message:** Validation of qualifier in a qualifier_constraints qualifier_set threw an unexpected exception!
+
+**Context:** identifier, qualifier_type_id, qualifier_value, reason
+
+**Description:** Validation of a specified 'qualifier_type_id' and 'qualifier_value' failed for a given exceptional reason!
 
 ### error.knowledge_graph.nodes.empty
 
 **Message:** No nodes found!
 
 **Description:** Knowledge graph in TRAPI messages must have a 'nodes' key and non-empty associated value!
 
@@ -532,239 +632,421 @@
 
 **Message:** No edges found!
 
 **Description:** Knowledge graph in TRAPI messages must have a 'edges' key and non-empty associated value!
 
 ### error.knowledge_graph.node.category.missing
 
-**Message:** '{identifier}' has a missing Biolink category!
+**Message:** Category is missing for node
 
-**Description:** Knowledge graph node must have a 'node' key with a non-empty associated value!
+**Context:** identifier
 
-### error.knowledge_graph.node.category.unknown
+**Description:** Category value must be specified in an knowledge graph edge!
 
-**Message:** '{identifier}' is unknown!
+### error.knowledge_graph.node.category.not_a_category
 
-**Description:** Category specified in Knowledge Graph node is not recorded in specified version of Biolink. Replace with a defined category!
+**Message:** Node has invalid category
 
-### error.knowledge_graph.node.category.abstract
+**Context:** node_id, identifier
 
-**Message:** '{identifier}' is abstract!
+**Description:** Category specified in knowledge graph edge node is not recorded as a category term in specified version of Biolink. Replace with a known category!
 
-**Description:** 'Abstract' category from specified version of Biolink is specified in Knowledge Graph node. Replace with a concrete category!
+### error.knowledge_graph.node.category.unknown
 
-### error.knowledge_graph.node.category.mixin
+**Message:** Node has unknown category
 
-**Message:** '{identifier}' is a mixin!
+**Context:** node_id, identifier
 
-**Description:** 'Mixin' category from specified version of Biolink is specified in Knowledge Graph node. Replace with a concrete category!
+**Description:** Category specified in knowledge graph edge node is not a model element recorded in specified version of Biolink. Replace with a known category!
 
 ### error.knowledge_graph.node.id.missing
 
-**Message:** {identifier} node identifier is missing!
+**Message:** Node identifier is missing for node
+
+**Context:** identifier
 
 **Description:** Knowledge graph node must have a 'id' key with a non-empty associated value!
 
 ### error.knowledge_graph.node.missing_categories
 
-**Message:** Node '{identifier}' is missing its categories!
+**Message:** Categories are missing for node
+
+**Context:** identifier
 
 **Description:** Knowledge graph node must have a 'categories' key with a non-empty associated value!
 
 ### error.knowledge_graph.node.ids.not_array
 
-**Message:** Node '{identifier}.ids' slot value is not an array!
+**Message:** The 'ids' property value is not an array for node
 
-**Description:** Value of 'ids' slot in Query Graph node must be an array data type!
+**Context:** identifier
+
+**Description:** Value of 'ids' property in Query Graph node must be an array data type!
 
 ### error.knowledge_graph.node.empty_ids
 
-**Message:** Node '{identifier}.ids' slot array is empty!
+**Message:** The 'ids' property array is empty for node
+
+**Context:** identifier
 
-**Description:** Value of 'ids' array slot in Knowledge Graph node must contain one or more node identifiers!
+**Description:** Value of 'ids' array property in Knowledge Graph node must contain one or more node identifiers!
 
 ### error.knowledge_graph.node.categories.not_array
 
-**Message:** Node '{identifier}.categories' slot value is not an array!
+**Message:** The categories property value is not an array for node
+
+**Context:** identifier
+
+**Description:** Value of 'categories' property in Knowledge Graph node must be an array data type!
+
+### error.knowledge_graph.node.categories.not_concrete
+
+**Message:** None of the asserted categories are concrete for node
 
-**Description:** Value of 'categories' slot in Knowledge Graph node must be an array data type!
+**Context:** identifier, categories
+
+**Description:** Categories specified in knowledge graph edge node may not resolve to any (non-abstract, non-mixin) category terms in the specified version of Biolink. Add at least one 'concrete' category (as the most specific category?)!
 
 ### error.knowledge_graph.node.empty_categories
 
-**Message:** Node '{identifier}.categories' slot array is empty!
+**Message:** The 'categories' property array is empty for node
+
+**Context:** identifier
 
-**Description:** Value of 'categories' array slot in Knowledge Graph node must contain one or more node category terms!
+**Description:** Value of 'categories' array property in Knowledge Graph node must contain one or more node category terms!
 
 ### error.knowledge_graph.node.is_set.not_boolean
 
-**Message:** Node '{identifier}.is_set' slot is not a boolean value!
+**Message:** The 'is_set' property is not a boolean value for node
+
+**Context:** identifier
 
 **Description:** The 'is_set' field in node of Knowledge Graph, if present, must be a boolean value!
 
 ### error.knowledge_graph.edge.subject.missing
 
-**Message:** Edge '{identifier}' has a missing or empty 'subject' slot value!
+**Message:** The 'subject' property value is missing or empty for Edge
 
-**Description:** Knowledge graph edge must have a 'subject' key with a non-empty associated value!
+**Context:** identifier
+
+**Description:** Edge must have a 'subject' key with a non-empty associated value!
 
 ### error.knowledge_graph.edge.subject.missing_from_nodes
 
-**Message:** Edge 'subject' id '{object_id}' is missing from the nodes catalog!
+**Message:** The nodes catalog of query graph for missing the subject id recorded on Edge
+
+**Context:** edge_id, identifier
 
 **Description:** Every 'subject' identifier of every edge in a Knowledge Graph must also be recorded in the list of nodes for that graph!
 
 ### error.knowledge_graph.edge.object.missing
 
-**Message:** Edge '{identifier}' has a missing or empty 'object' slot value!
+**Message:** The 'object' property value  is missing or empty for Edge
+
+**Context:** identifier
 
-**Description:** Knowledge graph edge must have a 'object' key with a non-empty associated value!
+**Description:** Edge must have a 'object' key with a non-empty associated value!
 
 ### error.knowledge_graph.edge.object.missing_from_nodes
 
-**Message:** Edge 'object' id '{object_id}' is missing from the nodes catalog!
+**Message:** The nodes catalog of query graph for missing the object id recorded on Edge
+
+**Context:** edge_id, identifier
 
 **Description:** Every 'object' identifier of every edge in a Knowledge Graph must also be recorded in the list of nodes for that graph!
 
 ### error.knowledge_graph.edge.predicate.missing
 
-**Message:** Edge '{identifier}' predicate is missing or empty!
+**Message:** The predicate is missing or empty for Edge
+
+**Context:** identifier
 
-**Description:** Knowledge graph edge must have a 'predicate' key with a non-empty associated value!
+**Description:** Edge must have a 'predicate' key with a non-empty associated value!
 
 ### error.knowledge_graph.edge.predicate.unknown
 
-**Message:** Edge '{identifier}' predicate '{predicate}' is unknown!
+**Message:** Edge has unknown predicate
+
+**Context:** edge_id, identifier
 
 **Description:** Predicate specified in Knowledge Graph edge is not defined in specified version of Biolink. Replace with a defined predicate!
 
 ### error.knowledge_graph.edge.predicate.invalid
 
-**Message:** Edge '{identifier}' predicate '{predicate}' is invalid!
+**Message:** Edge has invalid predicate
+
+**Context:** edge_id, identifier
 
 **Description:** Predicate specified in Knowledge Graph edge is not defined as a predicate in specified version of Biolink. Replace with a defined predicate!
 
 ### error.knowledge_graph.edge.predicate.not_array
 
-**Message:** Edge '{identifier}' predicate slot value is not an array!
+**Message:** The predicate property value is not an array for Edge
+
+**Context:** identifier
 
-**Description:** Value of the 'predicate' slot in Knowledge Graph edge must be an array data type!
+**Description:** Value of the 'predicate' property in Knowledge Graph edge must be an array data type!
 
 ### error.knowledge_graph.edge.predicate.empty_array
 
-**Message:** Value of the 'predicate' array slot in Knowledge Graph edge must contain one or more predicates!
+**Message:** The predicate property value is an empty array for Edge
+
+**Context:** identifier
 
-**Description:** Value of the 'predicate' array slot in Knowledge Graph edge must contain one or more predicates!
+**Description:** Value of the 'predicate' array property in Knowledge Graph edge must contain one or more predicates!
 
 ### error.knowledge_graph.edge.predicate.abstract
 
-**Message:** '{identifier}' is abstract!
+**Message:** Edge is not permitted to have an 'abstract' predicate
 
-**Description:** Knowledge Graph data validation is currently strict: cannot have 'abstract' predicates!
+**Context:** edge_id, identifier
+
+**Description:** Knowledge Graph data validation is currently strict: cannot have 'abstract' predicates! Replace with a concrete predicate.
 
 ### error.knowledge_graph.edge.predicate.mixin
 
-**Message:** '{identifier}' is a mixin!
+**Message:** Edge is not permitted to have an 'mixin' predicate
+
+**Context:** edge_id, identifier
 
-**Description:** Knowledge Graph data validation is currently strict: cannot have 'mixin' predicates!
+**Description:** Knowledge Graph data validation is currently strict: cannot have 'mixin' predicates! Replace with a concrete predicate.
 
 ### error.knowledge_graph.edge.attribute.missing
 
-**Message:** Edge '{identifier}' has no 'attributes' key!
+**Message:** Missing 'attributes' key for Edge
+
+**Context:** identifier
 
-**Description:** Knowledge graph edge must have a 'attributes' key with a non-empty associated value!
+**Description:** Edge must have a 'attributes' key with a non-empty associated value!
 
 ### error.knowledge_graph.edge.attribute.empty
 
-**Message:** Edge '{identifier}' has empty attributes!
+**Message:** Empty attributes in Edge
 
-**Description:** Value of 'attributes' slot in Knowledge Graph edge must contain a list of one or more attributes!
+**Context:** identifier
+
+**Description:** Value of 'attributes' property in Knowledge Graph edge must contain a list of one or more attributes!
 
 ### error.knowledge_graph.edge.attribute.not_array
 
-**Message:** Edge '{identifier}' attributes are not an array!
+**Message:** The attributes are not an array in Edge
+
+**Context:** identifier
 
-**Description:** Value of the 'attributes' slot in Knowledge Graph edge must be an array of attributes!
+**Description:** Value of the 'attributes' property in Knowledge Graph edge must be an array of attributes!
 
 ### error.knowledge_graph.edge.attribute.type_id.unknown
 
-**Message:** '{identifier}' is unknown attribute type identifier!
+**Message:** Edge has unknown attribute_type_id
+
+**Context:** edge_id, identifier
 
 **Description:** Edge Attribute type identifier specified in knowledge graph edge is not recorded in specified version of Biolink. Replace with a known term!
 
 ### error.knowledge_graph.edge.attribute.type_id.abstract
 
-**Message:** '{identifier}' is abstract attribute type identifier!
+**Message:** Edge is not permitted to have an 'abstract' attribute_type_id
 
-**Description:** Edge data validation is currently strict: attribute type identifiers cannot be 'abstract'. Replace with a concrete attribute type identifier!
+**Context:** edge_id, identifier
+
+**Description:** Edge data validation is currently strict: attribute type identifiers cannot be 'abstract'. Replace with a concrete attribute_type_id!
 
 ### error.knowledge_graph.edge.attribute.type_id.mixin
 
-**Message:** '{identifier}' is a mixin attribute type identifier!
+**Message:** Edge is not permitted to have an 'mixin' attribute_type_id
+
+**Context:** edge_id, identifier
 
-**Description:** Edge data validation is currently strict: attribute type identifiers cannot be of type 'mixin'. Replace with a concrete attribute type identifier!
+**Description:** Edge data validation is currently strict: attribute type identifiers cannot be of type 'mixin'. Replace with a concrete attribute_type_id!
 
 ### error.knowledge_graph.edge.attribute.type_id.missing
 
-**Message:** Edge '{identifier}' attribute is missing its 'attribute_type_id' property!
+**Message:** An attribute is missing its 'attribute_type_id' property in Edge
+
+**Context:** identifier
 
 **Description:** The attribute of a Knowledge graph edge must have a 'attribute_type_id' key with a non-empty associated value!
 
 ### error.knowledge_graph.edge.attribute.type_id.empty
 
-**Message:** Edge'{identifier}' attribute empty 'attribute_type_id' property!
+**Message:** An attribute has empty 'attribute_type_id' property in Edge
+
+**Context:** identifier
 
 **Description:** The value of the 'attribute_type_id' of an attribute of a Knowledge graph edge must not be empty!
 
 ### error.knowledge_graph.edge.attribute.type_id.not_curie
 
-**Message:** Edge '{identifier}' attribute_type_id '{attribute_type_id}' is not a CURIE!
+**Message:** Edge has a value that is not a CURIE for attribute_type_id
+
+**Context:** edge_id, identifier
 
 **Description:** The 'attribute_type_id' of a Knowledge graph edge attribute must be a controlled vocabulary term specified by a CURIE!
 
 ### error.knowledge_graph.edge.attribute.value.missing
 
-**Message:** Edge '{identifier}' attribute is missing its 'value' property!
+**Message:** An attribute is missing its 'value' property in Edge
+
+**Context:** identifier
 
 **Description:** An attribute of a Knowledge graph edge must have a 'value' key with a non-empty associated value!
 
 ### error.knowledge_graph.edge.attribute.value.empty
 
-**Message:** Edge '{identifier}' attribute empty 'value' property!
+**Message:** An attribute has an empty value in Edge
+
+**Context:** identifier
 
 **Description:** The value of an attribute of a Knowledge graph edge must not be empty!
 
 ### error.knowledge_graph.edge.provenance.infores.missing
 
-**Message:** Edge '{identifier}' has provenance value '{infores}' which is not a well-formed InfoRes CURIE!
+**Message:** Edge has provenance value which is not a well-formed InfoRes CURIE
+
+**Context:** edge_id, identifier
 
 **Description:** The value of an attribute specifying the provenance of a Knowledge graph edge must be the well-formed InfoRes CURIE of a knowledge source!
 
 ### error.knowledge_graph.edge.provenance.missing_primary
 
-**Message:** Edge '{identifier}' does not record its 'primary' knowledge source?
+**Message:** A 'primary' knowledge source is missing for Edge
+
+**Context:** identifier
 
-**Description:** Knowledge graph edge attributes should record the 'infores' identifier of their primary knowledge source provenance with respect to KP.
+**Description:** Edge attributes should record the 'infores' identifier of their primary knowledge source provenance with respect to KP.
 
 ### error.knowledge_graph.edge.qualifiers.not_array
 
-**Message:** Edge '{identifier}' 'qualifiers' are not an array!
+**Message:** The 'qualifiers' property is not an array in Edge
 
-**Description:** Value of the 'qualifiers' slot in Knowledge Graph edge must be an array of attributes!
+**Context:** identifier
+
+**Description:** Value of the 'qualifiers' property in Knowledge Graph edge must be an array of attributes!
 
 ### error.knowledge_graph.edge.qualifiers.empty
 
-**Message:** Edge '{identifier}' qualifiers property value is empty!
+**Message:** The qualifiers property value is empty in Edge
+
+**Context:** identifier
 
 **Description:** Value of a 'qualifiers' property in a Knowledge Graph must not be non-empty array!
 
 ### error.knowledge_graph.edge.qualifiers.qualifier.type_id.unknown
 
-**Message:** Edge '{identifier}' qualifier type_id '{qualifier_type_id}' is unknown!
+**Message:** Edge has unknown qualifier_type_id
+
+**Context:** edge_id, identifier
 
 **Description:** A qualifier qualifier_type_id must be defined in the specified version of Biolink!
 
 ### error.knowledge_graph.edge.qualifiers.qualifier.value.unresolved
 
-**Message:** Edge '{identifier}' qualifier_value '{qualifier_value}' for '{qualifier_type_id}' cannot be resolved!
+**Message:** Qualifier_type_id for edge has unresolved qualifier_value
+
+**Context:** edge_id, identifier, qualifier_type_id
 
 **Description:** A 'qualifier_value' for the specified 'qualifier_type_id' of a qualifier likely could not be resolved without knowledge of the edge category!
 
+### error.knowledge_graph.edge.qualifiers.qualifier.value.not_a_predicate
+
+**Message:** Qualifier_type_id 'biolink:qualified_predicate' for edge has a qualifier_value which is not a Biolink predicate.
+
+**Context:** identifier, qualifier_value
+
+**Description:** The 'qualifier_value' for 'biolink:qualified_predicate' should be a Biolink predicate term!
+
+### error.knowledge_graph.edge.qualifiers.qualifier.invalid
+
+**Message:** Validation of qualifier in qualifiers threw an unexpected exception
+
+**Context:** identifier, qualifier_type_id, qualifier_value, reason
+
+**Description:** Validation of a specified 'qualifier_type_id' and 'qualifier_value' failed for a given exceptional reason!
+
+### error.knowledge_graph.edge.sources.missing
+
+**Message:** Missing 'sources' key for Edge
+
+**Context:** identifier
+
+**Description:** Edge must have a 'sources' key with a non-empty associated value!
+
+### error.knowledge_graph.edge.sources.empty
+
+**Message:** Empty 'sources' property in Edge
+
+**Context:** identifier
+
+**Description:** Value of 'sources' property in Knowledge Graph edge must contain a list of one or more RetrievalSource entries!
+
+### error.knowledge_graph.edge.sources.not_array
+
+**Message:** The 'sources' are not an array in Edge
+
+**Context:** identifier
+
+**Description:** Value of the 'sources' property in Knowledge Graph edge must be an array of RetrievalSource entries!
+
+### error.knowledge_graph.edge.sources.retrieval_source.resource_id.infores.not_curie
+
+**Message:** Infores value is not a valid well-formed CURIE
+
+**Context:** edge_id, identifier
+
+**Description:** A 'retrieval_source.resource_id' value must be a well-formed infores CURIE!
+
+### error.knowledge_graph.edge.sources.retrieval_source.resource_id.infores.invalid
+
+**Message:** Invalid Infores namespace
+
+**Context:** edge_id, identifier
+
+**Description:** A 'retrieval_source.resource_id' Infores CURIE must come from the Infores namespace!
+
+### error.knowledge_graph.edge.sources.retrieval_source.resource_id.infores.unknown
+
+**Message:** Unregistered infores
+
+**Context:** edge_id, identifier
+
+**Description:** A 'retrieval_source.resource_id' value must be a registered Infores identifier!
+
+### error.knowledge_graph.edge.sources.retrieval_source.resource_id.empty
+
+**Message:** Empty 'resource_id' property in Edge
+
+**Context:** identifier
+
+**Description:** Value of the 'resource_id' property in the RetrievalSource of a Knowledge Graph Edge must be a non-empty Infores identifier!
+
+### error.knowledge_graph.edge.sources.retrieval_source.upstream_resource_ids.infores.not_curie
+
+**Message:** Infores value is not a valid well-formed CURIE
+
+**Context:** edge_id, identifier
+
+**Description:** A 'retrieval_source.upstream_resource_ids' values must be a well-formed Infores CURIE!
+
+### error.knowledge_graph.edge.sources.retrieval_source.upstream_resource_ids.infores.invalid
+
+**Message:** Invalid Infores namespace
+
+**Context:** edge_id, identifier
+
+**Description:** A 'retrieval_source.upstream_resource_ids' Infores CURIEs must come from the Infores namespace!
+
+### error.knowledge_graph.edge.sources.retrieval_source.upstream_resource_ids.infores.unknown
+
+**Message:** Unregistered Infores
+
+**Context:** edge_id, identifier
+
+**Description:** A 'retrieval_source.upstream_resource_ids' values must be registered infores identifiers!
+
+### error.knowledge_graph.edge.sources.retrieval_source.resource_role.empty
+
+**Message:** Empty 'resource_role' property in Edge
+
+**Context:** identifier
+
+**Description:** Value of the 'resource_role' property in the RetrievalSource of a Knowledge Graph Edge must be a non-empty ResourceRole enum value!
+
```

### Comparing `reasoner_validator-3.4.9/reasoner_validator/__init__.py` & `reasoner_validator-3.5.0/reasoner_validator/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,18 @@
     BiolinkValidator
 )
 
 # Maximum number of data points to scrutinize
 # in various parts TRAPI Query Response.Message
 from reasoner_validator.trapi import check_trapi_validity, TRAPISchemaValidator
 from reasoner_validator.trapi.mapping import MappingValidator, check_node_edge_mappings
+from reasoner_validator.versioning import SemVer, SemVerError
+
+import logging
+logger = logging.getLogger(__name__)
 
 # Unspoken assumption here is that validation of results returned for
 # Biolink Model release compliance only needs to be superficial
 RESULT_TEST_DATA_SAMPLE_SIZE = 10
 
 
 class TRAPIResponseValidator(ValidationReporter):
@@ -23,35 +27,40 @@
     """
 
     def __init__(
             self,
             trapi_version: Optional[str] = None,
             biolink_version: Optional[str] = None,
             sources: Optional[Dict] = None,
-            strict_validation: bool = False
+            strict_validation: bool = False,
+            suppress_empty_data_warnings: bool = False
     ):
         """
         :param trapi_version: version of component against which to validate the message (mandatory, no default)
         :type trapi_version: str
         :param biolink_version: Biolink Model (SemVer) release against which the knowledge graph is to be
                                 validated (Default: if None, use the Biolink Model Toolkit default version).
         :type biolink_version: Optional[str] = None
-        :param sources: Dictionary of validation context identifying the ARA and KP for provenance attribute validation
+        :param sources: Dictionary of validation context identifying the ARA and KP for provenance attribute validation.
         :type sources: Dict
         :param strict_validation: if True, some tests validate as 'error'; None or False, simply issue a 'warning'
         :type strict_validation: Optional[bool] = None
+        :param suppress_empty_data_warnings: validation normally reports empty Message query graph, knowledge graph
+                       and results as warnings. This flag suppresses the reporting of such warnings (default: False).
+        :type suppress_empty_data_warnings: bool
         """
         ValidationReporter.__init__(
             self,
             prefix="Validate TRAPI Response",
             trapi_version=trapi_version,
             biolink_version=biolink_version,
             sources=sources,
             strict_validation=strict_validation
         )
+        self.suppress_empty_data_warnings = suppress_empty_data_warnings
 
     def sanitize_trapi_query(self, response: Dict) -> Dict:
         """
 
         :param response: Dict full TRAPI Response JSON object
         :return: Dict, response with discretionary removal of content which
                        triggers (temporarily) unwarranted TRAPI validation failures
@@ -66,15 +75,19 @@
                 if 'parameters' in step and not step['parameters']:
                     # There are some workflow types that have mandatory need for 'parameters'
                     # but this should be caught in a later schema validation step
                     self.report("warning.trapi.response.workflow.parameters.null")
                     step.pop('parameters')
         return response
 
-    def check_compliance_of_trapi_response(self, response: Optional[Dict], edges_limit: int = 100):
+    def check_compliance_of_trapi_response(
+            self,
+            response: Optional[Dict],
+            edges_limit: int = 100
+    ):
         """
         One stop validation of all components of a TRAPI-schema compliant
         Query.Response, including its Message against a designated Biolink Model release.
         The high level structure of a Query.Response is described in
         https://github.com/NCATSTranslator/ReasonerAPI/blob/master/docs/reference.md#response-.
 
         The TRAPI Query.Response.Message is a Python Dictionary with three entries:
@@ -84,41 +97,49 @@
                            returned from the target resource (KP, ARA) for the query.
         * Results: a list of (annotated) node and edge bindings pointing into the Knowledge Graph, to represent the
                    specific answers (subgraphs) satisfying the query graph constraints.
 
         :param response: Query.Response to be validated.
         :type response: Optional[Dict]
         :param edges_limit: integer maximum number of edges to be validated in the knowledge graph. A value of zero
-                            triggers validation of all edges in the knowledge graph (could take awhile! Default: 100)
+                            triggers validation of all edges in the knowledge graph (Default: 100)
         :type edges_limit: int
 
-        :returns: Validator cataloging "information", "warning" and "error" messages (may be empty)
+        :returns: Validator cataloging "information", "warning" and "error" messages (could be empty)
         :rtype: ValidationReporter
         """
-        if not (response and 'message' in response):
-            self.report("error.trapi.response.empty")
+        if not (response and "message" in response):
+            if not self.suppress_empty_data_warnings:
+                self.report("error.trapi.response.empty")
+
+            # nothing more to validate?
+            return
+
+        message: Optional[Dict] = response['message']
+        if not message:
+            if not self.suppress_empty_data_warnings:
+                self.report("error.trapi.response.message.empty")
+
+            # ... also, nothing more here to validate?
+            return
 
         response = self.sanitize_trapi_query(response)
 
         trapi_validator: TRAPISchemaValidator = check_trapi_validity(
             instance=response,
             component="Response",
             trapi_version=self.trapi_version
         )
         if trapi_validator.has_messages():
             self.merge(trapi_validator)
 
         status: Optional[str] = response['status'] if 'status' in response else None
-        if status and status not in ["Success", "QueryNotTraversable", "KPsNotAvailable"]:
+        if status and status not in ["OK", "Success", "QueryNotTraversable", "KPsNotAvailable"]:
             self.report("warning.trapi.response.status.unknown", identifier=status)
 
-        message: Optional[Dict] = response['message']
-        if not message:
-            self.report("error.trapi.response.message.empty")
-
         # Sequentially validate the Query Graph, Knowledge Graph then validate
         # the Results (which rely on the validity of the other two components)
         elif self.has_valid_query_graph(message) and \
                 self.has_valid_knowledge_graph(message, edges_limit):
             self.has_valid_results(message)
 
     @staticmethod
@@ -190,20 +211,22 @@
         """
         Validate a TRAPI Query Graph.
         :param message: input message expected to contain the 'query_graph'
         :return: bool, False, if validation errors
         """
         # Query Graph must not be missing...
         if 'query_graph' not in message:
-            self.report(code="error.trapi.response.query_graph.missing")
+            if not self.suppress_empty_data_warnings:
+                self.report(code="error.trapi.response.query_graph.missing")
         else:
             # ... nor empty
             query_graph = message['query_graph']
             if not (query_graph and len(query_graph) > 0):
-                self.report(code="error.trapi.response.query_graph.empty")
+                if not self.suppress_empty_data_warnings:
+                    self.report(code="error.trapi.response.query_graph.empty")
             else:
                 # Validate the TRAPI compliance of the Query Graph
                 trapi_validator: TRAPISchemaValidator = check_trapi_validity(
                     instance=query_graph,
                     component="QueryGraph",
                     trapi_version=self.trapi_version
                 )
@@ -240,26 +263,28 @@
         """
         # This integrity constraint may not really be necessary
         # since negative numbers are functionally inequivalent to zero
         assert edges_limit >= 0, "The 'edges_limit' must be zero or a positive integer!"
 
         # The Knowledge Graph should not be missing
         if 'knowledge_graph' not in message:
-            self.report(code="error.trapi.response.knowledge_graph.missing")
+            if not self.suppress_empty_data_warnings:
+                self.report(code="error.trapi.response.knowledge_graph.missing")
         else:
             knowledge_graph = message['knowledge_graph']
             # The Knowledge Graph should also not generally be empty? Issue a warning
             if not (
                     knowledge_graph and len(knowledge_graph) > 0 and
                     "nodes" in knowledge_graph and knowledge_graph["nodes"] and
                     "edges" in knowledge_graph and knowledge_graph["edges"]
             ):
-                self.report(code="warning.response.knowledge_graph.empty")
                 # An empty knowledge graph (warning) does not generally invalidate
                 # the whole Message, but no more validation tests are needed
+                if not self.suppress_empty_data_warnings:
+                    self.report(code="warning.response.knowledge_graph.empty")
             else:
                 mapping_validator: MappingValidator = check_node_edge_mappings(knowledge_graph)
                 if mapping_validator.has_messages():
                     self.merge(mapping_validator)
 
                 # ...then if not empty, validate a subgraph sample of the associated
                 # Knowledge Graph (since some TRAPI response kg's may be huge!)
@@ -275,14 +300,15 @@
                     self.merge(trapi_validator)
 
                 # Verify that the sample of the knowledge graph is
                 # compliant to the currently applicable Biolink Model release
                 biolink_validator: BiolinkValidator = \
                     check_biolink_model_compliance_of_knowledge_graph(
                         graph=kg_sample,
+                        trapi_version=self.trapi_version,
                         biolink_version=self.biolink_version,
                         sources=self.sources,
                         # the ValidationReporter calling this function *might*
                         # have an explicit strict_validation override (if not None)
                         strict_validation=self.strict_validation
                     )
                 if biolink_validator.has_messages():
@@ -299,42 +325,68 @@
         """
 
         #     :param output_element: test target, as edge 'subject' or 'object'
         #     :type output_element: str
         #     :param output_node_binding: node 'a' or 'b' of the ('one hop') QGraph test query
         #     :type output_node_binding: str
 
+        trapi_1_4_0: bool
+        try:  # try block ... Sanity check: in case the trapi_version is somehow invalid?
+            target_version: SemVer = SemVer.from_string(self.trapi_version)
+            trapi_1_4_0 = target_version >= SemVer.from_string("1.4.0")
+        except SemVerError as sve:
+            logger.error(f"has_valid_results() 'self.trapi_version' seems invalid: {str(sve)}. Reset to latest?")
+            self.trapi_version = "1.4.0"
+            trapi_1_4_0 = True
+
         # The Message.Results key should not be missing?
         if 'results' not in message:
-            self.report(code="error.trapi.response.results.missing")
+            if not self.suppress_empty_data_warnings:
+                self.report(code="error.trapi.response.results.missing")
         else:
             results = message['results']
+
             if not (results and len(results) > 0):
-                self.report(code="warning.response.results.empty")
-                # An empty result (warning) does not generally invalidate
-                # the whole Message, but no more validation tests are needed
+                if not self.suppress_empty_data_warnings:
+                    self.report(code="warning.response.results.empty")
+                    # An empty result (warning) does not generally invalidate
+                    # the whole Message, but no more validation tests are needed
+
             elif not isinstance(results, List):
                 # The Message.results should be an array of Result objects
+                # TODO: Is this test unnecessary, since TRAPI schema
+                #       validation (below) should normally catch this?
                 self.report(code="error.trapi.response.results.non_array")
+
             else:
                 # Validate a subsample of a non-empty Message.results component.
                 results_sample = self.sample_results(results)
                 for result in results_sample:
+
+                    # generally validate against the pertinent schema
                     trapi_validator: TRAPISchemaValidator = check_trapi_validity(
                         instance=result,
                         component="Result",
                         trapi_version=self.trapi_version
                     )
                     if trapi_validator.has_messages():
                         # Record the error messages associated with the Result set then... don't continue
                         self.merge(trapi_validator)
 
-                    # TODO: here, we might wish to compare the Results against the contents of the KnowledgeGraph,
-                    #       with respect to node input values from the QueryGraph but this is tricky to do solely
-                    #       with the subsamples, which may not completely overlap.
+                    # Maybe some additional TRAPI-release specific non-schematic validation here?
+                    if trapi_1_4_0:
+                        # TODO: implement me!
+                        pass
+                    else:
+                        pass
+
+                    # TODO: here, we could try to compare the Results against the contents of the KnowledgeGraph,
+                    #       with respect to node input values from the QueryGraph, but this is tricky to do solely
+                    #       with the subsamples, which may not completely overlap,
+                    #       and may also be somewhat computationally intensive?
 
                     # ...Finally, check that the sample Results contained the object of the Query
 
                     # The 'output_element' is 'subject' or 'object' target (unknown) of retrieval
                     # The 'output_node_binding' is (subject) 'a' or (object) 'b' keys in
                     # the QueryGraph.Nodes to be bound
                     # In principle, we detect which node in the QueryGraph has 'ids' associated with its node record
```

### Comparing `reasoner_validator-3.4.9/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.5.0/reasoner_validator/biolink/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,45 +2,48 @@
 Version-specific Biolink Model semantic validation of knowledge graph components.
 """
 from typing import Optional, Any, Dict, List, Tuple, Set
 from enum import Enum
 from functools import lru_cache
 from urllib.error import HTTPError
 from pprint import PrettyPrinter
-import logging
+
 
 from bmt import Toolkit
 from bmt.utils import parse_name
 from linkml_runtime.linkml_model import ClassDefinition, Element
 
 from reasoner_validator.sri.util import is_curie
 from reasoner_validator.report import ValidationReporter
 from reasoner_validator.versioning import SemVer, SemVerError
 
+import logging
 logger = logging.getLogger(__name__)
 
 pp = PrettyPrinter(indent=4)
 
 
 def _get_biolink_model_schema(biolink_version: Optional[str] = None) -> Optional[str]:
     # Get Biolink Model Schema
     if biolink_version:
         try:
-            svm = SemVer.from_string(biolink_version, ignore_prefix='v')
+            svm = SemVer.from_string(biolink_version)
 
             # Sanity check: override SemVer object to ignore prerelease and
             # buildmetadata variants of the Biolink Version given
             svm = SemVer(major=svm.major, minor=svm.minor, patch=svm.patch)
+
         except SemVerError:
             raise TypeError(
                 "The 'biolink_version' argument '"
                 + biolink_version
                 + "' is not a properly formatted semantic version?"
             )
 
+
         if svm >= SemVer.from_string("2.2.14"):
             biolink_version = "v" + str(svm)
         else:
             biolink_version = str(svm)
         schema = f"https://raw.githubusercontent.com/biolink/biolink-model/{biolink_version}/biolink-model.yaml"
         return schema
     else:
@@ -85,33 +88,37 @@
 class BiolinkValidator(ValidationReporter):
     """
     Wrapper class for Biolink Model validation.
     """
     def __init__(
         self,
         graph_type: TRAPIGraphType,
+        trapi_version: Optional[str] = None,
         biolink_version: Optional[str] = None,
         sources: Optional[Dict[str, str]] = None,
         strict_validation: bool = False
     ):
         """
         Biolink Validator constructor.
 
         :param graph_type: type of graph data being validated
         :type graph_type: TRAPIGraphType
-        :param biolink_version: caller specified Biolink Model version (default: None)
+        :param trapi_version: caller specified Biolink Model version (default: None, which takes the TRAPI 'latest')
+        :type trapi_version: Optional[str] or None
+        :param biolink_version: caller specified Biolink Model version (default: None, which takes the BMT 'latest')
         :type biolink_version: Optional[str] or None
         :param sources: Dictionary of validation context identifying the ARA and KP for provenance attribute validation
         :type sources: Optional[Dict[str,str]]
         """
         self.bmt: Toolkit = get_biolink_model_toolkit(biolink_version=biolink_version)
         resolved_biolink_version = self.bmt.get_model_version()
         ValidationReporter.__init__(
             self,
             prefix=f"Biolink Validation of {graph_type.value}",
+            trapi_version=trapi_version,
             biolink_version=resolved_biolink_version,
             sources=sources,
             strict_validation=strict_validation
         )
         self.graph_type: TRAPIGraphType = graph_type
         self.nodes: Set[str] = set()
 
@@ -124,15 +131,15 @@
             current: SemVer = SemVer.from_string(self.biolink_version)
             target: SemVer = SemVer.from_string(version)
             return current >= target
         except SemVerError as sve:
             logger.error(f"minimum_required_biolink_version() error: {str(sve)}")
             return False
 
-    def get_result(self) -> Tuple[str, Optional[Dict[str, Dict[str, Optional[List[Dict[str,str]]]]]]]:
+    def get_result(self) -> Tuple[str, Optional[Dict[str, Dict[str, Optional[List[Dict[str, str]]]]]]]:
         """
         Get result of validation.
 
         :return: model version of the validation and dictionary of reported validation messages.
         :rtype Tuple[str, Optional[Dict[str, Set[str]]]]
         """
         return self.bmt.get_model_version(), self.get_messages()
@@ -154,78 +161,102 @@
             #       probably no longer relevant to the community?
             if 'categories' in slots:
                 if not isinstance(slots["categories"], List):
                     self.report(code="error.knowledge_graph.node.categories.not_array", identifier=node_id)
                 else:
                     categories = slots["categories"]
                     node_prefix_mapped: bool = False
+                    concrete_category_found: bool = False
                     for category in categories:
                         category: Optional[ClassDefinition] = \
                             self.validate_category(
                                 context="knowledge_graph",
                                 node_id=node_id,
                                 category=category
                             )
+                        # Only 'concrete' (non-abstract, non-mixin, preferably,
+                        # non-deprecated) categories are of interest here,
+                        # since only they will have associated namespaces
                         if category:
+                            concrete_category_found: bool = True
                             possible_subject_categories = self.bmt.get_element_by_prefix(node_id)
-                            if category.name in possible_subject_categories:
+                            if possible_subject_categories and category.name in possible_subject_categories:
                                 node_prefix_mapped = True
+                                # don't need to search any more categories
+                                break
+
+                    if not concrete_category_found:
+                        self.report(
+                            code="error.knowledge_graph.node.categories.not_concrete",
+                            identifier=node_id,
+                            categories=str(categories)
+                        )
+
                     if not node_prefix_mapped:
                         self.report(
-                            code="warning.knowledge_graph.node.unmapped_prefix",
-                            identifier=node_id, categories=str(categories)
+                            code="warning.knowledge_graph.node.id.unmapped_prefix",
+                            identifier=node_id,
+                            categories=str(categories)
                         )
             else:
                 self.report(
                     code="error.knowledge_graph.node.category.missing",
                     context=self.graph_type.value, identifier=node_id
                 )
 
             # TODO: Do we need to (or can we) validate here, any other Knowledge Graph node fields? Perhaps not yet?
 
         else:  # Query Graph node validation
 
+            has_node_ids: bool
             if "ids" in slots and slots["ids"]:
-                ids = slots["ids"]
-                if not isinstance(ids, List):
+                has_node_ids = True
+                node_ids = slots["ids"]
+                if not isinstance(node_ids, List):
                     self.report(code="error.query_graph.node.ids.not_array", identifier=node_id)
                     # we'll pretend that the ids were mistakenly
                     # just a scalar string, then continue validating
-                    ids = [ids]
+                    node_ids = [node_ids]
             else:
-                ids = list()  # a null "ids" value is permitted in QNodes
+                has_node_ids = False
+                node_ids = list()  # a null "ids" value is permitted in QNodes
 
             if "categories" in slots:
                 categories = slots["categories"]
                 if categories:
                     if not isinstance(categories, List):
                         self.report(code="error.query_graph.node.categories.not_array", identifier=node_id)
                     else:
-                        id_prefix_mapped: Dict = {identifier: False for identifier in ids}
+                        id_prefix_mapped: Dict = {identifier: False for identifier in node_ids}
                         for category in categories:
-                            # category validation may report an error internally
                             category: Optional[ClassDefinition] = \
                                 self.validate_category(
                                     context="query_graph",
                                     node_id=node_id,
                                     category=category
                                 )
+                            # Only 'concrete' (non-abstract, non-mixin, preferably, non-deprecated)
+                            # categories will be tested here for identifier namespaces.  Also, we
+                            # actually don't care if Query Graphs don't have at least one concrete category...
                             if category:
-                                for identifier in ids:  # may be empty list if not provided...
+                                for identifier in node_ids:  # may be empty list if not provided...
                                     possible_subject_categories = self.bmt.get_element_by_prefix(identifier)
                                     if category.name in possible_subject_categories:
                                         id_prefix_mapped[identifier] = True
-                        unmapped_ids = [
-                            identifier for identifier in id_prefix_mapped if not id_prefix_mapped[identifier]
-                        ]
-                        if unmapped_ids:
+                                        node_ids.remove(identifier)
+                                        # found a suitable mapping for the given identifier
+                                        break
+
+                        # At this point, if any 'node_ids' are NOT
+                        # removed (above), then they are unmapped
+                        if has_node_ids and node_ids:
                             self.report(
-                                code="warning.query_graph.node.ids.unmapped_to_categories",
+                                code="warning.query_graph.node.ids.unmapped_prefix",
                                 identifier=node_id,
-                                unmapped_ids=str(unmapped_ids),
+                                unmapped_ids=str(node_ids),
                                 categories=str(categories)
                             )
 
                 # else:  # null "categories" value is permitted in QNodes by nullable: true
             # else:  # missing "categories" key is permitted in QNodes by nullable: true
 
             if 'is_set' in slots:
@@ -236,105 +267,181 @@
 
             # constraints  # TODO: how do we validate node constraints?
             pass
 
     def set_nodes(self, nodes: Set):
         self.nodes.update(nodes)
 
-    def validate_element_status(self, context: str, name: str) -> Optional[Element]:
+    def validate_element_status(self, context: str, identifier: str, edge_id: str) -> Optional[Element]:
         """
         Detect element missing from Biolink, or is deprecated, abstract or mixin, signalled as a failure or warning.
 
-        :param context: parsing context (e.g. 'Node')
-        :param name: name of putative Biolink element ('class')
+        :param context: str, parsing context (e.g. 'Node')
+        :param identifier: str, name of the putative Biolink element ('class')
+        :param edge_id: str, identifier of enclosing edge containing the element (e.g. the 'edge_id')
 
         :return: Optional[Element], Biolink Element resolved to 'name' if element no validation error; None otherwise.
         """
-        element: Optional[Element] = self.bmt.get_element(name)
+        element: Optional[Element] = self.bmt.get_element(identifier)
         if not element:
-            self.report(code=f"error.{context}.unknown", identifier=name)
+            self.report(code=f"error.{context}.unknown", identifier=identifier, edge_id=edge_id)
             return None
+
         if element.deprecated:
-            self.report(code=f"warning.{context}.deprecated", identifier=name)
+            # We won't index the instances where the deprecated element is seen, since we assume that
+            # component developers learning about the issue will globally fix it in their graphs
+            self.report(code=f"warning.{context}.deprecated", identifier=identifier)
             # return None - a deprecated term is not treated as a failure but just as a warning
+
         if element.abstract:
             if self.strict_validation:
-                self.report(code=f"error.{context}.abstract",  identifier=name)
+                self.report(code=f"error.{context}.abstract", identifier=identifier, edge_id=edge_id)
                 return None
             else:
-                self.report(code=f"info.{context}.abstract", identifier=name)
-        elif self.bmt.is_mixin(name):
+                self.report(code=f"info.{context}.abstract", identifier=identifier, edge_id=edge_id)
+
+        elif self.bmt.is_mixin(identifier):
             # A mixin cannot be instantiated ...
             if self.strict_validation:
-                self.report(code=f"error.{context}.mixin", identifier=name)
+                self.report(code=f"error.{context}.mixin", identifier=identifier, edge_id=edge_id)
                 return None
             else:
-                self.report(code=f"info.{context}.mixin", identifier=name)
+                self.report(code=f"info.{context}.mixin", identifier=identifier, edge_id=edge_id)
+
         return element
 
+    def get_target_sources(self) -> Tuple[Optional[str], Optional[str], Optional[str]]:
+        """
+        Returns infores prefix normalized validation caller provided tTarget provenance sources metadata.
+        :return: Tuple[Optional[str], Optional[str], Optional[str]] of ara_source, kp_source, kp_source_type
+        """
+        ara_source: Optional[str] = None
+        kp_source: Optional[str] = None
+        kp_source_type: Optional[str] = None
+        if self.sources:
+            if 'ara_source' in self.sources and self.sources['ara_source']:
+                ara_source: str = self.sources['ara_source']
+                if not ara_source.startswith("infores:"):
+                    ara_source = f"infores:{ara_source}"
+            if 'kp_source' in self.sources and self.sources['kp_source']:
+                kp_source: str = self.sources['kp_source']
+                if not kp_source.startswith("infores:"):
+                    kp_source = f"infores:{kp_source}"
+            kp_source_type = self.sources['kp_source_type'] \
+                if 'kp_source_type' in self.sources and self.sources['kp_source_type'] else 'aggregator'
+            kp_source_type = f"biolink:{kp_source_type}_knowledge_source"
+
+        return ara_source, kp_source, kp_source_type
+
+    def validate_provenance(
+            self,
+            edge_id,
+            ara_source, found_ara_knowledge_source,
+            kp_source, found_kp_knowledge_source, kp_source_type,
+            found_primary_knowledge_source
+    ):
+        """
+        Validates ARA and KP sources based on surveyed Edge slots (in 'attributes' pre-1.4.0; in 'sources', post-1.4.0).
+
+        :param edge_id: str, string identifier for the edge (for reporting purposes)
+        :param ara_source: str, user specified target ARA infores
+        :param found_ara_knowledge_source: bool, True if target ARA infores knowledge source was found
+        :param kp_source: str, user specified target KP infores
+        :param found_kp_knowledge_source:  bool, True if target KP infores knowledge source was found
+        :param kp_source_type:  str, user specified KP knowledge source type (i.e. primary, aggregate, etc.)
+        :param found_primary_knowledge_source: List[str], list of all infores discovered tagged as 'primary'
+        :return:
+        """
+        if ara_source and not found_ara_knowledge_source:
+            # found target ARA knowledge source (if applicable)
+            self.report(
+                code="warning.knowledge_graph.edge.provenance.ara.missing",
+                identifier=ara_source,
+                edge_id=edge_id
+            )
+
+        if kp_source and not found_kp_knowledge_source:
+            # found target KP knowledge source (if applicable)
+            self.report(
+                code="warning.knowledge_graph.edge.provenance.kp.missing",
+                identifier=kp_source,
+                kp_source_type=kp_source_type,
+                identedge_idifier=edge_id
+            )
+
+        if not found_primary_knowledge_source:
+            # Found a primary tagged source...
+            self.report(
+                code="error.knowledge_graph.edge.provenance.missing_primary",
+                identifier=edge_id
+            )
+        elif len(found_primary_knowledge_source) > 1:
+            # ... but only one!
+            self.report(
+                code="warning.knowledge_graph.edge.provenance.multiple_primary",
+                identifier=edge_id,
+                sources=",".join(found_primary_knowledge_source)
+            )
+
     def validate_attributes(self, edge_id: str, edge: Dict):
         """
+        Validate Knowledge Edge Attributes.
+
         :param edge_id: str, string identifier for the edge (for reporting purposes)
         :param edge: Dict, the edge object associated with some attributes are expected to be found
         :return: None (validation messages captured in the 'self' BiolinkValidator context)
         """
+        # we only report errors about missing or empty edge attributes if TRAPI 1.3.0 or earlier,
+        # since earlier TRAPI releases are minimally expected to record provenance attributes
         if 'attributes' not in edge:
-            self.report(code="error.knowledge_graph.edge.attribute.missing", identifier=edge_id)
+            if not self.minimum_required_trapi_version("1.4.0-beta"):
+                self.report(code="error.knowledge_graph.edge.attribute.missing", identifier=edge_id)
         elif not edge['attributes']:
-            self.report(code="error.knowledge_graph.edge.attribute.empty", identifier=edge_id)
+            if not self.minimum_required_trapi_version("1.4.0-beta"):
+                self.report(code="error.knowledge_graph.edge.attribute.empty", identifier=edge_id)
         elif not isinstance(edge['attributes'], List):
             self.report(code="error.knowledge_graph.edge.attribute.not_array", identifier=edge_id)
         else:
             attributes = edge['attributes']
 
-            ara_source: Optional[str] = None
-            kp_source: Optional[str] = None
-            kp_source_type: Optional[str] = None
-            if self.sources:
-                if 'ara_source' in self.sources and self.sources['ara_source']:
-                    ara_source: str = self.sources['ara_source']
-                    if not ara_source.startswith("infores:"):
-                        ara_source = f"infores:{ara_source}"
-                if 'kp_source' in self.sources and self.sources['kp_source']:
-                    kp_source: str = self.sources['kp_source']
-                    if not kp_source.startswith("infores:"):
-                        kp_source = f"infores:{kp_source}"
-                kp_source_type = self.sources['kp_source_type'] \
-                    if 'kp_source_type' in self.sources and self.sources['kp_source_type'] else 'aggregator'
-                kp_source_type = f"biolink:{kp_source_type}_knowledge_source"
+            ara_source: Optional[str]
+            kp_source: Optional[str]
+            kp_source_type: Optional[str]
+            ara_source, kp_source, kp_source_type = self.get_target_sources()
 
             # Expecting ARA and KP 'aggregator_knowledge_source' attributes?
             found_ara_knowledge_source = False
             found_kp_knowledge_source = False
 
             # also track primary_knowledge_source attribute cardinality now
             found_primary_knowledge_source: List[str] = list()
 
             for attribute in attributes:
 
                 # Validate attribute_type_id
                 if 'attribute_type_id' not in attribute:
                     self.report(
                         code="error.knowledge_graph.edge.attribute.type_id.missing",
-                        identifier=str(edge_id)
+                        identifier=edge_id
                     )
                 elif not attribute['attribute_type_id']:
                     self.report(
                         code="error.knowledge_graph.edge.attribute.type_id.empty",
-                        identifier=str(edge_id)
+                        identifier=edge_id
                     )
                 elif 'value' not in attribute:
                     self.report(
                         code="error.knowledge_graph.edge.attribute.value.missing",
-                        identifier=str(edge_id)
+                        identifier=edge_id
                     )
-                elif not attribute['value']:
+                elif not attribute['value'] or \
+                        str(attribute['value']).upper() in ["N/A","NONE","NULL"]:
                     self.report(
                         code="error.knowledge_graph.edge.attribute.value.empty",
-                        identifier=str(edge_id)
+                        identifier=edge_id
                     )
                 else:
                     attribute_type_id: str = attribute['attribute_type_id']
                     value = attribute['value']
 
                     # TODO: there seems to be non-uniformity in provenance attribute values for some KP/ARA's
                     #       in which a value is returned as a Python list (of at least one element?) instead
@@ -342,163 +449,190 @@
                     #       we'll coerce scalar values into a list, then iterate.
                     if not isinstance(value, List):
                         value = [value]
 
                     if not is_curie(attribute_type_id):
                         self.report(
                             code="error.knowledge_graph.edge.attribute.type_id.not_curie",
-                            identifier=str(edge_id),
-                            attribute_type_id=str(attribute_type_id)
+                            identifier=attribute_type_id,
+                            edge_id=edge_id
                         )
                     else:
                         # 'attribute_type_id' is a CURIE, but how well does it map?
                         prefix = attribute_type_id.split(":", 1)[0]
                         if prefix == 'biolink':
                             biolink_class = self.validate_element_status(
                                 context="knowledge_graph.edge.attribute.type_id",
-                                name=attribute_type_id
+                                identifier=attribute_type_id,
+                                edge_id=edge_id
                             )
                             if biolink_class:
                                 if not self.bmt.is_association_slot(attribute_type_id):
                                     self.report(
                                         code="warning.knowledge_graph.edge.attribute.type_id.not_association_slot",
-                                        identifier=str(edge_id),
-                                        attribute_type_id=str(attribute_type_id)
+                                        identifier=attribute_type_id,
+                                        edge_id=edge_id
                                     )
 
                                 else:
                                     # it is a Biolink 'association_slot' but now, validate what kind?
 
                                     # TODO: only check knowledge_source provenance here for now.
                                     #       Are there other association_slots to be validated here too?
 
-                                    # Check Edge Provenance attributes
-                                    if attribute_type_id not in \
-                                            [
-                                                "biolink:aggregator_knowledge_source",
-                                                "biolink:primary_knowledge_source",
-                                                "biolink:original_knowledge_source"
-
-                                            ]:
-
-                                        # TODO: not interested in any other attribute_type_id's at this moment
-                                        continue
-
-                                    # ... now, check the infores values against various expectations
-                                    for infores in value:
-                                        if not infores.startswith("infores:"):
-                                            self.report(
-                                                code="error.knowledge_graph.edge.provenance.infores.missing",
-                                                identifier=str(edge_id),
-                                                infores=str(infores)
-                                            )
-                                        else:
-                                            if attribute_type_id == "biolink:primary_knowledge_source":
-                                                found_primary_knowledge_source.append(infores)
-
-                                            if ara_source and \
-                                                    attribute_type_id == "biolink:aggregator_knowledge_source" and \
-                                                    infores == ara_source:
-                                                found_ara_knowledge_source = True
-                                            elif kp_source and \
-                                                    attribute_type_id == kp_source_type and \
-                                                    infores == kp_source:
-                                                found_kp_knowledge_source = True
+                                    # Edge provenance tags only recorded in Edge attributes prior to TRAPI 1.4.0-beta
+                                    if not self.minimum_required_trapi_version("1.4.0-beta"):
+
+                                        if attribute_type_id not in \
+                                                [
+                                                    "biolink:aggregator_knowledge_source",
+                                                    "biolink:primary_knowledge_source",
+
+                                                    # Note: deprecated since Biolink release 3.0.2
+                                                    #       but this is probably caught above in the
+                                                    #       'validate_element_status' method predicate
+                                                    "biolink:original_knowledge_source"
+
+                                                ]:
+
+                                            # TODO: not interested here in any other
+                                            #       attribute_type_id's at this moment
+                                            continue
+
+                                        # ... now, check the infores values against various expectations
+                                        for infores in value:
+                                            if not infores.startswith("infores:"):
+                                                self.report(
+                                                    code="error.knowledge_graph.edge.provenance.infores.missing",
+                                                    identifier=str(infores),
+                                                    edge_id=edge_id
+                                                )
+                                            else:
+                                                if attribute_type_id == "biolink:primary_knowledge_source":
+                                                    found_primary_knowledge_source.append(infores)
+
+                                                if ara_source and \
+                                                        attribute_type_id == "biolink:aggregator_knowledge_source" and \
+                                                        infores == ara_source:
+                                                    found_ara_knowledge_source = True
+                                                elif kp_source and \
+                                                        attribute_type_id == kp_source_type and \
+                                                        infores == kp_source:
+                                                    found_kp_knowledge_source = True
 
                         # if not a Biolink association_slot, at least,
                         # check if it is an id prefix known to Biolink.
                         # We won't call it a hard error, but issue a warning
                         elif not self.bmt.get_element_by_prefix(prefix):
                             self.report(
                                 code="warning.knowledge_graph.edge.attribute.type_id.unknown_prefix",
-                                identifier=str(edge_id),
-                                attribute_type_id=str(attribute_type_id)
+                                identifier=attribute_type_id,
+                                edge_id=edge_id
                             )
-
+                        # TODO: probably need to take a closer look at validating outlier terms here
+                        #       Maybe enumerations will help
                         else:
                             self.report(
                                 code="info.knowledge_graph.edge.attribute.type_id.non_biolink_prefix",
-                                identifier=str(edge_id),
-                                attribute_type_id=str(attribute_type_id)
+                                identifier=attribute_type_id,
+                                edge_id=edge_id
                             )
 
-            # TODO: After all the attributes have been scanned,
-            #       check for provenance. Treat as warnings for now.
-            if ara_source and not found_ara_knowledge_source:
-                self.report(
-                    code="warning.knowledge_graph.edge.provenance.ara.missing",
-                    identifier=str(edge_id),
-                    ara_source=ara_source
-                )
-
-            if kp_source and not found_kp_knowledge_source:
-                self.report(
-                    code="warning.knowledge_graph.edge.provenance.kp.missing",
-                    identifier=str(edge_id),
-                    kp_source=kp_source,
-                    kp_source_type=kp_source_type
-                )
+            # Edge provenance tags only recorded in Edge attributes prior to TRAPI 1.4.0-beta
+            if not self.minimum_required_trapi_version("1.4.0-beta"):
 
-            if not found_primary_knowledge_source:
-                self.report(
-                    code="error.knowledge_graph.edge.provenance.missing_primary",
-                    identifier=str(edge_id)
-                )
-            elif len(found_primary_knowledge_source) > 1:
-                self.report(
-                    code="warning.knowledge_graph.edge.provenance.multiple_primary",
-                    identifier=str(edge_id),
-                    sources=",".join(found_primary_knowledge_source)
+                # TODO: After all the attributes have been scanned,
+                #       check for provenance. Treat as warnings for now.
+                self.validate_provenance(
+                    edge_id,
+                    ara_source, found_ara_knowledge_source,
+                    kp_source, found_kp_knowledge_source, kp_source_type,
+                    found_primary_knowledge_source
                 )
 
     def validate_attribute_constraints(self, edge_id: str, edge: Dict):
+        """
+        Validate Query Edge Attributes.
+
+        :param edge_id: str, string identifier for the edge (for reporting purposes)
+        :param edge: Dict, the edge object associated with some attributes are expected to be found
+        :return: None (validation messages captured in the 'self' BiolinkValidator context)
+        """
         if 'attribute_constraints' not in edge or edge['attribute_constraints'] is None:
             return  # nullable: true... missing key or None value is ok?
         elif not isinstance(edge['attribute_constraints'], List):
             self.report(code="error.query_graph.edge.attribute_constraints.not_array", identifier=edge_id)
         elif not edge['attribute_constraints']:
             return  # nullable: true... an empty 'attribute_constraints' array is ok?
         else:
             # TODO: not yet sure what else to do here (if anything...yet)
             attribute_constraints: List = edge['attribute_constraints']
 
     def validate_qualifier_entry(self, context: str, edge_id: str, qualifiers: List[Dict[str, str]]):
+        """
+        Validate Qualifier Entry (JSON Object).
+
+        :param context: str, Validation (subcode) context:
+                        - query graph qualifier constraints ("query_graph.edge.qualifier_constraints.qualifier_set") or
+                        - knowledge graph edge qualifiers (knowledge_graph.edge.qualifiers)
+        :param edge_id: str, string identifier for the edge (for reporting purposes)
+        :param qualifiers: List[Dict[str, str]], of qualifier entries to be validated.
+        :return: None (validation messages captured in the 'self' BiolinkValidator context)
+        """
         for qualifier in qualifiers:
             qualifier_type_id: str = qualifier['qualifier_type_id']
             qualifier_value: str = qualifier['qualifier_value']
             try:
                 if not self.bmt.is_qualifier(name=qualifier_type_id):
                     self.report(
                         code=f"error.{context}.qualifier.type_id.unknown",
-                        identifier=edge_id,
-                        qualifier_type_id=qualifier_type_id
+                        identifier=qualifier_type_id,
+                        edge_id=edge_id
                     )
-                elif not self.bmt.validate_qualifier(
-                        # TODO: temporary workaround, parse 'qualifier_type_id' to core name
-                        qualifier_type_id=parse_name(qualifier_type_id),
+                elif qualifier_type_id == "biolink:qualified_predicate":
+                    if not self.bmt.is_predicate(qualifier_value):
+                        # special case of qualifier must have Biolink predicates as values
+                        self.report(
+                            code=f"error.{context}.qualifier.value.not_a_predicate",
+                            identifier=qualifier_value,
+                            edge_id=edge_id
+                        )
+
+                # A Query Graph miss on qualifier_value is less an issue since there may not be enough
+                # context to resolve the 'qualifier_value'; whereas a Knowledge Graph miss is more severe
+                # TODO: however, we somehow need to leverage TRAPI MetaEdge.association metadata here?
+                elif context.startswith("knowledge_graph") and not self.bmt.validate_qualifier(
+                        qualifier_type_id=qualifier_type_id,
                         qualifier_value=qualifier_value
                 ):
                     self.report(
                         code=f"error.{context}.qualifier.value.unresolved",
-                        identifier=edge_id,
-                        qualifier_type_id=qualifier_type_id,
-                        qualifier_value=qualifier_value
+                        identifier=qualifier_value,
+                        edge_id=edge_id,
+                        qualifier_type_id=qualifier_type_id
                     )
-
             except Exception as e:
                 # broad spectrum exception to trap anticipated short term issues with BMT validation
                 logger.error(f"BMT validate_qualifier Exception: {str(e)}")
                 self.report(
                     code=f"error.{context}.qualifier.invalid",
                     identifier=edge_id,
                     qualifier_type_id=qualifier_type_id,
-                    qualifier_value=qualifier_value
+                    qualifier_value=qualifier_value,
+                    reason=str(e)
                 )
 
     def validate_qualifiers(self, edge_id: str, edge: Dict):
+        """
+        Validate Knowledge Edge Qualifiers.
+
+        :param edge_id: str, string identifier for the edge (for reporting purposes)
+        :param edge: Dict, the edge object associated with some attributes are expected to be found
+        :return: None (validation messages captured in the 'self' BiolinkValidator context)
+        """
         # Edge qualifiers will only be seen in Biolink 3 data,
         # but with missing 'qualifiers', no validation is attempted
         if 'qualifiers' not in edge or edge['qualifiers'] is None:
             return  # nullable: true... missing key or None value is ok?
         elif not isinstance(edge['qualifiers'], List):
             self.report(code="error.knowledge_graph.edge.qualifiers.not_array", identifier=edge_id)
         elif not edge['qualifiers']:
@@ -508,14 +642,21 @@
             self.validate_qualifier_entry(
                 context="knowledge_graph.edge.qualifiers",
                 edge_id=edge_id,
                 qualifiers=qualifiers
             )
 
     def validate_qualifier_constraints(self, edge_id: str, edge: Dict):
+        """
+        Validate Query Edge Qualifier Constraints.
+
+        :param edge_id: str, string identifier for the edge (for reporting purposes)
+        :param edge: Dict, the edge object associated with some attributes are expected to be found
+        :return: None (validation messages captured in the 'self' BiolinkValidator context)
+        """
         # Edge qualifiers will only be seen in Biolink 3 data,
         # but with missing 'qualifier_constraints', no validation is attempted
         if 'qualifier_constraints' not in edge or edge['qualifier_constraints'] is None:
             return  # nullable: true... missing key or None value is ok?
         elif not edge['qualifier_constraints']:
             return  # nullable: true... an empty 'qualifier_constraints' array is ok?
         else:
@@ -535,43 +676,184 @@
                     qualifier_set: List = qualifier_set_entry['qualifier_set']
                     self.validate_qualifier_entry(
                         context="query_graph.edge.qualifier_constraints.qualifier_set",
                         edge_id=edge_id,
                         qualifiers=qualifier_set
                     )
 
+    def validate_infores(self, context: str, edge_id: str, identifier: str):
+        code_prefix: str = f"error.knowledge_graph.edge.sources.retrieval_source.{context}.infores"
+        if not is_curie(identifier):
+            self.report(
+                code=f"{code_prefix}.not_curie",
+                identifier=identifier,
+                edge_id=edge_id
+            )
+        elif not identifier.startswith("infores:"):
+            # not sure how absolute the need is for this to be an Infores. We'll be lenient for now?
+            self.report(
+                code=f"{code_prefix}.invalid",
+                identifier=identifier,
+                edge_id=edge_id
+            )
+        # TODO: infores is causing too much instability for now so support has been removed from BMT
+        # TODO: reimplement using YAML version of infores catalog
+        # elif not self.bmt.get_infores_details(identifier):
+        #     # if this method returns 'None' then this is an unregistered infores?
+        #     self.report(
+        #         code=f"{code_prefix}.unknown",
+        #         identifier=identifier,
+        #         edge_id=edge_id
+        #     )
+
+    def validate_sources(self, edge_id: str, edge: Dict):
+        """
+        Validate (TRAPI 1.4.0-beta ++) Edge.sources provenance.
+
+        :param edge_id: str, string identifier for the edge (for reporting purposes)
+        :param edge: Dict, the edge object associated with some attributes are expected to be found
+        :return: None (validation messages captured in the 'self' BiolinkValidator context)
+        """
+        # we ought not to have to test for the absence of the 'sources' tag
+        # if general TRAPI schema validation is run, since it will catch such missing data
+        # however, this method may be directly run on invalid TRAPI data, so...
+        if 'sources' not in edge:
+            self.report(code="error.knowledge_graph.edge.sources.missing", identifier=edge_id)
+        elif not edge['sources']:
+            # Cardinality of 'sources' array is also validated by the TRAPI schema
+            # but for the same reasons noted above, we check again here.
+            self.report(code="error.knowledge_graph.edge.sources.empty", identifier=edge_id)
+        elif not isinstance(edge['sources'], List):
+            self.report(code="error.knowledge_graph.edge.sources.not_array", identifier=edge_id)
+        else:
+            edge_sources = edge['sources']
+
+            # The RetrievalSource items in the 'sources' array is also partially validated insofar as JSONSchema can
+            # validate based on the TRAPI schema; however, some kinds of validation are either not deterministic from
+            # the schema. The remainder of this method validates an initial basic 'semantic' subset of RetrievalSource
+            # content for which the validation is both easy and deemed generally useful. This includes detection of
+            # anticipated Edge provenance roles (i.e. mandatory 'primary' and tests against expected provenance tags)
+
+            # Method caller associated Edge sources to be checked
+
+            ara_source: Optional[str]
+            kp_source: Optional[str]
+            kp_source_type: Optional[str]
+            ara_source, kp_source, kp_source_type = self.get_target_sources()
+
+            # Expecting ARA and KP 'aggregator_knowledge_source' attributes?
+            found_ara_knowledge_source = False
+            found_kp_knowledge_source = False
+
+            # also track primary_knowledge_source attribute cardinality now
+            found_primary_knowledge_source: List[str] = list()
+
+            for retrieval_source in edge_sources:
+
+                # TRAPI schema validation will generally validate the requisite
+                # 'RetrievalSource' entries (i.e. mandatory object keys and valid key value
+                # data types), but here, we go the last (semantic) mile, for the model:
+
+                # 1. 'resource_id': should be a well-formed CURIE which is an Infores which may
+                #    include one of the expected Infores entries (from target sources noted above)
+                if not ("resource_id" in retrieval_source and retrieval_source["resource_id"]):
+                    self.report(
+                        code="error.knowledge_graph.edge.sources.retrieval_source.resource_id.empty",
+                        identifier=edge_id
+                    )
+                    continue
+                elif not ("resource_role" in retrieval_source and retrieval_source["resource_role"]):
+                    # TODO: check if this is ever encountered... maybe TRAPI validation already catches it earlier?
+                    self.report(
+                        code="error.knowledge_graph.edge.sources.retrieval_source.resource_role.empty",
+                        identifier=edge_id
+                    )
+                    continue
+
+                resource_id: str = retrieval_source["resource_id"]
+                resource_role: str = retrieval_source["resource_role"]
+                self. validate_infores(context="resource_id", edge_id=edge_id, identifier=resource_id)
+                if resource_id == ara_source:
+                    found_ara_knowledge_source = True
+                if resource_id == kp_source and resource_role == kp_source_type:
+                    found_kp_knowledge_source = True
+
+                # ... even if the resource_id fails aspects of validation, we'll keep going...
+
+                # 2. 'resource_role': will have already been TRAPI validated, but is at least one
+                #    (but only one?) of 'RetrievalSource' entries the mandatory 'primary'?
+                if resource_id and resource_role == "primary_knowledge_source":
+                    # the cardinality of this will be checked below...
+                    found_primary_knowledge_source.append(resource_id)
+
+                # 3. If provided (Optional), are all 'upstream_resource_ids' well-formed Infores CURIES
+                #    and may include some expected Infores entries (from target sources noted above)?
+                if "upstream_resource_ids" in retrieval_source:
+                    upstream_resource_ids: Optional[List[str]] = retrieval_source["upstream_resource_ids"]
+                    # Note: the TRAPI schema doesn't currently tag this field as nullable, so we check
+                    if upstream_resource_ids:
+                        for identifier in upstream_resource_ids:
+                            self.validate_infores(
+                                context="upstream_resource_ids",
+                                edge_id=edge_id,
+                                identifier=identifier
+                            )
+                            if resource_id == ara_source:
+                                found_ara_knowledge_source = True
+
+                            # we don't worry about kp_source_type here since it is
+                            # not directly annotated with the upstream_resource_ids
+                            if resource_id == kp_source:
+                                found_kp_knowledge_source = True
+
+                # 4. If provided (Optional), we *could* check the optional 'source_record_urls'
+                #    if they are all resolvable URLs (but maybe we do not attempt this for now...)
+                #
+                # if "source_record_urls" in retrieval_source:
+                #     source_record_urls: Optional[List[str]] = retrieval_source["source_record_urls"]
+
+            # TODO: After all the 'sources' RetrievalSource entries have been scanned, then
+            #       perform a complete validation check for complete expected provenance.
+            self.validate_provenance(
+                edge_id,
+                ara_source, found_ara_knowledge_source,
+                kp_source, found_kp_knowledge_source, kp_source_type,
+                found_primary_knowledge_source
+            )
+
     def validate_predicate(self, edge_id: str, predicate: str):
         """
         :param edge_id: identifier of the edge whose predicate is being validated
         :param predicate: putative Biolink Model predicate to be validated
         :return:
         """
         graph_type_context: str = self.graph_type.name.lower()
         if graph_type_context != "input_edge":
             graph_type_context += ".edge"
         context: str = f"{graph_type_context}.predicate"
 
         # Validate the putative predicate as *not* being abstract, deprecated or a mixin
         biolink_class = self.validate_element_status(
             context=context,
-            name=predicate
+            identifier=predicate,
+            edge_id=edge_id
         )
         if biolink_class:
             if not self.bmt.is_predicate(predicate):
                 self.report(
                     code=f"error.{context}.invalid",
-                    identifier=edge_id,
-                    predicate=predicate
+                    identifier=predicate,
+                    edge_id=edge_id
                 )
             elif self.minimum_required_biolink_version("2.2.0") and \
                     not self.bmt.is_translator_canonical_predicate(predicate):
                 self.report(
                     code=f"warning.{context}.non_canonical",
-                    identifier=edge_id,
-                    predicate=predicate
+                    identifier=predicate,
+                    edge_id=edge_id
                 )
 
     def validate_graph_edge(self, edge: Dict):
         """
         Validate slot properties of a relationship ('biolink:Association') edge.
 
         :param edge: dictionary of slot properties of the edge.
@@ -595,16 +877,21 @@
         edge_id = f"{str(subject_id)}--{edge_label}->{str(object_id)}"
 
         context: str = self.graph_type.name.lower()
 
         # Validate Subject node
         if not subject_id:
             self.report(code=f"error.{context}.edge.subject.missing", identifier=edge_id)
+
         elif subject_id not in self.nodes:
-            self.report(code=f"error.{context}.edge.subject.missing_from_nodes", object_id=subject_id)
+            self.report(
+                code=f"error.{context}.edge.subject.missing_from_nodes",
+                identifier=subject_id,
+                edge_id=edge_id
+            )
 
         # Validate Predicates
         if self.graph_type is TRAPIGraphType.Knowledge_Graph:
             if not predicate:
                 self.report(
                     code="error.knowledge_graph.edge.predicate.missing",
                     context=self.graph_type.value,
@@ -627,71 +914,109 @@
                         continue  # sanity check
                     self.validate_predicate(edge_id=edge_id, predicate=predicate)
 
         # Validate Object Node
         if not object_id:
             self.report(code=f"error.{context}.edge.object.missing", identifier=edge_id)
         elif object_id not in self.nodes:
-            self.report(code=f"error.{context}.edge.object.missing_from_nodes", object_id=object_id)
+            self.report(
+                code=f"error.{context}.edge.object.missing_from_nodes",
+                identifier=object_id,
+                edge_id=edge_id
+            )
 
         # Validate edge attributes (or attribute_constraints)
         # and (Biolink 3) edge qualifiers (or qualifier_constraints)
         if self.graph_type is TRAPIGraphType.Knowledge_Graph:
             self.validate_attributes(edge_id=edge_id, edge=edge)
             self.validate_qualifiers(edge_id=edge_id, edge=edge)
+
+            # Edge provenance 'sources' field is only recorded in
+            # Edge attributes, from TRAPI 1.4.0-beta onwards
+            if self.minimum_required_trapi_version("1.4.0-beta"):
+                self.validate_sources(edge_id=edge_id, edge=edge)
         else:
             self.validate_attribute_constraints(edge_id=edge_id, edge=edge)
             self.validate_qualifier_constraints(edge_id=edge_id, edge=edge)
 
     def validate_category(
             self,
             context: str,
             node_id: Optional[str],
             category: Optional[str]
     ) -> ClassDefinition:
         """
         Validate a Biolink category.
 
+        Only returns a non-None value if it is a 'concrete' category, and reports 'unknown' or 'missing'
+        (None or empty string) category names as errors; deprecated categories are reported as warnings;
+        but both 'mixin' and 'abstract' categories are accepted as valid categories silently ignored,
+        but are not considered 'concrete', thus the method returns None.
+
         :param context: str, label for context of concept whose category is being validated, i.e. 'Subject' or 'Object'
         :param node_id: str, CURIE of concept node whose category is being validated
         :param category: str, CURIE of putative concept 'category'
-        :return:
+
+        :return: category as a ClassDefinition, only returned if 'concrete'; None otherwise.
         """
         biolink_class: Optional[ClassDefinition] = None
         if category:
-            # this method reports unknown Biolink Elements
-            biolink_class = self.validate_element_status(
-                    context=f"{context}.node.category",
-                    name=category
-            )
-            if biolink_class and not self.bmt.is_category(category):
-                self.report(code=f"error.{context}.node.category.unknown", identifier=node_id, category=category)
-                biolink_class = None
+            biolink_class = self.bmt.get_element(category)
+            if biolink_class:
+                if biolink_class.deprecated:
+                    self.report(
+                        code=f"warning.{context}.node.category.deprecated",
+                        identifier=category,
+                        node_id=node_id
+                    )
+                if biolink_class.abstract or self.bmt.is_mixin(category):
+                    biolink_class = None
+                elif not self.bmt.is_category(category):
+                    self.report(
+                        code=f"error.{context}.node.category.not_a_category",
+                        identifier=category,
+                        node_id=node_id
+                    )
+                    biolink_class = None
+            else:
+                self.report(
+                    code=f"error.{context}.node.category.unknown",
+                    identifier=category,
+                    node_id=node_id
+                )
         else:
             self.report(code=f"error.{context}.node.category.missing", identifier=node_id)
 
         return biolink_class
 
-    def validate_input_edge_node(self, context: str, node_id: Optional[str], category: Optional[str]):
+    def validate_input_edge_node(self, context: str, node_id: Optional[str], category_name: Optional[str]):
         if node_id:
-            biolink_class: Optional[ClassDefinition] = self.validate_category(
+            category: Optional[ClassDefinition] = self.validate_category(
                 context="input_edge",
                 node_id=node_id,
-                category=category
+                category=category_name
             )
-            if biolink_class:
+            if category:
+                # Since input edges are used in Query Graphs, we ought not to actually
+                # care if they don't have at least one concrete category...However, it
+                # is unlikely for non-concrete classes to resolve to a TRAPI response containing them!
                 possible_subject_categories = self.bmt.get_element_by_prefix(node_id)
-                if biolink_class.name not in possible_subject_categories:
+                if category.name not in possible_subject_categories:
                     self.report(
                         code="warning.input_edge.node.id.unmapped_to_category",
                         context=context,
                         identifier=node_id,
-                        category=category
+                        category=category_name
                     )
-            # else, we will have already reported an error in validate_category()
+            else:
+                self.report(
+                    code="warning.input_edge.node.category.not_concrete",
+                    identifier=node_id,
+                    category=category_name
+                )
         else:
             self.report(code="error.input_edge.node.id.missing", identifier=context)
 
     def check_biolink_model_compliance_of_input_edge(self, edge: Dict[str, str]):
         """
         Validate a templated test input edge contents against the current BMT Biolink Model release.
 
@@ -716,35 +1041,35 @@
         object_curie = edge['object'] if 'object' in edge else None
 
         edge_id = f"{str(subject_curie)}--{predicate}->{str(object_curie)}"
 
         self.validate_input_edge_node(
             context='Subject',
             node_id=subject_curie,
-            category=subject_category_curie
+            category_name=subject_category_curie
         )
         if not predicate:
             self.report(
                 code="error.input_edge.predicate.missing",
                 identifier=edge_id
             )
         else:
             self.validate_predicate(edge_id=edge_id, predicate=predicate)
 
         self.validate_input_edge_node(
             context='Object',
             node_id=object_curie,
-            category=object_category_curie
+            category_name=object_category_curie
         )
 
     def check_biolink_model_compliance(self, graph: Dict):
         """
         Validate a TRAPI-schema compliant Message graph-like data structure
         against the currently active Biolink Model Toolkit model version.
-    
+
         :param graph: knowledge graph to be validated
         :type graph: Dict
         """
         if not graph:
             self.report(code="warning.graph.empty", identifier=self.graph_type.value)
             return  # nothing really more to do here!
 
@@ -799,20 +1124,20 @@
         'subject': 'UBERON:0005453',
         'object': 'UBERON:0035769'
     }
 
     :param edge: basic contents of a templated input edge - S-P-O including concept Biolink Model categories
     :type edge: Dict[str,str]
     :param biolink_version: Biolink Model (SemVer) release against which the knowledge graph is to be
-                            validated (Default: if None, use the Biolink Model Toolkit default version.
+                            validated (Default: if None, use the Biolink Model Toolkit default version).
     :type biolink_version: Optional[str] = None
     :param strict_validation: if True, abstract and mixin elements validate as 'error'; False, issue 'info' message.
     :type strict_validation: bool = False
 
-    :returns: Biolink Model validator cataloging validation messages (may be empty)
+    :returns: Biolink Model validator cataloging validation messages (maybe empty)
     :rtype: BiolinkValidator
     """
     if strict_validation is None:
         # Test Input Edges are like Query Graph data,
         # hence, abstract and mixins ARE permitted
         strict_validation = False
     validator = BiolinkValidator(
@@ -835,65 +1160,73 @@
 
     Since a Query graph is usually an incomplete knowledge graph specification,
     the validation undertaken is not 'strict'
 
     :param graph: query graph to be validated
     :type graph: Dict
     :param biolink_version: Biolink Model (SemVer) release against which the knowledge graph is to be
-                            validated (Default: if None, use the Biolink Model Toolkit default version.
+                            validated (Default: if None, use the Biolink Model Toolkit default version).
     :type biolink_version: Optional[str] = None
     :param strict_validation: if True, abstract and mixin elements validate as 'error'; False, issue 'info' message.
     :type strict_validation: Optional[bool] = None; defaults to 'False' if not set
 
-    :returns: Biolink Model validator cataloging validation messages (may be empty)
+    :returns: Biolink Model validator cataloging validation messages (maybe empty)
     :rtype: BiolinkValidator
     """
     # One typically won't be stringent in QueryGraph validation; however,
     # the strict_validation flag is set to a default of 'False' only if it is NOT set
     if strict_validation is None:
-        # Query Graph data can use abstract and mixins
+        # The default is that abstract and mixins are
+        # allowed in Query Graphs for a TRAPI query
         strict_validation = False
+
     validator = BiolinkValidator(
         graph_type=TRAPIGraphType.Query_Graph,
         biolink_version=biolink_version,
         strict_validation=strict_validation
     )
     validator.check_biolink_model_compliance(graph)
     return validator
 
 
-def check_biolink_model_compliance_of_knowledge_graph(
+def  check_biolink_model_compliance_of_knowledge_graph(
     graph: Dict,
+    trapi_version: Optional[str] = None,
     biolink_version: Optional[str] = None,
     sources: Optional[Dict] = None,
     strict_validation: Optional[bool] = None
 ) -> BiolinkValidator:
     """
-    Strict validation of a TRAPI-schema compliant Message Knowledge Graph
-     against a designated Biolink Model release.
+    Strict validation of a TRAPI-schema compliant Message Knowledge Graph against a designated Biolink Model release.
 
     :param graph: knowledge graph to be validated.
     :type graph: Dict
+    :param trapi_version: TRAPI schema (SemVer) release against which the knowledge graph is to be
+                            validated (Default: if None, use the latest available version).
+    :type trapi_version: Optional[str] = None
     :param biolink_version: Biolink Model (SemVer) release against which the knowledge graph is to be
-                            validated (Default: if None, use the Biolink Model Toolkit default version.
+                            validated (Default: if None, use the Biolink Model Toolkit default version).
     :type biolink_version: Optional[str] = None
     :param sources: Dictionary of validation context identifying the ARA and KP for provenance attribute validation
     :type sources: Dict
     :param strict_validation: if True, abstract and mixin elements validate as 'error'; False, issue 'info' message.
     :type strict_validation: Optional[bool] = None; defaults to 'True' if not set
 
-    :returns: Biolink Model validator cataloging validation messages (may be empty)
+    :returns: Biolink Model validator cataloging validation messages (maybe empty)
     :rtype: BiolinkValidator
     """
     # One typically will want stringent validation for Knowledge Graphs; however,
     # the strict_validation flag is set to a default of 'True' only if it is NOT set
     if strict_validation is None:
-        # Knowledge Graphs generally ought NOT to use abstract and mixins
+        # Knowledge Graphs generally ought NOT to use
+        # abstract and mixins in TRAPI Responses (and Requests)
         strict_validation = True
+
     validator = BiolinkValidator(
         graph_type=TRAPIGraphType.Knowledge_Graph,
+        trapi_version=trapi_version,
         biolink_version=biolink_version,
         sources=sources,
         strict_validation=strict_validation
     )
     validator.check_biolink_model_compliance(graph)
     return validator
```

### Comparing `reasoner_validator-3.4.9/reasoner_validator/sri/util.py` & `reasoner_validator-3.5.0/reasoner_validator/sri/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,45 @@
 import logging
 import re
 from functools import lru_cache
 from json import JSONDecodeError
 from typing import Dict, List, Optional
 
 import requests
-from kgx.prefix_manager import PrefixManager
 
 logger = logging.getLogger(__name__)
 
 # Endpoint for the Translator Normalizer service
 NODE_NORMALIZER_URL = 'https://nodenormalization-sri.renci.org/get_normalized_nodes'
 
 
+@lru_cache()
+def is_curie(s: str) -> bool:
+    """
+    Check if a given string is a CURIE.
+
+    Parameters
+    ----------
+    s: str
+        A string
+
+    Returns
+    -------
+    bool
+        Whether or not the given string is a CURIE
+
+    """
+    if isinstance(s, str):
+        m = re.match(r"^[^ <()>:]*:[^/ :]+$", s)
+        return bool(m)
+    else:
+        return False
+
+
+
 # TODO: not sure to what maxsize for LRU cache
 #       should be set so we just take the default
 @lru_cache()
 def get_aliases(identifier: str):
     """
     Get clique of related identifiers from the Node Normalizer
     """
@@ -30,15 +53,15 @@
     # TODO: maybe check for IRI's here and attempt to translate
     #       (Q: now do we access the prefix map from BMT to do this?)
     # if PrefixManager.is_iri(identifier):
     #     identifier = PrefixManager.contract(identifier)
 
     # We won't raise a RuntimeError for other various
     # erroneous runtime conditions but simply report warnings
-    if not PrefixManager.is_curie(identifier):
+    if not is_curie(identifier):
 
         logging.warning(f"get_aliases(): identifier '{identifier}' is not a CURIE thus cannot resolve its aliases?")
         return list()
 
     # Use the Translator Node Normalizer service to resolve the identifier clique
     response = requests.get(NODE_NORMALIZER_URL, params={'curie': identifier})
```

### Comparing `reasoner_validator-3.4.9/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.5.0/reasoner_validator/trapi/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,27 +6,37 @@
 import jsonschema
 import requests
 
 from yaml import load, CLoader as Loader
 
 from reasoner_validator.report import ValidationReporter
 from reasoner_validator.trapi.mapping import check_node_edge_mappings
-from reasoner_validator.versioning import latest, GIT_ORG, GIT_REPO, branches
+from reasoner_validator.versioning import (
+    SemVer,
+    SemVerError,
+    get_latest_version,
+    GIT_ORG,
+    GIT_REPO,
+    branches
+)
+
+import logging
+logger = logging.getLogger(__name__)
 
 
 @lru_cache()
 def _load_schema(schema_version: str):
     """Load schema from GitHub."""
     result = requests.get(
         f"https://raw.githubusercontent.com/{GIT_ORG}/{GIT_REPO}/{schema_version}/TranslatorReasonerAPI.yaml"
     )
     spec = load(result.text, Loader=Loader)
     components = spec["components"]["schemas"]
     for component, schema in components.items():
-        openapi_to_jsonschema(schema)
+        openapi_to_jsonschema(schema, version=schema_version)
     schemas = dict()
     for component in components:
         # build json schema against which we validate
         subcomponents = copy.deepcopy(components)
         schema = subcomponents.pop(component)
         schema["components"] = {"schemas": subcomponents}
         schemas[component] = schema
@@ -35,21 +45,26 @@
 
 def load_schema(target: str):
     """
     Load schema from GitHub.
     :param target: release semver or git branch name containing the target TRAPI schema.
     :return: loaded TRAPI schema
     """
-    mapped_release = latest.get(target)
+    mapped_release = get_latest_version(target)
     if mapped_release:
-        schema_version = f"v{mapped_release}"  # version tag has 'v' prefix on the release identifier
+        schema_version = mapped_release
     elif target in branches:
+        # cases in which a branch name is
+        # given instead of a release number
         schema_version = target
     else:
-        raise ValueError(f"No TRAPI version {target}")
+        err_msg: str = f"No TRAPI version {target}"
+        logger.error(err_msg)
+        raise ValueError(err_msg)
+
     return _load_schema(schema_version)
 
 
 def fix_nullable(schema) -> None:
     """Fix nullable schema."""
     if "oneOf" in schema:
         schema["oneOf"].append({"type": "null"})
@@ -62,25 +77,46 @@
             key: schema.pop(key)
             for key in list(schema.keys())
         },
         {"type": "null"},
     ]
 
 
-def openapi_to_jsonschema(schema) -> None:
-    """Convert OpenAPI schema to JSON schema."""
-    if "allOf" in schema:
-        # September 1, 2022 hacky patch to rewrite 'allOf' tagged subschemata to 'oneOf'
-        # TODO: TRAPI needs to change this in release 1.4
+def openapi_to_jsonschema(schema, version: str) -> None:
+    """
+    Convert OpenAPI schema to JSON schema.
+    :param schema: Dict, in-memory representation of the OpenAPI schema to be validated.
+    :param version: str, TRAPI version against which the schema is currently being validated.
+    :return:
+    """
+
+    mapped_semver: Optional[SemVer]
+    try:
+        mapped_semver = SemVer.from_string(version)
+    except SemVerError as sve:
+        # if we cannot map the version, then it may simply
+        # be a non-versioned branch of the schemata
+        logger.error(str(sve))
+        mapped_semver = None
+
+    # we'll only tweak mapped schemata and
+    # such releases that are prior to TRAPI 1.4.0-beta
+    if (mapped_semver and not (mapped_semver >= SemVer.from_string("1.4.0-beta"))) \
+            and "allOf" in schema:
+        # September 1, 2022 hacky patch to rewrite 'allOf'
+        # tagged schemata, in TRAPI 1.3.0 or earlier, to 'oneOf'
         schema["oneOf"] = schema.pop("allOf")
+
     if schema.get("type", None) == "object":
         for tag, prop in schema.get("properties", dict()).items():
-            openapi_to_jsonschema(prop)
+            openapi_to_jsonschema(prop, version=version)
+
     if schema.get("type", None) == "array":
-        openapi_to_jsonschema(schema.get("items", dict()))
+        openapi_to_jsonschema(schema.get("items", dict()), version=version)
+
     if schema.pop("nullable", False):
         fix_nullable(schema)
 
 
 class TRAPISchemaValidator(ValidationReporter):
     """
     TRAPI Validator is a wrapper class for validating
@@ -122,14 +158,15 @@
 
         Examples
         --------
         >>> TRAPISchemaValidator(trapi_version="1.3.0").validate({"message": {}}, "QGraph")
 
         """
         schema = load_schema(self.trapi_version)[component]
+        print("instance", instance)
         jsonschema.validate(instance, schema)
 
     def is_valid_trapi_query(self, instance, component: str = "Query"):
         """Make sure that the Message is a syntactically valid TRAPI Query JSON object.
 
         Parameters
         ----------
@@ -148,15 +185,15 @@
         """
         try:
             self.validate(
                 instance=instance,
                 component=component
             )
         except jsonschema.ValidationError as e:
-            self.report(code="error.trapi.validation", identifier=self.trapi_version, exception=e.message)
+            self.report(code="error.trapi.validation", identifier=self.trapi_version, reason=e.message)
 
 
 def check_trapi_validity(instance, trapi_version: str, component: str = "Query") -> TRAPISchemaValidator:
     """
     Checks schema compliance of a Query component against a given TRAPI version.
 
     Parameters
```

### Comparing `reasoner_validator-3.4.9/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.5.0/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.9/reasoner_validator/validation_codes.py` & `reasoner_validator-3.5.0/reasoner_validator/validation_codes.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 
 class CodeDictionary:
 
     CODE_DICTIONARY: str = abspath(join(dirname(__file__), "codes.yaml"))
 
     MESSAGE = "$message"
+    CONTEXT = "$context"
     DESCRIPTION = "$description"
 
     code_dictionary: Optional[Dict] = None
 
     @classmethod
     def _get_code_dictionary(cls) -> Dict:
         if not cls.code_dictionary:
@@ -26,19 +27,21 @@
             with open(cls.CODE_DICTIONARY, mode='r') as f:
                 cls.code_dictionary = load(f, Loader=BaseLoader)
         return cls.code_dictionary
 
     @classmethod
     def filter_copy_by_facet(cls, tree: Dict, facet: str) -> Dict:
         """
-        Copy subtree, filtering out leaf data by specified facet.
+        Copy subtree, filtering out leaf data by specified facet. Leaves are simply identified by
+        the presence of the mandatory '$message' tree parameter dictionary key.
 
         :param tree: Dict, message code dictionary tree to be copied, possibly filtered by facet
         :param facet: str, constraint on code entry facet to be returned; if specified, should be either
-                        "message" or "description" (default: return all facets of the code entry)
+                        "message", "context" or "description" (default: return all facets of the code entry)
+
         :return: Dict, tree filtered by facet
         """
         if facet:
             if cls.MESSAGE in tree:
                 # Terminate recursion; Copy this leaf in the subtree, filtering on the specified 'facet'
                 return {key: value for key, value in tree.items() if key == f"${facet.lower()}"}
             else:
@@ -96,14 +99,20 @@
                 return None
 
             return cls.filter_copy_by_facet(subtree, facet)
 
         else:
             return cls._get_nested_code_entry(subtree, path, pos, facet, is_leaf)
 
+    @staticmethod
+    def get_message_type(code: str) -> str:
+        assert code, "Empty code!"
+        code_path = code.split(".")
+        return code_path[0]
+
     @classmethod
     def get_code_subtree(
             cls,
             code: str,
             facet: Optional[str] = None,
             is_leaf: Optional[bool] = False
     ) -> Optional[Tuple[str, Dict]]:
@@ -111,37 +120,39 @@
         Get subtree of specified dot-delimited tag name, returned with message type (i.e. info, warning, error).
         If optional 'is_leaf' flag is set to True, then only return the code if it is a terminal leaf in the code tree.
 
         :param code: Optional[str], dot delimited validation message code identifier (None is ok, but returns None)
         :param facet: Optional[str], constraint on code entry facet to be returned; if specified, should be either
                                      "message" or "description" (default: return all facets of the code entry)
         :param is_leaf: Optional[bool], only return entry if it is a 'leaf' of the code tree (default: False)
+
         :return: Optional[Tuple[str, Dict[str,str]]], 2-tuple of the code type (i.e. info, warning, error) and the
                  validation message entry (dictionary); None if empty code or code unknown in the code dictionary,
                  or (if the is_leaf option is 'True') if the code doesn't resolve to a single leaf.
         """
         if not code:
             return None
 
         codes: Dict = cls._get_code_dictionary()
         code_path = code.split(".")
         value: Optional[Dict[str, str]] = cls._get_nested_code_entry(codes, code_path, 0, facet, is_leaf)
         if value is not None:
-            return code_path[0], value
+            return cls.get_message_type(code), value
         else:
             return None
 
     @classmethod
     def get_code_entry(cls, code: Optional[str], facet: Optional[str] = None) -> Optional[Dict[str, str]]:
         """
         Get the single code entry corresponding to the given code, if available.
 
         :param code: Optional[str], dot delimited validation message code identifier (None is ok, but returns None)
         :param facet: Optional[str], constraint on code entry facet to be returned; if specified, should be either
                                      "message" or "description" (default: return all facets of the code entry)
+
         :return: Dict, single terminal leaf code entry (complete with indicated or all facets); None, if not available
         """
         value: Optional[Tuple[str, Dict[str, str]]] = cls.get_code_subtree(code, facet=facet, is_leaf=True)
         if not value:
             return None
         entry: Optional[Dict[str, str]]
         message_type, entry = value
@@ -149,93 +160,114 @@
 
     @classmethod
     def get_message_template(cls, code: Optional[str]) -> Optional[str]:
         entry: Optional[Dict[str, str]] = cls.get_code_entry(code)
         return entry[cls.MESSAGE] if entry else None
 
     @classmethod
+    def get_message_context(cls, code: Optional[str]) -> Optional[List[str]]:
+        entry: Optional[Dict[str, str]] = cls.get_code_entry(code)
+        return entry[cls.CONTEXT] if entry else None
+
+    @classmethod
     def get_description(cls, code: Optional[str]) -> Optional[str]:
         entry: Optional[Dict[str, str]] = cls.get_code_entry(code)
         return entry[cls.DESCRIPTION] if entry else None
 
+    @staticmethod
+    def validation_code_tag(code: str) -> str:
+        assert code, "Empty code!"
+        path: List[str] = [part for part in code.replace("_", ".").split(".")]
+        code_parts: List[str] = [part.capitalize() for part in path[1:-1]]
+        tag: str = ' '.join(code_parts) if code_parts else path[-1].capitalize()
+        return tag
+
     @classmethod
     def display(
             cls,
             code: str,  # code for specific validation message template
             parameters: Optional[
                 Dict[
                     str,  # message template 'identifier' key value
                     Optional[
                         List[
                             Dict[str, str]  # dictionary of other template parameters (if present)
                         ]
                     ]
                 ]
-            ] = None
+            ] = None,
+            add_prefix: bool = False
     ) -> List[str]:
         """
         Generate one or more full messages from provided Validation Reporter code
         and associated parameters (if applicable).
 
-        :param code: str, valid (dot delimited YAML key path) identified code,
-                     which should be registered in the project codes.yaml file.
+        :param code: str,  valid (dot delimited YAML key path) identified code,
+                           which should be registered in the project codes.yaml file.
         :param parameters: Optional[Dict[str, Optional[List[Dict[str, str]]]]], collection of all
                            message parameters dictionaries associated with list of messages of the given code,
                            indexed by their unique 'identifier' template field (note: all messages with
                            one or more template parameters are expected to have an 'identifier' parameter,
                            the values for which corresponding to the keys of the dictionary. The value of those
                            keys are either 'None' if the identifier is the only template parameter, or alternately,
                            a list of dictionaries containing all the other expected parameters keys and their values
                            for every distinct message).
+        :param add_prefix: bool, flag to prepend a prefix for the message type
+                           (i.e. error, warning, info) to displayed messages (default: False)
+
         :return: List[str], list of decoded messages
         """
         value: Optional[Tuple[str, Dict[str, str]]] = cls.get_code_subtree(code, is_leaf=True)
         assert value, f"CodeDictionary.display(): unknown message code {code}"
-        message_type, entry = value
-        code_parts: List[str] = [part.capitalize() for part in code.replace("_", ".").split(".")[1:-1]]
-        context: str = ' '.join(code_parts) + ': ' if code_parts else ''
-        template: str = entry[cls.MESSAGE]
+
+        message_type = cls.get_message_type(code)
+        message_type_prefix: str = f"{message_type.upper()} - " if add_prefix else ""
+        context: str = cls.validation_code_tag(code) + ": " if add_prefix else ""
+
+        template: str = cls.get_message_template(code)
+
         if parameters:
             # Message template parameterized with one or more sets of additional
             # named message parameters, assumed to be referenced by the template
             message_list: List = list()
             for identifier in parameters.keys():
                 other_parameters: Optional[List[Dict[str, str]]] = parameters[identifier]
                 identifier_dict: Dict = {'identifier': identifier}
                 if other_parameters:
                     # is a list of one or more dictionaries of additional parameters
                     for another_parameter_dict in other_parameters:
                         # make copies, to be safe...
                         content: Dict = identifier_dict.copy()
                         content.update(another_parameter_dict)
                         message_list.append(
-                            f"{message_type.upper()} - "
-                            f"{context}{template.format(**content)}"
+                            f"{message_type_prefix}{context}{template.format(**content)}"
                         )
                 else:
                     message_list.append(
-                        f"{message_type.upper()} - "
-                        f"{context}{template.format(**identifier_dict)}"
+                        f"{message_type_prefix}{context}{template.format(**identifier_dict)}"
                     )
             return message_list
         else:
             # simple scalar message without parameterization?
-            return [f"{message_type.upper()} - {context}{template}"]
+            return [f"{message_type_prefix}{context}{template}"]
 
     @classmethod
     def _dump_code_markdown_entries(cls, root: str, code_subtree: Dict, markdown_file):
         for tag, value in code_subtree.items():
             if cls.MESSAGE not in value:
                 # Recurse down to leaf of tree
                 cls._dump_code_markdown_entries(f"{root}.{tag}", value, markdown_file)
             else:
                 print(f"### {root}.{tag}\n", file=markdown_file)
                 message: str = value[cls.MESSAGE]
+                context: str = value[cls.CONTEXT] if cls.CONTEXT in value else None
                 description: str = value[cls.DESCRIPTION] if cls.DESCRIPTION in value else None
                 print(f"**Message:** {message}\n", file=markdown_file)
+                if context:
+                    print(f"**Context:** {', '.join(context)}\n", file=markdown_file)
                 if description:
                     print(f"**Description:** {description}\n", file=markdown_file)
 
     @classmethod
     def markdown(cls, filename: str = DEFAULT_CODES_DOCUMENTATION_FILE) -> bool:
         """Dump the Code Dictionary into a validation_codes_dictionary.md Markdown file, for documentation purposes.
```

### Comparing `reasoner_validator-3.4.9/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.5.0/tests/test_biolink_compliance_validation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Unit tests for the generic (shared) components of the SRI Testing Framework
 """
 from typing import Tuple, Optional, Dict
 from sys import stderr
-import copy
+from copy import deepcopy
 from pprint import PrettyPrinter
 import logging
 import pytest
 from bmt import Toolkit
 from linkml_runtime.linkml_model import SlotDefinition
 
 from reasoner_validator import TRAPISchemaValidator
@@ -22,19 +22,17 @@
 from tests.test_validation_report import check_messages
 
 logger = logging.getLogger(__name__)
 logger.setLevel("DEBUG")
 
 pp = PrettyPrinter(indent=4)
 
-# TRAPI 1.4 is still a work-in-progress as of February 2023, so we stay with 1.3 for now(?)
-LATEST_TRAPI_VERSION = "1.3"
-
-# January 25, 2023 - as of reasoner-validator 3.1.0, we don't pretend to totally support Biolink Models
-# any earlier than 3.1.1.  If earlier biolink model compliance testing is desired,
+# January 25, 2023 - as of reasoner-validator 3.1.0,
+# we don't pretend to totally support Biolink Models any earlier than 3.1.1.
+# If earlier biolink model compliance testing is desired,
 # then perhaps reasoner-validator version 3.0.5 or earlier can be used.
 LATEST_BIOLINK_MODEL_VERSION = "3.2.0"
 
 
 def test_set_default_biolink_versioned_global_environment():
     validator = BiolinkValidator(graph_type=TRAPIGraphType.Knowledge_Graph)
     model_version = validator.get_biolink_version()
@@ -311,37 +309,35 @@
         #         'predicate': 'biolink:physically_interacts_with',
         #         'subject': 'CHEBI:27300',
         #         'object': 'Orphanet:120464'
         #     },
         #     # f"{INPUT_EDGE_PREFIX}: WARNING - Subject 'biolink:Nutrient' is deprecated?"
         #     "warning.input_edge.node.category.deprecated"
         # ),
-        (   # Query 18 - inform that the input category is a mixin?
+        (   # Query 18 - Issue a warning for input_edge data with a category that is a mixin?
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:GeneOrGeneProduct',
                 'object_category': 'biolink:Protein',
                 'predicate': 'biolink:related_to',
                 'subject': 'HGNC:9604',
                 'object': 'UniProtKB:P23219'
             },
-            # f"{INPUT_EDGE_PREFIX}: INFO - Subject element 'biolink:GeneOrGeneProduct' is a mixin."
-            "info.input_edge.node.category.mixin"
+            "warning.input_edge.node.category.not_concrete"
         ),
-        (   # Query 19 - inform that the input category is abstract?
+        (   # Query 19 - Issue a warning for input_edge data with a category that is abstract?
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:AdministrativeEntity',
                 'object_category': 'biolink:Agent',
                 'predicate': 'biolink:related_to',
                 'subject': 'isbn:1234',
                 'object': 'ORCID:1234'
             },
-            # f"{INPUT_EDGE_PREFIX}: INFO - Subject element 'biolink:AdministrativeEntity' is abstract."
-            "info.input_edge.node.category.abstract"
+            "warning.input_edge.node.category.not_concrete"
         )
     ]
 )
 def test_check_biolink_model_compliance_of_input_edge(query: Tuple):
     validator: BiolinkValidator = check_biolink_model_compliance_of_input_edge(edge=query[1], biolink_version=query[0])
     check_messages(validator, query[2])
 
@@ -712,19 +708,19 @@
                         "predicates": ["biolink:treats"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
             # f"{QUERY_GRAPH_PREFIX}: WARNING - Node 'type-2 diabetes' has identifiers ['FOO:12345', 'BAR:67890'] " +
             # "unmapped to the target categories: ['biolink:Disease', 'biolink:Gene']?"
-            "warning.query_graph.node.ids.unmapped_to_categories"
+            "warning.query_graph.node.ids.unmapped_prefix"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 21: Abstract category in query graph
+            # Query 21: Abstract category in query graph? Simply ignored now during validation...
             {
                 "nodes": {
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                     "drug": {
                         "categories": ["biolink:BiologicalEntity"]
                     }
                 },
@@ -732,20 +728,19 @@
                     "treats": {
                         "subject": "drug",
                         "predicates": ["biolink:treats"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
-            # f"{QUERY_GRAPH_PREFIX}: INFO - Query Graph Node element 'biolink:BiologicalEntity' is abstract."
-            "info.query_graph.node.category.abstract"
+            ""
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 22: Mixin category in query graph
+            # Query 22: Mixin category in query graph? Simply ignored now during validation...
             {
                 "nodes": {
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                     "drug": {
                         "categories": ["biolink:ChemicalOrDrugOrTreatment"]
                     }
                 },
@@ -753,16 +748,15 @@
                     "treats": {
                         "subject": "drug",
                         "predicates": ["biolink:treats"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
-            # f"{QUERY_GRAPH_PREFIX}: INFO - Query Graph Node element 'biolink:ChemicalOrDrugOrTreatment' is a mixin."
-            "info.query_graph.node.category.mixin"
+            ""
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
             # Query 23: Query edge predicate is a mixin
             {
                 "nodes": {
                     "IRS1": {"ids": ["HGNC:6125"], "categories": ["biolink:Gene"]},
@@ -854,184 +848,282 @@
             {
                 "attributes": []
             },
             get_ara_test_case(),
             # "Edge has empty attributes!"
             "error.knowledge_graph.edge.attribute.empty"
         ),
+    ]
+)
+def test_pre_trapi_1_4_0_validate_missing_or_empty_attributes(query: Tuple):
+    validator = BiolinkValidator(
+        graph_type=TRAPIGraphType.Knowledge_Graph,
+        trapi_version="1.3.0",
+        biolink_version=LATEST_BIOLINK_MODEL_VERSION,
+        sources=query[1]
+    )
+    validator.validate_attributes(edge_id="test_validate_attributes unit test", edge=query[0])
+    check_messages(validator, query[2])
+
+
+@pytest.mark.parametrize(
+    "query",
+    [
+        # These tests should all pass in TRAPI releases >= 1.4.0-beta
+        # (
+        #         "mock_edge",  # mock data has dumb edges: don't worry about the S-P-O, just the attributes
+        #         "mock_context",
+        #         "AssertError_message"
+        # ),   # set 3rd argument to AssertError message if test edge should 'fail'; otherwise, empty string (for pass)
         (
-            # Query 3. Empty attributes
-            {
-                "attributes": {"not_a_list"}
-            },
+            # Query 0. 'attributes' key missing in edge record is None
+            {},
             get_ara_test_case(),
-            # "Edge attributes are not an array!"
-            "error.knowledge_graph.edge.attribute.not_array"
+            # "Edge has no 'attributes' key!"
+            ""
         ),
         (
-            # Query 4. attribute missing its 'attribute_type_id' field
+            # Query 1. Empty attributes
             {
-                "attributes": [
-                    {"value": ""}
-                ]
+                "attributes": None
             },
             get_ara_test_case(),
-            # "Edge attribute missing its 'attribute_type_id' property!"
-            "error.knowledge_graph.edge.attribute.type_id.missing"
+            # "Edge has empty attributes!"
+            ""
         ),
         (
-            # Query 5. attribute missing its 'value' field
+            # Query 2. Empty attributes
             {
-                "attributes": [
-                    {"attribute_type_id": "biolink:p_value"}
-                ]
+                "attributes": []
             },
             get_ara_test_case(),
-            # "Edge attribute missing its 'value' property!"
-            "error.knowledge_graph.edge.attribute.value.missing"
+            # "Edge has empty attributes!"
+            ""
         ),
+    ]
+)
+def test_post_1_4_0_trapi_validate_missing_or_empty_attributes(query: Tuple):
+    validator = BiolinkValidator(
+        graph_type=TRAPIGraphType.Knowledge_Graph,
+        biolink_version=LATEST_BIOLINK_MODEL_VERSION,
+        sources=query[1]
+    )
+    validator.validate_attributes(edge_id="test_validate_attributes unit test", edge=query[0])
+    check_messages(validator, query[2])
+
+
+@pytest.mark.parametrize(
+    "query",
+    [
         (
-            # Query 6. Missing ARA knowledge source provenance?
+            # Query 0. Missing ARA knowledge source provenance?
             {
                 "attributes": [
                     {
                         "attribute_type_id": "biolink:aggregator_knowledge_source",
                         "value": "infores:sri-reference-kg"
                     },
                 ]
             },
             get_ara_test_case(),
             # "missing ARA knowledge source provenance!"
             "warning.knowledge_graph.edge.provenance.ara.missing"
         ),
         (
-            # Query 7. value is an empty list?
+            # Query 1. KP provenance value is not a well-formed InfoRes CURIE? Should fail?
             {
                 "attributes": [
                     {
                         "attribute_type_id": "biolink:aggregator_knowledge_source",
-                        "value": []
+                        "value": "infores:aragorn"
                     },
+                    {
+                        "attribute_type_id": "biolink:primary_knowledge_source",
+                        "value": "panther"
+                    }
                 ]
             },
             get_ara_test_case(),
-            # "value is an empty list!"
-            "error.knowledge_graph.edge.attribute.value.empty"
+            # "Edge has provenance value '{infores}' which is not a well-formed InfoRes CURIE!"
+            "error.knowledge_graph.edge.provenance.infores.missing"
         ),
         (
-            # Query 8. KP provenance value is not a well-formed InfoRes CURIE? Should fail?
+            # Query 2. KP provenance value is missing?
             {
                 "attributes": [
                     {
                         "attribute_type_id": "biolink:aggregator_knowledge_source",
                         "value": "infores:aragorn"
-                    },
+                    }
+                ]
+            },
+            get_ara_test_case(),
+            # "is missing as expected knowledge source provenance!"
+            "warning.knowledge_graph.edge.provenance.kp.missing"
+        ),
+        (
+            # Query 3. Missing 'primary' nor 'original' knowledge source
+            {
+                "attributes": [
                     {
-                        "attribute_type_id": "biolink:primary_knowledge_source",
-                        "value": "infores:panther"
+                        "attribute_type_id": "biolink:aggregator_knowledge_source",
+                        "value": "infores:aragorn"
                     },
                     {
-                        "attribute_type_id": "non_a_curie",
-                        "value": "something"
+                        "attribute_type_id": "biolink:aggregator_knowledge_source",
+                        "value": "infores:panther"
                     }
                 ]
+
+            },
+            get_ara_test_case({"kp_source_type": "aggregator"}),
+            # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Edge has neither a 'primary' nor 'original' knowledge source?"
+            "error.knowledge_graph.edge.provenance.missing_primary"
+        )
+    ]
+)
+def test_pre_1_4_0_validate_provenance(query: Tuple):
+    """TRAPI pre-1.4.0 releases recorded provenance in attributes. This unit test checks for this"""
+    validator = BiolinkValidator(
+        graph_type=TRAPIGraphType.Knowledge_Graph,
+        trapi_version="1.3.0",
+        biolink_version=LATEST_BIOLINK_MODEL_VERSION,
+        sources=query[1]
+    )
+    validator.validate_attributes(edge_id="test_validate_attributes unit test", edge=query[0])
+    check_messages(validator, query[2])
+
+
+@pytest.mark.parametrize(
+    "query",
+    [
+        (
+            # Query 0. Attributes are not a proper array
+            {
+                "attributes": {"not_a_list"}
+            },
+            get_ara_test_case(),
+            # "Edge attributes are not an array!"
+            "error.knowledge_graph.edge.attribute.not_array"
+        ),
+        (
+            # Query 1. attribute missing its 'attribute_type_id' field
+            {
+                "attributes": [
+                    {"value": ""}
+                ]
             },
             get_ara_test_case(),
-            # "is not a well-formed CURIE!"
-            "error.knowledge_graph.edge.attribute.type_id.not_curie"
+            # "Edge attribute missing its 'attribute_type_id' property!"
+            "error.knowledge_graph.edge.attribute.type_id.missing"
+        ),
+        (
+            # Query 2. attribute missing its 'value' field
+            {
+                "attributes": [
+                    {"attribute_type_id": "biolink:p_value"}
+                ]
+            },
+            get_ara_test_case(),
+            # "Edge attribute missing its 'value' property!"
+            "error.knowledge_graph.edge.attribute.value.missing"
         ),
         (
-            # Query 9. KP provenance value is not a well-formed InfoRes CURIE? Should fail?
+            # Query 3. value is an empty list?
             {
                 "attributes": [
                     {
                         "attribute_type_id": "biolink:aggregator_knowledge_source",
-                        "value": "infores:aragorn"
+                        "value": []
                     },
+                ]
+            },
+            get_ara_test_case(),
+            "error.knowledge_graph.edge.attribute.value.empty"
+        ),
+        (
+            # Query 4. value is the string "null"?
+            {
+                "attributes": [
                     {
-                        "attribute_type_id": "biolink:primary_knowledge_source",
-                        "value": "panther"
-                    }
+                        "attribute_type_id": "biolink:aggregator_knowledge_source",
+                        "value": "null"
+                    },
                 ]
             },
             get_ara_test_case(),
-            # "Edge has provenance value '{infores}' which is not a well-formed InfoRes CURIE!"
-            "error.knowledge_graph.edge.provenance.infores.missing"
+            "error.knowledge_graph.edge.attribute.value.empty"
         ),
         (
-            # Query 10. KP provenance value is missing?
+            # Query 5. value is the string "N/A"?
             {
                 "attributes": [
                     {
                         "attribute_type_id": "biolink:aggregator_knowledge_source",
-                        "value": "infores:aragorn"
-                    }
+                        "value": "N/A"
+                    },
                 ]
             },
             get_ara_test_case(),
-            # "is missing as expected knowledge source provenance!"
-            "warning.knowledge_graph.edge.provenance.kp.missing"
+            "error.knowledge_graph.edge.attribute.value.empty"
+        ),
+        (
+            # Query 6. value is the string "None"
+            {
+                "attributes": [
+                    {
+                        "attribute_type_id": "biolink:aggregator_knowledge_source",
+                        "value": "None"
+                    },
+                ]
+            },
+            get_ara_test_case(),
+            "error.knowledge_graph.edge.attribute.value.empty"
         ),
-        # (   # No longer present in Biolink 3.1.1
-        #     # Query xx. kp type is 'original'. Should draw a WARNING about deprecation
-        #     {
-        #         "attributes": [
-        #             {
-        #                 "attribute_type_id": "biolink:aggregator_knowledge_source",
-        #                 "value": "infores:aragorn"
-        #             },
-        #             {
-        #                 "attribute_type_id": "biolink:original_knowledge_source",
-        #                 "value": "infores:panther"
-        #             }
-        #         ]
-        #     },
-        #     get_ara_test_case(),
-        #     # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Attribute Type ID element " +
-        #     # "'biolink:original_knowledge_source' is deprecated?"
-        #     "warning.knowledge_graph.attribute.type_id.deprecated"
-        # ),
         (
-            # Query 11. kp type is 'primary'. Should pass?
+            # Query 7. KP provenance value is not a well-formed InfoRes CURIE? Should fail?
             {
                 "attributes": [
                     {
                         "attribute_type_id": "biolink:aggregator_knowledge_source",
                         "value": "infores:aragorn"
                     },
                     {
                         "attribute_type_id": "biolink:primary_knowledge_source",
                         "value": "infores:panther"
+                    },
+                    {
+                        "attribute_type_id": "non_a_curie",
+                        "value": "something"
                     }
                 ]
             },
             get_ara_test_case(),
-            ""
+            # "is not a well-formed CURIE!"
+            "error.knowledge_graph.edge.attribute.type_id.not_curie"
         ),
         (
-            # Query 12. Missing 'primary' nor 'original' knowledge source
+            # Query 8. kp type is 'primary'. Should pass?
             {
                 "attributes": [
                     {
                         "attribute_type_id": "biolink:aggregator_knowledge_source",
                         "value": "infores:aragorn"
                     },
                     {
-                        "attribute_type_id": "biolink:aggregator_knowledge_source",
+                        "attribute_type_id": "biolink:primary_knowledge_source",
                         "value": "infores:panther"
                     }
                 ]
-
             },
-            get_ara_test_case({"kp_source_type": "aggregator"}),
-            # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Edge has neither a 'primary' nor 'original' knowledge source?"
-            "error.knowledge_graph.edge.provenance.missing_primary"
+            get_ara_test_case(),
+            ""
         ),
         (
-            # Query 13. Is complete and should pass?
+            # Query 9. Is complete and should pass?
             {
                 "attributes": [
                     {
                         "attribute_type_id": "biolink:aggregator_knowledge_source",
                         "value": "infores:aragorn"
                     },
                     {
@@ -1045,38 +1137,59 @@
                 ]
             },
             get_ara_test_case({"kp_source_type": "aggregator"}),
             ""
         )
     ]
 )
-def test_validate_attributes(query: Tuple):
+def test_latest_validate_attributes(query: Tuple):
     validator = BiolinkValidator(
         graph_type=TRAPIGraphType.Knowledge_Graph,
+        # trapi_version="latest",
         biolink_version=LATEST_BIOLINK_MODEL_VERSION,
         sources=query[1]
     )
     validator.validate_attributes(edge_id="test_validate_attributes unit test", edge=query[0])
     check_messages(validator, query[2])
 
 
-def qualifier_validator(tested_method, edge_model: str, query: Tuple[Dict, str]):
+def qualifier_validator(
+        tested_method,
+        edge_model: str,
+        query: Tuple[Dict, str],
+        trapi_version: Optional[str] = None
+):
+    # TODO: to review: which of the validation tests that may be overridden by earlier TRAPI validation
     # Sanity check: does TRAPI validation catch this first?
-    trapi_validator = TRAPISchemaValidator(trapi_version=LATEST_TRAPI_VERSION)
+    trapi_validator = TRAPISchemaValidator(trapi_version=trapi_version)
     # Wrap Qualifiers inside a small mock QEdge
-    mock_edge: Dict = copy.deepcopy(query[0])
+    mock_edge: Dict = deepcopy(query[0])
     mock_edge["subject"] = "mock_subject"
+
+    if trapi_validator.minimum_required_trapi_version("1.4.0-beta"):
+        # not testing Edge semantics here but rather, the qualifiers,
+        # but from 1.4.0-beta(2) onwards, we also need
+        # a non-null predicate and the new 'sources' field here!
+        mock_edge["predicate"] = "biolink:related_to"
+        mock_edge["sources"] = [
+            {
+                "resource_id": "infores:molepro",
+                "resource_role": "primary_knowledge_source"
+            }
+        ]
+
     mock_edge["object"] = "mock_object"
     trapi_validator.is_valid_trapi_query(mock_edge, edge_model)
     if trapi_validator.has_errors():
         validator = trapi_validator
     else:
         # if you get this far,then attempt additional Biolink Validation
         validator = BiolinkValidator(
             graph_type=TRAPIGraphType.Query_Graph,
+            trapi_version=trapi_version,
             biolink_version=LATEST_BIOLINK_MODEL_VERSION
         )
         tested_method(
             validator,
             edge_id=f"{tested_method.__name__} unit test",
             edge=query[0]
         )
@@ -1185,90 +1298,74 @@
                             }
                         ]
                     }
                 ]
             },
             "error.trapi.validation"
         ),
-        (  # Query 12 - 'qualifier_type_id' property value is not a Biolink CURIE
-            {
-                'qualifier_constraints': [
-                    {
-                        "qualifier_set": [
-                            {
-                                'qualifier_type_id': "not-a-curie",
-                                'qualifier_value': "fake-qualifier-value"
-                            }
-                        ]
-                    }
-                ]
-            },
-            "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.type_id.unknown"
-        ),
-        (  # Query 13 - 'qualifier_type_id' property value is unknown
+        (  # Query 12 - 'qualifier_type_id' property value is unknown
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
                             {
                                 'qualifier_type_id': "biolink:unknown_qualifier",
                                 'qualifier_value': "fake-qualifier-value"
                             }
                         ]
                     }
                 ]
             },
             "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.type_id.unknown"
         ),
-        (  # Query 14 - 'qualifier_type_id' property value is valid but abstract
+        (  # Query 13 - 'qualifier_type_id' property value is valid but abstract
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
                             {
                                 'qualifier_type_id': "biolink:aspect_qualifier",
                                 'qualifier_value': "stability"
                             }
                         ]
                     }
                 ]
             },
-            # "info.query_graph.edge.qualifier.abstract"
-            "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.value.unresolved"
+            ""  # this will pass here since Query Graphs are allowed to have abstract qualifiers?
         ),
-        (  # Query 15 - 'qualifier_type_id' property value is not a Biolink qualifier term
+        (  # Query 14 - 'qualifier_type_id' property value is not a Biolink qualifier term
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
                             {
                                 'qualifier_type_id': "biolink:related_to",
                                 'qualifier_value': "fake-qualifier-value"
                             }
                         ]
                     }
                 ]
             },
             "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.type_id.unknown"
         ),
-        (  # Query 16 - 'qualifier' entry is missing its 'qualifier_value' property - invalidated by TRAPI schema
+        (  # Query 15 - 'qualifier' entry is missing its 'qualifier_value' property - invalidated by TRAPI schema
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
                             {
                                 'qualifier_type_id': "biolink:object_direction_qualifier"
                             }
                         ]
                     }
                 ]
             },
             "error.trapi.validation"
         ),
-        (   # Query 17 - qualifier_type_id 'object_direction_qualifier' is a valid Biolink qualifier type and
+        (   # Query 16 - qualifier_type_id 'object_direction_qualifier' is a valid Biolink qualifier type and
             #            'upregulated' a valid corresponding 'permissible value' enum 'qualifier_value'
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
                             {
                                 'qualifier_type_id': "biolink:object_direction_qualifier",
@@ -1293,40 +1390,95 @@
         #                     }
         #                 ]
         #             }
         #         ]
         #     },
         #     ""    # this other use case should also pass
         # ),
-        (   # Query 18 - 'qualifier_type_id' is a valid Biolink qualifier type and
-            #             'UBERON:0001981' a valid corresponding 'reachable from' enum 'qualifier_value'
+        (   # Query 18 - 'qualifier_type_id' is the special qualifier case 'biolink:qualified_predicate'
+            #            with a Biolink predicate as its value
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
                             {
-                                'qualifier_type_id': "biolink:anatomical_context_qualifier",
-                                'qualifier_value': "UBERON:0001981"  # Blood Vessel
+                                'qualifier_type_id': "biolink:qualified_predicate",
+                                'qualifier_value': "biolink:causes"
                             }
                         ]
                     }
                 ]
             },
-            ""    # this particular use case should also pass
+            ""  # this particular use case should also pass
+        ),
+        (   # Query 19 - 'qualifier_type_id' is the special qualifier case 'biolink:qualified_predicate'
+            #            an incorrect value, which is not a Biolink predicate
+            {
+                'qualifier_constraints': [
+                    {
+                        "qualifier_set": [
+                            {
+                                'qualifier_type_id': "biolink:qualified_predicate",
+                                'qualifier_value': "biolink:Association"
+                            }
+                        ]
+                    }
+                ]
+            },
+            "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.value.not_a_predicate"
         )
     ]
 )
 def test_validate_qualifier_constraints(query: Tuple[Dict, str]):
+    # TODO: to review: which of the validation tests that may be overridden by earlier TRAPI validation
     qualifier_validator(
         tested_method=BiolinkValidator.validate_qualifier_constraints,
         edge_model="QEdge",
         query=query
     )
 
 
+QC_QS_NOT_A_CURIE = {
+    'qualifier_constraints': [
+        {
+            "qualifier_set": [
+                {
+                    'qualifier_type_id': "not-a-curie",
+                    'qualifier_value': "fake-qualifier-value"
+                }
+            ]
+        }
+    ]
+}
+
+
+@pytest.mark.parametrize(
+    "query",
+    [
+        (  # Query 0 - 'qualifier_type_id' value not a Biolink CURIE - seen as 'unknown' in TRAPI < 1.4.0-beta
+            "1.3.0",
+            QC_QS_NOT_A_CURIE,
+            "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.type_id.unknown"
+        ),
+        (  # Query 1 - 'qualifier_type_id' value not a Biolink CURIE - schema validation error in TRAPI < 1.4.0-beta
+            "1.4.0-beta",
+            QC_QS_NOT_A_CURIE,
+            "error.trapi.validation"
+        )
+    ]
+)
+def test_validate_biolink_curie_in_qualifier_constraints(query: Tuple[str, Dict, str]):
+    qualifier_validator(
+        tested_method=BiolinkValidator.validate_qualifier_constraints,
+        edge_model="QEdge",
+        query=query[1:],
+        trapi_version=query[0]
+    )
+
+
 @pytest.mark.parametrize(
     "query",
     [
         (  # Query 0 - no 'qualifiers' key - since nullable: true, this should pass
             {},
             ""
         ),
@@ -1367,116 +1519,131 @@
                         # 'qualifier_type_id': "",
                         'qualifier_value': ""
                     }
                 ]
             },
             "error.trapi.validation"
         ),
-        (  # Query 7 - 'qualifier_type_id' property value is not a Biolink CURIE
-            {
-                'qualifiers': [
-                    {
-                        'qualifier_type_id': "not-a-curie",
-                        'qualifier_value': "fake-qualifier-value"
-                    }
-                ]
-            },
-            "error.knowledge_graph.edge.qualifiers.qualifier.type_id.unknown"
-        ),
-        (  # Query 8 - 'qualifier_type_id' property value is unknown
+        (  # Query 7 - 'qualifier_type_id' property value is unknown
             {
                 'qualifiers': [
                     {
                         'qualifier_type_id': "biolink:unknown_qualifier",
                         'qualifier_value': "fake-qualifier-value"
                     }
                 ]
             },
             "error.knowledge_graph.edge.qualifiers.qualifier.type_id.unknown"
         ),
-        (  # Query 9 - 'qualifier_type_id' property value is valid but abstract
+        (  # Query 8 - 'qualifier_type_id' property value is valid but abstract
             {
                 'qualifiers': [
                     {
                         'qualifier_type_id': "biolink:aspect_qualifier",
                         'qualifier_value': "stability"
                     }
                 ]
             },
             # "info.query_graph.edge.qualifier.abstract"
             "error.knowledge_graph.edge.qualifiers.qualifier.value.unresolved"
         ),
-        (  # Query 10 - 'qualifier_type_id' property value is not a Biolink qualifier term
+        (  # Query 9 - 'qualifier_type_id' property value is not a Biolink qualifier term
             {
                 'qualifiers': [
                     {
                         'qualifier_type_id': "biolink:related_to",
                         'qualifier_value': "fake-qualifier-value"
                     }
                 ]
             },
             "error.knowledge_graph.edge.qualifiers.qualifier.type_id.unknown"
         ),
-        (  # Query 11 - 'qualifier' entry is missing its 'qualifier_value' property - invalidated by TRAPI schema
+        (  # Query 10 - 'qualifier' entry is missing its 'qualifier_value' property - invalidated by TRAPI schema
             {
                 'qualifiers': [
                     {
                         'qualifier_type_id': "biolink:object_direction_qualifier"
                     }
                 ]
             },
             "error.trapi.validation"
         ),
-        (   # Query 12 - qualifier_type_id 'object_direction_qualifier' is a valid Biolink qualifier type and
+        (   # Query 11 - qualifier_type_id 'object_direction_qualifier' is a valid Biolink qualifier type and
             #            'upregulated' a valid corresponding 'permissible value' enum 'qualifier_value'
             {
                 'qualifiers': [
                     {
                         'qualifier_type_id': "biolink:object_direction_qualifier",
                         'qualifier_value': "upregulated"
                     }
                 ]
             },
             ""    # this particular use case should pass
         ),
-        # (   #  *** Currently unsupported use case:
-        #     # Query xx - 'qualifier_type_id' is a valid Biolink qualifier type and 'RO:0002213'
-        #     #            is an 'exact match' to a 'upregulated', the above 'qualifier_value'
+        # (   # This use case was discussed with Sierra on 11 April 2023 and
+        #     # decided to be out-of-scope of enum values for is_permissible_value_of_enum()
+        #
+        #     # Query ## - 'qualifier_type_id' is a valid Biolink qualifier type and 'RO:0002213'
+        #     #            is an 'exact match' to a 'upregulated', the above 'qualifier_value'.
+        #     #            This unit test won't pass without a modification of the Biolink Model Toolkit
+        #     #            method for validating qualifier values to accept mapped values.
         #     {
         #         'qualifiers': [
         #             {
         #                 'qualifier_type_id': "biolink:object_direction_qualifier",
         #                 'qualifier_value': "RO:0002213"   # RO 'exact match' term for 'upregulated'
         #             }
         #         ]
         #     },
-        #     ""    # this other use case should also pass
-        # ),
-        (   # Query 13 - 'qualifier_type_id' is a valid Biolink qualifier type and
-            #             'UBERON:0001981' a valid corresponding 'reachable from' enum 'qualifier_value'
-            {
-                'qualifiers': [
-                    {
-                        'qualifier_type_id': "biolink:anatomical_context_qualifier",
-                        'qualifier_value': "UBERON:0001981"  # Blood Vessel
-                    }
-                ]
-            },
-            ""    # this particular use case should also pass
-        )
+        #     ""
+        # )
     ]
 )
 def test_validate_qualifiers(query: Tuple):
     qualifier_validator(
         tested_method=BiolinkValidator.validate_qualifiers,
         edge_model="Edge",
         query=query
     )
 
 
+Q_NOT_A_CURIE = {
+    'qualifiers': [
+        {
+            'qualifier_type_id': "not-a-curie",
+            'qualifier_value': "fake-qualifier-value"
+        }
+    ]
+}
+
+
+@pytest.mark.parametrize(
+    "query",
+    [
+        (  # Query 0 - 'qualifier_type_id' value not a Biolink CURIE - seen as 'unknown' in TRAPI < 1.4.0-beta
+                "1.3.0",
+                Q_NOT_A_CURIE,
+                "error.knowledge_graph.edge.qualifiers.qualifier.type_id.unknown"
+        ),
+        (  # Query 1 - 'qualifier_type_id' value not a Biolink CURIE - schema validation error in TRAPI < 1.4.0-beta
+                "1.4.0-beta",
+                Q_NOT_A_CURIE,
+                "error.trapi.validation"
+        )
+    ]
+)
+def test_validate_biolink_curie_in_qualifiers(query: Tuple[str, Dict, str]):
+    qualifier_validator(
+        tested_method=BiolinkValidator.validate_qualifiers,
+        edge_model="Edge",
+        query=query[1:],
+        trapi_version=query[0]
+    )
+
+
 ##################################
 # Validate TRAPI Knowledge Graph #
 ##################################
 @pytest.mark.parametrize(
     "query",
     [
         (
@@ -1529,15 +1696,21 @@
                                "attribute_type_id": "biolink:aggregator_knowledge_source",
                                "attributes": [],
                                "description": "Molecular Data Provider",
                                "original_attribute_name": "biolink:aggregator_knowledge_source",
                                "value": "infores:molepro",
                                "value_type_id": "biolink:InformationResource"
                            }
-                        ]
+                        ],
+                       "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                       ]
                     }
                 }
             },
             ""
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
@@ -1594,15 +1767,21 @@
                     "NCBIGene:29974": {}
                 },
                 "edges": {
                    "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}]
+                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Node 'NCBIGene:29974' is missing its categories!"
             "error.knowledge_graph.node.category.missing"
         ),
         (
@@ -1615,90 +1794,159 @@
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}]
+                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Node 'NCBIGene:29974.categories' slot value is not an array!"
             "error.knowledge_graph.node.categories.not_array"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 7: unknown category specified
+            # Query 7: Knowledge Graph 'categories' list values should include
+            #          at least one (non-abstract, non-mixin) category term
+            {
+                "nodes": {
+                    "UniProtKB:Q14191": {
+                       "categories": ["biolink:GeneProductMixin"]
+                    },
+                    "CHEBI:18420": {
+                        "name": "Magnesium",
+                        "categories": ["biolink:SmallMolecule"]
+                    }
+                },
+                "edges": {
+                    "edge_1": {
+                        "subject": "UniProtKB:Q14191",
+                        "predicate": "biolink:physically_interacts_with",
+                        "object": "CHEBI:18420",
+                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
+                    }
+                }
+            },
+            # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Node 'NCBIGene:29974.categories' slot value is not an array!"
+            "error.knowledge_graph.node.categories.not_concrete"
+        ),
+        (
+            LATEST_BIOLINK_MODEL_VERSION,
+            # Query 8: unknown category specified
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:NonsenseCategory"
                        ]
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}]
+                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Knowledge Graph Node element 'biolink:NonsenseCategory' is unknown!"
             "error.knowledge_graph.node.category.unknown"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 8: abstract category not allowed in Knowledge Graphs
+            # Query 9: abstract category in Knowledge Graphs? Itself ignored now during validation,
+            #          although if at least one 'concrete' class is not given, other related
+            #          validation errors (e.g. 'unmapped_prefix'?) may be reported?
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
-                           "biolink:AdministrativeEntity"
+                           "biolink:Entity",
+                           "biolink:Gene"
                        ]
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}]
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:primary_knowledge_source",
+                                "value": "infores:my-kp"
+                            }
+                        ],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
-            # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Knowledge Graph Node element " +
-            # "'biolink:AdministrativeEntity' is abstract!"
-            "error.knowledge_graph.node.category.abstract"
+            ""
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 9: mixin category not allowed in Knowledge Graphs
+            # Query 10: mixin category in Knowledge Graphs? Itself ignored now during validation,
+            #          although if at least one 'concrete' class is not given with id_prefix mappings,
+            #          other related validation errors (e.g. 'unmapped_prefix'?) may be reported?
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
-                           "biolink:GeneOrGeneProduct"
+                           "biolink:GeneOrGeneProduct",
+                           "biolink:Gene"
                        ]
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}]
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:primary_knowledge_source",
+                                "value": "infores:my-kp"
+                            }
+                        ],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
-            # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Knowledge Graph Node element 'biolink:GeneOrGeneProduct' is a mixin!"
-            "error.knowledge_graph.node.category.mixin"
+            ""
         ),
         # (   # no longer testable in Biolink 3.1.1 since Nutrient is
         #     # gone and no other deprecated categories in this release
         #     LATEST_BIOLINK_MODEL,
         #     # Query xx: deprecated category triggers a warning in Knowledge Graphs
         #     {
         #         "nodes": {
@@ -1723,15 +1971,15 @@
         #         }
         #     },
         #  f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Knowledge Graph Node element 'biolink:OntologyClass' is deprecated!"
         #     "warning.knowledge_graph.node.category.deprecated"
         # ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 10: invalid node CURIE prefix namespace, for specified category
+            # Query 11: invalid node CURIE prefix namespace, for specified category
             {
                 "nodes": {
                     "FOO:1234": {
                        "categories": [
                            "biolink:Gene"
                        ],
                     },
@@ -1747,50 +1995,62 @@
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:primary_knowledge_source",
                                 "value": "infores:my-kp"
                             }
+                        ],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
                         ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Node 'FOO:1234' " +
             # "is unmapped to the target categories: ['biolink:Gene']?"
-            "warning.knowledge_graph.node.unmapped_prefix"
+            "warning.knowledge_graph.node.id.unmapped_prefix"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 11: missing or empty subject, predicate, object values
+            # Query 12: missing or empty subject, predicate, object values
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     }
                 },
                 "edges": {
                     "edge_1": {
                         # "subject": "",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}]
+                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
             # ditto for predicate and object... but identical code pattern thus we only test missing subject id here
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge 'None--biolink:interacts_with->NCBIGene:29974' " +
             # "has a missing or empty 'subject' slot value!"
             "error.knowledge_graph.edge.subject.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 12: 'subject' id is missing from the nodes catalog
+            # Query 13: 'subject' id is missing from the nodes catalog
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -1802,24 +2062,30 @@
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:12345",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}]
+                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge 'subject' id 'NCBIGene:12345' is missing from the nodes catalog!"
             "error.knowledge_graph.edge.subject.missing_from_nodes"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 13: predicate is unknown
+            # Query 14: predicate is unknown
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -1831,24 +2097,30 @@
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:unknown_predicate",
                         "object": "PUBCHEM.COMPOUND:597",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}]
+                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Predicate element 'biolink:unknown_predicate' is unknown!"
             "error.knowledge_graph.edge.predicate.unknown"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 14: predicate is invalid - may be a valid Biolink element but is not a predicate
+            # Query 15: predicate is invalid - may be a valid Biolink element but is not a predicate
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -1860,24 +2132,30 @@
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:has_unit",
                         "object": "PUBCHEM.COMPOUND:597",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}]
+                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Predicate element 'biolink:has_unit' is invalid!"
             "error.knowledge_graph.edge.predicate.invalid"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 15: predicate is a mixin - not allowed in Knowledge Graphs
+            # Query 16: predicate is a mixin - not allowed in Knowledge Graphs
             {
                 "nodes": {
                     "HGNC:3059": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -1889,24 +2167,30 @@
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "HGNC:3059",
                         "predicate": "biolink:increases_amount_or_activity_of",
                         "object": "HGNC:391",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}]
+                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
             # "{KNOWLEDGE_GRAPH_PREFIX}: ERROR -Predicate element 'biolink:increases_amount_or_activity of' is a mixin!"
             "error.knowledge_graph.edge.predicate.mixin"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 16: predicate is abstract - not allowed in Knowledge Graphs
+            # Query 17: predicate is abstract - not allowed in Knowledge Graphs
             {
                 "nodes": {
                     "PMID:1234": {
                        "categories": [
                            "biolink:InformationContentEntity"
                        ]
                     },
@@ -1918,24 +2202,30 @@
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "PMID:1234",
                         "predicate": "biolink:contributor",
                         "object": "ORCID:56789",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}]
+                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Predicate element 'biolink:contributor' is abstract!"
             "error.knowledge_graph.edge.predicate.abstract"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 17: predicate is non-canonical
+            # Query 18: predicate is non-canonical
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -1947,24 +2237,30 @@
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:affected_by",
                         "object": "PUBCHEM.COMPOUND:597",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}]
+                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Edge predicate 'biolink:affected_by' is non-canonical?"
             "warning.knowledge_graph.edge.predicate.non_canonical"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 18: 'object' id is missing from the nodes catalog
+            # Query 19: 'object' id is missing from the nodes catalog
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -1976,25 +2272,31 @@
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:678",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}]
+                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge 'object' id " +
             # f"'PUBCHEM.COMPOUND:678' is missing from the nodes catalog!"
             "error.knowledge_graph.edge.object.missing_from_nodes"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 19: attribute 'attribute_type_id' is missing
+            # Query 20: attribute 'attribute_type_id' is missing
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2006,24 +2308,30 @@
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
-                        "attributes": [{"value": "some value"}]
+                        "attributes": [{"value": "some value"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge attribute is missing its 'attribute_type_id' key!"
             "error.knowledge_graph.edge.attribute.type_id.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 20: attribute 'value' is missing?
+            # Query 21: attribute 'value' is missing?
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2035,24 +2343,30 @@
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}]
+                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge attribute is missing its 'value' key!"
             "error.knowledge_graph.edge.attribute.value.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 21: 'attribute_type_id' is not a CURIE
+            # Query 22: 'attribute_type_id' is not a CURIE
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2064,24 +2378,30 @@
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
-                        "attributes": [{"attribute_type_id": "not_a_curie", "value": "some value"}]
+                        "attributes": [{"attribute_type_id": "not_a_curie", "value": "some value"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge attribute_type_id 'not_a_curie' is not a CURIE!"
             "error.knowledge_graph.edge.attribute.type_id.not_curie"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 22: 'attribute_type_id' is not a 'biolink:association_slot' (biolink:synonym is a node property)
+            # Query 23: 'attribute_type_id' is not a 'biolink:association_slot' (biolink:synonym is a node property)
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2093,25 +2413,31 @@
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
-                        "attributes": [{"attribute_type_id": "biolink:synonym", "value": "some synonym"}]
+                        "attributes": [{"attribute_type_id": "biolink:synonym", "value": "some synonym"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Edge attribute_type_id "
             # "'biolink:synonym' is not a biolink:association_slot?"
             "warning.knowledge_graph.edge.attribute.type_id.not_association_slot"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 23: 'attribute_type_id' has a 'biolink' CURIE prefix and is an association_slot, so it should pass
+            # Query 24: 'attribute_type_id' has a 'biolink' CURIE prefix and is an association_slot, so it should pass
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2126,23 +2452,29 @@
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [
                             {"attribute_type_id": "biolink:negated", "value": "some value"},
                             {"attribute_type_id": "biolink:primary_knowledge_source", "value": "infores:hmdb"}
+                        ],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
                         ]
                     }
                 }
             },
             ""  # this should recognize the 'attribute_type_id' as a Biolink CURIE
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 24: 'attribute_type_id' has a CURIE prefix namespace unknown to Biolink?
+            # Query 25: 'attribute_type_id' has a CURIE prefix namespace unknown to Biolink?
             {
                 "nodes": {
                     "NCBIGene:29974": {
                        "categories": [
                            "biolink:Gene"
                        ]
                     },
@@ -2154,51 +2486,29 @@
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
-                        "attributes": [{"attribute_type_id": "foo:bar", "value": "some value"}]
+                        "attributes": [{"attribute_type_id": "foo:bar", "value": "some value"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Edge attribute_type_id 'foo:bar' " +
             # f"has a CURIE prefix namespace unknown to Biolink!"
+            # TODO: Code for validating this is commented out pending a BMT repair of the test
             "warning.knowledge_graph.edge.attribute.type_id.unknown_prefix"
         ),
-        (
-            LATEST_BIOLINK_MODEL_VERSION,
-            # Query 25: has missing or empty attributes?
-            {
-                "nodes": {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    },
-                    "PUBCHEM.COMPOUND:597": {
-                        "name": "cytosine",
-                        "categories": [
-                            "biolink:SmallMolecule"
-                        ],
-                    }
-                },
-                "edges": {
-                    "edge_1": {
-                        "subject": "NCBIGene:29974",
-                        "predicate": "biolink:physically_interacts_with",
-                        "object": "PUBCHEM.COMPOUND:597",
-                        # "attributes": [{"attribute_type_id": "biolink:knowledge_source"}]
-                    }
-                }
-            },
-            # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge has no 'attributes' key!"
-            "error.knowledge_graph.edge.attribute.missing"
-        ),
         (   # Query 26:  # An earlier Biolink Model won't recognize a category not found in its specified release
             "1.8.2",
             {
                 # Sample nodes
                 'nodes': {
                     "NCBIGene:29974": {
                        "categories": [
@@ -2226,7 +2536,142 @@
     ]
 )
 def test_check_biolink_model_compliance_of_knowledge_graph(query: Tuple):
     validator: BiolinkValidator = check_biolink_model_compliance_of_knowledge_graph(
         graph=query[1], biolink_version=query[0]
     )
     check_messages(validator, query[2])
+
+
+MESSAGE_EDGE_WITHOUT_ATTRIBUTES = {
+    "nodes": {
+        "NCBIGene:29974": {
+            "categories": [
+                "biolink:Gene"
+            ]
+        },
+        "PUBCHEM.COMPOUND:597": {
+            "name": "cytosine",
+            "categories": [
+                "biolink:SmallMolecule"
+            ],
+        }
+    },
+    "edges": {
+        "edge_1": {
+            "subject": "NCBIGene:29974",
+            "predicate": "biolink:physically_interacts_with",
+            "object": "PUBCHEM.COMPOUND:597",
+            # "attributes": [{"attribute_type_id": "biolink:knowledge_source"}]
+        }
+    }
+}
+
+
+def test_pre_trapi_1_4_0_validate_attributes():
+    # message edges must have at least some 'provenance' attributes
+    edge_without_attributes = deepcopy(MESSAGE_EDGE_WITHOUT_ATTRIBUTES)
+    validator: BiolinkValidator = check_biolink_model_compliance_of_knowledge_graph(
+        graph=edge_without_attributes,
+        trapi_version="1.3.0",
+        biolink_version=LATEST_BIOLINK_MODEL_VERSION
+    )
+    check_messages(validator, "error.knowledge_graph.edge.attribute.missing")
+
+
+SAMPLE_RETRIEVAL_SOURCE = {
+    # required, infores CURIE to an Information Resource
+    "resource_id": "infores:molepro",
+
+    # required, string drawn from the TRAPI ResourceRoleEnum
+    # values that were formerly recorded as TRAPI attributes
+    # are now presented as first class edge annotation
+    "resource_role": "primary_knowledge_source"
+}
+
+SAMPLE_RETRIEVAL_SOURCE_EMPTY_RESOURCE_ID = {
+    # required, string drawn from the TRAPI ResourceRoleEnum
+    # values that were formerly recorded as TRAPI attributes
+    # are now presented as first class edge annotation
+    "resource_role": "primary_knowledge_source"
+}
+
+SAMPLE_RETRIEVAL_SOURCE_EMPTY_RESOURCE_ROLE = {
+    # required, infores CURIE to an Information Resource
+    "resource_id": "infores:molepro",
+}
+
+SAMPLE_RETRIEVAL_SOURCE_RESOURCE_ID_NOT_CURIE = {
+    # required, infores CURIE to an Information Resource
+    "resource_id": "molepro",
+
+    # required, string drawn from the TRAPI ResourceRoleEnum
+    # values that were formerly recorded as TRAPI attributes
+    # are now presented as first class edge annotation
+    "resource_role": "primary_knowledge_source"
+}
+
+SAMPLE_RETRIEVAL_SOURCE_RESOURCE_ID_INFORES_INVALID = {
+    # required, infores CURIE to an Information Resource
+    "resource_id": "not-an-infores:molepro",
+
+    # required, string drawn from the TRAPI ResourceRoleEnum
+    # values that were formerly recorded as TRAPI attributes
+    # are now presented as first class edge annotation
+    "resource_role": "primary_knowledge_source"
+}
+
+SAMPLE_RETRIEVAL_SOURCE_RESOURCE_ID_INFORES_UNKNOWN = {
+    # required, infores CURIE to an Information Resource
+    "resource_id": "infores:my-favorite-kp",
+
+    # required, string drawn from the TRAPI ResourceRoleEnum
+    # values that were formerly recorded as TRAPI attributes
+    # are now presented as first class edge annotation
+    "resource_role": "primary_knowledge_source"
+}
+
+
+@pytest.mark.parametrize(
+    "sources,validation_code",
+    [
+        ([SAMPLE_RETRIEVAL_SOURCE], ""),  # No validation code generated?
+        (None, "error.knowledge_graph.edge.sources.missing"),
+        ([], "error.knowledge_graph.edge.sources.empty"),
+        ("not-an-array", "error.knowledge_graph.edge.sources.not_array"),
+        (
+            [SAMPLE_RETRIEVAL_SOURCE_EMPTY_RESOURCE_ID],
+            "error.knowledge_graph.edge.sources.retrieval_source.resource_id.empty"
+        ),
+        (
+            [SAMPLE_RETRIEVAL_SOURCE_EMPTY_RESOURCE_ROLE],
+            "error.knowledge_graph.edge.sources.retrieval_source.resource_role.empty"
+        ),
+        (
+            [SAMPLE_RETRIEVAL_SOURCE_RESOURCE_ID_NOT_CURIE],
+            "error.knowledge_graph.edge.sources.retrieval_source.resource_id.infores.not_curie"
+        ),
+        (
+            [SAMPLE_RETRIEVAL_SOURCE_RESOURCE_ID_INFORES_INVALID],
+            "error.knowledge_graph.edge.sources.retrieval_source.resource_id.infores.invalid"
+        ),
+        # TODO: need method to determine if an infores is known with recent changes to BMT
+        # (
+        #     [SAMPLE_RETRIEVAL_SOURCE_RESOURCE_ID_INFORES_UNKNOWN],
+        #     "error.knowledge_graph.edge.sources.retrieval_source.resource_id.infores.unknown"
+        # )
+    ]
+)
+def test_latest_trapi_validate_sources(sources: bool, validation_code: str):
+    # no attributes are strictly needed in 1.4.0-beta now that (mandatory)
+    # Edge provenance is recorded in the Edge.sources list of RetrievalSource
+    # message edges must have at least some 'provenance' attributes
+    sample_message = deepcopy(MESSAGE_EDGE_WITHOUT_ATTRIBUTES)
+    if sources is not None:
+        edge = sample_message["edges"]["edge_1"]
+        edge["sources"] = sources
+    validator: BiolinkValidator = check_biolink_model_compliance_of_knowledge_graph(
+        graph=sample_message,
+        # trapi_version="latest",  # 1.4.0++
+        biolink_version=LATEST_BIOLINK_MODEL_VERSION
+    )
+    check_messages(validator, validation_code)
```

### Comparing `reasoner_validator-3.4.9/tests/test_response_validator.py` & `reasoner_validator-3.5.0/tests/test_response_validator.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from reasoner_validator import TRAPIResponseValidator
 from tests.test_validation_report import check_messages
 
 logger = logging.getLogger(__name__)
 logger.setLevel("DEBUG")
 
+PRE_TRAPI_1_4_0 = "1.3.0"
 
 _TEST_QG_1 = {
     "nodes": {
         "type-2 diabetes": {"ids": ["MONDO:0005148"]},
         "drug": {
             "categories": ["biolink:Drug"]
         }
@@ -74,15 +75,15 @@
                    "attribute_type_id": "biolink:aggregator_knowledge_source",
                    "attributes": [],
                    "description": "Molecular Data Provider",
                    "original_attribute_name": "biolink:aggregator_knowledge_source",
                    "value": "infores:molepro",
                    "value_type_id": "biolink:InformationResource"
                }
-            ]
+            ],
         }
     }
 
 _TEST_KG_1 = {
     'nodes': _TEST_NODES_1,
     'edges': _TEST_EDGES_1
 }
@@ -111,15 +112,15 @@
                    "attribute_type_id": "biolink:aggregator_knowledge_source",
                    "attributes": [],
                    "description": "Molecular Data Provider",
                    "original_attribute_name": "biolink:aggregator_knowledge_source",
                    "value": "infores:molepro",
                    "value_type_id": "biolink:InformationResource"
                }
-            ]
+           ],
         }
     }
 
 _TEST_KG_2 = {
     'nodes': _TEST_NODES_1,
     'edges': _TEST_EDGES_2
 }
@@ -160,19 +161,19 @@
 # Sample edge 3
 _TEST_EDGES_3 = {
        "edge_1": {
            "subject": "PMID:11156626",
            "predicate": "biolink:contributor",
            "object": "ORCID:0000-0002-4447-5978",
            "attributes": [
-                {
-                    "attribute_type_id": "biolink:primary_knowledge_source",
-                    "value": "infores:automat-text-mining-provider"
-                }
-            ]
+               {
+                   "attribute_type_id": "biolink:primary_knowledge_source",
+                   "value": "infores:automat-text-mining-provider"
+               }
+           ],
         }
     }
 
 _TEST_KG_3 = {
     'nodes': _TEST_NODES_2,
     'edges': _TEST_EDGES_3
 }
@@ -205,15 +206,15 @@
                    "attribute_type_id": "biolink:primary_knowledge_source",
                    "value": "infores:automat-text-mining-provider"
                },
                {
                    "attribute_type_id": "biolink:primary_knowledge_source",
                    "value": "infores:hmdb"
                }
-           ]
+           ],
         }
     }
 
 
 _TEST_KG_4 = {
     'nodes': _TEST_NODES_1,
     'edges': _TEST_EDGES_4
@@ -324,193 +325,193 @@
     [
         (   # Query 0 - Completely empty Response.Message
             {
                 "message": {
 
                 }
             },
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
-            None,
-            None,
+            False,
             # "Validate TRAPI Response: ERROR - Response returned an empty Message Query Graph!"
             "error.trapi.response.message.empty"
         ),
         (   # Query 1 - Response.Message also devoid of content, missing QGraph trapped first....
             {
                 "message": {
                     "knowledge_graph": None,
                     "results": None
                 }
             },
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
-            None,
-            None,
+            False,
             # "Validate TRAPI Response: ERROR - TRAPI Message is missing its Query Graph!"
             "error.trapi.response.query_graph.missing"
         ),
         (   # Query 2 - Response.Message also devoid of content, null QGraph trapped first....
             {
                 "message": {
                     "query_graph": None,
                     "knowledge_graph": None,
                     "results": None
                 }
             },
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
-            None,
-            None,
+            False,
             # "Validate TRAPI Response: ERROR - Response returned an null or empty Message Query Graph!"
             "error.trapi.response.query_graph.empty"
         ),
         (
             # Query 3 - Partly empty Response.Message with a modest but
             #           workable query graph? Missing KG trapped next?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     # "knowledge_graph": None,
                     "results": None
                 }
             },
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
-            None,
-            None,
+            False,
             # "Validate TRAPI Response: ERROR - TRAPI Message is missing its Knowledge Graph component?"
             "error.trapi.response.knowledge_graph.missing"
         ),
         (
             # Query 4 - Partly empty Response.Message with a modest
             #           but workable query graph? Empty KG trapped next?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": None,
                     "results": None
                 }
             },
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
-            None,
-            None,
+            False,
             # "Validate TRAPI Response: WARNING - Response returned an empty Message Knowledge Graph?"
             "warning.response.knowledge_graph.empty"
         ),
         (
             # Query 5 - Partly empty Response.Message with a modest but workable
             #           query and knowledge graphs? Missing Results detected next?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     # "results": None
                 }
             },
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
-            None,
-            None,
+            False,
             # "Validate TRAPI Response: ERROR - TRAPI Message is missing its Results component!"
             "error.trapi.response.results.missing"
         ),
         (
             # Query 6 - Partly empty Response.Message with a modest but workable query and
             #           knowledge graphs? Null valued Results detected next - just issue a warning?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": None
                 }
             },
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
-            None,
-            None,
+            False,
             # "Validate TRAPI Response: WARNING -Response returned empty Message.results?"
             "warning.response.results.empty"
         ),
         (
             # Query 7 - Partly empty Response.Message with a modest but workable
             #           query and knowledge graphs? Non-array Results detected next?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": {"invalid results"}
                 }
             },
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
-            None,
-            None,
+            False,
             # "Validate TRAPI Response: ERROR - the 'Response.Message.Results' field
             # is not TRAPI schema validated since it has the wrong format!"
             "error.trapi.validation"
         ),
         (
             # Query 8 - Partly empty Response.Message with a modest but workable query and
             #           knowledge graphs? Empty Results detected next - just issue a warning?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": []
                 }
             },
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
-            None,
-            None,
+            False,
             # "Validate TRAPI Response: ERROR - Response returned empty Message.results?"
             "warning.response.results.empty"
         ),
         (
             # Query 9 - Full Message, without 'sources' and 'strict_validation': False - should pass?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
-            None,
-            None,
+            False,
             ""
         ),
         (
             # Query 10 - Full Message, with strict validation - still passes
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
-            None,
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             True,
             ""
         ),
         (
             # Query 11 - Full Message, with strict validation and non-null sources that match
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
-            None,
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             {
                 "ara_source": None,
                 "kp_source": "infores:hmdb",
                 "kp_source_type": "primary"
             },
             True,
@@ -521,15 +522,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
-            None,
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             {
                 "ara_source": None,
                 "kp_source": "infores:molepro",
                 "kp_source_type": "primary"
             },
             True,
@@ -540,15 +541,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
-            None,
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             {
                 "ara_source": "infores:aragorn",
                 "kp_source": "infores:hmdb",
                 "kp_source_type": "primary"
             },
             True,
@@ -559,15 +560,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
-            None,
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             {
                 "ara_source": "infores:molepro",
                 "kp_source": "infores:hmdb",
                 "kp_source_type": "primary"
             },
             True,
@@ -578,15 +579,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
-            None,
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             {
                 "ara_source": None,
                 "kp_source": "infores:molepro",
                 "kp_source_type": "aggregator"
             },
             True,
@@ -598,15 +599,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_2,
                     "results": _TEST_RESULTS_1
                 }
             },
-            None,
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             {
                 "ara_source": None,
                 "kp_source": "infores:molepro",
                 "kp_source_type": "aggregator"
             },
             True,
@@ -618,128 +619,117 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_4,
                     "results": _TEST_RESULTS_1
                 }
             },
-            None,
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             {
                 "ara_source": None,
                 "kp_source": "infores:molepro",
                 "kp_source_type": "aggregator"
             },
             True,
             "warning.knowledge_graph.edge.provenance.multiple_primary"
         ),
         (
-            # Query 18 - Full Message, with non-strict validation
+            # Query 18 - Full Message, with non-strict validation.
+            #            Both knowledge graph nodes have 'mixin' categories,
+            #            the list of categories for knowledge graphs
+            #            must have at least one concrete category,
+            #            hence, a validation error is now reported:
             {
                 "message": {
                     "query_graph": _TEST_QG_2,
                     "knowledge_graph": _TEST_KG_3,
                     "results": _TEST_RESULTS_2
                 }
             },
-            None,
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             False,
-            ""
+            "error.knowledge_graph.node.categories.not_concrete"
         ),
         (
-            # Query 19 - Full Message, WITH strict validation - abstract category?
+            # Query 19 - Full Message, WITH strict validation - abstract predicate?
             {
                 "message": {
                     "query_graph": _TEST_QG_2,
                     "knowledge_graph": _TEST_KG_3,
                     "results": _TEST_RESULTS_2
                 }
             },
-            None,
-            None,
-            None,
-            True,
-            "error.query_graph.node.category.abstract"
-        ),
-        (
-            # Query 20 - Full Message, WITH strict validation - abstract predicate?
-            {
-                "message": {
-                    "query_graph": _TEST_QG_2,
-                    "knowledge_graph": _TEST_KG_3,
-                    "results": _TEST_RESULTS_2
-                }
-            },
-            None,
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             True,
             "error.query_graph.edge.predicate.abstract"
         ),
         (
-            # Query 21 - Valid full Message, under strict validation.
+            # Query 20 - Valid full Message, under strict validation.
             #            Message is valid, but the 'workflow' field is not an array?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 },
                 "workflow": "workflows-not-an-array"
             },
-            None,
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             True,
             # "Validate TRAPI Response: ERROR - TRAPI schena error: the 'workflow' field must be an array"
             "error.trapi.validation"
         ),
         (
-            # Query 22 - Valid full Message, under strict validation.
+            # Query 21 - Valid full Message, under strict validation.
             #            Message is valid, the 'workflow' field is an array,
             #            but the single list entry is an invalid workflow spec?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 },
                 "workflow": ["not-a-valid-workflow-spec"]
             },
-            None,
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             True,
             # "Validate TRAPI Response: ERROR - TRAPI schena error: the 'workflow' field must be an array of
             # a 'workflow' JSON objects, with contents as defined by the workflow schema.
             "error.trapi.validation"
         ),
         (
-            # Query 23 - Valid full Message, under strict validation.
+            # Query 22 - Valid full Message, under strict validation.
             #            Message is valid, the 'workflow' field is an array,
             #            but the single list entry is in the workflow schema
             #            and has at least the one required field 'id'
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 },
                 "workflow": [{"id": "annotate"}]
             },
-            None,
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             True,
             ""   # this simple workflow spec should pass?
         ),
         (
-            # Query 24 - Valid full Message, under strict validation. Message is valid, the 'workflow' field is array,
+            # Query 23 - Valid full Message, under strict validation. Message is valid, the 'workflow' field is array,
             #            but the single list entry is an elaborated 'real world' workflow spec,
             #            but one entry overlay_compute_ngd is incomplete - doesn't fully validate!
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
@@ -766,24 +756,24 @@
                       "id": "score"
                     },
                     {
                       "id": "complete_results"
                     }
                 ]
             },
-            None,
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             True,
             # "Validate TRAPI Response: ERROR - TRAPI schema validation error: the 'workflow'
             # field entry overlay_compute_ngd is missing a required parameter 'qnodes_keys'
             "error.trapi.validation"
         ),
         (
-            # Query 25 - Valid full Message, under strict validation. Message is valid, the 'workflow' field is array,
+            # Query 24 - Valid full Message, under strict validation. Message is valid, the 'workflow' field is array,
             #            but the single list entry is an elaborated 'real world' workflow spec
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 },
@@ -810,39 +800,39 @@
                       "id": "score"
                     },
                     {
                       "id": "complete_results"
                     }
                 ]
             },
-            None,
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             True,
             ""   # this simple workflow spec should pass?
         ),
         (
-            # Query 26 - Valid full Message, under strict validation. Message is valid,
+            # Query 25 - Valid full Message, under strict validation. Message is valid,
             #            the 'workflow' field is an array, but runner_parameters is None.
-            #            This is technically invalid but we have a code patch which should filter it out (for now)
+            #            This is technically invalid, but we have a code patch which should filter it out (for now)
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 },
                 "workflow": [
                     {
                         "id": "lookup",
                         "runner_parameters": None,
                         "parameters": None
                     }
                 ]
             },
-            None,
+            PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             True,
             ""   # this filtered workflow spec should pass
         )
     ]
 )
@@ -851,7 +841,129 @@
         trapi_version=query[1],
         biolink_version=query[2],
         sources=query[3],
         strict_validation=query[4]
     )
     validator.check_compliance_of_trapi_response(response=query[0])
     check_messages(validator, query[5], no_errors=True)
+
+
+@pytest.mark.parametrize(
+    "response,trapi_version,biolink_version,sources,strict_validation,code",
+    [
+        (   # Query 0 - Completely empty Response.Message
+            {
+                "message": {
+
+                }
+            },
+            PRE_TRAPI_1_4_0,  # trapi_version
+            None,
+            None,
+            False,
+            ""
+        ),
+        (   # Query 1 - Response.Message also devoid of content, missing QGraph trapped first....
+            {
+                "message": {
+                    "knowledge_graph": None,
+                    "results": None
+                }
+            },
+            PRE_TRAPI_1_4_0,  # trapi_version
+            None,
+            None,
+            False,
+            ""
+        ),
+        (   # Query 2 - Response.Message also devoid of content, null QGraph trapped first....
+            {
+                "message": {
+                    "query_graph": None,
+                    "knowledge_graph": None,
+                    "results": None
+                }
+            },
+            PRE_TRAPI_1_4_0,  # trapi_version
+            None,
+            None,
+            False,
+            ""
+        ),
+        (
+            # Query 3 - Partly empty Response.Message with a modest but
+            #           workable query graph? Missing KG trapped next?
+            {
+                "message": {
+                    "query_graph": _TEST_QG_1,
+                    # "knowledge_graph": None,
+                    "results": None
+                }
+            },
+            PRE_TRAPI_1_4_0,  # trapi_version
+            None,
+            None,
+            False,
+            ""
+        ),
+        (
+            # Query 4 - Partly empty Response.Message with a modest
+            #           but workable query graph? Empty KG trapped next?
+            {
+                "message": {
+                    "query_graph": _TEST_QG_1,
+                    "knowledge_graph": None,
+                    "results": None
+                }
+            },
+            PRE_TRAPI_1_4_0,  # trapi_version
+            None,
+            None,
+            False,
+            ""
+        ),
+        (
+            # Query 5 - Partly empty Response.Message with a modest but workable
+            #           query and knowledge graphs? Missing Results detected next?
+            {
+                "message": {
+                    "query_graph": _TEST_QG_1,
+                    "knowledge_graph": _TEST_KG_1,
+                    # "results": None
+                }
+            },
+            PRE_TRAPI_1_4_0,  # trapi_version
+            None,
+            None,
+            False,
+            ""
+        ),
+        (
+            # Query 6 - Partly empty Response.Message with a modest but workable query and
+            #           knowledge graphs? Null valued Results detected next - just issue a warning?
+            {
+                "message": {
+                    "query_graph": _TEST_QG_1,
+                    "knowledge_graph": _TEST_KG_1,
+                    "results": None
+                }
+            },
+            PRE_TRAPI_1_4_0,  # trapi_version
+            None,
+            None,
+            False,
+            ""
+        )
+    ]
+)
+def test_check_biolink_model_compliance_of_trapi_response_suppressing_empty_data_warnings(
+        response, trapi_version, biolink_version, sources, strict_validation, code
+):
+    validator: TRAPIResponseValidator = TRAPIResponseValidator(
+        trapi_version=trapi_version,
+        biolink_version=biolink_version,
+        sources=sources,
+        strict_validation=strict_validation,
+        suppress_empty_data_warnings=True
+    )
+    validator.check_compliance_of_trapi_response(response=response)
+    check_messages(validator, code, no_errors=True)
```

### Comparing `reasoner_validator-3.4.9/tests/test_validation_report.py` & `reasoner_validator-3.5.0/tests/test_validation_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 """Testing Validation Report methods"""
 from typing import Optional, Dict, Tuple, List
+from sys import stderr
+
 import pytest
 
 from reasoner_validator.report import ValidationReporter
 from reasoner_validator.validation_codes import CodeDictionary
+from reasoner_validator.versioning import get_latest_version
 
-TEST_TRAPI_VERSION = "1.3.0"
+TEST_TRAPI_VERSION = get_latest_version(ValidationReporter.DEFAULT_TRAPI_VERSION)
 TEST_BIOLINK_VERSION = "2.4.8"
 
 
 def check_messages(validator: ValidationReporter, code, no_errors: bool = False):
     messages: Dict[str, Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]] = validator.get_messages()
     if code:
         # TODO: 'code' should be found in code.yaml
         # value: Optional[Tuple[str, str]] = CodeDictionary.get_code_subtree(code)
         # assert value is not None
         message_type = validator.get_message_type(code)
         if message_type == "error":
+            print("code is:", code)
+            print("message_type", message_type)
+            print("messages['errors']:", messages['errors'])
+            for error_code in messages['errors']:
+                print("error code is:", error_code)
             assert any([error_code == code for error_code in messages['errors']])
         elif message_type == "warning":
             assert any([warning_code == code for warning_code in messages['warnings']])
         elif message_type == "info":
             assert any([info_code == code for info_code in messages['information']])
     else:
         if no_errors:
@@ -43,62 +51,62 @@
 
     result = CodeDictionary.get_code_subtree("info.compliant", is_leaf=True)
     assert result is not None
     message_type, leaf = result
     assert leaf is not None
     assert isinstance(leaf, Dict)
     assert all([key in [CodeDictionary.MESSAGE, CodeDictionary.DESCRIPTION] for key in leaf])
-    assert leaf[CodeDictionary.MESSAGE] == "Biolink Model-compliant TRAPI Message."
+    assert leaf[CodeDictionary.MESSAGE] == "Biolink Model-compliant TRAPI Message"
     assert leaf[CodeDictionary.DESCRIPTION].startswith("Specified TRAPI message completely satisfies")
 
     assert CodeDictionary.get_code_subtree("info.compliant", is_leaf=False) is None
 
 
 def test_get_code_subtree_facet_message():
 
     result = CodeDictionary.get_code_subtree("info.compliant", facet="message", is_leaf=True)
     assert result is not None
     message_type, leaf = result
     assert leaf is not None
     assert isinstance(leaf, Dict)
     assert CodeDictionary.MESSAGE in leaf
-    assert leaf[CodeDictionary.MESSAGE] == "Biolink Model-compliant TRAPI Message."
+    assert leaf[CodeDictionary.MESSAGE] == "Biolink Model-compliant TRAPI Message"
     assert CodeDictionary.DESCRIPTION not in leaf
 
-    result = CodeDictionary.get_code_subtree("info.query_graph.node.category", facet="message")
+    result = CodeDictionary.get_code_subtree("info.input_edge.predicate", facet="message")
     assert result is not None
     message_type, subtree = result
     assert subtree is not None
     assert isinstance(subtree, Dict)
     assert all([key in ["abstract", "mixin"] for key in subtree])
     assert CodeDictionary.MESSAGE in subtree["abstract"]
-    assert subtree["abstract"][CodeDictionary.MESSAGE] == "'{identifier}' is abstract."
+    assert subtree["abstract"][CodeDictionary.MESSAGE] == "Edge has an 'abstract' predicate"
     assert CodeDictionary.DESCRIPTION not in subtree["abstract"]
 
 
 def test_get_code_subtree_facet_description():
 
     result = CodeDictionary.get_code_subtree("info.compliant", facet="description", is_leaf=True)
     assert result is not None
     message_type, leaf = result
     assert leaf is not None
     assert isinstance(leaf, Dict)
     assert CodeDictionary.DESCRIPTION in leaf
     assert leaf[CodeDictionary.DESCRIPTION].startswith("Specified TRAPI message completely satisfies")
     assert CodeDictionary.MESSAGE not in leaf
 
-    result = CodeDictionary.get_code_subtree("info.query_graph.node.category", facet="description")
+    result = CodeDictionary.get_code_subtree("info.input_edge.predicate", facet="description")
     assert result is not None
     message_type, subtree = result
     assert subtree is not None
     assert isinstance(subtree, Dict)
     assert all([key in ["abstract", "mixin"] for key in subtree])
     assert CodeDictionary.DESCRIPTION in subtree["mixin"]
     assert subtree["mixin"][CodeDictionary.DESCRIPTION] == \
-           "TRAPI Message Query Graphs can have 'mixin' category classes."
+           "Input edge data can have 'mixin' predicates, when the mode of validation is 'non-strict'."
     assert CodeDictionary.MESSAGE not in subtree["mixin"]
 
 
 def test_get_code_subtree_internal_subtree():
     assert CodeDictionary.get_code_subtree("warning") is not None
 
     result = CodeDictionary.get_code_subtree("warning.knowledge_graph")
@@ -115,32 +123,32 @@
 
 def test_get_entry():
     assert CodeDictionary.get_code_entry("") is None
 
     code_entry: Optional[Dict] = CodeDictionary.get_code_entry("info.compliant")
     assert code_entry is not None
     assert CodeDictionary.MESSAGE in code_entry
-    assert code_entry[CodeDictionary.MESSAGE] == "Biolink Model-compliant TRAPI Message."
+    assert code_entry[CodeDictionary.MESSAGE] == "Biolink Model-compliant TRAPI Message"
 
     # Higher level subtrees, not terminal leaf entries?
     assert CodeDictionary.get_code_entry("info") is None
     assert CodeDictionary.get_code_entry("info.query_graph") is None
     assert CodeDictionary.get_code_entry("info.query_graph.node") is None
     assert CodeDictionary.get_code_entry("warning") is None
     assert CodeDictionary.get_code_entry("error") is None
 
     # Unknown code?
     assert CodeDictionary.get_code_entry("foo.bar") is None
 
 
 def test_get_message_template():
     assert CodeDictionary.get_message_template("") is None
-    assert CodeDictionary.get_message_template("info.compliant") == "Biolink Model-compliant TRAPI Message."
+    assert CodeDictionary.get_message_template("info.compliant") == "Biolink Model-compliant TRAPI Message"
     assert CodeDictionary.get_message_template("error.trapi.request.invalid") == \
-           "{identifier} could not generate a valid TRAPI query request object because {reason}!"
+           "Test could not generate a valid TRAPI query request object using identified element"
     assert CodeDictionary.get_message_template("foo.bar") is None
 
 
 def test_get_description():
     assert CodeDictionary.get_description("") is None
     info_compliant = CodeDictionary.get_description("info.compliant")
     assert info_compliant is not None
@@ -148,74 +156,65 @@
     info_attribute = CodeDictionary.get_description("warning.knowledge_graph.edge.attribute.type_id.non_biolink_prefix")
     assert info_attribute is not None
     assert info_attribute.startswith("Non-Biolink CURIEs are tolerated")
     assert CodeDictionary.get_description("foo.bar") is None
 
 
 def test_message_display():
-    assert "INFO - Biolink Model-compliant TRAPI Message." in CodeDictionary.display(code="info.compliant")
+    assert "INFO - Compliant: Biolink Model-compliant TRAPI Message" in CodeDictionary.display(
+        code="info.compliant",
+        add_prefix=True
+    )
     assert "ERROR - Knowledge Graph Nodes: No nodes found!" \
-           in CodeDictionary.display("error.knowledge_graph.nodes.empty")
-    identifier_dict: Dict = {"identifier": "biolink:AdministrativeEntity"}
-    assert "INFO - Input Edge Node Category: 'biolink:AdministrativeEntity' is abstract." \
+           in CodeDictionary.display("error.knowledge_graph.nodes.empty", add_prefix=True)
+    assert "INFO - Excluded: All test case S-P-O triples from " + \
+           "resource test location, or specific user excluded S-P-O triples" \
            in CodeDictionary.display(
-                code="info.input_edge.node.category.abstract",
-                parameters={"biolink:AdministrativeEntity": None}  # this code has no other parameters
+                code="info.excluded",
+                parameters={"a->biolink:related_to->b": None},  # this code has no other parameters
+                add_prefix=True
+            )
+    assert "INFO - Input Edge Predicate: Edge has an 'abstract' predicate" \
+           in CodeDictionary.display(
+                code="info.input_edge.predicate.abstract",
+                parameters={
+                    "biolink:contributor": [
+                        {"edge_id": "a->biolink:related_to->b"}
+                    ]
+                },  # this code has one other parameter named 'element_name'
+                add_prefix=True
             )
-
-
-def test_validator_reporter_message_display():
-    reporter = ValidationReporter(prefix="Test Validation Report", trapi_version=TEST_TRAPI_VERSION)
-    messages: List[str] = reporter.display(messages={
-            "info.input_edge.node.category.abstract": {
-                "biolink:AdministrativeEntity": None
-            }
-    })
-    assert "Test Validation Report: INFO - Input Edge Node Category: 'biolink:AdministrativeEntity' is abstract." \
-        in messages
-
-    messages = reporter.display(messages={
-            # validation code revolving to template
-            "error.input_edge.predicate.invalid":
-            {
-                # this identifier is an 'edge_id'
-                "a--biolink:not_a_predicate->b": [
-                    {"predicate":  "biolink:not_a_predicate"}  # other parameters
-                ]
-            }
-    })
-    assert "Test Validation Report: ERROR - Input Edge Predicate: " +\
-           "Edge 'a--biolink:not_a_predicate->b' predicate 'biolink:not_a_predicate' is invalid!" in messages
 
 
 def test_unknown_message_code():
     with pytest.raises(AssertionError):
         CodeDictionary.display(code="foo.bar")
 
 
 def test_message_report():
     reporter = ValidationReporter(prefix="First Validation Report", trapi_version=TEST_TRAPI_VERSION)
     reporter.report(code="info.compliant")
     reporter.report(
         code="info.input_edge.predicate.abstract",
-        identifier="biolink:contributor"
+        identifier="biolink:contributor",
+        edge_id="a->biolink:contributor->b"
     )
     report: Dict[str, Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]] = reporter.get_messages()
     assert 'information' in report
     assert len(report['information']) > 0
     messages: List[str] = list()
     for code, parameters in report['information'].items():
-        messages.extend(CodeDictionary.display(code, parameters))
-    assert "INFO - Biolink Model-compliant TRAPI Message." in messages
-    assert "INFO - Input Edge Predicate: 'biolink:contributor' is abstract." in messages
+        messages.extend(CodeDictionary.display(code, parameters, add_prefix=True))
+    assert "INFO - Compliant: Biolink Model-compliant TRAPI Message" in messages
+    assert "INFO - Input Edge Predicate: Edge has an 'abstract' predicate" in messages
 
 
 def test_messages():
     # Loading and checking a first reporter
-    reporter1 = ValidationReporter(prefix="First Validation Report", trapi_version=TEST_TRAPI_VERSION)
+    reporter1 = ValidationReporter(prefix="1st Test Message Set", trapi_version=TEST_TRAPI_VERSION)
     assert reporter1.get_trapi_version() == TEST_TRAPI_VERSION
     assert reporter1.get_biolink_version() is None
     assert not reporter1.has_messages()
     reporter1.report("info.compliant")
     assert reporter1.has_messages()
     assert reporter1.has_information()
     assert not reporter1.has_warnings()
@@ -223,22 +222,23 @@
     reporter1.report("warning.graph.empty", identifier="Reporter1 Unit Test")
     assert reporter1.has_warnings()
     reporter1.report("error.knowledge_graph.nodes.empty")
     assert reporter1.has_errors()
 
     # Testing merging of messages from a second reporter
     reporter2 = ValidationReporter(
-        prefix="Second Validation Report",
+        prefix="2nd Test Message Set",
         biolink_version=TEST_BIOLINK_VERSION
     )
     assert reporter2.get_trapi_version() == TEST_TRAPI_VERSION
     assert reporter2.get_biolink_version() == TEST_BIOLINK_VERSION
     reporter2.report(
         code="info.query_graph.edge.predicate.mixin",
-        identifier="biolink:this_is_a_mixin"
+        identifier="biolink:this_is_a_mixin",
+        edge_id="a-biolink:this_is_a_mixin->b"
     )
     reporter2.report("warning.response.results.empty")
     reporter2.report("error.knowledge_graph.edges.empty")
     reporter1.merge(reporter2)
     assert reporter1.get_trapi_version() == TEST_TRAPI_VERSION
     assert reporter1.get_biolink_version() == TEST_BIOLINK_VERSION
     
@@ -248,32 +248,32 @@
     reporter1.merge(reporter3)
     assert reporter1.get_trapi_version() == TEST_TRAPI_VERSION
     assert reporter1.get_biolink_version() == TEST_BIOLINK_VERSION
 
     # testing addition a few raw batch messages
     new_messages: Dict[str, Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]] = {
         "information": {
-            "info.input_edge.predicate.abstract": {
-                "Dolly": None
+            "info.excluded": {
+                "Horace van der Gelder": None
             }
         },
         "warnings": {
-            "warning.knowledge_graph.node.unmapped_prefix": {
+            "warning.knowledge_graph.node.id.unmapped_prefix": {
                 "Will Robinson": [
                     {
                         "categories": "Lost in Space"
                     }
                 ]
             }
         },
         "errors": {
             "error.trapi.validation": {
                 "6.6.6": [
                     {
-                        'exception': "Dave, this can only be due to human error..."
+                        'reason': "Dave, this can only be due to human error..."
                     }
                 ]
 
             }
         }
     }
     reporter1.add_messages(new_messages)
@@ -281,44 +281,84 @@
     # Verify what we have
     messages: Dict[str, Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]] = reporter1.get_messages()
 
     assert "information" in messages
     assert len(messages['information']) > 0
     information: List[str] = list()
     for code, parameters in messages['information'].items():
-        information.extend(CodeDictionary.display(code, parameters))
-    assert "INFO - Input Edge Predicate: 'Dolly' is abstract." in information
+        information.extend(CodeDictionary.display(code, parameters, add_prefix=True))
+    assert "INFO - Excluded: All test case S-P-O triples from resource test location, " + \
+           "or specific user excluded S-P-O triples" in information
 
     assert "warnings" in messages
     assert len(messages['warnings']) > 0
     warnings: List[str] = list()
     for code, parameters in messages['warnings'].items():
-        warnings.extend(CodeDictionary.display(code, parameters))
-    assert "WARNING - Knowledge Graph Node Unmapped: 'Will Robinson' is unmapped " + \
-           "to the target categories 'Lost in Space'?" in warnings
+        warnings.extend(CodeDictionary.display(code, parameters, add_prefix=True))
+    assert "WARNING - Knowledge Graph Node Id Unmapped: " + \
+           "Node identifier found unmapped to target categories for node" in warnings
 
     assert "errors" in messages
     assert len(messages['errors']) > 0
     errors: List[str] = list()
     for code, parameters in messages['errors'].items():
-        errors.extend(CodeDictionary.display(code, parameters))
-    assert "ERROR - Trapi: TRAPI 6.6.6 schema exception: 'Dave, this can only be due to human error...'!" in errors
+        errors.extend(CodeDictionary.display(code, parameters, add_prefix=True))
+    assert "ERROR - Trapi: Schema validation exception" in errors
     
     obj = reporter1.to_dict()
     assert obj["trapi_version"] == TEST_TRAPI_VERSION
     assert obj["biolink_version"] == TEST_BIOLINK_VERSION
     assert "messages" in obj
     assert "errors" in obj["messages"]
     assert "error.trapi.validation" in obj["messages"]["errors"]
     messages: Optional[Dict[str, List[Dict[str, str]]]] = obj["messages"]["errors"]["error.trapi.validation"]
     assert messages, "Empty 'error.trapi.validation' messages set?"
     assert "6.6.6" in messages
     message_subset: List = messages["6.6.6"]
     assert "Dave, this can only be due to human error..."\
-           in [message['exception'] for message in message_subset if 'exception' in message]
+           in [message['reason'] for message in message_subset if 'reason' in message]
+
+    for n in range(0, 10):
+        reporter1.report(code="error.input_edge.node.category.missing", identifier=f"biolink:not_a_category_{n}")
+
+    for c in range(0, 5):
+        for n in range(0, 10):
+            reporter1.report(
+                code="error.input_edge.node.category.unknown",
+                identifier=f"biolink:not_a_category_{c}",
+                node_id=f"n{n}"
+            )
+
+    # Informal test of a text 'dump' of all the messages as a
+    # text blob, using the 'display_all' method to format them
+    print(
+        "\n\nThis is an indirect 'test' of the ValidationReporter.dump() method\n"
+        "which simply executes the function and look at the results here on the console:",
+        file=stderr
+    )
+    reporter1.dump(file=stderr)
+
+    print(
+        f"\n{'-'*80}\n" +
+        "ValidatorReporter.dump() with title suppressed using 'title=None'\n" +
+        "and compressed using 'id_rows=2', 'msg_rows=3', 'compress=True':\n",
+        file=stderr
+    )
+    reporter1.dump(title=None, id_rows=2, msg_rows=3, compact_format=True, file=stderr)
+
+    print(
+        f"\n{'-'*80}\n" +
+        "ValidatorReporter.dump() resetting the title to a user string\n" +
+        "and compressed using 'id_rows=1', 'msg_rows=1', 'compress=True':\n",
+        file=stderr
+    )
+    reporter1.dump(title="My KP Validation Report", id_rows=1, msg_rows=1, compact_format=True, file=stderr)
+
+    validation_report: str = reporter1.dumps(id_rows=2, msg_rows=3)
+    assert validation_report.startswith("Errors:")
 
 
 def test_validator_method():
 
     reporter = ValidationReporter(
         prefix="Test Validator Method",
         trapi_version=TEST_TRAPI_VERSION,
@@ -350,24 +390,24 @@
 
     messages: Dict[str, Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]] = reporter.get_messages()
 
     assert "warnings" in messages
     assert len(messages['warnings']) > 0
     warnings: List[str] = list()
     for code, parameters in messages['warnings'].items():
-        warnings.extend(CodeDictionary.display(code, parameters))
-    assert "WARNING - Graph: Fake data is empty?" in warnings
+        warnings.extend(CodeDictionary.display(code, parameters, add_prefix=True))
+    assert "WARNING - Graph: Empty graph" in warnings
 
     assert "errors" in messages
     assert len(messages['errors']) > 0
     errors: List[str] = list()
     for code, parameters in messages['errors'].items():
-        errors.extend(CodeDictionary.display(code, parameters))
+        errors.extend(CodeDictionary.display(code, parameters, add_prefix=True))
     assert "ERROR - Knowledge Graph Edge Provenance Infores: " + \
-           "Edge 'fake-edge-id' has provenance value 'foo:bar' which is not a well-formed InfoRes CURIE!" in errors
+           "Edge has provenance value which is not a well-formed InfoRes CURIE" in errors
 
 
 # has_validation_errors(root_key: str = 'validation', case: Optional[Dict] = None)
 @pytest.mark.parametrize(
     "query",
     [
         (
```

### Comparing `reasoner_validator-3.4.9/PKG-INFO` & `reasoner_validator-3.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.4.9
+Version: 3.5.0
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
@@ -14,38 +14,43 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Provides-Extra: dev
 Provides-Extra: docs
+Provides-Extra: web
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: bmt (>=1.0.3,<2.0.0)
-Requires-Dist: fastapi (>=0.68,<0.69)
+Requires-Dist: bmt (>=1.0.15,<2.0.0)
+Requires-Dist: fastapi (>=0.68,<0.69) ; extra == "web"
 Requires-Dist: jsonschema (>=4.17.0,<5.0.0)
-Requires-Dist: kgx (>=1.7.0,<2.0.0)
-Requires-Dist: myst-parser[docs] (>=0.18.1,<0.19.0) ; extra == "docs"
-Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: numpydoc[docs] (>=1.5.0,<2.0.0) ; extra == "docs"
+Requires-Dist: myst-parser (>=0.18.1,<0.19.0) ; extra == "docs"
+Requires-Dist: numpydoc (>=1.5.0,<2.0.0) ; extra == "docs"
 Requires-Dist: pydantic (>=1.8.0,<2.0.0)
-Requires-Dist: pytest (>=7.2.2,<8.0.0)
+Requires-Dist: pytest (>=7.2.2,<8.0.0) ; extra == "dev"
+Requires-Dist: pytest-cov (>=4.0.0,<5.0.0) ; extra == "dev"
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: sphinx[docs] (>=5.3.0,<6.0.0) ; extra == "docs"
-Requires-Dist: uvicorn (>=0.15,<0.16)
+Requires-Dist: sphinx (>=5.3.0,<6.0.0) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme (>=1.2.1,<2.0.0) ; extra == "docs"
+Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
+Requires-Dist: uvicorn (>=0.15,<0.16) ; extra == "web"
 Project-URL: Bug Tracker, https://github.com/NCATSTranslator/reasoner-validator/issues
 Project-URL: Change Log, https://github.com/NCATSTranslator/reasoner-validator/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://translator-reasoner-validator.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/NCATSTranslator/reasoner-validator
 Description-Content-Type: text/markdown
 
 # Reasoner Validator
 
 [![Pyversions](https://img.shields.io/pypi/pyversions/reasoner-validator)](https://pypi.python.org/pypi/reasoner-validator)
-[![pypi](https://github.com/NCATSTranslator/reasoner-validator/workflows/pypi/badge.svg)](https://pypi.org/project/reasoner-validator/)
+[![Publish Python Package](https://github.com/NCATSTranslator/reasoner-validator/actions/workflows/pypi_publish.yml/badge.svg)](https://pypi.org/project/reasoner-validator/)
+[![Sphinx Documentation](https://github.com/NCATSTranslator/reasoner-validator/actions/workflows/doc_pages.yml/badge.svg)](https://github.com/NCATSTranslator/reasoner-validator/actions/workflows/doc_pages.yml)
+[![Run tests](https://github.com/NCATSTranslator/reasoner-validator/actions/workflows/test.yml/badge.svg)](https://github.com/NCATSTranslator/reasoner-validator/actions/workflows/test.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
 
 This package provides software methods to Translator components (e.g. Knowledge Providers and Autonomous Relay Agents) using *any version* of the
 [Translator Reasoner API (TRAPI)](https://github.com/NCATSTranslator/ReasonerAPI/blob/master/README.md) and the [Biolink Model](https://github.com/biolink/biolink-model/blob/master/README.md).
 
 See [the full documentation](https://ncatstranslator.github.io/reasoner-validator/) and [the contributor guidelines](https://github.com/NCATSTranslator/reasoner-validator/blob/master/.github/CONTRIBUTING.md).
 
@@ -53,44 +58,83 @@
 
 ## Python Dependency
 
 The Reasoner Validator now requires Python 3.9 or later (some library dependencies now force this).
 
 ## Installing the Module
 
-The module may be installed directly from pypi.org.
+The module may be installed directly from pypi.org using (Python 3) `pip` or `pip3`, namely:
 
 ```bash
 pip install reasoner-validator
 ```
 
+If you want to install it with the extra dependencies for using it as a web service, you can use:
+
+```bash
+pip install "reasoner-validator[web]"
+```
+
 ## Installing and working with the module locally from source
 
 As of release 3.1.6, this project uses the [poetry dependency management](https://python-poetry.org) tool to orchestrate its installation and dependencies.
 
 After [installing poetry](https://python-poetry.org/docs/#installation) and cloning the project, the poetry installation may be run:
 
 ```bash
 git clone https://github.com/NCATSTranslator/reasoner-validator.git
 cd reasoner-validator
 poetry install
 ```
 
+To develop this package, install with all extras dependencies using:
+
+```bash
+poetry install --all-extras
+```
+
 ## Running Validation against an ARS UUID Result(*)
 
-A local script **`ars_uuid_result_test_runner.py`** is available to run TRAPI Response validation against a UUID indexed query result of the Biomedical Knowledge Translator "Autonomous Relay System" (ARS).
+A local script **`ars_uuid_result_test_runner.py`** is available to run TRAPI Response validation against a 
+UUID indexed query result of the Biomedical Knowledge Translator "Autonomous Relay System" (ARS).
 
 For usage, type:
 
 ```bash
 ./ars_uuid_result_test_runner.py --help
 ```
 
 (*) Thank you Eric Deutsch for the prototype of this script
 
+## Running tests
+
+To run the test locally install with the `dev` dependencies group if not already done:
+
+```bash
+poetry install --extras dev
+```
+
+Run the tests with coverage report:
+
+```bash
+poetry run pytest --cov
+```
+
+Run the tests with detailed coverage report in a HTML page:
+
+```bash
+poetry run pytest --cov --cov-report html
+```
+
+Serve the report on http://localhost:3000:
+
+```bash
+python -m http.server 3000 --directory ./htmlcov
+```
+
 ## Building the Documentation Locally
 
 All paths here are relative to the root project directory.
 
 First install the documentation-specific dependencies.
 
 ```bash
@@ -119,36 +163,42 @@
 
 ### API
 
 The web service has a single POST endpoint `/validate` taking a simple JSON request body, as follows:
 
 ```json
 {
-  "trapi_version": "1.3.0",
-  "biolink_version": "3.2.1",
+  "trapi_version": "1.4.0-beta",
+  "biolink_version": "3.2.6",
   "sources": {
     "ara_source": "infores:aragorn",
     "kp_source": "infores:panther",
     "kp_source_type": "primary"
   },
   "strict_validation": true,
-  "message": {...}
+  "response": {<some full JSON object of a TRAPI query Response...>}
 }
 ```
 
 The request body consists of JSON data structure with two top level tag:
 
 - An **optional** `trapi_version` tag can be given a value of the TRAPI version against which the message will be validated, expressed as a SemVer string (defaults to 'latest' if omitted; partial SemVer strings are resolved to their 'latest' minor and patch releases). 
 - An **optional** `biolink_version` tag can be given a value of the Biolink Model version against which the message knowledge graph semantic contents will be validated, expressed as a SemVer string (defaults to 'latest' Biolink Model Toolkit supported version, if omitted). 
 - An **optional** `sources` with an object dictionary (example shown) specifying the ARA and KP sources involved in the TRAPI call (specified by infores CURIE) and the expected KP provenance source type, i.e. 'primary' implies that the KP is tagged as a 'biolink:primary_knowledge_source'. Optional in that the root "sources" or any of the subsidiary tags may be omitted (default to None)
 - An **optional** `strict_validation` flag (default: None or 'false'). If 'true' then follow strict validation rules, such as treating as 'error' states the use of `category`, `predicate` and `attribute_type_id` that are of type `abstract` or `mixin`  as errors. 
-- A **mandatory** `message` tag should have as its value the complete TRAPI **Message** JSON data structure to be validated (see example below).
+- A **mandatory** `message` tag should have as its value the complete JSON TRAPI **Response** to be validated (See the example below)
 
 ### Running the Web Service Directly
 
+First install the web-specific dependencies.
+
+```bash
+poetry install --extras web
+```
+
 The service may be run directly as a Python module. The web services module may be directly run, as follows. 
 
 ```shell
 python -m api.main
 ```
 
 Note that [poetry automatically uses any existing virtual environment](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment), but you can otherwise also enter the one that is created by poetry by default:
@@ -159,15 +209,15 @@
 exit  # exit the poetry shell
 ```
 
 Go to  http://localhost/docs to see the service documentation and to use the simple UI to input TRAPI messages for validation.
 
 ### Typical Output
 
-As an example of the kind of output to expect, if one posts the following JSON message data to the **/validate** endpoint:
+As an example of the kind of output to expect, if one posts the following TRAPI Response JSON data structure to the **/validate** endpoint:
 
 ```json
 {
   "trapi_version": "1.3.0",
   "biolink_version": "3.2.1",
   "response": {
       "message": {
```

