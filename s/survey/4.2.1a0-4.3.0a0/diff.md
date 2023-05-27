# Comparing `tmp/survey-4.2.1a0.tar.gz` & `tmp/survey-4.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survey-4.2.1a0.tar", last modified: Sat May 27 08:56:09 2023, max compression
+gzip compressed data, was "survey-4.3.0a0.tar", last modified: Sat May 27 18:34:08 2023, max compression
```

## Comparing `survey-4.2.1a0.tar` & `survey-4.3.0a0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:56:09.578457 survey-4.2.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-27 08:55:59.000000 survey-4.2.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-27 08:56:09.578457 survey-4.2.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-27 08:55:59.000000 survey-4.2.1a0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 08:56:09.578457 survey-4.2.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-27 08:55:59.000000 survey-4.2.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:56:09.578457 survey-4.2.1a0/survey/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_controls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:56:09.578457 survey-4.2.1a0/survey/_core/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_core/_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_core/_console.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_core/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_core/_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_core/_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_core/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_core/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_core/_io_os.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_core/_io_os_nt.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_core/_io_os_posix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_core/_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_core/_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_core/_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_funnels.py
--rw-r--r--   0 runner    (1001) docker     (123)    13214 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_mutates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_printers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_searches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_visuals.py
--rw-r--r--   0 runner    (1001) docker     (123)    58488 2023-05-27 08:55:59.000000 survey-4.2.1a0/survey/_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:56:09.578457 survey-4.2.1a0/survey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-27 08:56:09.000000 survey-4.2.1a0/survey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-27 08:56:09.000000 survey-4.2.1a0/survey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 08:56:09.000000 survey-4.2.1a0/survey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-27 08:56:09.000000 survey-4.2.1a0/survey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 08:56:09.000000 survey-4.2.1a0/survey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:08.941357 survey-4.3.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-27 18:33:59.000000 survey-4.3.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-27 18:34:08.941357 survey-4.3.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-27 18:33:59.000000 survey-4.3.0a0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 18:34:08.941357 survey-4.3.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-27 18:33:59.000000 survey-4.3.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:08.937356 survey-4.3.0a0/survey/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_controls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:08.941357 survey-4.3.0a0/survey/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_io_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_io_os_nt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_io_os_posix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_funnels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13214 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_mutates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_printers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_visuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59354 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:08.937356 survey-4.3.0a0/survey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-27 18:34:08.000000 survey-4.3.0a0/survey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-27 18:34:08.000000 survey-4.3.0a0/survey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 18:34:08.000000 survey-4.3.0a0/survey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-27 18:34:08.000000 survey-4.3.0a0/survey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 18:34:08.000000 survey-4.3.0a0/survey.egg-info/top_level.txt
```

### Comparing `survey-4.2.1a0/LICENSE` & `survey-4.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/PKG-INFO` & `survey-4.3.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 4.2.1a0
+Version: 4.3.0a0
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
 Requires-Python: >=3.11
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `survey-4.2.1a0/README.rst` & `survey-4.3.0a0/README.rst`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/setup.py` & `survey-4.3.0a0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.rst') as file:
     readme = file.read()
 
 author = 'Exahilosys'
 project = 'survey'
