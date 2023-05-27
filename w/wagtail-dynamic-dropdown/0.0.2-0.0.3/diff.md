# Comparing `tmp/wagtail-dynamic-dropdown-0.0.2.tar.gz` & `tmp/wagtail-dynamic-dropdown-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wagtail-dynamic-dropdown-0.0.2.tar", last modified: Wed Aug 17 15:49:35 2022, max compression
+gzip compressed data, was "dist/wagtail-dynamic-dropdown-0.0.3.tar", last modified: Mon Aug 22 16:19:08 2022, max compression
```

## Comparing `wagtail-dynamic-dropdown-0.0.2.tar` & `wagtail-dynamic-dropdown-0.0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/
--rw-r--r--   0 kuba       (501) staff       (20)     3002 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/PKG-INFO
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown.egg-info/
--rwxr-xr-x   0 kuba       (501) staff       (20)     3002 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown.egg-info/PKG-INFO
--rwxr-xr-x   0 kuba       (501) staff       (20)     1166 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown.egg-info/SOURCES.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)       31 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown.egg-info/top_level.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        1 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown.egg-info/dependency_links.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)     1087 2022-04-03 09:11:19.000000 wagtail-dynamic-dropdown-0.0.2/LICENSE
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/tests/
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/tests/testapp/
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/tests/testapp/migrations/
--rwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-04-06 18:24:43.000000 wagtail-dynamic-dropdown-0.0.2/tests/testapp/migrations/__init__.py
--rwxr-xr-x   0 kuba       (501) staff       (20)     1370 2022-04-06 18:24:55.000000 wagtail-dynamic-dropdown-0.0.2/tests/testapp/migrations/0001_initial.py
--rwxr-xr-x   0 kuba       (501) staff       (20)      842 2022-04-08 15:55:27.000000 wagtail-dynamic-dropdown-0.0.2/tests/testapp/models.py
--rwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-04-06 17:29:34.000000 wagtail-dynamic-dropdown-0.0.2/tests/testapp/__init__.py
--rwxr-xr-x   0 kuba       (501) staff       (20)      259 2022-04-08 16:58:14.000000 wagtail-dynamic-dropdown-0.0.2/tests/testapp/dynamic_functions.py
--rwxr-xr-x   0 kuba       (501) staff       (20)     3324 2022-04-08 17:17:33.000000 wagtail-dynamic-dropdown-0.0.2/tests/test_page.py
--rwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-04-06 16:32:27.000000 wagtail-dynamic-dropdown-0.0.2/tests/__init__.py
--rwxr-xr-x   0 kuba       (501) staff       (20)     1194 2022-04-08 15:42:21.000000 wagtail-dynamic-dropdown-0.0.2/tests/test_edit_handlers.py
--rwxr-xr-x   0 kuba       (501) staff       (20)     1651 2022-04-08 15:22:42.000000 wagtail-dynamic-dropdown-0.0.2/tests/test_widget.py
--rwxr-xr-x   0 kuba       (501) staff       (20)     2408 2022-04-08 15:56:04.000000 wagtail-dynamic-dropdown-0.0.2/tests/settings.py
--rwxr-xr-x   0 kuba       (501) staff       (20)      248 2022-04-06 18:04:24.000000 wagtail-dynamic-dropdown-0.0.2/tests/urls.py
--rwxr-xr-x   0 kuba       (501) staff       (20)      145 2022-04-03 11:48:52.000000 wagtail-dynamic-dropdown-0.0.2/MANIFEST.in
--rwxr-xr-x   0 kuba       (501) staff       (20)       39 2022-04-03 11:49:25.000000 wagtail-dynamic-dropdown-0.0.2/setup.py
--rwxr-xr-x   0 kuba       (501) staff       (20)      598 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/setup.cfg
--rwxr-xr-x   0 kuba       (501) staff       (20)     1905 2022-04-09 10:49:33.000000 wagtail-dynamic-dropdown-0.0.2/README.rst
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/migrations/
--rwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-04-02 12:00:15.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/migrations/__init__.py
--rwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-04-02 12:00:15.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/__init__.py
--rwxr-xr-x   0 kuba       (501) staff       (20)      184 2022-04-02 12:00:15.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/apps.py
--rwxr-xr-x   0 kuba       (501) staff       (20)     1718 2022-04-06 18:57:08.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/widgets.py
--rwxr-xr-x   0 kuba       (501) staff       (20)      651 2022-08-17 15:39:24.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/edit_handlers.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/static/
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/static/wagtail_dynamic_dropdown/
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/static/wagtail_dynamic_dropdown/js/
--rwxr-xr-x   0 kuba       (501) staff       (20)     1846 2022-04-02 17:56:16.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/static/wagtail_dynamic_dropdown/js/dynamic_dropdown.js
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/static/wagtail_dynamic_dropdown/styles/
--rwxr-xr-x   0 kuba       (501) staff       (20)     1758 2022-04-02 17:52:53.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/static/wagtail_dynamic_dropdown/styles/dynamic_dropdown.css
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/templates/
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/templates/wagtail_dynamic_dropdown/
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-17 15:49:35.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/templates/wagtail_dynamic_dropdown/widgets/
--rwxr-xr-x   0 kuba       (501) staff       (20)     1001 2022-04-02 17:45:57.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/templates/wagtail_dynamic_dropdown/widgets/dynamic_dropdown.html
--rwxr-xr-x   0 kuba       (501) staff       (20)      348 2022-04-02 17:57:28.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/templates/wagtail_dynamic_dropdown/widgets/dynamic_dropdown_option.html
--rwxr-xr-x   0 kuba       (501) staff       (20)      204 2022-04-02 17:13:46.000000 wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/templates/wagtail_dynamic_dropdown/widgets/dynamic_dropdown_input.html
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/
+-rw-r--r--   0 kuba       (501) staff       (20)     2995 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/PKG-INFO
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown.egg-info/
+-rwxr-xr-x   0 kuba       (501) staff       (20)     2995 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown.egg-info/PKG-INFO
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1166 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)       31 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown.egg-info/top_level.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        1 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1087 2022-04-03 09:11:19.000000 wagtail-dynamic-dropdown-0.0.3/LICENSE
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/tests/
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/tests/testapp/
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/tests/testapp/migrations/
+-rwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-04-06 18:24:43.000000 wagtail-dynamic-dropdown-0.0.3/tests/testapp/migrations/__init__.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1370 2022-04-06 18:24:55.000000 wagtail-dynamic-dropdown-0.0.3/tests/testapp/migrations/0001_initial.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)      842 2022-04-08 15:55:27.000000 wagtail-dynamic-dropdown-0.0.3/tests/testapp/models.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-04-06 17:29:34.000000 wagtail-dynamic-dropdown-0.0.3/tests/testapp/__init__.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)      259 2022-04-08 16:58:14.000000 wagtail-dynamic-dropdown-0.0.3/tests/testapp/dynamic_functions.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)     3324 2022-04-08 17:17:33.000000 wagtail-dynamic-dropdown-0.0.3/tests/test_page.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-04-06 16:32:27.000000 wagtail-dynamic-dropdown-0.0.3/tests/__init__.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1194 2022-04-08 15:42:21.000000 wagtail-dynamic-dropdown-0.0.3/tests/test_edit_handlers.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1651 2022-04-08 15:22:42.000000 wagtail-dynamic-dropdown-0.0.3/tests/test_widget.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)     2408 2022-04-08 15:56:04.000000 wagtail-dynamic-dropdown-0.0.3/tests/settings.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)      248 2022-04-06 18:04:24.000000 wagtail-dynamic-dropdown-0.0.3/tests/urls.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)      145 2022-04-03 11:48:52.000000 wagtail-dynamic-dropdown-0.0.3/MANIFEST.in
+-rwxr-xr-x   0 kuba       (501) staff       (20)       39 2022-04-03 11:49:25.000000 wagtail-dynamic-dropdown-0.0.3/setup.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)      598 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/setup.cfg
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1898 2022-08-17 15:53:32.000000 wagtail-dynamic-dropdown-0.0.3/README.rst
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/migrations/
+-rwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-04-02 12:00:15.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/migrations/__init__.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-04-02 12:00:15.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/__init__.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)      184 2022-04-02 12:00:15.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/apps.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1718 2022-04-06 18:57:08.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/widgets.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1216 2022-08-22 16:16:06.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/edit_handlers.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/static/
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/static/wagtail_dynamic_dropdown/
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/static/wagtail_dynamic_dropdown/js/
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1846 2022-04-02 17:56:16.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/static/wagtail_dynamic_dropdown/js/dynamic_dropdown.js
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/static/wagtail_dynamic_dropdown/styles/
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1758 2022-04-02 17:52:53.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/static/wagtail_dynamic_dropdown/styles/dynamic_dropdown.css
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/templates/
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/templates/wagtail_dynamic_dropdown/
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-08-22 16:19:08.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/templates/wagtail_dynamic_dropdown/widgets/
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1001 2022-04-02 17:45:57.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/templates/wagtail_dynamic_dropdown/widgets/dynamic_dropdown.html
+-rwxr-xr-x   0 kuba       (501) staff       (20)      348 2022-04-02 17:57:28.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/templates/wagtail_dynamic_dropdown/widgets/dynamic_dropdown_option.html
+-rwxr-xr-x   0 kuba       (501) staff       (20)      204 2022-04-02 17:13:46.000000 wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/templates/wagtail_dynamic_dropdown/widgets/dynamic_dropdown_input.html
```

### Comparing `wagtail-dynamic-dropdown-0.0.2/PKG-INFO` & `wagtail-dynamic-dropdown-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-dynamic-dropdown
-Version: 0.0.2
+Version: 0.0.3
 Summary: UNKNOWN
 Home-page: https://github.com/LilJack118/wagtail-dynamic-dropdown
 Author: LilJack118
 Author-email: jakub@kachange.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/LilJack118/wagtail-dynamic-dropdown/issues
 Description: Wagtail Dynamic Dropdown
