# Comparing `tmp/pymarc-5.0.0.tar.gz` & `tmp/pymarc-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymarc-5.0.0.tar", last modified: Mon May  1 12:17:32 2023, max compression
+gzip compressed data, was "pymarc-5.1.0.tar", last modified: Sat May 27 14:36:03 2023, max compression
```

## Comparing `pymarc-5.0.0.tar` & `pymarc-5.1.0.tar`

### file list

```diff
@@ -1,74 +1,73 @@
-drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-01 12:17:32.842829 pymarc-5.0.0/
--rw-r--r--   0 edsummers   (505) staff       (20)      650 2022-03-02 20:54:44.000000 pymarc-5.0.0/CONTRIBUTING.md
--rw-r--r--   0 edsummers   (505) staff       (20)     3061 2023-04-17 10:38:11.000000 pymarc-5.0.0/LICENSE
--rw-r--r--   0 edsummers   (505) staff       (20)      150 2022-03-02 20:54:44.000000 pymarc-5.0.0/MANIFEST.in
--rw-r--r--   0 edsummers   (505) staff       (20)    12174 2023-05-01 12:17:32.843049 pymarc-5.0.0/PKG-INFO
--rw-r--r--   0 edsummers   (505) staff       (20)    11290 2023-05-01 11:24:10.000000 pymarc-5.0.0/README.md
--rw-r--r--   0 edsummers   (505) staff       (20)    10604 2022-03-02 20:54:44.000000 pymarc-5.0.0/README_pt_Br.md
-drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-01 12:17:32.791262 pymarc-5.0.0/docs/
-drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-01 12:17:32.796232 pymarc-5.0.0/docs/source/
--rw-r--r--   0 edsummers   (505) staff       (20)    10360 2022-03-02 20:54:44.000000 pymarc-5.0.0/docs/source/conf.py
--rw-r--r--   0 edsummers   (505) staff       (20)     8403 2023-05-01 11:24:10.000000 pymarc-5.0.0/docs/source/index.rst
-drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-01 12:17:32.804486 pymarc-5.0.0/pymarc/
--rw-r--r--   0 edsummers   (505) staff       (20)      552 2022-03-02 20:54:44.000000 pymarc-5.0.0/pymarc/__init__.py
--rw-r--r--   0 edsummers   (505) staff       (20)      467 2022-03-02 20:54:44.000000 pymarc-5.0.0/pymarc/constants.py
--rw-r--r--   0 edsummers   (505) staff       (20)     3080 2023-05-01 11:24:10.000000 pymarc-5.0.0/pymarc/exceptions.py
--rw-r--r--   0 edsummers   (505) staff       (20)    13619 2023-05-01 11:24:10.000000 pymarc-5.0.0/pymarc/field.py
--rw-r--r--   0 edsummers   (505) staff       (20)     9989 2023-05-01 11:24:10.000000 pymarc-5.0.0/pymarc/leader.py
--rw-r--r--   0 edsummers   (505) staff       (20)     6617 2023-05-01 11:24:10.000000 pymarc-5.0.0/pymarc/marc8.py
--rw-r--r--   0 edsummers   (505) staff       (20)   835551 2022-03-02 20:54:44.000000 pymarc-5.0.0/pymarc/marc8_mapping.py
--rw-r--r--   0 edsummers   (505) staff       (20)     2322 2023-05-01 11:24:10.000000 pymarc-5.0.0/pymarc/marcjson.py
--rw-r--r--   0 edsummers   (505) staff       (20)     6443 2023-05-01 11:24:10.000000 pymarc-5.0.0/pymarc/marcxml.py
--rw-r--r--   0 edsummers   (505) staff       (20)     8700 2023-05-01 11:24:10.000000 pymarc-5.0.0/pymarc/reader.py
--rw-r--r--   0 edsummers   (505) staff       (20)    24455 2023-05-01 11:24:10.000000 pymarc-5.0.0/pymarc/record.py
--rw-r--r--   0 edsummers   (505) staff       (20)     6316 2022-03-02 20:54:44.000000 pymarc-5.0.0/pymarc/writer.py
-drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-01 12:17:32.806640 pymarc-5.0.0/pymarc.egg-info/
--rw-r--r--   0 edsummers   (505) staff       (20)    12174 2023-05-01 12:17:32.000000 pymarc-5.0.0/pymarc.egg-info/PKG-INFO
--rw-r--r--   0 edsummers   (505) staff       (20)     1289 2023-05-01 12:17:32.000000 pymarc-5.0.0/pymarc.egg-info/SOURCES.txt
--rw-r--r--   0 edsummers   (505) staff       (20)        1 2023-05-01 12:17:32.000000 pymarc-5.0.0/pymarc.egg-info/dependency_links.txt
--rw-r--r--   0 edsummers   (505) staff       (20)        7 2023-05-01 12:17:32.000000 pymarc-5.0.0/pymarc.egg-info/top_level.txt
--rw-r--r--   0 edsummers   (505) staff       (20)      282 2023-04-25 13:12:39.000000 pymarc-5.0.0/release.md
--rw-r--r--   0 edsummers   (505) staff       (20)       46 2022-03-02 20:54:44.000000 pymarc-5.0.0/requirements.dev.txt
--rw-r--r--   0 edsummers   (505) staff       (20)      177 2023-05-01 12:17:32.843793 pymarc-5.0.0/setup.cfg
--rw-r--r--   0 edsummers   (505) staff       (20)     1392 2023-05-01 11:24:10.000000 pymarc-5.0.0/setup.py
-drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-01 12:17:32.842298 pymarc-5.0.0/test/
--rw-r--r--   0 edsummers   (505) staff       (20)     5344 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/1251.dat
--rw-r--r--   0 edsummers   (505) staff       (20)        0 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/__init__.py
--rw-r--r--   0 edsummers   (505) staff       (20)     1339 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/alphatag.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     1632 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/bad_eacc_encoding.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     1980 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/bad_indicator.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     1491 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/bad_marc8_escape.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     1017 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/bad_records.mrc
--rw-r--r--   0 edsummers   (505) staff       (20)      756 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/bad_subfield_code.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     2063 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/bad_tag.xml
--rw-r--r--   0 edsummers   (505) staff       (20)     9063 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/batch.json
--rw-r--r--   0 edsummers   (505) staff       (20)     8247 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/batch.xml
--rw-r--r--   0 edsummers   (505) staff       (20)     2710 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/diacritic.dat
--rw-r--r--   0 edsummers   (505) staff       (20)    20388 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/marc.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     1117 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/marc8-to-unicode.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     1117 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/marc8.dat
--rw-r--r--   0 edsummers   (505) staff       (20)      794 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/multi_isbn.dat
--rw-r--r--   0 edsummers   (505) staff       (20)      755 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/one.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     3260 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/one.json
--rw-r--r--   0 edsummers   (505) staff       (20)    49461 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/regression45.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     6591 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/test.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     9410 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/test.json
--rw-r--r--   0 edsummers   (505) staff       (20)     1551 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/test_encode.py
--rw-r--r--   0 edsummers   (505) staff       (20)    11822 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/test_field.py
--rw-r--r--   0 edsummers   (505) staff       (20)     5666 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/test_json.py
--rw-r--r--   0 edsummers   (505) staff       (20)     2869 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/test_leader.py
--rw-r--r--   0 edsummers   (505) staff       (20)     8822 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/test_marc8.py
--rw-r--r--   0 edsummers   (505) staff       (20)    55430 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/test_marc8.txt
--rw-r--r--   0 edsummers   (505) staff       (20)     1923 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/test_ordered_fields.py
--rw-r--r--   0 edsummers   (505) staff       (20)     8939 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/test_reader.py
--rw-r--r--   0 edsummers   (505) staff       (20)    25406 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/test_record.py
--rw-r--r--   0 edsummers   (505) staff       (20)     1652 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/test_utf8.py
--rw-r--r--   0 edsummers   (505) staff       (20)    38127 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/test_utf8.txt
--rw-r--r--   0 edsummers   (505) staff       (20)    23386 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/test_writer.py
--rw-r--r--   0 edsummers   (505) staff       (20)     3907 2022-03-02 22:13:36.000000 pymarc-5.0.0/test/test_xml.py
--rw-r--r--   0 edsummers   (505) staff       (20)     2499 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/testunimarc.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     1438 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/utf8.xml
--rw-r--r--   0 edsummers   (505) staff       (20)     1474 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/utf8_errors.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     1004 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/utf8_invalid.mrc
--rw-r--r--   0 edsummers   (505) staff       (20)     1123 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/utf8_with_leader_flag.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     1123 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/utf8_without_leader_flag.dat
+drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-27 14:36:03.508230 pymarc-5.1.0/
+-rw-r--r--   0 edsummers   (505) staff       (20)      650 2022-03-02 20:54:44.000000 pymarc-5.1.0/CONTRIBUTING.md
+-rw-r--r--   0 edsummers   (505) staff       (20)     3061 2023-04-17 10:38:11.000000 pymarc-5.1.0/LICENSE
+-rw-r--r--   0 edsummers   (505) staff       (20)      150 2022-03-02 20:54:44.000000 pymarc-5.1.0/MANIFEST.in
+-rw-r--r--   0 edsummers   (505) staff       (20)    12201 2023-05-27 14:36:03.508386 pymarc-5.1.0/PKG-INFO
+-rw-r--r--   0 edsummers   (505) staff       (20)    11297 2023-05-27 14:31:28.000000 pymarc-5.1.0/README.md
+-rw-r--r--   0 edsummers   (505) staff       (20)    10604 2022-03-02 20:54:44.000000 pymarc-5.1.0/README_pt_Br.md
+drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-27 14:36:03.484583 pymarc-5.1.0/docs/
+drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-27 14:36:03.488311 pymarc-5.1.0/docs/source/
+-rw-r--r--   0 edsummers   (505) staff       (20)    10360 2022-03-02 20:54:44.000000 pymarc-5.1.0/docs/source/conf.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     8426 2023-05-27 14:31:28.000000 pymarc-5.1.0/docs/source/index.rst
+drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-27 14:36:03.493385 pymarc-5.1.0/pymarc/
+-rw-r--r--   0 edsummers   (505) staff       (20)      552 2022-03-02 20:54:44.000000 pymarc-5.1.0/pymarc/__init__.py
+-rw-r--r--   0 edsummers   (505) staff       (20)      467 2022-03-02 20:54:44.000000 pymarc-5.1.0/pymarc/constants.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     3080 2023-05-01 11:24:10.000000 pymarc-5.1.0/pymarc/exceptions.py
+-rw-r--r--   0 edsummers   (505) staff       (20)    13619 2023-05-01 11:24:10.000000 pymarc-5.1.0/pymarc/field.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     9989 2023-05-01 11:24:10.000000 pymarc-5.1.0/pymarc/leader.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     7050 2023-05-27 14:31:28.000000 pymarc-5.1.0/pymarc/marc8.py
+-rw-r--r--   0 edsummers   (505) staff       (20)   835551 2022-03-02 20:54:44.000000 pymarc-5.1.0/pymarc/marc8_mapping.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     2322 2023-05-01 11:24:10.000000 pymarc-5.1.0/pymarc/marcjson.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     6443 2023-05-01 11:24:10.000000 pymarc-5.1.0/pymarc/marcxml.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     8700 2023-05-01 11:24:10.000000 pymarc-5.1.0/pymarc/reader.py
+-rw-r--r--   0 edsummers   (505) staff       (20)    24455 2023-05-01 11:24:10.000000 pymarc-5.1.0/pymarc/record.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     6316 2022-03-02 20:54:44.000000 pymarc-5.1.0/pymarc/writer.py
+drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-27 14:36:03.494746 pymarc-5.1.0/pymarc.egg-info/
+-rw-r--r--   0 edsummers   (505) staff       (20)    12201 2023-05-27 14:36:03.000000 pymarc-5.1.0/pymarc.egg-info/PKG-INFO
+-rw-r--r--   0 edsummers   (505) staff       (20)     1278 2023-05-27 14:36:03.000000 pymarc-5.1.0/pymarc.egg-info/SOURCES.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)        1 2023-05-27 14:36:03.000000 pymarc-5.1.0/pymarc.egg-info/dependency_links.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)        7 2023-05-27 14:36:03.000000 pymarc-5.1.0/pymarc.egg-info/top_level.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)       46 2022-03-02 20:54:44.000000 pymarc-5.1.0/requirements.dev.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)      177 2023-05-27 14:36:03.508934 pymarc-5.1.0/setup.cfg
+-rw-r--r--   0 edsummers   (505) staff       (20)     1392 2023-05-27 14:33:35.000000 pymarc-5.1.0/setup.py
+drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-27 14:36:03.507952 pymarc-5.1.0/test/
+-rw-r--r--   0 edsummers   (505) staff       (20)     5344 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/1251.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)        0 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/__init__.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     1339 2023-05-01 11:24:10.000000 pymarc-5.1.0/test/alphatag.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1632 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/bad_eacc_encoding.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1980 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/bad_indicator.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1491 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/bad_marc8_escape.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1017 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/bad_records.mrc
+-rw-r--r--   0 edsummers   (505) staff       (20)      756 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/bad_subfield_code.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     2063 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/bad_tag.xml
+-rw-r--r--   0 edsummers   (505) staff       (20)     9063 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/batch.json
+-rw-r--r--   0 edsummers   (505) staff       (20)     8247 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/batch.xml
+-rw-r--r--   0 edsummers   (505) staff       (20)     2710 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/diacritic.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)    20388 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/marc.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1117 2023-05-01 11:24:10.000000 pymarc-5.1.0/test/marc8-to-unicode.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1117 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/marc8.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)      794 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/multi_isbn.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)      755 2023-05-01 11:24:10.000000 pymarc-5.1.0/test/one.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     3260 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/one.json
+-rw-r--r--   0 edsummers   (505) staff       (20)    49461 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/regression45.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     6591 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/test.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     9410 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/test.json
+-rw-r--r--   0 edsummers   (505) staff       (20)     1551 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/test_encode.py
+-rw-r--r--   0 edsummers   (505) staff       (20)    11822 2023-05-01 11:24:10.000000 pymarc-5.1.0/test/test_field.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     5666 2023-05-01 11:24:10.000000 pymarc-5.1.0/test/test_json.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     2869 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/test_leader.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     8684 2023-05-27 14:31:28.000000 pymarc-5.1.0/test/test_marc8.py
+-rw-r--r--   0 edsummers   (505) staff       (20)    55430 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/test_marc8.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)     1923 2023-05-01 11:24:10.000000 pymarc-5.1.0/test/test_ordered_fields.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     8939 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/test_reader.py
+-rw-r--r--   0 edsummers   (505) staff       (20)    25406 2023-05-01 11:24:10.000000 pymarc-5.1.0/test/test_record.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     1652 2023-05-01 11:24:10.000000 pymarc-5.1.0/test/test_utf8.py
+-rw-r--r--   0 edsummers   (505) staff       (20)    38127 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/test_utf8.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)    23386 2023-05-01 11:24:10.000000 pymarc-5.1.0/test/test_writer.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     3907 2022-03-02 22:13:36.000000 pymarc-5.1.0/test/test_xml.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     2499 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/testunimarc.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1438 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/utf8.xml
+-rw-r--r--   0 edsummers   (505) staff       (20)     1474 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/utf8_errors.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1004 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/utf8_invalid.mrc
+-rw-r--r--   0 edsummers   (505) staff       (20)     1123 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/utf8_with_leader_flag.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1123 2022-03-02 20:54:44.000000 pymarc-5.1.0/test/utf8_without_leader_flag.dat
```

### Comparing `pymarc-5.0.0/CONTRIBUTING.md` & `pymarc-5.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/LICENSE` & `pymarc-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/PKG-INFO` & `pymarc-5.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pymarc
-Version: 5.0.0
+Version: 5.1.0
 Summary: Read, write and modify MARC bibliographic data
 Home-page: http://gitlab.com/pymarc/pymarc
 Author: Ed Summers
 Author-email: ehs@pobox.com
 License: http://www.opensource.org/licenses/bsd-license.php
