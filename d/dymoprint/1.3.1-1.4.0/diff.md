# Comparing `tmp/dymoprint-1.3.1.tar.gz` & `tmp/dymoprint-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dymoprint-1.3.1.tar", last modified: Mon Jan  2 19:58:31 2023, max compression
+gzip compressed data, was "dymoprint-1.4.0.tar", last modified: Sat May 27 16:20:17 2023, max compression
```

## Comparing `dymoprint-1.3.1.tar` & `dymoprint-1.4.0.tar`

### file list

```diff
@@ -1,45 +1,58 @@
-drwxrwxr-x   0 mares     (1000) mares     (1000)        0 2023-01-02 19:58:31.036078 dymoprint-1.3.1/
-drwxrwxr-x   0 mares     (1000) mares     (1000)        0 2023-01-02 19:58:31.024077 dymoprint-1.3.1/.github/
-drwxrwxr-x   0 mares     (1000) mares     (1000)        0 2023-01-02 19:58:31.024077 dymoprint-1.3.1/.github/workflows/
--rw-rw-r--   0 mares     (1000) mares     (1000)      834 2021-03-24 22:00:16.000000 dymoprint-1.3.1/.github/workflows/pypi-publish.yml
--rw-rw-r--   0 mares     (1000) mares     (1000)      545 2021-03-24 22:00:16.000000 dymoprint-1.3.1/.github/workflows/tests.yml
--rw-rw-r--   0 mares     (1000) mares     (1000)      813 2021-03-23 18:36:17.000000 dymoprint-1.3.1/.gitignore
--rw-rw-r--   0 mares     (1000) mares     (1000)      595 2023-01-02 17:58:35.000000 dymoprint-1.3.1/.pre-commit-config.yaml
--rw-rw-r--   0 mares     (1000) mares     (1000)      499 2023-01-02 13:23:38.000000 dymoprint-1.3.1/91-dymo-labelmanager-pnp.rules
--rw-rw-r--   0 mares     (1000) mares     (1000)    11324 2021-03-23 18:36:17.000000 dymoprint-1.3.1/LICENSE
--rw-rw-r--   0 mares     (1000) mares     (1000)     5714 2023-01-02 19:58:31.036078 dymoprint-1.3.1/PKG-INFO
--rw-rw-r--   0 mares     (1000) mares     (1000)     4847 2022-11-13 18:43:28.000000 dymoprint-1.3.1/README.md
--rwxrwxr-x   0 mares     (1000) mares     (1000)      536 2020-08-30 18:44:23.000000 dymoprint-1.3.1/TODO.md
-drwxrwxr-x   0 mares     (1000) mares     (1000)        0 2023-01-02 19:58:31.024077 dymoprint-1.3.1/data/
-drwxrwxr-x   0 mares     (1000) mares     (1000)        0 2023-01-02 19:58:31.032077 dymoprint-1.3.1/data/fonts/
--rw-rw-r--   0 mares     (1000) mares     (1000)   690516 2020-09-05 20:36:11.000000 dymoprint-1.3.1/data/fonts/Carlito-Bold.ttf
--rw-rw-r--   0 mares     (1000) mares     (1000)   816716 2020-09-05 20:36:11.000000 dymoprint-1.3.1/data/fonts/Carlito-BoldItalic.ttf
--rw-rw-r--   0 mares     (1000) mares     (1000)   623416 2020-09-05 20:36:11.000000 dymoprint-1.3.1/data/fonts/Carlito-Italic.ttf
--rw-rw-r--   0 mares     (1000) mares     (1000)   635996 2020-09-05 20:36:11.000000 dymoprint-1.3.1/data/fonts/Carlito-Regular.ttf
--rw-rw-r--   0 mares     (1000) mares     (1000)     4247 2021-03-23 18:36:17.000000 dymoprint-1.3.1/data/fonts/LICENSE
--rw-rw-r--   0 mares     (1000) mares     (1000)        0 2020-08-31 23:36:12.000000 dymoprint-1.3.1/data/fonts/__init__.py
--rw-rw-r--   0 mares     (1000) mares     (1000)      184 2020-08-30 14:15:04.000000 dymoprint-1.3.1/dymo-labelmanager-pnp.conf
--rw-rw-r--   0 mares     (1000) mares     (1000)      302 2020-09-05 20:52:50.000000 dymoprint-1.3.1/dymoprint.ini
--rw-rw-r--   0 mares     (1000) mares     (1000)     1833 2021-03-24 00:11:19.000000 dymoprint-1.3.1/pyproject.toml
--rw-rw-r--   0 mares     (1000) mares     (1000)     1337 2023-01-02 19:58:31.036078 dymoprint-1.3.1/setup.cfg
--rw-rw-r--   0 mares     (1000) mares     (1000)      535 2021-03-23 18:36:17.000000 dymoprint-1.3.1/setup.py
-drwxrwxr-x   0 mares     (1000) mares     (1000)        0 2023-01-02 19:58:31.032077 dymoprint-1.3.1/src/
--rw-rw-r--   0 mares     (1000) mares     (1000)      533 2020-09-05 21:05:25.000000 dymoprint-1.3.1/src/README.md
--rw-rw-r--   0 mares     (1000) mares     (1000)        0 2020-09-05 22:31:57.000000 dymoprint-1.3.1/src/__init__.py
-drwxrwxr-x   0 mares     (1000) mares     (1000)        0 2023-01-02 19:58:31.036078 dymoprint-1.3.1/src/dymoprint/
--rw-rw-r--   0 mares     (1000) mares     (1000)      106 2021-03-23 18:36:17.000000 dymoprint-1.3.1/src/dymoprint/__init__.py
--rwxrwxr-x   0 mares     (1000) mares     (1000)     3891 2021-03-23 18:36:17.000000 dymoprint-1.3.1/src/dymoprint/barcode_writer.py
--rwxrwxr-x   0 mares     (1000) mares     (1000)    11131 2023-01-02 19:52:16.000000 dymoprint-1.3.1/src/dymoprint/command_line.py
--rwxrwxr-x   0 mares     (1000) mares     (1000)     1575 2023-01-02 19:35:17.000000 dymoprint-1.3.1/src/dymoprint/constants.py
--rw-rw-r--   0 mares     (1000) mares     (1000)     1149 2021-03-23 18:36:17.000000 dymoprint-1.3.1/src/dymoprint/font_config.py
--rwxrwxr-x   0 mares     (1000) mares     (1000)     7349 2023-01-02 19:54:03.000000 dymoprint-1.3.1/src/dymoprint/labeler.py
--rw-rw-r--   0 mares     (1000) mares     (1000)      256 2021-03-23 18:36:17.000000 dymoprint-1.3.1/src/dymoprint/metadata.py
--rw-rw-r--   0 mares     (1000) mares     (1000)      961 2021-03-23 22:43:26.000000 dymoprint-1.3.1/src/dymoprint/unicode_blocks.py
--rwxrwxr-x   0 mares     (1000) mares     (1000)     3342 2021-03-23 18:36:17.000000 dymoprint-1.3.1/src/dymoprint/utils.py
-drwxrwxr-x   0 mares     (1000) mares     (1000)        0 2023-01-02 19:58:31.036078 dymoprint-1.3.1/src/dymoprint.egg-info/
--rw-rw-r--   0 mares     (1000) mares     (1000)     5714 2023-01-02 19:58:30.000000 dymoprint-1.3.1/src/dymoprint.egg-info/PKG-INFO
--rw-rw-r--   0 mares     (1000) mares     (1000)      918 2023-01-02 19:58:31.000000 dymoprint-1.3.1/src/dymoprint.egg-info/SOURCES.txt
--rw-rw-r--   0 mares     (1000) mares     (1000)        1 2023-01-02 19:58:30.000000 dymoprint-1.3.1/src/dymoprint.egg-info/dependency_links.txt
--rw-rw-r--   0 mares     (1000) mares     (1000)       58 2023-01-02 19:58:30.000000 dymoprint-1.3.1/src/dymoprint.egg-info/entry_points.txt
--rw-rw-r--   0 mares     (1000) mares     (1000)      123 2023-01-02 19:58:30.000000 dymoprint-1.3.1/src/dymoprint.egg-info/requires.txt
--rw-rw-r--   0 mares     (1000) mares     (1000)       26 2023-01-02 19:58:30.000000 dymoprint-1.3.1/src/dymoprint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.951106 dymoprint-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.943106 dymoprint-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.943106 dymoprint-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-27 16:20:01.000000 dymoprint-1.4.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-27 16:20:01.000000 dymoprint-1.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-27 16:20:01.000000 dymoprint-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-27 16:20:01.000000 dymoprint-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-27 16:20:01.000000 dymoprint-1.4.0/91-dymo-labelmanager-pnp.rules
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-05-27 16:20:01.000000 dymoprint-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-27 16:20:17.951106 dymoprint-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-27 16:20:01.000000 dymoprint-1.4.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-05-27 16:20:01.000000 dymoprint-1.4.0/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.943106 dymoprint-1.4.0/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.947106 dymoprint-1.4.0/data/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   690516 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/Carlito-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   816716 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/Carlito-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   623416 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/Carlito-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   635996 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/Carlito-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/barcode_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/gui_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/img_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/qr_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/txt_icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.947106 dymoprint-1.4.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-05-27 16:20:01.000000 dymoprint-1.4.0/doc/DymoPrint_example_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40573 2023-05-27 16:20:01.000000 dymoprint-1.4.0/doc/DymoPrint_example_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-05-27 16:20:01.000000 dymoprint-1.4.0/doc/DymoPrint_example_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-27 16:20:01.000000 dymoprint-1.4.0/dymo-labelmanager-pnp.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-27 16:20:01.000000 dymoprint-1.4.0/dymoprint.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-27 16:20:01.000000 dymoprint-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-27 16:20:17.951106 dymoprint-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-27 16:20:01.000000 dymoprint-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.951106 dymoprint-1.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.951106 dymoprint-1.4.0/src/dymoprint/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3891 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/barcode_writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5638 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/command_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1575 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12575 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/dymo_print_engines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/font_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7501 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/labeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/q_dymo_label_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/q_dymo_labels_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/unicode_blocks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3360 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.951106 dymoprint-1.4.0/src/dymoprint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-27 16:20:17.000000 dymoprint-1.4.0/src/dymoprint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-27 16:20:17.000000 dymoprint-1.4.0/src/dymoprint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 16:20:17.000000 dymoprint-1.4.0/src/dymoprint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-27 16:20:17.000000 dymoprint-1.4.0/src/dymoprint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-27 16:20:17.000000 dymoprint-1.4.0/src/dymoprint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-27 16:20:17.000000 dymoprint-1.4.0/src/dymoprint.egg-info/top_level.txt
```

### Comparing `dymoprint-1.3.1/.github/workflows/pypi-publish.yml` & `dymoprint-1.4.0/.github/workflows/pypi-publish.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# This workflow will upload a Python Package using Twine when a release is created
-# For more information see: https://help.github.com/en/actions/language-and-framework-guides/using-python-with-github-actions#publishing-to-package-registries
-
 name: Upload Python Package
 
 on:
   release:
     types: [created]
