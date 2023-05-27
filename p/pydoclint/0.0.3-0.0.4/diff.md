# Comparing `tmp/pydoclint-0.0.3.tar.gz` & `tmp/pydoclint-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoclint-0.0.3.tar", last modified: Fri May 19 06:24:32 2023, max compression
+gzip compressed data, was "pydoclint-0.0.4.tar", last modified: Sat May 27 10:28:49 2023, max compression
```

## Comparing `pydoclint-0.0.3.tar` & `pydoclint-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:24:32.877374 pydoclint-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-19 06:24:18.000000 pydoclint-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-05-19 06:24:32.877374 pydoclint-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-05-19 06:24:18.000000 pydoclint-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:24:32.873373 pydoclint-0.0.3/pydoclint/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/flake8_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:24:32.877374 pydoclint-0.0.3/pydoclint/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/astTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/internal_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/method_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/return_yield_raise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/violation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/walk.py
--rw-r--r--   0 runner    (1001) docker     (123)    12357 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:24:32.873373 pydoclint-0.0.3/pydoclint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-05-19 06:24:32.000000 pydoclint-0.0.3/pydoclint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-19 06:24:32.000000 pydoclint-0.0.3/pydoclint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:24:32.000000 pydoclint-0.0.3/pydoclint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-19 06:24:32.000000 pydoclint-0.0.3/pydoclint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-19 06:24:32.000000 pydoclint-0.0.3/pydoclint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 06:24:32.000000 pydoclint-0.0.3/pydoclint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-19 06:24:32.877374 pydoclint-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-19 06:24:18.000000 pydoclint-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:24:32.877374 pydoclint-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21080 2023-05-19 06:24:18.000000 pydoclint-0.0.3/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:28:49.309871 pydoclint-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-27 10:28:34.000000 pydoclint-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-05-27 10:28:49.309871 pydoclint-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-05-27 10:28:34.000000 pydoclint-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:28:49.301870 pydoclint-0.0.4/pydoclint/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/flake8_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:28:49.305871 pydoclint-0.0.4/pydoclint/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/astTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/internal_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/method_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/return_yield_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/unparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/violation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:28:49.305871 pydoclint-0.0.4/pydoclint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-05-27 10:28:49.000000 pydoclint-0.0.4/pydoclint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-27 10:28:49.000000 pydoclint-0.0.4/pydoclint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 10:28:49.000000 pydoclint-0.0.4/pydoclint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-27 10:28:49.000000 pydoclint-0.0.4/pydoclint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-27 10:28:49.000000 pydoclint-0.0.4/pydoclint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 10:28:49.000000 pydoclint-0.0.4/pydoclint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-27 10:28:49.309871 pydoclint-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-27 10:28:34.000000 pydoclint-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:28:49.309871 pydoclint-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    23976 2023-05-27 10:28:34.000000 pydoclint-0.0.4/tests/test_main.py
```

### Comparing `pydoclint-0.0.3/LICENSE` & `pydoclint-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.3/PKG-INFO` & `pydoclint-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.0.3
+Version: 0.0.4
 Summary: A linter to check arguments in Python docstrings
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
@@ -85,35 +85,50 @@
 
 ## 3. Style violation codes
 
 `pydoclint` currently has the following style violation codes:
 
 ### 3.1. `DOC1xx`: Violations about input arguments
 
-| Code     | Explanation                                                                                                                                    |
-| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
-| `DOC101` | Docstring contains fewer arguments than in function signature                                                                                  |
-| `DOC102` | Docstring contains more arguments than in function signature                                                                                   |
-| `DOC103` | Docstring arguments are different from function arguments. (Or did you miss the space between the argument name and the ":" in the docstring?) |
-| `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                              |
-| `DOC105` | Argument names match, but type hints do not match                                                                                              |
+| Code     | Explanation                                                                                                                                          |
+| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `DOC101` | Docstring contains fewer arguments than in function signature                                                                                        |
+| `DOC102` | Docstring contains more arguments than in function signature                                                                                         |
+| `DOC103` | Docstring arguments are different from function arguments. (Or could be other formatting issues: https://github.com/jsh9/pydoclint/#notes-on-doc103) |
+| `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                                    |
+| `DOC105` | Argument names match, but type hints do not match                                                                                                    |
+
+#### Notes on `DOC103`:
+
+Other potential causes to `DOC103` include:
+
+- Numpy docstring style requires this style: `arg1 : int` (a space between
+  `arg1` and `:`) but people sometimes write `arg1: int`. This will trigger
+  `DOC103`.
+- In the Google style, writing an `Args:` section without the preceding summary
+  will also trigger `DOC103`.
 
 ### 3.2. `DOC2xx`: Violations about return argument(s)
 
 | Code     | Explanation                                                                                          |
 | -------- | ---------------------------------------------------------------------------------------------------- |
 | `DOC201` | Function/method does not have a return section in docstring                                          |
 | `DOC202` | Function/method has a return section in docstring, but there are no return statements or annotations |
 
 ### 3.3. `DOC3xx`: Violations about class docstring and class constructor
 
