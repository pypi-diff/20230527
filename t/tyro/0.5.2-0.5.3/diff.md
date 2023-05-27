# Comparing `tmp/tyro-0.5.2.tar.gz` & `tmp/tyro-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tyro-0.5.2.tar", max compression
+gzip compressed data, was "tyro-0.5.3.tar", max compression
```

## Comparing `tyro-0.5.2.tar` & `tyro-0.5.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1065 2023-05-10 07:27:30.566393 tyro-0.5.2/LICENSE
--rw-r--r--   0        0        0     4445 2023-05-10 07:29:30.531699 tyro-0.5.2/README.md
--rw-r--r--   0        0        0     1866 2023-05-10 07:27:30.570393 tyro-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      406 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/__init__.py
--rw-r--r--   0        0        0    22530 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_argparse_formatter.py
--rw-r--r--   0        0        0    19335 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_arguments.py
--rw-r--r--   0        0        0     8560 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_calling.py
--rw-r--r--   0        0        0    15642 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_cli.py
--rw-r--r--   0        0        0      101 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_deprecated.py
--rw-r--r--   0        0        0    11749 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_docstrings.py
--rw-r--r--   0        0        0    30130 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_fields.py
--rw-r--r--   0        0        0    23100 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_instantiators.py
--rw-r--r--   0        0        0    21122 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_parsers.py
--rw-r--r--   0        0        0    11374 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_resolver.py
--rw-r--r--   0        0        0      383 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_singleton.py
--rw-r--r--   0        0        0     4949 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/_strings.py
--rw-r--r--   0        0        0     3793 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/_subcommand_matching.py
--rw-r--r--   0        0        0      764 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/_typing.py
--rw-r--r--   0        0        0     1206 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/_unsafe_cache.py
--rw-r--r--   0        0        0     1083 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/conf/__init__.py
--rw-r--r--   0        0        0     1998 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/conf/_confstruct.py
--rw-r--r--   0        0        0     5781 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/conf/_markers.py
--rw-r--r--   0        0        0      579 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/extras/__init__.py
--rw-r--r--   0        0        0     2055 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/extras/_base_configs.py
--rw-r--r--   0        0        0     1129 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/extras/_choices_type.py
--rw-r--r--   0        0        0     8196 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/extras/_serialization.py
--rw-r--r--   0        0        0        0 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/py.typed
--rw-r--r--   0        0        0     5552 1970-01-01 00:00:00.000000 tyro-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-27 10:12:15.896200 tyro-0.5.3/LICENSE
+-rw-r--r--   0        0        0     4445 2023-05-27 10:16:06.311375 tyro-0.5.3/README.md
+-rw-r--r--   0        0        0     1866 2023-05-27 10:12:15.896200 tyro-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      406 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/__init__.py
+-rw-r--r--   0        0        0    22530 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_argparse_formatter.py
+-rw-r--r--   0        0        0    19335 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_arguments.py
+-rw-r--r--   0        0        0     8560 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_calling.py
+-rw-r--r--   0        0        0    15674 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_cli.py
+-rw-r--r--   0        0        0      101 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_deprecated.py
+-rw-r--r--   0        0        0    11749 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_docstrings.py
+-rw-r--r--   0        0        0    30130 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_fields.py
+-rw-r--r--   0        0        0    23376 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_instantiators.py
+-rw-r--r--   0        0        0    21122 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_parsers.py
+-rw-r--r--   0        0        0    11374 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_resolver.py
+-rw-r--r--   0        0        0      383 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_singleton.py
+-rw-r--r--   0        0        0     4949 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_strings.py
+-rw-r--r--   0        0        0     3793 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_subcommand_matching.py
+-rw-r--r--   0        0        0      764 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_typing.py
+-rw-r--r--   0        0        0     1206 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_unsafe_cache.py
+-rw-r--r--   0        0        0     1083 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/conf/__init__.py
+-rw-r--r--   0        0        0     1998 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/conf/_confstruct.py
+-rw-r--r--   0        0        0     5805 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/conf/_markers.py
+-rw-r--r--   0        0        0      579 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/extras/__init__.py
+-rw-r--r--   0        0        0     2354 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/extras/_base_configs.py
+-rw-r--r--   0        0        0     1258 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/extras/_choices_type.py
+-rw-r--r--   0        0        0     8196 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/extras/_serialization.py
+-rw-r--r--   0        0        0        0 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/py.typed
+-rw-r--r--   0        0        0     5552 1970-01-01 00:00:00.000000 tyro-0.5.3/PKG-INFO
```

### Comparing `tyro-0.5.2/LICENSE` & `tyro-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tyro-0.5.2/README.md` & `tyro-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `tyro-0.5.2/pyproject.toml` & `tyro-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tyro"
-version = "0.5.2"
+version = "0.5.3"
 description = "Strongly typed, zero-effort CLI interfaces"
 authors = ["brentyi <brentyi@berkeley.edu>"]
 include = ["./tyro/**/*"]
 readme = "README.md"
 repository = "https://github.com/brentyi/tyro"
 homepage = "https://github.com/brentyi/tyro"
 documentation = "https://brentyi.github.io/tyro/"
```

