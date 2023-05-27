# Comparing `tmp/plum_dispatch-2.0.1.tar.gz` & `tmp/plum_dispatch-2.1.0.tar.gz`

## Comparing `plum_dispatch-2.0.1.tar` & `plum_dispatch-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 plum_dispatch-2.0.1/plum/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 plum_dispatch-2.0.1/plum/_version.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 plum_dispatch-2.0.1/plum/alias.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 plum_dispatch-2.0.1/plum/autoreload.py
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 plum_dispatch-2.0.1/plum/dispatcher.py
--rw-r--r--   0        0        0    14852 2020-02-02 00:00:00.000000 plum_dispatch-2.0.1/plum/function.py
--rw-r--r--   0        0        0    12609 2020-02-02 00:00:00.000000 plum_dispatch-2.0.1/plum/parametric.py
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 plum_dispatch-2.0.1/plum/promotion.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 plum_dispatch-2.0.1/plum/resolver.py
--rw-r--r--   0        0        0     9805 2020-02-02 00:00:00.000000 plum_dispatch-2.0.1/plum/signature.py
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 plum_dispatch-2.0.1/plum/type.py
--rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 plum_dispatch-2.0.1/plum/util.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 plum_dispatch-2.0.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 plum_dispatch-2.0.1/LICENCE.txt
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 plum_dispatch-2.0.1/README.md
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 plum_dispatch-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 plum_dispatch-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/_version.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/alias.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/autoreload.py
+-rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/dispatcher.py
+-rw-r--r--   0        0        0    15920 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/function.py
+-rw-r--r--   0        0        0    12609 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/parametric.py
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/promotion.py
+-rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/resolver.py
+-rw-r--r--   0        0        0     9805 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/signature.py
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/type.py
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/util.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/LICENCE.txt
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/README.md
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/PKG-INFO
```

### Comparing `plum_dispatch-2.0.1/plum/__init__.py` & `plum_dispatch-2.1.0/plum/__init__.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.0.1/plum/alias.py` & `plum_dispatch-2.1.0/plum/alias.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.0.1/plum/autoreload.py` & `plum_dispatch-2.1.0/plum/autoreload.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         _update_instances_original = autoreload.update_instances
 
     # Then, override :func:`update_instance`.
     autoreload.update_instances = _update_instances
 
 
 def deactivate_autoreload():
-    """Disable Plum's autoreload hack. This undoes that
+    """Disable Plum's autoreload hack. This undoes what
     :func:`.autoreload.activate_autoreload` did."""
     global _update_instances_original
     if _update_instances_original is None:
         raise RuntimeError("Plum Autoreload module was never activated.")
 
     from IPython.extensions import autoreload
```

### Comparing `plum_dispatch-2.0.1/plum/dispatcher.py` & `plum_dispatch-2.1.0/plum/dispatcher.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.0.1/plum/function.py` & `plum_dispatch-2.1.0/plum/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import textwrap
 from functools import wraps
 from types import MethodType
 from typing import Any
 
 from .resolver import AmbiguousLookupError, NotFoundLookupError, Resolver
 from .signature import Signature, append_default_args, extract_signature
 from .type import resolve_type_hint
@@ -51,31 +52,44 @@
 
 
 _owner_transfer = {}
 """dict[type, type]: When the keys of this dictionary are detected as the owner of
 a function (see :meth:`Function.owner`), make the corresponding value the owner."""
 
 
-class Function:
+class _FunctionMeta(type):
+    """:class:`Function` implements `__doc__`, which overrides the docstring of the
+    class. This simple metaclass ensures that `Function.__doc__` still prints as the
+    docstring of the class."""
+
+    @property
+    def __doc__(self):
+        return self._class_doc
+
+
+class Function(metaclass=_FunctionMeta):
     """A function.
 
     Args:
         f (function): Function that is wrapped.
         owner (str, optional): Name of the class that owns the function.
     """
 
+    # When we set `__doc__`, we will lose the docstring of the class, so we save it now.
+    # Correctly printing the docstring is handled by :class:`_FunctionMeta`.
+    _class_doc = __doc__
+
     _instances = []
 
     def __init__(self, f, owner=None):
         Function._instances.append(self)
 
         self._f = f
-        self._doc = ""
-        wraps(f)(self)  # This will correctly populate `self._doc`.
         self._cache = {}
+        wraps(f)(self)  # Sets `self._doc`.
 
         # `owner` is the name of the owner. We will later attempt to resolve to
         # which class it actually points.
         self._owner_name = owner
         self._owner = None
 
         # Initialise pending and resolved methods.
@@ -95,29 +109,41 @@
                 self._owner = _owner_transfer[self._owner]
         return self._owner
 
     @property
     def __doc__(self):
         """str or None: Documentation of the function. This consists of the
         documentation of the function given at initialisation with the documentation
