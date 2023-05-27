# Comparing `tmp/reasoner_validator-3.5.0.tar.gz` & `tmp/reasoner_validator-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.5.0.tar", max compression
+gzip compressed data, was "reasoner_validator-3.5.2.tar", max compression
```

## Comparing `reasoner_validator-3.5.0.tar` & `reasoner_validator-3.5.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1153 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/LICENSE
--rw-r--r--   0        0        0    12066 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/README.md
--rw-r--r--   0        0        0      131 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/Makefile
--rw-r--r--   0        0        0     2288 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/conf.py
--rw-r--r--   0        0        0    18216 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/index.rst
--rw-r--r--   0        0        0      795 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/make.bat
--rw-r--r--   0        0        0      136 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    36012 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2056 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/pyproject.toml
--rw-r--r--   0        0        0    20298 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    59678 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    39221 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0    26512 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4350 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0     6837 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    13781 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0     9165 2023-05-27 00:11:15.708252 reasoner_validator-3.5.0/reasoner_validator/versioning.py
--rw-r--r--   0        0        0        0 2023-05-27 00:11:15.712252 reasoner_validator-3.5.0/tests/__init__.py
--rw-r--r--   0        0        0   102228 2023-05-27 00:11:15.712252 reasoner_validator-3.5.0/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    31906 2023-05-27 00:11:15.712252 reasoner_validator-3.5.0/tests/test_response_validator.py
--rw-r--r--   0        0        0     4546 2023-05-27 00:11:15.712252 reasoner_validator-3.5.0/tests/test_semver.py
--rw-r--r--   0        0        0    26567 2023-05-27 00:11:15.712252 reasoner_validator-3.5.0/tests/test_validate.py
--rw-r--r--   0        0        0    19017 2023-05-27 00:11:15.712252 reasoner_validator-3.5.0/tests/test_validation_report.py
--rw-r--r--   0        0        0     2068 2023-05-27 00:11:15.712252 reasoner_validator-3.5.0/tests/test_workflows.py
--rw-r--r--   0        0        0    14105 1970-01-01 00:00:00.000000 reasoner_validator-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/LICENSE
+-rw-r--r--   0        0        0    12066 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/README.md
+-rw-r--r--   0        0        0      131 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/Makefile
+-rw-r--r--   0        0        0     2288 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/conf.py
+-rw-r--r--   0        0        0    18216 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    36025 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2093 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/pyproject.toml
+-rw-r--r--   0        0        0    20298 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    59678 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    39243 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0    26512 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4350 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0     7035 2023-05-27 03:34:04.809362 reasoner_validator-3.5.2/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    13781 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0     9165 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0        0 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/tests/__init__.py
+-rw-r--r--   0        0        0   102228 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    31906 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/tests/test_response_validator.py
+-rw-r--r--   0        0        0     4546 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/tests/test_semver.py
+-rw-r--r--   0        0        0    26567 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/tests/test_validate.py
+-rw-r--r--   0        0        0    19013 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2068 2023-05-27 03:34:04.813362 reasoner_validator-3.5.2/tests/test_workflows.py
+-rw-r--r--   0        0        0    14105 1970-01-01 00:00:00.000000 reasoner_validator-3.5.2/PKG-INFO
```

### Comparing `reasoner_validator-3.5.0/LICENSE` & `reasoner_validator-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/README.md` & `reasoner_validator-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/docs/Makefile` & `reasoner_validator-3.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/docs/conf.py` & `reasoner_validator-3.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/docs/index.rst` & `reasoner_validator-3.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/docs/make.bat` & `reasoner_validator-3.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/docs/validation_codes_dictionary.md` & `reasoner_validator-3.5.2/docs/validation_codes_dictionary.md`

 * *Files 0% similar despite different names*

```diff
@@ -290,19 +290,19 @@
 
 **Context:** identifier, biolink_release
 
 **Description:** This knowledge statement is not compliant to the specified release of the Biolink Model. Review associated messages for underlying cause!
 
 ### error.trapi.validation
 
-**Message:** Schema validation exception
+**Message:** Schema validation error
 
-**Context:** identifier, reason
+**Context:** identifier, component, reason
 
-**Description:** TRAPI query attempt triggered an abnormal server exception as noted.
+**Description:** JSON Schema validation error reported for specified TRAPI query component.
 
 ### error.trapi.request.invalid
 
 **Message:** Test could not generate a valid TRAPI query request object using identified element
 
 **Context:** identifier, test, reason
