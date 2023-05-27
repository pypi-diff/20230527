# Comparing `tmp/DAWG2-0.9.0.tar.gz` & `tmp/DAWG2-0.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DAWG2-0.9.0.tar", last modified: Sat May 27 18:11:10 2023, max compression
+gzip compressed data, was "DAWG2-0.9.0rc1.tar", last modified: Tue May 23 19:51:40 2023, max compression
```

## Comparing `DAWG2-0.9.0.tar` & `DAWG2-0.9.0rc1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:11:10.351655 DAWG2-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-27 18:10:59.000000 DAWG2-0.9.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-27 18:10:59.000000 DAWG2-0.9.0/CHANGES.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:11:10.339655 DAWG2-0.9.0/DAWG2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-05-27 18:11:10.000000 DAWG2-0.9.0/DAWG2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-27 18:11:10.000000 DAWG2-0.9.0/DAWG2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 18:11:10.000000 DAWG2-0.9.0/DAWG2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-27 18:11:10.000000 DAWG2-0.9.0/DAWG2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-27 18:10:59.000000 DAWG2-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-27 18:10:59.000000 DAWG2-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-05-27 18:11:10.347655 DAWG2-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-27 18:10:59.000000 DAWG2-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:11:10.339655 DAWG2-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-05-27 18:10:59.000000 DAWG2-0.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-05-27 18:10:59.000000 DAWG2-0.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-05-27 18:10:59.000000 DAWG2-0.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-05-27 18:10:59.000000 DAWG2-0.9.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:11:10.339655 DAWG2-0.9.0/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/COPYING
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:11:10.339655 DAWG2-0.9.0/lib/b64/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2502 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/b64/cdecode.c
--rwxr-xr-x   0 runner    (1001) docker     (123)      648 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/b64/cdecode.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     2557 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/b64/cencode.c
--rwxr-xr-x   0 runner    (1001) docker     (123)      723 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/b64/cencode.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1427 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/b64/decode.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/b64/encode.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:11:10.343654 DAWG2-0.9.0/lib/dawgdic/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/base-types.h
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/base-unit.h
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/bit-pool.h
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/completer.h
--rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/dawg-builder.h
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/dawg-unit.h
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/dawg.h
--rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/dictionary-builder.h
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/dictionary-extra-unit.h
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/dictionary-unit.h
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/dictionary.h
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/guide-builder.h
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/guide-unit.h
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/guide.h
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/link-table.h
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/object-pool.h
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/ranked-completer-candidate.h
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/ranked-completer-node.h
--rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/ranked-completer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/ranked-guide-builder.h
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/ranked-guide-link.h
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/ranked-guide-unit.h
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-27 18:10:59.000000 DAWG2-0.9.0/lib/dawgdic/ranked-guide.h
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 18:11:10.351655 DAWG2-0.9.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1648 2023-05-27 18:10:59.000000 DAWG2-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:11:10.347655 DAWG2-0.9.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)   107216 2023-05-27 18:11:09.000000 DAWG2-0.9.0/src/_base_types.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-27 18:10:59.000000 DAWG2-0.9.0/src/_base_types.pxd
--rw-r--r--   0 runner    (1001) docker     (123)   108028 2023-05-27 18:11:09.000000 DAWG2-0.9.0/src/_completer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-27 18:10:59.000000 DAWG2-0.9.0/src/_completer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)   107155 2023-05-27 18:11:09.000000 DAWG2-0.9.0/src/_dawg.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-27 18:10:59.000000 DAWG2-0.9.0/src/_dawg.pxd
--rw-r--r--   0 runner    (1001) docker     (123)   107408 2023-05-27 18:11:09.000000 DAWG2-0.9.0/src/_dawg_builder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-27 18:10:59.000000 DAWG2-0.9.0/src/_dawg_builder.pxd
--rw-r--r--   0 runner    (1001) docker     (123)   107781 2023-05-27 18:11:09.000000 DAWG2-0.9.0/src/_dictionary.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-27 18:10:59.000000 DAWG2-0.9.0/src/_dictionary.pxd
--rw-r--r--   0 runner    (1001) docker     (123)   108081 2023-05-27 18:11:09.000000 DAWG2-0.9.0/src/_dictionary_builder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-27 18:10:59.000000 DAWG2-0.9.0/src/_dictionary_builder.pxd
--rw-r--r--   0 runner    (1001) docker     (123)   107462 2023-05-27 18:11:09.000000 DAWG2-0.9.0/src/_dictionary_unit.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-27 18:10:59.000000 DAWG2-0.9.0/src/_dictionary_unit.pxd
--rw-r--r--   0 runner    (1001) docker     (123)   107631 2023-05-27 18:11:09.000000 DAWG2-0.9.0/src/_guide.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-27 18:10:59.000000 DAWG2-0.9.0/src/_guide.pxd
--rw-r--r--   0 runner    (1001) docker     (123)   108111 2023-05-27 18:11:09.000000 DAWG2-0.9.0/src/_guide_builder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-27 18:10:59.000000 DAWG2-0.9.0/src/_guide_builder.pxd
--rw-r--r--   0 runner    (1001) docker     (123)   107327 2023-05-27 18:11:09.000000 DAWG2-0.9.0/src/_guide_unit.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-27 18:10:59.000000 DAWG2-0.9.0/src/_guide_unit.pxd
--rw-r--r--   0 runner    (1001) docker     (123)   107507 2023-05-27 18:11:09.000000 DAWG2-0.9.0/src/b64_decode.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-27 18:10:59.000000 DAWG2-0.9.0/src/b64_decode.pxd
--rw-r--r--   0 runner    (1001) docker     (123)  1133784 2023-05-27 18:11:09.000000 DAWG2-0.9.0/src/dawg.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    30775 2023-05-27 18:10:59.000000 DAWG2-0.9.0/src/dawg.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   107344 2023-05-27 18:11:10.000000 DAWG2-0.9.0/src/iostream.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-27 18:10:59.000000 DAWG2-0.9.0/src/iostream.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:11:10.347655 DAWG2-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-27 18:10:59.000000 DAWG2-0.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-27 18:10:59.000000 DAWG2-0.9.0/tests/test_dawg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-27 18:10:59.000000 DAWG2-0.9.0/tests/test_payload_dawg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-27 18:10:59.000000 DAWG2-0.9.0/tests/test_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-27 18:10:59.000000 DAWG2-0.9.0/tox.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-05-27 18:10:59.000000 DAWG2-0.9.0/update_cpp.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:51:40.936749 DAWG2-0.9.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/CHANGES.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:51:40.924749 DAWG2-0.9.0rc1/DAWG2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-23 19:51:40.000000 DAWG2-0.9.0rc1/DAWG2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-23 19:51:40.000000 DAWG2-0.9.0rc1/DAWG2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:51:40.000000 DAWG2-0.9.0rc1/DAWG2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 19:51:40.000000 DAWG2-0.9.0rc1/DAWG2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-23 19:51:40.936749 DAWG2-0.9.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:51:40.924749 DAWG2-0.9.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:51:40.924749 DAWG2-0.9.0rc1/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/COPYING
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:51:40.928749 DAWG2-0.9.0rc1/lib/b64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2502 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/b64/cdecode.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)      648 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/b64/cdecode.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2557 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/b64/cencode.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)      723 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/b64/cencode.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1427 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/b64/decode.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/b64/encode.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:51:40.928749 DAWG2-0.9.0rc1/lib/dawgdic/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/base-types.h
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/base-unit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/bit-pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/completer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/dawg-builder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/dawg-unit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/dawg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/dictionary-builder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/dictionary-extra-unit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/dictionary-unit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/dictionary.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/guide-builder.h
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/guide-unit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/guide.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/link-table.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/object-pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/ranked-completer-candidate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/ranked-completer-node.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/ranked-completer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/ranked-guide-builder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/ranked-guide-link.h
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/ranked-guide-unit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/lib/dawgdic/ranked-guide.h
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 19:51:40.936749 DAWG2-0.9.0rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1651 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:51:40.936749 DAWG2-0.9.0rc1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)   107013 2023-05-23 19:51:40.000000 DAWG2-0.9.0rc1/src/_base_types.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/src/_base_types.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)   107825 2023-05-23 19:51:40.000000 DAWG2-0.9.0rc1/src/_completer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/src/_completer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)   106952 2023-05-23 19:51:40.000000 DAWG2-0.9.0rc1/src/_dawg.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/src/_dawg.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)   107205 2023-05-23 19:51:40.000000 DAWG2-0.9.0rc1/src/_dawg_builder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/src/_dawg_builder.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)   107578 2023-05-23 19:51:40.000000 DAWG2-0.9.0rc1/src/_dictionary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/src/_dictionary.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)   107878 2023-05-23 19:51:40.000000 DAWG2-0.9.0rc1/src/_dictionary_builder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/src/_dictionary_builder.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)   107259 2023-05-23 19:51:40.000000 DAWG2-0.9.0rc1/src/_dictionary_unit.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/src/_dictionary_unit.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)   107428 2023-05-23 19:51:40.000000 DAWG2-0.9.0rc1/src/_guide.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/src/_guide.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)   107908 2023-05-23 19:51:40.000000 DAWG2-0.9.0rc1/src/_guide_builder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/src/_guide_builder.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)   107124 2023-05-23 19:51:40.000000 DAWG2-0.9.0rc1/src/_guide_unit.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/src/_guide_unit.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)   107304 2023-05-23 19:51:40.000000 DAWG2-0.9.0rc1/src/b64_decode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/src/b64_decode.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)  1132821 2023-05-23 19:51:39.000000 DAWG2-0.9.0rc1/src/dawg.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30775 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/src/dawg.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   107141 2023-05-23 19:51:40.000000 DAWG2-0.9.0rc1/src/iostream.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/src/iostream.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:51:40.936749 DAWG2-0.9.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/tests/test_dawg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/tests/test_payload_dawg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/tests/test_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/tox.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-05-23 19:51:27.000000 DAWG2-0.9.0rc1/update_cpp.sh
```

### Comparing `DAWG2-0.9.0/CHANGES.rst` & `DAWG2-0.9.0rc1/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 Changes
 =======
 
 0.9.0 (2023-05-23)
 ------------------
 