@@ -15,15 +15,15 @@
         the choices are not migrated to the database.
         
         Install
         -------
         
         ::
         
-           pip install wagtail-dynamic-dropdown==0.0.1
+           pip install wagtail-dynamic-dropdown
         
         Then add ``wagtail_dynamic_dropdown`` to your installed apps:
         
         ::
         
            INSTALLED_APPS = [
                ...
```

### Comparing `wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown.egg-info/PKG-INFO` & `wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-dynamic-dropdown
-Version: 0.0.2
+Version: 0.0.3
 Summary: UNKNOWN
 Home-page: https://github.com/LilJack118/wagtail-dynamic-dropdown
 Author: LilJack118
 Author-email: jakub@kachange.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/LilJack118/wagtail-dynamic-dropdown/issues
 Description: Wagtail Dynamic Dropdown
@@ -15,15 +15,15 @@
         the choices are not migrated to the database.
         
         Install
         -------
         
         ::
         
-           pip install wagtail-dynamic-dropdown==0.0.1
+           pip install wagtail-dynamic-dropdown
         
         Then add ``wagtail_dynamic_dropdown`` to your installed apps:
         
         ::
         
            INSTALLED_APPS = [
                ...
```

### Comparing `wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown.egg-info/SOURCES.txt` & `wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail-dynamic-dropdown-0.0.2/LICENSE` & `wagtail-dynamic-dropdown-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-dynamic-dropdown-0.0.2/tests/testapp/migrations/0001_initial.py` & `wagtail-dynamic-dropdown-0.0.3/tests/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-dynamic-dropdown-0.0.2/tests/testapp/models.py` & `wagtail-dynamic-dropdown-0.0.3/tests/testapp/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-dynamic-dropdown-0.0.2/tests/test_page.py` & `wagtail-dynamic-dropdown-0.0.3/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `wagtail-dynamic-dropdown-0.0.2/tests/test_edit_handlers.py` & `wagtail-dynamic-dropdown-0.0.3/tests/test_edit_handlers.py`

 * *Files identical despite different names*

### Comparing `wagtail-dynamic-dropdown-0.0.2/tests/test_widget.py` & `wagtail-dynamic-dropdown-0.0.3/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `wagtail-dynamic-dropdown-0.0.2/tests/settings.py` & `wagtail-dynamic-dropdown-0.0.3/tests/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-dynamic-dropdown-0.0.2/setup.cfg` & `wagtail-dynamic-dropdown-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-dynamic-dropdown
-version = 0.0.2
+version = 0.0.3
 author = LilJack118
 author_email = jakub@kachange.com
 long_description = file: README.rst
 long_description_content_type = text/markdown
 url = https://github.com/LilJack118/wagtail-dynamic-dropdown
 project_urls = 
 	Bug Tracker = https://github.com/LilJack118/wagtail-dynamic-dropdown/issues
```

### Comparing `wagtail-dynamic-dropdown-0.0.2/README.rst` & `wagtail-dynamic-dropdown-0.0.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 the choices are not migrated to the database.
 
 Install
 -------
 
 ::
 
-   pip install wagtail-dynamic-dropdown==0.0.1
+   pip install wagtail-dynamic-dropdown
 
 Then add ``wagtail_dynamic_dropdown`` to your installed apps:
 
 ::
 
    INSTALLED_APPS = [
        ...
```

### Comparing `wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/widgets.py` & `wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/static/wagtail_dynamic_dropdown/js/dynamic_dropdown.js` & `wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/static/wagtail_dynamic_dropdown/js/dynamic_dropdown.js`

 * *Files identical despite different names*

### Comparing `wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/static/wagtail_dynamic_dropdown/styles/dynamic_dropdown.css` & `wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/static/wagtail_dynamic_dropdown/styles/dynamic_dropdown.css`

 * *Files identical despite different names*

### Comparing `wagtail-dynamic-dropdown-0.0.2/wagtail_dynamic_dropdown/templates/wagtail_dynamic_dropdown/widgets/dynamic_dropdown.html` & `wagtail-dynamic-dropdown-0.0.3/wagtail_dynamic_dropdown/templates/wagtail_dynamic_dropdown/widgets/dynamic_dropdown.html`

 * *Files identical despite different names*

