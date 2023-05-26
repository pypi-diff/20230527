# Comparing `tmp/pyderive3-0.0.1.tar.gz` & `tmp/pyderive3-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyderive3-0.0.1.tar", last modified: Thu May 25 03:15:15 2023, max compression
+gzip compressed data, was "pyderive3-0.0.2.tar", last modified: Fri May 26 22:06:24 2023, max compression
```

## Comparing `pyderive3-0.0.1.tar` & `pyderive3-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-25 03:15:15.697110 pyderive3-0.0.1/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2271 2023-05-25 03:15:15.697110 pyderive3-0.0.1/PKG-INFO
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1846 2023-05-25 03:11:27.000000 pyderive3-0.0.1/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-25 03:15:15.697110 pyderive3-0.0.1/pyderive/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1118 2023-05-25 02:50:26.000000 pyderive3-0.0.1/pyderive/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     3106 2023-05-14 23:24:22.000000 pyderive3-0.0.1/pyderive/abc.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     9741 2023-05-25 03:08:08.000000 pyderive3-0.0.1/pyderive/compile.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     8566 2023-05-25 02:41:26.000000 pyderive3-0.0.1/pyderive/dataclass.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5160 2023-05-25 02:41:24.000000 pyderive3-0.0.1/pyderive/parse.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-25 03:15:15.697110 pyderive3-0.0.1/pyderive3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2271 2023-05-25 03:15:15.000000 pyderive3-0.0.1/pyderive3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      279 2023-05-25 03:15:15.000000 pyderive3-0.0.1/pyderive3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-05-25 03:15:15.000000 pyderive3-0.0.1/pyderive3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       18 2023-05-25 03:15:15.000000 pyderive3-0.0.1/pyderive3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        9 2023-05-25 03:15:15.000000 pyderive3-0.0.1/pyderive3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-05-25 03:15:15.697110 pyderive3-0.0.1/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      708 2023-05-14 23:30:36.000000 pyderive3-0.0.1/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-26 22:06:24.262397 pyderive3-0.0.2/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2320 2023-05-26 22:06:24.262397 pyderive3-0.0.2/PKG-INFO
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1895 2023-05-25 03:21:30.000000 pyderive3-0.0.2/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-26 22:06:24.258397 pyderive3-0.0.2/pyderive/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1118 2023-05-25 02:50:26.000000 pyderive3-0.0.2/pyderive/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     3212 2023-05-25 07:08:25.000000 pyderive3-0.0.2/pyderive/abc.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     9862 2023-05-26 22:02:21.000000 pyderive3-0.0.2/pyderive/compile.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     8833 2023-05-25 23:25:33.000000 pyderive3-0.0.2/pyderive/dataclass.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     5284 2023-05-26 21:59:25.000000 pyderive3-0.0.2/pyderive/parse.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-26 22:06:24.262397 pyderive3-0.0.2/pyderive3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2320 2023-05-26 22:06:24.000000 pyderive3-0.0.2/pyderive3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      279 2023-05-26 22:06:24.000000 pyderive3-0.0.2/pyderive3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-05-26 22:06:24.000000 pyderive3-0.0.2/pyderive3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       18 2023-05-26 22:06:24.000000 pyderive3-0.0.2/pyderive3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        9 2023-05-26 22:06:24.000000 pyderive3-0.0.2/pyderive3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-05-26 22:06:24.262397 pyderive3-0.0.2/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      708 2023-05-25 07:09:26.000000 pyderive3-0.0.2/setup.py
```

### Comparing `pyderive3-0.0.1/PKG-INFO` & `pyderive3-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: pyderive3
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python3 Custom Data Class Helpers
 Home-page: https://github.com/imgurbot12/pyderive
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 pyderive
--------------
+---------
 
 Python3 Custom Dataclass Helpers
 
+### Installation
+
+```bash
+pip install pyderive3
+```
+
 ### Features
 
 ##### Expanded Reimplementation of Dataclasses
 
 ###### Default Standards Implemented
 
 _'slots' kwarg now supported in older versions of python such as 3.8_
```

### Comparing `pyderive3-0.0.1/README.md` & `pyderive3-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 pyderive
--------------
+---------
 
 Python3 Custom Dataclass Helpers
 
+### Installation
+
+```bash
+pip install pyderive3
+```
+
 ### Features
 
 ##### Expanded Reimplementation of Dataclasses
 
 ###### Default Standards Implemented
 
 _'slots' kwarg now supported in older versions of python such as 3.8_
