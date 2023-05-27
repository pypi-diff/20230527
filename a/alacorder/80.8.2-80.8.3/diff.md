# Comparing `tmp/alacorder-80.8.2.tar.gz` & `tmp/alacorder-80.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.8.2.tar", max compression
+gzip compressed data, was "alacorder-80.8.3.tar", max compression
```

## Comparing `alacorder-80.8.2.tar` & `alacorder-80.8.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.8.2/LICENSE
--rw-r--r--   0        0        0     7315 2023-05-26 22:11:39.116260 alacorder-80.8.2/README.md
--rw-r--r--   0        0        0      746 2023-05-26 22:14:29.812276 alacorder-80.8.2/pyproject.toml
--rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.8.2/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.8.2/src/alacorder/__init__.py
--rw-r--r--   0        0        0   279023 2023-05-26 22:11:58.155606 alacorder-80.8.2/src/alacorder/__main__.py
--rw-r--r--   0        0        0   279023 2023-05-26 22:11:52.493194 alacorder-80.8.2/src/alacorder/alac.py
--rw-r--r--   0        0        0     8286 1970-01-01 00:00:00.000000 alacorder-80.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.8.3/LICENSE
+-rw-r--r--   0        0        0     7315 2023-05-26 22:11:39.116260 alacorder-80.8.3/README.md
+-rw-r--r--   0        0        0      746 2023-05-27 17:57:08.979906 alacorder-80.8.3/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-26 22:17:08.501994 alacorder-80.8.3/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.8.3/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.8.3/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   279748 2023-05-27 17:56:59.058798 alacorder-80.8.3/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   279748 2023-05-27 17:56:53.219581 alacorder-80.8.3/src/alacorder/alac.py
+-rw-r--r--   0        0        0     8286 1970-01-01 00:00:00.000000 alacorder-80.8.3/PKG-INFO
```

### Comparing `alacorder-80.8.2/LICENSE` & `alacorder-80.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.2/README.md` & `alacorder-80.8.3/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.2/pyproject.toml` & `alacorder-80.8.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.8.2"
+version = "80.8.3"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.8.2/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-80.8.3/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.2/src/alacorder/__main__.py` & `alacorder-80.8.3/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.8.2"
+version = "80.8.3"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3260,14 +3260,15 @@
     for col in tempcols:
         if col not in query.columns:
             query = query.with_columns([pl.lit("").alias(col)])
 
     query = query.with_columns(
         [
             pl.col("RETRIEVED").cast(pl.Utf8, strict=False),
+            pl.col("TEMP_NAME").str.replace(",","").str.extract(r'^([A-Z]+ [A-Z]+)')
         ]
     )
 
     if goodquery:
         print(f"{query.shape[0]} queries read from input query file.")
         return query
     else:
@@ -3338,15 +3339,14 @@
     login(driver, cID=cID, uID=uID, pwd=pwd, window=window)
 
     for i, r in enumerate(query.rows(named=True)):
         if query[i, "QUERY_COMPLETE"] == "Y":
             continue
         if driver.current_url == "https://v2.alacourt.com/frmlogin.aspx":
             login(driver, cID, uID, pwd, window=window)
