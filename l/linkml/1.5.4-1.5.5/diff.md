# Comparing `tmp/linkml-1.5.4.tar.gz` & `tmp/linkml-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml-1.5.4.tar", max compression
+gzip compressed data, was "linkml-1.5.5.tar", max compression
```

## Comparing `linkml-1.5.4.tar` & `linkml-1.5.5.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     6555 2023-05-26 20:00:09.694554 linkml-1.5.4/LICENSE
--rw-r--r--   0        0        0     1369 2023-05-26 20:00:09.694554 linkml-1.5.4/README.md
--rw-r--r--   0        0        0     3227 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/__init__.py
--rw-r--r--   0        0        0      326 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/_version.py
--rw-r--r--   0        0        0    51005 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/PythonGenNotes.md
--rw-r--r--   0        0        0     4158 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/README.md
--rw-r--r--   0        0        0      616 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/common/__init__.py
--rw-r--r--   0        0        0     2040 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/common/type_designators.py
--rw-r--r--   0        0        0     3118 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/csvgen.py
--rw-r--r--   0        0        0     2873 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/class.md.jinja2
--rw-r--r--   0        0        0     2682 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/class_diagram.md.jinja2
--rw-r--r--   0        0        0     1321 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/common_metadata.md.jinja2
--rw-r--r--   0        0        0     1018 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/enum.md.jinja2
--rw-r--r--   0        0        0     1466 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/index.md.jinja2
--rw-r--r--   0        0        0      501 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/index.tex.jinja2
--rw-r--r--   0        0        0       70 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/schema.md.jinja2
--rw-r--r--   0        0        0     2557 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/slot.md.jinja2
--rw-r--r--   0        0        0     1704 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/subset.md.jinja2
--rw-r--r--   0        0        0      635 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen/type.md.jinja2
--rw-r--r--   0        0        0    32994 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/docgen.py
--rw-r--r--   0        0        0     5112 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/dotgen.py
--rw-r--r--   0        0        0    10913 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/erdiagramgen.py
--rw-r--r--   0        0        0     6894 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/excelgen.py
--rw-r--r--   0        0        0     6393 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/golanggen.py
--rw-r--r--   0        0        0     3575 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/golrgen.py
--rw-r--r--   0        0        0     2347 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/graphqlgen.py
--rw-r--r--   0        0        0      444 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/javagen/example_template.java.jinja2
--rw-r--r--   0        0        0     1737 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/javagen/java_record_template.jinja2
--rw-r--r--   0        0        0     5499 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/javagen.py
--rw-r--r--   0        0        0     8821 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/jsonldcontextgen.py
--rw-r--r--   0        0        0     7952 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/jsonldgen.py
--rw-r--r--   0        0        0    21688 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/jsonschemagen.py
--rw-r--r--   0        0        0     3555 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/linkmlgen.py
--rw-r--r--   0        0        0    34422 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/markdowngen.py
--rw-r--r--   0        0        0     6532 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/namespacegen.py
--rw-r--r--   0        0        0     7831 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/oocodegen.py
--rw-r--r--   0        0        0    27365 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/owlgen.py
--rw-r--r--   0        0        0     4911 2023-05-26 20:00:09.714554 linkml-1.5.4/linkml/generators/prefixmapgen.py
--rw-r--r--   0        0        0     9811 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/projectgen.py
--rw-r--r--   0        0        0     2443 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/protogen.py
--rw-r--r--   0        0        0    22150 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/pydanticgen.py
--rw-r--r--   0        0        0    50389 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/pythongen.py
--rw-r--r--   0        0        0     2825 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/rdfgen.py
--rw-r--r--   0        0        0     5621 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/shaclgen.py
--rw-r--r--   0        0        0     9547 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/shexgen.py
--rw-r--r--   0        0        0     6632 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/sparqlgen.py
--rw-r--r--   0        0        0      166 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2575 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py
--rw-r--r--   0        0        0     1625 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py
--rw-r--r--   0        0        0     9334 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/sqlalchemygen.py
--rw-r--r--   0        0        0    18626 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/sqlddlgen.py
--rw-r--r--   0        0        0    11387 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/sqltablegen.py
--rw-r--r--   0        0        0     7177 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/sssomgen.py
--rw-r--r--   0        0        0     1788 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/string_template.md
--rw-r--r--   0        0        0     3020 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/summarygen.py
--rw-r--r--   0        0        0     4760 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/terminusdbgen.py
--rw-r--r--   0        0        0     6094 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/typescriptgen.py
--rw-r--r--   0        0        0     1746 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/yamlgen.py
--rw-r--r--   0        0        0    13311 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/generators/yumlgen.py
--rw-r--r--   0        0        0        0 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/__init__.py
--rw-r--r--   0        0        0     4323 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/cli.py
--rw-r--r--   0        0        0      292 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/config/datamodel/.linkmllint.yaml
--rw-r--r--   0        0        0        0 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/config/datamodel/__init__.py
--rw-r--r--   0        0        0    17711 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/config/datamodel/config.py
--rw-r--r--   0        0        0     6980 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/config/datamodel/config.yaml
--rw-r--r--   0        0        0      540 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/config/default.yaml
--rw-r--r--   0        0        0      198 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/config/recommended.yaml
--rw-r--r--   0        0        0      269 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/formatters/__init__.py
--rw-r--r--   0        0        0      518 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/formatters/formatter.py
--rw-r--r--   0        0        0      767 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/formatters/json_formatter.py
--rw-r--r--   0        0        0     2605 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/formatters/markdown_formatter.py
--rw-r--r--   0        0        0     2085 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/formatters/terminal_formatter.py
--rw-r--r--   0        0        0      871 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/formatters/tsv_formatter.py
--rw-r--r--   0        0        0     5004 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/linter.py
--rw-r--r--   0        0        0    11649 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/linter/rules.py
--rw-r--r--   0        0        0       55 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/reporting/__init__.py
--rw-r--r--   0        0        0     9189 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/reporting/model.py
--rw-r--r--   0        0        0        0 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/transformers/__init__.py
--rw-r--r--   0        0        0    18594 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/transformers/relmodel_transformer.py
--rw-r--r--   0        0        0     5455 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/transformers/schema_renamer.py
--rw-r--r--   0        0        0        0 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/__init__.py
--rw-r--r--   0        0        0     6463 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/converter.py
--rw-r--r--   0        0        0     4384 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/datautils.py
--rw-r--r--   0        0        0      490 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/datavalidator.py
--rw-r--r--   0        0        0     6999 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/execute_tutorial.py
--rw-r--r--   0        0        0    39737 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/generator.py
--rw-r--r--   0        0        0      445 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/helpers.py
--rw-r--r--   0        0        0     5773 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/ifabsent_functions.py
--rw-r--r--   0        0        0     9498 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/mergeutils.py
--rw-r--r--   0        0        0     4560 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/rawloader.py
--rw-r--r--   0        0        0     9065 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/schema_builder.py
--rw-r--r--   0        0        0    13464 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/schema_fixer.py
--rw-r--r--   0        0        0    48537 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/schemaloader.py
--rw-r--r--   0        0        0    19733 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/schemasynopsis.py
--rw-r--r--   0        0        0    16297 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/sqlutils.py
--rw-r--r--   0        0        0     2395 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/typereferences.py
--rw-r--r--   0        0        0     1514 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/utils/validation.py
--rw-r--r--   0        0        0      140 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/validators/__init__.py
--rw-r--r--   0        0        0     6255 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/validators/jsonschemavalidator.py
--rw-r--r--   0        0        0     4873 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/validators/sparqlvalidator.py
--rw-r--r--   0        0        0        0 2023-05-26 20:00:09.718554 linkml-1.5.4/linkml/workspaces/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 20:00:09.722554 linkml-1.5.4/linkml/workspaces/datamodel/__init__.py
--rw-r--r--   0        0        0    15641 2023-05-26 20:00:09.722554 linkml-1.5.4/linkml/workspaces/datamodel/workspaces.py
--rw-r--r--   0        0        0     4233 2023-05-26 20:00:09.722554 linkml-1.5.4/linkml/workspaces/datamodel/workspaces.yaml
--rw-r--r--   0        0        0    11912 2023-05-26 20:00:09.722554 linkml-1.5.4/linkml/workspaces/example_runner.py
--rw-r--r--   0        0        0     4973 2023-05-26 20:00:40.366927 linkml-1.5.4/pyproject.toml
--rw-r--r--   0        0        0     6700 1970-01-01 00:00:00.000000 linkml-1.5.4/setup.py
--rw-r--r--   0        0        0     3847 1970-01-01 00:00:00.000000 linkml-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     6555 2023-05-27 01:45:11.889278 linkml-1.5.5/LICENSE
+-rw-r--r--   0        0        0     1369 2023-05-27 01:45:11.889278 linkml-1.5.5/README.md
+-rw-r--r--   0        0        0     3227 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/__init__.py
+-rw-r--r--   0        0        0      326 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/_version.py
+-rw-r--r--   0        0        0    51005 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/PythonGenNotes.md
+-rw-r--r--   0        0        0     4158 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/README.md
+-rw-r--r--   0        0        0      616 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/common/__init__.py
+-rw-r--r--   0        0        0     2040 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/common/type_designators.py
+-rw-r--r--   0        0        0     3118 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/csvgen.py
+-rw-r--r--   0        0        0     2873 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen/class.md.jinja2
+-rw-r--r--   0        0        0     2682 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen/class_diagram.md.jinja2
+-rw-r--r--   0        0        0     1321 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen/common_metadata.md.jinja2
+-rw-r--r--   0        0        0     1018 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen/enum.md.jinja2
+-rw-r--r--   0        0        0     1466 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen/index.md.jinja2
+-rw-r--r--   0        0        0      501 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen/index.tex.jinja2
+-rw-r--r--   0        0        0       70 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen/schema.md.jinja2
+-rw-r--r--   0        0        0     2557 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen/slot.md.jinja2
+-rw-r--r--   0        0        0     1704 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/docgen/subset.md.jinja2
+-rw-r--r--   0        0        0      635 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/docgen/type.md.jinja2
+-rw-r--r--   0        0        0    32994 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen.py
+-rw-r--r--   0        0        0     5112 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/dotgen.py
+-rw-r--r--   0        0        0    10913 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/erdiagramgen.py
+-rw-r--r--   0        0        0     6894 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/excelgen.py
+-rw-r--r--   0        0        0     6393 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/golanggen.py
+-rw-r--r--   0        0        0     3575 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/golrgen.py
+-rw-r--r--   0        0        0     2347 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/graphqlgen.py
+-rw-r--r--   0        0        0      444 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/javagen/example_template.java.jinja2
+-rw-r--r--   0        0        0     1737 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/javagen/java_record_template.jinja2
+-rw-r--r--   0        0        0     5499 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/javagen.py
+-rw-r--r--   0        0        0     8821 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/jsonldcontextgen.py
+-rw-r--r--   0        0        0     7952 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/jsonldgen.py
+-rw-r--r--   0        0        0    21688 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/jsonschemagen.py
+-rw-r--r--   0        0        0     3555 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/linkmlgen.py
+-rw-r--r--   0        0        0    34422 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/markdowngen.py
+-rw-r--r--   0        0        0     6532 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/namespacegen.py
+-rw-r--r--   0        0        0     7831 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/oocodegen.py
+-rw-r--r--   0        0        0    29182 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/owlgen.py
+-rw-r--r--   0        0        0     4911 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/prefixmapgen.py
+-rw-r--r--   0        0        0     9811 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/projectgen.py
+-rw-r--r--   0        0        0     2443 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/protogen.py
+-rw-r--r--   0        0        0    22150 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/pydanticgen.py
+-rw-r--r--   0        0        0    50389 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/pythongen.py
+-rw-r--r--   0        0        0     2825 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/rdfgen.py
+-rw-r--r--   0        0        0     5621 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/shaclgen.py
+-rw-r--r--   0        0        0     9547 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/shexgen.py
+-rw-r--r--   0        0        0     6632 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/sparqlgen.py
+-rw-r--r--   0        0        0      166 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2575 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py
+-rw-r--r--   0        0        0     1625 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py
+-rw-r--r--   0        0        0     9334 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/sqlalchemygen.py
+-rw-r--r--   0        0        0    18626 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/sqlddlgen.py
+-rw-r--r--   0        0        0    11387 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/sqltablegen.py
+-rw-r--r--   0        0        0     7177 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/sssomgen.py
+-rw-r--r--   0        0        0     1788 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/string_template.md
+-rw-r--r--   0        0        0     3020 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/summarygen.py
+-rw-r--r--   0        0        0     4760 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/terminusdbgen.py
+-rw-r--r--   0        0        0     6094 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/typescriptgen.py
+-rw-r--r--   0        0        0     1746 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/yamlgen.py
+-rw-r--r--   0        0        0    13311 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/yumlgen.py
+-rw-r--r--   0        0        0        0 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/__init__.py
+-rw-r--r--   0        0        0     4323 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/cli.py
+-rw-r--r--   0        0        0      292 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/config/datamodel/.linkmllint.yaml
+-rw-r--r--   0        0        0        0 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/config/datamodel/__init__.py
+-rw-r--r--   0        0        0    17711 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/config/datamodel/config.py
+-rw-r--r--   0        0        0     6980 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/config/datamodel/config.yaml
+-rw-r--r--   0        0        0      540 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/config/default.yaml
+-rw-r--r--   0        0        0      198 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/config/recommended.yaml
+-rw-r--r--   0        0        0      269 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/formatters/__init__.py
+-rw-r--r--   0        0        0      518 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/formatters/formatter.py
+-rw-r--r--   0        0        0      767 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/formatters/json_formatter.py
+-rw-r--r--   0        0        0     2605 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/formatters/markdown_formatter.py
+-rw-r--r--   0        0        0     2085 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/formatters/terminal_formatter.py
+-rw-r--r--   0        0        0      871 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/formatters/tsv_formatter.py
+-rw-r--r--   0        0        0     5004 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/linter.py
+-rw-r--r--   0        0        0    11649 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/rules.py
+-rw-r--r--   0        0        0       55 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/reporting/__init__.py
+-rw-r--r--   0        0        0     9189 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/reporting/model.py
+-rw-r--r--   0        0        0        0 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/transformers/__init__.py
+-rw-r--r--   0        0        0    18594 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/transformers/relmodel_transformer.py
+-rw-r--r--   0        0        0     5455 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/transformers/schema_renamer.py
+-rw-r--r--   0        0        0        0 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/__init__.py
+-rw-r--r--   0        0        0     6463 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/converter.py
+-rw-r--r--   0        0        0     4384 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/datautils.py
+-rw-r--r--   0        0        0      490 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/datavalidator.py
+-rw-r--r--   0        0        0     6999 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/execute_tutorial.py
+-rw-r--r--   0        0        0    39737 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/generator.py
+-rw-r--r--   0        0        0      445 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/helpers.py
+-rw-r--r--   0        0        0     5773 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/ifabsent_functions.py
+-rw-r--r--   0        0        0     9498 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/mergeutils.py
+-rw-r--r--   0        0        0     4560 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/rawloader.py
+-rw-r--r--   0        0        0     9065 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/schema_builder.py
+-rw-r--r--   0        0        0    13464 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/schema_fixer.py
+-rw-r--r--   0        0        0    48537 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/schemaloader.py
+-rw-r--r--   0        0        0    19733 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/schemasynopsis.py
+-rw-r--r--   0        0        0    16297 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/sqlutils.py
+-rw-r--r--   0        0        0     2395 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/typereferences.py
+-rw-r--r--   0        0        0     1514 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/validation.py
+-rw-r--r--   0        0        0      140 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/validators/__init__.py
+-rw-r--r--   0        0        0     6255 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/validators/jsonschemavalidator.py
+-rw-r--r--   0        0        0     4873 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/validators/sparqlvalidator.py
+-rw-r--r--   0        0        0        0 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/workspaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/workspaces/datamodel/__init__.py
+-rw-r--r--   0        0        0    15641 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/workspaces/datamodel/workspaces.py
+-rw-r--r--   0        0        0     4233 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/workspaces/datamodel/workspaces.yaml
+-rw-r--r--   0        0        0    11912 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/workspaces/example_runner.py
+-rw-r--r--   0        0        0     4974 2023-05-27 01:45:45.953462 linkml-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0     6458 1970-01-01 00:00:00.000000 linkml-1.5.5/setup.py
+-rw-r--r--   0        0        0     3529 1970-01-01 00:00:00.000000 linkml-1.5.5/PKG-INFO
```

### Comparing `linkml-1.5.4/LICENSE` & `linkml-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/README.md` & `linkml-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/__init__.py` & `linkml-1.5.5/linkml/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/PythonGenNotes.md` & `linkml-1.5.5/linkml/generators/PythonGenNotes.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/README.md` & `linkml-1.5.5/linkml/generators/README.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/__init__.py` & `linkml-1.5.5/linkml/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/common/type_designators.py` & `linkml-1.5.5/linkml/generators/common/type_designators.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/csvgen.py` & `linkml-1.5.5/linkml/generators/csvgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/docgen/class.md.jinja2` & `linkml-1.5.5/linkml/generators/docgen/class.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/docgen/class_diagram.md.jinja2` & `linkml-1.5.5/linkml/generators/docgen/class_diagram.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/docgen/common_metadata.md.jinja2` & `linkml-1.5.5/linkml/generators/docgen/common_metadata.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/docgen/enum.md.jinja2` & `linkml-1.5.5/linkml/generators/docgen/enum.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/docgen/index.md.jinja2` & `linkml-1.5.5/linkml/generators/docgen/index.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/docgen/slot.md.jinja2` & `linkml-1.5.5/linkml/generators/docgen/slot.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/docgen/subset.md.jinja2` & `linkml-1.5.5/linkml/generators/docgen/subset.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/docgen/type.md.jinja2` & `linkml-1.5.5/linkml/generators/docgen/type.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/docgen.py` & `linkml-1.5.5/linkml/generators/docgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/dotgen.py` & `linkml-1.5.5/linkml/generators/dotgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/erdiagramgen.py` & `linkml-1.5.5/linkml/generators/erdiagramgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/excelgen.py` & `linkml-1.5.5/linkml/generators/excelgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/golanggen.py` & `linkml-1.5.5/linkml/generators/golanggen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/golrgen.py` & `linkml-1.5.5/linkml/generators/golrgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/graphqlgen.py` & `linkml-1.5.5/linkml/generators/graphqlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/javagen/java_record_template.jinja2` & `linkml-1.5.5/linkml/generators/javagen/java_record_template.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/javagen.py` & `linkml-1.5.5/linkml/generators/javagen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/jsonldcontextgen.py` & `linkml-1.5.5/linkml/generators/jsonldcontextgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/jsonldgen.py` & `linkml-1.5.5/linkml/generators/jsonldgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/jsonschemagen.py` & `linkml-1.5.5/linkml/generators/jsonschemagen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/linkmlgen.py` & `linkml-1.5.5/linkml/generators/linkmlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/markdowngen.py` & `linkml-1.5.5/linkml/generators/markdowngen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/namespacegen.py` & `linkml-1.5.5/linkml/generators/namespacegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/oocodegen.py` & `linkml-1.5.5/linkml/generators/oocodegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/owlgen.py` & `linkml-1.5.5/linkml/generators/owlgen.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 model classes are translated to OWL classes, slots to OWL properties.
 """
 import logging
 import os
 from dataclasses import dataclass, field
 from enum import Enum, unique
-from typing import Optional, TextIO, Union, Set, List
+from typing import List, Optional, Set, TextIO, Union
 
 import click
 from linkml_runtime.linkml_model.meta import (ClassDefinition,
                                               ClassDefinitionName, Definition,
-                                              Element, EnumDefinition,
+                                              Element, ElementName,
+                                              EnumDefinition,
                                               EnumDefinitionName,
                                               SchemaDefinition, SlotDefinition,
                                               SlotDefinitionName,
                                               TypeDefinition,
                                               TypeDefinitionName)
 from linkml_runtime.utils.formatutils import camelcase, underscore
 from rdflib import OWL, RDF, BNode, Graph, Literal, URIRef
@@ -56,21 +57,23 @@
 
     `OWL Generator Docs <https://linkml.io/linkml/generators/owl>`_
 
     Attributes:
         type_objects    if True, represent TypeDefinitions as objects; if False, as literals
         metaclasses     if True, include OWL representations of ClassDefinition, SlotDefinition, etc. Introduces punning
     """
