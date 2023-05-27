# Comparing `tmp/pymedio-0.2.8.tar.gz` & `tmp/pymedio-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymedio-0.2.8.tar", last modified: Fri Mar  4 15:03:30 2022, max compression
+gzip compressed data, was "pymedio-0.2.9.tar", last modified: Fri Mar 11 17:26:49 2022, max compression
```

## Comparing `pymedio-0.2.8.tar` & `pymedio-0.2.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 15:03:30.683376 pymedio-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-03-04 15:03:20.000000 pymedio-0.2.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3481 2022-03-04 15:03:20.000000 pymedio-0.2.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2684 2022-03-04 15:03:20.000000 pymedio-0.2.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11949 2022-03-04 15:03:20.000000 pymedio-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-03-04 15:03:20.000000 pymedio-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-03-04 15:03:30.683376 pymedio-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4456 2022-03-04 15:03:20.000000 pymedio-0.2.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 15:03:30.683376 pymedio-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-03-04 15:03:20.000000 pymedio-0.2.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-03-04 15:03:20.000000 pymedio-0.2.8/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     5128 2022-03-04 15:03:20.000000 pymedio-0.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-03-04 15:03:20.000000 pymedio-0.2.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-03-04 15:03:20.000000 pymedio-0.2.8/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-03-04 15:03:20.000000 pymedio-0.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-03-04 15:03:20.000000 pymedio-0.2.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-03-04 15:03:20.000000 pymedio-0.2.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-03-04 15:03:20.000000 pymedio-0.2.8/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-03-04 15:03:20.000000 pymedio-0.2.8/docs/pymedio.rst
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-03-04 15:03:20.000000 pymedio-0.2.8/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-03-04 15:03:20.000000 pymedio-0.2.8/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 15:03:30.683376 pymedio-0.2.8/pymedio/
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-03-04 15:03:20.000000 pymedio-0.2.8/pymedio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5510 2022-03-04 15:03:20.000000 pymedio-0.2.8/pymedio/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    23971 2022-03-04 15:03:20.000000 pymedio-0.2.8/pymedio/dicom.py
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-03-04 15:03:20.000000 pymedio-0.2.8/pymedio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    14306 2022-03-04 15:03:20.000000 pymedio-0.2.8/pymedio/functional.py
--rw-r--r--   0 runner    (1001) docker     (121)     7554 2022-03-04 15:03:20.000000 pymedio-0.2.8/pymedio/image.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-04 15:03:20.000000 pymedio-0.2.8/pymedio/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2022-03-04 15:03:20.000000 pymedio-0.2.8/pymedio/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     4849 2022-03-04 15:03:20.000000 pymedio-0.2.8/pymedio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 15:03:30.683376 pymedio-0.2.8/pymedio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-03-04 15:03:30.000000 pymedio-0.2.8/pymedio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-03-04 15:03:30.000000 pymedio-0.2.8/pymedio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-04 15:03:30.000000 pymedio-0.2.8/pymedio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-04 15:03:29.000000 pymedio-0.2.8/pymedio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-03-04 15:03:30.000000 pymedio-0.2.8/pymedio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-03-04 15:03:30.000000 pymedio-0.2.8/pymedio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-03-04 15:03:20.000000 pymedio-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-03-04 15:03:30.687376 pymedio-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-04 15:03:20.000000 pymedio-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 15:03:30.683376 pymedio-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-03-04 15:03:20.000000 pymedio-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11413 2022-03-04 15:03:20.000000 pymedio-0.2.8/tests/test_pymedio.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-11 17:26:49.715198 pymedio-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-03-11 17:26:29.000000 pymedio-0.2.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3481 2022-03-11 17:26:29.000000 pymedio-0.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-03-11 17:26:29.000000 pymedio-0.2.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11949 2022-03-11 17:26:29.000000 pymedio-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2022-03-11 17:26:29.000000 pymedio-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-03-11 17:26:49.715198 pymedio-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4456 2022-03-11 17:26:29.000000 pymedio-0.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-11 17:26:49.711198 pymedio-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2022-03-11 17:26:29.000000 pymedio-0.2.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-03-11 17:26:29.000000 pymedio-0.2.9/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5128 2022-03-11 17:26:29.000000 pymedio-0.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-03-11 17:26:29.000000 pymedio-0.2.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-03-11 17:26:29.000000 pymedio-0.2.9/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2022-03-11 17:26:29.000000 pymedio-0.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-03-11 17:26:29.000000 pymedio-0.2.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      767 2022-03-11 17:26:29.000000 pymedio-0.2.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-03-11 17:26:29.000000 pymedio-0.2.9/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-03-11 17:26:29.000000 pymedio-0.2.9/docs/pymedio.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-03-11 17:26:29.000000 pymedio-0.2.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-03-11 17:26:29.000000 pymedio-0.2.9/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-11 17:26:49.715198 pymedio-0.2.9/pymedio/
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2022-03-11 17:26:29.000000 pymedio-0.2.9/pymedio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7849 2022-03-11 17:26:29.000000 pymedio-0.2.9/pymedio/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24418 2022-03-11 17:26:29.000000 pymedio-0.2.9/pymedio/dicom.py
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-03-11 17:26:29.000000 pymedio-0.2.9/pymedio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14306 2022-03-11 17:26:29.000000 pymedio-0.2.9/pymedio/functional.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7554 2022-03-11 17:26:29.000000 pymedio-0.2.9/pymedio/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-11 17:26:29.000000 pymedio-0.2.9/pymedio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     1405 2022-03-11 17:26:29.000000 pymedio-0.2.9/pymedio/typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4832 2022-03-11 17:26:29.000000 pymedio-0.2.9/pymedio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-11 17:26:49.715198 pymedio-0.2.9/pymedio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-03-11 17:26:49.000000 pymedio-0.2.9/pymedio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2022-03-11 17:26:49.000000 pymedio-0.2.9/pymedio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-11 17:26:49.000000 pymedio-0.2.9/pymedio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-11 17:26:48.000000 pymedio-0.2.9/pymedio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-03-11 17:26:49.000000 pymedio-0.2.9/pymedio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-03-11 17:26:49.000000 pymedio-0.2.9/pymedio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-03-11 17:26:29.000000 pymedio-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-03-11 17:26:49.715198 pymedio-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-11 17:26:29.000000 pymedio-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-11 17:26:49.715198 pymedio-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-03-11 17:26:29.000000 pymedio-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12390 2022-03-11 17:26:29.000000 pymedio-0.2.9/tests/test_pymedio.py
```

### Comparing `pymedio-0.2.8/CONTRIBUTING.rst` & `pymedio-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pymedio-0.2.8/HISTORY.rst` & `pymedio-0.2.9/HISTORY.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =======
 History
 =======
 
