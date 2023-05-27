# Comparing `tmp/mkdocs-enumerate-headings-plugin-0.6.0.tar.gz` & `tmp/mkdocs-enumerate-headings-plugin-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-enumerate-headings-plugin-0.6.0.tar", last modified: Mon Feb 20 09:21:42 2023, max compression
+gzip compressed data, was "mkdocs-enumerate-headings-plugin-0.6.1.tar", last modified: Sat May 27 08:40:08 2023, max compression
```

## Comparing `mkdocs-enumerate-headings-plugin-0.6.0.tar` & `mkdocs-enumerate-headings-plugin-0.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 09:21:42.910022 mkdocs-enumerate-headings-plugin-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-02-20 09:21:16.000000 mkdocs-enumerate-headings-plugin-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-02-20 09:21:42.910022 mkdocs-enumerate-headings-plugin-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-02-20 09:21:16.000000 mkdocs-enumerate-headings-plugin-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 09:21:42.906022 mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 09:21:16.000000 mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-02-20 09:21:16.000000 mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin/exclude.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-02-20 09:21:16.000000 mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin/heading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-02-20 09:21:16.000000 mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin/html_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-02-20 09:21:16.000000 mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 09:21:42.906022 mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-02-20 09:21:42.000000 mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-02-20 09:21:42.000000 mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 09:21:42.000000 mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-20 09:21:42.000000 mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 09:21:42.000000 mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-20 09:21:42.000000 mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 09:21:42.910022 mkdocs-enumerate-headings-plugin-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-02-20 09:21:16.000000 mkdocs-enumerate-headings-plugin-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 09:21:42.910022 mkdocs-enumerate-headings-plugin-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 09:21:16.000000 mkdocs-enumerate-headings-plugin-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-02-20 09:21:16.000000 mkdocs-enumerate-headings-plugin-0.6.0/tests/test_builds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-02-20 09:21:16.000000 mkdocs-enumerate-headings-plugin-0.6.0/tests/test_heading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-02-20 09:21:16.000000 mkdocs-enumerate-headings-plugin-0.6.0/tests/test_html_page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:40:08.170551 mkdocs-enumerate-headings-plugin-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-05-27 08:40:08.170551 mkdocs-enumerate-headings-plugin-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:40:08.166551 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/exclude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/heading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/html_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:40:08.170551 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-05-27 08:40:08.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-27 08:40:08.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 08:40:08.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-27 08:40:08.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 08:40:08.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-27 08:40:08.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 08:40:08.170551 mkdocs-enumerate-headings-plugin-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:40:08.170551 mkdocs-enumerate-headings-plugin-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/tests/test_builds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/tests/test_heading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/tests/test_html_page.py
```

### Comparing `mkdocs-enumerate-headings-plugin-0.6.0/LICENSE` & `mkdocs-enumerate-headings-plugin-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-enumerate-headings-plugin-0.6.0/PKG-INFO` & `mkdocs-enumerate-headings-plugin-0.6.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-enumerate-headings-plugin
-Version: 0.6.0
+Version: 0.6.1
 Summary: MkDocs Plugin to enumerate the headings (h1-h6) across site pages
 Home-page: https://github.com/timvink/mkdocs-enumerate-headings-plugin.git
 Author: timvink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs enumerate headings plugin
 Classifier: Intended Audience :: Developers
@@ -94,24 +94,27 @@
 
 ```yml
 plugins:
     - enumerate-headings:
         toc_depth: 0
         strict: true
         increment_across_pages: true
+        include:
+          - "*"
         exclude:
           - index.md
           - another_page.md
         restart_increment_after:
           - second_section.md
 ```
 
 - **`toc_depth`** (default `0`): Up to which level the table of contents should be enumerated as well. Default is 0, which means the TOC is not enumerated at all. Max is 6 (showing all enumeration)
 - **`strict`** (default `true`): Raise errors instead of warnings when first heading on a page is not a level one heading (single `#`) and your MkDocs theme has not inserted the page title as a heading 1 for you. Note that in `strict: false` mode the heading numbers might be incorrect between pages and before and after a level 1 heading.
 - **`increment_across_pages`** (default `true`): Increment the chapter number for each new page (in the order they appear in the navigation). If disabled, each page will start from 1.