-version = '4.2.1-alpha'
+version = '4.3.0-alpha'
 
 url = 'https://github.com/{0}/{1}'.format(author, project)
 
 setuptools.setup(
     name = project,
     python_requires = '>=3.11',
     version = version,
```

### Comparing `survey-4.2.1a0/survey/__init__.py` & `survey-4.3.0a0/survey/__init__.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_colors.py` & `survey-4.3.0a0/survey/_colors.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_controls.py` & `survey-4.3.0a0/survey/_controls.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_core/__init__.py` & `survey-4.3.0a0/survey/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_core/_ansi.py` & `survey-4.3.0a0/survey/_core/_ansi.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_core/_console.py` & `survey-4.3.0a0/survey/_core/_console.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_core/_cursor.py` & `survey-4.3.0a0/survey/_core/_cursor.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_core/_handle.py` & `survey-4.3.0a0/survey/_core/_handle.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_core/_helpers.py` & `survey-4.3.0a0/survey/_core/_helpers.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_core/_io.py` & `survey-4.3.0a0/survey/_core/_io.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_core/_io_os.py` & `survey-4.3.0a0/survey/_core/_io_os.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_core/_io_os_nt.py` & `survey-4.3.0a0/survey/_core/_io_os_nt.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_core/_io_os_posix.py` & `survey-4.3.0a0/survey/_core/_io_os_posix.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_core/_render.py` & `survey-4.3.0a0/survey/_core/_render.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_core/_screen.py` & `survey-4.3.0a0/survey/_core/_screen.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_core/_source.py` & `survey-4.3.0a0/survey/_core/_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,17 @@
     def _read(self):
 
         if self._buffer:
             return
         
         text = self._io.recv()
 
+        if text == '\x1b':
+            return
+
         self._buffer.extend(text)
         
     def _get(self):
 
         self._read()
 
         try:
```

### Comparing `survey-4.2.1a0/survey/_funnels.py` & `survey-4.3.0a0/survey/_funnels.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_graphics.py` & `survey-4.3.0a0/survey/_graphics.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_handle.py` & `survey-4.3.0a0/survey/_handle.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_helpers.py` & `survey-4.3.0a0/survey/_helpers.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_mutates.py` & `survey-4.3.0a0/survey/_mutates.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_printers.py` & `survey-4.3.0a0/survey/_printers.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_routines.py` & `survey-4.3.0a0/survey/_routines.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_searches.py` & `survey-4.3.0a0/survey/_searches.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_stage.py` & `survey-4.3.0a0/survey/_stage.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_theme.py` & `survey-4.3.0a0/survey/_theme.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_utils.py` & `survey-4.3.0a0/survey/_utils.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_visuals.py` & `survey-4.3.0a0/survey/_visuals.py`

 * *Files identical despite different names*

### Comparing `survey-4.2.1a0/survey/_widgets.py` & `survey-4.3.0a0/survey/_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,29 +27,39 @@
 
 __all__ = ('WidgetError', 'Widget', 'start', 
            'BaseText', 'Input', 'Numeric', 'Conceal', 'AutoSubmit', 'Inquire', 
            'BaseMesh', 'BaseList', 'Select', 'Basket', 'Count', 'DateTime',
            'Form')
 
 
-class WidgetError(_helpers.InfoErrorMixin, Exception):
+class Abort(_helpers.InfoErrorMixin, Exception):
+
+    """
+    Raised when an invokation needs to stop. May include a message.
+    """
 
     __slots__ = ()
 
 
-class Abort(WidgetError):
+
+class Escape(Exception):
+
+    """
+    Raised when the users pressed the ``Esc`` button.
+    """
 
     __slots__ = ()
 
 
-_type_Widget_init_mutate  : typing.TypeAlias = _mutates.Mutate
-_type_Widget_init_visual  : typing.TypeAlias = _visuals.Visual
-_type_Widget_init_callback: typing.TypeAlias = _handle._type_Handle_init_callback
-_type_Widget_init_delegate: typing.TypeAlias = typing.Callable[[_core.Event], bool]
-_type_Widget_init_validate: typing.TypeAlias = typing.Callable[[typing.Any], None]
+_type_Widget_init_mutate   : typing.TypeAlias = _mutates.Mutate
+_type_Widget_init_visual   : typing.TypeAlias = _visuals.Visual
+_type_Widget_init_callback : typing.TypeAlias = _handle._type_Handle_init_callback
+_type_Widget_init_delegate : typing.TypeAlias = typing.Callable[[_core.Event], bool]
+_type_Widget_init_validate : typing.TypeAlias = typing.Callable[[typing.Any], None]
+_type_Widget_init_escapable: typing.TypeAlias = bool
 
 _type_Widget_invoke_event: typing.TypeAlias = _core.Event
 _type_Widget_invoke_info : typing.TypeAlias = _core._type_ansi_parse_return
 
 
 class Widget:
 
@@ -66,30 +76,31 @@
         Used with ``(event)`` and decides whether to continue the invokation.
     :param validate:
         Used with ``(result)`` upon submission, forbidden by raising :exc:`.Abort`.
     """
 
     _mark_result_c = object()
 
-    __slots__ = ('_mutate', '_handle', '_visual', '_delegate', '_validate', '_result_c')
+    __slots__ = ('_mutate', '_handle', '_visual', '_delegate', '_validate', '_escapable', '_result_c')
 
     def __init_subclass__(cls, controls = (), **kwargs):
 
         pre_controls = getattr(cls, '_controls', ())
         
         cls._controls = (*pre_controls, *controls)
 
         super().__init_subclass__(**kwargs)
 
     def __init__(self, 
-                 mutate  : _type_Widget_init_mutate, 
-                 visual  : _type_Widget_init_visual, 
-                 callback: _type_Widget_init_callback = None, 
-                 delegate: _type_Widget_init_delegate = None,
-                 validate: _type_Widget_init_validate = None):
+                 mutate   : _type_Widget_init_mutate, 
+                 visual   : _type_Widget_init_visual, 
+                 callback : _type_Widget_init_callback  = None, 
+                 delegate : _type_Widget_init_delegate  = None,
+                 validate : _type_Widget_init_validate  = None,
+                 escapable: _type_Widget_init_escapable = False):
         
         self._delegate = delegate
         self._validate = validate
         self._result_c = self._mark_result_c
 
         self._mutate = mutate
 
@@ -97,14 +108,16 @@
 
         for control in self._controls:
             handle.add(control)
 
         self._handle = handle
         self._visual = visual
 
+        self._escapable = escapable
+
     @property
     def mutate(self):
 
         """
         The underlying mutate.
         """
 
@@ -160,14 +173,17 @@
             Contains details used during the operation.
 
         .. note::
 
             If :paramref:`.delegate` is provided and returns :code:`False`, nothing happens.
         """
 
+        if self._escapable and event == _core.Event.escape:
+            raise Escape()
+
         self._invoke(event, info)
     
     def _sketch(self, *args, **kwargs):
 
         return self._visual.get(*args, **kwargs)
     
     def sketch(self, 
@@ -390,14 +406,15 @@
 
 _type_BaseText_init_lines       : typing.TypeAlias = _mutates._type_Text_init_lines 
 _type_BaseText_init_point       : typing.TypeAlias = _mutates._type_Text_init_point
 _type_BaseText_init_multi       : typing.TypeAlias = bool
 _type_BaseText_init_callback    : typing.TypeAlias = _type_Widget_init_callback
 _type_BaseText_init_delegate    : typing.TypeAlias = _type_Widget_init_delegate
 _type_BaseText_init_validate    : typing.TypeAlias = _type_Widget_init_validate
+_type_BaseText_init_escapable   : typing.TypeAlias = _type_Widget_init_escapable
 _type_BaseText_init_funnel_enter: typing.TypeAlias = _visuals._type_Text_init_funnel_enter
 _type_BaseText_init_funnel_leave: typing.TypeAlias = _visuals._type_Text_init_funnel_leave
 
 
 _BaseText_controls = (
     _controls.text_insert,
     _controls.text_move_left,
@@ -438,14 +455,15 @@
     def __init__(self, 
                  lines       : _type_BaseText_init_lines, 
                  point       : _type_BaseText_init_point,
                  multi       : _type_BaseText_init_multi        = False,
                  callback    : _type_BaseText_init_callback     = None,
                  delegate    : _type_BaseText_init_delegate     = None,
                  validate    : _type_BaseText_init_validate     = None,
+                 escapable   : _type_BaseText_init_escapable    = False,
                  funnel_enter: _type_BaseText_init_funnel_enter = None, 
                  funnel_leave: _type_BaseText_init_funnel_leave = None):
 
         mutate = _mutates.Text(lines, point)
 
         def visual_get(*args):
             return (mutate.lines, mutate.point)
@@ -463,15 +481,16 @@
         callback = _helpers.chain_functions(callback, handle.invoke)
 
         super().__init__(
             mutate, 
             visual,
             callback = callback,
             delegate = delegate,
-            validate = validate
+            validate = validate,
+            escapable = escapable
         )
 
 
 _type_Input_init_value: typing.TypeAlias = str
 _type_Input_init_index: typing.TypeAlias = int
 
 
@@ -850,14 +869,15 @@
 _type_BaseMesh_init_clean       : typing.TypeAlias = _mutates._type_Mesh_init_clean
 _type_BaseMesh_init_scout       : typing.TypeAlias = _mutates._type_Mesh_init_scout
 _type_BaseMesh_init_rigid       : typing.TypeAlias = _mutates._type_Mesh_init_rigid
 _type_BaseMesh_init_focus       : typing.TypeAlias = bool | typing.Callable[[_core.Event], bool] 
 _type_BaseMesh_init_callback    : typing.TypeAlias = _type_Widget_init_callback
 _type_BaseMesh_init_delegate    : typing.TypeAlias = _type_Widget_init_delegate
 _type_BaseMesh_init_validate    : typing.TypeAlias = _type_Widget_init_validate
+_type_BaseMesh_init_escapable   : typing.TypeAlias = _type_Widget_init_escapable
 _type_BaseMesh_init_funnel_enter: typing.TypeAlias = _visuals._type_Mesh_init_funnel_enter
 _type_BaseMesh_init_funnel_leave: typing.TypeAlias = _visuals._type_Mesh_init_funnel_leave
 
 
 _BaseMesh_controls = (
     _controls.mesh_move_left,
     _controls.mesh_move_right,
@@ -893,14 +913,16 @@
         When :class:`~typing.Callable`, it is used on each invokation to determine whether to delegate it to the currently pointed-at tile instead.
     :param callback:
         Same as :paramref:`.Widget.callback`.
     :param delegate:
         Same as :paramref:`.Widget.delegate`.
     :param validate:
         Same as :paramref:`.Widget.validate`.
+    :param escapable:
+        Same as :paramref:`.Widget.escapable`.
     :param funnel_enter:
         Same as :paramref:`.visuals.Mesh.funnel_enter`.
     :param funnel_leave:
         Same as :paramref:`.visuals.Mesh.funnel_leave`.
     """
 
     __slots__ = ('_focus',)
@@ -913,14 +935,15 @@
                  clean       : _type_BaseMesh_init_clean        = False,
                  scout       : _type_BaseMesh_init_scout        = None, 
                  rigid       : _type_BaseMesh_init_rigid        = False,
                  focus       : _type_BaseMesh_init_focus        = False,
                  callback    : _type_BaseMesh_init_callback     = None,
                  delegate    : _type_BaseMesh_init_delegate     = None,
                  validate    : _type_BaseMesh_init_validate     = None,
+                 escapable   : _type_BaseMesh_init_escapable    = True,
                  funnel_enter: _type_BaseMesh_init_funnel_enter = None, 
                  funnel_leave: _type_BaseMesh_init_funnel_leave = None):
         
         if tiles is _helpers.auto:
             tiles = ()
 
         tiles = dict(tiles)
@@ -949,14 +972,15 @@
         visual = _visuals.Mesh(visual_get, funnel_enter, funnel_leave)
 
         self._focus = focus
 
         super().__init__(
             mutate, 
             visual,
+            escapable = escapable,
             validate = validate,
             delegate = delegate,
             callback = callback
         )
 
     @property
     def focus(self):
```

### Comparing `survey-4.2.1a0/survey.egg-info/PKG-INFO` & `survey-4.3.0a0/survey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 4.2.1a0
+Version: 4.3.0a0
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
 Requires-Python: >=3.11
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `survey-4.2.1a0/survey.egg-info/SOURCES.txt` & `survey-4.3.0a0/survey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

