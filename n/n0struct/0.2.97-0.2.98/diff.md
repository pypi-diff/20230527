# Comparing `tmp/n0struct-0.2.97.tar.gz` & `tmp/n0struct-0.2.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\n0struct-0.2.97.tar", last modified: Sun May 14 20:42:10 2023, max compression
+gzip compressed data, was "dist\n0struct-0.2.98.tar", last modified: Sat May 27 10:01:32 2023, max compression
```

## Comparing `n0struct-0.2.97.tar` & `n0struct-0.2.98.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 20:42:10.493233 n0struct-0.2.97/
--rw-rw-rw-   0        0        0    11558 2022-09-04 19:16:09.000000 n0struct-0.2.97/LICENSE
--rw-rw-rw-   0        0        0     1060 2023-05-14 20:42:10.508854 n0struct-0.2.97/PKG-INFO
--rw-rw-rw-   0        0        0      590 2022-09-04 19:16:09.000000 n0struct-0.2.97/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 20:42:10.462022 n0struct-0.2.97/n0struct/
--rw-rw-rw-   0        0        0      988 2023-05-13 11:12:54.000000 n0struct-0.2.97/n0struct/__init__.py
--rw-rw-rw-   0        0        0     3671 2023-05-12 12:43:36.000000 n0struct-0.2.97/n0struct/n0struct_arrays.py
--rw-rw-rw-   0        0        0     2104 2023-05-13 11:27:25.000000 n0struct-0.2.97/n0struct/n0struct_comprehensions.py
--rw-rw-rw-   0        0        0    13176 2023-04-25 08:08:57.000000 n0struct-0.2.97/n0struct/n0struct_date.py
--rw-rw-rw-   0        0        0     3389 2023-05-13 05:52:52.000000 n0struct-0.2.97/n0struct/n0struct_files.py
--rw-rw-rw-   0        0        0    29365 2023-05-14 20:33:53.000000 n0struct-0.2.97/n0struct/n0struct_files_csv.py
--rw-rw-rw-   0        0        0     7117 2023-05-13 11:56:28.000000 n0struct-0.2.97/n0struct/n0struct_files_fwf.py
--rw-rw-rw-   0        0        0    15648 2023-05-13 11:36:31.000000 n0struct-0.2.97/n0struct/n0struct_findall.py
--rw-rw-rw-   0        0        0     4070 2023-04-25 08:08:57.000000 n0struct-0.2.97/n0struct/n0struct_git.py
--rw-rw-rw-   0        0        0    20960 2023-05-14 20:41:00.000000 n0struct-0.2.97/n0struct/n0struct_logging.py
--rw-rw-rw-   0        0        0     2287 2023-04-25 08:08:57.000000 n0struct-0.2.97/n0struct/n0struct_mask.py
--rw-rw-rw-   0        0        0    12168 2023-04-25 08:08:57.000000 n0struct-0.2.97/n0struct/n0struct_n0dict_.py
--rw-rw-rw-   0        0        0    17116 2023-05-13 12:19:09.000000 n0struct-0.2.97/n0struct/n0struct_n0dict__.py
--rw-rw-rw-   0        0        0     7519 2023-05-13 11:50:12.000000 n0struct-0.2.97/n0struct/n0struct_n0list_.py
--rw-rw-rw-   0        0        0    75645 2023-05-13 12:22:04.000000 n0struct-0.2.97/n0struct/n0struct_n0list_n0dict.py
--rw-rw-rw-   0        0        0      917 2023-04-25 08:08:57.000000 n0struct-0.2.97/n0struct/n0struct_random.py
--rw-rw-rw-   0        0        0     3852 2023-04-25 08:08:57.000000 n0struct-0.2.97/n0struct/n0struct_references.py
--rw-rw-rw-   0        0        0     3235 2023-05-12 12:49:17.000000 n0struct-0.2.97/n0struct/n0struct_transform_structure.py
--rw-rw-rw-   0        0        0    18218 2023-05-14 15:31:16.000000 n0struct-0.2.97/n0struct/n0struct_utils.py
--rw-rw-rw-   0        0        0     6659 2023-05-12 12:42:29.000000 n0struct-0.2.97/n0struct/n0struct_utils_compare.py
--rw-rw-rw-   0        0        0     4120 2023-05-12 12:42:54.000000 n0struct-0.2.97/n0struct/n0struct_utils_find.py
-drwxrwxrwx   0        0        0        0 2023-05-14 20:42:10.493233 n0struct-0.2.97/n0struct/test/
--rw-rw-rw-   0        0        0        0 2022-09-04 19:16:09.000000 n0struct-0.2.97/n0struct/test/__init__.py
--rw-rw-rw-   0        0        0      136 2022-09-04 19:16:09.000000 n0struct-0.2.97/n0struct/test/__main__.py
--rw-rw-rw-   0        0        0    33051 2023-05-13 12:06:10.000000 n0struct-0.2.97/n0struct/test/test_n0struct.py
--rw-rw-rw-   0        0        0     2572 2023-03-06 04:48:48.000000 n0struct-0.2.97/n0struct/test/test_n0struct2.py
--rw-rw-rw-   0        0        0      890 2023-05-13 12:07:38.000000 n0struct-0.2.97/n0struct/test/test_n0struct3.py
--rw-rw-rw-   0        0        0     1490 2023-05-13 12:23:25.000000 n0struct-0.2.97/n0struct/test/test_n0struct4.py
-drwxrwxrwx   0        0        0        0 2023-05-14 20:42:10.477641 n0struct-0.2.97/n0struct.egg-info/
--rw-rw-rw-   0        0        0     1060 2023-05-14 20:42:10.000000 n0struct-0.2.97/n0struct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1032 2023-05-14 20:42:10.000000 n0struct-0.2.97/n0struct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 20:42:10.000000 n0struct-0.2.97/n0struct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-14 20:42:10.000000 n0struct-0.2.97/n0struct.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       55 2023-05-14 20:42:10.000000 n0struct-0.2.97/n0struct.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 20:42:10.000000 n0struct-0.2.97/n0struct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 20:42:10.508854 n0struct-0.2.97/setup.cfg
--rw-rw-rw-   0        0        0     2476 2023-04-02 07:28:40.000000 n0struct-0.2.97/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:01:32.347421 n0struct-0.2.98/
+-rw-rw-rw-   0        0        0    11558 2022-09-04 19:16:09.000000 n0struct-0.2.98/LICENSE
+-rw-rw-rw-   0        0        0     1060 2023-05-27 10:01:32.347421 n0struct-0.2.98/PKG-INFO
+-rw-rw-rw-   0        0        0      590 2022-09-04 19:16:09.000000 n0struct-0.2.98/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 10:01:32.316165 n0struct-0.2.98/n0struct/
+-rw-rw-rw-   0        0        0      988 2023-05-13 11:12:54.000000 n0struct-0.2.98/n0struct/__init__.py
+-rw-rw-rw-   0        0        0     3671 2023-05-12 12:43:36.000000 n0struct-0.2.98/n0struct/n0struct_arrays.py
+-rw-rw-rw-   0        0        0     2104 2023-05-13 11:27:25.000000 n0struct-0.2.98/n0struct/n0struct_comprehensions.py
+-rw-rw-rw-   0        0        0    13176 2023-04-25 08:08:57.000000 n0struct-0.2.98/n0struct/n0struct_date.py
+-rw-rw-rw-   0        0        0     3389 2023-05-13 05:52:52.000000 n0struct-0.2.98/n0struct/n0struct_files.py
+-rw-rw-rw-   0        0        0    29723 2023-05-27 09:55:21.000000 n0struct-0.2.98/n0struct/n0struct_files_csv.py
+-rw-rw-rw-   0        0        0     7117 2023-05-13 11:56:28.000000 n0struct-0.2.98/n0struct/n0struct_files_fwf.py
+-rw-rw-rw-   0        0        0    15648 2023-05-13 11:36:31.000000 n0struct-0.2.98/n0struct/n0struct_findall.py
+-rw-rw-rw-   0        0        0     4070 2023-04-25 08:08:57.000000 n0struct-0.2.98/n0struct/n0struct_git.py
+-rw-rw-rw-   0        0        0    20514 2023-05-27 10:00:27.000000 n0struct-0.2.98/n0struct/n0struct_logging.py
+-rw-rw-rw-   0        0        0     2287 2023-04-25 08:08:57.000000 n0struct-0.2.98/n0struct/n0struct_mask.py
+-rw-rw-rw-   0        0        0    10093 2023-05-26 08:59:17.000000 n0struct-0.2.98/n0struct/n0struct_n0dict_.py
+-rw-rw-rw-   0        0        0    17116 2023-05-13 12:19:09.000000 n0struct-0.2.98/n0struct/n0struct_n0dict__.py
+-rw-rw-rw-   0        0        0     8568 2023-05-22 16:31:02.000000 n0struct-0.2.98/n0struct/n0struct_n0list_.py
+-rw-rw-rw-   0        0        0    75645 2023-05-13 12:22:04.000000 n0struct-0.2.98/n0struct/n0struct_n0list_n0dict.py
+-rw-rw-rw-   0        0        0      917 2023-04-25 08:08:57.000000 n0struct-0.2.98/n0struct/n0struct_random.py
+-rw-rw-rw-   0        0        0     3852 2023-04-25 08:08:57.000000 n0struct-0.2.98/n0struct/n0struct_references.py
+-rw-rw-rw-   0        0        0     3235 2023-05-12 12:49:17.000000 n0struct-0.2.98/n0struct/n0struct_transform_structure.py
+-rw-rw-rw-   0        0        0    18218 2023-05-14 15:31:16.000000 n0struct-0.2.98/n0struct/n0struct_utils.py
+-rw-rw-rw-   0        0        0     6659 2023-05-12 12:42:29.000000 n0struct-0.2.98/n0struct/n0struct_utils_compare.py
+-rw-rw-rw-   0        0        0     4120 2023-05-12 12:42:54.000000 n0struct-0.2.98/n0struct/n0struct_utils_find.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:01:32.347421 n0struct-0.2.98/n0struct/test/
+-rw-rw-rw-   0        0        0        0 2022-09-04 19:16:09.000000 n0struct-0.2.98/n0struct/test/__init__.py
+-rw-rw-rw-   0        0        0      136 2022-09-04 19:16:09.000000 n0struct-0.2.98/n0struct/test/__main__.py
+-rw-rw-rw-   0        0        0    33051 2023-05-13 12:06:10.000000 n0struct-0.2.98/n0struct/test/test_n0struct.py
+-rw-rw-rw-   0        0        0     2572 2023-03-06 04:48:48.000000 n0struct-0.2.98/n0struct/test/test_n0struct2.py
+-rw-rw-rw-   0        0        0      890 2023-05-13 12:07:38.000000 n0struct-0.2.98/n0struct/test/test_n0struct3.py
+-rw-rw-rw-   0        0        0     1490 2023-05-13 12:23:25.000000 n0struct-0.2.98/n0struct/test/test_n0struct4.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:01:32.347421 n0struct-0.2.98/n0struct.egg-info/
+-rw-rw-rw-   0        0        0     1060 2023-05-27 10:01:32.000000 n0struct-0.2.98/n0struct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1032 2023-05-27 10:01:32.000000 n0struct-0.2.98/n0struct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 10:01:32.000000 n0struct-0.2.98/n0struct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-27 10:01:32.000000 n0struct-0.2.98/n0struct.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-05-27 10:01:32.000000 n0struct-0.2.98/n0struct.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-27 10:01:32.000000 n0struct-0.2.98/n0struct.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 10:01:32.363011 n0struct-0.2.98/setup.cfg
+-rw-rw-rw-   0        0        0     2476 2023-04-02 07:28:40.000000 n0struct-0.2.98/setup.py
```

### Comparing `n0struct-0.2.97/LICENSE` & `n0struct-0.2.98/LICENSE`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/PKG-INFO` & `n0struct-0.2.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n0struct
-Version: 0.2.97
+Version: 0.2.98
 Summary: list/dict extensions allow to load/save/serialize/deserialize xml/json/csv/dsv/fwf files into python/from structures, compare them and work with them using xpath approach
 Home-page: https://github.com/pythonist552/n0struct/
 Author: pythonist552
 Author-email: pythonist552@gmail.com
 License: ASL
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `n0struct-0.2.97/README.md` & `n0struct-0.2.98/README.md`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/__init__.py` & `n0struct-0.2.98/n0struct/__init__.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/n0struct_arrays.py` & `n0struct-0.2.98/n0struct/n0struct_arrays.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/n0struct_comprehensions.py` & `n0struct-0.2.98/n0struct/n0struct_comprehensions.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/n0struct_date.py` & `n0struct-0.2.98/n0struct/n0struct_date.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/n0struct_files.py` & `n0struct-0.2.98/n0struct/n0struct_files.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/n0struct_files_csv.py` & `n0struct-0.2.98/n0struct/n0struct_files_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 from pathlib import Path
 from .n0struct_n0list_n0dict import n0dict
 from .n0struct_n0list_n0dict import n0list
 from n0struct import * # required to use external functions in validate_csv_row()
 # ******************************************************************************
 # ******************************************************************************
 def parse_complex_csv_line(
-    line: str,
-    delimiter: str = ',',
+    line: typing.Union[str, bytes],
+    delimiter: typing.Union[str, bytes] = ',',
     process_field: callable = lambda field_value: field_value,  # possible to field_value.strip()
-    EOL: str = '\n',
+    EOL: typing.Union[str, bytes] = '\n',
 ) -> list:
     fields_in_the_row = []
     flag_quotes_in_the_begining = flag_expect_delimiter_or_quotes = False
     field_value = ""
     for offset, ch in enumerate(line.strip(EOL)):
+        if isinstance(ch, int):
+            ch = chr(ch)
         if ch == delimiter and (flag_quotes_in_the_begining == False or flag_expect_delimiter_or_quotes == True):
             # The next field is started
             fields_in_the_row.append(process_field(field_value))
             flag_quotes_in_the_begining = flag_expect_delimiter_or_quotes = False
             field_value = ""
             continue  # skip delimiter
         elif ch == '"':
@@ -42,15 +44,15 @@
     file_name: str,
     column_names: typing.Union[list, tuple, None] = None,
     delimiter: str = ',',
     process_field: typing.Union[callable, None] = None,
     # process_field == None
     #   strip_field == False                    lambda field_value: field_value
     #   strip_field == True                     lambda field_value: field_value.strip()
-    EOL: str = '\n',
+    EOL: str = None,   # AUTO # EOL: str = '\r\n',  # FOR WINDOWS ONLY!!!
     contains_header: typing.Union[bool, str, list, tuple, None] = None,
     # contains_header == True || False          ***LEGACY***
     #   header_is_mandatory == None             Copy value from contains_header into header_is_mandatory
     #   header_is_mandatory != contains_header  Exception
     #
     # contains_header == "???"
     #   contains_header == row[0]
@@ -164,27 +166,34 @@
         if isinstance(strip_line, bool) and strip_line == True:
             process_line = lambda line_value: line_value.strip()
         elif callable(strip_line):
             process_line = strip_line
         else:
             process_line = lambda line_value: line_value
 
+    if read_mode == 'b':
+        EOL = EOL.encode('cp1251')
 
-    with open(file_name, mode='r'+read_mode, encoding=encoding) as in_file:
+    with open(
+        file_name,
+        mode='r'+read_mode,
+        encoding=encoding if read_mode == 't' else None,
+        newline=EOL if read_mode == 't' else None
+    ) as in_file:
         # skip empty lines at the begining of the file
         while True:
             file_offset = in_file.tell()
             line = in_file.readline()  # removed walrus operator for compatibility with 3.7
             if not line:
                 raise EOFError("Empty file or file only with spaces")
             header_line = process_line(line.rstrip(EOL))
             if header_line:
                 break
 
-        possible_column_names = parse_csv_line(header_line, delimiter, process_field)
+        possible_column_names = parse_csv_line(header_line, delimiter, process_field, EOL)
 
         first_line_is_header = False
         if contains_header:
             if isinstance(contains_header, str):
                 if possible_column_names[0] != contains_header:
                     if header_is_mandatory:
                         raise ReferenceError(f"First line is not header {possible_column_names}. Expected first column '{contains_header}'")
```

