# Comparing `tmp/d20-orm-2.0.1.tar.gz` & `tmp/d20-orm-2.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\d20\tools\libs\arangodb_python_orm\dist\.tmp-rilemvnz\d20-orm-2.0.1.tar", last modified: Fri May 26 23:59:50 2023, max compression
+gzip compressed data, was "D:\d20\tools\libs\arangodb_python_orm\dist\.tmp-0hfmkq5_\d20-orm-2.0.1a1.tar", last modified: Sat May 27 00:03:44 2023, max compression
```

## Comparing `d20-orm-2.0.1.tar` & `d20-orm-2.0.1a1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 23:59:50.667264 d20-orm-2.0.1/
--rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-orm-2.0.1/LICENSE
--rw-rw-rw-   0        0        0      893 2023-05-26 23:59:50.668274 d20-orm-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-04-25 02:17:24.000000 d20-orm-2.0.1/README.md
--rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-orm-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       72 2023-05-26 23:59:50.670629 d20-orm-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      874 2023-05-26 23:59:17.000000 d20-orm-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 23:59:50.481692 d20-orm-2.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 23:59:50.545114 d20-orm-2.0.1/src/d20_orm.egg-info/
--rw-rw-rw-   0        0        0      893 2023-05-26 23:59:50.000000 d20-orm-2.0.1/src/d20_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      607 2023-05-26 23:59:50.000000 d20-orm-2.0.1/src/d20_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 23:59:50.000000 d20-orm-2.0.1/src/d20_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-26 23:59:50.000000 d20-orm-2.0.1/src/d20_orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 23:59:50.000000 d20-orm-2.0.1/src/d20_orm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-26 23:59:50.613543 d20-orm-2.0.1/src/dtwentyORM/
--rw-rw-rw-   0        0        0     8911 2023-04-25 23:14:04.000000 d20-orm-2.0.1/src/dtwentyORM/BasicElement.py
--rw-rw-rw-   0        0        0     7211 2023-04-26 01:00:51.000000 d20-orm-2.0.1/src/dtwentyORM/DBConnector.py
--rw-rw-rw-   0        0        0     4749 2023-04-26 00:06:49.000000 d20-orm-2.0.1/src/dtwentyORM/Element.py
--rw-rw-rw-   0        0        0     7462 2023-04-06 00:37:34.000000 d20-orm-2.0.1/src/dtwentyORM/Error.py
--rw-rw-rw-   0        0        0     3632 2023-04-18 00:32:09.000000 d20-orm-2.0.1/src/dtwentyORM/GraphClassFactory.py
--rw-rw-rw-   0        0        0     5136 2023-04-26 01:16:05.000000 d20-orm-2.0.1/src/dtwentyORM/Metadata.py
--rw-rw-rw-   0        0        0       95 2023-04-06 00:37:34.000000 d20-orm-2.0.1/src/dtwentyORM/__init__.py
--rw-rw-rw-   0        0        0      161 2023-02-28 02:21:55.000000 d20-orm-2.0.1/src/dtwentyORM/__version__.py
--rw-rw-rw-   0        0        0     1427 2023-04-18 00:31:28.000000 d20-orm-2.0.1/src/dtwentyORM/support.py
-drwxrwxrwx   0        0        0        0 2023-05-26 23:59:50.665958 d20-orm-2.0.1/test/
--rw-rw-rw-   0        0        0      476 2023-04-25 02:17:24.000000 d20-orm-2.0.1/test/test_basic_element_test.py
--rw-rw-rw-   0        0        0      611 2023-04-25 02:17:24.000000 d20-orm-2.0.1/test/test_build_db.py
--rw-rw-rw-   0        0        0      331 2023-04-25 02:17:24.000000 d20-orm-2.0.1/test/test_crud_collection.py
--rw-rw-rw-   0        0        0      253 2023-04-25 02:17:24.000000 d20-orm-2.0.1/test/test_metadata.py
--rw-rw-rw-   0        0        0      105 2023-04-05 22:18:50.000000 d20-orm-2.0.1/test/test_params.py
+drwxrwxrwx   0        0        0        0 2023-05-27 00:03:44.839816 d20-orm-2.0.1a1/
+-rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-orm-2.0.1a1/LICENSE
+-rw-rw-rw-   0        0        0      895 2023-05-27 00:03:44.839816 d20-orm-2.0.1a1/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-04-25 02:17:24.000000 d20-orm-2.0.1a1/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-orm-2.0.1a1/pyproject.toml
+-rw-rw-rw-   0        0        0       72 2023-05-27 00:03:44.842356 d20-orm-2.0.1a1/setup.cfg
+-rw-rw-rw-   0        0        0      876 2023-05-27 00:03:12.000000 d20-orm-2.0.1a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 00:03:44.774678 d20-orm-2.0.1a1/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 00:03:44.806846 d20-orm-2.0.1a1/src/d20_orm.egg-info/
+-rw-rw-rw-   0        0        0      895 2023-05-27 00:03:44.000000 d20-orm-2.0.1a1/src/d20_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2023-05-27 00:03:44.000000 d20-orm-2.0.1a1/src/d20_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 00:03:44.000000 d20-orm-2.0.1a1/src/d20_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-27 00:03:44.000000 d20-orm-2.0.1a1/src/d20_orm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-27 00:03:44.000000 d20-orm-2.0.1a1/src/d20_orm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 00:03:44.831128 d20-orm-2.0.1a1/src/dtwentyORM/
+-rw-rw-rw-   0        0        0     8911 2023-04-25 23:14:04.000000 d20-orm-2.0.1a1/src/dtwentyORM/BasicElement.py
+-rw-rw-rw-   0        0        0     7213 2023-05-27 00:02:43.000000 d20-orm-2.0.1a1/src/dtwentyORM/DBConnector.py
+-rw-rw-rw-   0        0        0     4749 2023-04-26 00:06:49.000000 d20-orm-2.0.1a1/src/dtwentyORM/Element.py
+-rw-rw-rw-   0        0        0     7462 2023-04-06 00:37:34.000000 d20-orm-2.0.1a1/src/dtwentyORM/Error.py
+-rw-rw-rw-   0        0        0     3632 2023-04-18 00:32:09.000000 d20-orm-2.0.1a1/src/dtwentyORM/GraphClassFactory.py
+-rw-rw-rw-   0        0        0     5136 2023-04-26 01:16:05.000000 d20-orm-2.0.1a1/src/dtwentyORM/Metadata.py
+-rw-rw-rw-   0        0        0       95 2023-04-06 00:37:34.000000 d20-orm-2.0.1a1/src/dtwentyORM/__init__.py
+-rw-rw-rw-   0        0        0      161 2023-02-28 02:21:55.000000 d20-orm-2.0.1a1/src/dtwentyORM/__version__.py
+-rw-rw-rw-   0        0        0     1427 2023-04-18 00:31:28.000000 d20-orm-2.0.1a1/src/dtwentyORM/support.py
+drwxrwxrwx   0        0        0        0 2023-05-27 00:03:44.838802 d20-orm-2.0.1a1/test/
+-rw-rw-rw-   0        0        0      476 2023-04-25 02:17:24.000000 d20-orm-2.0.1a1/test/test_basic_element_test.py
+-rw-rw-rw-   0        0        0      611 2023-04-25 02:17:24.000000 d20-orm-2.0.1a1/test/test_build_db.py
+-rw-rw-rw-   0        0        0      331 2023-04-25 02:17:24.000000 d20-orm-2.0.1a1/test/test_crud_collection.py
+-rw-rw-rw-   0        0        0      253 2023-04-25 02:17:24.000000 d20-orm-2.0.1a1/test/test_metadata.py
+-rw-rw-rw-   0        0        0      105 2023-04-05 22:18:50.000000 d20-orm-2.0.1a1/test/test_params.py
```

### Comparing `d20-orm-2.0.1/LICENSE` & `d20-orm-2.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.1/PKG-INFO` & `d20-orm-2.0.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-orm
-Version: 2.0.1
+Version: 2.0.1a1
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/arangodb_python_orm
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/arangodb_python_orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-orm-2.0.1/setup.py` & `d20-orm-2.0.1a1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="d20-orm",
-    version="2.0.1",
+    version="2.0.1a1",
     author="Alex Sánchez Vega",
     author_email="alex@d20.services",
     description="A small ORM for multimodel DBs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/d20services/arangodb_python_orm",
     project_urls={
```

### Comparing `d20-orm-2.0.1/src/d20_orm.egg-info/PKG-INFO` & `d20-orm-2.0.1a1/src/d20_orm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-orm
-Version: 2.0.1
+Version: 2.0.1a1
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/arangodb_python_orm
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/arangodb_python_orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-orm-2.0.1/src/d20_orm.egg-info/SOURCES.txt` & `d20-orm-2.0.1a1/src/d20_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.1/src/dtwentyORM/BasicElement.py` & `d20-orm-2.0.1a1/src/dtwentyORM/BasicElement.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.1/src/dtwentyORM/DBConnector.py` & `d20-orm-2.0.1a1/src/dtwentyORM/DBConnector.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import json
 import re
 
 class DBConnector():
 
 
-    def __init__(self, db_name=None, conf={}, create_if_not_exists=False):
+    def __init__(self, db_name=None, conf=None, create_if_not_exists=False):
         if type(conf) == dict:
             arangoURL= conf.get(f'DBURL', json.loads(os.environ.get(f'DBURL', None)))
             username=conf.get(f'DBUSERNAME', os.environ.get(f'DBUSERNAME',  None))
             password=conf.get(f'DBPASSWORD', os.environ.get(f'DBPASSWORD', None))
         else:
             arangoURL=json.loads(os.environ.get(f'DBURL', None))
             username=os.environ.get(f'DBUSERNAME', None)
```

### Comparing `d20-orm-2.0.1/src/dtwentyORM/Element.py` & `d20-orm-2.0.1a1/src/dtwentyORM/Element.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.1/src/dtwentyORM/Error.py` & `d20-orm-2.0.1a1/src/dtwentyORM/Error.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.1/src/dtwentyORM/GraphClassFactory.py` & `d20-orm-2.0.1a1/src/dtwentyORM/GraphClassFactory.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.1/src/dtwentyORM/Metadata.py` & `d20-orm-2.0.1a1/src/dtwentyORM/Metadata.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.1/src/dtwentyORM/support.py` & `d20-orm-2.0.1a1/src/dtwentyORM/support.py`

 * *Files identical despite different names*

### Comparing `d20-orm-2.0.1/test/test_build_db.py` & `d20-orm-2.0.1a1/test/test_build_db.py`

 * *Files identical despite different names*

