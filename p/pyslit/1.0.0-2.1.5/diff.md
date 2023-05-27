# Comparing `tmp/pyslit-1.0.0.tar.gz` & `tmp/pyslit-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslit-1.0.0.tar", last modified: Fri May 26 19:07:24 2023, max compression
+gzip compressed data, was "pyslit-2.1.5.tar", last modified: Sat May 27 12:09:39 2023, max compression
```

## Comparing `pyslit-1.0.0.tar` & `pyslit-2.1.5.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 19:07:23.993620 pyslit-1.0.0/
--rw-rw-rw-   0        0        0     1082 2023-05-26 04:35:22.000000 pyslit-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4061 2023-05-26 19:07:23.991427 pyslit-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3656 2023-05-26 19:06:02.000000 pyslit-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 19:07:23.945083 pyslit-1.0.0/pyslit/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:07:23.989426 pyslit-1.0.0/pyslit/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:07:23.987056 pyslit-1.0.0/pyslit/src/pyslit.egg-info/
--rw-rw-rw-   0        0        0     4061 2023-05-26 19:07:23.000000 pyslit-1.0.0/pyslit/src/pyslit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-05-26 19:07:23.000000 pyslit-1.0.0/pyslit/src/pyslit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 19:07:23.000000 pyslit-1.0.0/pyslit/src/pyslit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-26 19:07:23.000000 pyslit-1.0.0/pyslit/src/pyslit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10398 2023-05-26 18:44:27.000000 pyslit-1.0.0/pyslit/src/pyslit.py
--rw-rw-rw-   0        0        0       42 2023-05-26 19:07:23.993620 pyslit-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1263 2023-05-26 19:00:55.000000 pyslit-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 12:09:39.842187 pyslit-2.1.5/
+-rw-rw-rw-   0        0        0     1082 2023-05-26 04:35:22.000000 pyslit-2.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     5541 2023-05-27 12:09:39.842187 pyslit-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4998 2023-05-27 12:09:09.000000 pyslit-2.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 12:09:39.782341 pyslit-2.1.5/pyslit/
+drwxrwxrwx   0        0        0        0 2023-05-27 12:09:39.832653 pyslit-2.1.5/pyslit/src/
+-rw-rw-rw-   0        0        0     8622 2023-05-27 11:52:33.000000 pyslit-2.1.5/pyslit/src/Music_player.py
+drwxrwxrwx   0        0        0        0 2023-05-27 12:09:39.822651 pyslit-2.1.5/pyslit/src/pyslit.egg-info/
+-rw-rw-rw-   0        0        0     5541 2023-05-27 12:09:39.000000 pyslit-2.1.5/pyslit/src/pyslit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2023-05-27 12:09:39.000000 pyslit-2.1.5/pyslit/src/pyslit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 12:09:39.000000 pyslit-2.1.5/pyslit/src/pyslit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-05-27 12:09:39.000000 pyslit-2.1.5/pyslit/src/pyslit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-27 12:09:39.000000 pyslit-2.1.5/pyslit/src/pyslit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13307 2023-05-27 10:03:28.000000 pyslit-2.1.5/pyslit/src/pyslit.py
+-rw-rw-rw-   0        0        0       42 2023-05-27 12:09:39.842187 pyslit-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1637 2023-05-27 12:07:08.000000 pyslit-2.1.5/setup.py
```

### Comparing `pyslit-1.0.0/LICENSE.txt` & `pyslit-2.1.5/LICENSE.txt`

 * *Files identical despite different names*