```

### Comparing `pyderive3-0.0.1/pyderive/__init__.py` & `pyderive3-0.0.2/pyderive/__init__.py`

 * *Files identical despite different names*

### Comparing `pyderive3-0.0.1/pyderive/abc.py` & `pyderive3-0.0.2/pyderive/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,19 +58,23 @@
     init:            bool           = True
     repr:            bool           = True
     hash:            bool           = True
     compare:         bool           = True
     kw_only:         bool           = False
     frozen:          bool           = False
     field_type:      FieldType      = FieldType.STANDARD
-    
+ 
     @abstractmethod
     def __init__(self, name: str, anno: Type, default: Any = MISSING):
         raise NotImplementedError
 
+    def finalize(self):
+        """run finalize when field variables are finished compiling"""
+        pass
+
 class Field(FieldDef):
 
     def __init__(self,
         name:            str,
         anno:            Type,
         default:         Any            = MISSING,
         default_factory: DefaultFactory = MISSING,
```

### Comparing `pyderive3-0.0.1/pyderive/compile.py` & `pyderive3-0.0.2/pyderive/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,25 +187,27 @@
     :param fields: ordered fields used to generate hash-function
     :return:       hash-function
     """
     names   = [f.name for f in fields if f.hash]
     names_t = _tuple_str(names, 'self')
     return _create_fn('__hash__', ['self'], [f'return hash({names_t})'])
 
-def assign_func(cls: Type, func: Callable, name: Optional[str] = None) -> bool:
+def assign_func(cls: Type, func: Callable, 
+    name: Optional[str] = None, overwrite: bool = False) -> bool:
     """
     assign function to the object and modify qualname
 
-    :param cls:  class object to assign to
-    :param func: function to assign to value
-    :param name: name of function to assign
-    :return:     true if object already exists else false
+    :param cls:       class object to assign to
+    :param func:      function to assign to value
+    :param name:      name of function to assign
+    :param overwrite: allow for overwrite if enabled
+    :return:          true if object already exists else false
     """
     name = name or func.__name__
-    if name in cls.__dict__:
+    if not overwrite and name in cls.__dict__:
         return True
     if isinstance(func, FunctionType):
         func.__qualname__ = f'{cls.__qualname__}.{func.__name__}'
     setattr(cls, name, func)
     return False
 
 def add_slots(cls: Type, fields: Fields, frozen: bool = False) -> Type:
```

### Comparing `pyderive3-0.0.1/pyderive/dataclass.py` & `pyderive3-0.0.2/pyderive/dataclass.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 DataClass stdlib recreation using existing helpers
 """
 import abc
 import copy
 from typing import * 
-from typing_extensions import dataclass_transform
+from typing_extensions import dataclass_transform, runtime_checkable
 
 from .abc import *
 from .parse import *
 from .compile import *
 
 #** Variables **#
 __all__ = [
@@ -58,14 +58,15 @@
     (True,  False, True,  True ): _hash_err,
     (True,  True,  False, False): _hash_add,
     (True,  True,  False, True ): _hash_err,
     (True,  True,  True,  False): _hash_add,
     (True,  True,  True,  True ): _hash_err,
 }
 
+@runtime_checkable
 class DataClassLike(Generic[F], Protocol):
     """Protocol for DataClass-Like Objects"""
     __datafields__: List[F]
 
 #** Functions **#
 
 def field(*_, **kwargs) -> Any:
@@ -139,16 +140,16 @@
     if not is_dataclass(cls):
         raise TypeError('asdict() should be called on dataclass instances')
     return _asdict_inner(cls, recurse, dict_factory, 0) #type: ignore
 
 @dataclass_transform(field_specifiers=(FieldDef, Field, field))
 def _process_class(
     cls: TypeT,
-    init:        bool = True,
-    repr:        bool = True,
+    init:        Optional[bool] = None,
+    repr:        Optional[bool] = None,
     eq:          bool = True,
     order:       bool = False,
     unsafe_hash: bool = False,
     frozen:      bool = False,
     match_args:  bool = True,
     kw_only:     bool = False,
     slots:       bool = False,
@@ -161,19 +162,22 @@
     # parse and conregate fields
     struct = parse_fields(cls, factory=field, recurse=recurse)
     fields = flatten_fields(struct)
     freeze = frozen or any(f.frozen for f in fields)
     # assign fields to dataclass
     setattr(cls, FIELD_ATTR, fields)
     # build functions
-    if init:
+    if init or init is None:
+        overwrite = init is True
         post_init = hasattr(cls, POST_INIT)
-        assign_func(cls, create_init(fields, kw_only, post_init, frozen))
-    if repr:
-        assign_func(cls, create_repr(fields))
+        initfunc  = create_init(fields, kw_only, post_init, frozen)
+        assign_func(cls, initfunc, overwrite=overwrite)
+    if repr or repr is None:
+        overwrite = repr is True
+        assign_func(cls, create_repr(fields), overwrite=overwrite)
     if eq:
         assign_func(cls, create_compare(fields, '__eq__', '=='))
     if order:
         funcs = [('lt', '<'), ('le', '<='), ('gt', '>'), ('ge', '>=')]
         for name, op in funcs:
             fname = f'__{name}__'
             func  = create_compare(fields, fname, op)
@@ -203,32 +207,32 @@
     # update abstraction-methods on re-creation and return
     abc.update_abstractmethods(cls)
     return cls
 
 @overload
 @dataclass_transform(field_specifiers=(FieldDef, Field, field))
 def dataclass(cls: Type[T], 
-    init:        bool = True,
-    repr:        bool = True,
+    init:        Optional[bool] = None,
+    repr:        Optional[bool] = None,
     eq:          bool = True,
     order:       bool = False,
     unsafe_hash: bool = False,
     frozen:      bool = False,
     match_args:  bool = True,
     kw_only:     bool = False,
     slots:       bool = False,
     recurse:     bool = False,
     field:       Type[FieldDef] = Field,
 ) -> Type[T]:
     ...
 
 @overload
 def dataclass(*,
-    init:        bool = True,
-    repr:        bool = True,
+    init:        Optional[bool] = None,
+    repr:        Optional[bool] = None,
     eq:          bool = True,
     order:       bool = False,
     unsafe_hash: bool = False,
     frozen:      bool = False,
     match_args:  bool = True,
     kw_only:     bool = False,
     slots:       bool = False,
```

### Comparing `pyderive3-0.0.1/pyderive/parse.py` & `pyderive3-0.0.2/pyderive/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,16 @@
                     f'unsupported field-type {fclass!r}. must use {fallow!r}')
             else:
                 field = factory(name, anno, default)
             # handle InitVar
             if not isinstance(anno, type) and isinstance(anno, InitVar):
                 field.anno = anno.type
                 field.field_type = FieldType.INIT_VAR 
+            # finalize field build and assign to struct
+            field.finalize()
             fields.fields[name] = field
         # apply fields to baseclass to allow for inheritance
         if fields.fields:
             setattr(base, DERIVE_ATTR, fields)
     # ensure fields were parsed
     if fields is None:
         raise RuntimeError(f'DataClass Field-Parse Failed: {cls!r}')
@@ -128,15 +130,15 @@
     # sort fields
     struct = FlatStruct()
     kwargs = False # track when kwargs have been spotted
     for fields in heigharchy:
         for name in fields.order:
             field   = fields.fields[name]
             default = has_default(field)
-            kwargs  = kwargs or default
+            kwargs  = kwargs or (default and field.init and not field.kw_only)
             missing = name not in struct.fields
             # raise error if non-kwarg found after kwargs start
             if order_kw and kwargs and missing and not default:
                 raise TypeError(
                     f'non-default argument {name!r} follows default argument')
             # append vardef to order and set/replace definition
             if missing:
```

### Comparing `pyderive3-0.0.1/pyderive3.egg-info/PKG-INFO` & `pyderive3-0.0.2/pyderive3.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: pyderive3
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python3 Custom Data Class Helpers
 Home-page: https://github.com/imgurbot12/pyderive
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 pyderive
--------------
+---------
 
 Python3 Custom Dataclass Helpers
 
+### Installation
+
+```bash
+pip install pyderive3
+```
+
 ### Features
 
 ##### Expanded Reimplementation of Dataclasses
 
 ###### Default Standards Implemented
 
 _'slots' kwarg now supported in older versions of python such as 3.8_
```

### Comparing `pyderive3-0.0.1/setup.py` & `pyderive3-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name='pyderive3',
-    version='0.0.1',
+    version='0.0.2',
     license='MIT',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     url='https://github.com/imgurbot12/pyderive',
     description="Python3 Custom Data Class Helpers",
     long_description=readme,
     long_description_content_type="text/markdown",
```

