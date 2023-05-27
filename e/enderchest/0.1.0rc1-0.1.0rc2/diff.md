# Comparing `tmp/enderchest-0.1.0rc1.tar.gz` & `tmp/enderchest-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enderchest-0.1.0rc1.tar", last modified: Fri May 26 21:57:43 2023, max compression
+gzip compressed data, was "enderchest-0.1.0rc2.tar", last modified: Sat May 27 18:51:41 2023, max compression
```

## Comparing `enderchest-0.1.0rc1.tar` & `enderchest-0.1.0rc2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:57:43.359450 enderchest-0.1.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-26 21:57:43.359450 enderchest-0.1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:57:43.359450 enderchest-0.1.0rc1/enderchest/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-26 21:57:43.359450 enderchest-0.1.0rc1/enderchest/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17119 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    31131 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/craft.py
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/enderchest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    23728 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/place.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/shulker_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:57:43.355450 enderchest-0.1.0rc1/enderchest/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/sync/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/sync/rsync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:57:43.355450 enderchest-0.1.0rc1/enderchest/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    19693 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/test/test_craft.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/test/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/test/test_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    20455 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/test/test_place.py
--rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/test/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:57:43.359450 enderchest-0.1.0rc1/enderchest/test/testing_files/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/test/testing_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/test/testing_files/enderchest.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/test/testing_files/instgroups.json
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/test/testing_files/launcher_profiles.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/test/testing_files/options.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/test/testing_files/version_manifest_v2.json
--rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/enderchest/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:57:43.351450 enderchest-0.1.0rc1/enderchest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-26 21:57:43.000000 enderchest-0.1.0rc1/enderchest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-26 21:57:43.000000 enderchest-0.1.0rc1/enderchest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:57:43.000000 enderchest-0.1.0rc1/enderchest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 21:57:43.000000 enderchest-0.1.0rc1/enderchest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-26 21:57:43.000000 enderchest-0.1.0rc1/enderchest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 21:57:43.000000 enderchest-0.1.0rc1/enderchest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-26 21:57:43.359450 enderchest-0.1.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-05-26 21:57:33.000000 enderchest-0.1.0rc1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:51:41.850005 enderchest-0.1.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-27 18:51:41.850005 enderchest-0.1.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:51:41.854005 enderchest-0.1.0rc2/enderchest/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-27 18:51:41.854005 enderchest-0.1.0rc2/enderchest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31131 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/enderchest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23728 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/shulker_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:51:41.850005 enderchest-0.1.0rc2/enderchest/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/sync/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/sync/rsync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:51:41.850005 enderchest-0.1.0rc2/enderchest/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20078 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/test_craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/test_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20851 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/test_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:51:41.850005 enderchest-0.1.0rc2/enderchest/test/testing_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/testing_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/testing_files/enderchest.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/testing_files/instgroups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/testing_files/launcher_profiles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/testing_files/options.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/testing_files/version_manifest_v2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/enderchest/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:51:41.850005 enderchest-0.1.0rc2/enderchest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-27 18:51:41.000000 enderchest-0.1.0rc2/enderchest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-27 18:51:41.000000 enderchest-0.1.0rc2/enderchest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 18:51:41.000000 enderchest-0.1.0rc2/enderchest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 18:51:41.000000 enderchest-0.1.0rc2/enderchest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-27 18:51:41.000000 enderchest-0.1.0rc2/enderchest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-27 18:51:41.000000 enderchest-0.1.0rc2/enderchest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-27 18:51:41.854005 enderchest-0.1.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-05-27 18:51:34.000000 enderchest-0.1.0rc2/versioneer.py
```

### Comparing `enderchest-0.1.0rc1/LICENSE` & `enderchest-0.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/PKG-INFO` & `enderchest-0.1.0rc2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,12 @@
-Metadata-Version: 2.1
-Name: enderchest
-Version: 0.1.0rc1
-Summary: syncing and linking for all your Minecraft instances
-Home-page: https://github.com/OpenBagTwo/EnderChest
-Author: Gili "OpenBagTwo" Barlev
-License: GPL v3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # EnderChest
 
