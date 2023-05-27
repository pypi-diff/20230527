# Comparing `tmp/dtbase-0.0.1.tar.gz` & `tmp/dtbase-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtbase-0.0.1.tar", max compression
+gzip compressed data, was "dtbase-0.0.2.tar", max compression
```

## Comparing `dtbase-0.0.1.tar` & `dtbase-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-26 19:06:50.655580 dtbase-0.0.1/dtbase/__init__.py
--rw-r--r--   0        0        0     5281 2023-05-26 23:45:18.887306 dtbase-0.0.1/dtbase/config.py
--rw-r--r--   0        0        0     5723 2023-05-26 23:41:03.392028 dtbase-0.0.1/dtbase/engine.py
--rw-r--r--   0        0        0      369 2023-05-26 23:51:45.540892 dtbase-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      632 2023-05-26 23:53:01.085302 dtbase-0.0.1/setup.py
--rw-r--r--   0        0        0      412 2023-05-26 23:53:01.085498 dtbase-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-05-26 23:58:37.938978 dtbase-0.0.2/dtbase/__init__.py
+-rw-r--r--   0        0        0     5281 2023-05-26 23:45:18.887306 dtbase-0.0.2/dtbase/config.py
+-rw-r--r--   0        0        0     5718 2023-05-26 23:58:37.934512 dtbase-0.0.2/dtbase/engine.py
+-rw-r--r--   0        0        0      369 2023-05-26 23:58:37.937495 dtbase-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      632 2023-05-26 23:58:47.685747 dtbase-0.0.2/setup.py
+-rw-r--r--   0        0        0      412 2023-05-26 23:58:47.685947 dtbase-0.0.2/PKG-INFO
```

### Comparing `dtbase-0.0.1/dtbase/config.py` & `dtbase-0.0.2/dtbase/config.py`

 * *Files identical despite different names*

### Comparing `dtbase-0.0.1/dtbase/engine.py` & `dtbase-0.0.2/dtbase/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-__all__ = [
-		'DetaBase',
-]
+__all__ = ['DetaBase']
 
 from typing import Union, Optional
 from deta import Deta
 from dhint.hints import *
 from .config import DetaConfig
```

### Comparing `dtbase-0.0.1/setup.py` & `dtbase-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['deta[async]==1.1.0a2', 'dhint>=0.0.5,<0.0.6', 'starlette>=0.27.0,<0.28.0']
 
 setup_kwargs = {
     'name': 'dtbase',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

