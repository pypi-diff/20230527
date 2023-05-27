# Comparing `tmp/digital_unit-1.5.4.tar.gz` & `tmp/digital_unit-1.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital_unit-1.5.4.tar", last modified: Sat May 27 05:53:16 2023, max compression
+gzip compressed data, was "digital_unit-1.5b0.tar", last modified: Thu May 25 14:15:13 2023, max compression
```

## Comparing `digital_unit-1.5.4.tar` & `digital_unit-1.5b0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 05:53:16.884515 digital_unit-1.5.4/
--rw-rw-rw-   0        0        0     1998 2023-05-27 05:53:16.885515 digital_unit-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     1713 2023-05-27 05:52:29.000000 digital_unit-1.5.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 05:53:16.867517 digital_unit-1.5.4/digital_unit/
--rw-rw-rw-   0        0        0     1010 2023-05-27 05:45:16.000000 digital_unit-1.5.4/digital_unit/Area.py
--rw-rw-rw-   0        0        0      797 2023-05-24 12:55:26.000000 digital_unit-1.5.4/digital_unit/Lenth.py
--rw-rw-rw-   0        0        0     1003 2023-05-27 05:42:32.000000 digital_unit-1.5.4/digital_unit/Volume.py
--rw-rw-rw-   0        0        0      137 2023-05-27 05:29:59.000000 digital_unit-1.5.4/digital_unit/__init__.py
--rw-rw-rw-   0        0        0     1050 2023-05-24 14:05:13.000000 digital_unit-1.5.4/digital_unit/root.py
--rw-rw-rw-   0        0        0      330 2023-05-25 13:54:40.000000 digital_unit-1.5.4/digital_unit/sample.py
-drwxrwxrwx   0        0        0        0 2023-05-27 05:53:16.881515 digital_unit-1.5.4/digital_unit.egg-info/
--rw-rw-rw-   0        0        0     1998 2023-05-27 05:53:16.000000 digital_unit-1.5.4/digital_unit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-05-27 05:53:16.000000 digital_unit-1.5.4/digital_unit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 05:53:16.000000 digital_unit-1.5.4/digital_unit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-27 05:53:16.000000 digital_unit-1.5.4/digital_unit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-27 05:53:16.886515 digital_unit-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0      956 2023-05-27 05:53:10.000000 digital_unit-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:15:13.849369 digital_unit-1.5b0/
+-rw-rw-rw-   0        0        0      240 2023-05-25 14:15:13.848379 digital_unit-1.5b0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-25 14:15:13.831365 digital_unit-1.5b0/digital_unit/
+-rw-rw-rw-   0        0        0      827 2023-05-24 12:55:31.000000 digital_unit-1.5b0/digital_unit/Area.py
+-rw-rw-rw-   0        0        0      797 2023-05-24 12:55:26.000000 digital_unit-1.5b0/digital_unit/Lenth.py
+-rw-rw-rw-   0        0        0      169 2023-05-25 14:12:42.000000 digital_unit-1.5b0/digital_unit/__init__.py
+-rw-rw-rw-   0        0        0     1050 2023-05-24 14:05:13.000000 digital_unit-1.5b0/digital_unit/root.py
+-rw-rw-rw-   0        0        0      330 2023-05-25 13:54:40.000000 digital_unit-1.5b0/digital_unit/sample.py
+-rw-rw-rw-   0        0        0      294 2023-05-25 14:15:08.000000 digital_unit-1.5b0/digital_unit/volume.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:15:13.845265 digital_unit-1.5b0/digital_unit.egg-info/
+-rw-rw-rw-   0        0        0      240 2023-05-25 14:15:13.000000 digital_unit-1.5b0/digital_unit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-25 14:15:13.000000 digital_unit-1.5b0/digital_unit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 14:15:13.000000 digital_unit-1.5b0/digital_unit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-25 14:15:13.000000 digital_unit-1.5b0/digital_unit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 14:15:13.850380 digital_unit-1.5b0/setup.cfg
+-rw-rw-rw-   0        0        0      776 2023-05-25 14:08:23.000000 digital_unit-1.5b0/setup.py
```

### Comparing `digital_unit-1.5.4/digital_unit/Area.py` & `digital_unit-1.5b0/digital_unit/Area.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,20 +23,13 @@
         self.measure = 10_000.0
     def __str__(self) -> str:
         return 'hm²'
 
 class SquareCentiMeter(Area):
     def __init__(self) -> None:
         super().__init__()
-        self.measure = 0.0001
+        self.measure = 1.0
     def __str__(self) -> str:
         return 'cm²'
-    
-class SquareDecimeter(Area):
-    def __init__(self) -> None:
-        super().__init__()
-        self.measure = 0.01
-    def __str__(self) -> str:
-        return 'dm²'
```

### Comparing `digital_unit-1.5.4/digital_unit/Lenth.py` & `digital_unit-1.5b0/digital_unit/Lenth.py`

 * *Files identical despite different names*

### Comparing `digital_unit-1.5.4/digital_unit/root.py` & `digital_unit-1.5b0/digital_unit/root.py`

 * *Files identical despite different names*

### Comparing `digital_unit-1.5.4/setup.py` & `digital_unit-1.5b0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from distutils.core import setup
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
 setup(
   name = 'digital_unit',         # How you named your package folder (MyLib)
   packages = ['digital_unit'],   # Chose the same as "name"
-  version = '1.5.4',      # Start with a small number and increase it with every change you make
+  version = '1.5b0',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'number and units',   # Give a short description about your library
   author = 'st201109',                   # Type in your name
   author_email = 'st20110913@outlook.com',      # Type in your E-Mail
   
   keywords = ['SOME', 'MEANINGFULL', 'MATH'],   # Keywords that define your package best
-  long_description = long_description,
-  long_description_content_type="text/markdown",
 
   classifiers=[ 
     'Programming Language :: Python :: 3.6',
-
   ],
 )
```

