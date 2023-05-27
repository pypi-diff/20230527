# Comparing `tmp/PyDAO_9000-1.1.tar.gz` & `tmp/PyDAO_9000-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDAO_9000-1.1.tar", last modified: Sat May 27 15:25:39 2023, max compression
+gzip compressed data, was "PyDAO_9000-1.2.tar", last modified: Sat May 27 15:57:40 2023, max compression
```

## Comparing `PyDAO_9000-1.1.tar` & `PyDAO_9000-1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 15:25:39.894575 PyDAO_9000-1.1/
--rw-rw-rw-   0        0        0     1090 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/LICENSE
--rw-rw-rw-   0        0        0     4210 2023-05-27 15:25:39.894575 PyDAO_9000-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-27 15:25:39.441457 PyDAO_9000-1.1/PyDAO_9000.egg-info/
--rw-rw-rw-   0        0        0     4210 2023-05-27 15:25:39.000000 PyDAO_9000-1.1/PyDAO_9000.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1040 2023-05-27 15:25:39.000000 PyDAO_9000-1.1/PyDAO_9000.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 15:25:39.000000 PyDAO_9000-1.1/PyDAO_9000.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-27 15:25:39.000000 PyDAO_9000-1.1/PyDAO_9000.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3696 2023-05-27 15:08:06.000000 PyDAO_9000-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 15:25:39.535198 PyDAO_9000-1.1/SqltDAO/
-drwxrwxrwx   0        0        0        0 2023-05-27 15:25:39.660199 PyDAO_9000-1.1/SqltDAO/CodeGen01/
--rw-rw-rw-   0        0        0     3108 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/CodeGen01/CodeGen.py
--rw-rw-rw-   0        0        0      865 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/CodeGen01/CodeLevel.py
--rw-rw-rw-   0        0        0      264 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/CodeGen01/DaoExceptions.py
--rw-rw-rw-   0        0        0      475 2023-05-27 15:22:37.000000 PyDAO_9000-1.1/SqltDAO/CodeGen01/Meta.py
--rw-rw-rw-   0        0        0     1816 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/CodeGen01/Normalizers.py
--rw-rw-rw-   0        0        0     4309 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/CodeGen01/OrderClass.py
--rw-rw-rw-   0        0        0    12389 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/CodeGen01/SqlSyntax.py
--rw-rw-rw-   0        0        0     7315 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/CodeGen01/TextDataDetector.py
--rw-rw-rw-   0        0        0    13912 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/CrudMeister.py
-drwxrwxrwx   0        0        0        0 2023-05-27 15:25:39.753944 PyDAO_9000-1.1/SqltDAO/DaoTest01/
--rw-rw-rw-   0        0        0      678 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/DaoTest01/GenNasdaq.py
--rw-rw-rw-   0        0        0      507 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/DaoTest01/GenNasdaqTest.py
--rw-rw-rw-   0        0        0     3252 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/DaoTest01/Income.py
--rw-rw-rw-   0        0        0     3054 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/DaoTest01/NasdaqDAO.py
--rw-rw-rw-   0        0        0     3488 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/DaoTest01/foo.py
--rw-rw-rw-   0        0        0      847 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/DaoTest01/tc001_driver.py
--rw-rw-rw-   0        0        0      691 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/DaoTest01/tc001_gen.py
--rw-rw-rw-   0        0        0     2923 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/Demo123.py
-drwxrwxrwx   0        0        0        0 2023-05-27 15:25:39.832072 PyDAO_9000-1.1/SqltDAO/Gui/
--rw-rw-rw-   0        0        0     6185 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/Gui/Data2Code.py
--rw-rw-rw-   0        0        0     6553 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/Gui/DataAI.py
--rw-rw-rw-   0        0        0     4628 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/Gui/DataFrameOne.py
--rw-rw-rw-   0        0        0     4892 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/Gui/DataPreferences.py
--rw-rw-rw-   0        0        0     4771 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/Gui/StandardEntry.py
--rw-rw-rw-   0        0        0     6403 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/Gui/TableDef.py
--rw-rw-rw-   0        0        0     3504 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/Ledger.py
-drwxrwxrwx   0        0        0        0 2023-05-27 15:25:39.894575 PyDAO_9000-1.1/SqltDAO/SchemaDef/
--rw-rw-rw-   0        0        0     8393 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/SchemaDef/DataDetective.py
--rw-rw-rw-   0        0        0     9378 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/SchemaDef/Factory.py
--rw-rw-rw-   0        0        0     8987 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/SchemaDef/OrderDef.py
--rw-rw-rw-   0        0        0     3179 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/SchemaDef/Table.py
--rw-rw-rw-   0        0        0     3602 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/UpdateTestCase.py
--rw-rw-rw-   0        0        0      103 2023-05-27 11:01:18.000000 PyDAO_9000-1.1/SqltDAO/__init__.py
--rw-rw-rw-   0        0        0     7759 2023-05-27 14:43:15.000000 PyDAO_9000-1.1/SqltDAO/main.py
--rw-rw-rw-   0        0        0      503 2023-05-27 15:23:10.000000 PyDAO_9000-1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 15:25:39.894575 PyDAO_9000-1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 15:57:40.155782 PyDAO_9000-1.2/
+-rw-rw-rw-   0        0        0     1090 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/LICENSE
+-rw-rw-rw-   0        0        0     4209 2023-05-27 15:57:40.155782 PyDAO_9000-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-27 15:57:40.030781 PyDAO_9000-1.2/PyDAO_9000.egg-info/
+-rw-rw-rw-   0        0        0     4209 2023-05-27 15:57:39.000000 PyDAO_9000-1.2/PyDAO_9000.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1040 2023-05-27 15:57:39.000000 PyDAO_9000-1.2/PyDAO_9000.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 15:57:39.000000 PyDAO_9000-1.2/PyDAO_9000.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-27 15:57:39.000000 PyDAO_9000-1.2/PyDAO_9000.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3695 2023-05-27 15:38:38.000000 PyDAO_9000-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 15:57:40.062030 PyDAO_9000-1.2/SqltDAO/
+drwxrwxrwx   0        0        0        0 2023-05-27 15:57:40.093280 PyDAO_9000-1.2/SqltDAO/CodeGen01/
+-rw-rw-rw-   0        0        0     3108 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/CodeGen01/CodeGen.py
+-rw-rw-rw-   0        0        0      865 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/CodeGen01/CodeLevel.py
+-rw-rw-rw-   0        0        0      264 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/CodeGen01/DaoExceptions.py
+-rw-rw-rw-   0        0        0      475 2023-05-27 15:22:37.000000 PyDAO_9000-1.2/SqltDAO/CodeGen01/Meta.py
+-rw-rw-rw-   0        0        0     1816 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/CodeGen01/Normalizers.py
+-rw-rw-rw-   0        0        0     4309 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/CodeGen01/OrderClass.py
+-rw-rw-rw-   0        0        0    12389 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/CodeGen01/SqlSyntax.py
+-rw-rw-rw-   0        0        0     7315 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/CodeGen01/TextDataDetector.py
+-rw-rw-rw-   0        0        0    13912 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/CrudMeister.py
+drwxrwxrwx   0        0        0        0 2023-05-27 15:57:40.108907 PyDAO_9000-1.2/SqltDAO/DaoTest01/
+-rw-rw-rw-   0        0        0      678 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/DaoTest01/GenNasdaq.py
+-rw-rw-rw-   0        0        0      507 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/DaoTest01/GenNasdaqTest.py
+-rw-rw-rw-   0        0        0     3252 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/DaoTest01/Income.py
+-rw-rw-rw-   0        0        0     3054 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/DaoTest01/NasdaqDAO.py
+-rw-rw-rw-   0        0        0     3488 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/DaoTest01/foo.py
+-rw-rw-rw-   0        0        0      847 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/DaoTest01/tc001_driver.py
+-rw-rw-rw-   0        0        0      691 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/DaoTest01/tc001_gen.py
+-rw-rw-rw-   0        0        0     2923 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/Demo123.py
+drwxrwxrwx   0        0        0        0 2023-05-27 15:57:40.140152 PyDAO_9000-1.2/SqltDAO/Gui/
+-rw-rw-rw-   0        0        0     6185 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/Gui/Data2Code.py
+-rw-rw-rw-   0        0        0     6553 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/Gui/DataAI.py
+-rw-rw-rw-   0        0        0     4628 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/Gui/DataFrameOne.py
+-rw-rw-rw-   0        0        0     4892 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/Gui/DataPreferences.py
+-rw-rw-rw-   0        0        0     4771 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/Gui/StandardEntry.py
+-rw-rw-rw-   0        0        0     6403 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/Gui/TableDef.py
+-rw-rw-rw-   0        0        0     3504 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/Ledger.py
+drwxrwxrwx   0        0        0        0 2023-05-27 15:57:40.140152 PyDAO_9000-1.2/SqltDAO/SchemaDef/
+-rw-rw-rw-   0        0        0     8393 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/SchemaDef/DataDetective.py
+-rw-rw-rw-   0        0        0     9378 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/SchemaDef/Factory.py
+-rw-rw-rw-   0        0        0     8987 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/SchemaDef/OrderDef.py
+-rw-rw-rw-   0        0        0     3179 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/SchemaDef/Table.py
+-rw-rw-rw-   0        0        0     3602 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/UpdateTestCase.py
+-rw-rw-rw-   0        0        0      103 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/__init__.py
+-rw-rw-rw-   0        0        0     7747 2023-05-27 15:38:24.000000 PyDAO_9000-1.2/SqltDAO/main.py
+-rw-rw-rw-   0        0        0      503 2023-05-27 15:52:15.000000 PyDAO_9000-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 15:57:40.155782 PyDAO_9000-1.2/setup.cfg
```

### Comparing `PyDAO_9000-1.1/LICENSE` & `PyDAO_9000-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/PKG-INFO` & `PyDAO_9000-1.2/PyDAO_9000.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: PyDAO_9000
-Version: 1.1
+Name: PyDAO-9000
+Version: 1.2
 Summary: All-In-One File SQL Code Generator
 Author-email: Randall Nagy <r.a.nagy@gmail.com>
 Project-URL: Homepage, https://github.com/soft9000/PyDAO
 Project-URL: Bug Tracker, https://github.com/soft9000/PyDAO/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -45,15 +45,15 @@
 Once installed most will probably want to use the GUI:
 
 ```
 >>> from SqltDAO import main as PyDAO
 >>> PyDAO.Main.mainloop()
 ```
 
