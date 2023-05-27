# Comparing `tmp/PyDAO_9000-0.9.tar.gz` & `tmp/PyDAO_9000-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDAO_9000-0.9.tar", last modified: Sat May 27 13:52:34 2023, max compression
+gzip compressed data, was "PyDAO_9000-1.0.tar", last modified: Sat May 27 14:50:40 2023, max compression
```

## Comparing `PyDAO_9000-0.9.tar` & `PyDAO_9000-1.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 13:52:34.806335 PyDAO_9000-0.9/
--rw-rw-rw-   0        0        0     1090 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/LICENSE
--rw-rw-rw-   0        0        0     4270 2023-05-27 13:52:34.806335 PyDAO_9000-0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-27 13:52:34.696965 PyDAO_9000-0.9/PyDAO_9000.egg-info/
--rw-rw-rw-   0        0        0     4270 2023-05-27 13:52:34.000000 PyDAO_9000-0.9/PyDAO_9000.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1040 2023-05-27 13:52:34.000000 PyDAO_9000-0.9/PyDAO_9000.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 13:52:34.000000 PyDAO_9000-0.9/PyDAO_9000.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-27 13:52:34.000000 PyDAO_9000-0.9/PyDAO_9000.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3756 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 13:52:34.728201 PyDAO_9000-0.9/SqltDAO/
-drwxrwxrwx   0        0        0        0 2023-05-27 13:52:34.743826 PyDAO_9000-0.9/SqltDAO/CodeGen01/
--rw-rw-rw-   0        0        0     3108 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/CodeGen01/CodeGen.py
--rw-rw-rw-   0        0        0      865 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/CodeGen01/CodeLevel.py
--rw-rw-rw-   0        0        0      264 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/CodeGen01/DaoExceptions.py
--rw-rw-rw-   0        0        0      485 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/CodeGen01/Meta.py
--rw-rw-rw-   0        0        0     1816 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/CodeGen01/Normalizers.py
--rw-rw-rw-   0        0        0     4309 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/CodeGen01/OrderClass.py
--rw-rw-rw-   0        0        0    12389 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/CodeGen01/SqlSyntax.py
--rw-rw-rw-   0        0        0     7315 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/CodeGen01/TextDataDetector.py
--rw-rw-rw-   0        0        0    13912 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/CrudMeister.py
-drwxrwxrwx   0        0        0        0 2023-05-27 13:52:34.759454 PyDAO_9000-0.9/SqltDAO/DaoTest01/
--rw-rw-rw-   0        0        0      678 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/DaoTest01/GenNasdaq.py
--rw-rw-rw-   0        0        0      507 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/DaoTest01/GenNasdaqTest.py
--rw-rw-rw-   0        0        0     3252 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/DaoTest01/Income.py
--rw-rw-rw-   0        0        0     3054 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/DaoTest01/NasdaqDAO.py
--rw-rw-rw-   0        0        0     3488 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/DaoTest01/foo.py
--rw-rw-rw-   0        0        0      847 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/DaoTest01/tc001_driver.py
--rw-rw-rw-   0        0        0      691 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/DaoTest01/tc001_gen.py
--rw-rw-rw-   0        0        0     2923 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/Demo123.py
-drwxrwxrwx   0        0        0        0 2023-05-27 13:52:34.790700 PyDAO_9000-0.9/SqltDAO/Gui/
--rw-rw-rw-   0        0        0     6185 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/Gui/Data2Code.py
--rw-rw-rw-   0        0        0     6553 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/Gui/DataAI.py
--rw-rw-rw-   0        0        0     4628 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/Gui/DataFrameOne.py
--rw-rw-rw-   0        0        0     4892 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/Gui/DataPreferences.py
--rw-rw-rw-   0        0        0     4771 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/Gui/StandardEntry.py
--rw-rw-rw-   0        0        0     6403 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/Gui/TableDef.py
--rw-rw-rw-   0        0        0     3504 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/Ledger.py
-drwxrwxrwx   0        0        0        0 2023-05-27 13:52:34.790700 PyDAO_9000-0.9/SqltDAO/SchemaDef/
--rw-rw-rw-   0        0        0     8393 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/SchemaDef/DataDetective.py
--rw-rw-rw-   0        0        0     9378 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/SchemaDef/Factory.py
--rw-rw-rw-   0        0        0     8987 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/SchemaDef/OrderDef.py
--rw-rw-rw-   0        0        0     3179 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/SchemaDef/Table.py
--rw-rw-rw-   0        0        0     3602 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/UpdateTestCase.py
--rw-rw-rw-   0        0        0      103 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/__init__.py
--rw-rw-rw-   0        0        0     7586 2023-05-27 11:01:18.000000 PyDAO_9000-0.9/SqltDAO/main.py
--rw-rw-rw-   0        0        0      502 2023-05-27 13:51:41.000000 PyDAO_9000-0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 13:52:34.806335 PyDAO_9000-0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 14:50:40.885977 PyDAO_9000-1.0/
+-rw-rw-rw-   0        0        0     1090 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/LICENSE
+-rw-rw-rw-   0        0        0     4240 2023-05-27 14:50:40.885977 PyDAO_9000-1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-27 14:50:40.792237 PyDAO_9000-1.0/PyDAO_9000.egg-info/
+-rw-rw-rw-   0        0        0     4240 2023-05-27 14:50:40.000000 PyDAO_9000-1.0/PyDAO_9000.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1040 2023-05-27 14:50:40.000000 PyDAO_9000-1.0/PyDAO_9000.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 14:50:40.000000 PyDAO_9000-1.0/PyDAO_9000.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-27 14:50:40.000000 PyDAO_9000-1.0/PyDAO_9000.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3726 2023-05-27 14:12:23.000000 PyDAO_9000-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 14:50:40.807857 PyDAO_9000-1.0/SqltDAO/
+drwxrwxrwx   0        0        0        0 2023-05-27 14:50:40.839105 PyDAO_9000-1.0/SqltDAO/CodeGen01/
+-rw-rw-rw-   0        0        0     3108 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/CodeGen01/CodeGen.py
+-rw-rw-rw-   0        0        0      865 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/CodeGen01/CodeLevel.py
+-rw-rw-rw-   0        0        0      264 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/CodeGen01/DaoExceptions.py
+-rw-rw-rw-   0        0        0      485 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/CodeGen01/Meta.py
+-rw-rw-rw-   0        0        0     1816 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/CodeGen01/Normalizers.py
+-rw-rw-rw-   0        0        0     4309 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/CodeGen01/OrderClass.py
+-rw-rw-rw-   0        0        0    12389 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/CodeGen01/SqlSyntax.py
+-rw-rw-rw-   0        0        0     7315 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/CodeGen01/TextDataDetector.py
+-rw-rw-rw-   0        0        0    13912 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/CrudMeister.py
+drwxrwxrwx   0        0        0        0 2023-05-27 14:50:40.854735 PyDAO_9000-1.0/SqltDAO/DaoTest01/
+-rw-rw-rw-   0        0        0      678 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/DaoTest01/GenNasdaq.py
+-rw-rw-rw-   0        0        0      507 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/DaoTest01/GenNasdaqTest.py
+-rw-rw-rw-   0        0        0     3252 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/DaoTest01/Income.py
+-rw-rw-rw-   0        0        0     3054 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/DaoTest01/NasdaqDAO.py
+-rw-rw-rw-   0        0        0     3488 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/DaoTest01/foo.py
+-rw-rw-rw-   0        0        0      847 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/DaoTest01/tc001_driver.py
+-rw-rw-rw-   0        0        0      691 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/DaoTest01/tc001_gen.py
+-rw-rw-rw-   0        0        0     2923 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/Demo123.py
+drwxrwxrwx   0        0        0        0 2023-05-27 14:50:40.885977 PyDAO_9000-1.0/SqltDAO/Gui/
+-rw-rw-rw-   0        0        0     6185 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/Gui/Data2Code.py
+-rw-rw-rw-   0        0        0     6553 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/Gui/DataAI.py
+-rw-rw-rw-   0        0        0     4628 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/Gui/DataFrameOne.py
+-rw-rw-rw-   0        0        0     4892 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/Gui/DataPreferences.py
+-rw-rw-rw-   0        0        0     4771 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/Gui/StandardEntry.py
+-rw-rw-rw-   0        0        0     6403 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/Gui/TableDef.py
+-rw-rw-rw-   0        0        0     3504 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/Ledger.py
+drwxrwxrwx   0        0        0        0 2023-05-27 14:50:40.885977 PyDAO_9000-1.0/SqltDAO/SchemaDef/
+-rw-rw-rw-   0        0        0     8393 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/SchemaDef/DataDetective.py
+-rw-rw-rw-   0        0        0     9378 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/SchemaDef/Factory.py
+-rw-rw-rw-   0        0        0     8987 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/SchemaDef/OrderDef.py
+-rw-rw-rw-   0        0        0     3179 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/SchemaDef/Table.py
+-rw-rw-rw-   0        0        0     3602 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/UpdateTestCase.py
+-rw-rw-rw-   0        0        0      103 2023-05-27 11:01:18.000000 PyDAO_9000-1.0/SqltDAO/__init__.py
+-rw-rw-rw-   0        0        0     7759 2023-05-27 14:43:15.000000 PyDAO_9000-1.0/SqltDAO/main.py
+-rw-rw-rw-   0        0        0      502 2023-05-27 14:49:54.000000 PyDAO_9000-1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 14:50:40.885977 PyDAO_9000-1.0/setup.cfg
```

### Comparing `PyDAO_9000-0.9/LICENSE` & `PyDAO_9000-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/PKG-INFO` & `PyDAO_9000-1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDAO_9000
-Version: 0.9
+Version: 1.0
 Summary: All-In-One File SQL Code Generator
 Author-email: Randall Nagy <r.a.nagy@gmail.com>
 Project-URL: Homepage, https://github.com/soft9000/PyDAO
 Project-URL: Bug Tracker, https://github.com/soft9000/PyDAO/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 License-File: LICENSE
 
 # PyDAO 9000
 The Soft9000/PyDAO ("__PyDAO 9000__") Project allows us to quickly create a Python Class from either a GUI, API, textual (CSV, TDF, Enpiped, etc.) data file, or using a Python Dictionary. 
 
 Best of all the code generated by __PyDAO 9000__ is 100% Core Python 3 - no other files are required!
 