+
     schema: Union[str, TextIO, SchemaDefinition] = None
 
     # ClassVars
     generatorname = os.path.basename(__file__)
     generatorversion = "0.1.1"
     valid_formats = ["owl", "ttl"] + [
-        x.name for x in rdflib_plugins(None, rdflib_Parser) if "/" not in str(x.name)]
+        x.name for x in rdflib_plugins(None, rdflib_Parser) if "/" not in str(x.name)
+    ]
     visits_are_sorted = True
     uses_schemaloader = True
     requires_metamodel = True
 
     # ObjectVars
     metadata_profile: MetadataProfile = None
     ontology_uri_suffix: str = None
@@ -500,34 +503,77 @@
                     g.add((pv_uri, RDF.type, enum_uri))
         if all([pv is not None for pv in pv_uris]):
             union_bnode = BNode()
             Collection(self.graph, union_bnode, pv_uris)
             self.graph.add((enum_uri, OWL.unionOf, union_bnode))
 
     def _add_element_properties(self, uri: URIRef, el: Element) -> None:
+        metamodel = self.metamodel
         for k, v in el.__dict__.items():
-            if k in self.metamodel.schema.slots:
+            if k in metamodel.schema.slots:
                 defining_slot = self.metamodel.schema.slots[k]
-                if v is not None and ("owl" in defining_slot.in_subset or "OwlProfile" in defining_slot.in_subset):
-                    ve = v if isinstance(v, list) else [v]
+                if v is not None and (
+                    "owl" in defining_slot.in_subset
+                    or "OwlProfile" in defining_slot.in_subset
+                ):
+                    if isinstance(v, list):
+                        ve = v
+                    elif isinstance(v, dict):
+                        ve = v.values()
+                    else:
+                        ve = [v]
                     for e in ve:
+                        if isinstance(
+                            e,
+                            (
+                                ClassDefinition,
+                                SlotDefinition,
+                                TypeDefinition,
+                                EnumDefinition,
+                            ),
+                        ):
+                            return
                         if (
                             k == "name"
                             and isinstance(el, SlotDefinition)
                             and el.alias is not None
                         ):
                             prop_uri = RDFS.label
                             e = el.alias
                         else:
                             prop_uri = URIRef(
                                 self.metamodel.namespaces.uri_for(
                                     defining_slot.slot_uri
                                 )
                             )
-                        self.graph.add((uri, prop_uri, Literal(e)))
+                        object = self._as_rdf_element(e, defining_slot)
+                        if object is not None:
+                            self.graph.add((uri, prop_uri, object))
+
+    def _as_rdf_element(
+        self, element: Union[ElementName, Element], parent_slot: SlotDefinition
+    ) -> Optional[Union[URIRef, Literal]]:
+        if parent_slot.range in self.metamodel.schema.types:
+            return Literal(element)
+        elif parent_slot.range in self.metamodel.schema.enums:
+            return Literal(element)
+        elif parent_slot.range in self.metamodel.schema.classes:
+            if parent_slot.inlined:
+                element_name = element.name
+            else:
+                element_name = element
+            if element_name in self.metamodel.schema.classes:
+                return self._class_uri(element_name)
+            elif element_name in self.metamodel.schema.types:
+                return self._type_uri(element_name)
+            elif element_name in self.metamodel.schema.enums:
+                return self._enum_uri(element_name)
+        else:
+            logging.warning(f"Unknown range {defining_slot.range}")
+            return None
 
     def _range_is_datatype(self, slot: SlotDefinition) -> bool:
         if self.type_objects:
             return False
         else:
             return slot.range in self.schema.types
 