```

### Comparing `reasoner_validator-3.5.0/pyproject.toml` & `reasoner_validator-3.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.5.0"
+version = "3.5.2"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
-    "Kenneth Morton <kenneth kenny@covar.com>"
+    "Kenneth Morton <kenneth kenny@covar.com>",
+    "Sierra Moxon <smoxon@lbl.gov>"
 ]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/NCATSTranslator"
 repository = "https://github.com/NCATSTranslator/reasoner-validator"
 documentation = "https://translator-reasoner-validator.readthedocs.io/en/latest/"
```

### Comparing `reasoner_validator-3.5.0/reasoner_validator/__init__.py` & `reasoner_validator-3.5.2/reasoner_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.5.2/reasoner_validator/biolink/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/reasoner_validator/codes.yaml` & `reasoner_validator-3.5.2/reasoner_validator/codes.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -252,19 +252,20 @@
     $message: "S-P-O statement is not compliant to Biolink Model release"
     $context:
       - identifier
       - biolink_release
     $description: "This knowledge statement is not compliant to the specified release of the Biolink Model. Review associated messages for underlying cause!"
   trapi:
     validation:
-      $message: "Schema validation exception"
+      $message: "Schema validation error"
       $context:
         - identifier
+        - component
         - reason
-      $description: "TRAPI query attempt triggered an abnormal server exception as noted."
+      $description: "JSON Schema validation error reported for specified TRAPI query component."
     request:
       invalid:
         $message: "Test could not generate a valid TRAPI query request object using identified element"
         $context:
           - identifier
           - test
           - reason
```

### Comparing `reasoner_validator-3.5.0/reasoner_validator/report.py` & `reasoner_validator-3.5.2/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/reasoner_validator/sri/util.py` & `reasoner_validator-3.5.2/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.5.2/reasoner_validator/trapi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 
         Examples
         --------
         >>> TRAPISchemaValidator(trapi_version="1.3.0").validate({"message": {}}, "QGraph")
 
         """
         schema = load_schema(self.trapi_version)[component]
-        print("instance", instance)
+        # print("instance", instance)
         jsonschema.validate(instance, schema)
 
     def is_valid_trapi_query(self, instance, component: str = "Query"):
         """Make sure that the Message is a syntactically valid TRAPI Query JSON object.
 
         Parameters
         ----------
@@ -185,15 +185,19 @@
         """
         try:
             self.validate(
                 instance=instance,
                 component=component
             )
         except jsonschema.ValidationError as e:
-            self.report(code="error.trapi.validation", identifier=self.trapi_version, reason=e.message)
+            if len(e.message) <= 160:
+                reason = e.message
+            else:
+                reason = e.message[0:49] + " "*5 + "... " + " "*5 + e.message[-100:-1]
+            self.report(code="error.trapi.validation", identifier=self.trapi_version, component=component, reason=reason)
 
 
 def check_trapi_validity(instance, trapi_version: str, component: str = "Query") -> TRAPISchemaValidator:
     """
     Checks schema compliance of a Query component against a given TRAPI version.
 
     Parameters
```

### Comparing `reasoner_validator-3.5.0/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.5.2/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/reasoner_validator/validation_codes.py` & `reasoner_validator-3.5.2/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/reasoner_validator/versioning.py` & `reasoner_validator-3.5.2/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.5.2/tests/test_biolink_compliance_validation.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/tests/test_response_validator.py` & `reasoner_validator-3.5.2/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/tests/test_semver.py` & `reasoner_validator-3.5.2/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/tests/test_validate.py` & `reasoner_validator-3.5.2/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/tests/test_validation_report.py` & `reasoner_validator-3.5.2/tests/test_validation_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,15 +298,15 @@
            "Node identifier found unmapped to target categories for node" in warnings
 
     assert "errors" in messages
     assert len(messages['errors']) > 0
     errors: List[str] = list()
     for code, parameters in messages['errors'].items():
         errors.extend(CodeDictionary.display(code, parameters, add_prefix=True))
-    assert "ERROR - Trapi: Schema validation exception" in errors
+    assert "ERROR - Trapi: Schema validation error" in errors
     
     obj = reporter1.to_dict()
     assert obj["trapi_version"] == TEST_TRAPI_VERSION
     assert obj["biolink_version"] == TEST_BIOLINK_VERSION
     assert "messages" in obj
     assert "errors" in obj["messages"]
     assert "error.trapi.validation" in obj["messages"]["errors"]
```

### Comparing `reasoner_validator-3.5.0/tests/test_workflows.py` & `reasoner_validator-3.5.2/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.0/PKG-INFO` & `reasoner_validator-3.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.5.0
+Version: 3.5.2
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

