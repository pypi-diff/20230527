# Comparing `tmp/nssurge_utils-0.1.5.tar.gz` & `tmp/nssurge_utils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nssurge_utils-0.1.5.tar", max compression
+gzip compressed data, was "nssurge_utils-0.1.6.tar", max compression
```

## Comparing `nssurge_utils-0.1.5.tar` & `nssurge_utils-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-05-24 03:07:21.792499 nssurge_utils-0.1.5/README.md
--rw-r--r--   0        0        0    25596 2023-05-24 13:57:27.194926 nssurge_utils-0.1.5/data/countryFlagsNamesAndDialCodes.json
--rw-r--r--   0        0        0       22 2023-05-27 01:12:21.116366 nssurge_utils-0.1.5/nssurge_utils/__init__.py
--rw-r--r--   0        0        0      624 2023-05-24 13:22:53.300899 nssurge_utils-0.1.5/nssurge_utils/config.py
--rwxr-xr-x   0        0        0     7623 2023-05-24 13:53:38.873303 nssurge_utils-0.1.5/nssurge_utils/extract_proxy.py
--rw-r--r--   0        0        0     1809 2023-05-24 12:59:45.993775 nssurge_utils-0.1.5/nssurge_utils/parsers.py
--rw-r--r--   0        0        0      880 2023-05-24 12:09:19.509286 nssurge_utils-0.1.5/nssurge_utils/predicates.py
--rw-r--r--   0        0        0     1098 2023-05-24 14:00:56.636289 nssurge_utils-0.1.5/nssurge_utils/transform.py
--rw-r--r--   0        0        0      298 2023-05-24 03:20:15.526307 nssurge_utils-0.1.5/nssurge_utils/types.py
--rw-r--r--   0        0        0     7790 2023-05-24 13:39:00.489727 nssurge_utils-0.1.5/nssurge_utils/utils.py
--rw-r--r--   0        0        0      897 2023-05-27 01:12:21.115836 nssurge_utils-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 nssurge_utils-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-24 03:07:21.792499 nssurge_utils-0.1.6/README.md
+-rw-r--r--   0        0        0       22 2023-05-27 04:35:31.788349 nssurge_utils-0.1.6/nssurge_utils/__init__.py
+-rw-r--r--   0        0        0      684 2023-05-27 04:31:06.932174 nssurge_utils-0.1.6/nssurge_utils/config.py
+-rw-r--r--   0        0        0    25596 2023-05-24 13:57:27.194926 nssurge_utils-0.1.6/nssurge_utils/data/countryFlagsNamesAndDialCodes.json
+-rwxr-xr-x   0        0        0     7783 2023-05-27 04:32:56.407074 nssurge_utils-0.1.6/nssurge_utils/extract_proxy.py
+-rw-r--r--   0        0        0     1809 2023-05-24 12:59:45.993775 nssurge_utils-0.1.6/nssurge_utils/parsers.py
+-rw-r--r--   0        0        0      880 2023-05-24 12:09:19.509286 nssurge_utils-0.1.6/nssurge_utils/predicates.py
+-rw-r--r--   0        0        0     1098 2023-05-24 14:00:56.636289 nssurge_utils-0.1.6/nssurge_utils/transform.py
+-rw-r--r--   0        0        0      298 2023-05-24 03:20:15.526307 nssurge_utils-0.1.6/nssurge_utils/types.py
+-rw-r--r--   0        0        0     7790 2023-05-24 13:39:00.489727 nssurge_utils-0.1.6/nssurge_utils/utils.py
+-rw-r--r--   0        0        0      899 2023-05-27 04:35:31.786976 nssurge_utils-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 nssurge_utils-0.1.6/PKG-INFO
```

### Comparing `nssurge_utils-0.1.5/data/countryFlagsNamesAndDialCodes.json` & `nssurge_utils-0.1.6/nssurge_utils/data/countryFlagsNamesAndDialCodes.json`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.5/nssurge_utils/config.py` & `nssurge_utils-0.1.6/nssurge_utils/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,12 +10,14 @@
 #     print(section)
 
 # must be the first ones
 special_proxy_group_value = {'select', 'url-test'}
 
 from pathlib import Path
 
-parent_dir = Path(__file__).parent.parent
-data_dir = parent_dir / 'data'
+package_dir = Path(__file__).parent
+parent_dir = package_dir.parent
+# data_dir = parent_dir / 'data'
+data_dir = package_dir / 'data'
 countryFlagsNamesAndDialCodes_json_path = (
     data_dir / 'countryFlagsNamesAndDialCodes.json'
 )
```

### Comparing `nssurge_utils-0.1.5/nssurge_utils/extract_proxy.py` & `nssurge_utils-0.1.6/nssurge_utils/extract_proxy.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from nssurge_utils.config import surge_config_sections, special_proxy_group_value
 from nssurge_utils.parsers import parse_section, unparse_section
 from nssurge_utils.predicates import name_contains, value_contains
 from nssurge_utils.transform import (
     sanitize_proxy_name,
     proxy_name_add_flag_emoji_before_country_code,
 )
+from nssurge_utils import __version__
 
 
 def get_args():
     """Get command-line arguments"""
 
     parser = argparse.ArgumentParser(
         description='Extract the [Proxy] section from a Surge config file',
@@ -94,14 +95,20 @@
     parser.add_argument(
         '-f',
         '--add-flag-emoji',
         action='store_true',
         help='Add flag emoji to proxy names',
     )
 
+    parser.add_argument(
+        '--version',
+        action='version',
+        version=f'%(prog)s {__version__}',
+    )
+
     args = parser.parse_args()
     if args.add_to_proxy_group and not args.add_to_proxy:
         parser.error(
             '--add-to-proxy-group requires --add-to-proxy to be specified as well'
         )
     if not args.output:
         args.output = args.add_to_proxy
```

### Comparing `nssurge_utils-0.1.5/nssurge_utils/parsers.py` & `nssurge_utils-0.1.6/nssurge_utils/parsers.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.5/nssurge_utils/predicates.py` & `nssurge_utils-0.1.6/nssurge_utils/predicates.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.5/nssurge_utils/transform.py` & `nssurge_utils-0.1.6/nssurge_utils/transform.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.5/nssurge_utils/utils.py` & `nssurge_utils-0.1.6/nssurge_utils/utils.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.5/pyproject.toml` & `nssurge_utils-0.1.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "nssurge-utils"
-version = "0.1.5"
+version = "0.1.6"
 description = "NSSurge Utilities"
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "nssurge_utils" }]
-include = ["data"]
+# include = ["data"]
 license = "MIT"
 homepage = "https://github.com/tddschn/nssurge-utils"
 repository = "https://github.com/tddschn/nssurge-utils"
 classifiers = ["Topic :: Utilities"]
 keywords = ["nssurge", "surge", "utils"]
 [tool.poetry.scripts]
 nssurge-extract-proxy = "nssurge_utils.extract_proxy:main"
```

### Comparing `nssurge_utils-0.1.5/PKG-INFO` & `nssurge_utils-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nssurge-utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: NSSurge Utilities
 Home-page: https://github.com/tddschn/nssurge-utils
 License: MIT
 Keywords: nssurge,surge,utils
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```