-If you want to support the effort, fell free to purchase one of [our books on amazon](https://www.amazon.com/Randall-Nagy/e/B08ZJLH1VN) or [training opportunuties](https://www.udemy.com/user/randallnagy2/).
+If you want to support the effort feel free to purchase one of [our books on amazon](https://www.amazon.com/Randall-Nagy/e/B08ZJLH1VN) or [training opportunuties](https://www.udemy.com/user/randallnagy2/).
 
 PyDAO UI: https://github.com/soft9000/PyDAO/blob/master/SqltDAO/main.py
 
 
 API Example
 ------------
 For those who would rather create the DAO directly without needing a file full of data:
```

### Comparing `PyDAO_9000-1.1/PyDAO_9000.egg-info/PKG-INFO` & `PyDAO_9000-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: PyDAO-9000
-Version: 1.1
+Name: PyDAO_9000
+Version: 1.2
 Summary: All-In-One File SQL Code Generator
 Author-email: Randall Nagy <r.a.nagy@gmail.com>
 Project-URL: Homepage, https://github.com/soft9000/PyDAO
 Project-URL: Bug Tracker, https://github.com/soft9000/PyDAO/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -45,15 +45,15 @@
 Once installed most will probably want to use the GUI:
 
 ```
 >>> from SqltDAO import main as PyDAO
 >>> PyDAO.Main.mainloop()
 ```
 
-If you want to support the effort, fell free to purchase one of [our books on amazon](https://www.amazon.com/Randall-Nagy/e/B08ZJLH1VN) or [training opportunuties](https://www.udemy.com/user/randallnagy2/).
+If you want to support the effort feel free to purchase one of [our books on amazon](https://www.amazon.com/Randall-Nagy/e/B08ZJLH1VN) or [training opportunuties](https://www.udemy.com/user/randallnagy2/).
 
 PyDAO UI: https://github.com/soft9000/PyDAO/blob/master/SqltDAO/main.py
 
 
 API Example
 ------------
 For those who would rather create the DAO directly without needing a file full of data:
```

### Comparing `PyDAO_9000-1.1/PyDAO_9000.egg-info/SOURCES.txt` & `PyDAO_9000-1.2/PyDAO_9000.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/README.md` & `PyDAO_9000-1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Once installed most will probably want to use the GUI:
 
 ```
 >>> from SqltDAO import main as PyDAO
 >>> PyDAO.Main.mainloop()
 ```
 
-If you want to support the effort, fell free to purchase one of [our books on amazon](https://www.amazon.com/Randall-Nagy/e/B08ZJLH1VN) or [training opportunuties](https://www.udemy.com/user/randallnagy2/).
+If you want to support the effort feel free to purchase one of [our books on amazon](https://www.amazon.com/Randall-Nagy/e/B08ZJLH1VN) or [training opportunuties](https://www.udemy.com/user/randallnagy2/).
 
 PyDAO UI: https://github.com/soft9000/PyDAO/blob/master/SqltDAO/main.py
 
 
 API Example
 ------------
 For those who would rather create the DAO directly without needing a file full of data:
```

### Comparing `PyDAO_9000-1.1/SqltDAO/CodeGen01/CodeGen.py` & `PyDAO_9000-1.2/SqltDAO/CodeGen01/CodeGen.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/CodeGen01/CodeLevel.py` & `PyDAO_9000-1.2/SqltDAO/CodeGen01/CodeLevel.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/CodeGen01/Normalizers.py` & `PyDAO_9000-1.2/SqltDAO/CodeGen01/Normalizers.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/CodeGen01/OrderClass.py` & `PyDAO_9000-1.2/SqltDAO/CodeGen01/OrderClass.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/CodeGen01/SqlSyntax.py` & `PyDAO_9000-1.2/SqltDAO/CodeGen01/SqlSyntax.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/CodeGen01/TextDataDetector.py` & `PyDAO_9000-1.2/SqltDAO/CodeGen01/TextDataDetector.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/CrudMeister.py` & `PyDAO_9000-1.2/SqltDAO/CrudMeister.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/DaoTest01/GenNasdaq.py` & `PyDAO_9000-1.2/SqltDAO/DaoTest01/GenNasdaq.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/DaoTest01/Income.py` & `PyDAO_9000-1.2/SqltDAO/DaoTest01/Income.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/DaoTest01/NasdaqDAO.py` & `PyDAO_9000-1.2/SqltDAO/DaoTest01/NasdaqDAO.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/DaoTest01/foo.py` & `PyDAO_9000-1.2/SqltDAO/DaoTest01/foo.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/DaoTest01/tc001_driver.py` & `PyDAO_9000-1.2/SqltDAO/DaoTest01/tc001_driver.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/DaoTest01/tc001_gen.py` & `PyDAO_9000-1.2/SqltDAO/DaoTest01/tc001_gen.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/Demo123.py` & `PyDAO_9000-1.2/SqltDAO/Demo123.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/Gui/Data2Code.py` & `PyDAO_9000-1.2/SqltDAO/Gui/Data2Code.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/Gui/DataAI.py` & `PyDAO_9000-1.2/SqltDAO/Gui/DataAI.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/Gui/DataFrameOne.py` & `PyDAO_9000-1.2/SqltDAO/Gui/DataFrameOne.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/Gui/DataPreferences.py` & `PyDAO_9000-1.2/SqltDAO/Gui/DataPreferences.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/Gui/StandardEntry.py` & `PyDAO_9000-1.2/SqltDAO/Gui/StandardEntry.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/Gui/TableDef.py` & `PyDAO_9000-1.2/SqltDAO/Gui/TableDef.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/Ledger.py` & `PyDAO_9000-1.2/SqltDAO/Ledger.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/SchemaDef/DataDetective.py` & `PyDAO_9000-1.2/SqltDAO/SchemaDef/DataDetective.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/SchemaDef/Factory.py` & `PyDAO_9000-1.2/SqltDAO/SchemaDef/Factory.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/SchemaDef/OrderDef.py` & `PyDAO_9000-1.2/SqltDAO/SchemaDef/OrderDef.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/SchemaDef/Table.py` & `PyDAO_9000-1.2/SqltDAO/SchemaDef/Table.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/UpdateTestCase.py` & `PyDAO_9000-1.2/SqltDAO/UpdateTestCase.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.1/SqltDAO/main.py` & `PyDAO_9000-1.2/SqltDAO/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         zpref = DataPreferences(self, self.home)
         if zpref.has_changed():
             pass
 
     def _on_about(self):
         messagebox.showinfo(
             self.ztitle,
-            "Mode: Cross-platform Testing")
+            "Official Release")
 
     def _show_order(self):
         if not self.order_def:
             return False
         self.table_frame.empty()
         for key in self.order_def._zdict_tables:
             td1 = self.order_def._zdict_tables[key]
```