-![PyDAO Project Logo](https://github.com/soft9000/PyDAO/blob/master/PyDAO_GitLogo.png)
+![PyDAO Project Logo](PyDAO_GitLogo.png)
 
 _Workflows include_: 
 
 (1) Creating stand-alone __PyDAO 9000__ DAO script(s.) 
 
 (2) Extracting __PyDAO 9000__ projects from textual (CSV, etc.) data files, 
 
@@ -34,19 +34,19 @@
 Project Video: https://youtu.be/azCokv4iI8k
 
 All four (4) workflows are supported - feel free to give each a try!
 
 
 MAIN.py
 -------
-![PyDAO GUI](https://github.com/soft9000/PyDAO/blob/master/PyDAO_GUI.png)
+![PyDAO GUI](PyDAO_GUI.png)
 
 2021/02/18: Have been using row factories for awhile now. Decided to share. We also can now .insert + .update our DAO's 'object.fields' data, as well.
 
-2023/05/37: Yeas latter the GUI is working well enough to declare what we have as Release.
+2023/05/37: Years latter the project is working well enough to declare what we have as an [Official PyPy Package](https://pypi.org/project/PyDAO-9000/).
 
 If you want to support the effort, fell free to purchase one of [our books on amazon](https://www.amazon.com/Randall-Nagy/e/B08ZJLH1VN) or [training opportunuties](https://www.udemy.com/user/randallnagy2/).
 
 PyDAO UI: https://github.com/soft9000/PyDAO/blob/master/SqltDAO/main.py
 
 
 API Example
```

### Comparing `PyDAO_9000-0.9/PyDAO_9000.egg-info/PKG-INFO` & `PyDAO_9000-1.0/PyDAO_9000.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDAO-9000
-Version: 0.9
+Version: 1.0
 Summary: All-In-One File SQL Code Generator
 Author-email: Randall Nagy <r.a.nagy@gmail.com>
 Project-URL: Homepage, https://github.com/soft9000/PyDAO
 Project-URL: Bug Tracker, https://github.com/soft9000/PyDAO/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 License-File: LICENSE
 
 # PyDAO 9000
 The Soft9000/PyDAO ("__PyDAO 9000__") Project allows us to quickly create a Python Class from either a GUI, API, textual (CSV, TDF, Enpiped, etc.) data file, or using a Python Dictionary. 
 
 Best of all the code generated by __PyDAO 9000__ is 100% Core Python 3 - no other files are required!
 
-![PyDAO Project Logo](https://github.com/soft9000/PyDAO/blob/master/PyDAO_GitLogo.png)
+![PyDAO Project Logo](PyDAO_GitLogo.png)
 
 _Workflows include_: 
 
 (1) Creating stand-alone __PyDAO 9000__ DAO script(s.) 
 
 (2) Extracting __PyDAO 9000__ projects from textual (CSV, etc.) data files, 
 
@@ -34,19 +34,19 @@
 Project Video: https://youtu.be/azCokv4iI8k
 
 All four (4) workflows are supported - feel free to give each a try!
 
 
 MAIN.py
 -------
-![PyDAO GUI](https://github.com/soft9000/PyDAO/blob/master/PyDAO_GUI.png)
+![PyDAO GUI](PyDAO_GUI.png)
 
 2021/02/18: Have been using row factories for awhile now. Decided to share. We also can now .insert + .update our DAO's 'object.fields' data, as well.
 
-2023/05/37: Yeas latter the GUI is working well enough to declare what we have as Release.
+2023/05/37: Years latter the project is working well enough to declare what we have as an [Official PyPy Package](https://pypi.org/project/PyDAO-9000/).
 
 If you want to support the effort, fell free to purchase one of [our books on amazon](https://www.amazon.com/Randall-Nagy/e/B08ZJLH1VN) or [training opportunuties](https://www.udemy.com/user/randallnagy2/).
 
 PyDAO UI: https://github.com/soft9000/PyDAO/blob/master/SqltDAO/main.py
 
 
 API Example
```

### Comparing `PyDAO_9000-0.9/PyDAO_9000.egg-info/SOURCES.txt` & `PyDAO_9000-1.0/PyDAO_9000.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/README.md` & `PyDAO_9000-1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # PyDAO 9000
 The Soft9000/PyDAO ("__PyDAO 9000__") Project allows us to quickly create a Python Class from either a GUI, API, textual (CSV, TDF, Enpiped, etc.) data file, or using a Python Dictionary. 
 
 Best of all the code generated by __PyDAO 9000__ is 100% Core Python 3 - no other files are required!
 
-![PyDAO Project Logo](https://github.com/soft9000/PyDAO/blob/master/PyDAO_GitLogo.png)
+![PyDAO Project Logo](PyDAO_GitLogo.png)
 
 _Workflows include_: 
 
 (1) Creating stand-alone __PyDAO 9000__ DAO script(s.) 
 
 (2) Extracting __PyDAO 9000__ projects from textual (CSV, etc.) data files, 
 
@@ -20,19 +20,19 @@
 Project Video: https://youtu.be/azCokv4iI8k
 
 All four (4) workflows are supported - feel free to give each a try!
 
 
 MAIN.py
 -------
-![PyDAO GUI](https://github.com/soft9000/PyDAO/blob/master/PyDAO_GUI.png)
+![PyDAO GUI](PyDAO_GUI.png)
 
 2021/02/18: Have been using row factories for awhile now. Decided to share. We also can now .insert + .update our DAO's 'object.fields' data, as well.
 
-2023/05/37: Yeas latter the GUI is working well enough to declare what we have as Release.
+2023/05/37: Years latter the project is working well enough to declare what we have as an [Official PyPy Package](https://pypi.org/project/PyDAO-9000/).
 
 If you want to support the effort, fell free to purchase one of [our books on amazon](https://www.amazon.com/Randall-Nagy/e/B08ZJLH1VN) or [training opportunuties](https://www.udemy.com/user/randallnagy2/).
 
 PyDAO UI: https://github.com/soft9000/PyDAO/blob/master/SqltDAO/main.py
 
 
 API Example
```

### Comparing `PyDAO_9000-0.9/SqltDAO/CodeGen01/CodeGen.py` & `PyDAO_9000-1.0/SqltDAO/CodeGen01/CodeGen.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/CodeGen01/CodeLevel.py` & `PyDAO_9000-1.0/SqltDAO/CodeGen01/CodeLevel.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/CodeGen01/Normalizers.py` & `PyDAO_9000-1.0/SqltDAO/CodeGen01/Normalizers.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/CodeGen01/OrderClass.py` & `PyDAO_9000-1.0/SqltDAO/CodeGen01/OrderClass.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/CodeGen01/SqlSyntax.py` & `PyDAO_9000-1.0/SqltDAO/CodeGen01/SqlSyntax.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/CodeGen01/TextDataDetector.py` & `PyDAO_9000-1.0/SqltDAO/CodeGen01/TextDataDetector.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/CrudMeister.py` & `PyDAO_9000-1.0/SqltDAO/CrudMeister.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/DaoTest01/GenNasdaq.py` & `PyDAO_9000-1.0/SqltDAO/DaoTest01/GenNasdaq.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/DaoTest01/Income.py` & `PyDAO_9000-1.0/SqltDAO/DaoTest01/Income.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/DaoTest01/NasdaqDAO.py` & `PyDAO_9000-1.0/SqltDAO/DaoTest01/NasdaqDAO.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/DaoTest01/foo.py` & `PyDAO_9000-1.0/SqltDAO/DaoTest01/foo.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/DaoTest01/tc001_driver.py` & `PyDAO_9000-1.0/SqltDAO/DaoTest01/tc001_driver.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/DaoTest01/tc001_gen.py` & `PyDAO_9000-1.0/SqltDAO/DaoTest01/tc001_gen.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/Demo123.py` & `PyDAO_9000-1.0/SqltDAO/Demo123.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/Gui/Data2Code.py` & `PyDAO_9000-1.0/SqltDAO/Gui/Data2Code.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/Gui/DataAI.py` & `PyDAO_9000-1.0/SqltDAO/Gui/DataAI.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/Gui/DataFrameOne.py` & `PyDAO_9000-1.0/SqltDAO/Gui/DataFrameOne.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/Gui/DataPreferences.py` & `PyDAO_9000-1.0/SqltDAO/Gui/DataPreferences.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/Gui/StandardEntry.py` & `PyDAO_9000-1.0/SqltDAO/Gui/StandardEntry.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/Gui/TableDef.py` & `PyDAO_9000-1.0/SqltDAO/Gui/TableDef.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/Ledger.py` & `PyDAO_9000-1.0/SqltDAO/Ledger.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/SchemaDef/DataDetective.py` & `PyDAO_9000-1.0/SqltDAO/SchemaDef/DataDetective.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/SchemaDef/Factory.py` & `PyDAO_9000-1.0/SqltDAO/SchemaDef/Factory.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/SchemaDef/OrderDef.py` & `PyDAO_9000-1.0/SqltDAO/SchemaDef/OrderDef.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/SchemaDef/Table.py` & `PyDAO_9000-1.0/SqltDAO/SchemaDef/Table.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/UpdateTestCase.py` & `PyDAO_9000-1.0/SqltDAO/UpdateTestCase.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-0.9/SqltDAO/main.py` & `PyDAO_9000-1.0/SqltDAO/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,27 +188,35 @@
             for zz in zsub[1]:
                 zdrop.add_command(label=zz[0], command=zz[1])
         self.config(menu=zmain)
         self._set_frame()
         return True
 
     def run(self):
-        self.mainloop()
+        super().mainloop()
         return True
 
     def end(self):
         return True
+    
+    @staticmethod
+    def mainloop():
+        main = Main()
+        try:
+            if main.begin():
+                main.run()
+                return True
+        except Exception as ex:
+            print(str(ex))
+            return False
+        finally:
+            try:
+                main.end()
+            except:
+                pass
+
 
 
 if __name__ == "__main__":
-    main = Main()
-    try:
-        if main.begin():
-            main.run()
-    except Exception as ex:
-        print(str(ex))
-    finally:
-        try:
-            main.end()
-        except:
-            pass
+    Main.mainloop()
+
```

