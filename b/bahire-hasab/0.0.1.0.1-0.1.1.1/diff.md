# Comparing `tmp/bahire-hasab-0.0.1.0.1.tar.gz` & `tmp/bahire-hasab-0.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bahire-hasab-0.0.1.0.1.tar", last modified: Sat May 27 08:15:02 2023, max compression
+gzip compressed data, was "bahire-hasab-0.1.1.1.tar", last modified: Sat May 27 08:38:02 2023, max compression
```

## Comparing `bahire-hasab-0.0.1.0.1.tar` & `bahire-hasab-0.1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:15:02.353632 bahire-hasab-0.0.1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-27 08:14:48.000000 bahire-hasab-0.0.1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-27 08:15:02.353632 bahire-hasab-0.0.1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-27 08:14:48.000000 bahire-hasab-0.0.1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-27 08:14:48.000000 bahire-hasab-0.0.1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 08:15:02.353632 bahire-hasab-0.0.1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-27 08:14:48.000000 bahire-hasab-0.0.1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:15:02.353632 bahire-hasab-0.0.1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:15:02.353632 bahire-hasab-0.0.1.0.1/src/bahire_hasab/
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-05-27 08:14:48.000000 bahire-hasab-0.0.1.0.1/src/bahire_hasab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:15:02.353632 bahire-hasab-0.0.1.0.1/src/bahire_hasab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-27 08:15:02.000000 bahire-hasab-0.0.1.0.1/src/bahire_hasab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-27 08:15:02.000000 bahire-hasab-0.0.1.0.1/src/bahire_hasab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 08:15:02.000000 bahire-hasab-0.0.1.0.1/src/bahire_hasab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-27 08:15:02.000000 bahire-hasab-0.0.1.0.1/src/bahire_hasab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:38:02.452838 bahire-hasab-0.1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-27 08:37:47.000000 bahire-hasab-0.1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-27 08:38:02.452838 bahire-hasab-0.1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-27 08:37:47.000000 bahire-hasab-0.1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-27 08:37:47.000000 bahire-hasab-0.1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 08:38:02.452838 bahire-hasab-0.1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-27 08:37:47.000000 bahire-hasab-0.1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:38:02.452838 bahire-hasab-0.1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:38:02.452838 bahire-hasab-0.1.1.1/src/bahire_hasab/
+-rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-05-27 08:37:47.000000 bahire-hasab-0.1.1.1/src/bahire_hasab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:38:02.452838 bahire-hasab-0.1.1.1/src/bahire_hasab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-27 08:38:02.000000 bahire-hasab-0.1.1.1/src/bahire_hasab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-27 08:38:02.000000 bahire-hasab-0.1.1.1/src/bahire_hasab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 08:38:02.000000 bahire-hasab-0.1.1.1/src/bahire_hasab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-27 08:38:02.000000 bahire-hasab-0.1.1.1/src/bahire_hasab.egg-info/top_level.txt
```

### Comparing `bahire-hasab-0.0.1.0.1/LICENSE` & `bahire-hasab-0.1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bahire-hasab-0.0.1.0.1/PKG-INFO` & `bahire-hasab-0.1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bahire-hasab
-Version: 0.0.1.0.1
+Version: 0.1.1.1
 Home-page: https://github.com/hunderaweke/bahire-hasab
 Author: Hundera Awoke
 Author-email: hunderaweke@gmail.com
 Keywords: bahire_hasab
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bahire-hasab Version: 0.0.1.0.1 Home-page: https://
+Metadata-Version: 2.1 Name: bahire-hasab Version: 0.1.1.1 Home-page: https://
 github.com/hunderaweke/bahire-hasab Author: Hundera Awoke Author-email:
 hunderaweke@gmail.com Keywords: bahire_hasab Description-Content-Type: text/
 markdown License-File: LICENSE
       ****** ð Bahire Hassab(á£áá¨ áá³á¥) ðªð¹ ð¦ ******
 - A python module for calculating Ethiopian Holidays and Lents ## Table Of
 Content - [Description](#description) - [Installation](#installation) -
 [Documentation](#documentation) - [Todo](#todo) ## Description - This is a
```

### Comparing `bahire-hasab-0.0.1.0.1/README.md` & `bahire-hasab-0.1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bahire-hasab-0.0.1.0.1/src/bahire_hasab/__init__.py` & `bahire-hasab-0.1.1.1/src/bahire_hasab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Author: Hundera Awoke
 # Date: 26/5/2023 G.C.
-# Copyright
+# Copyright (c) 2023 Hundera Awoke
 class BahireHasab:
     def __init__(self, ametemihret) -> None:
         self.ametemihret = ametemihret
         self.amete_alem = self.ametemihret + 5500
         self.wengelawi_dic = {1: "ማቴዎስ", 2: "ማርቆስ", 3: "ሉቃስ", 4: "ዮሐንስ"}
         self.months = {
             "መስከረም": 1,
@@ -117,15 +117,14 @@
 
     def find_mebaja_hamer(self) -> int:
         beale_metk = self.beale_metk
         TEWSAK = {"ቅዳሜ": 8, "እሁድ": 7, "ሰኞ": 6, "ማግሰኞ": 5, "ረቡዕ": 4, "ሐሙስ": 3, "አርብ": 2}
         self.day = self.find_day_name(month_date_string= beale_metk)
         metk = self.metk
         tewsak = TEWSAK[self.day]
-        print(metk)
         self.mebaja_hamer = tewsak + metk if tewsak + metk < 30 else tewsak
         return self.mebaja_hamer 
 
     def find_neneweh(self) -> str:
         "A function for finding the day of tsome Neneweh"
         if 15 <= self.mebaja_hamer <= 30:
             month = "ጥር"
```

### Comparing `bahire-hasab-0.0.1.0.1/src/bahire_hasab.egg-info/PKG-INFO` & `bahire-hasab-0.1.1.1/src/bahire_hasab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bahire-hasab
-Version: 0.0.1.0.1
+Version: 0.1.1.1
 Home-page: https://github.com/hunderaweke/bahire-hasab
 Author: Hundera Awoke
 Author-email: hunderaweke@gmail.com
 Keywords: bahire_hasab
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bahire-hasab Version: 0.0.1.0.1 Home-page: https://
+Metadata-Version: 2.1 Name: bahire-hasab Version: 0.1.1.1 Home-page: https://
 github.com/hunderaweke/bahire-hasab Author: Hundera Awoke Author-email:
 hunderaweke@gmail.com Keywords: bahire_hasab Description-Content-Type: text/
 markdown License-File: LICENSE
       ****** ð Bahire Hassab(á£áá¨ áá³á¥) ðªð¹ ð¦ ******
 - A python module for calculating Ethiopian Holidays and Lents ## Table Of
 Content - [Description](#description) - [Installation](#installation) -
 [Documentation](#documentation) - [Todo](#todo) ## Description - This is a
```

