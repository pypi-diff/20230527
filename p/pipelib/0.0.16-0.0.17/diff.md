# Comparing `tmp/pipelib-0.0.16.tar.gz` & `tmp/pipelib-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipelib-0.0.16.tar", last modified: Sun Mar 19 18:58:24 2023, max compression
+gzip compressed data, was "pipelib-0.0.17.tar", last modified: Sat May 27 04:35:15 2023, max compression
```

## Comparing `pipelib-0.0.16.tar` & `pipelib-0.0.17.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-19 18:58:24.205724 pipelib-0.0.16/
--rw-r--r--   0 runner    (1001) docker     (122)    15830 2023-03-19 18:58:04.000000 pipelib-0.0.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-03-19 18:58:04.000000 pipelib-0.0.16/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-03-19 18:58:24.205724 pipelib-0.0.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2022 2023-03-19 18:58:04.000000 pipelib-0.0.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-19 18:58:24.201724 pipelib-0.0.16/pipelib/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5538 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-19 18:58:24.201724 pipelib-0.0.16/pipelib/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/pipelines/container.py
--rw-r--r--   0 runner    (1001) docker     (122)      430 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/pipelines/git.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-19 18:58:24.201724 pipelib-0.0.16/pipelib/steps/
--rw-r--r--   0 runner    (1001) docker     (122)      474 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-19 18:58:24.201724 pipelib-0.0.16/pipelib/steps/container/
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/steps/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4028 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/steps/container/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-19 18:58:24.201724 pipelib-0.0.16/pipelib/steps/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/steps/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      982 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/steps/filters/git.py
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/steps/filters/numeric.py
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/steps/filters/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-19 18:58:24.201724 pipelib-0.0.16/pipelib/steps/release/
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/steps/release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/steps/release/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-19 18:58:24.201724 pipelib-0.0.16/pipelib/steps/sort/
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/steps/sort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/steps/sort/basic.py
--rw-r--r--   0 runner    (1001) docker     (122)     8164 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/steps/step.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-19 18:58:24.201724 pipelib-0.0.16/pipelib/steps/transform/
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/steps/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/steps/transform/numeric.py
--rw-r--r--   0 runner    (1001) docker     (122)     1702 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/steps/transform/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-19 18:58:24.205724 pipelib-0.0.16/pipelib/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     7119 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/tests/test_steps.py
--rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-19 18:58:24.205724 pipelib-0.0.16/pipelib/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      435 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/utils/docs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/utils/fileio.py
--rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/utils/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     3961 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/utils/terminal.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-19 18:58:24.205724 pipelib-0.0.16/pipelib/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/wrappers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3658 2023-03-19 18:58:04.000000 pipelib-0.0.16/pipelib/wrappers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-19 18:58:24.201724 pipelib-0.0.16/pipelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-03-19 18:58:24.000000 pipelib-0.0.16/pipelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-03-19 18:58:24.000000 pipelib-0.0.16/pipelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-19 18:58:24.000000 pipelib-0.0.16/pipelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-19 18:58:24.000000 pipelib-0.0.16/pipelib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-03-19 18:58:24.000000 pipelib-0.0.16/pipelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-03-19 18:58:24.000000 pipelib-0.0.16/pipelib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-03-19 18:58:04.000000 pipelib-0.0.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-03-19 18:58:24.205724 pipelib-0.0.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3096 2023-03-19 18:58:04.000000 pipelib-0.0.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 04:35:15.817790 pipelib-0.0.17/
+-rw-r--r--   0 runner    (1001) docker     (122)    15830 2023-05-27 04:34:52.000000 pipelib-0.0.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-27 04:34:52.000000 pipelib-0.0.17/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-05-27 04:35:15.817790 pipelib-0.0.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2022 2023-05-27 04:34:52.000000 pipelib-0.0.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 04:35:15.801789 pipelib-0.0.17/pipelib/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5538 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 04:35:15.805789 pipelib-0.0.17/pipelib/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/pipelines/container.py
+-rw-r--r--   0 runner    (1001) docker     (122)      430 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/pipelines/git.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 04:35:15.805789 pipelib-0.0.17/pipelib/steps/
+-rw-r--r--   0 runner    (1001) docker     (122)      474 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 04:35:15.809790 pipelib-0.0.17/pipelib/steps/container/
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/steps/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4028 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/steps/container/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 04:35:15.809790 pipelib-0.0.17/pipelib/steps/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/steps/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      982 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/steps/filters/git.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/steps/filters/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/steps/filters/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 04:35:15.809790 pipelib-0.0.17/pipelib/steps/release/
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/steps/release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/steps/release/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 04:35:15.813790 pipelib-0.0.17/pipelib/steps/sort/
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/steps/sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/steps/sort/basic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8164 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/steps/step.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 04:35:15.813790 pipelib-0.0.17/pipelib/steps/transform/
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/steps/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/steps/transform/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1702 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/steps/transform/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 04:35:15.813790 pipelib-0.0.17/pipelib/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7119 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/tests/test_steps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/tests/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 04:35:15.813790 pipelib-0.0.17/pipelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/utils/docs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/utils/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/utils/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3961 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/utils/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 04:35:15.817790 pipelib-0.0.17/pipelib/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/wrappers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3731 2023-05-27 04:34:52.000000 pipelib-0.0.17/pipelib/wrappers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 04:35:15.805789 pipelib-0.0.17/pipelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-05-27 04:35:15.000000 pipelib-0.0.17/pipelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1259 2023-05-27 04:35:15.000000 pipelib-0.0.17/pipelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-27 04:35:15.000000 pipelib-0.0.17/pipelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-27 04:35:15.000000 pipelib-0.0.17/pipelib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-27 04:35:15.000000 pipelib-0.0.17/pipelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-27 04:35:15.000000 pipelib-0.0.17/pipelib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-27 04:34:52.000000 pipelib-0.0.17/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-05-27 04:35:15.817790 pipelib-0.0.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3096 2023-05-27 04:34:52.000000 pipelib-0.0.17/setup.py
```

### Comparing `pipelib-0.0.16/LICENSE` & `pipelib-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/PKG-INFO` & `pipelib-0.0.17/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipelib
-Version: 0.0.16
+Version: 0.0.17
 Summary: A command line client and functions for collation.
 Home-page: https://github.com/vsoch/pipelib
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: library for collating (filtering,comparing,ordering) things
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pipelib Version: 0.0.16 Summary: A command line
+Metadata-Version: 2.1 Name: pipelib Version: 0.0.17 Summary: A command line
 client and functions for collation. Home-page: https://github.com/vsoch/pipelib
 Author: Vanessa Sochat Author-email: vsoch@users.noreply.github.com Maintainer:
 Vanessa Sochat License: LICENSE Keywords: library for collating
 (filtering,comparing,ordering) things Classifier: Intended Audience :: Science/
 Research Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Mozilla Public License 2.0 (MPL 2.0) Classifier: Programming
 Language :: C Classifier: Programming Language :: Python Classifier: Topic ::
