# Comparing `tmp/automation_file-0.0.1.tar.gz` & `tmp/automation_file-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_file-0.0.1.tar", last modified: Sun Apr 30 07:14:42 2023, max compression
+gzip compressed data, was "automation_file-0.0.2.tar", last modified: Sat May 27 05:06:51 2023, max compression
```

## Comparing `automation_file-0.0.1.tar` & `automation_file-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 07:14:42.986016 automation_file-0.0.1/
--rw-rw-rw-   0        0        0     1084 2023-04-29 15:33:58.000000 automation_file-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      644 2023-04-30 07:14:42.985019 automation_file-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-04-29 15:33:58.000000 automation_file-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 07:14:42.973055 automation_file-0.0.1/automation_file.egg-info/
--rw-rw-rw-   0        0        0      644 2023-04-30 07:14:42.000000 automation_file-0.0.1/automation_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-04-30 07:14:42.000000 automation_file-0.0.1/automation_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 07:14:42.000000 automation_file-0.0.1/automation_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-30 07:14:42.000000 automation_file-0.0.1/automation_file.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-30 07:14:42.975046 automation_file-0.0.1/file_automation/
--rw-rw-rw-   0        0        0        0 2023-04-29 15:36:35.000000 automation_file-0.0.1/file_automation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:14:42.977041 automation_file-0.0.1/file_automation/excel/
--rw-rw-rw-   0        0        0        0 2023-04-29 17:31:01.000000 automation_file-0.0.1/file_automation/excel/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-29 17:31:16.000000 automation_file-0.0.1/file_automation/excel/openyxl_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:14:42.980032 automation_file-0.0.1/file_automation/pdf/
--rw-rw-rw-   0        0        0        0 2023-04-29 17:32:43.000000 automation_file-0.0.1/file_automation/pdf/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-29 17:32:57.000000 automation_file-0.0.1/file_automation/pdf/pypdf_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:14:42.981032 automation_file-0.0.1/file_automation/utils/
--rw-rw-rw-   0        0        0        0 2023-04-29 16:59:14.000000 automation_file-0.0.1/file_automation/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:14:42.984022 automation_file-0.0.1/file_automation/word/
--rw-rw-rw-   0        0        0        0 2023-04-29 18:01:26.000000 automation_file-0.0.1/file_automation/word/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-29 18:01:40.000000 automation_file-0.0.1/file_automation/word/python_docx_wrapper.py
--rw-rw-rw-   0        0        0      873 2023-04-29 17:53:59.000000 automation_file-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 07:14:42.986016 automation_file-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 05:06:51.824068 automation_file-0.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-04-29 15:33:58.000000 automation_file-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1372 2023-05-27 05:06:51.821561 automation_file-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-05-26 18:14:27.000000 automation_file-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 05:06:51.793652 automation_file-0.0.2/automation_file.egg-info/
+-rw-rw-rw-   0        0        0     1372 2023-05-27 05:06:51.000000 automation_file-0.0.2/automation_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      594 2023-05-27 05:06:51.000000 automation_file-0.0.2/automation_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 05:06:51.000000 automation_file-0.0.2/automation_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-27 05:06:51.000000 automation_file-0.0.2/automation_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 05:06:51.794934 automation_file-0.0.2/file_automation/
+-rw-rw-rw-   0        0        0      712 2023-05-20 05:53:45.000000 automation_file-0.0.2/file_automation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 05:06:51.801429 automation_file-0.0.2/file_automation/dir/
+-rw-rw-rw-   0        0        0        0 2023-05-20 05:53:45.000000 automation_file-0.0.2/file_automation/dir/__init__.py
+-rw-rw-rw-   0        0        0     1230 2023-05-20 05:53:45.000000 automation_file-0.0.2/file_automation/dir/dir_process.py
+drwxrwxrwx   0        0        0        0 2023-05-27 05:06:51.804975 automation_file-0.0.2/file_automation/file/
+-rw-rw-rw-   0        0        0        0 2023-05-20 05:53:45.000000 automation_file-0.0.2/file_automation/file/__init__.py
+-rw-rw-rw-   0        0        0     2205 2023-05-20 05:53:45.000000 automation_file-0.0.2/file_automation/file/file_process.py
+drwxrwxrwx   0        0        0        0 2023-05-27 05:06:51.808966 automation_file-0.0.2/file_automation/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-29 16:59:14.000000 automation_file-0.0.2/file_automation/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 05:06:51.813483 automation_file-0.0.2/file_automation/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-20 05:53:45.000000 automation_file-0.0.2/file_automation/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-20 05:53:45.000000 automation_file-0.0.2/file_automation/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      165 2023-05-20 05:53:45.000000 automation_file-0.0.2/file_automation/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-27 05:06:51.819566 automation_file-0.0.2/file_automation/zip/
+-rw-rw-rw-   0        0        0        0 2023-05-20 05:53:45.000000 automation_file-0.0.2/file_automation/zip/__init__.py
+-rw-rw-rw-   0        0        0     2383 2023-05-20 05:53:45.000000 automation_file-0.0.2/file_automation/zip/zip_process.py
+-rw-rw-rw-   0        0        0      873 2023-05-27 05:06:23.000000 automation_file-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 05:06:51.825071 automation_file-0.0.2/setup.cfg
```

### Comparing `automation_file-0.0.1/LICENSE` & `automation_file-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.1/pyproject.toml` & `automation_file-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_file"
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