@@ -567,15 +613,15 @@
 
     def _add_metamodel_class(self, cname: str) -> None:
         metac = self.metamodel.schema.classes[cname]
         metac_uri = self.metamodel.namespaces[METAMODEL_NAMESPACE_NAME][
             camelcase(metac.name)
         ]
         self.graph.add((metac_uri, RDF.type, OWL.Class))
-        self._add_element_properties(metac_uri, metac)
+        # self._add_element_properties(metac_uri, metac)
 
     def slot_owl_type(self, slot: SlotDefinition) -> URIRef:
         if self.type_objects:
             return OWL.ObjectProperty
         elif slot.range in self.schema.classes:
             return OWL.ObjectProperty
         elif slot.range in self.schema.enums:
```

### Comparing `linkml-1.5.4/linkml/generators/prefixmapgen.py` & `linkml-1.5.5/linkml/generators/prefixmapgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/projectgen.py` & `linkml-1.5.5/linkml/generators/projectgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/protogen.py` & `linkml-1.5.5/linkml/generators/protogen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/pydanticgen.py` & `linkml-1.5.5/linkml/generators/pydanticgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/pythongen.py` & `linkml-1.5.5/linkml/generators/pythongen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/rdfgen.py` & `linkml-1.5.5/linkml/generators/rdfgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/shaclgen.py` & `linkml-1.5.5/linkml/generators/shaclgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/shexgen.py` & `linkml-1.5.5/linkml/generators/shexgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/sparqlgen.py` & `linkml-1.5.5/linkml/generators/sparqlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py` & `linkml-1.5.5/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py` & `linkml-1.5.5/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/sqlalchemygen.py` & `linkml-1.5.5/linkml/generators/sqlalchemygen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/sqlddlgen.py` & `linkml-1.5.5/linkml/generators/sqlddlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/sqltablegen.py` & `linkml-1.5.5/linkml/generators/sqltablegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/sssomgen.py` & `linkml-1.5.5/linkml/generators/sssomgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/string_template.md` & `linkml-1.5.5/linkml/generators/string_template.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/summarygen.py` & `linkml-1.5.5/linkml/generators/summarygen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/terminusdbgen.py` & `linkml-1.5.5/linkml/generators/terminusdbgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/typescriptgen.py` & `linkml-1.5.5/linkml/generators/typescriptgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/yamlgen.py` & `linkml-1.5.5/linkml/generators/yamlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/generators/yumlgen.py` & `linkml-1.5.5/linkml/generators/yumlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/linter/cli.py` & `linkml-1.5.5/linkml/linter/cli.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/linter/config/datamodel/config.py` & `linkml-1.5.5/linkml/linter/config/datamodel/config.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/linter/config/datamodel/config.yaml` & `linkml-1.5.5/linkml/linter/config/datamodel/config.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/linter/config/default.yaml` & `linkml-1.5.5/linkml/linter/config/default.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/linter/formatters/formatter.py` & `linkml-1.5.5/linkml/linter/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/linter/formatters/json_formatter.py` & `linkml-1.5.5/linkml/linter/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/linter/formatters/markdown_formatter.py` & `linkml-1.5.5/linkml/linter/formatters/markdown_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/linter/formatters/terminal_formatter.py` & `linkml-1.5.5/linkml/linter/formatters/terminal_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/linter/formatters/tsv_formatter.py` & `linkml-1.5.5/linkml/linter/formatters/tsv_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/linter/linter.py` & `linkml-1.5.5/linkml/linter/linter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/linter/rules.py` & `linkml-1.5.5/linkml/linter/rules.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/reporting/model.py` & `linkml-1.5.5/linkml/reporting/model.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/transformers/relmodel_transformer.py` & `linkml-1.5.5/linkml/transformers/relmodel_transformer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/transformers/schema_renamer.py` & `linkml-1.5.5/linkml/transformers/schema_renamer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/utils/converter.py` & `linkml-1.5.5/linkml/utils/converter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/utils/datautils.py` & `linkml-1.5.5/linkml/utils/datautils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/utils/execute_tutorial.py` & `linkml-1.5.5/linkml/utils/execute_tutorial.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/utils/generator.py` & `linkml-1.5.5/linkml/utils/generator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/utils/ifabsent_functions.py` & `linkml-1.5.5/linkml/utils/ifabsent_functions.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/utils/mergeutils.py` & `linkml-1.5.5/linkml/utils/mergeutils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/utils/rawloader.py` & `linkml-1.5.5/linkml/utils/rawloader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/utils/schema_builder.py` & `linkml-1.5.5/linkml/utils/schema_builder.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/utils/schema_fixer.py` & `linkml-1.5.5/linkml/utils/schema_fixer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/utils/schemaloader.py` & `linkml-1.5.5/linkml/utils/schemaloader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/utils/schemasynopsis.py` & `linkml-1.5.5/linkml/utils/schemasynopsis.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/utils/sqlutils.py` & `linkml-1.5.5/linkml/utils/sqlutils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/utils/typereferences.py` & `linkml-1.5.5/linkml/utils/typereferences.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/utils/validation.py` & `linkml-1.5.5/linkml/utils/validation.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/validators/jsonschemavalidator.py` & `linkml-1.5.5/linkml/validators/jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/validators/sparqlvalidator.py` & `linkml-1.5.5/linkml/validators/sparqlvalidator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/workspaces/datamodel/workspaces.py` & `linkml-1.5.5/linkml/workspaces/datamodel/workspaces.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/workspaces/datamodel/workspaces.yaml` & `linkml-1.5.5/linkml/workspaces/datamodel/workspaces.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/linkml/workspaces/example_runner.py` & `linkml-1.5.5/linkml/workspaces/example_runner.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.4/pyproject.toml` & `linkml-1.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkml"
-version = "1.5.4"
+version = "1.5.5"
 description = "Linked Open Data Modeling Language"
 authors = [
     "Chris Mungall <cjmungall@lbl.gov>",
     "Harold Solbrig <solbrig@jhu.edu>",
     "Sujay Patil <spatil@lbl.gov>",
     "Harshad Hegde <hhegde@lbl.gov>",
     "Sierra Moxon <smoxon@lbl.gov>",
@@ -102,45 +102,45 @@
 graphviz = ">=0.10.1"
 hbreader = "*"
 isodate = ">=0.6.0"
 jinja2 = ">= 3.1.0"
 jsonasobj2 = "==1.*,>=1.0.0,>=1.0.3"
 jsonschema = {extras = ["format"], version = ">=4.0.0"}
 linkml-dataops = "*"
-linkml-runtime = ">=1.5.0"
-myst-parser = "*"
+linkml-runtime = ">=1.5.3"
 openpyxl = "*"
 parse = "*"
 prefixcommons = ">=0.1.7"
-prefixmaps = "^0.1.3"
+prefixmaps = ">=0.1.3"
 pydantic = "*"
 pyjsg = ">=0.11.6"
 pyshex = ">=0.7.20"
 pyshexc = ">=0.8.3"
 python-dateutil = "*"
 pyyaml = "*"
 rdflib = ">=6.0.0"
 requests = ">=2.22"
-sphinx = "*"
-sphinx-click = "*"
-sphinx-rtd-theme = "*"
 sqlalchemy = ">=1.4.31"
 watchdog = ">=0.9.0"
-tox = "^3.25.1"
-furo = {version = "^2023.03.27", extras = ["docs"]}
-sphinxcontrib-mermaid = {version = "^0.7.1", extras = ["docs"]}
 typing-extensions = {version = "^4.5.0", python = "3.7"}
 
 [tool.poetry.dev-dependencies]
 chardet = "*"
 ipykernel = "*"
 ipython-genutils = "*"
 nbconvert = "*"
 nbformat = "*"
 coverage = "^6.4.1"
+tox = "^3.25.1"
+furo = {version = "^2023.03.27", extras = ["docs"]}
+sphinxcontrib-mermaid = {version = "^0.7.1", extras = ["docs"]}
+sphinx = "*"
+sphinx-click = "*"
+sphinx-rtd-theme = "*"
+myst-parser = "*"
 
 [tool.poetry.extras]
 docs = ["Sphinx", "sphinxcontrib-mermaid", "furo"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `linkml-1.5.4/setup.py` & `linkml-1.5.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,39 +27,32 @@
  'graphviz>=0.10.1',
  'hbreader',
  'isodate>=0.6.0',
  'jinja2>=3.1.0',
  'jsonasobj2>=1.0.3,<2.0.0',
  'jsonschema[format]>=4.0.0',
  'linkml-dataops',
- 'linkml-runtime>=1.5.0',
- 'myst-parser',
+ 'linkml-runtime>=1.5.3',
  'openpyxl',
  'parse',
  'prefixcommons>=0.1.7',
- 'prefixmaps>=0.1.3,<0.2.0',
+ 'prefixmaps>=0.1.3',
  'pydantic',
  'pyjsg>=0.11.6',
  'pyshex>=0.7.20',
  'pyshexc>=0.8.3',
  'python-dateutil',
  'pyyaml',
  'rdflib>=6.0.0',
  'requests>=2.22',
- 'sphinx-click',
- 'sphinx-rtd-theme',
  'sqlalchemy>=1.4.31',
- 'tox>=3.25.1,<4.0.0',
  'watchdog>=0.9.0']
 
 extras_require = \
-{':extra == "docs"': ['sphinx',
-                      'furo[docs]>=2023.03.27,<2024.0.0',
-                      'sphinxcontrib-mermaid[docs]>=0.7.1,<0.8.0'],
- ':python_version == "3.7"': ['typing-extensions>=4.5.0,<5.0.0']}
+{':python_version == "3.7"': ['typing-extensions>=4.5.0,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['gen-csv = linkml.generators.csvgen:cli',
                      'gen-doc = linkml.generators.docgen:cli',
                      'gen-erdiagram = linkml.generators.erdiagramgen:cli',
                      'gen-excel = linkml.generators.excelgen:cli',
                      'gen-golang = linkml.generators.golanggen:cli',
@@ -108,15 +101,15 @@
                      'linkml-sqldb = linkml.utils.sqlutils:main',
                      'linkml-validate = '
                      'linkml.validators.jsonschemavalidator:cli',
                      'run-tutorial = linkml.utils.execute_tutorial:cli']}
 
 setup_kwargs = {
     'name': 'linkml',
-    'version': '1.5.4',
+    'version': '1.5.5',
     'description': 'Linked Open Data Modeling Language',
     'long_description': '[![Pyversions](https://img.shields.io/pypi/pyversions/linkml.svg)](https://pypi.python.org/pypi/linkml)\n![](https://github.com/linkml/linkml/workflows/Build/badge.svg)\n[![PyPi](https://img.shields.io/pypi/v/linkml.svg)](https://pypi.python.org/pypi/linkml)\n[![badge](https://img.shields.io/badge/launch-binder-579ACA.svg)](https://mybinder.org/v2/gh/linkml/linkml/main?filepath=notebooks)\n[![DOI](https://zenodo.org/badge/13996/linkml/linkml.svg)](https://zenodo.org/badge/latestdoi/13996/linkml/linkml)\n[![PyPIDownloadsTotal](https://pepy.tech/badge/linkml)](https://pepy.tech/project/linkml)\n[![PyPIDownloadsMonth](https://img.shields.io/pypi/dm/linkml?logo=PyPI&color=blue)](https://pypi.org/project/linkml)\n[![codecov](https://codecov.io/gh/linkml/linkml/branch/main/graph/badge.svg?token=WNQNG986UN)](https://codecov.io/gh/linkml/linkml)\n\n\n# LinkML - Linked Data Modeling Language\n\nLinkML is a linked data modeling language following object-oriented and ontological principles. LinkML models are typically authored in YAML, and can be converted to other schema representation formats such as JSON or RDF.\n\nThis repo holds the tools for generating and working with LinkML. For the LinkML schema (metamodel), please see https://github.com/linkml/linkml-model\n\nThe complete documentation for LinkML can be found here:\n\n - [linkml.io/linkml](https://linkml.io/linkml)\n',
     'author': 'Chris Mungall',
     'author_email': 'cjmungall@lbl.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://linkml.io/linkml/',
```

### Comparing `linkml-1.5.4/PKG-INFO` & `linkml-1.5.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml
-Version: 1.5.4
+Version: 1.5.5
 Summary: Linked Open Data Modeling Language
 Home-page: https://linkml.io/linkml/
 Keywords: schema,linked data,data modeling,rdf,owl,biolink
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.7.6,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,42 +22,35 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Requires-Dist: antlr4-python3-runtime (>=4.9.0,<4.10)
 Requires-Dist: click (>=7.0)
-Requires-Dist: furo[docs] (>=2023.03.27,<2024.0.0) ; extra == "docs"
 Requires-Dist: graphviz (>=0.10.1)
 Requires-Dist: hbreader
 Requires-Dist: isodate (>=0.6.0)
 Requires-Dist: jinja2 (>=3.1.0)
 Requires-Dist: jsonasobj2 (>=1.0.3,<2.0.0)
 Requires-Dist: jsonschema[format] (>=4.0.0)
 Requires-Dist: linkml-dataops
-Requires-Dist: linkml-runtime (>=1.5.0)
-Requires-Dist: myst-parser
+Requires-Dist: linkml-runtime (>=1.5.3)
 Requires-Dist: openpyxl
 Requires-Dist: parse
 Requires-Dist: prefixcommons (>=0.1.7)
-Requires-Dist: prefixmaps (>=0.1.3,<0.2.0)
+Requires-Dist: prefixmaps (>=0.1.3)
 Requires-Dist: pydantic
 Requires-Dist: pyjsg (>=0.11.6)
 Requires-Dist: pyshex (>=0.7.20)
 Requires-Dist: pyshexc (>=0.8.3)
 Requires-Dist: python-dateutil
 Requires-Dist: pyyaml
 Requires-Dist: rdflib (>=6.0.0)
 Requires-Dist: requests (>=2.22)
-Requires-Dist: sphinx ; extra == "docs"
-Requires-Dist: sphinx-click
-Requires-Dist: sphinx-rtd-theme
-Requires-Dist: sphinxcontrib-mermaid[docs] (>=0.7.1,<0.8.0) ; extra == "docs"
 Requires-Dist: sqlalchemy (>=1.4.31)
-Requires-Dist: tox (>=3.25.1,<4.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version == "3.7"
 Requires-Dist: watchdog (>=0.9.0)
 Project-URL: Documentation, https://linkml.io/linkml/
 Project-URL: Repository, https://github.com/linkml/linkml
 Description-Content-Type: text/markdown
 
 [![Pyversions](https://img.shields.io/pypi/pyversions/linkml.svg)](https://pypi.python.org/pypi/linkml)
```

