# Comparing `tmp/exc2dic-1.0.2.tar.gz` & `tmp/exc2dic-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exc2dic-1.0.2.tar", last modified: Sat May 27 09:38:36 2023, max compression
+gzip compressed data, was "exc2dic-1.0.3.tar", last modified: Sat May 27 09:40:29 2023, max compression
```

## Comparing `exc2dic-1.0.2.tar` & `exc2dic-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:38:36.691665 exc2dic-1.0.2/
--rw-r--r--   0 hmy        (501) staff       (20)      201 2023-05-27 09:38:36.691512 exc2dic-1.0.2/PKG-INFO
-drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:38:36.690623 exc2dic-1.0.2/exc2dic/
--rw-r--r--   0 hmy        (501) staff       (20)       33 2023-05-27 09:36:26.000000 exc2dic-1.0.2/exc2dic/__init__.py
--rw-r--r--   0 hmy        (501) staff       (20)     1196 2023-05-27 09:00:58.000000 exc2dic-1.0.2/exc2dic/read_dict.py
-drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:38:36.691312 exc2dic-1.0.2/exc2dic.egg-info/
--rw-r--r--   0 hmy        (501) staff       (20)      201 2023-05-27 09:38:36.000000 exc2dic-1.0.2/exc2dic.egg-info/PKG-INFO
--rw-r--r--   0 hmy        (501) staff       (20)      203 2023-05-27 09:38:36.000000 exc2dic-1.0.2/exc2dic.egg-info/SOURCES.txt
--rw-r--r--   0 hmy        (501) staff       (20)        1 2023-05-27 09:38:36.000000 exc2dic-1.0.2/exc2dic.egg-info/dependency_links.txt
--rw-r--r--   0 hmy        (501) staff       (20)        7 2023-05-27 09:38:36.000000 exc2dic-1.0.2/exc2dic.egg-info/requires.txt
--rw-r--r--   0 hmy        (501) staff       (20)        8 2023-05-27 09:38:36.000000 exc2dic-1.0.2/exc2dic.egg-info/top_level.txt
--rw-r--r--   0 hmy        (501) staff       (20)       38 2023-05-27 09:38:36.691717 exc2dic-1.0.2/setup.cfg
--rw-r--r--   0 hmy        (501) staff       (20)      326 2023-05-27 09:38:12.000000 exc2dic-1.0.2/setup.py
+drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:40:29.917566 exc2dic-1.0.3/
+-rw-r--r--   0 hmy        (501) staff       (20)      201 2023-05-27 09:40:29.917422 exc2dic-1.0.3/PKG-INFO
+drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:40:29.916348 exc2dic-1.0.3/exc2dic/
+-rw-r--r--   0 hmy        (501) staff       (20)       32 2023-05-27 09:39:59.000000 exc2dic-1.0.3/exc2dic/__init__.py
+-rw-r--r--   0 hmy        (501) staff       (20)     1196 2023-05-27 09:00:58.000000 exc2dic-1.0.3/exc2dic/read_dict.py
+drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:40:29.917222 exc2dic-1.0.3/exc2dic.egg-info/
+-rw-r--r--   0 hmy        (501) staff       (20)      201 2023-05-27 09:40:29.000000 exc2dic-1.0.3/exc2dic.egg-info/PKG-INFO
+-rw-r--r--   0 hmy        (501) staff       (20)      203 2023-05-27 09:40:29.000000 exc2dic-1.0.3/exc2dic.egg-info/SOURCES.txt
+-rw-r--r--   0 hmy        (501) staff       (20)        1 2023-05-27 09:40:29.000000 exc2dic-1.0.3/exc2dic.egg-info/dependency_links.txt
+-rw-r--r--   0 hmy        (501) staff       (20)        7 2023-05-27 09:40:29.000000 exc2dic-1.0.3/exc2dic.egg-info/requires.txt
+-rw-r--r--   0 hmy        (501) staff       (20)        8 2023-05-27 09:40:29.000000 exc2dic-1.0.3/exc2dic.egg-info/top_level.txt
+-rw-r--r--   0 hmy        (501) staff       (20)       38 2023-05-27 09:40:29.917612 exc2dic-1.0.3/setup.cfg
+-rw-r--r--   0 hmy        (501) staff       (20)      326 2023-05-27 09:40:07.000000 exc2dic-1.0.3/setup.py
```

### Comparing `exc2dic-1.0.2/exc2dic/read_dict.py` & `exc2dic-1.0.3/exc2dic/read_dict.py`

 * *Files identical despite different names*

