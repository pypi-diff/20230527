# Comparing `tmp/clown_sort-1.4.1.tar.gz` & `tmp/clown_sort-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.4.1.tar", max compression
+gzip compressed data, was "clown_sort-1.5.0.tar", max compression
```

## Comparing `clown_sort-1.4.1.tar` & `clown_sort-1.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2330 2023-05-22 02:18:01.650330 clown_sort-1.4.1/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.4.1/LICENSE
--rw-r--r--   0        0        0     7796 2023-05-09 18:33:06.154216 clown_sort-1.4.1/README.md
--rw-r--r--   0        0        0     3316 2023-04-24 00:56:40.931125 clown_sort-1.4.1/clown_sort/__init__.py
--rw-r--r--   0        0        0     7622 2023-05-22 01:52:09.100468 clown_sort-1.4.1/clown_sort/config.py
--rw-r--r--   0        0        0     9021 2023-05-09 18:20:37.530028 clown_sort-1.4.1/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4745 2023-05-09 18:20:37.530359 clown_sort-1.4.1/clown_sort/files/image_file.py
--rw-r--r--   0        0        0     1330 2023-04-24 00:42:15.932759 clown_sort-1.4.1/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0    10796 2023-05-09 18:20:37.530660 clown_sort-1.4.1/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3139 2023-05-09 18:20:37.531050 clown_sort-1.4.1/clown_sort/sort_selector.py
--rw-r--r--   0        0        0     9596 2023-05-22 02:07:43.101538 clown_sort-1.4.1/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.4.1/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.4.1/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.4.1/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3372 2023-04-30 19:27:53.085722 clown_sort-1.4.1/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.4.1/clown_sort/util/logging.py
--rw-r--r--   0        0        0     3354 2023-04-16 21:09:14.093347 clown_sort-1.4.1/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      520 2023-05-09 18:20:37.532239 clown_sort-1.4.1/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1558 2023-05-22 02:18:01.659658 clown_sort-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     9160 1970-01-01 00:00:00.000000 clown_sort-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     2492 2023-05-27 16:07:40.622832 clown_sort-1.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.5.0/LICENSE
+-rw-r--r--   0        0        0     8122 2023-05-27 16:06:01.552589 clown_sort-1.5.0/README.md
+-rw-r--r--   0        0        0     3316 2023-04-24 00:56:40.931125 clown_sort-1.5.0/clown_sort/__init__.py
+-rw-r--r--   0        0        0     7622 2023-05-22 01:52:09.100468 clown_sort-1.5.0/clown_sort/config.py
+-rw-r--r--   0        0        0     9021 2023-05-09 18:20:37.530028 clown_sort-1.5.0/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.5.0/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0     1330 2023-04-24 00:42:15.932759 clown_sort-1.5.0/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0    11214 2023-05-27 16:06:01.553498 clown_sort-1.5.0/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3233 2023-05-27 16:06:01.553887 clown_sort-1.5.0/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0     9617 2023-05-23 08:44:53.817611 clown_sort-1.5.0/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.5.0/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.5.0/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.5.0/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3372 2023-04-30 19:27:53.085722 clown_sort-1.5.0/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.5.0/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     3354 2023-04-16 21:09:14.093347 clown_sort-1.5.0/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.5.0/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1558 2023-05-27 16:07:40.628723 clown_sort-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     9486 1970-01-01 00:00:00.000000 clown_sort-1.5.0/PKG-INFO
```

### Comparing `clown_sort-1.4.1/CHANGELOG.md` & `clown_sort-1.5.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # NEXT RELEASE
 
+# 1.5.0
+* Combobox instead of radio buttons for manual fallback directory select
+* Replace fewer special characters in filenames
+* New default crypto sort rules
+
 ### 1.4.1
 * Make --manual-fallback and --only-if-match mutually exclusive
 * New default crypto sort rules
 
 ## 1.4.0
 * Add `--manual-fallback` option
 * Handle truncated image file binary errors