-| Code     | Explanation                                                                                 |
-| -------- | ------------------------------------------------------------------------------------------- |
-| `DOC301` | `__init__()` should not have a docstring; please combine it with the docstring of the class |
-| `DOC302` | The docstring for the class does not need a "Returns" sections                              |
+| Code     | Explanation                                                                                             |
+| -------- | ------------------------------------------------------------------------------------------------------- |
+| `DOC301` | `__init__()` should not have a docstring; please combine it with the docstring of the class             |
+| `DOC302` | The class docstring does not need a "Returns" section, because `__init__()` cannot return anything      |
+| `DOC303` | The `__init__()` docstring does not need a "Returns" section, because it cannot return anything         |
+| `DOC304` | Class docstring has an argument/parameter section; please put it in the `__init__()` docstring          |
+| `DOC305` | Class docstring has a "Raises" section; please put it in the `__init__()` docstring                     |
+| `DOC306` | The class docstring does not need a "Yields" section, because `__init__()` cannot yield anything        |
+| `DOC307` | The `__init__()` docstring does not need a "Yields" section, because `__init__()` cannot yield anything |
 
 ### 3.4. `DOC4xx`: Violations about "yield" statements
 
 | Code     | Explanation                                                                                                                   |
 | -------- | ----------------------------------------------------------------------------------------------------------------------------- |
 | `DOC401` | Function/method returns a Generator, but the docstring does not have a "Yields" section                                       |
 | `DOC402` | Function/method has "yield" statements, but the docstring does not have a "Yields" section                                    |
@@ -229,7 +244,13 @@
 ```
 
 ### 4.7. `--skip-checking-raises` (shortform: `-scr`, default: `False`)
 
 If `True`, _pydoclint_ won't report `DOC501` or `DOC502` if there are `raise`
 statements in the function/method but there aren't any "raises" sections in the
 docstring (or vice versa).
+
+### 4.8. `--allow-init-docstring` (shortform: `-aid`, default: `False`)
+
+If it is set to `True`, having a docstring for class constructors
+(`__init__()`) is allowed, and the arguments are expected to be documented
+under `__init__()` rather than in the class docstring.
```

### Comparing `pydoclint-0.0.3/README.md` & `pydoclint-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -72,35 +72,50 @@
 
 ## 3. Style violation codes
 
 `pydoclint` currently has the following style violation codes:
 
 ### 3.1. `DOC1xx`: Violations about input arguments
 
-| Code     | Explanation                                                                                                                                    |
-| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
-| `DOC101` | Docstring contains fewer arguments than in function signature                                                                                  |
-| `DOC102` | Docstring contains more arguments than in function signature                                                                                   |
-| `DOC103` | Docstring arguments are different from function arguments. (Or did you miss the space between the argument name and the ":" in the docstring?) |
-| `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                              |
-| `DOC105` | Argument names match, but type hints do not match                                                                                              |
+| Code     | Explanation                                                                                                                                          |
+| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `DOC101` | Docstring contains fewer arguments than in function signature                                                                                        |
+| `DOC102` | Docstring contains more arguments than in function signature                                                                                         |
+| `DOC103` | Docstring arguments are different from function arguments. (Or could be other formatting issues: https://github.com/jsh9/pydoclint/#notes-on-doc103) |
+| `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                                    |
+| `DOC105` | Argument names match, but type hints do not match                                                                                                    |
+
+#### Notes on `DOC103`:
+
+Other potential causes to `DOC103` include:
+
+- Numpy docstring style requires this style: `arg1 : int` (a space between
+  `arg1` and `:`) but people sometimes write `arg1: int`. This will trigger
+  `DOC103`.
+- In the Google style, writing an `Args:` section without the preceding summary
+  will also trigger `DOC103`.
 
 ### 3.2. `DOC2xx`: Violations about return argument(s)
 
 | Code     | Explanation                                                                                          |
 | -------- | ---------------------------------------------------------------------------------------------------- |
 | `DOC201` | Function/method does not have a return section in docstring                                          |
 | `DOC202` | Function/method has a return section in docstring, but there are no return statements or annotations |
 
 ### 3.3. `DOC3xx`: Violations about class docstring and class constructor
 
-| Code     | Explanation                                                                                 |
-| -------- | ------------------------------------------------------------------------------------------- |
-| `DOC301` | `__init__()` should not have a docstring; please combine it with the docstring of the class |
-| `DOC302` | The docstring for the class does not need a "Returns" sections                              |
+| Code     | Explanation                                                                                             |
+| -------- | ------------------------------------------------------------------------------------------------------- |
+| `DOC301` | `__init__()` should not have a docstring; please combine it with the docstring of the class             |
+| `DOC302` | The class docstring does not need a "Returns" section, because `__init__()` cannot return anything      |
+| `DOC303` | The `__init__()` docstring does not need a "Returns" section, because it cannot return anything         |
+| `DOC304` | Class docstring has an argument/parameter section; please put it in the `__init__()` docstring          |
+| `DOC305` | Class docstring has a "Raises" section; please put it in the `__init__()` docstring                     |
+| `DOC306` | The class docstring does not need a "Yields" section, because `__init__()` cannot yield anything        |
+| `DOC307` | The `__init__()` docstring does not need a "Yields" section, because `__init__()` cannot yield anything |
 
 ### 3.4. `DOC4xx`: Violations about "yield" statements
 
 | Code     | Explanation                                                                                                                   |
 | -------- | ----------------------------------------------------------------------------------------------------------------------------- |
 | `DOC401` | Function/method returns a Generator, but the docstring does not have a "Yields" section                                       |
 | `DOC402` | Function/method has "yield" statements, but the docstring does not have a "Yields" section                                    |
