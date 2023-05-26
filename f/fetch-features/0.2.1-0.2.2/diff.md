# Comparing `tmp/fetch_features-0.2.1.tar.gz` & `tmp/fetch_features-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fetch_features-0.2.1.tar", last modified: Sun May 14 08:00:07 2023, max compression
+gzip compressed data, was "fetch_features-0.2.2.tar", last modified: Fri May 26 22:13:33 2023, max compression
```

## Comparing `fetch_features-0.2.1.tar` & `fetch_features-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-14 08:00:07.037840 fetch_features-0.2.1/
--rw-r--r--   0 msp        (501) staff       (20)     1507 2023-04-07 00:12:37.000000 fetch_features-0.2.1/LICENSE.md
--rw-r--r--   0 msp        (501) staff       (20)     3130 2023-05-14 08:00:07.037226 fetch_features-0.2.1/PKG-INFO
--rwxr-xr-x   0 msp        (501) staff       (20)     2404 2023-05-14 07:49:12.000000 fetch_features-0.2.1/README.md
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-14 08:00:07.022525 fetch_features-0.2.1/images/
--rw-r--r--   0 msp        (501) staff       (20)   340268 2023-04-30 01:32:33.000000 fetch_features-0.2.1/images/fetch_features_gui.png
--rw-r--r--   0 msp        (501) staff       (20)     1130 2023-05-14 07:55:58.000000 fetch_features-0.2.1/pyproject.toml
--rw-r--r--   0 msp        (501) staff       (20)       38 2023-05-14 08:00:07.037989 fetch_features-0.2.1/setup.cfg
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-14 08:00:07.019341 fetch_features-0.2.1/src/
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-14 08:00:07.029414 fetch_features-0.2.1/src/fetch_features.egg-info/
--rw-r--r--   0 msp        (501) staff       (20)     3130 2023-05-14 08:00:06.000000 fetch_features-0.2.1/src/fetch_features.egg-info/PKG-INFO
--rw-r--r--   0 msp        (501) staff       (20)      466 2023-05-14 08:00:07.000000 fetch_features-0.2.1/src/fetch_features.egg-info/SOURCES.txt
--rw-r--r--   0 msp        (501) staff       (20)        1 2023-05-14 08:00:06.000000 fetch_features-0.2.1/src/fetch_features.egg-info/dependency_links.txt
--rw-r--r--   0 msp        (501) staff       (20)       50 2023-05-14 08:00:06.000000 fetch_features-0.2.1/src/fetch_features.egg-info/entry_points.txt
--rw-r--r--   0 msp        (501) staff       (20)      146 2023-05-14 08:00:06.000000 fetch_features-0.2.1/src/fetch_features.egg-info/requires.txt
--rw-r--r--   0 msp        (501) staff       (20)        8 2023-05-14 08:00:06.000000 fetch_features-0.2.1/src/fetch_features.egg-info/top_level.txt
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-14 08:00:07.035680 fetch_features-0.2.1/src/fetcher/
--rw-r--r--   0 msp        (501) staff       (20)        0 2023-05-04 15:38:40.000000 fetch_features-0.2.1/src/fetcher/__init__.py
--rw-r--r--   0 msp        (501) staff       (20)     1239 2023-05-13 22:48:30.000000 fetch_features-0.2.1/src/fetcher/__main__.py
--rwx------   0 msp        (501) staff       (20)    16395 2023-05-13 22:49:16.000000 fetch_features-0.2.1/src/fetcher/access_genbank.py
--rwx------   0 msp        (501) staff       (20)    33243 2023-05-04 16:18:08.000000 fetch_features-0.2.1/src/fetcher/database.py
--rw-r--r--   0 msp        (501) staff       (20)    17348 2023-05-13 22:50:35.000000 fetch_features-0.2.1/src/fetcher/gui.py
--rw-r--r--   0 msp        (501) staff       (20)    10144 2023-05-14 07:41:02.000000 fetch_features-0.2.1/src/fetcher/user_input.py
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-26 22:13:33.875060 fetch_features-0.2.2/
+-rw-r--r--   0 msp        (501) staff       (20)     1507 2023-04-07 00:12:37.000000 fetch_features-0.2.2/LICENSE.md
+-rw-r--r--   0 msp        (501) staff       (20)     3235 2023-05-26 22:13:33.874471 fetch_features-0.2.2/PKG-INFO
+-rwxr-xr-x   0 msp        (501) staff       (20)     2509 2023-05-26 22:10:06.000000 fetch_features-0.2.2/README.md
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-26 22:13:33.859080 fetch_features-0.2.2/images/
+-rw-r--r--   0 msp        (501) staff       (20)   340268 2023-04-30 01:32:33.000000 fetch_features-0.2.2/images/fetch_features_gui.png
+-rw-r--r--   0 msp        (501) staff       (20)     1156 2023-05-26 21:25:14.000000 fetch_features-0.2.2/pyproject.toml
+-rw-r--r--   0 msp        (501) staff       (20)       38 2023-05-26 22:13:33.875201 fetch_features-0.2.2/setup.cfg
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-26 22:13:33.855887 fetch_features-0.2.2/src/
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-26 22:13:33.867561 fetch_features-0.2.2/src/fetch_features.egg-info/
+-rw-r--r--   0 msp        (501) staff       (20)     3235 2023-05-26 22:13:33.000000 fetch_features-0.2.2/src/fetch_features.egg-info/PKG-INFO
+-rw-r--r--   0 msp        (501) staff       (20)      466 2023-05-26 22:13:33.000000 fetch_features-0.2.2/src/fetch_features.egg-info/SOURCES.txt
+-rw-r--r--   0 msp        (501) staff       (20)        1 2023-05-26 22:13:33.000000 fetch_features-0.2.2/src/fetch_features.egg-info/dependency_links.txt
+-rw-r--r--   0 msp        (501) staff       (20)       57 2023-05-26 22:13:33.000000 fetch_features-0.2.2/src/fetch_features.egg-info/entry_points.txt
+-rw-r--r--   0 msp        (501) staff       (20)      159 2023-05-26 22:13:33.000000 fetch_features-0.2.2/src/fetch_features.egg-info/requires.txt
+-rw-r--r--   0 msp        (501) staff       (20)        8 2023-05-26 22:13:33.000000 fetch_features-0.2.2/src/fetch_features.egg-info/top_level.txt
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-26 22:13:33.873347 fetch_features-0.2.2/src/fetcher/
+-rw-r--r--   0 msp        (501) staff       (20)        0 2023-05-04 15:38:40.000000 fetch_features-0.2.2/src/fetcher/__init__.py
+-rw-r--r--   0 msp        (501) staff       (20)     1239 2023-05-13 22:48:30.000000 fetch_features-0.2.2/src/fetcher/__main__.py
+-rwx------   0 msp        (501) staff       (20)    16395 2023-05-13 22:49:16.000000 fetch_features-0.2.2/src/fetcher/access_genbank.py
+-rwx------   0 msp        (501) staff       (20)    33243 2023-05-04 16:18:08.000000 fetch_features-0.2.2/src/fetcher/database.py
+-rw-r--r--   0 msp        (501) staff       (20)    17348 2023-05-13 22:50:35.000000 fetch_features-0.2.2/src/fetcher/gui.py
+-rw-r--r--   0 msp        (501) staff       (20)    10405 2023-05-26 21:57:12.000000 fetch_features-0.2.2/src/fetcher/user_input.py
```

### Comparing `fetch_features-0.2.1/LICENSE.md` & `fetch_features-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.1/PKG-INFO` & `fetch_features-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetch_features
-Version: 0.2.1
+Version: 0.2.2
 Summary: Fetch features from a list of accession or BioSample numbers.
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/fetch_features
 Keywords: unique identifier,accession number,BioSample number,GenBank,sequence features
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -28,33 +28,34 @@
 ```
 
 ## Usage and options
 
 To view all the options run:
 
 ```bash