+0.2.9 (2022-03-11)
+------------------
+
+* Add rudimentary ``resample_image`` to ``BasicImage``.
+* Add optional ``info`` string to ``BasicImage``.
+* Remove duplicate position images in ``remove_anomalous_image`` method (by default).
+
 0.2.8 (2022-03-04)
 ------------------
 
 * Bump minimum required numpy version to v1.22 since it's required for type annotations.
 
 0.2.7 (2022-02-24)
 ------------------
```

### Comparing `pymedio-0.2.8/LICENSE` & `pymedio-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymedio-0.2.8/PKG-INFO` & `pymedio-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymedio
-Version: 0.2.8
+Version: 0.2.9
 Summary: read arbitrary medical images in python
 Home-page: https://github.com/jcreinhold/pymedio
 Author: Jacob Reinhold
 Author-email: jcreinhold@gmail.com
 License: MIT license
 Project-URL: Bug Tracker, https://github.com/jcreinhold/pymedio/issues
 Project-URL: Documentation, https://pymedio.readthedocs.io/
```

### Comparing `pymedio-0.2.8/README.rst` & `pymedio-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `pymedio-0.2.8/docs/Makefile` & `pymedio-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymedio-0.2.8/docs/conf.py` & `pymedio-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pymedio-0.2.8/docs/installation.rst` & `pymedio-0.2.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pymedio-0.2.8/docs/make.bat` & `pymedio-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymedio-0.2.8/docs/pymedio.rst` & `pymedio-0.2.9/docs/pymedio.rst`

 * *Files identical despite different names*

