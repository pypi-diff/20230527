# Comparing `tmp/nssurge_utils-0.1.6.tar.gz` & `tmp/nssurge_utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nssurge_utils-0.1.6.tar", max compression
+gzip compressed data, was "nssurge_utils-0.1.7.tar", max compression
```

## Comparing `nssurge_utils-0.1.6.tar` & `nssurge_utils-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0        0 2023-05-24 03:07:21.792499 nssurge_utils-0.1.6/README.md
--rw-r--r--   0        0        0       22 2023-05-27 04:35:31.788349 nssurge_utils-0.1.6/nssurge_utils/__init__.py
--rw-r--r--   0        0        0      684 2023-05-27 04:31:06.932174 nssurge_utils-0.1.6/nssurge_utils/config.py
--rw-r--r--   0        0        0    25596 2023-05-24 13:57:27.194926 nssurge_utils-0.1.6/nssurge_utils/data/countryFlagsNamesAndDialCodes.json
--rwxr-xr-x   0        0        0     7783 2023-05-27 04:32:56.407074 nssurge_utils-0.1.6/nssurge_utils/extract_proxy.py
--rw-r--r--   0        0        0     1809 2023-05-24 12:59:45.993775 nssurge_utils-0.1.6/nssurge_utils/parsers.py
--rw-r--r--   0        0        0      880 2023-05-24 12:09:19.509286 nssurge_utils-0.1.6/nssurge_utils/predicates.py
--rw-r--r--   0        0        0     1098 2023-05-24 14:00:56.636289 nssurge_utils-0.1.6/nssurge_utils/transform.py
--rw-r--r--   0        0        0      298 2023-05-24 03:20:15.526307 nssurge_utils-0.1.6/nssurge_utils/types.py
--rw-r--r--   0        0        0     7790 2023-05-24 13:39:00.489727 nssurge_utils-0.1.6/nssurge_utils/utils.py
--rw-r--r--   0        0        0      899 2023-05-27 04:35:31.786976 nssurge_utils-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 nssurge_utils-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-24 03:07:21.792499 nssurge_utils-0.1.7/README.md
+-rw-r--r--   0        0        0       22 2023-05-27 15:20:45.316385 nssurge_utils-0.1.7/nssurge_utils/__init__.py
+-rwxr-xr-x   0        0        0     3964 2023-05-27 15:20:15.536311 nssurge_utils-0.1.7/nssurge_utils/add_to_section.py
+-rw-r--r--   0        0        0      815 2023-05-27 14:49:39.624596 nssurge_utils-0.1.7/nssurge_utils/config.py
+-rw-r--r--   0        0        0    25596 2023-05-24 13:57:27.194926 nssurge_utils-0.1.7/nssurge_utils/data/countryFlagsNamesAndDialCodes.json
+-rwxr-xr-x   0        0        0     7783 2023-05-27 04:32:56.407074 nssurge_utils-0.1.7/nssurge_utils/extract_proxy.py
+-rw-r--r--   0        0        0     1809 2023-05-24 12:59:45.993775 nssurge_utils-0.1.7/nssurge_utils/parsers.py
+-rw-r--r--   0        0        0      880 2023-05-24 12:09:19.509286 nssurge_utils-0.1.7/nssurge_utils/predicates.py
+-rw-r--r--   0        0        0     1098 2023-05-24 14:00:56.636289 nssurge_utils-0.1.7/nssurge_utils/transform.py
+-rw-r--r--   0        0        0      298 2023-05-24 03:20:15.526307 nssurge_utils-0.1.7/nssurge_utils/types.py
+-rw-r--r--   0        0        0     8765 2023-05-27 14:59:08.293315 nssurge_utils-0.1.7/nssurge_utils/utils.py
+-rw-r--r--   0        0        0      961 2023-05-27 15:20:45.315349 nssurge_utils-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 nssurge_utils-0.1.7/PKG-INFO
```

### Comparing `nssurge_utils-0.1.6/nssurge_utils/config.py` & `nssurge_utils-0.1.7/nssurge_utils/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,7 +17,9 @@
 package_dir = Path(__file__).parent
 parent_dir = package_dir.parent
 # data_dir = parent_dir / 'data'
 data_dir = package_dir / 'data'
 countryFlagsNamesAndDialCodes_json_path = (
     data_dir / 'countryFlagsNamesAndDialCodes.json'
 )
