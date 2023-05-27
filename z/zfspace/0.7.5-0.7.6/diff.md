# Comparing `tmp/zfspace-0.7.5-py3-none-any.whl.zip` & `tmp/zfspace-0.7.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 13360 bytes, number of entries: 8
+Zip file size: 13358 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      149 b- defN 20-Feb-02 00:00 zfspace/__init__.py
 -rwxr-xr-x  2.0 unx       57 b- defN 20-Feb-02 00:00 zfspace/__main__.py
 -rwxr-xr-x  2.0 unx    23089 b- defN 20-Feb-02 00:00 zfspace/zfspace.py
-?rw-r--r--  2.0 unx     3238 b- defN 20-Feb-02 00:00 zfspace-0.7.5.dist-info/METADATA
-?rw-r--r--  2.0 unx       83 b- defN 20-Feb-02 00:00 zfspace-0.7.5.dist-info/WHEEL
-?rw-r--r--  2.0 unx       41 b- defN 20-Feb-02 00:00 zfspace-0.7.5.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     7048 b- defN 20-Feb-02 00:00 zfspace-0.7.5.dist-info/license_files/LICENSE
-?rw-r--r--  2.0 unx      628 b- defN 20-Feb-02 00:00 zfspace-0.7.5.dist-info/RECORD
-8 files, 34333 bytes uncompressed, 12266 bytes compressed:  64.3%
+?rw-r--r--  2.0 unx     3238 b- defN 20-Feb-02 00:00 zfspace-0.7.6.dist-info/METADATA
+?rw-r--r--  2.0 unx       83 b- defN 20-Feb-02 00:00 zfspace-0.7.6.dist-info/WHEEL
+?rw-r--r--  2.0 unx       41 b- defN 20-Feb-02 00:00 zfspace-0.7.6.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     7048 b- defN 20-Feb-02 00:00 zfspace-0.7.6.dist-info/license_files/LICENSE
+?rw-r--r--  2.0 unx      628 b- defN 20-Feb-02 00:00 zfspace-0.7.6.dist-info/RECORD
+8 files, 34333 bytes uncompressed, 12264 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: zfspace/__main__.py
 Comment: 
 
 Filename: zfspace/zfspace.py
 Comment: 
 
-Filename: zfspace-0.7.5.dist-info/METADATA
+Filename: zfspace-0.7.6.dist-info/METADATA
 Comment: 
 
-Filename: zfspace-0.7.5.dist-info/WHEEL
+Filename: zfspace-0.7.6.dist-info/WHEEL
 Comment: 
 
-Filename: zfspace-0.7.5.dist-info/entry_points.txt
+Filename: zfspace-0.7.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: zfspace-0.7.5.dist-info/license_files/LICENSE
+Filename: zfspace-0.7.6.dist-info/license_files/LICENSE
 Comment: 
 
-Filename: zfspace-0.7.5.dist-info/RECORD
+Filename: zfspace-0.7.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zfspace/__init__.py

```diff
@@ -1,4 +1,4 @@
 from .zfspace import main  # noqa
 
 # Version is updated with bump2version helper. Do not update manually or you will lose sync
-__version__ = '0.7.5'
+__version__ = '0.7.6'
```

## zfspace/zfspace.py

```diff
@@ -13,15 +13,15 @@
 import os
 import math
 import difflib
 import argparse
 import copy
 
 # Version is updated with bump2version helper. Do not update manually or you will lose sync
-__version__ = '0.7.5'
+__version__ = '0.7.6'
 filter_level = 0.368  # This value will be overwritten by default argparse filter value
 
 term_format = dict(PURPLE='\033[95m', CYAN='\033[96m', DARKCYAN='\033[36m', BLUE='\033[94m',
                    GREEN='\033[92m', YELLOW='\033[93m', RED='\033[91m', BOLD='\033[1m',
                    UNDERLINE='\033[4m', WHITEBOLD='\033[1;37m', END='\033[0m')
```

## Comparing `zfspace-0.7.5.dist-info/METADATA` & `zfspace-0.7.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zfspace
-Version: 0.7.5
+Version: 0.7.6
 Summary: zfspace tool helps to analyze how zfs disk space is used
 Project-URL: Bug Tracker, https://github.com/Zapunidi/zfspace/issues
 Project-URL: Homepage, https://github.com/Zapunidi/zfspace
 Author-email: Sergey Zapunidi <zapunidy@gmail.com>
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
```

## Comparing `zfspace-0.7.5.dist-info/license_files/LICENSE` & `zfspace-0.7.6.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