### Comparing `pymedio-0.2.8/pymedio/base.py` & `pymedio-0.2.9/pymedio/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 from __future__ import annotations
 
 __all__ = ["BasicImage"]
 
 import builtins
+import collections.abc
 import typing
 import warnings
 
 import numpy as np
 import numpy.typing as npt
 
 import pymedio.typing as miot
@@ -27,26 +28,31 @@
     _affine: npt.NDArray
 
     def __new__(
         cls: typing.Type[_Image],
         data: npt.ArrayLike,
         affine: npt.NDArray | None = None,
         *,
+        info: builtins.str | npt.NDArray[np.str_] | None = None,
         copy: builtins.bool = False,
     ) -> _Image:
         obj = cls._check_data(data, copy=copy).view(cls)
         obj._affine = cls._check_affine(affine)
         obj._affine.flags.writeable = False
+        obj._info = cls._check_info(info)
+        obj._info.flags.writeable = False
         return obj
 
     def __array_finalize__(self, obj: builtins.object) -> None:
         if obj is None:
             return
         self._affine = self._check_affine(getattr(obj, "_affine", None))
         self._affine.flags.writeable = False
+        self._info = self._check_info(getattr(obj, "info", None))
+        self._info.flags.writeable = False
 
     @property
     def repr_properties(self) -> builtins.list[builtins.str]:
         return [
             f"shape: {self.shape}",
             f"spacing: {self.get_spacing_string()}",
             f"dtype: {self.dtype.name}",
@@ -65,14 +71,15 @@
         method: _UfuncMethod,
         *inputs: typing.Any,
         out: typing.Any = None,
         **kwargs: typing.Any,
     ) -> typing.Any:
 
         affine = self.affine
+        info = self.info
 
         ufunc_args = []
         for input_ in inputs:
             if isinstance(input_, BasicImage):
                 ufunc_args.append(input_.view(np.ndarray))
             else:
                 ufunc_args.append(input_)
@@ -90,35 +97,48 @@
             outputs = (None,) * ufunc.nout
 
         results = super().__array_ufunc__(ufunc, method, *ufunc_args, **kwargs)
 
         if method == "at":
             if isinstance(inputs[0], BasicImage):
                 inputs[0].affine = affine
+                inputs[0].info = info
             return
 
         if ufunc.nout == 1:
             results = (results,)
 
         results = tuple(
-            (self.__class__(np.asarray(result), affine) if output is None else output)
+            (
+                self.__class__(np.asarray(result), affine, info=info)
+                if output is None
+                else output
+            )
             for result, output in zip(results, outputs)
         )
 
         return results[0] if len(results) == 1 else results
 
     @property
     def affine(self) -> npt.NDArray[np.float64]:
         return self._affine
 
     @affine.setter
     def affine(self, new_affine: npt.NDArray) -> None:
         self._affine = self._check_affine(new_affine)
 
     @property
+    def info(self) -> npt.NDArray[np.str_]:
+        return self._affine
+
+    @info.setter
+    def info(self, new_info: builtins.str | npt.NDArray[np.str_] | None) -> None:
+        self._info = self._check_info(new_info)
+
+    @property
     def direction(self) -> miot.Direction:
         _, _, direction = miou.get_metadata_from_ras_affine(self.affine, lps=False)
         return direction
 
     @property
     def spacing(self) -> builtins.tuple[miot.Float, ...]:
         """Voxel spacing in mm."""
