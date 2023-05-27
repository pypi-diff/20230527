# Comparing `tmp/shlep-3.1.0.tar.gz` & `tmp/shlep-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shlep-3.1.0.tar", last modified: Sat May 27 20:24:30 2023, max compression
+gzip compressed data, was "shlep-3.1.1.tar", last modified: Sat May 27 20:30:01 2023, max compression
```

## Comparing `shlep-3.1.0.tar` & `shlep-3.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-3.1.0/LICENSE
--rw-r--r--   0        0        0     2332 2023-05-27 20:10:45.441977 shlep-3.1.0/README.md
--rw-r--r--   0        0        0      454 2023-05-27 20:24:30.187373 shlep-3.1.0/pyproject.toml
--rw-r--r--   0        0        0       24 2023-05-27 20:10:45.436465 shlep-3.1.0/shlep/__init__.py
--rw-r--r--   0        0        0     3756 2023-05-27 20:23:16.844711 shlep-3.1.0/shlep/main.py
--rw-r--r--   0        0        0     2613 1970-01-01 00:00:00.000000 shlep-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-3.1.1/LICENSE
+-rw-r--r--   0        0        0     2332 2023-05-27 20:10:45.441977 shlep-3.1.1/README.md
+-rw-r--r--   0        0        0      454 2023-05-27 20:30:01.598827 shlep-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-05-27 20:10:45.436465 shlep-3.1.1/shlep/__init__.py
+-rw-r--r--   0        0        0     3763 2023-05-27 20:29:44.925163 shlep-3.1.1/shlep/main.py
+-rw-r--r--   0        0        0     2613 1970-01-01 00:00:00.000000 shlep-3.1.1/PKG-INFO
```

### Comparing `shlep-3.1.0/LICENSE` & `shlep-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shlep-3.1.0/README.md` & `shlep-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `shlep-3.1.0/shlep/main.py` & `shlep-3.1.1/shlep/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     if not spec:
         return True
     return spec.match_file(str(path.relative_to(base)))
 
 
 def shlep(
     directory: Path | str,
-    indent: int,
+    indent: int | None,
     additional_excludes: list[str],
     output_format: str,
     output_file: Path | str = None,
     quiet=False,
 ) -> str:
     """
     Generate a file of all files in a directory.
```

### Comparing `shlep-3.1.0/PKG-INFO` & `shlep-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shlep
-Version: 3.1.0
+Version: 3.1.1
 Summary: gather directory contents into a single file
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Requires-Dist: pathspec>=0.11.1
 Description-Content-Type: text/markdown
```

