# Comparing `tmp/Python Redis Caching-0.0.5.tar.gz` & `tmp/Python Redis Caching-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Python Redis Caching-0.0.5.tar", last modified: Sat May 27 16:56:44 2023, max compression
+gzip compressed data, was "Python Redis Caching-0.0.6.tar", last modified: Sat May 27 17:10:45 2023, max compression
```

## Comparing `Python Redis Caching-0.0.5.tar` & `Python Redis Caching-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hoang     (1000) hoang     (1000)        0 2023-05-27 16:56:44.125930 Python Redis Caching-0.0.5/
--rw-rw-r--   0 hoang     (1000) hoang     (1000)      589 2023-05-27 16:56:44.125930 Python Redis Caching-0.0.5/PKG-INFO
-drwxrwxr-x   0 hoang     (1000) hoang     (1000)        0 2023-05-27 16:56:44.125930 Python Redis Caching-0.0.5/Python_Redis_Caching.egg-info/
--rw-rw-r--   0 hoang     (1000) hoang     (1000)      589 2023-05-27 16:56:44.000000 Python Redis Caching-0.0.5/Python_Redis_Caching.egg-info/PKG-INFO
--rw-rw-r--   0 hoang     (1000) hoang     (1000)      315 2023-05-27 16:56:44.000000 Python Redis Caching-0.0.5/Python_Redis_Caching.egg-info/SOURCES.txt
--rw-rw-r--   0 hoang     (1000) hoang     (1000)        1 2023-05-27 16:56:44.000000 Python Redis Caching-0.0.5/Python_Redis_Caching.egg-info/dependency_links.txt
--rw-rw-r--   0 hoang     (1000) hoang     (1000)        6 2023-05-27 16:56:44.000000 Python Redis Caching-0.0.5/Python_Redis_Caching.egg-info/requires.txt
--rw-rw-r--   0 hoang     (1000) hoang     (1000)       12 2023-05-27 16:56:44.000000 Python Redis Caching-0.0.5/Python_Redis_Caching.egg-info/top_level.txt
--rw-rw-r--   0 hoang     (1000) hoang     (1000)       13 2023-05-27 16:19:28.000000 Python Redis Caching-0.0.5/README.md
--rw-rw-r--   0 hoang     (1000) hoang     (1000)       95 2023-05-27 16:44:00.000000 Python Redis Caching-0.0.5/pyproject.toml
-drwxrwxr-x   0 hoang     (1000) hoang     (1000)        0 2023-05-27 16:56:44.125930 Python Redis Caching-0.0.5/redis_cache/
--rw-rw-r--   0 hoang     (1000) hoang     (1000)        0 2023-05-27 16:17:19.000000 Python Redis Caching-0.0.5/redis_cache/__init__.py
--rw-rw-r--   0 hoang     (1000) hoang     (1000)      983 2023-05-27 16:16:35.000000 Python Redis Caching-0.0.5/redis_cache/cache_manager.py
--rw-rw-r--   0 hoang     (1000) hoang     (1000)      559 2023-05-27 16:56:44.125930 Python Redis Caching-0.0.5/setup.cfg
--rw-rw-r--   0 hoang     (1000) hoang     (1000)      761 2023-05-27 16:56:37.000000 Python Redis Caching-0.0.5/setup.py
+drwxrwxr-x   0 hoang     (1000) hoang     (1000)        0 2023-05-27 17:10:45.922758 Python Redis Caching-0.0.6/
+-rw-rw-r--   0 hoang     (1000) hoang     (1000)      930 2023-05-27 17:10:45.922758 Python Redis Caching-0.0.6/PKG-INFO
+drwxrwxr-x   0 hoang     (1000) hoang     (1000)        0 2023-05-27 17:10:45.922758 Python Redis Caching-0.0.6/Python_Redis_Caching.egg-info/
+-rw-rw-r--   0 hoang     (1000) hoang     (1000)      930 2023-05-27 17:10:45.000000 Python Redis Caching-0.0.6/Python_Redis_Caching.egg-info/PKG-INFO
+-rw-rw-r--   0 hoang     (1000) hoang     (1000)      315 2023-05-27 17:10:45.000000 Python Redis Caching-0.0.6/Python_Redis_Caching.egg-info/SOURCES.txt
+-rw-rw-r--   0 hoang     (1000) hoang     (1000)        1 2023-05-27 17:10:45.000000 Python Redis Caching-0.0.6/Python_Redis_Caching.egg-info/dependency_links.txt
+-rw-rw-r--   0 hoang     (1000) hoang     (1000)        6 2023-05-27 17:10:45.000000 Python Redis Caching-0.0.6/Python_Redis_Caching.egg-info/requires.txt
+-rw-rw-r--   0 hoang     (1000) hoang     (1000)       12 2023-05-27 17:10:45.000000 Python Redis Caching-0.0.6/Python_Redis_Caching.egg-info/top_level.txt
+-rw-rw-r--   0 hoang     (1000) hoang     (1000)      354 2023-05-27 17:04:31.000000 Python Redis Caching-0.0.6/README.md
+-rw-rw-r--   0 hoang     (1000) hoang     (1000)       95 2023-05-27 16:44:00.000000 Python Redis Caching-0.0.6/pyproject.toml
+drwxrwxr-x   0 hoang     (1000) hoang     (1000)        0 2023-05-27 17:10:45.922758 Python Redis Caching-0.0.6/redis_cache/
+-rw-rw-r--   0 hoang     (1000) hoang     (1000)        0 2023-05-27 16:17:19.000000 Python Redis Caching-0.0.6/redis_cache/__init__.py
+-rw-rw-r--   0 hoang     (1000) hoang     (1000)      962 2023-05-27 17:09:33.000000 Python Redis Caching-0.0.6/redis_cache/cache_manager.py
+-rw-rw-r--   0 hoang     (1000) hoang     (1000)      559 2023-05-27 17:10:45.922758 Python Redis Caching-0.0.6/setup.cfg
+-rw-rw-r--   0 hoang     (1000) hoang     (1000)      761 2023-05-27 17:10:00.000000 Python Redis Caching-0.0.6/setup.py
```

### Comparing `Python Redis Caching-0.0.5/Python_Redis_Caching.egg-info/PKG-INFO` & `Python Redis Caching-0.0.6/Python_Redis_Caching.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 Metadata-Version: 2.1
 Name: Python-Redis-Caching