-fetcher --help
+fetch_features --help
 ```
 
 Output:
 
 ```
-usage: fetcher [-h] [-i, INPUT] [-t, TYPE] [-e, EMAIL] [-o, OUTPUT] [-s, SAVE-AS]
-               [--access-biosample-from-accession] [--gui]
+usage: fetch_features [-h] [-v] [-i INPUT] [-t TYPE] [-e EMAIL] [-o OUTPUT] [-s SAVE_AS]
+                      [--access-biosample-from-accession] [--gui]
 
   __      _       _        __            _
  / _| ___| |_ ___| |__    / _| ___  __ _| |_ _   _ _ __ ___  ___
 | |_ / _ \ __/ __| '_ \  | |_ / _ \/ _` | __| | | | '__/ _ \/ __|
 |  _|  __/ || (__| | | | |  _|  __/ (_| | |_| |_| | | |  __/\__ \
 |_|  \___|\__\___|_| |_| |_|  \___|\__,_|\__|\__,_|_|  \___||___/
 
 Fetch features from a list of accession or BioSample numbers.
 
 Help:
   -h, --help            Show this help message and exit.
+  -v, --version         Show program's version number and exit
 
 Required:
   -i INPUT, --input INPUT
                         Path to input file with list of unique identifiers (UIDs).
                         The user should provide the list of UIDs in a txt or xlsx file.
   -t TYPE, --type TYPE  Type of unique identifier: `accession` or `biosample`.
                         The `biosample` option fetches the information of the most
@@ -74,27 +75,27 @@
 ```
 
 ## Usage examples
 
 1. The simplest command. The output is in the current working directoy.
 
 ```bash
-fetcher -i path/to/list.txt -t accession -e email@address.com
+fetch_features -i path/to/list.txt -t accession -e email@address.com
 ```
 
 2. In this example, the output is in your Documents.
 
 ```bash
-fetcher -i path/to/list.txt -t accession -e email@address.com -o ~/Documents
+fetch_features -i path/to/list.txt -t accession -e email@address.com -o ~/Documents
 ```
 
 3. If you prefer the GUI version.
 
 ```bash
-fetcher --gui
+fetch_features --gui
 ```
 
 <p align="center">
   <picture>
     <img src="./images/fetch_features_gui.png">
   </picture>
 </p>
```

### Comparing `fetch_features-0.2.1/README.md` & `fetch_features-0.2.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -11,33 +11,34 @@
 ```
 
 ## Usage and options
 
 To view all the options run:
 
 ```bash
-fetcher --help
+fetch_features --help
 ```
 
 Output:
 
 ```
-usage: fetcher [-h] [-i, INPUT] [-t, TYPE] [-e, EMAIL] [-o, OUTPUT] [-s, SAVE-AS]
-               [--access-biosample-from-accession] [--gui]
+usage: fetch_features [-h] [-v] [-i INPUT] [-t TYPE] [-e EMAIL] [-o OUTPUT] [-s SAVE_AS]
+                      [--access-biosample-from-accession] [--gui]
 
   __      _       _        __            _
  / _| ___| |_ ___| |__    / _| ___  __ _| |_ _   _ _ __ ___  ___
 | |_ / _ \ __/ __| '_ \  | |_ / _ \/ _` | __| | | | '__/ _ \/ __|
 |  _|  __/ || (__| | | | |  _|  __/ (_| | |_| |_| | | |  __/\__ \
 |_|  \___|\__\___|_| |_| |_|  \___|\__,_|\__|\__,_|_|  \___||___/
 
 Fetch features from a list of accession or BioSample numbers.
 
 Help:
   -h, --help            Show this help message and exit.
+  -v, --version         Show program's version number and exit
 
 Required:
   -i INPUT, --input INPUT
                         Path to input file with list of unique identifiers (UIDs).
                         The user should provide the list of UIDs in a txt or xlsx file.
   -t TYPE, --type TYPE  Type of unique identifier: `accession` or `biosample`.
                         The `biosample` option fetches the information of the most
@@ -57,27 +58,27 @@
 ```
 
 ## Usage examples
 
 1. The simplest command. The output is in the current working directoy.
 
 ```bash
-fetcher -i path/to/list.txt -t accession -e email@address.com
+fetch_features -i path/to/list.txt -t accession -e email@address.com
 ```
 
 2. In this example, the output is in your Documents.
 
 ```bash
-fetcher -i path/to/list.txt -t accession -e email@address.com -o ~/Documents
+fetch_features -i path/to/list.txt -t accession -e email@address.com -o ~/Documents
 ```
 
 3. If you prefer the GUI version.
 
 ```bash
-fetcher --gui
+fetch_features --gui
 ```
 
 <p align="center">
   <picture>
     <img src="./images/fetch_features_gui.png">
   </picture>
 </p>
```

### Comparing `fetch_features-0.2.1/images/fetch_features_gui.png` & `fetch_features-0.2.2/images/fetch_features_gui.png`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.1/pyproject.toml` & `fetch_features-0.2.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fetch_features"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     {name = "Ivan Muñoz-Gutierrez", email = "ivan.munoz.gutierrez@gmail.com"},
 ]
 description = "Fetch features from a list of accession or BioSample numbers."
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = [
@@ -29,14 +29,15 @@
     "darkdetect==0.8.0",
     "numpy==1.24.3",
     "pandas==2.0.1",
     "python-dateutil==2.8.2",
     "pytz==2023.3",
     "six==1.16.0",
     "tzdata==2023.3",
+    "toml==0.10.2"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ivanmugu/fetch_features"
 
 [project.scripts]
-fetcher = "fetcher.__main__:main"
+fetch_features = "fetcher.__main__:main"
```

### Comparing `fetch_features-0.2.1/src/fetch_features.egg-info/PKG-INFO` & `fetch_features-0.2.2/src/fetch_features.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetch-features
-Version: 0.2.1
+Version: 0.2.2
 Summary: Fetch features from a list of accession or BioSample numbers.
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/fetch_features
 Keywords: unique identifier,accession number,BioSample number,GenBank,sequence features
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -28,33 +28,34 @@
 ```
 
 ## Usage and options
 
 To view all the options run:
 
 ```bash
-fetcher --help
+fetch_features --help
 ```
 
 Output:
 
 ```
-usage: fetcher [-h] [-i, INPUT] [-t, TYPE] [-e, EMAIL] [-o, OUTPUT] [-s, SAVE-AS]
-               [--access-biosample-from-accession] [--gui]
+usage: fetch_features [-h] [-v] [-i INPUT] [-t TYPE] [-e EMAIL] [-o OUTPUT] [-s SAVE_AS]
+                      [--access-biosample-from-accession] [--gui]
 
   __      _       _        __            _
  / _| ___| |_ ___| |__    / _| ___  __ _| |_ _   _ _ __ ___  ___
 | |_ / _ \ __/ __| '_ \  | |_ / _ \/ _` | __| | | | '__/ _ \/ __|
 |  _|  __/ || (__| | | | |  _|  __/ (_| | |_| |_| | | |  __/\__ \
 |_|  \___|\__\___|_| |_| |_|  \___|\__,_|\__|\__,_|_|  \___||___/
 
 Fetch features from a list of accession or BioSample numbers.
 
 Help:
   -h, --help            Show this help message and exit.
+  -v, --version         Show program's version number and exit
 
 Required:
   -i INPUT, --input INPUT
                         Path to input file with list of unique identifiers (UIDs).
                         The user should provide the list of UIDs in a txt or xlsx file.
   -t TYPE, --type TYPE  Type of unique identifier: `accession` or `biosample`.
                         The `biosample` option fetches the information of the most
@@ -74,27 +75,27 @@
 ```
 
 ## Usage examples
 
 1. The simplest command. The output is in the current working directoy.
 
 ```bash
-fetcher -i path/to/list.txt -t accession -e email@address.com
+fetch_features -i path/to/list.txt -t accession -e email@address.com
 ```
 
 2. In this example, the output is in your Documents.
 
 ```bash
-fetcher -i path/to/list.txt -t accession -e email@address.com -o ~/Documents
+fetch_features -i path/to/list.txt -t accession -e email@address.com -o ~/Documents
 ```
 
 3. If you prefer the GUI version.
 
 ```bash
-fetcher --gui
+fetch_features --gui
 ```
 
 <p align="center">
   <picture>
     <img src="./images/fetch_features_gui.png">
   </picture>
 </p>
```

### Comparing `fetch_features-0.2.1/src/fetcher/__main__.py` & `fetch_features-0.2.2/src/fetcher/__main__.py`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.1/src/fetcher/access_genbank.py` & `fetch_features-0.2.2/src/fetcher/access_genbank.py`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.1/src/fetcher/database.py` & `fetch_features-0.2.2/src/fetcher/database.py`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.1/src/fetcher/gui.py` & `fetch_features-0.2.2/src/fetcher/gui.py`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.1/src/fetcher/user_input.py` & `fetch_features-0.2.2/src/fetcher/user_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,20 @@
 import sys
 import argparse
 from argparse import Namespace
 import textwrap
 from pathlib import Path
 import re
 from typing import Union
+import pkg_resources
 
-
-# Usage mesasge.
-usage_msg = (
-    "fetcher [-h] [-i, INPUT] [-t, TYPE] [-e, EMAIL] [-o, OUTPUT] " +
-    "[-s, SAVE-AS]\n" +
-    "               [--access-biosample-from-accession] [--gui]"
-)
 # Description message.
 description_msg = r"""
-  __      _       _        __            _                       
- / _| ___| |_ ___| |__    / _| ___  __ _| |_ _   _ _ __ ___  ___ 
+  __      _       _        __            _
+ / _| ___| |_ ___| |__    / _| ___  __ _| |_ _   _ _ __ ___  ___
 | |_ / _ \ __/ __| '_ \  | |_ / _ \/ _` | __| | | | '__/ _ \/ __|
 |  _|  __/ || (__| | | | |  _|  __/ (_| | |_| |_| | | |  __/\__ \
 |_|  \___|\__\___|_| |_| |_|  \___|\__,_|\__|\__,_|_|  \___||___/
 
 Fetch features from a list of accession or BioSample numbers.
 """
 
@@ -42,27 +36,30 @@
 3. If you prefer the GUI version.
 $ fetcher --gui
 """
 
 
 class UserInput:
     """Class to save user input via the commmand line."""
+    # TODO: include a `type` option for the type of identifiers in the list.
 
     def __init__(
             self,
             infile: Union[Path, None] = None,
             extention_infile: Union[str, None] = None,
+            uid_type: Union[str, None] = None,
             email: Union[str, None] = None,
             output_folder: Path = Path('.'),
             access_biosample_from_accession: bool = False,
             save_as: str = 'csv',
             use_gui: bool = False
     ):
         self.infile = infile
         self.extention_infile = extention_infile
+        self.uid_type = uid_type
         self.email = email
         self.output_folder = output_folder
         self.access_biosample_from_accession = access_biosample_from_accession
         self.save_as = save_as
         self.use_gui = use_gui
 
 
@@ -72,16 +69,16 @@
     Returns
     -------
     user_input : UserInput object
     """
     # Parse arguments and provide help.
     parser = argparse.ArgumentParser(
         add_help=False,
-        prog='fetcher',
-        usage=usage_msg,
+        prog='fetch_features',
+        # usage=usage_msg,
         formatter_class=argparse.RawTextHelpFormatter,
         description=description_msg,
         epilog=textwrap.dedent(epilog_msg)
     )
     # Make argument groups.
     helper = parser.add_argument_group('Help')
     required = parser.add_argument_group('Required')
@@ -90,14 +87,20 @@
     # Help argument #
     # ############# #
     # Make help argument.
     helper.add_argument(
         '-h', '--help', action='help',
         help='Show this help message and exit.',
     )
+    prog_version = pkg_resources.get_distribution('fetch_features').version
+    helper.add_argument(
+        '-v', '--version', action='version',
+        version=f'%(prog)s {prog_version}',
+        help="Show program's version number and exit"
+    )
 
     # ################## #
     # Required arguments #
     # ################## #
     # Make input argument.
     required.add_argument(
         '-i', '--input',
@@ -151,15 +154,17 @@
         '--gui',
         action='store_true',
         help="Activate GUI."
     )
     # ################################################################ #
     # Parse command line arguments and store info in a UserInput class #
     # ################################################################ #
-    user_input = get_command_line_input(parser.parse_args())
+    args = parser.parse_args()
+    print(args.__dict__)
+    user_input = get_command_line_input(args)
     check_required_and_gui_arguments(user_input)
 
     return user_input
 
 
 def get_command_line_input(command_line_input: Namespace) -> UserInput:
     """Get user input from command line."""
```

