# Comparing `tmp/memos_cli-0.1.0.tar.gz` & `tmp/memos_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memos_cli-0.1.0.tar", max compression
+gzip compressed data, was "memos_cli-0.1.1.tar", max compression
```

## Comparing `memos_cli-0.1.0.tar` & `memos_cli-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-05-19 19:07:11.029905 memos_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0      853 2023-05-21 19:09:31.582203 memos_cli-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-19 12:17:53.228120 memos_cli-0.1.0/client/__init__.py
--rw-r--r--   0        0        0      887 2023-05-21 18:34:31.316236 memos_cli-0.1.0/client/auth.py
--rw-r--r--   0        0        0       71 2023-05-19 15:38:36.486995 memos_cli-0.1.0/client/memo.py
--rw-r--r--   0        0        0     1030 2023-05-19 20:10:56.719183 memos_cli-0.1.0/client/model.py
--rw-r--r--   0        0        0      325 2023-05-21 18:31:29.545239 memos_cli-0.1.0/client/session.py
--rw-r--r--   0        0        0        0 2023-05-19 16:59:20.185347 memos_cli-0.1.0/common/__init__.py
--rw-r--r--   0        0        0      692 2023-05-21 18:44:48.689226 memos_cli-0.1.0/common/config.py
--rw-r--r--   0        0        0       88 2023-05-21 19:04:02.726208 memos_cli-0.1.0/memos/__init__.py
--rw-r--r--   0        0        0      366 2023-05-19 15:17:48.856905 memos_cli-0.1.0/memos/auth/__init__.py
--rw-r--r--   0        0        0      430 2023-05-21 18:27:43.251242 memos_cli-0.1.0/memos/auth/signin.py
--rw-r--r--   0        0        0      270 2023-05-19 17:23:20.388452 memos_cli-0.1.0/memos/auth/signout.py
--rw-r--r--   0        0        0      307 2023-05-19 16:57:02.020337 memos_cli-0.1.0/memos/auth/whoami.py
--rw-r--r--   0        0        0      751 2023-05-21 19:05:15.534207 memos_cli-0.1.0/memos/cli.py
--rw-r--r--   0        0        0      333 2023-05-19 20:11:53.951187 memos_cli-0.1.0/memos/echo.py
--rw-r--r--   0        0        0      998 2023-05-21 19:03:05.816209 memos_cli-0.1.0/memos/edit.py
--rw-r--r--   0        0        0     1003 2023-05-21 19:02:59.288209 memos_cli-0.1.0/memos/list.py
--rw-r--r--   0        0        0      781 2023-05-21 19:02:54.983209 memos_cli-0.1.0/memos/new.py
--rw-r--r--   0        0        0      347 2023-05-21 19:02:49.501210 memos_cli-0.1.0/memos/remove.py
--rw-r--r--   0        0        0      596 2023-05-19 19:06:33.746902 memos_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 memos_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-19 19:07:11.029905 memos_cli-0.1.1/LICENSE
+-rw-r--r--   0        0        0      853 2023-05-21 19:09:31.582203 memos_cli-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 12:17:53.228120 memos_cli-0.1.1/client/__init__.py
+-rw-r--r--   0        0        0      887 2023-05-21 18:34:31.316236 memos_cli-0.1.1/client/auth.py
+-rw-r--r--   0        0        0       71 2023-05-19 15:38:36.486995 memos_cli-0.1.1/client/memo.py
+-rw-r--r--   0        0        0     1030 2023-05-19 20:10:56.719183 memos_cli-0.1.1/client/model.py
+-rw-r--r--   0        0        0      325 2023-05-21 18:31:29.545239 memos_cli-0.1.1/client/session.py
+-rw-r--r--   0        0        0        0 2023-05-19 16:59:20.185347 memos_cli-0.1.1/common/__init__.py
+-rw-r--r--   0        0        0      692 2023-05-21 18:44:48.689226 memos_cli-0.1.1/common/config.py
+-rw-r--r--   0        0        0       88 2023-05-21 19:04:02.726208 memos_cli-0.1.1/memos/__init__.py
+-rw-r--r--   0        0        0      366 2023-05-19 15:17:48.856905 memos_cli-0.1.1/memos/auth/__init__.py
+-rw-r--r--   0        0        0      430 2023-05-21 18:27:43.251242 memos_cli-0.1.1/memos/auth/signin.py
+-rw-r--r--   0        0        0      270 2023-05-19 17:23:20.388452 memos_cli-0.1.1/memos/auth/signout.py
+-rw-r--r--   0        0        0      307 2023-05-19 16:57:02.020337 memos_cli-0.1.1/memos/auth/whoami.py
+-rw-r--r--   0        0        0      806 2023-05-27 12:05:20.159987 memos_cli-0.1.1/memos/cli.py
+-rw-r--r--   0        0        0     3302 2023-05-27 12:04:32.504988 memos_cli-0.1.1/memos/click_aliases.py
+-rw-r--r--   0        0        0      333 2023-05-19 20:11:53.951187 memos_cli-0.1.1/memos/echo.py
+-rw-r--r--   0        0        0      998 2023-05-21 19:03:05.816209 memos_cli-0.1.1/memos/edit.py
+-rw-r--r--   0        0        0     1003 2023-05-21 19:02:59.288209 memos_cli-0.1.1/memos/list.py
+-rw-r--r--   0        0        0      781 2023-05-21 19:02:54.983209 memos_cli-0.1.1/memos/new.py
+-rw-r--r--   0        0        0      347 2023-05-21 19:02:49.501210 memos_cli-0.1.1/memos/remove.py
+-rw-r--r--   0        0        0      571 2023-05-27 12:06:23.384986 memos_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1318 1970-01-01 00:00:00.000000 memos_cli-0.1.1/PKG-INFO
```

### Comparing `memos_cli-0.1.0/LICENSE` & `memos_cli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `memos_cli-0.1.0/README.md` & `memos_cli-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `memos_cli-0.1.0/client/auth.py` & `memos_cli-0.1.1/client/auth.py`

 * *Files identical despite different names*

### Comparing `memos_cli-0.1.0/client/model.py` & `memos_cli-0.1.1/client/model.py`

 * *Files identical despite different names*

### Comparing `memos_cli-0.1.0/common/config.py` & `memos_cli-0.1.1/common/config.py`

 * *Files identical despite different names*

### Comparing `memos_cli-0.1.0/memos/cli.py` & `memos_cli-0.1.1/memos/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import click
-from click_aliases import ClickAliasedGroup
 from memos import __VERSION__
