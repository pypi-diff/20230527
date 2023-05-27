# Comparing `tmp/test_helper_vbot3-1.3.tar.gz` & `tmp/test_helper_vbot3-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_helper_vbot3-1.3.tar", last modified: Wed May 17 10:53:14 2023, max compression
+gzip compressed data, was "test_helper_vbot3-1.4.tar", last modified: Sat May 27 09:44:51 2023, max compression
```

## Comparing `test_helper_vbot3-1.3.tar` & `test_helper_vbot3-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 10:53:14.011744 test_helper_vbot3-1.3/
--rw-rw-rw-   0        0        0     1094 2023-05-13 15:59:41.000000 test_helper_vbot3-1.3/LICENSE
--rw-rw-rw-   0        0        0       60 2023-05-14 08:37:46.000000 test_helper_vbot3-1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1036 2023-05-17 10:53:14.011744 test_helper_vbot3-1.3/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-05-14 08:39:31.000000 test_helper_vbot3-1.3/README.md
--rw-rw-rw-   0        0        0      110 2023-05-14 08:37:46.000000 test_helper_vbot3-1.3/pyproject.toml
--rw-rw-rw-   0        0        0      707 2023-05-17 10:53:14.011744 test_helper_vbot3-1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-17 10:53:14.011744 test_helper_vbot3-1.3/test_helper_vbot3.egg-info/
--rw-rw-rw-   0        0        0     1036 2023-05-17 10:53:13.000000 test_helper_vbot3-1.3/test_helper_vbot3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-05-17 10:53:13.000000 test_helper_vbot3-1.3/test_helper_vbot3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 10:53:13.000000 test_helper_vbot3-1.3/test_helper_vbot3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-17 10:53:13.000000 test_helper_vbot3-1.3/test_helper_vbot3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-17 10:53:13.000000 test_helper_vbot3-1.3/test_helper_vbot3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 10:53:14.011744 test_helper_vbot3-1.3/tester_vbot3/
--rw-rw-rw-   0        0        0     4078 2023-05-16 07:09:11.000000 test_helper_vbot3-1.3/tester_vbot3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 09:44:51.779849 test_helper_vbot3-1.4/
+-rw-rw-rw-   0        0        0     1094 2023-05-13 15:59:41.000000 test_helper_vbot3-1.4/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-05-14 08:37:46.000000 test_helper_vbot3-1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1036 2023-05-27 09:44:51.779849 test_helper_vbot3-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-05-14 08:39:31.000000 test_helper_vbot3-1.4/README.md
+-rw-rw-rw-   0        0        0      110 2023-05-14 08:37:46.000000 test_helper_vbot3-1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      707 2023-05-27 09:44:51.779849 test_helper_vbot3-1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 09:44:51.779849 test_helper_vbot3-1.4/test_helper_vbot3.egg-info/
+-rw-rw-rw-   0        0        0     1036 2023-05-27 09:44:51.000000 test_helper_vbot3-1.4/test_helper_vbot3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-05-27 09:44:51.000000 test_helper_vbot3-1.4/test_helper_vbot3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 09:44:51.000000 test_helper_vbot3-1.4/test_helper_vbot3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-27 09:44:51.000000 test_helper_vbot3-1.4/test_helper_vbot3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-27 09:44:51.000000 test_helper_vbot3-1.4/test_helper_vbot3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 09:44:51.779849 test_helper_vbot3-1.4/tester_vbot3/
+-rw-rw-rw-   0        0        0     4078 2023-05-16 07:09:11.000000 test_helper_vbot3-1.4/tester_vbot3/__init__.py
```

### Comparing `test_helper_vbot3-1.3/LICENSE` & `test_helper_vbot3-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `test_helper_vbot3-1.3/PKG-INFO` & `test_helper_vbot3-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_helper_vbot3
-Version: 1.3
+Version: 1.4
 Summary: Tester for Vbot3
 Home-page: https://github.com/vb64/test.helper.vbot3
 Author: Vitaly Bogomolov
 Author-email: mail@vitaly-bogomolov.ru
 Project-URL: Bug Tracker, https://github.com/vb64/test.helper.vbot3/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `test_helper_vbot3-1.3/README.md` & `test_helper_vbot3-1.4/README.md`

 * *Files identical despite different names*

### Comparing `test_helper_vbot3-1.3/setup.cfg` & `test_helper_vbot3-1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6573 745f 6865 6c70 6572 5f76   = test_helper_v
 00000020: 626f 7433 0d0a 7665 7273 696f 6e20 3d20  bot3..version = 
-00000030: 312e 330d 0a61 7574 686f 7220 3d20 5669  1.3..author = Vi
+00000030: 312e 340d 0a61 7574 686f 7220 3d20 5669  1.4..author = Vi
 00000040: 7461 6c79 2042 6f67 6f6d 6f6c 6f76 0d0a  taly Bogomolov..
 00000050: 6175 7468 6f72 5f65 6d61 696c 203d 206d  author_email = m
 00000060: 6169 6c40 7669 7461 6c79 2d62 6f67 6f6d  ail@vitaly-bogom
 00000070: 6f6c 6f76 2e72 750d 0a64 6573 6372 6970  olov.ru..descrip
 00000080: 7469 6f6e 203d 2054 6573 7465 7220 666f  tion = Tester fo
 00000090: 7220 5662 6f74 330d 0a6c 6f6e 675f 6465  r Vbot3..long_de
 000000a0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
@@ -32,14 +32,14 @@
 000001f0: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
 00000200: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
 00000210: 7061 636b 6167 6573 203d 2074 6573 7465  packages = teste
 00000220: 725f 7662 6f74 330d 0a70 7974 686f 6e5f  r_vbot3..python_
 00000230: 7265 7175 6972 6573 203d 203e 3d33 2e37  requires = >=3.7
 00000240: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
 00000250: 6573 203d 200d 0a09 7465 6c65 6d75 6c61  es = ...telemula
-00000260: 746f 7233 3d3d 312e 330d 0a09 7465 7374  tor3==1.3...test
+00000260: 746f 7233 3d3d 312e 340d 0a09 7465 7374  tor3==1.4...test
 00000270: 6572 5f66 6c61 736b 3d3d 312e 320d 0a09  er_flask==1.2...
 00000280: 7465 7374 2d68 656c 7065 722d 6761 6533  test-helper-gae3
 00000290: 3d3d 312e 320d 0a0d 0a5b 6567 675f 696e  ==1.2....[egg_in
 000002a0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
 000002b0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
 000002c0: 0a0d 0a                                  ...
```

### Comparing `test_helper_vbot3-1.3/test_helper_vbot3.egg-info/PKG-INFO` & `test_helper_vbot3-1.4/test_helper_vbot3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-helper-vbot3
-Version: 1.3
+Version: 1.4
 Summary: Tester for Vbot3
 Home-page: https://github.com/vb64/test.helper.vbot3
 Author: Vitaly Bogomolov
 Author-email: mail@vitaly-bogomolov.ru
 Project-URL: Bug Tracker, https://github.com/vb64/test.helper.vbot3/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `test_helper_vbot3-1.3/tester_vbot3/__init__.py` & `test_helper_vbot3-1.4/tester_vbot3/__init__.py`

 * *Files identical despite different names*

