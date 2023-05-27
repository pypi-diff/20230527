# Comparing `tmp/GBT_parser-1.0.24.tar.gz` & `tmp/GBT_parser-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GBT_parser-1.0.24.tar", last modified: Sat May 27 13:01:23 2023, max compression
+gzip compressed data, was "GBT_parser-1.0.4.tar", last modified: Fri May 26 10:54:59 2023, max compression
```

## Comparing `GBT_parser-1.0.24.tar` & `GBT_parser-1.0.4.tar`

### file list

```diff
@@ -1,285 +1,285 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.741617 GBT_parser-1.0.24/
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.402755 GBT_parser-1.0.24/GBT_parser.egg-info/
--rw-rw-rw-   0        0        0      453 2023-05-27 13:01:23.000000 GBT_parser-1.0.24/GBT_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9817 2023-05-27 13:01:23.000000 GBT_parser-1.0.24/GBT_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 13:01:23.000000 GBT_parser-1.0.24/GBT_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-27 13:01:23.000000 GBT_parser-1.0.24/GBT_parser.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      226 2023-05-27 13:01:23.000000 GBT_parser-1.0.24/GBT_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-27 13:01:23.000000 GBT_parser-1.0.24/GBT_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1107 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/LICENSE
--rw-rw-rw-   0        0        0      116 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/MANIFEST.in
--rw-rw-rw-   0        0        0     5142 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/Makefile
--rw-rw-rw-   0        0        0      453 2023-05-27 13:01:23.740615 GBT_parser-1.0.24/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-27 08:27:25.000000 GBT_parser-1.0.24/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.416818 GBT_parser-1.0.24/cantools/
--rw-rw-rw-   0        0        0     3122 2023-04-27 08:41:02.000000 GBT_parser-1.0.24/cantools/__init__.py
--rw-rw-rw-   0        0        0       76 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/cantools/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.423748 GBT_parser-1.0.24/cantools/autosar/
--rw-rw-rw-   0        0        0      129 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/autosar/__init__.py
--rw-rw-rw-   0        0        0     5976 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/autosar/end_to_end.py
--rw-rw-rw-   0        0        0     3885 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/autosar/secoc.py
--rw-rw-rw-   0        0        0     1247 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/autosar/snakeauth.py
--rw-rw-rw-   0        0        0      595 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/compat.py
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.427750 GBT_parser-1.0.24/cantools/database/
--rw-rw-rw-   0        0        0    14667 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.447758 GBT_parser-1.0.24/cantools/database/can/
--rw-rw-rw-   0        0        0      162 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/__init__.py
--rw-rw-rw-   0        0        0      853 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/attribute.py
--rw-rw-rw-   0        0        0     2326 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/attribute_definition.py
--rw-rw-rw-   0        0        0     2594 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/bus.py
--rw-rw-rw-   0        0        0    55788 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/c_source.py
--rw-rw-rw-   0        0        0    18598 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/database.py
--rw-rw-rw-   0        0        0     3497 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/environment_variable.py
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.456753 GBT_parser-1.0.24/cantools/database/can/formats/
--rw-rw-rw-   0        0        0        0 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/cantools/database/can/formats/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.469752 GBT_parser-1.0.24/cantools/database/can/formats/arxml/
--rw-rw-rw-   0        0        0     2731 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/formats/arxml/__init__.py
--rw-rw-rw-   0        0        0      152 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/formats/arxml/bus_specifics.py
--rw-rw-rw-   0        0        0      471 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/formats/arxml/database_specifics.py
--rw-rw-rw-   0        0        0    13303 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/formats/arxml/ecu_extract_loader.py
--rw-rw-rw-   0        0        0     1483 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/formats/arxml/end_to_end_properties.py
--rw-rw-rw-   0        0        0     2119 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/formats/arxml/message_specifics.py
--rw-rw-rw-   0        0        0      232 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/formats/arxml/node_specifics.py
--rw-rw-rw-   0        0        0     3377 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/formats/arxml/secoc_properties.py
--rw-rw-rw-   0        0        0   100529 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/formats/arxml/system_loader.py
--rw-rw-rw-   0        0        0     1770 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/formats/arxml/utils.py
--rw-rw-rw-   0        0        0    66250 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/formats/dbc.py
--rw-rw-rw-   0        0        0     2546 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/formats/dbc_specifics.py
--rw-rw-rw-   0        0        0    15993 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/formats/kcd.py
--rw-rw-rw-   0        0        0    36438 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/formats/sym.py
--rw-rw-rw-   0        0        0      369 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/cantools/database/can/formats/utils.py
--rw-rw-rw-   0        0        0      861 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/internal_database.py
--rw-rw-rw-   0        0        0    49341 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/message.py
--rw-rw-rw-   0        0        0     3089 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/node.py
--rw-rw-rw-   0        0        0    14595 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/signal.py
--rw-rw-rw-   0        0        0     1386 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/can/signal_group.py
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.476772 GBT_parser-1.0.24/cantools/database/diagnostics/
--rw-rw-rw-   0        0        0       78 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/diagnostics/__init__.py
--rw-rw-rw-   0        0        0     2855 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/diagnostics/data.py
--rw-rw-rw-   0        0        0     3311 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/diagnostics/database.py
--rw-rw-rw-   0        0        0     3452 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/diagnostics/did.py
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.478758 GBT_parser-1.0.24/cantools/database/diagnostics/formats/
--rw-rw-rw-   0        0        0        0 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/cantools/database/diagnostics/formats/__init__.py
--rw-rw-rw-   0        0        0     6888 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/diagnostics/formats/cdd.py
--rw-rw-rw-   0        0        0      170 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/diagnostics/internal_database.py
--rw-rw-rw-   0        0        0      196 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/cantools/database/errors.py
--rw-rw-rw-   0        0        0    15342 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/database/utils.py
--rw-rw-rw-   0        0        0      105 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/cantools/errors.py
--rw-rw-rw-   0        0        0     4748 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/j1939.py
--rw-rw-rw-   0        0        0    15265 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/logreader.py
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.488758 GBT_parser-1.0.24/cantools/subparsers/
--rw-rw-rw-   0        0        0        0 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/cantools/subparsers/__init__.py
--rw-rw-rw-   0        0        0     7778 2023-05-26 10:23:50.000000 GBT_parser-1.0.24/cantools/subparsers/__utils__.py
--rw-rw-rw-   0        0        0     1537 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/cantools/subparsers/convert.py
--rw-rw-rw-   0        0        0     2794 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/subparsers/decode.py
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.490752 GBT_parser-1.0.24/cantools/subparsers/dump/
--rw-rw-rw-   0        0        0     5995 2023-04-28 22:16:26.000000 GBT_parser-1.0.24/cantools/subparsers/dump/__init__.py
--rw-rw-rw-   0        0        0    12225 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/subparsers/dump/formatting.py
--rw-rw-rw-   0        0        0     4307 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/subparsers/generate_c_source.py
--rw-rw-rw-   0        0        0    14663 2023-04-27 09:16:27.000000 GBT_parser-1.0.24/cantools/subparsers/list.py
--rw-rw-rw-   0        0        0    24413 2023-05-27 12:55:22.000000 GBT_parser-1.0.24/cantools/subparsers/monitor.py
--rw-rw-rw-   0        0        0    35519 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/subparsers/plot.py
--rw-rw-rw-   0        0        0    16034 2023-04-27 09:03:36.000000 GBT_parser-1.0.24/cantools/tester.py
--rw-rw-rw-   0        0        0     2109 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/cantools/typechecking.py
--rw-rw-rw-   0        0        0       25 2023-05-27 13:00:56.000000 GBT_parser-1.0.24/cantools/version.py
--rw-rw-rw-   0        0        0     1007 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 13:01:23.741617 GBT_parser-1.0.24/setup.cfg
--rw-rw-rw-   0        0        0     1486 2023-05-26 11:12:07.000000 GBT_parser-1.0.24/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.514150 GBT_parser-1.0.24/tests/
--rw-rw-rw-   0        0        0        0 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/__init__.py
--rw-rw-rw-   0        0        0      295 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/dummy.c
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.368305 GBT_parser-1.0.24/tests/files/
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.538502 GBT_parser-1.0.24/tests/files/arxml/
--rw-rw-rw-   0        0        0     9947 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/arxml/compu_method_no_category.arxml
--rw-rw-rw-   0        0        0    18542 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/arxml/ecu-extract-4.2.arxml
--rw-rw-rw-   0        0        0    38300 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/arxml/system-3.2.3.arxml
--rw-rw-rw-   0        0        0    72577 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/arxml/system-4.2.arxml
--rw-rw-rw-   0        0        0      282 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/arxml/system-DAI-3.1.2.arxml
--rw-rw-rw-   0        0        0    14079 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/arxml/system-bad-root-tag-4.2.arxml
--rw-rw-rw-   0        0        0     1302 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/arxml/system-dangling-reference-4.2.arxml
--rw-rw-rw-   0        0        0    30885 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/arxml/system-float-values.arxml
--rw-rw-rw-   0        0        0      264 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/arxml/system-illegal-namespace-4.2.arxml
--rw-rw-rw-   0        0        0      265 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/arxml/system-illegal-root-4.2.arxml
--rw-rw-rw-   0        0        0      273 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/arxml/system-illegal-version-4.2.2.1.0.arxml
--rw-rw-rw-   0        0        0     4153 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/arxml/system-missing-denominator-4.2.arxml
--rw-rw-rw-   0        0        0     4162 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/arxml/system-missing-factor-4.2.arxml
--rw-rw-rw-   0        0        0     3943 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/arxml/system-missing-rational-4.2.arxml
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.622381 GBT_parser-1.0.24/tests/files/c_source/
--rw-rw-rw-   0        0        0    54386 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/abs.c
--rw-rw-rw-   0        0        0    96994 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/abs.h
--rw-rw-rw-   0        0        0     1770 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/camel_case_empty.c
--rw-rw-rw-   0        0        0     2807 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/camel_case_empty.h
--rw-rw-rw-   0        0        0     2459 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/choices.c
--rw-rw-rw-   0        0        0     3661 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/choices.h
--rw-rw-rw-   0        0        0     6880 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/floating_point.c
--rw-rw-rw-   0        0        0     6066 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/floating_point.h
--rw-rw-rw-   0        0        0     7078 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/floating_point_bit_fields.c
--rw-rw-rw-   0        0        0     6418 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/floating_point_bit_fields.h
--rw-rw-rw-   0        0        0     8474 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/floating_point_use_float.c
--rw-rw-rw-   0        0        0     8414 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/floating_point_use_float.h
--rw-rw-rw-   0        0        0     1826 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/letter_terminated_can_id_6_0.c
--rw-rw-rw-   0        0        0     2925 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/letter_terminated_can_id_6_0.h
--rw-rw-rw-   0        0        0     5494 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/min_max_only_6_0.c
--rw-rw-rw-   0        0        0     5898 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/min_max_only_6_0.h
--rw-rw-rw-   0        0        0     4632 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/motohawk.c
--rw-rw-rw-   0        0        0     5376 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/motohawk.h
--rw-rw-rw-   0        0        0     4786 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/motohawk_bit_fields.c
--rw-rw-rw-   0        0        0     5664 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/motohawk_bit_fields.h
--rw-rw-rw-   0        0        0     3963 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/motohawk_no_floating_point_numbers.c
--rw-rw-rw-   0        0        0     4114 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/motohawk_no_floating_point_numbers.h
--rw-rw-rw-   0        0        0     4112 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/motohawk_sender_node.c
--rw-rw-rw-   0        0        0     4956 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/motohawk_sender_node.h
--rw-rw-rw-   0        0        0     3655 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/motohawk_sender_node_no_floating_point_numbers.c
--rw-rw-rw-   0        0        0     4114 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/motohawk_sender_node_no_floating_point_numbers.h
--rw-rw-rw-   0        0        0     8399 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/multiplex.c
--rw-rw-rw-   0        0        0    11748 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/multiplex.h
--rw-rw-rw-   0        0        0    19855 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/multiplex_2.c
--rw-rw-rw-   0        0        0    19932 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/multiplex_2.h
--rw-rw-rw-   0        0        0     7722 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/multiplex_2_fuzzer.c
--rw-rw-rw-   0        0        0     5375 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/multiplex_2_fuzzer.h
--rw-rw-rw-   0        0        0     1790 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/multiplex_2_fuzzer.mk
--rw-rw-rw-   0        0        0     4744 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/my_database_name.c
--rw-rw-rw-   0        0        0     5576 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/my_database_name.h
--rw-rw-rw-   0        0        0     2138 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/no_signals.c
--rw-rw-rw-   0        0        0     3820 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/no_signals.h
--rw-rw-rw-   0        0        0    16637 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/open_actuator.c
--rw-rw-rw-   0        0        0    26206 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/open_actuator.h
--rw-rw-rw-   0        0        0    11894 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/open_actuator_no_floating_point_numbers.c
--rw-rw-rw-   0        0        0    17130 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/open_actuator_no_floating_point_numbers.h
--rw-rw-rw-   0        0        0     9754 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/open_actuator_sender_node.c
--rw-rw-rw-   0        0        0    17669 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/open_actuator_sender_node.h
--rw-rw-rw-   0        0        0     7625 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/open_actuator_sender_node_no_floating_point_numbers.c
--rw-rw-rw-   0        0        0    13576 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/open_actuator_sender_node_no_floating_point_numbers.h
--rw-rw-rw-   0        0        0    12653 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/padding_bit_order.c
--rw-rw-rw-   0        0        0    16664 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/padding_bit_order.h
--rw-rw-rw-   0        0        0    26296 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/signed.c
--rw-rw-rw-   0        0        0    26265 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/signed.h
--rw-rw-rw-   0        0        0    27385 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/signed_bit_fields.c
--rw-rw-rw-   0        0        0    28251 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/signed_bit_fields.h
--rw-rw-rw-   0        0        0   434422 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/c_source/vehicle.c
--rw-rw-rw-   0        0        0   672980 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/c_source/vehicle.h
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.632717 GBT_parser-1.0.24/tests/files/cdd/
--rw-rw-rw-   0        0        0   855589 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/cdd/example-diddatarefs.cdd
--rw-rw-rw-   0        0        0   389046 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/cdd/example.cdd
--rw-rw-rw-   0        0        0   389048 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/cdd/invalid-bo-example.cdd
--rw-rw-rw-   0        0        0   389046 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/cdd/le-example.cdd
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.712618 GBT_parser-1.0.24/tests/files/dbc/
--rw-rw-rw-   0        0        0      685 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/BU_BO_REL_.dbc
--rw-rw-rw-   0        0        0      736 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/BU_BO_REL_Message.dbc
--rw-rw-rw-   0        0        0       85 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/CamelCaseEmpty.dbc
--rw-rw-rw-   0        0        0    14428 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/abs.dbc
--rw-rw-rw-   0        0        0      428 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/add_two_dbc_files_1.dbc
--rw-rw-rw-   0        0        0      409 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/add_two_dbc_files_2.dbc
--rw-rw-rw-   0        0        0      650 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/attribute_Event.dbc
--rw-rw-rw-   0        0        0     3269 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/attributes.dbc
--rw-rw-rw-   0        0        0     1272 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/attributes_relation.dbc
--rw-rw-rw-   0        0        0      471 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/bad_message_length.dbc
--rw-rw-rw-   0        0        0     3303 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/big_numbers.dbc
--rw-rw-rw-   0        0        0     2728 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/bus_comment.dbc
--rw-rw-rw-   0        0        0      766 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/choices.dbc
--rw-rw-rw-   0        0        0      748 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/choices_issue_with_name.dbc
--rw-rw-rw-   0        0        0     1316 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/comments_hex_and_motorola_converted_from_sym.dbc
--rw-rw-rw-   0        0        0      694 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/cp1252.dbc
--rw-rw-rw-   0        0        0      651 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/dump_signal_choices.dbc
--rw-rw-rw-   0        0        0     2099 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/emc32.dbc
--rw-rw-rw-   0        0        0      811 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/empty_choice.dbc
--rw-rw-rw-   0        0        0       38 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/empty_ns.dbc
--rw-rw-rw-   0        0        0      891 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/floating_point.dbc
--rw-rw-rw-   0        0        0      916 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/floating_point_use_float.dbc
--rw-rw-rw-   0        0        0     2804 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/dbc/foobar.dbc
--rw-rw-rw-   0        0        0     1222 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/issue_163_newline.dbc
--rw-rw-rw-   0        0        0     2750 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/issue_168.DBC
--rw-rw-rw-   0        0        0     3984 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/issue_184_extended_mux_cascaded.dbc
--rw-rw-rw-   0        0        0     3991 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/issue_184_extended_mux_cascaded_dumped.dbc
--rw-rw-rw-   0        0        0     4021 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/issue_184_extended_mux_independent_multiplexors.dbc
--rw-rw-rw-   0        0        0     4030 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/issue_184_extended_mux_independent_multiplexors_dumped.dbc
--rw-rw-rw-   0        0        0     3771 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/issue_184_extended_mux_multiple_values.dbc
--rw-rw-rw-   0        0        0     3862 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/issue_184_extended_mux_multiple_values_dumped.dbc
--rw-rw-rw-   0        0        0     3332 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/issue_199.dbc
--rw-rw-rw-   0        0        0     3334 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/issue_199_extended.dbc
--rw-rw-rw-   0        0        0      616 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/issue_207_sig_plus.dbc
--rw-rw-rw-   0        0        0      811 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/issue_228.dbc
--rw-rw-rw-   0        0        0     1671 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/issue_62.dbc
--rw-rw-rw-   0        0        0      794 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/issue_63.dbc
--rw-rw-rw-   0        0        0     3840 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/j1939.dbc
--rw-rw-rw-   0        0        0     5044 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/long_names.dbc
--rw-rw-rw-   0        0        0     5136 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/long_names_multiple_relations.dbc
--rw-rw-rw-   0        0        0     5138 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/long_names_multiple_relations_dumped.dbc
--rw-rw-rw-   0        0        0       85 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/message-dlc-zero.dbc
--rw-rw-rw-   0        0        0      895 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/mod_name_len_dest.dbc
--rw-rw-rw-   0        0        0     1198 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/mod_name_len_src.dbc
--rw-rw-rw-   0        0        0      822 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/motohawk.dbc
--rw-rw-rw-   0        0        0      996 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/motohawk_with_comments.dbc
--rw-rw-rw-   0        0        0     4998 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/msxii_system_can.dbc
--rw-rw-rw-   0        0        0      593 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/multiple_senders.dbc
--rw-rw-rw-   0        0        0     2355 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/multiplex.dbc
--rw-rw-rw-   0        0        0     5322 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/multiplex_2.dbc
--rw-rw-rw-   0        0        0     5393 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/multiplex_2_dumped.dbc
--rw-rw-rw-   0        0        0     3905 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/multiplex_choices.dbc
--rw-rw-rw-   0        0        0     4784 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/multiplex_choices_dumped.dbc
--rw-rw-rw-   0        0        0     2705 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/multiplex_dumped.dbc
--rw-rw-rw-   0        0        0      580 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/no_sender.dbc
--rw-rw-rw-   0        0        0      180 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/no_signals.dbc
--rw-rw-rw-   0        0        0     2710 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/open_actuator.dbc
--rw-rw-rw-   0        0        0     1035 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/padding_bit_order.dbc
--rw-rw-rw-   0        0        0     1301 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/sig_groups.dbc
--rw-rw-rw-   0        0        0     1164 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/sig_groups_del.dbc
--rw-rw-rw-   0        0        0     1339 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/sig_groups_out.dbc
--rw-rw-rw-   0        0        0     1774 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/signed.dbc
--rw-rw-rw-   0        0        0     2765 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/socialledge-written-by-cantools-with-default-sort-signals.dbc
--rw-rw-rw-   0        0        0     2765 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/socialledge-written-by-cantools-with-sort-signals-by-name.dbc
--rw-rw-rw-   0        0        0     2765 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/socialledge-written-by-cantools.dbc
--rw-rw-rw-   0        0        0     2808 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/socialledge.dbc
--rw-rw-rw-   0        0        0      642 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/test_extended_id_dump.dbc
--rw-rw-rw-   0        0        0      668 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/test_multiplex_dump.dbc
--rw-rw-rw-   0        0        0      954 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/timing.dbc
--rw-rw-rw-   0        0        0      767 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/val_table.dbc
--rw-rw-rw-   0        0        0      542 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/variable_dlc.dbc
--rw-rw-rw-   0        0        0    72742 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/dbc/vehicle.dbc
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.720618 GBT_parser-1.0.24/tests/files/kcd/
--rw-rw-rw-   0        0        0      513 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/kcd/bad_message_length.kcd
--rw-rw-rw-   0        0        0     2399 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/kcd/dump.kcd
--rw-rw-rw-   0        0        0      189 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/kcd/empty.kcd
--rw-rw-rw-   0        0        0     2457 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/kcd/message_layout.kcd
--rw-rw-rw-   0        0        0     1240 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/kcd/signal_range.kcd
--rw-rw-rw-   0        0        0     1219 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/kcd/tester.kcd
--rw-rw-rw-   0        0        0    15989 2023-04-26 06:56:48.000000 GBT_parser-1.0.24/tests/files/kcd/the_homer.kcd
--rw-rw-rw-   0        0        0   107162 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/kcd/vehicle.kcd
-drwxrwxrwx   0        0        0        0 2023-05-27 13:01:23.739617 GBT_parser-1.0.24/tests/files/sym/
--rw-rw-rw-   0        0        0      188 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/bad_message_length.sym
--rw-rw-rw-   0        0        0      296 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/big-endian.sym
--rw-rw-rw-   0        0        0      839 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/comments_hex_and_motorola.sym
--rw-rw-rw-   0        0        0       65 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/empty-6.0.sym
--rw-rw-rw-   0        0        0      197 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/empty-enum-6.0.sym
--rw-rw-rw-   0        0        0      539 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/issue_138.sym
--rw-rw-rw-   0        0        0      557 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/jopp-5.0.sym
--rw-rw-rw-   0        0        0      915 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/jopp-6.0.sym
--rw-rw-rw-   0        0        0      159 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/letter-terminated-can-id-6.0.sym
--rw-rw-rw-   0        0        0      324 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/min-max-only-6.0.sym
--rw-rw-rw-   0        0        0      356 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/multiplexed_variables.sym
--rw-rw-rw-   0        0        0      113 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/receive-6.0.sym
--rw-rw-rw-   0        0        0      110 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/send-6.0.sym
--rw-rw-rw-   0        0        0      161 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/sendreceive-6.0.sym
--rw-rw-rw-   0        0        0      495 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/signal-types-6.0.sym
--rw-rw-rw-   0        0        0      516 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/special-chars-6.0.sym
--rw-rw-rw-   0        0        0      163 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/test_extended_id_dump.sym
--rw-rw-rw-   0        0        0      217 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/test_multiplex_dump.sym
--rw-rw-rw-   0        0        0      410 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/type-extended-cycle-dash-p.sym
--rw-rw-rw-   0        0        0      379 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/files/sym/variables-color-enum-6.0.sym
--rw-rw-rw-   0        0        0     3025 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/test.mk
--rw-rw-rw-   0        0        0     8875 2023-04-27 09:16:42.000000 GBT_parser-1.0.24/tests/test_autosar.py
--rw-rw-rw-   0        0        0    22213 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/test_basic.c
--rw-rw-rw-   0        0        0    12895 2023-04-26 06:54:20.000000 GBT_parser-1.0.24/tests/test_bit_fields.c
--rw-rw-rw-   0        0        0    52984 2023-04-27 09:16:42.000000 GBT_parser-1.0.24/tests/test_command_line.py
--rw-rw-rw-   0        0        0     9322 2023-04-27 09:16:42.000000 GBT_parser-1.0.24/tests/test_convert.py
--rw-rw-rw-   0        0        0   279918 2023-04-27 09:17:03.000000 GBT_parser-1.0.24/tests/test_database.py
--rw-rw-rw-   0        0        0     1738 2023-04-27 09:16:43.000000 GBT_parser-1.0.24/tests/test_database_utils.py
--rw-rw-rw-   0        0        0    25231 2023-04-27 09:16:43.000000 GBT_parser-1.0.24/tests/test_diagnostics_database.py
--rw-rw-rw-   0        0        0    31403 2023-04-27 09:16:44.000000 GBT_parser-1.0.24/tests/test_dump.py
--rw-rw-rw-   0        0        0    19144 2023-04-27 09:16:44.000000 GBT_parser-1.0.24/tests/test_list.py
--rw-rw-rw-   0        0        0    23693 2023-04-27 09:16:44.000000 GBT_parser-1.0.24/tests/test_logreader.py
--rw-rw-rw-   0        0        0    57132 2023-04-27 09:16:45.000000 GBT_parser-1.0.24/tests/test_monitor.py
--rw-rw-rw-   0        0        0   108148 2023-04-27 09:16:45.000000 GBT_parser-1.0.24/tests/test_plot.py
--rw-rw-rw-   0        0        0     3940 2023-04-27 09:16:45.000000 GBT_parser-1.0.24/tests/test_plot_unittests.py
--rw-rw-rw-   0        0        0     3033 2023-04-27 09:16:46.000000 GBT_parser-1.0.24/tests/test_plot_without_mock.py
--rw-rw-rw-   0        0        0    11764 2023-04-27 09:16:46.000000 GBT_parser-1.0.24/tests/test_tester.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.903961 GBT_parser-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.581962 GBT_parser-1.0.4/GBT_parser.egg-info/
+-rw-rw-rw-   0        0        0      452 2023-05-26 10:54:59.000000 GBT_parser-1.0.4/GBT_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9817 2023-05-26 10:54:59.000000 GBT_parser-1.0.4/GBT_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 10:54:59.000000 GBT_parser-1.0.4/GBT_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-26 10:54:59.000000 GBT_parser-1.0.4/GBT_parser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      225 2023-05-26 10:54:59.000000 GBT_parser-1.0.4/GBT_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-26 10:54:59.000000 GBT_parser-1.0.4/GBT_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1107 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      116 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5142 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/Makefile
+-rw-rw-rw-   0        0        0      452 2023-05-26 10:54:59.903961 GBT_parser-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-27 08:27:25.000000 GBT_parser-1.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.596962 GBT_parser-1.0.4/cantools/
+-rw-rw-rw-   0        0        0     3122 2023-04-27 08:41:02.000000 GBT_parser-1.0.4/cantools/__init__.py
+-rw-rw-rw-   0        0        0       76 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/cantools/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.602962 GBT_parser-1.0.4/cantools/autosar/
+-rw-rw-rw-   0        0        0      129 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/autosar/__init__.py
+-rw-rw-rw-   0        0        0     5976 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/autosar/end_to_end.py
+-rw-rw-rw-   0        0        0     3885 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/autosar/secoc.py
+-rw-rw-rw-   0        0        0     1247 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/autosar/snakeauth.py
+-rw-rw-rw-   0        0        0      595 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/compat.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.607963 GBT_parser-1.0.4/cantools/database/
+-rw-rw-rw-   0        0        0    14667 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.623962 GBT_parser-1.0.4/cantools/database/can/
+-rw-rw-rw-   0        0        0      162 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/__init__.py
+-rw-rw-rw-   0        0        0      853 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/attribute.py
+-rw-rw-rw-   0        0        0     2326 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/attribute_definition.py
+-rw-rw-rw-   0        0        0     2594 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/bus.py
+-rw-rw-rw-   0        0        0    55788 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/c_source.py
+-rw-rw-rw-   0        0        0    18598 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/database.py
+-rw-rw-rw-   0        0        0     3497 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/environment_variable.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.631962 GBT_parser-1.0.4/cantools/database/can/formats/
+-rw-rw-rw-   0        0        0        0 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/cantools/database/can/formats/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.643963 GBT_parser-1.0.4/cantools/database/can/formats/arxml/
+-rw-rw-rw-   0        0        0     2731 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/formats/arxml/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/formats/arxml/bus_specifics.py
+-rw-rw-rw-   0        0        0      471 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/formats/arxml/database_specifics.py
+-rw-rw-rw-   0        0        0    13303 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/formats/arxml/ecu_extract_loader.py
+-rw-rw-rw-   0        0        0     1483 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/formats/arxml/end_to_end_properties.py
+-rw-rw-rw-   0        0        0     2119 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/formats/arxml/message_specifics.py
+-rw-rw-rw-   0        0        0      232 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/formats/arxml/node_specifics.py
+-rw-rw-rw-   0        0        0     3377 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/formats/arxml/secoc_properties.py
+-rw-rw-rw-   0        0        0   100529 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/formats/arxml/system_loader.py
+-rw-rw-rw-   0        0        0     1770 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/formats/arxml/utils.py
+-rw-rw-rw-   0        0        0    66250 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/formats/dbc.py
+-rw-rw-rw-   0        0        0     2546 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/formats/dbc_specifics.py
+-rw-rw-rw-   0        0        0    15993 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/formats/kcd.py
+-rw-rw-rw-   0        0        0    36438 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/formats/sym.py
+-rw-rw-rw-   0        0        0      369 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/cantools/database/can/formats/utils.py
+-rw-rw-rw-   0        0        0      861 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/internal_database.py
+-rw-rw-rw-   0        0        0    49341 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/message.py
+-rw-rw-rw-   0        0        0     3089 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/node.py
+-rw-rw-rw-   0        0        0    14595 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/signal.py
+-rw-rw-rw-   0        0        0     1386 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/can/signal_group.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.650961 GBT_parser-1.0.4/cantools/database/diagnostics/
+-rw-rw-rw-   0        0        0       78 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/diagnostics/__init__.py
+-rw-rw-rw-   0        0        0     2855 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/diagnostics/data.py
+-rw-rw-rw-   0        0        0     3311 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/diagnostics/database.py
+-rw-rw-rw-   0        0        0     3452 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/diagnostics/did.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.652963 GBT_parser-1.0.4/cantools/database/diagnostics/formats/
+-rw-rw-rw-   0        0        0        0 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/cantools/database/diagnostics/formats/__init__.py
+-rw-rw-rw-   0        0        0     6888 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/diagnostics/formats/cdd.py
+-rw-rw-rw-   0        0        0      170 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/diagnostics/internal_database.py
+-rw-rw-rw-   0        0        0      196 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/cantools/database/errors.py
+-rw-rw-rw-   0        0        0    15342 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/database/utils.py
+-rw-rw-rw-   0        0        0      105 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/cantools/errors.py
+-rw-rw-rw-   0        0        0     4748 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/j1939.py
+-rw-rw-rw-   0        0        0    15265 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/logreader.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.661961 GBT_parser-1.0.4/cantools/subparsers/
+-rw-rw-rw-   0        0        0        0 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/cantools/subparsers/__init__.py
+-rw-rw-rw-   0        0        0     7778 2023-05-26 10:23:50.000000 GBT_parser-1.0.4/cantools/subparsers/__utils__.py
+-rw-rw-rw-   0        0        0     1537 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/cantools/subparsers/convert.py
+-rw-rw-rw-   0        0        0     2794 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/subparsers/decode.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.664961 GBT_parser-1.0.4/cantools/subparsers/dump/
+-rw-rw-rw-   0        0        0     5995 2023-04-28 22:16:26.000000 GBT_parser-1.0.4/cantools/subparsers/dump/__init__.py
+-rw-rw-rw-   0        0        0    12225 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/subparsers/dump/formatting.py
+-rw-rw-rw-   0        0        0     4307 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/subparsers/generate_c_source.py
+-rw-rw-rw-   0        0        0    14663 2023-04-27 09:16:27.000000 GBT_parser-1.0.4/cantools/subparsers/list.py
+-rw-rw-rw-   0        0        0    23204 2023-05-26 09:16:34.000000 GBT_parser-1.0.4/cantools/subparsers/monitor.py
+-rw-rw-rw-   0        0        0    35519 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/subparsers/plot.py
+-rw-rw-rw-   0        0        0    16034 2023-04-27 09:03:36.000000 GBT_parser-1.0.4/cantools/tester.py
+-rw-rw-rw-   0        0        0     2109 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/cantools/typechecking.py
+-rw-rw-rw-   0        0        0       24 2023-05-26 10:54:51.000000 GBT_parser-1.0.4/cantools/version.py
+-rw-rw-rw-   0        0        0     1007 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 10:54:59.904961 GBT_parser-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1485 2023-05-13 12:31:04.000000 GBT_parser-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.685962 GBT_parser-1.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      295 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/dummy.c
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.545964 GBT_parser-1.0.4/tests/files/
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.701961 GBT_parser-1.0.4/tests/files/arxml/
+-rw-rw-rw-   0        0        0     9947 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/arxml/compu_method_no_category.arxml
+-rw-rw-rw-   0        0        0    18542 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/arxml/ecu-extract-4.2.arxml
+-rw-rw-rw-   0        0        0    38300 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/arxml/system-3.2.3.arxml
+-rw-rw-rw-   0        0        0    72577 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/arxml/system-4.2.arxml
+-rw-rw-rw-   0        0        0      282 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/arxml/system-DAI-3.1.2.arxml
+-rw-rw-rw-   0        0        0    14079 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/arxml/system-bad-root-tag-4.2.arxml
+-rw-rw-rw-   0        0        0     1302 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/arxml/system-dangling-reference-4.2.arxml
+-rw-rw-rw-   0        0        0    30885 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/arxml/system-float-values.arxml
+-rw-rw-rw-   0        0        0      264 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/arxml/system-illegal-namespace-4.2.arxml
+-rw-rw-rw-   0        0        0      265 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/arxml/system-illegal-root-4.2.arxml
+-rw-rw-rw-   0        0        0      273 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/arxml/system-illegal-version-4.2.2.1.0.arxml
+-rw-rw-rw-   0        0        0     4153 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/arxml/system-missing-denominator-4.2.arxml
+-rw-rw-rw-   0        0        0     4162 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/arxml/system-missing-factor-4.2.arxml
+-rw-rw-rw-   0        0        0     3943 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/arxml/system-missing-rational-4.2.arxml
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.771962 GBT_parser-1.0.4/tests/files/c_source/
+-rw-rw-rw-   0        0        0    54386 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/abs.c
+-rw-rw-rw-   0        0        0    96994 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/abs.h
+-rw-rw-rw-   0        0        0     1770 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/camel_case_empty.c
+-rw-rw-rw-   0        0        0     2807 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/camel_case_empty.h
+-rw-rw-rw-   0        0        0     2459 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/choices.c
+-rw-rw-rw-   0        0        0     3661 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/choices.h
+-rw-rw-rw-   0        0        0     6880 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/floating_point.c
+-rw-rw-rw-   0        0        0     6066 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/floating_point.h
+-rw-rw-rw-   0        0        0     7078 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/floating_point_bit_fields.c
+-rw-rw-rw-   0        0        0     6418 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/floating_point_bit_fields.h
+-rw-rw-rw-   0        0        0     8474 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/floating_point_use_float.c
+-rw-rw-rw-   0        0        0     8414 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/floating_point_use_float.h
+-rw-rw-rw-   0        0        0     1826 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/letter_terminated_can_id_6_0.c
+-rw-rw-rw-   0        0        0     2925 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/letter_terminated_can_id_6_0.h
+-rw-rw-rw-   0        0        0     5494 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/min_max_only_6_0.c
+-rw-rw-rw-   0        0        0     5898 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/min_max_only_6_0.h
+-rw-rw-rw-   0        0        0     4632 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/motohawk.c
+-rw-rw-rw-   0        0        0     5376 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/motohawk.h
+-rw-rw-rw-   0        0        0     4786 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/motohawk_bit_fields.c
+-rw-rw-rw-   0        0        0     5664 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/motohawk_bit_fields.h
+-rw-rw-rw-   0        0        0     3963 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/motohawk_no_floating_point_numbers.c
+-rw-rw-rw-   0        0        0     4114 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/motohawk_no_floating_point_numbers.h
+-rw-rw-rw-   0        0        0     4112 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/motohawk_sender_node.c
+-rw-rw-rw-   0        0        0     4956 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/motohawk_sender_node.h
+-rw-rw-rw-   0        0        0     3655 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/motohawk_sender_node_no_floating_point_numbers.c
+-rw-rw-rw-   0        0        0     4114 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/motohawk_sender_node_no_floating_point_numbers.h
+-rw-rw-rw-   0        0        0     8399 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/multiplex.c
+-rw-rw-rw-   0        0        0    11748 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/multiplex.h
+-rw-rw-rw-   0        0        0    19855 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/multiplex_2.c
+-rw-rw-rw-   0        0        0    19932 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/multiplex_2.h
+-rw-rw-rw-   0        0        0     7722 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/multiplex_2_fuzzer.c
+-rw-rw-rw-   0        0        0     5375 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/multiplex_2_fuzzer.h
+-rw-rw-rw-   0        0        0     1790 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/multiplex_2_fuzzer.mk
+-rw-rw-rw-   0        0        0     4744 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/my_database_name.c
+-rw-rw-rw-   0        0        0     5576 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/my_database_name.h
+-rw-rw-rw-   0        0        0     2138 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/no_signals.c
+-rw-rw-rw-   0        0        0     3820 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/no_signals.h
+-rw-rw-rw-   0        0        0    16637 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/open_actuator.c
+-rw-rw-rw-   0        0        0    26206 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/open_actuator.h
+-rw-rw-rw-   0        0        0    11894 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/open_actuator_no_floating_point_numbers.c
+-rw-rw-rw-   0        0        0    17130 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/open_actuator_no_floating_point_numbers.h
+-rw-rw-rw-   0        0        0     9754 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/open_actuator_sender_node.c
+-rw-rw-rw-   0        0        0    17669 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/open_actuator_sender_node.h
+-rw-rw-rw-   0        0        0     7625 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/open_actuator_sender_node_no_floating_point_numbers.c
+-rw-rw-rw-   0        0        0    13576 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/open_actuator_sender_node_no_floating_point_numbers.h
+-rw-rw-rw-   0        0        0    12653 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/padding_bit_order.c
+-rw-rw-rw-   0        0        0    16664 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/padding_bit_order.h
+-rw-rw-rw-   0        0        0    26296 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/signed.c
+-rw-rw-rw-   0        0        0    26265 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/signed.h
+-rw-rw-rw-   0        0        0    27385 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/signed_bit_fields.c
+-rw-rw-rw-   0        0        0    28251 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/signed_bit_fields.h
+-rw-rw-rw-   0        0        0   434422 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/c_source/vehicle.c
+-rw-rw-rw-   0        0        0   672980 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/c_source/vehicle.h
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.781961 GBT_parser-1.0.4/tests/files/cdd/
+-rw-rw-rw-   0        0        0   855589 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/cdd/example-diddatarefs.cdd
+-rw-rw-rw-   0        0        0   389046 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/cdd/example.cdd
+-rw-rw-rw-   0        0        0   389048 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/cdd/invalid-bo-example.cdd
+-rw-rw-rw-   0        0        0   389046 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/cdd/le-example.cdd
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.865961 GBT_parser-1.0.4/tests/files/dbc/
+-rw-rw-rw-   0        0        0      685 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/BU_BO_REL_.dbc
+-rw-rw-rw-   0        0        0      736 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/BU_BO_REL_Message.dbc
+-rw-rw-rw-   0        0        0       85 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/CamelCaseEmpty.dbc
+-rw-rw-rw-   0        0        0    14428 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/abs.dbc
+-rw-rw-rw-   0        0        0      428 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/add_two_dbc_files_1.dbc
+-rw-rw-rw-   0        0        0      409 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/add_two_dbc_files_2.dbc
+-rw-rw-rw-   0        0        0      650 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/attribute_Event.dbc
+-rw-rw-rw-   0        0        0     3269 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/attributes.dbc
+-rw-rw-rw-   0        0        0     1272 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/attributes_relation.dbc
+-rw-rw-rw-   0        0        0      471 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/bad_message_length.dbc
+-rw-rw-rw-   0        0        0     3303 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/big_numbers.dbc
+-rw-rw-rw-   0        0        0     2728 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/bus_comment.dbc
+-rw-rw-rw-   0        0        0      766 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/choices.dbc
+-rw-rw-rw-   0        0        0      748 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/choices_issue_with_name.dbc
+-rw-rw-rw-   0        0        0     1316 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/comments_hex_and_motorola_converted_from_sym.dbc
+-rw-rw-rw-   0        0        0      694 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/cp1252.dbc
+-rw-rw-rw-   0        0        0      651 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/dump_signal_choices.dbc
+-rw-rw-rw-   0        0        0     2099 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/emc32.dbc
+-rw-rw-rw-   0        0        0      811 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/empty_choice.dbc
+-rw-rw-rw-   0        0        0       38 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/empty_ns.dbc
+-rw-rw-rw-   0        0        0      891 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/floating_point.dbc
+-rw-rw-rw-   0        0        0      916 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/floating_point_use_float.dbc
+-rw-rw-rw-   0        0        0     2804 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/dbc/foobar.dbc
+-rw-rw-rw-   0        0        0     1222 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/issue_163_newline.dbc
+-rw-rw-rw-   0        0        0     2750 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/issue_168.DBC
+-rw-rw-rw-   0        0        0     3984 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/issue_184_extended_mux_cascaded.dbc
+-rw-rw-rw-   0        0        0     3991 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/issue_184_extended_mux_cascaded_dumped.dbc
+-rw-rw-rw-   0        0        0     4021 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/issue_184_extended_mux_independent_multiplexors.dbc
+-rw-rw-rw-   0        0        0     4030 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/issue_184_extended_mux_independent_multiplexors_dumped.dbc
+-rw-rw-rw-   0        0        0     3771 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/issue_184_extended_mux_multiple_values.dbc
+-rw-rw-rw-   0        0        0     3862 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/issue_184_extended_mux_multiple_values_dumped.dbc
+-rw-rw-rw-   0        0        0     3332 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/issue_199.dbc
+-rw-rw-rw-   0        0        0     3334 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/issue_199_extended.dbc
+-rw-rw-rw-   0        0        0      616 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/issue_207_sig_plus.dbc
+-rw-rw-rw-   0        0        0      811 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/issue_228.dbc
+-rw-rw-rw-   0        0        0     1671 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/issue_62.dbc
+-rw-rw-rw-   0        0        0      794 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/issue_63.dbc
+-rw-rw-rw-   0        0        0     3840 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/j1939.dbc
+-rw-rw-rw-   0        0        0     5044 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/long_names.dbc
+-rw-rw-rw-   0        0        0     5136 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/long_names_multiple_relations.dbc
+-rw-rw-rw-   0        0        0     5138 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/long_names_multiple_relations_dumped.dbc
+-rw-rw-rw-   0        0        0       85 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/message-dlc-zero.dbc
+-rw-rw-rw-   0        0        0      895 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/mod_name_len_dest.dbc
+-rw-rw-rw-   0        0        0     1198 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/mod_name_len_src.dbc
+-rw-rw-rw-   0        0        0      822 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/motohawk.dbc
+-rw-rw-rw-   0        0        0      996 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/motohawk_with_comments.dbc
+-rw-rw-rw-   0        0        0     4998 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/msxii_system_can.dbc
+-rw-rw-rw-   0        0        0      593 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/multiple_senders.dbc
+-rw-rw-rw-   0        0        0     2355 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/multiplex.dbc
+-rw-rw-rw-   0        0        0     5322 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/multiplex_2.dbc
+-rw-rw-rw-   0        0        0     5393 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/multiplex_2_dumped.dbc
+-rw-rw-rw-   0        0        0     3905 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/multiplex_choices.dbc
+-rw-rw-rw-   0        0        0     4784 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/multiplex_choices_dumped.dbc
+-rw-rw-rw-   0        0        0     2705 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/multiplex_dumped.dbc
+-rw-rw-rw-   0        0        0      580 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/no_sender.dbc
+-rw-rw-rw-   0        0        0      180 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/no_signals.dbc
+-rw-rw-rw-   0        0        0     2710 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/open_actuator.dbc
+-rw-rw-rw-   0        0        0     1035 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/padding_bit_order.dbc
+-rw-rw-rw-   0        0        0     1301 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/sig_groups.dbc
+-rw-rw-rw-   0        0        0     1164 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/sig_groups_del.dbc
+-rw-rw-rw-   0        0        0     1339 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/sig_groups_out.dbc
+-rw-rw-rw-   0        0        0     1774 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/signed.dbc
+-rw-rw-rw-   0        0        0     2765 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/socialledge-written-by-cantools-with-default-sort-signals.dbc
+-rw-rw-rw-   0        0        0     2765 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/socialledge-written-by-cantools-with-sort-signals-by-name.dbc
+-rw-rw-rw-   0        0        0     2765 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/socialledge-written-by-cantools.dbc
+-rw-rw-rw-   0        0        0     2808 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/socialledge.dbc
+-rw-rw-rw-   0        0        0      642 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/test_extended_id_dump.dbc
+-rw-rw-rw-   0        0        0      668 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/test_multiplex_dump.dbc
+-rw-rw-rw-   0        0        0      954 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/timing.dbc
+-rw-rw-rw-   0        0        0      767 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/val_table.dbc
+-rw-rw-rw-   0        0        0      542 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/variable_dlc.dbc
+-rw-rw-rw-   0        0        0    72742 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/dbc/vehicle.dbc
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.876961 GBT_parser-1.0.4/tests/files/kcd/
+-rw-rw-rw-   0        0        0      513 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/kcd/bad_message_length.kcd
+-rw-rw-rw-   0        0        0     2399 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/kcd/dump.kcd
+-rw-rw-rw-   0        0        0      189 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/kcd/empty.kcd
+-rw-rw-rw-   0        0        0     2457 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/kcd/message_layout.kcd
+-rw-rw-rw-   0        0        0     1240 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/kcd/signal_range.kcd
+-rw-rw-rw-   0        0        0     1219 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/kcd/tester.kcd
+-rw-rw-rw-   0        0        0    15989 2023-04-26 06:56:48.000000 GBT_parser-1.0.4/tests/files/kcd/the_homer.kcd
+-rw-rw-rw-   0        0        0   107162 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/kcd/vehicle.kcd
+drwxrwxrwx   0        0        0        0 2023-05-26 10:54:59.901960 GBT_parser-1.0.4/tests/files/sym/
+-rw-rw-rw-   0        0        0      188 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/bad_message_length.sym
+-rw-rw-rw-   0        0        0      296 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/big-endian.sym
+-rw-rw-rw-   0        0        0      839 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/comments_hex_and_motorola.sym
+-rw-rw-rw-   0        0        0       65 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/empty-6.0.sym
+-rw-rw-rw-   0        0        0      197 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/empty-enum-6.0.sym
+-rw-rw-rw-   0        0        0      539 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/issue_138.sym
+-rw-rw-rw-   0        0        0      557 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/jopp-5.0.sym
+-rw-rw-rw-   0        0        0      915 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/jopp-6.0.sym
+-rw-rw-rw-   0        0        0      159 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/letter-terminated-can-id-6.0.sym
+-rw-rw-rw-   0        0        0      324 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/min-max-only-6.0.sym
+-rw-rw-rw-   0        0        0      356 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/multiplexed_variables.sym
+-rw-rw-rw-   0        0        0      113 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/receive-6.0.sym
+-rw-rw-rw-   0        0        0      110 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/send-6.0.sym
+-rw-rw-rw-   0        0        0      161 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/sendreceive-6.0.sym
+-rw-rw-rw-   0        0        0      495 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/signal-types-6.0.sym
+-rw-rw-rw-   0        0        0      516 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/special-chars-6.0.sym
+-rw-rw-rw-   0        0        0      163 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/test_extended_id_dump.sym
+-rw-rw-rw-   0        0        0      217 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/test_multiplex_dump.sym
+-rw-rw-rw-   0        0        0      410 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/type-extended-cycle-dash-p.sym
+-rw-rw-rw-   0        0        0      379 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/files/sym/variables-color-enum-6.0.sym
+-rw-rw-rw-   0        0        0     3025 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/test.mk
+-rw-rw-rw-   0        0        0     8875 2023-04-27 09:16:42.000000 GBT_parser-1.0.4/tests/test_autosar.py
+-rw-rw-rw-   0        0        0    22213 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/test_basic.c
+-rw-rw-rw-   0        0        0    12895 2023-04-26 06:54:20.000000 GBT_parser-1.0.4/tests/test_bit_fields.c
+-rw-rw-rw-   0        0        0    52984 2023-04-27 09:16:42.000000 GBT_parser-1.0.4/tests/test_command_line.py
+-rw-rw-rw-   0        0        0     9322 2023-04-27 09:16:42.000000 GBT_parser-1.0.4/tests/test_convert.py
+-rw-rw-rw-   0        0        0   279918 2023-04-27 09:17:03.000000 GBT_parser-1.0.4/tests/test_database.py
+-rw-rw-rw-   0        0        0     1738 2023-04-27 09:16:43.000000 GBT_parser-1.0.4/tests/test_database_utils.py
+-rw-rw-rw-   0        0        0    25231 2023-04-27 09:16:43.000000 GBT_parser-1.0.4/tests/test_diagnostics_database.py
+-rw-rw-rw-   0        0        0    31403 2023-04-27 09:16:44.000000 GBT_parser-1.0.4/tests/test_dump.py
+-rw-rw-rw-   0        0        0    19144 2023-04-27 09:16:44.000000 GBT_parser-1.0.4/tests/test_list.py
+-rw-rw-rw-   0        0        0    23693 2023-04-27 09:16:44.000000 GBT_parser-1.0.4/tests/test_logreader.py
+-rw-rw-rw-   0        0        0    57132 2023-04-27 09:16:45.000000 GBT_parser-1.0.4/tests/test_monitor.py
+-rw-rw-rw-   0        0        0   108148 2023-04-27 09:16:45.000000 GBT_parser-1.0.4/tests/test_plot.py
+-rw-rw-rw-   0        0        0     3940 2023-04-27 09:16:45.000000 GBT_parser-1.0.4/tests/test_plot_unittests.py
+-rw-rw-rw-   0        0        0     3033 2023-04-27 09:16:46.000000 GBT_parser-1.0.4/tests/test_plot_without_mock.py
+-rw-rw-rw-   0        0        0    11764 2023-04-27 09:16:46.000000 GBT_parser-1.0.4/tests/test_tester.py
```

### Comparing `GBT_parser-1.0.24/GBT_parser.egg-info/SOURCES.txt` & `GBT_parser-1.0.4/GBT_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/LICENSE` & `GBT_parser-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/Makefile` & `GBT_parser-1.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/__init__.py` & `GBT_parser-1.0.4/cantools/__init__.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/autosar/end_to_end.py` & `GBT_parser-1.0.4/cantools/autosar/end_to_end.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/autosar/secoc.py` & `GBT_parser-1.0.4/cantools/autosar/secoc.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/autosar/snakeauth.py` & `GBT_parser-1.0.4/cantools/autosar/snakeauth.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/compat.py` & `GBT_parser-1.0.4/cantools/compat.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/__init__.py` & `GBT_parser-1.0.4/cantools/database/__init__.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/attribute.py` & `GBT_parser-1.0.4/cantools/database/can/attribute.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/attribute_definition.py` & `GBT_parser-1.0.4/cantools/database/can/attribute_definition.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/bus.py` & `GBT_parser-1.0.4/cantools/database/can/bus.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/c_source.py` & `GBT_parser-1.0.4/cantools/database/can/c_source.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/database.py` & `GBT_parser-1.0.4/cantools/database/can/database.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/environment_variable.py` & `GBT_parser-1.0.4/cantools/database/can/environment_variable.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/formats/arxml/__init__.py` & `GBT_parser-1.0.4/cantools/database/can/formats/arxml/__init__.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/formats/arxml/ecu_extract_loader.py` & `GBT_parser-1.0.4/cantools/database/can/formats/arxml/ecu_extract_loader.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/formats/arxml/end_to_end_properties.py` & `GBT_parser-1.0.4/cantools/database/can/formats/arxml/end_to_end_properties.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/formats/arxml/message_specifics.py` & `GBT_parser-1.0.4/cantools/database/can/formats/arxml/message_specifics.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/formats/arxml/secoc_properties.py` & `GBT_parser-1.0.4/cantools/database/can/formats/arxml/secoc_properties.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/formats/arxml/system_loader.py` & `GBT_parser-1.0.4/cantools/database/can/formats/arxml/system_loader.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/formats/arxml/utils.py` & `GBT_parser-1.0.4/cantools/database/can/formats/arxml/utils.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/formats/dbc.py` & `GBT_parser-1.0.4/cantools/database/can/formats/dbc.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/formats/dbc_specifics.py` & `GBT_parser-1.0.4/cantools/database/can/formats/dbc_specifics.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/formats/kcd.py` & `GBT_parser-1.0.4/cantools/database/can/formats/kcd.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/formats/sym.py` & `GBT_parser-1.0.4/cantools/database/can/formats/sym.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/internal_database.py` & `GBT_parser-1.0.4/cantools/database/can/internal_database.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/message.py` & `GBT_parser-1.0.4/cantools/database/can/message.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/node.py` & `GBT_parser-1.0.4/cantools/database/can/node.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/signal.py` & `GBT_parser-1.0.4/cantools/database/can/signal.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/can/signal_group.py` & `GBT_parser-1.0.4/cantools/database/can/signal_group.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/diagnostics/data.py` & `GBT_parser-1.0.4/cantools/database/diagnostics/data.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/diagnostics/database.py` & `GBT_parser-1.0.4/cantools/database/diagnostics/database.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/diagnostics/did.py` & `GBT_parser-1.0.4/cantools/database/diagnostics/did.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/diagnostics/formats/cdd.py` & `GBT_parser-1.0.4/cantools/database/diagnostics/formats/cdd.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/database/utils.py` & `GBT_parser-1.0.4/cantools/database/utils.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/j1939.py` & `GBT_parser-1.0.4/cantools/j1939.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/logreader.py` & `GBT_parser-1.0.4/cantools/logreader.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/subparsers/__utils__.py` & `GBT_parser-1.0.4/cantools/subparsers/__utils__.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/subparsers/convert.py` & `GBT_parser-1.0.4/cantools/subparsers/convert.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/subparsers/decode.py` & `GBT_parser-1.0.4/cantools/subparsers/decode.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/subparsers/dump/__init__.py` & `GBT_parser-1.0.4/cantools/subparsers/dump/__init__.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/subparsers/dump/formatting.py` & `GBT_parser-1.0.4/cantools/subparsers/dump/formatting.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/subparsers/generate_c_source.py` & `GBT_parser-1.0.4/cantools/subparsers/generate_c_source.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/subparsers/list.py` & `GBT_parser-1.0.4/cantools/subparsers/list.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/subparsers/monitor.py` & `GBT_parser-1.0.4/cantools/subparsers/monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import argparse
 import bisect
 import curses
 import queue
 import re
 import time
