# Comparing `tmp/clown_sort-1.5.0.tar.gz` & `tmp/clown_sort-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.5.0.tar", max compression
+gzip compressed data, was "clown_sort-1.5.1.tar", max compression
```

## Comparing `clown_sort-1.5.0.tar` & `clown_sort-1.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2492 2023-05-27 16:07:40.622832 clown_sort-1.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.5.0/LICENSE
--rw-r--r--   0        0        0     8122 2023-05-27 16:06:01.552589 clown_sort-1.5.0/README.md
--rw-r--r--   0        0        0     3316 2023-04-24 00:56:40.931125 clown_sort-1.5.0/clown_sort/__init__.py
--rw-r--r--   0        0        0     7622 2023-05-22 01:52:09.100468 clown_sort-1.5.0/clown_sort/config.py
--rw-r--r--   0        0        0     9021 2023-05-09 18:20:37.530028 clown_sort-1.5.0/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.5.0/clown_sort/files/image_file.py
--rw-r--r--   0        0        0     1330 2023-04-24 00:42:15.932759 clown_sort-1.5.0/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0    11214 2023-05-27 16:06:01.553498 clown_sort-1.5.0/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3233 2023-05-27 16:06:01.553887 clown_sort-1.5.0/clown_sort/sort_selector.py
--rw-r--r--   0        0        0     9617 2023-05-23 08:44:53.817611 clown_sort-1.5.0/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.5.0/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.5.0/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.5.0/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3372 2023-04-30 19:27:53.085722 clown_sort-1.5.0/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.5.0/clown_sort/util/logging.py
--rw-r--r--   0        0        0     3354 2023-04-16 21:09:14.093347 clown_sort-1.5.0/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.5.0/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1558 2023-05-27 16:07:40.628723 clown_sort-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     9486 1970-01-01 00:00:00.000000 clown_sort-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2551 2023-05-27 20:42:49.322886 clown_sort-1.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.5.1/LICENSE
+-rw-r--r--   0        0        0     8105 2023-05-27 20:38:10.332600 clown_sort-1.5.1/README.md
+-rw-r--r--   0        0        0     3316 2023-04-24 00:56:40.931125 clown_sort-1.5.1/clown_sort/__init__.py
+-rw-r--r--   0        0        0     7615 2023-05-27 20:40:26.997436 clown_sort-1.5.1/clown_sort/config.py
+-rw-r--r--   0        0        0     9021 2023-05-09 18:20:37.530028 clown_sort-1.5.1/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.5.1/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0     1321 2023-05-27 20:40:17.853554 clown_sort-1.5.1/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0    11214 2023-05-27 16:06:01.553498 clown_sort-1.5.1/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3233 2023-05-27 16:06:01.553887 clown_sort-1.5.1/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0     9634 2023-05-27 20:38:08.842118 clown_sort-1.5.1/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.5.1/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.5.1/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.5.1/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3372 2023-04-30 19:27:53.085722 clown_sort-1.5.1/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.5.1/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     3354 2023-04-16 21:09:14.093347 clown_sort-1.5.1/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.5.1/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1619 2023-05-27 20:42:49.329300 clown_sort-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     9527 1970-01-01 00:00:00.000000 clown_sort-1.5.1/PKG-INFO
```

### Comparing `clown_sort-1.5.0/CHANGELOG.md` & `clown_sort-1.5.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # NEXT RELEASE
 
+### 1.5.1
+* Fix the install messages for missing packages
+
 # 1.5.0
 * Combobox instead of radio buttons for manual fallback directory select
 * Replace fewer special characters in filenames
 * New default crypto sort rules
 
 ### 1.4.1
 * Make --manual-fallback and --only-if-match mutually exclusive