@@ -216,7 +231,13 @@
 ```
 
 ### 4.7. `--skip-checking-raises` (shortform: `-scr`, default: `False`)
 
 If `True`, _pydoclint_ won't report `DOC501` or `DOC502` if there are `raise`
 statements in the function/method but there aren't any "raises" sections in the
 docstring (or vice versa).
+
+### 4.8. `--allow-init-docstring` (shortform: `-aid`, default: `False`)
+
+If it is set to `True`, having a docstring for class constructors
+(`__init__()`) is allowed, and the arguments are expected to be documented
+under `__init__()` rather than in the class docstring.
```

### Comparing `pydoclint-0.0.3/pydoclint/flake8_entry.py` & `pydoclint-0.0.4/pydoclint/flake8_entry.py`

 * *Files 15% similar despite different names*

```diff
@@ -49,48 +49,61 @@
         parser.add_option(
             '-scr',
             '--skip-checking-raises',
             action='store',
             default='False',
             help='If True, skip checking docstring "Raises" section against "raise" statements',
         )
+        parser.add_option(
+            '-aid',
+            '--allow-init-docstring',
+            action='store',
+            default='False',
+            help='If True, allow both __init__() and the class def to have docstrings',
+        )
 
     @classmethod
     def parse_options(cls, options):  # noqa: D102
         cls.check_type_hint = options.check_type_hint
         cls.check_arg_order = options.check_arg_order
         cls.skip_checking_short_docstrings = (
             options.skip_checking_short_docstrings
         )
         cls.skip_checking_raises = options.skip_checking_raises
+        cls.allow_init_docstring = options.allow_init_docstring
         cls.style = options.style
 
     def run(self) -> Generator[Tuple[int, int, str, Any], None, None]:
         """Run the linter and yield the violation information"""
         checkTypeHint = self._bool('--check-type-hint', self.check_type_hint)
         checkArgOrder = self._bool('--check-arg-order', self.check_arg_order)
         skipCheckingShortDocstrings = self._bool(
             '--skip-checking-short-docstrings',
             self.skip_checking_short_docstrings,
         )
         skipCheckingRaises = self._bool(
             '--skip-checking-raises',
             self.skip_checking_raises,
         )
+        allowInitDocstring = self._bool(
+            '--allow-init-docstring',
+            self.allow_init_docstring,
+        )
 
         if self.style not in {'numpy', 'google'}:
             raise ValueError(
                 'Invalid value for "--style": must be "numpy" or "google"'
             )
 
         v = Visitor(
             checkTypeHint=checkTypeHint,
             checkArgOrder=checkArgOrder,
             skipCheckingShortDocstrings=skipCheckingShortDocstrings,
             skipCheckingRaises=skipCheckingRaises,
+            allowInitDocstring=allowInitDocstring,
             style=self.style,
         )
         v.visit(self._tree)
         violationInfo = [_.getInfoForFlake8() for _ in v.violations]
         for line, colOffset, msg in violationInfo:
             yield line, colOffset, msg, type(self)
```

### Comparing `pydoclint-0.0.3/pydoclint/main.py` & `pydoclint-0.0.4/pydoclint/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,22 @@
     '-scr',
     '--skip-checking-raises',
     type=bool,
     show_default=True,
     default=False,
     help='If True, skip checking docstring "Raises" section against "raise" statements',
 )