+from memos.click_aliases import ClickAliasedGroup
 from memos.auth import auth_command
 from memos.echo import echo_command
 from memos.edit import edit_command
 from memos.list import list_command
 from memos.new import new_command
 from memos.remove import remove_command
 
@@ -18,14 +18,14 @@
     """Prints Memos CLI version"""
     click.echo(f'Memos CLI v{__VERSION__}')
 
 
 cli.add_command(auth_command)
 cli.add_command(echo_command)
 cli.add_command(edit_command)
-cli.add_command(list_command)
+cli.add_command(list_command, aliases=['ls'])
 cli.add_command(new_command)
-cli.add_command(remove_command)
+cli.add_command(remove_command, aliases=['rm', 'delete', 'del'])
 cli.add_command(version_command)
 
 if __name__ == '__main__':
     cli()
```

### Comparing `memos_cli-0.1.0/memos/edit.py` & `memos_cli-0.1.1/memos/edit.py`

 * *Files identical despite different names*

### Comparing `memos_cli-0.1.0/memos/list.py` & `memos_cli-0.1.1/memos/list.py`

 * *Files identical despite different names*

### Comparing `memos_cli-0.1.0/memos/new.py` & `memos_cli-0.1.1/memos/new.py`

 * *Files identical despite different names*

### Comparing `memos_cli-0.1.0/PKG-INFO` & `memos_cli-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: memos-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: A CLI frontend for memos self-hosted memo hub
 Author: Giulio De Matteis
 Author-email: hello@giuliodematte.is
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: click-aliases (>=1.0.1,<2.0.0)
 Requires-Dist: prettytable (>=3.7.0,<4.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Memos CLI
 
 *To use this cli, you must have a self-hosted [✍️memos](https://github.com/usememos/memos) server set up and running.*
```

