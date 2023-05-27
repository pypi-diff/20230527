# Comparing `tmp/exc2dic-1.0.4.tar.gz` & `tmp/exc2dic-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exc2dic-1.0.4.tar", last modified: Sat May 27 09:53:29 2023, max compression
+gzip compressed data, was "exc2dic-1.0.5.tar", last modified: Sat May 27 09:55:00 2023, max compression
```

## Comparing `exc2dic-1.0.4.tar` & `exc2dic-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:53:29.125602 exc2dic-1.0.4/
--rw-r--r--   0 hmy        (501) staff       (20)      201 2023-05-27 09:53:29.125484 exc2dic-1.0.4/PKG-INFO
-drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:53:29.124580 exc2dic-1.0.4/exc2dic/
--rw-r--r--   0 hmy        (501) staff       (20)       32 2023-05-27 09:39:59.000000 exc2dic-1.0.4/exc2dic/__init__.py
--rw-r--r--   0 hmy        (501) staff       (20)     1196 2023-05-27 09:00:58.000000 exc2dic-1.0.4/exc2dic/read_excel.py
-drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:53:29.125303 exc2dic-1.0.4/exc2dic.egg-info/
--rw-r--r--   0 hmy        (501) staff       (20)      201 2023-05-27 09:53:29.000000 exc2dic-1.0.4/exc2dic.egg-info/PKG-INFO
--rw-r--r--   0 hmy        (501) staff       (20)      204 2023-05-27 09:53:29.000000 exc2dic-1.0.4/exc2dic.egg-info/SOURCES.txt
--rw-r--r--   0 hmy        (501) staff       (20)        1 2023-05-27 09:53:29.000000 exc2dic-1.0.4/exc2dic.egg-info/dependency_links.txt
--rw-r--r--   0 hmy        (501) staff       (20)        7 2023-05-27 09:53:29.000000 exc2dic-1.0.4/exc2dic.egg-info/requires.txt
--rw-r--r--   0 hmy        (501) staff       (20)        8 2023-05-27 09:53:29.000000 exc2dic-1.0.4/exc2dic.egg-info/top_level.txt
--rw-r--r--   0 hmy        (501) staff       (20)       38 2023-05-27 09:53:29.125652 exc2dic-1.0.4/setup.cfg
--rw-r--r--   0 hmy        (501) staff       (20)      326 2023-05-27 09:51:43.000000 exc2dic-1.0.4/setup.py
+drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:55:00.193347 exc2dic-1.0.5/
+-rw-r--r--   0 hmy        (501) staff       (20)      201 2023-05-27 09:55:00.193226 exc2dic-1.0.5/PKG-INFO
+drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:55:00.192367 exc2dic-1.0.5/exc2dic/
+-rw-r--r--   0 hmy        (501) staff       (20)       33 2023-05-27 09:54:38.000000 exc2dic-1.0.5/exc2dic/__init__.py
+-rw-r--r--   0 hmy        (501) staff       (20)     1196 2023-05-27 09:00:58.000000 exc2dic-1.0.5/exc2dic/read_excel.py
+drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:55:00.193054 exc2dic-1.0.5/exc2dic.egg-info/
+-rw-r--r--   0 hmy        (501) staff       (20)      201 2023-05-27 09:55:00.000000 exc2dic-1.0.5/exc2dic.egg-info/PKG-INFO
+-rw-r--r--   0 hmy        (501) staff       (20)      204 2023-05-27 09:55:00.000000 exc2dic-1.0.5/exc2dic.egg-info/SOURCES.txt
+-rw-r--r--   0 hmy        (501) staff       (20)        1 2023-05-27 09:55:00.000000 exc2dic-1.0.5/exc2dic.egg-info/dependency_links.txt
+-rw-r--r--   0 hmy        (501) staff       (20)        7 2023-05-27 09:55:00.000000 exc2dic-1.0.5/exc2dic.egg-info/requires.txt
+-rw-r--r--   0 hmy        (501) staff       (20)        8 2023-05-27 09:55:00.000000 exc2dic-1.0.5/exc2dic.egg-info/top_level.txt
+-rw-r--r--   0 hmy        (501) staff       (20)       38 2023-05-27 09:55:00.193388 exc2dic-1.0.5/setup.cfg
+-rw-r--r--   0 hmy        (501) staff       (20)      326 2023-05-27 09:54:58.000000 exc2dic-1.0.5/setup.py
```

### Comparing `exc2dic-1.0.4/exc2dic/read_excel.py` & `exc2dic-1.0.5/exc2dic/read_excel.py`

 * *Files identical despite different names*