### Comparing `n0struct-0.2.97/n0struct/n0struct_files_fwf.py` & `n0struct-0.2.98/n0struct/n0struct_files_fwf.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/n0struct_findall.py` & `n0struct-0.2.98/n0struct/n0struct_findall.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/n0struct_git.py` & `n0struct-0.2.98/n0struct/n0struct_git.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/n0struct_logging.py` & `n0struct-0.2.98/n0struct/n0struct_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 __debug_show_object_type = True
 def set_debug_show_object_type(debug_show_object_type: bool):
     global __debug_show_object_type
     __debug_show_object_type = debug_show_object_type
 
 
-__debug_show_object_id = True
+__debug_show_object_id = False
 def set_debug_show_object_id(debug_show_object_id: bool):
     global __debug_show_object_id
     __debug_show_object_id = debug_show_object_id
 
 
 __debug_show_item_count = True
 def set_debug_show_item_count(debug_show_item_count: bool):
@@ -353,41 +353,27 @@
     depends of value in global variable __debug_level.
 
     :param var_object:
     :param var_name:
     :param level:
     :return:
     """
-    prefix = (
-                (str(type(var_object)) or "").replace("<class '", "<").replace("'>", ">")
-                if __debug_show_object_type
-                else ""
-             ) + (
-                (
-                    (" " if __debug_show_object_type else "") + f"id={id(var_object)}"
-                )
-                if __debug_show_object_id
-                else ""
-             )
-    if prefix:
-        prefix += " "
-
     n0print(
-        f"{prefix}{var_name}{' == ' if prefix or var_name else ''}" +
-            n0pretty(
-                var_object,
-                show_type = show_type,
-                pairs_in_one_line = pairs_in_one_line,
-                json_convention = json_convention,
-                skip_empty_arrays = skip_empty_arrays,
-                skip_simple_types = skip_simple_types,
-                auto_quotes = auto_quotes,
-                show_item_count = show_item_count,
-            )
-        ,
+        (f"id={id(var_object)} " if __debug_show_object_id else "")
+        + (f"{var_name} == " if var_name else "")
+        + n0pretty(
+            var_object,
+            show_type = show_type,
+            pairs_in_one_line = pairs_in_one_line,
+            json_convention = json_convention,
+            skip_empty_arrays = skip_empty_arrays,
+            skip_simple_types = skip_simple_types,
+            auto_quotes = auto_quotes,
+            show_item_count = show_item_count,
+        ),
         level = level,
         internal_call = internal_call + 1,
     )
 # ******************************************************************************
 def n0debug(var_name: str, level: str = "DEBUG",
 
             show_type: bool = None,
```

### Comparing `n0struct-0.2.97/n0struct/n0struct_mask.py` & `n0struct-0.2.98/n0struct/n0struct_mask.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/n0struct_n0dict_.py` & `n0struct-0.2.98/n0struct/n0struct_n0dict_.py`

 * *Files 17% similar despite different names*

```diff
@@ -101,39 +101,36 @@
                 if not len(parent.items()):
                     return ""
                 for key, value in parent.items():
                     if result:
                         result += "\n"
                         
                     if isinstance(value, (list, tuple)):
-                        for i, subitm in enumerate(value):
-                            if i:
-                                result += "\n"
-                            sub_result = self.__xml(subitm, indent+inc_indent, inc_indent)
-                            if not sub_result:
-                                if isinstance(sub_result, str):
-                                    result += " "*indent + f"<{key}></{key}>"
-                                else:
-                                    result += " "*indent + f"<{key}/>"
-                            else:
-                                if '>' in sub_result:
-                                    result += " "*indent + f"<{key}>\n{sub_result}\n" + " "*indent + f"</{key}>"
-                                else:
-                                    result += " "*indent + f"<{key}>{sub_result}</{key}>"
+                        if not value:
+                            result += " "*indent + f"<{key}/>"
+                        else:
+                            result += " "*indent + f"<{key}>"
+                            for i, subitm in enumerate(value):
+                                result += "\n" + self.__xml(subitm, indent+inc_indent, inc_indent)
+                            result += "\n" +" "*indent + f"</{key}>"
                     elif isinstance(value, (int, float)):
                         if not key.startswith("@"):
                             result += " "*indent + f"<{key}>{value}</{key}>"
+                        else:
+                            raise NotImplementedError(f"Export of attibtures ({key}) is not supported yet")
                     elif isinstance(value, str):
                         if not key.startswith("@"):
                             result += " "*indent + f"<{key}>"
                             if value.lstrip().upper().startswith("<![CDATA[") and value.rstrip().endswith("]]>"):
-                                result += value
+                                result += "\n" + " "*(indent+inc_indent) + value + "\n" + " "*indent
                             else:
                                 result += value.translate(html_entities)
                             result += f"</{key}>"
+                        else:
+                            raise NotImplementedError(f"Export of attibtures ({key}) is not supported yet")
                     elif isinstance(value, dict):
                         sub_result = self.__xml(value, indent+inc_indent, inc_indent)
 
                         attribs = ""
                         attribs_of_current_key = [(__key[1:], __value) for __key,__value in value.items() if __key.startswith("@")]
                         if len(attribs_of_current_key):
                             for __key, __value in attribs_of_current_key:
@@ -167,51 +164,14 @@
         Public function: export self into xml result string
         """
         return (f'<?xml version={quote}1.0{quote} encoding={quote}{encoding}{quote}?>\n' if encoding else '') + \
             self.__xml(self, 0, indent)
     # **************************************************************************
     # JSON
     # **************************************************************************