-        # driver.implicitly_wait(1)
         results = party_search(
             driver,
             name=r["TEMP_NAME"],
             party_type=r["TEMP_PARTY_TYPE"],
             ssn=r["TEMP_SSN"],
             dob=r["TEMP_DOB"],
             county=r["TEMP_COUNTY"],
@@ -4079,14 +4079,16 @@
     sentences = sentences.select("CaseNo","Name","AIS","Institution","Race","Sex","HairColor","EyeColor","Height","Weight","BirthYear","Custody","Sentenced","Offense","Term","SentenceJailCredit","Type","County","SUF","AdmitDate","TotalTerm","TimeServed","JailCredit","GoodTimeReceived","GoodTimeRevoked","MinReleaseDate","ParoleConsiderationDate","ParoleStatus")
     return sentences
 
 
 def crawl_adoc(path, window=None):
     alphabet = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
     print("Connecting to ADOC...")
+    opt = webdriver.ChromeOptions()
+    opt.add_argument("--headless=new")
     driver = webdriver.Chrome()
     driver.get("http://www.doc.state.al.us/inmatesearch")
     results = []
     if not window:
         for x in tqdm(alphabet):
             last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
             last_name_box.send_keys(x)
@@ -4806,25 +4808,29 @@
             window["MA"].update(disabled=False)
             window["TB"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["SUM"].update(disabled=False)
             window["RN"].update(disabled=False)
             window["MT"].update(disabled=False)
             window["NEWQUERY"].update(disabled=False)
+            window["ADOC-FETCH-NEWQUERY"].update(disabled=False)
+            window["CRAWL"].update(disabled=False)
         elif "COMPLETE" in event:
             print("Alacorder completed the task.")
             window["AA"].update(disabled=False)
             window["SQ"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["TB"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["SUM"].update(disabled=False)
             window["RN"].update(disabled=False)
             window["MT"].update(disabled=False)
             window["NEWQUERY"].update(disabled=False)
+            window["CRAWL"].update(disabled=False)
+            window["ADOC-FETCH-NEWQUERY"].update(disabled=False)
             window["PROGRESS"].update(current_count=0, max=100)
             sg.popup("Alacorder completed the task.")
             continue
         elif event == "NEWQUERY":
             if window["SQ-INPUTPATH"].get() == "":
                 sg.popup(
                     "To create empty query template, enter file output path (extension must be .xlsx) in Input Path, then press the New Query button to try again."
@@ -4845,14 +4851,20 @@
                 no_write=False,
                 overwrite=window["SUM-OVERWRITE"].get(),
                 window=window,
             )
             thread = threading.Thread(target=pairs, args=[cf], daemon=True).start()
             print("Creating AIS / Unique ID pairs template...")
             window["MT"].update(disabled=True)
+        elif event == "ADOC-FETCH-NEWQUERY":
+            if window["ADOC-FETCH-INPUTPATH"].get() == '':
+                sg.popup("Enter valid path and try again.")
+                continue
+            out = pl.DataFrame({'AIS': [], 'FirstName': [], 'LastName': []})
+            write(out, sheet_names=["adoc-fetch-template"], path=window["ADOC-FETCH-INPUTPATH"].get())
         elif event == "SUM":
             cf = set(
                 window["SUM-INPUTPATH"].get(),
                 window["SUM-OUTPUTPATH"].get(),
                 pairs=window["SUM-PAIRS"].get(),
                 vrr_summary=True,
                 log=True,
```

### Comparing `alacorder-80.8.2/src/alacorder/alac.py` & `alacorder-80.8.3/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.8.2"
+version = "80.8.3"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3260,14 +3260,15 @@
     for col in tempcols:
         if col not in query.columns:
             query = query.with_columns([pl.lit("").alias(col)])
 
     query = query.with_columns(
         [
             pl.col("RETRIEVED").cast(pl.Utf8, strict=False),
+            pl.col("TEMP_NAME").str.replace(",","").str.extract(r'^([A-Z]+ [A-Z]+)')
         ]
     )
 
     if goodquery:
         print(f"{query.shape[0]} queries read from input query file.")
         return query
     else:
@@ -3338,15 +3339,14 @@
     login(driver, cID=cID, uID=uID, pwd=pwd, window=window)
 
     for i, r in enumerate(query.rows(named=True)):
         if query[i, "QUERY_COMPLETE"] == "Y":
             continue
         if driver.current_url == "https://v2.alacourt.com/frmlogin.aspx":
             login(driver, cID, uID, pwd, window=window)
-        # driver.implicitly_wait(1)
         results = party_search(
             driver,
             name=r["TEMP_NAME"],
             party_type=r["TEMP_PARTY_TYPE"],
             ssn=r["TEMP_SSN"],
             dob=r["TEMP_DOB"],
             county=r["TEMP_COUNTY"],
@@ -4079,14 +4079,16 @@
     sentences = sentences.select("CaseNo","Name","AIS","Institution","Race","Sex","HairColor","EyeColor","Height","Weight","BirthYear","Custody","Sentenced","Offense","Term","SentenceJailCredit","Type","County","SUF","AdmitDate","TotalTerm","TimeServed","JailCredit","GoodTimeReceived","GoodTimeRevoked","MinReleaseDate","ParoleConsiderationDate","ParoleStatus")
     return sentences
 
 
 def crawl_adoc(path, window=None):
     alphabet = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
     print("Connecting to ADOC...")
+    opt = webdriver.ChromeOptions()
+    opt.add_argument("--headless=new")
     driver = webdriver.Chrome()
     driver.get("http://www.doc.state.al.us/inmatesearch")
     results = []
     if not window:
         for x in tqdm(alphabet):
             last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
             last_name_box.send_keys(x)
@@ -4806,25 +4808,29 @@
             window["MA"].update(disabled=False)
             window["TB"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["SUM"].update(disabled=False)
             window["RN"].update(disabled=False)
             window["MT"].update(disabled=False)
             window["NEWQUERY"].update(disabled=False)
+            window["ADOC-FETCH-NEWQUERY"].update(disabled=False)
+            window["CRAWL"].update(disabled=False)
         elif "COMPLETE" in event:
             print("Alacorder completed the task.")
             window["AA"].update(disabled=False)
             window["SQ"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["TB"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["SUM"].update(disabled=False)
             window["RN"].update(disabled=False)
             window["MT"].update(disabled=False)
             window["NEWQUERY"].update(disabled=False)
+            window["CRAWL"].update(disabled=False)
+            window["ADOC-FETCH-NEWQUERY"].update(disabled=False)
             window["PROGRESS"].update(current_count=0, max=100)
             sg.popup("Alacorder completed the task.")
             continue
         elif event == "NEWQUERY":
             if window["SQ-INPUTPATH"].get() == "":
                 sg.popup(
                     "To create empty query template, enter file output path (extension must be .xlsx) in Input Path, then press the New Query button to try again."
@@ -4845,14 +4851,20 @@
                 no_write=False,
                 overwrite=window["SUM-OVERWRITE"].get(),
                 window=window,
             )
             thread = threading.Thread(target=pairs, args=[cf], daemon=True).start()
             print("Creating AIS / Unique ID pairs template...")
             window["MT"].update(disabled=True)
+        elif event == "ADOC-FETCH-NEWQUERY":
+            if window["ADOC-FETCH-INPUTPATH"].get() == '':
+                sg.popup("Enter valid path and try again.")
+                continue
+            out = pl.DataFrame({'AIS': [], 'FirstName': [], 'LastName': []})
+            write(out, sheet_names=["adoc-fetch-template"], path=window["ADOC-FETCH-INPUTPATH"].get())
         elif event == "SUM":
             cf = set(
                 window["SUM-INPUTPATH"].get(),
                 window["SUM-OUTPUTPATH"].get(),
                 pairs=window["SUM-PAIRS"].get(),
                 vrr_summary=True,
                 log=True,
```

### Comparing `alacorder-80.8.2/PKG-INFO` & `alacorder-80.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.8.2
+Version: 80.8.3
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

