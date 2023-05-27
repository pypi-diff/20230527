# Comparing `tmp/customtkinterx-0.1.0.tar.gz` & `tmp/customtkinterx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customtkinterx-0.1.0.tar", max compression
+gzip compressed data, was "customtkinterx-0.1.1.tar", max compression
```

## Comparing `customtkinterx-0.1.0.tar` & `customtkinterx-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      251 2023-05-27 08:34:56.407692 customtkinterx-0.1.0/customtkinterx/__init__.py
--rw-r--r--   0        0        0     3775 2023-05-27 09:25:30.265070 customtkinterx-0.1.0/customtkinterx/CTkCustom.py
--rw-r--r--   0        0        0     5306 2023-05-27 08:36:14.109297 customtkinterx-0.1.0/customtkinterx/CTkFluentTheme.py
--rw-r--r--   0        0        0     4686 2023-05-27 08:31:22.732978 customtkinterx-0.1.0/customtkinterx/Fluent.json
--rw-r--r--   0        0        0      344 2023-05-27 09:43:44.168234 customtkinterx-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1048 2023-05-27 09:39:01.342825 customtkinterx-0.1.0/README.md
--rw-r--r--   0        0        0     1380 1970-01-01 00:00:00.000000 customtkinterx-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      251 2023-05-27 08:34:56.407692 customtkinterx-0.1.1/customtkinterx/__init__.py
+-rw-r--r--   0        0        0     3775 2023-05-27 09:25:30.265070 customtkinterx-0.1.1/customtkinterx/CTkCustom.py
+-rw-r--r--   0        0        0     5306 2023-05-27 08:36:14.109297 customtkinterx-0.1.1/customtkinterx/CTkFluentTheme.py
+-rw-r--r--   0        0        0     4686 2023-05-27 08:31:22.732978 customtkinterx-0.1.1/customtkinterx/Fluent.json
+-rw-r--r--   0        0        0      343 2023-05-27 09:47:17.417981 customtkinterx-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1048 2023-05-27 09:39:01.342825 customtkinterx-0.1.1/README.md
+-rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 customtkinterx-0.1.1/PKG-INFO
```

### Comparing `customtkinterx-0.1.0/customtkinterx/CTkCustom.py` & `customtkinterx-0.1.1/customtkinterx/CTkCustom.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.1.0/customtkinterx/CTkFluentTheme.py` & `customtkinterx-0.1.1/customtkinterx/CTkFluentTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.1.0/customtkinterx/Fluent.json` & `customtkinterx-0.1.1/customtkinterx/Fluent.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.1.0/README.md` & `customtkinterx-0.1.1/README.md`

 * *Files identical despite different names*

