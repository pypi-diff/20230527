# Comparing `tmp/bonbast-0.5.5.tar.gz` & `tmp/bonbast-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bonbast-0.5.5.tar", last modified: Sun May  7 22:13:50 2023, max compression
+gzip compressed data, was "bonbast-0.5.6.tar", last modified: Sat May 27 16:49:28 2023, max compression
```

## Comparing `bonbast-0.5.5.tar` & `bonbast-0.5.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:50.398656 bonbast-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-07 22:13:18.000000 bonbast-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-05-07 22:13:50.398656 bonbast-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-07 22:13:18.000000 bonbast-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-07 22:13:18.000000 bonbast-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 22:13:50.398656 bonbast-0.5.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-05-07 22:13:18.000000 bonbast-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:50.382656 bonbast-0.5.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:50.390656 bonbast-0.5.5/src/bonbast/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:50.394656 bonbast-0.5.5/src/bonbast/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/helpers/click_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/helpers/currency_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:50.394656 bonbast-0.5.5/src/bonbast/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/managers/storage_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/managers/token_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:50.398656 bonbast-0.5.5/src/bonbast/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/models/coin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/models/currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/models/gold.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/models/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/models/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-07 22:13:18.000000 bonbast-0.5.5/src/bonbast/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:13:50.390656 bonbast-0.5.5/src/bonbast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-05-07 22:13:50.000000 bonbast-0.5.5/src/bonbast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-07 22:13:50.000000 bonbast-0.5.5/src/bonbast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 22:13:50.000000 bonbast-0.5.5/src/bonbast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-07 22:13:50.000000 bonbast-0.5.5/src/bonbast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-07 22:13:50.000000 bonbast-0.5.5/src/bonbast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-07 22:13:50.000000 bonbast-0.5.5/src/bonbast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:49:28.275555 bonbast-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-27 16:49:05.000000 bonbast-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-05-27 16:49:28.275555 bonbast-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-27 16:49:05.000000 bonbast-0.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-27 16:49:05.000000 bonbast-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 16:49:28.275555 bonbast-0.5.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-05-27 16:49:05.000000 bonbast-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:49:28.271555 bonbast-0.5.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:49:28.271555 bonbast-0.5.6/src/bonbast/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:49:28.271555 bonbast-0.5.6/src/bonbast/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/helpers/click_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/helpers/currency_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:49:28.271555 bonbast-0.5.6/src/bonbast/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/managers/storage_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/managers/token_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:49:28.275555 bonbast-0.5.6/src/bonbast/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/models/coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/models/currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/models/gold.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/models/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-27 16:49:05.000000 bonbast-0.5.6/src/bonbast/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:49:28.271555 bonbast-0.5.6/src/bonbast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-05-27 16:49:28.000000 bonbast-0.5.6/src/bonbast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-27 16:49:28.000000 bonbast-0.5.6/src/bonbast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 16:49:28.000000 bonbast-0.5.6/src/bonbast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 16:49:28.000000 bonbast-0.5.6/src/bonbast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-27 16:49:28.000000 bonbast-0.5.6/src/bonbast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-27 16:49:28.000000 bonbast-0.5.6/src/bonbast.egg-info/top_level.txt
```

### Comparing `bonbast-0.5.5/LICENSE` & `bonbast-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.5/PKG-INFO` & `bonbast-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonbast
-Version: 0.5.5
+Version: 0.5.6
 Summary: Get currencies exchange rates for IRR from Bonbast.com
 Author-email: Amir Hossein SamadiPour <samadipoor2@gmail.com>, Alireza Azadi <alireza_azadi@hotmail.com>, Iliya Aghamajidi <dozheiny@gmail.com>, Parsa Shahmaleki <parsampsh@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Amir Hossein SamadiPour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bonbast-0.5.5/README.md` & `bonbast-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.5/pyproject.toml` & `bonbast-0.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bonbast"
