# Comparing `tmp/makenote-1.3-py3-none-any.whl.zip` & `tmp/makenote-1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 17362 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       20 b- defN 23-May-26 10:04 makenote/__init__.py
--rwxrwxr-x  2.0 unx     8459 b- defN 23-May-26 10:04 makenote-1.3.data/scripts/makenote
--rw-rw-r--  2.0 unx    35099 b- defN 23-May-26 10:04 makenote-1.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3022 b- defN 23-May-26 10:04 makenote-1.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-26 10:04 makenote-1.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-May-26 10:04 makenote-1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      547 b- defN 23-May-26 10:04 makenote-1.3.dist-info/RECORD
-7 files, 47248 bytes uncompressed, 16392 bytes compressed:  65.3%
+Zip file size: 17704 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx       20 b- defN 23-May-26 22:40 makenote/__init__.py
+-rwxrwxr-x  2.0 unx    10744 b- defN 23-May-26 22:40 makenote-1.5.data/scripts/makenote
+-rw-rw-r--  2.0 unx    35099 b- defN 23-May-26 22:40 makenote-1.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3022 b- defN 23-May-26 22:40 makenote-1.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-26 22:40 makenote-1.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-26 22:40 makenote-1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      548 b- defN 23-May-26 22:40 makenote-1.5.dist-info/RECORD
+7 files, 49534 bytes uncompressed, 16734 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: makenote/__init__.py
 Comment: 
 
-Filename: makenote-1.3.data/scripts/makenote
+Filename: makenote-1.5.data/scripts/makenote
 Comment: 
 
-Filename: makenote-1.3.dist-info/LICENSE
+Filename: makenote-1.5.dist-info/LICENSE
 Comment: 
 
-Filename: makenote-1.3.dist-info/METADATA
+Filename: makenote-1.5.dist-info/METADATA
 Comment: 
 
-Filename: makenote-1.3.dist-info/WHEEL
+Filename: makenote-1.5.dist-info/WHEEL
 Comment: 
 
-Filename: makenote-1.3.dist-info/top_level.txt
+Filename: makenote-1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: makenote-1.3.dist-info/RECORD
+Filename: makenote-1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## makenote/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.3"
+__version__ = "1.5"
```

## Comparing `makenote-1.3.data/scripts/makenote` & `makenote-1.5.data/scripts/makenote`

 * *Files 13% similar despite different names*

```diff
@@ -7,38 +7,45 @@
 import shutil
 
 # default table name
 default_table_name = 'journals'
 
 # database file is stored here.
 diaryFileName = f'{os.getenv("HOME")}/.local/share/makenote/databases/diaryFile.db'
+diaryFileName = f'./1.db'
 
 parser = argparse.ArgumentParser(prefix_chars='-', prog='makenote',
                                  formatter_class=argparse.RawDescriptionHelpFormatter,
                                  description='add notes to diary or show them',
                                  epilog='''examples:
     makenote -t journals it was a nice day today!
     makenote -show journals''')
 
 parser.add_argument("-s", '--show', dest='show',
                     help="table to show", nargs='?', const=default_table_name, metavar='TABLE_NAME')
+parser.add_argument("-T", '--tail', dest='tail',
+                    help="show last 10 items of table", nargs='?', const=default_table_name, metavar='TABLE_NAME')
+
 # parser.add_argument("-d", '--default', dest='default',
 #                     help="set default table", default=None)
 parser.add_argument("-c", '--create', dest='create_table',
                     help="create table", default=None, metavar='TABLE_NAME')
 parser.add_argument("-l", '--list', dest='list_tables',
                     help="list tables", default=None, action="store_true")
 parser.add_argument("-t", "--table", dest="table_name", help="table for notes",
                     default=default_table_name)
 parser.add_argument("-m", "--merge",  help="merge two databases",
                     default=None, nargs=3, metavar=('FIRST','SECOND','OUTPUT'))
 parser.add_argument("-x", "--export",  help="export database into file",
                     default=None, metavar='FILENAME')
 parser.add_argument("text",  help="text", default=None, nargs='*')
 
