# Comparing `tmp/vision6D-0.0.8.tar.gz` & `tmp/vision6D-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vision6D-0.0.8.tar", last modified: Sat May 27 00:10:38 2023, max compression
+gzip compressed data, was "dist\vision6D-0.0.9.tar", last modified: Sat May 27 00:14:57 2023, max compression
```

## Comparing `vision6D-0.0.8.tar` & `vision6D-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 00:10:38.613222 vision6D-0.0.8/
--rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1603 2023-05-27 00:10:38.614312 vision6D-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-05-27 00:06:55.000000 vision6D-0.0.8/README.md
--rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0     1918 2023-05-27 00:10:38.619226 vision6D-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      366 2023-05-27 00:07:57.000000 vision6D-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 00:10:38.422145 vision6D-0.0.8/test/
--rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.0.8/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.0.8/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-05-27 00:10:38.467145 vision6D-0.0.8/vision6D/
--rw-rw-rw-   0        0        0    45165 2023-05-27 00:06:55.000000 vision6D-0.0.8/vision6D/GUI.py
--rw-rw-rw-   0        0        0      939 2023-05-27 00:06:55.000000 vision6D-0.0.8/vision6D/__init__.py
--rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.0.8/vision6D/app.py
--rw-rw-rw-   0        0        0    12369 2023-05-27 00:06:55.000000 vision6D-0.0.8/vision6D/config.py
-drwxrwxrwx   0        0        0        0 2023-05-27 00:10:38.600224 vision6D-0.0.8/vision6D/data/
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.0.8/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.0.8/vision6D/data/ossiclesCoordinateMappingv1.json
--rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.0.8/vision6D/data/style.qss
--rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.0.8/vision6D/interface.py
--rw-rw-rw-   0        0        0    27855 2023-05-27 00:06:55.000000 vision6D-0.0.8/vision6D/interface_gui.py
--rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.0.8/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.0.8/vision6D/run_gui.py
--rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.0.8/vision6D/run_interface.py
--rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.0.8/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-27 00:10:38.538156 vision6D-0.0.8/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1603 2023-05-27 00:10:37.000000 vision6D-0.0.8/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-05-27 00:10:37.000000 vision6D-0.0.8/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 00:10:37.000000 vision6D-0.0.8/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      248 2023-05-27 00:10:37.000000 vision6D-0.0.8/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-27 00:10:37.000000 vision6D-0.0.8/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 00:14:56.976513 vision6D-0.0.9/
+-rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1603 2023-05-27 00:14:56.976513 vision6D-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-05-27 00:06:55.000000 vision6D-0.0.9/README.md
+-rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1927 2023-05-27 00:14:56.981517 vision6D-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      165 2023-05-27 00:14:24.000000 vision6D-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 00:14:56.894510 vision6D-0.0.9/test/
+-rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.0.9/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.0.9/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-05-27 00:14:56.918515 vision6D-0.0.9/vision6D/
+-rw-rw-rw-   0        0        0    45165 2023-05-27 00:06:55.000000 vision6D-0.0.9/vision6D/GUI.py
+-rw-rw-rw-   0        0        0      939 2023-05-27 00:06:55.000000 vision6D-0.0.9/vision6D/__init__.py
+-rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.0.9/vision6D/app.py
+-rw-rw-rw-   0        0        0    12369 2023-05-27 00:06:55.000000 vision6D-0.0.9/vision6D/config.py
+drwxrwxrwx   0        0        0        0 2023-05-27 00:14:56.973513 vision6D-0.0.9/vision6D/data/
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.0.9/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.0.9/vision6D/data/ossiclesCoordinateMappingv1.json
+-rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.0.9/vision6D/data/style.qss
+-rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.0.9/vision6D/interface.py
+-rw-rw-rw-   0        0        0    27855 2023-05-27 00:06:55.000000 vision6D-0.0.9/vision6D/interface_gui.py
+-rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.0.9/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.0.9/vision6D/run_gui.py
+-rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.0.9/vision6D/run_interface.py
+-rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.0.9/vision6D/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-27 00:14:56.962515 vision6D-0.0.9/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1603 2023-05-27 00:14:56.000000 vision6D-0.0.9/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-05-27 00:14:56.000000 vision6D-0.0.9/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 00:14:56.000000 vision6D-0.0.9/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-05-27 00:14:56.000000 vision6D-0.0.9/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-27 00:14:56.000000 vision6D-0.0.9/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.0.8/LICENSE` & `vision6D-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.8/PKG-INFO` & `vision6D-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.0.8
+Version: 0.0.9
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.0.8/README.md` & `vision6D-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.8/setup.cfg` & `vision6D-0.0.9/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e38 0d0a 7572  sion = 0.0.8..ur
+00000020: 7369 6f6e 203d 2030 2e30 2e39 0d0a 7572  sion = 0.0.9..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
@@ -52,69 +52,70 @@
 00000330: 7079 0d0a 096d 6174 706c 6f74 6c69 620d  py...matplotlib.
 00000340: 0a09 7472 696d 6573 680d 0a09 6561 7379  ..trimesh...easy
 00000350: 6469 6374 0d0a 0970 696c 6c6f 770d 0a09  dict...pillow...
 00000360: 7363 6970 790d 0a09 7079 7465 7374 0d0a  scipy...pytest..
 00000370: 0970 7974 6573 742d 6c61 7a79 2d66 6978  .pytest-lazy-fix
 00000380: 7475 7265 0d0a 0970 7265 2d63 6f6d 6d69  ture...pre-commi
 00000390: 740d 0a09 6f70 656e 6376 2d70 7974 686f  t...opencv-pytho
