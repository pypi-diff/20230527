# Comparing `tmp/cwltest-2.3.20230108193615.tar.gz` & `tmp/cwltest-2.3.20230527113600.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwltest-2.3.20230108193615.tar", last modified: Sun Jan  8 19:48:13 2023, max compression
+gzip compressed data, was "cwltest-2.3.20230527113600.tar", last modified: Sat May 27 11:44:35 2023, max compression
```

## Comparing `cwltest-2.3.20230108193615.tar` & `cwltest-2.3.20230527113600.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:48:13.104600 cwltest-2.3.20230108193615/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)    11357 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/LICENSE
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      274 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/MANIFEST.in
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     6513 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/Makefile
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     4100 2023-01-08 19:48:13.104600 cwltest-2.3.20230108193615/PKG-INFO
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     3044 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/README.rst
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:48:13.084600 cwltest-2.3.20230108193615/cwltest/
--rwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      334 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/cwltest/__init__.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       82 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/cwltest/__main__.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     3654 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/cwltest/argparser.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     5425 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/cwltest/compare.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      585 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/cwltest/cwltest-schema.yml
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      738 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/cwltest/hooks.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     7459 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/cwltest/main.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)    12772 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/cwltest/plugin.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/cwltest/py.typed
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)    15390 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/cwltest/utils.py
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:48:13.088600 cwltest-2.3.20230108193615/cwltest.egg-info/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     4100 2023-01-08 19:48:13.000000 cwltest-2.3.20230108193615/cwltest.egg-info/PKG-INFO
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     3484 2023-01-08 19:48:13.000000 cwltest-2.3.20230108193615/cwltest.egg-info/SOURCES.txt
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        1 2023-01-08 19:48:13.000000 cwltest-2.3.20230108193615/cwltest.egg-info/dependency_links.txt
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       95 2023-01-08 19:48:13.000000 cwltest-2.3.20230108193615/cwltest.egg-info/entry_points.txt
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      117 2023-01-08 19:48:13.000000 cwltest-2.3.20230108193615/cwltest.egg-info/requires.txt
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        8 2023-01-08 19:48:13.000000 cwltest-2.3.20230108193615/cwltest.egg-info/top_level.txt
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        1 2023-01-08 19:45:08.000000 cwltest-2.3.20230108193615/cwltest.egg-info/zip-safe
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1181 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/gittaggers.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       65 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-requirements.txt
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:48:13.088600 cwltest-2.3.20230108193615/mypy-stubs/
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:48:13.088600 cwltest-2.3.20230108193615/mypy-stubs/cachecontrol/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      219 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/cachecontrol/__init__.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      226 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/cachecontrol/cache.pyi
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:48:13.088600 cwltest-2.3.20230108193615/mypy-stubs/cachecontrol/caches/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      273 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/cachecontrol/caches/__init__.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      873 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/cachecontrol/caches/file_cache.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      169 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/cachecontrol/compat.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      470 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/cachecontrol/controller.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      532 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/cachecontrol/wrapper.pyi
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:48:13.088600 cwltest-2.3.20230108193615/mypy-stubs/defusedxml/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      180 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/defusedxml/ElementTree.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/defusedxml/__init__.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     2521 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/junit_xml.pyi
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:48:13.092600 cwltest-2.3.20230108193615/mypy-stubs/rdflib/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1292 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/__init__.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      674 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/collection.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      231 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/compare.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     8351 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/graph.pyi
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:48:13.096600 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     2010 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_CSVW.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      493 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_DC.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1034 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_DCAT.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     2361 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1109 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_DOAP.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1847 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_FOAF.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     4691 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_ODRL2.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1259 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_ORG.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     2260 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_OWL.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      441 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_PROF.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     4520 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_PROV.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1105 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_QB.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      620 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_RDF.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      519 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_RDFS.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)    41401 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_SDO.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     4965 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_SH.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      943 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_SKOS.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1075 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_SOSA.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      680 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_SSN.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     2462 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_TIME.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      927 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_VOID.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1742 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_XSD.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     2282 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/__init__.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      131 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/parser.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      724 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/paths.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      288 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/plugin.pyi
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:48:13.096600 cwltest-2.3.20230108193615/mypy-stubs/rdflib/plugins/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      118 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/plugins/__init__.pyi
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:48:13.096600 cwltest-2.3.20230108193615/mypy-stubs/rdflib/plugins/parsers/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      126 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       34 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1352 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/query.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1398 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/resource.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1337 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/rdflib/term.pyi
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:48:13.096600 cwltest-2.3.20230108193615/mypy-stubs/ruamel/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/mypy-stubs/ruamel/__init__.pyi
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      103 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/requirements.txt
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      371 2023-01-08 19:48:13.104600 cwltest-2.3.20230108193615/setup.cfg
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     2459 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/setup.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       63 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/test-requirements.txt
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:48:13.100600 cwltest-2.3.20230108193615/tests/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       25 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/__init__.py
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:48:13.104600 cwltest-2.3.20230108193615/tests/test-data/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      462 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/conformance_test_v1.0.cwltest.yml
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      440 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/conformance_test_v1.2.cwltest.yaml
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        2 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/cores.txt
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1077 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/cwltool-conftest.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      424 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/exclude-tags.yml
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       99 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/integer-id.yml
--rwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      999 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/mock_cwl_runner.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      266 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/multi-lined-doc.yml
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      292 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/optional-error.yml
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      266 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/optional-unsupported.yml
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      537 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/required-unsupported.yml
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/return-0.cwl
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/return-1.cwl
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/return-unsupported.cwl
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      138 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/short-names.yml
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      113 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/string-id.yml
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       90 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/timeout.cwl
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      240 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/timeout.yml
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:48:13.104600 cwltest-2.3.20230108193615/tests/test-data/v1.0/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      178 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/v1.0/args.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       81 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/v1.0/cat-job.json
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      104 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/v1.0/cat-n-job.json
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/v1.0/cat1-job.json
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1048 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/v1.0/cat1-testcli.cwl
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/v1.0/cat2-job.json
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        3 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/v1.0/empty.json
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       12 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/v1.0/hello.txt
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      207 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test-data/with-and-without-short-names.yml
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      372 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test_argparse.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     3188 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test_categories.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)    13244 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test_compare.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      883 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test_exclude_tags.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      387 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test_integer_id.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      721 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test_multi_lined_doc.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     4511 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test_plugin.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      817 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test_prepare.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1669 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test_short_names.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      316 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test_string_id.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1516 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/test_timeout.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1147 2023-01-08 19:45:04.000000 cwltest-2.3.20230108193615/tests/util.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 11:44:35.968758 cwltest-2.3.20230527113600/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11357 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      274 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     6513 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/Makefile
+-rw-r--r--   0 michael   (1000) michael   (1000)     4100 2023-05-27 11:44:35.968758 cwltest-2.3.20230527113600/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     3044 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 11:44:35.956758 cwltest-2.3.20230527113600/cwltest/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      334 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/cwltest/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       82 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/cwltest/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3654 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/cwltest/argparser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8789 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/cwltest/compare.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      585 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/cwltest/cwltest-schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      738 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/cwltest/hooks.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7451 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/cwltest/main.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    12772 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/cwltest/plugin.py
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/cwltest/py.typed
+-rw-r--r--   0 michael   (1000) michael   (1000)    15390 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/cwltest/utils.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 11:44:35.956758 cwltest-2.3.20230527113600/cwltest.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     4100 2023-05-27 11:44:35.000000 cwltest-2.3.20230527113600/cwltest.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     3484 2023-05-27 11:44:35.000000 cwltest-2.3.20230527113600/cwltest.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-27 11:44:35.000000 cwltest-2.3.20230527113600/cwltest.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       95 2023-05-27 11:44:35.000000 cwltest-2.3.20230527113600/cwltest.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      117 2023-05-27 11:44:35.000000 cwltest-2.3.20230527113600/cwltest.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-05-27 11:44:35.000000 cwltest-2.3.20230527113600/cwltest.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-27 11:41:23.000000 cwltest-2.3.20230527113600/cwltest.egg-info/zip-safe
+-rw-r--r--   0 michael   (1000) michael   (1000)     1181 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/gittaggers.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       65 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 11:44:35.956758 cwltest-2.3.20230527113600/mypy-stubs/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 11:44:35.960758 cwltest-2.3.20230527113600/mypy-stubs/cachecontrol/
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/cachecontrol/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      226 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/cachecontrol/cache.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 11:44:35.960758 cwltest-2.3.20230527113600/mypy-stubs/cachecontrol/caches/
+-rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/cachecontrol/caches/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      873 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/cachecontrol/caches/file_cache.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/cachecontrol/compat.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      470 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/cachecontrol/controller.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      532 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/cachecontrol/wrapper.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 11:44:35.960758 cwltest-2.3.20230527113600/mypy-stubs/defusedxml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      180 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/defusedxml/ElementTree.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/defusedxml/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2521 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/junit_xml.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 11:44:35.960758 cwltest-2.3.20230527113600/mypy-stubs/rdflib/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1292 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/collection.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      231 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/compare.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     8351 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/graph.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 11:44:35.964758 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2010 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_CSVW.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_DC.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1034 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_DCAT.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2361 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1109 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_DOAP.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1847 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_FOAF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4691 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_ODRL2.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1259 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_ORG.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2260 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_OWL.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      441 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_PROF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4520 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_PROV.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1105 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_QB.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      620 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_RDF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      519 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_RDFS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)    41401 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_SDO.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4965 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_SH.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      943 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_SKOS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1075 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_SOSA.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_SSN.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2462 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_TIME.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      927 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_VOID.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_XSD.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2282 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      724 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/paths.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      288 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/plugin.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 11:44:35.964758 cwltest-2.3.20230527113600/mypy-stubs/rdflib/plugins/
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/plugins/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 11:44:35.964758 cwltest-2.3.20230527113600/mypy-stubs/rdflib/plugins/parsers/
+-rw-r--r--   0 michael   (1000) michael   (1000)      126 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)       34 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1352 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/query.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1398 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/resource.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1337 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/rdflib/term.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 11:44:35.964758 cwltest-2.3.20230527113600/mypy-stubs/ruamel/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/mypy-stubs/ruamel/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      103 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      204 2023-05-27 11:44:35.968758 cwltest-2.3.20230527113600/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     2459 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/setup.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       63 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/test-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 11:44:35.964758 cwltest-2.3.20230527113600/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)       25 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 11:44:35.968758 cwltest-2.3.20230527113600/tests/test-data/
+-rw-r--r--   0 michael   (1000) michael   (1000)      462 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/conformance_test_v1.0.cwltest.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      440 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/conformance_test_v1.2.cwltest.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)        2 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/cores.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     1077 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/cwltool-conftest.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      424 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/exclude-tags.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/integer-id.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      999 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/mock_cwl_runner.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      266 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/multi-lined-doc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      292 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/optional-error.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      266 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/optional-unsupported.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      537 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/required-unsupported.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/return-0.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/return-1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/return-unsupported.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      138 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/short-names.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      113 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/string-id.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       90 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/timeout.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      240 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/timeout.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-27 11:44:35.968758 cwltest-2.3.20230527113600/tests/test-data/v1.0/
+-rw-r--r--   0 michael   (1000) michael   (1000)      178 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/v1.0/args.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       81 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/v1.0/cat-job.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      104 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/v1.0/cat-n-job.json
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/v1.0/cat1-job.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1048 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/v1.0/cat1-testcli.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/v1.0/cat2-job.json
+-rw-r--r--   0 michael   (1000) michael   (1000)        3 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/v1.0/empty.json
+-rw-r--r--   0 michael   (1000) michael   (1000)       12 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/v1.0/hello.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      207 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test-data/with-and-without-short-names.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      372 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test_argparse.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3188 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test_categories.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    16268 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test_compare.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      883 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test_exclude_tags.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      387 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test_integer_id.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      721 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test_multi_lined_doc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4511 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test_plugin.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      817 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test_prepare.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1669 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test_short_names.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      316 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test_string_id.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1516 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/test_timeout.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1147 2023-05-27 11:41:18.000000 cwltest-2.3.20230527113600/tests/util.py
```

### Comparing `cwltest-2.3.20230108193615/LICENSE` & `cwltest-2.3.20230527113600/LICENSE`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/Makefile` & `cwltest-2.3.20230527113600/Makefile`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/PKG-INFO` & `cwltest-2.3.20230527113600/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwltest
-Version: 2.3.20230108193615
+Version: 2.3.20230527113600
 Summary: Common Workflow Language testing framework
 Home-page: https://github.com/common-workflow-language/cwltest
 Download-URL: https://github.com/common-workflow-language/cwltest
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
 Classifier: Environment :: Console
