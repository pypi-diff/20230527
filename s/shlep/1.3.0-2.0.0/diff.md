# Comparing `tmp/shlep-1.3.0.tar.gz` & `tmp/shlep-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shlep-1.3.0.tar", last modified: Fri May 26 15:55:35 2023, max compression
+gzip compressed data, was "shlep-2.0.0.tar", last modified: Fri May 26 23:09:51 2023, max compression
```

## Comparing `shlep-1.3.0.tar` & `shlep-2.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-1.3.0/LICENSE
--rw-r--r--   0        0        0     2348 2023-05-26 15:54:07.624515 shlep-1.3.0/README.md
--rw-r--r--   0        0        0      454 2023-05-26 15:55:35.501531 shlep-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       32 2023-05-26 04:01:45.741927 shlep-1.3.0/shlep/__init__.py
--rw-r--r--   0        0        0     3941 2023-05-26 15:45:24.441652 shlep-1.3.0/shlep/main.py
--rw-r--r--   0        0        0     2629 1970-01-01 00:00:00.000000 shlep-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2348 2023-05-26 15:54:07.624515 shlep-2.0.0/README.md
+-rw-r--r--   0        0        0      454 2023-05-26 23:09:51.987838 shlep-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-05-26 04:01:45.741927 shlep-2.0.0/shlep/__init__.py
+-rw-r--r--   0        0        0     3661 2023-05-26 23:08:48.583274 shlep-2.0.0/shlep/main.py
+-rw-r--r--   0        0        0     2629 1970-01-01 00:00:00.000000 shlep-2.0.0/PKG-INFO
```

### Comparing `shlep-1.3.0/LICENSE` & `shlep-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shlep-1.3.0/README.md` & `shlep-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `shlep-1.3.0/shlep/main.py` & `shlep-2.0.0/shlep/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,21 +58,15 @@
                 content = path.read_text()
             except UnicodeDecodeError:
                 logger.error(f"Could not read {path}")
             else:
                 files_list.append({"path": str(path), "content": content})
 
     if output_format == "json":
-        output = json.dumps({"files": files_list}, indent=indent)
-    elif output_format == "csv":
-        output = f"path,content{os.linesep}"
-        for file in files_list:
-            file_path = file["path"]
-            file_content = file["content"]
-            output += f"{file_path},{file_content}{os.linesep}"
+        output = json.dumps(files_list, indent=indent)
     else:  # plaintext
         output = ""
         len_files_list = len(files_list)
         for i, file in enumerate(files_list, start=1):
             filepath = file["path"]
             file_content = file["content"]
             output += f"`{filepath}`"
@@ -113,17 +107,17 @@
         type=str,
         action="append",
         help="Additional files or directories to exclude.",
     )
     parser.add_argument(
         "-f",
         "--format",
-        choices=["json", "csv", "plaintext"],
+        choices=["json", "plaintext"],
         default="json",
-        help="The output format. Can be 'json', 'csv', or 'plaintext'. Default is 'json'.",
+        help="The output format. Can be 'json' or 'plaintext'. Default is 'json'.",
     )
     args = parser.parse_args()
     excluded = args.exclude or []
     create_output(args.directory, args.indent, excluded, args.format, args.output_file)
 
 
 if __name__ == "__main__":
```

### Comparing `shlep-1.3.0/PKG-INFO` & `shlep-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shlep
-Version: 1.3.0
+Version: 2.0.0
 Summary: gather directory contents into a single file
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Requires-Dist: pathspec>=0.11.1
 Description-Content-Type: text/markdown
```

