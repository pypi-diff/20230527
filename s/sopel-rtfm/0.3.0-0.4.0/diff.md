# Comparing `tmp/sopel-rtfm-0.3.0.tar.gz` & `tmp/sopel-rtfm-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel-rtfm-0.3.0.tar", last modified: Thu Oct  7 15:44:41 2021, max compression
+gzip compressed data, was "sopel-rtfm-0.4.0.tar", last modified: Sat May 27 16:40:40 2023, max compression
```

## Comparing `sopel-rtfm-0.3.0.tar` & `sopel-rtfm-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 dgw       (1000) dgw       (1000)        0 2021-10-07 15:45:14.156679 sopel-rtfm-0.3.0/
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)     1022 2021-06-17 11:28:29.000000 sopel-rtfm-0.3.0/COPYING
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)      109 2021-06-17 11:28:29.000000 sopel-rtfm-0.3.0/MANIFEST.in
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)      571 2021-10-07 15:44:28.000000 sopel-rtfm-0.3.0/NEWS
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)     2686 2021-10-07 15:45:14.156679 sopel-rtfm-0.3.0/PKG-INFO
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)      945 2021-06-17 12:44:47.000000 sopel-rtfm-0.3.0/README.md
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)      729 2021-10-07 15:45:14.161680 sopel-rtfm-0.3.0/setup.cfg
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)      687 2021-06-17 11:28:29.000000 sopel-rtfm-0.3.0/setup.py
-drwxrwxrwx   0 dgw       (1000) dgw       (1000)        0 2021-10-07 15:45:14.037676 sopel-rtfm-0.3.0/sopel_rtfm/
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)     4663 2021-10-07 15:40:12.000000 sopel-rtfm-0.3.0/sopel_rtfm/__init__.py
-drwxrwxrwx   0 dgw       (1000) dgw       (1000)        0 2021-10-07 15:45:14.142712 sopel-rtfm-0.3.0/sopel_rtfm.egg-info/
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)     2686 2021-10-07 15:45:13.000000 sopel-rtfm-0.3.0/sopel_rtfm.egg-info/PKG-INFO
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)      315 2021-10-07 15:45:13.000000 sopel-rtfm-0.3.0/sopel_rtfm.egg-info/SOURCES.txt
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)        1 2021-10-07 15:45:13.000000 sopel-rtfm-0.3.0/sopel_rtfm.egg-info/dependency_links.txt
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)       35 2021-10-07 15:45:13.000000 sopel-rtfm-0.3.0/sopel_rtfm.egg-info/entry_points.txt
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)        1 2021-06-17 12:28:42.000000 sopel-rtfm-0.3.0/sopel_rtfm.egg-info/not-zip-safe
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)       29 2021-10-07 15:45:13.000000 sopel-rtfm-0.3.0/sopel_rtfm.egg-info/requires.txt
--rwxrwxrwx   0 dgw       (1000) dgw       (1000)       11 2021-10-07 15:45:13.000000 sopel-rtfm-0.3.0/sopel_rtfm.egg-info/top_level.txt
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-05-27 16:40:40.091105 sopel-rtfm-0.4.0/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     1022 2023-05-27 16:32:27.000000 sopel-rtfm-0.4.0/COPYING
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      109 2023-05-27 16:32:27.000000 sopel-rtfm-0.4.0/MANIFEST.in
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      652 2023-05-27 16:39:39.000000 sopel-rtfm-0.4.0/NEWS
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     2214 2023-05-27 16:40:40.091105 sopel-rtfm-0.4.0/PKG-INFO
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      945 2023-05-27 16:32:27.000000 sopel-rtfm-0.4.0/README.md
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      729 2023-05-27 16:40:40.092605 sopel-rtfm-0.4.0/setup.cfg
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      687 2023-05-27 16:32:27.000000 sopel-rtfm-0.4.0/setup.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-05-27 16:40:40.067135 sopel-rtfm-0.4.0/sopel_rtfm/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     4671 2023-05-27 16:32:27.000000 sopel-rtfm-0.4.0/sopel_rtfm/__init__.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-05-27 16:40:40.090105 sopel-rtfm-0.4.0/sopel_rtfm.egg-info/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     2214 2023-05-27 16:40:39.000000 sopel-rtfm-0.4.0/sopel_rtfm.egg-info/PKG-INFO
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      315 2023-05-27 16:40:39.000000 sopel-rtfm-0.4.0/sopel_rtfm.egg-info/SOURCES.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-05-27 16:40:39.000000 sopel-rtfm-0.4.0/sopel_rtfm.egg-info/dependency_links.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       34 2023-05-27 16:40:39.000000 sopel-rtfm-0.4.0/sopel_rtfm.egg-info/entry_points.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-05-27 16:40:39.000000 sopel-rtfm-0.4.0/sopel_rtfm.egg-info/not-zip-safe
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       29 2023-05-27 16:40:39.000000 sopel-rtfm-0.4.0/sopel_rtfm.egg-info/requires.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       11 2023-05-27 16:40:39.000000 sopel-rtfm-0.4.0/sopel_rtfm.egg-info/top_level.txt
```

### Comparing `sopel-rtfm-0.3.0/COPYING` & `sopel-rtfm-0.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `sopel-rtfm-0.3.0/NEWS` & `sopel-rtfm-0.4.0/NEWS`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+0.4.0
+=====
+
+Added:
+* `.docs` command alias, for when `.rtfm` feels harsh (#2)
+
+
 0.3.0
 =====
 
 Added:
 * Proper help output for `.rtfm` command (#1)
 
 Changed:
```

### Comparing `sopel-rtfm-0.3.0/README.md` & `sopel-rtfm-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sopel-rtfm-0.3.0/setup.cfg` & `sopel-rtfm-0.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sopel-rtfm
-version = 0.3.0
+version = 0.4.0
 description = A plugin to suggest documentation links when someone asks a basic question.
 author = dgw
 author_email = dgw@technobabbl.es
 url = https://github.com/sopel-irc/sopel-rtfm
 license = Eiffel Forum License, version 2
 classifiers = 
 	Intended Audience :: Developers
```

### Comparing `sopel-rtfm-0.3.0/setup.py` & `sopel-rtfm-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `sopel-rtfm-0.3.0/sopel_rtfm/__init__.py` & `sopel-rtfm-0.4.0/sopel_rtfm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     for key in ['rtfm_base', 'rtfm_inventory', 'rtfm_objects']:
         try:
             del bot.memory[key]
         except KeyError:
             pass
 
 
-@module.commands('rtfm')
+@module.commands('rtfm', 'docs')
 @module.example('.rtfm bind_host')
 @module.output_prefix('[rtfm] ')
 def suggest_doc_link(bot, trigger):
     """Search the configured Sphinx object inventory and output a link to the best match."""
     query = trigger.group(2)
 
     if not query:
```