-        of all other registered methods appended."""
+        of all other registered methods appended.
+
+        Upon instantiation, this property is available through `obj.__doc__`.
+        """
         self._resolve_pending_registrations()
 
-        # Derive the basis of the docstring from `self._f`.
-        doc = self._doc
+        # Derive the basis of the docstring from `self._f`, removing any indentation.
+        doc = self._doc.strip()
+        if doc:
+            # Do not include the first line when removing the indentation.
+            lines = doc.splitlines()
+            doc = lines[0]
+            # There might not be more than one line.
+            if len(lines) > 1:
+                doc += "\n" + textwrap.dedent("\n".join(lines[1:]))
 
         # Append the docstrings of all other implementations to it. Exclude the
-        # docstring from `self._f`, because that one forms the basis.
+        # docstring from `self._f`, because that one forms the basis (see boave).
         resolver_doc = self._resolver.doc(exclude=self._f)
         if resolver_doc:
-            # Ensure a newline.
-            while doc[-2:] != "\n\n":
-                doc += "\n"
-            doc += "This function has further implementations documented below.\n\n"
+            # Add a newline if the documentation is non-empty.
+            if doc:
+                doc = doc + "\n\n"
             doc += resolver_doc
+            # Replace separators with horizontal lines of the right length.
+            separator_length = max(map(len, doc.splitlines()))
+            doc = doc.replace("<separator>", "-" * separator_length)
 
         # If the docstring is empty, return `None`, which is consistent with omitting
         # the docstring.
         return doc if doc else None
 
     @__doc__.setter
     def __doc__(self, value):
```

### Comparing `plum_dispatch-2.0.1/plum/parametric.py` & `plum_dispatch-2.1.0/plum/parametric.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.0.1/plum/promotion.py` & `plum_dispatch-2.1.0/plum/promotion.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.0.1/plum/resolver.py` & `plum_dispatch-2.1.0/plum/resolver.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,64 @@
 import pydoc
+import sys
 
 __all__ = ["AmbiguousLookupError", "NotFoundLookupError"]
 
 
 class AmbiguousLookupError(LookupError):
     """A signature cannot be resolved due to ambiguity."""
 
 
 class NotFoundLookupError(LookupError):
     """A signature cannot be resolved because no applicable method can be found."""
 
 
+def _document(f):
+    """Generate documentation for a function `f`.
+
+    The generated documentation contains both the function definition and the
+    docstring. The docstring is on the same level of indentation of the function
+    definition. There will be no trailing newlines.
+
+    If the package :mod:`sphinx` is not imported, then the function definition will
+    be preceded by the string `<separator>`.
+
+    If the package :mod:`sphinx` is imported, then the function definition will include
+    a Sphinx directive to displays the function definition in a nice way.
+
+    Args:
+        f (function): Function.
+
+    Returns:
+        str: Documentation for `f`.
+    """
+    # :class:`pydoc._PlainTextDoc` removes styling. This styling will display
+    # erroneously in Sphinx.
+    parts = pydoc._PlainTextDoc().document(f).rstrip().split("\n")
+
+    # Separate out the function definition and the lines corresponding to the body.
+    title = parts[0]
+    body = parts[1:]
+
+    # Remove indentation from every line of the body. This indentation defaults to
+    # four spaces.
+    body = [line[4:] for line in body]
+
+    # If `sphinx` is imported, assume that we're building the documentation. In that
+    # case, display the function definition in a nice way.
+    if "sphinx" in sys.modules:
+        title = ".. py:function:: " + title + "\n   :noindex:"
+    else:
+        title = "<separator>\n\n" + title
+    title += "\n"  # Add a newline to separate the title from the body.
+
+    # Ensure that there are no trailing newlines. This can happen if the body is empty.
+    return "\n".join([title] + body).rstrip()
+
+
 class Resolver:
     """Method resolver.
 
     Attributes:
         signatures (list[:class:`.signature.Signature`]): Registered signatures.
         is_faithful (bool): Whether all signatures are faithful or not.
     """
