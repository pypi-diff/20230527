# Comparing `tmp/ctwin32-2.1.0.tar.gz` & `tmp/ctwin32-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctwin32-2.1.0.tar", last modified: Mon Mar 27 05:34:02 2023, max compression
+gzip compressed data, was "ctwin32-2.2.0.tar", last modified: Sat May 27 04:28:45 2023, max compression
```

## Comparing `ctwin32-2.1.0.tar` & `ctwin32-2.2.0.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 05:34:02.877712 ctwin32-2.1.0/
--rw-rw-rw-   0        0        0     1057 2023-01-07 08:48:10.000000 ctwin32-2.1.0/LICENSE
--rw-rw-rw-   0        0        0       14 2023-03-27 05:21:14.000000 ctwin32-2.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2474 2023-03-27 05:34:02.877712 ctwin32-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1550 2022-12-17 04:38:52.000000 ctwin32-2.1.0/README.md
--rw-rw-rw-   0        0        0     1617 2023-01-11 05:59:42.000000 ctwin32-2.1.0/bld.py
-drwxrwxrwx   0        0        0        0 2023-03-27 05:34:02.849695 ctwin32-2.1.0/ctwin32/
--rw-rw-rw-   0        0        0   219585 2023-03-27 05:30:05.000000 ctwin32-2.1.0/ctwin32/__init__.py
--rw-rw-rw-   0        0        0    39279 2023-03-09 05:59:53.000000 ctwin32-2.1.0/ctwin32/advapi.py
--rw-rw-rw-   0        0        0    17652 2023-02-05 05:13:44.000000 ctwin32-2.1.0/ctwin32/bcrypt.py
--rw-rw-rw-   0        0        0     4696 2023-01-07 08:47:22.000000 ctwin32-2.1.0/ctwin32/cfgmgr.py
--rw-rw-rw-   0        0        0     8673 2023-01-07 08:47:22.000000 ctwin32-2.1.0/ctwin32/comctl.py
--rw-rw-rw-   0        0        0     4352 2023-01-07 08:47:22.000000 ctwin32-2.1.0/ctwin32/gdi.py
--rw-rw-rw-   0        0        0    13791 2023-01-07 08:47:22.000000 ctwin32-2.1.0/ctwin32/iphlpapi.py
--rw-rw-rw-   0        0        0    39581 2023-02-05 06:36:56.000000 ctwin32-2.1.0/ctwin32/kernel.py
--rw-rw-rw-   0        0        0     5950 2023-01-07 08:47:22.000000 ctwin32-2.1.0/ctwin32/misc.py
--rw-rw-rw-   0        0        0     5266 2023-01-07 08:47:22.000000 ctwin32-2.1.0/ctwin32/msi.py
--rw-rw-rw-   0        0        0    17117 2023-02-05 04:24:42.000000 ctwin32-2.1.0/ctwin32/ntdll.py
--rw-rw-rw-   0        0        0     4182 2023-03-12 06:03:22.000000 ctwin32-2.1.0/ctwin32/psapi.py
--rw-rw-rw-   0        0        0     6327 2023-01-07 08:47:22.000000 ctwin32-2.1.0/ctwin32/secur.py
--rw-rw-rw-   0        0        0    17561 2023-01-07 08:47:22.000000 ctwin32-2.1.0/ctwin32/setupapi.py
--rw-rw-rw-   0        0        0     7840 2023-01-07 08:47:22.000000 ctwin32-2.1.0/ctwin32/shell.py
--rw-rw-rw-   0        0        0    44006 2023-01-07 08:47:22.000000 ctwin32-2.1.0/ctwin32/user.py
--rw-rw-rw-   0        0        0     4979 2023-01-07 08:47:22.000000 ctwin32-2.1.0/ctwin32/version.py
--rw-rw-rw-   0        0        0     6878 2023-01-07 08:47:22.000000 ctwin32-2.1.0/ctwin32/virtdisk.py
--rw-rw-rw-   0        0        0    28582 2023-02-05 06:37:11.000000 ctwin32-2.1.0/ctwin32/wndcls.py
--rw-rw-rw-   0        0        0    12775 2023-03-18 06:52:12.000000 ctwin32-2.1.0/ctwin32/wtypes.py
-drwxrwxrwx   0        0        0        0 2023-03-27 05:34:02.853696 ctwin32-2.1.0/ctwin32.egg-info/
--rw-rw-rw-   0        0        0     2474 2023-03-27 05:34:02.000000 ctwin32-2.1.0/ctwin32.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1089 2023-03-27 05:34:02.000000 ctwin32-2.1.0/ctwin32.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 05:34:02.000000 ctwin32-2.1.0/ctwin32.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-27 05:34:02.000000 ctwin32-2.1.0/ctwin32.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-01-24 05:12:00.000000 ctwin32-2.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-03-27 05:34:02.877712 ctwin32-2.1.0/samples/
--rw-rw-rw-   0        0        0     2571 2023-01-07 08:47:22.000000 ctwin32-2.1.0/samples/arp_table.py
--rw-rw-rw-   0        0        0     2529 2023-02-05 05:49:15.000000 ctwin32-2.1.0/samples/atta_vdisk.py
--rw-rw-rw-   0        0        0     3999 2023-01-24 05:13:07.000000 ctwin32-2.1.0/samples/calendar.pyw
--rw-rw-rw-   0        0        0     7327 2023-03-26 04:11:00.000000 ctwin32-2.1.0/samples/dump_ver_res.py
--rw-rw-rw-   0        0        0     2754 2023-01-07 08:47:22.000000 ctwin32-2.1.0/samples/endis_bsl_usb.py
--rw-rw-rw-   0        0        0     2300 2023-01-07 08:47:22.000000 ctwin32-2.1.0/samples/exbinmsi.py
--rw-rw-rw-   0        0        0     7490 2023-01-07 08:47:22.000000 ctwin32-2.1.0/samples/extract_ico.py
--rw-rw-rw-   0        0        0     4738 2023-01-07 08:47:22.000000 ctwin32-2.1.0/samples/find_zombies.py
--rw-rw-rw-   0        0        0     2026 2023-03-24 04:56:31.000000 ctwin32-2.1.0/samples/fopa.py
--rw-rw-rw-   0        0        0     4124 2023-01-24 05:13:26.000000 ctwin32-2.1.0/samples/hello_wnd.pyw
--rw-rw-rw-   0        0        0     6825 2023-02-05 06:01:54.000000 ctwin32-2.1.0/samples/keyview.pyw
--rw-rw-rw-   0        0        0     1989 2023-02-05 05:42:07.000000 ctwin32-2.1.0/samples/listpipes.py
--rw-rw-rw-   0        0        0     3701 2023-01-07 08:47:22.000000 ctwin32-2.1.0/samples/logonsessions.py
--rw-rw-rw-   0        0        0     2011 2023-01-07 08:47:22.000000 ctwin32-2.1.0/samples/netifaces.py
--rw-rw-rw-   0        0        0     2270 2023-01-07 08:47:22.000000 ctwin32-2.1.0/samples/np_dev.py
--rw-rw-rw-   0        0        0     3172 2023-01-24 04:50:54.000000 ctwin32-2.1.0/samples/py_ver.py
--rw-rw-rw-   0        0        0     5164 2023-01-07 08:47:22.000000 ctwin32-2.1.0/samples/remove_drive_by_letter.py
--rw-rw-rw-   0        0        0     6485 2023-02-05 05:34:26.000000 ctwin32-2.1.0/samples/rm_sign_tool.py
--rw-rw-rw-   0        0        0     5460 2023-01-07 08:47:22.000000 ctwin32-2.1.0/samples/senv.py
--rw-rw-rw-   0        0        0     4568 2023-01-07 08:47:22.000000 ctwin32-2.1.0/samples/simple_aes.py
--rw-rw-rw-   0        0        0     3372 2023-01-07 08:47:22.000000 ctwin32-2.1.0/samples/stopnow.py
--rw-rw-rw-   0        0        0     2253 2023-01-07 08:47:22.000000 ctwin32-2.1.0/samples/sua_enums.py
--rw-rw-rw-   0        0        0     2703 2023-01-12 03:55:54.000000 ctwin32-2.1.0/samples/test_sign_tool.py
--rw-rw-rw-   0        0        0     1996 2023-01-07 08:47:22.000000 ctwin32-2.1.0/samples/uptime_evt.py
--rw-rw-rw-   0        0        0     2559 2023-01-07 08:47:22.000000 ctwin32-2.1.0/samples/virt_term_seq.py
--rw-rw-rw-   0        0        0       42 2023-03-27 05:34:02.877712 ctwin32-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1185 2023-03-24 04:44:28.000000 ctwin32-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 04:28:45.108689 ctwin32-2.2.0/
+-rw-rw-rw-   0        0        0     1057 2023-01-07 08:48:10.000000 ctwin32-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-03-27 05:21:14.000000 ctwin32-2.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2575 2023-05-27 04:28:45.108689 ctwin32-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1651 2023-03-30 05:59:34.000000 ctwin32-2.2.0/README.md
+-rw-rw-rw-   0        0        0     1617 2023-01-11 05:59:42.000000 ctwin32-2.2.0/bld.py
+drwxrwxrwx   0        0        0        0 2023-05-27 04:28:45.082105 ctwin32-2.2.0/ctwin32/
+-rw-rw-rw-   0        0        0   222711 2023-05-27 04:25:20.000000 ctwin32-2.2.0/ctwin32/__init__.py
+-rw-rw-rw-   0        0        0    39112 2023-05-26 05:24:56.000000 ctwin32-2.2.0/ctwin32/advapi.py
+-rw-rw-rw-   0        0        0    17770 2023-04-11 05:50:33.000000 ctwin32-2.2.0/ctwin32/bcrypt.py
+-rw-rw-rw-   0        0        0     4696 2023-01-07 08:47:22.000000 ctwin32-2.2.0/ctwin32/cfgmgr.py
+-rw-rw-rw-   0        0        0     9079 2023-04-11 05:50:42.000000 ctwin32-2.2.0/ctwin32/comctl.py
+-rw-rw-rw-   0        0        0     4352 2023-01-07 08:47:22.000000 ctwin32-2.2.0/ctwin32/gdi.py
+-rw-rw-rw-   0        0        0    13791 2023-01-07 08:47:22.000000 ctwin32-2.2.0/ctwin32/iphlpapi.py
+-rw-rw-rw-   0        0        0    42469 2023-05-06 04:06:32.000000 ctwin32-2.2.0/ctwin32/kernel.py
+-rw-rw-rw-   0        0        0     5950 2023-01-07 08:47:22.000000 ctwin32-2.2.0/ctwin32/misc.py
+-rw-rw-rw-   0        0        0     5174 2023-04-08 15:00:11.000000 ctwin32-2.2.0/ctwin32/msi.py
+-rw-rw-rw-   0        0        0    17900 2023-05-26 17:30:01.000000 ctwin32-2.2.0/ctwin32/ntdll.py
+-rw-rw-rw-   0        0        0     4182 2023-03-12 06:03:22.000000 ctwin32-2.2.0/ctwin32/psapi.py
+-rw-rw-rw-   0        0        0     6252 2023-05-24 06:03:37.000000 ctwin32-2.2.0/ctwin32/secur.py
+-rw-rw-rw-   0        0        0    17498 2023-04-08 15:00:11.000000 ctwin32-2.2.0/ctwin32/setupapi.py
+-rw-rw-rw-   0        0        0     7921 2023-05-06 04:07:18.000000 ctwin32-2.2.0/ctwin32/shell.py
+-rw-rw-rw-   0        0        0    44298 2023-05-27 04:08:36.000000 ctwin32-2.2.0/ctwin32/user.py
+-rw-rw-rw-   0        0        0     4923 2023-04-11 05:52:35.000000 ctwin32-2.2.0/ctwin32/version.py
+-rw-rw-rw-   0        0        0     6877 2023-04-11 05:52:41.000000 ctwin32-2.2.0/ctwin32/virtdisk.py
+-rw-rw-rw-   0        0        0    28509 2023-04-11 05:53:33.000000 ctwin32-2.2.0/ctwin32/wndcls.py
+-rw-rw-rw-   0        0        0    14247 2023-04-11 15:35:26.000000 ctwin32-2.2.0/ctwin32/wtypes.py
+drwxrwxrwx   0        0        0        0 2023-05-27 04:28:45.086106 ctwin32-2.2.0/ctwin32.egg-info/
+-rw-rw-rw-   0        0        0     2575 2023-05-27 04:28:45.000000 ctwin32-2.2.0/ctwin32.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1147 2023-05-27 04:28:45.000000 ctwin32-2.2.0/ctwin32.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 04:28:45.000000 ctwin32-2.2.0/ctwin32.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-27 04:28:45.000000 ctwin32-2.2.0/ctwin32.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-01-24 05:12:00.000000 ctwin32-2.2.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-27 04:28:45.108111 ctwin32-2.2.0/samples/
+-rw-rw-rw-   0        0        0     2571 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/arp_table.py
+-rw-rw-rw-   0        0        0     2529 2023-02-05 05:49:15.000000 ctwin32-2.2.0/samples/atta_vdisk.py
+-rw-rw-rw-   0        0        0     3999 2023-01-24 05:13:07.000000 ctwin32-2.2.0/samples/calendar.pyw
+-rw-rw-rw-   0        0        0     7327 2023-03-26 04:11:00.000000 ctwin32-2.2.0/samples/dump_ver_res.py
+-rw-rw-rw-   0        0        0     2754 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/endis_bsl_usb.py
+-rw-rw-rw-   0        0        0     2300 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/exbinmsi.py
+-rw-rw-rw-   0        0        0     7490 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/extract_ico.py
+-rw-rw-rw-   0        0        0     4738 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/find_zombies.py
+-rw-rw-rw-   0        0        0     2026 2023-03-24 04:56:31.000000 ctwin32-2.2.0/samples/fopa.py
+-rw-rw-rw-   0        0        0     4124 2023-01-24 05:13:26.000000 ctwin32-2.2.0/samples/hello_wnd.pyw
+-rw-rw-rw-   0        0        0     6825 2023-02-05 06:01:54.000000 ctwin32-2.2.0/samples/keyview.pyw
+-rw-rw-rw-   0        0        0     1989 2023-02-05 05:42:07.000000 ctwin32-2.2.0/samples/listpipes.py
+-rw-rw-rw-   0        0        0     3701 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/logonsessions.py
+-rw-rw-rw-   0        0        0     2011 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/netifaces.py
+-rw-rw-rw-   0        0        0     2270 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/np_dev.py
+-rw-rw-rw-   0        0        0     7698 2023-05-27 03:58:52.000000 ctwin32-2.2.0/samples/power_requests.py
+-rw-rw-rw-   0        0        0     5274 2023-04-08 15:36:59.000000 ctwin32-2.2.0/samples/print_reparse_points.py
+-rw-rw-rw-   0        0        0     3172 2023-01-24 04:50:54.000000 ctwin32-2.2.0/samples/py_ver.py
+-rw-rw-rw-   0        0        0     5164 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/remove_drive_by_letter.py
+-rw-rw-rw-   0        0        0     6485 2023-02-05 05:34:26.000000 ctwin32-2.2.0/samples/rm_sign_tool.py
+-rw-rw-rw-   0        0        0     5460 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/senv.py
+-rw-rw-rw-   0        0        0     4568 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/simple_aes.py
+-rw-rw-rw-   0        0        0     3372 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/stopnow.py
+-rw-rw-rw-   0        0        0     2253 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/sua_enums.py
+-rw-rw-rw-   0        0        0     2703 2023-01-12 03:55:54.000000 ctwin32-2.2.0/samples/test_sign_tool.py
+-rw-rw-rw-   0        0        0     2063 2023-04-10 15:30:40.000000 ctwin32-2.2.0/samples/uptime_evt.py
+-rw-rw-rw-   0        0        0     2559 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/virt_term_seq.py
+-rw-rw-rw-   0        0        0       42 2023-05-27 04:28:45.108689 ctwin32-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1185 2023-04-03 04:37:37.000000 ctwin32-2.2.0/setup.py
```

### Comparing `ctwin32-2.1.0/LICENSE` & `ctwin32-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/PKG-INFO` & `ctwin32-2.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctwin32
-Version: 2.1.0
+Version: 2.2.0
 Summary: Access selected win32 APIs through ctypes
 Author: Rocco Matano
 License: MIT License
 Project-URL: homepage, https://github.com/RoccoMatano/ctwin32
 Project-URL: changelog, https://github.com/RoccoMatano/ctwin32/blob/master/changelog.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,20 +16,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ![](https://raw.githubusercontent.com/RoccoMatano/ctwin32/master/doc/images/ctwin32.ico) ctwin32
