# Comparing `tmp/coolapi-0.0.1.tar.gz` & `tmp/coolapi-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolapi-0.0.1.tar", last modified: Thu May 25 18:08:51 2023, max compression
+gzip compressed data, was "coolapi-1.0.tar", last modified: Sat May 27 11:54:59 2023, max compression
```

## Comparing `coolapi-0.0.1.tar` & `coolapi-1.0.tar`

### file list

```diff
@@ -1,4 +1,7 @@
--rw-r--r--   0        0        0    10943 2023-04-25 13:18:06.439303 coolapi-0.0.1/LICENSE
--rw-r--r--   0        0        0      124 2023-05-25 18:08:47.098665 coolapi-0.0.1/coolapi.py
--rw-r--r--   0        0        0      314 2023-05-25 18:08:47.098665 coolapi-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      162 1970-01-01 00:00:00.000000 coolapi-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 coolapi-1.0/LICENSE
+-rw-r--r--   0        0        0     5292 2023-05-27 11:40:02.442076 coolapi-1.0/README.md
+-rw-r--r--   0        0        0    11358 2023-05-14 02:53:10.000000 coolapi-1.0/coolapi/Licenses of dependent packages/tornado/LICENSE
+-rw-r--r--   0        0        0       43 2023-05-26 07:00:38.945694 coolapi-1.0/coolapi/__init__.py
+-rw-r--r--   0        0        0     1668 2023-05-27 11:00:33.037396 coolapi-1.0/coolapi/_coolapi.py
+-rw-r--r--   0        0        0      611 2023-05-27 11:28:03.719778 coolapi-1.0/pyproject.toml
+-rw-r--r--   0        0        0     5557 1970-01-01 00:00:00.000000 coolapi-1.0/PKG-INFO
```

### Comparing `coolapi-0.0.1/LICENSE` & `coolapi-1.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
    
 
-   Copyright [2023] [x]
+   Copyright [2023] [许灿标]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

