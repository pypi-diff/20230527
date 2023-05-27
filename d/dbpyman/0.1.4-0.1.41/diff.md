# Comparing `tmp/dbpyman-0.1.4.tar.gz` & `tmp/dbpyman-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbpyman-0.1.4.tar", last modified: Sat May 27 11:34:01 2023, max compression
+gzip compressed data, was "dbpyman-0.1.41.tar", last modified: Sat May 27 11:35:33 2023, max compression
```

## Comparing `dbpyman-0.1.4.tar` & `dbpyman-0.1.41.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 11:34:01.683629 dbpyman-0.1.4/
--rw-rw-rw-   0        0        0     1091 2023-05-09 18:13:07.000000 dbpyman-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     3934 2023-05-27 11:34:01.683629 dbpyman-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3345 2023-05-26 19:49:20.000000 dbpyman-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 11:34:01.668669 dbpyman-0.1.4/dbpyman.egg-info/
--rw-rw-rw-   0        0        0     3934 2023-05-27 11:34:01.000000 dbpyman-0.1.4/dbpyman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-27 11:34:01.000000 dbpyman-0.1.4/dbpyman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 11:34:01.000000 dbpyman-0.1.4/dbpyman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-27 11:34:01.000000 dbpyman-0.1.4/dbpyman.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 11:34:01.671661 dbpyman-0.1.4/py_discord_db_management/
--rw-rw-rw-   0        0        0        0 2023-05-09 18:05:53.000000 dbpyman-0.1.4/py_discord_db_management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 11:34:01.676648 dbpyman-0.1.4/py_discord_db_management/classes/
--rw-rw-rw-   0        0        0        0 2023-05-24 17:07:59.000000 dbpyman-0.1.4/py_discord_db_management/classes/__init__.py
--rw-rw-rw-   0        0        0     1469 2023-05-27 11:33:34.000000 dbpyman-0.1.4/py_discord_db_management/classes/column.py
--rw-rw-rw-   0        0        0     2768 2023-05-26 20:13:55.000000 dbpyman-0.1.4/py_discord_db_management/classes/database.py
--rw-rw-rw-   0        0        0     1234 2023-05-26 20:02:24.000000 dbpyman-0.1.4/py_discord_db_management/classes/table.py
--rw-rw-rw-   0        0        0      588 2023-05-24 17:07:59.000000 dbpyman-0.1.4/py_discord_db_management/dbpyman.py
-drwxrwxrwx   0        0        0        0 2023-05-27 11:34:01.681634 dbpyman-0.1.4/py_discord_db_management/views/
--rw-rw-rw-   0        0        0        0 2023-05-24 17:07:59.000000 dbpyman-0.1.4/py_discord_db_management/views/__init__.py
--rw-rw-rw-   0        0        0     3732 2023-05-26 19:49:20.000000 dbpyman-0.1.4/py_discord_db_management/views/table_add_data_view.py
--rw-rw-rw-   0        0        0     2769 2023-05-26 20:15:39.000000 dbpyman-0.1.4/py_discord_db_management/views/table_categories_view.py
--rw-rw-rw-   0        0        0      958 2023-05-26 19:49:20.000000 dbpyman-0.1.4/py_discord_db_management/views/table_overview_view.py
--rw-rw-rw-   0        0        0      577 2023-05-27 11:33:46.000000 dbpyman-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 11:34:01.683629 dbpyman-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 11:35:33.735602 dbpyman-0.1.41/
+-rw-rw-rw-   0        0        0     1091 2023-05-09 18:13:07.000000 dbpyman-0.1.41/LICENSE
+-rw-rw-rw-   0        0        0     3935 2023-05-27 11:35:33.734604 dbpyman-0.1.41/PKG-INFO
+-rw-rw-rw-   0        0        0     3345 2023-05-26 19:49:20.000000 dbpyman-0.1.41/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 11:35:33.721639 dbpyman-0.1.41/dbpyman.egg-info/
+-rw-rw-rw-   0        0        0     3935 2023-05-27 11:35:33.000000 dbpyman-0.1.41/dbpyman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-27 11:35:33.000000 dbpyman-0.1.41/dbpyman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 11:35:33.000000 dbpyman-0.1.41/dbpyman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-27 11:35:33.000000 dbpyman-0.1.41/dbpyman.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 11:35:33.723634 dbpyman-0.1.41/py_discord_db_management/
+-rw-rw-rw-   0        0        0        0 2023-05-09 18:05:53.000000 dbpyman-0.1.41/py_discord_db_management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:35:33.728620 dbpyman-0.1.41/py_discord_db_management/classes/
+-rw-rw-rw-   0        0        0        0 2023-05-24 17:07:59.000000 dbpyman-0.1.41/py_discord_db_management/classes/__init__.py
+-rw-rw-rw-   0        0        0     1385 2023-05-27 11:35:17.000000 dbpyman-0.1.41/py_discord_db_management/classes/column.py
+-rw-rw-rw-   0        0        0     2768 2023-05-26 20:13:55.000000 dbpyman-0.1.41/py_discord_db_management/classes/database.py
+-rw-rw-rw-   0        0        0     1234 2023-05-26 20:02:24.000000 dbpyman-0.1.41/py_discord_db_management/classes/table.py
+-rw-rw-rw-   0        0        0      588 2023-05-24 17:07:59.000000 dbpyman-0.1.41/py_discord_db_management/dbpyman.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:35:33.733607 dbpyman-0.1.41/py_discord_db_management/views/
+-rw-rw-rw-   0        0        0        0 2023-05-24 17:07:59.000000 dbpyman-0.1.41/py_discord_db_management/views/__init__.py
+-rw-rw-rw-   0        0        0     3732 2023-05-26 19:49:20.000000 dbpyman-0.1.41/py_discord_db_management/views/table_add_data_view.py
+-rw-rw-rw-   0        0        0     2769 2023-05-26 20:15:39.000000 dbpyman-0.1.41/py_discord_db_management/views/table_categories_view.py
+-rw-rw-rw-   0        0        0      958 2023-05-26 19:49:20.000000 dbpyman-0.1.41/py_discord_db_management/views/table_overview_view.py
+-rw-rw-rw-   0        0        0      578 2023-05-27 11:35:22.000000 dbpyman-0.1.41/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 11:35:33.735602 dbpyman-0.1.41/setup.cfg
```

### Comparing `dbpyman-0.1.4/LICENSE` & `dbpyman-0.1.41/LICENSE`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.4/PKG-INFO` & `dbpyman-0.1.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbpyman
-Version: 0.1.4
+Version: 0.1.41
 Summary: A package used to modify & view your MySQL database data dynamically
 Author-email: JanikCodes <janiksielaff@gmx.de>
 Project-URL: Homepage, https://github.com/JanikCodes/py_discord_db_management
 Project-URL: Bug Tracker, https://github.com/JanikCodes/py_discord_db_management/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dbpyman-0.1.4/README.md` & `dbpyman-0.1.41/README.md`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.4/dbpyman.egg-info/PKG-INFO` & `dbpyman-0.1.41/dbpyman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbpyman
-Version: 0.1.4
+Version: 0.1.41
 Summary: A package used to modify & view your MySQL database data dynamically
 Author-email: JanikCodes <janiksielaff@gmx.de>
 Project-URL: Homepage, https://github.com/JanikCodes/py_discord_db_management
 Project-URL: Bug Tracker, https://github.com/JanikCodes/py_discord_db_management/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dbpyman-0.1.4/dbpyman.egg-info/SOURCES.txt` & `dbpyman-0.1.41/dbpyman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.4/py_discord_db_management/classes/column.py` & `dbpyman-0.1.41/py_discord_db_management/classes/column.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,11 @@
                 return True
             return False
 
     def get_key(self):
         return self.__key
 
     def get_default(self):
-        if self.__null == 'NO' and not self.__default:
-            return str()
-
         return self.__default
 
     def get_extra(self):
         return self.__extra
```

### Comparing `dbpyman-0.1.4/py_discord_db_management/classes/database.py` & `dbpyman-0.1.41/py_discord_db_management/classes/database.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.4/py_discord_db_management/classes/table.py` & `dbpyman-0.1.41/py_discord_db_management/classes/table.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.4/py_discord_db_management/dbpyman.py` & `dbpyman-0.1.41/py_discord_db_management/dbpyman.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.4/py_discord_db_management/views/table_add_data_view.py` & `dbpyman-0.1.41/py_discord_db_management/views/table_add_data_view.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.4/py_discord_db_management/views/table_categories_view.py` & `dbpyman-0.1.41/py_discord_db_management/views/table_categories_view.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.4/py_discord_db_management/views/table_overview_view.py` & `dbpyman-0.1.41/py_discord_db_management/views/table_overview_view.py`

 * *Files identical despite different names*

### Comparing `dbpyman-0.1.4/pyproject.toml` & `dbpyman-0.1.41/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbpyman"
-version = "0.1.4"
+version = "0.1.41"
 authors = [
   { name="JanikCodes", email="janiksielaff@gmx.de" },
 ]
 description = "A package used to modify & view your MySQL database data dynamically"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

