# Comparing `tmp/usellm-0.0.2.tar.gz` & `tmp/usellm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usellm-0.0.2.tar", last modified: Sat May 27 17:59:58 2023, max compression
+gzip compressed data, was "usellm-0.0.3.tar", last modified: Sat May 27 19:44:30 2023, max compression
```

## Comparing `usellm-0.0.2.tar` & `usellm-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-05-27 17:59:58.897798 usellm-0.0.2/
--rw-r--r--   0 jovian     (501) staff       (20)     1063 2023-05-10 15:34:43.000000 usellm-0.0.2/LICENSE
--rw-r--r--   0 jovian     (501) staff       (20)      172 2023-05-27 17:59:58.897676 usellm-0.0.2/PKG-INFO
--rw-r--r--   0 jovian     (501) staff       (20)      591 2023-05-27 17:57:33.000000 usellm-0.0.2/README.md
--rw-r--r--   0 jovian     (501) staff       (20)       38 2023-05-27 17:59:58.897832 usellm-0.0.2/setup.cfg
--rw-r--r--   0 jovian     (501) staff       (20)      296 2023-05-27 17:58:06.000000 usellm-0.0.2/setup.py
-drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-05-27 17:59:58.897116 usellm-0.0.2/usellm/
--rw-r--r--   0 jovian     (501) staff       (20)       90 2023-05-27 17:31:49.000000 usellm-0.0.2/usellm/__init__.py
--rw-r--r--   0 jovian     (501) staff       (20)     2102 2023-05-27 17:58:50.000000 usellm-0.0.2/usellm/use_llm.py
--rw-r--r--   0 jovian     (501) staff       (20)       72 2023-05-27 17:32:05.000000 usellm-0.0.2/usellm/utils.py
-drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-05-27 17:59:58.897532 usellm-0.0.2/usellm.egg-info/
--rw-r--r--   0 jovian     (501) staff       (20)      172 2023-05-27 17:59:58.000000 usellm-0.0.2/usellm.egg-info/PKG-INFO
--rw-r--r--   0 jovian     (501) staff       (20)      199 2023-05-27 17:59:58.000000 usellm-0.0.2/usellm.egg-info/SOURCES.txt
--rw-r--r--   0 jovian     (501) staff       (20)        1 2023-05-27 17:59:58.000000 usellm-0.0.2/usellm.egg-info/dependency_links.txt
--rw-r--r--   0 jovian     (501) staff       (20)        7 2023-05-27 17:59:58.000000 usellm-0.0.2/usellm.egg-info/top_level.txt
+drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-05-27 19:44:30.789788 usellm-0.0.3/
+-rw-r--r--   0 jovian     (501) staff       (20)     1063 2023-05-10 15:34:43.000000 usellm-0.0.3/LICENSE
+-rw-r--r--   0 jovian     (501) staff       (20)      172 2023-05-27 19:44:30.789639 usellm-0.0.3/PKG-INFO
+-rw-r--r--   0 jovian     (501) staff       (20)     3476 2023-05-27 19:44:21.000000 usellm-0.0.3/README.md
+-rw-r--r--   0 jovian     (501) staff       (20)       38 2023-05-27 19:44:30.789826 usellm-0.0.3/setup.cfg
+-rw-r--r--   0 jovian     (501) staff       (20)      282 2023-05-27 19:44:21.000000 usellm-0.0.3/setup.py
+drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-05-27 19:44:30.788654 usellm-0.0.3/usellm/
+-rw-r--r--   0 jovian     (501) staff       (20)       90 2023-05-27 17:31:49.000000 usellm-0.0.3/usellm/__init__.py
+-rw-r--r--   0 jovian     (501) staff       (20)     3628 2023-05-27 19:44:21.000000 usellm-0.0.3/usellm/use_llm.py
+-rw-r--r--   0 jovian     (501) staff       (20)       72 2023-05-27 17:32:05.000000 usellm-0.0.3/usellm/utils.py
+drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-05-27 19:44:30.789487 usellm-0.0.3/usellm.egg-info/
+-rw-r--r--   0 jovian     (501) staff       (20)      172 2023-05-27 19:44:30.000000 usellm-0.0.3/usellm.egg-info/PKG-INFO
+-rw-r--r--   0 jovian     (501) staff       (20)      228 2023-05-27 19:44:30.000000 usellm-0.0.3/usellm.egg-info/SOURCES.txt
+-rw-r--r--   0 jovian     (501) staff       (20)        1 2023-05-27 19:44:30.000000 usellm-0.0.3/usellm.egg-info/dependency_links.txt
+-rw-r--r--   0 jovian     (501) staff       (20)       17 2023-05-27 19:44:30.000000 usellm-0.0.3/usellm.egg-info/requires.txt
+-rw-r--r--   0 jovian     (501) staff       (20)        7 2023-05-27 19:44:30.000000 usellm-0.0.3/usellm.egg-info/top_level.txt
```

### Comparing `usellm-0.0.2/LICENSE` & `usellm-0.0.3/LICENSE`

 * *Files identical despite different names*