+
+DEFAULT_RULE_TO_PREPEND = 'RULE-SET,https://cdn.jsdelivr.net/gh/dler-io/Rules@main/Surge/Surge%203/Provider/ChatGPT.list,ChatGPT'
```

### Comparing `nssurge_utils-0.1.6/nssurge_utils/data/countryFlagsNamesAndDialCodes.json` & `nssurge_utils-0.1.7/nssurge_utils/data/countryFlagsNamesAndDialCodes.json`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.6/nssurge_utils/extract_proxy.py` & `nssurge_utils-0.1.7/nssurge_utils/extract_proxy.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.6/nssurge_utils/parsers.py` & `nssurge_utils-0.1.7/nssurge_utils/parsers.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.6/nssurge_utils/predicates.py` & `nssurge_utils-0.1.7/nssurge_utils/predicates.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.6/nssurge_utils/transform.py` & `nssurge_utils-0.1.7/nssurge_utils/transform.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.6/nssurge_utils/utils.py` & `nssurge_utils-0.1.7/nssurge_utils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,14 +60,46 @@
     import re
 
     if section is None:
         return re.match(r'^\[(.*)\]', line) is not None
     return re.match(r'^\[' + section + r'\]', line) is not None
 
 
+def add_to_file_partition(
+    to_add: str,
+    target_file: PathLike,
+    is_first_marker: Callable[[str], bool],
+    is_second_marker: Callable[[str], bool],
+    prepend: bool = True,
+    replace: bool = False,
+    output_file: PathLike | None = None,
+) -> None:
+    extracted_input_lines = [to_add]
+
+    # Process output file
+    target_lines = partition_lines(
+        file_line_generator(target_file),
+        is_first_marker,
+        is_second_marker,
+        include_markers=(False, False),
+        # transform_fn=transform_fn,
+    )
+    if replace:
+        replaced_lines = extracted_input_lines
+    elif prepend:
+        replaced_lines = extracted_input_lines + target_lines[1]
+    else:
+        replaced_lines = target_lines[1] + extracted_input_lines
+    output_lines = target_lines[0] + replaced_lines + target_lines[2]
+    if output_file is None:
+        output_file = target_file
+    with open(output_file, 'w') as file:
+        file.writelines(output_lines)
+
+
 def merge_file_partitions(
     input_file: PathLike,
     target_file: PathLike,
     is_first_marker_input: Callable[[str], bool],
     is_second_marker_input: Callable[[str], bool],
     is_first_marker_output: Callable[[str], bool],
     is_second_marker_output: Callable[[str], bool],
```

### Comparing `nssurge_utils-0.1.6/pyproject.toml` & `nssurge_utils-0.1.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 name = "nssurge-utils"
-version = "0.1.6"
+version = "0.1.7"
 description = "NSSurge Utilities"
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "nssurge_utils" }]
 # include = ["data"]
 license = "MIT"
 homepage = "https://github.com/tddschn/nssurge-utils"
 repository = "https://github.com/tddschn/nssurge-utils"
 classifiers = ["Topic :: Utilities"]
 keywords = ["nssurge", "surge", "utils"]
+
 [tool.poetry.scripts]
 nssurge-extract-proxy = "nssurge_utils.extract_proxy:main"
+nssurge-add-to-section = "nssurge_utils.add_to_section:main"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tddschn/nssurge-utils/issues"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `nssurge_utils-0.1.6/PKG-INFO` & `nssurge_utils-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nssurge-utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: NSSurge Utilities
 Home-page: https://github.com/tddschn/nssurge-utils
 License: MIT
 Keywords: nssurge,surge,utils
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```

