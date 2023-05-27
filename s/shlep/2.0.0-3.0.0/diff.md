# Comparing `tmp/shlep-2.0.0.tar.gz` & `tmp/shlep-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shlep-2.0.0.tar", last modified: Fri May 26 23:09:51 2023, max compression
+gzip compressed data, was "shlep-3.0.0.tar", last modified: Sat May 27 20:14:39 2023, max compression
```

## Comparing `shlep-2.0.0.tar` & `shlep-3.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-2.0.0/LICENSE
--rw-r--r--   0        0        0     2348 2023-05-26 15:54:07.624515 shlep-2.0.0/README.md
--rw-r--r--   0        0        0      454 2023-05-26 23:09:51.987838 shlep-2.0.0/pyproject.toml
--rw-r--r--   0        0        0       32 2023-05-26 04:01:45.741927 shlep-2.0.0/shlep/__init__.py
--rw-r--r--   0        0        0     3661 2023-05-26 23:08:48.583274 shlep-2.0.0/shlep/main.py
--rw-r--r--   0        0        0     2629 1970-01-01 00:00:00.000000 shlep-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2332 2023-05-27 20:10:45.441977 shlep-3.0.0/README.md
+-rw-r--r--   0        0        0      454 2023-05-27 20:14:39.785686 shlep-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-05-27 20:10:45.436465 shlep-3.0.0/shlep/__init__.py
+-rw-r--r--   0        0        0     3742 2023-05-27 20:10:45.439459 shlep-3.0.0/shlep/main.py
+-rw-r--r--   0        0        0     2613 1970-01-01 00:00:00.000000 shlep-3.0.0/PKG-INFO
```

### Comparing `shlep-2.0.0/LICENSE` & `shlep-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shlep-2.0.0/README.md` & `shlep-3.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -52,23 +52,23 @@
   -f {json,csv,plaintext}, --format {json,csv,plaintext}
                         The output format. Can be 'json', 'csv', or 'plaintext'. Default is 'json'.
 ```
 
 ### Programmatically in Python
 
 ```python
-from shlep import create_output
+from shlep import shlep
 
 directory = "path/to/your/directory"
 indent = 2
 additional_excludes = [".env", "node_modules/"]
 output_format = "json"
 output_file = "output.json"
 
-create_output(directory, indent, additional_excludes, output_format, output_file)
+shlep(directory, indent, additional_excludes, output_format, output_file)
 ```
 
 ## License
 
 This project is licensed under the Apache License 2.0. You can find the full license text in the [LICENSE](LICENSE) file.
 
 [pipx]: https://pypa.github.io/pipx/
```

### Comparing `shlep-2.0.0/shlep/main.py` & `shlep-3.0.0/shlep/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,33 +13,35 @@
 
 def _is_excluded(base: Path, path: Path, spec: PathSpec = None):
     if not spec:
         return True
     return spec.match_file(str(path.relative_to(base)))
 
 
-def create_output(
+def shlep(
     directory: str,
     indent: int,
     additional_excludes: list[str],
     output_format: str,
     output_file: str = None,
-) -> None:
+    quiet=False,
+) -> str:
     """
     Generate a file of all files in a directory.
 
     Args:
         directory: The directory to analyze.
         indent: The number of spaces to use for indentation in the output JSON.
         additional_excludes: Additional files or directories to exclude.
         output_format: The output format. Can be 'json', 'csv', or 'plaintext'. Default is 'json'.
         output_file: The output file to generate. If not specified, output is printed to stdout.
+        quiet: don't print output to stdout
 
-    Returns:
-        None
+    Returns (str):
+        output
     """
     files_list = []
     base = Path(directory).expanduser()
 
     if (gitignore := base / ".gitignore").exists():
         with gitignore.open() as f:
             additional_excludes.extend(
@@ -74,17 +76,19 @@
             output += f"```{os.linesep + file_content}```"
             if not i == len_files_list:
                 output += os.linesep * 2 + "---" + os.linesep * 2
 
     if output_file:
         with Path(output_file).expanduser().open("w") as f:
             f.write(output)
-    else:
+    elif not quiet:
         print(output)
 
+    return output
+
 
 def cli():
     parser = argparse.ArgumentParser(
         prog="shlep",
         usage="%(prog)s [OPTIONS] directory",
         description="Gather directory contents into a single output.",
     )
@@ -113,12 +117,12 @@
         "--format",
         choices=["json", "plaintext"],
         default="json",
         help="The output format. Can be 'json' or 'plaintext'. Default is 'json'.",
     )
     args = parser.parse_args()
     excluded = args.exclude or []
-    create_output(args.directory, args.indent, excluded, args.format, args.output_file)
+    shlep(args.directory, args.indent, excluded, args.format, args.output_file)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `shlep-2.0.0/PKG-INFO` & `shlep-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shlep
-Version: 2.0.0
+Version: 3.0.0
 Summary: gather directory contents into a single file
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Requires-Dist: pathspec>=0.11.1
 Description-Content-Type: text/markdown
 
@@ -62,23 +62,23 @@
   -f {json,csv,plaintext}, --format {json,csv,plaintext}
                         The output format. Can be 'json', 'csv', or 'plaintext'. Default is 'json'.
 ```
 
 ### Programmatically in Python
 
 ```python
-from shlep import create_output
+from shlep import shlep
 
 directory = "path/to/your/directory"
 indent = 2
 additional_excludes = [".env", "node_modules/"]
 output_format = "json"
 output_file = "output.json"
 
-create_output(directory, indent, additional_excludes, output_format, output_file)
+shlep(directory, indent, additional_excludes, output_format, output_file)
 ```
 
 ## License
 
 This project is licensed under the Apache License 2.0. You can find the full license text in the [LICENSE](LICENSE) file.
 
 [pipx]: https://pypa.github.io/pipx/
```

