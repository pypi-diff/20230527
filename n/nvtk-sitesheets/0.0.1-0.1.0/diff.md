# Comparing `tmp/nvtk-sitesheets-0.0.1.tar.gz` & `tmp/nvtk-sitesheets-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvtk-sitesheets-0.0.1.tar", last modified: Thu Nov  3 11:25:22 2022, max compression
+gzip compressed data, was "nvtk-sitesheets-0.1.0.tar", last modified: Sat May 27 07:14:38 2023, max compression
```

## Comparing `nvtk-sitesheets-0.0.1.tar` & `nvtk-sitesheets-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       92 2022-04-01 06:53:53.903195 nvtk-sitesheets-0.0.1/README.md
--rw-r--r--   0        0        0        0 2022-11-03 11:20:35.076434 nvtk-sitesheets-0.0.1/nvtk_ssm/__init__.py
--rwxr-xr-x   0        0        0      912 2022-10-17 11:34:40.713742 nvtk-sitesheets-0.0.1/nvtk_ssm/doubleA5.py
--rwxr-xr-x   0        0        0     2857 2022-11-03 11:24:44.382907 nvtk-sitesheets-0.0.1/nvtk_ssm/ssm.py
--rw-r--r--   0        0        0      932 2022-11-03 11:22:28.851524 nvtk-sitesheets-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       61 2022-04-01 07:49:29.293419 nvtk-sitesheets-0.0.1/requirements.txt
--rw-r--r--   0        0        0    10997 2022-10-17 11:41:20.645654 nvtk-sitesheets-0.0.1/templates/ctx-site-sheet.ods
--rw-r--r--   0        0        0    24539 2022-10-17 11:30:26.719465 nvtk-sitesheets-0.0.1/templates/ctx-site-sheet.svg
--rw-r--r--   0        0        0    20815 2022-04-01 07:50:31.411684 nvtk-sitesheets-0.0.1/templates/khs-site-sheet.svg
--rw-r--r--   0        0        0    73681 2022-11-03 11:02:38.070012 nvtk-sitesheets-0.0.1/templates/pathocom-scoring-sheet-v5.svg
--rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 nvtk-sitesheets-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1631 2023-05-26 21:02:01.915212 nvtk-sitesheets-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2022-11-03 11:20:35.076434 nvtk-sitesheets-0.1.0/nvtk_ssm/__init__.py
+-rwxr-xr-x   0        0        0      912 2022-10-17 11:34:40.713742 nvtk-sitesheets-0.1.0/nvtk_ssm/doubleA5.py
+-rwxr-xr-x   0        0        0     2864 2023-05-26 20:41:01.414880 nvtk-sitesheets-0.1.0/nvtk_ssm/ssm.py
+-rw-r--r--   0        0        0     5427 2023-05-26 20:43:56.817185 nvtk-sitesheets-0.1.0/nvtk_ssm/svglue.py
+-rw-r--r--   0        0        0      964 2023-05-27 07:09:25.151448 nvtk-sitesheets-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    24539 2022-10-17 11:30:26.719465 nvtk-sitesheets-0.1.0/templates/ctx-site-sheet.svg
+-rw-r--r--   0        0        0    51561 2023-05-26 20:33:03.604261 nvtk-sitesheets-0.1.0/templates/ctx_v2.svg
+-rw-r--r--   0        0        0    20815 2022-04-01 07:50:31.411684 nvtk-sitesheets-0.1.0/templates/khs-site-sheet.svg
+-rw-r--r--   0        0        0    73681 2022-11-03 11:02:38.070012 nvtk-sitesheets-0.1.0/templates/pathocom-scoring-sheet-v5.svg
+-rw-r--r--   0        0        0    43830 2023-05-26 21:00:18.741856 nvtk-sitesheets-0.1.0/templates/test.jpg
+-rw-r--r--   0        0        0     2405 1970-01-01 00:00:00.000000 nvtk-sitesheets-0.1.0/PKG-INFO
```

### Comparing `nvtk-sitesheets-0.0.1/nvtk_ssm/doubleA5.py` & `nvtk-sitesheets-0.1.0/nvtk_ssm/doubleA5.py`

 * *Files identical despite different names*

### Comparing `nvtk-sitesheets-0.0.1/nvtk_ssm/ssm.py` & `nvtk-sitesheets-0.1.0/nvtk_ssm/ssm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-import svglue
+from . import svglue
 import cairosvg
 import qrcode
 from PyPDF2 import PdfFileMerger
 from tqdm import tqdm
 
 import argparse
 import sys
```

### Comparing `nvtk-sitesheets-0.0.1/pyproject.toml` & `nvtk-sitesheets-0.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [project]
-version = "0.0.1"
+version = "0.1.0"
 name = "nvtk-sitesheets"
 description = "Tool to create templated metadata sheets for fieldwork experiments"
 keywords=["qrcode", "fieldwork",]
 dependencies = [
-    "svglue",
+    #"svglue", # Now vendored
+    "cairosvg",
     "qrcode",
     "PyPDF2",
     "pillow",
     "qrcode",
     "tqdm",
 ]
 readme = "README.md"
```

### Comparing `nvtk-sitesheets-0.0.1/templates/ctx-site-sheet.svg` & `nvtk-sitesheets-0.1.0/templates/ctx-site-sheet.svg`

 * *Files identical despite different names*

### Comparing `nvtk-sitesheets-0.0.1/templates/khs-site-sheet.svg` & `nvtk-sitesheets-0.1.0/templates/khs-site-sheet.svg`

 * *Files identical despite different names*

### Comparing `nvtk-sitesheets-0.0.1/templates/pathocom-scoring-sheet-v5.svg` & `nvtk-sitesheets-0.1.0/templates/pathocom-scoring-sheet-v5.svg`

 * *Files identical despite different names*