+Platform: UNKNOWN
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -126,28 +127,29 @@
 ```python
 for f in record.get_fields('650'):
     print(f)
 ```
 
 If you are new to MARC fields [Understanding
 MARC](http://www.loc.gov/marc/umb/) is a pretty good primer, and the [MARC 21
-Formats](http://www.loc.gov/marc/marcdocz.html) page at the Library of Congress is a good reference once you understand the basics.
+Formats](http://www.loc.gov/marc/marcdocz.html) page at the Library of Congress 
+is a good reference once you understand the basics.
 
 ### Writing
 
 *Note: As of v5.0.0 `Subfield` is used to create subfields. Prior to v5,
 subfields were constructed and accessed as a list of strings, e.g., `[code,
 value, code, value]`. In v5.0.0 this has been changed to organize the subfields
 into a list of tuples, e.g., `[(code, value), (code, value)]`. The `Subfield`
 is implemented as a `NamedTuple` so that the tuples can be constructed as
 `Subfield(code=code, value=value)`. The old style of creating subfields is no
 longer supported. Attempting to pass a list of strings to the `subfields`
 parameter for the `Field` constructor will raise a `ValueError`. For
-convenience the `Field.convert_legacy_subfields` can be used to convert a
-legacy list of strings into a list of `Subfield`s.*
+convenience the `Field.convert_legacy_subfields` class method can be used to 
+convert a legacy list of strings into a list of `Subfield`s.*
 
 Here's an example of creating a record and writing it out to a file.
 
 ```python
 from pymarc import Record, Field, Subfield
 
 record = Record()
@@ -217,15 +219,15 @@
 can:
 
 ```python
 
 from pymarc import map_xml
 
 def print_title(r):
-    print(r.title())
+    print(r.title)
 
 map_xml(print_title, 'test/batch.xml')
 ```
 
 Also, if you prefer you can pass in a file like object in addition to the path
 to both *map_xml* and *parse_xml_to_array*:
 
@@ -245,15 +247,15 @@
 
 with open('test/one.dat','rb') as fh:
     reader = MARCReader(fh)
     for record in reader:
         print(record.as_json(indent=2))
 ```
 
-```javascript
+```json
 {
   "leader": "01060cam  22002894a 4500",
   "fields": [
     {
       "001": "11778504"
     },
     {
@@ -410,7 +412,9 @@
 GitLab to submit feature requests or bug reports. If you've got an itch to
 scratch, please scratch it, and send merge requests on
 [GitLab](http://gitlab.com/pymarc/pymarc).
 
 If you start working with MARC you may feel like you need moral support
 in addition to technical support. The
 [#code4lib](ircs://irc.libera.chat/code4lib) channel on [Libera](https://libera.chat/) is a good place for both.
+
+
```

### Comparing `pymarc-5.0.0/README.md` & `pymarc-5.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -263,444 +263,445 @@
 00001060: 2070 7265 7474 7920 676f 6f64 2070 7269   pretty good pri
 00001070: 6d65 722c 2061 6e64 2074 6865 205b 4d41  mer, and the [MA
 00001080: 5243 2032 310a 466f 726d 6174 735d 2868  RC 21.Formats](h
 00001090: 7474 703a 2f2f 7777 772e 6c6f 632e 676f  ttp://www.loc.go
 000010a0: 762f 6d61 7263 2f6d 6172 6364 6f63 7a2e  v/marc/marcdocz.
 000010b0: 6874 6d6c 2920 7061 6765 2061 7420 7468  html) page at th
 000010c0: 6520 4c69 6272 6172 7920 6f66 2043 6f6e  e Library of Con
-000010d0: 6772 6573 7320 6973 2061 2067 6f6f 6420  gress is a good 
-000010e0: 7265 6665 7265 6e63 6520 6f6e 6365 2079  reference once y
-000010f0: 6f75 2075 6e64 6572 7374 616e 6420 7468  ou understand th
-00001100: 6520 6261 7369 6373 2e0a 0a23 2323 2057  e basics...### W
-00001110: 7269 7469 6e67 0a0a 2a4e 6f74 653a 2041  riting..*Note: A
-00001120: 7320 6f66 2076 352e 302e 3020 6053 7562  s of v5.0.0 `Sub
-00001130: 6669 656c 6460 2069 7320 7573 6564 2074  field` is used t
-00001140: 6f20 6372 6561 7465 2073 7562 6669 656c  o create subfiel
-00001150: 6473 2e20 5072 696f 7220 746f 2076 352c  ds. Prior to v5,
-00001160: 0a73 7562 6669 656c 6473 2077 6572 6520  .subfields were 
-00001170: 636f 6e73 7472 7563 7465 6420 616e 6420  constructed and 
-00001180: 6163 6365 7373 6564 2061 7320 6120 6c69  accessed as a li
-00001190: 7374 206f 6620 7374 7269 6e67 732c 2065  st of strings, e
-000011a0: 2e67 2e2c 2060 5b63 6f64 652c 0a76 616c  .g., `[code,.val
-000011b0: 7565 2c20 636f 6465 2c20 7661 6c75 655d  ue, code, value]
-000011c0: 602e 2049 6e20 7635 2e30 2e30 2074 6869  `. In v5.0.0 thi
-000011d0: 7320 6861 7320 6265 656e 2063 6861 6e67  s has been chang
-000011e0: 6564 2074 6f20 6f72 6761 6e69 7a65 2074  ed to organize t
-000011f0: 6865 2073 7562 6669 656c 6473 0a69 6e74  he subfields.int
-00001200: 6f20 6120 6c69 7374 206f 6620 7475 706c  o a list of tupl
-00001210: 6573 2c20 652e 672e 2c20 605b 2863 6f64  es, e.g., `[(cod
-00001220: 652c 2076 616c 7565 292c 2028 636f 6465  e, value), (code
-00001230: 2c20 7661 6c75 6529 5d60 2e20 5468 6520  , value)]`. The 
-00001240: 6053 7562 6669 656c 6460 0a69 7320 696d  `Subfield`.is im
-00001250: 706c 656d 656e 7465 6420 6173 2061 2060  plemented as a `
-00001260: 4e61 6d65 6454 7570 6c65 6020 736f 2074  NamedTuple` so t
-00001270: 6861 7420 7468 6520 7475 706c 6573 2063  hat the tuples c
-00001280: 616e 2062 6520 636f 6e73 7472 7563 7465  an be constructe
-00001290: 6420 6173 0a60 5375 6266 6965 6c64 2863  d as.`Subfield(c
-000012a0: 6f64 653d 636f 6465 2c20 7661 6c75 653d  ode=code, value=
-000012b0: 7661 6c75 6529 602e 2054 6865 206f 6c64  value)`. The old
-000012c0: 2073 7479 6c65 206f 6620 6372 6561 7469   style of creati
-000012d0: 6e67 2073 7562 6669 656c 6473 2069 7320  ng subfields is 
-000012e0: 6e6f 0a6c 6f6e 6765 7220 7375 7070 6f72  no.longer suppor
-000012f0: 7465 642e 2041 7474 656d 7074 696e 6720  ted. Attempting 
-00001300: 746f 2070 6173 7320 6120 6c69 7374 206f  to pass a list o
-00001310: 6620 7374 7269 6e67 7320 746f 2074 6865  f strings to the
-00001320: 2060 7375 6266 6965 6c64 7360 0a70 6172   `subfields`.par
-00001330: 616d 6574 6572 2066 6f72 2074 6865 2060  ameter for the `
-00001340: 4669 656c 6460 2063 6f6e 7374 7275 6374  Field` construct
-00001350: 6f72 2077 696c 6c20 7261 6973 6520 6120  or will raise a 
-00001360: 6056 616c 7565 4572 726f 7260 2e20 466f  `ValueError`. Fo
-00001370: 720a 636f 6e76 656e 6965 6e63 6520 7468  r.convenience th
-00001380: 6520 6046 6965 6c64 2e63 6f6e 7665 7274  e `Field.convert
-00001390: 5f6c 6567 6163 795f 7375 6266 6965 6c64  _legacy_subfield
-000013a0: 7360 2063 616e 2062 6520 7573 6564 2074  s` can be used t
-000013b0: 6f20 636f 6e76 6572 7420 610a 6c65 6761  o convert a.lega
-000013c0: 6379 206c 6973 7420 6f66 2073 7472 696e  cy list of strin
-000013d0: 6773 2069 6e74 6f20 6120 6c69 7374 206f  gs into a list o
-000013e0: 6620 6053 7562 6669 656c 6460 732e 2a0a  f `Subfield`s.*.
-000013f0: 0a48 6572 6527 7320 616e 2065 7861 6d70  .Here's an examp
-00001400: 6c65 206f 6620 6372 6561 7469 6e67 2061  le of creating a
-00001410: 2072 6563 6f72 6420 616e 6420 7772 6974   record and writ
-00001420: 696e 6720 6974 206f 7574 2074 6f20 6120  ing it out to a 
-00001430: 6669 6c65 2e0a 0a60 6060 7079 7468 6f6e  file...```python
-00001440: 0a66 726f 6d20 7079 6d61 7263 2069 6d70  .from pymarc imp
-00001450: 6f72 7420 5265 636f 7264 2c20 4669 656c  ort Record, Fiel
-00001460: 642c 2053 7562 6669 656c 640a 0a72 6563  d, Subfield..rec
-00001470: 6f72 6420 3d20 5265 636f 7264 2829 0a72  ord = Record().r
-00001480: 6563 6f72 642e 6164 645f 6669 656c 6428  ecord.add_field(
-00001490: 0a20 2020 2046 6965 6c64 280a 2020 2020  .    Field(.    
-000014a0: 2020 2020 7461 673d 2732 3435 272c 0a20      tag='245',. 
-000014b0: 2020 2020 2020 2069 6e64 6963 6174 6f72         indicator
-000014c0: 733d 5b27 3027 2c20 2731 275d 2c0a 2020  s=['0', '1'],.  
-000014d0: 2020 2020 2020 7375 6266 6965 6c64 733d        subfields=
-000014e0: 5b0a 2020 2020 2020 2020 2020 2020 5375  [.            Su
-000014f0: 6266 6965 6c64 2863 6f64 653d 2761 272c  bfield(code='a',
-00001500: 2076 616c 7565 3d27 5468 6520 7072 6167   value='The prag
-00001510: 6d61 7469 6320 7072 6f67 7261 6d6d 6572  matic programmer
-00001520: 203a 2027 292c 0a20 2020 2020 2020 2020   : '),.         
-00001530: 2020 2053 7562 6669 656c 6428 636f 6465     Subfield(code
-00001540: 3d27 6227 2c20 7661 6c75 653d 2766 726f  ='b', value='fro
-00001550: 6d20 6a6f 7572 6e65 796d 616e 2074 6f20  m journeyman to 
-00001560: 6d61 7374 6572 202f 2729 2c0a 2020 2020  master /'),.    
-00001570: 2020 2020 2020 2020 5375 6266 6965 6c64          Subfield
-00001580: 2863 6f64 653d 2763 272c 2076 616c 7565  (code='c', value
-00001590: 3d27 416e 6472 6577 2048 756e 742c 2044  ='Andrew Hunt, D
-000015a0: 6176 6964 2054 686f 6d61 732e 2729 0a20  avid Thomas.'). 
-000015b0: 2020 2020 2020 205d 2929 0a77 6974 6820         ])).with 
-000015c0: 6f70 656e 2827 6669 6c65 2e64 6174 272c  open('file.dat',
-000015d0: 2027 7762 2729 2061 7320 6f75 743a 0a20   'wb') as out:. 
-000015e0: 2020 206f 7574 2e77 7269 7465 2872 6563     out.write(rec
-000015f0: 6f72 642e 6173 5f6d 6172 6328 2929 0a60  ord.as_marc()).`
-00001600: 6060 0a0a 546f 2063 6f6e 7665 7274 2066  ``..To convert f
-00001610: 726f 6d20 7468 6520 6f6c 6420 7374 7269  rom the old stri
-00001620: 6e67 206c 6973 7420 746f 2061 206c 6973  ng list to a lis
-00001630: 7420 6f66 2060 5375 6266 6965 6c64 6073  t of `Subfield`s
-00001640: 2c20 7468 6520 602e 636f 6e76 6572 745f  , the `.convert_
-00001650: 6c65 6761 6379 5f73 7562 6669 656c 6473  legacy_subfields
-00001660: 6020 636c 6173 7320 6d65 7468 6f64 0a69  ` class method.i
-00001670: 7320 7072 6f76 6964 6564 206f 6e20 7468  s provided on th
-00001680: 6520 6046 6965 6c64 6020 636c 6173 732e  e `Field` class.
-00001690: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-000016a0: 2070 796d 6172 6320 696d 706f 7274 2046   pymarc import F
-000016b0: 6965 6c64 2c20 5375 6266 6965 6c64 0a0a  ield, Subfield..
-000016c0: 6c65 6761 6379 5f66 6965 6c64 733a 206c  legacy_fields: l
-000016d0: 6973 745b 7374 725d 203d 205b 2761 272c  ist[str] = ['a',
-000016e0: 2027 5468 6520 7072 6167 6d61 7469 6320   'The pragmatic 
-000016f0: 7072 6f67 7261 6d6d 6572 203a 2027 2c0a  programmer : ',.
-00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001710: 2020 2020 2020 2020 2020 2020 2762 272c              'b',
-00001720: 2027 6672 6f6d 206a 6f75 726e 6579 6d61   'from journeyma
-00001730: 6e20 746f 206d 6173 7465 7220 2f27 2c0a  n to master /',.
-00001740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001750: 2020 2020 2020 2020 2020 2020 2763 272c              'c',
-00001760: 2027 416e 6472 6577 2048 756e 742c 2044   'Andrew Hunt, D
-00001770: 6176 6964 2054 686f 6d61 7327 5d0a 0a63  avid Thomas']..c
-00001780: 6f64 6564 5f66 6965 6c64 733a 206c 6973  oded_fields: lis
-00001790: 745b 5375 6266 6965 6c64 5d20 3d20 4669  t[Subfield] = Fi
-000017a0: 656c 642e 636f 6e76 6572 745f 6c65 6761  eld.convert_lega
-000017b0: 6379 5f73 7562 6669 656c 6473 286c 6567  cy_subfields(leg
-000017c0: 6163 795f 6669 656c 6473 290a 6060 600a  acy_fields).```.
-000017d0: 0a23 2323 2055 7064 6174 696e 670a 0a55  .### Updating..U
-000017e0: 7064 6174 696e 6720 776f 726b 7320 7468  pdating works th
-000017f0: 6520 7361 6d65 2077 6179 2c20 796f 7520  e same way, you 
-00001800: 7265 6164 2069 7420 696e 2c20 6d6f 6469  read it in, modi
-00001810: 6679 2069 742c 2061 6e64 2074 6865 6e20  fy it, and then 
-00001820: 7772 6974 6520 6974 206f 7574 0a61 6761  write it out.aga
-00001830: 696e 3a0a 0a60 6060 7079 7468 6f6e 0a66  in:..```python.f
-00001840: 726f 6d20 7079 6d61 7263 2069 6d70 6f72  rom pymarc impor
-00001850: 7420 4d41 5243 5265 6164 6572 0a77 6974  t MARCReader.wit
-00001860: 6820 6f70 656e 2827 7465 7374 2f6d 6172  h open('test/mar
-00001870: 632e 6461 7427 2c20 2772 6227 2920 6173  c.dat', 'rb') as
-00001880: 2066 683a 0a20 2020 2072 6561 6465 7220   fh:.    reader 
-00001890: 3d20 4d41 5243 5265 6164 6572 2866 6829  = MARCReader(fh)
-000018a0: 0a20 2020 2072 6563 6f72 6420 3d20 6e65  .    record = ne
-000018b0: 7874 2872 6561 6465 7229 0a20 2020 2072  xt(reader).    r
-000018c0: 6563 6f72 645b 2732 3435 275d 5b27 6127  ecord['245']['a'
-000018d0: 5d20 3d20 2754 6865 205a 6f6d 6269 6520  ] = 'The Zombie 
-000018e0: 5072 6f67 7261 6d6d 6572 203a 2027 0a77  Programmer : '.w
-000018f0: 6974 6820 6f70 656e 2827 6669 6c65 2e64  ith open('file.d
-00001900: 6174 272c 2027 7762 2729 2061 7320 6f75  at', 'wb') as ou
-00001910: 743a 0a20 2020 206f 7574 2e77 7269 7465  t:.    out.write
-00001920: 2872 6563 6f72 642e 6173 5f6d 6172 6328  (record.as_marc(
-00001930: 2929 0a60 6060 0a0a 0a23 2323 204a 534f  )).```...### JSO
-00001940: 4e20 616e 6420 584d 4c0a 0a49 6620 796f  N and XML..If yo
-00001950: 7520 6669 6e64 2079 6f75 7273 656c 6620  u find yourself 
-00001960: 7573 696e 6720 4d41 5243 2064 6174 6120  using MARC data 
-00001970: 6120 6661 6972 2062 6974 2c20 616e 6420  a fair bit, and 
-00001980: 6469 7374 7269 6275 7469 6e67 2069 742c  distributing it,
-00001990: 2079 6f75 206d 6179 0a6d 616b 6520 6f74   you may.make ot
-000019a0: 6865 7220 6465 7665 6c6f 7065 7273 2061  her developers a
-000019b0: 2062 6974 2068 6170 7069 6572 2062 7920   bit happier by 
-000019c0: 7573 696e 6720 7468 6520 4a53 4f4e 206f  using the JSON o
-000019d0: 7220 584d 4c20 7365 7269 616c 697a 6174  r XML serializat
-000019e0: 696f 6e73 2e20 5468 650a 6d61 696e 2062  ions. The.main b
-000019f0: 656e 6566 6974 2074 6f20 7573 696e 6720  enefit to using 
-00001a00: 584d 4c20 6f72 204a 534f 4e20 6973 2074  XML or JSON is t
-00001a10: 6861 7420 7468 6520 5554 4638 2063 6861  hat the UTF8 cha
-00001a20: 7261 6374 6572 2065 6e63 6f64 696e 6720  racter encoding 
-00001a30: 6973 2075 7365 642c 0a72 6174 6865 7220  is used,.rather 
-00001a40: 7468 616e 2074 6865 2066 7275 7374 7261  than the frustra
-00001a50: 7469 6e67 6c79 2061 7263 6861 6963 204d  tingly archaic M
-00001a60: 4152 4338 2065 6e63 6f64 696e 672e 2041  ARC8 encoding. A
-00001a70: 6c73 6f20 7468 6579 2077 696c 6c20 6265  lso they will be
-00001a80: 2061 626c 6520 746f 0a75 7365 2073 7461   able to.use sta
-00001a90: 6e64 6172 6420 4a53 4f4e 2061 6e64 2058  ndard JSON and X
-00001aa0: 4d4c 2072 6561 6469 6e67 2f77 7269 7469  ML reading/writi
-00001ab0: 6e67 2074 6f6f 6c73 2074 6f20 6765 7420  ng tools to get 
-00001ac0: 6174 2074 6865 2064 6174 6120 7468 6579  at the data they
-00001ad0: 2077 616e 740a 696e 7374 6561 6420 6f66   want.instead of
-00001ae0: 2073 6f6d 6520 6372 617a 7920 4d41 5243   some crazy MARC
-00001af0: 2070 726f 6365 7373 696e 6720 6c69 6272   processing libr
-00001b00: 6172 7920 6c69 6b65 2c20 6168 656d 2c20  ary like, ahem, 
-00001b10: 7079 6d61 7263 2e0a 0a2a 2a58 4d4c 2a2a  pymarc...**XML**
-00001b20: 0a0a 546f 2070 6172 7365 2061 2066 696c  ..To parse a fil
-00001b30: 6520 6f66 204d 4152 4358 4d4c 2072 6563  e of MARCXML rec
-00001b40: 6f72 6473 2079 6f75 2063 616e 3a0a 0a60  ords you can:..`
-00001b50: 6060 7079 7468 6f6e 0a0a 6672 6f6d 2070  ``python..from p
-00001b60: 796d 6172 6320 696d 706f 7274 2070 6172  ymarc import par
-00001b70: 7365 5f78 6d6c 5f74 6f5f 6172 7261 790a  se_xml_to_array.
-00001b80: 0a72 6563 6f72 6473 203d 2070 6172 7365  .records = parse
-00001b90: 5f78 6d6c 5f74 6f5f 6172 7261 7928 2774  _xml_to_array('t
-00001ba0: 6573 742f 6261 7463 682e 786d 6c27 290a  est/batch.xml').
-00001bb0: 6060 600a 0a49 6620 796f 7520 6861 7665  ```..If you have
-00001bc0: 2061 206c 6172 6765 2058 4d4c 2066 696c   a large XML fil
-00001bd0: 6520 616e 6420 776f 756c 6420 7261 7468  e and would rath
-00001be0: 6572 206e 6f74 2072 6561 6420 7468 656d  er not read them
-00001bf0: 2061 6c6c 2069 6e74 6f20 6d65 6d6f 7279   all into memory
-00001c00: 2079 6f75 0a63 616e 3a0a 0a60 6060 7079   you.can:..```py
-00001c10: 7468 6f6e 0a0a 6672 6f6d 2070 796d 6172  thon..from pymar
-00001c20: 6320 696d 706f 7274 206d 6170 5f78 6d6c  c import map_xml
-00001c30: 0a0a 6465 6620 7072 696e 745f 7469 746c  ..def print_titl
-00001c40: 6528 7229 3a0a 2020 2020 7072 696e 7428  e(r):.    print(
-00001c50: 722e 7469 746c 6528 2929 0a0a 6d61 705f  r.title())..map_
-00001c60: 786d 6c28 7072 696e 745f 7469 746c 652c  xml(print_title,
-00001c70: 2027 7465 7374 2f62 6174 6368 2e78 6d6c   'test/batch.xml
-00001c80: 2729 0a60 6060 0a0a 416c 736f 2c20 6966  ').```..Also, if
-00001c90: 2079 6f75 2070 7265 6665 7220 796f 7520   you prefer you 
-00001ca0: 6361 6e20 7061 7373 2069 6e20 6120 6669  can pass in a fi
-00001cb0: 6c65 206c 696b 6520 6f62 6a65 6374 2069  le like object i
-00001cc0: 6e20 6164 6469 7469 6f6e 2074 6f20 7468  n addition to th
-00001cd0: 6520 7061 7468 0a74 6f20 626f 7468 202a  e path.to both *
-00001ce0: 6d61 705f 786d 6c2a 2061 6e64 202a 7061  map_xml* and *pa
-00001cf0: 7273 655f 786d 6c5f 746f 5f61 7272 6179  rse_xml_to_array
-00001d00: 2a3a 0a0a 6060 6070 7974 686f 6e0a 6672  *:..```python.fr
-00001d10: 6f6d 2070 796d 6172 6320 696d 706f 7274  om pymarc import
-00001d20: 2070 6172 7365 5f78 6d6c 5f74 6f5f 6172   parse_xml_to_ar
-00001d30: 7261 790a 0a72 6563 6f72 6473 203d 2070  ray..records = p
-00001d40: 6172 7365 5f78 6d6c 5f74 6f5f 6172 7261  arse_xml_to_arra
-00001d50: 7928 6f70 656e 2827 7465 7374 2f62 6174  y(open('test/bat
-00001d60: 6368 2e78 6d6c 2729 290a 6060 600a 0a2a  ch.xml')).```..*
-00001d70: 2a4a 534f 4e2a 2a0a 0a4a 534f 4e20 7375  *JSON**..JSON su
-00001d80: 7070 6f72 7420 6973 2066 6169 726c 7920  pport is fairly 
-00001d90: 6d69 6e69 6d61 6c20 696e 2074 6861 7420  minimal in that 
-00001da0: 796f 7520 6361 6e20 6361 6c6c 2061 2060  you can call a `
-00001db0: 7079 6d61 7263 2e52 6563 6f72 6460 2773  pymarc.Record`'s
-00001dc0: 0a60 6173 5f6a 736f 6e28 2960 206d 6574  .`as_json()` met
-00001dd0: 686f 6420 746f 2072 6574 7572 6e20 4a53  hod to return JS
-00001de0: 4f4e 2066 6f72 2061 2067 6976 656e 204d  ON for a given M
-00001df0: 4152 4320 5265 636f 7264 3a0a 0a60 6060  ARC Record:..```
-00001e00: 7079 7468 6f6e 0a66 726f 6d20 7079 6d61  python.from pyma
-00001e10: 7263 2069 6d70 6f72 7420 4d41 5243 5265  rc import MARCRe
-00001e20: 6164 6572 0a0a 7769 7468 206f 7065 6e28  ader..with open(
-00001e30: 2774 6573 742f 6f6e 652e 6461 7427 2c27  'test/one.dat','
-00001e40: 7262 2729 2061 7320 6668 3a0a 2020 2020  rb') as fh:.    
-00001e50: 7265 6164 6572 203d 204d 4152 4352 6561  reader = MARCRea
-00001e60: 6465 7228 6668 290a 2020 2020 666f 7220  der(fh).    for 
-00001e70: 7265 636f 7264 2069 6e20 7265 6164 6572  record in reader
-00001e80: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
-00001e90: 7265 636f 7264 2e61 735f 6a73 6f6e 2869  record.as_json(i
-00001ea0: 6e64 656e 743d 3229 290a 6060 600a 0a60  ndent=2)).```..`
-00001eb0: 6060 6a61 7661 7363 7269 7074 0a7b 0a20  ``javascript.{. 
-00001ec0: 2022 6c65 6164 6572 223a 2022 3031 3036   "leader": "0106
-00001ed0: 3063 616d 2020 3232 3030 3238 3934 6120  0cam  22002894a 
-00001ee0: 3435 3030 222c 0a20 2022 6669 656c 6473  4500",.  "fields
-00001ef0: 223a 205b 0a20 2020 207b 0a20 2020 2020  ": [.    {.     
-00001f00: 2022 3030 3122 3a20 2231 3137 3738 3530   "001": "1177850
-00001f10: 3422 0a20 2020 207d 2c0a 2020 2020 7b0a  4".    },.    {.
-00001f20: 2020 2020 2020 2230 3130 223a 207b 0a20        "010": {. 
-00001f30: 2020 2020 2020 2022 696e 6431 223a 2022         "ind1": "
-00001f40: 2022 2c0a 2020 2020 2020 2020 2273 7562   ",.        "sub
-00001f50: 6669 656c 6473 223a 205b 0a20 2020 2020  fields": [.     
-00001f60: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00001f70: 2020 2022 6122 3a20 2220 2020 3939 3034     "a": "   9904
-00001f80: 3335 3831 2022 0a20 2020 2020 2020 2020  3581 ".         
-00001f90: 207d 0a20 2020 2020 2020 205d 2c0a 2020   }.        ],.  
-00001fa0: 2020 2020 2020 2269 6e64 3222 3a20 2220        "ind2": " 
-00001fb0: 220a 2020 2020 2020 7d0a 2020 2020 7d2c  ".      }.    },
-00001fc0: 0a20 2020 207b 0a20 2020 2020 2022 3130  .    {.      "10
-00001fd0: 3022 3a20 7b0a 2020 2020 2020 2020 2269  0": {.        "i
-00001fe0: 6e64 3122 3a20 2231 222c 0a20 2020 2020  nd1": "1",.     
-00001ff0: 2020 2022 7375 6266 6965 6c64 7322 3a20     "subfields": 
-00002000: 5b0a 2020 2020 2020 2020 2020 7b0a 2020  [.          {.  
-00002010: 2020 2020 2020 2020 2020 2261 223a 2022            "a": "
-00002020: 4875 6e74 2c20 416e 6472 6577 2c22 0a20  Hunt, Andrew,". 
-00002030: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00002040: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00002050: 2020 2020 2264 223a 2022 3139 3634 2d22      "d": "1964-"
-00002060: 0a20 2020 2020 2020 2020 207d 0a20 2020  .          }.   
-00002070: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00002080: 2269 6e64 3222 3a20 2220 220a 2020 2020  "ind2": " ".    
-00002090: 2020 7d0a 2020 2020 7d2c 0a20 2020 207b    }.    },.    {
-000020a0: 0a20 2020 2020 2022 3234 3522 3a20 7b0a  .      "245": {.
-000020b0: 2020 2020 2020 2020 2269 6e64 3122 3a20          "ind1": 
-000020c0: 2231 222c 0a20 2020 2020 2020 2022 7375  "1",.        "su
-000020d0: 6266 6965 6c64 7322 3a20 5b0a 2020 2020  bfields": [.    
-000020e0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-000020f0: 2020 2020 2261 223a 2022 5468 6520 7072      "a": "The pr
-00002100: 6167 6d61 7469 6320 7072 6f67 7261 6d6d  agmatic programm
-00002110: 6572 203a 220a 2020 2020 2020 2020 2020  er :".          
-00002120: 7d2c 0a20 2020 2020 2020 2020 207b 0a20  },.          {. 
-00002130: 2020 2020 2020 2020 2020 2022 6222 3a20             "b": 
-00002140: 2266 726f 6d20 6a6f 7572 6e65 796d 616e  "from journeyman
-00002150: 2074 6f20 6d61 7374 6572 202f 220a 2020   to master /".  
-00002160: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00002170: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00002180: 2020 2022 6322 3a20 2241 6e64 7265 7720     "c": "Andrew 
-00002190: 4875 6e74 2c20 4461 7669 6420 5468 6f6d  Hunt, David Thom
-000021a0: 6173 2e22 0a20 2020 2020 2020 2020 207d  as.".          }
-000021b0: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
-000021c0: 2020 2020 2269 6e64 3222 3a20 2234 220a      "ind2": "4".
-000021d0: 2020 2020 2020 7d0a 2020 2020 7d2c 0a20        }.    },. 
-000021e0: 2020 207b 0a20 2020 2020 2022 3236 3022     {.      "260"
-000021f0: 3a20 7b0a 2020 2020 2020 2020 2269 6e64  : {.        "ind
-00002200: 3122 3a20 2220 222c 0a20 2020 2020 2020  1": " ",.       
-00002210: 2022 7375 6266 6965 6c64 7322 3a20 5b0a   "subfields": [.
-00002220: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-00002230: 2020 2020 2020 2020 2261 223a 2022 5265          "a": "Re
-00002240: 6164 696e 672c 204d 6173 7320 3a22 0a20  ading, Mass :". 
-00002250: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00002260: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00002270: 2020 2020 2262 223a 2022 4164 6469 736f      "b": "Addiso
-00002280: 6e2d 5765 736c 6579 2c22 0a20 2020 2020  n-Wesley,".     
-00002290: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-000022a0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-000022b0: 2263 223a 2022 3230 3030 2e22 0a20 2020  "c": "2000.".   
-000022c0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-000022d0: 205d 2c0a 2020 2020 2020 2020 2269 6e64   ],.        "ind
-000022e0: 3222 3a20 2220 220a 2020 2020 2020 7d0a  2": " ".      }.
-000022f0: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
-00002300: 2020 2022 3330 3022 3a20 7b0a 2020 2020     "300": {.    
-00002310: 2020 2020 2269 6e64 3122 3a20 2220 222c      "ind1": " ",
-00002320: 0a20 2020 2020 2020 2022 7375 6266 6965  .        "subfie
-00002330: 6c64 7322 3a20 5b0a 2020 2020 2020 2020  lds": [.        
-00002340: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00002350: 2261 223a 2022 7878 6976 2c20 3332 3120  "a": "xxiv, 321 
-00002360: 702e 203b 220a 2020 2020 2020 2020 2020  p. ;".          
-00002370: 7d2c 0a20 2020 2020 2020 2020 207b 0a20  },.          {. 
-00002380: 2020 2020 2020 2020 2020 2022 6322 3a20             "c": 
-00002390: 2232 3420 636d 2e22 0a20 2020 2020 2020  "24 cm.".       
-000023a0: 2020 207d 0a20 2020 2020 2020 205d 2c0a     }.        ],.
-000023b0: 2020 2020 2020 2020 2269 6e64 3222 3a20          "ind2": 
-000023c0: 2220 220a 2020 2020 2020 7d0a 2020 2020  " ".      }.    
-000023d0: 7d2c 0a20 2020 207b 0a20 2020 2020 2022  },.    {.      "
-000023e0: 3530 3422 3a20 7b0a 2020 2020 2020 2020  504": {.        
-000023f0: 2269 6e64 3122 3a20 2220 222c 0a20 2020  "ind1": " ",.   
-00002400: 2020 2020 2022 7375 6266 6965 6c64 7322       "subfields"
-00002410: 3a20 5b0a 2020 2020 2020 2020 2020 7b0a  : [.          {.
-00002420: 2020 2020 2020 2020 2020 2020 2261 223a              "a":
-00002430: 2022 496e 636c 7564 6573 2062 6962 6c69   "Includes bibli
-00002440: 6f67 7261 7068 6963 616c 2072 6566 6572  ographical refer
-00002450: 656e 6365 732e 220a 2020 2020 2020 2020  ences.".        
-00002460: 2020 7d0a 2020 2020 2020 2020 5d2c 0a20    }.        ],. 
-00002470: 2020 2020 2020 2022 696e 6432 223a 2022         "ind2": "
-00002480: 2022 0a20 2020 2020 207d 0a20 2020 207d   ".      }.    }
-00002490: 2c0a 2020 2020 7b0a 2020 2020 2020 2236  ,.    {.      "6
-000024a0: 3530 223a 207b 0a20 2020 2020 2020 2022  50": {.        "
-000024b0: 696e 6431 223a 2022 2022 2c0a 2020 2020  ind1": " ",.    
-000024c0: 2020 2020 2273 7562 6669 656c 6473 223a      "subfields":
-000024d0: 205b 0a20 2020 2020 2020 2020 207b 0a20   [.          {. 
-000024e0: 2020 2020 2020 2020 2020 2022 6122 3a20             "a": 
-000024f0: 2243 6f6d 7075 7465 7220 7072 6f67 7261  "Computer progra
-00002500: 6d6d 696e 672e 220a 2020 2020 2020 2020  mming.".        
-00002510: 2020 7d0a 2020 2020 2020 2020 5d2c 0a20    }.        ],. 
-00002520: 2020 2020 2020 2022 696e 6432 223a 2022         "ind2": "
-00002530: 3022 0a20 2020 2020 207d 0a20 2020 207d  0".      }.    }
-00002540: 2c0a 2020 2020 7b0a 2020 2020 2020 2237  ,.    {.      "7
-00002550: 3030 223a 207b 0a20 2020 2020 2020 2022  00": {.        "
-00002560: 696e 6431 223a 2022 3122 2c0a 2020 2020  ind1": "1",.    
-00002570: 2020 2020 2273 7562 6669 656c 6473 223a      "subfields":
-00002580: 205b 0a20 2020 2020 2020 2020 207b 0a20   [.          {. 
-00002590: 2020 2020 2020 2020 2020 2022 6122 3a20             "a": 
-000025a0: 2254 686f 6d61 732c 2044 6176 6964 2c22  "Thomas, David,"
-000025b0: 0a20 2020 2020 2020 2020 207d 2c0a 2020  .          },.  
-000025c0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-000025d0: 2020 2020 2020 2264 223a 2022 3139 3536        "d": "1956
-000025e0: 2d22 0a20 2020 2020 2020 2020 207d 0a20  -".          }. 
-000025f0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-00002600: 2020 2269 6e64 3222 3a20 2220 220a 2020    "ind2": " ".  
-00002610: 2020 2020 7d0a 2020 2020 7d0a 2020 5d0a      }.    }.  ].
-00002620: 7d0a 6060 600a 0a49 6620 796f 7520 7761  }.```..If you wa
-00002630: 6e74 2074 6f20 7061 7273 6520 6120 6669  nt to parse a fi
-00002640: 6c65 206f 6620 4d41 5243 4a53 4f4e 2072  le of MARCJSON r
-00002650: 6563 6f72 6473 2079 6f75 2063 616e 3a0a  ecords you can:.
-00002660: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
-00002670: 7079 6d61 7263 2069 6d70 6f72 7420 7061  pymarc import pa
-00002680: 7273 655f 6a73 6f6e 5f74 6f5f 6172 7261  rse_json_to_arra
-00002690: 790a 0a72 6563 6f72 6473 203d 2070 6172  y..records = par
-000026a0: 7365 5f6a 736f 6e5f 746f 5f61 7272 6179  se_json_to_array
-000026b0: 286f 7065 6e28 2774 6573 742f 6261 7463  (open('test/batc
-000026c0: 682e 6a73 6f6e 2729 290a 0a70 7269 6e74  h.json'))..print
-000026d0: 2872 6563 6f72 6473 5b30 5d29 0a60 6060  (records[0]).```
-000026e0: 0a0a 6060 600a 3d4c 4452 2020 3030 3932  ..```.=LDR  0092
-000026f0: 356e 6a6d 2020 3232 3030 3237 3737 6120  5njm  22002777a 
-00002700: 3435 3030 0a3d 3030 3120 2035 3633 3732  4500.=001  56372
-00002710: 3431 0a3d 3030 3320 2044 4c43 0a3d 3030  41.=003  DLC.=00
-00002720: 3520 2031 3939 3230 3832 3630 3834 3033  5  1992082608403
-00002730: 362e 300a 3d30 3037 2020 7364 7562 756d  6.0.=007  sdubum
-00002740: 656e 6e6d 706c 750a 3d30 3038 2020 3931  ennmplu.=008  91
-00002750: 3039 3236 7331 3935 375c 5c5c 5c6e 7975  0926s1957\\\\nyu
-00002760: 7575 6e5c 5c5c 5c5c 5c5c 5c5c 5c5c 5c5c  uun\\\\\\\\\\\\\
-00002770: 5c65 6e67 5c5c 0a3d 3031 3020 205c 5c24  \eng\\.=010  \\$
-00002780: 6120 2020 3931 3735 3833 3335 0a3d 3032  a   91758335.=02
-00002790: 3820 2030 3024 6131 3235 3924 6241 746c  8  00$a1259$bAtl
-000027a0: 616e 7469 630a 3d30 3430 2020 5c5c 2461  antic.=040  \\$a
-000027b0: 444c 4324 6344 4c43 0a3d 3035 3020 2030  DLC$cDLC.=050  0
-000027c0: 3024 6141 746c 616e 7469 6320 3132 3539  0$aAtlantic 1259
-000027d0: 0a3d 3234 3520 2030 3424 6154 6865 2047  .=245  04$aThe G
-000027e0: 7265 6174 2052 6179 2043 6861 726c 6573  reat Ray Charles
-000027f0: 2468 5b73 6f75 6e64 2072 6563 6f72 6469  $h[sound recordi
-00002800: 6e67 5d2e 0a3d 3236 3020 205c 5c24 614e  ng]..=260  \\$aN
-00002810: 6577 2059 6f72 6b2c 204e 2e59 2e20 3a24  ew York, N.Y. :$
-00002820: 6241 746c 616e 7469 632c 2463 5b31 3935  bAtlantic,$c[195
-00002830: 373f 5d0a 3d33 3030 2020 5c5c 2461 3120  7?].=300  \\$a1 
-00002840: 736f 756e 6420 6469 7363 203a 2462 616e  sound disc :$ban
-00002850: 616c 6f67 2c20 3333 2031 2f33 2072 706d  alog, 33 1/3 rpm
-00002860: 203b 2463 3132 2069 6e2e 0a3d 3531 3120   ;$c12 in..=511 
-00002870: 2030 5c24 6152 6179 2043 6861 726c 6573   0\$aRay Charles
-00002880: 2c20 7069 616e 6f20 2620 6365 6c65 7374  , piano & celest
-00002890: 652e 0a3d 3530 3520 2030 5c24 6154 6865  e..=505  0\$aThe
-000028a0: 2052 6179 202d 2d20 4d79 206d 656c 616e   Ray -- My melan
-000028b0: 6368 6f6c 7920 6261 6279 202d 2d20 426c  choly baby -- Bl
-000028c0: 6163 6b20 636f 6666 6565 202d 2d20 5468  ack coffee -- Th
-000028d0: 6572 6527 7320 6e6f 2079 6f75 202d 2d20  ere's no you -- 
-000028e0: 446f 6f64 6c69 6e27 202d 2d20 5377 6565  Doodlin' -- Swee
-000028f0: 7420 7369 7874 6565 6e20 6261 7273 202d  t sixteen bars -
-00002900: 2d20 4920 7375 7272 656e 6465 7220 6465  - I surrender de
-00002910: 6172 202d 2d20 556e 6465 6369 6465 642e  ar -- Undecided.
-00002920: 0a3d 3530 3020 205c 5c24 6142 7269 6566  .=500  \\$aBrief
-00002930: 2072 6563 6f72 642e 0a3d 3635 3020 205c   record..=650  \
-00002940: 3024 614a 617a 7a24 7931 3935 312d 3139  0$aJazz$y1951-19
-00002950: 3630 2e0a 3d36 3530 2020 5c30 2461 5069  60..=650  \0$aPi
-00002960: 616e 6f20 7769 7468 206a 617a 7a20 656e  ano with jazz en
-00002970: 7365 6d62 6c65 2e0a 3d37 3030 2020 315c  semble..=700  1\
-00002980: 2461 4368 6172 6c65 732c 2052 6179 2c24  $aCharles, Ray,$
-00002990: 6431 3933 302d 2434 7072 660a 6060 600a  d1930-$4prf.```.
-000029a0: 0a53 7570 706f 7274 0a2d 2d2d 2d2d 2d2d  .Support.-------
-000029b0: 0a0a 5468 6520 7079 6d61 7263 2064 6576  ..The pymarc dev
-000029c0: 656c 6f70 6572 7320 656e 636f 7572 6167  elopers encourag
-000029d0: 6520 796f 7520 746f 206a 6f69 6e20 7468  e you to join th
-000029e0: 6520 5b70 796d 6172 6320 476f 6f67 6c65  e [pymarc Google
-000029f0: 0a47 726f 7570 5d28 6874 7470 3a2f 2f67  .Group](http://g
-00002a00: 726f 7570 732e 676f 6f67 6c65 2e63 6f6d  roups.google.com
-00002a10: 2f67 726f 7570 2f70 796d 6172 6329 2069  /group/pymarc) i
-00002a20: 6620 796f 7520 6e65 6564 2068 656c 702e  f you need help.
-00002a30: 2020 416c 736f 2c20 706c 6561 7365 0a66    Also, please.f
-00002a40: 6565 6c20 6672 6565 2074 6f20 7573 6520  eel free to use 
-00002a50: 5b69 7373 7565 2074 7261 636b 696e 675d  [issue tracking]
-00002a60: 2868 7474 7073 3a2f 2f67 6974 6c61 622e  (https://gitlab.
-00002a70: 636f 6d2f 7079 6d61 7263 2f70 796d 6172  com/pymarc/pymar
-00002a80: 632f 6973 7375 6573 2920 6f6e 0a47 6974  c/issues) on.Git
-00002a90: 4c61 6220 746f 2073 7562 6d69 7420 6665  Lab to submit fe
-00002aa0: 6174 7572 6520 7265 7175 6573 7473 206f  ature requests o
-00002ab0: 7220 6275 6720 7265 706f 7274 732e 2049  r bug reports. I
-00002ac0: 6620 796f 7527 7665 2067 6f74 2061 6e20  f you've got an 
-00002ad0: 6974 6368 2074 6f0a 7363 7261 7463 682c  itch to.scratch,
-00002ae0: 2070 6c65 6173 6520 7363 7261 7463 6820   please scratch 
-00002af0: 6974 2c20 616e 6420 7365 6e64 206d 6572  it, and send mer
-00002b00: 6765 2072 6571 7565 7374 7320 6f6e 0a5b  ge requests on.[
-00002b10: 4769 744c 6162 5d28 6874 7470 3a2f 2f67  GitLab](http://g
-00002b20: 6974 6c61 622e 636f 6d2f 7079 6d61 7263  itlab.com/pymarc
-00002b30: 2f70 796d 6172 6329 2e0a 0a49 6620 796f  /pymarc)...If yo
-00002b40: 7520 7374 6172 7420 776f 726b 696e 6720  u start working 
-00002b50: 7769 7468 204d 4152 4320 796f 7520 6d61  with MARC you ma
-00002b60: 7920 6665 656c 206c 696b 6520 796f 7520  y feel like you 
-00002b70: 6e65 6564 206d 6f72 616c 2073 7570 706f  need moral suppo
-00002b80: 7274 0a69 6e20 6164 6469 7469 6f6e 2074  rt.in addition t
-00002b90: 6f20 7465 6368 6e69 6361 6c20 7375 7070  o technical supp
-00002ba0: 6f72 742e 2054 6865 0a5b 2363 6f64 6534  ort. The.[#code4
-00002bb0: 6c69 625d 2869 7263 733a 2f2f 6972 632e  lib](ircs://irc.
-00002bc0: 6c69 6265 7261 2e63 6861 742f 636f 6465  libera.chat/code
-00002bd0: 346c 6962 2920 6368 616e 6e65 6c20 6f6e  4lib) channel on
-00002be0: 205b 4c69 6265 7261 5d28 6874 7470 733a   [Libera](https:
-00002bf0: 2f2f 6c69 6265 7261 2e63 6861 742f 2920  //libera.chat/) 
-00002c00: 6973 2061 2067 6f6f 6420 706c 6163 6520  is a good place 
-00002c10: 666f 7220 626f 7468 2e0a                 for both..
+000010d0: 6772 6573 7320 0a69 7320 6120 676f 6f64  gress .is a good
+000010e0: 2072 6566 6572 656e 6365 206f 6e63 6520   reference once 
+000010f0: 796f 7520 756e 6465 7273 7461 6e64 2074  you understand t
+00001100: 6865 2062 6173 6963 732e 0a0a 2323 2320  he basics...### 
+00001110: 5772 6974 696e 670a 0a2a 4e6f 7465 3a20  Writing..*Note: 
+00001120: 4173 206f 6620 7635 2e30 2e30 2060 5375  As of v5.0.0 `Su
+00001130: 6266 6965 6c64 6020 6973 2075 7365 6420  bfield` is used 
+00001140: 746f 2063 7265 6174 6520 7375 6266 6965  to create subfie
+00001150: 6c64 732e 2050 7269 6f72 2074 6f20 7635  lds. Prior to v5
+00001160: 2c0a 7375 6266 6965 6c64 7320 7765 7265  ,.subfields were
+00001170: 2063 6f6e 7374 7275 6374 6564 2061 6e64   constructed and
+00001180: 2061 6363 6573 7365 6420 6173 2061 206c   accessed as a l
+00001190: 6973 7420 6f66 2073 7472 696e 6773 2c20  ist of strings, 
+000011a0: 652e 672e 2c20 605b 636f 6465 2c0a 7661  e.g., `[code,.va
+000011b0: 6c75 652c 2063 6f64 652c 2076 616c 7565  lue, code, value
+000011c0: 5d60 2e20 496e 2076 352e 302e 3020 7468  ]`. In v5.0.0 th
+000011d0: 6973 2068 6173 2062 6565 6e20 6368 616e  is has been chan
+000011e0: 6765 6420 746f 206f 7267 616e 697a 6520  ged to organize 
+000011f0: 7468 6520 7375 6266 6965 6c64 730a 696e  the subfields.in
+00001200: 746f 2061 206c 6973 7420 6f66 2074 7570  to a list of tup
+00001210: 6c65 732c 2065 2e67 2e2c 2060 5b28 636f  les, e.g., `[(co
+00001220: 6465 2c20 7661 6c75 6529 2c20 2863 6f64  de, value), (cod
+00001230: 652c 2076 616c 7565 295d 602e 2054 6865  e, value)]`. The
+00001240: 2060 5375 6266 6965 6c64 600a 6973 2069   `Subfield`.is i
+00001250: 6d70 6c65 6d65 6e74 6564 2061 7320 6120  mplemented as a 
+00001260: 604e 616d 6564 5475 706c 6560 2073 6f20  `NamedTuple` so 
+00001270: 7468 6174 2074 6865 2074 7570 6c65 7320  that the tuples 
+00001280: 6361 6e20 6265 2063 6f6e 7374 7275 6374  can be construct
+00001290: 6564 2061 730a 6053 7562 6669 656c 6428  ed as.`Subfield(
+000012a0: 636f 6465 3d63 6f64 652c 2076 616c 7565  code=code, value
+000012b0: 3d76 616c 7565 2960 2e20 5468 6520 6f6c  =value)`. The ol
+000012c0: 6420 7374 796c 6520 6f66 2063 7265 6174  d style of creat
+000012d0: 696e 6720 7375 6266 6965 6c64 7320 6973  ing subfields is
+000012e0: 206e 6f0a 6c6f 6e67 6572 2073 7570 706f   no.longer suppo
+000012f0: 7274 6564 2e20 4174 7465 6d70 7469 6e67  rted. Attempting
+00001300: 2074 6f20 7061 7373 2061 206c 6973 7420   to pass a list 
+00001310: 6f66 2073 7472 696e 6773 2074 6f20 7468  of strings to th
+00001320: 6520 6073 7562 6669 656c 6473 600a 7061  e `subfields`.pa
+00001330: 7261 6d65 7465 7220 666f 7220 7468 6520  rameter for the 
+00001340: 6046 6965 6c64 6020 636f 6e73 7472 7563  `Field` construc
+00001350: 746f 7220 7769 6c6c 2072 6169 7365 2061  tor will raise a
+00001360: 2060 5661 6c75 6545 7272 6f72 602e 2046   `ValueError`. F
+00001370: 6f72 0a63 6f6e 7665 6e69 656e 6365 2074  or.convenience t
+00001380: 6865 2060 4669 656c 642e 636f 6e76 6572  he `Field.conver
+00001390: 745f 6c65 6761 6379 5f73 7562 6669 656c  t_legacy_subfiel
+000013a0: 6473 6020 636c 6173 7320 6d65 7468 6f64  ds` class method
+000013b0: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
+000013c0: 0a63 6f6e 7665 7274 2061 206c 6567 6163  .convert a legac
+000013d0: 7920 6c69 7374 206f 6620 7374 7269 6e67  y list of string
+000013e0: 7320 696e 746f 2061 206c 6973 7420 6f66  s into a list of
+000013f0: 2060 5375 6266 6965 6c64 6073 2e2a 0a0a   `Subfield`s.*..
+00001400: 4865 7265 2773 2061 6e20 6578 616d 706c  Here's an exampl
+00001410: 6520 6f66 2063 7265 6174 696e 6720 6120  e of creating a 
+00001420: 7265 636f 7264 2061 6e64 2077 7269 7469  record and writi
+00001430: 6e67 2069 7420 6f75 7420 746f 2061 2066  ng it out to a f
+00001440: 696c 652e 0a0a 6060 6070 7974 686f 6e0a  ile...```python.
+00001450: 6672 6f6d 2070 796d 6172 6320 696d 706f  from pymarc impo
+00001460: 7274 2052 6563 6f72 642c 2046 6965 6c64  rt Record, Field
+00001470: 2c20 5375 6266 6965 6c64 0a0a 7265 636f  , Subfield..reco
+00001480: 7264 203d 2052 6563 6f72 6428 290a 7265  rd = Record().re
+00001490: 636f 7264 2e61 6464 5f66 6965 6c64 280a  cord.add_field(.
+000014a0: 2020 2020 4669 656c 6428 0a20 2020 2020      Field(.     
+000014b0: 2020 2074 6167 3d27 3234 3527 2c0a 2020     tag='245',.  
+000014c0: 2020 2020 2020 696e 6469 6361 746f 7273        indicators
+000014d0: 3d5b 2730 272c 2027 3127 5d2c 0a20 2020  =['0', '1'],.   
+000014e0: 2020 2020 2073 7562 6669 656c 6473 3d5b       subfields=[
+000014f0: 0a20 2020 2020 2020 2020 2020 2053 7562  .            Sub
+00001500: 6669 656c 6428 636f 6465 3d27 6127 2c20  field(code='a', 
+00001510: 7661 6c75 653d 2754 6865 2070 7261 676d  value='The pragm
+00001520: 6174 6963 2070 726f 6772 616d 6d65 7220  atic programmer 
+00001530: 3a20 2729 2c0a 2020 2020 2020 2020 2020  : '),.          
+00001540: 2020 5375 6266 6965 6c64 2863 6f64 653d    Subfield(code=
+00001550: 2762 272c 2076 616c 7565 3d27 6672 6f6d  'b', value='from
+00001560: 206a 6f75 726e 6579 6d61 6e20 746f 206d   journeyman to m
+00001570: 6173 7465 7220 2f27 292c 0a20 2020 2020  aster /'),.     
+00001580: 2020 2020 2020 2053 7562 6669 656c 6428         Subfield(
+00001590: 636f 6465 3d27 6327 2c20 7661 6c75 653d  code='c', value=
+000015a0: 2741 6e64 7265 7720 4875 6e74 2c20 4461  'Andrew Hunt, Da
+000015b0: 7669 6420 5468 6f6d 6173 2e27 290a 2020  vid Thomas.').  
+000015c0: 2020 2020 2020 5d29 290a 7769 7468 206f        ])).with o
+000015d0: 7065 6e28 2766 696c 652e 6461 7427 2c20  pen('file.dat', 
+000015e0: 2777 6227 2920 6173 206f 7574 3a0a 2020  'wb') as out:.  
+000015f0: 2020 6f75 742e 7772 6974 6528 7265 636f    out.write(reco
+00001600: 7264 2e61 735f 6d61 7263 2829 290a 6060  rd.as_marc()).``
+00001610: 600a 0a54 6f20 636f 6e76 6572 7420 6672  `..To convert fr
+00001620: 6f6d 2074 6865 206f 6c64 2073 7472 696e  om the old strin
+00001630: 6720 6c69 7374 2074 6f20 6120 6c69 7374  g list to a list
+00001640: 206f 6620 6053 7562 6669 656c 6460 732c   of `Subfield`s,
+00001650: 2074 6865 2060 2e63 6f6e 7665 7274 5f6c   the `.convert_l
+00001660: 6567 6163 795f 7375 6266 6965 6c64 7360  egacy_subfields`
+00001670: 2063 6c61 7373 206d 6574 686f 640a 6973   class method.is
+00001680: 2070 726f 7669 6465 6420 6f6e 2074 6865   provided on the
+00001690: 2060 4669 656c 6460 2063 6c61 7373 2e0a   `Field` class..
+000016a0: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+000016b0: 7079 6d61 7263 2069 6d70 6f72 7420 4669  pymarc import Fi
+000016c0: 656c 642c 2053 7562 6669 656c 640a 0a6c  eld, Subfield..l
+000016d0: 6567 6163 795f 6669 656c 6473 3a20 6c69  egacy_fields: li
+000016e0: 7374 5b73 7472 5d20 3d20 5b27 6127 2c20  st[str] = ['a', 
+000016f0: 2754 6865 2070 7261 676d 6174 6963 2070  'The pragmatic p
+00001700: 726f 6772 616d 6d65 7220 3a20 272c 0a20  rogrammer : ',. 
+00001710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001720: 2020 2020 2020 2020 2020 2027 6227 2c20             'b', 
+00001730: 2766 726f 6d20 6a6f 7572 6e65 796d 616e  'from journeyman
+00001740: 2074 6f20 6d61 7374 6572 202f 272c 0a20   to master /',. 
+00001750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001760: 2020 2020 2020 2020 2020 2027 6327 2c20             'c', 
+00001770: 2741 6e64 7265 7720 4875 6e74 2c20 4461  'Andrew Hunt, Da
+00001780: 7669 6420 5468 6f6d 6173 275d 0a0a 636f  vid Thomas']..co
+00001790: 6465 645f 6669 656c 6473 3a20 6c69 7374  ded_fields: list
+000017a0: 5b53 7562 6669 656c 645d 203d 2046 6965  [Subfield] = Fie
+000017b0: 6c64 2e63 6f6e 7665 7274 5f6c 6567 6163  ld.convert_legac
+000017c0: 795f 7375 6266 6965 6c64 7328 6c65 6761  y_subfields(lega
+000017d0: 6379 5f66 6965 6c64 7329 0a60 6060 0a0a  cy_fields).```..
+000017e0: 2323 2320 5570 6461 7469 6e67 0a0a 5570  ### Updating..Up
+000017f0: 6461 7469 6e67 2077 6f72 6b73 2074 6865  dating works the
+00001800: 2073 616d 6520 7761 792c 2079 6f75 2072   same way, you r
+00001810: 6561 6420 6974 2069 6e2c 206d 6f64 6966  ead it in, modif
+00001820: 7920 6974 2c20 616e 6420 7468 656e 2077  y it, and then w
+00001830: 7269 7465 2069 7420 6f75 740a 6167 6169  rite it out.agai
+00001840: 6e3a 0a0a 6060 6070 7974 686f 6e0a 6672  n:..```python.fr
+00001850: 6f6d 2070 796d 6172 6320 696d 706f 7274  om pymarc import
+00001860: 204d 4152 4352 6561 6465 720a 7769 7468   MARCReader.with
+00001870: 206f 7065 6e28 2774 6573 742f 6d61 7263   open('test/marc
+00001880: 2e64 6174 272c 2027 7262 2729 2061 7320  .dat', 'rb') as 
+00001890: 6668 3a0a 2020 2020 7265 6164 6572 203d  fh:.    reader =
+000018a0: 204d 4152 4352 6561 6465 7228 6668 290a   MARCReader(fh).
+000018b0: 2020 2020 7265 636f 7264 203d 206e 6578      record = nex
+000018c0: 7428 7265 6164 6572 290a 2020 2020 7265  t(reader).    re
+000018d0: 636f 7264 5b27 3234 3527 5d5b 2761 275d  cord['245']['a']
+000018e0: 203d 2027 5468 6520 5a6f 6d62 6965 2050   = 'The Zombie P
+000018f0: 726f 6772 616d 6d65 7220 3a20 270a 7769  rogrammer : '.wi
+00001900: 7468 206f 7065 6e28 2766 696c 652e 6461  th open('file.da
+00001910: 7427 2c20 2777 6227 2920 6173 206f 7574  t', 'wb') as out
+00001920: 3a0a 2020 2020 6f75 742e 7772 6974 6528  :.    out.write(
+00001930: 7265 636f 7264 2e61 735f 6d61 7263 2829  record.as_marc()
+00001940: 290a 6060 600a 0a0a 2323 2320 4a53 4f4e  ).```...### JSON
+00001950: 2061 6e64 2058 4d4c 0a0a 4966 2079 6f75   and XML..If you
+00001960: 2066 696e 6420 796f 7572 7365 6c66 2075   find yourself u
+00001970: 7369 6e67 204d 4152 4320 6461 7461 2061  sing MARC data a
+00001980: 2066 6169 7220 6269 742c 2061 6e64 2064   fair bit, and d
+00001990: 6973 7472 6962 7574 696e 6720 6974 2c20  istributing it, 
+000019a0: 796f 7520 6d61 790a 6d61 6b65 206f 7468  you may.make oth
+000019b0: 6572 2064 6576 656c 6f70 6572 7320 6120  er developers a 
+000019c0: 6269 7420 6861 7070 6965 7220 6279 2075  bit happier by u
+000019d0: 7369 6e67 2074 6865 204a 534f 4e20 6f72  sing the JSON or
+000019e0: 2058 4d4c 2073 6572 6961 6c69 7a61 7469   XML serializati
+000019f0: 6f6e 732e 2054 6865 0a6d 6169 6e20 6265  ons. The.main be
+00001a00: 6e65 6669 7420 746f 2075 7369 6e67 2058  nefit to using X
+00001a10: 4d4c 206f 7220 4a53 4f4e 2069 7320 7468  ML or JSON is th
+00001a20: 6174 2074 6865 2055 5446 3820 6368 6172  at the UTF8 char
+00001a30: 6163 7465 7220 656e 636f 6469 6e67 2069  acter encoding i
+00001a40: 7320 7573 6564 2c0a 7261 7468 6572 2074  s used,.rather t
+00001a50: 6861 6e20 7468 6520 6672 7573 7472 6174  han the frustrat
+00001a60: 696e 676c 7920 6172 6368 6169 6320 4d41  ingly archaic MA
+00001a70: 5243 3820 656e 636f 6469 6e67 2e20 416c  RC8 encoding. Al
+00001a80: 736f 2074 6865 7920 7769 6c6c 2062 6520  so they will be 
+00001a90: 6162 6c65 2074 6f0a 7573 6520 7374 616e  able to.use stan
+00001aa0: 6461 7264 204a 534f 4e20 616e 6420 584d  dard JSON and XM
+00001ab0: 4c20 7265 6164 696e 672f 7772 6974 696e  L reading/writin
+00001ac0: 6720 746f 6f6c 7320 746f 2067 6574 2061  g tools to get a
+00001ad0: 7420 7468 6520 6461 7461 2074 6865 7920  t the data they 
+00001ae0: 7761 6e74 0a69 6e73 7465 6164 206f 6620  want.instead of 
+00001af0: 736f 6d65 2063 7261 7a79 204d 4152 4320  some crazy MARC 
+00001b00: 7072 6f63 6573 7369 6e67 206c 6962 7261  processing libra
+00001b10: 7279 206c 696b 652c 2061 6865 6d2c 2070  ry like, ahem, p
+00001b20: 796d 6172 632e 0a0a 2a2a 584d 4c2a 2a0a  ymarc...**XML**.
+00001b30: 0a54 6f20 7061 7273 6520 6120 6669 6c65  .To parse a file
+00001b40: 206f 6620 4d41 5243 584d 4c20 7265 636f   of MARCXML reco
+00001b50: 7264 7320 796f 7520 6361 6e3a 0a0a 6060  rds you can:..``
+00001b60: 6070 7974 686f 6e0a 0a66 726f 6d20 7079  `python..from py
+00001b70: 6d61 7263 2069 6d70 6f72 7420 7061 7273  marc import pars
+00001b80: 655f 786d 6c5f 746f 5f61 7272 6179 0a0a  e_xml_to_array..
+00001b90: 7265 636f 7264 7320 3d20 7061 7273 655f  records = parse_
+00001ba0: 786d 6c5f 746f 5f61 7272 6179 2827 7465  xml_to_array('te
+00001bb0: 7374 2f62 6174 6368 2e78 6d6c 2729 0a60  st/batch.xml').`
+00001bc0: 6060 0a0a 4966 2079 6f75 2068 6176 6520  ``..If you have 
+00001bd0: 6120 6c61 7267 6520 584d 4c20 6669 6c65  a large XML file
+00001be0: 2061 6e64 2077 6f75 6c64 2072 6174 6865   and would rathe
+00001bf0: 7220 6e6f 7420 7265 6164 2074 6865 6d20  r not read them 
+00001c00: 616c 6c20 696e 746f 206d 656d 6f72 7920  all into memory 
+00001c10: 796f 750a 6361 6e3a 0a0a 6060 6070 7974  you.can:..```pyt
+00001c20: 686f 6e0a 0a66 726f 6d20 7079 6d61 7263  hon..from pymarc
+00001c30: 2069 6d70 6f72 7420 6d61 705f 786d 6c0a   import map_xml.
+00001c40: 0a64 6566 2070 7269 6e74 5f74 6974 6c65  .def print_title
+00001c50: 2872 293a 0a20 2020 2070 7269 6e74 2872  (r):.    print(r
+00001c60: 2e74 6974 6c65 290a 0a6d 6170 5f78 6d6c  .title)..map_xml
+00001c70: 2870 7269 6e74 5f74 6974 6c65 2c20 2774  (print_title, 't
+00001c80: 6573 742f 6261 7463 682e 786d 6c27 290a  est/batch.xml').
+00001c90: 6060 600a 0a41 6c73 6f2c 2069 6620 796f  ```..Also, if yo
+00001ca0: 7520 7072 6566 6572 2079 6f75 2063 616e  u prefer you can
+00001cb0: 2070 6173 7320 696e 2061 2066 696c 6520   pass in a file 
+00001cc0: 6c69 6b65 206f 626a 6563 7420 696e 2061  like object in a
+00001cd0: 6464 6974 696f 6e20 746f 2074 6865 2070  ddition to the p
+00001ce0: 6174 680a 746f 2062 6f74 6820 2a6d 6170  ath.to both *map
+00001cf0: 5f78 6d6c 2a20 616e 6420 2a70 6172 7365  _xml* and *parse
+00001d00: 5f78 6d6c 5f74 6f5f 6172 7261 792a 3a0a  _xml_to_array*:.
+00001d10: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00001d20: 7079 6d61 7263 2069 6d70 6f72 7420 7061  pymarc import pa
+00001d30: 7273 655f 786d 6c5f 746f 5f61 7272 6179  rse_xml_to_array
+00001d40: 0a0a 7265 636f 7264 7320 3d20 7061 7273  ..records = pars
+00001d50: 655f 786d 6c5f 746f 5f61 7272 6179 286f  e_xml_to_array(o
+00001d60: 7065 6e28 2774 6573 742f 6261 7463 682e  pen('test/batch.
+00001d70: 786d 6c27 2929 0a60 6060 0a0a 2a2a 4a53  xml')).```..**JS
+00001d80: 4f4e 2a2a 0a0a 4a53 4f4e 2073 7570 706f  ON**..JSON suppo
+00001d90: 7274 2069 7320 6661 6972 6c79 206d 696e  rt is fairly min
+00001da0: 696d 616c 2069 6e20 7468 6174 2079 6f75  imal in that you
+00001db0: 2063 616e 2063 616c 6c20 6120 6070 796d   can call a `pym
+00001dc0: 6172 632e 5265 636f 7264 6027 730a 6061  arc.Record`'s.`a
+00001dd0: 735f 6a73 6f6e 2829 6020 6d65 7468 6f64  s_json()` method
+00001de0: 2074 6f20 7265 7475 726e 204a 534f 4e20   to return JSON 
+00001df0: 666f 7220 6120 6769 7665 6e20 4d41 5243  for a given MARC
+00001e00: 2052 6563 6f72 643a 0a0a 6060 6070 7974   Record:..```pyt
+00001e10: 686f 6e0a 6672 6f6d 2070 796d 6172 6320  hon.from pymarc 
+00001e20: 696d 706f 7274 204d 4152 4352 6561 6465  import MARCReade
+00001e30: 720a 0a77 6974 6820 6f70 656e 2827 7465  r..with open('te
+00001e40: 7374 2f6f 6e65 2e64 6174 272c 2772 6227  st/one.dat','rb'
+00001e50: 2920 6173 2066 683a 0a20 2020 2072 6561  ) as fh:.    rea
+00001e60: 6465 7220 3d20 4d41 5243 5265 6164 6572  der = MARCReader
+00001e70: 2866 6829 0a20 2020 2066 6f72 2072 6563  (fh).    for rec
+00001e80: 6f72 6420 696e 2072 6561 6465 723a 0a20  ord in reader:. 
+00001e90: 2020 2020 2020 2070 7269 6e74 2872 6563         print(rec
+00001ea0: 6f72 642e 6173 5f6a 736f 6e28 696e 6465  ord.as_json(inde
+00001eb0: 6e74 3d32 2929 0a60 6060 0a0a 6060 606a  nt=2)).```..```j
+00001ec0: 736f 6e0a 7b0a 2020 226c 6561 6465 7222  son.{.  "leader"
+00001ed0: 3a20 2230 3130 3630 6361 6d20 2032 3230  : "01060cam  220
+00001ee0: 3032 3839 3461 2034 3530 3022 2c0a 2020  02894a 4500",.  
+00001ef0: 2266 6965 6c64 7322 3a20 5b0a 2020 2020  "fields": [.    
+00001f00: 7b0a 2020 2020 2020 2230 3031 223a 2022  {.      "001": "
+00001f10: 3131 3737 3835 3034 220a 2020 2020 7d2c  11778504".    },
+00001f20: 0a20 2020 207b 0a20 2020 2020 2022 3031  .    {.      "01
+00001f30: 3022 3a20 7b0a 2020 2020 2020 2020 2269  0": {.        "i
+00001f40: 6e64 3122 3a20 2220 222c 0a20 2020 2020  nd1": " ",.     
+00001f50: 2020 2022 7375 6266 6965 6c64 7322 3a20     "subfields": 
+00001f60: 5b0a 2020 2020 2020 2020 2020 7b0a 2020  [.          {.  
+00001f70: 2020 2020 2020 2020 2020 2261 223a 2022            "a": "
+00001f80: 2020 2039 3930 3433 3538 3120 220a 2020     99043581 ".  
+00001f90: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00001fa0: 2020 5d2c 0a20 2020 2020 2020 2022 696e    ],.        "in
+00001fb0: 6432 223a 2022 2022 0a20 2020 2020 207d  d2": " ".      }
+00001fc0: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
+00001fd0: 2020 2020 2231 3030 223a 207b 0a20 2020      "100": {.   
+00001fe0: 2020 2020 2022 696e 6431 223a 2022 3122       "ind1": "1"
+00001ff0: 2c0a 2020 2020 2020 2020 2273 7562 6669  ,.        "subfi
+00002000: 656c 6473 223a 205b 0a20 2020 2020 2020  elds": [.       
+00002010: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00002020: 2022 6122 3a20 2248 756e 742c 2041 6e64   "a": "Hunt, And
+00002030: 7265 772c 220a 2020 2020 2020 2020 2020  rew,".          
+00002040: 7d2c 0a20 2020 2020 2020 2020 207b 0a20  },.          {. 
+00002050: 2020 2020 2020 2020 2020 2022 6422 3a20             "d": 
+00002060: 2231 3936 342d 220a 2020 2020 2020 2020  "1964-".        
+00002070: 2020 7d0a 2020 2020 2020 2020 5d2c 0a20    }.        ],. 
+00002080: 2020 2020 2020 2022 696e 6432 223a 2022         "ind2": "
+00002090: 2022 0a20 2020 2020 207d 0a20 2020 207d   ".      }.    }
+000020a0: 2c0a 2020 2020 7b0a 2020 2020 2020 2232  ,.    {.      "2
+000020b0: 3435 223a 207b 0a20 2020 2020 2020 2022  45": {.        "
+000020c0: 696e 6431 223a 2022 3122 2c0a 2020 2020  ind1": "1",.    
+000020d0: 2020 2020 2273 7562 6669 656c 6473 223a      "subfields":
+000020e0: 205b 0a20 2020 2020 2020 2020 207b 0a20   [.          {. 
+000020f0: 2020 2020 2020 2020 2020 2022 6122 3a20             "a": 
+00002100: 2254 6865 2070 7261 676d 6174 6963 2070  "The pragmatic p
+00002110: 726f 6772 616d 6d65 7220 3a22 0a20 2020  rogrammer :".   
+00002120: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00002130: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00002140: 2020 2262 223a 2022 6672 6f6d 206a 6f75    "b": "from jou
+00002150: 726e 6579 6d61 6e20 746f 206d 6173 7465  rneyman to maste
+00002160: 7220 2f22 0a20 2020 2020 2020 2020 207d  r /".          }
+00002170: 2c0a 2020 2020 2020 2020 2020 7b0a 2020  ,.          {.  
+00002180: 2020 2020 2020 2020 2020 2263 223a 2022            "c": "
+00002190: 416e 6472 6577 2048 756e 742c 2044 6176  Andrew Hunt, Dav
+000021a0: 6964 2054 686f 6d61 732e 220a 2020 2020  id Thomas.".    
+000021b0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000021c0: 5d2c 0a20 2020 2020 2020 2022 696e 6432  ],.        "ind2
+000021d0: 223a 2022 3422 0a20 2020 2020 207d 0a20  ": "4".      }. 
+000021e0: 2020 207d 2c0a 2020 2020 7b0a 2020 2020     },.    {.    
+000021f0: 2020 2232 3630 223a 207b 0a20 2020 2020    "260": {.     
+00002200: 2020 2022 696e 6431 223a 2022 2022 2c0a     "ind1": " ",.
+00002210: 2020 2020 2020 2020 2273 7562 6669 656c          "subfiel
+00002220: 6473 223a 205b 0a20 2020 2020 2020 2020  ds": [.         
+00002230: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00002240: 6122 3a20 2252 6561 6469 6e67 2c20 4d61  a": "Reading, Ma
+00002250: 7373 203a 220a 2020 2020 2020 2020 2020  ss :".          
+00002260: 7d2c 0a20 2020 2020 2020 2020 207b 0a20  },.          {. 
+00002270: 2020 2020 2020 2020 2020 2022 6222 3a20             "b": 
+00002280: 2241 6464 6973 6f6e 2d57 6573 6c65 792c  "Addison-Wesley,
+00002290: 220a 2020 2020 2020 2020 2020 7d2c 0a20  ".          },. 
+000022a0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+000022b0: 2020 2020 2020 2022 6322 3a20 2232 3030         "c": "200
+000022c0: 302e 220a 2020 2020 2020 2020 2020 7d0a  0.".          }.
+000022d0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+000022e0: 2020 2022 696e 6432 223a 2022 2022 0a20     "ind2": " ". 
+000022f0: 2020 2020 207d 0a20 2020 207d 2c0a 2020       }.    },.  
+00002300: 2020 7b0a 2020 2020 2020 2233 3030 223a    {.      "300":
+00002310: 207b 0a20 2020 2020 2020 2022 696e 6431   {.        "ind1
+00002320: 223a 2022 2022 2c0a 2020 2020 2020 2020  ": " ",.        
+00002330: 2273 7562 6669 656c 6473 223a 205b 0a20  "subfields": [. 
+00002340: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00002350: 2020 2020 2020 2022 6122 3a20 2278 7869         "a": "xxi
+00002360: 762c 2033 3231 2070 2e20 3b22 0a20 2020  v, 321 p. ;".   
+00002370: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00002380: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00002390: 2020 2263 223a 2022 3234 2063 6d2e 220a    "c": "24 cm.".
+000023a0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+000023b0: 2020 2020 5d2c 0a20 2020 2020 2020 2022      ],.        "
+000023c0: 696e 6432 223a 2022 2022 0a20 2020 2020  ind2": " ".     
+000023d0: 207d 0a20 2020 207d 2c0a 2020 2020 7b0a   }.    },.    {.
+000023e0: 2020 2020 2020 2235 3034 223a 207b 0a20        "504": {. 
+000023f0: 2020 2020 2020 2022 696e 6431 223a 2022         "ind1": "
+00002400: 2022 2c0a 2020 2020 2020 2020 2273 7562   ",.        "sub
+00002410: 6669 656c 6473 223a 205b 0a20 2020 2020  fields": [.     
+00002420: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00002430: 2020 2022 6122 3a20 2249 6e63 6c75 6465     "a": "Include
+00002440: 7320 6269 626c 696f 6772 6170 6869 6361  s bibliographica
+00002450: 6c20 7265 6665 7265 6e63 6573 2e22 0a20  l references.". 
+00002460: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00002470: 2020 205d 2c0a 2020 2020 2020 2020 2269     ],.        "i
+00002480: 6e64 3222 3a20 2220 220a 2020 2020 2020  nd2": " ".      
+00002490: 7d0a 2020 2020 7d2c 0a20 2020 207b 0a20  }.    },.    {. 
+000024a0: 2020 2020 2022 3635 3022 3a20 7b0a 2020       "650": {.  
+000024b0: 2020 2020 2020 2269 6e64 3122 3a20 2220        "ind1": " 
+000024c0: 222c 0a20 2020 2020 2020 2022 7375 6266  ",.        "subf
+000024d0: 6965 6c64 7322 3a20 5b0a 2020 2020 2020  ields": [.      
+000024e0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+000024f0: 2020 2261 223a 2022 436f 6d70 7574 6572    "a": "Computer
+00002500: 2070 726f 6772 616d 6d69 6e67 2e22 0a20   programming.". 
+00002510: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00002520: 2020 205d 2c0a 2020 2020 2020 2020 2269     ],.        "i
+00002530: 6e64 3222 3a20 2230 220a 2020 2020 2020  nd2": "0".      
+00002540: 7d0a 2020 2020 7d2c 0a20 2020 207b 0a20  }.    },.    {. 
+00002550: 2020 2020 2022 3730 3022 3a20 7b0a 2020       "700": {.  
+00002560: 2020 2020 2020 2269 6e64 3122 3a20 2231        "ind1": "1
+00002570: 222c 0a20 2020 2020 2020 2022 7375 6266  ",.        "subf
+00002580: 6965 6c64 7322 3a20 5b0a 2020 2020 2020  ields": [.      
+00002590: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+000025a0: 2020 2261 223a 2022 5468 6f6d 6173 2c20    "a": "Thomas, 
+000025b0: 4461 7669 642c 220a 2020 2020 2020 2020  David,".        
+000025c0: 2020 7d2c 0a20 2020 2020 2020 2020 207b    },.          {
+000025d0: 0a20 2020 2020 2020 2020 2020 2022 6422  .            "d"
+000025e0: 3a20 2231 3935 362d 220a 2020 2020 2020  : "1956-".      
+000025f0: 2020 2020 7d0a 2020 2020 2020 2020 5d2c      }.        ],
+00002600: 0a20 2020 2020 2020 2022 696e 6432 223a  .        "ind2":
+00002610: 2022 2022 0a20 2020 2020 207d 0a20 2020   " ".      }.   
+00002620: 207d 0a20 205d 0a7d 0a60 6060 0a0a 4966   }.  ].}.```..If
+00002630: 2079 6f75 2077 616e 7420 746f 2070 6172   you want to par
+00002640: 7365 2061 2066 696c 6520 6f66 204d 4152  se a file of MAR
+00002650: 434a 534f 4e20 7265 636f 7264 7320 796f  CJSON records yo
+00002660: 7520 6361 6e3a 0a0a 6060 6070 7974 686f  u can:..```pytho
+00002670: 6e0a 6672 6f6d 2070 796d 6172 6320 696d  n.from pymarc im
+00002680: 706f 7274 2070 6172 7365 5f6a 736f 6e5f  port parse_json_
+00002690: 746f 5f61 7272 6179 0a0a 7265 636f 7264  to_array..record
+000026a0: 7320 3d20 7061 7273 655f 6a73 6f6e 5f74  s = parse_json_t
+000026b0: 6f5f 6172 7261 7928 6f70 656e 2827 7465  o_array(open('te
+000026c0: 7374 2f62 6174 6368 2e6a 736f 6e27 2929  st/batch.json'))
+000026d0: 0a0a 7072 696e 7428 7265 636f 7264 735b  ..print(records[
+000026e0: 305d 290a 6060 600a 0a60 6060 0a3d 4c44  0]).```..```.=LD
+000026f0: 5220 2030 3039 3235 6e6a 6d20 2032 3230  R  00925njm  220
+00002700: 3032 3737 3761 2034 3530 300a 3d30 3031  02777a 4500.=001
+00002710: 2020 3536 3337 3234 310a 3d30 3033 2020    5637241.=003  
+00002720: 444c 430a 3d30 3035 2020 3139 3932 3038  DLC.=005  199208
+00002730: 3236 3038 3430 3336 2e30 0a3d 3030 3720  26084036.0.=007 
+00002740: 2073 6475 6275 6d65 6e6e 6d70 6c75 0a3d   sdubumennmplu.=
+00002750: 3030 3820 2039 3130 3932 3673 3139 3537  008  910926s1957
+00002760: 5c5c 5c5c 6e79 7575 756e 5c5c 5c5c 5c5c  \\\\nyuuun\\\\\\
+00002770: 5c5c 5c5c 5c5c 5c5c 656e 675c 5c0a 3d30  \\\\\\\\eng\\.=0
+00002780: 3130 2020 5c5c 2461 2020 2039 3137 3538  10  \\$a   91758
+00002790: 3333 350a 3d30 3238 2020 3030 2461 3132  335.=028  00$a12
+000027a0: 3539 2462 4174 6c61 6e74 6963 0a3d 3034  59$bAtlantic.=04
+000027b0: 3020 205c 5c24 6144 4c43 2463 444c 430a  0  \\$aDLC$cDLC.
+000027c0: 3d30 3530 2020 3030 2461 4174 6c61 6e74  =050  00$aAtlant
+000027d0: 6963 2031 3235 390a 3d32 3435 2020 3034  ic 1259.=245  04
+000027e0: 2461 5468 6520 4772 6561 7420 5261 7920  $aThe Great Ray 
+000027f0: 4368 6172 6c65 7324 685b 736f 756e 6420  Charles$h[sound 
+00002800: 7265 636f 7264 696e 675d 2e0a 3d32 3630  recording]..=260
+00002810: 2020 5c5c 2461 4e65 7720 596f 726b 2c20    \\$aNew York, 
+00002820: 4e2e 592e 203a 2462 4174 6c61 6e74 6963  N.Y. :$bAtlantic
+00002830: 2c24 635b 3139 3537 3f5d 0a3d 3330 3020  ,$c[1957?].=300 
+00002840: 205c 5c24 6131 2073 6f75 6e64 2064 6973   \\$a1 sound dis
+00002850: 6320 3a24 6261 6e61 6c6f 672c 2033 3320  c :$banalog, 33 
+00002860: 312f 3320 7270 6d20 3b24 6331 3220 696e  1/3 rpm ;$c12 in
+00002870: 2e0a 3d35 3131 2020 305c 2461 5261 7920  ..=511  0\$aRay 
+00002880: 4368 6172 6c65 732c 2070 6961 6e6f 2026  Charles, piano &
+00002890: 2063 656c 6573 7465 2e0a 3d35 3035 2020   celeste..=505  
+000028a0: 305c 2461 5468 6520 5261 7920 2d2d 204d  0\$aThe Ray -- M
+000028b0: 7920 6d65 6c61 6e63 686f 6c79 2062 6162  y melancholy bab
+000028c0: 7920 2d2d 2042 6c61 636b 2063 6f66 6665  y -- Black coffe
+000028d0: 6520 2d2d 2054 6865 7265 2773 206e 6f20  e -- There's no 
+000028e0: 796f 7520 2d2d 2044 6f6f 646c 696e 2720  you -- Doodlin' 
+000028f0: 2d2d 2053 7765 6574 2073 6978 7465 656e  -- Sweet sixteen
+00002900: 2062 6172 7320 2d2d 2049 2073 7572 7265   bars -- I surre
+00002910: 6e64 6572 2064 6561 7220 2d2d 2055 6e64  nder dear -- Und
+00002920: 6563 6964 6564 2e0a 3d35 3030 2020 5c5c  ecided..=500  \\
+00002930: 2461 4272 6965 6620 7265 636f 7264 2e0a  $aBrief record..
+00002940: 3d36 3530 2020 5c30 2461 4a61 7a7a 2479  =650  \0$aJazz$y
+00002950: 3139 3531 2d31 3936 302e 0a3d 3635 3020  1951-1960..=650 
+00002960: 205c 3024 6150 6961 6e6f 2077 6974 6820   \0$aPiano with 
+00002970: 6a61 7a7a 2065 6e73 656d 626c 652e 0a3d  jazz ensemble..=
+00002980: 3730 3020 2031 5c24 6143 6861 726c 6573  700  1\$aCharles
+00002990: 2c20 5261 792c 2464 3139 3330 2d24 3470  , Ray,$d1930-$4p
+000029a0: 7266 0a60 6060 0a0a 5375 7070 6f72 740a  rf.```..Support.
+000029b0: 2d2d 2d2d 2d2d 2d0a 0a54 6865 2070 796d  -------..The pym
+000029c0: 6172 6320 6465 7665 6c6f 7065 7273 2065  arc developers e
+000029d0: 6e63 6f75 7261 6765 2079 6f75 2074 6f20  ncourage you to 
+000029e0: 6a6f 696e 2074 6865 205b 7079 6d61 7263  join the [pymarc
+000029f0: 2047 6f6f 676c 650a 4772 6f75 705d 2868   Google.Group](h
+00002a00: 7474 703a 2f2f 6772 6f75 7073 2e67 6f6f  ttp://groups.goo
+00002a10: 676c 652e 636f 6d2f 6772 6f75 702f 7079  gle.com/group/py
+00002a20: 6d61 7263 2920 6966 2079 6f75 206e 6565  marc) if you nee
+00002a30: 6420 6865 6c70 2e20 2041 6c73 6f2c 2070  d help.  Also, p
+00002a40: 6c65 6173 650a 6665 656c 2066 7265 6520  lease.feel free 
+00002a50: 746f 2075 7365 205b 6973 7375 6520 7472  to use [issue tr
+00002a60: 6163 6b69 6e67 5d28 6874 7470 733a 2f2f  acking](https://
+00002a70: 6769 746c 6162 2e63 6f6d 2f70 796d 6172  gitlab.com/pymar
+00002a80: 632f 7079 6d61 7263 2f69 7373 7565 7329  c/pymarc/issues)
+00002a90: 206f 6e0a 4769 744c 6162 2074 6f20 7375   on.GitLab to su
+00002aa0: 626d 6974 2066 6561 7475 7265 2072 6571  bmit feature req
+00002ab0: 7565 7374 7320 6f72 2062 7567 2072 6570  uests or bug rep
+00002ac0: 6f72 7473 2e20 4966 2079 6f75 2776 6520  orts. If you've 
+00002ad0: 676f 7420 616e 2069 7463 6820 746f 0a73  got an itch to.s
+00002ae0: 6372 6174 6368 2c20 706c 6561 7365 2073  cratch, please s
+00002af0: 6372 6174 6368 2069 742c 2061 6e64 2073  cratch it, and s
+00002b00: 656e 6420 6d65 7267 6520 7265 7175 6573  end merge reques
+00002b10: 7473 206f 6e0a 5b47 6974 4c61 625d 2868  ts on.[GitLab](h
+00002b20: 7474 703a 2f2f 6769 746c 6162 2e63 6f6d  ttp://gitlab.com
+00002b30: 2f70 796d 6172 632f 7079 6d61 7263 292e  /pymarc/pymarc).
+00002b40: 0a0a 4966 2079 6f75 2073 7461 7274 2077  ..If you start w
+00002b50: 6f72 6b69 6e67 2077 6974 6820 4d41 5243  orking with MARC
+00002b60: 2079 6f75 206d 6179 2066 6565 6c20 6c69   you may feel li
+00002b70: 6b65 2079 6f75 206e 6565 6420 6d6f 7261  ke you need mora
+00002b80: 6c20 7375 7070 6f72 740a 696e 2061 6464  l support.in add
+00002b90: 6974 696f 6e20 746f 2074 6563 686e 6963  ition to technic
+00002ba0: 616c 2073 7570 706f 7274 2e20 5468 650a  al support. The.
+00002bb0: 5b23 636f 6465 346c 6962 5d28 6972 6373  [#code4lib](ircs
+00002bc0: 3a2f 2f69 7263 2e6c 6962 6572 612e 6368  ://irc.libera.ch
+00002bd0: 6174 2f63 6f64 6534 6c69 6229 2063 6861  at/code4lib) cha
+00002be0: 6e6e 656c 206f 6e20 5b4c 6962 6572 615d  nnel on [Libera]
+00002bf0: 2868 7474 7073 3a2f 2f6c 6962 6572 612e  (https://libera.
+00002c00: 6368 6174 2f29 2069 7320 6120 676f 6f64  chat/) is a good
+00002c10: 2070 6c61 6365 2066 6f72 2062 6f74 682e   place for both.
+00002c20: 0a                                       .
```

### Comparing `pymarc-5.0.0/README_pt_Br.md` & `pymarc-5.1.0/README_pt_Br.md`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/docs/source/conf.py` & `pymarc-5.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/docs/source/index.rst` & `pymarc-5.1.0/docs/source/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 .. code-block:: python
 
     from pymarc import MARCReader
 
     with open('test/marc.dat', 'rb') as fh:
         reader = MARCReader(fh)
         for record in reader:
-            print(record.title())
+            print(record.title)
 
     The pragmatic programmer : from journeyman to master /
     Programming Python /
     Learning Python /
     Python cookbook /
     Python programming for the absolute beginner /
     Web programming : techniques for integrating Python, Linux, Apache, and MySQL /
@@ -75,15 +75,15 @@
     from pymarc import exceptions as exc
 
     with open('test/marc.dat', 'rb') as fh:
         reader = MARCReader(fh)
         for record in reader:
             if record:
                 # consume the record:
-                print(record.title())
+                print(record.title)
             elif isinstance(reader.current_exception, exc.FatalReaderError):
                 # data file format error
                 # reader will raise StopIteration
                 print(reader.current_exception)
                 print(reader.current_chunk)
             else:
                 # fix the record data, skip or stop reading:
@@ -92,22 +92,22 @@
                 # break/continue/raise
 
 `FatalReaderError` happens when reader can't determine record's boundaries in
 the data stream. To avoid data misinterpretation it stops.
 In case of other errors (wrong encodind etc.) reader continues to
 the next record.
 
-A pymarc.Record object has a few handy methods like title for
-getting at bits of a bibliographic record, others include: author,
-isbn, subjects, location, notes, physical description, publisher,
-pubyear. But really, to work with MARC data you need to understand the
+A `pymarc.Record` object has a few handy properties like `title` for
+getting at bits of a bibliographic record, others include: `author`,
+`isbn`, `subjects`, `location`, `notes`, `physicaldescription`, `publisher`,
+`pubyear`. But really, to work with MARC data you need to understand the
 numeric field tags and subfield codes that are used to designate
 various bits of information. There is a lot more hiding in a MARC
-record than these methods provide access to. For example the title
-method extracts the information from the 245 field, subfields a and b.
+record than these properties provide access to. For example the title
+property extracts the information from the 245 field, subfields a and b.
 You can access `245a` like so:
 
 .. code-block:: python
 
     print(record['245']['a'])
 
 Some fields like subjects can repeat. In cases like that you will want
```

### Comparing `pymarc-5.0.0/pymarc/__init__.py` & `pymarc-5.1.0/pymarc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/pymarc/exceptions.py` & `pymarc-5.1.0/pymarc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/pymarc/field.py` & `pymarc-5.1.0/pymarc/field.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/pymarc/leader.py` & `pymarc-5.1.0/pymarc/leader.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/pymarc/marc8.py` & `pymarc-5.1.0/pymarc/marc8.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,19 +129,26 @@
 
             def is_multibyte(charset):
                 return charset == 0x31
 
             mb_flag = is_multibyte(self.g0)
 
             if mb_flag:
-                code_point = (
-                    ord(marc8_string[pos : pos + 1]) * 65536
-                    + ord(marc8_string[pos + 1 : pos + 2]) * 256
-                    + ord(marc8_string[pos + 2 : pos + 3])
-                )
+                # conditional check if string longer than pos+3 because of malformed marc8 string
+                if len(marc8_string) < pos + 3:
+                    sys.stderr.write(
+                        f"Multi-byte position {pos+3} exceeds length of marc8 string {len(marc8_string)}\n"
+                    )
+                    code_point = 32  # Sets last character as a blank string
+                else:
+                    code_point = (
+                        ord(marc8_string[pos : pos + 1]) * 65536
+                        + ord(marc8_string[pos + 1 : pos + 2]) * 256
+                        + ord(marc8_string[pos + 2 : pos + 3])
+                    )
                 pos += 3
             else:
                 code_point = ord(marc8_string[pos : pos + 1])
                 pos += 1
 
             if code_point < 0x20 or 0x80 < code_point < 0xA0:
                 uni = chr(code_point)
```

### Comparing `pymarc-5.0.0/pymarc/marc8_mapping.py` & `pymarc-5.1.0/pymarc/marc8_mapping.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/pymarc/marcjson.py` & `pymarc-5.1.0/pymarc/marcjson.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/pymarc/marcxml.py` & `pymarc-5.1.0/pymarc/marcxml.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/pymarc/reader.py` & `pymarc-5.1.0/pymarc/reader.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/pymarc/record.py` & `pymarc-5.1.0/pymarc/record.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/pymarc/writer.py` & `pymarc-5.1.0/pymarc/writer.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/pymarc.egg-info/PKG-INFO` & `pymarc-5.1.0/pymarc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pymarc
-Version: 5.0.0
+Version: 5.1.0
 Summary: Read, write and modify MARC bibliographic data
 Home-page: http://gitlab.com/pymarc/pymarc
 Author: Ed Summers
 Author-email: ehs@pobox.com
 License: http://www.opensource.org/licenses/bsd-license.php
+Platform: UNKNOWN
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -126,28 +127,29 @@
 ```python
 for f in record.get_fields('650'):
     print(f)
 ```
 
 If you are new to MARC fields [Understanding
 MARC](http://www.loc.gov/marc/umb/) is a pretty good primer, and the [MARC 21
-Formats](http://www.loc.gov/marc/marcdocz.html) page at the Library of Congress is a good reference once you understand the basics.
+Formats](http://www.loc.gov/marc/marcdocz.html) page at the Library of Congress 
+is a good reference once you understand the basics.
 
 ### Writing
 
 *Note: As of v5.0.0 `Subfield` is used to create subfields. Prior to v5,
 subfields were constructed and accessed as a list of strings, e.g., `[code,
 value, code, value]`. In v5.0.0 this has been changed to organize the subfields
 into a list of tuples, e.g., `[(code, value), (code, value)]`. The `Subfield`
 is implemented as a `NamedTuple` so that the tuples can be constructed as
 `Subfield(code=code, value=value)`. The old style of creating subfields is no
 longer supported. Attempting to pass a list of strings to the `subfields`
 parameter for the `Field` constructor will raise a `ValueError`. For
-convenience the `Field.convert_legacy_subfields` can be used to convert a
-legacy list of strings into a list of `Subfield`s.*
+convenience the `Field.convert_legacy_subfields` class method can be used to 
+convert a legacy list of strings into a list of `Subfield`s.*
 
 Here's an example of creating a record and writing it out to a file.
 
 ```python
 from pymarc import Record, Field, Subfield
 
 record = Record()
@@ -217,15 +219,15 @@
 can:
 
 ```python
 
 from pymarc import map_xml
 
 def print_title(r):
-    print(r.title())
+    print(r.title)
 
 map_xml(print_title, 'test/batch.xml')
 ```
 
 Also, if you prefer you can pass in a file like object in addition to the path
 to both *map_xml* and *parse_xml_to_array*:
 
@@ -245,15 +247,15 @@
 
 with open('test/one.dat','rb') as fh:
     reader = MARCReader(fh)
     for record in reader:
         print(record.as_json(indent=2))
 ```
 
-```javascript
+```json
 {
   "leader": "01060cam  22002894a 4500",
   "fields": [
     {
       "001": "11778504"
     },
     {
@@ -410,7 +412,9 @@
 GitLab to submit feature requests or bug reports. If you've got an itch to
 scratch, please scratch it, and send merge requests on
 [GitLab](http://gitlab.com/pymarc/pymarc).
 
 If you start working with MARC you may feel like you need moral support
 in addition to technical support. The
 [#code4lib](ircs://irc.libera.chat/code4lib) channel on [Libera](https://libera.chat/) is a good place for both.
+
+
```

### Comparing `pymarc-5.0.0/pymarc.egg-info/SOURCES.txt` & `pymarc-5.1.0/pymarc.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 README_pt_Br.md
-release.md
 requirements.dev.txt
 setup.cfg
 setup.py
 docs/source/conf.py
 docs/source/index.rst
 pymarc/__init__.py
 pymarc/constants.py
```

### Comparing `pymarc-5.0.0/setup.py` & `pymarc-5.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # propagated, or distributed according to the terms contained in the LICENSE
 # file.
 
 """Pymarc setup."""
 
 from setuptools import setup
 
-version = "5.0.0"
+version = "5.1.0"
 
 classifiers = """
 Intended Audience :: Education
 Intended Audience :: Developers
 Intended Audience :: Information Technology
 License :: OSI Approved :: BSD License
 Programming Language :: Python :: 3
```

### Comparing `pymarc-5.0.0/test/1251.dat` & `pymarc-5.1.0/test/1251.dat`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/alphatag.dat` & `pymarc-5.1.0/test/alphatag.dat`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/bad_eacc_encoding.dat` & `pymarc-5.1.0/test/bad_eacc_encoding.dat`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/bad_indicator.dat` & `pymarc-5.1.0/test/bad_indicator.dat`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/bad_marc8_escape.dat` & `pymarc-5.1.0/test/bad_marc8_escape.dat`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/bad_records.mrc` & `pymarc-5.1.0/test/bad_records.mrc`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/bad_subfield_code.dat` & `pymarc-5.1.0/test/bad_subfield_code.dat`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/bad_tag.xml` & `pymarc-5.1.0/test/bad_tag.xml`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/batch.json` & `pymarc-5.1.0/test/batch.json`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/batch.xml` & `pymarc-5.1.0/test/batch.xml`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/diacritic.dat` & `pymarc-5.1.0/test/diacritic.dat`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/marc.dat` & `pymarc-5.1.0/test/marc.dat`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/marc8-to-unicode.dat` & `pymarc-5.1.0/test/marc8-to-unicode.dat`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/marc8.dat` & `pymarc-5.1.0/test/marc8.dat`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/multi_isbn.dat` & `pymarc-5.1.0/test/multi_isbn.dat`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/one.dat` & `pymarc-5.1.0/test/one.dat`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/one.json` & `pymarc-5.1.0/test/one.json`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/regression45.dat` & `pymarc-5.1.0/test/regression45.dat`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/test.dat` & `pymarc-5.1.0/test/test.dat`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/test.json` & `pymarc-5.1.0/test/test.json`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/test_encode.py` & `pymarc-5.1.0/test/test_encode.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/test_field.py` & `pymarc-5.1.0/test/test_field.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/test_json.py` & `pymarc-5.1.0/test/test_json.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/test_leader.py` & `pymarc-5.1.0/test/test_leader.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/test_marc8.py` & `pymarc-5.1.0/test/test_marc8.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,20 +63,16 @@
             except AssertionError:
                 self.assertTrue("Was enable to decode invalid MARC")
 
     def test_marc8_reader_to_unicode_bad_eacc_sequence(self):
         with open("test/bad_eacc_encoding.dat", "rb") as fh:
             reader = MARCReader(fh, to_unicode=True, hide_utf8_warnings=True)
             record = next(reader)
-            self.assertIsNone(record, "Was able to decode invalid MARC8")
-            self.assertIsInstance(
-                reader.current_exception,
-                UnicodeDecodeError,
-                "Caught UnicodeDecodeError as expected",
-            )
+            self.assertEqual(len(record["880"]["a"]), 12)
+            self.assertTrue(record["880"]["a"].endswith(" "))
 
     def test_marc8_reader_to_unicode_bad_escape(self):
         with open("test/bad_marc8_escape.dat", "rb") as fh:
             reader = MARCReader(fh, to_unicode=True)
             r = next(reader)
             self.assertEqual(type(r), Record)
             upublisher = r["260"]["b"]
```

### Comparing `pymarc-5.0.0/test/test_marc8.txt` & `pymarc-5.1.0/test/test_marc8.txt`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/test_ordered_fields.py` & `pymarc-5.1.0/test/test_ordered_fields.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/test_reader.py` & `pymarc-5.1.0/test/test_reader.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/test_record.py` & `pymarc-5.1.0/test/test_record.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/test_utf8.py` & `pymarc-5.1.0/test/test_utf8.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/test_utf8.txt` & `pymarc-5.1.0/test/test_utf8.txt`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/test_writer.py` & `pymarc-5.1.0/test/test_writer.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/test_xml.py` & `pymarc-5.1.0/test/test_xml.py`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/testunimarc.dat` & `pymarc-5.1.0/test/testunimarc.dat`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/utf8.xml` & `pymarc-5.1.0/test/utf8.xml`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/utf8_errors.dat` & `pymarc-5.1.0/test/utf8_errors.dat`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/utf8_invalid.mrc` & `pymarc-5.1.0/test/utf8_invalid.mrc`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/utf8_with_leader_flag.dat` & `pymarc-5.1.0/test/utf8_with_leader_flag.dat`

 * *Files identical despite different names*

### Comparing `pymarc-5.0.0/test/utf8_without_leader_flag.dat` & `pymarc-5.1.0/test/utf8_without_leader_flag.dat`

 * *Files identical despite different names*