+parser.add_argument("-u", "--update",  help="edit note. add entry number",
+                    default=None, metavar='note_id', type=int)
+
 args = parser.parse_args()
 
 def add_note(sqlite_cursor, table_name, note_text):
     
     date_and_time = datetime.datetime.now()
 
     sqlite_cursor.execute(
@@ -47,21 +54,69 @@
     # let user know it works
     if show_style == 1:
         print(f'{datetime.datetime.ctime(date_and_time)} - {table_name} - note saved!')
     elif show_style == 2:
         print(f'\u001b[36m{datetime.datetime.ctime(date_and_time)}\u001b[0m - {table_name} - note saved!')
 
 
+def update_entry(sqlite_cursor, table_name, note_id: int, note_text: str) -> None:
+    try:
+        # get the record from sqlite
+        sqlite_cursor.execute(f"SELECT * FROM {table_name} LIMIT {note_id - 1}, 1;")
+        record = sqlite_cursor.fetchone()
+        
+        print(f"entry {note_id} with text \"{record[1]}\" updated")
+
+        cur.execute(f"""UPDATE {table_name} SET note = "{note_text}" LIMIT {note_id-1},{1};""")
+
+    except sqlite3.OperationalError as error_text:
+        print(error_text)
+        exit(1)
+
+
+def tail_show_table(sqlite_cursor, table_name, limit):
+    try:
+        # get records from sqlite
+        sqlite_cursor.execute(f"SELECT count(*) FROM {table_name}")
+        N = sqlite_cursor.fetchone()[0]
+        records = sqlite_cursor.execute(f"SELECT * FROM {table_name} LIMIT {N - limit}, {limit};")
+        # print them all
+        i = 0
+        for r in records:
+            i += 1
+            print(i, end="  ")
+
+            # if style number 1 is selected
+            if show_style == 1:
+                # replace that utf representation of نیم‌فاصله with itself
+                r[1].replace('\u200c', ' ')
+                # remove miliseconds from date and time and print a in a stylized format
+                print(f'{r[0][:10]}   {r[0][10:18]}    {r[1]}')
+            
+            elif show_style == 2:
+                print(f'\u001b[36m{r[0][:10]} {r[0][10:18]}\u001b[0m  {r[1]}')
+
+            # if no show style is specified
+            else:
+                # print in python default style of printing
+                print(r)
+    # if there was an error, print error text and exit
+    except sqlite3.OperationalError as error_text:
+        print(error_text)
+        exit(1)
 
 def show_table(sqlite_cursor, table_name):
     try:
         # get records from sqlite
         records = sqlite_cursor.execute(f"SELECT * FROM {table_name};")
         # print them all
+        i = 0
         for r in records:
+            i += 1
+            print(i, end="  ")
 
             # if style number 1 is selected
             if show_style == 1:
                 # replace that utf representation of نیم‌فاصله with itself
                 r[1].replace('\u200c', ' ')
                 # remove miliseconds from date and time and print a in a stylized format
                 print(f'{r[0][:10]}   {r[0][10:18]}    {r[1]}')
@@ -196,27 +251,30 @@
 # connect to sqlite file
 con = sqlite3.connect(diaryFileName)
 # define a cursor to execute commands
 cur = con.cursor()
 
 if args.show:
     show_table(cur, args.show)
+elif args.tail:
+    tail_show_table(cur, args.tail, limit=10)
 elif args.list_tables:
     list_tables(cur)
 elif args.create_table:
     make_table(cur, args.create_table)
 elif args.export:
     shutil.copy(diaryFileName, args.export)
     print(f'exported to {os.path.realpath(args.export)}')
 elif args.merge:
     firstdb, seconddb, outdb = args.merge
     merge_databases_by_name(firstdb, seconddb, outdb)
 # elif args.default:
 #     default_table_name = args.default
 #     table_name = args.default
+
 else:
 
     # note will be added to this table
     table_name = args.table_name
 
     if not table_exists(cur, table_name):
         print(f'table {table_name} does not exist')
@@ -231,14 +289,17 @@
         note_text = ' '.join(args.text)
     else:
         try:
             note_text = ''.join(sys.stdin.readlines())[:-1]
         except KeyboardInterrupt:
             exit(1)
 
-    add_note(cur, table_name, note_text)
+    if args.update:
+        update_entry(cur, args.table_name, args.update, note_text)
+    else:
+        add_note(cur, table_name, note_text)
 
 # commit all changes in the database so they are saved.
 con.commit()
 
 # close the database file
 con.close()
```

## Comparing `makenote-1.3.dist-info/LICENSE` & `makenote-1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `makenote-1.3.dist-info/METADATA` & `makenote-1.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makenote
-Version: 1.3
+Version: 1.5
 Summary: command line tool for quickly writing journals
 Home-page: https://github.com/ekm507/makenote
 Author: Erfan Kheirollahi
 Author-email: ekm507@gmail.com
 License: UNKNOWN
 Keywords: makenote
 Platform: UNKNOWN
```

