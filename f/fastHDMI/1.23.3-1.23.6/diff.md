# Comparing `tmp/fastHDMI-1.23.3.tar.gz` & `tmp/fastHDMI-1.23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastHDMI-1.23.3.tar", last modified: Thu Apr 20 03:57:05 2023, max compression
+gzip compressed data, was "fastHDMI-1.23.6.tar", last modified: Thu Apr 20 06:09:08 2023, max compression
```

## Comparing `fastHDMI-1.23.3.tar` & `fastHDMI-1.23.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-20 03:57:05.828760 fastHDMI-1.23.3/
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    34523 2022-11-10 23:21:11.000000 fastHDMI-1.23.3/LICENSE
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      103 2023-04-17 22:35:24.000000 fastHDMI-1.23.3/MANIFEST.in
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    46504 2023-04-20 03:57:05.828760 fastHDMI-1.23.3/PKG-INFO
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     5931 2023-02-19 04:38:00.000000 fastHDMI-1.23.3/README.md
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     1170 2023-04-20 03:50:07.000000 fastHDMI-1.23.3/pyproject.toml
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)       38 2023-04-20 03:57:05.828760 fastHDMI-1.23.3/setup.cfg
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      298 2023-04-16 23:35:56.000000 fastHDMI-1.23.3/setup.py
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-20 03:57:05.828760 fastHDMI-1.23.3/src/
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-20 03:57:05.828760 fastHDMI-1.23.3/src/fastHDMI/
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)   227176 2023-04-18 05:45:38.000000 fastHDMI-1.23.3/src/fastHDMI/__init__.py
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)   900663 2023-04-20 03:57:05.000000 fastHDMI-1.23.3/src/fastHDMI/cython_fun.c
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     1956 2023-04-20 03:48:05.000000 fastHDMI-1.23.3/src/fastHDMI/cython_fun.pyx
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-20 03:57:05.828760 fastHDMI-1.23.3/src/fastHDMI.egg-info/
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    46504 2023-04-20 03:57:05.000000 fastHDMI-1.23.3/src/fastHDMI.egg-info/PKG-INFO
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      325 2023-04-20 03:57:05.000000 fastHDMI-1.23.3/src/fastHDMI.egg-info/SOURCES.txt
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)        1 2023-04-20 03:57:05.000000 fastHDMI-1.23.3/src/fastHDMI.egg-info/dependency_links.txt
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      147 2023-04-20 03:57:05.000000 fastHDMI-1.23.3/src/fastHDMI.egg-info/requires.txt
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)        9 2023-04-20 03:57:05.000000 fastHDMI-1.23.3/src/fastHDMI.egg-info/top_level.txt
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-20 03:57:05.828760 fastHDMI-1.23.3/tests/
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     4258 2023-04-17 23:06:01.000000 fastHDMI-1.23.3/tests/test.py
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-20 06:09:08.072994 fastHDMI-1.23.6/
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    34523 2022-11-10 23:21:11.000000 fastHDMI-1.23.6/LICENSE
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      103 2023-04-17 22:35:24.000000 fastHDMI-1.23.6/MANIFEST.in
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    46504 2023-04-20 06:09:08.072994 fastHDMI-1.23.6/PKG-INFO
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     5931 2023-02-19 04:38:00.000000 fastHDMI-1.23.6/README.md
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     1170 2023-04-20 06:04:47.000000 fastHDMI-1.23.6/pyproject.toml
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)       38 2023-04-20 06:09:08.072994 fastHDMI-1.23.6/setup.cfg
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      298 2023-04-16 23:35:56.000000 fastHDMI-1.23.6/setup.py
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-20 06:09:08.068994 fastHDMI-1.23.6/src/
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-20 06:09:08.068994 fastHDMI-1.23.6/src/fastHDMI/
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)   227256 2023-04-20 06:02:17.000000 fastHDMI-1.23.6/src/fastHDMI/__init__.py
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)   900663 2023-04-20 06:09:07.000000 fastHDMI-1.23.6/src/fastHDMI/cython_fun.c
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     1956 2023-04-20 03:48:05.000000 fastHDMI-1.23.6/src/fastHDMI/cython_fun.pyx
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-20 06:09:08.068994 fastHDMI-1.23.6/src/fastHDMI.egg-info/
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    46504 2023-04-20 06:09:08.000000 fastHDMI-1.23.6/src/fastHDMI.egg-info/PKG-INFO
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      325 2023-04-20 06:09:08.000000 fastHDMI-1.23.6/src/fastHDMI.egg-info/SOURCES.txt
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)        1 2023-04-20 06:09:08.000000 fastHDMI-1.23.6/src/fastHDMI.egg-info/dependency_links.txt
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      147 2023-04-20 06:09:08.000000 fastHDMI-1.23.6/src/fastHDMI.egg-info/requires.txt
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)        9 2023-04-20 06:09:08.000000 fastHDMI-1.23.6/src/fastHDMI.egg-info/top_level.txt
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-20 06:09:08.068994 fastHDMI-1.23.6/tests/
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     4258 2023-04-17 23:06:01.000000 fastHDMI-1.23.6/tests/test.py
```

### Comparing `fastHDMI-1.23.3/LICENSE` & `fastHDMI-1.23.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastHDMI-1.23.3/PKG-INFO` & `fastHDMI-1.23.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastHDMI
-Version: 1.23.3
+Version: 1.23.6
 Summary: Use FFT-based mutual information and accelerated gradient method to screen variables and optimize nonconvex sparse learning problems on large CSV files or large genetic bed/bim/fam files. Multiprocessing is now available.
 Author-email: Kai Yang <kai.yang2@mail.mcgill.ca>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `fastHDMI-1.23.3/README.md` & `fastHDMI-1.23.6/README.md`

 * *Files identical despite different names*

