# Comparing `tmp/cccconverter_ostrichb-0.90.1.tar.gz` & `tmp/cccconverter_ostrichb-0.90.2.tar.gz`

## Comparing `cccconverter_ostrichb-0.90.1.tar` & `cccconverter_ostrichb-0.90.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/.DS_Store
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/convert_dict.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/cccconverter/__init__.py
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/cccconverter/convert.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/cccconverter/parse_dict.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/cccconverter/spilt.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/dict/finals.csv
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/dict/initials.csv
--rw-r--r--   0        0        0   276837 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/src/dict/yuet_dict.csv
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/LICENSE.txt
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/README.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/pyproject.toml
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.1/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.2/.DS_Store
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.2/convert_dict.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.2/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.2/cccconverter/__init__.py
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.2/cccconverter/convert.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.2/cccconverter/parse_dict.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.2/cccconverter/spilt.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.2/cccconverter/dict/finals.csv
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.2/cccconverter/dict/initials.csv
+-rw-r--r--   0        0        0   276837 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.2/cccconverter/dict/yuet_dict.csv
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.2/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.2/LICENSE.txt
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.2/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.2/pyproject.toml
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 cccconverter_ostrichb-0.90.2/PKG-INFO
```

### Comparing `cccconverter_ostrichb-0.90.1/src/convert_dict.py` & `cccconverter_ostrichb-0.90.2/convert_dict.py`

 * *Files identical despite different names*

### Comparing `cccconverter_ostrichb-0.90.1/src/test.py` & `cccconverter_ostrichb-0.90.2/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import unittest
 from cccconverter.convert import *
+from cccconverter.parse_dict import *
 
 
 class TestConvert(unittest.TestCase):
     def test_convert_single_syllable(self):
         self.assertEqual(convert_single_syllable('jung'), ['yung', 'yong'])
 
     def test_convert_single_character(self):
@@ -25,9 +26,14 @@
                           ('雲', 'wan/wun/wen'),
                           ('山', 'shaan/shan/saan/san'),
                           ('子',
                            'tsz/tszi/tszu/tsi/tsee/chz/chzi/chzu/chi/chee||'
                            'chz/chzi/chzu/chi/chee/tsz/tszi/tszu/tsi/tsee')])
 
 
+class TestParseDict(unittest.TestCase):
+    def test_get_yuet_dict(self):
+        logging.info(get_yuet_dict())
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cccconverter_ostrichb-0.90.1/src/cccconverter/convert.py` & `cccconverter_ostrichb-0.90.2/cccconverter/convert.py`

 * *Files identical despite different names*

### Comparing `cccconverter_ostrichb-0.90.1/src/cccconverter/parse_dict.py` & `cccconverter_ostrichb-0.90.2/cccconverter/parse_dict.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import csv
 import pathlib
 
 
-dict_path = pathlib.Path(__file__).parent.parent.joinpath('dict')
+dict_path = pathlib.Path(__file__).parent.joinpath('dict')
 
 
 def get_initials_dict():
     """
     Get the all the initials of the Yuet-ping dictionary and convert it to a dictionary variable.
     :return: dict
     """
```

### Comparing `cccconverter_ostrichb-0.90.1/src/cccconverter/spilt.py` & `cccconverter_ostrichb-0.90.2/cccconverter/spilt.py`

 * *Files identical despite different names*

### Comparing `cccconverter_ostrichb-0.90.1/src/dict/yuet_dict.csv` & `cccconverter_ostrichb-0.90.2/cccconverter/dict/yuet_dict.csv`

 * *Files identical despite different names*

### Comparing `cccconverter_ostrichb-0.90.1/.gitignore` & `cccconverter_ostrichb-0.90.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cccconverter_ostrichb-0.90.1/LICENSE.txt` & `cccconverter_ostrichb-0.90.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cccconverter_ostrichb-0.90.1/README.md` & `cccconverter_ostrichb-0.90.2/README.md`

 * *Files identical despite different names*

### Comparing `cccconverter_ostrichb-0.90.1/pyproject.toml` & `cccconverter_ostrichb-0.90.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
+[tool.hatch.build]
+sources = ["src"]
+
 [tool.hatch.build.targets.wheel]
-only-include = ["src/cccconverter", "src/dict"]
+only-include = ["src/cccconverter"]
 
 
 [project]
 name = "cccconverter_ostrichb"
-version = "0.90.1"
+version = "0.90.2"
 authors = [
   { name="Ostrichbeta Chan", email="ostrichb@yandex.com" },
 ]
 description = "A Hong Kong Government Cantonese Romanisation converter"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cccconverter_ostrichb-0.90.1/PKG-INFO` & `cccconverter_ostrichb-0.90.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cccconverter_ostrichb
-Version: 0.90.1
+Version: 0.90.2
 Summary: A Hong Kong Government Cantonese Romanisation converter
 Project-URL: Homepage, https://github.com/Ostrichbeta/CCCConverter
 Project-URL: Bug Tracker, https://github.com/Ostrichbeta/CCCConverterissues
 Author-email: Ostrichbeta Chan <ostrichb@yandex.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