### Comparing `tyro-0.5.2/tyro/_argparse_formatter.py` & `tyro-0.5.3/tyro/_argparse_formatter.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.2/tyro/_arguments.py` & `tyro-0.5.3/tyro/_arguments.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.2/tyro/_calling.py` & `tyro-0.5.3/tyro/_calling.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.2/tyro/_cli.py` & `tyro-0.5.3/tyro/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,14 +365,15 @@
     )
 
     # Generate parser!
     with _argparse_formatter.ansi_context():
         parser = argparse.ArgumentParser(
             prog=prog,
             formatter_class=_argparse_formatter.TyroArgparseHelpFormatter,
+            allow_abbrev=False,
         )
         parser_definition.apply(parser)
 
         # Print help message when no arguments are passed in. (but arguments are
         # expected)
         if len(args) == 0 and parser_definition.has_required_args:
             args = ["--help"]
```

### Comparing `tyro-0.5.2/tyro/_docstrings.py` & `tyro-0.5.3/tyro/_docstrings.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.2/tyro/_fields.py` & `tyro-0.5.3/tyro/_fields.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.2/tyro/_instantiators.py` & `tyro-0.5.3/tyro/_instantiators.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,21 @@
     Final,
     Literal,
     get_args,
     get_origin,
     get_type_hints,
 )
 
+# There are cases where typing.Literal doesn't match typing_extensions.Literal:
+# https://github.com/python/typing_extensions/pull/148
+try:
+    from typing import Literal as LiteralAlternate
+except ImportError:
+    LiteralAlternate = Literal  # type: ignore
+
 from . import _strings
 from ._typing import TypeForm
 from .conf import _markers
 
 _StandardInstantiator = Callable[[List[str]], Any]
 _AppendNargsInstantiator = Callable[[List[List[str]]], Any]
 # Special case: the only time that argparse doesn't give us a string is when the
@@ -321,15 +328,15 @@
             list,
             set,
             deque,
         ),
         _instantiator_from_tuple: (tuple,),
         _instantiator_from_dict: (dict, collections.abc.Mapping),
         _instantiator_from_union: (Union,),
-        _instantiator_from_literal: (Literal,),
+        _instantiator_from_literal: (Literal, LiteralAlternate),
     }.items():
         if type_origin in matched_origins:
             return make(typ, type_from_typevar, markers)
 
     raise UnsupportedTypeAnnotationError(  # pragma: no cover
         f"Unsupported type {typ} with origin {type_origin}"
     )
```

### Comparing `tyro-0.5.2/tyro/_parsers.py` & `tyro-0.5.3/tyro/_parsers.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.2/tyro/_resolver.py` & `tyro-0.5.3/tyro/_resolver.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.2/tyro/_strings.py` & `tyro-0.5.3/tyro/_strings.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.2/tyro/_subcommand_matching.py` & `tyro-0.5.3/tyro/_subcommand_matching.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.2/tyro/_typing.py` & `tyro-0.5.3/tyro/_typing.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.2/tyro/_unsafe_cache.py` & `tyro-0.5.3/tyro/_unsafe_cache.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.2/tyro/conf/__init__.py` & `tyro-0.5.3/tyro/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.2/tyro/conf/_confstruct.py` & `tyro-0.5.3/tyro/conf/_confstruct.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.2/tyro/conf/_markers.py` & `tyro-0.5.3/tyro/conf/_markers.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,26 +74,27 @@
 ```
 
 This is more robust to reordering of options, ensuring that any new options can simply
 be placed at the end of the command>
 """
 
 OmitSubcommandPrefixes = Annotated[T, None]
-"""Make flags used for keyword arguments in subcommands shorter by omitting prefixes.
+"""Make flags used for keyword arguments in subcommands shorter by omitting the
+subcommand-specific portion of the prefix.
 
 If we have a structure with the field:
 
     cmd: Union[NestedTypeA, NestedTypeB]
 
 By default, `--cmd.arg` may be generated as a flag for each dataclass in the union.
 If subcommand prefixes are omitted, we would instead simply have `--arg`.
 """
 
 OmitArgPrefixes = Annotated[T, None]
-"""Make flags used for keyword arguments in arguments shorter by omitting prefixes.
+"""Make flags used for keyword arguments shorter by omitting prefixes.
 
 If we have a structure with the field:
 
     cmd: NestedType
 
 By default, `--cmd.arg` may be generated as a flag. If prefixes are omitted, we would
 instead simply have `--arg`.
```

