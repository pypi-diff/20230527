# Comparing `tmp/linkml_transformer-0.1.4.tar.gz` & `tmp/linkml_transformer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml_transformer-0.1.4.tar", max compression
+gzip compressed data, was "linkml_transformer-0.1.5.tar", max compression
```

## Comparing `linkml_transformer-0.1.4.tar` & `linkml_transformer-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     4047 2023-05-03 23:35:01.794835 linkml_transformer-0.1.4/README.md
--rw-r--r--   0        0        0      742 2023-05-03 23:35:40.643670 linkml_transformer-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/cli/__init__.py
--rw-r--r--   0        0        0     3627 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/cli/cli.py
--rw-r--r--   0        0        0       61 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/compiler/__init__.py
--rw-r--r--   0        0        0      463 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/compiler/awk_compiler.py
--rw-r--r--   0        0        0     1124 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/compiler/compiler.py
--rw-r--r--   0        0        0     2353 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/compiler/python_compiler.py
--rw-r--r--   0        0        0      399 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/compiler/r2rml_compiler.py
--rw-r--r--   0        0        0      411 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/compiler/sparql_compiler.py
--rw-r--r--   0        0        0      427 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/compiler/sql_compiler.py
--rw-r--r--   0        0        0      476 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/compiler/sssom_compiler.py
--rw-r--r--   0        0        0      480 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/datamodel/specification_view.py
--rw-r--r--   0        0        0    12387 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/datamodel/transformer_model.py
--rw-r--r--   0        0        0     7874 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/datamodel/transformer_model.yaml
--rw-r--r--   0        0        0        0 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/importer/__init__.py
--rw-r--r--   0        0        0      642 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/importer/importer.py
--rw-r--r--   0        0        0        0 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/schema_mapper/__init__.py
--rw-r--r--   0        0        0     5265 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/schema_mapper/schema_mapper.py
--rw-r--r--   0        0        0        0 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/transformer/__init__.py
--rw-r--r--   0        0        0     1373 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/transformer/inference.py
--rw-r--r--   0        0        0     6691 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/transformer/object_transformer.py
--rw-r--r--   0        0        0      247 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/transformer/rdflib_transformer.py
--rw-r--r--   0        0        0     5753 2023-05-03 23:35:01.810835 linkml_transformer-0.1.4/src/linkml_transformer/transformer/transformer.py
--rw-r--r--   0        0        0        0 2023-05-03 23:35:01.810835 linkml_transformer-0.1.4/src/linkml_transformer/utils/__init__.py
--rw-r--r--   0        0        0     1306 2023-05-03 23:35:01.810835 linkml_transformer-0.1.4/src/linkml_transformer/utils/dynamic_object.py
--rw-r--r--   0        0        0      242 2023-05-03 23:35:01.810835 linkml_transformer-0.1.4/src/linkml_transformer/utils/inverter.py
--rw-r--r--   0        0        0      783 2023-05-03 23:35:01.810835 linkml_transformer-0.1.4/src/linkml_transformer/utils/loaders.py
--rw-r--r--   0        0        0     9492 2023-05-03 23:35:01.810835 linkml_transformer-0.1.4/src/linkml_transformer/utils/multi_file_transformer.py
--rw-r--r--   0        0        0     4530 1970-01-01 00:00:00.000000 linkml_transformer-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4047 2023-05-27 01:43:12.205126 linkml_transformer-0.1.5/README.md
+-rw-r--r--   0        0        0      762 2023-05-27 01:44:01.305289 linkml_transformer-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/cli/__init__.py
+-rw-r--r--   0        0        0     3627 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/cli/cli.py
+-rw-r--r--   0        0        0       61 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/compiler/__init__.py
+-rw-r--r--   0        0        0      463 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/compiler/awk_compiler.py
+-rw-r--r--   0        0        0     1124 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/compiler/compiler.py
+-rw-r--r--   0        0        0     2915 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/compiler/python_compiler.py
+-rw-r--r--   0        0        0      399 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/compiler/r2rml_compiler.py
+-rw-r--r--   0        0        0      411 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/compiler/sparql_compiler.py
+-rw-r--r--   0        0        0      427 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/compiler/sql_compiler.py
+-rw-r--r--   0        0        0      476 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/compiler/sssom_compiler.py
+-rw-r--r--   0        0        0      480 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/datamodel/specification_view.py
+-rw-r--r--   0        0        0    12387 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/datamodel/transformer_model.py
+-rw-r--r--   0        0        0     7874 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/datamodel/transformer_model.yaml
+-rw-r--r--   0        0        0        0 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/importer/__init__.py
+-rw-r--r--   0        0        0      642 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/importer/importer.py
+-rw-r--r--   0        0        0        0 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/schema_mapper/__init__.py
+-rw-r--r--   0        0        0     5265 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/schema_mapper/schema_mapper.py
+-rw-r--r--   0        0        0        0 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/transformer/__init__.py
+-rw-r--r--   0        0        0     6754 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/transformer/eval_utils.py
+-rw-r--r--   0        0        0     1373 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/transformer/inference.py
+-rw-r--r--   0        0        0     7792 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/transformer/object_transformer.py
+-rw-r--r--   0        0        0      247 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/transformer/rdflib_transformer.py
+-rw-r--r--   0        0        0     5753 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/transformer/transformer.py
+-rw-r--r--   0        0        0        0 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/utils/__init__.py
+-rw-r--r--   0        0        0     1306 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/utils/dynamic_object.py
+-rw-r--r--   0        0        0      242 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/utils/inverter.py
+-rw-r--r--   0        0        0      783 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/utils/loaders.py
+-rw-r--r--   0        0        0     9492 2023-05-27 01:43:12.225126 linkml_transformer-0.1.5/src/linkml_transformer/utils/multi_file_transformer.py
+-rw-r--r--   0        0        0     4572 1970-01-01 00:00:00.000000 linkml_transformer-0.1.5/PKG-INFO
```

### Comparing `linkml_transformer-0.1.4/README.md` & `linkml_transformer-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.1.4/pyproject.toml` & `linkml_transformer-0.1.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "linkml-transformer"
-version = "v0.1.4"
+version = "v0.1.5"
 description = ""
 authors = ["cmungall <cjm@berkeleybop.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 linkml-runtime = ">=1.5.2"
+asteval = "^0.9.29"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 linkml = ">=1.5.0"
 mkdocs-mermaid2-plugin = "^0.6.0"
```

### Comparing `linkml_transformer-0.1.4/src/linkml_transformer/cli/cli.py` & `linkml_transformer-0.1.5/src/linkml_transformer/cli/cli.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.1.4/src/linkml_transformer/compiler/compiler.py` & `linkml_transformer-0.1.5/src/linkml_transformer/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.1.4/src/linkml_transformer/compiler/python_compiler.py` & `linkml_transformer-0.1.5/src/linkml_transformer/compiler/python_compiler.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,29 +21,49 @@
 {% macro gen_slot_derivation(sd, force_singlevalued=False) -%}
 {%- if not force_singlevalued and sd.populated_from and induced_slots[sd.populated_from].multivalued -%}
  [ {{ gen_slot_derivation_value(sd, "x") }} for x in {{ gen_slot_derivation(sd, force_singlevalued=True) }} ]
 {%- else -%}
  {%- if sd.populated_from -%}
   source_object.{{ sd.populated_from }}
  {%- elif sd.expr -%}
+  {%- if '\n' in sd.expr -%}
+ gen_{{ sd.name }}(source_object)
+  {%- elif '{' in sd.expr and '}' in sd.expr -%}
+  {{ sd.expr|replace('{', '')|replace('}', '') }}
+  {%- else -%}
   {{ sd.expr }}
+  {%- endif -%}
  {%- else -%}
   None
  {%- endif -%}
 {%- endif -%}
 {%- endmacro %}
+{% macro gen_slot_derivation_defs(sd) -%}
+{% if sd.expr and '\n' in sd.expr %}
+
+    def gen_{{ sd.name }}(src):
+        target = None
+   {%- for line in sd.expr.split('\n') %}
+        {{ line }}
+   {%- endfor -%}
+        return target
+{% endif %}
+{%- endmacro %}
 def derive_{{ cd.name }}(
         source_object: {{ source_module }}.{{ cd.populated_from }}
     ) -> {{ target_module }}.{{ cd.name }}:
+{%-  for sd in cd.slot_derivations.values() -%}
+    {{  gen_slot_derivation_defs(sd) }}
+{%-  endfor %}
+
     return {{ cd.populated_from }}(
-       {%- for sd in cd.slot_derivations.values() %}
-       {{ sd.name }}={{ gen_slot_derivation(sd) }},
-       {%- endfor %}
+        {%- for sd in cd.slot_derivations.values() %}
+        {{ sd.name }}={{ gen_slot_derivation(sd) }},
+        {%- endfor %}
     )
-
 """
 
 
 class PythonCompiler(Compiler):
     """
     Compiles a Transformation Specification to Python code.
     """
```

### Comparing `linkml_transformer-0.1.4/src/linkml_transformer/datamodel/transformer_model.py` & `linkml_transformer-0.1.5/src/linkml_transformer/datamodel/transformer_model.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.1.4/src/linkml_transformer/datamodel/transformer_model.yaml` & `linkml_transformer-0.1.5/src/linkml_transformer/datamodel/transformer_model.yaml`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.1.4/src/linkml_transformer/importer/importer.py` & `linkml_transformer-0.1.5/src/linkml_transformer/importer/importer.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.1.4/src/linkml_transformer/schema_mapper/schema_mapper.py` & `linkml_transformer-0.1.5/src/linkml_transformer/schema_mapper/schema_mapper.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.1.4/src/linkml_transformer/transformer/inference.py` & `linkml_transformer-0.1.5/src/linkml_transformer/transformer/inference.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.1.4/src/linkml_transformer/transformer/object_transformer.py` & `linkml_transformer-0.1.5/src/linkml_transformer/transformer/object_transformer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
 from dataclasses import dataclass
 from typing import Any, Dict, Optional, Type, Union
 
+from asteval import Interpreter
 from linkml_runtime.index.object_index import ObjectIndex
-from linkml_runtime.utils.eval_utils import eval_expr
 from linkml_runtime.utils.yamlutils import YAMLRoot
 from pydantic import BaseModel
 
+from linkml_transformer.transformer.eval_utils import eval_expr
 from linkml_transformer.transformer.transformer import OBJECT_TYPE, Transformer
 from linkml_transformer.utils.dynamic_object import dynamic_object
 
 DICT_OBJ = Dict[str, Any]
 
 
 logger = logging.getLogger(__name__)
@@ -50,17 +51,18 @@
         source_obj: OBJECT_TYPE,
         source_type: str = None,
         target_type: str = None,
     ) -> Union[DICT_OBJ, Any]:
         """
         Transform a source object into a target object.
 
-        :param source_obj:
-        :param source_type:
-        :return:
+        :param source_obj: source data structure
+        :param source_type: name of the object type to cast the source object as
+        :param target_type: type to return the transformed object as
+        :return: transformed data, either as type target_type or a dictionary
         """
         sv = self.source_schemaview
         if source_type is None:
             [source_type] = [c.name for c in sv.all_classes().values() if c.tree_root]
         if source_type in sv.all_types():
             if target_type:
                 if target_type == "string":
@@ -73,19 +75,18 @@
                     return self.expand_curie(source_obj)
                 elif target_type == "curie":
                     return self.compress_uri(source_obj)
             return source_obj
         if source_type in sv.all_enums():
             # TODO: enum derivations
             return str(source_obj)
+        source_obj_typed = None
         if isinstance(source_obj, (BaseModel, YAMLRoot)):
             source_obj_typed = source_obj
             source_obj = vars(source_obj)
-        else:
-            source_obj_typed = None
         if not isinstance(source_obj, dict):
             logger.warning(f"Unexpected: {source_obj} for type {source_type}")
             return source_obj
         class_deriv = self._get_class_derivation(source_type)
         tgt_attrs = {}
         for slot_derivation in class_deriv.slot_derivations.values():
             v = None
@@ -106,16 +107,24 @@
                     ctxt_dict = {
                         k: getattr(ctxt_obj, k)
                         for k in ctxt_obj._attributes()
                         if not k.startswith("_")
                     }
                 else:
                     do = dynamic_object(source_obj, sv, source_type)
+                    ctxt_obj = do
                     ctxt_dict = vars(do)
-                v = eval_expr(slot_derivation.expr, **ctxt_dict, NULL=None)
+
+                try:
+                    v = eval_expr(slot_derivation.expr, **ctxt_dict, NULL=None)
+                except Exception:
+                    aeval = Interpreter(usersyms={"src": ctxt_obj, "target": None})
+                    aeval(slot_derivation.expr)
+                    v = aeval.symtable["target"]
+
             else:
                 source_class_slot = sv.induced_slot(slot_derivation.name, source_type)
                 v = source_obj.get(slot_derivation.name, None)
             if source_class_slot and v is not None:
                 target_range = slot_derivation.range
                 source_class_slot_range = source_class_slot.range
                 if source_class_slot.multivalued:
@@ -146,17 +155,30 @@
         return tgt_attrs
 
     def transform_object(
         self,
         source_obj: Union[YAMLRoot, BaseModel],
         target_class: Optional[Union[Type[YAMLRoot], Type[BaseModel]]] = None,
     ) -> Union[YAMLRoot, BaseModel]:
-        typ = type(source_obj)
-        typ_name = typ.__name__
+        """
+        Transform an object into an object of class target_class.
+
+        :param source_obj: source object
+        :type source_obj: Union[YAMLRoot, BaseModel]
+        :param target_class: class to transform the object into, defaults to None
+        :type target_class: Optional[Union[Type[YAMLRoot], Type[BaseModel]]], optional
+        :return: transformed object of class target_class
+        :rtype: Union[YAMLRoot, BaseModel]
+        """
+        if not target_class:
+            raise ValueError("No target_class specified for transform_object")
+
+        source_type = type(source_obj)
+        source_type_name = source_type.__name__
         # if isinstance(source_obj, YAMLRoot):
         #    source_obj_dict = json_dumper.to_dict(source_obj)
         # elif isinstance(source_obj, BaseModel):
         #    source_obj_dict = source_obj.dict()
         # else:
         #    raise ValueError(f"Do not know how to handle type: {typ}")
-        tr_obj_dict = self.transform(source_obj, typ_name)
+        tr_obj_dict = self.transform(source_obj, source_type_name)
         return target_class(**tr_obj_dict)
```

### Comparing `linkml_transformer-0.1.4/src/linkml_transformer/transformer/transformer.py` & `linkml_transformer-0.1.5/src/linkml_transformer/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.1.4/src/linkml_transformer/utils/dynamic_object.py` & `linkml_transformer-0.1.5/src/linkml_transformer/utils/dynamic_object.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.1.4/src/linkml_transformer/utils/loaders.py` & `linkml_transformer-0.1.5/src/linkml_transformer/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.1.4/src/linkml_transformer/utils/multi_file_transformer.py` & `linkml_transformer-0.1.5/src/linkml_transformer/utils/multi_file_transformer.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.1.4/PKG-INFO` & `linkml_transformer-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: linkml-transformer
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: asteval (>=0.9.29,<0.10.0)
 Requires-Dist: linkml-runtime (>=1.5.2)
 Description-Content-Type: text/markdown
 
 # linkml-transformer
 
 __Status__: pre-alpha code
```