@@ -128,15 +148,15 @@
     @property
     def origin(self) -> builtins.tuple[miot.Float, ...]:
         """Center of first voxel in array, in mm."""
         return tuple(self.affine[:3, 3])
 
     @property
     def memory(self) -> miot.Int:
-        """Number of Bytes that the tensor takes in the RAM."""
+        """Number of bytes that the image array occupies in RAM"""
         mem: builtins.int = np.prod(self.shape) * self.itemsize
         return mem
 
     def get_spacing_string(self) -> builtins.str:
         strings = [f"{n:.2g}" for n in self.spacing]
         string = f'({", ".join(strings)})'
         return string
@@ -159,19 +179,60 @@
             bad_type = type(affine)
             raise TypeError(f"Affine must be a NumPy array, not {bad_type}")
         if affine.shape != (4, 4):
             bad_shape = affine.shape
             raise ValueError(f"Affine shape must be (4, 4), not {bad_shape}")
         return miou.to_f64(affine)
 
+    @staticmethod
+    def _check_info(
+        info: builtins.str | npt.NDArray[np.str_] | None,
+    ) -> npt.NDArray[np.str_]:
+        if info is None:
+            info = ""
+        return np.asarray(info, dtype=np.str_)
+
     def to_npz(self, file: miot.PathLike | typing.BinaryIO) -> None:
-        np.savez_compressed(file, data=np.asarray(self), affine=self.affine)
+        np.savez_compressed(
+            file, data=np.asarray(self), affine=self.affine, info=self.info
+        )
 
     @classmethod
     def from_npz(
         cls, file: miot.PathLike | typing.BinaryIO, **np_load_kwargs
     ) -> _Image:
         _data = np.load(file, **np_load_kwargs)
-        return cls(_data["data"], affine=_data["affine"])
+        return cls(_data["data"], affine=_data["affine"], info=_data["info"])
 
     def torch_compatible(self) -> npt.NDArray:
         return miou.ensure_4d(miou.check_uint_to_int(np.asarray(self)))
+
+    def resample_image(self, shape: collections.abc.Sequence[builtins.int]) -> _Image:
+        if self.ndim != len(shape):
+            raise ValueError("length of 'shape' != number of dimensions in image.")
+        if any(s <= 0 for s in shape):
+            raise ValueError("All elements of 'shape' must be positive.")
+        data = np.asarray(self)
+        resolution_scale = np.empty(len(shape), dtype=np.float64)
+        for i, (new_s, s) in enumerate(zip(shape, self.shape)):
+            resolution_scale[i] = s / new_s
+
+            def interpolate(fp: np.ndarray) -> np.ndarray:
+                return np.interp(
+                    np.linspace(0, s, dtype=self.dtype, endpoint=False, num=new_s),
+                    np.arange(0, s, dtype=self.dtype),
+                    fp,
+                )
+
+            data = np.apply_along_axis(interpolate, i, data)
+        # https://math.stackexchange.com/q/1120209
+        rzs = self.affine[:3, :3]  # rotation, scale (zoom), shear
+        rotation, zs = np.linalg.qr(rzs)
+        scale = zs.diagonal()
+        shear = zs * (1.0 / scale)
+        new_affine = np.zeros_like(self.affine)
+        new_scale = scale * resolution_scale
+        new_affine[:3, :3] = (rotation * new_scale) @ shear
+        new_affine[:, 3] = self.affine[:, 3]
+        return self.__class__(
+            data.astype(self.dtype, copy=False), new_affine, info=self.info
+        )
```

### Comparing `pymedio-0.2.8/pymedio/dicom.py` & `pymedio-0.2.9/pymedio/dicom.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,17 +146,16 @@
         cls, slice_datasets: typing.Sequence[pydicom.Dataset]
     ) -> SortedSlices:
         """sort list of pydicom datasets into the correct order"""
         if not slice_datasets:
             raise ValueError("slice_datasets empty")
         image_orientation = miou.to_f64(slice_datasets[0].ImageOrientationPatient)
         cosines = Cosines.from_orientation(image_orientation)