```

### Comparing `clown_sort-1.5.0/LICENSE` & `clown_sort-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.0/README.md` & `clown_sort-1.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 # Setup
 [pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.
 ```
 pipx install clown_sort
 ```
 
-Some (not many) PDFs require the `pycryptodome` package to be parsed. If you don't have it they will just not be parsed; only the filename will be used for sorting. To avoid complicating the dependency situation this is offered as an optional installation which can be accomplished with `pipx install clown_sort[pycryptodome]`.
+Some (not many) PDFs require the `pycryptodome` package to be parsed. If you don't have it they will just not be parsed; only the filename will be used for sorting. To avoid complicating the dependency situation this is offered as an optional installation which can be accomplished with `pipx install clown_sort[pdf]`.
 
 Updating to the latest version can be accomplished with `pipx upgrade clown_sort`.
 
 
 ### Configuring With `.clown_sort` File
 If there are command line options you find yourself specifying repeatedly you can place them in a `.clown_sort` file. When you invoke `sort_screenshots` the following locations will be checked for `.clown_sort`:
 
@@ -112,15 +112,15 @@
 
 If you run with the `--manual-sort` command line the behavior is quite different. Rather than automatically sort files for you for every image file you will be greeted with a popup asking you for a desired filename and a radio button select of possible subdirectories off your `Sorted/` directory.
 
 A related command line option is `--manual-fallback` which will popup a window only when the file is an image and has not matched any of the configured sorting rules.
 
 To use this feature you must install the optional `PySimpleGUI` package which can be accomplished like this:
 ```sh
-pipx install clown_sort[PySimpleGUI]
+pipx install clown_sort[gui]
 ```
 
 ![](doc/manual_select_box.png)
 
 
 # Contributing
 Feel free to file issues or open pull requests.
```

### Comparing `clown_sort-1.5.0/clown_sort/__init__.py` & `clown_sort-1.5.1/clown_sort/__init__.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.0/clown_sort/config.py` & `clown_sort-1.5.1/clown_sort/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,16 @@
     except ModuleNotFoundError:
         msg = Text('ERROR: ', style='bright_red')
 
         msg.append(
             'PySimpleGUI package must be installed before you can use the manual selector. Try running:',
             style='bright_white'
         )
-        log_optional_module_warning('PySimpleGUI', msg)
+
+        log_optional_module_warning('gui', msg)
         sys.exit()
 
 
 # TODO: it sucks that this is here but it's dependency hell otherwise
 def log_optional_module_warning(module_name: str, msg: Optional[Text] = None) -> None:
     """msg is optional argument for a custom message, otherwise it's a warning"""
     if msg is None:
```

### Comparing `clown_sort-1.5.0/clown_sort/filename_extractor.py` & `clown_sort-1.5.1/clown_sort/filename_extractor.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.0/clown_sort/files/image_file.py` & `clown_sort-1.5.1/clown_sort/files/image_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.0/clown_sort/files/pdf_file.py` & `clown_sort-1.5.1/clown_sort/files/pdf_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
         self._extracted_text = None
 
         try:
             pdf_reader = PdfReader(self.file_path)
             self._extracted_text = '\\n\\n'.join([page.extract_text() for page in pdf_reader.pages])
         except DependencyError:
-            log_optional_module_warning('pycryptodome')
+            log_optional_module_warning('pdf')
         except (KeyError, TypeError):
             # TODO: failure on KeyError: '/Root' seems to have been fixed but not released yet
             # https://github.com/py-pdf/pypdf/pull/1784
             log.warn("Failed to parse PDF!")
 
         if self._extracted_text is not None:
             self._extracted_text = self._extracted_text.strip()
```

### Comparing `clown_sort-1.5.0/clown_sort/files/sortable_file.py` & `clown_sort-1.5.1/clown_sort/files/sortable_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.0/clown_sort/sort_selector.py` & `clown_sort-1.5.1/clown_sort/sort_selector.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.0/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.5.1/clown_sort/sorting_rules/crypto.csv`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 Bored Ape Yacht Club,BAYC|Bored[-_\s]*Ape|yuga[-_\s]*labs
 Bros,cryptomanran|trillionUSD|nic[-_\s]*carter|bitboy|ben[-_\s]*armstrong|basedkarbon|thecryptolark|adam([-_\s]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s]*Alfred|natbrunell|natalie[-_\s]*brunell|stackersatoshi|Max[-_\s]*Keiser|Cowboy[-_\s]*Crypto|minimalcsgo|greg16676935420|@Aridavidpaul|\bAri[-_\s]*Paul\b|raoul(gmi|[-_\s]*pal)|mccormack
 Broettes,Nicole[-_\s]*Behnam|natbrunell
 Bybit,\bBybit\b|Ben[-_\s]*Zhou|InvestByBit|TravelByBit
 Cardano,Cardano|[$\s]ADA[^\w]|Hoskinson|\bIOHK
 Cathie Wood,Cathie\s*Wood|\bARK(F|G|K|\s*Innovation|\s*Invest)|\bIZRL
 Celsius,celsius|mashinsky|levity[-_\s]*and[-_\s]*love|\bcelsian|Artur[-_\s]*Abreu|ronpaulbot
+China,fentanyl
 Circle,[@#]circle|usdc|circle[-_\s]*internet|disparte|\ballaire|jerallaire
 CMCC Global,CMCC[-_\s]*Global
 Coinbase,Coinbase|\$COIN|brian[-_\s]*armstrong|grewal\b|Asiff[-_\s]*Hirji|\bbalaji|Fred[-_\s]*Ehrsam|\bremitly\b|\$RELY\b
 Coinflex,Mark[-_\s]*Lamb|Roger[-_\s]*Ver|coinflex|Doug[-_\s]*Polk|OPNX|flexusd|Leslie[-_\s]*Lamb|dougpolkvids
 CoinLoan,coinloan|Faliushin\b
 CompoundFi,compoundfi|leshner|\bgonen\b
 Cross River Bank,CRB|Cross[-_\s]*River|Prestige[-_\s]*Capital|bae[-_\s]*communications|Zenfi|PeerIQ|\bupstart\b|\bUPST\b|\bLeumi\b|Hapoalim|BetterFin|\bMANTL\b|\bLvnv
@@ -91,15 +92,15 @@
 Messari,Ryan\s*Selkis|twobitidiot|messari|@robustus|Dan[-_\s]*McArdle
 Memes,\smeme
 Metallicus,FBBT|Nauvoo|Metallicus|Bitcoinwalking|Bruce[-_\s]*Stewart|\bHayner\b
 Metropolitan Commercial Bank,MCB\b|MCBankNY|Metropolitan[-_\s]*(Bank|Commercial)|Mission[-_\s]*Gateway|Aryeh[-_\s]*Realty
 Founders Bank,Michael[-_\s]*Bianchi|Founders[-_\s]*Bank
 Miles Guo,\bguo\b|\bhcoin|himalaya[-_\s]*exchange|\bbannon\b|\bfjb|\bkwok\b|brother[-_\s]*seven|kin[-_\s]*ming[-_\s]*je|william[-_\s]*je\b|\bHaoyun\b|\bLi[-_\s]*You\b
 Miners,bitcoin[-_\s]*min(ing|er)|\$(CORZ|IRIS|ARGO|HUT|HIVE|CAN|BLOK|BTCM)|Core[-_\s]*Scientific|Iris[-_\s]*Energy|Blockstream
-Moonpay,moonpay
+Moonpay,\bmoonpay
 MSTR,Saylor|MSTR
 MtGox,Mt[-_\s.]*Gox|\bwilly[-_\s]*bot
 Near Protocol,NEAR[-_\s]*Protocol|[$#]near\b|\bavichal\b|Rebecca[-_\s]*Rettig
 Nexo,\bNexo\b|Antoni[-_\s]*Trenchev|Georgi[-_\s]*Shulev|Lydia[-_\s]*Shuleva
 NFTs,crypto[-_\s]*punk|pudgy[-_\s]*penguin
 OKX,oke?[cx]|star[-_\s]*xu|\blennix[-_\s]*lai\b
 Olympus DAO,\bOlympus\b|OlympusDAO|\bOHM\b
```

### Comparing `clown_sort-1.5.0/clown_sort/util/argument_parser.py` & `clown_sort-1.5.1/clown_sort/util/argument_parser.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.0/clown_sort/util/constants.py` & `clown_sort-1.5.1/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.0/clown_sort/util/filesystem_helper.py` & `clown_sort-1.5.1/clown_sort/util/filesystem_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.0/clown_sort/util/rich_helper.py` & `clown_sort-1.5.1/clown_sort/util/rich_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.0/clown_sort/util/string_helper.py` & `clown_sort-1.5.1/clown_sort/util/string_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.5.0/pyproject.toml` & `clown_sort-1.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.5.0"
+version = "1.5.1"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
@@ -40,23 +40,25 @@
 pillow = "^9.4.0"
 filedate = "^2.0"
 python-dotenv = "^0.21.1"
 rich-argparse-plus = "^0.3.1.4"
 pyexiftool = "^0.5.5"
 pypdf = "^3.4.1"
 pycryptodome = {version = "^3.17", optional = true}
+pymupdf = {version = "^1.22.3", optional = true}
 
 [tool.poetry.extras]
-pdf = ['pycryptodome']
+pdf = ['pycryptodome', 'pymupdf']
 gui = ['PySimpleGUI']
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 bpython = "^0.24"
 
+
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
 
 
 [build-system]
```

### Comparing `clown_sort-1.5.0/PKG-INFO` & `clown_sort-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.5.0
+Version: 1.5.1
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -19,14 +19,15 @@
 Requires-Dist: PySimpleGUI (>=4.60.4,<5.0.0) ; extra == "gui"
 Requires-Dist: exif (>=1.5.0,<2.0.0)
 Requires-Dist: filedate (>=2.0,<3.0)
 Requires-Dist: piexif (>=1.1.3,<2.0.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: pycryptodome (>=3.17,<4.0) ; extra == "pdf"
 Requires-Dist: pyexiftool (>=0.5.5,<0.6.0)
+Requires-Dist: pymupdf (>=1.22.3,<2.0.0) ; extra == "pdf"
 Requires-Dist: pypdf (>=3.4.1,<4.0.0)
 Requires-Dist: pytesseract (>=0.3.10,<0.4.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
 Requires-Dist: rich (>=13.0.1,<14.0.0)
 Requires-Dist: rich-argparse-plus (>=0.3.1.4,<0.4.0.0)
 Description-Content-Type: text/markdown
 
@@ -97,15 +98,15 @@
 
 # Setup
 [pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.
 ```
 pipx install clown_sort
 ```
 
-Some (not many) PDFs require the `pycryptodome` package to be parsed. If you don't have it they will just not be parsed; only the filename will be used for sorting. To avoid complicating the dependency situation this is offered as an optional installation which can be accomplished with `pipx install clown_sort[pycryptodome]`.
+Some (not many) PDFs require the `pycryptodome` package to be parsed. If you don't have it they will just not be parsed; only the filename will be used for sorting. To avoid complicating the dependency situation this is offered as an optional installation which can be accomplished with `pipx install clown_sort[pdf]`.
 
 Updating to the latest version can be accomplished with `pipx upgrade clown_sort`.
 
 
 ### Configuring With `.clown_sort` File
 If there are command line options you find yourself specifying repeatedly you can place them in a `.clown_sort` file. When you invoke `sort_screenshots` the following locations will be checked for `.clown_sort`:
 
@@ -144,15 +145,15 @@
 
 If you run with the `--manual-sort` command line the behavior is quite different. Rather than automatically sort files for you for every image file you will be greeted with a popup asking you for a desired filename and a radio button select of possible subdirectories off your `Sorted/` directory.
 
 A related command line option is `--manual-fallback` which will popup a window only when the file is an image and has not matched any of the configured sorting rules.
 
 To use this feature you must install the optional `PySimpleGUI` package which can be accomplished like this:
 ```sh
-pipx install clown_sort[PySimpleGUI]
+pipx install clown_sort[gui]
 ```
 
 ![](doc/manual_select_box.png)
 
 
 # Contributing
 Feel free to file issues or open pull requests.
```

