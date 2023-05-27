# Comparing `tmp/asm2cfg-0.2.1.tar.gz` & `tmp/asm2cfg-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asm2cfg-0.2.1.tar", last modified: Sun Jun  5 15:08:49 2022, max compression
+gzip compressed data, was "asm2cfg-0.2.2.tar", last modified: Sat May 27 13:23:20 2023, max compression
```

## Comparing `asm2cfg-0.2.1.tar` & `asm2cfg-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 kazhuu    (1001) users      (984)        0 2022-06-05 15:08:49.339739 asm2cfg-0.2.1/
--rw-r--r--   0 kazhuu    (1001) users      (984)     1071 2022-02-27 15:19:58.000000 asm2cfg-0.2.1/LICENSE
--rw-r--r--   0 kazhuu    (1001) users      (984)    11746 2022-06-05 15:08:49.339739 asm2cfg-0.2.1/PKG-INFO
--rw-r--r--   0 kazhuu    (1001) users      (984)    11180 2022-06-05 15:00:09.000000 asm2cfg-0.2.1/README.md
--rw-r--r--   0 kazhuu    (1001) users      (984)      104 2022-02-27 15:19:58.000000 asm2cfg-0.2.1/pyproject.toml
--rw-r--r--   0 kazhuu    (1001) users      (984)     1313 2022-06-05 15:08:49.339739 asm2cfg-0.2.1/setup.cfg
-drwxr-xr-x   0 kazhuu    (1001) users      (984)        0 2022-06-05 15:08:49.339739 asm2cfg-0.2.1/src/
-drwxr-xr-x   0 kazhuu    (1001) users      (984)        0 2022-06-05 15:08:49.339739 asm2cfg-0.2.1/src/asm2cfg/
--rw-r--r--   0 kazhuu    (1001) users      (984)        0 2022-02-27 15:19:58.000000 asm2cfg-0.2.1/src/asm2cfg/__init__.py
--rw-r--r--   0 kazhuu    (1001) users      (984)      193 2022-02-27 15:19:58.000000 asm2cfg-0.2.1/src/asm2cfg/__main__.py
--rw-r--r--   0 kazhuu    (1001) users      (984)    20593 2022-06-05 05:29:06.000000 asm2cfg-0.2.1/src/asm2cfg/asm2cfg.py
--rw-r--r--   0 kazhuu    (1001) users      (984)     1263 2022-03-27 15:13:15.000000 asm2cfg-0.2.1/src/asm2cfg/command_line.py
-drwxr-xr-x   0 kazhuu    (1001) users      (984)        0 2022-06-05 15:08:49.339739 asm2cfg-0.2.1/src/asm2cfg.egg-info/
--rw-r--r--   0 kazhuu    (1001) users      (984)    11746 2022-06-05 15:08:49.000000 asm2cfg-0.2.1/src/asm2cfg.egg-info/PKG-INFO
--rw-r--r--   0 kazhuu    (1001) users      (984)      428 2022-06-05 15:08:49.000000 asm2cfg-0.2.1/src/asm2cfg.egg-info/SOURCES.txt
--rw-r--r--   0 kazhuu    (1001) users      (984)        1 2022-06-05 15:08:49.000000 asm2cfg-0.2.1/src/asm2cfg.egg-info/dependency_links.txt
--rw-r--r--   0 kazhuu    (1001) users      (984)       54 2022-06-05 15:08:49.000000 asm2cfg-0.2.1/src/asm2cfg.egg-info/entry_points.txt
--rw-r--r--   0 kazhuu    (1001) users      (984)       15 2022-06-05 15:08:49.000000 asm2cfg-0.2.1/src/asm2cfg.egg-info/requires.txt
--rw-r--r--   0 kazhuu    (1001) users      (984)        8 2022-06-05 15:08:49.000000 asm2cfg-0.2.1/src/asm2cfg.egg-info/top_level.txt
--rw-r--r--   0 kazhuu    (1001) users      (984)     3934 2022-06-05 15:00:09.000000 asm2cfg-0.2.1/src/gdb_asm2cfg.py
-drwxr-xr-x   0 kazhuu    (1001) users      (984)        0 2022-06-05 15:08:49.339739 asm2cfg-0.2.1/test/
--rw-r--r--   0 kazhuu    (1001) users      (984)     3179 2022-03-01 00:59:54.000000 asm2cfg-0.2.1/test/test_gdb.py
--rw-r--r--   0 kazhuu    (1001) users      (984)    13539 2022-03-27 15:13:15.000000 asm2cfg-0.2.1/test/test_parser.py
--rw-r--r--   0 kazhuu    (1001) users      (984)     6323 2022-03-27 15:13:15.000000 asm2cfg-0.2.1/test/test_regex.py
+drwxr-xr-x   0 kazhuu    (1001) users      (984)        0 2023-05-27 13:23:20.512737 asm2cfg-0.2.2/
+-rw-r--r--   0 kazhuu    (1001) users      (984)     1071 2022-02-27 15:19:58.000000 asm2cfg-0.2.2/LICENSE
+-rw-r--r--   0 kazhuu    (1001) users      (984)    11478 2023-05-27 13:23:20.512737 asm2cfg-0.2.2/PKG-INFO
+-rw-r--r--   0 kazhuu    (1001) users      (984)    10877 2023-05-27 06:52:14.000000 asm2cfg-0.2.2/README.md
+-rw-r--r--   0 kazhuu    (1001) users      (984)      104 2022-02-27 15:19:58.000000 asm2cfg-0.2.2/pyproject.toml
+-rw-r--r--   0 kazhuu    (1001) users      (984)     1348 2023-05-27 13:23:20.512737 asm2cfg-0.2.2/setup.cfg
+drwxr-xr-x   0 kazhuu    (1001) users      (984)        0 2023-05-27 13:23:20.509403 asm2cfg-0.2.2/src/
+drwxr-xr-x   0 kazhuu    (1001) users      (984)        0 2023-05-27 13:23:20.509403 asm2cfg-0.2.2/src/asm2cfg/
+-rw-r--r--   0 kazhuu    (1001) users      (984)        0 2022-02-27 15:19:58.000000 asm2cfg-0.2.2/src/asm2cfg/__init__.py
+-rw-r--r--   0 kazhuu    (1001) users      (984)      193 2022-02-27 15:19:58.000000 asm2cfg-0.2.2/src/asm2cfg/__main__.py
+-rw-r--r--   0 kazhuu    (1001) users      (984)    20594 2023-05-27 13:17:07.000000 asm2cfg-0.2.2/src/asm2cfg/asm2cfg.py
+-rw-r--r--   0 kazhuu    (1001) users      (984)     1263 2022-03-27 15:13:15.000000 asm2cfg-0.2.2/src/asm2cfg/command_line.py
+drwxr-xr-x   0 kazhuu    (1001) users      (984)        0 2023-05-27 13:23:20.509403 asm2cfg-0.2.2/src/asm2cfg.egg-info/
+-rw-r--r--   0 kazhuu    (1001) users      (984)    11478 2023-05-27 13:23:20.000000 asm2cfg-0.2.2/src/asm2cfg.egg-info/PKG-INFO
+-rw-r--r--   0 kazhuu    (1001) users      (984)      428 2023-05-27 13:23:20.000000 asm2cfg-0.2.2/src/asm2cfg.egg-info/SOURCES.txt
+-rw-r--r--   0 kazhuu    (1001) users      (984)        1 2023-05-27 13:23:20.000000 asm2cfg-0.2.2/src/asm2cfg.egg-info/dependency_links.txt
+-rw-r--r--   0 kazhuu    (1001) users      (984)       54 2023-05-27 13:23:20.000000 asm2cfg-0.2.2/src/asm2cfg.egg-info/entry_points.txt
+-rw-r--r--   0 kazhuu    (1001) users      (984)       15 2023-05-27 13:23:20.000000 asm2cfg-0.2.2/src/asm2cfg.egg-info/requires.txt
+-rw-r--r--   0 kazhuu    (1001) users      (984)        8 2023-05-27 13:23:20.000000 asm2cfg-0.2.2/src/asm2cfg.egg-info/top_level.txt
+-rw-r--r--   0 kazhuu    (1001) users      (984)     3934 2022-06-05 15:00:09.000000 asm2cfg-0.2.2/src/gdb_asm2cfg.py
+drwxr-xr-x   0 kazhuu    (1001) users      (984)        0 2023-05-27 13:23:20.512737 asm2cfg-0.2.2/test/
+-rw-r--r--   0 kazhuu    (1001) users      (984)     3179 2022-03-01 00:59:54.000000 asm2cfg-0.2.2/test/test_gdb.py
+-rw-r--r--   0 kazhuu    (1001) users      (984)    13591 2023-05-27 06:50:20.000000 asm2cfg-0.2.2/test/test_parser.py
+-rw-r--r--   0 kazhuu    (1001) users      (984)     6662 2023-05-27 13:17:07.000000 asm2cfg-0.2.2/test/test_regex.py
```

### Comparing `asm2cfg-0.2.1/LICENSE` & `asm2cfg-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asm2cfg-0.2.1/PKG-INFO` & `asm2cfg-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: asm2cfg
-Version: 0.2.1
-Summary: GDB extension to add commands to view and save disassembled functions as a dot control-flow graphs.
+Version: 0.2.2
+Summary: Python command-line tool and GDB extension to view and save x86, ARM and objdump assembly files as control-flow graph (CFG) pdf files.
 Home-page: https://github.com/Kazhuu/asm2cfg
 Author: Mauri Mustonen
 Author-email: kazooiebombchu@gmail.com
 Project-URL: Bug Tracker, https://github.com/Kazhuu/asm2cfg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,16 +13,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # asm2cfg
 ![CI status](https://github.com/Kazhuu/asm2cfg/actions/workflows/ci.yml/badge.svg)
 [![codecov](https://codecov.io/gh/Kazhuu/asm2cfg/branch/main/graph/badge.svg?token=ZHLOJO8Q3V)](https://codecov.io/gh/Kazhuu/asm2cfg)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/Kazhuu/asm2cfg.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Kazhuu/asm2cfg/alerts/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Kazhuu/asm2cfg.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Kazhuu/asm2cfg/context:python)
 
 Python command-line tool and GDB extension to view and save x86, ARM and objdump
 assembly files as control-flow graph (CFG) pdf files. From GDB debugging session
 use `viewcfg` command to view CFG and use `savecfg` command to save it to the
 pdf file.
 
 <p align="center">
@@ -38,25 +36,25 @@
 ## Table of Content
 
 <!-- vim-markdown-toc GFM -->
 
 * [Install](#install)
 * [Usage From GDB](#usage-from-gdb)
 * [Usage as Standalone](#usage-as-standalone)
-  * [Knowing Function Name](#knowing-function-name)
-  * [Disassemble Function](#disassemble-function)
-  * [Draw CFG](#draw-cfg)
-  * [Examples](#examples)
+    * [Knowing Function Name](#knowing-function-name)
+    * [Disassemble Function](#disassemble-function)
+    * [Draw CFG](#draw-cfg)
+    * [Examples](#examples)
 * [Development](#development)
-  * [Python Environment](#python-environment)
-  * [Testing](#testing)
-  * [Code Linting](#code-linting)
-  * [Command-Line Interface](#command-line-interface)
-  * [GDB Integration](#gdb-integration)
-  * [Current Development Goals](#current-development-goals)
+    * [Python Environment](#python-environment)
+    * [Testing](#testing)
+    * [Code Linting](#code-linting)
+    * [Command-Line Interface](#command-line-interface)
+    * [GDB Integration](#gdb-integration)
+    * [Current Development Goals](#current-development-goals)
 
 <!-- vim-markdown-toc -->
 
 ## Install
 
 Project can be installed with pip
```

### Comparing `asm2cfg-0.2.1/README.md` & `asm2cfg-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 
 # asm2cfg
 ![CI status](https://github.com/Kazhuu/asm2cfg/actions/workflows/ci.yml/badge.svg)
 [![codecov](https://codecov.io/gh/Kazhuu/asm2cfg/branch/main/graph/badge.svg?token=ZHLOJO8Q3V)](https://codecov.io/gh/Kazhuu/asm2cfg)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/Kazhuu/asm2cfg.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Kazhuu/asm2cfg/alerts/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Kazhuu/asm2cfg.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Kazhuu/asm2cfg/context:python)
 
 Python command-line tool and GDB extension to view and save x86, ARM and objdump
 assembly files as control-flow graph (CFG) pdf files. From GDB debugging session
 use `viewcfg` command to view CFG and use `savecfg` command to save it to the
 pdf file.
 
 <p align="center">
@@ -23,25 +21,25 @@
 ## Table of Content
 
 <!-- vim-markdown-toc GFM -->
 
 * [Install](#install)
 * [Usage From GDB](#usage-from-gdb)
 * [Usage as Standalone](#usage-as-standalone)
-  * [Knowing Function Name](#knowing-function-name)
-  * [Disassemble Function](#disassemble-function)
-  * [Draw CFG](#draw-cfg)
-  * [Examples](#examples)
+    * [Knowing Function Name](#knowing-function-name)
+    * [Disassemble Function](#disassemble-function)
+    * [Draw CFG](#draw-cfg)
+    * [Examples](#examples)
 * [Development](#development)
-  * [Python Environment](#python-environment)
-  * [Testing](#testing)
-  * [Code Linting](#code-linting)
-  * [Command-Line Interface](#command-line-interface)
-  * [GDB Integration](#gdb-integration)
-  * [Current Development Goals](#current-development-goals)
+    * [Python Environment](#python-environment)
+    * [Testing](#testing)
+    * [Code Linting](#code-linting)
+    * [Command-Line Interface](#command-line-interface)
+    * [GDB Integration](#gdb-integration)
+    * [Current Development Goals](#current-development-goals)
 
 <!-- vim-markdown-toc -->
 
 ## Install
 
 Project can be installed with pip
```

### Comparing `asm2cfg-0.2.1/setup.cfg` & `asm2cfg-0.2.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = asm2cfg
-version = 0.2.1
+version = 0.2.2
 author = Mauri Mustonen
 author_email = kazooiebombchu@gmail.com
-description = GDB extension to add commands to view and save disassembled functions as a dot control-flow graphs.
+description = Python command-line tool and GDB extension to view and save x86, ARM and objdump assembly files as control-flow graph (CFG) pdf files.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Kazhuu/asm2cfg
 project_urls = 
 	Bug Tracker = https://github.com/Kazhuu/asm2cfg/issues
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `asm2cfg-0.2.1/src/asm2cfg/asm2cfg.py` & `asm2cfg-0.2.2/src/asm2cfg/asm2cfg.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,15 @@
     return body, opcode, ops, line
 
 
 def parse_target(line):
     """
     Parses optional instruction branch target hint
     """
-    target_match = re.match(r'\s*<([a-zA-Z_@0-9]+)([+-]0x[0-9a-f]+|[+-][0-9]+)?>(.*)', line)
+    target_match = re.match(r'\s*<([a-zA-Z_@.0-9]+)([+-]0x[0-9a-f]+|[+-][0-9]+)?>(.*)', line)
     if target_match is None:
         return None, line
     offset = target_match[2] or '+0'
     address = Address(None, target_match[1], int(offset, 0))
     return address, target_match[3]
```

### Comparing `asm2cfg-0.2.1/src/asm2cfg/command_line.py` & `asm2cfg-0.2.2/src/asm2cfg/command_line.py`

 * *Files identical despite different names*

### Comparing `asm2cfg-0.2.1/src/asm2cfg.egg-info/PKG-INFO` & `asm2cfg-0.2.2/src/asm2cfg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: asm2cfg
-Version: 0.2.1
-Summary: GDB extension to add commands to view and save disassembled functions as a dot control-flow graphs.
+Version: 0.2.2
+Summary: Python command-line tool and GDB extension to view and save x86, ARM and objdump assembly files as control-flow graph (CFG) pdf files.
 Home-page: https://github.com/Kazhuu/asm2cfg
 Author: Mauri Mustonen
 Author-email: kazooiebombchu@gmail.com
 Project-URL: Bug Tracker, https://github.com/Kazhuu/asm2cfg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,16 +13,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # asm2cfg
 ![CI status](https://github.com/Kazhuu/asm2cfg/actions/workflows/ci.yml/badge.svg)
 [![codecov](https://codecov.io/gh/Kazhuu/asm2cfg/branch/main/graph/badge.svg?token=ZHLOJO8Q3V)](https://codecov.io/gh/Kazhuu/asm2cfg)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/Kazhuu/asm2cfg.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Kazhuu/asm2cfg/alerts/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Kazhuu/asm2cfg.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Kazhuu/asm2cfg/context:python)
 
 Python command-line tool and GDB extension to view and save x86, ARM and objdump
 assembly files as control-flow graph (CFG) pdf files. From GDB debugging session
 use `viewcfg` command to view CFG and use `savecfg` command to save it to the
 pdf file.
 
 <p align="center">
@@ -38,25 +36,25 @@
 ## Table of Content
 
 <!-- vim-markdown-toc GFM -->
 
 * [Install](#install)
 * [Usage From GDB](#usage-from-gdb)
 * [Usage as Standalone](#usage-as-standalone)
-  * [Knowing Function Name](#knowing-function-name)
-  * [Disassemble Function](#disassemble-function)
-  * [Draw CFG](#draw-cfg)
-  * [Examples](#examples)
+    * [Knowing Function Name](#knowing-function-name)
+    * [Disassemble Function](#disassemble-function)
+    * [Draw CFG](#draw-cfg)
+    * [Examples](#examples)
 * [Development](#development)
-  * [Python Environment](#python-environment)
-  * [Testing](#testing)
-  * [Code Linting](#code-linting)
-  * [Command-Line Interface](#command-line-interface)
-  * [GDB Integration](#gdb-integration)
-  * [Current Development Goals](#current-development-goals)
+    * [Python Environment](#python-environment)
+    * [Testing](#testing)
+    * [Code Linting](#code-linting)
+    * [Command-Line Interface](#command-line-interface)
+    * [GDB Integration](#gdb-integration)
+    * [Current Development Goals](#current-development-goals)
 
 <!-- vim-markdown-toc -->
 
 ## Install
 
 Project can be installed with pip
```

### Comparing `asm2cfg-0.2.1/src/gdb_asm2cfg.py` & `asm2cfg-0.2.2/src/gdb_asm2cfg.py`

 * *Files identical despite different names*

### Comparing `asm2cfg-0.2.1/test/test_gdb.py` & `asm2cfg-0.2.2/test/test_gdb.py`

 * *Files identical despite different names*

### Comparing `asm2cfg-0.2.1/test/test_parser.py` & `asm2cfg-0.2.2/test/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,15 +267,17 @@
    0x0000555555570058 <+1800>:	mov    0xe0(%rsp),%rdi
    0x0000555555570060 <+1808>:	test   %rdi,%rdi
 '''.split('\n')
         _, blocks = asm2cfg.parse_lines(lines, False, 'x86')
 
         self.assertEqual(len(blocks), 2)
 
-        ret_block, other_block = blocks.values()
+        blocks = list(blocks.values())
+        ret_block = blocks[0]
+        other_block = blocks[1]
 
         self.assertIs(ret_block.jump_edge, None)
         self.assertIs(ret_block.no_jump_edge, None)
         self.assertEqual(len(ret_block.instructions), 1)
 
         self.assertIs(other_block.jump_edge, None)
         self.assertIs(other_block.no_jump_edge, None)
```

### Comparing `asm2cfg-0.2.1/test/test_regex.py` & `asm2cfg-0.2.2/test/test_regex.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,14 +150,24 @@
 
         self.assertIsNot(address, None)
         self.assertIs(address.abs, None)
         self.assertEqual(address.base, '_Z19exportDebugifyStats')
         self.assertEqual(address.offset, 0)
         self.assertEqual(rest, '')
 
+    def test_with_dot(self):
+        line = '<stdin@GLIBC_2.2.5>'
+        address, rest = asm2cfg.parse_target(line)
+
+        self.assertIsNot(address, None)
+        self.assertIs(address.abs, None)
+        self.assertEqual(address.base, 'stdin@GLIBC_2.2.5')
+        self.assertEqual(address.offset, 0)
+        self.assertEqual(rest, '')
+
 
 class ParseCommentTestCase(unittest.TestCase):
     """
     Tests of parse_comment function
     """
 
     def setUp(self):
```

