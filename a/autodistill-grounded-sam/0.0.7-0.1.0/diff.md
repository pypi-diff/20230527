# Comparing `tmp/autodistill_grounded_sam-0.0.7.tar.gz` & `tmp/autodistill_grounded_sam-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill_grounded_sam-0.0.7.tar", last modified: Thu May 25 17:56:31 2023, max compression
+gzip compressed data, was "dist/autodistill_grounded_sam-0.1.0.tar", last modified: Sat May 27 02:59:42 2023, max compression
```

## Comparing `autodistill_grounded_sam-0.0.7.tar` & `autodistill_grounded_sam-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yeldarb    (501) staff       (20)        0 2023-05-25 17:56:31.517629 autodistill_grounded_sam-0.0.7/
--rw-r--r--   0 yeldarb    (501) staff       (20)      599 2023-05-25 17:56:31.517483 autodistill_grounded_sam-0.0.7/PKG-INFO
--rw-r--r--   0 yeldarb    (501) staff       (20)     3157 2023-05-24 22:17:32.000000 autodistill_grounded_sam-0.0.7/README.md
-drwxr-xr-x   0 yeldarb    (501) staff       (20)        0 2023-05-25 17:56:31.516106 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam/
--rw-r--r--   0 yeldarb    (501) staff       (20)       85 2023-05-25 16:48:41.000000 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam/__init__.py
--rw-r--r--   0 yeldarb    (501) staff       (20)     3522 2023-05-25 17:25:31.000000 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam/grounded_sam.py
--rw-r--r--   0 yeldarb    (501) staff       (20)     7893 2023-05-25 17:25:31.000000 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam/helpers.py
-drwxr-xr-x   0 yeldarb    (501) staff       (20)        0 2023-05-25 17:56:31.516987 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam.egg-info/
--rw-r--r--   0 yeldarb    (501) staff       (20)      599 2023-05-25 17:56:31.000000 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam.egg-info/PKG-INFO
--rw-r--r--   0 yeldarb    (501) staff       (20)      390 2023-05-25 17:56:31.000000 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam.egg-info/SOURCES.txt
--rw-r--r--   0 yeldarb    (501) staff       (20)        1 2023-05-25 17:56:31.000000 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam.egg-info/dependency_links.txt
--rw-r--r--   0 yeldarb    (501) staff       (20)      134 2023-05-25 17:56:31.000000 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam.egg-info/requires.txt
--rw-r--r--   0 yeldarb    (501) staff       (20)       25 2023-05-25 17:56:31.000000 autodistill_grounded_sam-0.0.7/autodistill_grounded_sam.egg-info/top_level.txt
--rw-r--r--   0 yeldarb    (501) staff       (20)       38 2023-05-25 17:56:31.517671 autodistill_grounded_sam-0.0.7/setup.cfg
--rw-r--r--   0 yeldarb    (501) staff       (20)     1592 2023-05-25 17:25:31.000000 autodistill_grounded_sam-0.0.7/setup.py
-drwxr-xr-x   0 yeldarb    (501) staff       (20)        0 2023-05-25 17:56:31.517132 autodistill_grounded_sam-0.0.7/test/
--rw-r--r--   0 yeldarb    (501) staff       (20)       41 2023-05-24 22:17:32.000000 autodistill_grounded_sam-0.0.7/test/test_hello.py
+drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      599 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/PKG-INFO
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     3157 2023-05-27 02:55:23.000000 autodistill_grounded_sam-0.1.0/README.md
+drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam/
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       85 2023-05-27 02:59:06.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam/__init__.py
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     2352 2023-05-27 02:55:23.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam/grounded_sam.py
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     4642 2023-05-27 02:55:23.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam/helpers.py
+drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam.egg-info/
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      599 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam.egg-info/PKG-INFO
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      390 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)        1 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      155 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam.egg-info/requires.txt
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       25 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam.egg-info/top_level.txt
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       38 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/setup.cfg
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     1592 2023-05-27 02:55:23.000000 autodistill_grounded_sam-0.1.0/setup.py
+drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/test/
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       41 2023-05-27 02:55:23.000000 autodistill_grounded_sam-0.1.0/test/test_hello.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `autodistill_grounded_sam-0.0.7/PKG-INFO` & `autodistill_grounded_sam-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill_grounded_sam
-Version: 0.0.7
+Version: 0.1.0
 Summary: Automatically distill large foundational models into smaller, in-domain models for deployment
 Home-page: https://github.com/autodistill/autodistill
 Author: Roboflow
 Author-email: jacob@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `autodistill_grounded_sam-0.0.7/README.md` & `autodistill_grounded_sam-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `autodistill_grounded_sam-0.0.7/autodistill_grounded_sam.egg-info/PKG-INFO` & `autodistill_grounded_sam-0.1.0/autodistill_grounded_sam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill-grounded-sam
-Version: 0.0.7
+Version: 0.1.0
 Summary: Automatically distill large foundational models into smaller, in-domain models for deployment
 Home-page: https://github.com/autodistill/autodistill
 Author: Roboflow
 Author-email: jacob@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `autodistill_grounded_sam-0.0.7/setup.py` & `autodistill_grounded_sam-0.1.0/setup.py`

 * *Files identical despite different names*

