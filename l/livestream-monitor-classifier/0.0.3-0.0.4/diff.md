# Comparing `tmp/livestream_monitor_classifier-0.0.3.tar.gz` & `tmp/livestream_monitor_classifier-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livestream_monitor_classifier-0.0.3.tar", last modified: Fri May 26 20:57:25 2023, max compression
+gzip compressed data, was "livestream_monitor_classifier-0.0.4.tar", last modified: Sat May 27 13:16:26 2023, max compression
```

## Comparing `livestream_monitor_classifier-0.0.3.tar` & `livestream_monitor_classifier-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:57:25.656480 livestream_monitor_classifier-0.0.3/
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     1061 2023-05-26 19:34:03.000000 livestream_monitor_classifier-0.0.3/LICENSE.txt
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      124 2023-05-26 20:15:08.000000 livestream_monitor_classifier-0.0.3/MANIFEST.in
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      864 2023-05-26 20:57:25.656566 livestream_monitor_classifier-0.0.3/PKG-INFO
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)       99 2023-05-24 20:43:52.000000 livestream_monitor_classifier-0.0.3/README.md
-drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:57:25.649282 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)       28 2023-05-26 19:18:27.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/__init__.py
-drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:57:25.651108 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/__pycache__/
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      272 2023-05-26 20:22:47.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     1400 2023-05-26 20:23:44.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/__pycache__/main.cpython-310.pyc
-drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:57:25.651631 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/data/
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     6460 2023-05-26 19:13:41.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/data/stopwords-custom.txt
-drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:57:25.652191 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/helper/
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 19:18:18.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/helper/__init__.py
-drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:57:25.654353 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/helper/__pycache__/
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      240 2023-05-26 20:22:47.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/helper/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     2025 2023-05-26 20:22:47.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/helper/__pycache__/preprocess.cpython-310.pyc
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     1493 2023-05-26 19:16:55.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/helper/preprocess.py
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      896 2023-05-26 20:23:43.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/main.py
-drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:57:25.654715 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/model/
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)   356572 2023-05-26 19:30:26.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/model/sklearn_MNB.model
-drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:57:25.650502 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier.egg-info/
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      864 2023-05-26 20:57:25.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier.egg-info/PKG-INFO
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      886 2023-05-26 20:57:25.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier.egg-info/SOURCES.txt
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)        1 2023-05-26 20:57:25.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier.egg-info/dependency_links.txt
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)       46 2023-05-26 20:57:25.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier.egg-info/requires.txt
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)       30 2023-05-26 20:57:25.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier.egg-info/top_level.txt
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      173 2023-05-26 20:57:25.657003 livestream_monitor_classifier-0.0.3/setup.cfg
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     1812 2023-05-26 20:56:46.000000 livestream_monitor_classifier-0.0.3/setup.py
+drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-27 13:16:26.682347 livestream_monitor_classifier-0.0.4/
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     1061 2023-05-26 19:34:03.000000 livestream_monitor_classifier-0.0.4/LICENSE.txt
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      124 2023-05-26 20:15:08.000000 livestream_monitor_classifier-0.0.4/MANIFEST.in
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      864 2023-05-27 13:16:26.682438 livestream_monitor_classifier-0.0.4/PKG-INFO
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)       99 2023-05-24 20:43:52.000000 livestream_monitor_classifier-0.0.4/README.md
+drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-27 13:16:26.675967 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)       28 2023-05-26 19:18:27.000000 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/__init__.py
+drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-27 13:16:26.677701 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/__pycache__/
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      272 2023-05-26 20:22:47.000000 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     1401 2023-05-27 13:03:12.000000 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/__pycache__/main.cpython-310.pyc
+drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-27 13:16:26.678238 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/data/
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     6460 2023-05-26 19:13:41.000000 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/data/stopwords-custom.txt
+drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-27 13:16:26.678799 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/helper/
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 19:18:18.000000 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/helper/__init__.py
+drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-27 13:16:26.679706 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/helper/__pycache__/
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      240 2023-05-26 20:22:47.000000 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/helper/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     2025 2023-05-26 20:22:47.000000 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/helper/__pycache__/preprocess.cpython-310.pyc
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     1493 2023-05-26 19:16:55.000000 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/helper/preprocess.py
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      907 2023-05-27 12:58:38.000000 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/main.py
+drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-27 13:16:26.680049 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/model/
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)   356572 2023-05-26 19:30:26.000000 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/model/sklearn_MNB.model
+drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-27 13:16:26.677132 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier.egg-info/
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      864 2023-05-27 13:16:26.000000 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier.egg-info/PKG-INFO
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      886 2023-05-27 13:16:26.000000 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier.egg-info/SOURCES.txt
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)        1 2023-05-27 13:16:26.000000 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier.egg-info/dependency_links.txt
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)       46 2023-05-27 13:16:26.000000 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier.egg-info/requires.txt
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)       30 2023-05-27 13:16:26.000000 livestream_monitor_classifier-0.0.4/livestream_monitor_classifier.egg-info/top_level.txt
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      173 2023-05-27 13:16:26.682833 livestream_monitor_classifier-0.0.4/setup.cfg
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     1812 2023-05-27 13:00:16.000000 livestream_monitor_classifier-0.0.4/setup.py
```

### Comparing `livestream_monitor_classifier-0.0.3/LICENSE.txt` & `livestream_monitor_classifier-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `livestream_monitor_classifier-0.0.3/PKG-INFO` & `livestream_monitor_classifier-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: livestream_monitor_classifier
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Machine Learning Classifier that used to for my personal thesis project called livestream monitor
 Home-page: https://github.com/rfirmansyh/livestream_monitor_classifier
-Download-URL: https://github.com/rfirmansyh/livestream_monitor_classifier/archive/refs/tags/v0.0.3.tar.gz
+Download-URL: https://github.com/rfirmansyh/livestream_monitor_classifier/archive/refs/tags/v0.0.4.tar.gz
 Author: Rahmad Firmansyah
 Author-email: rahmadfirmansyah.id@gmail.com
 License: MIT
 Keywords: rfirmansyh,livestream_monitor_classifier
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/__pycache__/main.cpython-310.pyc` & `livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/__pycache__/main.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 26 20:23:43 2023 UTC, .py size: 896 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4f15 7164 8003 0000  o.......O.qd....
+00000000: 6f0d 0d0a 0000 0000 7efe 7164 8b03 0000  o.......~.qd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6506 6507 8301  d.l.m.Z...e.e...
 00000060: 6a08 6405 1b00 5a09 4700 6406 6407 8400  j.d...Z.G.d.d...
 00000070: 6407 8302 5a0a 6401 5300 2908 e900 0000  d...Z.d.S.).....
@@ -39,50 +39,50 @@
 00000260: 0c01 0a01 0e01 7a13 436c 6173 7369 6669  ......z.Classifi
 00000270: 6572 2e5f 5f69 6e69 745f 5fda 0569 6e70  er.__init__..inp
 00000280: 7574 6302 0000 0000 0000 0000 0000 0005  utc.............
 00000290: 0000 0003 0000 0043 0000 0073 2a00 0000  .......C...s*...
 000002a0: 7c00 a000 7c01 a101 7d02 7c00 6a01 6a02  |...|...}.|.j.j.
 000002b0: a003 7c02 6701 a101 7d03 7c00 6a01 a004  ..|.g...}.|.j...
 000002c0: 7c03 a101 7d04 7c04 5300 7206 0000 0029  |...}.|.S.r....)
-000002d0: 0572 0c00 0000 720a 0000 005a 0d74 665f  .r....r....Z.tf_
+000002d0: 0572 0c00 0000 720a 0000 00da 0d74 665f  .r....r......tf_
 000002e0: 7665 6374 6f72 697a 6572 da09 7472 616e  vectorizer..tran
 000002f0: 7366 6f72 6dda 0770 7265 6469 6374 2905  sform..predict).
 00000300: 720e 0000 0072 1200 0000 5a16 7072 6564  r....r....Z.pred
 00000310: 6963 7465 645f 7072 6570 726f 6365 7373  icted_preprocess
 00000320: 6564 da0c 7072 6564 6963 7465 645f 7466  ed..predicted_tf
 00000330: da10 7072 6564 6963 7465 645f 7265 7375  ..predicted_resu
 00000340: 6c74 720f 0000 0072 0f00 0000 7210 0000  ltr....r....r...
-00000350: 0072 1400 0000 0f00 0000 7308 0000 000a  .r........s.....
+00000350: 0072 1500 0000 0f00 0000 7308 0000 000a  .r........s.....
 00000360: 0110 010c 0104 017a 1243 6c61 7373 6966  .......z.Classif
 00000370: 6965 722e 7072 6564 6963 74da 0669 6e70  ier.predict..inp
 00000380: 7574 7363 0200 0000 0000 0000 0000 0000  utsc............
 00000390: 0500 0000 0300 0000 4300 0000 7328 0000  ........C...s(..
 000003a0: 007c 00a0 007c 01a1 017d 027c 006a 016a  .|...|...}.|.j.j
 000003b0: 02a0 037c 02a1 017d 037c 006a 01a0 047c  ...|...}.|.j...|
 000003c0: 03a1 017d 047c 0453 0072 0600 0000 2905  ...}.|.S.r....).
-000003d0: 720d 0000 0072 0a00 0000 5a02 7466 7213  r....r....Z.tfr.
-000003e0: 0000 0072 1400 0000 2905 720e 0000 0072  ...r....).r....r
-000003f0: 1700 0000 5a1b 7072 6564 6963 7465 645f  ....Z.predicted_
-00000400: 7072 6570 726f 6365 7373 6564 5f6c 6973  preprocessed_lis
-00000410: 7472 1500 0000 7216 0000 0072 0f00 0000  tr....r....r....
-00000420: 720f 0000 0072 1000 0000 da0c 7072 6564  r....r......pred
-00000430: 6963 745f 6c69 7374 1500 0000 7308 0000  ict_list....s...
-00000440: 000a 010e 010c 0104 017a 1743 6c61 7373  .........z.Class
-00000450: 6966 6965 722e 7072 6564 6963 745f 6c69  ifier.predict_li
-00000460: 7374 4e29 08da 085f 5f6e 616d 655f 5fda  stN)...__name__.
-00000470: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000480: 7561 6c6e 616d 655f 5f72 1100 0000 da03  ualname__r......
-00000490: 7374 7272 1400 0000 7202 0000 0072 1800  strr....r....r..
-000004a0: 0000 720f 0000 0072 0f00 0000 720f 0000  ..r....r....r...
-000004b0: 0072 1000 0000 7205 0000 0009 0000 0073  .r....r........s
-000004c0: 0800 0000 0800 0801 0e05 1606 7205 0000  ............r...
-000004d0: 0029 0b72 0700 0000 da06 7479 7069 6e67  .).r......typing
-000004e0: 7202 0000 005a 2f6c 6976 6573 7472 6561  r....Z/livestrea
-000004f0: 6d5f 6d6f 6e69 746f 725f 636c 6173 7369  m_monitor_classi
-00000500: 6669 6572 2e68 656c 7065 722e 7072 6570  fier.helper.prep
-00000510: 726f 6365 7373 7203 0000 005a 0770 6174  rocessr....Z.pat
-00000520: 686c 6962 7204 0000 00da 085f 5f66 696c  hlibr......__fil
-00000530: 655f 5fda 0670 6172 656e 7472 0900 0000  e__..parentr....
-00000540: 7205 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00000550: 0f00 0000 7210 0000 00da 083c 6d6f 6475  ....r......<modu
-00000560: 6c65 3e01 0000 0073 0c00 0000 0800 0c01  le>....s........
-00000570: 0c01 0c01 0e02 1203                      ........
+000003d0: 720d 0000 0072 0a00 0000 7213 0000 0072  r....r....r....r
+000003e0: 1400 0000 7215 0000 0029 0572 0e00 0000  ....r....).r....
+000003f0: 7218 0000 005a 1b70 7265 6469 6374 6564  r....Z.predicted
+00000400: 5f70 7265 7072 6f63 6573 7365 645f 6c69  _preprocessed_li
+00000410: 7374 7216 0000 0072 1700 0000 720f 0000  str....r....r...
+00000420: 0072 0f00 0000 7210 0000 00da 0c70 7265  .r....r......pre
+00000430: 6469 6374 5f6c 6973 7415 0000 0073 0800  dict_list....s..
+00000440: 0000 0a01 0e01 0c01 0401 7a17 436c 6173  ..........z.Clas
+00000450: 7369 6669 6572 2e70 7265 6469 6374 5f6c  sifier.predict_l
+00000460: 6973 744e 2908 da08 5f5f 6e61 6d65 5f5f  istN)...__name__
+00000470: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000480: 7175 616c 6e61 6d65 5f5f 7211 0000 00da  qualname__r.....
+00000490: 0373 7472 7215 0000 0072 0200 0000 7219  .strr....r....r.
+000004a0: 0000 0072 0f00 0000 720f 0000 0072 0f00  ...r....r....r..
+000004b0: 0000 7210 0000 0072 0500 0000 0900 0000  ..r....r........
+000004c0: 7308 0000 0008 0008 010e 0516 0672 0500  s............r..
+000004d0: 0000 290b 7207 0000 00da 0674 7970 696e  ..).r......typin
+000004e0: 6772 0200 0000 5a2f 6c69 7665 7374 7265  gr....Z/livestre
+000004f0: 616d 5f6d 6f6e 6974 6f72 5f63 6c61 7373  am_monitor_class
+00000500: 6966 6965 722e 6865 6c70 6572 2e70 7265  ifier.helper.pre
+00000510: 7072 6f63 6573 7372 0300 0000 5a07 7061  processr....Z.pa
+00000520: 7468 6c69 6272 0400 0000 da08 5f5f 6669  thlibr......__fi
+00000530: 6c65 5f5f da06 7061 7265 6e74 7209 0000  le__..parentr...
+00000540: 0072 0500 0000 720f 0000 0072 0f00 0000  .r....r....r....
+00000550: 720f 0000 0072 1000 0000 da08 3c6d 6f64  r....r......<mod
+00000560: 756c 653e 0100 0000 730c 0000 0008 000c  ule>....s.......
+00000570: 010c 010c 010e 0212 03                   .........
```