-* Python 3.9, 3.10 and 3.11 support is added
+* Python 3.10 and 3.11 support is added
 
 0.8.0 (2020-02-19)
 ------------------
 
 * Python 3.8 support is added
 * Python 3.2, 3.3 and 3.4 support is dropped
 * Extension is rebuilt with Cython 0.29.15
```

### Comparing `DAWG2-0.9.0/DAWG2.egg-info/PKG-INFO` & `DAWG2-0.9.0rc1/DAWG2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DAWG2
-Version: 0.9.0
+Version: 0.9.0rc1
 Summary: Fast and memory efficient DAWG (DAFSA) for Python
 Home-page: https://github.com/pymorphy2-fork/DAWG/
 Author: Mikhail Korobov
 Author-email: kmike84@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -66,15 +66,15 @@
 
 Changes
 =======
 
 0.9.0 (2023-05-23)
 ------------------
 
-* Python 3.9, 3.10 and 3.11 support is added
+* Python 3.10 and 3.11 support is added
 
 0.8.0 (2020-02-19)
 ------------------
 
 * Python 3.8 support is added
 * Python 3.2, 3.3 and 3.4 support is dropped
 * Extension is rebuilt with Cython 0.29.15
```

### Comparing `DAWG2-0.9.0/DAWG2.egg-info/SOURCES.txt` & `DAWG2-0.9.0rc1/DAWG2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/LICENSE` & `DAWG2-0.9.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/PKG-INFO` & `DAWG2-0.9.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DAWG2
-Version: 0.9.0
+Version: 0.9.0rc1
 Summary: Fast and memory efficient DAWG (DAFSA) for Python
 Home-page: https://github.com/pymorphy2-fork/DAWG/
 Author: Mikhail Korobov
 Author-email: kmike84@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -66,15 +66,15 @@
 
 Changes
 =======
 
 0.9.0 (2023-05-23)
 ------------------
 