-        cs = cosines.slice
-        imps = (miou.to_f64(sd.ImagePositionPatient) for sd in slice_datasets)
-        positions = (np.dot(cs, imp).item() for imp in imps)
+        ipps = (miou.to_f64(sd.ImagePositionPatient) for sd in slice_datasets)
+        positions = (np.dot(cosines.slice, imp).item() for imp in ipps)
         _sorted = typing.cast(
             typing.Iterable[builtins.tuple[builtins.int, builtins.float]],
             sorted(enumerate(positions), key=operator.itemgetter(1)),
         )
         sorted_indices, sorted_positions = miou.unzip(_sorted)
         sorted_slice_datasets = tuple(slice_datasets[i] for i in sorted_indices)
         return cls(
@@ -182,30 +181,39 @@
                 else:
                     warnings.warn(msg)
             if not np.allclose(diffs, diffs[0], atol=0.0, rtol=missing_slices_cutoff):
                 msg = "There appear to be missing slices."
                 raise mioe.MissingSlicesException(msg)
 
     def remove_anomalous_slices(
-        self, *, strict_unique: builtins.bool = True
+        self,
+        *,
+        strict_unique_orientation: builtins.bool = True,
+        unique_positions: builtins.bool = True,
     ) -> SortedSlices:
         to_float_tuple = lambda xs: tuple(float(x) for x in xs)  # noqa: E731
         orientations = [to_float_tuple(s.ImageOrientationPatient) for s in self.slices]
-        if strict_unique:
+        if strict_unique_orientation:
             unq_oris: np.ndarray
             unq_oris, counts = np.unique(orientations, axis=0, return_counts=True)
             most_common_orientation = unq_oris[np.argmax(counts)]
         else:
             approx_unique_orientations = self._approx_unique(orientations)
             most_common_orientation = approx_unique_orientations[-1]
-        out = [
-            (s, idx, pos)
-            for s, idx, pos, o in self._zip(orientations)
-            if np.allclose(o, most_common_orientation, atol=ORIENTATION_ATOL)
-        ]
+        seen_positions = set()
+        out = []
+        for _slice, idx, pos, o in self._zip_with(orientations):
+            if np.allclose(o, most_common_orientation, atol=ORIENTATION_ATOL):
+                if unique_positions and pos in seen_positions:
+                    logger.debug(f"Slice at index {idx} has a non-unique position.")
+                    continue
+                out.append((_slice, idx, pos))
+                seen_positions.add(pos)
+            else:
+                logger.debug(f"Slice at index {idx} has a different orientation.")
         new_slices, new_indices, new_positions = miou.unzip(out)
         if (n_removed := (len(self) - len(new_slices))) > 1:
             warnings.warn(f"{n_removed} anomalous images removed.")
         elif n_removed < 0:
             raise RuntimeError("Images added in remove image func. Report error.")
         new_image_orientation = miou.to_f64(new_slices[0].ImageOrientationPatient)
         new_cosines = Cosines.from_orientation(new_image_orientation)
@@ -275,15 +283,15 @@
             sorted(
                 ((arr, count) for arr, count in approx_unique.items()),
                 key=operator.itemgetter(1),
             )
         )
         return approx_unq_arrs
 
