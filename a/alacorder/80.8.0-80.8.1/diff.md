# Comparing `tmp/alacorder-80.8.0.tar.gz` & `tmp/alacorder-80.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.8.0.tar", max compression
+gzip compressed data, was "alacorder-80.8.1.tar", max compression
```

## Comparing `alacorder-80.8.0.tar` & `alacorder-80.8.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.8.0/LICENSE
--rw-r--r--   0        0        0     6518 2023-05-23 14:35:47.192010 alacorder-80.8.0/README.md
--rw-r--r--   0        0        0      746 2023-05-25 18:10:16.703624 alacorder-80.8.0/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-23 18:11:50.134411 alacorder-80.8.0/src/alacorder/.DS_Store
--rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.8.0/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.8.0/src/alacorder/__init__.py
--rw-r--r--   0        0        0   255361 2023-05-25 18:09:25.182499 alacorder-80.8.0/src/alacorder/__main__.py
--rw-r--r--   0        0        0   255361 2023-05-25 18:08:54.049754 alacorder-80.8.0/src/alacorder/alac.py
--rw-r--r--   0        0        0     7489 1970-01-01 00:00:00.000000 alacorder-80.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.8.1/LICENSE
+-rw-r--r--   0        0        0     6518 2023-05-23 14:35:47.192010 alacorder-80.8.1/README.md
+-rw-r--r--   0        0        0      746 2023-05-26 18:56:57.618594 alacorder-80.8.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-23 18:11:50.134411 alacorder-80.8.1/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.8.1/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.8.1/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   278763 2023-05-26 18:56:26.356544 alacorder-80.8.1/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   278763 2023-05-26 18:56:22.758990 alacorder-80.8.1/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7489 1970-01-01 00:00:00.000000 alacorder-80.8.1/PKG-INFO
```

### Comparing `alacorder-80.8.0/LICENSE` & `alacorder-80.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.0/README.md` & `alacorder-80.8.1/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.0/pyproject.toml` & `alacorder-80.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.8.0"
+version = "80.8.1"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.8.0/src/alacorder/.DS_Store` & `alacorder-80.8.1/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.0/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-80.8.1/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.0/src/alacorder/__main__.py` & `alacorder-80.8.1/src/alacorder/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.8.0"
+version = "80.8.1"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3272,266 +3272,14 @@
         return query
     else:
         print(
             "Try again with at least one valid column header: [NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, NO_RECORDS, FILED_BEFORE, FILED_AFTER, RETRIEVED, CASES_FOUND, QUERY_COMPLETE]"
         )
         return None
 
