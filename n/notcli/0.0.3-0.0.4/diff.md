# Comparing `tmp/notcli-0.0.3.tar.gz` & `tmp/notcli-0.0.4.tar.gz`

## Comparing `notcli-0.0.3.tar` & `notcli-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 notcli-0.0.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 notcli-0.0.3/Makefile
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 notcli-0.0.3/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 notcli-0.0.3/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.3/.ruff_cache/content/1d8fcaa1aec41a57
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.3/.ruff_cache/content/33ac437c97c9ba7f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.3/.ruff_cache/content/51d54a3651c5700d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.3/.ruff_cache/content/632db596ee57b83e
--rw-r--r--   0        0        0     7050 2020-02-02 00:00:00.000000 notcli-0.0.3/.ruff_cache/content/742a7a177a653eaf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.3/.ruff_cache/content/a3343eae45f839a8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.3/.ruff_cache/content/a4c0834c4e94528c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.3/.ruff_cache/content/b0da38d3f5b9c71a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.3/.ruff_cache/content/bb1b9bc214883b06
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.3/.ruff_cache/content/d00de8a95d9bf53e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.3/.ruff_cache/content/d25adf9bbda239ae
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.3/.ruff_cache/content/f4b54a9b80a16016
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 notcli-0.0.3/examples/env_file
--rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 notcli-0.0.3/scripts/format.sh
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 notcli-0.0.3/scripts/lint.sh
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 notcli-0.0.3/scripts/test.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 notcli-0.0.3/src/notcli/__init__.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 notcli-0.0.3/src/notcli/app.py
--rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 notcli-0.0.3/src/notcli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notcli-0.0.3/src/notcli/conf/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 notcli-0.0.3/src/notcli/conf/settings.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 notcli-0.0.3/src/notcli/static/demo.css
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 notcli-0.0.3/src/notcli/static/modal.css
--rwxr-xr-x   0        0        0    16504 2020-02-02 00:00:00.000000 notcli-0.0.3/src/tty/ttyecho
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 notcli-0.0.3/tests/test_version.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 notcli-0.0.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 notcli-0.0.3/LICENSE
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 notcli-0.0.3/README.md
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 notcli-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 notcli-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 notcli-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 notcli-0.0.4/Makefile
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 notcli-0.0.4/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 notcli-0.0.4/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.4/.ruff_cache/content/1d8fcaa1aec41a57
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.4/.ruff_cache/content/33ac437c97c9ba7f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.4/.ruff_cache/content/51d54a3651c5700d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.4/.ruff_cache/content/632db596ee57b83e
+-rw-r--r--   0        0        0     7050 2020-02-02 00:00:00.000000 notcli-0.0.4/.ruff_cache/content/742a7a177a653eaf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.4/.ruff_cache/content/a3343eae45f839a8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.4/.ruff_cache/content/a4c0834c4e94528c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.4/.ruff_cache/content/b0da38d3f5b9c71a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.4/.ruff_cache/content/bb1b9bc214883b06
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.4/.ruff_cache/content/d00de8a95d9bf53e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.4/.ruff_cache/content/d25adf9bbda239ae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.4/.ruff_cache/content/f4b54a9b80a16016
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 notcli-0.0.4/examples/env_file
+-rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 notcli-0.0.4/scripts/format.sh
+-rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 notcli-0.0.4/scripts/lint.sh
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 notcli-0.0.4/scripts/test.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 notcli-0.0.4/src/notcli/__init__.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 notcli-0.0.4/src/notcli/app.py
+-rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 notcli-0.0.4/src/notcli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notcli-0.0.4/src/notcli/conf/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 notcli-0.0.4/src/notcli/conf/settings.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 notcli-0.0.4/src/notcli/static/demo.css
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 notcli-0.0.4/src/notcli/static/modal.css
+-rwxr-xr-x   0        0        0    16504 2020-02-02 00:00:00.000000 notcli-0.0.4/src/tty/ttyecho
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 notcli-0.0.4/tests/test_version.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 notcli-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 notcli-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 notcli-0.0.4/README.md
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 notcli-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 notcli-0.0.4/PKG-INFO
```

### Comparing `notcli-0.0.3/CONTRIBUTING.md` & `notcli-0.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `notcli-0.0.3/.ruff_cache/content/742a7a177a653eaf` & `notcli-0.0.4/.ruff_cache/content/742a7a177a653eaf`

 * *Files identical despite different names*

### Comparing `notcli-0.0.3/src/notcli/app.py` & `notcli-0.0.4/src/notcli/app.py`

 * *Files identical despite different names*

### Comparing `notcli-0.0.3/src/notcli/main.py` & `notcli-0.0.4/src/notcli/main.py`

 * *Files identical despite different names*

### Comparing `notcli-0.0.3/src/tty/ttyecho` & `notcli-0.0.4/src/tty/ttyecho`

 * *Files identical despite different names*

### Comparing `notcli-0.0.3/.gitignore` & `notcli-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `notcli-0.0.3/LICENSE` & `notcli-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `notcli-0.0.3/README.md` & `notcli-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,8 +37,9 @@
 ```
 
 This will display a list of commands along with a brief description of what each command does.
 
 | Command    | Description                                                     |
 |------------|-----------------------------------------------------------------|
 | `loadvars` | Loads variables from a file and exports them to the environment |
-| `help`     | Displays a list of available commands and their descriptions    |
+| `help`     | Displays a list of available commands and their descriptions    |
+| `version`  | Displays the version of `notcli`                                |
```

### Comparing `notcli-0.0.3/pyproject.toml` & `notcli-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `notcli-0.0.3/PKG-INFO` & `notcli-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notcli
-Version: 0.0.3
+Version: 0.0.4
 Summary: A CLI application to load variables from a file and export them to the environment, with a Textual-based UI for interactive usage.
 Project-URL: Homepage, https://github.com/godd0t/notcli
 License: MIT License
         
         Copyright (c) 2023 Lirim Shala
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -74,8 +74,9 @@
 ```
 
 This will display a list of commands along with a brief description of what each command does.
 
 | Command    | Description                                                     |
 |------------|-----------------------------------------------------------------|
 | `loadvars` | Loads variables from a file and exports them to the environment |
-| `help`     | Displays a list of available commands and their descriptions    |
+| `help`     | Displays a list of available commands and their descriptions    |
+| `version`  | Displays the version of `notcli`                                |
```