-    def __json(self, parent: dict, indent: int, inc_indent: int) -> str:
-        """
-        Private function: recursively export n0dict into json result string
-        """
-        result = ""
-        for key, value in parent.items():
-            if result:
-                result += ",\n"
-            if isinstance(value, list):
-                sub_result = ""
-                for i, subitm in enumerate(value):
-                    if sub_result:
-                        sub_result += ",\n"
-                    sub_sub_result = self.__json(subitm, (indent+inc_indent)*2, inc_indent)
-                    if sub_sub_result:
-                        if isinstance(subitm, dict):
-                            sub_result += " "*(indent+inc_indent) + "{" + f"\n{sub_sub_result}\n" + " "*(indent+inc_indent) + "}"
-                        elif isinstance(subitm, (list, tuple)):
-                            sub_result += " "*(indent+inc_indent) + f"[\n{sub_sub_result}\n" + " "*(indent+inc_indent) + "]"
-                if sub_result:
-                    result += " "*indent + f'"{key}": [\n{sub_result}\n' + " "*indent + "]"
-                else:
-                    result += " "*indent + f'"{key}": null'
-            elif isinstance(value, str):
-                result += " "*indent + f'"{key}": "{value}"'
-            elif isinstance(value, dict):
-                sub_result = self.__json(value, indent+inc_indent, inc_indent)
-                if sub_result:
-                    result += " "*indent + f'"{key}": ' + "{" + f"\n{sub_result}\n" + " "*indent + "}"
-                else:
-                    result += " "*indent + f'"{key}": null'
-            elif value is None:
-                result += " "*indent + f'"{key}": null'
-            else:
-                raise TypeError(f"Unknown type ({type(value)}) {key} == {value}")
-        return result
-    # **************************************************************************
     def to_json(self,
                 indent: int = 4,
                 pairs_in_one_line = True,
                 json_convention: bool = True,
                 skip_empty_arrays: bool = False,
                 compress: bool = False,
     ) -> str:
```

### Comparing `n0struct-0.2.97/n0struct/n0struct_n0dict__.py` & `n0struct-0.2.98/n0struct/n0struct_n0dict__.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/n0struct_n0list_.py` & `n0struct-0.2.98/n0struct/n0struct_n0list_.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import typing
 from .n0struct_utils import n0eval
 from .n0struct_findall import findall as n0struct_findall__findall
 from .n0struct_findall import findfirst as n0struct_findall__findfirst
+from .n0struct_logging import n0pretty
 # ******************************************************************************
 # ******************************************************************************
 class n0list_(list):
     def findall(self, xpath: str, raise_exception: bool = True):
         return n0struct_findall__findall(self, xpath, raise_exception)
     def findfirst(self, xpath: str, raise_exception: bool = True):
         return n0struct_findall__findfirst(self, xpath, raise_exception)
@@ -143,9 +144,35 @@
         return not self._consists_of(other_list, False)
     # **************************************************************************
     def __contains__(self, other_list):  # otherlist in n0list_([a])
         return self.consists_of_all(other_list)
     # **************************************************************************
     def not_consists_of_any(self, other_list):
         return not self._consists_of(other_list, True)
+    # **************************************************************************
+    # JSON
+    # **************************************************************************
+    def to_json(self,
+                indent: int = 4,
+                pairs_in_one_line = True,
+                json_convention: bool = True,
+                skip_empty_arrays: bool = False,
+                compress: bool = False,
+    ) -> str:
+        """
+        Public function: export self into json result string
+        """
+        if compress:
+            indent = 0
+
+        return n0pretty(self,
+                        show_type=False,
+                        auto_quotes=False,
+                        __quotes='"',
+                        __indent_size=indent,
+                        pairs_in_one_line=pairs_in_one_line,
+                        json_convention=json_convention,
+                        skip_empty_arrays=skip_empty_arrays,
+                        show_item_count=False,
+        )
 # ******************************************************************************
 # ******************************************************************************
