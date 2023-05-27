# Comparing `tmp/automation_file_dev-0.0.1.tar.gz` & `tmp/automation_file_dev-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_file_dev-0.0.1.tar", last modified: Sun Apr 30 07:10:12 2023, max compression
+gzip compressed data, was "automation_file_dev-0.0.2.tar", last modified: Sat May 27 05:08:15 2023, max compression
```

## Comparing `automation_file_dev-0.0.1.tar` & `automation_file_dev-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 07:10:12.718994 automation_file_dev-0.0.1/
--rw-rw-rw-   0        0        0     1084 2023-04-29 15:33:58.000000 automation_file_dev-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      648 2023-04-30 07:10:12.717997 automation_file_dev-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-04-29 15:33:58.000000 automation_file_dev-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 07:10:12.707027 automation_file_dev-0.0.1/automation_file_dev.egg-info/
--rw-rw-rw-   0        0        0      648 2023-04-30 07:10:12.000000 automation_file_dev-0.0.1/automation_file_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-04-30 07:10:12.000000 automation_file_dev-0.0.1/automation_file_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 07:10:12.000000 automation_file_dev-0.0.1/automation_file_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-30 07:10:12.000000 automation_file_dev-0.0.1/automation_file_dev.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-30 07:10:12.708023 automation_file_dev-0.0.1/file_automation/
--rw-rw-rw-   0        0        0        0 2023-04-29 15:36:35.000000 automation_file_dev-0.0.1/file_automation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:10:12.711016 automation_file_dev-0.0.1/file_automation/excel/
--rw-rw-rw-   0        0        0        0 2023-04-29 17:31:01.000000 automation_file_dev-0.0.1/file_automation/excel/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-29 17:31:16.000000 automation_file_dev-0.0.1/file_automation/excel/openyxl_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:10:12.714008 automation_file_dev-0.0.1/file_automation/pdf/
--rw-rw-rw-   0        0        0        0 2023-04-29 17:32:43.000000 automation_file_dev-0.0.1/file_automation/pdf/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-29 17:32:57.000000 automation_file_dev-0.0.1/file_automation/pdf/pypdf_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:10:12.715004 automation_file_dev-0.0.1/file_automation/utils/
--rw-rw-rw-   0        0        0        0 2023-04-29 16:59:14.000000 automation_file_dev-0.0.1/file_automation/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:10:12.716999 automation_file_dev-0.0.1/file_automation/word/
--rw-rw-rw-   0        0        0        0 2023-04-29 18:01:26.000000 automation_file_dev-0.0.1/file_automation/word/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-29 18:01:40.000000 automation_file_dev-0.0.1/file_automation/word/python_docx_wrapper.py
--rw-rw-rw-   0        0        0      877 2023-04-30 07:07:03.000000 automation_file_dev-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 07:10:12.719992 automation_file_dev-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 05:08:15.761092 automation_file_dev-0.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-04-29 15:33:58.000000 automation_file_dev-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1376 2023-05-27 05:08:15.760095 automation_file_dev-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-05-26 18:14:27.000000 automation_file_dev-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 05:08:15.739946 automation_file_dev-0.0.2/automation_file_dev.egg-info/
+-rw-rw-rw-   0        0        0     1376 2023-05-27 05:08:15.000000 automation_file_dev-0.0.2/automation_file_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2023-05-27 05:08:15.000000 automation_file_dev-0.0.2/automation_file_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 05:08:15.000000 automation_file_dev-0.0.2/automation_file_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-27 05:08:15.000000 automation_file_dev-0.0.2/automation_file_dev.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 05:08:15.740894 automation_file_dev-0.0.2/file_automation/
+-rw-rw-rw-   0        0        0      712 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 05:08:15.744066 automation_file_dev-0.0.2/file_automation/dir/
+-rw-rw-rw-   0        0        0        0 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/dir/__init__.py
+-rw-rw-rw-   0        0        0     1230 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/dir/dir_process.py
+drwxrwxrwx   0        0        0        0 2023-05-27 05:08:15.748059 automation_file_dev-0.0.2/file_automation/file/
+-rw-rw-rw-   0        0        0        0 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/file/__init__.py
+-rw-rw-rw-   0        0        0     2205 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/file/file_process.py
+drwxrwxrwx   0        0        0        0 2023-05-27 05:08:15.750053 automation_file_dev-0.0.2/file_automation/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-29 16:59:14.000000 automation_file_dev-0.0.2/file_automation/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 05:08:15.756105 automation_file_dev-0.0.2/file_automation/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      165 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-27 05:08:15.758100 automation_file_dev-0.0.2/file_automation/zip/
+-rw-rw-rw-   0        0        0        0 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/zip/__init__.py
+-rw-rw-rw-   0        0        0     2383 2023-05-20 05:53:45.000000 automation_file_dev-0.0.2/file_automation/zip/zip_process.py
+-rw-rw-rw-   0        0        0      877 2023-05-27 05:07:53.000000 automation_file_dev-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 05:08:15.761092 automation_file_dev-0.0.2/setup.cfg
```

### Comparing `automation_file_dev-0.0.1/LICENSE` & `automation_file_dev-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.1/pyproject.toml` & `automation_file_dev-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_file_dev"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "JE-Chen", email = "zenmailman@gmail.com" },
 ]
 description = ""
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.8"
 license = { text = "MIT" }
```