-    def _zip(
+    def _zip_with(
         self, *args: typing.Iterable[typing.Any]
     ) -> typing.Iterable[builtins.tuple[typing.Any, ...]]:
         return zip(self.slices, self.indices, self.positions, *args)
 
 
 @dataclasses.dataclass(frozen=True)
 class DICOMDir:
```

### Comparing `pymedio-0.2.8/pymedio/functional.py` & `pymedio-0.2.9/pymedio/functional.py`

 * *Files identical despite different names*

### Comparing `pymedio-0.2.8/pymedio/image.py` & `pymedio-0.2.9/pymedio/image.py`

 * *Files identical despite different names*

### Comparing `pymedio-0.2.8/pymedio/typing.py` & `pymedio-0.2.9/pymedio/typing.py`

 * *Files identical despite different names*

### Comparing `pymedio-0.2.8/pymedio/utils.py` & `pymedio-0.2.9/pymedio/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 
 def get_rotation_and_spacing_from_affine(
     affine: npt.NDArray[miot.DType],
 ) -> builtins.tuple[npt.NDArray[miot.DType], npt.NDArray[miot.DType]]:
     # From https://github.com/nipy/nibabel/blob/master/nibabel/orientations.py
     rotation_zoom = affine[:3, :3]
-    spacing = np.sqrt(np.sum(rotation_zoom * rotation_zoom, axis=0))
+    spacing = np.linalg.norm(rotation_zoom, axis=0)
     rotation = rotation_zoom / spacing
     return rotation, spacing
 
 
 def get_metadata_from_ras_affine(
     affine: npt.NDArray,
     *,
```

### Comparing `pymedio-0.2.8/pymedio.egg-info/PKG-INFO` & `pymedio-0.2.9/pymedio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymedio
-Version: 0.2.8
+Version: 0.2.9
 Summary: read arbitrary medical images in python
 Home-page: https://github.com/jcreinhold/pymedio
 Author: Jacob Reinhold
 Author-email: jcreinhold@gmail.com
 License: MIT license
 Project-URL: Bug Tracker, https://github.com/jcreinhold/pymedio/issues
 Project-URL: Documentation, https://pymedio.readthedocs.io/
```

### Comparing `pymedio-0.2.8/pymedio.egg-info/SOURCES.txt` & `pymedio-0.2.9/pymedio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymedio-0.2.8/setup.cfg` & `pymedio-0.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 dicom = 
 	pydicom>=2
 
 [options.package_data]
 pymedio = py.typed
 
 [bumpversion]
-current_version = 0.2.8
+current_version = 0.2.9
 commit = True
 tag = True
 
 [bumpversion:file:pymedio/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
```

### Comparing `pymedio-0.2.8/tests/test_pymedio.py` & `pymedio-0.2.9/tests/test_pymedio.py`

 * *Files 7% similar despite different names*

```diff
@@ -301,14 +301,36 @@
 
 
 def test_convert_to_torch(image: mioi.Image) -> None:
     torch = pytest.importorskip("torch")
     torch.as_tensor(image.torch_compatible())
 
 
+def test_resize(image: mioi.Image, dicom_image: pydicom.Dataset) -> None:
+    new_shape = np.array(image.shape) * 2
+    resized = image.resample_image(new_shape)  # type: ignore[arg-type]
+    assert resized.shape == tuple(new_shape)
+    orig_spacing: np.ndarray = np.array(image.spacing)
+    new_spacing: np.ndarray = np.array(resized.spacing)
+    assert np.allclose(orig_spacing, new_spacing * 2)
+    assert resized.dtype == image.dtype
+
+    datasets = [dicom_image]
+    dcmdir = miod.DICOMDir.from_datasets(datasets)
+    dcmimg: miod.DICOMImage = miod.DICOMImage.from_dicomdir(dcmdir)
+    image = mioi.Image.from_dicom_image(dcmimg)
+    new_shape = np.array(image.shape) * 2
+    resized = image.resample_image(new_shape)  # type: ignore[arg-type]
+    assert resized.shape == tuple(new_shape)
+    orig_spacing = np.array(image.spacing)
+    new_spacing = np.array(resized.spacing)
+    assert np.allclose(orig_spacing, new_spacing * 2)
+    assert resized.dtype == image.dtype
+
+
 def test_save_image(
     tmp_path_factory: pytest.TempPathFactory, image: mioi.Image
 ) -> None:
     save_path = tmp_path_factory.mktemp("save").resolve(strict=True)
     image.save(save_path / "test.nii.gz")
```