-Version: 0.0.5
+Version: 0.0.6
 Summary: Caching your data to Redis
 Home-page: https://github.com/nbmhoang/python-redis-caching
 Author: Hoang Nguyen
 Author-email: minhhoangnguyenbao99@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# Hello World
+# Use Redis as a backend for caching
+
+```python
+from redis_cache.cache_manager import CacheManager
+from datetime import timedelta
+from time import sleep
+
+cache = CacheManager('localhost', port=6379, db=1, expiration=timedelta(days=1))
+
+def sum(a, b):
+    sleep(2)
+    return a + b
+
+cache('S', sum, 8, 5) # Took 2.1s
+cache('S', sum, 8, 5) # Took 1.8ms
+```
```

### Comparing `Python Redis Caching-0.0.5/redis_cache/cache_manager.py` & `Python Redis Caching-0.0.6/redis_cache/cache_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from datetime import timedelta
 
 from typing import Callable
 
 class CacheManager:
 
     def __init__(self, host, port=6379, db=1, expiration=timedelta(days=1)) -> None:
-        self.redis_cli = redis.Redis(host=host, port=port, decode_responses=True, db=db)
-        self.expiration = expiration
+        self._redis_cli = redis.Redis(host=host, port=port, decode_responses=True, db=db)
+        self._expiration = expiration
     
     def _save_to_cache(self, key: str, data: dict) -> None:
-        self.redis_cli.set(key, json.dumps(data), ex=self.expiration)
+        self._redis_cli.set(key, json.dumps(data), ex=self._expiration)
 
     def _get_from_cache(self, key: str) -> dict | None:
-        if not self.redis_cli.exists(key):
+        if not self._redis_cli.exists(key):
             return None
-        return json.loads(self.redis_cli.get(key))
+        return json.loads(self._redis_cli.get(key))
 
     def use_cache(self, key: str, f: Callable, *args, **kwargs):
-        full_key = f'{key}_{hash(args)}_{hash(json.dumps(kwargs))}'
+        full_key = f'{key}_{hash(args)}'
         cache_data = self._get_from_cache(full_key)
         if cache_data is not None:
             return cache_data
         result = f(*args, **kwargs)
         self._save_to_cache(full_key, result)
         return result
```

### Comparing `Python Redis Caching-0.0.5/setup.cfg` & `Python Redis Caching-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Python Redis Caching
-version = 0.0.4
+version = 0.0.6
 author = Hoang Nguyen
 author_email = minhhoangnguyenbao99@gmail.com
 description = Caching your data to Redis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nbmhoang/python-redis-caching
 classifiers =
```

### Comparing `Python Redis Caching-0.0.5/setup.py` & `Python Redis Caching-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='Python Redis Caching',
-    version='0.0.5',
+    version='0.0.6',
     author='Hoang Nguyen',
     author_email='minhhoangnguyenbao99@gmail.com',
     description='Caching your data to Redis',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nbmhoang/python-redis-caching',
     install_requires=[
```