### Comparing `tyro-0.5.2/tyro/extras/__init__.py` & `tyro-0.5.3/tyro/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.2/tyro/extras/_base_configs.py` & `tyro-0.5.3/tyro/extras/_base_configs.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,35 +36,40 @@
         Annotated[
             Config,
             tyro.conf.subcommand("big", default=Config(...))
         ]
     ]
     ```
 
-    Direct use of `typing.Union` and `tyro.conf.subcommand()` should generally be
-    preferred, but this function can be helpful for succinictness.
-
+    Direct use of `typing.Union` and :func:`tyro.conf.subcommand()` should generally be
+    preferred, but this function can be helpful for succinctness.
 
     .. warning::
-
         The type returned by this function can be safely used as an input to
-        `tyro.cli()`, but for static analysis when used for annotations we recommend
-        applying a TYPE_CHECKING guard:
+        :func:`tyro.cli()`, but for static analysis when used for annotations we
+        recommend applying a `TYPE_CHECKING` guard:
 
         .. code-block:: python
 
             from typing import TYPE_CHECKING
 
             if TYPE_CHECKING:
                 # Static type seen by language servers, type checkers, etc.
                 SelectableConfig = Config
             else:
                 # Runtime type used by tyro.
                 SelectableConfig = subcommand_type_from_defaults(...)
 
+    Args:
+        defaults: A dictionary of default subcommand instances.
+        descriptions: A dictionary conttaining descriptions for helptext.
+        prefix_names: Whether to prefix subcommand names.
+
+    Returns:
+        A subcommand type, which can be passed to :func:`tyro.cli`.
     """
     return Union.__getitem__(  # type: ignore
         tuple(
             Annotated.__class_getitem__(  # type: ignore
                 (
                     type(v),
                     subcommand(
```

### Comparing `tyro-0.5.2/tyro/extras/_choices_type.py` & `tyro-0.5.3/tyro/extras/_choices_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,26 +10,30 @@
 
 def literal_type_from_choices(choices: Iterable[T]) -> TypeForm[T]:
     """Generate a `typing.Literal[]` type that constrains values to a set of choices.
 
     Using `Literal[...]` directly should generally be preferred, but this function can be
     helpful when choices are generated dynamically.
 
-
     .. warning::
-
         The type returned by this function can be safely used as an input to
-        `tyro.cli()`, but for static analysis when used for annotations we recommend
-        applying a TYPE_CHECKING guard:
+        :func:`tyro.cli()`, but for static analysis when used for annotations we
+        recommend applying a `TYPE_CHECKING` guard:
 
         .. code-block:: python
 
             from typing import TYPE_CHECKING
 
             if TYPE_CHECKING:
                 # Static type seen by language servers, type checkers, etc.
                 Color = str
             else:
                 # Runtime type used by tyro.
                 Color = literal_type_from_choices(["red", "green", "blue"])
+
+    Args:
+        choices: Options to choose from.
+
+    Returns:
+        A type that can be passed to :func:`tyro.cli()`.
     """
     return Literal.__getitem__(tuple(choices))  # type: ignore
```

### Comparing `tyro-0.5.2/tyro/extras/_serialization.py` & `tyro-0.5.3/tyro/extras/_serialization.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.2/PKG-INFO` & `tyro-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tyro
-Version: 0.5.2
+Version: 0.5.3
 Summary: Strongly typed, zero-effort CLI interfaces
 Home-page: https://github.com/brentyi/tyro
 Author: brentyi
 Author-email: brentyi@berkeley.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