@@ -32,26 +76,28 @@
                 concatenation.
 
         Returns:
             str: Concatenation of all docstrings.
         """
         # Generate all docstrings, possibly excluding `exclude`.
         docs = [
-            pydoc.TextDoc().document(sig.implementation)
+            _document(sig.implementation)
             for sig in self.signatures
             if not (exclude and sig.implementation == exclude)
         ]
         # This can yield duplicates, because of extra methods automatically generated by
         # :func:`.signature.append_default_args`. We remove these by simply only
         # keeping unique docstrings.
         unique_docs = []
         for d in docs:
             if d not in unique_docs:
                 unique_docs.append(d)
-        return "\n".join(unique_docs)
+        # The unique documentations have no trailing newlines, so separate them with
+        # a newline.
+        return "\n\n".join(unique_docs)
 
     def register(self, signature):
         """Register a new signature.
 
         Args:
             signature (:class:`.signature.Signature`): Signature to add.
         """
```

### Comparing `plum_dispatch-2.0.1/plum/signature.py` & `plum_dispatch-2.1.0/plum/signature.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.0.1/plum/type.py` & `plum_dispatch-2.1.0/plum/type.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.0.1/plum/util.py` & `plum_dispatch-2.1.0/plum/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 Args:
     x (type hint): Type hint.
 
 Returns:
     type hint: Unsubcripted version of `x`.
 """
 
