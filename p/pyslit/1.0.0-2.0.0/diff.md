# Comparing `tmp/pyslit-1.0.0.tar.gz` & `tmp/pyslit-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslit-1.0.0.tar", last modified: Fri May 26 19:07:24 2023, max compression
+gzip compressed data, was "pyslit-2.0.0.tar", last modified: Sat May 27 08:45:22 2023, max compression
```

## Comparing `pyslit-1.0.0.tar` & `pyslit-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,24 @@
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
+drwxrwxrwx   0        0        0        0 2023-05-27 08:45:22.863635 pyslit-2.0.0/
+-rw-rw-rw-   0        0        0     1082 2023-05-26 04:35:22.000000 pyslit-2.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      100 2023-05-27 08:27:39.000000 pyslit-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5597 2023-05-27 08:45:22.861636 pyslit-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5054 2023-05-27 06:37:03.000000 pyslit-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 08:45:22.805928 pyslit-2.0.0/pyslit/
+drwxrwxrwx   0        0        0        0 2023-05-27 08:45:22.844647 pyslit-2.0.0/pyslit/src/
+-rw-rw-rw-   0        0        0     8551 2023-05-27 08:25:37.000000 pyslit-2.0.0/pyslit/src/Music_player.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:45:22.858639 pyslit-2.0.0/pyslit/src/images/
+-rw-rw-rw-   0        0        0     4647 2021-10-02 04:07:19.000000 pyslit-2.0.0/pyslit/src/images/back.png
+-rw-rw-rw-   0        0        0     7903 2023-04-13 20:36:41.000000 pyslit-2.0.0/pyslit/src/images/forward.png
+-rw-rw-rw-   0        0        0     6782 2023-05-25 05:06:50.000000 pyslit-2.0.0/pyslit/src/images/icon.ico
+-rw-rw-rw-   0        0        0     4126 2021-10-02 04:07:19.000000 pyslit-2.0.0/pyslit/src/images/pause.png
+-rw-rw-rw-   0        0        0     4489 2021-10-02 04:07:19.000000 pyslit-2.0.0/pyslit/src/images/play.png
+-rw-rw-rw-   0        0        0      463 2021-10-02 04:07:19.000000 pyslit-2.0.0/pyslit/src/images/stop.png
+drwxrwxrwx   0        0        0        0 2023-05-27 08:45:22.840649 pyslit-2.0.0/pyslit/src/pyslit.egg-info/
+-rw-rw-rw-   0        0        0     5597 2023-05-27 08:45:22.000000 pyslit-2.0.0/pyslit/src/pyslit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2023-05-27 08:45:22.000000 pyslit-2.0.0/pyslit/src/pyslit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 08:45:22.000000 pyslit-2.0.0/pyslit/src/pyslit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-05-27 08:45:22.000000 pyslit-2.0.0/pyslit/src/pyslit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-27 08:45:22.000000 pyslit-2.0.0/pyslit/src/pyslit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13303 2023-05-27 06:24:57.000000 pyslit-2.0.0/pyslit/src/pyslit.py
+-rw-rw-rw-   0        0        0       42 2023-05-27 08:45:22.863635 pyslit-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1708 2023-05-27 08:44:50.000000 pyslit-2.0.0/setup.py
```

### Comparing `pyslit-1.0.0/LICENSE.txt` & `pyslit-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