```

### Comparing `pipelib-0.0.16/README.md` & `pipelib-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/pipelib/logger.py` & `pipelib-0.0.17/pipelib/logger.py`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/pipelib/pipeline.py` & `pipelib-0.0.17/pipelib/pipeline.py`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/pipelib/steps/container/tags.py` & `pipelib-0.0.17/pipelib/steps/container/tags.py`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/pipelib/steps/filters/git.py` & `pipelib-0.0.17/pipelib/steps/filters/git.py`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/pipelib/steps/filters/numeric.py` & `pipelib-0.0.17/pipelib/steps/filters/numeric.py`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/pipelib/steps/filters/strings.py` & `pipelib-0.0.17/pipelib/steps/filters/strings.py`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/pipelib/steps/release/tags.py` & `pipelib-0.0.17/pipelib/steps/release/tags.py`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/pipelib/steps/sort/basic.py` & `pipelib-0.0.17/pipelib/steps/sort/basic.py`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/pipelib/steps/step.py` & `pipelib-0.0.17/pipelib/steps/step.py`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/pipelib/steps/transform/strings.py` & `pipelib-0.0.17/pipelib/steps/transform/strings.py`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/pipelib/tests/test_pipelines.py` & `pipelib-0.0.17/pipelib/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/pipelib/tests/test_steps.py` & `pipelib-0.0.17/pipelib/tests/test_steps.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 # with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 import pytest
 
 import pipelib.utils
 from pipelib.steps import iter_steps
+from pipelib.steps.release.tags import MajorTagSort
 
 
 @pytest.mark.parametrize("step_type,step_name,step_module", list(iter_steps()))
 def test_step(tmp_path, step_type, step_name, step_module):
     """
     Test step basic functionality
     """