-* Python 3.9, 3.10 and 3.11 support is added
+* Python 3.10 and 3.11 support is added
 
 0.8.0 (2020-02-19)
 ------------------
 
 * Python 3.8 support is added
 * Python 3.2, 3.3 and 3.4 support is dropped
 * Extension is rebuilt with Cython 0.29.15
```

### Comparing `DAWG2-0.9.0/README.rst` & `DAWG2-0.9.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/docs/Makefile` & `DAWG2-0.9.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/docs/conf.py` & `DAWG2-0.9.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/docs/index.rst` & `DAWG2-0.9.0rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/docs/make.bat` & `DAWG2-0.9.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/COPYING` & `DAWG2-0.9.0rc1/lib/COPYING`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/b64/cdecode.c` & `DAWG2-0.9.0rc1/lib/b64/cdecode.c`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/b64/cdecode.h` & `DAWG2-0.9.0rc1/lib/b64/cdecode.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/b64/cencode.c` & `DAWG2-0.9.0rc1/lib/b64/cencode.c`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/b64/cencode.h` & `DAWG2-0.9.0rc1/lib/b64/cencode.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/b64/decode.h` & `DAWG2-0.9.0rc1/lib/b64/decode.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/b64/encode.h` & `DAWG2-0.9.0rc1/lib/b64/encode.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/base-unit.h` & `DAWG2-0.9.0rc1/lib/dawgdic/base-unit.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/bit-pool.h` & `DAWG2-0.9.0rc1/lib/dawgdic/bit-pool.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/completer.h` & `DAWG2-0.9.0rc1/lib/dawgdic/completer.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/dawg-builder.h` & `DAWG2-0.9.0rc1/lib/dawgdic/dawg-builder.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/dawg-unit.h` & `DAWG2-0.9.0rc1/lib/dawgdic/dawg-unit.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/dawg.h` & `DAWG2-0.9.0rc1/lib/dawgdic/dawg.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/dictionary-builder.h` & `DAWG2-0.9.0rc1/lib/dawgdic/dictionary-builder.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/dictionary-extra-unit.h` & `DAWG2-0.9.0rc1/lib/dawgdic/dictionary-extra-unit.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/dictionary-unit.h` & `DAWG2-0.9.0rc1/lib/dawgdic/dictionary-unit.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/dictionary.h` & `DAWG2-0.9.0rc1/lib/dawgdic/dictionary.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/guide-builder.h` & `DAWG2-0.9.0rc1/lib/dawgdic/guide-builder.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/guide-unit.h` & `DAWG2-0.9.0rc1/lib/dawgdic/guide-unit.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/guide.h` & `DAWG2-0.9.0rc1/lib/dawgdic/guide.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/link-table.h` & `DAWG2-0.9.0rc1/lib/dawgdic/link-table.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/object-pool.h` & `DAWG2-0.9.0rc1/lib/dawgdic/object-pool.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/ranked-completer-candidate.h` & `DAWG2-0.9.0rc1/lib/dawgdic/ranked-completer-candidate.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/ranked-completer-node.h` & `DAWG2-0.9.0rc1/lib/dawgdic/ranked-completer-node.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/ranked-completer.h` & `DAWG2-0.9.0rc1/lib/dawgdic/ranked-completer.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/ranked-guide-builder.h` & `DAWG2-0.9.0rc1/lib/dawgdic/ranked-guide-builder.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/ranked-guide-link.h` & `DAWG2-0.9.0rc1/lib/dawgdic/ranked-guide-link.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/ranked-guide-unit.h` & `DAWG2-0.9.0rc1/lib/dawgdic/ranked-guide-unit.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/lib/dawgdic/ranked-guide.h` & `DAWG2-0.9.0rc1/lib/dawgdic/ranked-guide.h`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/setup.py` & `DAWG2-0.9.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python
 import glob
 from setuptools import setup, Extension
 
 setup(
     name="DAWG2",
-    version="0.9.0",
+    version="0.9.0rc1",
     description="Fast and memory efficient DAWG (DAFSA) for Python",
     long_description=open('README.rst').read() + '\n\n' + open('CHANGES.rst').read(),
     author='Mikhail Korobov',
     author_email='kmike84@gmail.com',
     url='https://github.com/pymorphy2-fork/DAWG/',
 
     ext_modules=[
```

### Comparing `DAWG2-0.9.0/src/_base_types.cpp` & `DAWG2-0.9.0rc1/src/_base_types.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,20 +74,16 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1978,15 +1974,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -2174,15 +2170,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `DAWG2-0.9.0/src/_completer.cpp` & `DAWG2-0.9.0rc1/src/_completer.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,20 +74,16 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -2013,15 +2009,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -2209,15 +2205,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `DAWG2-0.9.0/src/_completer.pxd` & `DAWG2-0.9.0rc1/src/_completer.pxd`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/src/_dawg.cpp` & `DAWG2-0.9.0rc1/src/_dawg.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,20 +74,16 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1981,15 +1977,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -2177,15 +2173,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `DAWG2-0.9.0/src/_dawg.pxd` & `DAWG2-0.9.0rc1/src/_dawg.pxd`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/src/_dawg_builder.cpp` & `DAWG2-0.9.0rc1/src/_dawg_builder.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,20 +74,16 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1984,15 +1980,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -2180,15 +2176,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `DAWG2-0.9.0/src/_dawg_builder.pxd` & `DAWG2-0.9.0rc1/src/_dawg_builder.pxd`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/src/_dictionary.cpp` & `DAWG2-0.9.0rc1/src/_dictionary.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,20 +74,16 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -2001,15 +1997,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -2197,15 +2193,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `DAWG2-0.9.0/src/_dictionary.pxd` & `DAWG2-0.9.0rc1/src/_dictionary.pxd`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/src/_dictionary_builder.cpp` & `DAWG2-0.9.0rc1/src/_dictionary_builder.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,20 +74,16 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -2007,15 +2003,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -2203,15 +2199,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `DAWG2-0.9.0/src/_dictionary_unit.cpp` & `DAWG2-0.9.0rc1/src/_dictionary_unit.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,20 +74,16 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1981,15 +1977,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -2177,15 +2173,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `DAWG2-0.9.0/src/_dictionary_unit.pxd` & `DAWG2-0.9.0rc1/src/_dictionary_unit.pxd`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/src/_guide.cpp` & `DAWG2-0.9.0rc1/src/_guide.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,20 +74,16 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -2001,15 +1997,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -2197,15 +2193,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `DAWG2-0.9.0/src/_guide.pxd` & `DAWG2-0.9.0rc1/src/_guide.pxd`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/src/_guide_builder.cpp` & `DAWG2-0.9.0rc1/src/_guide_builder.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,20 +74,16 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -2013,15 +2009,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -2209,15 +2205,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `DAWG2-0.9.0/src/_guide_unit.cpp` & `DAWG2-0.9.0rc1/src/_guide_unit.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,20 +74,16 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1981,15 +1977,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -2177,15 +2173,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `DAWG2-0.9.0/src/b64_decode.cpp` & `DAWG2-0.9.0rc1/src/b64_decode.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,20 +74,16 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1995,15 +1991,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -2191,15 +2187,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `DAWG2-0.9.0/src/dawg.cpp` & `DAWG2-0.9.0rc1/src/dawg.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,20 +74,16 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -19981,15 +19977,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_4dawg_CompletionDAWG __pyx_vtable_4dawg_CompletionDAWG;
 
 static PyObject *__pyx_tp_new_4dawg_CompletionDAWG(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_4dawg_CompletionDAWG *p;
@@ -20094,15 +20090,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_4dawg_BytesDAWG __pyx_vtable_4dawg_BytesDAWG;
 
 static PyObject *__pyx_tp_new_4dawg_BytesDAWG(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_4dawg_BytesDAWG *p;
@@ -20243,15 +20239,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_4dawg_RecordDAWG __pyx_vtable_4dawg_RecordDAWG;
 
 static PyObject *__pyx_tp_new_4dawg_RecordDAWG(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_4dawg_RecordDAWG *p;
@@ -20268,15 +20264,18 @@
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->_struct);
-  if (PyType_IS_GC(__pyx_ptype_4dawg_BytesDAWG)) PyObject_GC_Track(o);
+  #if CYTHON_USE_TYPE_SLOTS
+  if (PyType_IS_GC(Py_TYPE(o)->tp_base))
+  #endif
+  PyObject_GC_Track(o);
   __pyx_tp_dealloc_4dawg_BytesDAWG(o);
 }
 
 static int __pyx_tp_traverse_4dawg_RecordDAWG(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_4dawg_RecordDAWG *p = (struct __pyx_obj_4dawg_RecordDAWG *)o;
   e = ((likely(__pyx_ptype_4dawg_BytesDAWG)) ? ((__pyx_ptype_4dawg_BytesDAWG->tp_traverse) ? __pyx_ptype_4dawg_BytesDAWG->tp_traverse(o, v, a) : 0) : __Pyx_call_next_tp_traverse(o, v, a, __pyx_tp_traverse_4dawg_RecordDAWG)); if (e) return e;
@@ -20365,15 +20364,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_4dawg_IntDAWG __pyx_vtable_4dawg_IntDAWG;
 
 static PyObject *__pyx_tp_new_4dawg_IntDAWG(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_4dawg_IntDAWG *p;
@@ -20484,15 +20483,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_4dawg_IntCompletionDAWG __pyx_vtable_4dawg_IntCompletionDAWG;
 
 static PyObject *__pyx_tp_new_4dawg_IntCompletionDAWG(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_4dawg_IntCompletionDAWG *p;
@@ -20605,15 +20604,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_4dawg___pyx_scope_struct__iterprefixes *__pyx_freelist_4dawg___pyx_scope_struct__iterprefixes[8];
 static int __pyx_freecount_4dawg___pyx_scope_struct__iterprefixes = 0;
 
@@ -20717,15 +20716,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_4dawg___pyx_scope_struct_1_compile_replaces *__pyx_freelist_4dawg___pyx_scope_struct_1_compile_replaces[8];
 static int __pyx_freecount_4dawg___pyx_scope_struct_1_compile_replaces = 0;
 
@@ -20835,15 +20834,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_4dawg___pyx_scope_struct_2_genexpr *__pyx_freelist_4dawg___pyx_scope_struct_2_genexpr[8];
 static int __pyx_freecount_4dawg___pyx_scope_struct_2_genexpr = 0;
 
@@ -20952,15 +20951,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_4dawg___pyx_scope_struct_3_iterkeys *__pyx_freelist_4dawg___pyx_scope_struct_3_iterkeys[8];
 static int __pyx_freecount_4dawg___pyx_scope_struct_3_iterkeys = 0;
 
@@ -21071,15 +21070,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_4dawg___pyx_scope_struct_4___init__ *__pyx_freelist_4dawg___pyx_scope_struct_4___init__[8];
 static int __pyx_freecount_4dawg___pyx_scope_struct_4___init__ = 0;
 
@@ -21196,15 +21195,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_4dawg___pyx_scope_struct_5_genexpr *__pyx_freelist_4dawg___pyx_scope_struct_5_genexpr[8];
 static int __pyx_freecount_4dawg___pyx_scope_struct_5_genexpr = 0;
 
@@ -21313,15 +21312,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_4dawg___pyx_scope_struct_6_iteritems *__pyx_freelist_4dawg___pyx_scope_struct_6_iteritems[8];
 static int __pyx_freecount_4dawg___pyx_scope_struct_6_iteritems = 0;
 
@@ -21435,15 +21434,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_4dawg___pyx_scope_struct_7_iterkeys *__pyx_freelist_4dawg___pyx_scope_struct_7_iterkeys[8];
 static int __pyx_freecount_4dawg___pyx_scope_struct_7_iterkeys = 0;
 
@@ -21554,15 +21553,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_4dawg___pyx_scope_struct_8___init__ *__pyx_freelist_4dawg___pyx_scope_struct_8___init__[8];
 static int __pyx_freecount_4dawg___pyx_scope_struct_8___init__ = 0;
 
@@ -21679,15 +21678,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_4dawg___pyx_scope_struct_9_genexpr *__pyx_freelist_4dawg___pyx_scope_struct_9_genexpr[8];
 static int __pyx_freecount_4dawg___pyx_scope_struct_9_genexpr = 0;
 
@@ -21796,15 +21795,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_4dawg___pyx_scope_struct_10_iteritems *__pyx_freelist_4dawg___pyx_scope_struct_10_iteritems[8];
 static int __pyx_freecount_4dawg___pyx_scope_struct_10_iteritems = 0;
 
@@ -21918,15 +21917,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_4dawg___pyx_scope_struct_11__iterable_from_argument *__pyx_freelist_4dawg___pyx_scope_struct_11__iterable_from_argument[8];
 static int __pyx_freecount_4dawg___pyx_scope_struct_11__iterable_from_argument = 0;
 
@@ -22036,15 +22035,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_4dawg___pyx_scope_struct_12_genexpr *__pyx_freelist_4dawg___pyx_scope_struct_12_genexpr[8];
 static int __pyx_freecount_4dawg___pyx_scope_struct_12_genexpr = 0;
 
@@ -22153,15 +22152,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_4dawg___pyx_scope_struct_13_iteritems *__pyx_freelist_4dawg___pyx_scope_struct_13_iteritems[8];
 static int __pyx_freecount_4dawg___pyx_scope_struct_13_iteritems = 0;
 
@@ -22272,15 +22271,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -25643,15 +25642,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -25915,15 +25914,15 @@
                         } else if (8 * sizeof(dawgdic::CharType) >= 4 * PyLong_SHIFT) {
                             return (dawgdic::CharType) (((((((((dawgdic::CharType)digits[3]) << PyLong_SHIFT) | (dawgdic::CharType)digits[2]) << PyLong_SHIFT) | (dawgdic::CharType)digits[1]) << PyLong_SHIFT) | (dawgdic::CharType)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26111,15 +26110,15 @@
                         } else if (8 * sizeof(dawgdic::SizeType) >= 4 * PyLong_SHIFT) {
                             return (dawgdic::SizeType) (((((((((dawgdic::SizeType)digits[3]) << PyLong_SHIFT) | (dawgdic::SizeType)digits[2]) << PyLong_SHIFT) | (dawgdic::SizeType)digits[1]) << PyLong_SHIFT) | (dawgdic::SizeType)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26421,15 +26420,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26617,15 +26616,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -27986,18 +27985,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030C0000
-    0,
-#endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
```

### Comparing `DAWG2-0.9.0/src/dawg.pyx` & `DAWG2-0.9.0rc1/src/dawg.pyx`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/src/iostream.cpp` & `DAWG2-0.9.0rc1/src/iostream.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,20 +74,16 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1992,15 +1988,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -2188,15 +2184,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `DAWG2-0.9.0/src/iostream.pxd` & `DAWG2-0.9.0rc1/src/iostream.pxd`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/tests/test_dawg.py` & `DAWG2-0.9.0rc1/tests/test_dawg.py`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/tests/test_payload_dawg.py` & `DAWG2-0.9.0rc1/tests/test_payload_dawg.py`

 * *Files identical despite different names*

### Comparing `DAWG2-0.9.0/tests/test_prediction.py` & `DAWG2-0.9.0rc1/tests/test_prediction.py`

 * *Files identical despite different names*

