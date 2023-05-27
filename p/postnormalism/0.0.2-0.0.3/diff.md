# Comparing `tmp/postnormalism-0.0.2.tar.gz` & `tmp/postnormalism-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postnormalism-0.0.2.tar", last modified: Sat May 20 00:50:16 2023, max compression
+gzip compressed data, was "postnormalism-0.0.3.tar", last modified: Sat May 27 03:02:00 2023, max compression
```

## Comparing `postnormalism-0.0.2.tar` & `postnormalism-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 00:50:16.482985 postnormalism-0.0.2/
--rw-rw-rw-   0        0        0     1119 2023-05-06 02:54:20.000000 postnormalism-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     6560 2023-05-20 00:50:16.481987 postnormalism-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5399 2023-05-20 00:44:01.000000 postnormalism-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 00:50:16.460985 postnormalism-0.0.2/postnormalism/
--rw-rw-rw-   0        0        0        5 2023-05-20 00:46:34.000000 postnormalism-0.0.2/postnormalism/VERSION
--rw-rw-rw-   0        0        0        0 2023-05-06 02:40:21.000000 postnormalism-0.0.2/postnormalism/__init__.py
--rw-rw-rw-   0        0        0     2143 2023-05-17 02:28:23.000000 postnormalism-0.0.2/postnormalism/core.py
-drwxrwxrwx   0        0        0        0 2023-05-20 00:50:16.478983 postnormalism-0.0.2/postnormalism/schema/
--rw-rw-rw-   0        0        0      131 2023-05-08 03:58:46.000000 postnormalism-0.0.2/postnormalism/schema/__init__.py
--rw-rw-rw-   0        0        0     1509 2023-05-17 02:29:40.000000 postnormalism-0.0.2/postnormalism/schema/database.py
--rw-rw-rw-   0        0        0     1082 2023-05-17 02:15:23.000000 postnormalism-0.0.2/postnormalism/schema/database_item.py
--rw-rw-rw-   0        0        0      408 2023-05-08 03:58:46.000000 postnormalism-0.0.2/postnormalism/schema/function.py
--rw-rw-rw-   0        0        0      774 2023-05-17 02:19:15.000000 postnormalism-0.0.2/postnormalism/schema/table.py
--rw-rw-rw-   0        0        0      711 2023-05-06 03:40:39.000000 postnormalism-0.0.2/postnormalism/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-20 00:50:16.473984 postnormalism-0.0.2/postnormalism.egg-info/
--rw-rw-rw-   0        0        0     6560 2023-05-20 00:50:16.000000 postnormalism-0.0.2/postnormalism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      480 2023-05-20 00:50:16.000000 postnormalism-0.0.2/postnormalism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 00:50:16.000000 postnormalism-0.0.2/postnormalism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-20 00:50:16.000000 postnormalism-0.0.2/postnormalism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1342 2023-05-20 00:26:25.000000 postnormalism-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-20 00:50:16.482985 postnormalism-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-20 00:50:16.480983 postnormalism-0.0.2/tests/
--rw-rw-rw-   0        0        0     1778 2023-05-06 17:12:44.000000 postnormalism-0.0.2/tests/test_core.py
--rw-rw-rw-   0        0        0     2288 2023-05-06 17:12:44.000000 postnormalism-0.0.2/tests/test_schema.py
+drwxrwxrwx   0        0        0        0 2023-05-27 03:02:00.157980 postnormalism-0.0.3/
+-rw-rw-rw-   0        0        0     1119 2023-05-06 02:54:20.000000 postnormalism-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     7408 2023-05-27 03:02:00.156979 postnormalism-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6247 2023-05-27 02:52:47.000000 postnormalism-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 03:02:00.090039 postnormalism-0.0.3/postnormalism/
+-rw-rw-rw-   0        0        0        5 2023-05-27 02:52:47.000000 postnormalism-0.0.3/postnormalism/VERSION
+-rw-rw-rw-   0        0        0        0 2023-05-06 02:40:21.000000 postnormalism-0.0.3/postnormalism/__init__.py
+-rw-rw-rw-   0        0        0     2143 2023-05-22 03:33:00.000000 postnormalism-0.0.3/postnormalism/core.py
+drwxrwxrwx   0        0        0        0 2023-05-27 03:02:00.139981 postnormalism-0.0.3/postnormalism/schema/
+-rw-rw-rw-   0        0        0      182 2023-05-20 21:39:27.000000 postnormalism-0.0.3/postnormalism/schema/__init__.py
+-rw-rw-rw-   0        0        0     4713 2023-05-20 22:09:21.000000 postnormalism-0.0.3/postnormalism/schema/database.py
+-rw-rw-rw-   0        0        0     1082 2023-05-17 02:15:23.000000 postnormalism-0.0.3/postnormalism/schema/database_item.py
+-rw-rw-rw-   0        0        0      408 2023-05-08 03:58:46.000000 postnormalism-0.0.3/postnormalism/schema/function.py
+-rw-rw-rw-   0        0        0      406 2023-05-20 21:52:37.000000 postnormalism-0.0.3/postnormalism/schema/migrations.py
+-rw-rw-rw-   0        0        0      774 2023-05-17 02:19:15.000000 postnormalism-0.0.3/postnormalism/schema/table.py
+-rw-rw-rw-   0        0        0      711 2023-05-06 03:40:39.000000 postnormalism-0.0.3/postnormalism/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-27 03:02:00.106038 postnormalism-0.0.3/postnormalism.egg-info/
+-rw-rw-rw-   0        0        0     7408 2023-05-27 03:02:00.000000 postnormalism-0.0.3/postnormalism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-05-27 03:02:00.000000 postnormalism-0.0.3/postnormalism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 03:02:00.000000 postnormalism-0.0.3/postnormalism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-27 03:02:00.000000 postnormalism-0.0.3/postnormalism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1342 2023-05-20 00:26:25.000000 postnormalism-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 03:02:00.157980 postnormalism-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 03:02:00.155982 postnormalism-0.0.3/tests/
+-rw-rw-rw-   0        0        0     1778 2023-05-06 17:12:44.000000 postnormalism-0.0.3/tests/test_core.py
+-rw-rw-rw-   0        0        0     2288 2023-05-06 17:12:44.000000 postnormalism-0.0.3/tests/test_schema.py
```

### Comparing `postnormalism-0.0.2/LICENSE` & `postnormalism-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `postnormalism-0.0.2/PKG-INFO` & `postnormalism-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,19 @@
-Metadata-Version: 2.1
-Name: postnormalism
-Version: 0.0.2
-Summary: Postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.
-Author-email: Zac Miller <zac@informatical.info>
-Maintainer-email: Zac Miller <zac@informatical.info>
-License: MIT License
-Project-URL: Homepage, https://github.com/jzmiller1/postnormalism
-Project-URL: Bug Tracker, https://github.com/jzmiller1/postnormalism/issues
-Project-URL: Repository, https://github.com/jzmiller1/postnormalism.git
-Project-URL: History, https://github.com/jzmiller1/postnormalism/blob/master/HISTORY.md
-Keywords: python,postgresql,schema
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # postnormalism: PostgreSQL Schema Management  
   
 postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.  
   
 ## Features  
   
 - Define tables and functions using Python dataclasses  
 - Create database items (Tables, Functions) with comments
 - Group related database items and create them within a single transaction  
 - Create a Database object that allows loading database items in a specified load order and managing database extensions
 - IF NOT EXISTS mode for loading
+- SQL Migration Loader
 
   
 ## NORM vs. ORM: Features Comparison  
   
 postnormalism is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It does not possess all the characteristics of a full-fledged ORM, focusing mainly on schema management and organization.  
   
 Here is a comparison of postnormalism's features with typical ORM characteristics:  
@@ -136,15 +116,39 @@
 
 universe.create(cursor)  
 
 connection.commit()  
 connection.close()  
 ```  
 