+[![PyPI version](https://badge.fury.io/py/enderchest.svg)](https://badge.fury.io/py/enderchest)
+![PyPI downloads](https://img.shields.io/pypi/dm/enderchest.svg)
+
 ![Linux](https://img.shields.io/badge/GNU/Linux-000000?style=flat-square&logo=linux&logoColor=white&color=eda445)
 ![SteamOS](https://img.shields.io/badge/SteamOS-3776AB.svg?style=flat-square&logo=steamdeck&logoColor=white&color=7055c3)
 ![Windows](https://img.shields.io/badge/Windows-0078D6?style=flat-square&logo=windows&logoColor=white)
 ![MacOS](https://img.shields.io/badge/mac%20os-000000?style=flat-square&logo=apple&logoColor=white&color=434334)
 
 [![python](https://img.shields.io/badge/Python-3.10,3.11-3776AB.svg?style=flat&logo=python&logoColor=white&color=ffdc53&labelColor=3d7aaa)](https://www.python.org)
 ![coverage](https://raw.githubusercontent.com/OpenBagTwo/EnderChest/gh-pages/coverage.svg)
@@ -35,18 +26,18 @@
 1. ...across server and client installations
 
 ## Installation
 
 EnderChest is written for **Python 3.11 or greater,** but should otherwise
 run on any architecture or operating system.
 
-The latest release can be installed from github via `pip`:
+The latest release can be installed from PyPI via `pip`:
 
 ```bash
-$ python -m pip install --user git+https://github.com/OpenBagTwo/EnderChest.git@release
+$ python -m pip install --user enderchest
 ```
 
 Full installation instructions can be found on
 [GitHub Pages](https://openbagtwo.github.io/EnderChest/dev/installation).
 
 ## Usage
```

### Comparing `enderchest-0.1.0rc1/README.md` & `enderchest-0.1.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,24 @@
+Metadata-Version: 2.1
+Name: enderchest
+Version: 0.1.0rc2
+Summary: syncing and linking for all your Minecraft instances
+Home-page: https://github.com/OpenBagTwo/EnderChest
+Author: Gili "OpenBagTwo" Barlev
+License: GPL v3
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # EnderChest
 
+[![PyPI version](https://badge.fury.io/py/enderchest.svg)](https://badge.fury.io/py/enderchest)
+![PyPI downloads](https://img.shields.io/pypi/dm/enderchest.svg)
+
 ![Linux](https://img.shields.io/badge/GNU/Linux-000000?style=flat-square&logo=linux&logoColor=white&color=eda445)
 ![SteamOS](https://img.shields.io/badge/SteamOS-3776AB.svg?style=flat-square&logo=steamdeck&logoColor=white&color=7055c3)
 ![Windows](https://img.shields.io/badge/Windows-0078D6?style=flat-square&logo=windows&logoColor=white)
 ![MacOS](https://img.shields.io/badge/mac%20os-000000?style=flat-square&logo=apple&logoColor=white&color=434334)
 
 [![python](https://img.shields.io/badge/Python-3.10,3.11-3776AB.svg?style=flat&logo=python&logoColor=white&color=ffdc53&labelColor=3d7aaa)](https://www.python.org)
 ![coverage](https://raw.githubusercontent.com/OpenBagTwo/EnderChest/gh-pages/coverage.svg)
@@ -23,18 +38,18 @@
 1. ...across server and client installations
 
 ## Installation
 
 EnderChest is written for **Python 3.11 or greater,** but should otherwise
 run on any architecture or operating system.
 
-The latest release can be installed from github via `pip`:
+The latest release can be installed from PyPI via `pip`:
 
 ```bash
-$ python -m pip install --user git+https://github.com/OpenBagTwo/EnderChest.git@release
+$ python -m pip install --user enderchest
 ```
 
 Full installation instructions can be found on
 [GitHub Pages](https://openbagtwo.github.io/EnderChest/dev/installation).
 
 ## Usage
```

### Comparing `enderchest-0.1.0rc1/enderchest/cli.py` & `enderchest-0.1.0rc2/enderchest/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from . import craft, gather, loggers, place, remote
 from ._version import get_versions
 
 # mainly because I think I'm gonna forget what names are canonical (it's the first ones)
 _create_aliases = ("craft", "create")
 _instance_aliases = tuple(
-    alias + plural for alias in ("minecraft", "instance") for plural in ("s", "")
+    alias + plural for alias in ("minecraft", "instance") for plural in ("", "s")
 )
 _shulker_aliases = ("shulker_box", "shulkerbox", "shulker")
 _remote_aliases = tuple(
     alias + plural for alias in ("enderchest", "remote") for plural in ("s", "")
 )
 _list_aliases = ("inventory", "list")
 
@@ -95,15 +95,15 @@
     ),
     (
         ("place",),
         "link (or update the links) from your instances to your EnderChest",
         _place,
     ),
     (
-        ("gather",) + tuple("gather " + alias for alias in _instance_aliases),
+        tuple("gather " + alias for alias in _instance_aliases),
         "register (or update the registry of) a Minecraft installation",
         _update_ender_chest,
     ),
     (
         tuple("gather " + alias for alias in _remote_aliases),
         "register (or update the registry of) a remote EnderChest",
         _update_ender_chest,
@@ -179,14 +179,15 @@
             "\nsyncing and linking for all your Minecraft instances"
         ),
         formatter_class=RawTextHelpFormatter,
     )
 
     enderchest_parser.add_argument(
         "-v",  # don't worry--this doesn't actually conflict with --verbose
+        "-V",
         "--version",
         action="version",
         version=f"%(prog)s v{get_versions()['version']}",
     )
 
     # these are really just for the sake of --help
     # (the parsed args aren't actually used)
@@ -365,15 +366,15 @@
             "abort",
         ),
         default="prompt",
         help="specify how to handle linking errors (default behavior is to prompt after every error)",
     )
 
     # gather instance options
-    gather_instance_parser = action_parsers[f"gather"]
+    gather_instance_parser = action_parsers[f"gather {_instance_aliases[0]}"]
     gather_instance_parser.add_argument(
         "search_paths",
         nargs="+",
         action="extend",
         type=Path,
         help="specify a folder or folders to search for Minecraft installations",
     )
```

### Comparing `enderchest-0.1.0rc1/enderchest/craft.py` & `enderchest-0.1.0rc2/enderchest/craft.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/enderchest.py` & `enderchest-0.1.0rc2/enderchest/enderchest.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/filesystem.py` & `enderchest-0.1.0rc2/enderchest/filesystem.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/gather.py` & `enderchest-0.1.0rc2/enderchest/gather.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/instance.py` & `enderchest-0.1.0rc2/enderchest/instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/loggers.py` & `enderchest-0.1.0rc2/enderchest/loggers.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/place.py` & `enderchest-0.1.0rc2/enderchest/place.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import fnmatch
 import itertools
 import logging
 import os
 from pathlib import Path
 from typing import Iterable
 
+from . import filesystem as fs
 from .gather import load_ender_chest, load_ender_chest_instances, load_shulker_boxes
 from .instance import InstanceSpec
 from .loggers import PLACE_LOGGER
 from .prompt import prompt
 from .shulker_box import ShulkerBox
 
 
@@ -29,15 +30,15 @@
     cleanup : bool, optional
         By default, this method will remove any broken links in your instances
         and servers folders. To disable this behavior, pass in `cleanup=False`
     error_handling : str, optional
         By default, if a linking failure occurs, this method will terminate
         immediately (`error_handling=abort`). Alternatively,
           - pass in `error_handling="ignore"` to continue as if the link failure
-            hadn't occrurred
+            hadn't occurred
           - pass in `error_handling="skip"` to abort linking the current instance
             to the current shulker box but otherwise continue on
           - pass in `error_handling="skip-instance"` to abort linking the current
             instance altogether but to otherwise continue on with other instances
           - pass in `error_handling="skip-shulker-box"` to abort linking to the current
             shulker box altogether but to otherwise continue on with other boxes
           - pass in `error_handling="prompt"` to ask what to do on each failure
@@ -169,14 +170,15 @@
                         break
                     case _:  # nothing to link, so might as well skip the rest
                         continue
 
             PLACE_LOGGER.info(f"Linking {instance.root} to {shulker_box.name}")
 
             resources = set(_rglob(box_root, shulker_box.max_link_depth))
+            resources.remove(fs.shulker_box_config(minecraft_root, shulker_box.name))
 
             match_exit = "pass"
             for link_folder in shulker_box.link_folders:
                 resources -= {box_root / link_folder}
                 resources -= set((box_root / link_folder).rglob("*"))
                 try:
                     link_resource(link_folder, box_root, instance_root)
```

### Comparing `enderchest-0.1.0rc1/enderchest/prompt.py` & `enderchest-0.1.0rc2/enderchest/prompt.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/remote.py` & `enderchest-0.1.0rc2/enderchest/remote.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/shulker_box.py` & `enderchest-0.1.0rc2/enderchest/shulker_box.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/sync/__init__.py` & `enderchest-0.1.0rc2/enderchest/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/sync/file.py` & `enderchest-0.1.0rc2/enderchest/sync/file.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/sync/rsync.py` & `enderchest-0.1.0rc2/enderchest/sync/rsync.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/test/conftest.py` & `enderchest-0.1.0rc2/enderchest/test/conftest.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/test/test_cli.py` & `enderchest-0.1.0rc2/enderchest/test/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
     def test_ignore_errors(self, place_log, flags):
         action, *_, options = cli.parse_args(["enderchest", "place", *flags])
         action(Path(), **options)
         assert place_log[0][1]["error_handling"] == "ignore"
 
 
 class TestGather(ActionTestSuite):
-    action = "gather"
+    action = "gather minecraft"
     required_args = ("~",)
 
     @pytest.mark.parametrize("with_root", (False, True), ids=("no_root", "with-root"))
     def test_gather_requires_at_least_one_search_path(self, with_root):
         more_args = ("--root", "/minecraft") if with_root else ()
         with pytest.raises(SystemExit):
             cli.parse_args(["enderchest", *self.action.split(), *more_args])
```

### Comparing `enderchest-0.1.0rc1/enderchest/test/test_craft.py` & `enderchest-0.1.0rc2/enderchest/test/test_craft.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 
 import pytest
 
 from enderchest import EnderChest, ShulkerBox, craft
 from enderchest import filesystem as fs
 from enderchest.enderchest import create_ender_chest
 from enderchest.gather import load_ender_chest, load_shulker_boxes
-from enderchest.shulker_box import create_shulker_box
+from enderchest.shulker_box import (
+    DEFAULT_SHULKER_FOLDERS,
+    STANDARD_LINK_FOLDERS,
+    create_shulker_box,
+)
 
 from . import utils
 
 
 class TestConfigWriting:
     def test_shulker_box_config_roundtrip(self, minecraft_root):
         original_shulker = ShulkerBox(
@@ -224,14 +228,26 @@
 
         # make sure all responses were used
         with pytest.raises(StopIteration):
             script_reader()
 
 
 class TestShulkerBoxCrafting:
+    def test_default_folders_and_link_folders_do_not_overlap(self):
+        assert (
+            len(
+                [
+                    folder
+                    for folder in STANDARD_LINK_FOLDERS
+                    if folder in DEFAULT_SHULKER_FOLDERS
+                ]
+            )
+            == 0
+        )
+
     def test_no_kwargs_routes_to_the_interactive_prompter(self, monkeypatch):
         prompt_log: list[tuple[Path, str]] = []
 
         def mock_prompt(root, name) -> Any:
             prompt_log.append((root, name))
             return "MockShulkerBox"
```

### Comparing `enderchest-0.1.0rc1/enderchest/test/test_gather.py` & `enderchest-0.1.0rc2/enderchest/test/test_gather.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/test/test_instance.py` & `enderchest-0.1.0rc2/enderchest/test/test_instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/test/test_place.py` & `enderchest-0.1.0rc2/enderchest/test/test_place.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Tests around instance-linking functionality"""
 import os
 import re
 from pathlib import Path
 
 import pytest
 
-from enderchest import ShulkerBox, place
+from enderchest import ShulkerBox
+from enderchest import filesystem as fs
+from enderchest import place
 
 from . import utils
 
 
 class TestRglob:
     def test_max_depth_of_one_is_equivalent_to_a_plain_glob(self, minecraft_root):
         glob = sorted(minecraft_root.iterdir())
@@ -105,14 +107,22 @@
         ).read_text() == "alexander\nmomoa\nbateman\n"
 
         assert (instance_folder / "usercache.json").resolve() == (
             minecraft_root / "EnderChest" / "global" / "usercache.json"
         )
 
     @utils.parametrize_over_instances("official", "axolotl")
+    def test_does_not_place_shulker_config(self, minecraft_root, instance):
+        place.place_ender_chest(minecraft_root)
+
+        instance_folder = utils.resolve(instance.root, minecraft_root)
+
+        assert not (instance_folder / fs.SHULKER_BOX_CONFIG_NAME).exists()
+
+    @utils.parametrize_over_instances("official", "axolotl")
     def test_link_folder_can_be_a_symlink(self, minecraft_root, instance):
         place.place_ender_chest(minecraft_root)
 
         instance_folder = utils.resolve(instance.root, minecraft_root)
 
         # the counterpoint to the whole "one assertion per test" rule--this
         # is a cascading case of figuring way of figuring out just how badly
```

### Comparing `enderchest-0.1.0rc1/enderchest/test/test_sync.py` & `enderchest-0.1.0rc2/enderchest/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/test/testing_files/enderchest.cfg` & `enderchest-0.1.0rc2/enderchest/test/testing_files/enderchest.cfg`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/test/testing_files/launcher_profiles.json` & `enderchest-0.1.0rc2/enderchest/test/testing_files/launcher_profiles.json`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest/test/utils.py` & `enderchest-0.1.0rc2/enderchest/test/utils.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/enderchest.egg-info/PKG-INFO` & `enderchest-0.1.0rc2/enderchest.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # EnderChest
 
+[![PyPI version](https://badge.fury.io/py/enderchest.svg)](https://badge.fury.io/py/enderchest)
+![PyPI downloads](https://img.shields.io/pypi/dm/enderchest.svg)
+
 ![Linux](https://img.shields.io/badge/GNU/Linux-000000?style=flat-square&logo=linux&logoColor=white&color=eda445)
 ![SteamOS](https://img.shields.io/badge/SteamOS-3776AB.svg?style=flat-square&logo=steamdeck&logoColor=white&color=7055c3)
 ![Windows](https://img.shields.io/badge/Windows-0078D6?style=flat-square&logo=windows&logoColor=white)
 ![MacOS](https://img.shields.io/badge/mac%20os-000000?style=flat-square&logo=apple&logoColor=white&color=434334)
 
 [![python](https://img.shields.io/badge/Python-3.10,3.11-3776AB.svg?style=flat&logo=python&logoColor=white&color=ffdc53&labelColor=3d7aaa)](https://www.python.org)
 ![coverage](https://raw.githubusercontent.com/OpenBagTwo/EnderChest/gh-pages/coverage.svg)
@@ -35,18 +38,18 @@
 1. ...across server and client installations
 
 ## Installation
 
 EnderChest is written for **Python 3.11 or greater,** but should otherwise
 run on any architecture or operating system.
 
-The latest release can be installed from github via `pip`:
+The latest release can be installed from PyPI via `pip`:
 
 ```bash
-$ python -m pip install --user git+https://github.com/OpenBagTwo/EnderChest.git@release
+$ python -m pip install --user enderchest
 ```
 
 Full installation instructions can be found on
 [GitHub Pages](https://openbagtwo.github.io/EnderChest/dev/installation).
 
 ## Usage
```

### Comparing `enderchest-0.1.0rc1/enderchest.egg-info/SOURCES.txt` & `enderchest-0.1.0rc2/enderchest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/setup.py` & `enderchest-0.1.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc1/versioneer.py` & `enderchest-0.1.0rc2/versioneer.py`

 * *Files identical despite different names*

