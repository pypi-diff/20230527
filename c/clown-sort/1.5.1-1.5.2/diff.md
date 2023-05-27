# Comparing `tmp/clown_sort-1.5.1.tar.gz` & `tmp/clown_sort-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.5.1.tar", max compression
+gzip compressed data, was "clown_sort-1.5.2.tar", max compression
```

## Comparing `clown_sort-1.5.1.tar` & `clown_sort-1.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2551 2023-05-27 20:42:49.322886 clown_sort-1.5.1/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.5.1/LICENSE
--rw-r--r--   0        0        0     8105 2023-05-27 20:38:10.332600 clown_sort-1.5.1/README.md
--rw-r--r--   0        0        0     3316 2023-04-24 00:56:40.931125 clown_sort-1.5.1/clown_sort/__init__.py
--rw-r--r--   0        0        0     7615 2023-05-27 20:40:26.997436 clown_sort-1.5.1/clown_sort/config.py
--rw-r--r--   0        0        0     9021 2023-05-09 18:20:37.530028 clown_sort-1.5.1/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.5.1/clown_sort/files/image_file.py
--rw-r--r--   0        0        0     1321 2023-05-27 20:40:17.853554 clown_sort-1.5.1/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0    11214 2023-05-27 16:06:01.553498 clown_sort-1.5.1/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3233 2023-05-27 16:06:01.553887 clown_sort-1.5.1/clown_sort/sort_selector.py
--rw-r--r--   0        0        0     9634 2023-05-27 20:38:08.842118 clown_sort-1.5.1/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.5.1/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.5.1/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.5.1/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3372 2023-04-30 19:27:53.085722 clown_sort-1.5.1/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.5.1/clown_sort/util/logging.py
--rw-r--r--   0        0        0     3354 2023-04-16 21:09:14.093347 clown_sort-1.5.1/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.5.1/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1619 2023-05-27 20:42:49.329300 clown_sort-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     9527 1970-01-01 00:00:00.000000 clown_sort-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     2591 2023-05-27 20:46:55.649797 clown_sort-1.5.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.5.2/LICENSE
+-rw-r--r--   0        0        0     8105 2023-05-27 20:38:10.332600 clown_sort-1.5.2/README.md
+-rw-r--r--   0        0        0     3316 2023-04-24 00:56:40.931125 clown_sort-1.5.2/clown_sort/__init__.py
+-rw-r--r--   0        0        0     7615 2023-05-27 20:45:42.054203 clown_sort-1.5.2/clown_sort/config.py
+-rw-r--r--   0        0        0     9021 2023-05-09 18:20:37.530028 clown_sort-1.5.2/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.5.2/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0     1321 2023-05-27 20:45:42.054851 clown_sort-1.5.2/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0    11214 2023-05-27 16:06:01.553498 clown_sort-1.5.2/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3233 2023-05-27 16:06:01.553887 clown_sort-1.5.2/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0     9617 2023-05-27 20:45:31.631557 clown_sort-1.5.2/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.5.2/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.5.2/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.5.2/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3372 2023-04-30 19:27:53.085722 clown_sort-1.5.2/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.5.2/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     3354 2023-04-16 21:09:14.093347 clown_sort-1.5.2/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.5.2/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1558 2023-05-27 20:46:55.654240 clown_sort-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     9469 1970-01-01 00:00:00.000000 clown_sort-1.5.2/PKG-INFO
```

### Comparing `clown_sort-1.5.1/CHANGELOG.md` & `clown_sort-1.5.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # NEXT RELEASE
 
+### 1.5.2
+* Override premature release
+
 ### 1.5.1
 * Fix the install messages for missing packages
 
 # 1.5.0
 * Combobox instead of radio buttons for manual fallback directory select
 * Replace fewer special characters in filenames
 * New default crypto sort rules