### Comparing `livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/data/stopwords-custom.txt` & `livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/data/stopwords-custom.txt`

 * *Files identical despite different names*

### Comparing `livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/helper/__pycache__/preprocess.cpython-310.pyc` & `livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/helper/__pycache__/preprocess.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/helper/preprocess.py` & `livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/helper/preprocess.py`

 * *Files identical despite different names*

### Comparing `livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/main.py` & `livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,11 +16,11 @@
     predicted_preprocessed = self.preprocess_get(input)
     predicted_tf = self.model.tf_vectorizer.transform([predicted_preprocessed])
     predicted_result = self.model.predict(predicted_tf)
     return predicted_result
     
   def predict_list(self, inputs: List[str]):
     predicted_preprocessed_list = self.preprocess_get_list(inputs)
-    predicted_tf = self.model.tf.transform(predicted_preprocessed_list)
+    predicted_tf = self.model.tf_vectorizer.transform(predicted_preprocessed_list)
     predicted_result = self.model.predict(predicted_tf)
     return predicted_result
```

### Comparing `livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/model/sklearn_MNB.model` & `livestream_monitor_classifier-0.0.4/livestream_monitor_classifier/model/sklearn_MNB.model`

 * *Files identical despite different names*

### Comparing `livestream_monitor_classifier-0.0.3/livestream_monitor_classifier.egg-info/PKG-INFO` & `livestream_monitor_classifier-0.0.4/livestream_monitor_classifier.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: livestream-monitor-classifier
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Machine Learning Classifier that used to for my personal thesis project called livestream monitor
 Home-page: https://github.com/rfirmansyh/livestream_monitor_classifier
