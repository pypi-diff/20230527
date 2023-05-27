# Comparing `tmp/lasfile-0.1.6.tar.gz` & `tmp/lasfile-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lasfile-0.1.6.tar", last modified: Sat May 27 03:03:24 2023, max compression
+gzip compressed data, was "lasfile-0.1.7.tar", last modified: Sat May 27 03:11:56 2023, max compression
```

## Comparing `lasfile-0.1.6.tar` & `lasfile-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 03:03:24.376558 lasfile-0.1.6/
--rw-rw-rw-   0        0        0     1084 2023-05-26 16:29:05.000000 lasfile-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       17 2023-05-27 03:01:07.000000 lasfile-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      612 2023-05-27 03:03:24.376558 lasfile-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-26 16:53:53.000000 lasfile-0.1.6/README.md
--rw-rw-rw-   0        0        0      501 2023-05-27 03:02:54.000000 lasfile-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 03:03:24.377558 lasfile-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 03:03:24.354557 lasfile-0.1.6/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 18:07:33.000000 lasfile-0.1.6/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 03:03:24.374558 lasfile-0.1.6/src/lasfile.egg-info/
--rw-rw-rw-   0        0        0      612 2023-05-27 03:03:24.000000 lasfile-0.1.6/src/lasfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-27 03:03:24.000000 lasfile-0.1.6/src/lasfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 03:03:24.000000 lasfile-0.1.6/src/lasfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-27 03:03:24.000000 lasfile-0.1.6/src/lasfile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-05-27 03:03:24.000000 lasfile-0.1.6/src/lasfile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-27 03:03:24.000000 lasfile-0.1.6/src/lasfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    55373 2023-05-27 03:00:47.000000 lasfile-0.1.6/src/lasfile.py
+drwxrwxrwx   0        0        0        0 2023-05-27 03:11:56.605076 lasfile-0.1.7/
+-rw-rw-rw-   0        0        0     1084 2023-05-26 16:29:05.000000 lasfile-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       17 2023-05-27 03:01:07.000000 lasfile-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      612 2023-05-27 03:11:56.604480 lasfile-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-26 16:53:53.000000 lasfile-0.1.7/README.md
+-rw-rw-rw-   0        0        0      501 2023-05-27 03:11:32.000000 lasfile-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 03:11:56.605582 lasfile-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 03:11:56.582427 lasfile-0.1.7/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 18:07:33.000000 lasfile-0.1.7/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 03:11:56.602726 lasfile-0.1.7/src/lasfile.egg-info/
+-rw-rw-rw-   0        0        0      612 2023-05-27 03:11:56.000000 lasfile-0.1.7/src/lasfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-27 03:11:56.000000 lasfile-0.1.7/src/lasfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 03:11:56.000000 lasfile-0.1.7/src/lasfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-27 03:11:56.000000 lasfile-0.1.7/src/lasfile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-05-27 03:11:56.000000 lasfile-0.1.7/src/lasfile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-27 03:11:56.000000 lasfile-0.1.7/src/lasfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    55392 2023-05-27 03:10:41.000000 lasfile-0.1.7/src/lasfile.py
```

### Comparing `lasfile-0.1.6/LICENSE` & `lasfile-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lasfile-0.1.6/PKG-INFO` & `lasfile-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lasfile
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python library for reading LAS files.
 Project-URL: homepage, https://github.com/bzlmnop/lasfile
 Keywords: las,CWLS,las logs,petrophysical logs
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lasfile-0.1.6/src/lasfile.egg-info/PKG-INFO` & `lasfile-0.1.7/src/lasfile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lasfile
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python library for reading LAS files.
 Project-URL: homepage, https://github.com/bzlmnop/lasfile
 Keywords: las,CWLS,las logs,petrophysical logs
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lasfile-0.1.6/src/lasfile.py` & `lasfile-0.1.7/src/lasfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         {
             "type": "data",
             "titles":["test_data"]
         }
     }
 }
 
-def get_version_num(data,handle_common_errors=True,accept_unknown_versions=False,allow_non_numeric=False):
+def get_version_num(data,handle_common_errors=True,accept_unknown_versions=False,allow_non_numeric=False,unknown_value=None):
     """
     Extracts and validates the version number from the given data.
 
     This function accepts either a string containing a version section, or a DataFrame containing a mnemonic column with a "VERS" value. It then tries to extract the version number and validate it. It handles several common errors, such as non-numeric versions, and allows the acceptance of unknown versions. 
 
     Parameters:
     ----------
```