```

### Comparing `cwltest-2.3.20230108193615/README.rst` & `cwltest-2.3.20230527113600/README.rst`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/cwltest/argparser.py` & `cwltest-2.3.20230527113600/cwltest/argparser.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/cwltest/cwltest-schema.yml` & `cwltest-2.3.20230527113600/cwltest/cwltest-schema.yml`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/cwltest/hooks.py` & `cwltest-2.3.20230527113600/cwltest/hooks.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/cwltest/main.py` & `cwltest-2.3.20230527113600/cwltest/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                 logger.warning(
                     "The `id` field with integer is deprecated. Use string identifier instead."
                 )
         else:
             logger.warning("The `id` field is missing.")
 
     if args.show_tags:
-        alltags = set()  # type: Set[str]
+        alltags: Set[str] = set()
         for t in tests:
             ts = t.get("tags", [])
             alltags |= set(ts)
         for tag in alltags:
             print(tag)
         return 0
```

### Comparing `cwltest-2.3.20230108193615/cwltest/plugin.py` & `cwltest-2.3.20230527113600/cwltest/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 import json
 import os
 import time
 import traceback
 from io import StringIO
 from pathlib import Path
 from typing import (
+    TYPE_CHECKING,
     Any,
     Dict,
     Iterator,
     List,
     Optional,
     Set,
-    TYPE_CHECKING,
     Tuple,
     Union,
     cast,
 )
 
 import pytest