-Download-URL: https://github.com/rfirmansyh/livestream_monitor_classifier/archive/refs/tags/v0.0.3.tar.gz
+Download-URL: https://github.com/rfirmansyh/livestream_monitor_classifier/archive/refs/tags/v0.0.4.tar.gz
 Author: Rahmad Firmansyah
 Author-email: rahmadfirmansyah.id@gmail.com
 License: MIT
 Keywords: rfirmansyh,livestream_monitor_classifier
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `livestream_monitor_classifier-0.0.3/livestream_monitor_classifier.egg-info/SOURCES.txt` & `livestream_monitor_classifier-0.0.4/livestream_monitor_classifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `livestream_monitor_classifier-0.0.3/setup.py` & `livestream_monitor_classifier-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from distutils.core import setup
 
 
 setup(
     name='livestream_monitor_classifier',
     packages=['livestream_monitor_classifier'],
-    version='0.0.3',
+    version='0.0.4',
     license='MIT',
     description='A Machine Learning Classifier that used to for my personal thesis project called livestream monitor',   # Give a short description about your library
     author='Rahmad Firmansyah',                   # Type in your name
     author_email='rahmadfirmansyah.id@gmail.com',      # Type in your E-Mail
     url='https://github.com/rfirmansyh/livestream_monitor_classifier',   # Provide either the link to your github or to your website
-    download_url='https://github.com/rfirmansyh/livestream_monitor_classifier/archive/refs/tags/v0.0.3.tar.gz',    # I explain this later on
+    download_url='https://github.com/rfirmansyh/livestream_monitor_classifier/archive/refs/tags/v0.0.4.tar.gz',    # I explain this later on
     keywords=['rfirmansyh', 'livestream_monitor_classifier'],   # Keywords that define your package best
     install_requires=[            # I get to this in a second
         'scikit-learn',
         'pandas',
         'joblib',
         'sastrawi',
         'unidecode',
```

