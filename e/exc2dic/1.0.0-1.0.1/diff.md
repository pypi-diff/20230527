# Comparing `tmp/exc2dic-1.0.0.tar.gz` & `tmp/exc2dic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exc2dic-1.0.0.tar", last modified: Sat May 27 09:15:34 2023, max compression
+gzip compressed data, was "exc2dic-1.0.1.tar", last modified: Sat May 27 09:32:06 2023, max compression
```

## Comparing `exc2dic-1.0.0.tar` & `exc2dic-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:15:34.471144 exc2dic-1.0.0/
--rw-r--r--   0 hmy        (501) staff       (20)      201 2023-05-27 09:15:34.471025 exc2dic-1.0.0/PKG-INFO
-drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:15:34.470697 exc2dic-1.0.0/exc2dic.egg-info/
--rw-r--r--   0 hmy        (501) staff       (20)      201 2023-05-27 09:15:34.000000 exc2dic-1.0.0/exc2dic.egg-info/PKG-INFO
--rw-r--r--   0 hmy        (501) staff       (20)      186 2023-05-27 09:15:34.000000 exc2dic-1.0.0/exc2dic.egg-info/SOURCES.txt
--rw-r--r--   0 hmy        (501) staff       (20)        1 2023-05-27 09:15:34.000000 exc2dic-1.0.0/exc2dic.egg-info/dependency_links.txt
--rw-r--r--   0 hmy        (501) staff       (20)        7 2023-05-27 09:15:34.000000 exc2dic-1.0.0/exc2dic.egg-info/requires.txt
--rw-r--r--   0 hmy        (501) staff       (20)       11 2023-05-27 09:15:34.000000 exc2dic-1.0.0/exc2dic.egg-info/top_level.txt
-drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:15:34.470830 exc2dic-1.0.0/excel2dict/
--rw-r--r--   0 hmy        (501) staff       (20)     1196 2023-05-27 09:00:58.000000 exc2dic-1.0.0/excel2dict/read_dict.py
--rw-r--r--   0 hmy        (501) staff       (20)       38 2023-05-27 09:15:34.471186 exc2dic-1.0.0/setup.cfg
--rw-r--r--   0 hmy        (501) staff       (20)      329 2023-05-27 09:14:46.000000 exc2dic-1.0.0/setup.py
+drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:32:06.766264 exc2dic-1.0.1/
+-rw-r--r--   0 hmy        (501) staff       (20)      201 2023-05-27 09:32:06.766120 exc2dic-1.0.1/PKG-INFO
+drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:32:06.765213 exc2dic-1.0.1/exc2dic.egg-info/
+-rw-r--r--   0 hmy        (501) staff       (20)      201 2023-05-27 09:32:06.000000 exc2dic-1.0.1/exc2dic.egg-info/PKG-INFO
+-rw-r--r--   0 hmy        (501) staff       (20)      209 2023-05-27 09:32:06.000000 exc2dic-1.0.1/exc2dic.egg-info/SOURCES.txt
+-rw-r--r--   0 hmy        (501) staff       (20)        1 2023-05-27 09:32:06.000000 exc2dic-1.0.1/exc2dic.egg-info/dependency_links.txt
+-rw-r--r--   0 hmy        (501) staff       (20)        7 2023-05-27 09:32:06.000000 exc2dic-1.0.1/exc2dic.egg-info/requires.txt
+-rw-r--r--   0 hmy        (501) staff       (20)       11 2023-05-27 09:32:06.000000 exc2dic-1.0.1/exc2dic.egg-info/top_level.txt
+drwxr-xr-x   0 hmy        (501) staff       (20)        0 2023-05-27 09:32:06.765699 exc2dic-1.0.1/excel2dict/
+-rw-r--r--   0 hmy        (501) staff       (20)       34 2023-05-27 09:30:35.000000 exc2dic-1.0.1/excel2dict/__init__.py
+-rw-r--r--   0 hmy        (501) staff       (20)     1196 2023-05-27 09:00:58.000000 exc2dic-1.0.1/excel2dict/read_dict.py
+-rw-r--r--   0 hmy        (501) staff       (20)       38 2023-05-27 09:32:06.766322 exc2dic-1.0.1/setup.cfg
+-rw-r--r--   0 hmy        (501) staff       (20)      329 2023-05-27 09:31:06.000000 exc2dic-1.0.1/setup.py
```

### Comparing `exc2dic-1.0.0/excel2dict/read_dict.py` & `exc2dic-1.0.1/excel2dict/read_dict.py`

 * *Files identical despite different names*

