# Comparing `tmp/IMDBTraktSyncer-1.3.1.tar.gz` & `tmp/IMDBTraktSyncer-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.3.1.tar", last modified: Thu May 25 05:35:37 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.3.2.tar", last modified: Fri May 26 22:09:11 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.3.1.tar` & `IMDBTraktSyncer-1.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 05:35:37.782499 IMDBTraktSyncer-1.3.1/
-drwxrwxrwx   0        0        0        0 2023-05-25 05:35:37.761485 IMDBTraktSyncer-1.3.1/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    22309 2023-05-25 05:33:53.000000 IMDBTraktSyncer-1.3.1/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.3.1/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1900 2023-05-23 23:43:19.000000 IMDBTraktSyncer-1.3.1/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4207 2023-05-24 23:10:07.000000 IMDBTraktSyncer-1.3.1/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3845 2023-05-20 20:45:06.000000 IMDBTraktSyncer-1.3.1/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     7752 2023-05-24 22:03:34.000000 IMDBTraktSyncer-1.3.1/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.3.1/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     6982 2023-05-25 05:26:36.000000 IMDBTraktSyncer-1.3.1/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-25 05:35:37.779485 IMDBTraktSyncer-1.3.1/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     8573 2023-05-25 05:35:37.000000 IMDBTraktSyncer-1.3.1/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-05-25 05:35:37.000000 IMDBTraktSyncer-1.3.1/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 05:35:37.000000 IMDBTraktSyncer-1.3.1/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-25 05:35:37.000000 IMDBTraktSyncer-1.3.1/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-25 05:35:37.000000 IMDBTraktSyncer-1.3.1/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-25 05:35:37.000000 IMDBTraktSyncer-1.3.1/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     8573 2023-05-25 05:35:37.781486 IMDBTraktSyncer-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     7856 2023-05-25 05:31:18.000000 IMDBTraktSyncer-1.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-25 05:35:37.783484 IMDBTraktSyncer-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1370 2023-05-25 05:33:43.000000 IMDBTraktSyncer-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 22:09:11.047336 IMDBTraktSyncer-1.3.2/
+drwxrwxrwx   0        0        0        0 2023-05-26 22:09:11.015326 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    22309 2023-05-25 05:33:53.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1900 2023-05-23 23:43:19.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4207 2023-05-24 23:10:07.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3858 2023-05-26 22:03:46.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     7752 2023-05-24 22:03:34.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     6982 2023-05-25 05:26:36.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-26 22:09:11.044336 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     8573 2023-05-26 22:09:10.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-05-26 22:09:10.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 22:09:10.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-26 22:09:10.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-26 22:09:10.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-26 22:09:10.000000 IMDBTraktSyncer-1.3.2/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     8573 2023-05-26 22:09:11.046325 IMDBTraktSyncer-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7856 2023-05-25 05:31:18.000000 IMDBTraktSyncer-1.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-26 22:09:11.047336 IMDBTraktSyncer-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1370 2023-05-26 22:04:29.000000 IMDBTraktSyncer-1.3.2/setup.py
```

### Comparing `IMDBTraktSyncer-1.3.1/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.1/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.1/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.1/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/errorHandling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import traceback
 import requests
+import time
 try:
     from IMDBTraktSyncer import verifyCredentials as VC
 except ImportError:
     import verifyCredentials as VC
 
 def report_error(error_message):
     github_issue_url = "https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/new?template=bug_report.yml"
```

### Comparing `IMDBTraktSyncer-1.3.1/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/imdbData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.1/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.1/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.3.2/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.1/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.3.2/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.3.1
+Version: 1.3.2
 Summary: This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.3.1/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.3.2/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.1/LICENSE` & `IMDBTraktSyncer-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.1/PKG-INFO` & `IMDBTraktSyncer-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.3.1
+Version: 1.3.2
 Summary: This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.3.1/README.md` & `IMDBTraktSyncer-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.1/setup.py` & `IMDBTraktSyncer-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.3.1'
+VERSION = '1.3.2'
 DESCRIPTION = 'This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