@@ -21,7 +22,22 @@
     docs = pipelib.utils.get_docstring(step_module)
 
     has_code = False
     for line in docs:
         if ">>>" in line:
             has_code = True
     assert has_code
+
+
+def test_release_tags() -> None:
+    """
+    Tests for MajorTagSort
+    """
+    items = ["v3", "v1", "v2-beta", "v2"]
+
+    step = MajorTagSort(ascending=True)
+    filtered = step.run(items)
+    assert [str(x) for x in filtered] == ["v1", "v2-beta", "v3"]
+
+    step = MajorTagSort(ascending=False)
+    filtered = step.run(items)
+    assert [str(x) for x in filtered] == ["v3", "v2-beta", "v1"]
```

### Comparing `pipelib-0.0.16/pipelib/tests/test_utils.py` & `pipelib-0.0.17/pipelib/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/pipelib/utils/fileio.py` & `pipelib-0.0.17/pipelib/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/pipelib/utils/inspect.py` & `pipelib-0.0.17/pipelib/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/pipelib/utils/terminal.py` & `pipelib-0.0.17/pipelib/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/pipelib/version.py` & `pipelib-0.0.17/pipelib/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Vanessa Sochat"
 __copyright__ = "Copyright 2022, Vanessa Sochat"
 __license__ = "MPL 2.0"
 
-__version__ = "0.0.16"
+__version__ = "0.0.17"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "pipelib"
 PACKAGE_URL = "https://github.com/vsoch/pipelib"
 KEYWORDS = "library for collating (filtering, comparing, ordering) things"
 DESCRIPTION = "A command line client and functions for collation."
 LICENSE = "LICENSE"
```

### Comparing `pipelib-0.0.16/pipelib/wrappers/base.py` & `pipelib-0.0.17/pipelib/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `pipelib-0.0.16/pipelib/wrappers/version.py` & `pipelib-0.0.17/pipelib/wrappers/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,17 @@
         if len(components) >= 2:
             self._major_minor = components[0:2]
         if len(components) >= 3:
             self._major_minor_patch = components[0:3]
         self.version = components
         print(f"Setting version to {self.version}")
 
+    def __hash__(self) -> int:
+        return hash(tuple(self.version))
+
     def __lt__(self, other) -> bool:
         return self.version < other.version
 
     def __le__(self, other) -> bool:
         return self.version <= other.version
 
     def __eq__(self, other) -> bool:
```

### Comparing `pipelib-0.0.16/pipelib.egg-info/PKG-INFO` & `pipelib-0.0.17/pipelib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipelib
-Version: 0.0.16
+Version: 0.0.17
 Summary: A command line client and functions for collation.
 Home-page: https://github.com/vsoch/pipelib
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: library for collating (filtering,comparing,ordering) things
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pipelib Version: 0.0.16 Summary: A command line
+Metadata-Version: 2.1 Name: pipelib Version: 0.0.17 Summary: A command line
 client and functions for collation. Home-page: https://github.com/vsoch/pipelib
 Author: Vanessa Sochat Author-email: vsoch@users.noreply.github.com Maintainer:
 Vanessa Sochat License: LICENSE Keywords: library for collating
 (filtering,comparing,ordering) things Classifier: Intended Audience :: Science/
 Research Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Mozilla Public License 2.0 (MPL 2.0) Classifier: Programming
 Language :: C Classifier: Programming Language :: Python Classifier: Topic ::
```

### Comparing `pipelib-0.0.16/pipelib.egg-info/SOURCES.txt` & `pipelib-0.0.17/pipelib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 pipelib/steps/transform/numeric.py
 pipelib/steps/transform/strings.py
 pipelib/tests/__init__.py
 pipelib/tests/helpers.py
 pipelib/tests/test_pipelines.py
 pipelib/tests/test_steps.py
 pipelib/tests/test_utils.py
+pipelib/tests/test_wrappers.py
 pipelib/utils/__init__.py
 pipelib/utils/docs.py
 pipelib/utils/fileio.py
 pipelib/utils/inspect.py
 pipelib/utils/terminal.py
 pipelib/wrappers/__init__.py
 pipelib/wrappers/base.py
```

### Comparing `pipelib-0.0.16/setup.py` & `pipelib-0.0.17/setup.py`

 * *Files identical despite different names*

