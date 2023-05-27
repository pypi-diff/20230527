# Comparing `tmp/gravitas-0.0.1.tar.gz` & `tmp/gravitas-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitas-0.0.1.tar", max compression
+gzip compressed data, was "gravitas-0.0.4.tar", max compression
```

## Comparing `gravitas-0.0.1.tar` & `gravitas-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0        4 2023-05-27 04:07:39.325347 gravitas-0.0.1/README.md
--rw-r--r--   0        0        0     1844 2023-05-27 04:29:06.552685 gravitas-0.0.1/build.py
--rw-r--r--   0        0        0      625 2023-05-27 04:25:07.816164 gravitas-0.0.1/pyproject.toml
--rw-r--r--   0        0        0  5121578 2023-05-27 01:15:07.470942 gravitas-0.0.1/src/EGM96
--rw-r--r--   0        0        0  6559245 2023-05-27 01:18:34.665548 gravitas-0.0.1/src/GRGM360
--rw-r--r--   0        0        0   731918 2023-05-27 03:41:09.634209 gravitas-0.0.1/src/MRO120F
--rw-r--r--   0        0        0      255 2023-05-27 02:23:57.048359 gravitas-0.0.1/src/__init__.py
--rwxr-xr-x   0        0        0    34292 2023-05-27 03:57:02.894875 gravitas-0.0.1/src/grav.so
--rw-r--r--   0        0        0     6152 2023-05-27 03:46:44.136925 gravitas-0.0.1/src/gravlib.c
--rw-r--r--   0        0        0     1288 2023-05-27 03:44:34.140209 gravitas-0.0.1/src/lib.py
--rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 gravitas-0.0.1/setup.py
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 gravitas-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        4 2023-05-27 04:07:39.325347 gravitas-0.0.4/README.md
+-rw-r--r--   0        0        0     1396 2023-05-27 04:38:13.803710 gravitas-0.0.4/build.py
+-rw-r--r--   0        0        0  5121578 2023-05-27 01:15:07.470942 gravitas-0.0.4/gravitas/EGM96
+-rw-r--r--   0        0        0  6559245 2023-05-27 01:18:34.665548 gravitas-0.0.4/gravitas/GRGM360
+-rw-r--r--   0        0        0   731918 2023-05-27 03:41:09.634209 gravitas-0.0.4/gravitas/MRO120F
+-rw-r--r--   0        0        0      255 2023-05-27 02:23:57.048359 gravitas-0.0.4/gravitas/__init__.py
+-rwxr-xr-x   0        0        0    34292 2023-05-27 03:57:02.894875 gravitas-0.0.4/gravitas/grav.so
+-rw-r--r--   0        0        0     6152 2023-05-27 03:46:44.136925 gravitas-0.0.4/gravitas/gravlib.c
+-rw-r--r--   0        0        0     1288 2023-05-27 03:44:34.140209 gravitas-0.0.4/gravitas/lib.py
+-rw-r--r--   0        0        0      603 2023-05-27 04:44:21.672843 gravitas-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 gravitas-0.0.4/PKG-INFO
```

### Comparing `gravitas-0.0.1/build.py` & `gravitas-0.0.4/build.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """Poetry build script for python_ctypes"""
-import os
-import shutil
-
 from distutils.command.build_ext import build_ext
 from distutils.core import Distribution
 from distutils.core import Extension
 from distutils.errors import CCompilerError
 from distutils.errors import DistutilsExecError
 from distutils.errors import DistutilsPlatformError
 
 
 extensions = [
-    Extension("grav", ["src/gravlib.c"]),
+    Extension("grav", ["gravitas/gravlib.c"]),
 ]
 
 
 class ExtBuilder(build_ext):
     # This class allows C extension building to fail.
 
     built_extensions = []
@@ -34,31 +31,18 @@
                   "python_ctypes will use the pure python version of the extension.".format(ext.name))
 
 
 def build(setup_kwargs):
     """
     This function is mandatory in order to build the extensions.
     """
-    print(setup_kwargs)
-    distribution = Distribution({"name": "src", "ext_modules": extensions})
-    distribution.package_dir = "src"
+    distribution = Distribution({"name": "gravitas", "ext_modules": extensions})
+    distribution.package_dir = "gravitas"
 
     cmd = ExtBuilder(distribution)
     cmd.ensure_finalized()
     cmd.run()
-
-    # Copy built extensions back to the project
-    # for output in cmd.get_outputs():
-    #     relative_extension = os.path.relpath(output, cmd.build_lib)
-    #     if not os.path.exists(output):
-    #         continue
-
-    #     shutil.copyfile(output, relative_extension)
-    #     mode = os.stat(relative_extension).st_mode
-    #     mode |= (mode & 0o444) >> 2
-    #     os.chmod(relative_extension, mode)
-
     return setup_kwargs
 
 
 if __name__ == "__main__":
     build({})
```

### Comparing `gravitas-0.0.1/pyproject.toml` & `gravitas-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "gravitas"
-version = "0.0.1"
+version = "0.0.4"
 description = "High-fidelity gravity fields for satellite propagation"
 authors = ["Liam Robinson <robin502@purdue.edu>"]
 readme = "README.md"
-packages = [{include = "src"}]
+packages = [{include = "gravitas"}]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: MacOS",
 ]
 
 [tool.poetry.build]
 script = "build.py"
-generate-setup-file = true
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 numpy = "^1.24.2"
 
 [build-system]
 requires = ["poetry-core", "setuptools"]
```

### Comparing `gravitas-0.0.1/src/EGM96` & `gravitas-0.0.4/gravitas/EGM96`

 * *Files identical despite different names*

### Comparing `gravitas-0.0.1/src/GRGM360` & `gravitas-0.0.4/gravitas/GRGM360`

 * *Files identical despite different names*

### Comparing `gravitas-0.0.1/src/MRO120F` & `gravitas-0.0.4/gravitas/MRO120F`

 * *Files identical despite different names*

### Comparing `gravitas-0.0.1/src/grav.so` & `gravitas-0.0.4/gravitas/grav.so`

 * *Files identical despite different names*

### Comparing `gravitas-0.0.1/src/gravlib.c` & `gravitas-0.0.4/gravitas/gravlib.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.0.1/src/lib.py` & `gravitas-0.0.4/gravitas/lib.py`

 * *Files identical despite different names*

### Comparing `gravitas-0.0.1/PKG-INFO` & `gravitas-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: gravitas
-Version: 0.0.1
+Version: 0.0.4
 Summary: High-fidelity gravity fields for satellite propagation
 Author: Liam Robinson
 Author-email: robin502@purdue.edu
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 test
```