### Comparing `fastHDMI-1.23.3/pyproject.toml` & `fastHDMI-1.23.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel>=0.34.2",
     "Cython>=0.29.21"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastHDMI"
-version = "1.23.3"
+version = "1.23.6"
 authors = [
   { name="Kai Yang", email="kai.yang2@mail.mcgill.ca" },
 ]
 description = "Use FFT-based mutual information and accelerated gradient method to screen variables and optimize nonconvex sparse learning problems on large CSV files or large genetic bed/bim/fam files. Multiprocessing is now available."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `fastHDMI-1.23.3/src/fastHDMI/__init__.py` & `fastHDMI-1.23.6/src/fastHDMI/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,16 +521,16 @@
     """
     if csv_engine == "dask":
         _ = _np.asarray(_df[__].dropna().compute())
     elif csv_engine in ["pyarrow", "c", "python",
                         "fastparquet"]:  # these are engines using pandas
         _ = _df[__].dropna().to_numpy()
 
-    _a = _[:, 0]
-    _b = _[:, 1]
+    _a = _[:, 0].copy() # such that _df won't be mutated
+    _b = _[:, 1].copy() # such that _df won't be mutated
     return _a, _b
 
 
 def binary_screening_csv(csv_file="_",
                          _usecols=[],
                          N=500,
                          kernel="epa",
```

### Comparing `fastHDMI-1.23.3/src/fastHDMI/cython_fun.c` & `fastHDMI-1.23.6/src/fastHDMI/cython_fun.c`

 * *Files identical despite different names*

### Comparing `fastHDMI-1.23.3/src/fastHDMI/cython_fun.pyx` & `fastHDMI-1.23.6/src/fastHDMI/cython_fun.pyx`

 * *Files identical despite different names*

### Comparing `fastHDMI-1.23.3/src/fastHDMI.egg-info/PKG-INFO` & `fastHDMI-1.23.6/src/fastHDMI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastHDMI
-Version: 1.23.3
+Version: 1.23.6
 Summary: Use FFT-based mutual information and accelerated gradient method to screen variables and optimize nonconvex sparse learning problems on large CSV files or large genetic bed/bim/fam files. Multiprocessing is now available.
 Author-email: Kai Yang <kai.yang2@mail.mcgill.ca>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `fastHDMI-1.23.3/tests/test.py` & `fastHDMI-1.23.6/tests/test.py`

 * *Files identical despite different names*