-  
+### Using exists Mode
+Calling Database.create with exists=True inserts a IF NOT EXISTS into all of your CREATE statements allowing you to easily add new items.
+
+```python
+universe.create(cursor, exists=True)
+```
+
+### Doing migrations
+Update your `DatabaseItem`s and write your SQL migration transaction.  If you create your Database instance with 
+a `migrations_folder` they will run during the create call.  Migration files should ideally be prefixed with a 
+load order (ex: 0001) and must end with `.sql`.
+
+```python
+universe = Database(
+    load_order=[
+        Material, get_material_for_variant,
+        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
+    ],
+    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto'],
+    migrations_folder='/example/folder/path'
+)
+
+```
+
+
 ## Contributing  
   
 Please submit a pull request or create an issue if you have any suggestions or improvements.  
   
 ## License  
   
 postnormalism is released under the MIT License. See the `LICENSE` file for more information.
```

### Comparing `postnormalism-0.0.2/README.md` & `postnormalism-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,40 @@
+Metadata-Version: 2.1
+Name: postnormalism
+Version: 0.0.3
+Summary: Postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.
+Author-email: Zac Miller <zac@informatical.info>
+Maintainer-email: Zac Miller <zac@informatical.info>
+License: MIT License
+Project-URL: Homepage, https://github.com/jzmiller1/postnormalism
+Project-URL: Bug Tracker, https://github.com/jzmiller1/postnormalism/issues
+Project-URL: Repository, https://github.com/jzmiller1/postnormalism.git
+Project-URL: History, https://github.com/jzmiller1/postnormalism/blob/master/HISTORY.md
+Keywords: python,postgresql,schema
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # postnormalism: PostgreSQL Schema Management  
   
 postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.  
   
 ## Features  
   
 - Define tables and functions using Python dataclasses  
 - Create database items (Tables, Functions) with comments
 - Group related database items and create them within a single transaction  
 - Create a Database object that allows loading database items in a specified load order and managing database extensions
 - IF NOT EXISTS mode for loading