```

### Comparing `n0struct-0.2.97/n0struct/n0struct_n0list_n0dict.py` & `n0struct-0.2.98/n0struct/n0struct_n0list_n0dict.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/n0struct_random.py` & `n0struct-0.2.98/n0struct/n0struct_random.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/n0struct_references.py` & `n0struct-0.2.98/n0struct/n0struct_references.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/n0struct_transform_structure.py` & `n0struct-0.2.98/n0struct/n0struct_transform_structure.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/n0struct_utils.py` & `n0struct-0.2.98/n0struct/n0struct_utils.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/n0struct_utils_compare.py` & `n0struct-0.2.98/n0struct/n0struct_utils_compare.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/n0struct_utils_find.py` & `n0struct-0.2.98/n0struct/n0struct_utils_find.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/test/test_n0struct.py` & `n0struct-0.2.98/n0struct/test/test_n0struct.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/test/test_n0struct2.py` & `n0struct-0.2.98/n0struct/test/test_n0struct2.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/test/test_n0struct3.py` & `n0struct-0.2.98/n0struct/test/test_n0struct3.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct/test/test_n0struct4.py` & `n0struct-0.2.98/n0struct/test/test_n0struct4.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/n0struct.egg-info/PKG-INFO` & `n0struct-0.2.98/n0struct.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n0struct
-Version: 0.2.97
+Version: 0.2.98
 Summary: list/dict extensions allow to load/save/serialize/deserialize xml/json/csv/dsv/fwf files into python/from structures, compare them and work with them using xpath approach
 Home-page: https://github.com/pythonist552/n0struct/
 Author: pythonist552
 Author-email: pythonist552@gmail.com
 License: ASL
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `n0struct-0.2.97/n0struct.egg-info/SOURCES.txt` & `n0struct-0.2.98/n0struct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.97/setup.py` & `n0struct-0.2.98/setup.py`

 * *Files identical despite different names*