-version = "0.5.5"
+version = "0.5.6"
 description = "Get currencies exchange rates for IRR from Bonbast.com"
 readme = "README.md"
 authors = [
     { name = "Amir Hossein SamadiPour", email = "samadipoor2@gmail.com" },
     { name = "Alireza Azadi", email = "alireza_azadi@hotmail.com" },
     { name = "Iliya Aghamajidi", email = "dozheiny@gmail.com" },
     { name = "Parsa Shahmaleki", email = "parsampsh@gmail.com" },
@@ -37,15 +37,15 @@
 
 [project.urls]
 repository = "https://github.com/SamadiPour/bonbast"
 #documentation = ""
 
 
 [tool.bumpver]
-current_version = "0.5.5"
+current_version = "0.5.6"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `bonbast-0.5.5/src/bonbast/helpers/click_callbacks.py` & `bonbast-0.5.6/src/bonbast/helpers/click_callbacks.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.5/src/bonbast/helpers/currency_flags.py` & `bonbast-0.5.6/src/bonbast/helpers/currency_flags.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.5/src/bonbast/helpers/utils.py` & `bonbast-0.5.6/src/bonbast/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.5/src/bonbast/main.py` & `bonbast-0.5.6/src/bonbast/main.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.5/src/bonbast/managers/storage_manager.py` & `bonbast-0.5.6/src/bonbast/managers/storage_manager.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.5/src/bonbast/managers/token_manager.py` & `bonbast-0.5.6/src/bonbast/managers/token_manager.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.5/src/bonbast/models/coin.py` & `bonbast-0.5.6/src/bonbast/models/coin.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.5/src/bonbast/models/currency.py` & `bonbast-0.5.6/src/bonbast/models/currency.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.5/src/bonbast/models/gold.py` & `bonbast-0.5.6/src/bonbast/models/gold.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.5/src/bonbast/models/token.py` & `bonbast-0.5.6/src/bonbast/models/token.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.5/src/bonbast/server.py` & `bonbast-0.5.6/src/bonbast/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 try:
     from .models import *
 except ImportError:
     from models import *
 
 BASE_URL = 'https://www.bonbast.com'
-USER_AGENT = 'Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) ' \
-             'Chrome/103.0.0.0 Mobile Safari/537.36'
+USER_AGENT = 'Mozilla/5.0 (Linux; Android 12.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) ' \
+             'Chrome/113.0.0.0 Mobile Safari/537.36'
 SELL = '1'
 BUY = '2'
 
 
 def int_try_parse(value) -> Optional[int]:
     try:
         return int(value)
@@ -50,18 +50,18 @@
     }
 
     try:
         r = requests.get(BASE_URL, headers=headers)
         r.raise_for_status()
     except requests.exceptions.HTTPError as err:
         raise SystemExit(err)
-    except requests.exceptions.ConnectionError as _:
+    except requests.exceptions.ConnectionError:
         raise SystemExit('Error: Failed to connect to bonbast')
 
-    search = re.search(r"param\s*=\s*\"(.+)\"", r.text, re.MULTILINE)
+    search = re.search(r"param\s*[=:]\s*\"(.+)\"", r.text, re.MULTILINE)
     if search is None or search.group(1) is None:
         raise SystemExit('Error: token not found in the main page')
 
     return search.group(1)
 
 
 def get_prices_from_api(token: str) -> Tuple[List[Currency], List[Coin], List[Gold]]:
@@ -73,39 +73,34 @@
         It will return False instead.
     """
     headers = {
         'authority': 'bonbast.com',
         'accept': 'application/json, text/javascript, */*; q=0.01',
         'accept-language': 'en-US,en;q=0.9,fa;q=0.8',
         'content-type': 'application/x-www-form-urlencoded; charset=UTF-8',
-        'cookie': 'cookieconsent_status=true; st_bb=0',
+        'cookie': 'st_bb=0',
         'origin': 'https://bonbast.com',
         'referer': 'https://bonbast.com/',
         'sec-ch-ua': '".Not/A)Brand";v="99", "Google Chrome";v="103", "Chromium";v="103"',
         'sec-ch-ua-mobile': '?1',
         'sec-ch-ua-platform': '"Android"',
         'sec-fetch-dest': 'empty',
         'sec-fetch-mode': 'cors',
         'sec-fetch-site': 'same-origin',
         'user-agent': USER_AGENT,
         'x-requested-with': 'XMLHttpRequest',
     }
 
-    data = {
-        'data': token,
-        'webdriver': 'false',
-    }
-
     try:
-        r = requests.post(f'{BASE_URL}/json', headers=headers, data=data)
+        r = requests.post(f'{BASE_URL}/json', headers=headers, data={'param': token})
         r.raise_for_status()
         r = r.json()
     except requests.exceptions.HTTPError as err:
         raise SystemExit(err)
-    except requests.exceptions.ConnectionError as _:
+    except requests.exceptions.ConnectionError:
         raise SystemExit('Error: Failed to connect to bonbast')
 
     if 'reset' in r:
         raise ResetAPIError('Error: token is expired')
 
     currencies: List[Currency] = []
     coins: List[Coin] = []
```

### Comparing `bonbast-0.5.5/src/bonbast/tables.py` & `bonbast-0.5.6/src/bonbast/tables.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.5/src/bonbast.egg-info/PKG-INFO` & `bonbast-0.5.6/src/bonbast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonbast
-Version: 0.5.5
+Version: 0.5.6
 Summary: Get currencies exchange rates for IRR from Bonbast.com
 Author-email: Amir Hossein SamadiPour <samadipoor2@gmail.com>, Alireza Azadi <alireza_azadi@hotmail.com>, Iliya Aghamajidi <dozheiny@gmail.com>, Parsa Shahmaleki <parsampsh@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Amir Hossein SamadiPour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bonbast-0.5.5/src/bonbast.egg-info/SOURCES.txt` & `bonbast-0.5.6/src/bonbast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