+  workflow_dispatch:
 
 jobs:
   deploy:
-
     runs-on: ubuntu-latest
-
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
+      with:
+        fetch-depth: 0
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: '3.x'
-    - name: Install dependencies
+    - name: Build
       run: |
-        python -m pip install --upgrade pip
-        pip install tox tox-gh-actions
-    - name: Build and publish
-      env:
-        TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
-        TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
+        python -m pip install --upgrade pip build twine
+        python -m build
+    - name: Test wheels
       run: |
-        tox -e publish -- --repository pypi
+        python -m twine check dist/*
+    - name: Publish
+      uses: pypa/gh-action-pypi-publish@v1.8.6
+      with:
+        user: ${{ secrets.PYPI_USERNAME }}
+        password: ${{ secrets.PYPI_PASSWORD }}
```

### Comparing `dymoprint-1.3.1/.github/workflows/tests.yml` & `dymoprint-1.4.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dymoprint-1.3.1/.gitignore` & `dymoprint-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dymoprint-1.3.1/.pre-commit-config.yaml` & `dymoprint-1.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dymoprint-1.3.1/LICENSE` & `dymoprint-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dymoprint-1.3.1/PKG-INFO` & `dymoprint-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dymoprint
-Version: 1.3.1
+Version: 1.4.0
 Summary: Linux Software to print with LabelManager PnP from Dymo
 Home-page: https://github.com/computerlyrik/dymoprint
 Author: Sebastian J. Bronner
 Author-email: waschtl@sbronner.com
 Maintainer: Ben Mares
 Maintainer-email: services-dymoprint@tensorial.com
 License: Apache License 2.0
@@ -35,14 +35,15 @@
 
 * Works on python 3.7 and up
 * Supports text printing
 * Supports qr code printing
 * Supports barcode printing
 * Supports image printing
 * Supports combined barcode / qrcode and text printing
+* GUI Application based on PyQt6 - expanded combinations
 
 ## Installation
 
 It is recommended to install dymoprint with [pipx](https://pypa.github.io/pipx/) so that it runs in an isolated virtual environment:
 
 ```bash
 pipx install dymoprint
@@ -176,14 +177,60 @@
 
 Any picture with JPEG standard may be printed. Beware it will be downsized to tape.
 
 ```dymoprint -p mypic.jpg ""```
 
 Take care of the trailing "" - you may enter text here which gets printed in front of the image
 
+## GUI
+
+### Run DymoPrint GUI
+
+```dymoprint_gui```
+
+
+### Features
+* Live preview
+* margin settings
+* type size selector
+* visualization of tape color schema
+* the ability to freely arrange the content using the "Node" list
+  * Text Node:
+    * payload text - can be multi-line
+    * font selector
+    * font scaling - the percentage of line-height
+    * frame border width steering
+  * Qr Node:
+    * payload text
+  * BarCode Node:
+    * payload text
+    * codding selector
+  * Image Node:
+    * path to file
+
+Nodes can be freely arranged, simply drag&drop rows on the list.
+To add or delete the node from the label - right-click on the list and select the action from the context menu.
+To print - click the print button.
+
+### Example
+
+Example 1: multiple text + QR code
+
+![alt](doc/DymoPrint_example_1.png)
+
+Example 2: two images + text with frame, white on red
+
+![alt](doc/DymoPrint_example_2.png)
+
+Example 3: barcode, text, image
+
+![alt](doc/DymoPrint_example_3.png)
+
+
+
 ## Development
 
 Besides the travis-ci one should run the following command on a feature implemention or change to ensure the same outcome on a real device:
 
 ```bash
 dymoprint Tst && \
 dymoprint -qr Tst && \
@@ -191,17 +238,17 @@
 dymoprint -qr qrencoded "qr_txt" && \
 dymoprint -c code128 Test "bc_txt"
 ```
 
 ### ToDo
 
 * (?)support multiple ProductIDs (1001, 1002) -> use usb-modeswitch?
-* put everything in classes that would need to be used by a GUI
+* ~~put everything in classes that would need to be used by a GUI~~
 * ~~for more options use command line parser framework~~
 * ~~allow selection of font with command line options~~
-* allow font size specification with command line option (points, pixels?)
+* ~~allow font size specification with command line option (points, pixels?)~~
 * ~~provide an option to show a preview of what the label will look like~~
 * ~~read and write a .dymoprint file containing user preferences~~
 * ~~print barcodes~~
 * ~~print graphics~~
 * ~~plot frame around label~~
 * vertical print
```

### Comparing `dymoprint-1.3.1/README.md` & `dymoprint-1.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 * Works on python 3.7 and up
 * Supports text printing
 * Supports qr code printing
 * Supports barcode printing
 * Supports image printing
 * Supports combined barcode / qrcode and text printing
+* GUI Application based on PyQt6 - expanded combinations
 
 ## Installation
 
 It is recommended to install dymoprint with [pipx](https://pypa.github.io/pipx/) so that it runs in an isolated virtual environment:
 
 ```bash
 pipx install dymoprint
@@ -154,14 +155,60 @@
 
 Any picture with JPEG standard may be printed. Beware it will be downsized to tape.
 
 ```dymoprint -p mypic.jpg ""```
 
 Take care of the trailing "" - you may enter text here which gets printed in front of the image
 
+## GUI
+
+### Run DymoPrint GUI
+
+```dymoprint_gui```
+
+
+### Features
+* Live preview
+* margin settings
+* type size selector
+* visualization of tape color schema
+* the ability to freely arrange the content using the "Node" list
+  * Text Node:
+    * payload text - can be multi-line
+    * font selector
+    * font scaling - the percentage of line-height
+    * frame border width steering
+  * Qr Node:
+    * payload text
+  * BarCode Node:
+    * payload text
+    * codding selector
+  * Image Node:
+    * path to file
+
+Nodes can be freely arranged, simply drag&drop rows on the list.
+To add or delete the node from the label - right-click on the list and select the action from the context menu.
+To print - click the print button.
+
+### Example
+
+Example 1: multiple text + QR code
+
+![alt](doc/DymoPrint_example_1.png)
+
+Example 2: two images + text with frame, white on red
+
+![alt](doc/DymoPrint_example_2.png)
+
+Example 3: barcode, text, image
+
+![alt](doc/DymoPrint_example_3.png)
+
+
+
 ## Development
 
 Besides the travis-ci one should run the following command on a feature implemention or change to ensure the same outcome on a real device:
 
 ```bash
 dymoprint Tst && \
 dymoprint -qr Tst && \
@@ -169,17 +216,17 @@
 dymoprint -qr qrencoded "qr_txt" && \
 dymoprint -c code128 Test "bc_txt"
 ```
 
 ### ToDo
 
 * (?)support multiple ProductIDs (1001, 1002) -> use usb-modeswitch?
-* put everything in classes that would need to be used by a GUI
+* ~~put everything in classes that would need to be used by a GUI~~
 * ~~for more options use command line parser framework~~
 * ~~allow selection of font with command line options~~
-* allow font size specification with command line option (points, pixels?)
+* ~~allow font size specification with command line option (points, pixels?)~~
 * ~~provide an option to show a preview of what the label will look like~~
 * ~~read and write a .dymoprint file containing user preferences~~
 * ~~print barcodes~~
 * ~~print graphics~~
 * ~~plot frame around label~~
 * vertical print
```

### Comparing `dymoprint-1.3.1/TODO.md` & `dymoprint-1.4.0/TODO.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 - [ ] support multiple ProductIDs (1001, 1002) -> use usb-modeswitch?
-- [ ] put everything in classes that would need to be used by a GUI
+- [x] put everything in classes that would need to be used by a GUI
 - [x] for more options use command line parser framework
 - [x] allow selection of font with command line options
-- [ ] allow font size specification with command line option (points, pixels?)
+- [x] allow font size specification with command line option (points, pixels?)
 - [x] provide an option to show a preview of what the label will look like
 - [x] read and write a .dymoprint file containing user preferences
 - [ ] print graphics and barcodes
 - [x] plot frame around label
```

### Comparing `dymoprint-1.3.1/data/fonts/Carlito-Bold.ttf` & `dymoprint-1.4.0/data/fonts/Carlito-Bold.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-1.3.1/data/fonts/Carlito-BoldItalic.ttf` & `dymoprint-1.4.0/data/fonts/Carlito-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-1.3.1/data/fonts/Carlito-Italic.ttf` & `dymoprint-1.4.0/data/fonts/Carlito-Italic.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-1.3.1/data/fonts/Carlito-Regular.ttf` & `dymoprint-1.4.0/data/fonts/Carlito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-1.3.1/data/fonts/LICENSE` & `dymoprint-1.4.0/data/fonts/LICENSE`

 * *Files identical despite different names*

### Comparing `dymoprint-1.3.1/pyproject.toml` & `dymoprint-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dymoprint-1.3.1/setup.cfg` & `dymoprint-1.4.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -32,25 +32,28 @@
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	appdirs
 	Pillow>=8.1.2,<10
 	PyQRCode>=1.2.1,<2
 	python-barcode>=0.13.1,<1
 	pyusb
+	PyQt6
+	PyQt6-tools
 python_requires = >=3.7,<4
 setup_requires = 
 	setuptools_scm
 
 [options.package_data]
 dymoprint_fonts = *
 
 [bdist_wheel]
 universal = 1
 
 [options.entry_points]
 console_scripts = 
 	dymoprint = dymoprint.command_line:main
+	dymoprint_gui = dymoprint.gui:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `dymoprint-1.3.1/setup.py` & `dymoprint-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `dymoprint-1.3.1/src/README.md` & `dymoprint-1.4.0/src/README.md`

 * *Files identical despite different names*

### Comparing `dymoprint-1.3.1/src/dymoprint/barcode_writer.py` & `dymoprint-1.4.0/src/dymoprint/barcode_writer.py`

 * *Files identical despite different names*

### Comparing `dymoprint-1.3.1/src/dymoprint/constants.py` & `dymoprint-1.4.0/src/dymoprint/constants.py`

 * *Files identical despite different names*

### Comparing `dymoprint-1.3.1/src/dymoprint/font_config.py` & `dymoprint-1.4.0/src/dymoprint/font_config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import re
 from configparser import ConfigParser
 
 from appdirs import user_config_dir
 
 import dymoprint_fonts
 
 from .constants import DEFAULT_FONT_STYLE, FLAG_TO_STYLE
@@ -27,7 +28,17 @@
         # reading FONTS section
         if not "FONTS" in conf.sections():
             die('! config file "%s" not valid. Please change or remove.' % CONFIG_FILE)
         for style in style_to_file.keys():
             style_to_file[style] = conf.get("FONTS", style)
 
     return style_to_file[FLAG_TO_STYLE.get(flag, DEFAULT_FONT_STYLE)]
+
+
+def parse_fonts() -> dict:
+    DEFAULT_FONT_DIR = os.path.dirname(dymoprint_fonts.__file__)
+    fonts = list()
+    for f in os.listdir(DEFAULT_FONT_DIR):
+        m = re.match(r"(.*-.*).ttf", f)
+        if m:
+            fonts.append((m.group(1), os.path.join(DEFAULT_FONT_DIR, f)))
+    return fonts
```

### Comparing `dymoprint-1.3.1/src/dymoprint/labeler.py` & `dymoprint-1.4.0/src/dymoprint/labeler.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,27 +22,30 @@
     with 'HLF' or 'MLF' in parentheses.
 
     A partial reference of the protocol is the Technical Reference for the
     LabelWriter 450:
     <https://download.dymo.com/dymo/technical-data-sheets/LW%20450%20Series%20Technical%20Reference.pdf>
     """
 
-    _MAX_BYTES_PER_LINE = 8  # 64 pixels on a 12mm tape
+    @staticmethod
+    def max_bytes_per_line(tape_size=12):
+        return int(8 * tape_size / 12)
 
     # Max number of print lines to send before waiting for a response. This helps
     # to avoid timeouts due to differences between data transfer and
     # printer speeds. I added this because I kept getting "IOError: [Errno
     # 110] Connection timed out" with long labels. Using dev.default_timeout
     # (1000) and the transfer speeds available in the descriptors somewhere, a
     # sensible timeout can also be calculated dynamically.
     synwait: Optional[int]
 
-    def __init__(self, devout, devin, synwait=None):
+    def __init__(self, devout, devin, synwait=None, tape_size=12):
         """Initialize the LabelManager object. (HLF)"""
 
+        self.tape_size = tape_size
         self.cmd: list[int] = []
         self.response = False
         self.bytesPerLine_ = None
         self.dotTab_ = 0
         self.maxLines = 200
         self.devout = devout
         self.devin = devin
@@ -114,15 +117,15 @@
         cmd = [ESC, ord("A")]
         self.buildCommand(cmd)
         self.response = True
 
     def dotTab(self, value):
         """Set the bias text height, in bytes. (MLF)"""
 
-        if value < 0 or value > self._MAX_BYTES_PER_LINE:
+        if value < 0 or value > self.max_bytes_per_line(self.tape_size):
             raise ValueError
         cmd = [ESC, ord("B"), value]
         self.buildCommand(cmd)
         self.dotTab_ = value
         self.bytesPerLine_ = None
 
     def tapeColor(self, value):
@@ -132,15 +135,15 @@
             raise ValueError
         cmd = [ESC, ord("C"), value]
         self.buildCommand(cmd)
 
     def bytesPerLine(self, value):
         """Set the number of bytes sent in the following lines. (MLF)"""
 
-        if value < 0 or value + self.dotTab_ > self._MAX_BYTES_PER_LINE:
+        if value < 0 or value + self.dotTab_ > self.max_bytes_per_line(self.tape_size):
             raise ValueError
         if value == self.bytesPerLine_:
             return
         cmd = [ESC, ord("D"), value]
         self.buildCommand(cmd)
         self.bytesPerLine_ = value
 
@@ -157,16 +160,16 @@
         cmd = [SYN] + value
         self.buildCommand(cmd)
 
     def chainMark(self):
         """Set Chain Mark. (MLF)"""
 
         self.dotTab(0)
-        self.bytesPerLine(self._MAX_BYTES_PER_LINE)
-        self.line([0x99] * self._MAX_BYTES_PER_LINE)
+        self.bytesPerLine(self.max_bytes_per_line(self.tape_size))
+        self.line([0x99] * self.max_bytes_per_line(self.tape_size))
 
     def skipLines(self, value):
         """Set number of lines of white to print. (MLF)"""
 
         if value <= 0:
             raise ValueError
         self.bytesPerLine(0)
```

### Comparing `dymoprint-1.3.1/src/dymoprint/unicode_blocks.py` & `dymoprint-1.4.0/src/dymoprint/unicode_blocks.py`

 * *Files identical despite different names*

### Comparing `dymoprint-1.3.1/src/dymoprint/utils.py` & `dymoprint-1.4.0/src/dymoprint/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 import os
 import re
 import struct
 import subprocess
 import sys
 import termios
 import textwrap
+from typing import NoReturn
 
 from PIL import ImageDraw
 
 
-def die(message=None):
+def die(message=None) -> NoReturn:
     if message:
         print(message, file=sys.stderr)
+        raise RuntimeError(message)
     sys.exit(1)
 
 
 def pprint(par, fd=sys.stdout):
     rows, columns = struct.unpack(
         "HH", fcntl.ioctl(sys.stderr, termios.TIOCGWINSZ, struct.pack("HH", 0, 0))
     )
@@ -71,28 +73,25 @@
         for filename in filenames:
             filepath = os.path.join(dirpath, filename)
             if os.stat(filepath).st_rdev == devnum:
                 return filepath
 
 
 def access_error(dev):
-    pprint("You do not have sufficient access to the device file %s:" % dev, sys.stderr)
+    die("You do not have sufficient access to the device file %s:" % dev, sys.stderr)
     subprocess.call(["ls", "-l", dev], stdout=sys.stderr)
     print(file=sys.stderr)
     filename = "91-dymo-labelmanager-pnp.rules"
-    pprint(
-        "You probably want to add a rule like one of the following in /etc/udev/rules.d/"
-        + filename,
-        sys.stderr,
+    die(
+        f"You probably want to add a rule like one of the following in /etc/udev/rules.d/{filename}"
     )
     with open(filename, "r") as fin:
         print(fin.read(), file=sys.stderr)
-    pprint(
+    die(
         "Following that, restart udev and re-plug your device. See README.md for details",
-        sys.stderr,
     )
 
 
 """ scaling pixel up, input: (x,y),scale-factor """
 
 
 def scaling(pix, sc):
```

### Comparing `dymoprint-1.3.1/src/dymoprint.egg-info/PKG-INFO` & `dymoprint-1.4.0/src/dymoprint.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dymoprint
-Version: 1.3.1
+Version: 1.4.0
 Summary: Linux Software to print with LabelManager PnP from Dymo
 Home-page: https://github.com/computerlyrik/dymoprint
 Author: Sebastian J. Bronner
 Author-email: waschtl@sbronner.com
 Maintainer: Ben Mares
 Maintainer-email: services-dymoprint@tensorial.com
 License: Apache License 2.0
@@ -35,14 +35,15 @@
 
 * Works on python 3.7 and up
 * Supports text printing
 * Supports qr code printing
 * Supports barcode printing
 * Supports image printing
 * Supports combined barcode / qrcode and text printing
+* GUI Application based on PyQt6 - expanded combinations
 
 ## Installation
 
 It is recommended to install dymoprint with [pipx](https://pypa.github.io/pipx/) so that it runs in an isolated virtual environment:
 
 ```bash
 pipx install dymoprint
@@ -176,14 +177,60 @@
 
 Any picture with JPEG standard may be printed. Beware it will be downsized to tape.
 
 ```dymoprint -p mypic.jpg ""```
 
 Take care of the trailing "" - you may enter text here which gets printed in front of the image
 
+## GUI
+
+### Run DymoPrint GUI
+
+```dymoprint_gui```
+
+
+### Features
+* Live preview
+* margin settings
+* type size selector
+* visualization of tape color schema
+* the ability to freely arrange the content using the "Node" list
+  * Text Node:
+    * payload text - can be multi-line
+    * font selector
+    * font scaling - the percentage of line-height
+    * frame border width steering
+  * Qr Node:
+    * payload text
+  * BarCode Node:
+    * payload text
+    * codding selector
+  * Image Node:
+    * path to file
+
+Nodes can be freely arranged, simply drag&drop rows on the list.
+To add or delete the node from the label - right-click on the list and select the action from the context menu.
+To print - click the print button.
+
+### Example
+
+Example 1: multiple text + QR code
+
+![alt](doc/DymoPrint_example_1.png)
+
+Example 2: two images + text with frame, white on red
+
+![alt](doc/DymoPrint_example_2.png)
+
+Example 3: barcode, text, image
+
+![alt](doc/DymoPrint_example_3.png)
+
+
+
 ## Development
 
 Besides the travis-ci one should run the following command on a feature implemention or change to ensure the same outcome on a real device:
 
 ```bash
 dymoprint Tst && \
 dymoprint -qr Tst && \
@@ -191,17 +238,17 @@
 dymoprint -qr qrencoded "qr_txt" && \
 dymoprint -c code128 Test "bc_txt"
 ```
 
 ### ToDo
 
 * (?)support multiple ProductIDs (1001, 1002) -> use usb-modeswitch?
-* put everything in classes that would need to be used by a GUI
+* ~~put everything in classes that would need to be used by a GUI~~
 * ~~for more options use command line parser framework~~
 * ~~allow selection of font with command line options~~
-* allow font size specification with command line option (points, pixels?)
+* ~~allow font size specification with command line option (points, pixels?)~~
 * ~~provide an option to show a preview of what the label will look like~~
 * ~~read and write a .dymoprint file containing user preferences~~
 * ~~print barcodes~~
 * ~~print graphics~~
 * ~~plot frame around label~~
 * vertical print
```

### Comparing `dymoprint-1.3.1/src/dymoprint.egg-info/SOURCES.txt` & `dymoprint-1.4.0/src/dymoprint.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,24 +13,36 @@
 .github/workflows/tests.yml
 data/fonts/Carlito-Bold.ttf
 data/fonts/Carlito-BoldItalic.ttf
 data/fonts/Carlito-Italic.ttf
 data/fonts/Carlito-Regular.ttf
 data/fonts/LICENSE
 data/fonts/__init__.py
+data/fonts/barcode_icon.png
+data/fonts/gui_icon.png
+data/fonts/img_icon.png
+data/fonts/qr_icon.png
+data/fonts/txt_icon.png
+doc/DymoPrint_example_1.png
+doc/DymoPrint_example_2.png
+doc/DymoPrint_example_3.png
 src/README.md
 src/__init__.py
 src/dymoprint_fonts
 src/dymoprint/__init__.py
 src/dymoprint/barcode_writer.py
 src/dymoprint/command_line.py
 src/dymoprint/constants.py
+src/dymoprint/dymo_print_engines.py
 src/dymoprint/font_config.py
+src/dymoprint/gui.py
 src/dymoprint/labeler.py
 src/dymoprint/metadata.py
+src/dymoprint/q_dymo_label_widgets.py
+src/dymoprint/q_dymo_labels_list.py
 src/dymoprint/unicode_blocks.py
 src/dymoprint/utils.py
 src/dymoprint.egg-info/PKG-INFO
 src/dymoprint.egg-info/SOURCES.txt
 src/dymoprint.egg-info/dependency_links.txt
 src/dymoprint.egg-info/entry_points.txt
 src/dymoprint.egg-info/requires.txt
```

