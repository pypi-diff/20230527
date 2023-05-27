# Comparing `tmp/madtypes-0.0.1.tar.gz` & `tmp/madtypes-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madtypes-0.0.1.tar", last modified: Sat May 27 00:52:59 2023, max compression
+gzip compressed data, was "madtypes-0.0.2.tar", last modified: Sat May 27 09:19:48 2023, max compression
```

## Comparing `madtypes-0.0.1.tar` & `madtypes-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 r17       (1000) r17       (1000)        0 2023-05-27 00:52:59.200938 madtypes-0.0.1/
--rw-rw-r--   0 r17       (1000) r17       (1000)      566 2023-05-27 00:52:59.200938 madtypes-0.0.1/PKG-INFO
--rw-rw-r--   0 r17       (1000) r17       (1000)     1025 2023-05-27 00:41:27.000000 madtypes-0.0.1/README.md
-drwxrwxr-x   0 r17       (1000) r17       (1000)        0 2023-05-27 00:52:59.200938 madtypes-0.0.1/madtypes/
--rw-rw-r--   0 r17       (1000) r17       (1000)     2608 2023-05-26 23:42:28.000000 madtypes-0.0.1/madtypes/__init__.py
-drwxrwxr-x   0 r17       (1000) r17       (1000)        0 2023-05-27 00:52:59.200938 madtypes-0.0.1/madtypes.egg-info/
--rw-rw-r--   0 r17       (1000) r17       (1000)      566 2023-05-27 00:52:59.000000 madtypes-0.0.1/madtypes.egg-info/PKG-INFO
--rw-rw-r--   0 r17       (1000) r17       (1000)      188 2023-05-27 00:52:59.000000 madtypes-0.0.1/madtypes.egg-info/SOURCES.txt
--rw-rw-r--   0 r17       (1000) r17       (1000)        1 2023-05-27 00:52:59.000000 madtypes-0.0.1/madtypes.egg-info/dependency_links.txt
--rw-rw-r--   0 r17       (1000) r17       (1000)        9 2023-05-27 00:52:59.000000 madtypes-0.0.1/madtypes.egg-info/top_level.txt
--rw-rw-r--   0 r17       (1000) r17       (1000)       38 2023-05-27 00:52:59.200938 madtypes-0.0.1/setup.cfg
--rw-rw-r--   0 r17       (1000) r17       (1000)      736 2023-05-27 00:52:52.000000 madtypes-0.0.1/setup.py
-drwxrwxr-x   0 r17       (1000) r17       (1000)        0 2023-05-27 00:52:59.200938 madtypes-0.0.1/tests/
--rw-rw-r--   0 r17       (1000) r17       (1000)     7201 2023-05-26 23:36:14.000000 madtypes-0.0.1/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:19:48.574770 madtypes-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-27 09:19:48.574770 madtypes-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-27 09:19:36.000000 madtypes-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:19:48.570770 madtypes-0.0.2/madtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-27 09:19:36.000000 madtypes-0.0.2/madtypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:19:48.574770 madtypes-0.0.2/madtypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-27 09:19:48.000000 madtypes-0.0.2/madtypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-27 09:19:48.000000 madtypes-0.0.2/madtypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:19:48.000000 madtypes-0.0.2/madtypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-27 09:19:48.000000 madtypes-0.0.2/madtypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 09:19:48.574770 madtypes-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-27 09:19:36.000000 madtypes-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:19:48.574770 madtypes-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-05-27 09:19:36.000000 madtypes-0.0.2/tests/test_schema.py
```

### Comparing `madtypes-0.0.1/madtypes/__init__.py` & `madtypes-0.0.2/madtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `madtypes-0.0.1/setup.py` & `madtypes-0.0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
+with open("README.md", "r") as f:
+    long_description = f.read()
+
 setup(
     name="madtypes",
-    version="0.0.1",
+    version="0.0.2",
     author="6r17",
     author_email="patrick.borowy@proton.me",
     description="Python typing that will raise TypeError at runtime",
-    long_description="""
-    # https://github.com/6r17/madtypes
-    - 💢 Python class typing that will raise TypeError at runtime
-    - 📖 Render to dict or json
-    - 🌐 [Json-Schema](https://json-schema.org/)
-    """,
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/6r17/madtypes",
     packages=find_packages(include=["madtypes"]),
-    keywords="typing",
+    keywords=["typing", "json", "json-schema"],
+    python_requires=">=3.9",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `madtypes-0.0.1/tests/test_schema.py` & `madtypes-0.0.2/tests/test_schema.py`

 * *Files identical despite different names*