```

### Comparing `clown_sort-1.4.1/LICENSE` & `clown_sort-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.1/README.md` & `clown_sort-1.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,25 +43,28 @@
 # Get help
 sort_screenshots -h
 
 # Dry run with default cryptocurrency sort rules (dry runs don't actually move anything,
 # they just show you what will happen if you run again with the --execute flag)
 sort_screenshots
 
-# Execute default cryptocurrency sort rules against ~/Pictures/Screenshots
-sort_screenshots --execute
+# Execute default cryptocurrency sort rules against ~/Pictures/Screenshots with debug logging
+sort_screenshots --execute --debug
 
 # Sort a different directory of screenshots
 sort_screenshots --screenshots-dir /Users/hrollins/Pictures/get_in_the_van/tourphotos --execute
 
 # Sort with custom rules
 sort_screenshots --rules-csv /Users/hrollins/my_war.csv --execute
 
 # Sort pdfs
 sort_screenshots -f '.*pdf$' -e
+
+# Sort all but put up the manual folder / filename selector window if file doesn't match any sort rules
+sort_screenshots -a -mf -e
 ```
 
 # Setup
 [pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.
 ```
 pipx install clown_sort
 ```
@@ -91,27 +94,29 @@
 The default is for the tool to run in "dry run" mode, meaning it doesn't actually do anything - it just shows you what it _would_ do if you added the `--execute` flag. **YOU ARE ADVISED TO MAKE A BACKUP OF YOUR SCREENSHOTS FOLDER BEFORE HITTING THE `--execute` FLAG.**
 
 While every effort has been made to use Python's cross platform `Pathlib` module as much as possible sometimes shit gets wonky on other platforms. This is 100x as true on Windows - Clown Sort has never been tested on a Windows platform.
 
 ### Help Screen
 ![](doc/sort_screenshots_help.png)
 
-(In my personal usuage I tend to run the tool with the `--all` and `--only-if-match` options.)
+(In my personal usuage I tend to run the tool with the `--all` and `--manual-fallback` options.)
 
 ### Custom Sorting Rules
 The default is to sort cryptocurrency related content but you can define your own CSV of rules with two columns `folder` and `regex`. The value in `folder` specifies the subdirectory to sort into and `regex` is the pattern to match against. See [the default crypto related configuration](clown_sort/sorting_rules/crypto.csv) for an example. An explanation of regular expressions is beyond the scope of this README but many resources are available to help. If you're not good at regexes just remember that any alphanumeric string is a regex that will match that string. [pythex](http://pythex.org/) is a great website for testing your regexes.
 
 ### Example Output (Automated Sorting)
 ![](doc/output_example.png)
 
 
 ## Manually Sorting (Experimental)
 **This is an experimental feature.** It's only been tested on macOS.
 
-If you run with the `--manual-sort` command line the behavior is quite different. Rather than automatically sort files for you, instead for every file you will be greeted with a popup asking you for a desired filename and a radio button select of possible subdirectories off your `Sorted/` directory.
+If you run with the `--manual-sort` command line the behavior is quite different. Rather than automatically sort files for you for every image file you will be greeted with a popup asking you for a desired filename and a radio button select of possible subdirectories off your `Sorted/` directory.
+
+A related command line option is `--manual-fallback` which will popup a window only when the file is an image and has not matched any of the configured sorting rules.
 
 To use this feature you must install the optional `PySimpleGUI` package which can be accomplished like this:
 ```sh
 pipx install clown_sort[PySimpleGUI]
 ```
 
 ![](doc/manual_select_box.png)
```

### Comparing `clown_sort-1.4.1/clown_sort/__init__.py` & `clown_sort-1.5.0/clown_sort/__init__.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.1/clown_sort/config.py` & `clown_sort-1.5.0/clown_sort/config.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.1/clown_sort/filename_extractor.py` & `clown_sort-1.5.0/clown_sort/filename_extractor.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.1/clown_sort/files/image_file.py` & `clown_sort-1.5.0/clown_sort/files/image_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,47 +17,45 @@
 from clown_sort.config import Config
 from clown_sort.filename_extractor import FilenameExtractor
 from clown_sort.files.sortable_file import RuleMatch, SortableFile
 from clown_sort.util.filesystem_helper import copy_file_creation_time
 from clown_sort.util.logging import log
 from clown_sort.util.rich_helper import console, warning_text
 