-000003a0: 6e0d 0a09 7363 696b 6974 2d69 6d61 6765  n...scikit-image
-000003b0: 0d0a 0963 6861 7264 6574 0d0a 0970 7967  ...chardet...pyg
-000003c0: 656f 6465 7369 630d 0a09 5079 5174 350d  eodesic...PyQt5.
-000003d0: 0a09 7079 7669 7374 6171 740d 0a0d 0a5b  ..pyvistaqt....[
-000003e0: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
-000003f0: 6461 7461 5d0d 0a2a 203d 202a 2e70 6e67  data]..* = *.png
-00000400: 2c20 2a2e 6a70 672c 202a 2e71 6d6c 0d0a  , *.jpg, *.qml..
-00000410: 0d0a 5b62 6469 7374 5f77 6865 656c 5d0d  ..[bdist_wheel].
-00000420: 0a75 6e69 7665 7273 616c 203d 2074 7275  .universal = tru
-00000430: 650d 0a0d 0a5b 7364 6973 745d 0d0a 666f  e....[sdist]..fo
-00000440: 726d 6174 7320 3d20 7a69 702c 2067 7a74  rmats = zip, gzt
-00000450: 6172 0d0a 0d0a 5b63 6f76 6572 6167 653a  ar....[coverage:
-00000460: 7265 706f 7274 5d0d 0a73 686f 775f 6d69  report]..show_mi
-00000470: 7373 696e 6720 3d20 7472 7565 0d0a 6578  ssing = true..ex
-00000480: 636c 7564 655f 6c69 6e65 7320 3d20 0d0a  clude_lines = ..
-00000490: 0970 7261 676d 613a 206e 6f20 636f 7665  .pragma: no cove
-000004a0: 720d 0a09 6966 2046 616c 7365 0d0a 0d0a  r...if False....
-000004b0: 5b67 7265 656e 5d0d 0a66 696c 652d 7061  [green]..file-pa
-000004c0: 7474 6572 6e20 3d20 7465 7374 5f2a 2e70  ttern = test_*.p
-000004d0: 790d 0a76 6572 626f 7365 203d 2032 0d0a  y..verbose = 2..
-000004e0: 6e6f 2d73 6b69 702d 7265 706f 7274 203d  no-skip-report =
-000004f0: 2074 7275 650d 0a71 7569 6574 2d73 7464   true..quiet-std
-00000500: 6f75 7420 3d20 7472 7565 0d0a 7275 6e2d  out = true..run-
-00000510: 636f 7665 7261 6765 203d 2074 7275 650d  coverage = true.
-00000520: 0a0d 0a5b 7079 646f 6373 7479 6c65 5d0d  ...[pydocstyle].
-00000530: 0a6d 6174 6368 2d64 6972 203d 2028 3f21  .match-dir = (?!
-00000540: 7465 7374 7329 283f 2172 6573 6f75 7263  tests)(?!resourc
-00000550: 6573 2928 3f21 646f 6373 295b 5e5c 2e5d  es)(?!docs)[^\.]
-00000560: 2e2a 0d0a 6d61 7463 6820 3d20 283f 2174  .*..match = (?!t
-00000570: 6573 7429 283f 2173 6574 7570 295b 5e5c  est)(?!setup)[^\
-00000580: 2e5f 5d2e 2a5c 2e70 790d 0a69 6e68 6572  ._].*\.py..inher
-00000590: 6974 203d 2066 616c 7365 0d0a 6967 6e6f  it = false..igno
-000005a0: 7265 203d 2044 3230 302c 2044 3230 332c  re = D200, D203,
-000005b0: 2044 3231 332c 2044 3430 362c 2044 3430   D213, D406, D40
-000005c0: 370d 0a0d 0a5b 666c 616b 6538 5d0d 0a6d  7....[flake8]..m
-000005d0: 6178 2d6c 696e 652d 6c65 6e67 7468 203d  ax-line-length =
-000005e0: 2039 390d 0a64 6f63 7465 7374 7320 3d20   99..doctests = 
-000005f0: 5472 7565 0d0a 6578 636c 7564 6520 3d20  True..exclude = 
-00000600: 2e67 6974 2c20 2e65 6767 732c 205f 5f70  .git, .eggs, __p
-00000610: 7963 6163 6865 5f5f 2c20 7465 7374 732f  ycache__, tests/
-00000620: 2c20 646f 6373 2f2c 2062 7569 6c64 2f2c  , docs/, build/,
-00000630: 2064 6973 742f 0d0a 0d0a 5b6d 7970 795d   dist/....[mypy]
-00000640: 0d0a 6469 7361 6c6c 6f77 5f61 6e79 5f64  ..disallow_any_d
-00000650: 6563 6f72 6174 6564 203d 2074 7275 650d  ecorated = true.
-00000660: 0a64 6973 616c 6c6f 775f 616e 795f 6765  .disallow_any_ge
-00000670: 6e65 7269 6373 203d 2074 7275 650d 0a64  nerics = true..d
-00000680: 6973 616c 6c6f 775f 616e 795f 756e 696d  isallow_any_unim
-00000690: 706f 7274 6564 203d 2066 616c 7365 0d0a  ported = false..
-000006a0: 6469 7361 6c6c 6f77 5f73 7562 636c 6173  disallow_subclas
-000006b0: 7369 6e67 5f61 6e79 203d 2066 616c 7365  sing_any = false
-000006c0: 0d0a 6469 7361 6c6c 6f77 5f75 6e74 7970  ..disallow_untyp
-000006d0: 6564 5f63 616c 6c73 203d 2074 7275 650d  ed_calls = true.
-000006e0: 0a64 6973 616c 6c6f 775f 756e 7479 7065  .disallow_untype
-000006f0: 645f 6465 6673 203d 2074 7275 650d 0a69  d_defs = true..i
-00000700: 676e 6f72 655f 6d69 7373 696e 675f 696d  gnore_missing_im
-00000710: 706f 7274 7320 3d20 7472 7565 0d0a 7761  ports = true..wa
-00000720: 726e 5f75 6e75 7365 645f 6967 6e6f 7265  rn_unused_ignore
-00000730: 7320 3d20 7472 7565 0d0a 7761 726e 5f72  s = true..warn_r
-00000740: 6574 7572 6e5f 616e 7920 3d20 7472 7565  eturn_any = true
-00000750: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-00000760: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000770: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+000003a0: 6e2d 6865 6164 6c65 7373 0d0a 0973 6369  n-headless...sci
+000003b0: 6b69 742d 696d 6167 650d 0a09 6368 6172  kit-image...char
+000003c0: 6465 740d 0a09 7079 6765 6f64 6573 6963  det...pygeodesic
+000003d0: 0d0a 0950 7951 7435 0d0a 0970 7976 6973  ...PyQt5...pyvis
+000003e0: 7461 7174 0d0a 0d0a 5b6f 7074 696f 6e73  taqt....[options
+000003f0: 2e70 6163 6b61 6765 5f64 6174 615d 0d0a  .package_data]..
+00000400: 2a20 3d20 2a2e 706e 672c 202a 2e6a 7067  * = *.png, *.jpg
+00000410: 2c20 2a2e 716d 6c0d 0a0d 0a5b 6264 6973  , *.qml....[bdis
+00000420: 745f 7768 6565 6c5d 0d0a 756e 6976 6572  t_wheel]..univer
+00000430: 7361 6c20 3d20 7472 7565 0d0a 0d0a 5b73  sal = true....[s
+00000440: 6469 7374 5d0d 0a66 6f72 6d61 7473 203d  dist]..formats =
+00000450: 207a 6970 2c20 677a 7461 720d 0a0d 0a5b   zip, gztar....[
+00000460: 636f 7665 7261 6765 3a72 6570 6f72 745d  coverage:report]
+00000470: 0d0a 7368 6f77 5f6d 6973 7369 6e67 203d  ..show_missing =
+00000480: 2074 7275 650d 0a65 7863 6c75 6465 5f6c   true..exclude_l
+00000490: 696e 6573 203d 200d 0a09 7072 6167 6d61  ines = ...pragma
+000004a0: 3a20 6e6f 2063 6f76 6572 0d0a 0969 6620  : no cover...if 
+000004b0: 4661 6c73 650d 0a0d 0a5b 6772 6565 6e5d  False....[green]
+000004c0: 0d0a 6669 6c65 2d70 6174 7465 726e 203d  ..file-pattern =
+000004d0: 2074 6573 745f 2a2e 7079 0d0a 7665 7262   test_*.py..verb
+000004e0: 6f73 6520 3d20 320d 0a6e 6f2d 736b 6970  ose = 2..no-skip
+000004f0: 2d72 6570 6f72 7420 3d20 7472 7565 0d0a  -report = true..
+00000500: 7175 6965 742d 7374 646f 7574 203d 2074  quiet-stdout = t
+00000510: 7275 650d 0a72 756e 2d63 6f76 6572 6167  rue..run-coverag
+00000520: 6520 3d20 7472 7565 0d0a 0d0a 5b70 7964  e = true....[pyd
+00000530: 6f63 7374 796c 655d 0d0a 6d61 7463 682d  ocstyle]..match-
+00000540: 6469 7220 3d20 283f 2174 6573 7473 2928  dir = (?!tests)(
+00000550: 3f21 7265 736f 7572 6365 7329 283f 2164  ?!resources)(?!d
+00000560: 6f63 7329 5b5e 5c2e 5d2e 2a0d 0a6d 6174  ocs)[^\.].*..mat
+00000570: 6368 203d 2028 3f21 7465 7374 2928 3f21  ch = (?!test)(?!
+00000580: 7365 7475 7029 5b5e 5c2e 5f5d 2e2a 5c2e  setup)[^\._].*\.
+00000590: 7079 0d0a 696e 6865 7269 7420 3d20 6661  py..inherit = fa
+000005a0: 6c73 650d 0a69 676e 6f72 6520 3d20 4432  lse..ignore = D2
+000005b0: 3030 2c20 4432 3033 2c20 4432 3133 2c20  00, D203, D213, 
+000005c0: 4434 3036 2c20 4434 3037 0d0a 0d0a 5b66  D406, D407....[f
+000005d0: 6c61 6b65 385d 0d0a 6d61 782d 6c69 6e65  lake8]..max-line
+000005e0: 2d6c 656e 6774 6820 3d20 3939 0d0a 646f  -length = 99..do
+000005f0: 6374 6573 7473 203d 2054 7275 650d 0a65  ctests = True..e
+00000600: 7863 6c75 6465 203d 202e 6769 742c 202e  xclude = .git, .
+00000610: 6567 6773 2c20 5f5f 7079 6361 6368 655f  eggs, __pycache_
+00000620: 5f2c 2074 6573 7473 2f2c 2064 6f63 732f  _, tests/, docs/
+00000630: 2c20 6275 696c 642f 2c20 6469 7374 2f0d  , build/, dist/.
+00000640: 0a0d 0a5b 6d79 7079 5d0d 0a64 6973 616c  ...[mypy]..disal
+00000650: 6c6f 775f 616e 795f 6465 636f 7261 7465  low_any_decorate
+00000660: 6420 3d20 7472 7565 0d0a 6469 7361 6c6c  d = true..disall
+00000670: 6f77 5f61 6e79 5f67 656e 6572 6963 7320  ow_any_generics 
+00000680: 3d20 7472 7565 0d0a 6469 7361 6c6c 6f77  = true..disallow
+00000690: 5f61 6e79 5f75 6e69 6d70 6f72 7465 6420  _any_unimported 
+000006a0: 3d20 6661 6c73 650d 0a64 6973 616c 6c6f  = false..disallo
+000006b0: 775f 7375 6263 6c61 7373 696e 675f 616e  w_subclassing_an
+000006c0: 7920 3d20 6661 6c73 650d 0a64 6973 616c  y = false..disal
+000006d0: 6c6f 775f 756e 7479 7065 645f 6361 6c6c  low_untyped_call
+000006e0: 7320 3d20 7472 7565 0d0a 6469 7361 6c6c  s = true..disall
+000006f0: 6f77 5f75 6e74 7970 6564 5f64 6566 7320  ow_untyped_defs 
+00000700: 3d20 7472 7565 0d0a 6967 6e6f 7265 5f6d  = true..ignore_m
+00000710: 6973 7369 6e67 5f69 6d70 6f72 7473 203d  issing_imports =
+00000720: 2074 7275 650d 0a77 6172 6e5f 756e 7573   true..warn_unus
+00000730: 6564 5f69 676e 6f72 6573 203d 2074 7275  ed_ignores = tru
+00000740: 650d 0a77 6172 6e5f 7265 7475 726e 5f61  e..warn_return_a
+00000750: 6e79 203d 2074 7275 650d 0a0d 0a5b 6567  ny = true....[eg
+00000760: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000770: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000780: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `vision6D-0.0.8/test/test_create_dataset.py` & `vision6D-0.0.9/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.8/test/test_projection.py` & `vision6D-0.0.9/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.8/vision6D/GUI.py` & `vision6D-0.0.9/vision6D/GUI.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.8/vision6D/__init__.py` & `vision6D-0.0.9/vision6D/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.8/vision6D/app.py` & `vision6D-0.0.9/vision6D/app.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.8/vision6D/config.py` & `vision6D-0.0.9/vision6D/config.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.8/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.0.9/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.8/vision6D/data/ossiclesCoordinateMappingv1.json` & `vision6D-0.0.9/vision6D/data/ossiclesCoordinateMappingv1.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.8/vision6D/data/style.qss` & `vision6D-0.0.9/vision6D/data/style.qss`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.8/vision6D/interface.py` & `vision6D-0.0.9/vision6D/interface.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.8/vision6D/interface_gui.py` & `vision6D-0.0.9/vision6D/interface_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.8/vision6D/mainwindow.py` & `vision6D-0.0.9/vision6D/mainwindow.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.8/vision6D/run_gui.py` & `vision6D-0.0.9/vision6D/run_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.8/vision6D/utils.py` & `vision6D-0.0.9/vision6D/utils.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.8/vision6D.egg-info/PKG-INFO` & `vision6D-0.0.9/vision6D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.0.8
+Version: 0.0.9
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.0.8/vision6D.egg-info/SOURCES.txt` & `vision6D-0.0.9/vision6D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