+- **`include`** (default *`["*"]`*): Specify a list of page source paths (one per line) that should have enumeration (included in processing by this plugin). This can be useful for example to include enumeration on only one directory. The source path of a page is relative to your `docs/` folder. You can also use [globs](https://docs.python.org/3/library/glob.html) instead of source paths. For example, to include `docs/subfolder/page.md` specify in your `mkdocs.yml` a line under `include:` with `- subfolder/page.md`
 - **`exclude`** (default *not specified*): Specify a list of page source paths (one per line) that should not have enumeration (excluded from processing by this plugin). This can be useful for example to remove enumeration from the front page. The source path of a page is relative to your `docs/` folder. You can also use [globs](https://docs.python.org/3/library/glob.html) instead of source paths. For example, to exclude `docs/subfolder/page.md` specify in your `mkdocs.yml` a line under `exclude:` with `- subfolder/page.md`
 - **`restart_increment_after`** (default *not specified*): Specify a list of page source paths (one per line) where enumeration should be restarted. This can be useful if you have multiple reports or tutorials in one mkdocs site. Paths behave as with `exclude` (can use globs).
 
 ## Contributing
 
 Contributions are very welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) before putting in any work.
```

### Comparing `mkdocs-enumerate-headings-plugin-0.6.0/README.md` & `mkdocs-enumerate-headings-plugin-0.6.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -72,24 +72,27 @@
 
 ```yml
 plugins:
     - enumerate-headings:
         toc_depth: 0
         strict: true
         increment_across_pages: true
+        include:
+          - "*"
         exclude:
           - index.md
           - another_page.md
         restart_increment_after:
           - second_section.md
 ```
 
 - **`toc_depth`** (default `0`): Up to which level the table of contents should be enumerated as well. Default is 0, which means the TOC is not enumerated at all. Max is 6 (showing all enumeration)
 - **`strict`** (default `true`): Raise errors instead of warnings when first heading on a page is not a level one heading (single `#`) and your MkDocs theme has not inserted the page title as a heading 1 for you. Note that in `strict: false` mode the heading numbers might be incorrect between pages and before and after a level 1 heading.
 - **`increment_across_pages`** (default `true`): Increment the chapter number for each new page (in the order they appear in the navigation). If disabled, each page will start from 1.
+- **`include`** (default *`["*"]`*): Specify a list of page source paths (one per line) that should have enumeration (included in processing by this plugin). This can be useful for example to include enumeration on only one directory. The source path of a page is relative to your `docs/` folder. You can also use [globs](https://docs.python.org/3/library/glob.html) instead of source paths. For example, to include `docs/subfolder/page.md` specify in your `mkdocs.yml` a line under `include:` with `- subfolder/page.md`
 - **`exclude`** (default *not specified*): Specify a list of page source paths (one per line) that should not have enumeration (excluded from processing by this plugin). This can be useful for example to remove enumeration from the front page. The source path of a page is relative to your `docs/` folder. You can also use [globs](https://docs.python.org/3/library/glob.html) instead of source paths. For example, to exclude `docs/subfolder/page.md` specify in your `mkdocs.yml` a line under `exclude:` with `- subfolder/page.md`
 - **`restart_increment_after`** (default *not specified*): Specify a list of page source paths (one per line) where enumeration should be restarted. This can be useful if you have multiple reports or tutorials in one mkdocs site. Paths behave as with `exclude` (can use globs).
 
 ## Contributing
 
 Contributions are very welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) before putting in any work.
```

### Comparing `mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin/exclude.py` & `mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/exclude.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,41 +3,63 @@
 Inspired by https://github.com/apenwarr/mkdocs-exclude
 """
 import os
 import fnmatch
 from typing import List
 
 
+def include(src_path: str, globs: List[str]) -> bool:
+    """
+    Determine if a src_path should be included.
+    Supports globs (e.g. folder/* or *.md).
+
+    Args:
+        src_path (src): Path of file
+        globs (list): list of globs of file paths to include
+    Returns:
+        (bool): whether src_path should be excluded
+    """
+    return matches_nix_path(src_path, globs)
+
+
 def exclude(src_path: str, globs: List[str]) -> bool:
     """
     Determine if a src_path should be excluded.
+
+    Args:
+        src_path (src): Path of file
+        globs (list): list of globs of file paths to include
+    Returns:
+        (bool): whether src_path should be excluded
+    """
+    return matches_nix_path(src_path, globs)
+
+
+def matches_nix_path(src_path: str, globs: List[str]) -> bool:
+    """
+    Determines if a src_path matches one of the provided glob patterns.
     Supports globs (e.g. folder/* or *.md).
     Credits: code inspired by / adapted from
     https://github.com/apenwarr/mkdocs-exclude/blob/master/mkdocs_exclude/plugin.py
+
     Args:
         src_path (src): Path of file
-        globs (list): list of globs
+        globs (list): list of globs of file paths to include
     Returns:
         (bool): whether src_path should be excluded
     """
+
     assert isinstance(src_path, str)
     assert isinstance(globs, list)
 
-    for g in globs:
-        if fnmatch.fnmatchcase(src_path, g):
-            return True
-
-        # Windows reports filenames as eg.  a\\b\\c instead of a/b/c.
-        # To make the same globs/regexes match filenames on Windows and
-        # other OSes, let's try matching against converted filenames.
-        # On the other hand, Unix actually allows filenames to contain
-        # literal \\ characters (although it is rare), so we won't
-        # always convert them.  We only convert if os.sep reports
-        # something unusual.  Conversely, some future mkdocs might
-        # report Windows filenames using / separators regardless of
-        # os.sep, so we *always* test with / above.
-        if os.sep != "/":
-            src_path_fix = src_path.replace(os.sep, "/")
-            if fnmatch.fnmatchcase(src_path_fix, g):
-                return True
+    # Windows reports filenames as eg.  a\\b\\c instead of a/b/c.
+    # To make the same globs/regexes match filenames on Windows and
+    # other OSes, let's try matching against converted filenames.
+    # On the other hand, Unix actually allows filenames to contain
+    # literal \\ characters (although it is rare), so we won't
+    # always convert them.  We only convert if os.sep reports
+    # something unusual.  Conversely, some future mkdocs might
+    # report Windows filenames using / separators regardless of
+    # os.sep, so we *always* test with / above.
+    fixed_path = src_path.replace(os.sep, "/")
 
-    return False
+    return any(fnmatch.fnmatch(fixed_path, glob) for glob in globs)
```

### Comparing `mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin/heading.py` & `mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/heading.py`

 * *Files identical despite different names*

### Comparing `mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin/html_page.py` & `mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/html_page.py`

 * *Files identical despite different names*

### Comparing `mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin/plugin.py` & `mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 import logging
 
 from collections import OrderedDict
 from mkdocs.config import config_options
 from mkdocs.plugins import BasePlugin
 from mkdocs.exceptions import ConfigurationError
 from mkdocs_enumerate_headings_plugin.html_page import HTMLPage
-from mkdocs_enumerate_headings_plugin.exclude import exclude
+from mkdocs_enumerate_headings_plugin.exclude import exclude, include
 from bs4 import BeautifulSoup
 
 logger = logging.getLogger("mkdocs.plugins")
 
 
 class EnumerateHeadingsPlugin(BasePlugin):
     config_scheme = (
         ("strict", config_options.Type(bool, default=True)),
         ("toc_depth", config_options.Type(int, default=0)),
         ("increment_across_pages", config_options.Type(bool, default=True)),
         ("restart_increment_after", config_options.Type(list, default=[])),
+        ("include", config_options.Type(list, default=["*"])),
         ("exclude", config_options.Type(list, default=[])),
     )
 
     def on_pre_build(self, config, **kwargs):
         """Validates plugin user configuration input
 
         Args:
@@ -91,18 +92,21 @@
             files: global files collection
         
         """
         chapter_counter = 0
         markdown_files_processed = {}
 
         for page in nav.pages:
-
+            # Include pages specified in config
+            included_pages = self.config.get("include", ["*"])
             # Exclude pages specified in config
             excluded_pages = self.config.get("exclude", [])
-            if exclude(page.file.src_path, excluded_pages):
+            if not include(page.file.src_path, included_pages) or exclude(
+                page.file.src_path, excluded_pages
+            ):
                 continue
 
             # We need to build the pages in order to find out
             # if there are more than one heading 1's in the page
             page.read_source(config)
             page.render(config, files)
             soup = BeautifulSoup(page.content, "html.parser")
```

### Comparing `mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin.egg-info/PKG-INFO` & `mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-enumerate-headings-plugin
-Version: 0.6.0
+Version: 0.6.1
 Summary: MkDocs Plugin to enumerate the headings (h1-h6) across site pages
 Home-page: https://github.com/timvink/mkdocs-enumerate-headings-plugin.git
 Author: timvink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs enumerate headings plugin
 Classifier: Intended Audience :: Developers
@@ -94,24 +94,27 @@
 
 ```yml
 plugins:
     - enumerate-headings:
         toc_depth: 0
         strict: true
         increment_across_pages: true
+        include:
+          - "*"
         exclude:
           - index.md
           - another_page.md
         restart_increment_after:
           - second_section.md
 ```
 
 - **`toc_depth`** (default `0`): Up to which level the table of contents should be enumerated as well. Default is 0, which means the TOC is not enumerated at all. Max is 6 (showing all enumeration)
 - **`strict`** (default `true`): Raise errors instead of warnings when first heading on a page is not a level one heading (single `#`) and your MkDocs theme has not inserted the page title as a heading 1 for you. Note that in `strict: false` mode the heading numbers might be incorrect between pages and before and after a level 1 heading.
 - **`increment_across_pages`** (default `true`): Increment the chapter number for each new page (in the order they appear in the navigation). If disabled, each page will start from 1.
+- **`include`** (default *`["*"]`*): Specify a list of page source paths (one per line) that should have enumeration (included in processing by this plugin). This can be useful for example to include enumeration on only one directory. The source path of a page is relative to your `docs/` folder. You can also use [globs](https://docs.python.org/3/library/glob.html) instead of source paths. For example, to include `docs/subfolder/page.md` specify in your `mkdocs.yml` a line under `include:` with `- subfolder/page.md`
 - **`exclude`** (default *not specified*): Specify a list of page source paths (one per line) that should not have enumeration (excluded from processing by this plugin). This can be useful for example to remove enumeration from the front page. The source path of a page is relative to your `docs/` folder. You can also use [globs](https://docs.python.org/3/library/glob.html) instead of source paths. For example, to exclude `docs/subfolder/page.md` specify in your `mkdocs.yml` a line under `exclude:` with `- subfolder/page.md`
 - **`restart_increment_after`** (default *not specified*): Specify a list of page source paths (one per line) where enumeration should be restarted. This can be useful if you have multiple reports or tutorials in one mkdocs site. Paths behave as with `exclude` (can use globs).
 
 ## Contributing
 
 Contributions are very welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) before putting in any work.
```

### Comparing `mkdocs-enumerate-headings-plugin-0.6.0/mkdocs_enumerate_headings_plugin.egg-info/SOURCES.txt` & `mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-enumerate-headings-plugin-0.6.0/setup.py` & `mkdocs-enumerate-headings-plugin-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mkdocs-enumerate-headings-plugin",
-    version="0.6.0",
+    version="0.6.1",
     description="MkDocs Plugin to enumerate the headings (h1-h6) across site pages",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs enumerate headings plugin",
     url="https://github.com/timvink/mkdocs-enumerate-headings-plugin.git",
     author="timvink",
     author_email="vinktim@gmail.com",
```

### Comparing `mkdocs-enumerate-headings-plugin-0.6.0/tests/test_builds.py` & `mkdocs-enumerate-headings-plugin-0.6.1/tests/test_builds.py`

 * *Files identical despite different names*

### Comparing `mkdocs-enumerate-headings-plugin-0.6.0/tests/test_heading.py` & `mkdocs-enumerate-headings-plugin-0.6.1/tests/test_heading.py`

 * *Files identical despite different names*

### Comparing `mkdocs-enumerate-headings-plugin-0.6.0/tests/test_html_page.py` & `mkdocs-enumerate-headings-plugin-0.6.1/tests/test_html_page.py`

 * *Files identical despite different names*