-THUMBNAIL_DIMENSIONS = (400, 400)
+THUMBNAIL_DIMENSIONS = (512, 512)
 IMAGE_DESCRIPTION = 'ImageDescription'
 FILENAME_LENGTH_TO_CONSIDER_SORTED = 80
 
 EXIF_CODES = {
     IMAGE_DESCRIPTION: 270,
 }
 
 
 class ImageFile(SortableFile):
-    def copy_file_to_sorted_dir(self, destination_path: Path, match: Optional[re.Match] = None) -> Path:
+    def copy_file_to_sorted_dir(self, destination_path: Path, match: Optional[re.Match] = None) -> None:
         """
         Copies to a new file and injects the ImageDescription exif tag.
         If :destination_subdir is given new file will be in :destination_subdir off
         of the configured :destination_dir. Returns new file path.
         """
         exif_data = self.raw_exif_dict()
         exif_data.update([(EXIF_CODES[IMAGE_DESCRIPTION], self.extracted_text())])
         self._log_copy_file(destination_path, match)
 
         if Config.dry_run:
-            return destination_path
+            return
 
         try:
             self.pillow_image_obj().save(destination_path, exif=exif_data)
             copy_file_creation_time(self.file_path, destination_path)
         except ValueError as e:
             console.print_exception()
             console.print(f"ERROR while processing '{self.file_path}'", style='bright_red')
             raise e
 
-        return destination_path
-
     def new_basename(self) -> str:
         """Return a descriptive string usable in a filename."""
         if self._new_basename is not None:
             return self._new_basename
 
         if self.extracted_text() is None \
                 or len(self.extracted_text()) == 0 \
@@ -66,21 +64,21 @@
         else:
             self._filename_extractor = FilenameExtractor(self)
             self._new_basename = self._filename_extractor.filename()
 
         self._new_basename = self._new_basename.replace('""', '"')
         return self._new_basename
 
-    def image_bytes(self) -> bytes:
+    def thumbnail_bytes(self) -> bytes:
         """Return bytes for a thumbnail."""
         image = self.pillow_image_obj()
         image.thumbnail(THUMBNAIL_DIMENSIONS)
-        _image_bytes = io.BytesIO()
-        image.save(_image_bytes, format="PNG")
-        return _image_bytes.getvalue()
+        _thumbnail_bytes = io.BytesIO()
+        image.save(_thumbnail_bytes, format="PNG")
+        return _thumbnail_bytes.getvalue()
 
     def extracted_text(self) -> Optional[str]:
         """Use Tesseract to OCR the text in the image, which is returned as a string."""
         if self.text_extraction_attempted:
             return self._extracted_text
 
         try:
