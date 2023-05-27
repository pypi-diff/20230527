# Comparing `tmp/bitstring-4.0.2.tar.gz` & `tmp/bitstring-4.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitstring-4.0.2.tar", last modified: Sun Apr 16 13:50:10 2023, max compression
+gzip compressed data, was "bitstring-4.1.0b1.tar", last modified: Sat May 27 12:59:43 2023, max compression
```

## Comparing `bitstring-4.0.2.tar` & `bitstring-4.1.0b1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 scottg     (501) staff       (20)        0 2023-04-16 13:50:10.654277 bitstring-4.0.2/
--rw-r--r--   0 scottg     (501) staff       (20)     1106 2021-07-17 21:23:45.000000 bitstring-4.0.2/LICENSE
--rw-r--r--   0 scottg     (501) staff       (20)      174 2023-04-16 13:48:24.000000 bitstring-4.0.2/MANIFEST.in
--rw-r--r--   0 scottg     (501) staff       (20)     6263 2023-04-16 13:50:10.653685 bitstring-4.0.2/PKG-INFO
--rw-r--r--   0 scottg     (501) staff       (20)     5507 2023-04-16 13:48:24.000000 bitstring-4.0.2/README.md
-drwxr-xr-x   0 scottg     (501) staff       (20)        0 2023-04-16 13:50:10.640687 bitstring-4.0.2/bitstring/
--rw-r--r--   0 scottg     (501) staff       (20)   200454 2023-04-16 13:48:24.000000 bitstring-4.0.2/bitstring/__init__.py
--rw-r--r--   0 scottg     (501) staff       (20)        0 2023-04-16 13:48:24.000000 bitstring-4.0.2/bitstring/py.typed
-drwxr-xr-x   0 scottg     (501) staff       (20)        0 2023-04-16 13:50:10.643530 bitstring-4.0.2/bitstring.egg-info/
--rw-r--r--   0 scottg     (501) staff       (20)     6263 2023-04-16 13:50:10.000000 bitstring-4.0.2/bitstring.egg-info/PKG-INFO
--rw-r--r--   0 scottg     (501) staff       (20)      430 2023-04-16 13:50:10.000000 bitstring-4.0.2/bitstring.egg-info/SOURCES.txt
--rw-r--r--   0 scottg     (501) staff       (20)        1 2023-04-16 13:50:10.000000 bitstring-4.0.2/bitstring.egg-info/dependency_links.txt
--rw-r--r--   0 scottg     (501) staff       (20)       10 2023-04-16 13:50:10.000000 bitstring-4.0.2/bitstring.egg-info/top_level.txt
--rw-r--r--   0 scottg     (501) staff       (20)      864 2023-04-16 13:48:24.000000 bitstring-4.0.2/pyproject.toml
--rw-r--r--   0 scottg     (501) staff       (20)    58558 2023-04-16 13:48:24.000000 bitstring-4.0.2/release_notes.txt
--rw-r--r--   0 scottg     (501) staff       (20)       38 2023-04-16 13:50:10.654487 bitstring-4.0.2/setup.cfg
-drwxr-xr-x   0 scottg     (501) staff       (20)        0 2023-04-16 13:50:10.652637 bitstring-4.0.2/tests/
--rw-r--r--   0 scottg     (501) staff       (20)        0 2023-04-14 20:44:35.000000 bitstring-4.0.2/tests/__init__.py
--rw-r--r--   0 scottg     (501) staff       (20)        8 2022-11-13 10:43:27.000000 bitstring-4.0.2/tests/smalltestfile
--rw-r--r--   0 scottg     (501) staff       (20)   125300 2022-11-13 10:43:27.000000 bitstring-4.0.2/tests/test.m1v
--rw-r--r--   0 scottg     (501) staff       (20)    24765 2023-04-16 13:48:24.000000 bitstring-4.0.2/tests/test_bitarray.py
--rw-r--r--   0 scottg     (501) staff       (20)    26826 2023-04-16 13:48:24.000000 bitstring-4.0.2/tests/test_bits.py
--rw-r--r--   0 scottg     (501) staff       (20)     1115 2022-11-13 10:43:27.000000 bitstring-4.0.2/tests/test_bitstore.py
--rw-r--r--   0 scottg     (501) staff       (20)   144643 2023-04-16 13:48:24.000000 bitstring-4.0.2/tests/test_bitstream.py
--rw-r--r--   0 scottg     (501) staff       (20)     4501 2023-04-16 13:48:24.000000 bitstring-4.0.2/tests/test_bitstring.py
--rw-r--r--   0 scottg     (501) staff       (20)     6806 2023-04-16 13:48:24.000000 bitstring-4.0.2/tests/test_constbitstream.py
+drwxr-xr-x   0 scottg     (501) staff       (20)        0 2023-05-27 12:59:43.745810 bitstring-4.1.0b1/
+-rw-r--r--   0 scottg     (501) staff       (20)     1106 2021-07-17 21:23:45.000000 bitstring-4.1.0b1/LICENSE
+-rw-r--r--   0 scottg     (501) staff       (20)      174 2023-04-16 13:48:24.000000 bitstring-4.1.0b1/MANIFEST.in
+-rw-r--r--   0 scottg     (501) staff       (20)     7153 2023-05-27 12:59:43.745040 bitstring-4.1.0b1/PKG-INFO
+-rw-r--r--   0 scottg     (501) staff       (20)     6395 2023-05-26 18:06:44.000000 bitstring-4.1.0b1/README.md
+drwxr-xr-x   0 scottg     (501) staff       (20)        0 2023-05-27 12:59:43.728462 bitstring-4.1.0b1/bitstring/
+-rw-r--r--   0 scottg     (501) staff       (20)   178953 2023-05-26 17:31:19.000000 bitstring-4.1.0b1/bitstring/__init__.py
+-rw-r--r--   0 scottg     (501) staff       (20)        0 2023-04-16 13:48:24.000000 bitstring-4.1.0b1/bitstring/py.typed
+drwxr-xr-x   0 scottg     (501) staff       (20)        0 2023-05-27 12:59:43.732718 bitstring-4.1.0b1/bitstring.egg-info/
+-rw-r--r--   0 scottg     (501) staff       (20)     7153 2023-05-27 12:59:43.000000 bitstring-4.1.0b1/bitstring.egg-info/PKG-INFO
+-rw-r--r--   0 scottg     (501) staff       (20)      444 2023-05-27 12:59:43.000000 bitstring-4.1.0b1/bitstring.egg-info/SOURCES.txt
+-rw-r--r--   0 scottg     (501) staff       (20)        1 2023-05-27 12:59:43.000000 bitstring-4.1.0b1/bitstring.egg-info/dependency_links.txt
+-rw-r--r--   0 scottg     (501) staff       (20)       16 2023-05-27 12:59:43.000000 bitstring-4.1.0b1/bitstring.egg-info/requires.txt
+-rw-r--r--   0 scottg     (501) staff       (20)       10 2023-05-27 12:59:43.000000 bitstring-4.1.0b1/bitstring.egg-info/top_level.txt
+-rw-r--r--   0 scottg     (501) staff       (20)      908 2023-04-30 17:41:22.000000 bitstring-4.1.0b1/pyproject.toml
+-rw-r--r--   0 scottg     (501) staff       (20)       38 2023-05-27 12:59:43.746065 bitstring-4.1.0b1/setup.cfg
+drwxr-xr-x   0 scottg     (501) staff       (20)        0 2023-05-27 12:59:43.743946 bitstring-4.1.0b1/tests/
+-rw-r--r--   0 scottg     (501) staff       (20)        0 2023-04-14 20:44:35.000000 bitstring-4.1.0b1/tests/__init__.py
+-rw-r--r--   0 scottg     (501) staff       (20)        8 2022-11-13 10:43:27.000000 bitstring-4.1.0b1/tests/smalltestfile
+-rw-r--r--   0 scottg     (501) staff       (20)   125300 2022-11-13 10:43:27.000000 bitstring-4.1.0b1/tests/test.m1v
+-rw-r--r--   0 scottg     (501) staff       (20)    27901 2023-05-26 17:30:24.000000 bitstring-4.1.0b1/tests/test_bitarray.py
+-rw-r--r--   0 scottg     (501) staff       (20)    26549 2023-05-20 15:39:35.000000 bitstring-4.1.0b1/tests/test_bits.py
+-rw-r--r--   0 scottg     (501) staff       (20)     3121 2023-05-26 15:43:26.000000 bitstring-4.1.0b1/tests/test_bitstore.py
+-rw-r--r--   0 scottg     (501) staff       (20)   143650 2023-05-26 17:49:42.000000 bitstring-4.1.0b1/tests/test_bitstream.py
+-rw-r--r--   0 scottg     (501) staff       (20)     5436 2023-05-26 15:43:26.000000 bitstring-4.1.0b1/tests/test_bitstring.py
+-rw-r--r--   0 scottg     (501) staff       (20)     7232 2023-05-26 17:42:45.000000 bitstring-4.1.0b1/tests/test_constbitstream.py
```

### Comparing `bitstring-4.0.2/LICENSE` & `bitstring-4.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `bitstring-4.0.2/PKG-INFO` & `bitstring-4.1.0b1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitstring
-Version: 4.0.2
+Version: 4.1.0b1
 Summary: Simple construction, analysis and modification of binary data.
 Author-email: Scott Griffiths <dr.scottgriffiths@gmail.com>
 Project-URL: homepage, https://github.com/scott-griffiths/bitstring
 Project-URL: documentation, https://bitstring.readthedocs.io/
 Keywords: binary,bitarray,bitvector
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,39 +19,54 @@
 
 
 ![bitstring](https://raw.githubusercontent.com/scott-griffiths/bitstring/main/doc/bitstring_logo_small.png "bitstring")
 
 **bitstring** is a pure Python module designed to help make
 the creation and analysis of binary data as simple and natural as possible.
 
-It has been maintained since 2006 and now has about 20 million downloads per year.
+It has been maintained since 2006 and now has many millions of downloads per year.
 
 
 You can try out the interactive walkthrough notebook on [binder](https://mybinder.org/v2/gh/scott-griffiths/bitstring/main?labpath=doc%2Fwalkthrough.ipynb), or take a look at the [static version](https://github.com/scott-griffiths/bitstring/blob/main/doc/walkthrough.ipynb).
 
 
 [![CI badge](https://github.com/scott-griffiths/bitstring/actions/workflows/.github/workflows/ci.yml/badge.svg)](https://github.com/scott-griffiths/bitstring/actions/workflows/ci.yml)
 [![Docs](https://img.shields.io/readthedocs/bitstring)](https://bitstring.readthedocs.io/en/latest/)
 [![Downloads](https://img.shields.io/pypi/dm/bitstring?color=blue)](https://pypistats.org/packages/bitstring) &nbsp; &nbsp; 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/scott-griffiths/bitstring/main?labpath=doc%2Fwalkthrough.ipynb)
 
+# \<<< 4.1 beta now available - the _speed_ update \>>>
+
+This version concentrats on what is perhaps bitstring's major weakness - speed.
+It's always been a pure Python module with no dependencies, which has a few advantages, but means it can't compete with C-coded extensions in terms of raw speed of operation.
+
+Version 4.1 of bitstring has been rewritten to use the `bitarray` type from the package of the same name as its underlying data type.
+This lets us keep the API and functionality of bitstring but gains (most of) the speed of bitarray.
+
+The 4.1 beta should be fully functional - there are no known issues.
+To install the beta you need to specify the precise version:
+
+    python -m pip install bitstring==4.1.0b1
+
+Please try it out and report any problems or observations.
+You shouldn't need to change any code - everything should just work the same as version 4.0, just faster.
 
 Overview
 --------
 
 * Create bitstrings from hex, octal, binary, files, formatted strings, bytes, integers and floats of different endiannesses.
 * Powerful binary packing and unpacking functions.
 * Bit-level slicing, joining, searching, replacing and more.
 * Read from and interpret bitstrings as streams of binary data.
 * Rich API - chances are that whatever you want to do there's a simple and elegant way of doing it.
 * Open source software, released under the MIT licence.
 
 
 > **Note** \
-> Version 4.0 of bitstring only supports Python 3.7 and later. \
+> Version 4 of bitstring only supports Python 3.7 and later. \
 > Use bitstring version 3.1 if you're using Python 2.7 or 3.6 or earlier.
 
 
 Documentation
 -------------
 The manual for the bitstring module is available at [Read the Docs](https://bitstring.readthedocs.org).
 It contains a walk-through of all the features and a complete [reference section](https://bitstring.readthedocs.io/en/stable/quick_ref.html).
```