+from cwltest.compare import CompareFail, compare
 from typing_extensions import Protocol
 
 from cwltest import REQUIRED, UNSUPPORTED_FEATURE, logger, utils
-from cwltest.compare import CompareFail, compare
 
 if TYPE_CHECKING:
     from _pytest._code.code import ExceptionInfo, _TracebackStyle
     from _pytest.compat import LEGACY_PATH
     from _pytest.config import Config
     from _pytest.config import Config as PytestConfig
     from _pytest.config import PytestPluginManager
@@ -232,32 +232,32 @@
                 name = utils.shortname(entry["id"])
             else:
                 name = entry.get("doc", "")
             item = CWLItem.from_parent(self, name=name, spec=entry)
             if include and name not in include:
                 item.add_marker(
                     pytest.mark.skip(
-                        reason=f"Test '{name}' is not in the include list: {','.join(include)}."
+                        reason=f"Test {name!r} is not in the include list: {','.join(include)}."
                     )
                 )
             elif exclude and name in exclude:
                 item.add_marker(
-                    pytest.mark.skip(reason=f"Test '{name}' is in the exclude list.")
+                    pytest.mark.skip(reason=f"Test {name!r} is in the exclude list.")
                 )
             elif tags and not tags.intersection(entry_tags):
                 item.add_marker(
                     pytest.mark.skip(
-                        reason=f"Test '{name}' with tags {','.join(entry_tags)}"
+                        reason=f"Test {name!r} with tags {','.join(entry_tags)}"
                         f" doesn't have a tag on the allowed tag list: {','.join(tags)}."
                     )
                 )
             elif exclude_tags and exclude_tags.intersection(entry_tags):
                 item.add_marker(
                     pytest.mark.skip(
-                        reason=f"Test '{name}' has one or more tags on the exclusion "
+                        reason=f"Test {name!r} has one or more tags on the exclusion "
                         f" tag list: {','.join(exclude_tags.intersection(entry_tags))}."
                     )
                 )
             yield item
 
 
 __OPTIONS: List[Tuple[str, Dict[str, Any]]] = [
```

### Comparing `cwltest-2.3.20230108193615/cwltest/utils.py` & `cwltest-2.3.20230527113600/cwltest/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from rdflib import Graph
 from ruamel.yaml.scalarstring import ScalarString
 from schema_salad.exceptions import ValidationException
 
 from cwltest import REQUIRED, UNSUPPORTED_FEATURE, logger, templock
 
 
-class CWLTestConfig(object):
+class CWLTestConfig:
     """Store configuration values for cwltest."""
 
     def __init__(
         self,
         basedir: Optional[str] = None,
         outdir: Optional[str] = None,
         classname: Optional[str] = None,
@@ -118,15 +118,15 @@
     if isinstance(obj, ScalarString):
         return str(obj)
     for typ in int, float, bool, str:
         if isinstance(obj, typ):
             return typ(obj)
     if obj is None:
         return None
-    raise Exception(f"Unsupported type {type(obj)} of '{obj}'.")
+    raise Exception(f"Unsupported type {type(obj)} of {obj!r}.")
 
 
 def generate_badges(
     badgedir: str, ntotal: Dict[str, int], npassed: Dict[str, int]
 ) -> None:
     """Generate badges with conformance levels."""
     os.mkdir(badgedir)
@@ -169,23 +169,26 @@
     """
     schema_resource = pkg_resources.resource_stream(__name__, "cwltest-schema.yml")
     cache: Optional[Dict[str, Union[str, Graph, bool]]] = {
         "https://w3id.org/cwl/cwltest/cwltest-schema.yml": schema_resource.read().decode(
             "utf-8"
         )
     }
-    (document_loader, avsc_names, _, _,) = schema_salad.schema.load_schema(
+    (
+        document_loader,
+        avsc_names,
+        _,
+        _,
+    ) = schema_salad.schema.load_schema(
         "https://w3id.org/cwl/cwltest/cwltest-schema.yml", cache=cache
     )
 
     if not isinstance(avsc_names, schema_salad.avro.schema.Names):
         print(avsc_names)
-        raise ValidationException(
-            "Wrong instance for avsc_names: {}".format(type(avsc_names))
-        )
+        raise ValidationException(f"Wrong instance for avsc_names: {type(avsc_names)}")
 
     tests, metadata = schema_salad.schema.load_and_validate(
         document_loader, avsc_names, path, True
     )
     tests = cast(List[Dict[str, Any]], _clean_ruamel(tests))
 
     return tests, metadata
```

### Comparing `cwltest-2.3.20230108193615/cwltest.egg-info/PKG-INFO` & `cwltest-2.3.20230527113600/cwltest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwltest
-Version: 2.3.20230108193615
+Version: 2.3.20230527113600
 Summary: Common Workflow Language testing framework
 Home-page: https://github.com/common-workflow-language/cwltest
 Download-URL: https://github.com/common-workflow-language/cwltest
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
 Classifier: Environment :: Console
```

### Comparing `cwltest-2.3.20230108193615/cwltest.egg-info/SOURCES.txt` & `cwltest-2.3.20230527113600/cwltest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/gittaggers.py` & `cwltest-2.3.20230527113600/gittaggers.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/cachecontrol/caches/file_cache.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/cachecontrol/caches/file_cache.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/cachecontrol/wrapper.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/cachecontrol/wrapper.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/junit_xml.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/junit_xml.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/__init__.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/collection.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/collection.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/graph.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/graph.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_CSVW.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_CSVW.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_DCAT.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_DCAT.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_DCTERMS.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_DCTERMS.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_DOAP.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_DOAP.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_FOAF.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_FOAF.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_ODRL2.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_ODRL2.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_ORG.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_ORG.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_OWL.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_OWL.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_PROV.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_PROV.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_QB.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_QB.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_RDF.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_RDF.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_RDFS.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_RDFS.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_SDO.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_SDO.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_SH.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_SH.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_SKOS.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_SKOS.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_SOSA.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_SOSA.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_SSN.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_SSN.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_TIME.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_TIME.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_VOID.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_VOID.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/_XSD.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/_XSD.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/namespace/__init__.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/namespace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/paths.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/paths.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/query.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/query.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/resource.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/resource.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/mypy-stubs/rdflib/term.pyi` & `cwltest-2.3.20230527113600/mypy-stubs/rdflib/term.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/setup.py` & `cwltest-2.3.20230527113600/setup.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/tests/test-data/cwltool-conftest.py` & `cwltest-2.3.20230527113600/tests/test-data/cwltool-conftest.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/tests/test-data/mock_cwl_runner.py` & `cwltest-2.3.20230527113600/tests/test-data/mock_cwl_runner.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/tests/test-data/required-unsupported.yml` & `cwltest-2.3.20230527113600/tests/test-data/required-unsupported.yml`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/tests/test-data/v1.0/cat1-testcli.cwl` & `cwltest-2.3.20230527113600/tests/test-data/v1.0/cat1-testcli.cwl`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/tests/test_categories.py` & `cwltest-2.3.20230527113600/tests/test_categories.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/tests/test_compare.py` & `cwltest-2.3.20230527113600/tests/test_compare.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import os
+from pathlib import Path
 from typing import Any, Dict
 
 import pytest
-from cwltest.compare import CompareFail, compare
+from cwltest.compare import CompareFail, _compare_directory, _compare_file, compare
 
 from .util import get_data
 
 
 def test_compare_any_success() -> None:
     expected = "Any"
     actual: Dict[str, Any] = {}
@@ -33,26 +35,141 @@
 
 def test_compare_contents_success() -> None:
     expected = {
         "location": "cores.txt",
         "size": 2,
         "class": "File",
         "contents": "2\n",
+        "checksum": "sha1$7448d8798a4380162d4b56f9b452e2f6f9e24e7a",
     }
     actual = {
         "basename": "cores.txt",
         "checksum": "sha1$7448d8798a4380162d4b56f9b452e2f6f9e24e7a",
         "class": "File",
         "location": "file:///var/folders/8x/2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/cores.txt",
         "path": get_data("tests/test-data/cores.txt"),
         "size": 2,
     }
     compare(expected, actual)
 
 
+def test_compare_contents_not_exist() -> None:
+    expected = {
+        "location": "cores.txt",
+        "class": "File",
+    }
+    actual = {
+        "basename": "cores.txt",
+        "class": "File",
+        "location": "file:///var/folders/8x/2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/cores.txt",
+        "path": "/none/exist/path/to/cores.txt",
+        "size": 2,
+    }
+    with pytest.raises(CompareFail):
+        _compare_file(expected, actual, False)
+
+
+def test_compare_file_different_size(tmp_path: Path) -> None:
+    expected = {
+        "location": "cores.txt",
+        "size": 2,
+        "class": "File",
+    }
+
+    path = tmp_path / "cores.txt"
+    with open(path, "w") as f:
+        f.write("hello")
+
+    actual = {
+        "basename": "cores.txt",
+        "class": "File",
+        "location": str(path),
+    }
+    with pytest.raises(CompareFail):
+        _compare_file(expected, actual, False)
+
+
+def test_compare_file_different_checksum(tmp_path: Path) -> None:
+    expected = {
+        "location": "cores.txt",
+        "class": "File",
+        "checksum": "sha1$7448d8798a4380162d4b56f9b452e2f6f9e24e7a",
+    }
+
+    path = tmp_path / "cores.txt"
+    with open(path, "w") as f:
+        f.write("hello")
+
+    actual = {
+        "basename": "cores.txt",
+        "class": "File",
+        "location": str(path),
+    }
+    with pytest.raises(CompareFail):
+        _compare_file(expected, actual, False)
+
+
+def test_compare_file_inconsistent_size(tmp_path: Path) -> None:
+    expected = {
+        "location": "cores.txt",
+        "class": "File",
+    }
+
+    path = tmp_path / "cores.txt"
+    with open(path, "w") as f:
+        f.write("hello")
+
+    actual = {
+        "basename": "cores.txt",
+        "class": "File",
+        "location": str(path),
+        "size": 65535,
+    }
+    with pytest.raises(CompareFail):
+        _compare_file(expected, actual, False)
+
+
+def test_compare_file_inconsistent_checksum(tmp_path: Path) -> None:
+    expected = {
+        "location": "cores.txt",
+        "class": "File",
+    }
+
+    path = tmp_path / "cores.txt"
+    with open(path, "w") as f:
+        f.write("hello")
+
+    actual = {
+        "basename": "cores.txt",
+        "checksum": "inconsistent-checksum",
+        "class": "File",
+        "location": str(path),
+    }
+    with pytest.raises(CompareFail):
+        _compare_file(expected, actual, False)
+
+
+def test_compare_directory(tmp_path: Path) -> None:
+    expected = {
+        "location": "dir",
+        "class": "Directory",
+        "listing": [],
+    }
+
+    path = tmp_path / "dir"
+    os.makedirs(path)
+
+    actual = {
+        "class": "Directory",
+        "location": str(path),
+        "listing": [],
+    }
+    _compare_directory(expected, actual, False)
+
+
 def test_compare_directory_success() -> None:
     expected = {
         "stuff": {
             "class": "Directory",
             "listing": [
                 {
                     "basename": "baz.txt",
@@ -96,15 +213,15 @@
                             "size": 0,
                         }
                     ],
                 },
             ],
         }
     }
-    compare(expected, actual)
+    compare(expected, actual, skip_details=True)
 
 
 def test_compare_directory_failure_different_listing() -> None:
     expected = {
         "stuff": {
             "class": "Directory",
             "listing": [
@@ -135,30 +252,34 @@
             "location": "file:///var/folders/8x/2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff",
             "path": "/var/folders/8x/2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff",
             "listing": [
                 {
                     "basename": "baz.txt",
                     "checksum": "sha1$da39a3ee5e6b4b0d3255bfef95601890afd80709",
                     "class": "File",
-                    "location": "file:///var/folders/8x/2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff/baz.txt",
+                    "location": "file:///var/folders/8x/"
+                    "2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff/baz.txt",
                     "path": "/var/folders/8x/2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff/baz.txt",
                     "size": 0,
                 },
                 {
                     "basename": "foo",
                     "class": "Directory",
-                    "location": "file:///var/folders/8x/2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff/foo",
+                    "location": "file:///var/folders/8x/"
+                    "2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff/foo",
                     "path": "/var/folders/8x/2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff/foo",
                     "listing": [
                         {
                             "basename": "bar.txt",
                             "checksum": "sha1$da39a3ee5e6b4b0d3255bfef95601890afd80775",
                             "class": "File",
-                            "location": "file:///var/folders/8x/2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff/foo/bar.txt",
-                            "path": "/var/folders/8x/2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff/foo/bar.txt",
+                            "location": "file:///var/folders/8x/"
+                            "2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff/foo/bar.txt",
+                            "path": "/var/folders/8x/"
+                            "2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff/foo/bar.txt",
                             "size": 0,
                         }
                     ],
                 },
             ],
         }
     }
@@ -198,15 +319,16 @@
             "location": "file:///var/folders/8x/2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff",
             "path": "/var/folders/8x/2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff",
             "listing": [
                 {
                     "basename": "baz.txt",
                     "checksum": "sha1$da39a3ee5e6b4b0d3255bfef95601890afd80709",
                     "class": "File",
-                    "location": "file:///var/folders/8x/2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff/baz.txt",
+                    "location": "file:///var/folders/8x/"
+                    "2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff/baz.txt",
                     "path": "/var/folders/8x/2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff/baz.txt",
                     "size": 0,
                 },
                 {
                     "basename": "foo",
                     "class": "Directory",
                     "location": "file:///var/folders/8x/2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/stuff/foo",
@@ -261,15 +383,15 @@
         "basename": "cores.txt",
         "checksum": "sha1$7448d8798a4380162d4b56f9b452e2f6f9e24e7a",
         "class": "File",
         "location": "file:///var/folders/8x/2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/cores.txt",
         "path": "/var/folders/8x/2df05_7j20j6r8y81w4qf43r0000gn/T/tmpG0EkrS/cores.txt",
         "size": 2,
     }
-    compare(expected, actual)
+    compare(expected, actual, skip_details=True)
 
 
 def test_compare_list_failure_missing() -> None:
     expected = {
         "args": [
             "tmap",
             "mapall",
```

### Comparing `cwltest-2.3.20230108193615/tests/test_exclude_tags.py` & `cwltest-2.3.20230527113600/tests/test_exclude_tags.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/tests/test_multi_lined_doc.py` & `cwltest-2.3.20230527113600/tests/test_multi_lined_doc.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/tests/test_plugin.py` & `cwltest-2.3.20230527113600/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/tests/test_prepare.py` & `cwltest-2.3.20230527113600/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/tests/test_short_names.py` & `cwltest-2.3.20230527113600/tests/test_short_names.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/tests/test_timeout.py` & `cwltest-2.3.20230527113600/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.3.20230108193615/tests/util.py` & `cwltest-2.3.20230527113600/tests/util.py`

 * *Files identical despite different names*

