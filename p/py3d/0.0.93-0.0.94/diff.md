# Comparing `tmp/py3d-0.0.93.tar.gz` & `tmp/py3d-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.0.93.tar", last modified: Thu May 25 16:42:26 2023, max compression
+gzip compressed data, was "py3d-0.0.94.tar", last modified: Sat May 27 07:46:39 2023, max compression
```

## Comparing `py3d-0.0.93.tar` & `py3d-0.0.94.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 16:42:26.209101 py3d-0.0.93/
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-25 16:42:26.209101 py3d-0.0.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-05-25 16:42:15.000000 py3d-0.0.93/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 16:42:26.205101 py3d-0.0.93/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-25 16:42:15.000000 py3d-0.0.93/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27651 2023-05-25 16:42:15.000000 py3d-0.0.93/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22603 2023-05-25 16:42:15.000000 py3d-0.0.93/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 16:42:26.209101 py3d-0.0.93/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-25 16:42:26.000000 py3d-0.0.93/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-25 16:42:26.000000 py3d-0.0.93/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 16:42:26.000000 py3d-0.0.93/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-25 16:42:26.000000 py3d-0.0.93/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-25 16:42:26.000000 py3d-0.0.93/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 16:42:26.209101 py3d-0.0.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-25 16:42:15.000000 py3d-0.0.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 07:46:39.304303 py3d-0.0.94/
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-27 07:46:39.304303 py3d-0.0.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-05-27 07:46:25.000000 py3d-0.0.94/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 07:46:39.300303 py3d-0.0.94/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-27 07:46:25.000000 py3d-0.0.94/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27964 2023-05-27 07:46:25.000000 py3d-0.0.94/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22609 2023-05-27 07:46:25.000000 py3d-0.0.94/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 07:46:39.304303 py3d-0.0.94/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-27 07:46:39.000000 py3d-0.0.94/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-27 07:46:39.000000 py3d-0.0.94/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-27 07:46:39.000000 py3d-0.0.94/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-27 07:46:39.000000 py3d-0.0.94/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-27 07:46:39.000000 py3d-0.0.94/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-27 07:46:39.304303 py3d-0.0.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-27 07:46:25.000000 py3d-0.0.94/setup.py
```

### Comparing `py3d-0.0.93/PKG-INFO` & `py3d-0.0.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.93
+Version: 0.0.94
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.0.93/README.md` & `py3d-0.0.94/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.0.93/py3d/core.py` & `py3d-0.0.94/py3d/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Dict
 import pathlib
 import uuid
 import json
 import struct
 
 pi = numpy.arccos(-1)
+__module__ = __import__(__name__)
 
 
 def sign(v):
     return numpy.sign(v, where=v != 0, out=numpy.ones_like(v))
 
 
 class View:
@@ -123,15 +124,18 @@
                 break
             tmp = []
             for s, t in zip(size, tp):
                 bt = f.read(s)
                 d, = struct.unpack(tp_map[(s, t)], bt)
                 tmp.append(d)
             ret.append(tmp)
-    return Vector(ret)
+    ret = Vector(ret)
+    for i, c in enumerate(cols):
+        setattr(ret, c, ret[:, i])
+    return ret
 
 
 class Data(numpy.ndarray):
     BASE_SHAPE = ()
 
     def __new__(cls, data: list | numpy.ndarray = [], n=()):
         return numpy.tile(data, n + (1,)).view(cls)
@@ -208,22 +212,31 @@
 
     @xyz.setter
     def xyz(self, v):
         self[..., 0:3] = v
 
     @property
     def U(self) -> Vector:
-        # unit vector, direction vector
+        '''
+        unit vector, direction vector
+        '''
         n = self.L
         return numpy.divide(self, n, where=n != 0)
 
     @property
     def H(self) -> Vector:
-        # Homogeneous vector
-        return numpy.insert(self, self.shape[-1], 1, axis=self.ndim-1).view(Vector)
+        '''
+        Homogeneous vector
+        '''
+        ret = numpy.insert(self, self.shape[-1], 1, axis=self.ndim-1)
+        w = ret.shape[-1]
+        if w in [2, 3, 4]:
+            return ret.view(getattr(__module__, f"Vector{w}"))
+        else:
+            return ret.view(Vector)
 
     @property
     def M(self) -> Vector:
         # mean vector
         return super().mean(axis=self.ndim-2)
 
     @property
@@ -370,15 +383,15 @@
         '''
         x = numpy.array(x)
         xp = numpy.array(xp)
         assert x.ndim <= xp.ndim == 1
         i = numpy.searchsorted(xp, x).clip(1, len(xp)-1)
         x0 = xp[i-1]
         x1 = xp[i]
-        d = ((x-x0)/(x1-x0)).reshape(-1,1)
+        d = ((x-x0)/(x1-x0)).reshape(-1, 1)
         f0 = self[i-1]
         f1 = self[i]
         return (1-d)*f0+d*f1
 
     def as_scaling(self) -> Transform:
         ret = Transform(n=self.n)
         ret[..., 0, 0] = self[..., 0]
```

### Comparing `py3d-0.0.93/py3d/viewer.html` & `py3d-0.0.94/py3d/viewer.html`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
                 0, 0, 1, 0,
                 0, 0, 0, 1]
         }
         static orthographic(fovy, aspect, near, far, distance) {
             return [
                 1 / aspect / distance / Math.tan(fovy / 2), 0, 0, 0,
                 0, 1 / distance / Math.tan(fovy / 2), 0, 0,
-                0, 0, 1 / (near - far), 0,
-                0, 0, near / (far - near), 1]
+                0, 0, -1 / (near - far), 0,
+                0, 0, -near / (far - near), 1]
         }
         static perspective(fovy, aspect, near, far) {
             const f = 1 / Math.tan(fovy / 2)
             return [
                 f / aspect, 0, 0, 0,
                 0, f, 0, 0,
                 0, 0, -(near + far) / (far - near), -1,
@@ -83,22 +83,22 @@
             }
             ret[12] = -m[12]
             ret[13] = -m[13]
             ret[14] = -m[14]
             return ret
         }
         static rgb2hex(r, g, b, a) {
-            return "#" + ((1 << 24) + (r * 255 << 16) + (g * 255 << 8) + b * 255 ).toString(16).slice(1)
+            return "#" + ((1 << 24) + (r * 255 << 16) + (g * 255 << 8) + b * 255).toString(16).slice(1)
         }
         static fround(value, digits) {
-            let tmp = 10**digits
+            let tmp = 10 ** digits
             return Math.round(value * tmp) / tmp
         }
         static fceil(value, digits) {
-            let tmp = 10**digits
+            let tmp = 10 ** digits
             return Math.ceil(value * tmp) / tmp
         }
         static ticks(min, max, step) {
             if (max <= min) {
                 return [[min], min, max]
             }
             let dig = Math.max(0, -Math.round(Math.log10(step)))
@@ -428,15 +428,15 @@
             let ny = p[1] / p[3]
             let nz = p[2] / p[3]
             if (Math.abs(nx) <= 1 && Math.abs(ny) <= 1 && Math.abs(nz) <= 1) {
                 let x = 0.5 * (1 + nx) * this.canvas.width
                 let y = 0.5 * (1 - ny) * this.canvas.height
                 div.style.left = x + "px"
                 div.style.top = y + "px"
-                if (typeof(color) == "string") {
+                if (typeof (color) == "string") {
                     div.style.color = color
                 } else {
                     div.style.color = mat.rgb2hex(color)
                     div.style.opacity = color[color.length - 1]
                 }
                 div.style.pointerEvents = "none"
                 this.labeldiv.append(div)
```

### Comparing `py3d-0.0.93/py3d.egg-info/PKG-INFO` & `py3d-0.0.94/py3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.93
+Version: 0.0.94
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.0.93/setup.py` & `py3d-0.0.94/setup.py`

 * *Files identical despite different names*