### Comparing `bitstring-4.0.2/README.md` & `bitstring-4.1.0b1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,54 @@
 
 
 ![bitstring](https://raw.githubusercontent.com/scott-griffiths/bitstring/main/doc/bitstring_logo_small.png "bitstring")
 
 **bitstring** is a pure Python module designed to help make
 the creation and analysis of binary data as simple and natural as possible.
 
-It has been maintained since 2006 and now has about 20 million downloads per year.
+It has been maintained since 2006 and now has many millions of downloads per year.
 
 
 You can try out the interactive walkthrough notebook on [binder](https://mybinder.org/v2/gh/scott-griffiths/bitstring/main?labpath=doc%2Fwalkthrough.ipynb), or take a look at the [static version](https://github.com/scott-griffiths/bitstring/blob/main/doc/walkthrough.ipynb).
 
 
 [![CI badge](https://github.com/scott-griffiths/bitstring/actions/workflows/.github/workflows/ci.yml/badge.svg)](https://github.com/scott-griffiths/bitstring/actions/workflows/ci.yml)
 [![Docs](https://img.shields.io/readthedocs/bitstring)](https://bitstring.readthedocs.io/en/latest/)
 [![Downloads](https://img.shields.io/pypi/dm/bitstring?color=blue)](https://pypistats.org/packages/bitstring) &nbsp; &nbsp; 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/scott-griffiths/bitstring/main?labpath=doc%2Fwalkthrough.ipynb)
 
+# \<<< 4.1 beta now available - the _speed_ update \>>>
+
+This version concentrats on what is perhaps bitstring's major weakness - speed.
+It's always been a pure Python module with no dependencies, which has a few advantages, but means it can't compete with C-coded extensions in terms of raw speed of operation.
+
+Version 4.1 of bitstring has been rewritten to use the `bitarray` type from the package of the same name as its underlying data type.
+This lets us keep the API and functionality of bitstring but gains (most of) the speed of bitarray.
+
+The 4.1 beta should be fully functional - there are no known issues.
+To install the beta you need to specify the precise version:
+
+    python -m pip install bitstring==4.1.0b1
+
+Please try it out and report any problems or observations.
+You shouldn't need to change any code - everything should just work the same as version 4.0, just faster.
 
 Overview
 --------
 
 * Create bitstrings from hex, octal, binary, files, formatted strings, bytes, integers and floats of different endiannesses.
 * Powerful binary packing and unpacking functions.
 * Bit-level slicing, joining, searching, replacing and more.
 * Read from and interpret bitstrings as streams of binary data.
 * Rich API - chances are that whatever you want to do there's a simple and elegant way of doing it.
 * Open source software, released under the MIT licence.
 
 
 > **Note** \
-> Version 4.0 of bitstring only supports Python 3.7 and later. \
+> Version 4 of bitstring only supports Python 3.7 and later. \
 > Use bitstring version 3.1 if you're using Python 2.7 or 3.6 or earlier.
 
 
 Documentation
 -------------
 The manual for the bitstring module is available at [Read the Docs](https://bitstring.readthedocs.org).
 It contains a walk-through of all the features and a complete [reference section](https://bitstring.readthedocs.io/en/stable/quick_ref.html).
```

### Comparing `bitstring-4.0.2/bitstring/__init__.py` & `bitstring-4.1.0b1/bitstring/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,45 +51,46 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
-__version__ = "4.0.2"
+__version__ = "4.1.0b1"
 
 __author__ = "Scott Griffiths"
 
 import copy
 import pathlib
 import sys
 import re
 import mmap
-import os
 import struct
-import operator
 import array
 import io
 from collections import abc
 import functools
 import types
-from typing import Generator, Sequence, Tuple, Union, List, Iterable, Any, Optional, Iterator, Pattern, Dict,\
+from typing import Generator, Tuple, Union, List, Iterable, Any, Optional, Pattern, Dict,\
     BinaryIO, TextIO, Callable, overload
-from contextlib import suppress
-
+import bitarray
+import bitarray.util
 
 # Things that can be converted to Bits when a Bits type is needed
-BitsType = Union['Bits', int, float, str, Iterable[Any], bool, BinaryIO, bytearray, bytes]
+BitsType = Union['Bits', int, float, str, Iterable[Any], bool, BinaryIO, bytearray, bytes, bitarray.bitarray]
 
 byteorder: str = sys.byteorder
 
 # An opaque way of adding module level properties. Taken from https://peps.python.org/pep-0549/
 _bytealigned: bool = False
 _lsb0: bool = False
 
+# The size of various caches used to improve performance
+CACHE_SIZE = 256
+
 
 class _MyModuleType(types.ModuleType):
     @property
     def bytealigned(self):
         """Determines whether a number of methods default to working only on byte boundaries."""
         return globals()['_bytealigned']
 
@@ -112,450 +113,198 @@
 
 
 sys.modules[__name__].__class__ = _MyModuleType
 
 # Maximum number of digits to use in __str__ and __repr__.
 MAX_CHARS: int = 250
 
-# Maximum size of caches used for speed optimisations.
-CACHE_SIZE: int = 1000
-
 
 class Error(Exception):
     """Base class for errors in the bitstring module."""
 
     def __init__(self, *params: object):
         self.msg = params[0] if params else ''
         self.params = params[1:]
 
 
 class ReadError(Error, IndexError):
     """Reading or peeking past the end of a bitstring."""
 
-    def __init__(self, *params: object):
-        Error.__init__(self, *params)
-
 
 class InterpretError(Error, ValueError):
     """Inappropriate interpretation of binary data."""
 
-    def __init__(self, *params: object):
-        Error.__init__(self, *params)
-
 
 class ByteAlignError(Error):
     """Whole-byte position or length needed."""
 
-    def __init__(self, *params: object):
-        Error.__init__(self, *params)
-
 
 class CreationError(Error, ValueError):
     """Inappropriate argument during bitstring creation."""
 
-    def __init__(self, *params: object):
-        Error.__init__(self, *params)
-
-
-class ByteStore:
-    """Stores raw bytes together with a bit offset and length.
 
-    Used internally - not part of public interface.
-    """
+def _offset_slice_indices_lsb0(key: slice, length: int, offset: int) -> slice:
+    # First convert slice to all integers
+    # Length already should take account of the offset
+    start, stop, step = key.indices(length)
+    new_start = length - stop - offset
+    new_stop = length - start - offset
+    # For negative step we sometimes get a negative stop, which can't be used correctly in a new slice
+    if new_stop < 0:
+        new_stop = None
+    return slice(new_start, new_stop, step)
+
+
+def _offset_slice_indices_msb0(key: slice, length: int, offset: int) -> slice:
+    # First convert slice to all integers
+    # Length already should take account of the offset
+    start, stop, step = key.indices(length)
+    start += offset
+    stop += offset
+    # For negative step we sometimes get a negative stop, which can't be used correctly in a new slice
+    if stop < 0:
+        stop = None
+    return slice(start, stop, step)
+
+
+class BitStore(bitarray.bitarray):
+    """A light wrapper around bitarray that does the LSB0 stuff"""
+
+    __slots__ = ('modified', 'length', 'offset', 'filename', 'immutable')
+
+    def __init__(self, *args, immutable: bool=False, frombytes: Optional[Union[bytes, bytearray]] = None, offset: int = 0, length: Optional[int] = None, filename: Optional[str] = None,
+                 **kwargs) -> None:
+        if frombytes is not None:
+            self.frombytes(frombytes)
+        self.immutable = immutable
+        # Here 'modified' means that it isn't just the underlying bitarray. It could have a different start and end, and be from a file.
+        # This also means that it shouldn't be changed further, so setting deleting etc. are disallowed.
+        self.modified = offset != 0 or length is not None or filename is not None
+        if self.modified:
+            assert immutable is True
+            # These class variable only exist if modified is True.
+            self.offset = offset
+            self.filename = filename
+            self.length = super().__len__() - self.offset if length is None else length
+
+            if self.length < 0:
+                raise CreationError("Can't create bitstring with a negative length.")
+            if self.length + self.offset > super().__len__():
+                self.length = super().__len__() - self.offset
+                raise CreationError(f"Can't create bitstring with a length of {self.length} and an offset of {self.offset} from {super().__len__()} bits of data.")
 
     @classmethod
-    def _setlsb0methods(cls, lsb0: bool) -> None:
+    def _setlsb0methods(cls, lsb0: bool = False):
         if lsb0:
-            cls.getbit = cls._getbit_lsb0  # type: ignore
-            cls.setbit = cls._setbit_lsb0  # type: ignore
-            cls.unsetbit = cls._unsetbit_lsb0  # type: ignore
-            cls.invertbit = cls._invertbit_lsb0  # type: ignore
-            cls.__iter__ = cls._iter_lsb0  # type: ignore
-        else:
-            cls.getbit = cls._getbit_msb0  # type: ignore
-            cls.setbit = cls._setbit_msb0  # type: ignore
-            cls.unsetbit = cls._unsetbit_msb0  # type: ignore
-            cls.invertbit = cls._invertbit_msb0  # type: ignore
-            cls.__iter__ = cls._iter_msb0  # type: ignore
-
-    __slots__ = ('offset', 'rawarray', 'bitlength')
-
-    def __init__(self, data: Union[bytearray, MmapByteArray],
-                 bitlength: Optional[int] = None, offset: int = 0) -> None:
-        self.rawarray = data
-        if bitlength is None:
-            bitlength = 8 * len(data) - offset
-        self.offset = offset
-        self.bitlength = bitlength
-
-    def _iter_lsb0(self) -> Iterator[bool]:
-        # TODO: Rewrite like _iter_msb0
-        # A rather slow but simple version
-        for p in range(0, self.bitlength):
-            yield self._getbit_lsb0(p)
-        return
+            cls.__setitem__ = cls.setitem_lsb0
+            cls.__delitem__ = cls.delitem_lsb0
+            cls.getindex = cls.getindex_lsb0
+            cls.getslice = cls.getslice_lsb0
+        else:
+            cls.__setitem__ = super().__setitem__
+            cls.__delitem__ = super().__delitem__
+            cls.getindex = cls.getindex_msb0
+            cls.getslice = cls.getslice_msb0
+
+    def __new__(cls, *args, **kwargs):
+        # Just pass on the buffer keyword, not the length, offset, filename and frombytes
+        new_kwargs = {'buffer': kwargs.get('buffer', None)}
+        return bitarray.bitarray.__new__(cls, *args, **new_kwargs)
+
+    def __add__(self, other: bitarray.bitarray):
+        assert not self.immutable
+        return BitStore(super().__add__(other))
 
-    def _iter_msb0(self) -> Iterator[bool]:
-        start_byte, start_bit = divmod(self.offset, 8)
-        end_byte, end_bit = divmod(self.offset + self.bitlength, 8)
+    def __iter__(self):
+        for i in range(0, len(self)):
+            yield self.getindex(i)
 
-        try:
-            byte = self.rawarray[start_byte]
-        except IndexError:
-            return  # Empty
-        if start_byte != end_byte:
-            for bit in range(start_bit, 8):
-                yield bool(byte & (128 >> bit))
-            start_bit = 0
-        else:
-            for bit in range(start_bit, end_bit):
-                yield bool(byte & (128 >> bit))
-            return
+    def copy(self):
+        x = BitStore(self.getslice(slice(None, None, None)))
+        return x
 
-        for byte in self.rawarray[start_byte + 1: end_byte]:
-            reversed_int = Bits._int8ReversalDict[byte]
-            for _ in range(0, 8):
-                yield bool(reversed_int & 1)
-                reversed_int >>= 1
-            start_bit = 0
-
-        if end_bit:
-            byte = self.rawarray[end_byte]
-            for bit in range(start_bit, end_bit):
-                yield bool(byte & (128 >> bit))
-
-    def _getbit_lsb0(self, pos: int) -> bool:
-        assert 0 <= pos < self.bitlength
-        pos = self.bitlength - pos - 1
-        byte, bit = divmod(self.offset + pos, 8)
-        return bool(self.rawarray[byte] & (128 >> bit))
-
-    def _getbit_msb0(self, pos: int) -> bool:
-        assert 0 <= pos < self.bitlength
-        byte, bit = divmod(self.offset + pos, 8)
-        return bool(self.rawarray[byte] & (128 >> bit))
-
-    def getbyte(self, pos: int) -> int:
-        """Direct access to byte data."""
-        return self.rawarray[pos]
-
-    def getbyteslice(self, start: int, end: int) -> bytearray:
-        """Direct access to byte data."""
-        return self.rawarray[start:end]
+    def __getitem__(self, item):
+        # Use getindex or getslice instead
+        raise NotImplementedError
 
-    @property
-    def bytelength(self) -> int:
-        if not self.bitlength:
-            return 0
-        sb = self.offset // 8
-        eb = (self.offset + self.bitlength - 1) // 8
-        return eb - sb + 1
-
-    def __copy__(self) -> ByteStore:
-        return ByteStore(self.rawarray[:], self.bitlength, self.offset)
-
-    def appendstore(self, store: ByteStore) -> None:
-        """Join another store on to the end of this one."""
-        if not store.bitlength:
-            return
-        # Set new array offset to the number of bits in the final byte of current array.
-        store = offsetcopy(store, (self.offset + self.bitlength) % 8)
-        if store.offset != 0:
-            # first do the byte with the join.
-            joinval = (self.rawarray.pop() & (255 ^ (255 >> store.offset)) |
-                       (store.getbyte(0) & (255 >> store.offset)))
-            self.rawarray.append(joinval)
-            self.rawarray.extend(store.rawarray[1:])
+    def getindex_msb0(self, index):
+        if self.modified and index >= 0:
+            index += self.offset
+        return super().__getitem__(index)
+
+    def getslice_msb0(self, key):
+        if self.modified:
+            key = _offset_slice_indices_msb0(key, len(self), self.offset)
+        return BitStore(super().__getitem__(key))
+
+    def getindex_lsb0(self, index):
+        if self.modified and index >= 0:
+            index += self.offset
+        return super().__getitem__(-index - 1)
+
+    def getslice_lsb0(self, key):
+        if self.modified:
+            key = _offset_slice_indices_lsb0(key, len(self), self.offset)
+        else:
+            key = _offset_slice_indices_lsb0(key, len(self), 0)
+        return BitStore(super().__getitem__(key))
+
+    def setitem_lsb0(self, key, value):
+        assert not self.immutable
+        if isinstance(key, int):
+            super().__setitem__(-key - 1, value)
+        else:
+            new_slice = _offset_slice_indices_lsb0(key, len(self), 0)
+            super().__setitem__(new_slice, value)
+
+    def delitem_lsb0(self, key):
+        assert not self.immutable
+        if isinstance(key, int):
+            super().__delitem__(-key - 1)
+        else:
+            new_slice = _offset_slice_indices_lsb0(key, len(self), 0)
+            super().__delitem__(new_slice)
+
+    def invert(self, index=None):
+        assert not self.immutable
+        if index is not None:
+            if _lsb0:
+                super().invert(-index - 1)
+            else:
+                super().invert(index)
         else:
-            self.rawarray.extend(store.rawarray)
-        self.bitlength += store.bitlength
+            super().invert()
 
-    def prependstore(self, store: ByteStore) -> None:
-        """Join another store on to the start of this one."""
-        if not store.bitlength:
-            return
-            # Set the offset of copy of store so that it's final byte
-        # ends in a position that matches the offset of self,
-        # then join self on to the end of it.
-        store = offsetcopy(store, (self.offset - store.bitlength) % 8)
-        assert (store.offset + store.bitlength) % 8 == self.offset % 8
-        bit_offset = self.offset % 8
-        if bit_offset:
-            # first do the byte with the join.
-            joinval = (store.getbyte(-1) & (255 ^ (255 >> bit_offset)) | 
-                       (self.rawarray[self.byteoffset] & (255 >> bit_offset)))
-            store.rawarray[-1] = joinval
-            store.rawarray.extend(self.rawarray[self.byteoffset + 1: self.byteoffset + self.bytelength])
+    def any_set(self) -> bool:
+        if self.modified:
+            return super().__getitem__(slice(self.offset, self.offset + self.length, None)).any()
         else:
-            store.rawarray.extend(self.rawarray[self.byteoffset: self.byteoffset + self.bytelength])
-        self.rawarray = store.rawarray
-        self.offset = store.offset
-        self.bitlength += store.bitlength
-
-    def _setbit_lsb0(self, pos: int) -> None:
-        assert 0 <= pos < self.bitlength
-        pos = self.bitlength - pos - 1
-        byte, bit = divmod(self.offset + pos, 8)
-        self.rawarray[byte] |= (128 >> bit)
-
-    def _setbit_msb0(self, pos: int) -> None:
-        assert 0 <= pos < self.bitlength
-        byte, bit = divmod(self.offset + pos, 8)
-        self.rawarray[byte] |= (128 >> bit)
-
-    def _unsetbit_lsb0(self, pos: int) -> None:
-        assert 0 <= pos < self.bitlength
-        pos = self.bitlength - pos - 1
-        byte, bit = divmod(self.offset + pos, 8)
-        self.rawarray[byte] &= ~(128 >> bit)
-
-    def _unsetbit_msb0(self, pos: int) -> None:
-        assert 0 <= pos < self.bitlength
-        byte, bit = divmod(self.offset + pos, 8)
-        self.rawarray[byte] &= ~(128 >> bit)
-
-    def _invertbit_lsb0(self, pos: int) -> None:
-        assert 0 <= pos < self.bitlength
-        pos = self.bitlength - pos - 1
-        byte, bit = divmod(self.offset + pos, 8)
-        self.rawarray[byte] ^= (128 >> bit)
-
-    def _invertbit_msb0(self, pos: int) -> None:
-        assert 0 <= pos < self.bitlength
-        byte, bit = divmod(self.offset + pos, 8)
-        self.rawarray[byte] ^= (128 >> bit)
-
-    def setbyte(self, pos: int, value: int) -> None:
-        self.rawarray[pos] = value
-
-    def setbyteslice(self, start: int, end: int, value: bytearray) -> None:
-        self.rawarray[start:end] = value
-
-    @property
-    def byteoffset(self) -> int:
-        return self.offset // 8
-
-    @property
-    def rawbytes(self) -> Union[bytearray, MmapByteArray]:
-        return self.rawarray
-
-
-def offsetcopy(s: ByteStore, newoffset: int) -> ByteStore:
-    """Return a copy of a ByteStore with the newoffset.
-
-    Not part of public interface.
-    """
-    assert 0 <= newoffset < 8
-    if s.bitlength == 0:
-        return copy.copy(s)
-    if newoffset == s.offset % 8:
-        return type(s)(s.getbyteslice(s.byteoffset, s.byteoffset + s.bytelength), s.bitlength, newoffset)
-
-    if isinstance(s.rawarray, MmapByteArray):
-        # Need to make a copy in memory first
-        v = int.from_bytes(s.rawarray[:], 'big')
-    else:
-        v = int.from_bytes(s.rawarray, 'big')
-    if newoffset < s.offset % 8:
-        # We need to shift everything left
-        shiftleft = s.offset % 8 - newoffset
-        v <<= shiftleft
-        v &= (1 << 8 * len(s.rawarray)) - 1
-        newdata = v.to_bytes(len(s.rawarray), 'big')
-    else:
-        # Shifting right, but we use a left shift as we don't want to lose any data
-        shiftleft = 8 - newoffset + s.offset % 8
-        v <<= shiftleft
-        newdata = v.to_bytes(len(s.rawarray) + 1, 'big')
-
-    bits_remaining_in_last_byte = (s.offset + s.bitlength) % 8
-    if bits_remaining_in_last_byte == 0:
-        bits_remaining_in_last_byte = 8
-    bits_remaining_in_last_byte -= shiftleft
-    if bits_remaining_in_last_byte <= 0 and len(newdata) > 1:
-        newdata = newdata[:-1]
-
-    new_s = type(s)(bytearray(newdata), s.bitlength, newoffset)
-    return new_s
-
+            return super().any()
 
-def equal(a: ByteStore, b: ByteStore) -> bool:
-    """Return True if ByteStores a == b.
-
-    Not part of public interface.
-    """
-    # We want to return False for inequality as soon as possible, which
-    # means we get lots of special cases.
-    # First the easy one - compare lengths:
-    a_bitlength = a.bitlength
-    b_bitlength = b.bitlength
-    if a_bitlength != b_bitlength:
-        return False
-    if not a_bitlength:
-        assert b_bitlength == 0
-        return True
-    # Make 'a' the one with the smaller offset
-    if (a.offset % 8) > (b.offset % 8):
-        a, b = b, a
-    # and create some aliases
-    a_bitoff = a.offset % 8
-    b_bitoff = b.offset % 8
-    a_byteoffset = a.byteoffset
-    b_byteoffset = b.byteoffset
-    a_bytelength = a.bytelength
-    b_bytelength = b.bytelength
-    da = a.rawarray
-    db = b.rawarray
-
-    # If they are pointing to the same data, they must be equal
-    if da is db and a.offset == b.offset:
-        return True
-
-    if a_bitoff == b_bitoff:
-        bits_spare_in_last_byte = 8 - (a_bitoff + a_bitlength) % 8
-        if bits_spare_in_last_byte == 8:
-            bits_spare_in_last_byte = 0
-        # Special case for a, b contained in a single byte
-        if a_bytelength == 1:
-            a_val = ((da[a_byteoffset] << a_bitoff) & 0xff) >> (8 - a_bitlength)
-            b_val = ((db[b_byteoffset] << b_bitoff) & 0xff) >> (8 - b_bitlength)
-            return a_val == b_val
-        # Otherwise check first byte
-        if da[a_byteoffset] & (0xff >> a_bitoff) != db[b_byteoffset] & (0xff >> b_bitoff):
-            return False
-        # then everything up to the last
-        b_a_offset = b_byteoffset - a_byteoffset
-        for x in range(1 + a_byteoffset, a_byteoffset + a_bytelength - 1):
-            if da[x] != db[b_a_offset + x]:
-                return False
-        # and finally the last byte
-        return (da[a_byteoffset + a_bytelength - 1] >> bits_spare_in_last_byte ==
-                db[b_byteoffset + b_bytelength - 1] >> bits_spare_in_last_byte)
-
-    assert a_bitoff != b_bitoff
-    # This is how much we need to shift a to the right to compare with b:
-    shift = b_bitoff - a_bitoff
-    # Special case for b only one byte long
-    if b_bytelength == 1:
-        assert a_bytelength == 1
-        a_val = ((da[a_byteoffset] << a_bitoff) & 0xff) >> (8 - a_bitlength)
-        b_val = ((db[b_byteoffset] << b_bitoff) & 0xff) >> (8 - b_bitlength)
-        return a_val == b_val
-    # Special case for a only one byte long
-    if a_bytelength == 1:
-        assert b_bytelength == 2
-        a_val = ((da[a_byteoffset] << a_bitoff) & 0xff) >> (8 - a_bitlength)
-        b_val = ((db[b_byteoffset] << 8) + db[b_byteoffset + 1]) << b_bitoff
-        b_val &= 0xffff
-        b_val >>= 16 - b_bitlength
-        return a_val == b_val
-
-    # Compare first byte of b with bits from first byte of a
-    if (da[a_byteoffset] & (0xff >> a_bitoff)) >> shift != db[b_byteoffset] & (0xff >> b_bitoff):
-        return False
-    # Now compare every full byte of b with bits from 2 bytes of a
-    for x in range(1, b_bytelength - 1):
-        # Construct byte from 2 bytes in a to compare to byte in b
-        b_val = db[b_byteoffset + x]
-        a_val = ((da[a_byteoffset + x - 1] << 8) + da[a_byteoffset + x]) >> shift
-        a_val &= 0xff
-        if a_val != b_val:
-            return False
-
-    # Now check bits in final byte of b
-    final_b_bits = (b.offset + b_bitlength) % 8
-    if not final_b_bits:
-        final_b_bits = 8
-    b_val = db[b_byteoffset + b_bytelength - 1] >> (8 - final_b_bits)
-    final_a_bits = (a.offset + a_bitlength) % 8
-    if not final_a_bits:
-        final_a_bits = 8
-    if b.bytelength > a_bytelength:
-        assert b_bytelength == a_bytelength + 1
-        a_val = da[a_byteoffset + a_bytelength - 1] >> (8 - final_a_bits)
-        a_val &= 0xff >> (8 - final_b_bits)
-        return a_val == b_val
-    assert a_bytelength == b_bytelength
-    a_val = da[a_byteoffset + a_bytelength - 2] << 8
-    a_val += da[a_byteoffset + a_bytelength - 1]
-    a_val >>= (8 - final_a_bits)
-    a_val &= 0xff >> (8 - final_b_bits)
-    return a_val == b_val
-
-
-class MmapByteArray:
-    """Looks like a bytearray, but from an mmap.
-
-    Not part of public interface.
-    """
-
-    __slots__ = ('filemap', 'filelength', 'source', 'byteoffset', 'bytelength')
-
-    def __init__(self, source: Union[BinaryIO, io.BufferedReader], bytelength: Optional[int] = None,
-                 byteoffset: Optional[int] = None) -> None:
-        self.source = source
-        source.seek(0, os.SEEK_END)
-        self.filelength = source.tell()
-        if byteoffset is None:
-            byteoffset = 0
-        if bytelength is None:
-            bytelength = self.filelength - byteoffset
-        self.byteoffset = byteoffset
-        self.bytelength = bytelength
-        self.filemap = mmap.mmap(source.fileno(), 0, access=mmap.ACCESS_READ)
-
-    @overload
-    def __getitem__(self, key: slice) -> bytearray: ...
-    @overload
-    def __getitem__(self, key: int) -> int: ...
-
-    def __getitem__(self, key: Union[slice, int]) -> Union[bytearray, int]:
-        if isinstance(key, slice):
-            start = key.start
-            stop = key.stop
-            if start is None:
-                start = 0
-            if stop is None:
-                stop = self.bytelength
-            assert key.step is None
-            assert 0 <= start < self.bytelength
-            assert 0 <= stop <= self.bytelength
-            s = slice(start + self.byteoffset, stop + self.byteoffset)
-            return bytearray(self.filemap.__getitem__(s))
+    def all_set(self) -> bool:
+        if self.modified:
+            return super().__getitem__(slice(self.offset, self.offset + self.length, None)).all()
         else:
-            return self.filemap[key + self.byteoffset]
-
-    def __len__(self) -> int:
-        return self.bytelength
-
-    # These methods shouldn't ever get called
-    def pop(self, __index: int = ...) -> int:
-        raise NotImplementedError
-    
-    def append(self, __item: Union[Sequence, int]) -> None:
-        raise NotImplementedError
+            return super().all()
 
-    def extend(self, __iterable_of_ints: Union[Iterable[Sequence], bytearray]) -> None:
-        raise NotImplementedError
-
-    def __iter__(self):
-        raise NotImplementedError
-    
-    def __setitem__(self, key: Union[slice, int], value: Any) -> None:
-        raise NotImplementedError
+    def __len__(self):
+        if self.modified:
+            return self.length
+        return super().__len__()
 
 
 def tidy_input_string(s: str) -> str:
     """Return string made lowercase and with all whitespace and underscores removed."""
     return ''.join(s.split()).lower().replace('_', '')
 
 
 INIT_NAMES: List[str] = ['uint', 'int', 'ue', 'se', 'sie', 'uie', 'hex', 'oct', 'bin', 'bits',
                          'uintbe', 'intbe', 'uintle', 'intle', 'uintne', 'intne',
-                         'float', 'floatbe', 'floatle', 'floatne', 'bfloat', 'bytes', 'bool', 'pad']
+                         'float', 'floatbe', 'floatle', 'floatne', 'bfloatbe', 'bfloatle', 'bfloatne', 'bfloat',
+                         'bytes', 'bool', 'pad']
 # Sort longest first as we want to match them in that order (so floatne before float etc.).
 INIT_NAMES.sort(key=len, reverse=True)
 
 TOKEN_RE: Pattern[str] = re.compile(r'^(?P<name>' + '|'.join(INIT_NAMES) +
                                     r'):?(?P<len>[^=]+)?(=(?P<value>.*))?$', re.IGNORECASE)
 # Tokens such as 'u32', 'f64=4.5' or 'i6=-3'
 SHORT_TOKEN_RE: Pattern[str] = re.compile(r'^(?P<name>[uifboh]):?(?P<len>\d+)?(=(?P<value>.*))?$', re.IGNORECASE)
@@ -620,32 +369,29 @@
             tokens = [REPLACEMENTS_LE[c] for c in fmt]
         else:
             assert endian == '>'
             tokens = [REPLACEMENTS_BE[c] for c in fmt]
     return tokens
 
 
-def tokenparser(fmt: str, keys: Optional[Tuple[str, ...]] = None, token_cache: Dict = {}) -> \
+@functools.lru_cache(CACHE_SIZE)
+def tokenparser(fmt: str, keys: Optional[Tuple[str, ...]] = None) -> \
         Tuple[bool, List[Tuple[str, Optional[int], Optional[str]]]]:
     """Divide the format string into tokens and parse them.
 
     Return stretchy token and list of [initialiser, length, value]
     initialiser is one of: hex, oct, bin, uint, int, se, ue, 0x, 0o, 0b etc.
     length is None if not known, as is value.
 
     If the token is in the keyword dictionary (keys) then it counts as a
     special case and isn't messed with.
 
     tokens must be of the form: [factor*][initialiser][:][length][=value]
 
     """
-    try:
-        return token_cache[(fmt, keys)]
-    except KeyError:
-        token_key = (fmt, keys)
     # Very inefficient expanding of brackets.
     fmt = expand_brackets(fmt)
     # Split tokens by ',' and remove whitespace
     # The meta_tokens can either be ordinary single tokens or multiple
     # struct-format token strings.
     meta_tokens = (''.join(f.split()) for f in fmt.split(','))
     return_values = []
@@ -728,19 +474,17 @@
                     if not keys or length not in keys:
                         raise ValueError(f"Don't understand length '{length}' of token.")
             ret_vals.append([name, length, value])
         # This multiplies by the multiplicative factor, but this means that
         # we can't allow keyword values as multipliers (e.g. n*uint:8).
         # The only way to do this would be to return the factor in some fashion
         # (we can't use the key's value here as it would mean that we couldn't
-        # sensibly continue to cache the function's results. (TODO).
-        return_values.extend(ret_vals * factor)
+        # sensibly continue to cache the function's results.
+        return_values.extend(tuple(ret_vals * factor))
     return_values = [tuple(x) for x in return_values]
-    if len(token_cache) < CACHE_SIZE:
-        token_cache[token_key] = stretchy_token, return_values
     return stretchy_token, return_values
 
 
 def expand_brackets(s: str) -> str:
     """Remove whitespace and expand all brackets."""
     s = ''.join(s.split())
     while True:
@@ -770,14 +514,301 @@
                 matchstart = m.start('factor')
                 s = s[0:matchstart] + (factor - 1) * (s[start + 1:p] + ',') + s[start + 1:p] + s[p + 1:]
             else:
                 raise ValueError(f"Failed to parse '{s}'.")
     return s
 
 
+def _str_to_bitstore(s: str, _str_to_bitstore_cache = {}) -> BitStore:
+    try:
+        return _str_to_bitstore_cache[s]
+    except KeyError:
+        try:
+            _, tokens = tokenparser(s)
+        except ValueError as e:
+            raise CreationError(*e.args)
+        bs = BitStore()
+        if tokens:
+            bs = bs + _bitstore_from_token(*tokens[0])
+            for token in tokens[1:]:
+                bs = bs + _bitstore_from_token(*token)
+        bs.immutable = True
+        _str_to_bitstore_cache[s] = bs
+        if len(_str_to_bitstore_cache) > CACHE_SIZE:
+            # Remove the oldest one. FIFO.
+            del _str_to_bitstore_cache[next(iter(_str_to_bitstore_cache))]
+        return bs
+
+
+def _bin2bitstore(binstring: str) -> BitStore:
+    binstring = tidy_input_string(binstring)
+    binstring = binstring.replace('0b', '')
+    return _bin2bitstore_unsafe(binstring)
+
+
+def _bin2bitstore_unsafe(binstring: str) -> BitStore:
+    try:
+        return BitStore(binstring)
+    except ValueError:
+        raise CreationError(f"Invalid character in bin initialiser {binstring}.")
+
+
+def _hex2bitstore(hexstring: str) -> BitStore:
+    hexstring = tidy_input_string(hexstring)
+    hexstring = hexstring.replace('0x', '')
+    try:
+        ba = bitarray.util.hex2ba(hexstring)
+    except ValueError:
+        raise CreationError("Invalid symbol in hex initialiser.")
+    return BitStore(ba)
+
+
+def _oct2bitstore(octstring: str) -> BitStore:
+    octstring = tidy_input_string(octstring)
+    octstring = octstring.replace('0o', '')
+    try:
+        ba = bitarray.util.base2ba(8, octstring)
+    except ValueError:
+        raise CreationError("Invalid symbol in oct initialiser.")
+    return BitStore(ba)
+
+
+def _ue2bitstore(i: Union[str, int]) -> BitStore:
+    i = int(i)
+    if _lsb0:
+        raise CreationError("Exp-Golomb codes cannot be used in lsb0 mode.")
+    if i < 0:
+        raise CreationError("Cannot use negative initialiser for unsigned exponential-Golomb.")
+    if i == 0:
+        return BitStore('1')
+    tmp = i + 1
+    leadingzeros = -1
+    while tmp > 0:
+        tmp >>= 1
+        leadingzeros += 1
+    remainingpart = i + 1 - (1 << leadingzeros)
+    return BitStore('0' * leadingzeros + '1') + _uint2bitstore(remainingpart, leadingzeros)
+
+
+def _se2bitstore(i: Union[str, int]) -> BitStore:
+    i = int(i)
+    if i > 0:
+        u = (i * 2) - 1
+    else:
+        u = -2 * i
+    return _ue2bitstore(u)
+
+
+def _uie2bitstore(i: Union[str, int]) -> BitStore:
+    if _lsb0:
+        raise CreationError("Exp-Golomb codes cannot be used in lsb0 mode.")
+    i = int(i)
+    if i < 0:
+        raise CreationError("Cannot use negative initialiser for unsigned interleaved exponential-Golomb.")
+    return BitStore('1' if i == 0 else '0' + '0'.join(bin(i + 1)[3:]) + '1')
+
+
+def _sie2bitstore(i: Union[str, int]) -> BitStore:
+    i = int(i)
+    if _lsb0:
+        raise CreationError("Exp-Golomb codes cannot be used in lsb0 mode.")
+    if i == 0:
+        return BitStore('1')
+    else:
+        return _uie2bitstore(abs(i)) + (BitStore('1') if i < 0 else BitStore('0'))
+
+
+def _bfloat2bitstore(f: Union[str, float]) -> BitStore:
+    f = float(f)
+    try:
+        b = struct.pack('>f', f)
+    except OverflowError:
+        # For consistency we overflow to 'inf'.
+        b = struct.pack('>f', float('inf') if f > 0 else float('-inf'))
+    return BitStore(frombytes=b[0:2])
+
+
+def _bfloatle2bitstore(f: Union[str, float]) -> BitStore:
+    f = float(f)
+    try:
+        b = struct.pack('<f', f)
+    except OverflowError:
+        # For consistency we overflow to 'inf'.
+        b = struct.pack('<f', float('inf') if f > 0 else float('-inf'))
+    return BitStore(frombytes=b[2:4])
+
+
+def _uint2bitstore(uint: Union[str, int], length: int) -> BitStore:
+    uint = int(uint)
+    try:
+        x = BitStore(bitarray.util.int2ba(uint, length=length, endian='big', signed=False))
+    except OverflowError:
+        if uint >= (1 << length):
+            msg = f"{uint} is too large an unsigned integer for a bitstring of length {length}. " \
+                  f"The allowed range is [0, {(1 << length) - 1}]."
+            raise CreationError(msg)
+        if uint < 0:
+            raise CreationError("uint cannot be initialised with a negative number.")
+    return x
+
+
+def _int2bitstore(i: Union[str, int], length: int) -> BitStore:
+    i = int(i)
+    try:
+        x = BitStore(bitarray.util.int2ba(i, length=length, endian='big', signed=True))
+    except OverflowError:
+        if i >= (1 << (length - 1)) or i < -(1 << (length - 1)):
+            raise CreationError(f"{i} is too large a signed integer for a bitstring of length {length}. "
+                                f"The allowed range is [{-(1 << (length - 1))}, {(1 << (length - 1)) - 1}].")
+    return x
+
+
+def _uintbe2bitstore(i: Union[str, int], length: int) -> BitStore:
+    if length % 8 != 0:
+        raise CreationError(f"Big-endian integers must be whole-byte. Length = {length} bits.")
+    return _uint2bitstore(i, length)
+
+
+def _intbe2bitstore(i: int, length: int) -> BitStore:
+    if length % 8 != 0:
+        raise CreationError(f"Big-endian integers must be whole-byte. Length = {length} bits.")
+    return _int2bitstore(i, length)
+
+
+def _uintle2bitstore(i: int, length: int) -> BitStore:
+    if length % 8 != 0:
+        raise CreationError(f"Little-endian integers must be whole-byte. Length = {length} bits.")
+    x = _uint2bitstore(i, length).tobytes()
+    return BitStore(frombytes=x[::-1])
+
+
+def _intle2bitstore(i: int, length: int) -> BitStore:
+    if length % 8 != 0:
+        raise CreationError(f"Little-endian integers must be whole-byte. Length = {length} bits.")
+    x = _int2bitstore(i, length).tobytes()
+    return BitStore(frombytes=x[::-1])
+
+
+def _float2bitstore(f: Union[str, float], length: int) -> BitStore:
+    f = float(f)
+    try:
+        fmt = {16: '>e', 32: '>f', 64: '>d'}[length]
+    except KeyError:
+        raise InterpretError(f"Floats can only be 16, 32 or 64 bits long, not {length} bits")
+    try:
+        b = struct.pack(fmt, f)
+        assert len(b)*8 == length
+    except (OverflowError, struct.error):
+        # If float64 doesn't fit it automatically goes to 'inf'. This reproduces that behaviour for other types.
+        if length in [16, 32]:
+            b = struct.pack(fmt, float('inf') if f > 0 else float('-inf'))
+    return BitStore(frombytes=b)
+
+
+def _floatle2bitstore(f: Union[str, float], length: int) -> BitStore:
+    f = float(f)
+    try:
+        fmt = {16: '<e', 32: '<f', 64: '<d'}[length]
+    except KeyError:
+        raise InterpretError(f"Floats can only be 16, 32 or 64 bits long, not {length} bits")
+    try:
+        b = struct.pack(fmt, f)
+        assert len(b)*8 == length
+    except (OverflowError, struct.error):
+        # If float64 doesn't fit it automatically goes to 'inf'. This reproduces that behaviour for other types.
+        if length in [16, 32]:
+            b = struct.pack(fmt, float('inf') if f > 0 else float('-inf'))
+    return BitStore(frombytes=b)
+
+
+# Create native-endian functions as aliases depending on the byteorder
+if byteorder == 'little':
+    _uintne2bitstore = _uintle2bitstore
+    _intne2bitstore = _intle2bitstore
+    _bfloatne2bitstore = _bfloatle2bitstore
+    _floatne2bitstore = _floatle2bitstore
+else:
+    _uintne2bitstore = _uintbe2bitstore
+    _intne2bitstore = _intbe2bitstore
+    _bfloatne2bitstore = _bfloat2bitstore
+    _floatne2bitstore = _float2bitstore
+
+# Given a string of the format 'name=value' get a bitstore representing it by using
+# _name2bitstore_func[name](value)
+_name2bitstore_func: Dict[str, Callable[..., BitStore]] = {
+    'hex': _hex2bitstore,
+    '0x':  _hex2bitstore,
+    '0X':  _hex2bitstore,
+    'bin': _bin2bitstore,
+    '0b':  _bin2bitstore,
+    '0B':  _bin2bitstore,
+    'oct': _oct2bitstore,
+    '0o':  _oct2bitstore,
+    '0O':  _oct2bitstore,
+    'se':  _se2bitstore,
+    'ue':  _ue2bitstore,
+    'sie': _sie2bitstore,
+    'uie': _uie2bitstore,
+    'bfloat': _bfloat2bitstore,
+    'bfloatbe': _bfloat2bitstore,
+    'bfloatle': _bfloatle2bitstore,
+    'bfloatne': _bfloatne2bitstore,
+}
+
+# Given a string of the format 'name[:]length=value' get a bitstore representing it by using
+# _name2bitstore_func_with_length[name](value, length)
+_name2bitstore_func_with_length: Dict[str, Callable[..., BitStore]] = {
+    'uint':   _uint2bitstore,
+    'int':    _int2bitstore,
+    'uintbe': _uintbe2bitstore,
+    'intbe':  _intbe2bitstore,
+    'uintle': _uintle2bitstore,
+    'intle':  _intle2bitstore,
+    'uintne': _uintne2bitstore,
+    'intne':  _intne2bitstore,
+    'float':   _float2bitstore,
+    'floatbe': _float2bitstore,  # same as 'float'
+    'floatle': _floatle2bitstore,
+    'floatne': _floatne2bitstore,
+}
+
+
+def _bitstore_from_token(name: str, token_length: Optional[int], value: Optional[str]) -> BitStore:
+    if token_length == 0:
+        return BitStore()
+    # For pad token just return the length in zero bits
+    if name == 'pad':
+        bs = BitStore(token_length)
+        bs.setall(0)
+        return bs
+    if value is None:
+        if token_length is None:
+            raise ValueError(f"Token has no value ({name}=???).")
+        else:
+            raise ValueError(f"Token has no value ({name}:{token_length}=???).")
+
+    if name in _name2bitstore_func:
+        bs = _name2bitstore_func[name](value)
+    elif name in _name2bitstore_func_with_length:
+        bs = _name2bitstore_func_with_length[name](value, token_length)
+    elif name == 'bool':
+        if value in (1, 'True', '1'):
+            bs = BitStore('1')
+        elif value in (0, 'False', '0'):
+            bs = BitStore('0')
+        else:
+            raise CreationError("bool token can only be 'True' or 'False'.")
+    else:
+        raise CreationError(f"Can't parse token name {name}.")
+    if token_length is not None and len(bs) != token_length:
+        raise CreationError(f"Token with length {token_length} packed with value of length {len(bs)} "
+                            f"({name}:{token_length}={value}).")
+    return bs
+
+
 class Bits:
     """A container holding an immutable sequence of bits.
 
     For a mutable container use the BitArray class instead.
 
     Methods:
 
@@ -834,30 +865,20 @@
 
     @classmethod
     def _setlsb0methods(cls, lsb0: bool) -> None:
         if lsb0:
             cls._find = cls._find_lsb0  # type: ignore
             cls._rfind = cls._rfind_lsb0  # type: ignore
             cls._findall = cls._findall_lsb0  # type: ignore
-            cls._slice = cls._slice_lsb0  # type: ignore
-            cls._truncatestart = cls._truncateright  # type: ignore
-            cls._truncateend = cls._truncateleft  # type: ignore
-            cls._validate_slice = cls._validate_slice_lsb0  # type: ignore
         else:
             cls._find = cls._find_msb0  # type: ignore
             cls._rfind = cls._rfind_msb0  # type: ignore
             cls._findall = cls._findall_msb0  # type: ignore
-            cls._slice = cls._slice_msb0  # type: ignore
-            cls._truncatestart = cls._truncateleft  # type: ignore
-            cls._truncateend = cls._truncateright  # type: ignore
-            cls._validate_slice = cls._validate_slice_msb0  # type: ignore
-
-    __slots__ = ('_datastore', '_pos')
-    # This converts a single octal digit to 3 bits.
-    _octToBits: List[str] = ['{0:03b}'.format(i) for i in range(8)]
+
+    __slots__ = ('_bitstore', '_pos')
 
     # Creates dictionaries to quickly reverse single bytes
     _int8ReversalDict: Dict[int, int] = {i: int("{0:08b}".format(i)[::-1], 2) for i in range(0x100)}
     _byteReversalDict: Dict[int, bytes] = {i: bytes([int("{0:08b}".format(i)[::-1], 2)]) for i in range(0x100)}
 
     def __init__(self, auto: Optional[BitsType] = None, length: Optional[int] = None,
                  offset: Optional[int] = None, **kwargs) -> None:
@@ -895,73 +916,44 @@
         length -- length of the bitstring in bits, if needed and appropriate.
                   It must be supplied for all integer and float initialisers.
         offset -- bit offset to the data. These offset bits are
                   ignored and this is mainly intended for use when
                   initialising using 'bytes' or 'filename'.
 
         """
-        pass
+        self._bitstore.immutable = True
 
     def __new__(cls, auto: Optional[BitsType] = None, length: Optional[int] = None,
-                offset: Optional[int] = None, _cache={}, **kwargs) -> Bits:
-        # For instances auto-initialised with a string we intern the instance for re-use.
-        if isinstance(auto, str):
-            try:
-                return _cache[auto]
-            except KeyError:
-                x = object.__new__(Bits)
-                try:
-                    _, tokens = tokenparser(auto)
-                except ValueError as e:
-                    raise CreationError(*e.args)
-                if offset is not None:
-                    raise CreationError("offset should not be specified when using string initialisation.")
-                if length is not None:
-                    raise CreationError("length should not be specified when using string initialisation.")
-                x._datastore = ByteStore(bytearray(0), 0)
-                for token in tokens:
-                    x._datastore.appendstore(Bits._init_with_token(*token)._datastore)
-                if len(_cache) < CACHE_SIZE:
-                    _cache[auto] = x
-                return x
-        if type(auto) is Bits:
-            return auto
-        x = super(Bits, cls).__new__(cls)
-        x._datastore = ByteStore(bytearray())
+                offset: Optional[int] = None, pos: Optional[int] = None, **kwargs) -> Bits:
+        x = object.__new__(cls)
+        if auto is None and not kwargs:
+            # No initialiser so fill with zero bits up to length
+            if length is not None:
+                x._bitstore = BitStore(length)
+                x._bitstore.setall(0)
+            else:
+                x._bitstore = BitStore()
+            return x
         x._initialise(auto, length, offset, **kwargs)
         return x
 
     def _initialise(self, auto: Any, length: Optional[int], offset: Optional[int], **kwargs) -> None:
         if length is not None and length < 0:
             raise CreationError("bitstring length cannot be negative.")
         if offset is not None and offset < 0:
             raise CreationError("offset must be >= 0.")
         if auto is not None:
-            self._initialise_from_auto(auto, length, offset)
-            return
-        if not kwargs:
-            # No initialisers, so initialise with nothing or zero bits
-            if length is not None and length != 0:
-                data = bytearray((length + 7) // 8)
-                self._setbytes_unsafe(data, length, 0)
-                return
-            self._setbytes_unsafe(bytearray(0), 0, 0)
+            self._setauto(auto, length, offset)
             return
         k, v = kwargs.popitem()
-
         try:
-            self._setfunc[k](self, v, length, offset)
+            setting_function = self._setfunc[k]
         except KeyError:
             raise CreationError(f"Unrecognised keyword '{k}' used to initialise.")
-
-    def _initialise_from_auto(self, auto: Any, length: Optional[int], offset: Optional[int]) -> None:
-        if offset is None:
-            offset = 0
-        self._setauto(auto, length, offset)
-        return
+        setting_function(self, v, length, offset)
 
     def __getattr__(self, attribute: str):
         if attribute == '_pos':
             # For the classes without pos it's easier to return None than throw an exception.
             return None
         # Support for arbitrary attributes like u16 or f64.
         letter_to_getter: Dict[str, Callable[..., Union[int, float, str]]] = \
@@ -993,15 +985,15 @@
             try:
                 return getattr(self, name)
             except AttributeError:
                 pass
         raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{attribute}'.")
 
     def __iter__(self) -> Iterable[bool]:
-        return iter(self._datastore)
+        return iter(self._bitstore)
 
     def __copy__(self) -> Bits:
         """Return a new copy of the Bits for the copy module."""
         # Note that if you want a new copy (different ID), use _copy instead.
         # The copy can return self as it's immutable.
         return self
 
@@ -1029,21 +1021,21 @@
             s._addright(bs)
         else:
             s = bs._copy()
             s = self.__class__(s)
             s._addleft(self)
         return s
 
-    def __radd__(self, bs: Any) -> Bits:
+    def __radd__(self, bs: BitsType) -> Bits:
         """Append current bitstring to bs and return new bitstring.
 
         bs -- the string for the 'auto' initialiser that will be appended to.
 
         """
-        bs = self._converttobitstring(bs)
+        bs = self.__class__(bs)
         return bs.__add__(self)
 
     @overload
     def __getitem__(self, key: slice) -> Bits: ...
     @overload
     def __getitem__(self, key: int) -> bool: ...
 
@@ -1055,50 +1047,20 @@
 
         >>> print(BitArray('0b00110')[1:4])
         '0b011'
         >>> print(BitArray('0x00112233')[1:3:8])
         '0x1122'
 
         """
-        length = self._getlength()
-        if isinstance(key, slice):
-            step = key.step if key.step is not None else 1
-            if step != 1:
-                # convert to binary string and use string slicing
-                bs = self.__class__()
-                if _lsb0:
-                    start = length - key.start - 1 if key.start is not None else None
-                    stop = length - key.stop - 1 if key.stop is not None else None
-                    bs._setbin_unsafe(self._getbin().__getitem__(slice(start, stop, -step))[::-1])
-                else:
-                    bs._setbin_unsafe(self._getbin().__getitem__(key))
-                return bs
-            start, stop = 0, length
-            if key.start is not None:
-                start = key.start
-                if key.start < 0:
-                    start += stop
-            if key.stop is not None:
-                stop = key.stop
-                if key.stop < 0:
-                    stop += length
-            start = max(start, 0)
-            stop = min(stop, length)
-            if start < stop:
-                return self._slice(start, stop)
-            else:
-                return self.__class__()
-        else:
-            # single element
-            if key < 0:
-                key += length
-            if not 0 <= key < length:
-                raise IndexError("Slice index out of range.")
-            # Single bit, return True or False
-            return self._datastore.getbit(key)
+        if isinstance(key, int):
+            return bool(self._bitstore.getindex(key))
+        x = self._bitstore.getslice(key)
+        bs = self.__class__()
+        bs._bitstore = x
+        return bs
 
     def __len__(self) -> int:
         """Return the length of the bitstring in bits."""
         return self._getlength()
 
     def __str__(self) -> str:
         """Return approximate string representation of bitstring for printing.
@@ -1131,41 +1093,41 @@
         """Return representation that could be used to recreate the bitstring.
 
         If the returned string is too long it will be truncated. See __str__().
 
         """
         length = self.len
         pos_string = "" if self._pos in (0, None) else f", pos={self._pos}"
-        if isinstance(self._datastore.rawarray, MmapByteArray):
+        if hasattr(self._bitstore, 'filename'):
             offsetstring = ''
-            if self._datastore.byteoffset or self._offset:
-                offsetstring = ", offset=%d" % (self._datastore.rawarray.byteoffset * 8 + self._offset)
-            lengthstring = ", length=%d" % length
-            return "{0}(filename={1}{2}{3}{4})".format(self.__class__.__name__,
-                                                       repr(str(self._datastore.rawarray.source.name)),
+            if self._bitstore.offset:
+                offsetstring = f', offset={self._bitstore.offset}'
+            lengthstring = f', length={length}'
+            return '{0}(filename={1}{2}{3}{4})'.format(self.__class__.__name__,
+                                                       repr(str(self._bitstore.filename)),
                                                        lengthstring, offsetstring, pos_string)
         else:
             s = self.__str__()
             lengthstring = ''
             if s.endswith('...'):
-                lengthstring = "  # length={0}".format(length)
+                lengthstring = f'  # length={length}'
             return "{0}('{1}'{2}){3}".format(self.__class__.__name__, s, pos_string, lengthstring)
 
     def __eq__(self, bs: Any) -> bool:
         """Return True if two bitstrings have the same binary representation.
 
         >>> BitArray('0b1110') == '0xe'
         True
 
         """
         try:
             bs = Bits(bs)
         except TypeError:
             return False
-        return equal(self._datastore, bs._datastore)
+        return self._bitstore == bs._bitstore
 
     def __ne__(self, bs: Any) -> bool:
         """Return False if two bitstrings have the same binary representation.
 
         >>> BitArray('0b111') == '0x7'
         False
 
@@ -1248,15 +1210,15 @@
         Raises ValueError if the two bitstrings have differing lengths.
 
         """
         bs = Bits(bs)
         if self.len != bs.len:
             raise ValueError("Bitstrings must have the same length for & operator.")
         s = self._copy()
-        s._iand(bs)
+        s._bitstore &= bs._bitstore
         return s
 
     def __rand__(self, bs: BitsType) -> Bits:
         """Bit-wise 'and' between two bitstrings. Returns new bitstring.
 
         bs -- the bitstring to '&' with.
 
@@ -1273,15 +1235,15 @@
         Raises ValueError if the two bitstrings have differing lengths.
 
         """
         bs = Bits(bs)
         if self.len != bs.len:
             raise ValueError("Bitstrings must have the same length for | operator.")
         s = self._copy()
-        s._ior(bs)
+        s._bitstore |= bs._bitstore
         return s
 
     def __ror__(self, bs: BitsType) -> Bits:
         """Bit-wise 'or' between two bitstrings. Returns new bitstring.
 
         bs -- The bitstring to '|' with.
 
@@ -1298,15 +1260,15 @@
         Raises ValueError if the two bitstrings have differing lengths.
 
         """
         bs = Bits(bs)
         if self.len != bs.len:
             raise ValueError("Bitstrings must have the same length for ^ operator.")
         s = self._copy()
-        s._ixor(bs)
+        s._bitstore ^= bs._bitstore
         return s
 
     def __rxor__(self, bs: BitsType) -> Bits:
         """Bit-wise 'xor' between two bitstrings. Returns new bitstring.
 
         bs -- The bitstring to '^' with.
 
@@ -1380,123 +1342,124 @@
         if token_length is not None and b.len != token_length:
             raise CreationError(f"Token with length {token_length} packed with value of length {b.len} "
                                 f"({name}:{token_length}={value}).")
         return b
 
     def _clear(self) -> None:
         """Reset the bitstring to an empty state."""
-        self._datastore = ByteStore(bytearray(0))
+        self._bitstore = BitStore()
 
-    def _setauto(self, s: Any, length: Optional[int], offset: int) -> None:
+    def _setauto(self, s: BitsType, length: Optional[int], offset: Optional[int]) -> None:
         """Set bitstring from a bitstring, file, bool, integer, array, iterable or string."""
         # As s can be so many different things it's important to do the checks
         # in the correct order, as some types are also other allowed types.
         # So str must be checked before Iterable
         # and bytes/bytearray before Iterable but after str!
+        if offset is None:
+            offset = 0
         if isinstance(s, Bits):
             if length is None:
                 length = s._getlength() - offset
-            self._setbytes_unsafe(s._datastore.rawbytes, length, s._offset + offset)
+            self._bitstore = s._bitstore.getslice(slice(offset, offset + length, None))
             return
 
         if isinstance(s, io.BytesIO):
             if length is None:
                 length = s.seek(0, 2) * 8 - offset
             byteoffset, offset = divmod(offset, 8)
             bytelength = (length + byteoffset * 8 + offset + 7) // 8 - byteoffset
             if length + byteoffset * 8 + offset > s.seek(0, 2) * 8:
                 raise CreationError("BytesIO object is not long enough for specified length and offset.")
-            self._datastore = ByteStore(bytearray(s.getvalue()[byteoffset: byteoffset + bytelength]),
-                                        length, offset)
+            self._bitstore = BitStore(frombytes=s.getvalue()[byteoffset: byteoffset + bytelength]).getslice(slice(offset, offset + length))
             return
 
         if isinstance(s, io.BufferedReader):
+            m = mmap.mmap(s.fileno(), 0, access=mmap.ACCESS_READ)
+            self._bitstore = BitStore(buffer=m, offset=offset, length=length, filename=s.name, immutable=True)
+            return
+
+        if isinstance(s, bitarray.bitarray):
             if length is None:
-                length = os.path.getsize(s.name) * 8 - offset
-            byteoffset, offset = divmod(offset, 8)
-            bytelength = (length + byteoffset * 8 + offset + 7) // 8 - byteoffset
-            m = MmapByteArray(s, bytelength, byteoffset)
-            if length + byteoffset * 8 + offset > m.filelength * 8:
-                raise CreationError("File is not long enough for specified length and offset.")
-            self._datastore = ByteStore(m, length, offset)
+                if offset > len(s):
+                    raise CreationError(f"Offset of {offset} too large for bitarray of length {len(s)}.")
+                self._bitstore = BitStore(s[offset:])
+            else:
+                if offset + length > len(s):
+                    raise CreationError(f"Offset of {offset} and length of {length} too large for bitarray of length {len(s)}.")
+                self._bitstore = BitStore(s[offset: offset + length])
             return
 
         if length is not None:
             raise CreationError("The length keyword isn't applicable to this initialiser.")
         if offset > 0:
             raise CreationError("The offset keyword isn't applicable to this initialiser.")
         if isinstance(s, str):
-            bs = self._converttobitstring(s)
-            assert bs._offset == 0
-            self._setbytes_unsafe(bs._datastore.rawbytes, bs.length, 0)
+            self._bitstore = _str_to_bitstore(s)
             return
         if isinstance(s, (bytes, bytearray)):
-            self._setbytes_unsafe(bytearray(s), len(s) * 8, 0)
+            self._bitstore = BitStore(frombytes=bytearray(s))
             return
         if isinstance(s, array.array):
-            b = s.tobytes()
-            self._setbytes_unsafe(bytearray(b), len(b) * 8, 0)
+            self._bitstore = BitStore(frombytes=bytearray(s.tobytes()))
             return
         if isinstance(s, int):
             # Initialise with s zero bits.
             if s < 0:
                 raise CreationError(f"Can't create bitstring of negative length {s}.")
-            data = bytearray((s + 7) // 8)
-            self._datastore = ByteStore(data, int(s), 0)
+            self._bitstore = BitStore(int(s))
+            self._bitstore.setall(0)
             return
         if isinstance(s, abc.Iterable):
             # Evaluate each item as True or False and set bits to 1 or 0.
             self._setbin_unsafe(''.join(str(int(bool(x))) for x in s))
             return
         raise TypeError(f"Cannot initialise bitstring from {type(s)}.")
 
     def _setfile(self, filename: str, length: Optional[int], offset: Optional[int]) -> None:
         """Use file as source of bits."""
         with open(pathlib.Path(filename), 'rb') as source:
             if offset is None:
                 offset = 0
-            if length is None:
-                length = os.path.getsize(source.name) * 8 - offset
-            byteoffset, offset = divmod(offset, 8)
-            bytelength = (length + byteoffset * 8 + offset + 7) // 8 - byteoffset
-            m = MmapByteArray(source, bytelength, byteoffset)
-            if length + byteoffset * 8 + offset > m.filelength * 8:
-                raise CreationError("File is not long enough for specified length and offset.")
-            self._datastore = ByteStore(m, length, offset)
+            m = mmap.mmap(source.fileno(), 0, access=mmap.ACCESS_READ)
+            self._bitstore = BitStore(buffer=m, offset=offset, length=length, filename=source.name, immutable=True)
+
+    def _setbitarray(self, ba: bitarray.bitarray, length: Optional[int], offset: Optional[int]) -> None:
+        if offset is None:
+            offset = 0
+        if offset > len(ba):
+            raise CreationError(f"Offset of {offset} too large for bitarray of length {len(ba)}.")
+        if length is None:
+            self._bitstore = BitStore(ba[offset:])
+        else:
+            if offset + length > len(ba):
+                raise CreationError(f"Offset of {offset} and length of {length} too large for bitarray of length {len(ba)}.")
+            self._bitstore = BitStore(ba[offset: offset + length])
 
-    def _setbytes_safe(self, data: Union[bytearray, bytes, MmapByteArray],
+    def _setbytes(self, data: Union[bytearray, bytes],
                        length: Optional[int] = None, offset: Optional[int] = None) -> None:
-        """Set the data from a string."""
+        """Set the data from a bytes or bytearray object."""
+        if offset is None and length is None:
+            self._bitstore = BitStore(frombytes=bytearray(data))
+            return
         data = bytearray(data)
         if offset is None:
             offset = 0
         if length is None:
             # Use to the end of the data
             length = len(data)*8 - offset
-            self._datastore = ByteStore(data, length, offset)
         else:
             if length + offset > len(data) * 8:
                 raise CreationError(f"Not enough data present. Need {length + offset} bits, have {len(data) * 8}.")
-            if length == 0:
-                self._datastore = ByteStore(bytearray(0))
-            else:
-                self._datastore = ByteStore(data, length, offset)
-
-    def _setbytes_unsafe(self, data: Union[bytearray, MmapByteArray], length: int, offset: int):
-        """Unchecked version of _setbytes_safe."""
-        self._datastore = type(self._datastore)(data[:], length, offset)
+        self._bitstore = BitStore(buffer=data).getslice_msb0(slice(offset, offset + length, None))
 
     def _readbytes(self, start: int, length: int) -> bytes:
         """Read bytes and return them. Note that length is in bits."""
         assert length % 8 == 0
         assert start + length <= self.len
-        if not (start + self._offset) % 8:
-            return bytes(self._datastore.getbyteslice((start + self._offset) // 8,
-                                                      (start + self._offset + length) // 8))
-        return self._slice(start, start + length).tobytes()
+        return self._bitstore.getslice(slice(start, start + length, None)).tobytes()
 
     def _getbytes(self) -> bytes:
         """Return the data as an ordinary bytes object."""
         if self.len % 8:
             raise InterpretError("Cannot interpret as bytes unambiguously - not multiple of 8 bits.")
         return self._readbytes(0, self.len)
 
@@ -1509,226 +1472,172 @@
         bytes_ = self._getbytes()
         # Replace unprintable characters with '.'
         string = ''.join('.' if x in Bits._unprintable else chr(x) for x in bytes_)
         return string
 
     def _setuint(self, uint: int, length: Optional[int] = None, _offset: None = None) -> None:
         """Reset the bitstring to have given unsigned int interpretation."""
-        with suppress(AttributeError):  # bitstring will only have a _datastore if it's been created
-            if length is None:
-                # Use the whole length. Deliberately not using .len here.
-                length = self._datastore.bitlength
+        # If no length given, and we've previously been given a length, use it.
+        if length is None and hasattr(self, 'len') and self.len != 0:
+            length = self.len
         if length is None or length == 0:
             raise CreationError("A non-zero length must be specified with a uint initialiser.")
         if _offset is not None:
             raise CreationError("An offset can't be specified with an integer initialiser.")
-        if uint >= (1 << length):
-            msg = f"{uint} is too large an unsigned integer for a bitstring of length {length}. "\
-                  f"The allowed range is [0, {(1 << length) - 1}]."
-            raise CreationError(msg)
-        if uint < 0:
-            raise CreationError("uint cannot be initialised with a negative number.")
-        data = int.to_bytes(uint, (length + 7) // 8, 'big')
-
-        offset = 8 - (length % 8)
-        if offset == 8:
-            offset = 0
-        self._setbytes_unsafe(bytearray(data), length, offset)
+        self._bitstore = _uint2bitstore(uint, length)
 
     def _readuint(self, start: int, length: int) -> int:
-        # TODO: This needs to be refactored again.
-        if _lsb0:
-            return self._readuint_lsb0(start, length)
-        else:
-            return self._readuint_msb0(start, length)
-
-    def _readuint_lsb0(self, start: int, length: int) -> int:
-        return self._readuint_msb0(self.len - start - length, length)
-
-    def _readuint_msb0(self, start: int, length: int) -> int:
         """Read bits and interpret as an unsigned int."""
         if length == 0:
             raise InterpretError("Cannot interpret a zero length bitstring as an integer.")
-        offset = self._offset
-        startbyte = (start + offset) // 8
-        endbyte = (start + offset + length - 1) // 8
-
-        i = int.from_bytes(self._datastore.getbyteslice(startbyte, endbyte + 1), 'big')
-        final_bits = 8 - ((start + offset + length) % 8)
-        if final_bits != 8:
-            i >>= final_bits
-        i &= (1 << length) - 1
-        return i
+        ip = bitarray.util.ba2int(self._bitstore.getslice(slice(start, start + length, None)), signed=False)
+        return ip
 
     def _getuint(self) -> int:
         """Return data as an unsigned int."""
-        return self._readuint(0, self.len)
+        if self.len == 0:
+            raise InterpretError("Cannot interpret a zero length bitstring as an integer.")
+        bs = self._bitstore.copy() if self._bitstore.modified else self._bitstore
+        return bitarray.util.ba2int(bs, signed=False)
 
     def _setint(self, int_: int, length: Optional[int] = None, _offset: None = None) -> None:
         """Reset the bitstring to have given signed int interpretation."""
         # If no length given, and we've previously been given a length, use it.
         if length is None and hasattr(self, 'len') and self.len != 0:
             length = self.len
         if length is None or length == 0:
             raise CreationError("A non-zero length must be specified with an int initialiser.")
-        if int_ >= (1 << (length - 1)) or int_ < -(1 << (length - 1)):
-            raise CreationError(f"{int_} is too large a signed integer for a bitstring of length {length}. "
-                                f"The allowed range is [{-(1 << (length - 1))}, {(1 << (length - 1)) - 1}].")
-        if int_ >= 0:
-            self._setuint(int_, length)
-            return
-        # Do the 2's complement thing. Add one, set to minus number, then flip bits.
-        self._setuint((-int_ - 1) ^ ((1 << length) - 1), length)
+        if _offset is not None:
+            raise CreationError("An offset can't be specified with an integer initialiser.")
+        self._bitstore = _int2bitstore(int_, length)
 
     def _readint(self, start: int, length: int) -> int:
         """Read bits and interpret as a signed int"""
-        ui = self._readuint(start, length)
-        if not ui >> (length - 1):
-            # Top bit not set, number is positive
-            return ui
-        # Top bit is set, so number is negative
-        tmp = (~(ui - 1)) & ((1 << length) - 1)
-        return -tmp
+        if length == 0:
+            raise InterpretError("Cannot interpret a zero length bitstring as an integer.")
+        ip = bitarray.util.ba2int(self._bitstore.getslice(slice(start, start + length, None)), signed=True)
+        return ip
 
     def _getint(self) -> int:
         """Return data as a two's complement signed int."""
-        return self._readint(0, self.len)
+        if self.len == 0:
+            raise InterpretError("Cannot interpret a zero length bitstring as an integer.")
+        bs = self._bitstore.copy() if self._bitstore.modified else self._bitstore
+        return bitarray.util.ba2int(bs, signed=True)
 
     def _setuintbe(self, uintbe: int, length: Optional[int] = None, _offset: None = None) -> None:
         """Set the bitstring to a big-endian unsigned int interpretation."""
-        if length is not None and length % 8 != 0:
-            raise CreationError(f"Big-endian integers must be whole-byte. Length = {length} bits.")
-        self._setuint(uintbe, length)
+        if length is None and hasattr(self, 'len') and self.len != 0:
+            length = self.len
+        if length is None or length == 0:
+            raise CreationError("A non-zero length must be specified with a uintbe initialiser.")
+        self._bitstore = _uintbe2bitstore(uintbe, length)
 
     def _readuintbe(self, start: int, length: int) -> int:
         """Read bits and interpret as a big-endian unsigned int."""
         if length % 8:
             raise InterpretError(f"Big-endian integers must be whole-byte. Length = {length} bits.")
         return self._readuint(start, length)
 
     def _getuintbe(self) -> int:
         """Return data as a big-endian two's complement unsigned int."""
         return self._readuintbe(0, self.len)
 
     def _setintbe(self, intbe: int, length: Optional[int] = None, _offset: None = None) -> None:
         """Set bitstring to a big-endian signed int interpretation."""
-        if length is not None and length % 8 != 0:
-            raise CreationError(f"Big-endian integers must be whole-byte. Length = {length} bits.")
-        self._setint(intbe, length)
+        if length is None and hasattr(self, 'len') and self.len != 0:
+            length = self.len
+        if length is None or length == 0:
+            raise CreationError("A non-zero length must be specified with a intbe initialiser.")
+        self._bitstore = _intbe2bitstore(intbe, length)
 
     def _readintbe(self, start: int, length: int) -> int:
         """Read bits and interpret as a big-endian signed int."""
         if length % 8:
             raise InterpretError(f"Big-endian integers must be whole-byte. Length = {length} bits.")
         return self._readint(start, length)
 
     def _getintbe(self) -> int:
         """Return data as a big-endian two's complement signed int."""
         return self._readintbe(0, self.len)
 
     def _setuintle(self, uintle: int, length: Optional[int] = None, _offset: None = None) -> None:
-        if length is not None and length % 8 != 0:
-            raise CreationError(f"Little-endian integers must be whole-byte. Length = {length} bits.")
-        self._setuint(uintle, length)
-        self._datastore.rawarray = self._datastore.rawarray[::-1]
+        if length is None and hasattr(self, 'len') and self.len != 0:
+            length = self.len
+        if length is None or length == 0:
+            raise CreationError("A non-zero length must be specified with a uintle initialiser.")
+        if _offset is not None:
+            raise CreationError("An offset can't be specified with an integer initialiser.")
+        self._bitstore = _uintle2bitstore(uintle, length)
 
     def _readuintle(self, start: int, length: int) -> int:
         """Read bits and interpret as a little-endian unsigned int."""
         if length % 8:
             raise InterpretError(f"Little-endian integers must be whole-byte. Length = {length} bits.")
-        assert start + length <= self.len
-        absolute_pos = start + self._offset
-        startbyte, offset = divmod(absolute_pos, 8)
-        val = 0
-        if not offset:
-            endbyte = (absolute_pos + length - 1) // 8
-            chunksize = 4  # for 'L' format
-            while endbyte - chunksize + 1 >= startbyte:
-                val <<= 8 * chunksize
-                val += struct.unpack('<L', bytes(self._datastore.getbyteslice(endbyte + 1 - chunksize, endbyte + 1)))[0]
-                endbyte -= chunksize
-            for b in range(endbyte, startbyte - 1, -1):
-                val <<= 8
-                val += self._datastore.getbyte(b)
-        else:
-            data = self._slice(start, start + length)
-            assert data.len % 8 == 0
-            data._reversebytes(0, self.len)
-            for b in bytearray(data.bytes):
-                val <<= 8
-                val += b
+        bs = BitStore(frombytes=self._bitstore.getslice(slice(start, start + length, None)).tobytes()[::-1])
+        val = bitarray.util.ba2int(bs, signed=False)
         return val
 
     def _getuintle(self) -> int:
         return self._readuintle(0, self.len)
 
     def _setintle(self, intle: int, length: Optional[int] = None, _offset: None = None) -> None:
-        if length is not None and length % 8 != 0:
-            raise CreationError(f"Little-endian integers must be whole-byte. Length = {length} bits.")
-        self._setint(intle, length)
-        self._datastore.rawarray = self._datastore.rawarray[::-1]
+        if length is None and hasattr(self, 'len') and self.len != 0:
+            length = self.len
+        if length is None or length == 0:
+            raise CreationError("A non-zero length must be specified with a uintle initialiser.")
+        if _offset is not None:
+            raise CreationError("An offset can't be specified with an integer initialiser.")
+        self._bitstore = _intle2bitstore(intle, length)
 
     def _readintle(self, start: int, length: int) -> int:
         """Read bits and interpret as a little-endian signed int."""
-        ui = self._readuintle(start, length)
-        if not ui >> (length - 1):
-            # Top bit not set, number is positive
-            return ui
-        # Top bit is set, so number is negative
-        tmp = (~(ui - 1)) & ((1 << length) - 1)
-        return -tmp
+        if length % 8:
+            raise InterpretError(f"Little-endian integers must be whole-byte. Length = {length} bits.")
+        bs = BitStore(frombytes=self._bitstore.getslice(slice(start, start + length, None)).tobytes()[::-1])
+        val = bitarray.util.ba2int(bs, signed=True)
+        return val
 
     def _getintle(self) -> int:
         return self._readintle(0, self.len)
 
-    def _setfloat(self, f: float, struct_dict: Dict[int, str], length: Optional[int] = None):
-        # If no length given, and we've previously been given a length, use it.
-        if length is None and hasattr(self, 'len') and self.len != 0:
-            length = self.len
-        if length is None or length == 0:
-            raise CreationError("A non-zero length must be specified with a float initialiser.")
-        try:
-            b = struct.pack(struct_dict[length], f)
-            self._setbytes_unsafe(bytearray(b), length, 0)
-        except KeyError:
-            raise CreationError(f"Floats can only be 16, 32 or 64 bits long, not {length} bits")
-        except (OverflowError, struct.error):
-            # If float64 doesn't fit it automatically goes to 'inf'. This reproduces that behaviour for other types.
-            if length in [16, 32]:
-                b = struct.pack(struct_dict[length], float('inf') if f > 0 else float('-inf'))
-                self._setbytes_unsafe(bytearray(b), length, 0)
-
     def _readfloat(self, start: int, length: int, struct_dict: Dict[int, str]) -> float:
         """Read bits and interpret as a float."""
         try:
             fmt = struct_dict[length]
         except KeyError:
             raise InterpretError(f"Floats can only be 16, 32 or 64 bits long, not {length} bits")
 
-        if _lsb0:
-            start = self._getlength() - start - length
-        startbyte, offset = divmod(start + self._offset, 8)
+        startbyte, offset = divmod(start, 8)
         if offset == 0:
-            return struct.unpack(fmt, bytes(self._datastore.getbyteslice(startbyte, startbyte + length // 8)))[0]
+            return struct.unpack(fmt, self._bitstore.getslice(slice(start, start + length, None)).tobytes())[0]
         else:
             return struct.unpack(fmt, self._readbytes(start, length))[0]
 
     def _setfloatbe(self, f: float, length: Optional[int] = None, _offset: None = None) -> None:
-        self._setfloat(f, {16: '>e', 32: '>f', 64: '>d'}, length)
+        if length is None and hasattr(self, 'len') and self.len != 0:
+            length = self.len
+        if length is None or length not in [16, 32, 64]:
+            raise CreationError("A length of 16, 32, or 64 must be specified with a float initialiser.")
+        self._bitstore = _float2bitstore(f, length)
 
     def _readfloatbe(self, start: int, length: int) -> float:
         """Read bits and interpret as a big-endian float."""
         return self._readfloat(start, length, {16: '>e', 32: '>f', 64: '>d'})
 
     def _getfloatbe(self) -> float:
         """Interpret the whole bitstring as a big-endian float."""
         return self._readfloatbe(0, self.len)
 
     def _setfloatle(self, f: float, length: Optional[int] = None, _offset: None = None) -> None:
-        self._setfloat(f, {16: '<e', 32: '<f', 64: '<d'}, length)
+        if length is None and hasattr(self, 'len') and self.len != 0:
+            length = self.len
+        if length is None or length not in [16, 32, 64]:
+            raise CreationError("A length of 16, 32, or 64 must be specified with a float initialiser.")
+        self._bitstore = _floatle2bitstore(f, length)
 
     def _readfloatle(self, start: int, length: int) -> float:
         """Read bits and interpret as a little-endian float."""
         return self._readfloat(start, length, {16: '<e', 32: '<f', 64: '<d'})
 
     def _getfloatle(self) -> float:
         """Interpret the whole bitstring as a little-endian float."""
@@ -1743,56 +1652,38 @@
         two_bytes = self._slice(start, start + 16)
         zero_padded = two_bytes + Bits(16)
         return zero_padded._getfloatbe()
 
     def _setbfloatbe(self, f: Union[float, str], length: Optional[int] = None, _offset: None = None) -> None:
         if length is not None and length != 16:
             raise CreationError(f"bfloats must be length 16, received a length of {length} bits.")
-        f = float(f)
-        four_byte_float = Bits(float=f, length=32)
-        self._setbytes_unsafe(four_byte_float._datastore.rawarray[0:2], 16, 0)
+        self._bitstore = _bfloat2bitstore(f)
 
     def _getbfloatle(self) -> float:
         return self._readbfloatle(0, self.len)
 
     def _readbfloatle(self, start: int, _length: int) -> float:
         two_bytes = self._slice(start, start + 16)
         zero_padded = Bits(16) + two_bytes
         return zero_padded._getfloatle()
 
     def _setbfloatle(self, f: Union[float, str], length: Optional[int] = None, _offset: None = None) -> None:
         if length is not None and length != 16:
             raise CreationError(f"bfloats must be length 16, received a length of {length} bits.")
-        f = float(f)
-        four_byte_float = Bits(floatle=f, length=32)
-        self._setbytes_unsafe(four_byte_float._datastore.rawarray[2:4], 16, 0)
+        self._bitstore = _bfloatle2bitstore(f)
 
     def _setue(self, i: int, _length: None = None, _offset: None = None) -> None:
         """Initialise bitstring with unsigned exponential-Golomb code for integer i.
 
         Raises CreationError if i < 0.
 
         """
-        if _lsb0:
-            raise CreationError("Exp-Golomb codes cannot be used in lsb0 mode.")
         if _length is not None or _offset is not None:
             raise CreationError("Cannot specify a length of offset for exponential-Golomb codes.")
-        if i < 0:
-            raise CreationError("Cannot use negative initialiser for unsigned exponential-Golomb.")
-        if not i:
-            self._setbin_unsafe('1')
-            return
-        tmp = i + 1
-        leadingzeros = -1
-        while tmp > 0:
-            tmp >>= 1
-            leadingzeros += 1
-        remainingpart = i + 1 - (1 << leadingzeros)
-        binstring = '0' * leadingzeros + '1' + Bits(uint=remainingpart, length=leadingzeros).bin
-        self._setbin_unsafe(binstring)
+        self._bitstore = _ue2bitstore(i)
 
     def _readue(self, pos: int, _length: None = None) -> Tuple[int, int]:
         """Return interpretation of next bits as unsigned exponential-Golomb code.
 
         Raises ReadError if the end of the bitstring is encountered while
         reading the code.
 
@@ -1831,19 +1722,15 @@
             raise InterpretError("Bitstring is not a single exponential-Golomb code.")
         return value
 
     def _setse(self, i: int, _length: None = None, _offset: None = None) -> None:
         """Initialise bitstring with signed exponential-Golomb code for integer i."""
         if _length is not None or _offset is not None:
             raise CreationError("Cannot specify a length of offset for exponential-Golomb codes.")
-        if i > 0:
-            u = (i * 2) - 1
-        else:
-            u = -2 * i
-        self._setue(u)
+        self._bitstore = _se2bitstore(i)
 
     def _getse(self) -> int:
         """Return data as signed exponential-Golomb code.
 
         Raises InterpretError if bitstring is not a single exponential-Golomb code.
 
         """
@@ -1873,19 +1760,17 @@
 
     def _setuie(self, i: int, _length: None = None, _offset: None = None) -> None:
         """Initialise bitstring with unsigned interleaved exponential-Golomb code for integer i.
 
         Raises CreationError if i < 0.
 
         """
-        if _lsb0:
-            raise CreationError("Exp-Golomb codes cannot be used in lsb0 mode.")
-        if i < 0:
-            raise CreationError("Cannot use negative initialiser for unsigned interleaved exponential-Golomb.")
-        self._setbin_unsafe('1' if i == 0 else '0' + '0'.join(bin(i + 1)[3:]) + '1')
+        if _length is not None or _offset is not None:
+            raise CreationError("Cannot specify a length of offset for exponential-Golomb codes.")
+        self._bitstore = _uie2bitstore(i)
 
     def _readuie(self, pos: int, _length: None = None) -> Tuple[int, int]:
         """Return interpretation of next bits as unsigned interleaved exponential-Golomb code.
 
         Raises ReadError if the end of the bitstring is encountered while
         reading the code.
 
@@ -1917,19 +1802,17 @@
                 raise ReadError
         except ReadError:
             raise InterpretError("Bitstring is not a single interleaved exponential-Golomb code.")
         return value
 
     def _setsie(self, i: int, _length: None = None, _offset: None = None) -> None:
         """Initialise bitstring with signed interleaved exponential-Golomb code for integer i."""
-        if not i:
-            self._setbin_unsafe('1')
-        else:
-            self._setuie(abs(i))
-            self._addright(Bits([i < 0]))
+        if _length is not None or _offset is not None:
+            raise CreationError("Cannot specify a length of offset for exponential-Golomb codes.")
+        self._bitstore = _sie2bitstore(i)
 
     def _getsie(self) -> int:
         """Return data as signed interleaved exponential-Golomb code.
 
         Raises InterpretError if bitstring is not a single exponential-Golomb code.
 
         """
@@ -1963,17 +1846,17 @@
 
     def _setbool(self, value: Union[bool, str], length: Optional[int] = None, _offset: None = None) -> None:
         # We deliberately don't want to have implicit conversions to bool here.
         # If we did then it would be difficult to deal with the 'False' string.
         if length is not None and length != 1:
             raise CreationError(f"bools must be length 1, received a length of {length} bits.")
         if value in (1, 'True'):
-            self._setbytes_unsafe(bytearray(b'\x80'), 1, 0)
+            self._bitstore = BitStore('1')
         elif value in (0, 'False'):
-            self._setbytes_unsafe(bytearray(b'\x00'), 1, 0)
+            self._bitstore = BitStore('0')
         else:
             raise CreationError(f"Cannot initialise boolean with {value}.")
 
     def _getbool(self) -> bool:
         if self.length != 1:
             raise InterpretError(f"For a bool interpretation a bitstring must be 1 bit long, not {self.length} bits.")
         return self[0]
@@ -1982,174 +1865,94 @@
         return self[pos], pos + 1
 
     def _readpad(self, _pos, _length) -> None:
         return None
 
     def _setbin_safe(self, binstring: str, _length: None = None, _offset: None = None) -> None:
         """Reset the bitstring to the value given in binstring."""
-        binstring = tidy_input_string(binstring)
-        # remove any 0b if present
-        binstring = binstring.replace('0b', '')
-        self._setbin_unsafe(binstring)
+        self._bitstore = _bin2bitstore(binstring)
 
     def _setbin_unsafe(self, binstring: str, _length: None = None, _offset: None = None) -> None:
         """Same as _setbin_safe, but input isn't sanity checked. binstring mustn't start with '0b'."""
-        if binstring == '':
-            self._setbytes_unsafe(bytearray(), 0, 0)
-            return
-        try:
-            i = int(binstring, 2)
-        except ValueError:
-            raise CreationError(f"Invalid character in bin initialiser {binstring}.")
-        if len(binstring) % 8 != 0:
-            i <<= 8 - (len(binstring) % 8)
-        b = i.to_bytes((len(binstring) + 7) // 8, 'big')
-        self._setbytes_unsafe(bytearray(b), len(binstring), 0)
+        self._bitstore = _bin2bitstore_unsafe(binstring)
 
     def _readbin(self, start: int, length: int) -> str:
         """Read bits and interpret as a binary string."""
         if length == 0:
             return ''
-        b = self._slice(start, start + length).tobytes()
-        integer = int.from_bytes(b, 'big')
-        c = "{:0{}b}".format(integer, 8*len(b))
-        return c[0:length]
+        return self._bitstore.getslice(slice(start, start + length, None)).to01()
 
     def _getbin(self) -> str:
         """Return interpretation as a binary string."""
         return self._readbin(0, self.len)
 
     def _setoct(self, octstring: str, _length: None = None, _offset: None = None) -> None:
         """Reset the bitstring to have the value given in octstring."""
-        octstring = tidy_input_string(octstring)
-        # remove any 0o if present
-        octstring = octstring.replace('0o', '')
-        binlist = []
-        for i in octstring:
-            try:
-                binlist.append(Bits._octToBits[int(i)])
-            except (ValueError, IndexError):
-                raise CreationError(f"Invalid symbol '{i}' in oct initialiser.")
-        self._setbin_unsafe(''.join(binlist))
+        self._bitstore = _oct2bitstore(octstring)
 
     def _readoct(self, start: int, length: int) -> str:
         """Read bits and interpret as an octal string."""
         if length % 3:
             raise InterpretError("Cannot convert to octal unambiguously - not multiple of 3 bits long.")
-        if not length:
-            return ''
-        # Get main octal bit by converting from int.
-        # Strip starting '0o'.
-        end = oct(self._readuint(start, length))[2:]
-        middle = '0' * (length // 3 - len(end))
-        return middle + end
+        s = bitarray.util.ba2base(8, self._bitstore.getslice(slice(start, start + length, None)))
+        return s
 
     def _getoct(self) -> str:
         """Return interpretation as an octal string."""
-        return self._readoct(0, self.len)
+        if self.len % 3:
+            raise InterpretError("Cannot convert to octal unambiguously - not multiple of 3 bits long.")
+        ba = self._bitstore.copy() if self._bitstore.modified else self._bitstore
+        return bitarray.util.ba2base(8, ba)
 
     def _sethex(self, hexstring: str, _length: None = None, _offset: None = None) -> None:
         """Reset the bitstring to have the value given in hexstring."""
-        hexstring = tidy_input_string(hexstring)
-        # remove any 0x if present
-        hexstring = hexstring.replace('0x', '')
-        length = len(hexstring)
-        if length % 2:
-            hexstring += '0'
-        try:
-            data = bytearray.fromhex(hexstring)
-        except ValueError:
-            raise CreationError("Invalid symbol in hex initialiser.")
-        self._setbytes_unsafe(data, length * 4, 0)
+        self._bitstore = _hex2bitstore(hexstring)
 
     def _readhex(self, start: int, length: int) -> str:
         """Read bits and interpret as a hex string."""
         if length % 4:
             raise InterpretError("Cannot convert to hex unambiguously - not a multiple of 4 bits long.")
-        if not length:
-            return ''
-        s = self._slice(start, start + length).tobytes()
-        s = s.hex()
-        # If there's one nibble too many then cut it off
-        return s[:-1] if (length // 4) % 2 else s
+        return bitarray.util.ba2hex(self._bitstore.getslice(slice(start, start + length, None)))
 
     def _gethex(self) -> str:
-        """Return the hexadecimal representation as a string prefixed with '0x'.
+        """Return the hexadecimal representation as a string.
 
         Raises an InterpretError if the bitstring's length is not a multiple of 4.
 
         """
-        return self._readhex(0, self.len)
-
-    def _getoffset(self) -> int:
-        return self._datastore.offset
+        if self.len % 4:
+            raise InterpretError("Cannot convert to hex unambiguously - not a multiple of 4 bits long.")
+        ba = self._bitstore.copy() if self._bitstore.modified else self._bitstore
+        return bitarray.util.ba2hex(ba)
 
     def _getlength(self) -> int:
         """Return the length of the bitstring in bits."""
-        return self._datastore.bitlength
-
-    @classmethod
-    def _converttobitstring(cls, bs: BitsType, offset: int = 0, cache: Dict = {}) -> Bits:
-        """Convert bs to a bitstring and return it.
-
-        offset gives the suggested bit offset of first significant
-        bit, to optimise append etc.
-
-        """
-        if isinstance(bs, Bits):
-            return bs
-        try:
-            return cache[(bs, offset)]
-        except KeyError:
-            if isinstance(bs, str):
-                b = cls()
-                try:
-                    _, tokens = tokenparser(bs)
-                except ValueError as e:
-                    raise CreationError(*e.args)
-                if tokens:
-                    b._addright(Bits._init_with_token(*tokens[0]))
-                    b._datastore = offsetcopy(b._datastore, offset)
-                    for token in tokens[1:]:
-                        b._addright(Bits._init_with_token(*token))
-                assert b.len == 0 or b._offset == offset
-                if len(cache) < CACHE_SIZE:
-                    cache[(bs, offset)] = b
-                return b
-        except TypeError:
-            # Unhashable type
-            pass
-        return cls(bs)
+        return len(self._bitstore)
 
     def _copy(self) -> Bits:
         """Create and return a new copy of the Bits (always in memory)."""
+        # Note that __copy__ may choose to return self if it's immutable. This method always makes a copy.
         s_copy = self.__class__()
-        s_copy._setbytes_unsafe(self._datastore.getbyteslice(0, self._datastore.bytelength),
-                                self.len, self._offset)
+        s_copy._bitstore = self._bitstore.copy()
         return s_copy
 
-    def _slice_lsb0(self, start: int, end: int) -> Bits:
-        """Used internally to get a slice, without error checking (LSB0)."""
-        return self._absolute_slice(self.length - end, self.length - start)
-
-    def _slice_msb0(self, start: int, end: int) -> Bits:
-        """Used internally to get a slice, without error checking (MSB0)."""
-        return self._absolute_slice(start, end)
+    def _slice(self, start: int, end: int) -> Bits:
+        """Used internally to get a slice, without error checking."""
+        bs = self.__class__()
+        bs._bitstore = self._bitstore.getslice(slice(start, end, None))
+        return bs
 
     def _absolute_slice(self, start: int, end: int) -> Bits:
         """Used internally to get a slice, without error checking.
         Uses MSB0 bit numbering even if LSB0 is set."""
         if end == start:
             return self.__class__()
         assert start < end, f"start={start}, end={end}"
-        offset = self._offset
-        startbyte, newoffset = divmod(start + offset, 8)
-        endbyte = (end + offset - 1) // 8
         bs = self.__class__()
-        bs._setbytes_unsafe(self._datastore.getbyteslice(startbyte, endbyte + 1), end - start, newoffset)
+        bs._bitstore = self._bitstore.getslice_msb0(slice(start, end, None))
         return bs
 
     def _readtoken(self, name: str, pos: int, length: Optional[int]) -> Tuple[Union[float, int, str, None, Bits], int]:
         """Reads a token from the bitstring and returns the result."""
         if length is not None and int(length) > self.length - pos:
             raise ReadError("Reading off the end of the data. "
                             f"Tried to read {int(length)} bits when only {self.length - pos} available.")
@@ -2161,182 +1964,84 @@
                 assert length is not None
                 return val, pos + length
         except KeyError:
             raise ValueError(f"Can't parse token {name}:{length}")
 
     def _addright(self, bs: Bits) -> None:
         """Add a bitstring to the RHS of the current bitstring."""
-        self._datastore.appendstore(bs._datastore)
+        self._bitstore += bs._bitstore
 
     def _addleft(self, bs: Bits) -> None:
         """Prepend a bitstring to the current bitstring."""
-        self._datastore.prependstore(bs._datastore)
-
-    def _reverse(self) -> None:
-        """Reverse all bits in-place."""
-        # Reverse the contents of each byte
-        n = [Bits._byteReversalDict[b] for b in self._datastore.rawbytes]
-        # Then reverse the order of the bytes
-        n.reverse()
-        # The new offset is the number of bits that were unused at the end.
-        newoffset = 8 - (self._offset + self.len) % 8
-        if newoffset == 8:
-            newoffset = 0
-        self._setbytes_unsafe(bytearray().join(n), self.length, newoffset)
+        if bs._bitstore.immutable:
+            self._bitstore = bs._bitstore.copy() + self._bitstore
+        else:
+            self._bitstore = bs._bitstore + self._bitstore
 
     def _truncateleft(self, bits: int) -> Bits:
         """Truncate bits from the start of the bitstring. Return the truncated bits."""
         assert 0 <= bits <= self.len
         if not bits:
             return Bits()
         truncated_bits = self._absolute_slice(0, bits)
         if bits == self.len:
             self._clear()
             return truncated_bits
-        bytepos, offset = divmod(self._offset + bits, 8)
-        self._setbytes_unsafe(self._datastore.getbyteslice(bytepos, self._datastore.bytelength), self.len - bits,
-                              offset)
+        self._bitstore = self._bitstore.getslice_msb0(slice(bits, None, None))
         return truncated_bits
 
     def _truncateright(self, bits: int) -> Bits:
         """Truncate bits from the end of the bitstring. Return the truncated bits."""
         assert 0 <= bits <= self.len
         if not bits:
             return Bits()
         truncated_bits = self._absolute_slice(self.length - bits, self.length)
         if bits == self.len:
             self._clear()
             return truncated_bits
-        newlength_in_bytes = (self._offset + self.len - bits + 7) // 8
-        self._setbytes_unsafe(self._datastore.getbyteslice(0, newlength_in_bytes), self.len - bits,
-                              self._offset)
+        self._bitstore = self._bitstore.getslice_msb0(slice(None, -bits, None))
         return truncated_bits
 
-    def _insert_lsb0(self, bs: Bits, pos: int) -> None:
-        """Insert bs at pos (LSB0)."""
-        self._insert_msb0(bs, self.len - pos)
-
-    def _insert_msb0(self, bs: Bits, pos: int) -> None:
+    def _insert(self, bs: Bits, pos: int) -> None:
         """Insert bs at pos."""
         assert 0 <= pos <= self.len
-        if pos > self.len // 2:
-            # Inserting nearer end, so cut off end.
-            end = self._truncateright(self.len - pos)
-            self._addright(bs)
-            self._addright(end)
-        else:
-            # Inserting nearer start, so cut off start.
-            start = self._slice(0, pos)
-            self._truncateleft(pos)
-            self._addleft(bs)
-            self._addleft(start)
+        self._bitstore[pos: pos] = bs._bitstore
         if self._pos is not None:
             self._pos = pos + bs.len
+        return
 
-    def _overwrite_lsb0(self, bs: Bits, pos: int) -> None:
-        """Overwrite with bs at pos (LSB0)."""
-        self._overwrite_msb0(bs, self.len - pos - bs.len)
-
-    def _overwrite_msb0(self, bs: Bits, pos: int) -> None:
+    def _overwrite(self, bs: Bits, pos: int) -> None:
         """Overwrite with bs at pos."""
         assert 0 <= pos <= self.len
         if bs is self:
             # Just overwriting with self, so do nothing.
             assert pos == 0
             return
-        if pos + bs.len > self.len:
-            # The overwrite goes past the end. Easiest thing is to extend with zeros then overwrite.
-            self._addright(Bits(pos + bs.len - self.len))
-        firstbytepos = (self._offset + pos) // 8
-        lastbytepos = (self._offset + pos + bs.len - 1) // 8
-        bytepos, bitoffset = divmod(self._offset + pos, 8)
-        if firstbytepos == lastbytepos:
-            mask = ((1 << bs.len) - 1) << (8 - bs.len - bitoffset)
-            self._datastore.setbyte(bytepos, self._datastore.getbyte(bytepos) & (~mask))
-            d = offsetcopy(bs._datastore, bitoffset)
-            self._datastore.setbyte(bytepos, self._datastore.getbyte(bytepos) | (d.getbyte(0) & mask))
-        else:
-            # Do first byte
-            mask = (1 << (8 - bitoffset)) - 1
-            self._datastore.setbyte(bytepos, self._datastore.getbyte(bytepos) & (~mask))
-            d = offsetcopy(bs._datastore, bitoffset)
-            self._datastore.setbyte(bytepos, self._datastore.getbyte(bytepos) | (d.getbyte(0) & mask))
-            # Now do all the full bytes
-            self._datastore.setbyteslice(firstbytepos + 1, lastbytepos, d.getbyteslice(1, lastbytepos - firstbytepos))
-            # and finally the last byte
-            bitsleft = (self._offset + pos + bs.len) % 8
-            if not bitsleft:
-                bitsleft = 8
-            mask = (1 << (8 - bitsleft)) - 1
-            self._datastore.setbyte(lastbytepos, self._datastore.getbyte(lastbytepos) & mask)
-            self._datastore.setbyte(lastbytepos,
-                                    self._datastore.getbyte(lastbytepos) | (d.getbyte(d.bytelength - 1) & ~mask))
-
-    def _delete_lsb0(self, bits: int, pos: int) -> None:
-        """Delete bits at pos (LSB0)."""
-        self._delete_msb0(bits, self.len - pos - bits)
+        self._bitstore[pos: pos + bs.len] = bs._bitstore
 
-    def _delete_msb0(self, bits: int, pos: int) -> None:
+    def _delete(self, bits: int, pos: int) -> None:
         """Delete bits at pos."""
         assert 0 <= pos <= self.len
         assert pos + bits <= self.len, f"pos={pos}, bits={bits}, len={self.len}"
-        if not pos:
-            # Cutting bits off at the start.
-            self._truncateleft(bits)
-            return
-        if pos + bits == self.len:
-            # Cutting bits off at the end.
-            self._truncateright(bits)
-            return
-        if pos > self.len - pos - bits:
-            # More bits before cut point than after it, so do bit shifting
-            # on the final bits.
-            end = self._slice_msb0(pos + bits, self.len)
-            assert self.len - pos > 0
-            self._truncateright(self.len - pos)
-            self._addright(end)
-            return
-        # More bits after the cut point than before it.
-        start = self._slice_msb0(0, pos)
-        self._truncateleft(pos + bits)
-        self._addleft(start)
+        del self._bitstore[pos: pos + bits]
         return
 
     def _reversebytes(self, start: int, end: int) -> None:
         """Reverse bytes in-place."""
-        # Make the start occur on a byte boundary
-        # TODO: We could be cleverer here to avoid changing the offset.
-        newoffset = 8 - (start % 8)
-        if newoffset == 8:
-            newoffset = 0
-        self._datastore = offsetcopy(self._datastore, newoffset)
-        # Now just reverse the byte data
-        toreverse = bytearray(self._datastore.getbyteslice((newoffset + start) // 8, (newoffset + end) // 8))
-        toreverse.reverse()
-        self._datastore.setbyteslice((newoffset + start) // 8, (newoffset + end) // 8, toreverse)
-
-    def _set(self, pos: int) -> None:
-        """Set bit at pos to 1."""
-        assert 0 <= pos < self.len
-        self._datastore.setbit(pos)
-
-    def _unset(self, pos: int) -> None:
-        """Set bit at pos to 0."""
-        assert 0 <= pos < self.len
-        self._datastore.unsetbit(pos)
+        assert (end - start) % 8 == 0
+        self._bitstore[start:end] = BitStore(frombytes=self._bitstore.getslice(slice(start, end, None)).tobytes()[::-1])
 
     def _invert(self, pos: int) -> None:
         """Flip bit at pos 1<->0."""
         assert 0 <= pos < self.len
-        self._datastore.invertbit(pos)
+        self._bitstore.invert(pos)
 
     def _invert_all(self) -> None:
         """Invert every bit."""
-        for p in range(self._datastore.byteoffset, self._datastore.byteoffset + self._datastore.bytelength):
-            self._datastore.rawarray[p] = 256 + ~self._datastore.rawarray[p]
+        self._bitstore.invert()
 
     def _ilshift(self, n: int) -> Bits:
         """Shift bits by n to the left in place. Return self."""
         assert 0 < n <= self.len
         self._addright(Bits(n))
         self._truncateleft(n)
         return self
@@ -2358,44 +2063,19 @@
         old_len: int = self.len
         while m * 2 < n:
             self._addright(self)
             m *= 2
         self._addright(self[0:(n - m) * old_len])
         return self
 
-    def _inplace_logical_helper(self, bs: Bits, f: Callable[[int, int], int]) -> Bits:
-        """Helper function containing most of the __ior__, __iand__, __ixor__ code."""
-        # Give the two bitstrings the same offset (modulo 8)
-        self_byteoffset, self_bitoffset = divmod(self._getoffset(), 8)
-        bs_byteoffset, bs_bitoffset = divmod(bs._getoffset(), 8)
-        if bs_bitoffset != self_bitoffset:
-            if not self_bitoffset:
-                bs._datastore = offsetcopy(bs._datastore, 0)
-            else:
-                self._datastore = offsetcopy(self._datastore, bs_bitoffset)
-        a = self._datastore.rawbytes
-        b = bs._datastore.rawbytes
-        for i in range(len(a)):
-            a[i] = f(a[i + self_byteoffset], b[i + bs_byteoffset])
-        return self
-
-    def _ior(self, bs: Bits) -> Bits:
-        return self._inplace_logical_helper(bs, operator.ior)
-
-    def _iand(self, bs: Bits) -> Bits:
-        return self._inplace_logical_helper(bs, operator.iand)
-
-    def _ixor(self, bs: Bits) -> Bits:
-        return self._inplace_logical_helper(bs, operator.xor)
-
     def _readbits(self, start: int, length: int) -> Bits:
         """Read some bits from the bitstring and return newly constructed bitstring."""
         return self._slice(start, start + length)
 
-    def _validate_slice_msb0(self, start: Optional[int], end: Optional[int]) -> Tuple[int, int]:
+    def _validate_slice(self, start: Optional[int], end: Optional[int]) -> Tuple[int, int]:
         """Validate start and end and return them as positive bit positions."""
         if start is None:
             start = 0
         elif start < 0:
             start += self._getlength()
         if end is None:
             end = self._getlength()
@@ -2405,18 +2085,14 @@
             raise ValueError("end is not a valid position in the bitstring.")
         if not 0 <= start <= self._getlength():
             raise ValueError("start is not a valid position in the bitstring.")
         if end < start:
             raise ValueError("end must not be less than start.")
         return start, end
 
-    def _validate_slice_lsb0(self, start: Optional[int], end: Optional[int]) -> Tuple[int, int]:
-        start, end = self._validate_slice_msb0(start, end)
-        return self._getlength() - end, self._getlength() - start
-
     def unpack(self, fmt: Union[str, List[Union[str, int]]], **kwargs) -> List[Union[float, int, str, None, Bits]]:
         """Interpret the whole bitstring using fmt and return list.
 
         fmt -- A single string or a list of strings with comma separated tokens
                describing how to interpret the bits in the bitstring. Items
                can also be integers, for reading new bitstring of the given length.
         kwargs -- A dictionary or keyword-value pairs - the keywords used in the
@@ -2426,15 +2102,15 @@
         are available then all bits to the end of the bitstring will be used.
 
         See the docstring for 'read' for token examples.
 
         """
         return self._readlist(fmt, 0, **kwargs)[0]
 
-    def _readlist(self, fmt: Union[str, List[Union[str, int]]], pos: int, **kwargs: int)\
+    def _readlist(self, fmt: Union[str, List[Union[str, int]]], pos: int, **kwargs: int) \
             -> Tuple[List[Union[float, int, str, None, Bits]], int]:
         tokens: List[Tuple[str, Optional[Union[str, int]], Optional[str]]] = []
         if isinstance(fmt, str):
             fmt = [fmt]
         keys = tuple(sorted(kwargs.keys()))
 
         def convert_length_strings(length_: Optional[Union[str, int]]) -> Optional[int]:
@@ -2499,89 +2175,14 @@
             value, newpos = self._readtoken(name, pos, length)
             bits_left -= newpos - pos
             pos = newpos
             if value is not None:
                 return_values.append(value)
         return return_values, pos
 
-    def _findbytes(self, bytes_: bytes, start: int, end: int) -> Union[Tuple[int], Tuple[()]]:
-        """Quicker version of find when everything's whole byte
-        and byte aligned.
-
-        """
-        assert self._datastore.offset == 0
-        # Extract data bytes from bitstring to be found.
-        bytepos = (start + 7) // 8
-        found = False
-        p = bytepos
-        finalpos = end // 8
-        increment = max(1024, len(bytes_) * 10)
-        buffersize = increment + len(bytes_)
-        while p < finalpos:
-            # Read in file or from memory in overlapping chunks and search the chunks.
-            buf = bytearray(self._datastore.getbyteslice(p, min(p + buffersize, finalpos)))
-            pos: int = buf.find(bytes_)
-            if pos != -1:
-                found = True
-                p += pos
-                break
-            p += increment
-        if not found:
-            return ()
-        return (p * 8,)
-
-    def _findbin(self, binstr: str, start: int, end: int, bytealigned: bool) -> Union[Tuple[int], Tuple[()]]:
-        """Find first occurrence of a binary string."""
-        p = start
-        length = len(binstr)
-        # We grab overlapping chunks of the binary representation and
-        # do an ordinary string search within that.
-        increment = max(4096, length * 64)
-        buffersize = increment + length
-        while p < end:
-            buf = self._readbin(p, min(buffersize, end - p))
-            pos = buf.find(binstr)
-            if pos != -1:
-                if not bytealigned:
-                    return (p + pos,)
-                if (p + pos) % 8 == 0:  # TODO: Is this logic only right for MSB0?
-                    return (p + pos,)
-                # Advance to just beyond the non-byte-aligned match and try again...
-                p += pos + 1
-                continue
-            p += increment
-        # Not found, return empty tuple
-        return ()
-
-    def _rfindbin(self, binstr: str, start: int, end: int, bytealigned: bool) -> Union[Tuple[int], Tuple[()]]:
-        """Find final occurrence of a binary string."""
-        p = end
-        # We grab overlapping chunks of the binary representation and
-        # do an ordinary string search within that.
-        increment = max(4096, len(binstr) * 64)
-        buffersize = increment + len(binstr)
-        while p > start:
-            start_pos = max(start, p - buffersize)
-            if not _lsb0:
-                buf = self._readbin(start_pos, p - start_pos)
-            else:
-                buf = self._readbin(self.len - p, p - start_pos)
-            pos = buf.rfind(binstr)
-            if pos != -1:
-                if not bytealigned:
-                    return (pos + start_pos,)
-                if (pos + start_pos) % 8 == 0:
-                    return (pos + start_pos,)
-                # Advance to just beyond the non-byte-aligned match and try again...
-                p = pos + start_pos + len(binstr) - 1
-                continue
-            p -= increment
-        # Not found, return empty tuple
-        return ()
-
     def find(self, bs: BitsType, start: Optional[int] = None, end: Optional[int] = None,
              bytealigned: Optional[bool] = None) -> Union[Tuple[int], Tuple[()]]:
         """Find first occurrence of substring bs.
 
         Returns a single item tuple with the bit position if found, or an
         empty tuple if not found. The bit position (pos property) will
         also be set to the start of the substring if it is found.
@@ -2601,39 +2202,46 @@
 
         """
         bs = Bits(bs)
         if bs.len == 0:
             raise ValueError("Cannot find an empty bitstring.")
         start, end = self._validate_slice(start, end)
         ba = _bytealigned if bytealigned is None else bytealigned
-        return self._find(bs, start, end, ba)
+        p = self._find(bs, start, end, ba)
+        # If called from a class that has a pos, set it
+        if p and self._pos is not None:
+            self._pos = p[0]
+        return p
 
     def _find_lsb0(self, bs: Bits, start: int, end: int, bytealigned: bool) -> Union[Tuple[int], Tuple[()]]:
+        # A forward find in lsb0 is very like a reverse find in msb0.
         assert start <= end
-        p = self._rfindbin(bs._getbin(), start, end, bytealigned)
+        assert _lsb0
+
+        new_slice = _offset_slice_indices_lsb0(slice(start, end, None), len(self), 0)
+        msb0_start, msb0_end = self._validate_slice(new_slice.start, new_slice.stop)
+        p = self._rfind_msb0(bs, msb0_start, msb0_end, bytealigned)
 
         if p:
-            newpos = self.length - p[0] - bs.length
-            if self._pos is not None:
-                self._pos = newpos
-            return (newpos,)
+            return (self.length - p[0] - bs.length,)
         else:
             return ()
 
     def _find_msb0(self, bs: Bits, start: int, end: int, bytealigned: bool) -> Union[Tuple[int], Tuple[()]]:
-        if bytealigned and not bs.len % 8 and not self._datastore.offset:
-            p = self._findbytes(bs.bytes, start, end)
-        else:
-            p = self._findbin(bs._getbin(), start, end, bytealigned)
-        # If called from a class that has a pos, set it
-        if p and self._pos is not None:
-            self._pos = p[0]
-        return p
+        """Find first occurrence of a binary string."""
+        while True:
+            p = self._bitstore.find(bs._bitstore, start, end)
+            if p == -1:
+                return ()
+            if not bytealigned or (p % 8) == 0:
+                return (p,)
+            # Advance to just beyond the non-byte-aligned match and try again...
+            start = p + 1
 
-    def findall(self, bs: Any, start: Optional[int] = None, end: Optional[int] = None, count: Optional[int] = None,
+    def findall(self, bs: BitsType, start: Optional[int] = None, end: Optional[int] = None, count: Optional[int] = None,
                 bytealigned: Optional[bool] = None) -> Generator[int, None, None]:
         """Find all occurrences of bs. Return generator of bit positions.
 
         bs -- The bitstring to find.
         start -- The bit position to start the search. Defaults to 0.
         end -- The bit position one past the last bit to search.
                Defaults to len(self).
@@ -2653,63 +2261,59 @@
         start, end = self._validate_slice(start, end)
         ba = _bytealigned if bytealigned is None else bytealigned
         return self._findall(bs, start, end, count, ba)
 
     def _findall_msb0(self, bs: Bits, start: int, end: int, count: Optional[int],
                       bytealigned: bool) -> Generator[int, None, None]:
         c = 0
-        if bytealigned and not bs.len % 8 and not self._datastore.offset:
-            # Use the quick find method
-            f = functools.partial(self._findbytes, bytes_=bs._getbytes())
-        else:
-            f = functools.partial(self._findbin, binstr=bs._getbin(), bytealigned=bytealigned)
-        while True:
+        for i in self._bitstore.getslice_msb0(slice(start, end, None)).itersearch(bs._bitstore):
             if count is not None and c >= count:
                 return
-            p = f(start=start, end=end)
-            if not p:
-                break
-            c += 1
-            if self._pos is not None:
-                self._pos = p[0]
-            yield p[0]
             if bytealigned:
-                start = p[0] + 8
+                if (start + i) % 8 == 0:
+                    c += 1
+                    yield start + i
             else:
-                start = p[0] + 1
-            if start >= end:
-                break
+                c += 1
+                yield start + i
         return
 
     def _findall_lsb0(self, bs: Bits, start: int, end: int, count: Optional[int],
                       bytealigned: bool) -> Generator[int, None, None]:
         assert start <= end
+        assert _lsb0
+
+        new_slice = _offset_slice_indices_lsb0(slice(start, end, None), len(self), 0)
+        msb0_start, msb0_end = self._validate_slice(new_slice.start, new_slice.stop)
+
         # Search chunks starting near the end and then moving back.
         c = 0
         increment = max(8192, bs.len * 80)
-        buffersize = min(increment + bs.len, end - start)
-        pos = max(start, end - buffersize)
+        buffersize = min(increment + bs.len, msb0_end - msb0_start)
+        pos = max(msb0_start, msb0_end - buffersize)
         while True:
-            found = list(self._findall_msb0(bs, start=pos, end=pos + buffersize, count=None,
-                                            bytealigned=bytealigned))
+            found = list(self._findall_msb0(bs, start=pos, end=pos + buffersize, count=None, bytealigned=False))
             if not found:
-                if pos == start:
+                if pos == msb0_start:
                     return
-                pos = max(start, pos - increment)
+                pos = max(msb0_start, pos - increment)
                 continue
             while found:
                 if count is not None and c >= count:
                     return
                 c += 1
-                yield self.len - found.pop() - bs.len
-            pos = max(start, pos - increment)
-            if pos == start:
+                lsb0_pos = self.len - found.pop() - bs.len
+                if not bytealigned or lsb0_pos % 8 == 0:
+                    yield lsb0_pos
+
+            pos = max(msb0_start, pos - increment)
+            if pos == msb0_start:
                 return
 
-    def rfind(self, bs: Any, start: Optional[int] = None, end: Optional[int] = None,
+    def rfind(self, bs: BitsType, start: Optional[int] = None, end: Optional[int] = None,
               bytealigned: Optional[bool] = None) -> Union[Tuple[int], Tuple[()]]:
         """Find final occurrence of substring bs.
 
         Returns a single item tuple with the bit position if found, or an
         empty tuple if not found. The bit position (pos property) will
         also be set to the start of the substring if it is found.
 
@@ -2732,24 +2336,39 @@
         p = self._rfind(bs, start, end, ba)
         # If called from a class that has a pos, set it
         if p and self._pos is not None:
             self._pos = p[0]
         return p
 
     def _rfind_msb0(self, bs: Bits, start: int, end: int, bytealigned: bool) -> Union[Tuple[int], Tuple[()]]:
-        return self._rfindbin(bs.bin, start, end, bytealigned)
+        """Find final occurrence of a binary string."""
+        increment = max(4096, len(bs) * 64)
+        buffersize = increment + len(bs)
+        p = end
+        while p > start:
+            start_pos = max(start, p - buffersize)
+            ps = list(self._findall_msb0(bs, start_pos, p, count=None, bytealigned=False))
+            if ps:
+                while ps:
+                    if not bytealigned or (ps[-1] % 8 == 0):
+                        return (ps[-1],)
+                    ps.pop()
+            p -= increment
+        return ()
 
     def _rfind_lsb0(self, bs: Bits, start: int, end: int, bytealigned: bool) -> Union[Tuple[int], Tuple[()]]:
         # A reverse find in lsb0 is very like a forward find in msb0.
-        p = self._find_msb0(bs, start, end, bytealigned)
+        assert start <= end
+        assert _lsb0
+        new_slice = _offset_slice_indices_lsb0(slice(start, end, None), len(self), 0)
+        msb0_start, msb0_end = self._validate_slice(new_slice.start, new_slice.stop)
+
+        p = self._find_msb0(bs, msb0_start, msb0_end, bytealigned)
         if p:
-            newpos = self.len - p[0] - bs.length
-            if self._pos is not None:
-                self._pos = newpos
-            return (newpos,)
+            return (self.len - p[0] - bs.length,)
         else:
             return ()
 
     def cut(self, bits: int, start: Optional[int] = None, end: Optional[int] = None,
             count: Optional[int] = None) -> Generator[Bits, None, None]:
         """Return bitstring generator by cutting into bits sized chunks.
 
@@ -2774,15 +2393,15 @@
                 return
             yield nextchunk
             if nextchunk._getlength() != bits:
                 return
             start_ += bits
         return
 
-    def split(self, delimiter: Any, start: Optional[int] = None, end: Optional[int] = None,
+    def split(self, delimiter: BitsType, start: Optional[int] = None, end: Optional[int] = None,
               count: Optional[int] = None, bytealigned: Optional[bool] = None) -> Generator[Bits, None, None]:
         """Return bitstring generator by splitting using a delimiter.
 
         The first item returned is the initial bitstring before the delimiter,
         which may be an empty bitstring.
 
         delimiter -- The bitstring used as the divider.
@@ -2793,27 +2412,23 @@
                  Default is to split as many times as possible.
         bytealigned -- If True splits will only occur on byte boundaries.
 
         Raises ValueError if the delimiter is empty.
 
         """
         delimiter = Bits(delimiter)
-        if not delimiter.len:
+        if len(delimiter) == 0:
             raise ValueError("split delimiter cannot be empty.")
         start, end = self._validate_slice(start, end)
         bytealigned_: bool = _bytealigned if bytealigned is None else bytealigned
         if count is not None and count < 0:
             raise ValueError("Cannot split - count must be >= 0.")
         if count == 0:
             return
-        if bytealigned_ and not delimiter.len % 8 and not self._datastore.offset:
-            # Use the quick find method
-            f = functools.partial(self._findbytes, bytes_=delimiter._getbytes())
-        else:
-            f = functools.partial(self._findbin, binstr=delimiter._getbin(), bytealigned=bytealigned_)
+        f = functools.partial(self._find_msb0, bs=delimiter, bytealigned=bytealigned_)
         found = f(start=start, end=end)
         if not found:
             # Initial bits are the whole bitstring being searched
             yield self._slice(start, end)
             return
         # yield the bytes before the first occurrence of the delimiter, even if empty
         yield self._slice(start, found[0])
@@ -2852,65 +2467,45 @@
 
     def tobytes(self) -> bytes:
         """Return the bitstring as bytes, padding with zero bits if needed.
 
         Up to seven zero bits will be added at the end to byte align.
 
         """
-        d = offsetcopy(self._datastore, 0).rawbytes
-        # Need to ensure that unused bits at end are set to zero
-        unusedbits = 8 - self.len % 8
-        if unusedbits != 8:
-            d[-1] &= (0xff << unusedbits)
-        return bytes(d)
+        return self._bitstore.tobytes()
+
+    def tobitarray(self) -> bitarray.bitarray:
+        """Convert the bitstring to a bitarray object."""
+        if self._bitstore.modified:
+            # Removes the offset and truncates to length
+            return bitarray.bitarray(self._bitstore.copy())
+        else:
+            return bitarray.bitarray(self._bitstore)
 
     def tofile(self, f: BinaryIO) -> None:
         """Write the bitstring to a file object, padding with zero bits if needed.
 
         Up to seven zero bits will be added at the end to byte align.
 
         """
-        # If the bitstring is file based then we don't want to read it all
-        # in to memory.
-        chunksize = 1024 * 1024  # 1 MiB chunks
-        if self._offset == 0:
-            a = 0
-            bytelen = self._datastore.bytelength
-            p = self._datastore.getbyteslice(a, min(a + chunksize, bytelen - 1))
-            while len(p) == chunksize:
-                f.write(p)
-                a += chunksize
-                p = self._datastore.getbyteslice(a, min(a + chunksize, bytelen - 1))
-            f.write(p)
-            # Now the final byte, ensuring that unused bits at end are set to 0.
-            bits_in_final_byte = self.len % 8
-            if not bits_in_final_byte:
-                bits_in_final_byte = 8
-            f.write(self[-bits_in_final_byte:].tobytes())
-        else:
-            # Really quite inefficient...
-            a = 0
-            b = a + chunksize * 8
-            while b <= self.len:
-                f.write(self._slice(a, b)._getbytes())
-                a += chunksize * 8
-                b += chunksize * 8
-            if a != self.len:
-                f.write(self._slice(a, self.len).tobytes())
+        # If the bitstring is file based then we don't want to read it all in to memory first.
+        chunk_size = 8 * 100 * 1024 * 1024  # 100 MiB
+        for chunk in self.cut(chunk_size):
+            f.write(chunk.tobytes())
 
     def startswith(self, prefix: BitsType, start: Optional[int] = None, end: Optional[int] = None) -> bool:
         """Return whether the current bitstring starts with prefix.
 
         prefix -- The bitstring to search for.
         start -- The bit position to start from. Defaults to 0.
         end -- The bit position to end at. Defaults to len(self).
 
         """
         prefix = Bits(prefix)
-        start, end = self._validate_slice_msb0(start, end)  # the _slice deals with msb0/lsb0
+        start, end = self._validate_slice(start, end)
         if end < start + prefix._getlength():
             return False
         end = start + prefix._getlength()
         return self._slice(start, end) == prefix
 
     def endswith(self, suffix: BitsType, start: Optional[int] = None, end: Optional[int] = None) -> bool:
         """Return whether the current bitstring ends with suffix.
@@ -2935,21 +2530,24 @@
         pos -- An iterable of bit positions. Negative numbers are treated in
                the same way as slice indices. Defaults to the whole bitstring.
 
         """
         value = bool(value)
         length = self.len
         if pos is None:
-            pos = range(self.len)
+            if value is True:
+                return self._bitstore.all_set()
+            else:
+                return not self._bitstore.any_set()
         for p in pos:
             if p < 0:
                 p += length
             if not 0 <= p < length:
                 raise IndexError(f"Bit position {p} out of range.")
-            if not self._datastore.getbit(p) is value:
+            if not bool(self._bitstore.getindex(p)) is value:
                 return False
         return True
 
     def any(self, value: Any, pos: Optional[Iterable[int]] = None) -> bool:
         """Return True if any of one or many bits are set to bool(value).
 
         value -- If value is True then checks for bits set to 1, otherwise
@@ -2957,36 +2555,39 @@
         pos -- An iterable of bit positions. Negative numbers are treated in
                the same way as slice indices. Defaults to the whole bitstring.
 
         """
         value = bool(value)
         length = self.len
         if pos is None:
-            pos = range(self.len)
+            if value is True:
+                return self._bitstore.any_set()
+            else:
+                return not self._bitstore.all_set()
         for p in pos:
             if p < 0:
                 p += length
             if not 0 <= p < length:
                 raise IndexError(f"Bit position {p} out of range.")
-            if self._datastore.getbit(p) is value:
+            if bool(self._bitstore.getindex(p)) is value:
                 return True
         return False
 
     def count(self, value: Any) -> int:
         """Return count of total number of either zero or one bits.
 
         value -- If bool(value) is True then bits set to 1 are counted, otherwise bits set
                  to 0 are counted.
 
         >>> Bits('0xef').count(1)
         7
 
         """
         # count the number of 1s (from which it's easy to work out the 0s).
-        count = (self._getbin()).count('1')
+        count = self._bitstore.count(1)
         return count if value else self.len - count
 
     def pp(self, fmt: str = 'bin', width: int = 120, sep: Optional[str] = ' ',
            show_offset: bool = True, stream: TextIO = sys.stdout) -> None:
         """Pretty print the bitstring's value.
 
         fmt -- Printed data format. One of 'bin', 'oct', 'hex' or 'bytes'. Defaults to 'bin'.
@@ -3173,15 +2774,14 @@
         _setuintne = _setuintbe
         _readuintne = _readuintbe
         _getuintne = _getuintbe
         _setintne = _setintbe
         _readintne = _readintbe
         _getintne = _getintbe
 
-    _offset = property(_getoffset)
 
     len = property(_getlength,
                    doc="""The length of the bitstring in bits. Read only.
                       """)
     length = property(_getlength,
                       doc="""The length of the bitstring in bits. Read only.
                       """)
@@ -3324,16 +2924,17 @@
                 'floatbe': _setfloatbe,
                 'uintle': _setuintle,
                 'intle': _setintle,
                 'floatle': _setfloatle,
                 'uintne': _setuintne,
                 'intne': _setintne,
                 'floatne': _setfloatne,
-                'bytes': _setbytes_safe,
-                'filename': _setfile}
+                'bytes': _setbytes,
+                'filename': _setfile,
+                'bitarray': _setbitarray}
 
 
 class BitArray(Bits):
     """A container holding a mutable sequence of bits.
 
     Subclass of the immutable Bits class. Inherits all of its
     methods (except __hash__) and adds mutating methods.
@@ -3406,26 +3007,20 @@
     len -- Length of the bitstring in bits.
 
     """
 
     @classmethod
     def _setlsb0methods(cls, lsb0: bool) -> None:
         if lsb0:
-            cls._overwrite = cls._overwrite_lsb0  # type: ignore
-            cls._insert = cls._insert_lsb0  # type: ignore
-            cls._delete = cls._delete_lsb0  # type: ignore
             cls._ror = cls._rol_msb0  # type: ignore
             cls._rol = cls._ror_msb0  # type: ignore
             cls._append = cls._append_lsb0  # type: ignore
             # An LSB0 prepend is an MSB0 append
             cls._prepend = cls._append_msb0  # type: ignore
         else:
-            cls._overwrite = cls._overwrite_msb0  # type: ignore
-            cls._insert = cls._insert_msb0  # type: ignore
-            cls._delete = cls._delete_msb0  # type: ignore
             cls._ror = cls._ror_msb0  # type: ignore
             cls._rol = cls._rol_msb0  # type: ignore
             cls._append = cls._append_msb0  # type: ignore
             cls._prepend = cls._append_lsb0  # type: ignore
 
     __slots__ = ()
 
@@ -3468,27 +3063,19 @@
         length -- length of the bitstring in bits, if needed and appropriate.
                   It must be supplied for all integer and float initialisers.
         offset -- bit offset to the data. These offset bits are
                   ignored and this is intended for use when
                   initialising using 'bytes' or 'filename'.
 
         """
-        # For mutable BitArrays we always read in files to memory:
-        super().__init__()
-
-    def __new__(cls, auto: Optional[BitsType] = None, length: Optional[int] = None,
-                offset: Optional[int] = None, **kwargs) -> Bits:
-        x = super(BitArray, cls).__new__(cls)
-        y = Bits.__new__(BitArray, auto, length, offset, **kwargs)
-        x._datastore = ByteStore(y._datastore.rawarray[:],
-                                 y._datastore.bitlength,
-                                 y._datastore.offset)
-        return x
+        if self._bitstore.immutable:
+            self._bitstore = self._bitstore.copy()
+            self._bitstore.immutable = False
 
-    def __setattr__(self, attribute, value):
+    def __setattr__(self, attribute, value) -> None:
         try:
             # First try the ordinary attribute setter
             super().__setattr__(attribute, value)
         except AttributeError:
             letter_to_setter: Dict[str, Callable[..., None]] =\
                 {'u': self._setuint,
                  'i': self._setint,
@@ -3498,25 +3085,21 @@
                  'h': self._sethex}
             short_token: Pattern[str] = re.compile(r'^(?P<name>[uifboh])(?P<len>\d+)$', re.IGNORECASE)
             m1_short = short_token.match(attribute)
             if m1_short:
                 length = int(m1_short.group('len'))
                 name = m1_short.group('name')
                 f = letter_to_setter[name]
-                a_copy = self._copy()
                 try:
                     f(value, length)
                 except AttributeError:
                     raise AttributeError(f"Can't set attribute {attribute} with value {value}.")
 
                 if self.len != length:
                     new_len = self.len
-                    # Reset to previous value
-                    self._setbytes_unsafe(a_copy._datastore.getbyteslice(0, a_copy._datastore.bytelength),
-                                          a_copy.len, a_copy._offset)
                     raise CreationError(f"Can't initialise with value of length {new_len} bits, "
                                         f"as attribute has length of {length} bits.")
                 return
             # Try to split into [name][length], then try standard properties
             name_length_pattern: Pattern[str] = re.compile(r'^(?P<name>[a-z]+)(?P<len>\d+)$', re.IGNORECASE)
             name_length = name_length_pattern.match(attribute)
             if name_length:
@@ -3525,23 +3108,15 @@
                 if length is not None:
                     length = int(length)
                     if name == 'bytes':
                         if len(value) != length:
                             raise CreationError(f"Wrong amount of byte data preset - {length} bytes needed, have {len(value)} bytes.")
                         length *= 8
                 try:
-                    a_copy = self._copy()
                     self._initialise(auto=None, length=length, offset=None, **{name: value})
-                    if length is not None and self.len != length:
-                        new_len = self.len
-                        # Reset to previous value
-                        self._setbytes_unsafe(a_copy._datastore.getbyteslice(0, a_copy._datastore.bytelength),
-                                              a_copy.len, a_copy._offset)
-                        raise CreationError(f"Can't initialise with value of length {new_len} bits, "
-                                            f"as attribute has length of {length} bits.")
                     return
                 except AttributeError:
                     pass
             raise AttributeError(f"Can't set attribute {attribute} with value {value}.")
 
     def __iadd__(self, bs: BitsType) -> BitArray:
         """Append bs to current bitstring. Return self.
@@ -3551,159 +3126,100 @@
         """
         self._append(bs)
         return self
 
     def __copy__(self) -> BitArray:
         """Return a new copy of the BitArray."""
         s_copy = BitArray()
-        if not isinstance(self._datastore, ByteStore):
-            # Let them both point to the same (invariant) array.
-            # If either gets modified then at that point they'll be read into memory.
-            s_copy._datastore = self._datastore
-        else:
-            s_copy._datastore = copy.copy(self._datastore)
+        s_copy._bitstore = self._bitstore.copy()
+        assert s_copy._bitstore.immutable == False
         return s_copy
     
     def __setitem__(self, key: Union[slice, int], value: BitsType) -> None:
-        if isinstance(key, slice):
-            # A slice
-            start, step = 0, 1
-            if key.step is not None:
-                step = key.step
-            if step != 1:
-                # convert to binary string and use string slicing
-                # TODO: Horribly inefficient
-                temp = list(self._getbin())
-                v = list(Bits(value)._getbin())
-                temp.__setitem__(key, v)
-                self._setbin_unsafe(''.join(temp))
-                return
-
-            # If value is an integer then we want to set the slice to that
-            # value rather than initialise a new bitstring of that length.
-            if not isinstance(value, int):
-                try:
-                    value = Bits(value)
-                except TypeError:
-                    raise TypeError(f"Bitstring, integer or string expected. Got {type(value)}.")
-            if key.start is not None:
-                start = key.start
-                if key.start < 0:
-                    start += self.len
-                if start < 0:
-                    start = 0
-            stop = self.len
-            if key.stop is not None:
-                stop = key.stop
-                if key.stop < 0:
-                    stop += self.len
-            if start > stop:
-                # The standard behaviour for lists is to just insert at the
-                # start position if stop < start and step == 1.
-                stop = start
-            if isinstance(value, int):
-                if value >= 0:
-                    value = self.__class__(uint=value, length=stop - start)
-                else:
-                    value = self.__class__(int=value, length=stop - start)
-            stop = min(stop, self.len)
-            start = max(start, 0)
-            start = min(start, stop)
-            if (stop - start) == value._getlength():
-                if value.len == 0:
-                    return
-                if step >= 0:
-                    self._overwrite(value, start)
-                else:
-                    self._overwrite(value.__getitem__(slice(None, None, 1)), start)
-            else:
-                # TODO: A delete then insert is wasteful - it could do unneeded shifts.
-                # Could be either overwrite + insert or overwrite + delete.
-                self._delete(stop - start, start)
-                if step >= 0:
-                    self._insert(value, start)
-                else:
-                    self._insert(value.__getitem__(slice(None, None, 1)), start)
-                # pos is now after the inserted piece.
-            return
-        else:
-            # single element
-            if key < 0:
-                key += self._getlength()
-            if not 0 <= key < self.len:
-                raise IndexError("Slice index out of range.")
+        length_before = self.len
+        if isinstance(key, int):
             if isinstance(value, int):
-                if not value:
-                    self._unset(key)
+                if value == 0:
+                    self._bitstore[key] = 0
                     return
                 if value in (1, -1):
-                    self._set(key)
+                    self._bitstore[key] = 1
                     return
                 raise ValueError(f"Cannot set a single bit with integer {value}.")
-            value = Bits(value)
-            if value.len == 1:
-                if value[0]:
-                    self._set(key)
+            else:
+                try:
+                    value = Bits(value)
+                except TypeError:
+                    raise TypeError(f"Bitstring, integer or string expected. Got {type(value)}.")
+                positive_key = key + self.len if key < 0 else key
+                if positive_key < 0 or positive_key >= len(self._bitstore):
+                    raise IndexError(f"Bit position {key} out of range.")
+                self._bitstore[positive_key: positive_key + 1] = value._bitstore
+                if self._pos is not None and self._pos >= positive_key:
+                    self._pos += self.len - length_before
+                return
+
+        assert isinstance(key, slice)
+        if isinstance(value, int):
+            if key.step not in [None, -1, 1]:
+                if value in [0, 1]:
+                    raise ValueError(f"Can't assign a single bit to a slice with a step value. "
+                                     f"Instead of 's[start:stop:step] = {value}' try 's.set({value}, range(start, stop, step))'.")
                 else:
-                    self._unset(key)
+                    raise ValueError("Can't assign an integer to a slice with a step value.")
+            # To find the length we first get the slice
+            s = self._bitstore.getslice(key)
+            length = len(s)
+            # Now create an int of the correct length
+            if value >= 0:
+                value = self.__class__(uint=value, length=length)
             else:
-                self._delete(1, key)
-                self._insert(value, key)
-            return
+                value = self.__class__(int=value, length=length)
+        else:
+            try:
+                value = Bits(value)
+            except TypeError:
+                raise TypeError(f"Bitstring, integer or string expected. Got {type(value)}.")
+        self._bitstore.__setitem__(key, value._bitstore)
+        if self._pos is not None:
+            start = key.start if key.start is not None else 0
+            positive_start = start if start >= 0 else start + self.len
+            if self._pos >= positive_start:
+                self._pos += self.len - length_before
+        return
 
     def __delitem__(self, key: Union[slice, int]) -> None:
         """Delete item or range.
 
         Indices are in units of the step parameter (default 1 bit).
         Stepping is used to specify the number of bits in each item.
 
         >>> a = BitArray('0x001122')
         >>> del a[1:2:8]
         >>> print a
         0x0022
 
         """
-        if isinstance(key, slice):
-            # A slice
-            start = 0
-            step = key.step if key.step is not None else 1
-            if step != 1:
-                # convert to binary string and use string slicing
-                # TODO: Horribly inefficient
-                temp = list(self._getbin())
-                temp.__delitem__(key)
-                self._setbin_unsafe(''.join(temp))
-                return
-            if key.start is not None:
-                start = key.start
-                if key.start < 0:
-                    start += self.len
-                if start < 0:
-                    start = 0
-            stop = self.len
-            if key.stop is not None:
-                stop = key.stop
-                if key.stop < 0:
-                    stop += self.len
-            if start > stop:
-                return
-            stop = min(stop, self.len)
-            start = max(start, 0)
-            start = min(start, stop)
-            self._delete(stop - start, start)
-            return
-        else:
-            # single element
-            if key < 0:
-                key += self._getlength()
-            if not 0 <= key < self._getlength():
-                raise IndexError("Slice index out of range.")
-            self._delete(1, key)
+        if self._pos is None:
+            self._bitstore.__delitem__(key)
             return
 
+        length_before = self.len
+        if isinstance(key, int):
+            start = key
+        else:
+            start = key.start if key.start is not None else 0
+        positive_start = start if start >= 0 else start + self.len
+        self._bitstore.__delitem__(key)
+        if self._pos >= positive_start:
+            self._pos += self.len - length_before
+            if self._pos < 0:
+                self._pos = 0
+        return
+
     def __ilshift__(self, n: int) -> Bits:
         """Shift bits by n to the left in place. Return self.
 
         n -- the number of bits to shift. Must be >= 0.
 
         """
         if n < 0:
@@ -3741,27 +3257,30 @@
             raise ValueError("Cannot multiply by a negative integer.")
         return self._imul(n)
 
     def __ior__(self, bs: BitsType) -> Bits:
         bs = Bits(bs)
         if self.len != bs.len:
             raise ValueError("Bitstrings must have the same length for |= operator.")
-        return self._ior(bs)
+        self._bitstore |= bs._bitstore
+        return self
 
     def __iand__(self, bs: BitsType) -> Bits:
         bs = Bits(bs)
         if self.len != bs.len:
             raise ValueError("Bitstrings must have the same length for &= operator.")
-        return self._iand(bs)
+        self._bitstore &= bs._bitstore
+        return self
 
     def __ixor__(self, bs: BitsType) -> Bits:
         bs = Bits(bs)
         if self.len != bs.len:
             raise ValueError("Bitstrings must have the same length for ^= operator.")
-        return self._ixor(bs)
+        self._bitstore ^= bs._bitstore
+        return self
 
     def replace(self, old: BitsType, new: BitsType, start: Optional[int] = None, end: Optional[int] = None,
                 count: Optional[int] = None, bytealigned: Optional[bool] = None) -> int:
         """Replace all occurrences of old with new in place.
 
         Returns number of replacements made.
 
@@ -3776,73 +3295,78 @@
         bytealigned -- If True replacements will only be made on byte
                        boundaries.
 
         Raises ValueError if old is empty or if start or end are
         out of range.
 
         """
+        if count == 0:
+            return 0
         old = Bits(old)
         new = Bits(new)
         if not old.len:
             raise ValueError("Empty bitstring cannot be replaced.")
         start, end = self._validate_slice(start, end)
         if bytealigned is None:
             bytealigned = _bytealigned
-        # Adjust count for use in split()
-        if count is not None:
-            count += 1
-        sections = self.split(old, start, end, count, bytealigned)
-        lengths = [s.len for s in sections]
-        if len(lengths) == 1:
-            # Didn't find anything to replace.
-            return 0  # no replacements done
         if new is self:
             # Prevent self assignment woes
             new = copy.copy(self)
-        positions = [lengths[0] + start]
-        for le in lengths[1:-1]:
-            # Next position is the previous one plus the length of the next section.
-            positions.append(positions[-1] + le)
-        # We have all the positions that need replacements. We do them
-        # in reverse order so that they won't move around as we replace.
-        positions.reverse()
-        if self._pos is not None:
-            # Need to calculate new pos, if this is a bitstream
-            newpos = self._pos
-            for p in positions:
-                self[p:p + old.len] = new
-            if old.len != new.len:
-                diff = new.len - old.len
-                for p in positions:
-                    if p >= newpos:
-                        continue
-                    if p + old.len <= newpos:
-                        newpos += diff
-                    else:
-                        newpos = p
-            self._pos = newpos
-        else:
-            for p in positions:
-                self[p:p + old.len] = new
-        return len(lengths) - 1
+
+        # First find all the places where we want to do the replacements
+        starting_points: List[int] = []
+        for x in self.findall(old, start, end, bytealigned=bytealigned):
+            if not starting_points:
+                starting_points.append(x)
+            elif x >= starting_points[-1] + old.len:
+                # Can only replace here if it hasn't already been replaced!
+                starting_points.append(x)
+            if len(starting_points) == count:
+                break
+        if not starting_points:
+            return 0
+        replacement_list = [self._bitstore.getslice(slice(0, starting_points[0], None))]
+        for i in range(len(starting_points) - 1):
+            replacement_list.append(new._bitstore)
+            replacement_list.append(self._bitstore.getslice(slice(starting_points[i] + old.len, starting_points[i + 1], None)))
+        # Final replacement
+        replacement_list.append(new._bitstore)
+        replacement_list.append(self._bitstore.getslice(slice(starting_points[-1] + old.len, None, None)))
+        if _lsb0:
+            # Addition of bitarray is always on the right, so assemble from other end
+            replacement_list.reverse()
+        self._bitstore.clear()
+        for r in replacement_list:
+            self._bitstore += r
+
+        if self._pos is not None and self._pos > starting_points[0]:
+            # Need to adjust our position in the bitstring
+            oldpos = self._pos
+            for starting_point in starting_points:
+                if oldpos > starting_point:
+                    if oldpos < starting_point + old.len:
+                        self._pos = starting_point + new.len
+                        break
+                    self._pos += new.len - old.len
+        return len(starting_points)
 
     def insert(self, bs: BitsType, pos: Optional[int] = None) -> None:
         """Insert bs at bit position pos.
 
         bs -- The bitstring to insert.
         pos -- The bit position to insert at.
 
         Raises ValueError if pos < 0 or pos > len(self).
 
         """
         bs = Bits(bs)
         if not bs.len:
             return
         if bs is self:
-            bs = self.__copy__()
+            bs = self._copy()
         if pos is None:
             pos = self._pos
             if pos is None:
                 raise TypeError("insert needs a bit position specified when used on a BitArray.")
         if pos < 0:
             pos += self._getlength()
         if not 0 <= pos <= self._getlength():
@@ -3886,17 +3410,15 @@
 
         bs -- The bitstring to prepend.
 
         """
         self._prepend(bs)
 
     def _append_msb0(self, bs: BitsType) -> None:
-        # The offset is a hint to make bs easily appendable.
-        bs = self._converttobitstring(bs, offset=(self.len + self._offset) % 8)
-        self._addright(bs)
+        self._addright(Bits(bs))
 
     def _append_lsb0(self, bs: BitsType) -> None:
         bs = Bits(bs)
         self._addleft(bs)
 
     def reverse(self, start: Optional[int] = None, end: Optional[int] = None) -> None:
         """Reverse bits in-place.
@@ -3908,18 +3430,18 @@
         Using on an empty bitstring will have no effect.
 
         Raises ValueError if start < 0, end > len(self) or end < start.
 
         """
         start, end = self._validate_slice(start, end)
         if start == 0 and end == self.len:
-            self._reverse()
+            self._bitstore.reverse()
             return
         s = self._slice(start, end)
-        s._reverse()
+        s._bitstore.reverse()
         self[start:end] = s
 
     def set(self, value: Any, pos: Optional[Union[int, Iterable[int]]] = None) -> None:
         """Set one or many bits to 1 or 0.
 
         value -- If bool(value) is True bits are set to 1, otherwise they are set to 0.
         pos -- Either a single bit position or an iterable of bit positions.
@@ -3929,24 +3451,22 @@
         Raises IndexError if pos < -len(self) or pos >= len(self).
 
         """
         if pos is None:
             # Set all bits to either 1 or 0
             self._setint(-1 if value else 0)
             return
-        f = self._set if value else self._unset
         if not isinstance(pos, abc.Iterable):
             pos = (pos,)
-        length = self.len
+        v = 1 if value else 0
+        if isinstance(pos, range):
+            self._bitstore.__setitem__(slice(pos.start, pos.stop, pos.step), v)
+            return
         for p in pos:
-            if p < 0:
-                p += length
-            if not 0 <= p < length:
-                raise IndexError(f"Bit position {p} out of range.")
-            f(p)
+            self._bitstore[p] = v
 
     def invert(self, pos: Optional[Union[Iterable[int], int]] = None) -> None:
         """Invert one or many bits from 0 to 1 or vice versa.
 
         pos -- Either a single bit position or an iterable of bit positions.
                Negative numbers are treated in the same way as slice indices.
 
@@ -3980,15 +3500,15 @@
         if not self.len:
             raise Error("Cannot rotate an empty bitstring.")
         if bits < 0:
             raise ValueError("Cannot rotate by negative amount.")
         self._ror(bits, start, end)
 
     def _ror_msb0(self, bits: int, start: Optional[int] = None, end: Optional[int] = None) -> None:
-        start, end = self._validate_slice_msb0(start, end)  # the _slice deals with msb0/lsb0
+        start, end = self._validate_slice(start, end)  # the _slice deals with msb0/lsb0
         bits %= (end - start)
         if not bits:
             return
         rhs = self._slice(end - bits, end)
         self._delete(bits, end - bits)
         self._insert(rhs, start)
 
@@ -4005,17 +3525,17 @@
         if not self.len:
             raise Error("Cannot rotate an empty bitstring.")
         if bits < 0:
             raise ValueError("Cannot rotate by negative amount.")
         self._rol(bits, start, end)
 
     def _rol_msb0(self, bits: int, start: Optional[int] = None, end: Optional[int] = None):
-        start, end = self._validate_slice_msb0(start, end)
+        start, end = self._validate_slice(start, end)
         bits %= (end - start)
-        if not bits:
+        if bits == 0:
             return
         lhs = self._slice(start, start + bits)
         self._delete(bits, start)
         self._insert(lhs, end - bits)
 
     def byteswap(self, fmt: Optional[Union[int, Iterable[int], str]] = None, start: Optional[int] = None,
                  end: Optional[int] = None, repeat: bool = True) -> int:
@@ -4141,15 +3661,15 @@
                        """)
     oct = property(Bits._getoct, Bits._setoct,
                    doc="""The bitstring as an octal string. Read and write.
                        """)
     bool = property(Bits._getbool, Bits._setbool,
                     doc="""The bitstring as a bool (True or False). Read and write.
                     """)
-    bytes = property(Bits._getbytes, Bits._setbytes_safe,
+    bytes = property(Bits._getbytes, Bits._setbytes,
                      doc="""The bitstring as a ordinary string. Read and write.
                       """)
     # Aliases for some properties
     f = float
     i = int
     u = uint
     b = bin
@@ -4263,24 +3783,20 @@
                   It must be supplied for all integer and float initialisers.
         offset -- bit offset to the data. These offset bits are
                   ignored and this is mainly intended for use when
                   initialising using 'bytes' or 'filename'.
         pos -- Initial bit position, defaults to 0.
 
         """
-        pass
-
-    def __new__(cls, auto: Optional[BitsType] = None, length: Optional[int] = None,
-                offset: Optional[int] = None, pos: int = 0, **kwargs) -> Bits:
-        x = super(ConstBitStream, cls).__new__(cls)
-        x._initialise(auto, length, offset, **kwargs)
-        x._pos = x._datastore.bitlength + pos if pos < 0 else pos
-        if x._pos < 0 or x._pos > x._datastore.bitlength:
-            raise CreationError(f"Cannot set pos to {pos} when length is {x._datastore.bitlength}.")
-        return x
+        if pos < 0:
+            pos += len(self._bitstore)
+        if pos < 0 or pos > len(self._bitstore):
+            raise CreationError(f"Cannot set pos to {pos} when length is {len(self._bitstore)}.")
+        self._pos = pos
+        self._bitstore.immutable = True
 
     def _setbytepos(self, bytepos: int) -> None:
         """Move to absolute byte-aligned position in stream."""
         self._setbitpos(bytepos * 8)
 
     def _getbytepos(self) -> int:
         """Return the current position in the stream in bytes. Must be byte aligned."""
@@ -4305,15 +3821,15 @@
         self._pos = 0
 
     def __copy__(self) -> ConstBitStream:
         """Return a new copy of the ConstBitStream for the copy module."""
         # Note that if you want a new copy (different ID), use _copy instead.
         # The copy can use the same datastore as it's immutable.
         s = ConstBitStream()
-        s._datastore = self._datastore
+        s._bitstore = self._bitstore
         # Reset the bit position, don't copy it.
         s._pos = 0
         return s
 
     def __add__(self, bs: BitsType) -> Bits:
         """Concatenate bitstrings and return new bitstring.
 
@@ -4472,29 +3988,29 @@
         """Align to next byte and return number of skipped bits.
 
         Raises ValueError if the end of the bitstring is reached before
         aligning to the next byte.
 
         """
         skipped = (8 - (self._pos % 8)) % 8
-        self.pos += self._offset + skipped
+        self.pos += skipped
         return skipped
 
     pos = property(_getbitpos, _setbitpos,
                    doc="""The position in the bitstring in bits. Read and write.
                       """)
     bitpos = property(_getbitpos, _setbitpos,
                       doc="""The position in the bitstring in bits. Read and write.
                       """)
     bytepos = property(_getbytepos, _setbytepos,
                        doc="""The position in the bitstring in bytes. Read and write.
                       """)
 
 
-class BitStream(ConstBitStream, BitArray):
+class BitStream(BitArray, ConstBitStream):
     """A container or stream holding a mutable sequence of bits
 
     Subclass of the ConstBitStream and BitArray classes. Inherits all of
     their methods.
 
     Methods:
 
@@ -4607,48 +4123,34 @@
                   It must be supplied for all integer and float initialisers.
         offset -- bit offset to the data. These offset bits are
                   ignored and this is intended for use when
                   initialising using 'bytes' or 'filename'.
         pos -- Initial bit position, defaults to 0.
 
         """
-        pass
-
-    def __new__(cls, auto: Optional[BitsType] = None, length: Optional[int] = None,
-                offset: Optional[int] = None, pos: int = 0, **kwargs) -> Bits:
-        x = super(BitStream, cls).__new__(cls)
-        y = ConstBitStream.__new__(BitStream, auto, length, offset, pos, **kwargs)
-        x._datastore = ByteStore(y._datastore.rawarray[:],
-                                 y._datastore.bitlength,
-                                 y._datastore.offset)
-        x._pos = y._pos
-        return x
+        ConstBitStream.__init__(self, auto, length, offset, pos, **kwargs)
+        if self._bitstore.immutable:
+            self._bitstore = self._bitstore.copy()
+            self._bitstore.immutable = False
 
     def __copy__(self) -> BitStream:
         """Return a new copy of the BitStream."""
         s_copy = BitStream()
         s_copy._pos = 0
-        if not isinstance(self._datastore, ByteStore):
-            # Let them both point to the same (invariant) array.
-            # If either gets modified then at that point they'll be read into memory.
-            s_copy._datastore = self._datastore
-        else:
-            s_copy._datastore = ByteStore(self._datastore.rawarray[:],
-                                          self._datastore.bitlength,
-                                          self._datastore.offset)
+        s_copy._bitstore = self._bitstore.copy()
         return s_copy
 
     def prepend(self, bs: BitsType) -> None:
         """Prepend a bitstring to the current bitstring.
 
         bs -- The bitstring to prepend.
 
         """
-        bs = self._converttobitstring(bs)
-        self._addleft(bs)
+        bs = Bits(bs)
+        super().prepend(bs)
         self._pos += bs.len
 
 
 def pack(fmt: Union[str, List[str]], *values, **kwargs) -> BitStream:
     """Pack the values according to the format string and return a new BitStream.
 
     fmt -- A single string or a list of strings with comma separated tokens
@@ -4726,15 +4228,15 @@
 # Whether to label the Least Significant Bit as bit 0. Default is False.
 
 def _switch_lsb0_methods(lsb0: bool) -> None:
     global _lsb0
     _lsb0 = lsb0
     Bits._setlsb0methods(lsb0)
     BitArray._setlsb0methods(lsb0)
-    ByteStore._setlsb0methods(lsb0)
+    BitStore._setlsb0methods(lsb0)
 
 
 # Initialise the default behaviour
 _switch_lsb0_methods(False)
 
 
 __all__ = ['ConstBitStream', 'BitStream', 'BitArray',
```

### Comparing `bitstring-4.0.2/bitstring.egg-info/PKG-INFO` & `bitstring-4.1.0b1/bitstring.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitstring
-Version: 4.0.2
+Version: 4.1.0b1
 Summary: Simple construction, analysis and modification of binary data.
 Author-email: Scott Griffiths <dr.scottgriffiths@gmail.com>
 Project-URL: homepage, https://github.com/scott-griffiths/bitstring
 Project-URL: documentation, https://bitstring.readthedocs.io/
 Keywords: binary,bitarray,bitvector
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,39 +19,54 @@
 
 
 ![bitstring](https://raw.githubusercontent.com/scott-griffiths/bitstring/main/doc/bitstring_logo_small.png "bitstring")
 
 **bitstring** is a pure Python module designed to help make
 the creation and analysis of binary data as simple and natural as possible.
 
-It has been maintained since 2006 and now has about 20 million downloads per year.
+It has been maintained since 2006 and now has many millions of downloads per year.
 
 
 You can try out the interactive walkthrough notebook on [binder](https://mybinder.org/v2/gh/scott-griffiths/bitstring/main?labpath=doc%2Fwalkthrough.ipynb), or take a look at the [static version](https://github.com/scott-griffiths/bitstring/blob/main/doc/walkthrough.ipynb).
 
 
 [![CI badge](https://github.com/scott-griffiths/bitstring/actions/workflows/.github/workflows/ci.yml/badge.svg)](https://github.com/scott-griffiths/bitstring/actions/workflows/ci.yml)
 [![Docs](https://img.shields.io/readthedocs/bitstring)](https://bitstring.readthedocs.io/en/latest/)
 [![Downloads](https://img.shields.io/pypi/dm/bitstring?color=blue)](https://pypistats.org/packages/bitstring) &nbsp; &nbsp; 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/scott-griffiths/bitstring/main?labpath=doc%2Fwalkthrough.ipynb)
 
+# \<<< 4.1 beta now available - the _speed_ update \>>>
+
+This version concentrats on what is perhaps bitstring's major weakness - speed.
+It's always been a pure Python module with no dependencies, which has a few advantages, but means it can't compete with C-coded extensions in terms of raw speed of operation.
+
+Version 4.1 of bitstring has been rewritten to use the `bitarray` type from the package of the same name as its underlying data type.
+This lets us keep the API and functionality of bitstring but gains (most of) the speed of bitarray.
+
+The 4.1 beta should be fully functional - there are no known issues.
+To install the beta you need to specify the precise version:
+
+    python -m pip install bitstring==4.1.0b1
+
+Please try it out and report any problems or observations.
+You shouldn't need to change any code - everything should just work the same as version 4.0, just faster.
 
 Overview
 --------
 
 * Create bitstrings from hex, octal, binary, files, formatted strings, bytes, integers and floats of different endiannesses.
 * Powerful binary packing and unpacking functions.
 * Bit-level slicing, joining, searching, replacing and more.
 * Read from and interpret bitstrings as streams of binary data.
 * Rich API - chances are that whatever you want to do there's a simple and elegant way of doing it.
 * Open source software, released under the MIT licence.
 
 
 > **Note** \
-> Version 4.0 of bitstring only supports Python 3.7 and later. \
+> Version 4 of bitstring only supports Python 3.7 and later. \
 > Use bitstring version 3.1 if you're using Python 2.7 or 3.6 or earlier.
 
 
 Documentation
 -------------
 The manual for the bitstring module is available at [Read the Docs](https://bitstring.readthedocs.org).
 It contains a walk-through of all the features and a complete [reference section](https://bitstring.readthedocs.io/en/stable/quick_ref.html).
```

### Comparing `bitstring-4.0.2/pyproject.toml` & `bitstring-4.1.0b1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bitstring"
-version = "4.0.2"
+version = "4.1.0b1"
 authors = [
   { name="Scott Griffiths", email="dr.scottgriffiths@gmail.com" },
 ]
 description = "Simple construction, analysis and modification of binary data."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -16,14 +16,17 @@
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = ["binary", "bitarray", "bitvector"]
+dependencies = [
+  "bitarray == 2.7.3",
+]
 
 [project.urls]
 homepage = "https://github.com/scott-griffiths/bitstring"
 documentation = "https://bitstring.readthedocs.io/"
 
 [tool.setuptools]
 packages = ["bitstring"]
```

### Comparing `bitstring-4.0.2/tests/test.m1v` & `bitstring-4.1.0b1/tests/test.m1v`

 * *Files identical despite different names*

### Comparing `bitstring-4.0.2/tests/test_bitarray.py` & `bitstring-4.1.0b1/tests/test_bitarray.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python
 """
 Unit tests for the bitarray module.
 """
 
 import unittest
 import sys
+import os
+import bitarray
 
 sys.path.insert(0, '..')
 import bitstring
 from bitstring import BitArray
 
 
 class All(unittest.TestCase):
@@ -133,14 +135,16 @@
             a += 'se'
         with self.assertRaises(ValueError):
             a += 'float:32'
 
     def testPrependAfterCreationFromDataWithOffset(self):
         s1 = BitArray(bytes=b'\x00\x00\x07\xff\xf0\x00', offset=21, length=15)
         self.assertFalse(s1.any(0))
+        b = s1.tobytes()
+        self.assertEqual(b, b'\xff\xfe')
         s1.prepend('0b0')
         self.assertEqual(s1.bin, '0111111111111111')
         s1.prepend('0b0')
         self.assertEqual(s1.bin, '00111111111111111')
 
 
 class ByteAligned(unittest.TestCase):
@@ -286,14 +290,25 @@
         a[7:1:-2] = [0, 0, 1]
         self.assertEqual(a.b, '1011001010')
         a[::-5] = [1, 1]
         self.assertEqual(a.bin, '1011101011')
         a[::-1] = [0, 0, 0, 0, 0, 0, 0, 0, 0, 1]
         self.assertEqual(a.bin, '1000000000')
 
+    def testSetSliceStepWithInt(self):
+        a = BitArray(9)
+        a[5:8] = -1
+        self.assertEqual(a.bin, '000001110')
+        a[:] = 10
+        self.assertEqual(a.bin, '000001010')
+        a[::-1] = 10
+        self.assertEqual(a.bin, '010100000')
+        with self.assertRaises(ValueError):
+            a[::2] = True
+
     def testSetSliceErrors(self):
         a = BitArray(8)
         with self.assertRaises(ValueError):
             a[::3] = [1]
 
         class A(object):
             pass
@@ -486,79 +501,88 @@
     def testRfind(self):
         a = BitArray('0b1000000')
         p = a.rfind('0b1')
         self.assertEqual(p, (6,))
         p = a.rfind('0b000')
         self.assertEqual(p, (3,))
 
-    # def testFindall(self):
-    #     a = BitArray('0b001000100001')
-    #     b = list(a.findall('0b1'))
-    #     self.assertEqual(b, [0, 5, 9])
-    #     c = list(a.findall('0b0001'))
-    #     self.assertEqual(c, [0, 5])
-    #     d = list(a.findall('0b10'))
-    #     self.assertEqual(d, [4, 8])
-    #     e = list(a.findall('0x198273641234'))
-    #     self.assertEqual(e, [])
-
-    # def testFindAllWithStartAndEnd(self):
-    #     a = BitArray('0xaabbccaabbccccbb')
-    #     b = list(a.findall('0xbb', start=0, end=8))
-    #     self.assertEqual(b, [0])
-    #     b = list(a.findall('0xbb', start=1, end=8))
-    #     self.assertEqual(b, [])
-    #     b = list(a.findall('0xbb', start=0, end=7))
-    #     self.assertEqual(b, [])
-    #     b = list(a.findall('0xbb', start=48))
-    #     self.assertEqual(b, [48])
-    #     b = list(a.findall('0xbb', start=47))
-    #     self.assertEqual(b, [48])
-    #     b = list(a.findall('0xbb', start=49))
-    #     self.assertEqual(b, [])
-
-    # def testFindAllByteAligned(self):
-    #     a = BitArray('0x0550550')
-    #     b = list(a.findall('0x55', bytealigned=True))
-    #     self.assertEqual(b, [16])
-
-    # def testFindAllWithCount(self):
-    #     a = BitArray('0b0001111101')
-    #     b = list(a.findall([1], start=1, count=1))
-    #     self.assertEqual(b, [2])
+    def testRfindWithStartAndEnd(self):
+        a = BitArray('0b11 0000 11 00')
+        p = a.rfind('0b11', start=8)
+        self.assertEqual(p[0], 8)
+        p = a.rfind('0b110', start=8)
+        self.assertEqual(p, ())
+        p = a.rfind('0b11', end=-1)
+        self.assertEqual(p[0], 2)
+
+    def testFindall(self):
+        a = BitArray('0b001000100001')
+        b = list(a.findall('0b1'))
+        self.assertEqual(b, [0, 5, 9])
+        c = list(a.findall('0b0001'))
+        self.assertEqual(c, [0, 5])
+        d = list(a.findall('0b10'))
+        self.assertEqual(d, [4, 8])
+        e = list(a.findall('0x198273641234'))
+        self.assertEqual(e, [])
+
+    def testFindAllWithStartAndEnd(self):
+        a = BitArray('0xaabbccaabbccccbb')
+        b = list(a.findall('0xbb', start=0, end=8))
+        self.assertEqual(b, [0])
+        b = list(a.findall('0xbb', start=1, end=8))
+        self.assertEqual(b, [])
+        b = list(a.findall('0xbb', start=0, end=7))
+        self.assertEqual(b, [])
+        b = list(a.findall('0xbb', start=48))
+        self.assertEqual(b, [48])
+        b = list(a.findall('0xbb', start=47))
+        self.assertEqual(b, [48])
+        b = list(a.findall('0xbb', start=49))
+        self.assertEqual(b, [])
+
+    def testFindAllByteAligned(self):
+        a = BitArray('0x0550550')
+        b = list(a.findall('0x55', bytealigned=True))
+        self.assertEqual(b, [16])
+
+    def testFindAllWithCount(self):
+        a = BitArray('0b0001111101')
+        b = list(a.findall([1], start=1, count=1))
+        self.assertEqual(b, [2])
 
     def testSplit(self):
         a = BitArray('0x4700004711472222')
         li = list(a.split('0x47', bytealigned=True))
         self.assertEqual(li, ['', '0x472222', '0x4711', '0x470000'])
 
     def testByteSwap(self):
-        a = BitArray('0xff00ff00ff00')
+        a = BitArray('0xaa00ff00ff00')
         n = a.byteswap(2, end=32, repeat=True)
         self.assertEqual(n, 2)
-        self.assertEqual(a, '0xff0000ff00ff')
+        self.assertEqual(a, '0xaa0000ff00ff')
 
     def testInsert(self):
         a = BitArray('0x0123456')
         a.insert('0xf', 4)
         self.assertEqual(a, '0x012345f6')
 
     def testOverwrite(self):
         a = BitArray('0x00000000')
         a.overwrite('0xdead', 4)
         self.assertEqual(a, '0x000dead0')
 
-    # def testReplace(self):
-    #     a = BitArray('0x0001100')
-    #     n = a.replace('0x1', '0xabc')
-    #     self.assertEqual(n, 2)
-    #     self.assertEqual(a, '0x000abcabc00')
-    #     n = a.replace([1], [0], end=12)
-    #     self.assertEqual(n, 2)
-    #     self.assertEqual(a, '0x000abcab000')
+    def testReplace(self):
+        a = BitArray('0x5551100')
+        n = a.replace('0x1', '0xabc')
+        self.assertEqual(n, 2)
+        self.assertEqual(a, '0x555abcabc00')
+        n = a.replace([1], [0], end=12)
+        self.assertEqual(n, 2)
+        self.assertEqual(a, '0x555abcab000')
 
     def testReverse(self):
         pass
 
     def testRor(self):
         a = BitArray('0b111000')
         a.ror(1)
@@ -711,14 +735,16 @@
         self.assertEqual(a.len, 0)
         a.i8 = 127
         a.i8 = -128
         with self.assertRaises(ValueError):
             a.i8 = 128
         with self.assertRaises(ValueError):
             a.i8 = -129
+        with self.assertRaises(bitstring.CreationError):
+            a.froggy16 = '0xabc'
 
     def testUnpack(self):
         a = BitArray('0xff160120')
         b = a.unpack('h8,2*u12')
         self.assertEqual(b, ['ff', 352, 288])
 
     def testReading(self):
@@ -829,7 +855,70 @@
         self.assertEqual(s, ninf64)
         s.f32 = -1e60
         self.assertEqual(s, ninf32)
         s.f16 = -100000
         self.assertEqual(s, ninf16)
         s.bfloat = -1e60
         self.assertEqual(s, ninfbfloat)
+
+    def testBigEndianStringInitialisers(self):
+        a = BitArray('bfloatbe=4.5')
+        b = BitArray('bfloatbe:16=-2.25')
+        self.assertEqual(a.bfloatbe, 4.5)
+        self.assertEqual(b.bfloatbe, -2.25)
+
+    def testLilleEndianStringInitialisers(self):
+        a = BitArray('bfloatle=4.5')
+        b = BitArray('bfloatle:16=-2.25')
+        self.assertEqual(a.bfloatle, 4.5)
+        self.assertEqual(b.bfloatle, -2.25)
+
+    def testNativeEndianStringInitialisers(self):
+        a = BitArray('bfloatne=4.5')
+        b = BitArray('bfloatne:16=-2.25')
+        self.assertEqual(a.bfloatne, 4.5)
+        self.assertEqual(b.bfloatne, -2.25)
+
+
+
+THIS_DIR = os.path.dirname(os.path.abspath(__file__))
+
+class BitarrayTests(unittest.TestCase):
+
+    def tearDown(self) -> None:
+        bitstring.lsb0 = False
+
+    def testToBitarray(self):
+        a = BitArray('0xff, 0b0')
+        b = a.tobitarray()
+        self.assertEqual(type(b), bitarray.bitarray)
+        self.assertEqual(b, bitarray.bitarray('111111110'))
+
+    def testToBitarrayLSB0(self):
+        bitstring.lsb0 = True
+        a = bitstring.Bits('0xff, 0b0')
+        b = a.tobitarray()
+        self.assertEqual(type(b), bitarray.bitarray)
+        self.assertEqual(b, bitarray.bitarray('111111110'))
+
+    def testFromFile(self):
+        a = bitstring.ConstBitStream(filename=os.path.join(THIS_DIR, 'smalltestfile'))
+        b = a.tobitarray()
+        self.assertEqual(a.bin, b.to01())
+
+    def testWithOffset(self):
+        a = bitstring.ConstBitStream(filename=os.path.join(THIS_DIR, 'smalltestfile'))
+        b = bitstring.ConstBitStream(filename=os.path.join(THIS_DIR, 'smalltestfile'), offset=11)
+        self.assertEqual(len(a), len(b) + 11)
+        self.assertEqual(a[11:].tobitarray(), b.tobitarray())
+
+    def testWithLength(self):
+        a = bitstring.ConstBitStream(filename=os.path.join(THIS_DIR, 'smalltestfile'))
+        b = bitstring.ConstBitStream(filename=os.path.join(THIS_DIR, 'smalltestfile'), length=11)
+        self.assertEqual(len(b), 11)
+        self.assertEqual(a[:11].tobitarray(), b.tobitarray())
+
+    def testWithOffsetAndLength(self):
+        a = bitstring.ConstBitStream(filename=os.path.join(THIS_DIR, 'smalltestfile'))
+        b = bitstring.ConstBitStream(filename=os.path.join(THIS_DIR, 'smalltestfile'), offset=17, length=7)
+        self.assertEqual(len(b), 7)
+        self.assertEqual(a[17:24].tobitarray(), b.tobitarray())
```

### Comparing `bitstring-4.0.2/tests/test_bits.py` & `bitstring-4.1.0b1/tests/test_bits.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python
 import io
 import unittest
 import sys
 
+import bitarray
+
 sys.path.insert(0, '..')
 import bitstring
 import array
 import os
 from bitstring import InterpretError
-from bitstring import MmapByteArray
-from bitstring import Bits, BitArray, ByteStore
+from bitstring import Bits, BitArray
 
 THIS_DIR = os.path.dirname(os.path.abspath(__file__))
 
 
 class Creation(unittest.TestCase):
     def testCreationFromBytes(self):
         s = Bits(bytes=b'\xa0\xff')
@@ -89,14 +90,15 @@
         with self.assertRaises(bitstring.CreationError):
             Bits(uint=0, length=0)
         with self.assertRaises(bitstring.CreationError):
             Bits(uint=12, length=-12)
 
     def testCreationFromInt(self):
         s = Bits(int=0, length=4)
+        temp = s.hex
         self.assertEqual(s.bin, '0000')
         s = Bits(int=1, length=2)
         self.assertEqual(s.bin, '01')
         s = Bits(int=-1, length=11)
         self.assertEqual(s.bin, '11111111111')
         s = Bits(int=12, length=7)
         self.assertEqual(s.int, 12)
@@ -168,17 +170,42 @@
         with self.assertRaises(bitstring.CreationError):
             _ = Bits(bool=0, length=2)
 
     def testCreationKeywordError(self):
         with self.assertRaises(bitstring.CreationError):
             Bits(squirrel=5)
 
-    def testDataStoreType(self):
-        a = Bits('0xf')
-        self.assertEqual(type(a._datastore), bitstring.ByteStore)
+    def testCreationFromBitarray(self):
+        ba = bitarray.bitarray('0010')
+        bs = Bits(ba)
+        self.assertEqual(bs.bin, '0010')
+        bs = Bits(ba, length=2)
+        self.assertEqual(bs.bin, '00')
+        bs2 = Bits(bitarray=ba)
+        self.assertEqual(bs2.bin, '0010')
+
+    def testCreationFromFrozenBitarray(self):
+        fba = bitarray.frozenbitarray('111100001')
+        ba = Bits(fba)
+        self.assertEqual(ba.bin, '111100001')
+        bs2 = Bits(bitarray=fba)
+        self.assertEqual(bs2.bin, '111100001')
+        bs3 = Bits(bitarray=fba, offset=4)
+        self.assertEqual(bs3.bin, '00001')
+        bs3 = Bits(bitarray=fba, offset=4, length=4)
+        self.assertEqual(bs3.bin, '0000')
+
+    def testCreationFromBitarrayErrors(self):
+        ba = bitarray.bitarray('0101')
+        with self.assertRaises(bitstring.CreationError):
+            _ = Bits(bitarray=ba, length=5)
+        with self.assertRaises(bitstring.CreationError):
+            _ = Bits(bitarray=ba, offset=5)
+        with self.assertRaises(bitstring.CreationError):
+            _ = Bits(ba, length=-1)
 
 
 class Initialisation(unittest.TestCase):
     def testEmptyInit(self):
         a = Bits()
         self.assertEqual(a, '')
 
@@ -257,17 +284,17 @@
         filename = os.path.join(THIS_DIR, 'smalltestfile')
         self.a = Bits(filename=filename)
         self.b = Bits(filename=filename, offset=16)
         self.c = Bits(filename=filename, offset=20, length=16)
         self.d = Bits(filename=filename, offset=20, length=4)
 
     def testCreationWithOffset(self):
-        self.assertEqual(self.a, '0x0123456789abcdef')
-        self.assertEqual(self.b, '0x456789abcdef')
-        self.assertEqual(self.c, '0x5678')
+        self.assertEqual(str(self.a), '0x0123456789abcdef')
+        self.assertEqual(str(self.b), '0x456789abcdef')
+        self.assertEqual(str(self.c), '0x5678')
 
     def testBitOperators(self):
         x = self.b[4:20]
         self.assertEqual(x, '0x5678')
         self.assertEqual((x & self.c).hex, self.c.hex)
         self.assertEqual(self.c ^ self.b[4:20], 16)
         self.assertEqual(self.a[23:36] | self.c[3:], self.c[3:])
@@ -277,49 +304,14 @@
         x = self.a[20:24] + self.c[-4:] + self.c[8:12]
         self.assertEqual(x, '0x587')
         x = self.b + x
         self.assertEqual(x.h, '456789abcdef587')
         x = BitArray(x)
         del x[12:24]
         self.assertEqual(x, '0x456abcdef587')
-        
-
-class Mmap(unittest.TestCase):
-    def setUp(self):
-        self.f = open(os.path.join(THIS_DIR, 'smalltestfile'), 'rb')
-
-    def tearDown(self):
-        self.f.close()
-
-    def testByteArrayEquivalence(self):
-        a = MmapByteArray(self.f)
-        self.assertEqual(a.bytelength, 8)
-        self.assertEqual(len(a), 8)
-        self.assertEqual(a[0], 0x01)
-        self.assertEqual(a[1], 0x23)
-        self.assertEqual(a[7], 0xef)
-        self.assertEqual(a[0:1], bytearray([1]))
-        self.assertEqual(a[:], bytearray([0x01, 0x23, 0x45, 0x67, 0x89, 0xab, 0xcd, 0xef]))
-        self.assertEqual(a[2:4], bytearray([0x45, 0x67]))
-
-    def testWithLength(self):
-        a = MmapByteArray(self.f, 3)
-        self.assertEqual(a[0], 0x01)
-        self.assertEqual(len(a), 3)
-
-    def testWithOffset(self):
-        a = MmapByteArray(self.f, None, 5)
-        self.assertEqual(len(a), 3)
-        self.assertEqual(a[0], 0xab)
-
-    def testWithLengthAndOffset(self):
-        a = MmapByteArray(self.f, 3, 3)
-        self.assertEqual(len(a), 3)
-        self.assertEqual(a[0], 0x67)
-        self.assertEqual(a[:], bytearray([0x67, 0x89, 0xab]))
 
 
 class Comparisons(unittest.TestCase):
     def testUnorderable(self):
         a = Bits(5)
         b = Bits(5)
         with self.assertRaises(TypeError):
@@ -350,43 +342,14 @@
 
     def testLongBool(self):
         a = Bits(1000)
         b = bool(a)
         self.assertTrue(b is False)
 
 
-# Some basic tests for the private ByteStore classes
-
-class ByteStoreCreation(unittest.TestCase):
-
-    def testProperties(self):
-        a = ByteStore(bytearray(b'abc'))
-        self.assertEqual(a.bytelength, 3)
-        self.assertEqual(a.offset, 0)
-        self.assertEqual(a.bitlength, 24)
-        self.assertEqual(a.rawarray, b'abc')
-
-    def testGetBit(self):
-        a = ByteStore(bytearray([0x0f]))
-        self.assertEqual(a.getbit(0), False)
-        self.assertEqual(a.getbit(3), False)
-        self.assertEqual(a.getbit(4), True)
-        self.assertEqual(a.getbit(7), True)
-
-        b = ByteStore(bytearray([0x0f]), 7, 1)
-        self.assertEqual(b.getbit(2), False)
-        self.assertEqual(b.getbit(3), True)
-
-    def testGetByte(self):
-        a = ByteStore(bytearray(b'abcde'), 1, 13)
-        self.assertEqual(a.getbyte(0), 97)
-        self.assertEqual(a.getbyte(1), 98)
-        self.assertEqual(a.getbyte(4), 101)
-
-
 class PadToken(unittest.TestCase):
 
     def testCreation(self):
         a = Bits('pad:10')
         self.assertEqual(a, Bits(10))
         b = Bits('pad:0')
         self.assertEqual(b, Bits())
@@ -501,43 +464,43 @@
 
         self.assertTrue('0b1' in Bits('0xf'))
         self.assertFalse('0b0' in Bits('0xf'))
 
 
 class ByteStoreImmutablity(unittest.TestCase):
     
-    def testBitsDataStoreType(self):
-        a = Bits('0b1')
-        b = Bits('0b111')
-        c = a + b
-        self.assertEqual(type(a._datastore), ByteStore)
-        self.assertEqual(type(b._datastore), ByteStore)
-        self.assertEqual(type(c._datastore), ByteStore)
+    # def testBitsDataStoreType(self):
+    #     a = Bits('0b1')
+    #     b = Bits('0b111')
+    #     c = a + b
+    #     self.assertEqual(type(a._datastore), ByteStore)
+    #     self.assertEqual(type(b._datastore), ByteStore)
+    #     self.assertEqual(type(c._datastore), ByteStore)
 
     def testImmutabilityBugAppend(self):
         a = Bits('0b111')
         b = a + '0b000'
         c = BitArray(b)
         c[1] = 0
         self.assertEqual(c.bin, '101000')
         self.assertEqual(a.b3, '111')
         self.assertEqual(b.bin, '111000')
-        self.assertEqual(type(b._datastore), ByteStore)
+        # self.assertEqual(type(b._datastore), ByteStore)
 
     def testImmutabilityBugPrepend(self):
         a = Bits('0b111')
         b = '0b000' + a
         c = BitArray(b)
         c[1] = 1
         self.assertEqual(b.bin, '000111')
         self.assertEqual(c.bin, '010111')
 
     def testImmutabilityBugCreation(self):
         a = Bits()
-        self.assertEqual(type(a._datastore), ByteStore)
+        # self.assertEqual(type(a._datastore), ByteStore)
 
 
 class Lsb0Indexing(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         bitstring.lsb0 = True
@@ -823,7 +786,39 @@
 
 class Copy(unittest.TestCase):
 
     def testCopyMethod(self):
         s = Bits('0xc00dee')
         t = s.copy()
         self.assertEqual(s, t)
+
+
+class NativeEndianIntegers(unittest.TestCase):
+
+    def testUintne(self):
+        s = Bits(uintne=454, length=160)
+        t = Bits('uintne160=454')
+        self.assertEqual(s, t)
+
+    def testIntne(self):
+        s = Bits(intne=-1000, length=64)
+        t = Bits('intne:64=-1000')
+        self.assertEqual(s, t)
+
+
+class NonNativeEndianIntegers(unittest.TestCase):
+
+    def setUp(self) -> None:
+        bitstring.byteorder = 'little' if bitstring.byteorder == 'big' else 'little'
+
+    def tearDown(self) -> None:
+        self.setUp()
+
+    def testUintne(self):
+        s = Bits(uintne=454, length=160)
+        t = Bits('uintne160=454')
+        self.assertEqual(s, t)
+
+    def testIntne(self):
+        s = Bits(intne=-1000, length=64)
+        t = Bits('intne:64=-1000')
+        self.assertEqual(s, t)
```

### Comparing `bitstring-4.0.2/tests/test_bitstream.py` & `bitstring-4.1.0b1/tests/test_bitstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import sys
 sys.path.insert(0, '..')
 import bitstring
 import copy
 import os
 import collections
 from bitstring import Bits, BitStream, ConstBitStream, pack
-from bitstring import offsetcopy
 
 THIS_DIR = os.path.dirname(os.path.abspath(__file__))
 
 try:
     collectionsAbc = collections.abc
 except AttributeError:  # Python 2.7
     collectionsAbc = collections
@@ -370,15 +369,15 @@
         c.replace(a, b)
         self.assertEqual(c, '0xcdef')
         self.assertEqual(a, '0xab')
         self.assertEqual(b, '0xcd')
         a = BitStream('0x0011223344')
         a.pos = 12
         a.replace('0x11', '0xfff', bytealigned=True)
-        self.assertEqual(a.pos, 8)
+        self.assertEqual(a.pos, 20)
         self.assertEqual(a, '0x00fff223344')
 
     def testReplaceWithSelf(self):
         a = BitStream('0b11')
         a.replace('0b1', a)
         self.assertEqual(a, '0xf')
         a.replace(a, a)
@@ -423,29 +422,28 @@
         with self.assertRaises(ValueError):
             a.replace('', 0o7, bytealigned=True)
         with self.assertRaises(ValueError):
             a.replace('0b1', '0b1', start=-100, bytealigned=True)
         with self.assertRaises(ValueError):
             a.replace('0b1', '0b1', end=19, bytealigned=True)
 
-
 class SliceAssignment(unittest.TestCase):
 
-    # TODO: Move this to another class
     def testSetSlice(self):
         a = BitStream()
         a[0:0] = '0xabcdef'
         self.assertEqual(a.bytepos, 3)
         a[4:16] = ''
         self.assertEqual(a, '0xaef')
-        self.assertEqual(a.bitpos, 4)
+        self.assertEqual(a.bitpos, 12)
         a[8:] = '0x00'
         self.assertEqual(a, '0xae00')
         self.assertEqual(a.bytepos, 2)
         a += '0xf'
+        self.assertEqual(a.bytepos, 2)
         a[8:] = '0xe'
         self.assertEqual(a, '0xaee')
         self.assertEqual(a.bitpos, 12)
         b = BitStream()
         b[0:800] = '0xffee'
         self.assertEqual(b, '0xffee')
         b[4:48] = '0xeed123'
@@ -461,29 +459,29 @@
     def testInsertingUsingSetItem(self):
         a = BitStream()
         a[0:0] = '0xdeadbeef'
         self.assertEqual(a, '0xdeadbeef')
         self.assertEqual(a.bytepos, 4)
         a[16:16] = '0xfeed'
         self.assertEqual(a, '0xdeadfeedbeef')
-        self.assertEqual(a.bytepos, 4)
+        self.assertEqual(a.bytepos, 6)
         a[0:0] = '0xa'
         self.assertEqual(a, '0xadeadfeedbeef')
-        self.assertEqual(a.bitpos, 4)
+        self.assertEqual(a.bitpos, 52)
         a.bytepos = 6
         a[0:0] = '0xff'
-        self.assertEqual(a.bytepos, 1)
+        self.assertEqual(a.bitpos, 56)
         a[8:0] = '0x00000'
         self.assertTrue(a.startswith('0xff00000adead'))
 
     def testSliceAssignmentBitPos(self):
         a = BitStream('int:64=-1')
         a.pos = 64
         a[0:8] = ''
-        self.assertEqual(a.pos, 0)
+        self.assertEqual(a.pos, 56)
         a.pos = 52
         a[48:56] = '0x0000'
         self.assertEqual(a.pos, 64)
         a[10:10] = '0x0'
         self.assertEqual(a.pos, 14)
         a[56:68] = '0x000'
         self.assertEqual(a.pos, 14)
@@ -918,30 +916,14 @@
         a.pos = 80
         a.bytepos -= 5
         self.assertEqual(a.bytepos, 5)
         a.pos -= 5
         self.assertEqual(a.pos, 35)
 
 
-class Offset(unittest.TestCase):
-    def testOffset1(self):
-        s = BitStream(bytes=b'\x00\x1b\x3f', offset=4)
-        self.assertEqual(s.read(8).bin, '00000001')
-        self.assertEqual(s.length, 20)
-
-    def testOffset2(self):
-        s1 = BitStream(bytes=b'\xf1\x02\x04')
-        s2 = BitStream(bytes=b'\xf1\x02\x04', length=23)
-        for i in [1, 2, 3, 4, 5, 6, 7, 6, 5, 4, 3, 2, 1, 0, 7, 3, 5, 1, 4]:
-            s1._datastore = offsetcopy(s1._datastore, i)
-            self.assertEqual(s1.hex, 'f10204')
-            s2._datastore = offsetcopy(s2._datastore, i)
-            self.assertEqual(s2.bin, '11110001000000100000010')
-
-
 class Append(unittest.TestCase):
     def testAppend(self):
         s1 = BitStream('0b00000')
         s1.append(BitStream(bool=True))
         self.assertEqual(s1.bin, '000001')
         self.assertEqual((BitStream('0x0102') + BitStream('0x0304')).hex, '01020304')
 
@@ -964,21 +946,14 @@
         s.pos += 11
         s.bytealign()
         self.assertEqual(s.bytepos, 2)
         s.pos -= 10
         s.bytealign()
         self.assertEqual(s.bytepos, 1)
 
-    def testByteAlignWithOffset(self):
-        s = BitStream(hex='0112233')
-        s._datastore = offsetcopy(s._datastore, 3)
-        bitstoalign = s.bytealign()
-        self.assertEqual(bitstoalign, 0)
-        self.assertEqual(s.read(5).bin, '00001')
-
     def testInsertByteAligned(self):
         s = BitStream('0x0011')
         s.insert(BitStream('0x22'), 8)
         self.assertEqual(s.hex, '002211')
         s = BitStream(0)
         s.insert(BitStream(bin='101'), 0)
         self.assertEqual(s.bin, '101')
@@ -1214,20 +1189,20 @@
         s = '0xff' + BitStream('0xee')
         self.assertEqual(s.hex, 'ffee')
 
     def testTruncateAsserts(self):
         s = BitStream('0x001122')
         s.bytepos = 2
         del s[-s.len:]
-        self.assertEqual(s.bytepos, 0)
+        # self.assertEqual(s.bytepos, 0)
         s.append('0x00')
         s.append('0x1122')
         s.bytepos = 2
         del s[:s.len]
-        self.assertEqual(s.bytepos, 0)
+        # self.assertEqual(s.bytepos, 0)
         s.append('0x00')
 
     def testOverwriteErrors(self):
         s = BitStream(bin='11111')
         with self.assertRaises(ValueError):
             s.overwrite(BitStream(bin='1'), -10)
         with self.assertRaises(ValueError):
@@ -1532,15 +1507,15 @@
         self.assertEqual(s.bin, '1100011000')
         s.prepend('')
         self.assertEqual(s.bin, '1100011000')
 
     def testNullSlice(self):
         s = BitStream('0x111')
         t = s[1:1]
-        self.assertEqual(t._datastore.bytelength, 0)
+        self.assertEqual(len(t), 0)
 
     def testMultipleAutos(self):
         s = BitStream('0xa')
         s.prepend('0xf')
         s.append('0xb')
         self.assertEqual(s, '0xfab')
         s.prepend(s)
@@ -1692,23 +1667,14 @@
         with self.assertRaises(TypeError):
             _ = a * 1.2
         with self.assertRaises(TypeError):
             _ = b * a
         with self.assertRaises(TypeError):
             a *= b
 
-    def testFileAndMemEquivalence(self):
-        filename = os.path.join(THIS_DIR, 'smalltestfile')
-        a = ConstBitStream(filename=filename)
-        b = BitStream(filename=filename)
-        self.assertTrue(isinstance(a._datastore.rawarray, bitstring.MmapByteArray))
-        self.assertTrue(isinstance(b._datastore.rawarray, bytearray))
-        self.assertEqual(a._datastore.getbyte(0), b._datastore.getbyte(0))
-        self.assertEqual(a._datastore.getbyteslice(1, 5), bytearray(b._datastore.getbyteslice(1, 5)))
-
 
 class BitWise(unittest.TestCase):
 
     def testBitwiseAnd(self):
         a = BitStream('0b01101')
         b = BitStream('0b00110')
         self.assertEqual((a & b).bin, '00100')
@@ -1724,27 +1690,29 @@
         self.assertEqual(d.bin, '0011000')
         d = '0b1111000' & c
         self.assertEqual(d.bin, '0011000')
 
     def testBitwiseOr(self):
         a = BitStream('0b111001001')
         b = BitStream('0b011100011')
-        self.assertEqual((a | b).bin, '111101011')
+        c = a | b
+        self.assertEqual(c.bin, '111101011')
         self.assertEqual((a | '0b000000000'), a)
         with self.assertRaises(ValueError):
             _ = a | '0b0000'
         with self.assertRaises(ValueError):
             _ = b | (a + '0b1')
         a = '0xff00' | BitStream('0x00f0')
         self.assertEqual(a.hex, 'fff0')
 
     def testBitwiseXor(self):
         a = BitStream('0b111001001')
         b = BitStream('0b011100011')
-        self.assertEqual((a ^ b).bin, '100101010')
+        c = a ^ b
+        self.assertEqual(c.bin, '100101010')
         self.assertEqual((a ^ '0b111100000').bin, '000101001')
         with self.assertRaises(ValueError):
             _ = a ^ '0b0000'
         with self.assertRaises(ValueError):
             _ = b ^ (a + '0b1')
         a = '0o707' ^ BitStream('0o777')
         self.assertEqual(a.oct, '070')
@@ -1947,15 +1915,15 @@
         p = a.findall('0x47', bytealigned=True)
         self.assertEqual(list(p), [0, 6 * 8, 7 * 8, 13 * 8])
         p = a.findall('0x4733', bytealigned=True)
         self.assertEqual(list(p), [0, 7 * 8])
         a = BitStream('0b1001001001001001001')
         p = a.findall('0b1001', bytealigned=False)
         self.assertEqual(list(p), [0, 3, 6, 9, 12, 15])
-        self.assertEqual(a.pos, 15)
+        self.assertEqual(a.pos, 0)
 
     def testFindAllGenerator(self):
         a = BitStream('0xff1234512345ff1234ff12ff')
         p = a.findall('0xff', bytealigned=True)
         self.assertEqual(next(p), 0)
         self.assertEqual(next(p), 6 * 8)
         self.assertEqual(next(p), 9 * 8)
@@ -1984,15 +1952,15 @@
             b = eval(a.__repr__())
             self.assertTrue(a == b)
         filename = os.path.join(THIS_DIR, 'test.m1v')
         for f in [ConstBitStream(filename=filename),
                   ConstBitStream(filename=filename, length=17),
                   ConstBitStream(filename=filename, length=23, offset=23102)]:
             f2 = eval(f.__repr__())
-            self.assertEqual(f._datastore.rawarray.source.name, f2._datastore.rawarray.source.name)
+            self.assertEqual(f._bitstore.filename, f2._bitstore.filename)
             self.assertTrue(f2.tobytes() == f.tobytes())
         a = BitStream('0b1')
         self.assertEqual(repr(a), "BitStream('0b1')")
         a += '0b11'
         a.pos = 2
         self.assertEqual(repr(a), "BitStream('0b111', pos=2)")
         a.pos = 0
@@ -2031,20 +1999,18 @@
         self.assertFalse(a)
 
     def testNonZeroBitsAtStart(self):
         a = BitStream(bytes=b'\xff', offset=2)
         b = BitStream('0b00')
         b += a
         self.assertTrue(b == '0b0011 1111')
-        self.assertEqual(a._datastore.rawbytes, b'\xff')
         self.assertEqual(a.tobytes(), b'\xfc')
 
     def testNonZeroBitsAtEnd(self):
         a = BitStream(bytes=b'\xff', length=5)
-        self.assertEqual(a._datastore.rawbytes, b'\xff')
         b = BitStream('0b00')
         a += b
         self.assertTrue(a == '0b1111100')
         self.assertEqual(a.tobytes(), b'\xf8')
         with self.assertRaises(ValueError):
             _ = a.bytes
 
@@ -2078,15 +2044,15 @@
         self.assertEqual(a[100:2:-1], '0b1110001')
 
     def testInsertionOrderAndBitpos(self):
         b = BitStream()
         b[0:0] = '0b0'
         b[0:0] = '0b1'
         self.assertEqual(b, '0b10')
-        self.assertEqual(b.bitpos, 1)
+        self.assertEqual(b.bitpos, 2)
         a = BitStream()
         a.insert('0b0')
         a.insert('0b1')
         self.assertEqual(a, '0b01')
         self.assertEqual(a.bitpos, 2)
 
     def testOverwriteOrderAndBitpos(self):
@@ -2202,14 +2168,15 @@
         for n in list(s.cut(4)):
             s.prepend(n)
         self.assertEqual(s, '0x43211234')
 
     def testJoinFunctions(self):
         a = BitStream().join(['0xa', '0xb', '0b1111'])
         self.assertEqual(a, '0xabf')
+        tmp = BitStream('0b1')
         a = BitStream('0b1').join(['0b0' for _ in range(10)])
         self.assertEqual(a, '0b0101010101010101010')
         a = BitStream('0xff').join([])
         self.assertFalse(a)
 
     def testAddingBitpos(self):
         a = BitStream('0xff')
@@ -2393,29 +2360,26 @@
             self.assertEqual(a.tobytes(), b'\xab\x00')
         del a[-1:]
         self.assertEqual(a.tobytes(), b'\xab')
 
     def testToFile(self):
         filename = os.path.join(THIS_DIR, 'temp_bitstring_unit_testing_file')
         a = BitStream('0x0000ff')[:17]
-        f = open(filename, 'wb')
-        a.tofile(f)
-        f.close()
+        with open(filename, 'wb') as f:
+            a.tofile(f)
         b = BitStream(filename=filename)
         self.assertEqual(b, '0x000080')
 
         a = BitStream('int:1000000=-1')
         self.assertEqual(a.int, -1)
-        f = open(filename, 'wb')
-        a.tofile(f)
-        f.close()
+        with open(filename, 'wb') as f:
+            a.tofile(f)
         b = BitStream(filename=filename)
         self.assertEqual(b.int, -1)
         self.assertEqual(b.len, 1000000)
-        os.remove(filename)
 
     def testTokenParser(self):
         tp = bitstring.tokenparser
         self.assertEqual(tp('hex'), (True, [('hex', None, None)]))
         self.assertEqual(tp('hex=14'), (True, [('hex', None, '14')]))
         self.assertEqual(tp('se'), (False, [('se', None, None)]))
         self.assertEqual(tp('ue=12'), (False, [('ue', None, '12')]))
@@ -2439,16 +2403,15 @@
             s2 = ConstBitStream(f)
             t2 = BitStream('0xc')
             t2.prepend(s2)
             self.assertTrue(t2.startswith('0x000001b3'))
             self.assertTrue(t2.endswith('0xc'))
             with open(filename, 'rb') as b:
                 u = BitStream(bytes=b.read())
-                # TODO: u == s2 is much slower than u.bytes == s2.bytes
-                self.assertEqual(u.bytes, s2.bytes)
+                self.assertTrue(u == s2)
 
     def testFileBasedCopy(self):
         with open(os.path.join(THIS_DIR, 'smalltestfile'), 'rb') as f:
             s = BitStream(f)
             t = BitStream(s)
             s.prepend('0b1')
             self.assertEqual(s[1:], t)
@@ -2511,15 +2474,15 @@
 
     def testLittleEndianInt(self):
         s = BitStream(int=100, length=16)
         self.assertEqual(s.intle, 25600)
         s = BitStream(intle=100, length=16)
         self.assertEqual(s.int, 25600)
         self.assertEqual(s.intle, 100)
-        s.intle += 5
+        s.intle = 105
         self.assertEqual(s.intle, 105)
         s = BitStream('intle:32=999')
         self.assertEqual(s.intle, 999)
         s.byteswap()
         self.assertEqual(s.int, 999)
         s = pack('intle:24', 1001)
         self.assertEqual(s.intle, 1001)
@@ -2862,15 +2825,15 @@
         b = a
         a += '0xe'
         self.assertEqual(b, '0xf')
         self.assertEqual(a, '0xfe')
         c = BitStream(a)
         self.assertEqual(a, c)
         a = ConstBitStream('0b1')
-        a._addright(a)
+        a += a
         self.assertEqual(a, '0b11')
         self.assertEqual(type(a), ConstBitStream)
         a._addleft(a)
         self.assertEqual(a, '0b1111')
         self.assertEqual(type(a), ConstBitStream)
 
     def testConstBitStreamHashibility(self):
@@ -2897,15 +2860,15 @@
         self.assertNotEqual(hash(a), hash(c))
 
     def testConstBitStreamCopy(self):
         a = ConstBitStream('0xabc')
         a.pos = 11
         b = copy.copy(a)
         b.pos = 4
-        self.assertEqual(id(a._datastore), id(b._datastore))
+        self.assertEqual(id(a._bitstore), id(b._bitstore))
         self.assertEqual(a.pos, 11)
         self.assertEqual(b.pos, 4)
 
     def testPython26stuff(self):
         s = BitStream('0xff')
         self.assertTrue(isinstance(s.tobytes(), bytes))
         self.assertTrue(isinstance(s.bytes, bytes))
@@ -3918,30 +3881,33 @@
     def testReadIntList(self):
         a = ConstBitStream('0xab, 0b110')
         b, c = a.readlist([8, 3])
         self.assertEqual(b.hex, 'ab')
         self.assertEqual(c.bin, '110')
 
 
-class FileReadingStrategy(unittest.TestCase):
-    def testBitStreamIsAlwaysRead(self):
-        filename = os.path.join(THIS_DIR, 'smalltestfile')
-        a = BitStream(filename=filename)
-        self.assertTrue(isinstance(a._datastore, bitstring.ByteStore))
-        with open(filename, 'rb') as f:
-            b = BitStream(f)
-            self.assertTrue(isinstance(b._datastore, bitstring.ByteStore))
-
-    def testBitsIsNeverRead(self):
-        filename = os.path.join(THIS_DIR, 'smalltestfile')
-        a = ConstBitStream(filename=filename)
-        self.assertTrue(isinstance(a._datastore.rawarray, bitstring.MmapByteArray))
-        with open(filename, 'rb') as f:
-            b = ConstBitStream(f)
-            self.assertTrue(isinstance(b._datastore.rawarray, bitstring.MmapByteArray))
+# class FileReadingStrategy(unittest.TestCase):
+#
+#
+#     def testBitStreamIsAlwaysRead(self):
+#         filename = os.path.join(THIS_DIR, 'smalltestfile')
+#         a = BitStream(filename=filename)
+#         self.assertTrue(isinstance(a._datastore, bitstring.ByteStore))
+#         with open(filename, 'rb') as f:
+#             b = BitStream(f)
+#             self.assertTrue(isinstance(b._datastore, bitstring.ByteStore))
+#
+#
+#     def testBitsIsNeverRead(self):
+#         filename = os.path.join(THIS_DIR, 'smalltestfile')
+#         a = ConstBitStream(filename=filename)
+#         self.assertTrue(isinstance(a._datastore.rawarray, bitstring.MmapByteArray))
+#         with open(filename, 'rb') as f:
+#             b = ConstBitStream(f)
+#             self.assertTrue(isinstance(b._datastore.rawarray, bitstring.MmapByteArray))
 
 
 class Count(unittest.TestCase):
     def testCount(self):
         a = ConstBitStream('0xf0f')
         self.assertEqual(a.count(True), 8)
         self.assertEqual(a.count(False), 4)
@@ -3995,14 +3961,16 @@
         s.overwrite(s)
         self.assertEqual(s, '0b1101')
 
 
 class Subclassing(unittest.TestCase):
 
     def testIsInstance(self):
+        b = BitStream()
+        self.assertTrue(isinstance(b, BitStream))
         class SubBits(BitStream):
             pass
         a = SubBits()
         self.assertTrue(isinstance(a, SubBits))
 
     def testClassType(self):
         class SubBits(BitStream):
@@ -4068,19 +4036,18 @@
         s.find('0b11', start=1)
         self.assertEqual(s.pos, 4)
 
     def testIter(self):
         s = BitStream('0b11000')
         self.assertEqual(list(s), [False, False, False, True, True])
 
-    # @unittest.expectedFailure
-    # def testBitPosAfterRfind(self):
-    #     s = BitStream('0b011 000010000110000')
-    #     s.rfind('0b11')
-    #     self.assertEqual(s.pos, 15)
+    def testBitPosAfterRfind(self):
+        s = BitStream('0b011 000010000110000')
+        s.rfind('0b11')
+        self.assertEqual(s.pos, 15)
 
     def testBitPosAfterFindall(self):
         pass
 
     def testBitPosAfterInsert(self):
         pass
 
@@ -4184,7 +4151,26 @@
         self.assertEqual(f'{b}', '0b0000000000')
         c = BitStream(filename=os.path.join(THIS_DIR, 'test.m1v'))
         self.assertEqual(f'{c}'[0:10], '0x000001b3')
 
     def testFormatStringsWithInterpretation(self):
         a = Bits('0xf')
         self.assertEqual(f'{a.bin}', '1111')
+
+
+class CacheingIssues(unittest.TestCase):
+
+    def testCacheWithOffset(self):
+        y = BitStream('0xdeadbeef1000')
+        with self.assertRaises(bitstring.CreationError):
+            x = BitStream('0xdeadbeef1000', offset=8)
+
+    def testCacheWithPos(self):
+        y = BitStream('0xdeadbeef1001', pos=3)
+        self.assertEqual(y.pos, 3)
+        x = BitStream('0xdeadbeef1001', pos=5)
+        self.assertEqual(x.pos, 5)
+
+    def testCacheWithLength(self):
+        y = BitStream('0xdeadbeef002')
+        with self.assertRaises(bitstring.CreationError):
+            x = BitStream('0xdeadbeef002', length=16)
```

### Comparing `bitstring-4.0.2/tests/test_bitstring.py` & `bitstring-4.1.0b1/tests/test_bitstring.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 import unittest
 from unittest import mock
 from contextlib import redirect_stdout
 import sys
 sys.path.insert(0, '..')
 import bitstring
 import copy
+from collections import abc
 
 
 class ModuleData(unittest.TestCase):
     def testVersion(self):
-        self.assertEqual(bitstring.__version__, '4.0.2')
+        self.assertEqual(bitstring.__version__, '4.1.0b1')
 
     def testAll(self):
         exported = ['ConstBitStream', 'BitStream', 'BitArray',
                     'Bits', 'pack', 'Error', 'ReadError',
                     'InterpretError', 'ByteAlignError', 'CreationError', 'bytealigned', 'lsb0']
         self.assertEqual(set(bitstring.__all__), set(exported))
 
@@ -36,45 +37,46 @@
         cba_copy = copy.copy(cba)
         self.assertTrue(cba is cba_copy)
 
     def testBitArrayCopy(self):
         ba = bitstring.BitArray(100)
         ba_copy = copy.copy(ba)
         self.assertFalse(ba is ba_copy)
-        self.assertFalse(ba._datastore is ba_copy._datastore)
+        self.assertFalse(ba._bitstore is ba_copy._bitstore)
         self.assertTrue(ba == ba_copy)
 
     def testConstBitStreamCopy(self):
         cbs = bitstring.ConstBitStream(100)
         cbs.pos = 50
         cbs_copy = copy.copy(cbs)
         self.assertEqual(cbs_copy.pos, 0)
-        self.assertTrue(cbs._datastore is cbs_copy._datastore)
+        self.assertTrue(cbs._bitstore is cbs_copy._bitstore)
         self.assertTrue(cbs == cbs_copy)
 
     def testBitStreamCopy(self):
         bs = bitstring.BitStream(100)
         bs.pos = 50
         bs_copy = copy.copy(bs)
         self.assertEqual(bs_copy.pos, 0)
-        self.assertFalse(bs._datastore is bs_copy._datastore)
+        self.assertFalse(bs._bitstore is bs_copy._bitstore)
         self.assertTrue(bs == bs_copy)
 
 
 class Interning(unittest.TestCase):
     def testBits(self):
         a = bitstring.Bits('0xf')
         b = bitstring.Bits('0xf')
-        self.assertTrue(a is b)
+        self.assertTrue(a._bitstore is b._bitstore)
         c = bitstring.Bits('0b1111')
         self.assertFalse(a is c)
 
     def testCBS(self):
         a = bitstring.ConstBitStream('0b11000')
         b = bitstring.ConstBitStream('0b11000')
+        self.assertTrue(a._bitstore is b._bitstore)
         self.assertFalse(a is b)
 
 
 class LSB0(unittest.TestCase):
     def testGettingAndSetting(self):
         self.assertEqual(bitstring._lsb0, False)
         bitstring.lsb0 = True
@@ -128,7 +130,27 @@
     def testShortInterpretations(self):
         with redirect_stdout(io.StringIO()) as f:
             with mock.patch('sys.argv', ['b.py', 'bin=001.b']):
                 bitstring.main()
         s = f.getvalue()
         self.assertEqual(s, '001\n')
 
+
+@unittest.expectedFailure
+class ABCs(unittest.TestCase):
+    def testBaseClasses(self):
+        # https://github.com/scott-griffiths/bitstring/issues/261
+        bits = bitstring.Bits()
+        self.assertTrue(isinstance(bits, abc.Sequence))
+        self.assertFalse(isinstance(bits, abc.MutableSequence))
+
+        bitarray = bitstring.BitArray()
+        self.assertTrue(isinstance(bitarray, abc.MutableSequence))
+        self.assertTrue(isinstance(bitarray, abc.Sequence))
+
+        constbitstream = bitstring.ConstBitStream()
+        self.assertTrue(isinstance(constbitstream, abc.Sequence))
+        self.assertFalse(isinstance(constbitstream, abc.MutableSequence))
+
+        bitstream = bitstring.BitArray()
+        self.assertTrue(isinstance(bitstream, abc.MutableSequence))
+        self.assertTrue(isinstance(bitstream, abc.Sequence))
```

### Comparing `bitstring-4.0.2/tests/test_constbitstream.py` & `bitstring-4.1.0b1/tests/test_constbitstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,19 +159,33 @@
 
     @classmethod
     def tearDownClass(cls):
         bitstring.lsb0 = False
 
     def testReadingHex(self):
         s = CBS('0xabcdef')
-        self.assertEqual(s.read(4), '0xf')
+        self.assertEqual(s.read('hex:4'), 'f')
         self.assertEqual(s.read(4), '0xe')
         self.assertEqual(s.pos, 8)
 
-    # TODO: Add more tests
+    def testReadingOct(self):
+        s = CBS('0o123456')
+        self.assertEqual(s.read('o6'), '56')
+        self.assertEqual(s.pos, 6)
+
+    def testReadingBin(self):
+        s = CBS('0b00011')
+        self.assertEqual(s.read('bin:3'), '011')
+        self.assertEqual(s.pos, 3)
+
+    def testReadingBytes(self):
+        s = CBS(bytes=b'54321')
+        self.assertEqual(s.pos, 0)
+        s.pos = 8
+        self.assertEqual(s.read('bytes:2'), b'32')
 
 
 class BytesIOCreation(unittest.TestCase):
 
     def testSimpleCreation(self):
         f = io.BytesIO(b"\x12\xff\x77helloworld")
         s = CBS(f)
```

