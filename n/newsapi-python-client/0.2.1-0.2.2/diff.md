# Comparing `tmp/newsapi-python-client-0.2.1.tar.gz` & `tmp/newsapi-python-client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newsapi-python-client-0.2.1.tar", last modified: Sat May 27 10:32:55 2023, max compression
+gzip compressed data, was "newsapi-python-client-0.2.2.tar", last modified: Sat May 27 10:38:28 2023, max compression
```

## Comparing `newsapi-python-client-0.2.1.tar` & `newsapi-python-client-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 10:32:55.119563 newsapi-python-client-0.2.1/
--rw-rw-rw-   0        0        0     1086 2023-05-27 09:04:11.000000 newsapi-python-client-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     2941 2023-05-27 10:32:55.118563 newsapi-python-client-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2086 2023-05-27 09:04:11.000000 newsapi-python-client-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 10:32:55.104564 newsapi-python-client-0.2.1/models/
--rw-rw-rw-   0        0        0        0 2023-05-27 09:05:25.000000 newsapi-python-client-0.2.1/models/__init__.py
--rw-rw-rw-   0        0        0     1580 2023-05-27 09:32:29.000000 newsapi-python-client-0.2.1/models/request_model.py
--rw-rw-rw-   0        0        0     1699 2023-05-27 09:31:28.000000 newsapi-python-client-0.2.1/models/response_model.py
-drwxrwxrwx   0        0        0        0 2023-05-27 10:32:55.115563 newsapi-python-client-0.2.1/newsapi_python_client.egg-info/
--rw-rw-rw-   0        0        0     2941 2023-05-27 10:32:55.000000 newsapi-python-client-0.2.1/newsapi_python_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-05-27 10:32:55.000000 newsapi-python-client-0.2.1/newsapi_python_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 10:32:55.000000 newsapi-python-client-0.2.1/newsapi_python_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-27 10:32:55.000000 newsapi-python-client-0.2.1/newsapi_python_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-27 10:32:55.000000 newsapi-python-client-0.2.1/newsapi_python_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 10:32:55.117564 newsapi-python-client-0.2.1/services/
--rw-rw-rw-   0        0        0        0 2023-05-27 09:13:02.000000 newsapi-python-client-0.2.1/services/__init__.py
--rw-rw-rw-   0        0        0     1033 2023-05-27 09:30:02.000000 newsapi-python-client-0.2.1/services/news_service.py
--rw-rw-rw-   0        0        0       42 2023-05-27 10:32:55.119563 newsapi-python-client-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1323 2023-05-27 10:32:42.000000 newsapi-python-client-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:38:28.029616 newsapi-python-client-0.2.2/
+-rw-rw-rw-   0        0        0     1086 2023-05-27 09:04:11.000000 newsapi-python-client-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     3099 2023-05-27 10:38:28.029616 newsapi-python-client-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2244 2023-05-27 10:37:45.000000 newsapi-python-client-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 10:38:28.013615 newsapi-python-client-0.2.2/models/
+-rw-rw-rw-   0        0        0        0 2023-05-27 09:05:25.000000 newsapi-python-client-0.2.2/models/__init__.py
+-rw-rw-rw-   0        0        0     1580 2023-05-27 09:32:29.000000 newsapi-python-client-0.2.2/models/request_model.py
+-rw-rw-rw-   0        0        0     1699 2023-05-27 09:31:28.000000 newsapi-python-client-0.2.2/models/response_model.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:38:28.025617 newsapi-python-client-0.2.2/newsapi_python_client.egg-info/
+-rw-rw-rw-   0        0        0     3099 2023-05-27 10:38:27.000000 newsapi-python-client-0.2.2/newsapi_python_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-05-27 10:38:27.000000 newsapi-python-client-0.2.2/newsapi_python_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 10:38:27.000000 newsapi-python-client-0.2.2/newsapi_python_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-27 10:38:27.000000 newsapi-python-client-0.2.2/newsapi_python_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-27 10:38:27.000000 newsapi-python-client-0.2.2/newsapi_python_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 10:38:28.027615 newsapi-python-client-0.2.2/services/
+-rw-rw-rw-   0        0        0        0 2023-05-27 09:13:02.000000 newsapi-python-client-0.2.2/services/__init__.py
+-rw-rw-rw-   0        0        0     1033 2023-05-27 09:30:02.000000 newsapi-python-client-0.2.2/services/news_service.py
+-rw-rw-rw-   0        0        0       42 2023-05-27 10:38:28.029616 newsapi-python-client-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1323 2023-05-27 10:38:22.000000 newsapi-python-client-0.2.2/setup.py
```

### Comparing `newsapi-python-client-0.2.1/LICENSE` & `newsapi-python-client-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `newsapi-python-client-0.2.1/PKG-INFO` & `newsapi-python-client-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newsapi-python-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python client to interact with News API from NewApi.org
 Home-page: https://github.com/roachseb/NewsAPI-Python-Client
 Author: Roach Sebastien
 Author-email: sebastien.r.r@hotmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -37,14 +37,21 @@
 ## Installation
 
 ```bash
 pip install newsapi-python-client
 ```
 
 ## Usage
+Create a secrets.json file in the base directory of the project with the following structure:
+
+```json
+{
+    "NEWS_API_KEY": "YOUR_NEWS_API_KEY"
+}
+```
 
 ```python
 from services.news_service import get_finance_news
 from models.request_model import RequestModel
 
 request_model = RequestModel(
     q='finance',
```

### Comparing `newsapi-python-client-0.2.1/README.md` & `newsapi-python-client-0.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,21 @@
 ## Installation
 
 ```bash
 pip install newsapi-python-client
 ```
 
 ## Usage
+Create a secrets.json file in the base directory of the project with the following structure:
+
+```json
+{
+    "NEWS_API_KEY": "YOUR_NEWS_API_KEY"
+}
+```
 
 ```python
 from services.news_service import get_finance_news
 from models.request_model import RequestModel
 
 request_model = RequestModel(
     q='finance',
```

### Comparing `newsapi-python-client-0.2.1/models/request_model.py` & `newsapi-python-client-0.2.2/models/request_model.py`

 * *Files identical despite different names*

### Comparing `newsapi-python-client-0.2.1/models/response_model.py` & `newsapi-python-client-0.2.2/models/response_model.py`

 * *Files identical despite different names*

### Comparing `newsapi-python-client-0.2.1/newsapi_python_client.egg-info/PKG-INFO` & `newsapi-python-client-0.2.2/newsapi_python_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newsapi-python-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python client to interact with News API from NewApi.org
 Home-page: https://github.com/roachseb/NewsAPI-Python-Client
 Author: Roach Sebastien
 Author-email: sebastien.r.r@hotmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -37,14 +37,21 @@
 ## Installation
 
 ```bash
 pip install newsapi-python-client
 ```
 
 ## Usage
+Create a secrets.json file in the base directory of the project with the following structure:
+
+```json
+{
+    "NEWS_API_KEY": "YOUR_NEWS_API_KEY"
+}
+```
 
 ```python
 from services.news_service import get_finance_news
 from models.request_model import RequestModel
 
 request_model = RequestModel(
     q='finance',
```

### Comparing `newsapi-python-client-0.2.1/services/news_service.py` & `newsapi-python-client-0.2.2/services/news_service.py`

 * *Files identical despite different names*

### Comparing `newsapi-python-client-0.2.1/setup.py` & `newsapi-python-client-0.2.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='newsapi-python-client',
-    version='0.2.1',
+    version='0.2.2',
     url='https://github.com/roachseb/NewsAPI-Python-Client',
     author='Roach Sebastien',
     author_email='sebastien.r.r@hotmail.com',
     packages=find_packages(exclude=['tests*']),
     install_requires=[
         'requests',
         'dataclasses;python_version<"3.7"'
```