+@click.option(
+    '-aid',
+    '--allow-init-docstring',
+    type=bool,
+    show_default=True,
+    default=False,
+    help='If True, allow both __init__() and the class def to have docstrings',
+)
 @click.argument(
     'paths',
     nargs=-1,
     type=click.Path(
         exists=True,
         file_okay=True,
         dir_okay=True,
@@ -111,14 +119,15 @@
         style: str,
         src: Optional[str],
         paths: Tuple[str, ...],
         check_type_hint: bool,
         check_arg_order: bool,
         skip_checking_short_docstrings: bool,
         skip_checking_raises: bool,
+        allow_init_docstring: bool,
 ) -> None:
     """Command-line entry point of pydoclint"""
     ctx.ensure_object(dict)
 
     if paths and src is not None:
         click.echo(
             main.get_usage(ctx)
@@ -137,14 +146,15 @@
         exclude=exclude,
         style=style,
         paths=paths,
         checkTypeHint=check_type_hint,
         checkArgOrder=check_arg_order,
         skipCheckingShortDocstrings=skip_checking_short_docstrings,
         skipCheckingRaises=skip_checking_raises,
+        allowInitDocstring=allow_init_docstring,
     )
 
     violationCounter: int = 0
     if len(violationsInAllFiles) > 0:
         counter = 0
         for filename, violationsInThisFile in violationsInAllFiles.items():
             counter += 1
@@ -180,14 +190,15 @@
 def _checkPaths(
         paths: Tuple[str, ...],
         style: str = 'numpy',
         checkTypeHint: bool = True,
         checkArgOrder: bool = True,
         skipCheckingShortDocstrings: bool = True,
         skipCheckingRaises: bool = False,
+        allowInitDocstring: bool = False,
         quiet: bool = False,
         exclude: str = '',
 ) -> Dict[str, List[Violation]]:
     filenames: List[Path] = []
 
     if not quiet:
         skipMsg = f'Skipping files that match this pattern: {exclude}'
@@ -214,38 +225,41 @@
         violationsInThisFile: List[Violation] = _checkFile(
             filename,
             style=style,
             checkTypeHint=checkTypeHint,
             checkArgOrder=checkArgOrder,
             skipCheckingShortDocstrings=skipCheckingShortDocstrings,
             skipCheckingRaises=skipCheckingRaises,
+            allowInitDocstring=allowInitDocstring,
         )
         allViolations[filename.as_posix()] = violationsInThisFile
 
     return allViolations
 
 
 def _checkFile(
         filename: Path,
         style: str = 'numpy',
         checkTypeHint: bool = True,
         checkArgOrder: bool = True,
         skipCheckingShortDocstrings: bool = True,
         skipCheckingRaises: bool = False,
+        allowInitDocstring: bool = False,
 ) -> List[Violation]:
     with open(filename) as fp:
         src: str = ''.join(fp.readlines())
 
     tree: ast.Module = ast.parse(src)
     visitor = Visitor(
         style=style,
         checkTypeHint=checkTypeHint,
         checkArgOrder=checkArgOrder,
         skipCheckingShortDocstrings=skipCheckingShortDocstrings,
         skipCheckingRaises=skipCheckingRaises,
+        allowInitDocstring=allowInitDocstring,
     )
     visitor.visit(tree)
     return visitor.violations
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pydoclint-0.0.3/pydoclint/utils/arg.py` & `pydoclint-0.0.4/pydoclint/utils/arg.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ast
 from typing import List, Optional, Set
 
 from docstring_parser.common import DocstringParam
 from numpydoc.docscrape import Parameter
 
-from pydoclint.utils.annotation import parseAnnotation
+from pydoclint.utils.annotation import unparseAnnotation
 
 
 class Arg:
     """
     A class to hold function input/return arguments.
 
     This class also defines some essential behaviors of an argument, such
@@ -24,19 +24,19 @@
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def __str__(self) -> str:
         return f'{self.name}: {self.typeHint}'
 
-    def __eq__(self, other: 'Arg') -> bool:
-        if not isinstance(other, Arg):
+    def __eq__(self, o: 'Arg') -> bool:
+        if not isinstance(o, Arg):
             return False
 
-        return self.name == other.name and self.typeHint == other.typeHint
+        return self.name == o.name and self._eq(self.typeHint, o.typeHint)
 
     def __lt__(self, other: 'Arg') -> bool:
         if not isinstance(other, Arg):
             raise TypeError('Cannot compare; `other` is not of "Arg" type')
 
         if self.name < other.name:
             return True
@@ -46,15 +46,15 @@
 
         return self.typeHint < other.typeHint
 
     def __le__(self, other: 'Arg') -> bool:
         return self < other or self == other
 
     def __hash__(self) -> int:
-        return hash((self.name, self.typeHint))
+        return hash((self.name, self._stripQuotes(self.typeHint)))
 
     def nameEquals(self, other: 'Arg') -> bool:
         """More lenient equality: only compare names"""
         return self.name == other.name
 
     @classmethod
     def fromNumpydocParam(cls, param: Parameter) -> 'Arg':
@@ -66,21 +66,29 @@
         """Construct an Arg object from a GoogleParser Parameter object"""
         return Arg(name=param.arg_name, typeHint=cls._str(param.type_name))
 
     @classmethod
     def fromAstArg(cls, astArg: ast.arg) -> 'Arg':
         """Construct an Arg object from a Python AST argument object"""
         anno = astArg.annotation
-        typeHint: str = '' if anno is None else parseAnnotation(anno)
+        typeHint: str = '' if anno is None else unparseAnnotation(anno)
         return Arg(name=astArg.arg, typeHint=typeHint)
 
     @classmethod
     def _str(cls, typeName: Optional[str]) -> str:
         return '' if typeName is None else typeName
 
+    @classmethod
+    def _eq(cls, str1: str, str2: str) -> bool:
+        return cls._stripQuotes(str1) == cls._stripQuotes(str2)
+
+    @classmethod
+    def _stripQuotes(cls, string: str) -> str:
+        return string.replace('"', '').replace("'", '')
+
 
 class ArgList:
     """
     A class to hold a list of `Arg` objects.
 
     This class also defines some behaviors of an argument list, such as
     equality, length calculation, etc.
@@ -101,18 +109,44 @@
 
     def __eq__(self, other: 'ArgList') -> bool:
         if not isinstance(other, ArgList):
             return False
 
         return self.infoList == other.infoList
 
+    @property
+    def isEmpty(self) -> bool:
+        """Whether the arg list is empty"""
+        return self.length == 0
+
+    @property
+    def nonEmpty(self) -> bool:
+        """Whether the arg list is non-empty"""
+        return not self.isEmpty
+
+    @property
     def length(self) -> int:
         """Calculate the length of the list"""
         return len(self.infoList)
 
+    @classmethod
+    def fromNumpydocParam(cls, params: List[Parameter]) -> 'ArgList':
+        """Construct an Arglist from a list of Parameter objects"""
+        return ArgList([Arg.fromNumpydocParam(_) for _ in params])
+
+    @classmethod
+    def fromGoogleParsedParam(cls, params: List[DocstringParam]) -> 'ArgList':
+        """Construct an ArgList from a list of DocstringParam objects"""
+        infoList = [
+            Arg.fromGoogleParsedParam(_)
+            for _ in params
+            if _.args[0] != 'attribute'  # we only need 'param' not 'attribute'
+        ]
+        return ArgList(infoList=infoList)
+
     def contains(self, arg: Arg) -> bool:
         """Whether a given `Arg` object exists in the list"""
         return arg.name in self.lookup
 
     def get(self, argName: str) -> Arg:
         """Retrieve an element from the list using `argName` as identifier"""
         if argName not in self.lookup:
@@ -144,15 +178,15 @@
         -------
         bool
             Whether the two objects are equal.
         """
         if not isinstance(other, ArgList):
             return False
 
-        if self.length() != other.length():
+        if self.length != other.length:
             return False
 
         verdict: bool
 
         if checkTypeHint:
             if orderMatters:  # most strict case
                 verdict = self == other
```

### Comparing `pydoclint-0.0.3/pydoclint/utils/doc.py` & `pydoclint-0.0.4/pydoclint/utils/doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from docstring_parser.common import DocstringReturns
 from docstring_parser.google import GoogleParser
 from numpydoc.docscrape import NumpyDocString
 
-from pydoclint.utils.arg import Arg, ArgList
+from pydoclint.utils.arg import ArgList
 from pydoclint.utils.internal_error import InternalError
 
 
 class Doc:
     """A class to hold docstring and to provide info on the parsed docstring"""
 
     def __init__(self, docstring: str, style: str = 'numpy') -> None:
@@ -71,25 +71,18 @@
 
         self._raiseException()  # noqa: R503
 
     @property
     def argList(self) -> ArgList:
         """The argument info in the docstring, presented as an ArgList"""
         if self.style == 'numpy':
-            return ArgList(
-                [
-                    Arg.fromNumpydocParam(_)
-                    for _ in self.parsed.get('Parameters', [])
-                ]
-            )
+            return ArgList.fromNumpydocParam(self.parsed.get('Parameters', []))
 
         if self.style == 'google':
-            return ArgList(
-                [Arg.fromGoogleParsedParam(_) for _ in self.parsed.params]
-            )
+            return ArgList.fromGoogleParsedParam(self.parsed.params)
 
         self._raiseException()  # noqa: R503
 
     @property
     def hasReturnsSection(self) -> bool:
         """Whether the docstring has a 'Returns' section"""
         if self.style == 'numpy':
```

### Comparing `pydoclint-0.0.3/pydoclint/utils/generic.py` & `pydoclint-0.0.4/pydoclint/utils/generic.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.3/pydoclint/utils/return_yield_raise.py` & `pydoclint-0.0.4/pydoclint/utils/return_yield_raise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ast
 from typing import Tuple, Type, Union
 
 from pydoclint.utils import walk
-from pydoclint.utils.annotation import parseAnnotation
+from pydoclint.utils.annotation import unparseAnnotation
 from pydoclint.utils.astTypes import BlockType, FuncOrAsyncFuncDef
 from pydoclint.utils.generic import getFunctionId
 
 ReturnType = Type[ast.Return]
 ExprType = Type[ast.Expr]
 YieldAndYieldFromTypes = Tuple[Type[ast.Yield], Type[ast.YieldFrom]]
 FuncOrAsyncFuncTypes = Tuple[Type[ast.FunctionDef], Type[ast.AsyncFunctionDef]]
@@ -18,15 +18,15 @@
 
 
 def hasGeneratorAsReturnAnnotation(node: FuncOrAsyncFuncDef) -> bool:
     """Check whether the function node has a 'Generator' return annotation"""
     if node.returns is None:
         return False
 
-    returnAnnotation: str = parseAnnotation(node.returns)
+    returnAnnotation: str = unparseAnnotation(node.returns)
     return returnAnnotation.startswith('Generator')
 
 
 def hasYieldStatements(node: FuncOrAsyncFuncDef) -> bool:
     """Check whether the function node has any yield statements"""
     thisId = getFunctionId(node)
     for child, parent in walk.walk(node):
```

### Comparing `pydoclint-0.0.3/pydoclint/utils/violation.py` & `pydoclint-0.0.4/pydoclint/utils/violation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 import types
 from typing import Tuple
 
 from pydoclint.utils.internal_error import InternalError
 
 VIOLATION_CODES = types.MappingProxyType({
+    1: 'Potential formatting errors in docstring. Error message:',
+
     101: 'Docstring contains fewer arguments than in function signature.',
     102: 'Docstring contains more arguments than in function signature.',
     103: (  # noqa: PAR001
         'Docstring arguments are different from function arguments.'
-        ' (Or did you miss the space between the argument name'
-        ' and the ":" in the docstring?).'
+        ' (Or could be other formatting issues: https://github.com/jsh9/pydoclint/#notes-on-doc103).'
     ),
     104: 'Arguments are the same in the docstring and the function signature, but are in a different order.',
     105: 'Argument names match, but type hints do not match',
+
     201: 'does not have a return section in docstring',
     202: 'has a return section in docstring, but there are no return statements or annotations',
+
     301: '__init__() should not have a docstring; please combine it with the docstring of the class',
-    302: 'The docstring for the class does not need a "Returns" sections',
+    302: 'The class docstring does not need a "Returns" section, because __init__() cannot return anything',
+    303: 'The __init__() docstring does not need a "Returns" section, because it cannot return anything',
+    304: 'Class docstring has an argument/parameter section; please put it in the __init__() docstring',
+    305: 'Class docstring has a "Raises" section; please put it in the __init__() docstring',
+    306: 'The class docstring does not need a "Yields" section, because __init__() cannot yield anything',
+    307: 'The __init__() docstring does not need a "Yields" section, because __init__() cannot yield anything',
+
     401: 'returns a Generator, but the docstring does not have a "Yields" section',
     402: 'has "yield" statements, but the docstring does not have a "Yields" section',
     403: 'has a "Yields" section in the docstring, but there are no "yield" statements or a Generator return annotation',
+
     501: 'has "raise" statements, but the docstring does not have a "Raises" section',
     502: 'has a "Raises" section in the docstring, but there are not "raise" statements in the body',
 })
 
 
 class Violation:
     """A class to hold information of a style violation"""
@@ -41,21 +51,21 @@
         self.line = line
         self.code = code
         self.msg = msgPrefix + ' ' + VIOLATION_CODES[code] + ' ' + msgPostfix
 
     @property
     def fullErrorCode(self) -> str:
         """Full error code, including the 'DOC' prefix"""
-        return f'DOC{self.code}'
+        return 'DOC' + f'{self.code}'.zfill(3)
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def __str__(self) -> str:
-        return f'DOC{self.code}: {self.msg}'
+        return f'{self.fullErrorCode}: {self.msg}'
 
     def _str(self, showLineNum: bool = False) -> str:
         if not showLineNum:
             return self.__str__()
 
         return f'{self.line}: {self.__str__()}'
```

### Comparing `pydoclint-0.0.3/pydoclint/utils/walk.py` & `pydoclint-0.0.4/pydoclint/utils/walk.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.3/pydoclint/visitor.py` & `pydoclint-0.0.4/pydoclint/visitor.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pydoclint.utils.doc import Doc
 from pydoclint.utils.generic import (
     collectFuncArgs,
     detectMethodType,
     generateMsgPrefix,
     getDocstring,
 )
+from pydoclint.utils.internal_error import InternalError
 from pydoclint.utils.method_type import MethodType
 from pydoclint.utils.return_yield_raise import (
     hasGeneratorAsReturnAnnotation,
     hasRaiseStatements,
     hasReturnAnnotation,
     hasReturnStatements,
     hasYieldStatements,
@@ -27,20 +28,22 @@
     def __init__(
             self,
             style: str = 'numpy',
             checkTypeHint: bool = True,
             checkArgOrder: bool = True,
             skipCheckingShortDocstrings: bool = True,
             skipCheckingRaises: bool = False,
+            allowInitDocstring: bool = False,
     ) -> None:
         self.style: str = style
         self.checkTypeHint: bool = checkTypeHint
         self.checkArgOrder: bool = checkArgOrder
         self.skipCheckingShortDocstrings: bool = skipCheckingShortDocstrings
         self.skipCheckingRaises: bool = skipCheckingRaises
+        self.allowInitDocstring: bool = allowInitDocstring
 
         self.parent: Optional[ast.AST] = None  # keep track of parent node
         self.violations: List[Violation] = []
 
     def visit_ClassDef(self, node: ast.ClassDef):  # noqa: D102
         currentParent = self.parent  # keep aside
         self.parent = node
@@ -56,27 +59,19 @@
         isClassConstructor: bool = node.name == '__init__' and isinstance(
             parent_, ast.ClassDef
         )
 
         docstring: str = getDocstring(node)
 
         if isClassConstructor:
-            className: str = parent_.name
-            if len(docstring) > 0:  # __init__() has its own docstring
-                self.violations.append(
-                    Violation(
-                        code=301,
-                        line=node.lineno,
-                        msgPrefix=f'Class `{className}`:',
-                    )
-                )
-
-            # Inspect class docstring instead, because that's what we care
-            # about when checking the class constructor.
-            docstring = getDocstring(parent_)
+            docstring = self._checkClassConstructorDocstrings(
+                node=node,
+                parent_=parent_,
+                initDocstring=docstring,
+            )
 
         argViolations: List[Violation]
         returnViolations: List[Violation]
         yieldViolations: List[Violation]
         raiseViolations: List[Violation]
 
         if docstring == '':
@@ -86,15 +81,27 @@
             # or pydocstyle (https://www.pydocstyle.org/en/stable/)
             # to determine whether a function needs a docstring.
             argViolations = []
             returnViolations = []
             yieldViolations = []
             raiseViolations = []
         else:
-            doc: Doc = Doc(docstring=docstring, style=self.style)
+            try:
+                doc: Doc = Doc(docstring=docstring, style=self.style)
+            except Exception as excp:
+                doc = Doc(docstring='', style=self.style)
+                self.violations.append(
+                    Violation(
+                        code=1,
+                        line=node.lineno,
+                        msgPrefix=f'Function/method `{node.name}`:',
+                        msgPostfix=str(excp).replace('\n', ' '),
+                    )
+                )
+
             isShort: bool = doc.isShortDocstring
             if self.skipCheckingShortDocstrings and isShort:
                 argViolations = []
                 returnViolations = []
                 yieldViolations = []
                 raiseViolations = []
             else:
@@ -110,16 +117,18 @@
                         raiseViolations = self.checkRaises(node, parent_, doc)
                     else:
                         raiseViolations = []
 
             if isClassConstructor:
                 # Re-check return violations because the rules are
                 # different for class constructors.
-                returnViolations = self.checkReturnsInClassConstructor(
-                    parent=parent_, doc=doc
+                returnViolations = (
+                    self.checkReturnsAndYieldsInClassConstructor(
+                        parent=parent_, doc=doc
+                    )
                 )
 
         self.violations.extend(argViolations)
         self.violations.extend(returnViolations)
         self.violations.extend(yieldViolations)
         self.violations.extend(raiseViolations)
 
@@ -130,14 +139,139 @@
     def visit_AsyncFunctionDef(self, node: ast.AsyncFunctionDef):  # noqa: D102
         # Treat async functions similarly to regular ones
         self.visit_FunctionDef(node)
 
     def visit_Raise(self, node: ast.Raise):  # noqa: D102
         self.generic_visit(node)
 
+    def _checkClassConstructorDocstrings(  # noqa: C901
+            self,
+            node: FuncOrAsyncFuncDef,
+            parent_: ast.ClassDef,
+            initDocstring: str,
+    ) -> str:
+        """
+        Check class docstring and __init__() docstring.
+
+        If only class docstring exists, or if __init__() is not allowed to have
+        its own docstring, return the class docstring for further checking.
+
+        Otherwise, return the __init__() docstring for further checking.
+        """
+        if not isinstance(parent_, ast.ClassDef):
+            msg = (
+                'This should not have happened; please contact the authors'
+                ' and share the full call stack.'
+            )
+            raise InternalError(msg)
+
+        className: str = parent_.name
+        classLineNum: int = parent_.lineno
+
+        classDocstring: str = getDocstring(parent_)
+
+        if len(initDocstring) == 0:  # __init__() doesn't have its own docstring
+            # Check class docstring instead, because that's what we care
+            # about when checking the class constructor.
+            return classDocstring
+
+        # Below: __init__() has its own docstring
+        if not self.allowInitDocstring:
+            self.violations.append(
+                Violation(
+                    code=301,
+                    line=node.lineno,
+                    msgPrefix=f'Class `{className}`:',
+                )
+            )
+            return classDocstring
+
+        # Below: __init__() is allowed to have a separate docstring
+        try:
+            classDoc = Doc(docstring=classDocstring, style=self.style)
+        except Exception as excp:
+            classDoc = Doc(docstring='', style=self.style)
+            self.violations.append(
+                Violation(
+                    code=1,
+                    line=parent_.lineno,
+                    msgPrefix=f'Class `{className}`:',
+                    msgPostfix=str(excp).replace('\n', ' '),
+                )
+            )
+
+        try:
+            initDoc = Doc(docstring=initDocstring, style=self.style)
+        except Exception as excp:
+            initDoc = Doc(docstring='', style=self.style)
+            self.violations.append(
+                Violation(
+                    code=1,
+                    line=node.lineno,
+                    msgPrefix=f'Method `{node.name}`',
+                    msgPostfix=str(excp).replace('\n', ' '),
+                )
+            )
+
+        if classDoc.hasReturnsSection:
+            self.violations.append(
+                Violation(
+                    code=302,
+                    line=classLineNum,
+                    msgPrefix=f'Class `{className}`:',
+                )
+            )
+
+        if initDoc.hasReturnsSection:
+            self.violations.append(
+                Violation(
+                    code=303,
+                    line=node.lineno,
+                    msgPrefix=f'Class `{className}`:',
+                )
+            )
+
+        if classDoc.argList.nonEmpty:
+            self.violations.append(
+                Violation(
+                    code=304,
+                    line=classLineNum,
+                    msgPrefix=f'Class `{className}`:',
+                )
+            )
+
+        if classDoc.hasYieldsSection:
+            self.violations.append(
+                Violation(
+                    code=306,
+                    line=classLineNum,
+                    msgPrefix=f'Class `{className}`:',
+                )
+            )
+
+        if initDoc.hasYieldsSection:
+            self.violations.append(
+                Violation(
+                    code=307,
+                    line=classLineNum,
+                    msgPrefix=f'Class `{className}`:',
+                )
+            )
+
+        if classDoc.hasRaisesSection:
+            self.violations.append(
+                Violation(
+                    code=305,
+                    line=classLineNum,
+                    msgPrefix=f'Class `{className}`:',
+                )
+            )
+
+        return initDocstring
+
     def checkArguments(  # noqa: C901
             self,
             node: FuncOrAsyncFuncDef,
             parent_: ast.AST,
             doc: Doc,
     ) -> List[Violation]:
         """
@@ -174,22 +308,22 @@
         v102 = Violation(code=102, line=lineNum, msgPrefix=msgPrefix)
         v104 = Violation(code=104, line=lineNum, msgPrefix=msgPrefix)
         v105 = Violation(code=105, line=lineNum, msgPrefix=msgPrefix)
 
         docArgs = doc.argList
         funcArgs = ArgList([Arg.fromAstArg(_) for _ in astArgList])
 
-        if docArgs.length() == 0 and funcArgs.length() == 0:
+        if docArgs.length == 0 and funcArgs.length == 0:
             return []
 
         violations: List[Violation] = []
-        if docArgs.length() < funcArgs.length():
+        if docArgs.length < funcArgs.length:
             violations.append(v101)
 
-        if docArgs.length() > funcArgs.length():
+        if docArgs.length > funcArgs.length:
             violations.append(v102)
 
         if not docArgs.equals(
             funcArgs,
             checkTypeHint=self.checkTypeHint,
             orderMatters=self.checkArgOrder,
         ):
@@ -270,30 +404,39 @@
 
         if docstringHasReturnSection and not (hasReturnStmt or hasReturnAnno):
             violations.append(v202)
 
         return violations
 
     @classmethod
-    def checkReturnsInClassConstructor(
+    def checkReturnsAndYieldsInClassConstructor(
             cls,
             parent: ast.ClassDef,
             doc: Doc,
     ) -> List[Violation]:
-        """Check the presence of a "Returns" section in class docstring"""
+        """Check the presence of a Returns/Yields section in class docstring"""
         violations: List[Violation] = []
         if doc.hasReturnsSection:
             violations.append(
                 Violation(
                     code=302,
                     line=parent.lineno,
                     msgPrefix=f'Class `{parent.name}`:',
                 )
             )
 
+        if doc.hasYieldsSection:
+            violations.append(
+                Violation(
+                    code=306,
+                    line=parent.lineno,
+                    msgPrefix=f'Class `{parent.name}`:',
+                )
+            )
+
         return violations
 
     @classmethod
     def checkYields(
             cls,
             node: FuncOrAsyncFuncDef,
             parent: ast.AST,
```

### Comparing `pydoclint-0.0.3/pydoclint.egg-info/PKG-INFO` & `pydoclint-0.0.4/pydoclint.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.0.3
+Version: 0.0.4
 Summary: A linter to check arguments in Python docstrings
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
@@ -85,35 +85,50 @@
 
 ## 3. Style violation codes
 
 `pydoclint` currently has the following style violation codes:
 
 ### 3.1. `DOC1xx`: Violations about input arguments
 
-| Code     | Explanation                                                                                                                                    |
-| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
-| `DOC101` | Docstring contains fewer arguments than in function signature                                                                                  |
-| `DOC102` | Docstring contains more arguments than in function signature                                                                                   |
-| `DOC103` | Docstring arguments are different from function arguments. (Or did you miss the space between the argument name and the ":" in the docstring?) |
-| `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                              |
-| `DOC105` | Argument names match, but type hints do not match                                                                                              |
+| Code     | Explanation                                                                                                                                          |
+| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `DOC101` | Docstring contains fewer arguments than in function signature                                                                                        |
+| `DOC102` | Docstring contains more arguments than in function signature                                                                                         |
+| `DOC103` | Docstring arguments are different from function arguments. (Or could be other formatting issues: https://github.com/jsh9/pydoclint/#notes-on-doc103) |
+| `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                                    |
+| `DOC105` | Argument names match, but type hints do not match                                                                                                    |
+
+#### Notes on `DOC103`:
+
+Other potential causes to `DOC103` include:
+
+- Numpy docstring style requires this style: `arg1 : int` (a space between
+  `arg1` and `:`) but people sometimes write `arg1: int`. This will trigger
+  `DOC103`.
+- In the Google style, writing an `Args:` section without the preceding summary
+  will also trigger `DOC103`.
 
 ### 3.2. `DOC2xx`: Violations about return argument(s)
 
 | Code     | Explanation                                                                                          |
 | -------- | ---------------------------------------------------------------------------------------------------- |
 | `DOC201` | Function/method does not have a return section in docstring                                          |
 | `DOC202` | Function/method has a return section in docstring, but there are no return statements or annotations |
 
 ### 3.3. `DOC3xx`: Violations about class docstring and class constructor
 
-| Code     | Explanation                                                                                 |
-| -------- | ------------------------------------------------------------------------------------------- |
-| `DOC301` | `__init__()` should not have a docstring; please combine it with the docstring of the class |
-| `DOC302` | The docstring for the class does not need a "Returns" sections                              |
+| Code     | Explanation                                                                                             |
+| -------- | ------------------------------------------------------------------------------------------------------- |
+| `DOC301` | `__init__()` should not have a docstring; please combine it with the docstring of the class             |
+| `DOC302` | The class docstring does not need a "Returns" section, because `__init__()` cannot return anything      |
+| `DOC303` | The `__init__()` docstring does not need a "Returns" section, because it cannot return anything         |
+| `DOC304` | Class docstring has an argument/parameter section; please put it in the `__init__()` docstring          |
+| `DOC305` | Class docstring has a "Raises" section; please put it in the `__init__()` docstring                     |
+| `DOC306` | The class docstring does not need a "Yields" section, because `__init__()` cannot yield anything        |
+| `DOC307` | The `__init__()` docstring does not need a "Yields" section, because `__init__()` cannot yield anything |
 
 ### 3.4. `DOC4xx`: Violations about "yield" statements
 
 | Code     | Explanation                                                                                                                   |
 | -------- | ----------------------------------------------------------------------------------------------------------------------------- |
 | `DOC401` | Function/method returns a Generator, but the docstring does not have a "Yields" section                                       |
 | `DOC402` | Function/method has "yield" statements, but the docstring does not have a "Yields" section                                    |
@@ -229,7 +244,13 @@
 ```
 
 ### 4.7. `--skip-checking-raises` (shortform: `-scr`, default: `False`)
 
 If `True`, _pydoclint_ won't report `DOC501` or `DOC502` if there are `raise`
 statements in the function/method but there aren't any "raises" sections in the
 docstring (or vice versa).
+
+### 4.8. `--allow-init-docstring` (shortform: `-aid`, default: `False`)
+
+If it is set to `True`, having a docstring for class constructors
+(`__init__()`) is allowed, and the arguments are expected to be documented
+under `__init__()` rather than in the class docstring.
```

### Comparing `pydoclint-0.0.3/pydoclint.egg-info/SOURCES.txt` & `pydoclint-0.0.4/pydoclint.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -18,10 +18,11 @@
 pydoclint/utils/arg.py
 pydoclint/utils/astTypes.py
 pydoclint/utils/doc.py
 pydoclint/utils/generic.py
 pydoclint/utils/internal_error.py
 pydoclint/utils/method_type.py
 pydoclint/utils/return_yield_raise.py
+pydoclint/utils/unparser.py
 pydoclint/utils/violation.py
 pydoclint/utils/walk.py
 tests/test_main.py
```

### Comparing `pydoclint-0.0.3/setup.cfg` & `pydoclint-0.0.4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydoclint
-version = 0.0.3
+version = 0.0.4
 description = A linter to check arguments in Python docstrings
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/pydoclint
 license = MIT
 license_file = LICENSE
 classifiers =
```

