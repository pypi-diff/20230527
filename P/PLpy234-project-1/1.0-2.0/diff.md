# Comparing `tmp/PLpy234 project 1-1.0.tar.gz` & `tmp/PLpy234 project 1-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PLpy234 project 1-1.0.tar", last modified: Thu May 25 12:43:34 2023, max compression
+gzip compressed data, was "PLpy234 project 1-2.0.tar", last modified: Sat May 27 15:36:38 2023, max compression
```

## Comparing `PLpy234 project 1-1.0.tar` & `PLpy234 project 1-2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 12:43:34.097673 PLpy234 project 1-1.0/
--rw-rw-rw-   0        0        0    35821 2023-05-24 14:53:16.000000 PLpy234 project 1-1.0/LICENSE
--rw-rw-rw-   0        0        0      125 2023-05-25 12:43:34.086707 PLpy234 project 1-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-25 12:43:34.057431 PLpy234 project 1-1.0/PLpy234_project_1.egg-info/
--rw-rw-rw-   0        0        0      125 2023-05-25 12:43:33.000000 PLpy234 project 1-1.0/PLpy234_project_1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-05-25 12:43:33.000000 PLpy234 project 1-1.0/PLpy234_project_1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 12:43:33.000000 PLpy234 project 1-1.0/PLpy234_project_1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 12:43:33.000000 PLpy234 project 1-1.0/PLpy234_project_1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       36 2023-05-24 14:42:39.000000 PLpy234 project 1-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 12:43:34.083745 PLpy234 project 1-1.0/moshpdf/
--rw-rw-rw-   0        0        0        0 2023-05-24 13:46:35.000000 PLpy234 project 1-1.0/moshpdf/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-24 13:51:28.000000 PLpy234 project 1-1.0/moshpdf/pdf2img.py
--rw-rw-rw-   0        0        0       42 2023-05-24 13:49:28.000000 PLpy234 project 1-1.0/moshpdf/pdf2txt.py
--rw-rw-rw-   0        0        0       42 2023-05-25 12:43:34.097673 PLpy234 project 1-1.0/setup.cfg
--rw-rw-rw-   0        0        0      237 2023-05-24 15:06:18.000000 PLpy234 project 1-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 15:36:38.311712 PLpy234 project 1-2.0/
+-rw-rw-rw-   0        0        0    35821 2023-05-24 14:53:16.000000 PLpy234 project 1-2.0/LICENSE
+-rw-rw-rw-   0        0        0      125 2023-05-27 15:36:38.310724 PLpy234 project 1-2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-27 15:36:38.285360 PLpy234 project 1-2.0/PLpy234_project_1.egg-info/
+-rw-rw-rw-   0        0        0      125 2023-05-27 15:36:38.000000 PLpy234 project 1-2.0/PLpy234_project_1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-05-27 15:36:38.000000 PLpy234 project 1-2.0/PLpy234_project_1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 15:36:38.000000 PLpy234 project 1-2.0/PLpy234_project_1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-27 15:36:38.000000 PLpy234 project 1-2.0/PLpy234_project_1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       38 2023-05-26 14:25:19.000000 PLpy234 project 1-2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 15:36:38.307753 PLpy234 project 1-2.0/moshpdf/
+-rw-rw-rw-   0        0        0        0 2023-05-24 13:46:35.000000 PLpy234 project 1-2.0/moshpdf/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 13:51:28.000000 PLpy234 project 1-2.0/moshpdf/pdf2img.py
+-rw-rw-rw-   0        0        0      283 2023-05-27 15:05:15.000000 PLpy234 project 1-2.0/moshpdf/pdf2txt.py
+-rw-rw-rw-   0        0        0       42 2023-05-27 15:36:38.311712 PLpy234 project 1-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      237 2023-05-27 15:36:22.000000 PLpy234 project 1-2.0/setup.py
```

### Comparing `PLpy234 project 1-1.0/LICENSE` & `PLpy234 project 1-2.0/LICENSE`

 * *Files identical despite different names*