```

### Comparing `clown_sort-1.5.1/LICENSE` & `clown_sort-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.1/README.md` & `clown_sort-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.1/clown_sort/__init__.py` & `clown_sort-1.5.2/clown_sort/__init__.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.1/clown_sort/config.py` & `clown_sort-1.5.2/clown_sort/config.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.1/clown_sort/filename_extractor.py` & `clown_sort-1.5.2/clown_sort/filename_extractor.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.1/clown_sort/files/image_file.py` & `clown_sort-1.5.2/clown_sort/files/image_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.1/clown_sort/files/pdf_file.py` & `clown_sort-1.5.2/clown_sort/files/pdf_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.1/clown_sort/files/sortable_file.py` & `clown_sort-1.5.2/clown_sort/files/sortable_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.1/clown_sort/sort_selector.py` & `clown_sort-1.5.2/clown_sort/sort_selector.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.1/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.5.2/clown_sort/sorting_rules/crypto.csv`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 Bored Ape Yacht Club,BAYC|Bored[-_\s]*Ape|yuga[-_\s]*labs
 Bros,cryptomanran|trillionUSD|nic[-_\s]*carter|bitboy|ben[-_\s]*armstrong|basedkarbon|thecryptolark|adam([-_\s]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s]*Alfred|natbrunell|natalie[-_\s]*brunell|stackersatoshi|Max[-_\s]*Keiser|Cowboy[-_\s]*Crypto|minimalcsgo|greg16676935420|@Aridavidpaul|\bAri[-_\s]*Paul\b|raoul(gmi|[-_\s]*pal)|mccormack
 Broettes,Nicole[-_\s]*Behnam|natbrunell
 Bybit,\bBybit\b|Ben[-_\s]*Zhou|InvestByBit|TravelByBit
 Cardano,Cardano|[$\s]ADA[^\w]|Hoskinson|\bIOHK
 Cathie Wood,Cathie\s*Wood|\bARK(F|G|K|\s*Innovation|\s*Invest)|\bIZRL
 Celsius,celsius|mashinsky|levity[-_\s]*and[-_\s]*love|\bcelsian|Artur[-_\s]*Abreu|ronpaulbot
-China,fentanyl
 Circle,[@#]circle|usdc|circle[-_\s]*internet|disparte|\ballaire|jerallaire
 CMCC Global,CMCC[-_\s]*Global
 Coinbase,Coinbase|\$COIN|brian[-_\s]*armstrong|grewal\b|Asiff[-_\s]*Hirji|\bbalaji|Fred[-_\s]*Ehrsam|\bremitly\b|\$RELY\b
 Coinflex,Mark[-_\s]*Lamb|Roger[-_\s]*Ver|coinflex|Doug[-_\s]*Polk|OPNX|flexusd|Leslie[-_\s]*Lamb|dougpolkvids
 CoinLoan,coinloan|Faliushin\b
 CompoundFi,compoundfi|leshner|\bgonen\b
 Cross River Bank,CRB|Cross[-_\s]*River|Prestige[-_\s]*Capital|bae[-_\s]*communications|Zenfi|PeerIQ|\bupstart\b|\bUPST\b|\bLeumi\b|Hapoalim|BetterFin|\bMANTL\b|\bLvnv
@@ -92,15 +91,15 @@
 Messari,Ryan\s*Selkis|twobitidiot|messari|@robustus|Dan[-_\s]*McArdle
 Memes,\smeme
 Metallicus,FBBT|Nauvoo|Metallicus|Bitcoinwalking|Bruce[-_\s]*Stewart|\bHayner\b
 Metropolitan Commercial Bank,MCB\b|MCBankNY|Metropolitan[-_\s]*(Bank|Commercial)|Mission[-_\s]*Gateway|Aryeh[-_\s]*Realty
 Founders Bank,Michael[-_\s]*Bianchi|Founders[-_\s]*Bank
 Miles Guo,\bguo\b|\bhcoin|himalaya[-_\s]*exchange|\bbannon\b|\bfjb|\bkwok\b|brother[-_\s]*seven|kin[-_\s]*ming[-_\s]*je|william[-_\s]*je\b|\bHaoyun\b|\bLi[-_\s]*You\b
 Miners,bitcoin[-_\s]*min(ing|er)|\$(CORZ|IRIS|ARGO|HUT|HIVE|CAN|BLOK|BTCM)|Core[-_\s]*Scientific|Iris[-_\s]*Energy|Blockstream
-Moonpay,\bmoonpay
+Moonpay,moonpay
 MSTR,Saylor|MSTR
 MtGox,Mt[-_\s.]*Gox|\bwilly[-_\s]*bot
 Near Protocol,NEAR[-_\s]*Protocol|[$#]near\b|\bavichal\b|Rebecca[-_\s]*Rettig
 Nexo,\bNexo\b|Antoni[-_\s]*Trenchev|Georgi[-_\s]*Shulev|Lydia[-_\s]*Shuleva
 NFTs,crypto[-_\s]*punk|pudgy[-_\s]*penguin
 OKX,oke?[cx]|star[-_\s]*xu|\blennix[-_\s]*lai\b
 Olympus DAO,\bOlympus\b|OlympusDAO|\bOHM\b
```

### Comparing `clown_sort-1.5.1/clown_sort/util/argument_parser.py` & `clown_sort-1.5.2/clown_sort/util/argument_parser.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.1/clown_sort/util/constants.py` & `clown_sort-1.5.2/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.1/clown_sort/util/filesystem_helper.py` & `clown_sort-1.5.2/clown_sort/util/filesystem_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.1/clown_sort/util/rich_helper.py` & `clown_sort-1.5.2/clown_sort/util/rich_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.1/clown_sort/util/string_helper.py` & `clown_sort-1.5.2/clown_sort/util/string_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.1/pyproject.toml` & `clown_sort-1.5.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.5.1"
+version = "1.5.2"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
@@ -40,25 +40,23 @@
 pillow = "^9.4.0"
 filedate = "^2.0"
 python-dotenv = "^0.21.1"
 rich-argparse-plus = "^0.3.1.4"
 pyexiftool = "^0.5.5"
 pypdf = "^3.4.1"
 pycryptodome = {version = "^3.17", optional = true}
-pymupdf = {version = "^1.22.3", optional = true}
 
 [tool.poetry.extras]
-pdf = ['pycryptodome', 'pymupdf']
+pdf = ['pycryptodome']
 gui = ['PySimpleGUI']
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 bpython = "^0.24"
 
-
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
 
 
 [build-system]
```

### Comparing `clown_sort-1.5.1/PKG-INFO` & `clown_sort-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.5.1
+Version: 1.5.2
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,14 @@
 Requires-Dist: PySimpleGUI (>=4.60.4,<5.0.0) ; extra == "gui"
 Requires-Dist: exif (>=1.5.0,<2.0.0)
 Requires-Dist: filedate (>=2.0,<3.0)
 Requires-Dist: piexif (>=1.1.3,<2.0.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: pycryptodome (>=3.17,<4.0) ; extra == "pdf"
 Requires-Dist: pyexiftool (>=0.5.5,<0.6.0)
-Requires-Dist: pymupdf (>=1.22.3,<2.0.0) ; extra == "pdf"
 Requires-Dist: pypdf (>=3.4.1,<4.0.0)
 Requires-Dist: pytesseract (>=0.3.10,<0.4.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
 Requires-Dist: rich (>=13.0.1,<14.0.0)
 Requires-Dist: rich-argparse-plus (>=0.3.1.4,<0.4.0.0)
 Description-Content-Type: text/markdown
```

