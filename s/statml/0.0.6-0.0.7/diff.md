# Comparing `tmp/statml-0.0.6.tar.gz` & `tmp/statml-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statml-0.0.6.tar", last modified: Sat May 27 02:36:59 2023, max compression
+gzip compressed data, was "statml-0.0.7.tar", last modified: Sat May 27 05:46:15 2023, max compression
```

## Comparing `statml-0.0.6.tar` & `statml-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 02:36:59.120626 statml-0.0.6/
--rw-rw-rw-   0        0        0       24 2023-05-27 00:51:22.000000 statml-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      381 2023-05-27 02:36:59.120626 statml-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       16 2023-05-20 12:40:16.000000 statml-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-27 02:36:59.120626 statml-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      608 2023-05-27 02:36:39.000000 statml-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 02:36:59.104999 statml-0.0.6/statml/
--rw-rw-rw-   0        0        0       21 2023-05-27 02:36:49.000000 statml-0.0.6/statml/__init__.py
--rw-rw-rw-   0        0        0     3621 2023-05-21 11:57:23.000000 statml-0.0.6/statml/playchat.py
--rw-rw-rw-   0        0        0     5209 2023-05-21 11:26:39.000000 statml-0.0.6/statml/stepwise.py
-drwxrwxrwx   0        0        0        0 2023-05-27 02:36:59.120626 statml-0.0.6/statml.egg-info/
--rw-rw-rw-   0        0        0      381 2023-05-27 02:36:58.000000 statml-0.0.6/statml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-27 02:36:59.000000 statml-0.0.6/statml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 02:36:58.000000 statml-0.0.6/statml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-27 02:36:58.000000 statml-0.0.6/statml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 05:46:15.224240 statml-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-05-27 03:19:10.000000 statml-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      518 2023-05-27 05:46:15.224240 statml-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2023-05-20 12:40:16.000000 statml-0.0.7/README.md
+-rw-rw-rw-   0        0        0      589 2023-05-27 05:41:07.000000 statml-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      247 2023-05-27 05:46:15.224240 statml-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 05:46:15.207600 statml-0.0.7/statml/
+-rw-rw-rw-   0        0        0       21 2023-05-27 05:41:20.000000 statml-0.0.7/statml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 05:46:15.191975 statml-0.0.7/statml/onebook/
+drwxrwxrwx   0        0        0        0 2023-05-27 05:46:15.207600 statml-0.0.7/statml/onebook/1/
+-rw-rw-rw-   0        0        0    49814 2023-05-07 11:48:47.000000 statml-0.0.7/statml/onebook/1/Ch2-2.ipynb
+-rw-rw-rw-   0        0        0     3621 2023-05-21 11:57:23.000000 statml-0.0.7/statml/playchat.py
+-rw-rw-rw-   0        0        0     5209 2023-05-21 11:26:39.000000 statml-0.0.7/statml/stepwise.py
+drwxrwxrwx   0        0        0        0 2023-05-27 05:46:15.207600 statml-0.0.7/statml.egg-info/
+-rw-rw-rw-   0        0        0      518 2023-05-27 05:46:15.000000 statml-0.0.7/statml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-05-27 05:46:15.000000 statml-0.0.7/statml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 05:46:15.000000 statml-0.0.7/statml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-27 05:46:15.000000 statml-0.0.7/statml.egg-info/top_level.txt
```

### Comparing `statml-0.0.6/statml/playchat.py` & `statml-0.0.7/statml/playchat.py`

 * *Files identical despite different names*

### Comparing `statml-0.0.6/statml/stepwise.py` & `statml-0.0.7/statml/stepwise.py`

 * *Files identical despite different names*

