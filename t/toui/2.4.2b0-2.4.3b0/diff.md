# Comparing `tmp/toui-2.4.2b0.tar.gz` & `tmp/toui-2.4.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-2.4.2b0.tar", last modified: Fri May 26 03:55:20 2023, max compression
+gzip compressed data, was "toui-2.4.3b0.tar", last modified: Sat May 27 06:01:49 2023, max compression
```

## Comparing `toui-2.4.2b0.tar` & `toui-2.4.3b0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 03:55:20.516293 toui-2.4.2b0/
--rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-2.4.2b0/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-2.4.2b0/MANIFEST.in
--rw-rw-rw-   0        0        0     3235 2023-05-26 03:55:20.515293 toui-2.4.2b0/PKG-INFO
--rw-rw-rw-   0        0        0     2860 2023-05-24 15:31:01.000000 toui-2.4.2b0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 03:55:20.258611 toui-2.4.2b0/examples/
--rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2023-05-26 03:55:20.263611 toui-2.4.2b0/images/
--rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-2.4.2b0/images/logo.png
--rw-rw-rw-   0        0        0       42 2023-05-26 03:55:20.516293 toui-2.4.2b0/setup.cfg
--rw-rw-rw-   0        0        0     1657 2023-05-23 17:57:05.000000 toui-2.4.2b0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 03:55:20.494293 toui-2.4.2b0/toui/
--rw-rw-rw-   0        0        0      271 2023-05-26 03:32:16.000000 toui-2.4.2b0/toui/__init__.py
--rw-rw-rw-   0        0        0      431 2023-05-23 15:00:55.000000 toui-2.4.2b0/toui/_defaults.py
--rw-rw-rw-   0        0        0     1406 2023-05-26 03:32:16.000000 toui-2.4.2b0/toui/_helpers.py
--rw-rw-rw-   0        0        0    10863 2023-05-26 03:45:07.000000 toui-2.4.2b0/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     8637 2023-05-26 03:42:45.000000 toui-2.4.2b0/toui/_signals.py
--rw-rw-rw-   0        0        0    31491 2023-05-26 03:32:16.000000 toui-2.4.2b0/toui/apps.py
--rw-rw-rw-   0        0        0    22886 2023-05-24 15:46:55.000000 toui-2.4.2b0/toui/elements.py
--rw-rw-rw-   0        0        0      316 2023-05-15 13:04:45.000000 toui-2.4.2b0/toui/exceptions.py
--rw-rw-rw-   0        0        0    18047 2023-05-23 16:30:18.000000 toui-2.4.2b0/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-2.4.2b0/toui/structure.py
-drwxrwxrwx   0        0        0        0 2023-05-26 03:55:20.513292 toui-2.4.2b0/toui.egg-info/
--rw-rw-rw-   0        0        0     3235 2023-05-26 03:55:19.000000 toui-2.4.2b0/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-05-26 03:55:20.000000 toui-2.4.2b0/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 03:55:19.000000 toui-2.4.2b0/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-05-26 03:55:19.000000 toui-2.4.2b0/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-26 03:55:19.000000 toui-2.4.2b0/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 06:01:49.444718 toui-2.4.3b0/
+-rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-2.4.3b0/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-2.4.3b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3296 2023-05-27 06:01:49.444718 toui-2.4.3b0/PKG-INFO
+-rw-rw-rw-   0        0        0     2921 2023-05-26 03:58:02.000000 toui-2.4.3b0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 06:01:49.123546 toui-2.4.3b0/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2023-05-27 06:01:49.170696 toui-2.4.3b0/images/
+-rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-2.4.3b0/images/logo.png
+-rw-rw-rw-   0        0        0       42 2023-05-27 06:01:49.452885 toui-2.4.3b0/setup.cfg
+-rw-rw-rw-   0        0        0     1657 2023-05-23 17:57:05.000000 toui-2.4.3b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 06:01:49.437279 toui-2.4.3b0/toui/
+-rw-rw-rw-   0        0        0      271 2023-05-27 05:58:40.000000 toui-2.4.3b0/toui/__init__.py
+-rw-rw-rw-   0        0        0      431 2023-05-23 15:00:55.000000 toui-2.4.3b0/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1406 2023-05-26 03:32:16.000000 toui-2.4.3b0/toui/_helpers.py
+-rw-rw-rw-   0        0        0    10863 2023-05-26 03:45:07.000000 toui-2.4.3b0/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     8637 2023-05-26 03:42:45.000000 toui-2.4.3b0/toui/_signals.py
+-rw-rw-rw-   0        0        0    31569 2023-05-27 04:41:53.000000 toui-2.4.3b0/toui/apps.py
+-rw-rw-rw-   0        0        0    22886 2023-05-24 15:46:55.000000 toui-2.4.3b0/toui/elements.py
+-rw-rw-rw-   0        0        0      316 2023-05-15 13:04:45.000000 toui-2.4.3b0/toui/exceptions.py
+-rw-rw-rw-   0        0        0    18047 2023-05-23 16:30:18.000000 toui-2.4.3b0/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-2.4.3b0/toui/structure.py
+drwxrwxrwx   0        0        0        0 2023-05-27 06:01:49.444718 toui-2.4.3b0/toui.egg-info/
+-rw-rw-rw-   0        0        0     3296 2023-05-27 06:01:48.000000 toui-2.4.3b0/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-05-27 06:01:48.000000 toui-2.4.3b0/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 06:01:48.000000 toui-2.4.3b0/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2023-05-27 06:01:48.000000 toui-2.4.3b0/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-27 06:01:48.000000 toui-2.4.3b0/toui.egg-info/top_level.txt
```

### Comparing `toui-2.4.2b0/LICENSE` & `toui-2.4.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-2.4.2b0/PKG-INFO` & `toui-2.4.3b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 2.4.2b0
+Version: 2.4.3b0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![ToUI Image](images/logo.png)
+![ToUI Image](https://github.com/mubarakalmehairbi/ToUI/blob/main/images/logo.png?raw=True)
 
 ![License](https://img.shields.io/github/license/mubarakalmehairbi/ToUI)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/toui)
 ![Latest version](https://img.shields.io/pypi/v/toui)
 ![Docs](https://img.shields.io/readthedocs/toui)
 
 # Overview
```

### Comparing `toui-2.4.2b0/README.md` & `toui-2.4.3b0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![ToUI Image](images/logo.png)
+![ToUI Image](https://github.com/mubarakalmehairbi/ToUI/blob/main/images/logo.png?raw=True)
 
 ![License](https://img.shields.io/github/license/mubarakalmehairbi/ToUI)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/toui)
 ![Latest version](https://img.shields.io/pypi/v/toui)
 ![Docs](https://img.shields.io/readthedocs/toui)
 
 # Overview
```

### Comparing `toui-2.4.2b0/examples/advanced_example_1_toui_blueprint.py` & `toui-2.4.3b0/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.2b0/examples/example_1_simple_website.py` & `toui-2.4.3b0/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.2b0/examples/example_2_simple_desktop_app.py` & `toui-2.4.3b0/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.2b0/examples/example_3_updating_page.py` & `toui-2.4.3b0/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.2b0/examples/example_4_function_with_arg.py` & `toui-2.4.3b0/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.2b0/examples/example_5_user_variables.py` & `toui-2.4.3b0/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.2b0/images/logo.png` & `toui-2.4.3b0/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-2.4.2b0/setup.py` & `toui-2.4.3b0/setup.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.2b0/toui/_helpers.py` & `toui-2.4.3b0/toui/_helpers.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.2b0/toui/_javascript_templates.py` & `toui-2.4.3b0/toui/_javascript_templates.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.2b0/toui/_signals.py` & `toui-2.4.3b0/toui/_signals.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.2b0/toui/apps.py` & `toui-2.4.3b0/toui/apps.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,14 +581,15 @@
         flask.Blueprint
 
         """
         self.add_pages(*blueprint.pages, blueprint=blueprint)
         self.flask_app.register_blueprint(blueprint=blueprint, **options)
 
     def _add_communication_method(self):
+        self.flask_app.config['SOCK_SERVER_OPTIONS'] = {'ping_interval': 25}
         self._socket = Sock(self.flask_app)
         self._socket.route("/toui-communicate")(self._communicate)
 
     def _add_user_vars(self):
         self.flask_app.config["CACHE_TYPE"] = "SimpleCache"
         self._cache = Cache(self.flask_app)
         self._user_vars = _UserVars(self._cache)
```

### Comparing `toui-2.4.2b0/toui/elements.py` & `toui-2.4.3b0/toui/elements.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.2b0/toui/pages.py` & `toui-2.4.3b0/toui/pages.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.2b0/toui/structure.py` & `toui-2.4.3b0/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.2b0/toui.egg-info/PKG-INFO` & `toui-2.4.3b0/toui.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 2.4.2b0
+Version: 2.4.3b0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![ToUI Image](images/logo.png)
+![ToUI Image](https://github.com/mubarakalmehairbi/ToUI/blob/main/images/logo.png?raw=True)
 
 ![License](https://img.shields.io/github/license/mubarakalmehairbi/ToUI)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/toui)
 ![Latest version](https://img.shields.io/pypi/v/toui)
 ![Docs](https://img.shields.io/readthedocs/toui)
 
 # Overview
```

### Comparing `toui-2.4.2b0/toui.egg-info/SOURCES.txt` & `toui-2.4.3b0/toui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