-get_args.__doc__ = """Get the arguments a subscripted type hint.
+get_args.__doc__ = """Get the arguments of a subscripted type hint.
 
 Args:
     x (type hint): Type hint.
 
 Returns:
     tuple: Arguments of `x`.
 """
```

### Comparing `plum_dispatch-2.0.1/LICENCE.txt` & `plum_dispatch-2.1.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.0.1/README.md` & `plum_dispatch-2.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,35 @@
-# [Plum: Multiple Dispatch in Python](https://github.com/wesselb/plum)
+# [Plum: Multiple Dispatch in Python](https://github.com/beartype/plum)
 
 [![DOI](https://zenodo.org/badge/110279931.svg)](https://zenodo.org/badge/latestdoi/110279931)
-[![CI](https://github.com/wesselb/plum/workflows/CI/badge.svg?branch=master)](https://github.com/beartype/plum/actions?query=workflow%3ACI)
-[![Coverage Status](https://coveralls.io/repos/github/wesselb/plum/badge.svg?branch=master&service=github)](https://coveralls.io/github/wesselb/plum?branch=master)
+[![CI](https://github.com/beartype/plum/workflows/CI/badge.svg?branch=master)](https://github.com/beartype/plum/actions?query=workflow%3ACI)
+[![Coverage Status](https://coveralls.io/repos/github/beartype/plum/badge.svg?branch=master&service=github)](https://coveralls.io/github/beartype/plum?branch=master)
 [![Latest Docs](https://img.shields.io/badge/docs-latest-blue.svg)](https://beartype.github.io/plum)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Everybody likes multiple dispatch, just like everybody likes plums.
 
+The design philosophy of Plum is to provide an implementation of multiple dispatch that is Pythonic, yet close to how [Julia](http://julia-lang.org/) does it.
+[See here for a comparison between Plum, `multipledispatch`, and `multimethod`.](https://beartype.github.io/plum/comparison.html)
+
 *Note:*
 Plum 2 is now powered by [Beartype](https://github.com/beartype/beartype)!
 If you notice any issues with the new release, please open an issue.
 
 # Installation
 
 Plum requires Python 3.7 or higher.
 
 ```bash
 pip install plum-dispatch
 ```
 
-# [Documentation](https://wesselb.github.io/plum)
+# [Documentation](https://beartype.github.io/plum)
 
-See [here](https://wesselb.github.io/plum).
+See [here](https://beartype.github.io/plum).
 
 # What's This?
 
 Plum brings your type annotations to life:
 
 ```python
 from numbers import Number
```

### Comparing `plum_dispatch-2.0.1/pyproject.toml` & `plum_dispatch-2.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "wheel",
     "build",
     "tox",
     "jupyter-book",
 ]
 
 [project.urls]
- repository = "https://github.com/wesselb/plum"
+repository = "https://github.com/beartype/plum"
 
 [tool.hatch.build]
 include = ["plum*"]
 
 [tool.hatch.version]
 source = "vcs"
```

### Comparing `plum_dispatch-2.0.1/PKG-INFO` & `plum_dispatch-2.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: plum-dispatch
-Version: 2.0.1
+Version: 2.1.0
 Summary: Multiple dispatch in Python
-Project-URL: repository, https://github.com/wesselb/plum
+Project-URL: repository, https://github.com/beartype/plum
 Author-email: Wessel Bruinsma <wessel.p.bruinsma@gmail.com>
 License: MIT
 License-File: LICENCE.txt
 Keywords: multiple dispatch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -22,39 +22,42 @@
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Requires-Dist: tox; extra == 'dev'
 Requires-Dist: wheel; extra == 'dev'
 Description-Content-Type: text/markdown
 
-# [Plum: Multiple Dispatch in Python](https://github.com/wesselb/plum)
+# [Plum: Multiple Dispatch in Python](https://github.com/beartype/plum)
 
 [![DOI](https://zenodo.org/badge/110279931.svg)](https://zenodo.org/badge/latestdoi/110279931)
-[![CI](https://github.com/wesselb/plum/workflows/CI/badge.svg?branch=master)](https://github.com/beartype/plum/actions?query=workflow%3ACI)
-[![Coverage Status](https://coveralls.io/repos/github/wesselb/plum/badge.svg?branch=master&service=github)](https://coveralls.io/github/wesselb/plum?branch=master)
+[![CI](https://github.com/beartype/plum/workflows/CI/badge.svg?branch=master)](https://github.com/beartype/plum/actions?query=workflow%3ACI)
+[![Coverage Status](https://coveralls.io/repos/github/beartype/plum/badge.svg?branch=master&service=github)](https://coveralls.io/github/beartype/plum?branch=master)
 [![Latest Docs](https://img.shields.io/badge/docs-latest-blue.svg)](https://beartype.github.io/plum)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Everybody likes multiple dispatch, just like everybody likes plums.
 
+The design philosophy of Plum is to provide an implementation of multiple dispatch that is Pythonic, yet close to how [Julia](http://julia-lang.org/) does it.
+[See here for a comparison between Plum, `multipledispatch`, and `multimethod`.](https://beartype.github.io/plum/comparison.html)
+
 *Note:*
 Plum 2 is now powered by [Beartype](https://github.com/beartype/beartype)!
 If you notice any issues with the new release, please open an issue.
 
 # Installation
 
 Plum requires Python 3.7 or higher.
 
 ```bash
 pip install plum-dispatch
 ```
 
-# [Documentation](https://wesselb.github.io/plum)
+# [Documentation](https://beartype.github.io/plum)
 
-See [here](https://wesselb.github.io/plum).
+See [here](https://beartype.github.io/plum).
 
 # What's This?
 
 Plum brings your type annotations to life:
 
 ```python
 from numbers import Number
```