```

### Comparing `clown_sort-1.4.1/clown_sort/files/pdf_file.py` & `clown_sort-1.5.0/clown_sort/files/pdf_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.1/clown_sort/files/sortable_file.py` & `clown_sort-1.5.0/clown_sort/files/sortable_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 Base class for sortable files of any type.
 """
 import re
+import platform
 import shutil
 from collections import namedtuple
 from os import path, remove
 from pathlib import Path
+from subprocess import run
 from typing import List, Optional, Union
 
 from exiftool import ExifToolHelper
 from rich.console import Console, ConsoleOptions, RenderResult
 from rich.panel import Panel
 from rich.prompt import Confirm
 from rich.text import Text
@@ -166,14 +168,24 @@
         destination_path = Config.sorted_screenshots_dir
 
         if subdir is not None:
             destination_path = destination_path.joinpath(subdir)
 
         return destination_path.joinpath(self.new_basename())
 
+    def preview(self) -> None:
+        """Attempt to open a separate application to view the image."""
+        log.info(f"Opening '{self.file_path}'")
+
+        if platform.system() == 'Windows':
+            log.debug("Windows platform detected; attempting to run the file itself...")
+            run([self.file_path])
+        else:
+            run(['open', self.file_path])
+
     def _log_copy_file(self, destination_path: Path, match: Optional[re.Match] = None) -> None:
         """Log info about a file copy."""
         if Config.debug:
             console.print(copying_file_log_message(self.basename, destination_path))
             return
 
         log_msg = Text('').append('Copying to ', style='dim')
```

### Comparing `clown_sort-1.4.1/clown_sort/sort_selector.py` & `clown_sort-1.5.0/clown_sort/sort_selector.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,96 +1,94 @@
 """
 Open a GUI window to allow manual name / select.
 TODO: rename to something more appropriate
 """
-import shutil
 import sys
 from os import path, remove
-from subprocess import run
-
-from rich.panel import Panel
-from rich.text import Text
 
 from clown_sort.config import Config
 from clown_sort.filename_extractor import FilenameExtractor
-from clown_sort.util.dict_helper import get_dict_key_by_value
 from clown_sort.util.logging import log
 from clown_sort.util.rich_helper import bullet_text, console, indented_bullet
+from clown_sort.util.string_helper import is_empty
 
 RADIO_COLS = 11
+SELECT_SIZE = 45
 DELETE = 'Delete'
 OK = 'Move'
 OPEN = 'Preview Image'
 SKIP = 'Skip'
 EXIT = 'Exit'
 
 
 def process_file_with_popup(image: 'ImageFile') -> None:
-    import PySimpleGUI as sg
-    file_msg = Text("Processing: '").append(str(image.file_path), style='cyan reverse').append("'...")
-    console.print(Panel(file_msg, expand=False))
-    extracted_text = ' '.join((image.extracted_text() or '').splitlines())
-    log.info(f"OCR Text: {extracted_text} ({len(extracted_text)} chars)")
+    # Do the import here so as to allow usage without installing PySimpleGUI
+    import PySimpleGUI as psg
+    psg.theme('SystemDefault1')
     suggested_filename = FilenameExtractor(image).filename()
-    input = sg.Input(suggested_filename, size=(len(suggested_filename), 1))
+    sort_dirs = [path.basename(dir) for dir in Config.get_sort_dirs()]
+    max_dirname_length = max([len(dir) for dir in sort_dirs])
 
     layout = [
-        [sg.Image(data=image.image_bytes(), key="-IMAGE-")],
-        #[sg.Text(image.extracted_text())],
-        [sg.Text("Enter file name:")],
-        [input]
-    ] + list(_subdir_radio_select_columns(sg)) + \
-        [[sg.Button(OK, bind_return_key=True), sg.Button(DELETE), sg.Button(OPEN), sg.Button(SKIP), sg.Button(EXIT)]]
+        [psg.Column([[psg.Image(data=image.thumbnail_bytes(), key="-IMAGE-")]], justification='center')],
+        [psg.HSep()],
+        [psg.Text("Choose Filename:")],
+        [psg.Input(suggested_filename, size=(len(suggested_filename), 1))],# font=("Courier New", 12))],
+        [
+            psg.Text(f"Choose Directory:"),
+            psg.Combo(sort_dirs, size=(max_dirname_length, SELECT_SIZE)),
+            psg.Text(f"(Enter custom text to create new directory. If no directory is chosen file will be copied to '{Config.sorted_screenshots_dir}'.)")
+        ],
+        [
+            psg.Button(OK, bind_return_key=True),
+            psg.Button(DELETE),
+            psg.Button(OPEN),
+            psg.Button(SKIP),
+            psg.Button(EXIT)
+        ]
+    ]
 
-    window = sg.Window(image.basename, layout)
+    window = psg.Window(image.basename, layout)
 
     # Event Loop
     while True:
         event, values = window.Read()
 
+        if event == OPEN:
+            image.preview()
+            continue
+
+        window.close()
+
         if event == DELETE:
             log.warning(f"Deleting '{image.file_path}'")
             remove(image.file_path)
-            window.close()
             return
-        elif event == OPEN:
-            log.info(f"Opening '{image.file_path}'")
-            run(['open', image.file_path])
-        elif event == SKIP:
-            window.close()
+        elif event == SKIP or event == psg.WIN_CLOSED:
             return
         elif event == EXIT:
-            window.close()
             sys.exit()
         elif event == OK:
             break
 
-    window.close()
+    log.debug(f"All values: {values}")
     chosen_filename = values[0]
+    new_subdir = values[1]
+    destination_dir = Config.sorted_screenshots_dir.joinpath(new_subdir)
 
-    if chosen_filename is None or len(chosen_filename) == 0:
+    if is_empty(chosen_filename):
         raise ValueError("Filename can't be blank!")
 
-    try:
-        new_dir = get_dict_key_by_value(values, True)
-    except ValueError:
-        new_dir = Config.sorted_screenshots_dir
-
-    new_filename = path.join(new_dir, chosen_filename)
-    log.info(f"Chosen Filename: '{chosen_filename}'\nDirectory: '{new_dir}'\nNew file: '{new_filename}'\nEvent: {event}\n")
-    log.debug(f"All values: {values}")
-    console.print(bullet_text(f"Moving '{image.file_path}' to '{new_filename}'..."))
-
-    if Config.dry_run:
-        console.print(indented_bullet("Dry run so not moving..."), style='dim')
-    else:
-        shutil.move(image.file_path, new_filename)
+    if not destination_dir.exists():
+        result = psg.popup_yes_no(f"Subdir '{new_subdir}' doesn't exist. Create?",  title="Unknown Subdirectory")
 
+        if result == 'Yes' and not Config.dry_run:
+            log.info(f"Creating directory '{new_subdir}'...")
+            destination_dir.mkdir()
+        else:
+            console.print(bullet_text(f"Directory not found. Skipping '{image.file_path}'..."))
+            return
 
-def _subdir_radio_select_columns(sg):
-    dirs = Config.get_sort_dirs()
-
-    for i in range(0, len(dirs), RADIO_COLS):
-        yield [
-            sg.Radio(path.basename(dir), "SORTDIR_RADIO", default=False, key=dir)
-            for dir in dirs[i: i + RADIO_COLS]
-        ]
+    new_filename = destination_dir.joinpath(chosen_filename)
+    log.info(f"Chosen Filename: '{chosen_filename}'\nSubdir: '{new_subdir}'\nNew file: '{new_filename}'\nEvent: {event}\n")
+    console.print(bullet_text(f"Moving '{image.file_path}' to '{new_filename}'..."))
+    image.copy_file_to_sorted_dir(new_filename)
```

### Comparing `clown_sort-1.4.1/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.5.0/clown_sort/sorting_rules/crypto.csv`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 Miners,bitcoin[-_\s]*min(ing|er)|\$(CORZ|IRIS|ARGO|HUT|HIVE|CAN|BLOK|BTCM)|Core[-_\s]*Scientific|Iris[-_\s]*Energy|Blockstream
 Moonpay,moonpay
 MSTR,Saylor|MSTR
 MtGox,Mt[-_\s.]*Gox|\bwilly[-_\s]*bot
 Near Protocol,NEAR[-_\s]*Protocol|[$#]near\b|\bavichal\b|Rebecca[-_\s]*Rettig
 Nexo,\bNexo\b|Antoni[-_\s]*Trenchev|Georgi[-_\s]*Shulev|Lydia[-_\s]*Shuleva
 NFTs,crypto[-_\s]*punk|pudgy[-_\s]*penguin
-OKX,oke?[cx]|star[-_\s]*xu
+OKX,oke?[cx]|star[-_\s]*xu|\blennix[-_\s]*lai\b
 Olympus DAO,\bOlympus\b|OlympusDAO|\bOHM\b
 OpenPayd,openpayd|CFD\s?Team
 OpenSea,OpenSea
 PAG,\bpag\b|Weijian[-_\s]*Shan
 Paradigm,Fred[-_\s]*Ehrsam|paradigm\b
 Paxful,paxful|Ray[-_\s]*(Youssef|Savant)|Artur[-_\s]*Schaback
 Paxos,paxos|BUSD|USDP|PAXG
```

### Comparing `clown_sort-1.4.1/clown_sort/util/argument_parser.py` & `clown_sort-1.5.0/clown_sort/util/argument_parser.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.1/clown_sort/util/constants.py` & `clown_sort-1.5.0/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.1/clown_sort/util/filesystem_helper.py` & `clown_sort-1.5.0/clown_sort/util/filesystem_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.1/clown_sort/util/rich_helper.py` & `clown_sort-1.5.0/clown_sort/util/rich_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.4.1/pyproject.toml` & `clown_sort-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.4.1"
+version = "1.5.0"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
```

### Comparing `clown_sort-1.4.1/PKG-INFO` & `clown_sort-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.4.1
+Version: 1.5.0
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -75,25 +75,28 @@
 # Get help
 sort_screenshots -h
 
 # Dry run with default cryptocurrency sort rules (dry runs don't actually move anything,
 # they just show you what will happen if you run again with the --execute flag)
 sort_screenshots
 
-# Execute default cryptocurrency sort rules against ~/Pictures/Screenshots
-sort_screenshots --execute
+# Execute default cryptocurrency sort rules against ~/Pictures/Screenshots with debug logging
+sort_screenshots --execute --debug
 
 # Sort a different directory of screenshots
 sort_screenshots --screenshots-dir /Users/hrollins/Pictures/get_in_the_van/tourphotos --execute
 
 # Sort with custom rules
 sort_screenshots --rules-csv /Users/hrollins/my_war.csv --execute
 
 # Sort pdfs
 sort_screenshots -f '.*pdf$' -e
+
+# Sort all but put up the manual folder / filename selector window if file doesn't match any sort rules
+sort_screenshots -a -mf -e
 ```
 
 # Setup
 [pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.
 ```
 pipx install clown_sort
 ```
@@ -123,27 +126,29 @@
 The default is for the tool to run in "dry run" mode, meaning it doesn't actually do anything - it just shows you what it _would_ do if you added the `--execute` flag. **YOU ARE ADVISED TO MAKE A BACKUP OF YOUR SCREENSHOTS FOLDER BEFORE HITTING THE `--execute` FLAG.**
 
 While every effort has been made to use Python's cross platform `Pathlib` module as much as possible sometimes shit gets wonky on other platforms. This is 100x as true on Windows - Clown Sort has never been tested on a Windows platform.
 
 ### Help Screen
 ![](doc/sort_screenshots_help.png)
 
-(In my personal usuage I tend to run the tool with the `--all` and `--only-if-match` options.)
+(In my personal usuage I tend to run the tool with the `--all` and `--manual-fallback` options.)
 
 ### Custom Sorting Rules
 The default is to sort cryptocurrency related content but you can define your own CSV of rules with two columns `folder` and `regex`. The value in `folder` specifies the subdirectory to sort into and `regex` is the pattern to match against. See [the default crypto related configuration](clown_sort/sorting_rules/crypto.csv) for an example. An explanation of regular expressions is beyond the scope of this README but many resources are available to help. If you're not good at regexes just remember that any alphanumeric string is a regex that will match that string. [pythex](http://pythex.org/) is a great website for testing your regexes.
 
 ### Example Output (Automated Sorting)
 ![](doc/output_example.png)
 
 
 ## Manually Sorting (Experimental)
 **This is an experimental feature.** It's only been tested on macOS.
 
-If you run with the `--manual-sort` command line the behavior is quite different. Rather than automatically sort files for you, instead for every file you will be greeted with a popup asking you for a desired filename and a radio button select of possible subdirectories off your `Sorted/` directory.
+If you run with the `--manual-sort` command line the behavior is quite different. Rather than automatically sort files for you for every image file you will be greeted with a popup asking you for a desired filename and a radio button select of possible subdirectories off your `Sorted/` directory.
+
+A related command line option is `--manual-fallback` which will popup a window only when the file is an image and has not matched any of the configured sorting rules.
 
 To use this feature you must install the optional `PySimpleGUI` package which can be accomplished like this:
 ```sh
 pipx install clown_sort[PySimpleGUI]
 ```
 
 ![](doc/manual_select_box.png)
```

