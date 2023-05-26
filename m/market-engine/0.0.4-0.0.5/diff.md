# Comparing `tmp/market-engine-0.0.4.tar.gz` & `tmp/market-engine-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market-engine-0.0.4.tar", last modified: Fri May 26 19:30:56 2023, max compression
+gzip compressed data, was "market-engine-0.0.5.tar", last modified: Fri May 26 22:45:43 2023, max compression
```

## Comparing `market-engine-0.0.4.tar` & `market-engine-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 19:30:56.023705 market-engine-0.0.4/
--rw-rw-rw-   0        0        0      216 2023-05-26 19:30:56.023705 market-engine-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 19:30:56.016704 market-engine-0.0.4/market_engine/
--rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.0.4/market_engine/__init__.py
--rw-rw-rw-   0        0        0      932 2023-05-26 19:30:35.000000 market-engine-0.0.4/market_engine/common.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:30:56.022704 market-engine-0.0.4/market_engine/modules/
--rw-rw-rw-   0        0        0    14007 2023-05-26 19:26:37.000000 market-engine-0.0.4/market_engine/modules/MarketAPI.py
--rw-rw-rw-   0        0        0     6989 2023-05-26 19:26:52.000000 market-engine-0.0.4/market_engine/modules/MarketDB.py
--rw-rw-rw-   0        0        0    14973 2023-05-26 19:26:44.000000 market-engine-0.0.4/market_engine/modules/MarketData.py
--rw-rw-rw-   0        0        0        0 2023-05-26 19:04:43.000000 market-engine-0.0.4/market_engine/modules/__init__.py
--rw-rw-rw-   0        0        0    38904 2023-05-26 19:04:00.000000 market-engine-0.0.4/market_engine/modules/categories.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:30:56.019705 market-engine-0.0.4/market_engine.egg-info/
--rw-rw-rw-   0        0        0      216 2023-05-26 19:30:55.000000 market-engine-0.0.4/market_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2023-05-26 19:30:55.000000 market-engine-0.0.4/market_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 19:30:55.000000 market-engine-0.0.4/market_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-05-26 19:30:55.000000 market-engine-0.0.4/market_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-26 19:30:55.000000 market-engine-0.0.4/market_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 19:30:56.023705 market-engine-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-05-26 19:30:45.000000 market-engine-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 22:45:43.736065 market-engine-0.0.5/
+-rw-rw-rw-   0        0        0      216 2023-05-26 22:45:43.736065 market-engine-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-26 22:45:43.730561 market-engine-0.0.5/market_engine/
+-rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.0.5/market_engine/__init__.py
+-rw-rw-rw-   0        0        0      932 2023-05-26 19:30:35.000000 market-engine-0.0.5/market_engine/common.py
+drwxrwxrwx   0        0        0        0 2023-05-26 22:45:43.734561 market-engine-0.0.5/market_engine/modules/
+-rw-rw-rw-   0        0        0    14007 2023-05-26 19:26:37.000000 market-engine-0.0.5/market_engine/modules/MarketAPI.py
+-rw-rw-rw-   0        0        0     6989 2023-05-26 19:26:52.000000 market-engine-0.0.5/market_engine/modules/MarketDB.py
+-rw-rw-rw-   0        0        0    15043 2023-05-26 22:45:19.000000 market-engine-0.0.5/market_engine/modules/MarketData.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 19:04:43.000000 market-engine-0.0.5/market_engine/modules/__init__.py
+-rw-rw-rw-   0        0        0    38904 2023-05-26 19:04:00.000000 market-engine-0.0.5/market_engine/modules/categories.py
+drwxrwxrwx   0        0        0        0 2023-05-26 22:45:43.733561 market-engine-0.0.5/market_engine.egg-info/
+-rw-rw-rw-   0        0        0      216 2023-05-26 22:45:43.000000 market-engine-0.0.5/market_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2023-05-26 22:45:43.000000 market-engine-0.0.5/market_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 22:45:43.000000 market-engine-0.0.5/market_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-05-26 22:45:43.000000 market-engine-0.0.5/market_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-26 22:45:43.000000 market-engine-0.0.5/market_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 22:45:43.736065 market-engine-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-05-26 22:45:35.000000 market-engine-0.0.5/setup.py
```

### Comparing `market-engine-0.0.4/market_engine/common.py` & `market-engine-0.0.5/market_engine/common.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.0.4/market_engine/modules/MarketAPI.py` & `market-engine-0.0.5/market_engine/modules/MarketAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.0.4/market_engine/modules/MarketDB.py` & `market-engine-0.0.5/market_engine/modules/MarketDB.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.0.4/market_engine/modules/MarketData.py` & `market-engine-0.0.5/market_engine/modules/MarketData.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,19 @@
 
     return best_match if best_score >= threshold else None
 
 
 def remove_common_words(name: str, common_words: set) -> str:
     name = remove_blueprint(name)
     threshold = 80  # Adjust this value based on the desired level of fuzzy matching
-
+    
+    ignore_list = ['primed']
+    
     words = name.split()
-    filtered_words = [word for word in words if not closest_common_word(word, common_words, threshold)]
+    filtered_words = [word for word in words if not (closest_common_word(word, common_words, threshold) and word not in ignore_list)]
     return ' '.join(filtered_words)
 
 
 def remove_blueprint(s: str) -> str:
     words = s.lower().split()
     if words[-1:] == ['blueprint'] and words[-2] not in ['prime', 'wraith', 'vandal']:
         return ' '.join(words[:-1])
```

### Comparing `market-engine-0.0.4/market_engine/modules/categories.py` & `market-engine-0.0.5/market_engine/modules/categories.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.0.4/setup.py` & `market-engine-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='market-engine',
-    version='0.0.4',
+    version='0.0.5',
     description='Engine for easily getting the orders, statistics, and other stats from warframe.market.',
     author='Jacob McBride',
     author_email='jake55111@gmail.com',
     packages=find_packages(),
     install_requires=[
         'aiohttp~=3.8.4',
         'discord~=2.2.2',
```