-
-def make_fetch_queue_from_crawl(df):
-    if isinstance(df, str):
-        df = read(df)
-    df = df.select(
-        [
-            pl.col("AIS"),
-            pl.col("Name").str.extract(r', ([A-Z]+)').alias("FirstName"),
-            pl.col("Name").str.extract(r'^([A-Z]+)').alias("LastName"),
-        ]
-    )
-    return df
-
-def adoc_fetch(df=None, path=None, cf=None):
-    if cf:
-        df = read(cf['INPUTS'])
-        path = cf['OUTPUT_PATH']
-    if df:
-        if isinstance(df, str):
-            dfpath = df
-            df = read(df)
-        else:
-            dfpath = None
-    if 'Retrieved' not in df.columns:
-        df = df.select("AIS", "FirstName", "LastName")
-        df = df.with_columns(pl.lit("").alias("Retrieved"))
-    df = df.with_columns(pl.col("AIS").cast(pl.Utf8, strict=False))
-    out = pl.DataFrame()
-    driver = webdriver.Chrome()
-    for i, r in enumerate(tqdm(df.rows(named=True))):
-        if r['Retrieved'] != '' and r['Retrieved'] != None:
-            continue
-        try:
-            out = pl.concat([out, read_top_result(driver, r['AIS'], r['FirstName'], r['LastName'])])
-        except:
-            pass
-        df[i, 'Retrieved'] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
-        if dfpath and df.shape[0] > 10 and i % 10 == 0:
-            write(df, sheet_names=["adoc_progress"], path=dfpath)
-        if df.shape[0] > 10 and i % 10 == 0 and path:
-            write(out, sheet_names=["adoc"], path=path)
-    if path:
-        write(out, sheet_names=["adoc"], path=path)
-    if dfpath:
-        write(df, sheet_names=["adoc_progress"], path=dfpath)
-    return out, df
-
-def read_top_result(driver, ais, first, last):
-    driver.get("http://www.doc.state.al.us/inmatesearch")
-    ais_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtAIS")
-    first_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtFName")
-    last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
-    send_button = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearch")
-    ais_box.send_keys(ais)
-    first_name_box.send_keys(first)
-    last_name_box.send_keys(last)
-    send_button.click()
-    urls = driver.find_elements(by=By.TAG_NAME, value="a")
-    results = []
-    for x in urls:
-        try:
-            if 'InmateResults' in x.get_attribute("ID"):
-                results += [x]
-        except:
-            pass
-    try:
-        results[0].click()
-        return read_adoc_page(driver)
-    except:
-        return pl.DataFrame()
-
-
-def filter_missing_cases(adoc_df, cases_df):
-    if isinstance(adoc_df, str):
-        adoc_df = read(adoc_df)
-    if isinstance(cases_df, str):
-        cases_df = read(cases_df)
-    if 'AllPagesText' in cases_df.columns:
-        cases_df = set(cases_df, table="cases", now=True)
-    cases_df = cases_df.with_columns(
-        pl.col("CaseNumber").str.extract(r'(\w\w-\d\d\d\d-\d\d\d\d\d\d)').alias("CaseNoFragment")
-    )
-    clist = cases_df.select("CaseNoFragment").to_series().to_list()
-    cmap = pl.DataFrame(
-        {
-            'Selection': ['94 - ARDMORE', '93 - ATHENS', '04 - AUTAUGA', '05 - BALDWIN', '06 - BARBOUR - CLAYTON', '69 - BARBOUR - EUFAULA', '89 - BERRY', '07 - BIBB', '08 - BLOUNT', '87 - BRUNDIDGE MUNICIPAL COURT', '09 - BULLOCK', '10 - BUTLER', '11 - CALHOUN', '12 - CHAMBERS', '13 - CHEROKEE', '90 - CHEROKEE', '14 - CHILTON', '15 - CHOCTAW', '16 - CLARKE', '17 - CLAY', '18 - CLEBURNE', '19 - COFFEE - ELBA', '71 - COFFEE - ENTERPRISE', '20 - COLBERT', '21 - CONECUH', '22 - COOSA', '23 - COVINGTON', '24 - CRENSHAW', '25 - CULLMAN', '26 - DALE', '27 - DALLAS', '28 - DeKALB', '29 - ELMORE', '30 - ESCAMBIA', '31 - ETOWAH', '32 - FAYETTE', '33 - FRANKLIN', '34 - GENEVA', '35 - GREENE', '36 - HALE', '37 - HENRY', '38 - HOUSTON', '39 - JACKSON', '68 - JEFFERSON - BESSEMER', '01 - JEFFERSON - BIRMINGHAM', '40 - LAMAR', '41 - LAUDERDALE', '42 - LAWRENCE', '43 - LEE', '44 - LIMESTONE', '82 - LIVINGSTON', '45 - LOWNDES', '46 - MACON', '47 - MADISON', '48 - MARENGO', '49 - MARION', '50 - MARSHALL', '92 - MILLBROOK', '02 - MOBILE', '51 - MONROE', '03 - MONTGOMERY', '52 - MORGAN', '53 - PERRY', '80 - PHENIX CITY', '54 - PICKENS', '55 - PIKE', '88 - PRATTVILLE', '56 - RANDOLPH', '57 - RUSSELL', '58 - SHELBY', '59 - ST. CLAIR - ASHVILLE', '75 - ST. CLAIR - PELL CITY', '81 - SUMITON MUNICIPAL COURT', '60 - SUMTER', '74 - TALLADEGA - SYLACAUGA', '61 - TALLADEGA - TALLADEGA', '70 - TALLAPOOSA - ALEX CITY', '62 - TALLAPOOSA - DADEVILLE', '63 - TUSCALOOSA', '64 - WALKER', '65 - WASHINGTON', '95 - WETUMPKA MUNICIPAL COURT', '66 - WILCOX', '67 - WINSTON'],
-            'CountyNumber': ['94', '93', '04', '05', '06', '69', '89', '07', '08', '87', '09', '10', '11', '12', '13', '90', '14', '15', '16', '17', '18', '19', '71', '20', '21', '22', '23', '24', '25', '26', '27', '28', '29', '30', '31', '32', '33', '34', '35', '36', '37', '38', '39', '68', '01', '40', '41', '42', '43', '44', '82', '45', '46', '47', '48', '49', '50', '92', '02', '51', '03', '52', '53', '80', '54', '55', '88', '56', '57', '58', '59', '75', '81', '60', '74', '61', '70', '62', '63', '64', '65', '95', '66', '67'],
-            'County': ['ARDMORE', 'ATHENS', 'AUTAUGA', 'BALDWIN', 'BARBOUR - CLAYTON', 'BARBOUR - EUFAULA', 'BERRY', 'BIBB', 'BLOUNT', 'BRUNDIDGE MUNICIPAL COURT', 'BULLOCK', 'BUTLER', 'CALHOUN', 'CHAMBERS', 'CHEROKEE', 'CHEROKEE', 'CHILTON', 'CHOCTAW', 'CLARKE', 'CLAY', 'CLEBURNE', 'COFFEE - ELBA', 'COFFEE - ENTERPRISE', 'COLBERT', 'CONECUH', 'COOSA', 'COVINGTON', 'CRENSHAW', 'CULLMAN', 'DALE', 'DALLAS', 'DeKALB', 'ELMORE', 'ESCAMBIA', 'ETOWAH', 'FAYETTE', 'FRANKLIN', 'GENEVA', 'GREENE', 'HALE', 'HENRY', 'HOUSTON', 'JACKSON', 'JEFFERSON - BESSEMER', 'JEFFERSON - BIRMINGHAM', 'LAMAR', 'LAUDERDALE', 'LAWRENCE', 'LEE', 'LIMESTONE', 'LIVINGSTON', 'LOWNDES', 'MACON', 'MADISON', 'MARENGO', 'MARION', 'MARSHALL', 'MILLBROOK', 'MOBILE', 'MONROE', 'MONTGOMERY', 'MORGAN', 'PERRY', 'PHENIX CITY', 'PICKENS', 'PIKE', 'PRATTVILLE', 'RANDOLPH', 'RUSSELL', 'SHELBY', 'ST. CLAIR - ASHVILLE', 'ST. CLAIR - PELL CITY', 'SUMITON MUNICIPAL COURT', 'SUMTER', 'TALLADEGA - SYLACAUGA', 'TALLADEGA - TALLADEGA', 'TALLAPOOSA - ALEX CITY', 'TALLAPOOSA - DADEVILLE', 'TUSCALOOSA', 'WALKER', 'WASHINGTON', 'WETUMPKA MUNICIPAL COURT', 'WILCOX', 'WINSTON'] 
-        }
-    )
-    adoc_df = adoc_df.join(cmap, on="County", how="left")
-    adoc_df = adoc_df.with_columns(
-        pl.concat_str(
-            [
-                pl.col("CountyNumber"),
-                pl.lit("-"),
-                pl.col("CaseNo").str.extract(r"(\w\w)"),
-                pl.lit("-"),
-                pl.col("CaseNo").str.extract(r'(\d\d\d\d)\-'),
-                pl.lit("-"),
-                pl.col("CaseNo").str.extract(r'\-(\d\d\d\d\d\d)'),
-            ]
-        ).alias("CaseNoFragment")
-    )
-    out = adoc_df.filter(pl.col("CaseNoFragment").is_in(clist).is_not())
-    out = out.filter(pl.col("CaseNoFragment").is_null().is_not())
-    return out
-
-def read_adoc_page(driver):
-    rl = driver.find_elements(by=By.TAG_NAME, value="tr")
-    alltxt = []
-    for r in rl:
-        alltxt += [r.text]
-    name = driver.find_element(by=By.ID, value="MainContent_DetailsView2_Label1").text
-    allt = pl.DataFrame({'Tables': "\n".join(alltxt)})
-    allt = allt.with_columns(pl.col("Tables").str.split("SUF"))
-    allt = allt.explode("Tables")
-    allt = allt.with_columns(pl.col("Tables").str.split("Sentences"))
-    allt = allt.explode("Tables")
-    details = allt.filter(pl.col("Tables").str.contains("Date Total Term"))
-    sentences = allt.filter(pl.col("Tables").str.contains("Sentenced"))
-    inmate = allt.filter(pl.col("Tables").str.contains("Eye Color"))
-    sentences = sentences.with_row_count()
-    details = details.with_row_count()
-    inmate = inmate.select(
-        [
-            pl.lit(name).alias("Name"),
-            pl.col("Tables").str.extract(r'AIS:\s+(\d{8})').alias("AIS"),
-            pl.col("Tables").str.extract(r'Institution: ([A-Z\s]+)').alias("Institution"
-             ),
-            pl.col("Tables").str.extract(r'Race: ([A-Z])').alias("Race"),
-            pl.col("Tables").str.extract(r'Sex: ([A-Z])').alias("Sex"),
-            pl.col("Tables").str.extract(r'Hair Color: ([A-Z]+)').alias("HairColor"),
-            pl.col("Tables").str.extract(r'Eye Color: ([A-Z]+)').alias("EyeColor"),
-            pl.col("Tables").str.extract(r'Height: (.+)').alias("Height"),
-            pl.col("Tables").str.extract(r'Weight: (\d+)').alias("Weight"),
-            pl.col("Tables").str.extract(r'Birth Year: (\d\d\d\d)').alias("BirthYear"),
-            pl.col("Tables").str.extract(r'Custody (.+)').alias("Custody")
-        ]
-    )
-    sentences = sentences.with_columns(pl.col("Tables").str.split('\n'))
-    sentences = sentences.explode("Tables")
-    sentences = sentences.filter(pl.col("Tables").str.contains("[A-Z]"))
-    sentences = sentences.filter(pl.col("Tables").str.contains("Sentenced").is_not())
-    sentences = sentences.unique()
-    sentences = sentences.select(
-        [
-            pl.col("row_nr"),
-            pl.col("Tables").str.extract(r'([^\s]+)').alias("CaseNo"),
-            pl.col("Tables").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("Sentenced"),
-            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d (.+?) \d+Y \d+M \d+D').alias("Offense"),
-            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? (\d+Y \d+M \d+D)').alias("Term"),
-            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D (\d+)').cast(pl.Int64, strict=False).alias("SentenceJailCredit"),
-            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D \d+ \d* ?(C?o?n?c?u?r?r?e?n?t?)').alias("Type"),
-            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D \d+ \d* ?C?o?n?c?u?r?r?e?n?t? ?([A-Z]+)').alias("County")
-        ]
-    )
-    sentences = sentences.with_columns(
-        [
-            pl.when(pl.col("Type")=="C")
-            .then("")
-            .otherwise(pl.col("Type"))
-            .alias("Type"),
-            pl.when(pl.col("Type")=="C")
-            .then(pl.concat_str([pl.lit("C"),pl.col("County")]))
-            .otherwise(pl.col("County"))
-            .alias("County")
-        ]
-    )
-    details = details.with_columns(pl.col("Tables").str.split("\n"))
-    details = details.explode("Tables")
-    details = details.filter(pl.col("Tables").str.contains("Admit Date").is_not())
-    details = details.filter(pl.col("Tables").str.contains("[A-Z]"))
-    details = details.select(
-        [
-            pl.col("row_nr"),
-            pl.col("Tables").str.extract(r'^([A-Z])').alias("SUF"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?(\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("AdmitDate"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d (\d+Y \d+M \d+D)').alias("TotalTerm"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D (\d+Y \d+M \d+D)').alias("TimeServed"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D (\d+)').alias("JailCredit"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?(\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D?)').str.replace(r'Days .+','Days').alias("GoodTimeReceived"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?(\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D?)').str.replace(r'^\d Days','').str.replace(r'^\d+Y \d+M \d+D','').str.replace(r'Days .+','Days').str.strip().alias("GoodTimeRevoked"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("MinReleaseDate"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? \d\d/\d\d/\d\d\d\d (\d?\d?/?\d?\d?/?\d?\d?\d?\d?)').str.to_date('%m/%d/%Y', strict=False).alias("ParoleConsiderationDate"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? \d\d/\d\d/\d\d\d\d \d?\d?/?\d?\d?/?\d?\d?\d?\d? (.+)').str.strip().alias("ParoleStatus")
-        ]
-    )
-    sentences = sentences.join(details, how="left", on="row_nr")
-    sentences = sentences.with_columns(pl.lit(0).alias("Match"))
-    inmate = inmate.with_columns(pl.lit(0).alias("Match"))
-    sentences = sentences.join(inmate, how="left", on="Match").select(pl.exclude("Match", "row_nr"))
-    sentences = sentences.select("CaseNo","Name","AIS","Institution","Race","Sex","HairColor","EyeColor","Height","Weight","BirthYear","Custody","Sentenced","Offense","Term","SentenceJailCredit","Type","County","SUF","AdmitDate","TotalTerm","TimeServed","JailCredit","GoodTimeReceived","GoodTimeRevoked","MinReleaseDate","ParoleConsiderationDate","ParoleStatus")
-    return sentences
-
-def crawl_adoc(path):
-    alphabet = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
-    print("Connecting to ADOC...")
-    driver = webdriver.Chrome()
-    driver.get("http://www.doc.state.al.us/inmatesearch")
-    results = []
-    for x in alphabet:
-        last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
-        last_name_box.send_keys(x)
-        driver.implicitly_wait(1)
-        send_button = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearch")
-        send_button.click()
-        driver.implicitly_wait(1)
-        more_results = True
-        try:
-            while more_results:
-                driver.implicitly_wait(1)
-                lists = driver.find_elements(by=By.TAG_NAME, value="tr")
-                for x in lists:
-                    results += [x.text]
-                    print(x.text)
-                try:
-                    current_page = driver.find_element(by=By.ID, value="MainContent_gvInmateResults_lblCurrent")
-                    total_pages = driver.find_element(by=By.ID, value='MainContent_gvInmateResults_lblPages')
-                except:
-                    more_results = False
-                    search_again = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearchAgain")
-                    search_again.click()
-                if int(current_page.text) == int(total_pages.text):
-                    more_results = False
-                    search_again = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearchAgain")
-                    search_again.click()
-                else:
-                    next_button = driver.find_element(by=By.ID, value="MainContent_gvInmateResults_btnNext")
-                    next_button.click()
-        except:
-            time.sleep(2)
-            driver.get("http://www.doc.state.al.us/inmatesearch")
-
-        out = pl.DataFrame({'Rows': results})
-        out = out.filter(pl.col("Rows").str.contains("Inmate").is_not())
-        out = out.filter(pl.col("Rows").str.contains("Pages").is_not())
-        out = out.select(
-            [
-                pl.col("Rows").str.extract(r'^([0-9Z]{8})').alias("AIS"),
-                pl.col("Rows").str.extract(r'^[0-9Z]{8} ([A-Z]+, [A-Z\s]+?) \w \w \d\d\d\d').alias("Name"),
-                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? (\w) \w \d\d\d\d').alias("Race"),
-                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w (\w) \d\d\d\d').alias("Sex"),
-                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w (\d\d\d\d)').alias("YOB").cast(pl.Int64, strict=False),
-                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d ([A-Z\s]+)').str.strip().alias("Institution"),
-                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d [A-Z\s]+ (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("ReleaseDate")
-            ]
-        )
-        print(out)
-        write(out, sheet_names=['inmates'], path=path, overwrite=True)
-    return out
-
 def fetch(
     querypath="",
     dirpath="",
     cID="",
     uID="",
     pwd="",
     criminal_only=False,
@@ -3970,14 +3718,156 @@
     driver.get("https://v2.alacourt.com/frmIndexSearchForm.aspx")
 
     print("Successfully connected and logged into Alacourt!")
 
     return driver
 
 
+def start_alacourt_driver(cID, uID, pwd, dirpath=None):
+    opt = webdriver.ChromeOptions()
+    if dirpath:
+        opt.add_experimental_option(
+            "prefs",
+            {
+                "download.default_directory": dirpath,  # Set default directory for downloads
+                "download.prompt_for_download": False,  # To auto download the file
+                "download.directory_upgrade": True,
+                "plugins.always_open_pdf_externally": True,  # Don't display PDF in chrome
+            },
+        )
+    else:
+        opt.add_experimental_option(
+            "prefs",
+            {
+                "download.prompt_for_download": False,  # To auto download the file
+                "download.directory_upgrade": True,
+                "plugins.always_open_pdf_externally": True,  # Don't display PDF in chrome
+            },
+        )
+    print("Starting browser... Do not close while in progress!")
+    driver = webdriver.Chrome(options=opt)
+    login(driver, cID=cID, uID=uID, pwd=pwd)
+    return driver
+
+
+def case_number_search(case_number, driver):
+    driver.get("https://v2.alacourt.com/frmcaselookupform.aspx")
+    county_select = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCounty")
+    division_select = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlDivision")
+    case_year_select = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCaseYear")
+    case_number_input = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtCaseNumber")
+    case_extension_select = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlExt")
+    number_of_cases_select = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlNumberOfCases")
+    cmap = pl.DataFrame(
+        {
+            'Selection': ['94 - ARDMORE', '93 - ATHENS', '04 - AUTAUGA', '05 - BALDWIN', '06 - BARBOUR - CLAYTON', '69 - BARBOUR - EUFAULA', '89 - BERRY', '07 - BIBB', '08 - BLOUNT', '87 - BRUNDIDGE MUNICIPAL COURT', '09 - BULLOCK', '10 - BUTLER', '11 - CALHOUN', '12 - CHAMBERS', '13 - CHEROKEE', '90 - CHEROKEE', '14 - CHILTON', '15 - CHOCTAW', '16 - CLARKE', '17 - CLAY', '18 - CLEBURNE', '19 - COFFEE - ELBA', '71 - COFFEE - ENTERPRISE', '20 - COLBERT', '21 - CONECUH', '22 - COOSA', '23 - COVINGTON', '24 - CRENSHAW', '25 - CULLMAN', '26 - DALE', '27 - DALLAS', '28 - DeKALB', '29 - ELMORE', '30 - ESCAMBIA', '31 - ETOWAH', '32 - FAYETTE', '33 - FRANKLIN', '34 - GENEVA', '35 - GREENE', '36 - HALE', '37 - HENRY', '38 - HOUSTON', '39 - JACKSON', '68 - JEFFERSON - BESSEMER', '01 - JEFFERSON - BIRMINGHAM', '40 - LAMAR', '41 - LAUDERDALE', '42 - LAWRENCE', '43 - LEE', '44 - LIMESTONE', '82 - LIVINGSTON', '45 - LOWNDES', '46 - MACON', '47 - MADISON', '48 - MARENGO', '49 - MARION', '50 - MARSHALL', '92 - MILLBROOK', '02 - MOBILE', '51 - MONROE', '03 - MONTGOMERY', '52 - MORGAN', '53 - PERRY', '80 - PHENIX CITY', '54 - PICKENS', '55 - PIKE', '88 - PRATTVILLE', '56 - RANDOLPH', '57 - RUSSELL', '58 - SHELBY', '59 - ST. CLAIR - ASHVILLE', '75 - ST. CLAIR - PELL CITY', '81 - SUMITON MUNICIPAL COURT', '60 - SUMTER', '74 - TALLADEGA - SYLACAUGA', '61 - TALLADEGA - TALLADEGA', '70 - TALLAPOOSA - ALEX CITY', '62 - TALLAPOOSA - DADEVILLE', '63 - TUSCALOOSA', '64 - WALKER', '65 - WASHINGTON', '95 - WETUMPKA MUNICIPAL COURT', '66 - WILCOX', '67 - WINSTON'],
+            'CountyNumber': ['94', '93', '04', '05', '06', '69', '89', '07', '08', '87', '09', '10', '11', '12', '13', '90', '14', '15', '16', '17', '18', '19', '71', '20', '21', '22', '23', '24', '25', '26', '27', '28', '29', '30', '31', '32', '33', '34', '35', '36', '37', '38', '39', '68', '01', '40', '41', '42', '43', '44', '82', '45', '46', '47', '48', '49', '50', '92', '02', '51', '03', '52', '53', '80', '54', '55', '88', '56', '57', '58', '59', '75', '81', '60', '74', '61', '70', '62', '63', '64', '65', '95', '66', '67'],
+            'County': ['ARDMORE', 'ATHENS', 'AUTAUGA', 'BALDWIN', 'BARBOUR - CLAYTON', 'BARBOUR - EUFAULA', 'BERRY', 'BIBB', 'BLOUNT', 'BRUNDIDGE MUNICIPAL COURT', 'BULLOCK', 'BUTLER', 'CALHOUN', 'CHAMBERS', 'CHEROKEE', 'CHEROKEE', 'CHILTON', 'CHOCTAW', 'CLARKE', 'CLAY', 'CLEBURNE', 'COFFEE - ELBA', 'COFFEE - ENTERPRISE', 'COLBERT', 'CONECUH', 'COOSA', 'COVINGTON', 'CRENSHAW', 'CULLMAN', 'DALE', 'DALLAS', 'DeKALB', 'ELMORE', 'ESCAMBIA', 'ETOWAH', 'FAYETTE', 'FRANKLIN', 'GENEVA', 'GREENE', 'HALE', 'HENRY', 'HOUSTON', 'JACKSON', 'JEFFERSON - BESSEMER', 'JEFFERSON - BIRMINGHAM', 'LAMAR', 'LAUDERDALE', 'LAWRENCE', 'LEE', 'LIMESTONE', 'LIVINGSTON', 'LOWNDES', 'MACON', 'MADISON', 'MARENGO', 'MARION', 'MARSHALL', 'MILLBROOK', 'MOBILE', 'MONROE', 'MONTGOMERY', 'MORGAN', 'PERRY', 'PHENIX CITY', 'PICKENS', 'PIKE', 'PRATTVILLE', 'RANDOLPH', 'RUSSELL', 'SHELBY', 'ST. CLAIR - ASHVILLE', 'ST. CLAIR - PELL CITY', 'SUMITON MUNICIPAL COURT', 'SUMTER', 'TALLADEGA - SYLACAUGA', 'TALLADEGA - TALLADEGA', 'TALLAPOOSA - ALEX CITY', 'TALLAPOOSA - DADEVILLE', 'TUSCALOOSA', 'WALKER', 'WASHINGTON', 'WETUMPKA MUNICIPAL COURT', 'WILCOX', 'WINSTON'] 
+        }
+    )
+    dmap = pl.DataFrame({'Code': ['CC', 'CS', 'CV', 'DC', 'DR', 'DV', 'EQ', 'JU', 'MC', 'SM', 'TP', 'TR'], 'Selection': ['CC - CIRCUIT-CRIMINAL', 'CS - CHILD SUPPORT', 'CV - CIRCUIT-CIVIL', 'DC - DISTRICT-CRIMINAL', 'DR - DOMESTIC RELATIONS', 'DV - DISTRICT-CIVIL', 'EQ - EQUITY-CASES', 'JU - JUVENILE', 'MC - MUNICIPAL-CRIMINAL', 'SM - SMALL CLAIMS', 'TP - MUNICIPAL-PARKING', 'TR - TRAFFIC'] })
+    county_number = case_number[0:2]
+    division_code = case_number[3:5]
+    case_year = case_number[6:10]
+    six_digit = case_number[11:17]
+    if len(case_number) >= 20:
+        extension = case_number[18:20]
+    else:
+        extension = "00"
+    county = cmap.filter(pl.col("CountyNumber")==county_number).select("Selection").to_series()[0]
+    division = dmap.filter(pl.col("Code")==division_code).select("Selection").to_series()[0]
+    county_select.send_keys(county)
+    division_select.send_keys(division)
+    case_year_select.send_keys(case_year)
+    case_number_input.send_keys(six_digit)
+    search_button = driver.find_element(by=By.ID, value="searchButton")
+    search_button.click()
+    try:
+        driver.implicitly_wait(1)
+        driver.find_element(by=By.ID, value="Label2")
+    except:
+        try:
+            driver.implicitly_wait(1)
+            driver.find_element(by=By.ID, value="ContentPlaceHolder1_lnkPrint").click()
+            driver.implicitly_wait(1)
+            driver.find_element(by=By.ID, value="btnPrintCase").click()
+        except:
+            try:
+                time.sleep(1)
+                driver.implicitly_wait(1)
+                driver.find_element(by=By.ID, value="ContentPlaceHolder1_lnkPrint").click()
+                driver.implicitly_wait(1)
+                time.sleep(1)
+                driver.find_element(by=By.ID, value="btnPrintCase").click()
+            except:
+                pass
+
+
+def fetch_by_case_numbers(df, driver, window):
+    if isinstance(df, str):
+        dfpath = df
+        df = read(df)
+    else:
+        dfpath = None
+    if 'CountyNumber' in df.columns:
+        df = df.select(pl.exclude("CountyNumber"))
+    cmap = pl.DataFrame(
+        {
+            'Selection': ['94 - ARDMORE', '93 - ATHENS', '04 - AUTAUGA', '05 - BALDWIN', '06 - BARBOUR - CLAYTON', '69 - BARBOUR - EUFAULA', '89 - BERRY', '07 - BIBB', '08 - BLOUNT', '87 - BRUNDIDGE MUNICIPAL COURT', '09 - BULLOCK', '10 - BUTLER', '11 - CALHOUN', '12 - CHAMBERS', '13 - CHEROKEE', '90 - CHEROKEE', '14 - CHILTON', '15 - CHOCTAW', '16 - CLARKE', '17 - CLAY', '18 - CLEBURNE', '19 - COFFEE - ELBA', '71 - COFFEE - ENTERPRISE', '20 - COLBERT', '21 - CONECUH', '22 - COOSA', '23 - COVINGTON', '24 - CRENSHAW', '25 - CULLMAN', '26 - DALE', '27 - DALLAS', '28 - DeKALB', '29 - ELMORE', '30 - ESCAMBIA', '31 - ETOWAH', '32 - FAYETTE', '33 - FRANKLIN', '34 - GENEVA', '35 - GREENE', '36 - HALE', '37 - HENRY', '38 - HOUSTON', '39 - JACKSON', '68 - JEFFERSON - BESSEMER', '01 - JEFFERSON - BIRMINGHAM', '40 - LAMAR', '41 - LAUDERDALE', '42 - LAWRENCE', '43 - LEE', '44 - LIMESTONE', '82 - LIVINGSTON', '45 - LOWNDES', '46 - MACON', '47 - MADISON', '48 - MARENGO', '49 - MARION', '50 - MARSHALL', '92 - MILLBROOK', '02 - MOBILE', '51 - MONROE', '03 - MONTGOMERY', '52 - MORGAN', '53 - PERRY', '80 - PHENIX CITY', '54 - PICKENS', '55 - PIKE', '88 - PRATTVILLE', '56 - RANDOLPH', '57 - RUSSELL', '58 - SHELBY', '59 - ST. CLAIR - ASHVILLE', '75 - ST. CLAIR - PELL CITY', '81 - SUMITON MUNICIPAL COURT', '60 - SUMTER', '74 - TALLADEGA - SYLACAUGA', '61 - TALLADEGA - TALLADEGA', '70 - TALLAPOOSA - ALEX CITY', '62 - TALLAPOOSA - DADEVILLE', '63 - TUSCALOOSA', '64 - WALKER', '65 - WASHINGTON', '95 - WETUMPKA MUNICIPAL COURT', '66 - WILCOX', '67 - WINSTON'],
+            'CountyNumber': ['94', '93', '04', '05', '06', '69', '89', '07', '08', '87', '09', '10', '11', '12', '13', '90', '14', '15', '16', '17', '18', '19', '71', '20', '21', '22', '23', '24', '25', '26', '27', '28', '29', '30', '31', '32', '33', '34', '35', '36', '37', '38', '39', '68', '01', '40', '41', '42', '43', '44', '82', '45', '46', '47', '48', '49', '50', '92', '02', '51', '03', '52', '53', '80', '54', '55', '88', '56', '57', '58', '59', '75', '81', '60', '74', '61', '70', '62', '63', '64', '65', '95', '66', '67'],
+            'County': ['ARDMORE', 'ATHENS', 'AUTAUGA', 'BALDWIN', 'BARBOUR - CLAYTON', 'BARBOUR - EUFAULA', 'BERRY', 'BIBB', 'BLOUNT', 'BRUNDIDGE MUNICIPAL COURT', 'BULLOCK', 'BUTLER', 'CALHOUN', 'CHAMBERS', 'CHEROKEE', 'CHEROKEE', 'CHILTON', 'CHOCTAW', 'CLARKE', 'CLAY', 'CLEBURNE', 'COFFEE - ELBA', 'COFFEE - ENTERPRISE', 'COLBERT', 'CONECUH', 'COOSA', 'COVINGTON', 'CRENSHAW', 'CULLMAN', 'DALE', 'DALLAS', 'DeKALB', 'ELMORE', 'ESCAMBIA', 'ETOWAH', 'FAYETTE', 'FRANKLIN', 'GENEVA', 'GREENE', 'HALE', 'HENRY', 'HOUSTON', 'JACKSON', 'JEFFERSON - BESSEMER', 'JEFFERSON - BIRMINGHAM', 'LAMAR', 'LAUDERDALE', 'LAWRENCE', 'LEE', 'LIMESTONE', 'LIVINGSTON', 'LOWNDES', 'MACON', 'MADISON', 'MARENGO', 'MARION', 'MARSHALL', 'MILLBROOK', 'MOBILE', 'MONROE', 'MONTGOMERY', 'MORGAN', 'PERRY', 'PHENIX CITY', 'PICKENS', 'PIKE', 'PRATTVILLE', 'RANDOLPH', 'RUSSELL', 'SHELBY', 'ST. CLAIR - ASHVILLE', 'ST. CLAIR - PELL CITY', 'SUMITON MUNICIPAL COURT', 'SUMTER', 'TALLADEGA - SYLACAUGA', 'TALLADEGA - TALLADEGA', 'TALLAPOOSA - ALEX CITY', 'TALLAPOOSA - DADEVILLE', 'TUSCALOOSA', 'WALKER', 'WASHINGTON', 'WETUMPKA MUNICIPAL COURT', 'WILCOX', 'WINSTON'] 
+        }
+    )
+    df = df.join(cmap, on="County", how="left")
+    if 'Selection_right' in df.columns:
+        df = df.select(pl.exclude("Selection_right"))
+    if "CaseNo" in df.columns and "CaseNumber" not in df.columns:
+        df = df.with_columns(
+            pl.concat_str(
+                [
+                    pl.col("CountyNumber"),
+                    pl.lit("-"),
+                    pl.col("CaseNo").str.extract(r'^(\w\w)'),
+                    pl.lit("-"),
+                    pl.col("CaseNo").str.extract(r'(\d\d\d\d)\-'),
+                    pl.lit("-"),
+                    pl.col("CaseNo").str.extract(r'\-(\d\d\d\d\d\d)')
+                ]
+            ).alias("CaseNumber")
+    )
+    if 'Retrieved' not in df.columns:
+        df = df.with_columns(pl.lit("").alias("Retrieved"))
+    if not window:
+        for i, r in enumerate(tqdm(df.rows(named=True))):
+            if r['CaseNumber'] == '' or r['CaseNumber'] == None:
+                continue
+            if r['Retrieved'] != '' and r['Retrieved'] != None:
+                continue
+            case_number_search(r['CaseNumber'], driver)
+            df[i, 'Retrieved'] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
+            if dfpath and i % 10 == 0:
+                write(df.select(pl.exclude("CountyNumber", "Selection")), sheet_names=["adoc"], path=dfpath, overwrite=True)
+    if window:
+        window.write_event_value("PROGRESS-TEXT", 0)
+        window.write_event_value("PROGRESS-TEXT-TOTAL", len(df.rows()))
+        for i, r in enumerate(df.rows(named=True)):
+            if r['CaseNumber'] == '' or r['CaseNumber'] == None:
+                continue
+            if r['Retrieved'] != '' and r['Retrieved'] != None:
+                continue
+            case_number_search(r['CaseNumber'], driver)
+            df[i, 'Retrieved'] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
+            window.write_event_value("PROGRESS-TEXT", i + 1)
+            if dfpath and i % 10 == 0:
+                write(df.select(pl.exclude("CountyNumber", "Selection")), sheet_names=["adoc"], path=dfpath, overwrite=True)
+        window.write_event_value("FETCH-CN-COMPLETE", True)
+    write(df, sheet_names=["adoc"], path=dfpath, overwrite=True)
+    return df.select(pl.exclude("CountyNumber", "Selection"))
+
+
 def empty_query(path):
     """Create empty spreadsheet to fill and import as query submit search list to retrieve matching case records from Alacourt.com.
 
     Args:
         path (str): Desired output path (.xls, .xlsx)
 
     """
@@ -3997,14 +3887,340 @@
                 "RETRIEVED": [],
                 "CASES_FOUND": []
             }
     )
     return write(empty, sheet_names="query", path=path, overwrite=True)
 
 
+#   #   #   #        ADOC INMATE SEARCH        #   #   #   #
+
+
+def make_adoc_fetch_queue_from_crawl(df):
+    if isinstance(df, str):
+        df = read(df)
+    df = df.select(
+        [
+            pl.col("AIS"),
+            pl.col("Name").str.extract(r', ([A-Z]+)').alias("FirstName"),
+            pl.col("Name").str.extract(r'^([A-Z]+)').alias("LastName"),
+        ]
+    )
+    return df
+
+
+def adoc_fetch(df=None, path=None, window=None, cf=None):
+    if cf:
+        df = read(cf['INPUTS'])
+        path = cf['OUTPUT_PATH']
+    if df:
+        if isinstance(df, str):
+            dfpath = df
+            df = read(df)
+        else:
+            dfpath = None
+    if 'FirstName' not in df.columns or 'LastName' not in df.columns:
+        df = make_adoc_fetch_queue_from_crawl(df)
+    if 'Retrieved' not in df.columns:
+        df = df.with_columns(pl.lit("").alias("Retrieved"))
+    df = df.with_columns(pl.col("AIS").cast(pl.Utf8, strict=False))
+    out = pl.DataFrame()
+    driver = webdriver.Chrome()
+    if not window:
+        for i, r in enumerate(tqdm(df.rows(named=True))):
+            if r['Retrieved'] != '' and r['Retrieved'] != None:
+                continue
+            try:
+                out = pl.concat([out, read_adoc_top_result(driver, r['AIS'], r['FirstName'], r['LastName'])])
+            except:
+                pass
+            df[i, 'Retrieved'] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
+            if dfpath and df.shape[0] > 10 and i % 10 == 0:
+                write(df, sheet_names=["adoc_progress"], path=dfpath)
+            if df.shape[0] > 10 and i % 10 == 0 and path:
+                write(out, sheet_names=["adoc"], path=path)
+    if window:
+        window.write_event_value("PROGRESS-TEXT", 0)
+        window.write_event_value("PROGRESS-TEXT-TOTAL", df.shape[0])
+        for i, r in enumerate(df.rows(named=True)):
+            if r['Retrieved'] != '' and r['Retrieved'] != None:
+                continue
+            try:
+                out = pl.concat([out, read_adoc_top_result(driver, r['AIS'], r['FirstName'], r['LastName'])])
+            except:
+                pass
+            df[i, 'Retrieved'] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
+            window.write_event_value("PROGRESS-TEXT", i + 1)
+            if dfpath and df.shape[0] > 10 and i % 10 == 0:
+                write(df, sheet_names=["adoc_progress"], path=dfpath)
+            if df.shape[0] > 10 and i % 10 == 0 and path:
+                write(out, sheet_names=["adoc"], path=path)
+        window.write_event_value("ADOC-FETCH-COMPLETE", True)
+    if path:
+        write(out, sheet_names=["adoc"], path=path)
+    if dfpath:
+        write(df, sheet_names=["adoc_progress"], path=dfpath)
+    return out, df
+
+
+def read_adoc_top_result(driver, ais, first, last):
+    driver.get("http://www.doc.state.al.us/inmatesearch")
+    ais_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtAIS")
+    first_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtFName")
+    last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
+    send_button = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearch")
+    ais_box.send_keys(ais)
+    first_name_box.send_keys(first)
+    last_name_box.send_keys(last)
+    send_button.click()
+    urls = driver.find_elements(by=By.TAG_NAME, value="a")
+    results = []
+    for x in urls:
+        try:
+            if 'InmateResults' in x.get_attribute("ID"):
+                results += [x]
+        except:
+            pass
+    try:
+        results[0].click()
+        return read_adoc_page(driver)
+    except:
+        return pl.DataFrame()
+
+
+def read_adoc_page(driver):
+    rl = driver.find_elements(by=By.TAG_NAME, value="tr")
+    alltxt = []
+    for r in rl:
+        alltxt += [r.text]
+    name = driver.find_element(by=By.ID, value="MainContent_DetailsView2_Label1").text
+    allt = pl.DataFrame({'Tables': "\n".join(alltxt)})
+    allt = allt.with_columns(pl.col("Tables").str.split("SUF"))
+    allt = allt.explode("Tables")
+    allt = allt.with_columns(pl.col("Tables").str.split("Sentences"))
+    allt = allt.explode("Tables")
+    details = allt.filter(pl.col("Tables").str.contains("Date Total Term"))
+    sentences = allt.filter(pl.col("Tables").str.contains("Sentenced"))
+    inmate = allt.filter(pl.col("Tables").str.contains("Eye Color"))
+    sentences = sentences.with_row_count()
+    details = details.with_row_count()
+    inmate = inmate.select(
+        [
+            pl.lit(name).alias("Name"),
+            pl.col("Tables").str.extract(r'AIS:\s+(\d{8})').alias("AIS"),
+            pl.col("Tables").str.extract(r'Institution: ([A-Z\s]+)').alias("Institution"
+             ),
+            pl.col("Tables").str.extract(r'Race: ([A-Z])').alias("Race"),
+            pl.col("Tables").str.extract(r'Sex: ([A-Z])').alias("Sex"),
+            pl.col("Tables").str.extract(r'Hair Color: ([A-Z]+)').alias("HairColor"),
+            pl.col("Tables").str.extract(r'Eye Color: ([A-Z]+)').alias("EyeColor"),
+            pl.col("Tables").str.extract(r'Height: (.+)').alias("Height"),
+            pl.col("Tables").str.extract(r'Weight: (\d+)').alias("Weight"),
+            pl.col("Tables").str.extract(r'Birth Year: (\d\d\d\d)').alias("BirthYear"),
+            pl.col("Tables").str.extract(r'Custody (.+)').alias("Custody")
+        ]
+    )
+    sentences = sentences.with_columns(pl.col("Tables").str.split('\n'))
+    sentences = sentences.explode("Tables")
+    sentences = sentences.filter(pl.col("Tables").str.contains("[A-Z]"))
+    sentences = sentences.filter(pl.col("Tables").str.contains("Sentenced").is_not())
+    sentences = sentences.unique()
+    sentences = sentences.select(
+        [
+            pl.col("row_nr"),
+            pl.col("Tables").str.extract(r'([^\s]+)').alias("CaseNo"),
+            pl.col("Tables").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("Sentenced"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d (.+?) \d+Y \d+M \d+D').alias("Offense"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? (\d+Y \d+M \d+D)').alias("Term"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D (\d+)').cast(pl.Int64, strict=False).alias("SentenceJailCredit"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D \d+ \d* ?(C?o?n?c?u?r?r?e?n?t?)').alias("Type"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D \d+ \d* ?C?o?n?c?u?r?r?e?n?t? ?([A-Z]+)').alias("County")
+        ]
+    )
+    sentences = sentences.with_columns(
+        [
+            pl.when(pl.col("Type")=="C")
+            .then("")
+            .otherwise(pl.col("Type"))
+            .alias("Type"),
+            pl.when(pl.col("Type")=="C")
+            .then(pl.concat_str([pl.lit("C"),pl.col("County")]))
+            .otherwise(pl.col("County"))
+            .alias("County")
+        ]
+    )
+    details = details.with_columns(pl.col("Tables").str.split("\n"))
+    details = details.explode("Tables")
+    details = details.filter(pl.col("Tables").str.contains("Admit Date").is_not())
+    details = details.filter(pl.col("Tables").str.contains("[A-Z]"))
+    details = details.select(
+        [
+            pl.col("row_nr"),
+            pl.col("Tables").str.extract(r'^([A-Z])').alias("SUF"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?(\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("AdmitDate"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d (\d+Y \d+M \d+D)').alias("TotalTerm"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D (\d+Y \d+M \d+D)').alias("TimeServed"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D (\d+)').alias("JailCredit"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?(\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D?)').str.replace(r'Days .+','Days').alias("GoodTimeReceived"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?(\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D?)').str.replace(r'^\d Days','').str.replace(r'^\d+Y \d+M \d+D','').str.replace(r'Days .+','Days').str.strip().alias("GoodTimeRevoked"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("MinReleaseDate"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? \d\d/\d\d/\d\d\d\d (\d?\d?/?\d?\d?/?\d?\d?\d?\d?)').str.to_date('%m/%d/%Y', strict=False).alias("ParoleConsiderationDate"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? \d\d/\d\d/\d\d\d\d \d?\d?/?\d?\d?/?\d?\d?\d?\d? (.+)').str.strip().alias("ParoleStatus")
+        ]
+    )
+    sentences = sentences.join(details, how="left", on="row_nr")
+    sentences = sentences.with_columns(pl.lit(0).alias("Match"))
+    inmate = inmate.with_columns(pl.lit(0).alias("Match"))
+    sentences = sentences.join(inmate, how="left", on="Match").select(pl.exclude("Match", "row_nr"))
+    sentences = sentences.select("CaseNo","Name","AIS","Institution","Race","Sex","HairColor","EyeColor","Height","Weight","BirthYear","Custody","Sentenced","Offense","Term","SentenceJailCredit","Type","County","SUF","AdmitDate","TotalTerm","TimeServed","JailCredit","GoodTimeReceived","GoodTimeRevoked","MinReleaseDate","ParoleConsiderationDate","ParoleStatus")
+    return sentences
+
+
+def crawl_adoc(path, window=None):
+    alphabet = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
+    print("Connecting to ADOC...")
+    driver = webdriver.Chrome()
+    driver.get("http://www.doc.state.al.us/inmatesearch")
+    results = []
+    if not window:
+        for x in tqdm(alphabet):
+            last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
+            last_name_box.send_keys(x)
+            driver.implicitly_wait(1)
+            send_button = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearch")
+            send_button.click()
+            driver.implicitly_wait(1)
+            more_results = True
+            try:
+                while more_results:
+                    driver.implicitly_wait(1)
+                    lists = driver.find_elements(by=By.TAG_NAME, value="tr")
+                    for x in lists:
+                        results += [x.text]
+                        print(x.text)
+                    try:
+                        current_page = driver.find_element(by=By.ID, value="MainContent_gvInmateResults_lblCurrent")
+                        total_pages = driver.find_element(by=By.ID, value='MainContent_gvInmateResults_lblPages')
+                    except:
+                        more_results = False
+                        search_again = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearchAgain")
+                        search_again.click()
+                    if int(current_page.text) == int(total_pages.text):
+                        more_results = False
+                        search_again = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearchAgain")
+                        search_again.click()
+                    else:
+                        next_button = driver.find_element(by=By.ID, value="MainContent_gvInmateResults_btnNext")
+                        next_button.click()
+            except:
+                time.sleep(2)
+                driver.get("http://www.doc.state.al.us/inmatesearch")
+
+            out = pl.DataFrame({'Rows': results})
+            out = out.filter(pl.col("Rows").str.contains("Inmate").is_not())
+            out = out.filter(pl.col("Rows").str.contains("Pages").is_not())
+            out = out.select(
+                [
+                    pl.col("Rows").str.extract(r'^([0-9Z]{8})').alias("AIS"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} ([A-Z]+, [A-Z\s]+?) \w \w \d\d\d\d').alias("Name"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? (\w) \w \d\d\d\d').alias("Race"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w (\w) \d\d\d\d').alias("Sex"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w (\d\d\d\d)').alias("YOB").cast(pl.Int64, strict=False),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d ([A-Z\s]+)').str.strip().alias("Institution"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d [A-Z\s]+ (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("ReleaseDate")
+                ]
+            )
+            print(out)
+            write(out, sheet_names=['inmates'], path=path, overwrite=True)
+    if window:
+        window.write_event_value("PROGRESS-TEXT", 0)
+        window.write_event_value("PROGRESS-TEXT-TOTAL", len(alphabet))
+        for i, x in enumerate(alphabet):
+            last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
+            last_name_box.send_keys(x)
+            driver.implicitly_wait(1)
+            send_button = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearch")
+            send_button.click()
+            driver.implicitly_wait(1)
+            more_results = True
+            try:
+                while more_results:
+                    driver.implicitly_wait(1)
+                    lists = driver.find_elements(by=By.TAG_NAME, value="tr")
+                    for x in lists:
+                        results += [x.text]
+                        print(x.text)
+                    try:
+                        current_page = driver.find_element(by=By.ID, value="MainContent_gvInmateResults_lblCurrent")
+                        total_pages = driver.find_element(by=By.ID, value='MainContent_gvInmateResults_lblPages')
+                    except:
+                        more_results = False
+                        search_again = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearchAgain")
+                        search_again.click()
+                    if int(current_page.text) == int(total_pages.text):
+                        more_results = False
+                        search_again = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearchAgain")
+                        search_again.click()
+                    else:
+                        next_button = driver.find_element(by=By.ID, value="MainContent_gvInmateResults_btnNext")
+                        next_button.click()
+            except:
+                time.sleep(2)
+                driver.get("http://www.doc.state.al.us/inmatesearch")
+
+            out = pl.DataFrame({'Rows': results})
+            out = out.filter(pl.col("Rows").str.contains("Inmate").is_not())
+            out = out.filter(pl.col("Rows").str.contains("Pages").is_not())
+            out = out.select(
+                [
+                    pl.col("Rows").str.extract(r'^([0-9Z]{8})').alias("AIS"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} ([A-Z]+, [A-Z\s]+?) \w \w \d\d\d\d').alias("Name"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? (\w) \w \d\d\d\d').alias("Race"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w (\w) \d\d\d\d').alias("Sex"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w (\d\d\d\d)').alias("YOB").cast(pl.Int64, strict=False),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d ([A-Z\s]+)').str.strip().alias("Institution"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d [A-Z\s]+ (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("ReleaseDate")
+                ]
+            )
+            window.write_event_value("PROGRESS-TEXT", i + 1)
+            write(out, sheet_names=['inmates'], path=path, overwrite=True)
+    return out
+
+
+def adoc_missing_cases(adoc_df, cases_df):
+    if isinstance(adoc_df, str):
+        adoc_df = read(adoc_df)
+    if isinstance(cases_df, str):
+        cases_df = set(cases_df, table="cases", now=True)
+    cmap = pl.DataFrame(
+        {
+            'Selection': ['94 - ARDMORE', '93 - ATHENS', '04 - AUTAUGA', '05 - BALDWIN', '06 - BARBOUR - CLAYTON', '69 - BARBOUR - EUFAULA', '89 - BERRY', '07 - BIBB', '08 - BLOUNT', '87 - BRUNDIDGE MUNICIPAL COURT', '09 - BULLOCK', '10 - BUTLER', '11 - CALHOUN', '12 - CHAMBERS', '13 - CHEROKEE', '90 - CHEROKEE', '14 - CHILTON', '15 - CHOCTAW', '16 - CLARKE', '17 - CLAY', '18 - CLEBURNE', '19 - COFFEE - ELBA', '71 - COFFEE - ENTERPRISE', '20 - COLBERT', '21 - CONECUH', '22 - COOSA', '23 - COVINGTON', '24 - CRENSHAW', '25 - CULLMAN', '26 - DALE', '27 - DALLAS', '28 - DeKALB', '29 - ELMORE', '30 - ESCAMBIA', '31 - ETOWAH', '32 - FAYETTE', '33 - FRANKLIN', '34 - GENEVA', '35 - GREENE', '36 - HALE', '37 - HENRY', '38 - HOUSTON', '39 - JACKSON', '68 - JEFFERSON - BESSEMER', '01 - JEFFERSON - BIRMINGHAM', '40 - LAMAR', '41 - LAUDERDALE', '42 - LAWRENCE', '43 - LEE', '44 - LIMESTONE', '82 - LIVINGSTON', '45 - LOWNDES', '46 - MACON', '47 - MADISON', '48 - MARENGO', '49 - MARION', '50 - MARSHALL', '92 - MILLBROOK', '02 - MOBILE', '51 - MONROE', '03 - MONTGOMERY', '52 - MORGAN', '53 - PERRY', '80 - PHENIX CITY', '54 - PICKENS', '55 - PIKE', '88 - PRATTVILLE', '56 - RANDOLPH', '57 - RUSSELL', '58 - SHELBY', '59 - ST. CLAIR - ASHVILLE', '75 - ST. CLAIR - PELL CITY', '81 - SUMITON MUNICIPAL COURT', '60 - SUMTER', '74 - TALLADEGA - SYLACAUGA', '61 - TALLADEGA - TALLADEGA', '70 - TALLAPOOSA - ALEX CITY', '62 - TALLAPOOSA - DADEVILLE', '63 - TUSCALOOSA', '64 - WALKER', '65 - WASHINGTON', '95 - WETUMPKA MUNICIPAL COURT', '66 - WILCOX', '67 - WINSTON'],
+            'CountyNumber': ['94', '93', '04', '05', '06', '69', '89', '07', '08', '87', '09', '10', '11', '12', '13', '90', '14', '15', '16', '17', '18', '19', '71', '20', '21', '22', '23', '24', '25', '26', '27', '28', '29', '30', '31', '32', '33', '34', '35', '36', '37', '38', '39', '68', '01', '40', '41', '42', '43', '44', '82', '45', '46', '47', '48', '49', '50', '92', '02', '51', '03', '52', '53', '80', '54', '55', '88', '56', '57', '58', '59', '75', '81', '60', '74', '61', '70', '62', '63', '64', '65', '95', '66', '67'],
+            'County': ['ARDMORE', 'ATHENS', 'AUTAUGA', 'BALDWIN', 'BARBOUR - CLAYTON', 'BARBOUR - EUFAULA', 'BERRY', 'BIBB', 'BLOUNT', 'BRUNDIDGE MUNICIPAL COURT', 'BULLOCK', 'BUTLER', 'CALHOUN', 'CHAMBERS', 'CHEROKEE', 'CHEROKEE', 'CHILTON', 'CHOCTAW', 'CLARKE', 'CLAY', 'CLEBURNE', 'COFFEE - ELBA', 'COFFEE - ENTERPRISE', 'COLBERT', 'CONECUH', 'COOSA', 'COVINGTON', 'CRENSHAW', 'CULLMAN', 'DALE', 'DALLAS', 'DeKALB', 'ELMORE', 'ESCAMBIA', 'ETOWAH', 'FAYETTE', 'FRANKLIN', 'GENEVA', 'GREENE', 'HALE', 'HENRY', 'HOUSTON', 'JACKSON', 'JEFFERSON - BESSEMER', 'JEFFERSON - BIRMINGHAM', 'LAMAR', 'LAUDERDALE', 'LAWRENCE', 'LEE', 'LIMESTONE', 'LIVINGSTON', 'LOWNDES', 'MACON', 'MADISON', 'MARENGO', 'MARION', 'MARSHALL', 'MILLBROOK', 'MOBILE', 'MONROE', 'MONTGOMERY', 'MORGAN', 'PERRY', 'PHENIX CITY', 'PICKENS', 'PIKE', 'PRATTVILLE', 'RANDOLPH', 'RUSSELL', 'SHELBY', 'ST. CLAIR - ASHVILLE', 'ST. CLAIR - PELL CITY', 'SUMITON MUNICIPAL COURT', 'SUMTER', 'TALLADEGA - SYLACAUGA', 'TALLADEGA - TALLADEGA', 'TALLAPOOSA - ALEX CITY', 'TALLAPOOSA - DADEVILLE', 'TUSCALOOSA', 'WALKER', 'WASHINGTON', 'WETUMPKA MUNICIPAL COURT', 'WILCOX', 'WINSTON'] 
+        }
+    )
+    adoc_df = adoc_df.join(cmap, on="County", how="left")
+    adoc_df = adoc_df.with_columns(
+        pl.concat_str(
+            [
+                pl.col("CountyNumber"),
+                pl.lit("-"),
+                pl.col("CaseNo").str.extract(r'^(\w\w)'),
+                pl.lit("-"),
+                pl.col("CaseNo").str.extract(r'(\d\d\d\d)\-'),
+                pl.lit("-"),
+                pl.col("CaseNo").str.extract(r'\-(\d\d\d\d\d\d)')
+            ]
+        ).alias("CaseNumber")
+    )
+    cn = cases_df.select(pl.col("CaseNumber").str.extract(r'([^\.]+)')).to_series().to_list()
+    adoc_df = adoc_df.filter(pl.col("CaseNumber").is_in(cn).is_not())
+    adoc_df = adoc_df.filter(pl.col("CaseNumber").is_null().is_not())
+    adoc_df = adoc_df.unique("CaseNumber")
+    return adoc_df.select(pl.exclude("CaseNumber","CountyNumber"))
+
 
 #   #   #   #      GRAPHICAL USER INTERFACE    #   #   #   #
 
 
 def loadgui():
     """
     Load PySimpleGUI tk graphical interface
@@ -4114,15 +4330,18 @@
                 size=[26, 10],
                 key="SQ-OUTPUTPATH",
             ),
             sg.FolderBrowse(
                 button_text="Select Folder", button_color=("white", "black")
             ),
         ],
-        [sg.Checkbox('Criminal Only', key="SQ-CRIMINALONLY", default=False)],
+        [
+            sg.Checkbox('Criminal Only', key="SQ-CRIMINALONLY", default=False),
+            sg.Checkbox('Search by Case Number', key='SQ-CASENUMBER', default=False)
+        ],
         [sg.Text("Alacourt.com Credentials", font=BODY_FONT)],
         [
             sg.Text("Customer ID: "),
             sg.Input(key="SQ-CUSTOMERID", size=(16, 1)),
         ],
         [
             sg.Text("User ID:"),
@@ -4139,14 +4358,91 @@
                 button_color=("white", "black"),
                 pad=(10, 10),
                 disabled_button_color=("grey", "black"),
                 bind_return_key=True,
             )
         ],
     ]
+    adoc_layout = [
+        [
+            sg.Text(
+                """Retrieve sentencing info from ADOC Inmate\nSearch.""",
+                font=HEADER_FONT,
+                pad=(5,5)
+            )
+        ],
+        [sg.Text(">> crawl", font=LOGO_FONT, pad=(5,5))],
+        [
+            sg.Text(
+                """Retrieve ADOC Inmate Search's full list of current inmates.""",
+                pad=(2, 2),
+            )
+        ],
+        [
+            sg.Text("Output Path: "),
+            sg.InputText(
+                tooltip="Output spreadsheet file path (.xlsx, .parquet, .json, .csv)",
+                size=[41, 1],
+                key="CRAWL-OUTPUTPATH",
+            ),
+        ],
+        [
+            sg.Button(
+                "Crawl ADOC",
+                button_color=("white", "black"),
+                key="CRAWL",
+                enable_events=True,
+                bind_return_key=True,
+                disabled_button_color=("grey", "black"),
+                pad=(10, 10),
+            )
+        ],
+        [sg.Text(">> fetch", font=LOGO_FONT, pad=(2,2))],
+        [
+            sg.Text(
+                """Retrieve ADOC Inmate Search results from query spreadsheet with AIS, \nFirstName, and LastName columns.""",
+                pad=(5, 5),
+            )
+        ],
+        [
+            sg.Text("Input Path: "),
+            sg.InputText(
+                tooltip="Query template (.xlsx)",
+                size=[22, 10],
+                key="ADOC-FETCH-INPUTPATH",
+                focus=True,
+            ),
+            sg.FileBrowse(button_text="Select File", button_color=("white", "black")),
+            sg.Button(
+                button_text="New Query",
+                button_color=("white", "black"),
+                k="ADOC-FETCH-NEWQUERY",
+                enable_events=True,
+            ),
+        ],
+        [
+            sg.Text("Output Path: "),
+            sg.InputText(
+                tooltip="Output spreadsheet file path (.xlsx, .parquet, .json, .csv)",
+                size=[41, 1],
+                key="ADOC-FETCH-OUTPUTPATH",
+            ),
+        ],
+        [
+            sg.Button(
+                "Search ADOC",
+                button_color=("white", "black"),
+                key="FETCH-ADOC",
+                enable_events=True,
+                bind_return_key=True,
+                disabled_button_color=("grey", "black"),
+                pad=(10, 10),
+            )
+        ],
+    ]
     archive_layout = [
         [
             sg.Text(
                 """Create full text archives from a directory\nof PDF cases.""",
                 font=HEADER_FONT,
                 pad=(5, 5),
             )
@@ -4443,14 +4739,15 @@
         layout=[
             [sg.Tab("fetch", layout=fetch_layout, pad=(2, 2))],
             [sg.Tab("archive", layout=archive_layout, pad=(2, 2))],
             [sg.Tab("table", layout=table_layout, pad=(2, 2))],
             [sg.Tab("pair", layout=sum_layout, pad=(2, 2))],
             [sg.Tab("rename", layout=rename_layout, pad=(2, 2))],
             [sg.Tab("append", layout=append_layout, pad=(2, 2))],
+            [sg.Tab("adoc", layout=adoc_layout, pad=(2, 2))],
             [sg.Tab("about", layout=about_layout, pad=(2, 2))],
         ],
     )
     layout = [
         [sg.Text("ALACORDER", font=LOGO_FONT, pad=(5, 5))],
         [tabs],
         [
@@ -4638,38 +4935,53 @@
         elif event == "SQ":
             if (
                 window["SQ-INPUTPATH"].get() == ""
                 or window["SQ-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
                 continue
-            try:
-                pwd = window["SQ-PASSWORD"].get()
-                window["SQ"].update(disabled=True)
-                thread = threading.Thread(
-                    target=fetch,
-                    args=(
-                        window["SQ-INPUTPATH"].get(),
-                        window["SQ-OUTPUTPATH"].get(),
-                        window["SQ-CUSTOMERID"].get(),
-                        window["SQ-USERID"].get(),
-                        pwd,
-                        window["SQ-CRIMINALONLY"].get(),
-                        None,
-                        False,
-                        False,
-                        window,
-                    ),
-                    daemon=True,
-                ).start()
-                continue
-            except:
-                print("Check configuration and try again.")
-                window["SQ"].update(disabled=False)
-                continue
+            if window["SQ-CASENUMBER"].get():
+                try:
+                    window["SQ"].update(disabled=True)
+                    driver = start_alacourt_driver(window["SQ-CUSTOMERID"].get(), window["SQ-USERID"].get(), window["SQ-PASSWORD"].get(), window["SQ-OUTPUTPATH"].get())
+                    thread = threading.Thread(
+                        target=fetch_by_case_numbers,
+                        args=(window["SQ-INPUTPATH"].get(), driver, window),
+                        daemon=True
+                    ).start()
+                    continue
+                except:
+                    print("Check configuration and try again.")
+                    window["SQ"].update(disabled=False)
+                    continue
+            else:
+                try:
+                    pwd = window["SQ-PASSWORD"].get()
+                    window["SQ"].update(disabled=True)
+                    thread = threading.Thread(
+                        target=fetch,
+                        args=(
+                            window["SQ-INPUTPATH"].get(),
+                            window["SQ-OUTPUTPATH"].get(),
+                            window["SQ-CUSTOMERID"].get(),
+                            window["SQ-USERID"].get(),
+                            pwd,
+                            window["SQ-CRIMINALONLY"].get(),
+                            None,
+                            False,
+                            False,
+                            window,
+                        ),
+                        daemon=True,
+                    ).start()
+                    continue
+                except:
+                    print("Check configuration and try again.")
+                    window["SQ"].update(disabled=False)
+                    continue
         elif event == "AA":
             if (
                 window["AA-INPUTPATH"].get() == ""
                 or window["AA-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
                 continue
@@ -4698,14 +5010,33 @@
                 window["RN"].update(disabled=True)
                 thread = threading.Thread(
                     target=rename_pdfs,
                     args=[cf],
                     daemon=True,
                 ).start()
                 continue
+        elif event == "CRAWL":
+            if window["CRAWL-OUTPUTPATH"].get() == "":
+                sg.popup("Enter valid path and try again.")
+                continue
+            window["CRAWL"].update(disabled=True)
+            thread = threading.Thread(
+                target=crawl_adoc,
+                args=(window["CRAWL-OUTPUTPATH"].get(), window),
+                daemon=True
+            ).start()
+        elif event == "FETCH-ADOC":
+            if window["ADOC-FETCH-INPUTPATH"].get() == '' or window["ADOC-FETCH-OUTPUTPATH"].get() == '':
+                sg.popup("Enter valid path and try again.")
+            window["FETCH-ADOC"].update(disabled=True)
+            thread = threading.Thread(
+                target=adoc_fetch,
+                args=(window["ADOC-FETCH-INPUTPATH"].get(), window["ADOC-FETCH-OUTPUTPATH"].get(), window),
+                daemon=True
+            ).start()
         else:
             pass
 
 
 #   #   #   #       COMMAND LINE INTERFACE     #   #   #   #
 
 
@@ -4723,15 +5054,45 @@
         loadgui()
 
 
 @main.command(name="start", help="Launch graphical user interface")
 def _cli_start():
     loadgui()
 
-@main.command(name="search-adoc", help="Retrieve records from ADOC Inmate Search")
+@main.command(name="missing", help="Identify cases missing in archive from adoc-fetch results")
+@click.option(
+    "--adoc-input",
+    "-in",
+    "adoc",
+    required=True,
+    prompt="Path to ADOC results spreadsheet",
+    help="Path to ADOC results spreadsheet from `adoc-fetch`",
+    type=click.Path()
+)
+@click.option(
+    "--archive-input",
+    "-arc",
+    "archive",
+    required=True,
+    prompt="Path to archive to check for missing cases",
+    help="Path to archive to check for missing cases"
+)
+@click.option(
+    "--output-path",
+    "-out",
+    "output",
+    required=True,
+    prompt="Path to output spreadsheet",
+    help="Path to output spreadsheet"
+)
+def _cli_missing(adoc, archive, output):
+    mc = adoc_missing_cases(adoc, archive)
+    write(mc, sheet_names=["missing"], path=output)
+
+@main.command(name="adoc-fetch", help="Retrieve records from ADOC Inmate Search")
 @click.option(
     "--input-path",
     "-query",
     "query",
     required=True,
     prompt="Path to query spreadsheet",
     help="Path to query spreadsheet",
@@ -4794,28 +5155,28 @@
     Returns:
         DataFrame: Appended archive
     """
     arc = append_archive(in_path, out_path)
     print("Completed task.")
     return arc
 
-@main.command(name="crawl-adoc", help="Retrieve current inmates list from ADOC")
+@main.command(name="adoc-crawl", help="Retrieve current inmates list from ADOC")
 @click.option(
     "--path",
     "-out",
     "path",
     required=True,
     prompt="Output table path",
     help="Path to output table",
     type=click.Path()
 )
 def _cli_crawl(path):
     crawl_adoc(path)
 
-@main.command(name="fetch", help="Fetch cases from Alacourt.com")
+@main.command(name="fetch", help="Fetch cases from Alacourt.com by party search")
 @click.option(
     "--input-path",
     "-in",
     "querypath",
     required=True,
     prompt="Path to query table",
     help="Path to query table/spreadsheet (.xls, .xlsx)",
@@ -6075,14 +6436,62 @@
         overwrite=overwrite,
         log=True,
     )
     p = pairs(conf)
     print("Created pair template at output path.")
     return p
 
+@main.command(name="fetch-cn", help="Fetch cases from Alacourt.com by case number")
+@click.option(
+    "--input-path",
+    "-in",
+    "query",
+    required=True,
+    type=click.Path(),
+    prompt="Query spreadsheet input",
+    help="Query spreadsheet with CaseNo or CaseNumber column"
+)
+@click.option(
+    "--output-path",
+    "-out",
+    "dirpath",
+    required=True,
+    type=click.Path(),
+    prompt="PDF downloads directory",
+    help="Directory to download PDFs to"
+)
+@click.option(
+    "--customer-id",
+    "-c",
+    "cID",
+    required=True,
+    prompt="Alacourt Customer ID",
+    help="Customer ID on Alacourt.com",
+)
+@click.option(
+    "--user-id",
+    "-u",
+    "uID",
+    required=True,
+    prompt="Alacourt User ID",
+    help="User ID on Alacourt.com",
+)
+@click.option(
+    "--password",
+    "-p",
+    "pwd",
+    required=True,
+    prompt="Alacourt Password",
+    help="Password on Alacourt.com",
+    hide_input=True,
+)
+def _cli_fetch_by_case_number(query, dirpath, cID, uID, pwd):
+    driver = start_alacourt_driver(cID, uID, pwd, dirpath)
+    return fetch_by_case_numbers(query, driver)
+
 
 @main.command(
     name="vrr-pairs", help="Create voting rights summary from input cases and pairs"
 )
 @click.option(
     "--input-path",
     "-in",
@@ -6129,14 +6538,15 @@
     )
     return vrr_summary(conf)
 
 
 if __name__ == "__main__":
     main()
 
+
 #   #   #   #           GETTER METHODS         #   #   #   #
 
 
 def get_paths(dirpath):
     """
     From path-like `dirpath`, return list of paths to pdfs in directory
     """
@@ -6566,14 +6976,15 @@
             .rstrip("S")
             .rstrip("P")
             .strip()
         )
     except:
         return ""
 
+
 def getArrestingAgencyType(text):
     try:
         out = re.search(r"([^0-9]+) Arresting Agency Type:", str(text)).group(1)
     except:
         return ''
     out = re.sub(r"^\-.+", "", out)
     out = re.sub(r"County\:", "", out)
@@ -7211,26 +7622,29 @@
             ", ".join(
                 re.findall(r"Probation Begin Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             ),
         ).strip(), '%m/%d/%Y')
     except:
         return None
 
+
 def getProbationPeriod(text):
     try:
         return re.search(r"Probation Period\: (\d+ Years, \d+ Months, \d+ Days\.)", str(text)).group(1)
     except:
         return ''
 
+
 def getLicenseSuspPeriod(text):
     try:
         return re.search(r"License Susp Period\: (\d+ Years, \d+ Months, \d+ Days\.)", str(text)).group(1)
     except:
         return ''
 
+
 def getProbationRevoke(text):
     try:
         return re.sub(
             r"(Probation Revoke:)",
             "",
             ", ".join(
                 re.findall(r"Probation Revoke: (\d\d?/\d\d?/\d\d\d\d)", str(text))
@@ -7318,65 +7732,67 @@
         out = re.sub(r"Time\:", "", out, re.DOTALL)
         out = re.sub(r"Description\:", "", out, re.DOTALL)
         out = re.sub(r"Court Action", "", out, re.DOTALL)
         return out.strip()
     else:
         return ""
 
+
 def getBalanceByFeeCode(text, code):
     pat = f"(ACTIVE[^\n]+{code}[^\n]+)"
     rows = re.findall(pat, text)
     tot = 0.0
     for r in rows:
         splr = re.findall(r"\$\d+\.\d{2}", r)
         if len(splr) > 0:
             bal = float(re.sub(r'\$','',splr[-1]))
             tot += bal
     if len(rows) == 0:
         return None
     if len(rows) > 0:
         return tot
 
+
 def getAmtDueByFeeCode(text, code):
     pat = f"(ACTIVE[^\n]+{code}[^\n]+)"
     rows = re.findall(pat, text)
     tot = 0.0
     for r in rows:
         splr = re.findall(r"\$\d+\.\d{2}", r)
         if len(splr) > 0:
             bal = float(re.sub(r'\$','',splr[0]))
             tot += bal
     if len(rows) == 0:
         return None
     if len(rows) > 0:
         return tot
 
+
 def getAmtPaidByFeeCode(text, code):
     pat = f"(ACTIVE[^\n]+{code}[^\n]+)"
     rows = re.findall(pat, text)
     tot = 0.0
     for r in rows:
         splr = re.findall(r"\$\d+\.\d{2}", r)
         if len(splr) > 0:
             bal = float(re.sub(r'\$','',splr[1]))
             tot += bal
     if len(rows) == 0:
         return None
     if len(rows) > 0:
         return tot
 
+
 def getAmtHoldByFeeCode(text, code):
     pat = f"(ACTIVE[^\n]+{code}[^\n]+)"
     rows = re.findall(pat, text)
     tot = 0.0
     for r in rows:
         splr = re.findall(r"\$\d+\.\d{2}", r)
         if len(splr) > 0:
             bal = float(re.sub(r'\$','',splr[2]))
             tot += bal
     if len(rows) == 0:
         return None
     if len(rows) > 0:
         return tot
 
-
-
```

### Comparing `alacorder-80.8.0/src/alacorder/alac.py` & `alacorder-80.8.1/src/alacorder/alac.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.8.0"
+version = "80.8.1"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3272,266 +3272,14 @@
         return query
     else:
         print(
             "Try again with at least one valid column header: [NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, NO_RECORDS, FILED_BEFORE, FILED_AFTER, RETRIEVED, CASES_FOUND, QUERY_COMPLETE]"
         )
         return None
 
-
-def make_fetch_queue_from_crawl(df):
-    if isinstance(df, str):
-        df = read(df)
-    df = df.select(
-        [
-            pl.col("AIS"),
-            pl.col("Name").str.extract(r', ([A-Z]+)').alias("FirstName"),
-            pl.col("Name").str.extract(r'^([A-Z]+)').alias("LastName"),
-        ]
-    )
-    return df
-
-def adoc_fetch(df=None, path=None, cf=None):
-    if cf:
-        df = read(cf['INPUTS'])
-        path = cf['OUTPUT_PATH']
-    if df:
-        if isinstance(df, str):
-            dfpath = df
-            df = read(df)
-        else:
-            dfpath = None
-    if 'Retrieved' not in df.columns:
-        df = df.select("AIS", "FirstName", "LastName")
-        df = df.with_columns(pl.lit("").alias("Retrieved"))
-    df = df.with_columns(pl.col("AIS").cast(pl.Utf8, strict=False))
-    out = pl.DataFrame()
-    driver = webdriver.Chrome()
-    for i, r in enumerate(tqdm(df.rows(named=True))):
-        if r['Retrieved'] != '' and r['Retrieved'] != None:
-            continue
-        try:
-            out = pl.concat([out, read_top_result(driver, r['AIS'], r['FirstName'], r['LastName'])])
-        except:
-            pass
-        df[i, 'Retrieved'] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
-        if dfpath and df.shape[0] > 10 and i % 10 == 0:
-            write(df, sheet_names=["adoc_progress"], path=dfpath)
-        if df.shape[0] > 10 and i % 10 == 0 and path:
-            write(out, sheet_names=["adoc"], path=path)
-    if path:
-        write(out, sheet_names=["adoc"], path=path)
-    if dfpath:
-        write(df, sheet_names=["adoc_progress"], path=dfpath)
-    return out, df
-
-def read_top_result(driver, ais, first, last):
-    driver.get("http://www.doc.state.al.us/inmatesearch")
-    ais_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtAIS")
-    first_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtFName")
-    last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
-    send_button = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearch")
-    ais_box.send_keys(ais)
-    first_name_box.send_keys(first)
-    last_name_box.send_keys(last)
-    send_button.click()
-    urls = driver.find_elements(by=By.TAG_NAME, value="a")
-    results = []
-    for x in urls:
-        try:
-            if 'InmateResults' in x.get_attribute("ID"):
-                results += [x]
-        except:
-            pass
-    try:
-        results[0].click()
-        return read_adoc_page(driver)
-    except:
-        return pl.DataFrame()
-
-
-def filter_missing_cases(adoc_df, cases_df):
-    if isinstance(adoc_df, str):
-        adoc_df = read(adoc_df)
-    if isinstance(cases_df, str):
-        cases_df = read(cases_df)
-    if 'AllPagesText' in cases_df.columns:
-        cases_df = set(cases_df, table="cases", now=True)
-    cases_df = cases_df.with_columns(
-        pl.col("CaseNumber").str.extract(r'(\w\w-\d\d\d\d-\d\d\d\d\d\d)').alias("CaseNoFragment")
-    )
-    clist = cases_df.select("CaseNoFragment").to_series().to_list()
-    cmap = pl.DataFrame(
-        {
-            'Selection': ['94 - ARDMORE', '93 - ATHENS', '04 - AUTAUGA', '05 - BALDWIN', '06 - BARBOUR - CLAYTON', '69 - BARBOUR - EUFAULA', '89 - BERRY', '07 - BIBB', '08 - BLOUNT', '87 - BRUNDIDGE MUNICIPAL COURT', '09 - BULLOCK', '10 - BUTLER', '11 - CALHOUN', '12 - CHAMBERS', '13 - CHEROKEE', '90 - CHEROKEE', '14 - CHILTON', '15 - CHOCTAW', '16 - CLARKE', '17 - CLAY', '18 - CLEBURNE', '19 - COFFEE - ELBA', '71 - COFFEE - ENTERPRISE', '20 - COLBERT', '21 - CONECUH', '22 - COOSA', '23 - COVINGTON', '24 - CRENSHAW', '25 - CULLMAN', '26 - DALE', '27 - DALLAS', '28 - DeKALB', '29 - ELMORE', '30 - ESCAMBIA', '31 - ETOWAH', '32 - FAYETTE', '33 - FRANKLIN', '34 - GENEVA', '35 - GREENE', '36 - HALE', '37 - HENRY', '38 - HOUSTON', '39 - JACKSON', '68 - JEFFERSON - BESSEMER', '01 - JEFFERSON - BIRMINGHAM', '40 - LAMAR', '41 - LAUDERDALE', '42 - LAWRENCE', '43 - LEE', '44 - LIMESTONE', '82 - LIVINGSTON', '45 - LOWNDES', '46 - MACON', '47 - MADISON', '48 - MARENGO', '49 - MARION', '50 - MARSHALL', '92 - MILLBROOK', '02 - MOBILE', '51 - MONROE', '03 - MONTGOMERY', '52 - MORGAN', '53 - PERRY', '80 - PHENIX CITY', '54 - PICKENS', '55 - PIKE', '88 - PRATTVILLE', '56 - RANDOLPH', '57 - RUSSELL', '58 - SHELBY', '59 - ST. CLAIR - ASHVILLE', '75 - ST. CLAIR - PELL CITY', '81 - SUMITON MUNICIPAL COURT', '60 - SUMTER', '74 - TALLADEGA - SYLACAUGA', '61 - TALLADEGA - TALLADEGA', '70 - TALLAPOOSA - ALEX CITY', '62 - TALLAPOOSA - DADEVILLE', '63 - TUSCALOOSA', '64 - WALKER', '65 - WASHINGTON', '95 - WETUMPKA MUNICIPAL COURT', '66 - WILCOX', '67 - WINSTON'],
-            'CountyNumber': ['94', '93', '04', '05', '06', '69', '89', '07', '08', '87', '09', '10', '11', '12', '13', '90', '14', '15', '16', '17', '18', '19', '71', '20', '21', '22', '23', '24', '25', '26', '27', '28', '29', '30', '31', '32', '33', '34', '35', '36', '37', '38', '39', '68', '01', '40', '41', '42', '43', '44', '82', '45', '46', '47', '48', '49', '50', '92', '02', '51', '03', '52', '53', '80', '54', '55', '88', '56', '57', '58', '59', '75', '81', '60', '74', '61', '70', '62', '63', '64', '65', '95', '66', '67'],
-            'County': ['ARDMORE', 'ATHENS', 'AUTAUGA', 'BALDWIN', 'BARBOUR - CLAYTON', 'BARBOUR - EUFAULA', 'BERRY', 'BIBB', 'BLOUNT', 'BRUNDIDGE MUNICIPAL COURT', 'BULLOCK', 'BUTLER', 'CALHOUN', 'CHAMBERS', 'CHEROKEE', 'CHEROKEE', 'CHILTON', 'CHOCTAW', 'CLARKE', 'CLAY', 'CLEBURNE', 'COFFEE - ELBA', 'COFFEE - ENTERPRISE', 'COLBERT', 'CONECUH', 'COOSA', 'COVINGTON', 'CRENSHAW', 'CULLMAN', 'DALE', 'DALLAS', 'DeKALB', 'ELMORE', 'ESCAMBIA', 'ETOWAH', 'FAYETTE', 'FRANKLIN', 'GENEVA', 'GREENE', 'HALE', 'HENRY', 'HOUSTON', 'JACKSON', 'JEFFERSON - BESSEMER', 'JEFFERSON - BIRMINGHAM', 'LAMAR', 'LAUDERDALE', 'LAWRENCE', 'LEE', 'LIMESTONE', 'LIVINGSTON', 'LOWNDES', 'MACON', 'MADISON', 'MARENGO', 'MARION', 'MARSHALL', 'MILLBROOK', 'MOBILE', 'MONROE', 'MONTGOMERY', 'MORGAN', 'PERRY', 'PHENIX CITY', 'PICKENS', 'PIKE', 'PRATTVILLE', 'RANDOLPH', 'RUSSELL', 'SHELBY', 'ST. CLAIR - ASHVILLE', 'ST. CLAIR - PELL CITY', 'SUMITON MUNICIPAL COURT', 'SUMTER', 'TALLADEGA - SYLACAUGA', 'TALLADEGA - TALLADEGA', 'TALLAPOOSA - ALEX CITY', 'TALLAPOOSA - DADEVILLE', 'TUSCALOOSA', 'WALKER', 'WASHINGTON', 'WETUMPKA MUNICIPAL COURT', 'WILCOX', 'WINSTON'] 
-        }
-    )
-    adoc_df = adoc_df.join(cmap, on="County", how="left")
-    adoc_df = adoc_df.with_columns(
-        pl.concat_str(
-            [
-                pl.col("CountyNumber"),
-                pl.lit("-"),
-                pl.col("CaseNo").str.extract(r"(\w\w)"),
-                pl.lit("-"),
-                pl.col("CaseNo").str.extract(r'(\d\d\d\d)\-'),
-                pl.lit("-"),
-                pl.col("CaseNo").str.extract(r'\-(\d\d\d\d\d\d)'),
-            ]
-        ).alias("CaseNoFragment")
-    )
-    out = adoc_df.filter(pl.col("CaseNoFragment").is_in(clist).is_not())
-    out = out.filter(pl.col("CaseNoFragment").is_null().is_not())
-    return out
-
-def read_adoc_page(driver):
-    rl = driver.find_elements(by=By.TAG_NAME, value="tr")
-    alltxt = []
-    for r in rl:
-        alltxt += [r.text]
-    name = driver.find_element(by=By.ID, value="MainContent_DetailsView2_Label1").text
-    allt = pl.DataFrame({'Tables': "\n".join(alltxt)})
-    allt = allt.with_columns(pl.col("Tables").str.split("SUF"))
-    allt = allt.explode("Tables")
-    allt = allt.with_columns(pl.col("Tables").str.split("Sentences"))
-    allt = allt.explode("Tables")
-    details = allt.filter(pl.col("Tables").str.contains("Date Total Term"))
-    sentences = allt.filter(pl.col("Tables").str.contains("Sentenced"))
-    inmate = allt.filter(pl.col("Tables").str.contains("Eye Color"))
-    sentences = sentences.with_row_count()
-    details = details.with_row_count()
-    inmate = inmate.select(
-        [
-            pl.lit(name).alias("Name"),
-            pl.col("Tables").str.extract(r'AIS:\s+(\d{8})').alias("AIS"),
-            pl.col("Tables").str.extract(r'Institution: ([A-Z\s]+)').alias("Institution"
-             ),
-            pl.col("Tables").str.extract(r'Race: ([A-Z])').alias("Race"),
-            pl.col("Tables").str.extract(r'Sex: ([A-Z])').alias("Sex"),
-            pl.col("Tables").str.extract(r'Hair Color: ([A-Z]+)').alias("HairColor"),
-            pl.col("Tables").str.extract(r'Eye Color: ([A-Z]+)').alias("EyeColor"),
-            pl.col("Tables").str.extract(r'Height: (.+)').alias("Height"),
-            pl.col("Tables").str.extract(r'Weight: (\d+)').alias("Weight"),
-            pl.col("Tables").str.extract(r'Birth Year: (\d\d\d\d)').alias("BirthYear"),
-            pl.col("Tables").str.extract(r'Custody (.+)').alias("Custody")
-        ]
-    )
-    sentences = sentences.with_columns(pl.col("Tables").str.split('\n'))
-    sentences = sentences.explode("Tables")
-    sentences = sentences.filter(pl.col("Tables").str.contains("[A-Z]"))
-    sentences = sentences.filter(pl.col("Tables").str.contains("Sentenced").is_not())
-    sentences = sentences.unique()
-    sentences = sentences.select(
-        [
-            pl.col("row_nr"),
-            pl.col("Tables").str.extract(r'([^\s]+)').alias("CaseNo"),
-            pl.col("Tables").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("Sentenced"),
-            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d (.+?) \d+Y \d+M \d+D').alias("Offense"),
-            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? (\d+Y \d+M \d+D)').alias("Term"),
-            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D (\d+)').cast(pl.Int64, strict=False).alias("SentenceJailCredit"),
-            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D \d+ \d* ?(C?o?n?c?u?r?r?e?n?t?)').alias("Type"),
-            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D \d+ \d* ?C?o?n?c?u?r?r?e?n?t? ?([A-Z]+)').alias("County")
-        ]
-    )
-    sentences = sentences.with_columns(
-        [
-            pl.when(pl.col("Type")=="C")
-            .then("")
-            .otherwise(pl.col("Type"))
-            .alias("Type"),
-            pl.when(pl.col("Type")=="C")
-            .then(pl.concat_str([pl.lit("C"),pl.col("County")]))
-            .otherwise(pl.col("County"))
-            .alias("County")
-        ]
-    )
-    details = details.with_columns(pl.col("Tables").str.split("\n"))
-    details = details.explode("Tables")
-    details = details.filter(pl.col("Tables").str.contains("Admit Date").is_not())
-    details = details.filter(pl.col("Tables").str.contains("[A-Z]"))
-    details = details.select(
-        [
-            pl.col("row_nr"),
-            pl.col("Tables").str.extract(r'^([A-Z])').alias("SUF"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?(\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("AdmitDate"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d (\d+Y \d+M \d+D)').alias("TotalTerm"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D (\d+Y \d+M \d+D)').alias("TimeServed"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D (\d+)').alias("JailCredit"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?(\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D?)').str.replace(r'Days .+','Days').alias("GoodTimeReceived"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?(\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D?)').str.replace(r'^\d Days','').str.replace(r'^\d+Y \d+M \d+D','').str.replace(r'Days .+','Days').str.strip().alias("GoodTimeRevoked"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("MinReleaseDate"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? \d\d/\d\d/\d\d\d\d (\d?\d?/?\d?\d?/?\d?\d?\d?\d?)').str.to_date('%m/%d/%Y', strict=False).alias("ParoleConsiderationDate"),
-            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? \d\d/\d\d/\d\d\d\d \d?\d?/?\d?\d?/?\d?\d?\d?\d? (.+)').str.strip().alias("ParoleStatus")
-        ]
-    )
-    sentences = sentences.join(details, how="left", on="row_nr")
-    sentences = sentences.with_columns(pl.lit(0).alias("Match"))
-    inmate = inmate.with_columns(pl.lit(0).alias("Match"))
-    sentences = sentences.join(inmate, how="left", on="Match").select(pl.exclude("Match", "row_nr"))
-    sentences = sentences.select("CaseNo","Name","AIS","Institution","Race","Sex","HairColor","EyeColor","Height","Weight","BirthYear","Custody","Sentenced","Offense","Term","SentenceJailCredit","Type","County","SUF","AdmitDate","TotalTerm","TimeServed","JailCredit","GoodTimeReceived","GoodTimeRevoked","MinReleaseDate","ParoleConsiderationDate","ParoleStatus")
-    return sentences
-
-def crawl_adoc(path):
-    alphabet = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
-    print("Connecting to ADOC...")
-    driver = webdriver.Chrome()
-    driver.get("http://www.doc.state.al.us/inmatesearch")
-    results = []
-    for x in alphabet:
-        last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
-        last_name_box.send_keys(x)
-        driver.implicitly_wait(1)
-        send_button = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearch")
-        send_button.click()
-        driver.implicitly_wait(1)
-        more_results = True
-        try:
-            while more_results:
-                driver.implicitly_wait(1)
-                lists = driver.find_elements(by=By.TAG_NAME, value="tr")
-                for x in lists:
-                    results += [x.text]
-                    print(x.text)
-                try:
-                    current_page = driver.find_element(by=By.ID, value="MainContent_gvInmateResults_lblCurrent")
-                    total_pages = driver.find_element(by=By.ID, value='MainContent_gvInmateResults_lblPages')
-                except:
-                    more_results = False
-                    search_again = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearchAgain")
-                    search_again.click()
-                if int(current_page.text) == int(total_pages.text):
-                    more_results = False
-                    search_again = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearchAgain")
-                    search_again.click()
-                else:
-                    next_button = driver.find_element(by=By.ID, value="MainContent_gvInmateResults_btnNext")
-                    next_button.click()
-        except:
-            time.sleep(2)
-            driver.get("http://www.doc.state.al.us/inmatesearch")
-
-        out = pl.DataFrame({'Rows': results})
-        out = out.filter(pl.col("Rows").str.contains("Inmate").is_not())
-        out = out.filter(pl.col("Rows").str.contains("Pages").is_not())
-        out = out.select(
-            [
-                pl.col("Rows").str.extract(r'^([0-9Z]{8})').alias("AIS"),
-                pl.col("Rows").str.extract(r'^[0-9Z]{8} ([A-Z]+, [A-Z\s]+?) \w \w \d\d\d\d').alias("Name"),
-                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? (\w) \w \d\d\d\d').alias("Race"),
-                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w (\w) \d\d\d\d').alias("Sex"),
-                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w (\d\d\d\d)').alias("YOB").cast(pl.Int64, strict=False),
-                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d ([A-Z\s]+)').str.strip().alias("Institution"),
-                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d [A-Z\s]+ (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("ReleaseDate")
-            ]
-        )
-        print(out)
-        write(out, sheet_names=['inmates'], path=path, overwrite=True)
-    return out
-
 def fetch(
     querypath="",
     dirpath="",
     cID="",
     uID="",
     pwd="",
     criminal_only=False,
@@ -3970,14 +3718,156 @@
     driver.get("https://v2.alacourt.com/frmIndexSearchForm.aspx")
 
     print("Successfully connected and logged into Alacourt!")
 
     return driver
 
 
+def start_alacourt_driver(cID, uID, pwd, dirpath=None):
+    opt = webdriver.ChromeOptions()
+    if dirpath:
+        opt.add_experimental_option(
+            "prefs",
+            {
+                "download.default_directory": dirpath,  # Set default directory for downloads
+                "download.prompt_for_download": False,  # To auto download the file
+                "download.directory_upgrade": True,
+                "plugins.always_open_pdf_externally": True,  # Don't display PDF in chrome
+            },
+        )
+    else:
+        opt.add_experimental_option(
+            "prefs",
+            {
+                "download.prompt_for_download": False,  # To auto download the file
+                "download.directory_upgrade": True,
+                "plugins.always_open_pdf_externally": True,  # Don't display PDF in chrome
+            },
+        )
+    print("Starting browser... Do not close while in progress!")
+    driver = webdriver.Chrome(options=opt)
+    login(driver, cID=cID, uID=uID, pwd=pwd)
+    return driver
+
+
+def case_number_search(case_number, driver):
+    driver.get("https://v2.alacourt.com/frmcaselookupform.aspx")
+    county_select = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCounty")
+    division_select = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlDivision")
+    case_year_select = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCaseYear")
+    case_number_input = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtCaseNumber")
+    case_extension_select = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlExt")
+    number_of_cases_select = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlNumberOfCases")
+    cmap = pl.DataFrame(
+        {
+            'Selection': ['94 - ARDMORE', '93 - ATHENS', '04 - AUTAUGA', '05 - BALDWIN', '06 - BARBOUR - CLAYTON', '69 - BARBOUR - EUFAULA', '89 - BERRY', '07 - BIBB', '08 - BLOUNT', '87 - BRUNDIDGE MUNICIPAL COURT', '09 - BULLOCK', '10 - BUTLER', '11 - CALHOUN', '12 - CHAMBERS', '13 - CHEROKEE', '90 - CHEROKEE', '14 - CHILTON', '15 - CHOCTAW', '16 - CLARKE', '17 - CLAY', '18 - CLEBURNE', '19 - COFFEE - ELBA', '71 - COFFEE - ENTERPRISE', '20 - COLBERT', '21 - CONECUH', '22 - COOSA', '23 - COVINGTON', '24 - CRENSHAW', '25 - CULLMAN', '26 - DALE', '27 - DALLAS', '28 - DeKALB', '29 - ELMORE', '30 - ESCAMBIA', '31 - ETOWAH', '32 - FAYETTE', '33 - FRANKLIN', '34 - GENEVA', '35 - GREENE', '36 - HALE', '37 - HENRY', '38 - HOUSTON', '39 - JACKSON', '68 - JEFFERSON - BESSEMER', '01 - JEFFERSON - BIRMINGHAM', '40 - LAMAR', '41 - LAUDERDALE', '42 - LAWRENCE', '43 - LEE', '44 - LIMESTONE', '82 - LIVINGSTON', '45 - LOWNDES', '46 - MACON', '47 - MADISON', '48 - MARENGO', '49 - MARION', '50 - MARSHALL', '92 - MILLBROOK', '02 - MOBILE', '51 - MONROE', '03 - MONTGOMERY', '52 - MORGAN', '53 - PERRY', '80 - PHENIX CITY', '54 - PICKENS', '55 - PIKE', '88 - PRATTVILLE', '56 - RANDOLPH', '57 - RUSSELL', '58 - SHELBY', '59 - ST. CLAIR - ASHVILLE', '75 - ST. CLAIR - PELL CITY', '81 - SUMITON MUNICIPAL COURT', '60 - SUMTER', '74 - TALLADEGA - SYLACAUGA', '61 - TALLADEGA - TALLADEGA', '70 - TALLAPOOSA - ALEX CITY', '62 - TALLAPOOSA - DADEVILLE', '63 - TUSCALOOSA', '64 - WALKER', '65 - WASHINGTON', '95 - WETUMPKA MUNICIPAL COURT', '66 - WILCOX', '67 - WINSTON'],
+            'CountyNumber': ['94', '93', '04', '05', '06', '69', '89', '07', '08', '87', '09', '10', '11', '12', '13', '90', '14', '15', '16', '17', '18', '19', '71', '20', '21', '22', '23', '24', '25', '26', '27', '28', '29', '30', '31', '32', '33', '34', '35', '36', '37', '38', '39', '68', '01', '40', '41', '42', '43', '44', '82', '45', '46', '47', '48', '49', '50', '92', '02', '51', '03', '52', '53', '80', '54', '55', '88', '56', '57', '58', '59', '75', '81', '60', '74', '61', '70', '62', '63', '64', '65', '95', '66', '67'],
+            'County': ['ARDMORE', 'ATHENS', 'AUTAUGA', 'BALDWIN', 'BARBOUR - CLAYTON', 'BARBOUR - EUFAULA', 'BERRY', 'BIBB', 'BLOUNT', 'BRUNDIDGE MUNICIPAL COURT', 'BULLOCK', 'BUTLER', 'CALHOUN', 'CHAMBERS', 'CHEROKEE', 'CHEROKEE', 'CHILTON', 'CHOCTAW', 'CLARKE', 'CLAY', 'CLEBURNE', 'COFFEE - ELBA', 'COFFEE - ENTERPRISE', 'COLBERT', 'CONECUH', 'COOSA', 'COVINGTON', 'CRENSHAW', 'CULLMAN', 'DALE', 'DALLAS', 'DeKALB', 'ELMORE', 'ESCAMBIA', 'ETOWAH', 'FAYETTE', 'FRANKLIN', 'GENEVA', 'GREENE', 'HALE', 'HENRY', 'HOUSTON', 'JACKSON', 'JEFFERSON - BESSEMER', 'JEFFERSON - BIRMINGHAM', 'LAMAR', 'LAUDERDALE', 'LAWRENCE', 'LEE', 'LIMESTONE', 'LIVINGSTON', 'LOWNDES', 'MACON', 'MADISON', 'MARENGO', 'MARION', 'MARSHALL', 'MILLBROOK', 'MOBILE', 'MONROE', 'MONTGOMERY', 'MORGAN', 'PERRY', 'PHENIX CITY', 'PICKENS', 'PIKE', 'PRATTVILLE', 'RANDOLPH', 'RUSSELL', 'SHELBY', 'ST. CLAIR - ASHVILLE', 'ST. CLAIR - PELL CITY', 'SUMITON MUNICIPAL COURT', 'SUMTER', 'TALLADEGA - SYLACAUGA', 'TALLADEGA - TALLADEGA', 'TALLAPOOSA - ALEX CITY', 'TALLAPOOSA - DADEVILLE', 'TUSCALOOSA', 'WALKER', 'WASHINGTON', 'WETUMPKA MUNICIPAL COURT', 'WILCOX', 'WINSTON'] 
+        }
+    )
+    dmap = pl.DataFrame({'Code': ['CC', 'CS', 'CV', 'DC', 'DR', 'DV', 'EQ', 'JU', 'MC', 'SM', 'TP', 'TR'], 'Selection': ['CC - CIRCUIT-CRIMINAL', 'CS - CHILD SUPPORT', 'CV - CIRCUIT-CIVIL', 'DC - DISTRICT-CRIMINAL', 'DR - DOMESTIC RELATIONS', 'DV - DISTRICT-CIVIL', 'EQ - EQUITY-CASES', 'JU - JUVENILE', 'MC - MUNICIPAL-CRIMINAL', 'SM - SMALL CLAIMS', 'TP - MUNICIPAL-PARKING', 'TR - TRAFFIC'] })
+    county_number = case_number[0:2]
+    division_code = case_number[3:5]
+    case_year = case_number[6:10]
+    six_digit = case_number[11:17]
+    if len(case_number) >= 20:
+        extension = case_number[18:20]
+    else:
+        extension = "00"
+    county = cmap.filter(pl.col("CountyNumber")==county_number).select("Selection").to_series()[0]
+    division = dmap.filter(pl.col("Code")==division_code).select("Selection").to_series()[0]
+    county_select.send_keys(county)
+    division_select.send_keys(division)
+    case_year_select.send_keys(case_year)
+    case_number_input.send_keys(six_digit)
+    search_button = driver.find_element(by=By.ID, value="searchButton")
+    search_button.click()
+    try:
+        driver.implicitly_wait(1)
+        driver.find_element(by=By.ID, value="Label2")
+    except:
+        try:
+            driver.implicitly_wait(1)
+            driver.find_element(by=By.ID, value="ContentPlaceHolder1_lnkPrint").click()
+            driver.implicitly_wait(1)
+            driver.find_element(by=By.ID, value="btnPrintCase").click()
+        except:
+            try:
+                time.sleep(1)
+                driver.implicitly_wait(1)
+                driver.find_element(by=By.ID, value="ContentPlaceHolder1_lnkPrint").click()
+                driver.implicitly_wait(1)
+                time.sleep(1)
+                driver.find_element(by=By.ID, value="btnPrintCase").click()
+            except:
+                pass
+
+
+def fetch_by_case_numbers(df, driver, window):
+    if isinstance(df, str):
+        dfpath = df
+        df = read(df)
+    else:
+        dfpath = None
+    if 'CountyNumber' in df.columns:
+        df = df.select(pl.exclude("CountyNumber"))
+    cmap = pl.DataFrame(
+        {
+            'Selection': ['94 - ARDMORE', '93 - ATHENS', '04 - AUTAUGA', '05 - BALDWIN', '06 - BARBOUR - CLAYTON', '69 - BARBOUR - EUFAULA', '89 - BERRY', '07 - BIBB', '08 - BLOUNT', '87 - BRUNDIDGE MUNICIPAL COURT', '09 - BULLOCK', '10 - BUTLER', '11 - CALHOUN', '12 - CHAMBERS', '13 - CHEROKEE', '90 - CHEROKEE', '14 - CHILTON', '15 - CHOCTAW', '16 - CLARKE', '17 - CLAY', '18 - CLEBURNE', '19 - COFFEE - ELBA', '71 - COFFEE - ENTERPRISE', '20 - COLBERT', '21 - CONECUH', '22 - COOSA', '23 - COVINGTON', '24 - CRENSHAW', '25 - CULLMAN', '26 - DALE', '27 - DALLAS', '28 - DeKALB', '29 - ELMORE', '30 - ESCAMBIA', '31 - ETOWAH', '32 - FAYETTE', '33 - FRANKLIN', '34 - GENEVA', '35 - GREENE', '36 - HALE', '37 - HENRY', '38 - HOUSTON', '39 - JACKSON', '68 - JEFFERSON - BESSEMER', '01 - JEFFERSON - BIRMINGHAM', '40 - LAMAR', '41 - LAUDERDALE', '42 - LAWRENCE', '43 - LEE', '44 - LIMESTONE', '82 - LIVINGSTON', '45 - LOWNDES', '46 - MACON', '47 - MADISON', '48 - MARENGO', '49 - MARION', '50 - MARSHALL', '92 - MILLBROOK', '02 - MOBILE', '51 - MONROE', '03 - MONTGOMERY', '52 - MORGAN', '53 - PERRY', '80 - PHENIX CITY', '54 - PICKENS', '55 - PIKE', '88 - PRATTVILLE', '56 - RANDOLPH', '57 - RUSSELL', '58 - SHELBY', '59 - ST. CLAIR - ASHVILLE', '75 - ST. CLAIR - PELL CITY', '81 - SUMITON MUNICIPAL COURT', '60 - SUMTER', '74 - TALLADEGA - SYLACAUGA', '61 - TALLADEGA - TALLADEGA', '70 - TALLAPOOSA - ALEX CITY', '62 - TALLAPOOSA - DADEVILLE', '63 - TUSCALOOSA', '64 - WALKER', '65 - WASHINGTON', '95 - WETUMPKA MUNICIPAL COURT', '66 - WILCOX', '67 - WINSTON'],
+            'CountyNumber': ['94', '93', '04', '05', '06', '69', '89', '07', '08', '87', '09', '10', '11', '12', '13', '90', '14', '15', '16', '17', '18', '19', '71', '20', '21', '22', '23', '24', '25', '26', '27', '28', '29', '30', '31', '32', '33', '34', '35', '36', '37', '38', '39', '68', '01', '40', '41', '42', '43', '44', '82', '45', '46', '47', '48', '49', '50', '92', '02', '51', '03', '52', '53', '80', '54', '55', '88', '56', '57', '58', '59', '75', '81', '60', '74', '61', '70', '62', '63', '64', '65', '95', '66', '67'],
+            'County': ['ARDMORE', 'ATHENS', 'AUTAUGA', 'BALDWIN', 'BARBOUR - CLAYTON', 'BARBOUR - EUFAULA', 'BERRY', 'BIBB', 'BLOUNT', 'BRUNDIDGE MUNICIPAL COURT', 'BULLOCK', 'BUTLER', 'CALHOUN', 'CHAMBERS', 'CHEROKEE', 'CHEROKEE', 'CHILTON', 'CHOCTAW', 'CLARKE', 'CLAY', 'CLEBURNE', 'COFFEE - ELBA', 'COFFEE - ENTERPRISE', 'COLBERT', 'CONECUH', 'COOSA', 'COVINGTON', 'CRENSHAW', 'CULLMAN', 'DALE', 'DALLAS', 'DeKALB', 'ELMORE', 'ESCAMBIA', 'ETOWAH', 'FAYETTE', 'FRANKLIN', 'GENEVA', 'GREENE', 'HALE', 'HENRY', 'HOUSTON', 'JACKSON', 'JEFFERSON - BESSEMER', 'JEFFERSON - BIRMINGHAM', 'LAMAR', 'LAUDERDALE', 'LAWRENCE', 'LEE', 'LIMESTONE', 'LIVINGSTON', 'LOWNDES', 'MACON', 'MADISON', 'MARENGO', 'MARION', 'MARSHALL', 'MILLBROOK', 'MOBILE', 'MONROE', 'MONTGOMERY', 'MORGAN', 'PERRY', 'PHENIX CITY', 'PICKENS', 'PIKE', 'PRATTVILLE', 'RANDOLPH', 'RUSSELL', 'SHELBY', 'ST. CLAIR - ASHVILLE', 'ST. CLAIR - PELL CITY', 'SUMITON MUNICIPAL COURT', 'SUMTER', 'TALLADEGA - SYLACAUGA', 'TALLADEGA - TALLADEGA', 'TALLAPOOSA - ALEX CITY', 'TALLAPOOSA - DADEVILLE', 'TUSCALOOSA', 'WALKER', 'WASHINGTON', 'WETUMPKA MUNICIPAL COURT', 'WILCOX', 'WINSTON'] 
+        }
+    )
+    df = df.join(cmap, on="County", how="left")
+    if 'Selection_right' in df.columns:
+        df = df.select(pl.exclude("Selection_right"))
+    if "CaseNo" in df.columns and "CaseNumber" not in df.columns:
+        df = df.with_columns(
+            pl.concat_str(
+                [
+                    pl.col("CountyNumber"),
+                    pl.lit("-"),
+                    pl.col("CaseNo").str.extract(r'^(\w\w)'),
+                    pl.lit("-"),
+                    pl.col("CaseNo").str.extract(r'(\d\d\d\d)\-'),
+                    pl.lit("-"),
+                    pl.col("CaseNo").str.extract(r'\-(\d\d\d\d\d\d)')
+                ]
+            ).alias("CaseNumber")
+    )
+    if 'Retrieved' not in df.columns:
+        df = df.with_columns(pl.lit("").alias("Retrieved"))
+    if not window:
+        for i, r in enumerate(tqdm(df.rows(named=True))):
+            if r['CaseNumber'] == '' or r['CaseNumber'] == None:
+                continue
+            if r['Retrieved'] != '' and r['Retrieved'] != None:
+                continue
+            case_number_search(r['CaseNumber'], driver)
+            df[i, 'Retrieved'] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
+            if dfpath and i % 10 == 0:
+                write(df.select(pl.exclude("CountyNumber", "Selection")), sheet_names=["adoc"], path=dfpath, overwrite=True)
+    if window:
+        window.write_event_value("PROGRESS-TEXT", 0)
+        window.write_event_value("PROGRESS-TEXT-TOTAL", len(df.rows()))
+        for i, r in enumerate(df.rows(named=True)):
+            if r['CaseNumber'] == '' or r['CaseNumber'] == None:
+                continue
+            if r['Retrieved'] != '' and r['Retrieved'] != None:
+                continue
+            case_number_search(r['CaseNumber'], driver)
+            df[i, 'Retrieved'] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
+            window.write_event_value("PROGRESS-TEXT", i + 1)
+            if dfpath and i % 10 == 0:
+                write(df.select(pl.exclude("CountyNumber", "Selection")), sheet_names=["adoc"], path=dfpath, overwrite=True)
+        window.write_event_value("FETCH-CN-COMPLETE", True)
+    write(df, sheet_names=["adoc"], path=dfpath, overwrite=True)
+    return df.select(pl.exclude("CountyNumber", "Selection"))
+
+
 def empty_query(path):
     """Create empty spreadsheet to fill and import as query submit search list to retrieve matching case records from Alacourt.com.
 
     Args:
         path (str): Desired output path (.xls, .xlsx)
 
     """
@@ -3997,14 +3887,340 @@
                 "RETRIEVED": [],
                 "CASES_FOUND": []
             }
     )
     return write(empty, sheet_names="query", path=path, overwrite=True)
 
 
+#   #   #   #        ADOC INMATE SEARCH        #   #   #   #
+
+
+def make_adoc_fetch_queue_from_crawl(df):
+    if isinstance(df, str):
+        df = read(df)
+    df = df.select(
+        [
+            pl.col("AIS"),
+            pl.col("Name").str.extract(r', ([A-Z]+)').alias("FirstName"),
+            pl.col("Name").str.extract(r'^([A-Z]+)').alias("LastName"),
+        ]
+    )
+    return df
+
+
+def adoc_fetch(df=None, path=None, window=None, cf=None):
+    if cf:
+        df = read(cf['INPUTS'])
+        path = cf['OUTPUT_PATH']
+    if df:
+        if isinstance(df, str):
+            dfpath = df
+            df = read(df)
+        else:
+            dfpath = None
+    if 'FirstName' not in df.columns or 'LastName' not in df.columns:
+        df = make_adoc_fetch_queue_from_crawl(df)
+    if 'Retrieved' not in df.columns:
+        df = df.with_columns(pl.lit("").alias("Retrieved"))
+    df = df.with_columns(pl.col("AIS").cast(pl.Utf8, strict=False))
+    out = pl.DataFrame()
+    driver = webdriver.Chrome()
+    if not window:
+        for i, r in enumerate(tqdm(df.rows(named=True))):
+            if r['Retrieved'] != '' and r['Retrieved'] != None:
+                continue
+            try:
+                out = pl.concat([out, read_adoc_top_result(driver, r['AIS'], r['FirstName'], r['LastName'])])
+            except:
+                pass
+            df[i, 'Retrieved'] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
+            if dfpath and df.shape[0] > 10 and i % 10 == 0:
+                write(df, sheet_names=["adoc_progress"], path=dfpath)
+            if df.shape[0] > 10 and i % 10 == 0 and path:
+                write(out, sheet_names=["adoc"], path=path)
+    if window:
+        window.write_event_value("PROGRESS-TEXT", 0)
+        window.write_event_value("PROGRESS-TEXT-TOTAL", df.shape[0])
+        for i, r in enumerate(df.rows(named=True)):
+            if r['Retrieved'] != '' and r['Retrieved'] != None:
+                continue
+            try:
+                out = pl.concat([out, read_adoc_top_result(driver, r['AIS'], r['FirstName'], r['LastName'])])
+            except:
+                pass
+            df[i, 'Retrieved'] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
+            window.write_event_value("PROGRESS-TEXT", i + 1)
+            if dfpath and df.shape[0] > 10 and i % 10 == 0:
+                write(df, sheet_names=["adoc_progress"], path=dfpath)
+            if df.shape[0] > 10 and i % 10 == 0 and path:
+                write(out, sheet_names=["adoc"], path=path)
+        window.write_event_value("ADOC-FETCH-COMPLETE", True)
+    if path:
+        write(out, sheet_names=["adoc"], path=path)
+    if dfpath:
+        write(df, sheet_names=["adoc_progress"], path=dfpath)
+    return out, df
+
+
+def read_adoc_top_result(driver, ais, first, last):
+    driver.get("http://www.doc.state.al.us/inmatesearch")
+    ais_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtAIS")
+    first_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtFName")
+    last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
+    send_button = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearch")
+    ais_box.send_keys(ais)
+    first_name_box.send_keys(first)
+    last_name_box.send_keys(last)
+    send_button.click()
+    urls = driver.find_elements(by=By.TAG_NAME, value="a")
+    results = []
+    for x in urls:
+        try:
+            if 'InmateResults' in x.get_attribute("ID"):
+                results += [x]
+        except:
+            pass
+    try:
+        results[0].click()
+        return read_adoc_page(driver)
+    except:
+        return pl.DataFrame()
+
+
+def read_adoc_page(driver):
+    rl = driver.find_elements(by=By.TAG_NAME, value="tr")
+    alltxt = []
+    for r in rl:
+        alltxt += [r.text]
+    name = driver.find_element(by=By.ID, value="MainContent_DetailsView2_Label1").text
+    allt = pl.DataFrame({'Tables': "\n".join(alltxt)})
+    allt = allt.with_columns(pl.col("Tables").str.split("SUF"))
+    allt = allt.explode("Tables")
+    allt = allt.with_columns(pl.col("Tables").str.split("Sentences"))
+    allt = allt.explode("Tables")
+    details = allt.filter(pl.col("Tables").str.contains("Date Total Term"))
+    sentences = allt.filter(pl.col("Tables").str.contains("Sentenced"))
+    inmate = allt.filter(pl.col("Tables").str.contains("Eye Color"))
+    sentences = sentences.with_row_count()
+    details = details.with_row_count()
+    inmate = inmate.select(
+        [
+            pl.lit(name).alias("Name"),
+            pl.col("Tables").str.extract(r'AIS:\s+(\d{8})').alias("AIS"),
+            pl.col("Tables").str.extract(r'Institution: ([A-Z\s]+)').alias("Institution"
+             ),
+            pl.col("Tables").str.extract(r'Race: ([A-Z])').alias("Race"),
+            pl.col("Tables").str.extract(r'Sex: ([A-Z])').alias("Sex"),
+            pl.col("Tables").str.extract(r'Hair Color: ([A-Z]+)').alias("HairColor"),
+            pl.col("Tables").str.extract(r'Eye Color: ([A-Z]+)').alias("EyeColor"),
+            pl.col("Tables").str.extract(r'Height: (.+)').alias("Height"),
+            pl.col("Tables").str.extract(r'Weight: (\d+)').alias("Weight"),
+            pl.col("Tables").str.extract(r'Birth Year: (\d\d\d\d)').alias("BirthYear"),
+            pl.col("Tables").str.extract(r'Custody (.+)').alias("Custody")
+        ]
+    )
+    sentences = sentences.with_columns(pl.col("Tables").str.split('\n'))
+    sentences = sentences.explode("Tables")
+    sentences = sentences.filter(pl.col("Tables").str.contains("[A-Z]"))
+    sentences = sentences.filter(pl.col("Tables").str.contains("Sentenced").is_not())
+    sentences = sentences.unique()
+    sentences = sentences.select(
+        [
+            pl.col("row_nr"),
+            pl.col("Tables").str.extract(r'([^\s]+)').alias("CaseNo"),
+            pl.col("Tables").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("Sentenced"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d (.+?) \d+Y \d+M \d+D').alias("Offense"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? (\d+Y \d+M \d+D)').alias("Term"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D (\d+)').cast(pl.Int64, strict=False).alias("SentenceJailCredit"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D \d+ \d* ?(C?o?n?c?u?r?r?e?n?t?)').alias("Type"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D \d+ \d* ?C?o?n?c?u?r?r?e?n?t? ?([A-Z]+)').alias("County")
+        ]
+    )
+    sentences = sentences.with_columns(
+        [
+            pl.when(pl.col("Type")=="C")
+            .then("")
+            .otherwise(pl.col("Type"))
+            .alias("Type"),
+            pl.when(pl.col("Type")=="C")
+            .then(pl.concat_str([pl.lit("C"),pl.col("County")]))
+            .otherwise(pl.col("County"))
+            .alias("County")
+        ]
+    )
+    details = details.with_columns(pl.col("Tables").str.split("\n"))
+    details = details.explode("Tables")
+    details = details.filter(pl.col("Tables").str.contains("Admit Date").is_not())
+    details = details.filter(pl.col("Tables").str.contains("[A-Z]"))
+    details = details.select(
+        [
+            pl.col("row_nr"),
+            pl.col("Tables").str.extract(r'^([A-Z])').alias("SUF"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?(\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("AdmitDate"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d (\d+Y \d+M \d+D)').alias("TotalTerm"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D (\d+Y \d+M \d+D)').alias("TimeServed"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D (\d+)').alias("JailCredit"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?(\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D?)').str.replace(r'Days .+','Days').alias("GoodTimeReceived"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?(\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D?)').str.replace(r'^\d Days','').str.replace(r'^\d+Y \d+M \d+D','').str.replace(r'Days .+','Days').str.strip().alias("GoodTimeRevoked"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("MinReleaseDate"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? \d\d/\d\d/\d\d\d\d (\d?\d?/?\d?\d?/?\d?\d?\d?\d?)').str.to_date('%m/%d/%Y', strict=False).alias("ParoleConsiderationDate"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? \d\d/\d\d/\d\d\d\d \d?\d?/?\d?\d?/?\d?\d?\d?\d? (.+)').str.strip().alias("ParoleStatus")
+        ]
+    )
+    sentences = sentences.join(details, how="left", on="row_nr")
+    sentences = sentences.with_columns(pl.lit(0).alias("Match"))
+    inmate = inmate.with_columns(pl.lit(0).alias("Match"))
+    sentences = sentences.join(inmate, how="left", on="Match").select(pl.exclude("Match", "row_nr"))
+    sentences = sentences.select("CaseNo","Name","AIS","Institution","Race","Sex","HairColor","EyeColor","Height","Weight","BirthYear","Custody","Sentenced","Offense","Term","SentenceJailCredit","Type","County","SUF","AdmitDate","TotalTerm","TimeServed","JailCredit","GoodTimeReceived","GoodTimeRevoked","MinReleaseDate","ParoleConsiderationDate","ParoleStatus")
+    return sentences
+
+
+def crawl_adoc(path, window=None):
+    alphabet = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
+    print("Connecting to ADOC...")
+    driver = webdriver.Chrome()
+    driver.get("http://www.doc.state.al.us/inmatesearch")
+    results = []
+    if not window:
+        for x in tqdm(alphabet):
+            last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
+            last_name_box.send_keys(x)
+            driver.implicitly_wait(1)
+            send_button = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearch")
+            send_button.click()
+            driver.implicitly_wait(1)
+            more_results = True
+            try:
+                while more_results:
+                    driver.implicitly_wait(1)
+                    lists = driver.find_elements(by=By.TAG_NAME, value="tr")
+                    for x in lists:
+                        results += [x.text]
+                        print(x.text)
+                    try:
+                        current_page = driver.find_element(by=By.ID, value="MainContent_gvInmateResults_lblCurrent")
+                        total_pages = driver.find_element(by=By.ID, value='MainContent_gvInmateResults_lblPages')
+                    except:
+                        more_results = False
+                        search_again = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearchAgain")
+                        search_again.click()
+                    if int(current_page.text) == int(total_pages.text):
+                        more_results = False
+                        search_again = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearchAgain")
+                        search_again.click()
+                    else:
+                        next_button = driver.find_element(by=By.ID, value="MainContent_gvInmateResults_btnNext")
+                        next_button.click()
+            except:
+                time.sleep(2)
+                driver.get("http://www.doc.state.al.us/inmatesearch")
+
+            out = pl.DataFrame({'Rows': results})
+            out = out.filter(pl.col("Rows").str.contains("Inmate").is_not())
+            out = out.filter(pl.col("Rows").str.contains("Pages").is_not())
+            out = out.select(
+                [
+                    pl.col("Rows").str.extract(r'^([0-9Z]{8})').alias("AIS"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} ([A-Z]+, [A-Z\s]+?) \w \w \d\d\d\d').alias("Name"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? (\w) \w \d\d\d\d').alias("Race"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w (\w) \d\d\d\d').alias("Sex"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w (\d\d\d\d)').alias("YOB").cast(pl.Int64, strict=False),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d ([A-Z\s]+)').str.strip().alias("Institution"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d [A-Z\s]+ (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("ReleaseDate")
+                ]
+            )
+            print(out)
+            write(out, sheet_names=['inmates'], path=path, overwrite=True)
+    if window:
+        window.write_event_value("PROGRESS-TEXT", 0)
+        window.write_event_value("PROGRESS-TEXT-TOTAL", len(alphabet))
+        for i, x in enumerate(alphabet):
+            last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
+            last_name_box.send_keys(x)
+            driver.implicitly_wait(1)
+            send_button = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearch")
+            send_button.click()
+            driver.implicitly_wait(1)
+            more_results = True
+            try:
+                while more_results:
+                    driver.implicitly_wait(1)
+                    lists = driver.find_elements(by=By.TAG_NAME, value="tr")
+                    for x in lists:
+                        results += [x.text]
+                        print(x.text)
+                    try:
+                        current_page = driver.find_element(by=By.ID, value="MainContent_gvInmateResults_lblCurrent")
+                        total_pages = driver.find_element(by=By.ID, value='MainContent_gvInmateResults_lblPages')
+                    except:
+                        more_results = False
+                        search_again = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearchAgain")
+                        search_again.click()
+                    if int(current_page.text) == int(total_pages.text):
+                        more_results = False
+                        search_again = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearchAgain")
+                        search_again.click()
+                    else:
+                        next_button = driver.find_element(by=By.ID, value="MainContent_gvInmateResults_btnNext")
+                        next_button.click()
+            except:
+                time.sleep(2)
+                driver.get("http://www.doc.state.al.us/inmatesearch")
+
+            out = pl.DataFrame({'Rows': results})
+            out = out.filter(pl.col("Rows").str.contains("Inmate").is_not())
+            out = out.filter(pl.col("Rows").str.contains("Pages").is_not())
+            out = out.select(
+                [
+                    pl.col("Rows").str.extract(r'^([0-9Z]{8})').alias("AIS"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} ([A-Z]+, [A-Z\s]+?) \w \w \d\d\d\d').alias("Name"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? (\w) \w \d\d\d\d').alias("Race"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w (\w) \d\d\d\d').alias("Sex"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w (\d\d\d\d)').alias("YOB").cast(pl.Int64, strict=False),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d ([A-Z\s]+)').str.strip().alias("Institution"),
+                    pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d [A-Z\s]+ (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("ReleaseDate")
+                ]
+            )
+            window.write_event_value("PROGRESS-TEXT", i + 1)
+            write(out, sheet_names=['inmates'], path=path, overwrite=True)
+    return out
+
+
+def adoc_missing_cases(adoc_df, cases_df):
+    if isinstance(adoc_df, str):
+        adoc_df = read(adoc_df)
+    if isinstance(cases_df, str):
+        cases_df = set(cases_df, table="cases", now=True)
+    cmap = pl.DataFrame(
+        {
+            'Selection': ['94 - ARDMORE', '93 - ATHENS', '04 - AUTAUGA', '05 - BALDWIN', '06 - BARBOUR - CLAYTON', '69 - BARBOUR - EUFAULA', '89 - BERRY', '07 - BIBB', '08 - BLOUNT', '87 - BRUNDIDGE MUNICIPAL COURT', '09 - BULLOCK', '10 - BUTLER', '11 - CALHOUN', '12 - CHAMBERS', '13 - CHEROKEE', '90 - CHEROKEE', '14 - CHILTON', '15 - CHOCTAW', '16 - CLARKE', '17 - CLAY', '18 - CLEBURNE', '19 - COFFEE - ELBA', '71 - COFFEE - ENTERPRISE', '20 - COLBERT', '21 - CONECUH', '22 - COOSA', '23 - COVINGTON', '24 - CRENSHAW', '25 - CULLMAN', '26 - DALE', '27 - DALLAS', '28 - DeKALB', '29 - ELMORE', '30 - ESCAMBIA', '31 - ETOWAH', '32 - FAYETTE', '33 - FRANKLIN', '34 - GENEVA', '35 - GREENE', '36 - HALE', '37 - HENRY', '38 - HOUSTON', '39 - JACKSON', '68 - JEFFERSON - BESSEMER', '01 - JEFFERSON - BIRMINGHAM', '40 - LAMAR', '41 - LAUDERDALE', '42 - LAWRENCE', '43 - LEE', '44 - LIMESTONE', '82 - LIVINGSTON', '45 - LOWNDES', '46 - MACON', '47 - MADISON', '48 - MARENGO', '49 - MARION', '50 - MARSHALL', '92 - MILLBROOK', '02 - MOBILE', '51 - MONROE', '03 - MONTGOMERY', '52 - MORGAN', '53 - PERRY', '80 - PHENIX CITY', '54 - PICKENS', '55 - PIKE', '88 - PRATTVILLE', '56 - RANDOLPH', '57 - RUSSELL', '58 - SHELBY', '59 - ST. CLAIR - ASHVILLE', '75 - ST. CLAIR - PELL CITY', '81 - SUMITON MUNICIPAL COURT', '60 - SUMTER', '74 - TALLADEGA - SYLACAUGA', '61 - TALLADEGA - TALLADEGA', '70 - TALLAPOOSA - ALEX CITY', '62 - TALLAPOOSA - DADEVILLE', '63 - TUSCALOOSA', '64 - WALKER', '65 - WASHINGTON', '95 - WETUMPKA MUNICIPAL COURT', '66 - WILCOX', '67 - WINSTON'],
+            'CountyNumber': ['94', '93', '04', '05', '06', '69', '89', '07', '08', '87', '09', '10', '11', '12', '13', '90', '14', '15', '16', '17', '18', '19', '71', '20', '21', '22', '23', '24', '25', '26', '27', '28', '29', '30', '31', '32', '33', '34', '35', '36', '37', '38', '39', '68', '01', '40', '41', '42', '43', '44', '82', '45', '46', '47', '48', '49', '50', '92', '02', '51', '03', '52', '53', '80', '54', '55', '88', '56', '57', '58', '59', '75', '81', '60', '74', '61', '70', '62', '63', '64', '65', '95', '66', '67'],
+            'County': ['ARDMORE', 'ATHENS', 'AUTAUGA', 'BALDWIN', 'BARBOUR - CLAYTON', 'BARBOUR - EUFAULA', 'BERRY', 'BIBB', 'BLOUNT', 'BRUNDIDGE MUNICIPAL COURT', 'BULLOCK', 'BUTLER', 'CALHOUN', 'CHAMBERS', 'CHEROKEE', 'CHEROKEE', 'CHILTON', 'CHOCTAW', 'CLARKE', 'CLAY', 'CLEBURNE', 'COFFEE - ELBA', 'COFFEE - ENTERPRISE', 'COLBERT', 'CONECUH', 'COOSA', 'COVINGTON', 'CRENSHAW', 'CULLMAN', 'DALE', 'DALLAS', 'DeKALB', 'ELMORE', 'ESCAMBIA', 'ETOWAH', 'FAYETTE', 'FRANKLIN', 'GENEVA', 'GREENE', 'HALE', 'HENRY', 'HOUSTON', 'JACKSON', 'JEFFERSON - BESSEMER', 'JEFFERSON - BIRMINGHAM', 'LAMAR', 'LAUDERDALE', 'LAWRENCE', 'LEE', 'LIMESTONE', 'LIVINGSTON', 'LOWNDES', 'MACON', 'MADISON', 'MARENGO', 'MARION', 'MARSHALL', 'MILLBROOK', 'MOBILE', 'MONROE', 'MONTGOMERY', 'MORGAN', 'PERRY', 'PHENIX CITY', 'PICKENS', 'PIKE', 'PRATTVILLE', 'RANDOLPH', 'RUSSELL', 'SHELBY', 'ST. CLAIR - ASHVILLE', 'ST. CLAIR - PELL CITY', 'SUMITON MUNICIPAL COURT', 'SUMTER', 'TALLADEGA - SYLACAUGA', 'TALLADEGA - TALLADEGA', 'TALLAPOOSA - ALEX CITY', 'TALLAPOOSA - DADEVILLE', 'TUSCALOOSA', 'WALKER', 'WASHINGTON', 'WETUMPKA MUNICIPAL COURT', 'WILCOX', 'WINSTON'] 
+        }
+    )
+    adoc_df = adoc_df.join(cmap, on="County", how="left")
+    adoc_df = adoc_df.with_columns(
+        pl.concat_str(
+            [
+                pl.col("CountyNumber"),
+                pl.lit("-"),
+                pl.col("CaseNo").str.extract(r'^(\w\w)'),
+                pl.lit("-"),
+                pl.col("CaseNo").str.extract(r'(\d\d\d\d)\-'),
+                pl.lit("-"),
+                pl.col("CaseNo").str.extract(r'\-(\d\d\d\d\d\d)')
+            ]
+        ).alias("CaseNumber")
+    )
+    cn = cases_df.select(pl.col("CaseNumber").str.extract(r'([^\.]+)')).to_series().to_list()
+    adoc_df = adoc_df.filter(pl.col("CaseNumber").is_in(cn).is_not())
+    adoc_df = adoc_df.filter(pl.col("CaseNumber").is_null().is_not())
+    adoc_df = adoc_df.unique("CaseNumber")
+    return adoc_df.select(pl.exclude("CaseNumber","CountyNumber"))
+
 
 #   #   #   #      GRAPHICAL USER INTERFACE    #   #   #   #
 
 
 def loadgui():
     """
     Load PySimpleGUI tk graphical interface
@@ -4114,15 +4330,18 @@
                 size=[26, 10],
                 key="SQ-OUTPUTPATH",
             ),
             sg.FolderBrowse(
                 button_text="Select Folder", button_color=("white", "black")
             ),
         ],
-        [sg.Checkbox('Criminal Only', key="SQ-CRIMINALONLY", default=False)],
+        [
+            sg.Checkbox('Criminal Only', key="SQ-CRIMINALONLY", default=False),
+            sg.Checkbox('Search by Case Number', key='SQ-CASENUMBER', default=False)
+        ],
         [sg.Text("Alacourt.com Credentials", font=BODY_FONT)],
         [
             sg.Text("Customer ID: "),
             sg.Input(key="SQ-CUSTOMERID", size=(16, 1)),
         ],
         [
             sg.Text("User ID:"),
@@ -4139,14 +4358,91 @@
                 button_color=("white", "black"),
                 pad=(10, 10),
                 disabled_button_color=("grey", "black"),
                 bind_return_key=True,
             )
         ],
     ]
+    adoc_layout = [
+        [
+            sg.Text(
+                """Retrieve sentencing info from ADOC Inmate\nSearch.""",
+                font=HEADER_FONT,
+                pad=(5,5)
+            )
+        ],
+        [sg.Text(">> crawl", font=LOGO_FONT, pad=(5,5))],
+        [
+            sg.Text(
+                """Retrieve ADOC Inmate Search's full list of current inmates.""",
+                pad=(2, 2),
+            )
+        ],
+        [
+            sg.Text("Output Path: "),
+            sg.InputText(
+                tooltip="Output spreadsheet file path (.xlsx, .parquet, .json, .csv)",
+                size=[41, 1],
+                key="CRAWL-OUTPUTPATH",
+            ),
+        ],
+        [
+            sg.Button(
+                "Crawl ADOC",
+                button_color=("white", "black"),
+                key="CRAWL",
+                enable_events=True,
+                bind_return_key=True,
+                disabled_button_color=("grey", "black"),
+                pad=(10, 10),
+            )
+        ],
+        [sg.Text(">> fetch", font=LOGO_FONT, pad=(2,2))],
+        [
+            sg.Text(
+                """Retrieve ADOC Inmate Search results from query spreadsheet with AIS, \nFirstName, and LastName columns.""",
+                pad=(5, 5),
+            )
+        ],
+        [
+            sg.Text("Input Path: "),
+            sg.InputText(
+                tooltip="Query template (.xlsx)",
+                size=[22, 10],
+                key="ADOC-FETCH-INPUTPATH",
+                focus=True,
+            ),
+            sg.FileBrowse(button_text="Select File", button_color=("white", "black")),
+            sg.Button(
+                button_text="New Query",
+                button_color=("white", "black"),
+                k="ADOC-FETCH-NEWQUERY",
+                enable_events=True,
+            ),
+        ],
+        [
+            sg.Text("Output Path: "),
+            sg.InputText(
+                tooltip="Output spreadsheet file path (.xlsx, .parquet, .json, .csv)",
+                size=[41, 1],
+                key="ADOC-FETCH-OUTPUTPATH",
+            ),
+        ],
+        [
+            sg.Button(
+                "Search ADOC",
+                button_color=("white", "black"),
+                key="FETCH-ADOC",
+                enable_events=True,
+                bind_return_key=True,
+                disabled_button_color=("grey", "black"),
+                pad=(10, 10),
+            )
+        ],
+    ]
     archive_layout = [
         [
             sg.Text(
                 """Create full text archives from a directory\nof PDF cases.""",
                 font=HEADER_FONT,
                 pad=(5, 5),
             )
@@ -4443,14 +4739,15 @@
         layout=[
             [sg.Tab("fetch", layout=fetch_layout, pad=(2, 2))],
             [sg.Tab("archive", layout=archive_layout, pad=(2, 2))],
             [sg.Tab("table", layout=table_layout, pad=(2, 2))],
             [sg.Tab("pair", layout=sum_layout, pad=(2, 2))],
             [sg.Tab("rename", layout=rename_layout, pad=(2, 2))],
             [sg.Tab("append", layout=append_layout, pad=(2, 2))],
+            [sg.Tab("adoc", layout=adoc_layout, pad=(2, 2))],
             [sg.Tab("about", layout=about_layout, pad=(2, 2))],
         ],
     )
     layout = [
         [sg.Text("ALACORDER", font=LOGO_FONT, pad=(5, 5))],
         [tabs],
         [
@@ -4638,38 +4935,53 @@
         elif event == "SQ":
             if (
                 window["SQ-INPUTPATH"].get() == ""
                 or window["SQ-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
                 continue
-            try:
-                pwd = window["SQ-PASSWORD"].get()
-                window["SQ"].update(disabled=True)
-                thread = threading.Thread(
-                    target=fetch,
-                    args=(
-                        window["SQ-INPUTPATH"].get(),
-                        window["SQ-OUTPUTPATH"].get(),
-                        window["SQ-CUSTOMERID"].get(),
-                        window["SQ-USERID"].get(),
-                        pwd,
-                        window["SQ-CRIMINALONLY"].get(),
-                        None,
-                        False,
-                        False,
-                        window,
-                    ),
-                    daemon=True,
-                ).start()
-                continue
-            except:
-                print("Check configuration and try again.")
-                window["SQ"].update(disabled=False)
-                continue
+            if window["SQ-CASENUMBER"].get():
+                try:
+                    window["SQ"].update(disabled=True)
+                    driver = start_alacourt_driver(window["SQ-CUSTOMERID"].get(), window["SQ-USERID"].get(), window["SQ-PASSWORD"].get(), window["SQ-OUTPUTPATH"].get())
+                    thread = threading.Thread(
+                        target=fetch_by_case_numbers,
+                        args=(window["SQ-INPUTPATH"].get(), driver, window),
+                        daemon=True
+                    ).start()
+                    continue
+                except:
+                    print("Check configuration and try again.")
+                    window["SQ"].update(disabled=False)
+                    continue
+            else:
+                try:
+                    pwd = window["SQ-PASSWORD"].get()
+                    window["SQ"].update(disabled=True)
+                    thread = threading.Thread(
+                        target=fetch,
+                        args=(
+                            window["SQ-INPUTPATH"].get(),
+                            window["SQ-OUTPUTPATH"].get(),
+                            window["SQ-CUSTOMERID"].get(),
+                            window["SQ-USERID"].get(),
+                            pwd,
+                            window["SQ-CRIMINALONLY"].get(),
+                            None,
+                            False,
+                            False,
+                            window,
+                        ),
+                        daemon=True,
+                    ).start()
+                    continue
+                except:
+                    print("Check configuration and try again.")
+                    window["SQ"].update(disabled=False)
+                    continue
         elif event == "AA":
             if (
                 window["AA-INPUTPATH"].get() == ""
                 or window["AA-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
                 continue
@@ -4698,14 +5010,33 @@
                 window["RN"].update(disabled=True)
                 thread = threading.Thread(
                     target=rename_pdfs,
                     args=[cf],
                     daemon=True,
                 ).start()
                 continue
+        elif event == "CRAWL":
+            if window["CRAWL-OUTPUTPATH"].get() == "":
+                sg.popup("Enter valid path and try again.")
+                continue
+            window["CRAWL"].update(disabled=True)
+            thread = threading.Thread(
+                target=crawl_adoc,
+                args=(window["CRAWL-OUTPUTPATH"].get(), window),
+                daemon=True
+            ).start()
+        elif event == "FETCH-ADOC":
+            if window["ADOC-FETCH-INPUTPATH"].get() == '' or window["ADOC-FETCH-OUTPUTPATH"].get() == '':
+                sg.popup("Enter valid path and try again.")
+            window["FETCH-ADOC"].update(disabled=True)
+            thread = threading.Thread(
+                target=adoc_fetch,
+                args=(window["ADOC-FETCH-INPUTPATH"].get(), window["ADOC-FETCH-OUTPUTPATH"].get(), window),
+                daemon=True
+            ).start()
         else:
             pass
 
 
 #   #   #   #       COMMAND LINE INTERFACE     #   #   #   #
 
 
@@ -4723,15 +5054,45 @@
         loadgui()
 
 
 @main.command(name="start", help="Launch graphical user interface")
 def _cli_start():
     loadgui()
 
-@main.command(name="search-adoc", help="Retrieve records from ADOC Inmate Search")
+@main.command(name="missing", help="Identify cases missing in archive from adoc-fetch results")
+@click.option(
+    "--adoc-input",
+    "-in",
+    "adoc",
+    required=True,
+    prompt="Path to ADOC results spreadsheet",
+    help="Path to ADOC results spreadsheet from `adoc-fetch`",
+    type=click.Path()
+)
+@click.option(
+    "--archive-input",
+    "-arc",
+    "archive",
+    required=True,
+    prompt="Path to archive to check for missing cases",
+    help="Path to archive to check for missing cases"
+)
+@click.option(
+    "--output-path",
+    "-out",
+    "output",
+    required=True,
+    prompt="Path to output spreadsheet",
+    help="Path to output spreadsheet"
+)
+def _cli_missing(adoc, archive, output):
+    mc = adoc_missing_cases(adoc, archive)
+    write(mc, sheet_names=["missing"], path=output)
+
+@main.command(name="adoc-fetch", help="Retrieve records from ADOC Inmate Search")
 @click.option(
     "--input-path",
     "-query",
     "query",
     required=True,
     prompt="Path to query spreadsheet",
     help="Path to query spreadsheet",
@@ -4794,28 +5155,28 @@
     Returns:
         DataFrame: Appended archive
     """
     arc = append_archive(in_path, out_path)
     print("Completed task.")
     return arc
 
-@main.command(name="crawl-adoc", help="Retrieve current inmates list from ADOC")
+@main.command(name="adoc-crawl", help="Retrieve current inmates list from ADOC")
 @click.option(
     "--path",
     "-out",
     "path",
     required=True,
     prompt="Output table path",
     help="Path to output table",
     type=click.Path()
 )
 def _cli_crawl(path):
     crawl_adoc(path)
 
-@main.command(name="fetch", help="Fetch cases from Alacourt.com")
+@main.command(name="fetch", help="Fetch cases from Alacourt.com by party search")
 @click.option(
     "--input-path",
     "-in",
     "querypath",
     required=True,
     prompt="Path to query table",
     help="Path to query table/spreadsheet (.xls, .xlsx)",
@@ -6075,14 +6436,62 @@
         overwrite=overwrite,
         log=True,
     )
     p = pairs(conf)
     print("Created pair template at output path.")
     return p
 
+@main.command(name="fetch-cn", help="Fetch cases from Alacourt.com by case number")
+@click.option(
+    "--input-path",
+    "-in",
+    "query",
+    required=True,
+    type=click.Path(),
+    prompt="Query spreadsheet input",
+    help="Query spreadsheet with CaseNo or CaseNumber column"
+)
+@click.option(
+    "--output-path",
+    "-out",
+    "dirpath",
+    required=True,
+    type=click.Path(),
+    prompt="PDF downloads directory",
+    help="Directory to download PDFs to"
+)
+@click.option(
+    "--customer-id",
+    "-c",
+    "cID",
+    required=True,
+    prompt="Alacourt Customer ID",
+    help="Customer ID on Alacourt.com",
+)
+@click.option(
+    "--user-id",
+    "-u",
+    "uID",
+    required=True,
+    prompt="Alacourt User ID",
+    help="User ID on Alacourt.com",
+)
+@click.option(
+    "--password",
+    "-p",
+    "pwd",
+    required=True,
+    prompt="Alacourt Password",
+    help="Password on Alacourt.com",
+    hide_input=True,
+)
+def _cli_fetch_by_case_number(query, dirpath, cID, uID, pwd):
+    driver = start_alacourt_driver(cID, uID, pwd, dirpath)
+    return fetch_by_case_numbers(query, driver)
+
 
 @main.command(
     name="vrr-pairs", help="Create voting rights summary from input cases and pairs"
 )
 @click.option(
     "--input-path",
     "-in",
@@ -6129,14 +6538,15 @@
     )
     return vrr_summary(conf)
 
 
 if __name__ == "__main__":
     main()
 
+
 #   #   #   #           GETTER METHODS         #   #   #   #
 
 
 def get_paths(dirpath):
     """
     From path-like `dirpath`, return list of paths to pdfs in directory
     """
@@ -6566,14 +6976,15 @@
             .rstrip("S")
             .rstrip("P")
             .strip()
         )
     except:
         return ""
 
+
 def getArrestingAgencyType(text):
     try:
         out = re.search(r"([^0-9]+) Arresting Agency Type:", str(text)).group(1)
     except:
         return ''
     out = re.sub(r"^\-.+", "", out)
     out = re.sub(r"County\:", "", out)
@@ -7211,26 +7622,29 @@
             ", ".join(
                 re.findall(r"Probation Begin Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             ),
         ).strip(), '%m/%d/%Y')
     except:
         return None
 
+
 def getProbationPeriod(text):
     try:
         return re.search(r"Probation Period\: (\d+ Years, \d+ Months, \d+ Days\.)", str(text)).group(1)
     except:
         return ''
 
+
 def getLicenseSuspPeriod(text):
     try:
         return re.search(r"License Susp Period\: (\d+ Years, \d+ Months, \d+ Days\.)", str(text)).group(1)
     except:
         return ''
 
+
 def getProbationRevoke(text):
     try:
         return re.sub(
             r"(Probation Revoke:)",
             "",
             ", ".join(
                 re.findall(r"Probation Revoke: (\d\d?/\d\d?/\d\d\d\d)", str(text))
@@ -7318,65 +7732,67 @@
         out = re.sub(r"Time\:", "", out, re.DOTALL)
         out = re.sub(r"Description\:", "", out, re.DOTALL)
         out = re.sub(r"Court Action", "", out, re.DOTALL)
         return out.strip()
     else:
         return ""
 
+
 def getBalanceByFeeCode(text, code):
     pat = f"(ACTIVE[^\n]+{code}[^\n]+)"
     rows = re.findall(pat, text)
     tot = 0.0
     for r in rows:
         splr = re.findall(r"\$\d+\.\d{2}", r)
         if len(splr) > 0:
             bal = float(re.sub(r'\$','',splr[-1]))
             tot += bal
     if len(rows) == 0:
         return None
     if len(rows) > 0:
         return tot
 
+
 def getAmtDueByFeeCode(text, code):
     pat = f"(ACTIVE[^\n]+{code}[^\n]+)"
     rows = re.findall(pat, text)
     tot = 0.0
     for r in rows:
         splr = re.findall(r"\$\d+\.\d{2}", r)
         if len(splr) > 0:
             bal = float(re.sub(r'\$','',splr[0]))
             tot += bal
     if len(rows) == 0:
         return None
     if len(rows) > 0:
         return tot
 
+
 def getAmtPaidByFeeCode(text, code):
     pat = f"(ACTIVE[^\n]+{code}[^\n]+)"
     rows = re.findall(pat, text)
     tot = 0.0
     for r in rows:
         splr = re.findall(r"\$\d+\.\d{2}", r)
         if len(splr) > 0:
             bal = float(re.sub(r'\$','',splr[1]))
             tot += bal
     if len(rows) == 0:
         return None
     if len(rows) > 0:
         return tot
 
+
 def getAmtHoldByFeeCode(text, code):
     pat = f"(ACTIVE[^\n]+{code}[^\n]+)"
     rows = re.findall(pat, text)
     tot = 0.0
     for r in rows:
         splr = re.findall(r"\$\d+\.\d{2}", r)
         if len(splr) > 0:
             bal = float(re.sub(r'\$','',splr[2]))
             tot += bal
     if len(rows) == 0:
         return None
     if len(rows) > 0:
         return tot
 
-
-
```

### Comparing `alacorder-80.8.0/PKG-INFO` & `alacorder-80.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.8.0
+Version: 80.8.1
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