-import logging
+
 import can
 from argparse_addons import Integer
-import datetime
+
 from .. import database
 from .__utils__ import format_message, format_multiplexed_name
-import os
+
+
 class QuitError(Exception):
     pass
+import cantools
 class Monitor(can.Listener):
 
     def __init__(self, stdscr, args):
         self._stdscr = stdscr
         print(f'Reading bus description file "{args.database}"...\r')
         self._dbase = database.load_file(args.database,
                                          encoding=args.encoding,
@@ -30,52 +32,36 @@
         self._compiled_filter = None
         self._formatted_messages = {}
         self._playing = True
         self._modified = True
         self._show_filter = False
         self._queue = queue.Queue()
         self._nrows, self._ncols = stdscr.getmaxyx()
-        self._count =1
+        # self._nrows = 11
+        # self._ncols = 17
         self._received = 0
         self._discarded = 0
         self._basetime = None
         self._page_first_row = 0
         self.multi_packet_payload_size = None
         self.multi_packet_num_packets = None
         self.multi_packet_pgn = None
         self.multi_packet_buffer = None
-        self._log = args.log
+
         stdscr.keypad(True)
         stdscr.nodelay(True)
         curses.use_default_colors()
         curses.curs_set(False)
         curses.init_pair(1, curses.COLOR_BLACK, curses.COLOR_GREEN)
         curses.init_pair(2, curses.COLOR_BLACK, curses.COLOR_CYAN)
         curses.init_pair(3, curses.COLOR_CYAN, curses.COLOR_BLACK)
 
-        if self._log: 
-            current_datetime = datetime.datetime.now()
-            datetime_string = current_datetime.strftime("%Y-%m-%d_%H-%M-%S")
-            log_file_path = os.path.join(os.getcwd(), f"Log_{datetime_string}.trc")
-            self.logger = logging.getLogger('can_logger')
-            self.logger.setLevel(logging.INFO)
-            file_handler = logging.FileHandler(log_file_path )
-            file_handler.setLevel(logging.INFO)
-            self.logger.addHandler(file_handler)   
-
         bus = self.create_bus(args)
-
         self._notifier = can.Notifier(bus, [self])
 
-
-    def finish_logging(self):
-        for handler in self.logger.handlers:
-            handler.close()
-        logging.shutdown()
-
     def create_bus(self, args):
         kwargs = {}
 
         if args.bit_rate is not None:
             kwargs['bitrate'] = int(args.bit_rate)
 
         if args.fd:
@@ -232,16 +218,14 @@
             if self._show_filter:
                 self.process_user_input_filter(key)
             else:
                 self.process_user_input_menu(key)
 
     def process_user_input_menu(self, key):
         if key == 'q':
-            if self._log: 
-                self.finish_logging()
             raise QuitError()
         elif key == 'p':
             self._playing = not self._playing
         elif key == 'r':
             self._playing = True
             self._filtered_sorted_message_names = []
             self._formatted_messages = {}
@@ -407,36 +391,29 @@
         
             
 ###################################################
     def try_update_message(self,message):
         # message = self._queue.get_nowait()
         frame_id = message.arbitration_id
         data = message.data
-        dlc= message.dlc
         timestamp = message.timestamp
-        
+
         if self._basetime is None:
             self._basetime = timestamp
 
         timestamp -= self._basetime
         self._received += 1
         # The above code is retrieving a message from a database based on a given frame ID. The
         # `get_message_by_frame_id()` method is called on the `_dbase` object, passing in the
         # `frame_id` variable as an argument. The retrieved message is then assigned to the
         # `message` variable.
         # message = self._dbase.get_message_by_frame_id(frame_id)
 
         try:
             message = self._dbase.get_message_by_frame_id(frame_id)
-            if self._log: 
-                timestamp =  round((timestamp*1000), 1)
-                log_str = f"{self._count:>6})   {timestamp:>9}  Rx     {frame_id:08X}  {dlc}  {' '.join(f'{b:02X}' for b in data)}"
-                self.logger.info(log_str)
-                self._count += 1
-            
         except KeyError:
             self._discarded += 1
             return
 
         if message.is_container:
             self._try_update_container(message, timestamp, data)
             return
@@ -674,13 +651,8 @@
     monitor_parser.add_argument(
         '--no-strict',
         action='store_true',
         help='Skip database consistency checks.')
     monitor_parser.add_argument(
         'database',
         help='Database file.')
-    monitor_parser.add_argument(
-        '-l','--log',
-        action='store_true',
-        help='To save a log file.')
     monitor_parser.set_defaults(func=_do_monitor)
-
```

### Comparing `GBT_parser-1.0.24/cantools/subparsers/plot.py` & `GBT_parser-1.0.4/cantools/subparsers/plot.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/tester.py` & `GBT_parser-1.0.4/cantools/tester.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/cantools/typechecking.py` & `GBT_parser-1.0.4/cantools/typechecking.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/pyproject.toml` & `GBT_parser-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/setup.py` & `GBT_parser-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
       install_requires=[
           'bitstruct>=8.16.1',
           'python-can>=3.3.4',
           'textparser>=0.21.1',
           'diskcache',
           'argparse_addons',
           'typing_extensions>=3.10.0.0',
-          'crccheck',
+          'crccheck'
           'windows-curses',
       ],
       extras_require={
           'plot': ['matplotlib'],
           'windows-all': ["windows-curses;platform_system=='Windows'"],
       },
       test_suite="tests",
```

### Comparing `GBT_parser-1.0.24/tests/files/arxml/compu_method_no_category.arxml` & `GBT_parser-1.0.4/tests/files/arxml/compu_method_no_category.arxml`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/arxml/ecu-extract-4.2.arxml` & `GBT_parser-1.0.4/tests/files/arxml/ecu-extract-4.2.arxml`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/arxml/system-3.2.3.arxml` & `GBT_parser-1.0.4/tests/files/arxml/system-3.2.3.arxml`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/arxml/system-4.2.arxml` & `GBT_parser-1.0.4/tests/files/arxml/system-4.2.arxml`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/arxml/system-bad-root-tag-4.2.arxml` & `GBT_parser-1.0.4/tests/files/arxml/system-bad-root-tag-4.2.arxml`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/arxml/system-dangling-reference-4.2.arxml` & `GBT_parser-1.0.4/tests/files/arxml/system-dangling-reference-4.2.arxml`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/arxml/system-float-values.arxml` & `GBT_parser-1.0.4/tests/files/arxml/system-float-values.arxml`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/arxml/system-missing-denominator-4.2.arxml` & `GBT_parser-1.0.4/tests/files/arxml/system-missing-denominator-4.2.arxml`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/arxml/system-missing-factor-4.2.arxml` & `GBT_parser-1.0.4/tests/files/arxml/system-missing-factor-4.2.arxml`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/arxml/system-missing-rational-4.2.arxml` & `GBT_parser-1.0.4/tests/files/arxml/system-missing-rational-4.2.arxml`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/abs.c` & `GBT_parser-1.0.4/tests/files/c_source/abs.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/abs.h` & `GBT_parser-1.0.4/tests/files/c_source/abs.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/camel_case_empty.c` & `GBT_parser-1.0.4/tests/files/c_source/camel_case_empty.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/camel_case_empty.h` & `GBT_parser-1.0.4/tests/files/c_source/camel_case_empty.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/choices.c` & `GBT_parser-1.0.4/tests/files/c_source/choices.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/choices.h` & `GBT_parser-1.0.4/tests/files/c_source/choices.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/floating_point.c` & `GBT_parser-1.0.4/tests/files/c_source/floating_point.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/floating_point.h` & `GBT_parser-1.0.4/tests/files/c_source/floating_point.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/floating_point_bit_fields.c` & `GBT_parser-1.0.4/tests/files/c_source/floating_point_bit_fields.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/floating_point_bit_fields.h` & `GBT_parser-1.0.4/tests/files/c_source/floating_point_bit_fields.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/floating_point_use_float.c` & `GBT_parser-1.0.4/tests/files/c_source/floating_point_use_float.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/floating_point_use_float.h` & `GBT_parser-1.0.4/tests/files/c_source/floating_point_use_float.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/letter_terminated_can_id_6_0.c` & `GBT_parser-1.0.4/tests/files/c_source/letter_terminated_can_id_6_0.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/letter_terminated_can_id_6_0.h` & `GBT_parser-1.0.4/tests/files/c_source/letter_terminated_can_id_6_0.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/min_max_only_6_0.c` & `GBT_parser-1.0.4/tests/files/c_source/min_max_only_6_0.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/min_max_only_6_0.h` & `GBT_parser-1.0.4/tests/files/c_source/min_max_only_6_0.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/motohawk.c` & `GBT_parser-1.0.4/tests/files/c_source/motohawk.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/motohawk.h` & `GBT_parser-1.0.4/tests/files/c_source/motohawk.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/motohawk_bit_fields.c` & `GBT_parser-1.0.4/tests/files/c_source/motohawk_bit_fields.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/motohawk_bit_fields.h` & `GBT_parser-1.0.4/tests/files/c_source/motohawk_bit_fields.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/motohawk_no_floating_point_numbers.c` & `GBT_parser-1.0.4/tests/files/c_source/motohawk_no_floating_point_numbers.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/motohawk_no_floating_point_numbers.h` & `GBT_parser-1.0.4/tests/files/c_source/motohawk_no_floating_point_numbers.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/motohawk_sender_node.c` & `GBT_parser-1.0.4/tests/files/c_source/motohawk_sender_node.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/motohawk_sender_node.h` & `GBT_parser-1.0.4/tests/files/c_source/motohawk_sender_node.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/motohawk_sender_node_no_floating_point_numbers.c` & `GBT_parser-1.0.4/tests/files/c_source/motohawk_sender_node_no_floating_point_numbers.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/motohawk_sender_node_no_floating_point_numbers.h` & `GBT_parser-1.0.4/tests/files/c_source/motohawk_sender_node_no_floating_point_numbers.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/multiplex.c` & `GBT_parser-1.0.4/tests/files/c_source/multiplex.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/multiplex.h` & `GBT_parser-1.0.4/tests/files/c_source/multiplex.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/multiplex_2.c` & `GBT_parser-1.0.4/tests/files/c_source/multiplex_2.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/multiplex_2.h` & `GBT_parser-1.0.4/tests/files/c_source/multiplex_2.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/multiplex_2_fuzzer.c` & `GBT_parser-1.0.4/tests/files/c_source/multiplex_2_fuzzer.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/multiplex_2_fuzzer.h` & `GBT_parser-1.0.4/tests/files/c_source/multiplex_2_fuzzer.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/multiplex_2_fuzzer.mk` & `GBT_parser-1.0.4/tests/files/c_source/multiplex_2_fuzzer.mk`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/my_database_name.c` & `GBT_parser-1.0.4/tests/files/c_source/my_database_name.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/my_database_name.h` & `GBT_parser-1.0.4/tests/files/c_source/my_database_name.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/no_signals.c` & `GBT_parser-1.0.4/tests/files/c_source/no_signals.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/no_signals.h` & `GBT_parser-1.0.4/tests/files/c_source/no_signals.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/open_actuator.c` & `GBT_parser-1.0.4/tests/files/c_source/open_actuator.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/open_actuator.h` & `GBT_parser-1.0.4/tests/files/c_source/open_actuator.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/open_actuator_no_floating_point_numbers.c` & `GBT_parser-1.0.4/tests/files/c_source/open_actuator_no_floating_point_numbers.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/open_actuator_no_floating_point_numbers.h` & `GBT_parser-1.0.4/tests/files/c_source/open_actuator_no_floating_point_numbers.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/open_actuator_sender_node.c` & `GBT_parser-1.0.4/tests/files/c_source/open_actuator_sender_node.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/open_actuator_sender_node.h` & `GBT_parser-1.0.4/tests/files/c_source/open_actuator_sender_node.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/open_actuator_sender_node_no_floating_point_numbers.c` & `GBT_parser-1.0.4/tests/files/c_source/open_actuator_sender_node_no_floating_point_numbers.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/open_actuator_sender_node_no_floating_point_numbers.h` & `GBT_parser-1.0.4/tests/files/c_source/open_actuator_sender_node_no_floating_point_numbers.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/padding_bit_order.c` & `GBT_parser-1.0.4/tests/files/c_source/padding_bit_order.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/padding_bit_order.h` & `GBT_parser-1.0.4/tests/files/c_source/padding_bit_order.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/signed.c` & `GBT_parser-1.0.4/tests/files/c_source/signed.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/signed.h` & `GBT_parser-1.0.4/tests/files/c_source/signed.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/signed_bit_fields.c` & `GBT_parser-1.0.4/tests/files/c_source/signed_bit_fields.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/signed_bit_fields.h` & `GBT_parser-1.0.4/tests/files/c_source/signed_bit_fields.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/vehicle.c` & `GBT_parser-1.0.4/tests/files/c_source/vehicle.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/c_source/vehicle.h` & `GBT_parser-1.0.4/tests/files/c_source/vehicle.h`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/cdd/example-diddatarefs.cdd` & `GBT_parser-1.0.4/tests/files/cdd/example-diddatarefs.cdd`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/cdd/example.cdd` & `GBT_parser-1.0.4/tests/files/cdd/example.cdd`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/cdd/invalid-bo-example.cdd` & `GBT_parser-1.0.4/tests/files/cdd/invalid-bo-example.cdd`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/cdd/le-example.cdd` & `GBT_parser-1.0.4/tests/files/cdd/le-example.cdd`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/BU_BO_REL_.dbc` & `GBT_parser-1.0.4/tests/files/dbc/BU_BO_REL_.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/BU_BO_REL_Message.dbc` & `GBT_parser-1.0.4/tests/files/dbc/BU_BO_REL_Message.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/abs.dbc` & `GBT_parser-1.0.4/tests/files/dbc/abs.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/attribute_Event.dbc` & `GBT_parser-1.0.4/tests/files/dbc/attribute_Event.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/attributes.dbc` & `GBT_parser-1.0.4/tests/files/dbc/attributes.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/attributes_relation.dbc` & `GBT_parser-1.0.4/tests/files/dbc/attributes_relation.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/big_numbers.dbc` & `GBT_parser-1.0.4/tests/files/dbc/big_numbers.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/bus_comment.dbc` & `GBT_parser-1.0.4/tests/files/dbc/bus_comment.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/choices.dbc` & `GBT_parser-1.0.4/tests/files/dbc/choices.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/choices_issue_with_name.dbc` & `GBT_parser-1.0.4/tests/files/dbc/choices_issue_with_name.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/comments_hex_and_motorola_converted_from_sym.dbc` & `GBT_parser-1.0.4/tests/files/dbc/comments_hex_and_motorola_converted_from_sym.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/cp1252.dbc` & `GBT_parser-1.0.4/tests/files/dbc/cp1252.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/dump_signal_choices.dbc` & `GBT_parser-1.0.4/tests/files/dbc/dump_signal_choices.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/emc32.dbc` & `GBT_parser-1.0.4/tests/files/dbc/emc32.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/empty_choice.dbc` & `GBT_parser-1.0.4/tests/files/dbc/empty_choice.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/floating_point.dbc` & `GBT_parser-1.0.4/tests/files/dbc/floating_point.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/floating_point_use_float.dbc` & `GBT_parser-1.0.4/tests/files/dbc/floating_point_use_float.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/foobar.dbc` & `GBT_parser-1.0.4/tests/files/dbc/foobar.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/issue_163_newline.dbc` & `GBT_parser-1.0.4/tests/files/dbc/issue_163_newline.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/issue_168.DBC` & `GBT_parser-1.0.4/tests/files/dbc/issue_168.DBC`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/issue_184_extended_mux_cascaded.dbc` & `GBT_parser-1.0.4/tests/files/dbc/issue_184_extended_mux_cascaded.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/issue_184_extended_mux_cascaded_dumped.dbc` & `GBT_parser-1.0.4/tests/files/dbc/issue_184_extended_mux_cascaded_dumped.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/issue_184_extended_mux_independent_multiplexors.dbc` & `GBT_parser-1.0.4/tests/files/dbc/issue_184_extended_mux_independent_multiplexors.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/issue_184_extended_mux_independent_multiplexors_dumped.dbc` & `GBT_parser-1.0.4/tests/files/dbc/issue_184_extended_mux_independent_multiplexors_dumped.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/issue_184_extended_mux_multiple_values.dbc` & `GBT_parser-1.0.4/tests/files/dbc/issue_184_extended_mux_multiple_values.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/issue_184_extended_mux_multiple_values_dumped.dbc` & `GBT_parser-1.0.4/tests/files/dbc/issue_184_extended_mux_multiple_values_dumped.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/issue_199.dbc` & `GBT_parser-1.0.4/tests/files/dbc/issue_199.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/issue_199_extended.dbc` & `GBT_parser-1.0.4/tests/files/dbc/issue_199_extended.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/issue_207_sig_plus.dbc` & `GBT_parser-1.0.4/tests/files/dbc/issue_207_sig_plus.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/issue_228.dbc` & `GBT_parser-1.0.4/tests/files/dbc/issue_228.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/issue_62.dbc` & `GBT_parser-1.0.4/tests/files/dbc/issue_62.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/issue_63.dbc` & `GBT_parser-1.0.4/tests/files/dbc/issue_63.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/j1939.dbc` & `GBT_parser-1.0.4/tests/files/dbc/j1939.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/long_names.dbc` & `GBT_parser-1.0.4/tests/files/dbc/long_names.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/long_names_multiple_relations.dbc` & `GBT_parser-1.0.4/tests/files/dbc/long_names_multiple_relations.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/long_names_multiple_relations_dumped.dbc` & `GBT_parser-1.0.4/tests/files/dbc/long_names_multiple_relations_dumped.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/mod_name_len_dest.dbc` & `GBT_parser-1.0.4/tests/files/dbc/mod_name_len_dest.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/mod_name_len_src.dbc` & `GBT_parser-1.0.4/tests/files/dbc/mod_name_len_src.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/motohawk.dbc` & `GBT_parser-1.0.4/tests/files/dbc/motohawk.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/motohawk_with_comments.dbc` & `GBT_parser-1.0.4/tests/files/dbc/motohawk_with_comments.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/msxii_system_can.dbc` & `GBT_parser-1.0.4/tests/files/dbc/msxii_system_can.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/multiple_senders.dbc` & `GBT_parser-1.0.4/tests/files/dbc/multiple_senders.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/multiplex.dbc` & `GBT_parser-1.0.4/tests/files/dbc/multiplex.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/multiplex_2.dbc` & `GBT_parser-1.0.4/tests/files/dbc/multiplex_2.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/multiplex_2_dumped.dbc` & `GBT_parser-1.0.4/tests/files/dbc/multiplex_2_dumped.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/multiplex_choices.dbc` & `GBT_parser-1.0.4/tests/files/dbc/multiplex_choices.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/multiplex_choices_dumped.dbc` & `GBT_parser-1.0.4/tests/files/dbc/multiplex_choices_dumped.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/multiplex_dumped.dbc` & `GBT_parser-1.0.4/tests/files/dbc/multiplex_dumped.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/no_sender.dbc` & `GBT_parser-1.0.4/tests/files/dbc/no_sender.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/open_actuator.dbc` & `GBT_parser-1.0.4/tests/files/dbc/open_actuator.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/padding_bit_order.dbc` & `GBT_parser-1.0.4/tests/files/dbc/padding_bit_order.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/sig_groups.dbc` & `GBT_parser-1.0.4/tests/files/dbc/sig_groups.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/sig_groups_del.dbc` & `GBT_parser-1.0.4/tests/files/dbc/sig_groups_del.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/sig_groups_out.dbc` & `GBT_parser-1.0.4/tests/files/dbc/sig_groups_out.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/signed.dbc` & `GBT_parser-1.0.4/tests/files/dbc/signed.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/socialledge-written-by-cantools-with-default-sort-signals.dbc` & `GBT_parser-1.0.4/tests/files/dbc/socialledge-written-by-cantools-with-default-sort-signals.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/socialledge-written-by-cantools-with-sort-signals-by-name.dbc` & `GBT_parser-1.0.4/tests/files/dbc/socialledge-written-by-cantools-with-sort-signals-by-name.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/socialledge-written-by-cantools.dbc` & `GBT_parser-1.0.4/tests/files/dbc/socialledge-written-by-cantools.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/socialledge.dbc` & `GBT_parser-1.0.4/tests/files/dbc/socialledge.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/test_extended_id_dump.dbc` & `GBT_parser-1.0.4/tests/files/dbc/test_extended_id_dump.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/test_multiplex_dump.dbc` & `GBT_parser-1.0.4/tests/files/dbc/test_multiplex_dump.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/timing.dbc` & `GBT_parser-1.0.4/tests/files/dbc/timing.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/val_table.dbc` & `GBT_parser-1.0.4/tests/files/dbc/val_table.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/variable_dlc.dbc` & `GBT_parser-1.0.4/tests/files/dbc/variable_dlc.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/dbc/vehicle.dbc` & `GBT_parser-1.0.4/tests/files/dbc/vehicle.dbc`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/kcd/bad_message_length.kcd` & `GBT_parser-1.0.4/tests/files/kcd/bad_message_length.kcd`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/kcd/dump.kcd` & `GBT_parser-1.0.4/tests/files/kcd/dump.kcd`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/kcd/message_layout.kcd` & `GBT_parser-1.0.4/tests/files/kcd/message_layout.kcd`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/kcd/signal_range.kcd` & `GBT_parser-1.0.4/tests/files/kcd/signal_range.kcd`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/kcd/tester.kcd` & `GBT_parser-1.0.4/tests/files/kcd/tester.kcd`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/kcd/the_homer.kcd` & `GBT_parser-1.0.4/tests/files/kcd/the_homer.kcd`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/kcd/vehicle.kcd` & `GBT_parser-1.0.4/tests/files/kcd/vehicle.kcd`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/sym/comments_hex_and_motorola.sym` & `GBT_parser-1.0.4/tests/files/sym/comments_hex_and_motorola.sym`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/sym/issue_138.sym` & `GBT_parser-1.0.4/tests/files/sym/issue_138.sym`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/sym/jopp-5.0.sym` & `GBT_parser-1.0.4/tests/files/sym/jopp-5.0.sym`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/sym/jopp-6.0.sym` & `GBT_parser-1.0.4/tests/files/sym/jopp-6.0.sym`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/files/sym/special-chars-6.0.sym` & `GBT_parser-1.0.4/tests/files/sym/special-chars-6.0.sym`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/test.mk` & `GBT_parser-1.0.4/tests/test.mk`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/test_autosar.py` & `GBT_parser-1.0.4/tests/test_autosar.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/test_basic.c` & `GBT_parser-1.0.4/tests/test_basic.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/test_bit_fields.c` & `GBT_parser-1.0.4/tests/test_bit_fields.c`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/test_command_line.py` & `GBT_parser-1.0.4/tests/test_command_line.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/test_convert.py` & `GBT_parser-1.0.4/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/test_database.py` & `GBT_parser-1.0.4/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/test_database_utils.py` & `GBT_parser-1.0.4/tests/test_database_utils.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/test_diagnostics_database.py` & `GBT_parser-1.0.4/tests/test_diagnostics_database.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/test_dump.py` & `GBT_parser-1.0.4/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/test_list.py` & `GBT_parser-1.0.4/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/test_logreader.py` & `GBT_parser-1.0.4/tests/test_logreader.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/test_monitor.py` & `GBT_parser-1.0.4/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/test_plot.py` & `GBT_parser-1.0.4/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/test_plot_unittests.py` & `GBT_parser-1.0.4/tests/test_plot_unittests.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/test_plot_without_mock.py` & `GBT_parser-1.0.4/tests/test_plot_without_mock.py`

 * *Files identical despite different names*

### Comparing `GBT_parser-1.0.24/tests/test_tester.py` & `GBT_parser-1.0.4/tests/test_tester.py`

 * *Files identical despite different names*