+- SQL Migration Loader
 
   
 ## NORM vs. ORM: Features Comparison  
   
 postnormalism is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It does not possess all the characteristics of a full-fledged ORM, focusing mainly on schema management and organization.  
   
 Here is a comparison of postnormalism's features with typical ORM characteristics:  
@@ -115,15 +137,39 @@
 
 universe.create(cursor)  
 
 connection.commit()  
 connection.close()  
 ```  
 
-  
+### Using exists Mode
+Calling Database.create with exists=True inserts a IF NOT EXISTS into all of your CREATE statements allowing you to easily add new items.
+
+```python
+universe.create(cursor, exists=True)
+```
+
+### Doing migrations
+Update your `DatabaseItem`s and write your SQL migration transaction.  If you create your Database instance with 
+a `migrations_folder` they will run during the create call.  Migration files should ideally be prefixed with a 
+load order (ex: 0001) and must end with `.sql`.
+
+```python
+universe = Database(
+    load_order=[
+        Material, get_material_for_variant,
+        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
+    ],
+    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto'],
+    migrations_folder='/example/folder/path'
+)
+
+```
+
+
 ## Contributing  
   
 Please submit a pull request or create an issue if you have any suggestions or improvements.  
   
 ## License  
   
 postnormalism is released under the MIT License. See the `LICENSE` file for more information.
```

### Comparing `postnormalism-0.0.2/postnormalism/core.py` & `postnormalism-0.0.3/postnormalism/core.py`

 * *Files identical despite different names*

### Comparing `postnormalism-0.0.2/postnormalism/schema/database_item.py` & `postnormalism-0.0.3/postnormalism/schema/database_item.py`

 * *Files identical despite different names*

### Comparing `postnormalism-0.0.2/postnormalism/schema/table.py` & `postnormalism-0.0.3/postnormalism/schema/table.py`

 * *Files identical despite different names*

### Comparing `postnormalism-0.0.2/postnormalism/utils.py` & `postnormalism-0.0.3/postnormalism/utils.py`

 * *Files identical despite different names*

### Comparing `postnormalism-0.0.2/postnormalism.egg-info/PKG-INFO` & `postnormalism-0.0.3/postnormalism.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postnormalism
-Version: 0.0.2
+Version: 0.0.3
 Summary: Postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.
 Author-email: Zac Miller <zac@informatical.info>
 Maintainer-email: Zac Miller <zac@informatical.info>
 License: MIT License
 Project-URL: Homepage, https://github.com/jzmiller1/postnormalism
 Project-URL: Bug Tracker, https://github.com/jzmiller1/postnormalism/issues
 Project-URL: Repository, https://github.com/jzmiller1/postnormalism.git
@@ -26,14 +26,15 @@
 ## Features  
   
 - Define tables and functions using Python dataclasses  
 - Create database items (Tables, Functions) with comments
 - Group related database items and create them within a single transaction  
 - Create a Database object that allows loading database items in a specified load order and managing database extensions
 - IF NOT EXISTS mode for loading
+- SQL Migration Loader
 
   
 ## NORM vs. ORM: Features Comparison  
   
 postnormalism is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It does not possess all the characteristics of a full-fledged ORM, focusing mainly on schema management and organization.  
   
 Here is a comparison of postnormalism's features with typical ORM characteristics:  
@@ -136,15 +137,39 @@
 
 universe.create(cursor)  
 
 connection.commit()  
 connection.close()  
 ```  
 
-  
+### Using exists Mode
+Calling Database.create with exists=True inserts a IF NOT EXISTS into all of your CREATE statements allowing you to easily add new items.
+
+```python
+universe.create(cursor, exists=True)
+```
+
+### Doing migrations
+Update your `DatabaseItem`s and write your SQL migration transaction.  If you create your Database instance with 
+a `migrations_folder` they will run during the create call.  Migration files should ideally be prefixed with a 
+load order (ex: 0001) and must end with `.sql`.
+
+```python
+universe = Database(
+    load_order=[
+        Material, get_material_for_variant,
+        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
+    ],
+    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto'],
+    migrations_folder='/example/folder/path'
+)
+
+```
+
+
 ## Contributing  
   
 Please submit a pull request or create an issue if you have any suggestions or improvements.  
   
 ## License  
   
 postnormalism is released under the MIT License. See the `LICENSE` file for more information.
```

### Comparing `postnormalism-0.0.2/pyproject.toml` & `postnormalism-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `postnormalism-0.0.2/tests/test_core.py` & `postnormalism-0.0.3/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `postnormalism-0.0.2/tests/test_schema.py` & `postnormalism-0.0.3/tests/test_schema.py`

 * *Files identical despite different names*

