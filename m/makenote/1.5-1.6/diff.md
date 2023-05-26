# Comparing `tmp/makenote-1.5-py3-none-any.whl.zip` & `tmp/makenote-1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 17704 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       20 b- defN 23-May-26 22:40 makenote/__init__.py
--rwxrwxr-x  2.0 unx    10744 b- defN 23-May-26 22:40 makenote-1.5.data/scripts/makenote
--rw-rw-r--  2.0 unx    35099 b- defN 23-May-26 22:40 makenote-1.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3022 b- defN 23-May-26 22:40 makenote-1.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-26 22:40 makenote-1.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-May-26 22:40 makenote-1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      548 b- defN 23-May-26 22:40 makenote-1.5.dist-info/RECORD
-7 files, 49534 bytes uncompressed, 16734 bytes compressed:  66.2%
+Zip file size: 17695 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx       20 b- defN 23-May-26 22:48 makenote/__init__.py
+-rwxrwxr-x  2.0 unx    10718 b- defN 23-May-26 22:48 makenote-1.6.data/scripts/makenote
+-rw-rw-r--  2.0 unx    35099 b- defN 23-May-26 22:48 makenote-1.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3022 b- defN 23-May-26 22:48 makenote-1.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-26 22:48 makenote-1.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-26 22:48 makenote-1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      548 b- defN 23-May-26 22:48 makenote-1.6.dist-info/RECORD
+7 files, 49508 bytes uncompressed, 16725 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: makenote/__init__.py
 Comment: 
 
-Filename: makenote-1.5.data/scripts/makenote
+Filename: makenote-1.6.data/scripts/makenote
 Comment: 
 
-Filename: makenote-1.5.dist-info/LICENSE
+Filename: makenote-1.6.dist-info/LICENSE
 Comment: 
 
-Filename: makenote-1.5.dist-info/METADATA
+Filename: makenote-1.6.dist-info/METADATA
 Comment: 
 
-Filename: makenote-1.5.dist-info/WHEEL
+Filename: makenote-1.6.dist-info/WHEEL
 Comment: 
 
-Filename: makenote-1.5.dist-info/top_level.txt
+Filename: makenote-1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: makenote-1.5.dist-info/RECORD
+Filename: makenote-1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## makenote/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.5"
+__version__ = "1.6"
```

## Comparing `makenote-1.5.data/scripts/makenote` & `makenote-1.6.data/scripts/makenote`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import shutil
 
 # default table name
 default_table_name = 'journals'
 
 # database file is stored here.
 diaryFileName = f'{os.getenv("HOME")}/.local/share/makenote/databases/diaryFile.db'
-diaryFileName = f'./1.db'
 
 parser = argparse.ArgumentParser(prefix_chars='-', prog='makenote',
                                  formatter_class=argparse.RawDescriptionHelpFormatter,
                                  description='add notes to diary or show them',
                                  epilog='''examples:
     makenote -t journals it was a nice day today!
     makenote -show journals''')
```

## Comparing `makenote-1.5.dist-info/LICENSE` & `makenote-1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `makenote-1.5.dist-info/METADATA` & `makenote-1.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makenote
-Version: 1.5
+Version: 1.6
 Summary: command line tool for quickly writing journals
 Home-page: https://github.com/ekm507/makenote
 Author: Erfan Kheirollahi
 Author-email: ekm507@gmail.com
 License: UNKNOWN
 Keywords: makenote
 Platform: UNKNOWN
```

