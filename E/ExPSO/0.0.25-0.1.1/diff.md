# Comparing `tmp/ExPSO-0.0.25.tar.gz` & `tmp/ExPSO-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExPSO-0.0.25.tar", last modified: Sat May 27 07:24:29 2023, max compression
+gzip compressed data, was "ExPSO-0.1.1.tar", last modified: Sat May 27 07:35:15 2023, max compression
```

## Comparing `ExPSO-0.0.25.tar` & `ExPSO-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 07:24:29.164837 ExPSO-0.0.25/
--rw-rw-rw-   0        0        0    35560 2023-05-07 11:50:19.000000 ExPSO-0.0.25/LICENSE
--rw-rw-rw-   0        0        0      862 2023-05-27 07:24:29.164837 ExPSO-0.0.25/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2023-05-27 07:20:41.000000 ExPSO-0.0.25/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 07:24:29.165859 ExPSO-0.0.25/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 07:24:29.097881 ExPSO-0.0.25/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 07:24:29.157833 ExPSO-0.0.25/src/ExPSO/
--rw-rw-rw-   0        0        0     9942 2023-05-27 07:08:41.000000 ExPSO-0.0.25/src/ExPSO/ExPSOClass.py
--rw-rw-rw-   0        0        0      124 2023-05-07 10:18:51.000000 ExPSO-0.0.25/src/ExPSO/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 07:24:29.163837 ExPSO-0.0.25/src/ExPSO.egg-info/
--rw-rw-rw-   0        0        0      862 2023-05-27 07:24:28.000000 ExPSO-0.0.25/src/ExPSO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-05-27 07:24:28.000000 ExPSO-0.0.25/src/ExPSO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 07:24:28.000000 ExPSO-0.0.25/src/ExPSO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-27 07:24:28.000000 ExPSO-0.0.25/src/ExPSO.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 07:35:15.337696 ExPSO-0.1.1/
+-rw-rw-rw-   0        0        0    35560 2023-05-07 11:50:19.000000 ExPSO-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    16539 2023-05-27 07:35:15.335695 ExPSO-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    15676 2023-05-27 07:32:24.000000 ExPSO-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1041 2023-05-27 07:32:07.000000 ExPSO-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 07:35:15.337696 ExPSO-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 07:35:15.274618 ExPSO-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 07:35:15.317681 ExPSO-0.1.1/src/ExPSO/
+-rw-rw-rw-   0        0        0     9942 2023-05-27 07:08:41.000000 ExPSO-0.1.1/src/ExPSO/ExPSOClass.py
+-rw-rw-rw-   0        0        0      124 2023-05-07 10:18:51.000000 ExPSO-0.1.1/src/ExPSO/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 07:35:15.331693 ExPSO-0.1.1/src/ExPSO.egg-info/
+-rw-rw-rw-   0        0        0    16539 2023-05-27 07:35:15.000000 ExPSO-0.1.1/src/ExPSO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-05-27 07:35:15.000000 ExPSO-0.1.1/src/ExPSO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 07:35:15.000000 ExPSO-0.1.1/src/ExPSO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-27 07:35:15.000000 ExPSO-0.1.1/src/ExPSO.egg-info/top_level.txt
```

### Comparing `ExPSO-0.0.25/LICENSE` & `ExPSO-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ExPSO-0.0.25/pyproject.toml` & `ExPSO-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   "scikit-learn"
 ]
 
 
 
 [project]
 name = "ExPSO"
-version = "0.0.25"
+version = "0.1.1"
 authors = [
   { name="Insaf Kraidia", email="insaf.kraidia@univ-constantine2.dz" },
   { name="Khelil Kassoul", email="khelil.kassoul@etu.unige.ch" },
   { name="Samir Brahim Belhaouari", email="sbelhaouari@hbku.edu.qa" },
   { name="Naoufel Cheikhrouhou",email="naoufel.cheikhrouhou@hesge.ch"},
   { name="Nicolas Zufferey",email="nicolas.zufferey.1@ulaval.ca"}
```

### Comparing `ExPSO-0.0.25/src/ExPSO/ExPSOClass.py` & `ExPSO-0.1.1/src/ExPSO/ExPSOClass.py`

 * *Files identical despite different names*