-
+# ![logo](https://raw.githubusercontent.com/RoccoMatano/ctwin32/master/doc/images/ctwin32.ico) ctwin32
 
 [![PyPI - Version](https://img.shields.io/pypi/v/ctwin32.svg)](https://pypi.org/project/ctwin32)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ctwin32.svg)](https://pypi.org/project/ctwin32)
 [![License - MIT](https://img.shields.io/badge/license-MIT-green)](https://spdx.org/licenses/MIT.html)
+[![PyPI - Stats](https://img.shields.io/pypi/dm/ctwin32)](https://pypistats.org/packages/ctwin32)
 
 -----
 
 ctwin32 is a pure Python module, that wraps some Windows APIs (win32) by using
 [ctypes](https://docs.python.org/3/library/ctypes.html). Since it is my personal
 playground, the selection of supported APIs and the way those are wrapped are
 solely dictated by my needs and preferences.
```

### Comparing `ctwin32-2.1.0/README.md` & `ctwin32-2.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# ![](https://raw.githubusercontent.com/RoccoMatano/ctwin32/master/doc/images/ctwin32.ico) ctwin32
-
+# ![logo](https://raw.githubusercontent.com/RoccoMatano/ctwin32/master/doc/images/ctwin32.ico) ctwin32
 
 [![PyPI - Version](https://img.shields.io/pypi/v/ctwin32.svg)](https://pypi.org/project/ctwin32)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ctwin32.svg)](https://pypi.org/project/ctwin32)
 [![License - MIT](https://img.shields.io/badge/license-MIT-green)](https://spdx.org/licenses/MIT.html)
+[![PyPI - Stats](https://img.shields.io/pypi/dm/ctwin32)](https://pypistats.org/packages/ctwin32)
 
 -----
 
 ctwin32 is a pure Python module, that wraps some Windows APIs (win32) by using
 [ctypes](https://docs.python.org/3/library/ctypes.html). Since it is my personal
 playground, the selection of supported APIs and the way those are wrapped are
 solely dictated by my needs and preferences.
```

### Comparing `ctwin32-2.1.0/bld.py` & `ctwin32-2.2.0/bld.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/ctwin32/__init__.py` & `ctwin32-2.2.0/ctwin32/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,23 +23,24 @@
 ################################################################################
 
 from types import SimpleNamespace as _namespace
 import ctypes
 from .wtypes import (
     DWORD,
     HANDLE,
+    OSVERSIONINFOEX,
     PWSTR,
     UINT,
     WCHAR,
     )
 ref = ctypes.byref
 
 ################################################################################
 
-__version__ = "2.1.0"
+__version__ = "2.2.0"
 
 ################################################################################
 
 def raise_if(condition):
     if condition:
         raise ctypes.WinError()
 
@@ -59,14 +60,32 @@
 
 def raise_on_hr(hr):
     if hr < 0:
         raise ctypes.WinError(hr)
 
 ################################################################################
 
+# similar to contextlib.suppress
+
+class suppress_winerr():
+    def __init__(self, *err_codes):
+        self._err_codes = err_codes
+
+    def __enter__(self):
+        pass
+
+    def __exit__(self, exctype, excinst, exctb):
+        return (
+            exctype is not None and
+            issubclass(exctype, OSError) and
+            excinst.winerror in self._err_codes
+            )
+
+################################################################################
+
 def fun_fact(function, signature):
     function.restype = signature[0]
     function.argtypes = signature[1:]
     return function
 
 ################################################################################
 
@@ -118,29 +137,44 @@
         return 0, None, None
     argc = len(args)
     chain = "\0".join(args) + "\0"
 
     class ArgumentBuffer(ctypes.Structure):
         _fields_ = (
             ("pointers", PWSTR * argc),
-            ("strings", WCHAR * len(chain))
+            ("strings", WCHAR * len(chain)),
             )
 
     buffer = ArgumentBuffer(strings=chain)
     argv = ctypes.addressof(buffer)
     str_addr = argv + ArgumentBuffer.strings.offset
     for i, arg in enumerate(args):
         buffer.pointers[i] = str_addr
         str_addr += ctypes.sizeof(WCHAR) * (len(arg) + 1)
     return argc, argv, buffer
 
 ################################################################################
 
 def ns_from_struct(cts):
-    return _namespace(**{f: getattr(cts, f) for f, _ in cts._fields_})
+    return _namespace(**{f: getattr(cts, f) for f, *_ in cts._fields_})
+
+################################################################################
+
+def _warn_win_ver():
+    osve = OSVERSIONINFOEX()
+    status = ctypes.WinDLL("ntdll.dll").RtlGetVersion(ref(osve))
+    if status == 0 and osve.dwMajorVersion < 10:
+        import warnings
+        msg = (
+            "ctwin32 does not intend to support old Windows versions "
+            "(< Windows 10). Be happy if it still works ;-)"
+            )
+        warnings.warn(msg, stacklevel=3)
+
+_warn_win_ver()
 
 ################################################################################
 
 INVALID_HANDLE_VALUE = HANDLE(-1).value
 HGDI_ERROR = INVALID_HANDLE_VALUE
 
 DBT_CONFIGCHANGECANCELED = 25
@@ -5863,22 +5897,26 @@
 DCB_SET = DCB_RESET | DCB_ACCUMULATE
 DCB_ENABLE = 4
 DCB_DISABLE = 8
 
 FILE_BEGIN = 0
 FILE_CURRENT = 1
 FILE_END = 2
-FILE_FLAG_WRITE_THROUGH = -2147483648
-FILE_FLAG_OVERLAPPED = 1073741824
-FILE_FLAG_NO_BUFFERING = 536870912
-FILE_FLAG_RANDOM_ACCESS = 268435456
-FILE_FLAG_SEQUENTIAL_SCAN = 134217728
-FILE_FLAG_DELETE_ON_CLOSE = 67108864
-FILE_FLAG_BACKUP_SEMANTICS = 33554432
-FILE_FLAG_POSIX_SEMANTICS = 16777216
+FILE_FLAG_WRITE_THROUGH = 0x80000000
+FILE_FLAG_OVERLAPPED = 0x40000000
+FILE_FLAG_NO_BUFFERING = 0x20000000
+FILE_FLAG_RANDOM_ACCESS = 0x10000000
+FILE_FLAG_SEQUENTIAL_SCAN = 0x08000000
+FILE_FLAG_DELETE_ON_CLOSE = 0x04000000
+FILE_FLAG_BACKUP_SEMANTICS = 0x02000000
+FILE_FLAG_POSIX_SEMANTICS = 0x01000000
+FILE_FLAG_SESSION_AWARE = 0x00800000
+FILE_FLAG_OPEN_REPARSE_POINT = 0x00200000
+FILE_FLAG_OPEN_NO_RECALL = 0x00100000
+FILE_FLAG_FIRST_PIPE_INSTANCE = 0x00080000
 CREATE_NEW = 1
 CREATE_ALWAYS = 2
 OPEN_EXISTING = 3
 OPEN_ALWAYS = 4
 TRUNCATE_EXISTING = 5
 PIPE_ACCESS_INBOUND = 1
 PIPE_ACCESS_OUTBOUND = 2
@@ -7782,7 +7820,62 @@
 DISABLE_NEWLINE_AUTO_RETURN = 0x0008
 ENABLE_LVB_GRID_WORLDWIDE = 0x0010
 
 LIST_MODULES_DEFAULT = 0x0
 LIST_MODULES_32BIT = 0x01
 LIST_MODULES_64BIT = 0x02
 LIST_MODULES_ALL = (LIST_MODULES_32BIT | LIST_MODULES_64BIT)
+
+IO_REPARSE_TAG_RESERVED_ZERO = 0x00000000
+IO_REPARSE_TAG_RESERVED_ONE = 0x00000001
+IO_REPARSE_TAG_RESERVED_TWO = 0x00000002
+IO_REPARSE_TAG_MOUNT_POINT = 0xA0000003
+IO_REPARSE_TAG_HSM = 0xC0000004
+IO_REPARSE_TAG_DRIVE_EXTENDER = 0x80000005
+IO_REPARSE_TAG_HSM2 = 0x80000006
+IO_REPARSE_TAG_SIS = 0x80000007
+IO_REPARSE_TAG_WIM = 0x80000008
+IO_REPARSE_TAG_CSV = 0x80000009
+IO_REPARSE_TAG_DFS = 0x8000000A
+IO_REPARSE_TAG_FILTER_MANAGER = 0x8000000B
+IO_REPARSE_TAG_SYMLINK = 0xA000000C
+IO_REPARSE_TAG_IIS_CACHE = 0xA0000010
+IO_REPARSE_TAG_DFSR = 0x80000012
+IO_REPARSE_TAG_DEDUP = 0x80000013
+IO_REPARSE_TAG_APPXSTRM = 0xC0000014
+IO_REPARSE_TAG_NFS = 0x80000014
+IO_REPARSE_TAG_FILE_PLACEHOLDER = 0x80000015
+IO_REPARSE_TAG_DFM = 0x80000016
+IO_REPARSE_TAG_WOF = 0x80000017
+IO_REPARSE_TAG_WCI = 0x80000018
+IO_REPARSE_TAG_WCI_1 = 0x90001018
+IO_REPARSE_TAG_GLOBAL_REPARSE = 0xA0000019
+IO_REPARSE_TAG_CLOUD = 0x9000001A
+IO_REPARSE_TAG_CLOUD_1 = 0x9000101A
+IO_REPARSE_TAG_CLOUD_2 = 0x9000201A
+IO_REPARSE_TAG_CLOUD_3 = 0x9000301A
+IO_REPARSE_TAG_CLOUD_4 = 0x9000401A
+IO_REPARSE_TAG_CLOUD_5 = 0x9000501A
+IO_REPARSE_TAG_CLOUD_6 = 0x9000601A
+IO_REPARSE_TAG_CLOUD_7 = 0x9000701A
+IO_REPARSE_TAG_CLOUD_8 = 0x9000801A
+IO_REPARSE_TAG_CLOUD_9 = 0x9000901A
+IO_REPARSE_TAG_CLOUD_A = 0x9000A01A
+IO_REPARSE_TAG_CLOUD_B = 0x9000B01A
+IO_REPARSE_TAG_CLOUD_C = 0x9000C01A
+IO_REPARSE_TAG_CLOUD_D = 0x9000D01A
+IO_REPARSE_TAG_CLOUD_E = 0x9000E01A
+IO_REPARSE_TAG_CLOUD_F = 0x9000F01A
+IO_REPARSE_TAG_APPEXECLINK = 0x8000001B
+IO_REPARSE_TAG_PROJFS = 0x9000001C
+IO_REPARSE_TAG_LX_SYMLINK = 0xA000001D
+IO_REPARSE_TAG_STORAGE_SYNC = 0x8000001E
+IO_REPARSE_TAG_WCI_TOMBSTONE = 0xA000001F
+IO_REPARSE_TAG_UNHANDLED = 0x80000020
+IO_REPARSE_TAG_ONEDRIVE = 0x80000021
+IO_REPARSE_TAG_PROJFS_TOMBSTONE = 0xA0000022
+IO_REPARSE_TAG_AF_UNIX = 0x80000023
+IO_REPARSE_TAG_LX_FIFO = 0x80000024
+IO_REPARSE_TAG_LX_CHR = 0x80000025
+IO_REPARSE_TAG_LX_BLK = 0x80000026
+IO_REPARSE_TAG_WCI_LINK = 0xA0000027
+IO_REPARSE_TAG_WCI_LINK_1 = 0xA0001027
```

### Comparing `ctwin32-2.1.0/ctwin32/advapi.py` & `ctwin32-2.2.0/ctwin32/advapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     WORD,
     )
 from . import (
     ref,
     raise_if,
     raise_on_zero,
     raise_on_err,
+    suppress_winerr,
     fun_fact,
     ns_from_struct,
     argc_argv_from_args,
     REG_DWORD,
     REG_QWORD,
     REG_SZ,
     REG_EXPAND_SZ,
@@ -333,24 +334,19 @@
         )
     return name.value
 
 ################################################################################
 
 def reg_enum_keys(key):
     index = 0
-    while True:
-        try:
+    with suppress_winerr(ERROR_NO_MORE_ITEMS):
+        while True:
             sub_key_name = RegEnumKeyEx(key, index)
             index += 1
             yield sub_key_name
-        except OSError as e:
-            if e.winerror == ERROR_NO_MORE_ITEMS:
-                break
-            else:
-                raise
 
 ################################################################################
 
 _RegEnumValue = fun_fact(
     _adv.RegEnumValueW, (
         LONG,
         HKEY,
@@ -392,24 +388,19 @@
 
     return (name.value,) + registry_to_py(typ.value, value.raw[:vlen.value])
 
 ################################################################################
 
 def reg_enum_values(key):
     index = 0
-    while True:
-        try:
+    with suppress_winerr(ERROR_NO_MORE_ITEMS):
+        while True:
             tpl = RegEnumValue(key, index)
             index += 1
             yield tpl
-        except OSError as e:
-            if e.winerror == ERROR_NO_MORE_ITEMS:
-                break
-            else:
-                raise
 
 ################################################################################
 
 _RegQueryValueEx = fun_fact(
     _adv.RegQueryValueExW, (
         LONG,
         HKEY,
@@ -1263,36 +1254,36 @@
         LastWritten=cred.LastWritten,
         Persist=cred.Persist,
         TargetAlias=cred.TargetAlias,
         )
 
 ################################################################################
 
-def CreadRead(TargetName, Type=CRED_TYPE_GENERIC, Flags=0):
+def CreadRead(target_name, typ=CRED_TYPE_GENERIC, flags=0):
     ptr = PCREDENTIAL()
     try:
-        raise_on_zero(_CredRead(TargetName, Type, Flags, ref(ptr)))
+        raise_on_zero(_CredRead(target_name, typ, flags, ref(ptr)))
         return _ns_from_cred(ptr.contents)
     finally:
         _CredFree(ptr)
 
 ################################################################################
 
-def CredEnumerate(Filter=None, Flags=0):
+def CredEnumerate(filter=None, flags=0):
     pptr = PPCREDENTIAL()
     cnt = DWORD()
     try:
-        raise_on_zero(_CredEnumerate(Filter, Flags, ref(cnt), ref(pptr)))
+        raise_on_zero(_CredEnumerate(filter, flags, ref(cnt), ref(pptr)))
         return tuple(_ns_from_cred(pptr[n].contents) for n in range(cnt.value))
     finally:
         _CredFree(pptr)
 
 ################################################################################
 
-def CredWrite(Credential, Flags=0):
+def CredWrite(credential, flags=0):
 
     # ============================== std fields ================================
 
     std_fields = (
         "Flags",
         "Type",
         "TargetName",
@@ -1300,38 +1291,38 @@
         "LastWritten",
         "Persist",
         "TargetAlias",
         "UserName",
         )
     cred = CREDENTIAL()
     for f in std_fields:
-        if (val := getattr(Credential, f, None)) is not None:
+        if (val := getattr(credential, f, None)) is not None:
             setattr(cred, f, val)
 
     # ================================= blob ===================================
 
-    if (val := getattr(Credential, "CredentialBlob", None)) is not None:
+    if (val := getattr(credential, "CredentialBlob", None)) is not None:
         cred.CredentialBlobSize = len(val)
         cred.CredentialBlob = (BYTE * len(val))(*tuple(map(int, val)))
 
     # ============================== attributes ================================
 
-    if ns_attr := getattr(Credential, "Attributes", None):
+    if ns_attr := getattr(credential, "Attributes", None):
         attr = (CREDENTIAL_ATTRIBUTE * len(ns_attr))()
         for i, a in enumerate(ns_attr):
             for f in ("Keyword", "Flags"):
                 if (val := getattr(a, f, None)) is not None:
                     setattr(attr[i], f, val)
             if val := getattr(a, "Value", None):
                 attr[i].ValueSize = len(val)
                 attr[i].Value = (BYTE * len(val))(*tuple(map(int, val)))
         cred.AttributeCount = len(ns_attr)
         cred.Attributes = ctypes.cast(attr, PCREDENTIAL_ATTRIBUTE)
 
-    raise_on_zero(_CredWrite(ref(cred), Flags))
+    raise_on_zero(_CredWrite(ref(cred), flags))
 
 ################################################################################
 
 _CloseEventLog = fun_fact(_adv.CloseEventLog, (BOOL, HANDLE))
 
 def CloseEventLog(hdl):
     raise_on_zero(_CloseEventLog(hdl))
@@ -1340,15 +1331,15 @@
 
 class EHANDLE(ScdToBeClosed, HANDLE, close_func=CloseEventLog, invalid=0):
     pass
 
 ################################################################################
 
 _OpenEventLog = fun_fact(
-    _adv.OpenEventLogW, (HANDLE, PWSTR, PWSTR,)
+    _adv.OpenEventLogW, (HANDLE, PWSTR, PWSTR)
     )
 
 def OpenEventLog(source, server=None):
     hdl = EHANDLE(_OpenEventLog(server, source))
     hdl.raise_on_invalid()
     return hdl
 
@@ -1390,22 +1381,22 @@
 
 def _evt_from_void_p(vpelr):
     # vpelr is PVOID for simpler address calculations
     strins = []
     elr = ctypes.cast(vpelr, PEVENTLOGRECORD).contents
     if elr.NumStrings:
         stroffs = elr.StringOffset
-        for i in range(elr.NumStrings):
+        for _ in range(elr.NumStrings):
             nxt = ctypes.wstring_at(vpelr.value + stroffs)
             stroffs += (len(nxt) + 1) * ctypes.sizeof(WCHAR)
             strins.append(nxt)
     sid = ""
     if elr.UserSidLength:
         sid = ConvertSidToStringSid(
-            ctypes.string_at(vpelr.value + elr.UserSidOffset)
+            ctypes.string_at(vpelr.value + elr.UserSidOffset, elr.UserSidLength)
             )
     data = ctypes.string_at(vpelr.value + elr.DataOffset, elr.DataLength)
     p_str = vpelr.value + ctypes.sizeof(EVENTLOGRECORD)
     src_name = ctypes.wstring_at(p_str)
     p_str += (len(src_name) + 1) * ctypes.sizeof(WCHAR)
     computer_name = ctypes.wstring_at(p_str)
```

### Comparing `ctwin32-2.1.0/ctwin32/bcrypt.py` & `ctwin32-2.2.0/ctwin32/bcrypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,27 +477,36 @@
         ULONG
         )
     )
 
 def BCryptSignHash(key, digest, flags=0):
     size = ULONG()
     raise_failed_status(
-        _BCryptSignHash(key, None, digest, len(digest), None, 0, ref(size), 0)
+        _BCryptSignHash(
+            key,
+            None,
+            digest,
+            len(digest),
+            None,
+            0,
+            ref(size),
+            flags
+            )
         )
     signature = ctypes.create_string_buffer(size.value)
     raise_failed_status(
         _BCryptSignHash(
             key,
             None,
             digest,
             len(digest),
             signature,
             len(signature),
             ref(size),
-            0
+            flags
             )
         )
     return bytes(signature)
 
 ################################################################################
 
 _BCryptVerifySignature = fun_fact(
```

### Comparing `ctwin32-2.1.0/ctwin32/cfgmgr.py` & `ctwin32-2.2.0/ctwin32/cfgmgr.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/ctwin32/comctl.py` & `ctwin32-2.2.0/ctwin32/comctl.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,25 @@
     manifest = (
         "<assembly xmlns='urn:schemas-microsoft-com:asm.v1' manifestVersion=",
         "'1.0'><dependency><dependentAssembly><assemblyIdentity type='win32'",
         " name='Microsoft.Windows.Common-Controls' version='6.0.0.0' ",
         "processorArchitecture='*' publicKeyToken='6595b64144ccf1df' ",
         "language='*'/></dependentAssembly></dependency></assembly>"
         )
+
+    # simply doing the following would lead to a sharing violation :-(
+    #
+    # with tempfile.NamedTemporaryFile() as f:
+    #     tmp_name = f.name
+    #     f.write("".join(manifest).encode("ascii"))
+    #     actx.lpSource = tmp_name
+    #     ctx = kernel.CreateActCtx(actx) # <- sharing violation here
+    #
+    # so it gets a little more complicated...
+
     tmp_name = None
     try:
         with tempfile.NamedTemporaryFile(delete=False) as f:
             tmp_name = f.name
             f.write("".join(manifest).encode("ascii"))
 
         # create activation context from manifest file
@@ -87,17 +98,19 @@
         ctx = kernel.CreateActCtx(actx)
     finally:
         # delete temporary file
         if tmp_name is not None:
             pathlib.Path(tmp_name).unlink()
 
     # activate context, load libray and and release the context
-    cookie = kernel.ActivateActCtx(ctx)
+    kernel.ActivateActCtx(ctx)
     comctl = ctypes.WinDLL("comctl32.dll")  # <- this calls LoadLibrary
-    kernel.DeactivateActCtx(0, cookie)
+
+    # Do NOT deactivate the context! Just decrement its ref-count by
+    # releasing it.
     kernel.ReleaseActCtx(ctx)
 
     # verify DLL version
     class DLLVERSIONINFO(ctypes.Structure):
         _fields_ = (
             ("cbSize", DWORD),
             ("dwMajorVersion", DWORD),
```

### Comparing `ctwin32-2.1.0/ctwin32/gdi.py` & `ctwin32-2.2.0/ctwin32/gdi.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/ctwin32/iphlpapi.py` & `ctwin32-2.2.0/ctwin32/iphlpapi.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/ctwin32/kernel.py` & `ctwin32-2.2.0/ctwin32/kernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,36 +38,42 @@
     PBYTE,
     PDWORD,
     POINTER,
     PSIZE_T,
     PULONG_PTR,
     PUSHORT,
     PVOID,
+    PWIN32_FIND_DATA,
     PWSTR,
     ScdToBeClosed,
     SHORT,
     SIZE_T,
     SYSTEMTIME,
     UINT,
     UINT_PTR,
     ULONG,
     ULONG_PTR,
     USHORT,
     WCHAR,
+    WIN32_FIND_DATA,
     WORD,
     )
 from . import (
     ref,
     raise_if,
     raise_on_zero,
     fun_fact,
+    ERROR_ACCESS_DENIED,
+    ERROR_FILE_NOT_FOUND,
     ERROR_INSUFFICIENT_BUFFER,
+    ERROR_NO_MORE_FILES,
     ERROR_RESOURCE_ENUM_USER_STOP,
     ERROR_RESOURCE_NAME_NOT_FOUND,
     ERROR_SUCCESS,
+    FILE_ATTRIBUTE_DIRECTORY,
     FILE_TYPE_CHAR,
     FILE_TYPE_UNKNOWN,
     INVALID_FILE_ATTRIBUTES,
     INVALID_HANDLE_VALUE,
     IMAGE_FILE_MACHINE_UNKNOWN,
     IMAGE_FILE_MACHINE_AMD64,
     IMAGE_FILE_MACHINE_I386,
@@ -260,21 +266,21 @@
         PVOID,
         DWORD,
         PDWORD,
         POVERLAPPED
         )
     )
 
-def DeviceIoControl(hdl, ioctl, in_bytes, out_len):
+def DeviceIoControl(hdl, ioctl, in_ctobj, out_len):
     bytes_returned = DWORD(0)
 
-    if in_bytes is None:
+    if in_ctobj is None or in_ctobj == 0:
         iptr, ilen = None, 0
     else:
-        iptr, ilen = ref(in_bytes), len(in_bytes)
+        iptr, ilen = ref(in_ctobj), ctypes.sizeof(in_ctobj)
 
     if out_len is None or out_len == 0:
         out, optr, olen = None, None, 0
     else:
         out = ctypes.create_string_buffer(out_len)
         optr, olen = ref(out), out_len
 
@@ -365,14 +371,25 @@
     )
 
 def TerminateProcess(handle, exit_code):
     raise_on_zero(_TerminateProcess(handle, exit_code))
 
 ################################################################################
 
+_GetExitCodeProcess = fun_fact(
+    _k32.GetExitCodeProcess, (BOOL, HANDLE, PDWORD)
+    )
+
+def GetExitCodeProcess(handle):
+    exit_code = DWORD()
+    raise_on_zero(_GetExitCodeProcess(handle, ref(exit_code)))
+    return exit_code.value
+
+################################################################################
+
 _QueryDosDevice = fun_fact(
     _k32.QueryDosDeviceW, (DWORD, PWSTR, PWSTR, DWORD)
     )
 
 def QueryDosDevice(device_name):
     size = 512
     buf = ctypes.create_unicode_buffer(size)
@@ -440,17 +457,17 @@
 def FileTimeToLocalSystemTime(ft):
     st = FileTimeToSystemTime(ft)
     raise_on_zero(_k32.SystemTimeToTzSpecificLocalTime(0, ref(st), ref(st)))
     return st
 
 ################################################################################
 
-def AdjustTime(SecondsToAdjust):
+def AdjustTime(seconds_to_adjust):
     ft = GetSystemTimeAsFileTime()
-    ft += int(SecondsToAdjust * 1e7)
+    ft += int(seconds_to_adjust * 1e7)
     st = FileTimeToSystemTime(ft)
     raise_on_zero(_k32.SetSystemTime(ref(st)))
 
 ################################################################################
 
 def GetCurrentThreadId():
     return _k32.GetCurrentThreadId()
@@ -510,15 +527,15 @@
     size = 512
     buf = ctypes.create_unicode_buffer(size)
     res = _GetPrivateProfileSectionNames(buf, size, filename)
     while res == size - 2:
         size *= 2
         buf = ctypes.create_unicode_buffer(size)
         res = _GetPrivateProfileSectionNames(buf, size, filename)
-    return buf[:res].split('\0')[:-1]
+    return buf[:res].split("\0")[:-1]
 
 ################################################################################
 
 _GetPrivateProfileSection = fun_fact(
     _k32.GetPrivateProfileSectionW,
     (DWORD, PWSTR, PWSTR, DWORD, PWSTR)
     )
@@ -527,18 +544,18 @@
     size = 512
     buf = ctypes.create_unicode_buffer(size)
     res = _GetPrivateProfileSection(secname, buf, size, filename)
     while res == size - 2:
         size *= 2
         buf = ctypes.create_unicode_buffer(size)
         res = _GetPrivateProfileSection(secname, buf, size, filename)
-    entries = buf[:res].split('\0')[:-1]
+    entries = buf[:res].split("\0")[:-1]
     d = _collections.OrderedDict()
     for e in entries:
-        k, v = e.split('=', 1)
+        k, v = e.split("=", 1)
         d[k] = v
     return d
 
 ################################################################################
 
 _WritePrivateProfileSection = fun_fact(
     _k32.WritePrivateProfileSectionW,
@@ -575,16 +592,15 @@
     size = 512
     while True:
         var = ctypes.create_unicode_buffer(size)
         req = _GetEnvironmentVariable(name, var, size)
         raise_on_zero(req)
         if req <= size:
             break
-        else:
-            size = req
+        size = req
     return var.value
 
 ################################################################################
 
 _SetEnvironmentVariable = fun_fact(
     _k32.SetEnvironmentVariableW,
     (BOOL, PWSTR, PWSTR)
@@ -641,16 +657,15 @@
     size = len(template)
     while True:
         var = ctypes.create_unicode_buffer(size)
         req = _ExpandEnvironmentStrings(template, var, size)
         raise_on_zero(req)
         if req <= size:
             break
-        else:
-            size = req
+        size = req
     return var.value
 
 ################################################################################
 
 class PROCESS_INFORMATION(ctypes.Structure):
     _fields_ = (
         ("hProcess", KHANDLE),
@@ -962,16 +977,15 @@
     size = 512
     while True:
         var = ctypes.create_unicode_buffer(size)
         req = _GlobalGetAtomName(atom, var, size)
         raise_on_zero(req)
         if req <= size:
             break
-        else:
-            size = req
+        size = req
     return var.value
 
 ################################################################################
 
 _FreeLibrary = fun_fact(_k32.FreeLibrary, (BOOL, HANDLE))
 
 def FreeLibrary(hmod):
@@ -1125,15 +1139,15 @@
                     if entry.Flags == MESSAGE_RESOURCE_UNICODE:
                         msg = ctypes.wstring_at(taddr, slen // 2)
                     else:
                         msg = ctypes.string_at(taddr, slen).decode(
                             "utf-8" if entry.Flags == MESSAGE_RESOURCE_UTF8
                             else get_ansi_encoding()
                             )
-                    return msg.strip('\0')
+                    return msg.strip("\0")
 
     raise ctypes.WinError(ERROR_RESOURCE_NAME_NOT_FOUND)
 
 ################################################################################
 
 class SYSTEM_INFO(ctypes.Structure):
     _fields_ = (
@@ -1353,7 +1367,91 @@
 
 def SetThreadErrorMode(mode):
     old = DWORD()
     raise_on_zero(_SetThreadErrorMode(mode, ref(old)))
     return old.value
 
 ################################################################################
+
+_FindClose = fun_fact(_k32.FindClose, (BOOL, HANDLE))
+
+def FindClose(hdl):
+    raise_on_zero(_FindClose(hdl))
+
+################################################################################
+
+class FFHANDLE(
+        ScdToBeClosed,
+        HANDLE,
+        close_func=FindClose,
+        invalid=INVALID_HANDLE_VALUE
+        ):
+    pass
+
+################################################################################
+
+_FindFirstFile = fun_fact(
+    _k32.FindFirstFileW, (HANDLE, PWSTR, PWIN32_FIND_DATA)
+    )
+
+def FindFirstFile(name, ignore_not_found=False):
+    find_data = WIN32_FIND_DATA()
+    hdl = FFHANDLE(_FindFirstFile(name, ref(find_data)))
+    if not hdl.is_valid():
+        err = GetLastError()
+        if ignore_not_found and err == ERROR_FILE_NOT_FOUND:
+            return None, None
+        raise ctypes.WinError(err)
+    return hdl, find_data
+
+################################################################################
+
+_FindNextFile = fun_fact(
+    _k32.FindNextFileW, (BOOL, HANDLE, PWIN32_FIND_DATA)
+    )
+
+def FindNextFile(hdl):
+    find_data = WIN32_FIND_DATA()
+    res = _FindNextFile(hdl, ref(find_data))
+    if not res:
+        err = GetLastError()
+        if err == ERROR_NO_MORE_FILES:
+            return None
+        raise ctypes.WinError(err)
+    return find_data
+
+################################################################################
+
+def iter_dir(directory, ignore_access_denied=True):
+    pattern = str(directory) + "\\*"
+    try:
+        hdl, info = FindFirstFile(pattern, True)
+    except OSError as e:
+        if ignore_access_denied and e.winerror == ERROR_ACCESS_DENIED:
+            return
+        raise
+    if hdl is None:
+        return
+    with hdl:
+        while True:
+            yield directory, info
+            is_sub = (
+                bool(info.dwFileAttributes & FILE_ATTRIBUTE_DIRECTORY) and
+                info.cFileName != "." and
+                info.cFileName != ".."
+                )
+            if is_sub:
+                sub = rf"{directory}\{info.cFileName}"
+                yield from iter_dir(sub, ignore_access_denied)
+
+            info = FindNextFile(hdl)
+            if info is None:
+                break
+
+################################################################################
+
+def find_file(name):
+    hdl, info = FindFirstFile(name)
+    hdl.close()
+    return info
+
+################################################################################
```

### Comparing `ctwin32-2.1.0/ctwin32/misc.py` & `ctwin32-2.2.0/ctwin32/misc.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/ctwin32/msi.py` & `ctwin32-2.2.0/ctwin32/msi.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     ScdToBeClosed,
     UINT,
     ULONG,
     )
 from . import (
     ref,
     raise_on_err,
+    suppress_winerr,
     fun_fact,
     ERROR_MORE_DATA,
     ERROR_NO_MORE_ITEMS
     )
 
 _msi = ctypes.WinDLL("msi.dll")
 
@@ -108,24 +109,18 @@
     hdl = MSIHANDLE()
     raise_on_err(_MsiViewFetch(view, ref(hdl)))
     return hdl
 
 ################################################################################
 
 def view_enum_records(view):
-    while True:
-        try:
-            record = MsiViewFetch(view)
-        except OSError as e:
-            if e.winerror == ERROR_NO_MORE_ITEMS:
-                break
-            else:
-                raise
-        with record:
-            yield record
+    with suppress_winerr(ERROR_NO_MORE_ITEMS):
+        while True:
+            with MsiViewFetch(view) as record:
+                yield record
 
 ################################################################################
 
 _MsiRecordGetString = fun_fact(
     _msi.MsiRecordGetStringW, (
         UINT,
         MSIHANDLE,
```

### Comparing `ctwin32-2.1.0/ctwin32/ntdll.py` & `ctwin32-2.2.0/ctwin32/ntdll.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,18 @@
     FILETIME,
     HANDLE,
     LARGE_INTEGER,
     LONG,
     LONG_PTR,
     INT,
     NTSTATUS,
+    OSVERSIONINFOEX,
     PBOOLEAN,
     POINTER,
+    POSVERSIONINFOEX,
     PULONG,
     PUNICODE_STRING,
     PVOID,
     UINT,
     UINT_PTR,
     ULARGE_INTEGER,
     ULONG,
@@ -49,14 +51,16 @@
     WCHAR,
     WORD,
     )
 from . import (
     ref,
     kernel,
     fun_fact,
+    ns_from_struct,
+    suppress_winerr,
     ERROR_FILE_NOT_FOUND,
     ERROR_NO_MORE_FILES,
     SystemProcessInformation,
     SystemProcessIdInformation,
     SystemExtendedHandleInformation,
     ProcessImageFileName,
     ProcessBasicInformation,
@@ -279,52 +283,46 @@
         pid = pi.UniqueProcessId if pi.UniqueProcessId else 0
         name = (
             str(pi.ImageName) if pi.ImageName.Buffer else
             ("idle" if pid == 0 else "system")
             )
         return _namespace(name=name, pid=pid)
 
-    res = []
     status = STATUS_INFO_LENGTH_MISMATCH
     while status == STATUS_INFO_LENGTH_MISMATCH:
         size = required_sys_info_size(SystemProcessInformation)
         buf = ctypes.create_string_buffer(size.value)
         status = NtQuerySystemInformation(
             SystemProcessInformation,
             ref(buf),
             size,
             ref(size)
             )
     raise_failed_status(status)
 
     pi = SYSTEM_PROCESS_INFORMATION.from_address(ctypes.addressof(buf))
-    res.append(_name_pid(pi))
+    res = [_name_pid(pi)]
 
-    while True:
-        if (offs := pi.NextEntryOffset) == 0:
-            break
+    while pi.NextEntryOffset:
         pi = SYSTEM_PROCESS_INFORMATION.from_address(
-            ctypes.addressof(pi) + offs
+            ctypes.addressof(pi) + pi.NextEntryOffset
             )
         res.append(_name_pid(pi))
     return res
 
 ################################################################################
 
 def _resolve_device_prefix(fname):
     dos_devices = {}
     for dc in "abcdefghijklmnopqrstuvwxyz":
         dn = dc + ":"
-        try:
+        with suppress_winerr(ERROR_FILE_NOT_FOUND):
             dos_devices[kernel.QueryDosDevice(dn)] = dn
-        except OSError as e:
-            if e.winerror != ERROR_FILE_NOT_FOUND:
-                raise e
 
-    for ddk in dos_devices.keys():
+    for ddk in dos_devices:
         if fname.startswith(ddk):
             fname = fname.replace(ddk, dos_devices[ddk], 1)
             break
     return fname
 
 ################################################################################
 
@@ -381,16 +379,15 @@
     _NtQuerySystemInformation(info, ref(hi), ctypes.sizeof(hi), ref(rlen))
     hi = _make_handle_info(hi.NumberOfHandles)
     raise_failed_status(
         _NtQuerySystemInformation(info, ref(hi), ctypes.sizeof(hi), ref(rlen))
         )
     if pid == -1:
         return list(hi.Handles)
-    else:
-        return [h for h in hi.Handles if pid == h.UniqueProcessId]
+    return [h for h in hi.Handles if pid == h.UniqueProcessId]
 
 ################################################################################
 
 def get_grouped_handles(pid=-1):
     grouped_handles = _defdict(list)
     for h in get_handles(pid):
         grouped_handles[h.UniqueProcessId].append(h)
@@ -501,19 +498,15 @@
             buf,
             bsize,
             1,  # FileDirectoryInformation
             False,
             None,
             restart_scan
             )
-        too_short = (
-            stat == STATUS_BUFFER_OVERFLOW
-            or stat == STATUS_INFO_LENGTH_MISMATCH
-            )
-        if too_short:
+        if stat in (STATUS_BUFFER_OVERFLOW, STATUS_INFO_LENGTH_MISMATCH):
             bsize *= 2
         else:
             break
     raise_failed_status(stat)
 
     pv = ctypes.cast(ctypes.addressof(buf), PVOID)
     dinfo = ctypes.cast(
@@ -539,19 +532,51 @@
         FileName=name,
         )
 
 ################################################################################
 
 def enum_directory_info(hdir):
     restart_scan = True
-    while True:
-        try:
+    with suppress_winerr(ERROR_NO_MORE_FILES):
+        while True:
             info = get_directory_info(hdir, restart_scan)
             restart_scan = False
             yield info
-        except OSError as e:
-            if e.winerror == ERROR_NO_MORE_FILES:
-                break
-            else:
-                raise
+
+################################################################################
+
+_RtlGetVersion = fun_fact(_nt.RtlGetVersion, (NTSTATUS, POSVERSIONINFOEX))
+
+def RtlGetVersion():
+    osve = OSVERSIONINFOEX()
+    raise_failed_status(_RtlGetVersion(ref(osve)))
+    return ns_from_struct(osve)
+
+################################################################################
+
+_NtPowerInformation = fun_fact(
+    _nt.NtPowerInformation, (
+        NTSTATUS,
+        LONG,
+        PVOID,
+        ULONG,
+        PVOID,
+        ULONG,
+        )
+    )
+
+def NtPowerInformation(pwr_info, in_bytes, out_len):
+    if in_bytes is None:
+        iptr, ilen = None, 0
+    else:
+        iptr, ilen = ref(in_bytes), len(in_bytes)
+
+    if out_len is None or out_len == 0:
+        out, optr, olen = ctypes.create_string_buffer(0), None, 0
+    else:
+        out = ctypes.create_string_buffer(out_len)
+        optr, olen = ref(out), out_len
+
+    raise_failed_status(_NtPowerInformation(pwr_info, iptr, ilen, optr, olen))
+    return out.raw
 
 ################################################################################
```

### Comparing `ctwin32-2.1.0/ctwin32/psapi.py` & `ctwin32-2.2.0/ctwin32/psapi.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/ctwin32/secur.py` & `ctwin32-2.2.0/ctwin32/secur.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     PPLUID,
     PVOID,
     PULONG,
     SYSTEMTIME,
     UNICODE_STRING,
     ULONG,
     )
-from . import ref, fun_fact
+from . import ref, fun_fact, suppress_winerr, ERROR_INVALID_PARAMETER
 from .ntdll import raise_failed_status
 from .kernel import FileTimeToLocalFileTime, FileTimeToSystemTime
 from .advapi import GetLengthSid, ConvertSidToStringSid
 
 _sec = ctypes.WinDLL("secur32.dll")
 
 ################################################################################
@@ -103,19 +103,16 @@
     ptr = PSECURITY_LOGON_SESSION_DATA()
     raise_failed_status(_LsaGetLogonSessionData(ref(luid), ref(ptr)))
     try:
         lsd = ptr.contents
         lli = lsd.LastLogonInfo
 
         def la2dt(la):
-            st = FileTimeToSystemTime(FILETIME(la))
-            if st.Year > 9999:
-                # datetime cannot handle years > 9999
-                st = SYSTEMTIME(9999, 12, 0, 31)
-            else:
+            st = FileTimeToSystemTime(FILETIME(0))
+            with suppress_winerr(ERROR_INVALID_PARAMETER):
                 st = FileTimeToSystemTime(FileTimeToLocalFileTime(FILETIME(la)))
             return st.to_datetime()
 
         return _namespace(
             LogonId=int(lsd.LogonId),
             UserName=str(lsd.UserName),
             LogonDomain=str(lsd.LogonDomain),
@@ -157,15 +154,15 @@
     )
 
 def LsaEnumerateLogonSessions():
     count = ULONG()
     pluid = PLUID()
     raise_failed_status(_LsaEnumerateLogonSessions(ref(count), ref(pluid)))
     try:
-        result = []
-        for idx in reversed(range(count.value)):
-            result.append(LsaGetLogonSessionData(pluid[idx]))
-        return result
+        return [
+            LsaGetLogonSessionData(pluid[idx])
+            for idx in reversed(range(count.value))
+            ]
     finally:
         LsaFreeReturnBuffer(pluid)
 
 ################################################################################
```

### Comparing `ctwin32-2.1.0/ctwin32/setupapi.py` & `ctwin32-2.2.0/ctwin32/setupapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,24 +41,26 @@
     ULONG_PTR,
     WCHAR,
     )
 from . import (
     ref,
     raise_on_zero,
     fun_fact,
+    suppress_winerr,
     INVALID_HANDLE_VALUE,
     DIGCF_PRESENT,
     DIGCF_ALLCLASSES,
     DIGCF_DEVICEINTERFACE,
     DICS_ENABLE,
     DICS_DISABLE,
     DICS_FLAG_CONFIGSPECIFIC,
     DIF_PROPERTYCHANGE,
     SPDRP_DEVICEDESC,
     ERROR_NO_MORE_ITEMS,
+    ERROR_NOT_FOUND,
     )
 from .cfgmgr import (
     CM_Get_Device_ID,
     CM_Get_DevNode_Status,
     CM_Enumerate_Enumerators,
     CM_Enumerate_Classes,
     )
@@ -179,33 +181,29 @@
     return _SetupDiEnumDeviceInfo(info_set, idx, deinda)
 
 ################################################################################
 
 def get_device_enumerators():
     res = []
     idx = 0
-    while True:
-        try:
+    with suppress_winerr(ERROR_NOT_FOUND):
+        while True:
             res.append(CM_Enumerate_Enumerators(idx))
             idx += 1
-        except OSError:
-            break
     return res
 
 ################################################################################
 
 def get_device_classes(flags=0):
     res = []
     idx = 0
-    while True:
-        try:
+    with suppress_winerr(ERROR_NOT_FOUND):
+        while True:
             res.append(CM_Enumerate_Classes(idx, flags))
             idx += 1
-        except OSError:
-            break
     return res
 
 ################################################################################
 
 _SetupDiClassNameFromGuid = fun_fact(
     _sua.SetupDiClassNameFromGuidW,
     (BOOL, PGUID, PWSTR, DWORD, PDWORD)
@@ -538,23 +536,19 @@
 
 ################################################################################
 
 def enum_dev_interfaces(guid):
     flags = DIGCF_PRESENT | DIGCF_DEVICEINTERFACE
     with SetupDiGetClassDevs(flags=flags, guid=guid) as info_set:
         idx = 0
-        while True:
-            try:
+        with suppress_winerr(ERROR_NO_MORE_ITEMS):
+            while True:
                 did = SetupDiEnumDeviceInterfaces(info_set, guid, idx)
-            except OSError as e:
-                if e.winerror == ERROR_NO_MORE_ITEMS:
-                    break
-                raise
-            idx += 1
-            yield info_set, did
+                idx += 1
+                yield info_set, did
 
 ################################################################################
 
 _SetupDiGetDeviceInterfaceDetail = fun_fact(
     _sua.SetupDiGetDeviceInterfaceDetailW, (
         BOOL,
         HANDLE,
```

### Comparing `ctwin32-2.1.0/ctwin32/shell.py` & `ctwin32-2.2.0/ctwin32/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,17 +169,20 @@
         wait=False,
         show=SW_SHOW
         ):
     sei = SHELLEXECUTEINFOW(str(file), verb, param, direc, wait, show)
 
     raise_on_zero(_ShellExecuteExW(ref(sei)))
 
+    rc = None
     if sei.hProcess is not None:
         kernel.WaitForSingleObject(sei.hProcess, INFINITE)
+        rc = kernel.GetExitCodeProcess(sei.hProcess)
         kernel.CloseHandle(sei.hProcess)
+    return rc
 
 ################################################################################
 
 def elevate(*args, direc=None, wait=False, show=SW_SHOW):
     file, param = args[0], cmdline_from_args(args[1:])
     ShellExecuteEx(file, "runas", param, direc, wait, show)
```

### Comparing `ctwin32-2.1.0/ctwin32/user.py` & `ctwin32-2.2.0/ctwin32/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     LRESULT,
     NTSTATUS,
     PDWORD,
     POINT,
     POINTER,
     PPOINT,
     PPVOID,
+    PPWSTR,
     PRECT,
     PVOID,
     PWSTR,
     SHORT,
     RECT,
     UINT,
     UINT_PTR,
@@ -61,32 +62,32 @@
 from . import (
     ref,
     kernel,
     raise_if,
     raise_on_zero,
     raise_on_err,
     fun_fact,
-    WAIT_FAILED,
+    CF_UNICODETEXT,
+    GMEM_MOVEABLE,
     GWL_STYLE,
     GWL_EXSTYLE,
     INPUT_KEYBOARD,
     KEYEVENTF_KEYUP,
-    MONITOR_DEFAULTTOPRIMARY,
-    SWP_NOSIZE,
-    SWP_NOZORDER,
-    GMEM_MOVEABLE,
-    CF_UNICODETEXT,
     LR_DEFAULTSIZE,
+    MONITOR_DEFAULTTOPRIMARY,
     SPI_GETNONCLIENTMETRICS,
     SPI_SETNONCLIENTMETRICS,
     SPI_GETWHEELSCROLLLINES,
     SPI_SETWHEELSCROLLLINES,
     SPI_GETWORKAREA,
     SPIF_UPDATEINIFILE,
     SPIF_SENDCHANGE,
+    SWP_NOSIZE,
+    SWP_NOZORDER,
+    WAIT_FAILED,
     WM_QUIT,
     )
 from .ntdll import (
     RtlNtStatusToDosError,
     proc_path_from_pid,
     STATUS_BUFFER_TOO_SMALL,
     )
@@ -391,15 +392,15 @@
         cl = self.__class__.__name__
         ln = self.length
         fl = self.flags
         sc = self.showCmd
         mi = f"({self.MinPosition.x}, {self.MinPosition.y})"
         ma = f"({self.MaxPosition.x}, {self.MaxPosition.y})"
         no = (
-            f"({self.NormalPosition.left}, {self.NormalPosition.top}, " +
+            f"({self.NormalPosition.left}, {self.NormalPosition.top}, ",
             f"{self.NormalPosition.right}, {self.NormalPosition.bottom})"
             )
         return f"{cl}({ln}, {fl}, {sc}, {mi}, {ma}, {no})"
 
 PWINDOWPLACEMENT = POINTER(WINDOWPLACEMENT)
 
 ################################################################################
@@ -551,15 +552,15 @@
         try:
             num = len(inputs)
             if not num:
                 return
             inputs = (INPUT * num)(*inputs)
             ptr = ctypes.cast(inputs, PINPUT)
         except Exception as e:
-            raise TypeError(f"expected INPUT or list of INPUTs: {e}")
+            raise TypeError(f"expected INPUT or list of INPUTs: {e}") from e
     raise_on_zero(_SendInput(num, ptr, ctypes.sizeof(INPUT)))
 
 ################################################################################
 
 _ExitWindowsEx = fun_fact(_usr.ExitWindowsEx, (BOOL, UINT, DWORD))
 
 def ExitWindowsEx(flags, reason):
@@ -613,16 +614,15 @@
     return mi
 
 ################################################################################
 
 def get_wnd_center(hwnd=None):
     if hwnd is None:
         return GetMonitorInfo(MonitorFromWindow(None)).rcMonitor.center
-    else:
-        return GetWindowRect(hwnd).center
+    return GetWindowRect(hwnd).center
 
 ################################################################################
 
 def center_wnd(to_be_centered, center_on=None):
     center_x, center_y = get_wnd_center(center_on)
     rc = GetWindowRect(to_be_centered)
     SetWindowPos(
@@ -644,32 +644,39 @@
 
     with kernel.create_process(arglist) as pi:
         WaitForInputIdle(pi.hProcess, 10000)
         EnumThreadWindows(pi.dwThreadId, center_wnd_cb, None)
 
 ################################################################################
 
+_LoadString = fun_fact(_usr.LoadStringW, (INT, HANDLE, UINT, PPWSTR, INT))
+
+def LoadString(hinst, strid):
+    ptr = PWSTR()
+    raise_on_zero(res := _LoadString(hinst, strid, ref(ptr), 0))
+    return ctypes.wstring_at(ptr, res)
+
+################################################################################
+
 _LoadCursor = fun_fact(_usr.LoadCursorW, (HANDLE, HANDLE, PWSTR))
 
 def LoadCursor(hinst, cname):
     if isinstance(cname, int) and cname < 2**16:
         cname = ctypes.cast(cname, PWSTR)
-    res = _LoadCursor(hinst, cname)
-    raise_on_zero(res)
+    raise_on_zero(res := _LoadCursor(hinst, cname))
     return res
 
 ################################################################################
 
 _LoadIcon = fun_fact(_usr.LoadIconW, (HANDLE, HANDLE, PWSTR))
 
 def LoadIcon(hinst, cname):
     if isinstance(cname, int) and cname < 2**16:
         cname = ctypes.cast(cname, PWSTR)
-    res = _LoadIcon(hinst, cname)
-    raise_on_zero(res)
+    raise_on_zero(res := _LoadIcon(hinst, cname))
     return res
 
 ################################################################################
 
 _DefWindowProc = fun_fact(
     _usr.DefWindowProcW, (LRESULT, HWND, UINT, WPARAM, LPARAM)
     )
@@ -1221,15 +1228,15 @@
         if not copied:
             kernel.GlobalFree(hcopy)
 
 ################################################################################
 
 def txt_from_clip(hwnd=None):
     if not IsClipboardFormatAvailable(CF_UNICODETEXT):
-        raise EnvironmentError("no clipboard text available")
+        raise OSError("no clipboard text available")
     OpenClipboard(hwnd)
     hmem = GetClipboardData(CF_UNICODETEXT)
     txt = ctypes.wstring_at(kernel.GlobalLock(hmem))
     kernel.GlobalUnlock(hmem)
     CloseClipboard()
     return txt
```

### Comparing `ctwin32-2.1.0/ctwin32/version.py` & `ctwin32-2.2.0/ctwin32/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     PWSTR,
     UINT,
     WORD,
     )
 from . import (
     ref,
     raise_on_zero,
+    suppress_winerr,
     fun_fact,
     ns_from_struct,
     ERROR_RESOURCE_TYPE_NOT_FOUND,
     )
 
 _ver = ctypes.WinDLL("version.dll")
 
@@ -96,16 +97,15 @@
 
 def VerQueryValue(block, subblock):
     value = PVOID()
     size = UINT()
     raise_on_zero(_VerQueryValue(block, subblock, ref(value), ref(size)))
     if "StringFileInfo" in subblock:
         return ctypes.wstring_at(value.value, size.value).strip("\0")
-    else:
-        return ctypes.string_at(value.value, size.value)
+    return ctypes.string_at(value.value, size.value)
 
 ################################################################################
 
 def get_binary_info(fname, block=None):
     if block is None:
         block = GetFileVersionInfo(fname)
     return ns_from_struct(
@@ -148,15 +148,12 @@
 
     # just take the first language
     lc = _LANG_CP.from_buffer_copy(lc_array)
     lang = f"\\StringFileInfo\\{lc.lang:04x}{lc.cp:04x}\\"
 
     result = {}
     for k in _str_info_names:
-        try:
+        with suppress_winerr(ERROR_RESOURCE_TYPE_NOT_FOUND):
             result[k] = VerQueryValue(block, lang + k)
-        except OSError as e:
-            if e.winerror != ERROR_RESOURCE_TYPE_NOT_FOUND:
-                raise
     return result
 
 ################################################################################
```

### Comparing `ctwin32-2.1.0/ctwin32/virtdisk.py` & `ctwin32-2.2.0/ctwin32/virtdisk.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 VIRTUAL_DISK_ACCESS_WRITABLE = 0x320000
 
 OPEN_VIRTUAL_DISK_FLAG_NONE = 0
 OPEN_VIRTUAL_DISK_FLAG_NO_PARENTS = 0x1
 OPEN_VIRTUAL_DISK_FLAG_BLANK_FILE = 0x2
 OPEN_VIRTUAL_DISK_FLAG_BOOT_DRIVE = 0x4
 OPEN_VIRTUAL_DISK_FLAG_CACHED_IO = 0x8
-OPEN_VIRTUAL_DISK_FLAG_CUSTOM_DIFF_CHAIN = 0x10,
+OPEN_VIRTUAL_DISK_FLAG_CUSTOM_DIFF_CHAIN = 0x10
 OPEN_VIRTUAL_DISK_FLAG_PARENT_CACHED_IO = 0x20
 OPEN_VIRTUAL_DISK_FLAG_VHDSET_FILE_ONLY = 0x40
 OPEN_VIRTUAL_DISK_FLAG_IGNORE_RELATIVE_PARENT_LOCATOR = 0x80
 OPEN_VIRTUAL_DISK_FLAG_NO_WRITE_HARDENING = 0x100
 OPEN_VIRTUAL_DISK_FLAG_SUPPORT_COMPRESSED_VOLUMES = 0x200
 
 OPEN_VIRTUAL_DISK_VERSION_UNSPECIFIED = 0
```

### Comparing `ctwin32-2.1.0/ctwin32/wndcls.py` & `ctwin32-2.2.0/ctwin32/wndcls.py`

 * *Files 20% similar despite different names*

```diff
@@ -345,18 +345,18 @@
 
     def end_paint(self, ps):
         user.EndPaint(self.hwnd, ps)
 
     def set_prop(self, name, data):
         user.SetProp(self.hwnd, name, data)
 
-    def get_prop(self, name, data):
+    def get_prop(self, name):
         return user.GetProp(self.hwnd, name)
 
-    def get_prop_def(self, name, data, default=None):
+    def get_prop_def(self, name, default=None):
         return user.get_prop_def(self.hwnd, name, default)
 
     def del_prop(self, name):
         return user.RemoveProp(self.hwnd, name)
 
 ################################################################################
 ################################################################################
@@ -380,17 +380,17 @@
 def _exception_in_callback(err_info):
     # During a callback from C code into python code (through ctypes) an
     # exception occured in that python code - described by the string
     # 'err_info'. Since there is no possibility to propagate this exception
     # to the python interpreter, we have to terminate the process. Before we
     # do that, we try to inform the user.
 
-    if sys.stderr is None or not hasattr(sys.stderr, 'mode'):
+    if sys.stderr is None or not hasattr(sys.stderr, "mode"):
         user.txt_to_clip(err_info)
-        err_info += '\nThe above text has been copied to the clipboard.'
+        err_info += "\nThe above text has been copied to the clipboard."
         user.MessageBox(
             None,
             err_info,
             "Terminating program",
             MB_OK | MB_ICONERROR
             )
     else:
@@ -444,16 +444,15 @@
 
             cparam = user.CREATESTRUCT.from_address(lp).lpCreateParams
             self = ctypes.cast(cparam, ctypes.py_object).value
             if isinstance(self, SimpleWnd):
                 self.hwnd = hwnd
                 self.set_prop(_PROP_SELF, cparam)
                 return self.on_message(msg, wp, lp)
-            else:
-                raise TypeError("not derived from SimpleWnd")
+            raise TypeError("not derived from SimpleWnd")
         except BaseException:
             _exception_in_callback(traceback.format_exc())
 
     ############################################################################
 
     def create(self, wcp):
         if self.is_window():
@@ -511,73 +510,73 @@
 
 def load_ico_lz_b85(lz_b85_data):
     return user.CreateIconFromResourceEx(from_lzb85(lz_b85_data))
 
 ################################################################################
 
 _py_icon = (
-    b'{Wp48S^xk9=GL@E0stWa761SMbT8$j;1H(;>RkX705Aj)f+J6yP9T}Bko})j#+i7N>;e(Cc8'
-    b'*b~t=p!4Q*Y-|8I`wx%g@F}t$1qY3`ER*6QY*}qNii+qAYq`NROBYh+Ot_RpNEGPRoAI1^Td'
-    b'&(&<AnDap)j_o`+IK<rpFw3)<etl<IYLkGU|B2d7e`60A9qtCtFsg1{>=)qA*sCV&QUE12Nq'
-    b'qR_6W0oGLTfny)d!CWv4njsF>CeO1THX!>_^ENrpO&Oy0;%fq$|!F3nno<dnv3(2y{c&itUa'
-    b'1iK56!K;Z`9i*&0yl8zC$m9Tv+nv1#?r;S#KU<`4!FpMXj?Ht_jotwz*o?L-cp`Gc?6%uw_6'
-    b't-iWwadkQ7p<wFOI{#$S>sEa%fQbn&d5~&Tf->4?!WxGsv#=5n_b6v8kR;1Cxo}y}5chHkKd'
-    b'+8<F2RVe^G^ZEH+XgIa*gbPH{u*_zX);IzvXAhgqBMc`{q6a%PeKwiU|3SKU_TZo;yWN+Jy5'
-    b'{H{pQ+Q)RoAL)HBGYX-&-tgz0xCGDfYU0rZ3x-h+7onOS%J|hx^_kxhEy4c&JL<s`(xMxnMY'
-    b'3?)MsDJGWRx;uosq;9nuFDfkJz-rEujXPpx0UITtH-mffmG<;y@p5W9+R*F!}6-#vKH-+lyX'
-    b';J+#?QvOB7uPy4C53q`2Bt%8BHejw~~yQp1p{IKP_zJ3!Oq7|+)Ds@pyQ_64-$*ww>zN_2t5'
-    b'o6k+215Gr)oYa5_P2;!g`oDgxp@9XFqjZ0x0m6TN5EZEvT?mtyP@QR*?VdVxiqkI%LqCL_04'
-    b'8HcMK?Ej3afNs@Qs2L9gev&tW=$BmQbP*Gs+reQAWKocl|u*?5E^;`<qa9m|E&NKq1GAK$lC'
-    b'4gp*7+h$GLJ;1nx8-No(Y%o*@?nBP8sE3D2`G3|+d)3Ul+wliQ~7A9gsR8N!>nL@g}ZSFIE<'
-    b'3m(pl;5Ur1C9Mqcuyh-kf^e??xt{`a4E{mmds6mf6NUP&GKgkxYRM(g}FU5>lb>wTQ(m8dsL'
-    b'{N-YuOa>4c3fm+n`!MpQ_(c6FmIq5-rI5_=(FhR{10ek%v;Pb!Y9)b1iKktnF@^w8;oP<S57'
-    b'B-quZtTE=3L>_6TdPcc0A*;>4w-Y=gs%Z@-EDdv0g4m8a#V|5<Zt;?(@wYrVb-Mk1Zdw%Y09'
-    b'Gn=e1&7;wA~N&ryFEU*V)J&^KvQY@Ak>Zm{0ooZsRK7?-#1(gu$iVqGdslP=0S|Q3<Fa-xec'
-    b'8uu5r%nQ4UlsMx^Vni(7Bskl7aQdNJe>Db2}fWQ}$geIyG@D7n&OyNG7>c!_70Cy>lzy?L6p'
-    b'<=%0-^CQkVI#_teeId#xO_L^xsUL?ycSIzlppqI74YA6(Zt6g{fFa6gQ(#f&Xs(UOr7@lz7L'
-    b'Xc%_<xA_oa^vO}LkvmhHHq%Qe_z3^am;#oZ~$FtL3o@Cl{K^hF6+CUh+JE8-<96BRbQ2sw+0'
-    b'07hXrCaq6ZRIn6iVjyQ^ufxm4gbLmXnMgIjh?7(|D&?Nlb2S%9rK@)Jz_irCdm`I{$-zZLXJ'
-    b'v!RG$;h}KR@@r7eX*74~#4FYiyZBtxv8w`%IDomf2+mQ=p-v-~~BnB4ky$7MTefMN~%ZLb%`'
-    b'9HAuZy>YC5wbuq}fsUv>XN>?<(K|l9W_i0*$<>pocq&1w+=2XX=ZTZ!b+9?|3)6=`R%F!}Z&'
-    b'a3Qm#HB{fW|T^Vk!~MbAjB%uoKE2KB?<{2C4_7P^XpCPOvLvb*=`u!@U??9&!FwtogjvKchT'
-    b'JYXIjeMr`}Q^G8vJ%n;<f;*!&FZ!Ihx~1V$NR`5Y3LJT5Gs{MWKOM$(1PgZT`{b##@>Y~@{s'
-    b')vnA~VaZp}VEy{WN=0EzUX~N5K4PI_3hVd(<@S@?%#NnfV#o&CTj&LSlM;dAJ}n;7UKjmt%e'
-    b'cG-MV+#m^)RYoItH4F4SpRv>o$*ci&39VZ{Gn)82#qhvYI77MY6k>v2iQs00000F``J)J91k'
-    b'700D*!s38CVB-0#!vBYQl0ssI200dcD'
+    b"{Wp48S^xk9=GL@E0stWa761SMbT8$j;1H(;>RkX705Aj)f+J6yP9T}Bko})j#+i7N>;e(Cc8"
+    b"*b~t=p!4Q*Y-|8I`wx%g@F}t$1qY3`ER*6QY*}qNii+qAYq`NROBYh+Ot_RpNEGPRoAI1^Td"
+    b"&(&<AnDap)j_o`+IK<rpFw3)<etl<IYLkGU|B2d7e`60A9qtCtFsg1{>=)qA*sCV&QUE12Nq"
+    b"qR_6W0oGLTfny)d!CWv4njsF>CeO1THX!>_^ENrpO&Oy0;%fq$|!F3nno<dnv3(2y{c&itUa"
+    b"1iK56!K;Z`9i*&0yl8zC$m9Tv+nv1#?r;S#KU<`4!FpMXj?Ht_jotwz*o?L-cp`Gc?6%uw_6"
+    b"t-iWwadkQ7p<wFOI{#$S>sEa%fQbn&d5~&Tf->4?!WxGsv#=5n_b6v8kR;1Cxo}y}5chHkKd"
+    b"+8<F2RVe^G^ZEH+XgIa*gbPH{u*_zX);IzvXAhgqBMc`{q6a%PeKwiU|3SKU_TZo;yWN+Jy5"
+    b"{H{pQ+Q)RoAL)HBGYX-&-tgz0xCGDfYU0rZ3x-h+7onOS%J|hx^_kxhEy4c&JL<s`(xMxnMY"
+    b"3?)MsDJGWRx;uosq;9nuFDfkJz-rEujXPpx0UITtH-mffmG<;y@p5W9+R*F!}6-#vKH-+lyX"
+    b";J+#?QvOB7uPy4C53q`2Bt%8BHejw~~yQp1p{IKP_zJ3!Oq7|+)Ds@pyQ_64-$*ww>zN_2t5"
+    b"o6k+215Gr)oYa5_P2;!g`oDgxp@9XFqjZ0x0m6TN5EZEvT?mtyP@QR*?VdVxiqkI%LqCL_04"
+    b"8HcMK?Ej3afNs@Qs2L9gev&tW=$BmQbP*Gs+reQAWKocl|u*?5E^;`<qa9m|E&NKq1GAK$lC"
+    b"4gp*7+h$GLJ;1nx8-No(Y%o*@?nBP8sE3D2`G3|+d)3Ul+wliQ~7A9gsR8N!>nL@g}ZSFIE<"
+    b"3m(pl;5Ur1C9Mqcuyh-kf^e??xt{`a4E{mmds6mf6NUP&GKgkxYRM(g}FU5>lb>wTQ(m8dsL"
+    b"{N-YuOa>4c3fm+n`!MpQ_(c6FmIq5-rI5_=(FhR{10ek%v;Pb!Y9)b1iKktnF@^w8;oP<S57"
+    b"B-quZtTE=3L>_6TdPcc0A*;>4w-Y=gs%Z@-EDdv0g4m8a#V|5<Zt;?(@wYrVb-Mk1Zdw%Y09"
+    b"Gn=e1&7;wA~N&ryFEU*V)J&^KvQY@Ak>Zm{0ooZsRK7?-#1(gu$iVqGdslP=0S|Q3<Fa-xec"
+    b"8uu5r%nQ4UlsMx^Vni(7Bskl7aQdNJe>Db2}fWQ}$geIyG@D7n&OyNG7>c!_70Cy>lzy?L6p"
+    b"<=%0-^CQkVI#_teeId#xO_L^xsUL?ycSIzlppqI74YA6(Zt6g{fFa6gQ(#f&Xs(UOr7@lz7L"
+    b"Xc%_<xA_oa^vO}LkvmhHHq%Qe_z3^am;#oZ~$FtL3o@Cl{K^hF6+CUh+JE8-<96BRbQ2sw+0"
+    b"07hXrCaq6ZRIn6iVjyQ^ufxm4gbLmXnMgIjh?7(|D&?Nlb2S%9rK@)Jz_irCdm`I{$-zZLXJ"
+    b"v!RG$;h}KR@@r7eX*74~#4FYiyZBtxv8w`%IDomf2+mQ=p-v-~~BnB4ky$7MTefMN~%ZLb%`"
+    b"9HAuZy>YC5wbuq}fsUv>XN>?<(K|l9W_i0*$<>pocq&1w+=2XX=ZTZ!b+9?|3)6=`R%F!}Z&"
+    b"a3Qm#HB{fW|T^Vk!~MbAjB%uoKE2KB?<{2C4_7P^XpCPOvLvb*=`u!@U??9&!FwtogjvKchT"
+    b"JYXIjeMr`}Q^G8vJ%n;<f;*!&FZ!Ihx~1V$NR`5Y3LJT5Gs{MWKOM$(1PgZT`{b##@>Y~@{s"
+    b")vnA~VaZp}VEy{WN=0EzUX~N5K4PI_3hVd(<@S@?%#NnfV#o&CTj&LSlM;dAJ}n;7UKjmt%e"
+    b"cG-MV+#m^)RYoItH4F4SpRv>o$*ci&39VZ{Gn)82#qhvYI77MY6k>v2iQs00000F``J)J91k"
+    b"700D*!s38CVB-0#!vBYQl0ssI200dcD"
     )
 
 def load_py_ico():
     return load_ico_lz_b85(_py_icon)
 
 ################################################################################
 
 _ctwin32_icon = (
-    b'{Wp48S^xk9=GL@E0stWa761SMbT8$j;0UJ#&0PQ#05Aj)f+J6yaHvHu1q>Gs(yZ)`rT4VqYn'
-    b'%B-HIH~>jeV{SNI_{JHVRTYsiKzK7CwQ=tJ2Ks!~srhl-I*p0o!hI-fpo^97Xi*4Q!Dd3X}v'
-    b'$8WKulmA{F!7oZCs)IAY;ZLMh6_No@b0ca=PkNzVlN3cC!ob60RrU0=4ndqroAy}qIF?$;ZH'
-    b'Ufdr4QqNydBJoi**2(b>LJtsq1--PQVunbK*nFuD0^<0YG0-)S3tS_@5y)&cQ=s^k)-n~=oM'
-    b'02WzYUu?pZecGjm&)ry+Orfv<jRMfx!kc1P+ahYuS(p%J>Y|E(NvE5ZQb(61)+uYPYcZKA?4'
-    b'y3*?c3~|o@e>T)A&e2>Qsiwrg(x})20YiS)c@q~frD|ufg|rFed$7w!;pG&;vB0orztE80g1'
-    b'5I$1~{%oA8kJqG8F5WFuF%de0KZlqk)<^C2K?eE3mj3mf16t&%ma@|F%17nc2|)O8_#Lldac'
-    b'FKC#?m7Ga6mIU+oCQ4>>QHY^>Au-AQr)+1y^BmO-flIkHJsV)N);I;ebT<`hX9)46w<Rg3FL'
-    b'i)nM%7pg~SO#qz-ze-1-*zMpUl#X<!?Q_$_PfG77v&?(kBe4H7IG?zCE?~%aW3h~O~Nk#)1H'
-    b'v=0R1#>@CNEYYT5RzSq>D#w>P>#BfdIYc)Z?l^6ml~-ykX8X8NnIqKq+G;v$hN(Y<Jt)r?c9'
-    b'>GCHY0zJilG#Dgj6g&_Ar1vUBMuh7e1c=)&+mJs_S(AEH(w+z@wOPz`09ec$bD^<B20sPmtQ'
-    b';9O8ejb}|4A@5yHoQ|la1UXI=fK{SBk8E0dNDC-7yw%?a9h+@fRDw!w6q>w{eR6p%f9?J2ey'
-    b'sbWHE%E5LjOC=}=%xLInY)d36&`<eV73u+U8SBisPCILL$*_AbshRHS~A(Eo9HFi__M)NO{L'
-    b'k}hiLF?7EhWwHZo$Xt984N&;?2^{2k^@GcRUbM$+nhqIJ0$;#L=XESY=_B_hRlCH6Hx-@ItE'
-    b'@4C^*r-Z*y%%>?H81t0$s$1c97#vHl%HhMw%^^5Tid??!_#@o>WP7mN#K1i21pownz?8>#_R'
-    b'67v0mi1&j!iRKMdj-fwjC}mJ4deM2@pDkT)?qtiS1a~80#D^R~9XM3@7QZL?zs-ZA-pCJo6{'
-    b'R>GbdV}c`%kbaf1&ZpLT&u%w>OgdQZ*~7)q(fpFA=qdeAt|9=O5NX(*%bl8iYPJ(FJbra1Lc'
-    b'1<m23X?h%S;!h}bzIodaWjLg}aLqJ_oc`_kb`^egLfTdLSI6#rFaK)MtiwsG%!qr%(+$M7=i'
-    b'FsygaUfDcG1`f1)_y!(vw(U!A(ly-<MbTl&@rjG$BKX<x{({u@XJ*QsEUvq@f(bmc6v=U8!5'
-    b'}p{K5@GE7Jm9Z!Bv3CFo#1ZHV7*nTNaA10bQO+6x22LetMJ2b#}!7h6#~GL*UD=`~w_>msdT'
-    b'YdUl6{}zNFtK;1wkl9@$K|*;m;I}jOF`7rfqE9`8A2}5MAYGOm&Bd@13Bgk?!sLhcJ65PFvq'
-    b'EK-oczoVl#{I->+Rapc9fQ>LT)>~&`%W3cz@D3$X)<L+qpZSQ4LslJyc~^rDkdX00000gHzk'
-    b'KXFSSV00HR<s1X1FO9VA)vBYQl0ssI200dcD'
+    b"{Wp48S^xk9=GL@E0stWa761SMbT8$j;0UJ#&0PQ#05Aj)f+J6yaHvHu1q>Gs(yZ)`rT4VqYn"
+    b"%B-HIH~>jeV{SNI_{JHVRTYsiKzK7CwQ=tJ2Ks!~srhl-I*p0o!hI-fpo^97Xi*4Q!Dd3X}v"
+    b"$8WKulmA{F!7oZCs)IAY;ZLMh6_No@b0ca=PkNzVlN3cC!ob60RrU0=4ndqroAy}qIF?$;ZH"
+    b"Ufdr4QqNydBJoi**2(b>LJtsq1--PQVunbK*nFuD0^<0YG0-)S3tS_@5y)&cQ=s^k)-n~=oM"
+    b"02WzYUu?pZecGjm&)ry+Orfv<jRMfx!kc1P+ahYuS(p%J>Y|E(NvE5ZQb(61)+uYPYcZKA?4"
+    b"y3*?c3~|o@e>T)A&e2>Qsiwrg(x})20YiS)c@q~frD|ufg|rFed$7w!;pG&;vB0orztE80g1"
+    b"5I$1~{%oA8kJqG8F5WFuF%de0KZlqk)<^C2K?eE3mj3mf16t&%ma@|F%17nc2|)O8_#Lldac"
+    b"FKC#?m7Ga6mIU+oCQ4>>QHY^>Au-AQr)+1y^BmO-flIkHJsV)N);I;ebT<`hX9)46w<Rg3FL"
+    b"i)nM%7pg~SO#qz-ze-1-*zMpUl#X<!?Q_$_PfG77v&?(kBe4H7IG?zCE?~%aW3h~O~Nk#)1H"
+    b"v=0R1#>@CNEYYT5RzSq>D#w>P>#BfdIYc)Z?l^6ml~-ykX8X8NnIqKq+G;v$hN(Y<Jt)r?c9"
+    b">GCHY0zJilG#Dgj6g&_Ar1vUBMuh7e1c=)&+mJs_S(AEH(w+z@wOPz`09ec$bD^<B20sPmtQ"
+    b";9O8ejb}|4A@5yHoQ|la1UXI=fK{SBk8E0dNDC-7yw%?a9h+@fRDw!w6q>w{eR6p%f9?J2ey"
+    b"sbWHE%E5LjOC=}=%xLInY)d36&`<eV73u+U8SBisPCILL$*_AbshRHS~A(Eo9HFi__M)NO{L"
+    b"k}hiLF?7EhWwHZo$Xt984N&;?2^{2k^@GcRUbM$+nhqIJ0$;#L=XESY=_B_hRlCH6Hx-@ItE"
+    b"@4C^*r-Z*y%%>?H81t0$s$1c97#vHl%HhMw%^^5Tid??!_#@o>WP7mN#K1i21pownz?8>#_R"
+    b"67v0mi1&j!iRKMdj-fwjC}mJ4deM2@pDkT)?qtiS1a~80#D^R~9XM3@7QZL?zs-ZA-pCJo6{"
+    b"R>GbdV}c`%kbaf1&ZpLT&u%w>OgdQZ*~7)q(fpFA=qdeAt|9=O5NX(*%bl8iYPJ(FJbra1Lc"
+    b"1<m23X?h%S;!h}bzIodaWjLg}aLqJ_oc`_kb`^egLfTdLSI6#rFaK)MtiwsG%!qr%(+$M7=i"
+    b"FsygaUfDcG1`f1)_y!(vw(U!A(ly-<MbTl&@rjG$BKX<x{({u@XJ*QsEUvq@f(bmc6v=U8!5"
+    b"}p{K5@GE7Jm9Z!Bv3CFo#1ZHV7*nTNaA10bQO+6x22LetMJ2b#}!7h6#~GL*UD=`~w_>msdT"
+    b"YdUl6{}zNFtK;1wkl9@$K|*;m;I}jOF`7rfqE9`8A2}5MAYGOm&Bd@13Bgk?!sLhcJ65PFvq"
+    b"EK-oczoVl#{I->+Rapc9fQ>LT)>~&`%W3cz@D3$X)<L+qpZSQ4LslJyc~^rDkdX00000gHzk"
+    b"KXFSSV00HR<s1X1FO9VA)vBYQl0ssI200dcD"
     )
 
 def load_ctwin32_ico():
     return load_ico_lz_b85(_ctwin32_icon)
 
 ################################################################################
 
@@ -633,16 +632,15 @@
                     return False
             else:
                 self = ctypes.cast(lp, ctypes.py_object).value
                 if isinstance(self, BaseDlg):
                     self.hwnd = hwnd
                     self.set_prop(_PROP_SELF, lp)
                     return self.on_init_dialog()
-                else:
-                    raise TypeError("not derived from BaseDlg")
+                raise TypeError("not derived from BaseDlg")
         except BaseException:
             _exception_in_callback(traceback.format_exc())
 
     ############################################################################
 
     def create_modeless(self, template):
         return user.CreateDialogIndirectParam(
@@ -819,15 +817,15 @@
 
         self.center(self.parent)
         return True
 
     ############################################################################
 
     def on_command(self, cmd_id, notification, ctrl):
-        if cmd_id == IDOK or cmd_id == IDCANCEL:
+        if cmd_id in (IDOK, IDCANCEL):
             if cmd_id == IDOK:
                 self.answer = self.get_item_text(self.ANSWER_ID)
             user.EndDialog(self.hwnd, cmd_id)
         return True
 
     ############################################################################
 
@@ -842,11 +840,10 @@
             215,
             72,
             caption,
             "MS Shell Dlg",
             (self.fontsize * self.get_dpi_scale_100() + 50) // 100
             )
 
-        if self.do_modal(template) == IDOK:
-            return self.answer
+        return self.answer if self.do_modal(template) == IDOK else None
 
 ################################################################################
```

### Comparing `ctwin32-2.1.0/ctwin32/wtypes.py` & `ctwin32-2.2.0/ctwin32/wtypes.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 ################################################################################
 
 import sys
 import ctypes
 from uuid import UUID
 from datetime import datetime
 
+# avoid circular dependency: ctwin32 -> wtypes -> ctwin32
+MAX_PATH = 260
+
 ################################################################################
 
 # integral types
 
 ENDIANNESS = sys.byteorder
 
 BYTE = ctypes.c_ubyte
@@ -299,14 +302,53 @@
         ("lfQuality", BYTE),
         ("lfPitchAndFamily", BYTE),
         ("lfFaceName", WCHAR * 32),
         )
 
 ################################################################################
 
+class OSVERSIONINFOEX(ctypes.Structure):
+    _fields_ = (
+        ("dwOSVersionInfoSize", DWORD),
+        ("dwMajorVersion", DWORD),
+        ("dwMinorVersion", DWORD),
+        ("dwBuildNumber", DWORD),
+        ("dwPlatformId", DWORD),
+        ("szCSDVersion", WCHAR * 128),
+        ("wServicePackMajor", WORD),
+        ("wServicePackMinor", WORD),
+        ("wSuiteMask", WORD),
+        ("wProductType", BYTE),
+        ("wReserved", BYTE),
+        )
+
+    def __init__(self):
+        self.dwOSVersionInfoSize = ctypes.sizeof(self)
+
+################################################################################
+
+class WIN32_FIND_DATA(ctypes.Structure):
+    _fields_ = (
+        ("dwFileAttributes", DWORD),
+        ("ftCreationTime", FILETIME),
+        ("ftLastAccessTime", FILETIME),
+        ("ftLastWriteTime", FILETIME),
+        ("nFileSizeHigh", DWORD),
+        ("nFileSizeLow", DWORD),
+        ("dwReserved0", DWORD),
+        ("dwReserved1", DWORD),
+        ("cFileName", WCHAR * MAX_PATH),
+        ("cAlternateFileName", WCHAR * 14),
+        ("dwFileType", DWORD),     # obsolete - do not use
+        ("dwCreatorType", DWORD),  # obsolete - do not use
+        ("wFinderFlags", WORD),    # obsolete - do not use
+        )
+
+################################################################################
+
 # pointer types
 
 PWSTR = ctypes.c_wchar_p
 PSTR = ctypes.c_char_p
 PVOID = ctypes.c_void_p
 POINTER = ctypes.POINTER
 PPWSTR = POINTER(PWSTR)
@@ -332,14 +374,16 @@
 PRECT = POINTER(RECT)
 PULONGLONG = POINTER(ULONGLONG)
 PUNICODE_STRING = POINTER(UNICODE_STRING)
 PLUID = POINTER(LUID)
 PPLUID = POINTER(PLUID)
 CallbackContextPtr = POINTER(CallbackContext)
 PLOGFONT = POINTER(LOGFONT)
+POSVERSIONINFOEX = POINTER(OSVERSIONINFOEX)
+PWIN32_FIND_DATA = POINTER(WIN32_FIND_DATA)
 
 ################################################################################
 
 # A class that allows to create types (by multiple inheritance) that are based
 # on ctypes._SimpleCData and can be used as context managers (i.e. can be used
 # in 'with' statements) in order to ensure that handles are orderly closed.
 # When defining such a type it must be configured with the approriate base
```

### Comparing `ctwin32-2.1.0/ctwin32.egg-info/PKG-INFO` & `ctwin32-2.2.0/ctwin32.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctwin32
-Version: 2.1.0
+Version: 2.2.0
 Summary: Access selected win32 APIs through ctypes
 Author: Rocco Matano
 License: MIT License
 Project-URL: homepage, https://github.com/RoccoMatano/ctwin32
 Project-URL: changelog, https://github.com/RoccoMatano/ctwin32/blob/master/changelog.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,20 +16,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ![](https://raw.githubusercontent.com/RoccoMatano/ctwin32/master/doc/images/ctwin32.ico) ctwin32
-
+# ![logo](https://raw.githubusercontent.com/RoccoMatano/ctwin32/master/doc/images/ctwin32.ico) ctwin32
 
 [![PyPI - Version](https://img.shields.io/pypi/v/ctwin32.svg)](https://pypi.org/project/ctwin32)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ctwin32.svg)](https://pypi.org/project/ctwin32)
 [![License - MIT](https://img.shields.io/badge/license-MIT-green)](https://spdx.org/licenses/MIT.html)
+[![PyPI - Stats](https://img.shields.io/pypi/dm/ctwin32)](https://pypistats.org/packages/ctwin32)
 
 -----
 
 ctwin32 is a pure Python module, that wraps some Windows APIs (win32) by using
 [ctypes](https://docs.python.org/3/library/ctypes.html). Since it is my personal
 playground, the selection of supported APIs and the way those are wrapped are
 solely dictated by my needs and preferences.
```

### Comparing `ctwin32-2.1.0/ctwin32.egg-info/SOURCES.txt` & `ctwin32-2.2.0/ctwin32.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 samples/fopa.py
 samples/hello_wnd.pyw
 samples/keyview.pyw
 samples/listpipes.py
 samples/logonsessions.py
 samples/netifaces.py
 samples/np_dev.py
+samples/power_requests.py
+samples/print_reparse_points.py
 samples/py_ver.py
 samples/remove_drive_by_letter.py
 samples/rm_sign_tool.py
 samples/senv.py
 samples/simple_aes.py
 samples/stopnow.py
 samples/sua_enums.py
```

### Comparing `ctwin32-2.1.0/pyproject.toml` & `ctwin32-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/arp_table.py` & `ctwin32-2.2.0/samples/arp_table.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/atta_vdisk.py` & `ctwin32-2.2.0/samples/atta_vdisk.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/calendar.pyw` & `ctwin32-2.2.0/samples/calendar.pyw`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/dump_ver_res.py` & `ctwin32-2.2.0/samples/dump_ver_res.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/endis_bsl_usb.py` & `ctwin32-2.2.0/samples/endis_bsl_usb.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/exbinmsi.py` & `ctwin32-2.2.0/samples/exbinmsi.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/extract_ico.py` & `ctwin32-2.2.0/samples/extract_ico.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/find_zombies.py` & `ctwin32-2.2.0/samples/find_zombies.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/fopa.py` & `ctwin32-2.2.0/samples/fopa.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/hello_wnd.pyw` & `ctwin32-2.2.0/samples/hello_wnd.pyw`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/keyview.pyw` & `ctwin32-2.2.0/samples/keyview.pyw`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/listpipes.py` & `ctwin32-2.2.0/samples/listpipes.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/logonsessions.py` & `ctwin32-2.2.0/samples/logonsessions.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/netifaces.py` & `ctwin32-2.2.0/samples/netifaces.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/np_dev.py` & `ctwin32-2.2.0/samples/np_dev.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/py_ver.py` & `ctwin32-2.2.0/samples/py_ver.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/remove_drive_by_letter.py` & `ctwin32-2.2.0/samples/remove_drive_by_letter.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/rm_sign_tool.py` & `ctwin32-2.2.0/samples/rm_sign_tool.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/senv.py` & `ctwin32-2.2.0/samples/senv.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/simple_aes.py` & `ctwin32-2.2.0/samples/simple_aes.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/stopnow.py` & `ctwin32-2.2.0/samples/stopnow.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/sua_enums.py` & `ctwin32-2.2.0/samples/sua_enums.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/test_sign_tool.py` & `ctwin32-2.2.0/samples/test_sign_tool.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/samples/uptime_evt.py` & `ctwin32-2.2.0/samples/uptime_evt.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,13 +36,14 @@
                     return e.TimeGenerated
             some_events = advapi.ReadEventLog(log)
     raise EnvironmentError("no boot event found")
 
 def up_time(time_boot=None):
     if time_boot is None:
         time_boot = boot_time()
-    return datetime.datetime.now() - time_boot
+    utime = datetime.datetime.now() - time_boot
+    return datetime.timedelta(seconds=int(utime.total_seconds()))
 
 if __name__ == "__main__":
     t_boot = boot_time()
     print(f"This computer was booted on {t_boot}.")
     print(f"It has been running for {up_time(t_boot)}.")
```

### Comparing `ctwin32-2.1.0/samples/virt_term_seq.py` & `ctwin32-2.2.0/samples/virt_term_seq.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.1.0/setup.py` & `ctwin32-2.2.0/setup.py`

 * *Files identical despite different names*

