# Comparing `tmp/cccconverter_ostrichb-0.90.0.tar.gz` & `tmp/cccconverter_ostrichb-0.90.1.tar.gz`

## Comparing `cccconverter_ostrichb-0.90.0.tar` & `cccconverter_ostrichb-0.90.1.tar`

### file list

```diff
@@ -1,21 +1,15 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/.idea/CCCConverter.iml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/.idea/misc.xml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/.idea/vcs.xml
--rw-r--r--   0        0        0    10446 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/.idea/workspace.xml
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/src/convert_dict.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/src/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/src/ccccoverter/__init__.py
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/src/ccccoverter/convert.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/src/ccccoverter/parse_dict.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/src/ccccoverter/spilt.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/src/dict/finals.csv
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/src/dict/initials.csv
--rw-r--r--   0        0        0   276837 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/src/dict/yuet_dict.csv
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/.gitignore
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/pyproject.toml
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/.DS_Store
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/convert_dict.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/cccconverter/__init__.py
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/cccconverter/convert.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/cccconverter/parse_dict.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/cccconverter/spilt.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/dict/finals.csv
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/dict/initials.csv
+-rw-r--r--   0        0        0   276837 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/dict/yuet_dict.csv
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/LICENSE.txt
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/README.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/pyproject.toml
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/PKG-INFO
```

### Comparing `cccconverter_ostrichb-0.90.0/src/convert_dict.py` & `cccconverter_ostrichb-0.90.1/src/convert_dict.py`

 * *Files identical despite different names*

### Comparing `cccconverter_ostrichb-0.90.0/src/test.py` & `cccconverter_ostrichb-0.90.1/src/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from ccccoverter.convert import *
+from cccconverter.convert import *
 
 
 class TestConvert(unittest.TestCase):
     def test_convert_single_syllable(self):
         self.assertEqual(convert_single_syllable('jung'), ['yung', 'yong'])
 
     def test_convert_single_character(self):
```

### Comparing `cccconverter_ostrichb-0.90.0/src/ccccoverter/convert.py` & `cccconverter_ostrichb-0.90.1/src/cccconverter/convert.py`

 * *Files identical despite different names*

### Comparing `cccconverter_ostrichb-0.90.0/src/ccccoverter/parse_dict.py` & `cccconverter_ostrichb-0.90.1/src/cccconverter/parse_dict.py`

 * *Files identical despite different names*

### Comparing `cccconverter_ostrichb-0.90.0/src/ccccoverter/spilt.py` & `cccconverter_ostrichb-0.90.1/src/cccconverter/spilt.py`

 * *Files identical despite different names*

### Comparing `cccconverter_ostrichb-0.90.0/src/dict/yuet_dict.csv` & `cccconverter_ostrichb-0.90.1/src/dict/yuet_dict.csv`

 * *Files identical despite different names*

### Comparing `cccconverter_ostrichb-0.90.0/.gitignore` & `cccconverter_ostrichb-0.90.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -134,7 +134,8 @@
 
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 
+.idea/
```

### Comparing `cccconverter_ostrichb-0.90.0/README.md` & `cccconverter_ostrichb-0.90.1/README.md`

 * *Files identical despite different names*

### Comparing `cccconverter_ostrichb-0.90.0/pyproject.toml` & `cccconverter_ostrichb-0.90.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
+[tool.hatch.build.targets.wheel]
+only-include = ["src/cccconverter", "src/dict"]
+
+
 [project]
 name = "cccconverter_ostrichb"
-version = "0.90.0"
+version = "0.90.1"
 authors = [
   { name="Ostrichbeta Chan", email="ostrichb@yandex.com" },
 ]
 description = "A Hong Kong Government Cantonese Romanisation converter"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cccconverter_ostrichb-0.90.0/PKG-INFO` & `cccconverter_ostrichb-0.90.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: cccconverter_ostrichb
-Version: 0.90.0
+Version: 0.90.1
 Summary: A Hong Kong Government Cantonese Romanisation converter
 Project-URL: Homepage, https://github.com/Ostrichbeta/CCCConverter
 Project-URL: Bug Tracker, https://github.com/Ostrichbeta/CCCConverterissues
 Author-email: Ostrichbeta Chan <ostrichb@yandex.com>
+License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # CCCConverter
```

