# Comparing `tmp/morpholib-0.7.0.dev1.tar.gz` & `tmp/morpholib-0.7.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\ksmall\Documents\Kenneth's stuff\Python\Morpho\pip\v0.7.0\dist\.tmp-e0ya94jd\morpholib-0.7.0.dev1.tar", last modified: Thu Mar  9 16:47:04 2023, max compression
+gzip compressed data, was "C:\Users\ksmall\Documents\Kenneth's stuff\Python\Morpho\pip\v0.7.1-test\dist\.tmp-zkv1ja08\morpholib-0.7.1.dev1.tar", last modified: Sat May 27 15:03:36 2023, max compression
```

## Comparing `morpholib-0.7.0.dev1.tar` & `morpholib-0.7.1.dev1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 16:47:04.201379 morpholib-0.7.0.dev1/
--rw-rw-rw-   0        0        0     1091 2021-09-29 20:39:14.000000 morpholib-0.7.0.dev1/LICENSE
--rw-rw-rw-   0        0        0     4151 2023-03-09 16:47:04.201379 morpholib-0.7.0.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     3762 2023-03-09 16:43:42.000000 morpholib-0.7.0.dev1/README.md
--rw-rw-rw-   0        0        0      110 2021-09-27 17:28:21.000000 morpholib-0.7.0.dev1/pyproject.toml
--rw-rw-rw-   0        0        0      665 2023-03-09 16:47:04.203379 morpholib-0.7.0.dev1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-09 16:47:04.096373 morpholib-0.7.0.dev1/src/
-drwxrwxrwx   0        0        0        0 2023-03-09 16:47:04.161377 morpholib-0.7.0.dev1/src/morpholib/
--rw-rw-rw-   0        0        0      459 2022-12-26 17:15:37.000000 morpholib-0.7.0.dev1/src/morpholib/__init__.py
--rw-rw-rw-   0        0        0    10478 2022-08-25 17:03:00.000000 morpholib-0.7.0.dev1/src/morpholib/actions.py
--rw-rw-rw-   0        0        0   162242 2023-03-09 16:23:34.000000 morpholib-0.7.0.dev1/src/morpholib/anim.py
--rw-rw-rw-   0        0        0    25632 2023-03-09 16:37:42.000000 morpholib-0.7.0.dev1/src/morpholib/base.py
--rw-rw-rw-   0        0        0     4241 2023-03-09 16:23:34.000000 morpholib-0.7.0.dev1/src/morpholib/bezier.py
--rw-rw-rw-   0        0        0    29327 2023-03-09 16:23:34.000000 morpholib-0.7.0.dev1/src/morpholib/calculus.py
--rw-rw-rw-   0        0        0    35954 2022-11-20 21:53:04.000000 morpholib-0.7.0.dev1/src/morpholib/color.py
--rw-rw-rw-   0        0        0      512 2022-12-26 17:15:37.000000 morpholib-0.7.0.dev1/src/morpholib/combo.py
--rw-rw-rw-   0        0        0    84780 2023-03-09 16:23:34.000000 morpholib-0.7.0.dev1/src/morpholib/figure.py
--rw-rw-rw-   0        0        0     9153 2023-03-09 16:23:34.000000 morpholib-0.7.0.dev1/src/morpholib/gadgets.py
--rw-rw-rw-   0        0        0     2513 2022-03-08 00:05:51.000000 morpholib-0.7.0.dev1/src/morpholib/giffer.py
--rw-rw-rw-   0        0        0     1721 2022-03-08 00:05:51.000000 morpholib-0.7.0.dev1/src/morpholib/graph.py
--rw-rw-rw-   0        0        0    41390 2023-03-09 16:23:34.000000 morpholib-0.7.0.dev1/src/morpholib/graphics.py
--rw-rw-rw-   0        0        0   183667 2023-03-09 16:23:34.000000 morpholib-0.7.0.dev1/src/morpholib/grid.py
--rw-rw-rw-   0        0        0     4019 2023-03-09 16:23:34.000000 morpholib-0.7.0.dev1/src/morpholib/latex.py
--rw-rw-rw-   0        0        0    12725 2022-12-26 17:15:37.000000 morpholib-0.7.0.dev1/src/morpholib/matrix.py
--rw-rw-rw-   0        0        0      709 2022-08-01 17:17:30.000000 morpholib-0.7.0.dev1/src/morpholib/sample.py
--rw-rw-rw-   0        0        0   108708 2023-03-09 16:23:34.000000 morpholib-0.7.0.dev1/src/morpholib/shapes.py
--rw-rw-rw-   0        0        0    80077 2023-03-09 16:23:34.000000 morpholib-0.7.0.dev1/src/morpholib/text.py
-drwxrwxrwx   0        0        0        0 2023-03-09 16:47:04.199379 morpholib-0.7.0.dev1/src/morpholib/tools/
--rw-rw-rw-   0        0        0       72 2022-03-08 00:05:51.000000 morpholib-0.7.0.dev1/src/morpholib/tools/__init__.py
--rw-rw-rw-   0        0        0        4 2022-03-08 00:05:51.000000 morpholib-0.7.0.dev1/src/morpholib/tools/base.py
--rw-rw-rw-   0        0        0    10924 2023-03-09 16:23:34.000000 morpholib-0.7.0.dev1/src/morpholib/tools/basics.py
--rw-rw-rw-   0        0        0       31 2022-06-16 19:16:16.000000 morpholib-0.7.0.dev1/src/morpholib/tools/color.py
--rw-rw-rw-   0        0        0     9182 2023-03-09 16:23:34.000000 morpholib-0.7.0.dev1/src/morpholib/tools/dev.py
--rw-rw-rw-   0        0        0     2093 2022-03-08 00:05:51.000000 morpholib-0.7.0.dev1/src/morpholib/tools/ktimer.py
--rw-rw-rw-   0        0        0     6348 2023-03-09 16:23:34.000000 morpholib-0.7.0.dev1/src/morpholib/tools/latex2svg.py
--rw-rw-rw-   0        0        0      811 2022-03-08 00:05:51.000000 morpholib-0.7.0.dev1/src/morpholib/tools/subimporter.py
--rw-rw-rw-   0        0        0     5098 2022-12-27 03:55:19.000000 morpholib-0.7.0.dev1/src/morpholib/transitions.py
--rw-rw-rw-   0        0        0     9128 2022-06-16 19:16:16.000000 morpholib-0.7.0.dev1/src/morpholib/video.py
-drwxrwxrwx   0        0        0        0 2023-03-09 16:47:04.176377 morpholib-0.7.0.dev1/src/morpholib.egg-info/
--rw-rw-rw-   0        0        0     4151 2023-03-09 16:47:04.000000 morpholib-0.7.0.dev1/src/morpholib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      974 2023-03-09 16:47:04.000000 morpholib-0.7.0.dev1/src/morpholib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 16:47:04.000000 morpholib-0.7.0.dev1/src/morpholib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-03-09 16:47:04.000000 morpholib-0.7.0.dev1/src/morpholib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-09 16:47:04.000000 morpholib-0.7.0.dev1/src/morpholib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 15:03:36.894612 morpholib-0.7.1.dev1/
+-rw-rw-rw-   0        0        0     1091 2021-09-29 20:39:14.000000 morpholib-0.7.1.dev1/LICENSE
+-rw-rw-rw-   0        0        0     4356 2023-05-27 15:03:36.894612 morpholib-0.7.1.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     3967 2023-05-27 15:02:41.000000 morpholib-0.7.1.dev1/README.md
+-rw-rw-rw-   0        0        0      110 2021-09-27 17:28:21.000000 morpholib-0.7.1.dev1/pyproject.toml
+-rw-rw-rw-   0        0        0      665 2023-05-27 15:03:36.894612 morpholib-0.7.1.dev1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 15:03:36.785412 morpholib-0.7.1.dev1/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 15:03:36.847813 morpholib-0.7.1.dev1/src/morpholib/
+-rw-rw-rw-   0        0        0      459 2022-12-26 17:15:37.000000 morpholib-0.7.1.dev1/src/morpholib/__init__.py
+-rw-rw-rw-   0        0        0    10495 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/actions.py
+-rw-rw-rw-   0        0        0   172890 2023-05-26 22:47:05.000000 morpholib-0.7.1.dev1/src/morpholib/anim.py
+-rw-rw-rw-   0        0        0    28588 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/base.py
+-rw-rw-rw-   0        0        0     4241 2023-03-12 21:13:07.000000 morpholib-0.7.1.dev1/src/morpholib/bezier.py
+-rw-rw-rw-   0        0        0    29327 2023-03-09 16:23:34.000000 morpholib-0.7.1.dev1/src/morpholib/calculus.py
+-rw-rw-rw-   0        0        0    36375 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/color.py
+-rw-rw-rw-   0        0        0      512 2022-12-26 17:15:37.000000 morpholib-0.7.1.dev1/src/morpholib/combo.py
+-rw-rw-rw-   0        0        0    86385 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/figure.py
+-rw-rw-rw-   0        0        0    10763 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/gadgets.py
+-rw-rw-rw-   0        0        0     2513 2022-03-08 00:05:51.000000 morpholib-0.7.1.dev1/src/morpholib/giffer.py
+-rw-rw-rw-   0        0        0     9517 2023-05-26 22:47:05.000000 morpholib-0.7.1.dev1/src/morpholib/graph.py
+-rw-rw-rw-   0        0        0    42139 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/graphics.py
+-rw-rw-rw-   0        0        0   193540 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/grid.py
+-rw-rw-rw-   0        0        0     6428 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/latex.py
+-rw-rw-rw-   0        0        0    13144 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/matrix.py
+-rw-rw-rw-   0        0        0      709 2022-08-01 17:17:30.000000 morpholib-0.7.1.dev1/src/morpholib/sample.py
+-rw-rw-rw-   0        0        0   113081 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/shapes.py
+-rw-rw-rw-   0        0        0    80385 2023-05-26 22:47:05.000000 morpholib-0.7.1.dev1/src/morpholib/text.py
+drwxrwxrwx   0        0        0        0 2023-05-27 15:03:36.894612 morpholib-0.7.1.dev1/src/morpholib/tools/
+-rw-rw-rw-   0        0        0       72 2022-03-08 00:05:51.000000 morpholib-0.7.1.dev1/src/morpholib/tools/__init__.py
+-rw-rw-rw-   0        0        0        4 2022-03-08 00:05:51.000000 morpholib-0.7.1.dev1/src/morpholib/tools/base.py
+-rw-rw-rw-   0        0        0    11946 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/tools/basics.py
+-rw-rw-rw-   0        0        0       31 2022-06-16 19:16:16.000000 morpholib-0.7.1.dev1/src/morpholib/tools/color.py
+-rw-rw-rw-   0        0        0    12210 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/tools/dev.py
+-rw-rw-rw-   0        0        0     2093 2022-03-08 00:05:51.000000 morpholib-0.7.1.dev1/src/morpholib/tools/ktimer.py
+-rw-rw-rw-   0        0        0     6348 2023-04-25 17:14:02.000000 morpholib-0.7.1.dev1/src/morpholib/tools/latex2svg.py
+-rw-rw-rw-   0        0        0      811 2022-03-08 00:05:51.000000 morpholib-0.7.1.dev1/src/morpholib/tools/subimporter.py
+-rw-rw-rw-   0        0        0     5370 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/transitions.py
+-rw-rw-rw-   0        0        0     9128 2022-06-16 19:16:16.000000 morpholib-0.7.1.dev1/src/morpholib/video.py
+drwxrwxrwx   0        0        0        0 2023-05-27 15:03:36.863412 morpholib-0.7.1.dev1/src/morpholib.egg-info/
+-rw-rw-rw-   0        0        0     4356 2023-05-27 15:03:36.000000 morpholib-0.7.1.dev1/src/morpholib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      974 2023-05-27 15:03:36.000000 morpholib-0.7.1.dev1/src/morpholib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 15:03:36.000000 morpholib-0.7.1.dev1/src/morpholib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-05-27 15:03:36.000000 morpholib-0.7.1.dev1/src/morpholib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-27 15:03:36.000000 morpholib-0.7.1.dev1/src/morpholib.egg-info/top_level.txt
```

### Comparing `morpholib-0.7.0.dev1/LICENSE` & `morpholib-0.7.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.0.dev1/PKG-INFO` & `morpholib-0.7.1.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morpholib
-Version: 0.7.0.dev1
+Version: 0.7.1.dev1
 Summary: A general-purpose programmatic animation tool
 Home-page: https://github.com/morpho-matters/morpholib
 Author: Kenneth Small
 Author-email: morpho.matters@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -51,14 +51,16 @@
 
 If you want to export animations as MP4s or small-sized GIFs, you will need to install [FFmpeg](https://ffmpeg.org/) for MP4 and/or [Gifsicle](https://www.lcdf.org/gifsicle/) for GIF. But if that doesn't matter to you (or if you just want to try out Morpho), you can still preview animations and export them as PNG sequences and large-sized GIFs just using the base installation of Morpho.
 
 Please note that FFmpeg and Gifsicle will need to be added to your PATH environment variable for Morpho to be able to access them by default.
 
 For Morpho to be able to parse LaTeX code, you must have a LaTeX distribution installed along with [dvisvgm](https://dvisvgm.de/). But if you're okay with not using Morpho's LaTeX features, this requirement is optional.
 
+SciPy is an optional, but recommended, dependency that is necessary currently for only few features (`flowStreamer` and `FlowField`). SciPy can be installed via pip with the command `pip install scipy`
+
 ### Testing the installation
 
 To see if it installed correctly, try running the following Python code:
 
 ```python
 import morpholib as morpho
 morpho.importAll()
```

### Comparing `morpholib-0.7.0.dev1/README.md` & `morpholib-0.7.1.dev1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 
 If you want to export animations as MP4s or small-sized GIFs, you will need to install [FFmpeg](https://ffmpeg.org/) for MP4 and/or [Gifsicle](https://www.lcdf.org/gifsicle/) for GIF. But if that doesn't matter to you (or if you just want to try out Morpho), you can still preview animations and export them as PNG sequences and large-sized GIFs just using the base installation of Morpho.
 
 Please note that FFmpeg and Gifsicle will need to be added to your PATH environment variable for Morpho to be able to access them by default.
 
 For Morpho to be able to parse LaTeX code, you must have a LaTeX distribution installed along with [dvisvgm](https://dvisvgm.de/). But if you're okay with not using Morpho's LaTeX features, this requirement is optional.
 
+SciPy is an optional, but recommended, dependency that is necessary currently for only few features (`flowStreamer` and `FlowField`). SciPy can be installed via pip with the command `pip install scipy`
+
 ### Testing the installation
 
 To see if it installed correctly, try running the following Python code:
 
 ```python
 import morpholib as morpho
 morpho.importAll()
```

### Comparing `morpholib-0.7.0.dev1/setup.cfg` & `morpholib-0.7.1.dev1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f72 7068 6f6c 6962 0d0a 7665   = morpholib..ve
-00000020: 7273 696f 6e20 3d20 302e 372e 302e 6465  rsion = 0.7.0.de
+00000020: 7273 696f 6e20 3d20 302e 372e 312e 6465  rsion = 0.7.1.de
 00000030: 7631 0d0a 6175 7468 6f72 203d 204b 656e  v1..author = Ken
 00000040: 6e65 7468 2053 6d61 6c6c 0d0a 6175 7468  neth Small..auth
 00000050: 6f72 5f65 6d61 696c 203d 206d 6f72 7068  or_email = morph
 00000060: 6f2e 6d61 7474 6572 7340 676d 6169 6c2e  o.matters@gmail.
 00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000080: 203d 2041 2067 656e 6572 616c 2d70 7572   = A general-pur
 00000090: 706f 7365 2070 726f 6772 616d 6d61 7469  pose programmati
```

### Comparing `morpholib-0.7.0.dev1/src/morpholib/actions.py` & `morpholib-0.7.1.dev1/src/morpholib/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         return
 
     # Add dz in place to all supported tweenables
     for tweenable in figure._state.values():
         if (tweenable.name in autoJumpNames and "nojump" not in tweenable.tags) \
             or ("jump" in tweenable.tags):
 
-            tweenable.value += dz
+            tweenable.value = tweenable.value + dz
 
         # This clause works, but doesn't handle alpha.
         # I've decided not to use it for now.
         # elif "figures" in tweenable.tags:
         #     figlist = tweenable.value
         #     for fig in figlist:
         #         _applyJump(fig, dz)
```

### Comparing `morpholib-0.7.0.dev1/src/morpholib/anim.py` & `morpholib-0.7.1.dev1/src/morpholib/anim.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 cr = cairo
 
 import morpholib as morpho
 import morpholib.transitions, morpholib.giffer
 from morpholib.tools.basics import *
 from morpholib.tools.ktimer import tic, toc
 import morpholib.tools.dev
+from morpholib.tools.dev import BoundingBoxFigure, makesubcopies, listselect
 
 # Backward compatibility because these functions used to live in anim.py
 from morpholib import screenCoords, physicalCoords, \
     pixelWidth, physicalWidth, pixelHeight, physicalHeight, \
     setupContext, clearContext, cairoJointStyle, object_hasattr
 
 import math, cmath
@@ -67,24 +68,36 @@
 
 class LayerMergeError(MergeError):
     pass
 
 class MaskConfigurationError(Exception):
     pass
 
+class AmbiguousValueError(ValueError):
+    pass
+
 ### CLASSES ###
 
 # Mainly for internal use.
 # Object created when the `sub` property is used in a Frame object.
 # Allows one to modify the attributes of the subfigures of a frame
 # all at once.
 class _SubAttributeManager(object):
-    def __init__(self, frame, /):
+    # `frame` is the Frame on which `.all` is being called.
+    # `origframe` is the Frame that should be returned by
+    # the set() method. If unspecified, it defaults to the
+    # value of `frame`. This is useful when calling .select[]
+    # since the return value of set() will be the true original
+    # Frame including unselected subfigures.
+    def __init__(self, frame, origframe=None, /):
+        if origframe is None:
+            origframe = frame
         # Bypass native setattr() because it's overridden below.
         object.__setattr__(self, "_subattrman_frame", frame)
+        object.__setattr__(self, "_subattrman_origframe", origframe)
 
     # Returns a function that when called will call the
     # corresponding method across all subfigures in the
     # Frame and collect their return values into a list
     # which will then be returned.
     def _subattrman_createSubmethod(self, name):
         def submethod(*args, **kwargs):
@@ -101,39 +114,35 @@
         try:
             commonValue = getattr(frame.figures[0], name)
         except AttributeError:
             raise AttributeError(f"Subfigures do not all possess attribute `{name}`")
         except IndexError:
             raise IndexError("Frame has no subfigures.")
 
-        # Convert tuple to list to facilitate possible
-        # cross-container comparisons later on.
-        # Also makes a copy of the list if it's already a list.
-        if isinstance(commonValue, (list, tuple)):
-            commonValue = list(commonValue)
+        commonValue_is_list_or_tuple = isinstance(commonValue, (list, tuple))
 
         # Check if the attribute is common to all the
         # subfigures and having the same value
         for subfigure in frame.figures:
             try:
                 value = getattr(subfigure, name)
             except AttributeError:
                 raise AttributeError(f"Subfigures do not all possess attribute `{name}`")
 
-            # Convert tuple to list so that cross-container comparison
-            # with commonValue will work
-            if isinstance(value, tuple) and isinstance(commonValue, list):
-                value = list(value)
+            if commonValue_is_list_or_tuple and isinstance(value, (list, tuple)):
+                # Convert value to commonValue's type so that cross-container
+                # comparison with commonValue will work
+                value = type(commonValue)(value)
             # Check if they are unequal
             if not isequal(value, commonValue):  # isequal() handles np.arrays too
                 if callable(commonValue):
                     return self._subattrman_createSubmethod(name)
-                raise ValueError(f"Subfigures do not have a common value for attribute `{name}`")
+                raise AmbiguousValueError(f"Subfigures do not have a common value for attribute `{name}`")
 
-        return commonValue
+        return commonValue if not isinstance(commonValue, (list, np.ndarray)) else commonValue.copy()
 
     def __setattr__(self, name, value):
         # Handle ordinary attribute sets if self possesses
         # the attribute.
         if object_hasattr(self, name):
             object.__setattr__(self, name, value)
 
@@ -141,15 +150,51 @@
         frame = self._subattrman_frame
         for subfigure in frame.figures:
             setattr(subfigure, name, value)
 
     def set(self, **kwargs):
         for name, value in kwargs.items():
             setattr(self, name, value)
-        return self._subattrman_frame
+        return self._subattrman_origframe
+
+
+class _MetaArray(np.ndarray):
+    """Array with metadata.
+    Thanks to @Bertrand L on StackOverflow for this!
+    https://stackoverflow.com/a/34967782"""
+
+    def __new__(cls, array, dtype=None, order=None, **kwargs):
+        obj = np.asarray(array, dtype=dtype, order=order).view(cls)
+        obj.metadata = kwargs
+        return obj
+
+    def __array_finalize__(self, obj):
+        if obj is None: return
+        self.metadata = getattr(obj, 'metadata', None)
+
+# Special version of _SubAttributeManager which in the case of an
+# AmbiguousValueError, returns a MetaArray of the values across all
+# subfigures. Mainly used for enabling the .iall and .iselect
+# features for subfigure in-place operations.
+class _InPlaceSubAttributeManager(_SubAttributeManager):
+    def __getattr__(self, name):
+        try:
+            return _SubAttributeManager.__getattr__(self, name)
+        except AmbiguousValueError:
+            # A MetaArray is used in order to distinguish these object arrays
+            # from regular numpy object arrays just in case a user is trying
+            # to update a value that is already natively an object array.
+            return _MetaArray([getattr(subfig, name) for subfig in self._subattrman_frame.figures], dtype=object)
+
+    def __setattr__(self, name, value):
+        if isinstance(value, _MetaArray):
+            for subfig, subvalue in zip(self._subattrman_frame.figures, value.tolist()):
+                setattr(subfig, name, subvalue)
+        else:
+            _SubAttributeManager.__setattr__(self, name, value)
 
 
 # Frame class. Groups figures together for simultaneous drawing.
 # Syntax: myframe = Frame(list_of_figures, **kwargs)
 #
 # Note that arbitrary keyword arguments can be supplied to the
 # Frame constructor, in which case they will be interpreted as
@@ -225,14 +270,32 @@
         # self.delay = 0
 
         # # Other (non-tweenable) attributes
         # self.delay = 0  # number of frames to delay at keyframe
 
         # self.defaultTween = Frame.tweenLinear
 
+    @property
+    def numfigs(self):
+        return len(self.figures)
+
+    # Modified because checking if the two figure lists are
+    # equal via vanilla Python list equality will not work.
+    # Instead, it goes thru the figure lists of self and other
+    # and checks if all corresponding figures appear equal.
+    def _appearsEqual(self, other, ignore=(), *args,
+        compareNonTweenables=False, compareSubNonTweenables=False, **kwargs):
+
+        ignore = set(ignore)
+        self_figures = self.figures
+        other_figures = other.figures
+        return morpho.Figure._appearsEqual(self, other, ignore=ignore.union({"figures"}), *args, compareNonTweenables=compareNonTweenables, **kwargs) and \
+            len(self_figures) == len(other_figures) and \
+            all(self_subfig._appearsEqual(other_subfig, ignore, *args, compareNonTweenables=(compareSubNonTweenables or compareNonTweenables), **kwargs) for self_subfig, other_subfig in zip(self_figures, other_figures))
+
     # # Returns True iff the "stylistic" attributes of two frames match
     # # i.e. their views, indices, and defaultTweens match.
     # # This can be used as a criterion on whether or not merging two frames
     # # can be done without affecting the other frame.
     # def matchesStyle(self, other):
     #     return self.defaultTween==other.defaultTween
 
@@ -260,53 +323,131 @@
         self.figures.extend(other.figures)
         return self
 
     @property
     def all(self):
         return _SubAttributeManager(self)
 
-    def _select(self, index, *, _asFrame=False):
-        if callable(index):
-            condition = index
-            selection = [fig for fig in self.figures if condition(fig)]
-        else:
-            selection = self.figures[index]
+    # Version of .all that is only meant to be used for in-place
+    # operations like `+=`.
+    # Example: myframe.iall[:3].pos += 2j
+    @property
+    def iall(self):
+        return _InPlaceSubAttributeManager(self)
+
+    def _select(self, index, *, _asFrame=False, _iall=False):
+        selection = list(listselect(self.figures, index).values())
 
         frm = type(self)(selection)
         frm._updateFrom(self, ignore="figures")
         if _asFrame:
             return frm
         else:
-            return frm.all
+            return _InPlaceSubAttributeManager(frm, self) if _iall else _SubAttributeManager(frm, self)
+
+    def _iselect(self, *args, **kwargs):
+        return self._select(*args, _iall=True, **kwargs)
 
     # Allows the modification of a subset of the subfigures
     # with the syntax:
     #   myframe.select[1:4].set(...)
     # You can also specify a choice function. That is, a function
     # that takes a subfigure as input and returns a boolean on
     # whether that figure should be selected.
     #   myframe.select[lambda fig: fig.width==0].set(...)
     @property
     def select(self):
         return morpho.tools.dev.Slicer(getter=self._select)
 
+    # Version of .select[] that is only meant to be used for in-place
+    # operations like `+=`.
+    # Example: myframe.iselect[:3].pos += 2j
+    @property
+    def iselect(self):
+        return morpho.tools.dev.Slicer(getter=self._iselect)
+
+
     def _sub(self, index):
         return self._select(index, _asFrame=True).copy()
 
     # Extracts a subframe of subfigures from the Frame.
     # Subfigures can be selected either via slice notation
     #   subframe = myframe.sub[1:4]
     # Or by choice function:
     #   subframe = myframe.sub[lambda fig: fig.width==0]
     # Note that the subfigures selected will be copied.
     @property
     def sub(self):
         return morpho.tools.dev.Slicer(getter=self._sub)
 
+    def _cut(self, index):
+
+        # Using _select() instead of sub[] here because
+        # we do NOT want to make copies of the subfigures
+        # in this case.
+        subframe = self._select(index, _asFrame=True)
+        figures = list(self.figures)
+        for subfig in subframe.figures:
+            while subfig in figures:
+                figures.remove(subfig)
+        self.figures = figures
+        return subframe
+
+    # Basically the same as sub[], but it also removes the selected
+    # subfigures from self's figure list. The selected subfiures
+    # are NOT copied since they are removed from self's figure list.
+    @property
+    def cut(self):
+        return morpho.tools.dev.Slicer(getter=self._cut)
+
+
+    # Partitions the Frame into a Frame of subframes
+    # splitting at the given list of indices.
+    #
+    # For example, `frm.partition([3, 6, 10])`
+    # will return a new Frame consisting of the 4 subframes
+    # frm.sub[:3], frm.sub[3:6], frm.sub[6:10], frm.sub[10:]
+    # in that order.
+    #
+    # Note that partition() will leave the original Frame figure
+    # that called it unchanged, and will return a new Frame
+    # of copies of the underlying subfigures per chunk.
+    #
+    # Subfigure names currently do not transfer.
+    def partition(self, indices):
+        if len(indices) == 0:
+            return Frame([self.sub[:]])
+
+        # Divide any negative indices mod len(self.figures)
+        # so they will be in the correct order relative to
+        # positive indices.
+        for n, index in enumerate(indices):
+            if index < 0:
+                indices[n] = index % len(self.figures)
+
+        chunks = []
+        chunks.append(self.sub[:indices[0]])
+        for n in range(1,len(indices)):
+            chunks.append(self.sub[indices[n-1] : indices[n]])
+        chunks.append(self.sub[indices[n]:])
+
+        return Frame(chunks)
 
+    # Given a Frame of subframes generated from calling partition(),
+    # combine() recombines them back into a single Frame figure.
+    #
+    # This method may not combine them perfectly if transformation
+    # tweenables of the underlying subframes were modified
+    # (e.g. `origin`) since these will not be transferred to the
+    # subfigures of those subframes.
+    def combine(self):
+        root = self.figures[0].copy()
+        for chunk in self.figures[1:]:
+            root.merge(chunk.copy())
+        return root
 
     # Allows you to give a name to a figure in the Frame that can
     # be referenced later using attribute access syntax.
     # This name mapping will persist even for a copy made of the
     # Frame figure.
     #
     # EXAMPLE:
@@ -553,14 +694,31 @@
 
         # Prevent the `origin` tweenable inherited from the Frame
         # class from being jumped in an actor action like fadeOut().
         # Jumping will instead be handled by individually jumping
         # each subfigure in the multifigure.
         self._state["origin"].tags.add("nojump")
 
+        # List of indices for subfigures that can be used for
+        # making subfigure copies as part of a tween.
+        self.NonTweenable("_subpool", set())
+
+    @property
+    def subpool(self):
+        return self._subpool
+
+    @subpool.setter
+    def subpool(self, value):
+        if isinstance(value, slice):
+            value = range(self.numfigs)[value]
+        self._subpool = value if type(value) is set else set(value)
+
+    def _appearsEqual(self, other, *args, compareSubNonTweenables=True, **kwargs):
+        return morpho.Frame._appearsEqual(self, other, *args, compareSubNonTweenables=compareSubNonTweenables, **kwargs)
+
     # # NOT IMPLEMENTED!!!
     # # Returns a StateStruct encapsulating all the tweenables
     # # of all the figures in the MultiFigure.
     # # Main example use case:
     # # my_multifig.all().alpha = 0 changes all the subfigures'
     # # alpha attribute to 0.
     # # By default, the tweenables encapsulated are all the
@@ -610,15 +768,16 @@
             return morpho.Frame.__getattr__(self, name)
 
         # Try to find the attribute in the first member figure
         # and if found, return it.
         fig = self.figures[0]
         try:
             # return fig.__getattribute__(name)
-            return getattr(fig, name)
+            # return getattr(fig, name)
+            return getattr(self.all, name)
         # This attribute is nowhere to be found anywhere. So give up.
         except AttributeError:
             # raise AttributeError("First member figure of type '"+type(fig)+"'' does not have attribute '"+name+"'")
             raise AttributeError("Could not find attribute '"+name+"' in either the main class or the first member figure!")
 
     # Modified setattr() first checks if the requested attribute already
     # exists as a findable attribute in the main class. If it is, it just
@@ -658,23 +817,44 @@
                 # See if it already exists as an attribute
                 # of the first member figure.
                 # fig.__getattribute__(name)
                 getattr(fig, name)
 
                 # If you got here, we didn't get an attribute error,
                 # so it should be a real attribute! Go ahead and set it!
-                fig.__setattr__(name, value)
+                self.all.__setattr__(name, value)
+                # fig.__setattr__(name, value)
 
             # Got an attribute error, so the given attribute isn't
             # even in the first member figure. Therefore, just assign it
             # as a regular (but new) attribute of the main class.
             except (AttributeError, IndexError):
                 # super().__setattr__(name, value)
                 morpho.Figure.__setattr__(self, name, value)
 
+    # Sets all given keyword inputs as toplevel attributes if they
+    # already exist as toplevel attributes. Any others are assigned
+    # as attributes of the subfigures.
+    def set(self, **kwargs):
+        # Dictionary holds all attribute mappings that don't
+        # correspond to toplevel attributes BUT DO correspond to
+        # subfigure attributes. These attributes will be assigned
+        # at the subfigure level
+        subset = dict()
+        if len(self.figures) > 0:
+            fig0 = self.figures[0]
+            for name in kwargs.copy():
+                if not object_hasattr(self, name) and name not in self._state \
+                and hasattr(fig0, name):
+                    subset[name] = kwargs.pop(name)
+        morpho.Figure.set(self, **kwargs)
+        self.all.set(**subset)
+        return self
+
+
     # Decorator for the tween methods in a MultiFigure subclass.
     # Reworks ordinary base class tween methods so that they work
     # in a multifigure setting.
     #
     # INPUTS
     # baseMethod = The method from the base class that should be
     #              modified. This method will be applied to the
@@ -687,44 +867,41 @@
     #              Defaults to Frame.tweenLinear.
     @staticmethod
     def Multi(baseMethod, mainMethod=Frame.tweenLinear):
 
         def wrapper(self, other, t, *args, **kwargs):
             # wrapper function for a MultiFigure tween method
 
-            # TODO: The following two blocks can probably be refactored
-            # into one since I think the only difference between them is
-            # that self and other reverse roles.
-
             # Temporarily extend the figure list of self or other
             # so that both have exactly the same number of subfigures.
-            diff = len(self.figures) - len(other.figures)
-            if diff > 0:
-                # Temporarily extend the figure list of other with copies of
-                # other's subfigures
-                orig_figures = other.figures
-                extension = []
-                for i in range(diff):
-                    extension.append(other.figures[i%len(other.figures)].copy())
-                other.figures = extension + other.figures
-                tw = wrapper(self, other, t, *args, **kwargs)
-                # Restore other to its original state
-                other.figures = orig_figures
-                return tw
-            elif diff < 0:
-                # Temporarily extend the figure list of self with copies of
-                # self's subfigures
-                orig_figures = self.figures
-                extension = []
-                for i in range(-diff):
-                    extension.append(self.figures[i%len(self.figures)].copy())
-                self.figures = extension + self.figures
+            len_self_figures = len(self.figures)
+            len_other_figures = len(other.figures)
+            diff = len_self_figures - len_other_figures
+
+            target, len_target_figures = (other, len_other_figures) if diff > 0 else (self, len_self_figures)
+            if diff != 0:
+                # Temporarily extend the figure list of target with copies of
+                # target's subfigures
+
+                # Generate the sorted pool of indices from which
+                # subfigure copies are allowed to be drawn.
+                subpool = {index % len_target_figures for index in target.subpool if index < len_target_figures}
+                if len(subpool) == 0:
+                    subpool = range(len_target_figures)
+                else:
+                    subpool = sorted(subpool)
+
+                # Make the copies and insert them uniformly
+                # amongst the original subfigures they came from.
+                orig_figures = target.figures
+                target.figures = target.figures[:]
+                makesubcopies(target.figures, subpool, abs(diff))
                 tw = wrapper(self, other, t, *args, **kwargs)
-                # Restore self to its original state
-                self.figures = orig_figures
+                # Restore target to its original state
+                target.figures = orig_figures
                 return tw
 
             # Tween each subfigure in self with its partner in other
             figures = []
             for fig, pig in zip(self.figures, other.figures):
                 twig = baseMethod(fig, pig, t, *args, **kwargs)
                 figures.append(twig)
@@ -909,24 +1086,29 @@
         if isinstance(figures, Frame):
             # super().__init__(figures.figures)
             super().__init__()
             self._updateFrom(figures, common=True)
         else:
             super().__init__(figures)
 
+    # Space version of Frame.partition().
+    def partition(self, *args, **kwargs):
+        return SpaceFrame(Frame.partition(self, *args, **kwargs))
+
     # Only for frames consisting only of space figures
     # (i.e. figures possessing a primitives() method and a 5 input
     # draw() method)
     #
     # Calls the primitives() method on all figures and merges all of
     # the lists into one big list of primitives and returns it.
     def primitives(self, camera): # orient=np.identity(3), focus=np.array([0,0,0], dtype=float)):
         primlist = []
         for fig in self.figures:
-            primlist.extend(fig.primitives(camera))
+            if fig.visible:
+                primlist.extend(fig.primitives(camera))
 
         return primlist
 
 # 3D version of the MultiFigure class. See "MultiFigure" for more info.
 class SpaceMultiFigure(SpaceFrame):
     def __getattr__(self, name):
         return MultiFigure.__getattr__(self, name)
@@ -1067,26 +1249,30 @@
 
 # Non-drawable figure whose purpose is to record information about the current
 # view of the complex plane that the Layer class should use to draw its actors.
 #
 # TWEENABLES
 # view = Viewbox of the complex plane ([xmin,xmax,ymin,ymax]).
 #        Default: [-5,5, -5,5]
-class Camera(morpho.Figure):
+class Camera(BoundingBoxFigure):
     def __init__(self, view=None):
         if view is None:
             view = [-5,5, -5,5]
 
         super().__init__()
 
         self.Tweenable("view", view, tags=["view", "scalar", "list"])
         self.Tweenable("rotation", 0, tags=["scalar"])
 
         self.defaultTween = type(self).tweenZoom
 
+    # Returns the current viewbox.
+    def box(self):
+        return self.view[:]
+
     # Zoom out the camera IN PLACE by the specified factor.
     # Optionally specify a complex number as the "focus", meaning
     # that point will remain at the same pixel after the zoom.
     # Defaults to the center of the viewbox.
     # Returns the camera figure it just acted on (self).
     def zoomOut(self, scale, focus=None):
         if scale <= 0:
@@ -1186,24 +1372,19 @@
         delta = (c*d1 + d**2 - (c+c1)*d) / height1
 
         self.view = [alpha, beta, gamma, delta]
 
 
     # Returns width of the viewbox: view[1] - view[0]
     def width(self):
-        return self.view[1] - self.view[0]
+        return self.boxWidth()
 
     # Returns height of the viewbox: view[3] - view[2]
     def height(self):
-        return self.view[3] - self.view[2]
-
-    # Returns the center of the view box as a complex number.
-    def center(self):
-        a,b,c,d = self.view
-        return ((a+b) + 1j*(c+d)) / 2
+        return self.boxHeight()
 
     # Given a complex number "pos" representing a position, this method returns
     # a new complex number corresponding to this position had the camera's
     # view been the unit square [0,1] x [0,1].
     # In other words, returns the RELATIVE coordinates of a position with
     # respect to the this camera's viewbox.
     #
@@ -1779,14 +1960,18 @@
             # since an actor has an unspecified time offset.
             other.timeOffset = self.timeOffset
             self.merge(other, atFrame, beforeActor)
         elif isinstance(other, Layer):
             # Compute time offset
             df = other.timeOffset - self.timeOffset + atFrame
 
+            # Set other owner's to self's owner just in case
+            # user wants to keep accessing `other` after the merge.
+            other.owner = self.owner
+
             # for actor in other.actors:
             # for n in range(len(other.actors)):
             for actor in reversed(other.actors):
                 # Adjust all the indices based on the time offsets
                 if df != 0:
                     timeline = {}
                     for keyID in actor.timeline:
@@ -1978,24 +2163,24 @@
     #
     # Note that this is a READ-ONLY function; you can't use it
     # to MODIFY the camera state. To do that, you have to use
     # layer.camera.time(f).view = [a,b,c,d]
     #
     # Set returnCamera = True to make the function return
     # the actual camera figure instead of just the view 4-vector.
-    def viewtime(self, f, useOffset=False, returnCamera=False):
+    def viewtime(self, f, useOffset=False, returnCamera=False, *, _skipTrivialTweens=False):
         if len(self.camera.timeline) == 0:
             raise IndexError("Camera timeline is empty.")
 
         # Adjust for time offset
         if useOffset:
             f -= self.timeOffset
 
         # Compute current view
-        viewFrame = self.camera.time(f)
+        viewFrame = self.camera.time(f, _skipTrivialTweens=_skipTrivialTweens)
         if viewFrame is None:
             # if len(self.camera.timeline) == 0:
             #     viewFrame = Frame()
             if f > self.camera.keyIDs[-1]:
                 viewFrame = self.camera.key(-1)
             else:
                 viewFrame = self.camera.key(0)
@@ -2156,14 +2341,25 @@
             self.end = round((self.end - center)/factor + center)
 
 
     # Equivalent to speedUp(1/factor). See speedUp() for more info.
     def slowDown(self, factor, center=0, useOffset=False, ignoreMask=False):
         self.speedUp(1/factor, center, useOffset, ignoreMask)
 
+    # Optimizes the Layer's actors for animation playback.
+    # See morpho.Actor._optimize() for more info.
+    def _optimize(self):
+        self.camera._optimize()
+        for actor in self.actors:
+            actor._optimize()
+
+    def _deoptimize(self):
+        self.camera._deoptimize()
+        for actor in self.actors:
+            actor._deoptimize()
 
     # Pretweens all the actors in the layer including the camera actor.
     # See Actor.pretween() for more info.
     # By default, masks are recursively pretweened as well, unless
     # ignoreMask = False
     def pretween(self, ignoreMask=False):
         # First pretween the camera.
@@ -2238,36 +2434,36 @@
     # useOffset=True means we're using global (i.e. Animation class) time.
     def draw(self, f, ctx, useOffset=False):
         if useOffset:
             # Convert f to equivalent local time coordinates.
             f -= self.timeOffset
 
         # Compute current view
-        cam = self.viewtime(f, returnCamera=True)  # Get camera figure
+        cam = self.viewtime(f, returnCamera=True, _skipTrivialTweens=True)  # Get camera figure
         if not cam.visible:
             return
 
         # Compile list of figures to draw
         figlist = []
         for actor in self.actors:
             if actor.visible:
-                fig = actor.time(f)
+                fig = actor.time(f, _skipTrivialTweens=True)
                 # if fig is None or not fig.visible:
                 #     continue
                 # else:
                 #     figlist.append(fig)
                 if fig is not None and fig.visible:
                     figlist.append(fig)
 
         # Sort based on zdepth
         figlist.sort(key=lambda fig: fig.zdepth) #, reverse=True)
 
         # NOTE: The "start" and "end" parameters of the masklayer are ignored
         # when drawing with masking!
-        if self.mask is None or not self.mask.visible or not self.mask.viewtime(f, returnCamera=True).visible:
+        if self.mask is None or not self.mask.visible or not self.mask.viewtime(f, returnCamera=True, _skipTrivialTweens=True).visible:
             # Draw all figures
             with cam._pushRotation(ctx):  # Apply camera rotation
                 for fig in figlist:
                     fig.draw(cam, ctx)
         else:  # Layer has a mask, so draw with masking
             # # Extract surface's width and height
             # surface = ctx.get_target()
@@ -2388,15 +2584,15 @@
     # Draw the spacelayer at the specified index on the given cairo context
     # if the camera is visible at that index.
     def draw(self, f, ctx, useOffset=False):
         if useOffset:
             f -= self.timeOffset
 
         # Compute current view
-        cam = self.viewtime(f, returnCamera=True)  # Get camera figure
+        cam = self.viewtime(f, returnCamera=True, _skipTrivialTweens=True)  # Get camera figure
         if not cam.visible:
             return
 
         # view = self.viewtime(f)
         # viewFrame = self.view.time(f)
         # if viewFrame is None:
         #     if len(self.view.timeline) == 0:
@@ -2407,15 +2603,15 @@
         #         viewFrame = self.view.key(0)
         # view = viewFrame.view
 
         # Compile list of figures to draw
         figlist = []
         for actor in self.actors:
             if actor.visible:
-                fig = actor.time(f)
+                fig = actor.time(f, _skipTrivialTweens=True)
                 if fig is None or not fig.visible:
                     continue
                 figlist.append(fig)
 
         # Sort based on zdepth
         figlist.sort(key=lambda fig: fig.zdepth) #, reverse=True)
 
@@ -2425,15 +2621,15 @@
                 # if "primitives" in dir(fig):
                 if object_hasattr(fig, "primitives"):
                     primlist.extend(fig.primitives(cam))
                     figlist.remove(fig)
 
         # NOTE: The "start" and "end" parameters of the masklayer are ignored
         # when drawing with masking!
-        if self.mask is None or not self.mask.visible or not self.mask.viewtime(f, returnCamera=True).visible:
+        if self.mask is None or not self.mask.visible or not self.mask.viewtime(f, returnCamera=True, _skipTrivialTweens=True).visible:
             with cam._pushRotation(ctx):  # Apply camera rotation
                 # Draw all non-primitive figures
                 for fig in figlist:
                     fig.draw(cam, ctx)
                 # Draw all primitive 2D figures
                 if self.poolPrimitives:
                     frame = Frame(primlist)
@@ -2497,14 +2693,19 @@
 # fullscreen = Boolean indicating whether animation should be played fullscreen.
 #              Default: False
 # screen = int denoting which monitor to display on (0 is primary monitor).
 #          Default: 0
 # locaterLayer = Given layer or layer list index, prints the physical coordinates
 #                of a mouse click relative to that layer whenever the animation
 #                playback is clicked. Default: None
+# locaterModifier = Complex to complex function which modifies
+#       complex number positions generated from the locater layer.
+#       The generated locator layer positions are passed into this
+#       function and the return value is printed to the console instead.
+#       Default: Identity (do nothing) function z |--> z
 # clickTime = Boolean if set to True, prints current frame index to console
 #             whenever animation is clicked to pause.
 #             Options: "frames", "seconds"
 #             Note: This ignores animation delays.
 # clickCopy = Boolean if set to True and locaterLayer is set, then every click
 #             will copy the complex coordinates of the click to the
 #             clipboard.
@@ -2574,14 +2775,19 @@
 
         # Given a layer, or an int representing the index of a layer
         # in the layer list, when the animation is clicked during playback,
         # it will print the physical coordinates of the click location
         # relative to the specified layer.
         self.locaterLayer = None
 
+        # Function that will be applied to the complex number
+        # position computed from the locater layer. By default
+        # it's the identity function z |--> z
+        self.locaterModifier = lambda z: z
+
         # Makes the animation print the current frame/time when
         # clicked to pause.
         # Options: "frames", "seconds"
         # Note: This ignores animation delays.
         self.clickTime = "none"
 
         # If set to True and locaterLayer is set, then every click
@@ -2641,14 +2847,23 @@
     def locatorLayer(self):
         return self.locaterLayer
 
     @locatorLayer.setter
     def locatorLayer(self, value):
         self.locaterLayer = value
 
+    # Alternate name for the locater modifier using "o" instead of "e".
+    @property
+    def locatorModifier(self):
+        return self.locaterModifier
+
+    @locatorModifier.setter
+    def locatorModifier(self, value):
+        self.locaterModifier = value
+
     @property
     def start(self):
         return self.firstIndex
 
     @start.setter
     def start(self, value):
         self.firstIndex = value
@@ -2693,14 +2908,15 @@
         ani.background = self.background
         ani.alpha = self.alpha
         ani.windowShape = self.windowShape[:]
         ani.resizable = self.resizable
         ani.fullscreen = self.fullscreen
         ani.screen = self.screen
         ani.locaterLayer = self.locaterLayer
+        ani.locaterModifier = self.locaterModifier
         ani.clickTime = self.clickTime
         ani.transition = self.transition
         ani.currentIndex = self.currentIndex
         ani.antialiasText = self.antialiasText
         ani.jointStyle = self.jointStyle
         ani.clickCopy = self.clickCopy
         ani.clickRound = self.clickRound
@@ -3398,37 +3614,55 @@
             f = self.currentIndex - layer.timeOffset
             if not layer.visible or not(layer.start <= f <= layer.end):
                 continue
 
             # Draw layer to current context
             layer.draw(f, self.context)
 
+    # Optimizes the animation for playback by optimizing
+    # all its actors.
+    # See morpho.Actor._optimize() for more info.
+    def _optimize(self):
+        for layer in self.layers:
+            layer._optimize()
+
+    def _deoptimize(self):
+        for layer in self.layers:
+            layer._deoptimize()
+
     # Export animation to file.
     # Can either be MP4, GIF animation, or PNG sequence depending on
     # the file extension given in the filepath.
     # Optional argument scale is a scale factor that scales the entire
     # animation window shape before exporting. Useful for downscaling an
     # animation while exporting test animations to speed up rendering.
     # Note: scaling seems to be done at the final pixel level, so specifying
     # scale > 1 will not actually increase the resolution of your animation.
-    def export(self, filepath, scale=1):
+    #
+    # Optional argument "optimize" can be set to False to prevent
+    # the animation from being optimized. This will probably rarely be
+    # desired.
+    def export(self, filepath, scale=1, *, optimize=True):
         # # Handle non-trivial scale factor.
         # if scale != 1:
         #     # Save original window shape
         #     windowShape = self.windowShape[:]
         #     # Scale window shape and export
         #     self.windowShape = tuple(map(lambda x: round(scale*x), windowShape))
         #     self.export(filepath)
         #     # Restore original window shape.
         #     self.windowShape = windowShape
         #     return
 
         if scale > 1:
             warn("scale > 1 will not actually improve resolution.")
 
+        if optimize:
+            self._optimize()
+
         # Get first and final indices if specified.
         if self.finalIndex is None:
             finalIndex = self.lastID()
         else:
             finalIndex = self.finalIndex
 
         if self.firstIndex is None:
@@ -3610,23 +3844,30 @@
 
     # Plays the animation in a separate window or possibly fullscreen.
     #
     # Optional arguments "window" and "autoclose" are mostly just holdovers
     # from a much older version of Morpho, and should probably just be left
     # alone. In the future, one or both of them may be removed.
     #
+    # Optional argument "optimize" can be set to False to prevent
+    # the animation from being optimized. This will probably rarely be
+    # desired.
+    #
     # KNOWN ISSUE: Morpho may sometimes crash if you attempt to call play()
     # multiple times in a single run of your code. To avoid, make sure you
     # only play one animation per execution of your code.
-    def play(self, window=None, autoclose=False):
+    def play(self, window=None, autoclose=False, *, optimize=True):
         # Verify the animation can be played.
         # if not self.verify():
         #     raise Exception("Animation can't be played because it is not configured properly!")
         self.sanityCheck()
 
+        if optimize:
+            self._optimize()
+
         if self.finalIndex is None:
             finalIndex = self.lastID()
         else:
             finalIndex = self.finalIndex
 
         if self.firstIndex is None:
             firstIndex = self.firstID()
@@ -3760,14 +4001,17 @@
                     # Treat it as an actual layer object
                     cam = mation.locaterLayer.viewtime(mation.currentIndex, returnCamera=True)
                 view = cam.view
 
                 z = physicalCoords(X, Y, view, mation.context)
                 z *= cmath.exp(-1j*cam.rotation)  # Adjust by camera rotation
 
+                # Apply modifier
+                z = mation.locaterModifier(z)
+
                 # Round the real and imag components of z if needed.
                 if self.clickRound is not None:
                     x,y = z.real, z.imag
                     x = round(x, self.clickRound)
                     y = round(y, self.clickRound)
                     z = x + y*1j
 
@@ -3813,15 +4057,21 @@
 
             tic()  # Reset runtime timer
 
 
         # Schedule drawing at the specified frame rate.
         # Only schedule the updater for animations that are more
         # than a single frame.
-        if finalIndex - firstIndex > 0:
+        # UPDATE: pyglet will occasionally crash when trying to
+        # play a 1-frame animation. Disabling the `else` clause
+        # here seems to fix it. In the future, this if-else
+        # clause may be fully removed, but I'm keeping this funny
+        # `if True` to preserve the previous behavior in case
+        # I want to revert.
+        if True or finalIndex - firstIndex > 0:
             # If the first frame is a delay frame, manually call
             # the doDelay() method because the updater won't see it.
             if self.currentIndex in self.delays:
                 self.doDelay()
             else:
                 # Draw frames at specified framerate
                 pg.clock.schedule_interval(self.update, 1.0/self.frameRate)
@@ -3873,14 +4123,15 @@
         self.active = False
         self.window = None
         self.context = None
         self.update = None
         self.paused = False
         self.currentIndex = 0
         self._keyIDs = None  # This var is only used once play() is called.
+        self._deoptimize()
 
     # This function verifies whether or not the animation is playable.
     # It's probably not perfect yet, so animations could still break
     # even if this function returns True, but it may help a little.
     def verify(self):
         try:
             self.sanityCheck()
```

### Comparing `morpholib-0.7.0.dev1/src/morpholib/base.py` & `morpholib-0.7.1.dev1/src/morpholib/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 To avoid name conflicts, please avoid using names in the
 outermost scope that could be names of subpackages.
 This can be done by avoiding names that are nothing but
 lowercase letters since convention has it that package
 names are all lowercase letters.
 '''
 
-from morpholib.tools.basics import tau, argShift, argShiftArray, arcCenter, arcCenterArray
+from morpholib.tools.basics import tau, argShift, argShiftArray, arcCenter, arcCenterArray, isequal
 import math
 import numpy as np
 import cairo
 cr = cairo
 # from warnings import filterwarnings
 
 # Ignore warnings by default.
 # This is mainly for the sake of the Spline class, which
 # uses some non-standard arithmetic intentionally.
 # filterwarnings("ignore")
 
 
-version = "0.7.0.dev1"  # Current public morpho version
-internalVersion = "2.4.0"  # Current internal morpho version
+version = "0.7.1.dev1"  # Current public morpho version
+internalVersion = "2.4.1ip"  # Current internal morpho version
 subversion = ""
 DEBUG_MODE = False
 
 
 ### CLASSES ###
 
 
@@ -126,31 +126,38 @@
     # this can't be done, the copied tweenable's value attribute
     # will just assign to the original's value.
     # i.e. twCopy.value = self.value
     # copy() will also make a copy of the tags set, but
     # it doesn't attempt to copy any of the other
     # attributes of the tweenable such as name, or metadata
     # as it assumes these are strings and hence immutable.
-    def copy(self):
+    def copy(self, deep=True):
         twCopy = Tweenable(
             name=self.name,
             tags=self.tags.copy(),
             value=self.value,
             metadata=self.metadata)
 
-        try:
-            twCopy.value = self.value.copy()
-        except Exception:  # Upon failure, just reassign and hope for the best.
-            # Actually, I think I DO want this line. It looks redundant,
-            # but if the try clause somehow messed up the assignment
-            # process itself, I'd like to reassign the initial value.
-            twCopy.value = self.value
+        if deep:
+            try:
+                twCopy.value = self.value.copy()
+            except Exception:  # Upon failure, just reassign and hope for the best.
+                # Actually, I think I DO want this line. It looks redundant,
+                # but if the try clause somehow messed up the assignment
+                # process itself, I'd like to reassign the initial value.
+                twCopy.value = self.value
 
         return twCopy
 
+    def __eq__(self, other):
+        return self.name == other.name and \
+            self.tags == other.tags and \
+            isequal(self.value, other.value) and \
+            self.metadata == other.metadata
+
     def __repr__(self):
         return "<"+self.name+": " + repr(self.value) + ">"
 
     def __str__(self):
         return repr(self)
 
 
@@ -226,15 +233,15 @@
     r = numTween(r1, r2, t)
     th = th1 + t*dth
 
     tw = r*cmath.exp(th*1j)
 
     return tw
 
-def spiralInterpArray(p,q,t, start=0, end=1):
+def spiralInterpArray(p,q,t):
 
     r1 = np.abs(p)
     r2 = np.abs(q)
 
     th1 = np.angle(p) % tau
     th2 = np.angle(q) % tau
     dth = argShiftArray(th1, th2)
@@ -244,14 +251,75 @@
     r = numTween1(r1, r2, t)
     th = th1 + t*dth
 
     tw = r*np.exp(th*1j)
 
     return tw
 
+# Performs spiral tween interpolation on two arrays of 3D nodes
+def spiralInterpArray3d(pseq, qseq, t, *, verbose=False):
+    if pseq.ndim < 2:
+        pseq = pseq.reshape(1,-1)
+    if qseq.ndim < 2:
+        qseq = qseq.reshape(1,-1)
+
+    r1 = np.linalg.norm(pseq, axis=1)  # N-vector
+    r2 = np.linalg.norm(qseq, axis=1)  # N-vector
+
+    # Suppress numpy warnings from nans that may develop
+    with np.errstate(all="ignore"):
+        dr = r2 - r1  # N-vector
+        crossProds = np.cross(pseq, qseq)  # N x 3 array
+        crossProdNorms = np.linalg.norm(crossProds, axis=1)  # N-vector
+
+        # Flag any node pairs that don't define a
+        # meaningful plane of rotation
+        bad = (np.abs(crossProdNorms) < 1e-10)
+        good = ~bad
+
+        angles = np.arccos(np.sum(pseq*qseq, axis=1)/(r1*r2))  # N-vector of angles between each node pair
+        angles[np.isnan(angles)] = math.pi
+
+        radii = r1 + t*dr  # New radii of tweened nodes (N-vector)
+        thetas = t*angles  # Angles to tilt p-nodes toward q-nodes (N-vector)
+        tilts = qseq[:,:,None]*pseq[:,None,:] - pseq[:,:,None]*qseq[:,None,:]  # N x 3 x 3 array of tilt products
+
+        normalizedTilts = tilts / crossProdNorms[:,None,None]  # N x 3 x 3 array
+        normalizedTilts_squared = np.matmul(normalizedTilts, normalizedTilts)  # N x 3 x 3
+        sin_thetas = np.sin(thetas)  # N-vector
+        one_minus_cos_thetas = 1-np.cos(thetas)  # N-vector
+
+        # N x 3 x 3 array of rotation matrices
+        rotators = np.eye(3)[None,:,:] + normalizedTilts*sin_thetas[:,None,None] \
+            + normalizedTilts_squared*one_minus_cos_thetas[:,None,None]
+
+        # Apply rotators to pseq
+        pseq_rotated = np.matmul(rotators, pseq[:,:,None])  # N x 3 x 1 array of new nodes
+        pseq_rotated = pseq_rotated.squeeze()  # N x 3 array
+        if pseq_rotated.ndim < 2:
+            pseq_rotated = pseq_rotated.reshape(1,-1)  # Force 1 x 3 array if just a single vector
+
+    # Apply radii
+    twseq = np.zeros(pseq.shape)
+    twseq[good] = radii[good][:,None] * pseq_rotated[good] / r1[good][:,None]  # N x 3 array
+
+    twseq[bad] = lerp0(pseq[bad], qseq[bad], t)
+
+    if verbose:
+        # Return many of the intermediate values calculated along with
+        # the final answer `twseq`
+        return dict(twseq=twseq, r1=r1, r2=r2, crossProds=crossProds,
+            crossProdNorms=crossProdNorms, bad=bad, good=good, angles=angles,
+            radii=radii, thetas=thetas, normalizedTilts=normalizedTilts,
+            normalizedTilts_squared=normalizedTilts_squared,
+            rotators=rotators)
+    else:
+        return twseq
+
+
 def pivotInterpArray(p,q,t, angle=tau/2, start=0, end=1):
     if not(start == 0 and end == 1):
         t = (t-start)/(end-start)  # Normalize
 
     c = arcCenterArray(p,q, angle)
     tw = (p-c)*np.exp(t*angle*1j) + c
```

### Comparing `morpholib-0.7.0.dev1/src/morpholib/bezier.py` & `morpholib-0.7.1.dev1/src/morpholib/bezier.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.0.dev1/src/morpholib/calculus.py` & `morpholib-0.7.1.dev1/src/morpholib/calculus.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.0.dev1/src/morpholib/color.py` & `morpholib-0.7.1.dev1/src/morpholib/color.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,24 @@
 from morpholib import object_hasattr
 
 import math, cairo
 import numpy as np
 from numbers import Number
 import colorsys
 
+# Checks if two color triplets code for the same color.
+# Works by seeing if each component is within 1/255 of
+# its partner.
+# e.g. matches([1,0,0], (0.99999,0,0)) --> True
+def matches(color1, color2):
+    color1 = np.array(color1, dtype=float)
+    color2 = np.array(color2, dtype=float)
+
+    return np.all(np.round(255*(color2-color1))==0).tolist()
+
 # Normalizes an RGB triplet in the range [0...255] into
 # the range [0.0, 1.0].
 # RGB can be specified as three separate inputs, or as a
 # tuple supplied as one input.
 # Optional upperbound argument can be supplied to change
 # what the max possible value for the input RGB values is.
 # Default: 255.
@@ -250,14 +260,17 @@
             return self.segment(a,b, normalize=True)
         else:
             return self.value(key)
 
     def __setitem__(self, key, value):
         self.data[key] = value
 
+    def __iter__(self):
+        return iter(self.data)
+
     def __len__(self):
         return len(self.data)
 
     # Returns the interpolated gradient value at the specified x in [0,1]
     # x can optionally be a 1D numpy array in which case the gradient is
     # evaluated on each x element-wise and the result is returned as a
     # matrix where each row corresponds to an x value.
```

### Comparing `morpholib-0.7.0.dev1/src/morpholib/combo.py` & `morpholib-0.7.1.dev1/src/morpholib/combo.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.0.dev1/src/morpholib/figure.py` & `morpholib-0.7.1.dev1/src/morpholib/figure.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,19 @@
         # Note that the static attribute can always be overridden
         # by manually calling the figure's tween() or fimage() methods.
         # It just means they won't be automatically called when
         # embedded as parts of frames, animations, or other higher
         # structures that incorporate figures.
         self.static = False
 
+        # Special hidden attribute only meant to be used during
+        # animation playback. Helps to make animations run more
+        # quickly when tweening between equal keyfigures.
+        self._static_acute = False
+
         # (DEPRECATED)
         # How many frames should the figure persist in an animation.
         # If set to oo (infinity), then the figure will
         # never disappear until the next keyfigure (if any).
         # If the delay period ends before the next keyfigure appears,
         # tweening will be done as if the figure were placed
         # at the frame where the delay ended.
@@ -120,14 +125,28 @@
     def tweenMethod(self):
         return self.defaultTween
 
     @tweenMethod.setter
     def tweenMethod(self, value):
         self.defaultTween = value
 
+    # Returns True iff self and other are both invisible, OR are
+    # exactly the same type AND their tweenables compare equal.
+    # Used to determine whether tweening will be required between
+    # two keyfigures in an Actor.
+    #
+    # Optionally, keyword `compareNonTweenables` can be set to True
+    # to make the check stricter by also checking that corresponding
+    # non-tweenables match between both figures.
+    def _appearsEqual(self, other, ignore=(), *, compareNonTweenables=False):
+        return not(self.visible or other.visible) or \
+            (type(self) is type(other) and \
+            all(self._state[name] == other._state[name] for name in self._state if name not in ignore)) and \
+            (not compareNonTweenables or all(isequal(getattr(self, name), getattr(other, name)) for name in self._nontweenables if name not in ignore))
+
     # Actor actions registry.
     # Maps action names to the action functions themselves.
     actions = {}
 
     # Action decorator adds an action function to
     # the figure's registry.
     @classmethod
@@ -317,15 +336,15 @@
 
         if copy:
             target = target.copy()
 
         # Update tweenables
         for name in target._state:
             if ((not common) or (name in self._state)) and name not in ignore:
-                self._state[name] = target._state[name]
+                self._state[name] = target._state[name] if copy else target._state[name].copy(deep=False)
         # Update non-tweenables
         for name in target._nontweenables:
             if ((not common) or (name in self._nontweenables)) and name not in ignore:
                 self._nontweenables.add(name)
                 setattr(self, name, getattr(target, name))
 
         # Update meta-settings
@@ -758,15 +777,15 @@
         # Convert string to tuple containing string
         elif isinstance(ig, str):
             ig = [ig]
         elif not isinstance(ig, list):
             ig = list(ig)
 
         # These tags are affected by the Spiral tween
-        tags = {"spiral", "complex"}
+        tags = {"spiral", "complex", "3d"}
 
         # Create new figure which will be the tweened figure
         # Initialize it to a copy of self.
         newfig = self.copy()
 
         # Perform spiral tween on all relevant tweenables
         for tweenable in self._state.values():
@@ -778,60 +797,32 @@
 
             # Since tweenSpiral() is acting, prevent tweenLinear() from acting
             # on this tweenable later on.
             ig.append(tweenable.name)
 
             P = tweenable.value
             Q = other._state[tweenable.name].value
-            if isinstance(P, list) or isinstance(P, tuple) \
-                or isinstance(P, np.ndarray):
-                listMode = True
+
+            # Convert into np.arrays with at least 1 dimension
+            P = np.array(P)
+            Q = np.array(Q)
+            if P.size == 1:
+                P.shape = 1
+            if Q.size == 1:
+                Q.shape = 1
+
+            # Perform spiral tween
+            if "3d" in tweenable.tags:
+                tw = morpho.spiralInterpArray3d(P, Q, t).squeeze()
             else:
-                listMode = False
-                P = [P]
-                Q = [Q]
-
-            # Perform spiral tween on each component
-            # FUTURE: Re-implement this like the modern tweenLinear()
-            # so that it converts the data into np.array form and
-            # then applies morpho.spiralInterpArray() to it and then
-            # converts back into the original type.
-            for i in range(len(P)):
-                p = P[i]
-                q = Q[i]
-                if type(p) in (list, tuple):
-                    p = p[0] + 1j*p[1]
-                if type(q) in (list, tuple):
-                    q = q[0] + 1j*q[1]
-                p = complex(p)
-                q = complex(q)
-
-                r1 = abs(p)
-                r2 = abs(q)
-
-                th1 = cmath.phase(p) % tau
-                th2 = cmath.phase(q) % tau
-                dth = argShift(th1, th2)
-
-                dr = r2 - r1
-
-                r = morpho.numTween(r1, r2, t)
-                th = th1 + t*dth
-
-                tw = r*cmath.exp(th*1j)
-
-                # FUTURE: Complex should be converted back into whatever
-                # vectory type it was in originally.
-                if listMode:
-                    # NOTE: This line assumes the vector is mutable.
-                    # Thus this will fail if given tuple (I think)!
-                    # Fix in the future!!
-                    newfig._state[tweenable.name].value[i] = tw
-                else:
-                    newfig._state[tweenable.name].value = tw
+                tw = morpho.spiralInterpArray(P, Q, t).squeeze()
+
+            if isinstance(tweenable.value, (list, tuple)):
+                tw = type(tweenable.value)(tw)
+            newfig._state[tweenable.name].value = tw
 
         # Use tweenLinear() on the remaining tweenables that this tween method
         # did not act on (e.g. scalars)
         # print(ig)
         # newfig = newfig.tweenLinear(other, t, ignore=ig)
         newfig = Figure.tweenLinear(newfig, other, t, ignore=ig)
 
@@ -1106,14 +1097,16 @@
 # animation to create a new figure morphing out of a copy of
 # another figure.
 #
 # `source` can also be an actor, in which case, its latest
 # keyfigure is taken as the source figure.
 @Figure.action
 def morphFrom(actor, source, duration=30, atFrame=None):
+    if duration < 2:
+        raise ValueError("Duration must be at least 2 frames.")
     if atFrame is None:
         atFrame = actor.lastID()
     if isinstance(source, Actor):
         source = source.last()
 
     # Save a copy of the latest keyfigure to use as the
     # target ending figure.
@@ -1127,17 +1120,23 @@
     fig1 = actor.newkey(atFrame, source.copy())
     fig1._updateSettings(fig0, includeTweenMethod=True)
     fig1.set(visible=True)
 
     # Set destination figure to be the original last keyfigure.
     actor.newendkey(duration, target)
 
-    # Keep only the first frame AFTER atFrame
-    actor.newkey(atFrame+1)
-    actor.delkey(atFrame)
+    # Keep only the first frame AFTER atFrame.
+    # We take a copy of the intial keyframe because we're not
+    # going to rely on creating perfectly seamless intermediate
+    # keyfigures (e.g. MultiText doesn't split tweens seamlessly).
+    actor.newkey(atFrame+1, actor.time(atFrame).copy())
+    # Doing invisibility instead of delkey because preserving
+    # the initial keyframe can be important for puppet skits.
+    actor.time(atFrame).visible = False
+    # actor.delkey(atFrame)
 
 
 # Base class for certain space figures.
 class SpaceFigure(Figure):
     # Default draw method of a SpaceFigure is to assume the
     # primitives() method exists, call it, get all the primitives,
     # and if it's not an empty list, package into a frame and draw.
@@ -1149,14 +1148,15 @@
         # Package into frame and draw!
         frame = morpho.Frame(primlist)
         frame.draw(camera, ctx)
 
         # prim = primlist[0]
         # prim.draw(camera, ctx)
 
+
 ### OTHER RELATED FUNCTIONS ###
 
 # Decorator generator returns a decorator that can be used on
 # a custom angle-specific pivot tween method. Mainly for use
 # in enabling custom tweenPivot() methods to be splittable.
 #
 # Example usage:
@@ -1866,15 +1866,22 @@
     # the key figure.
     # Optionally specify the latest key index. This is mainly used
     # internally for performance reasons. You probably don't need
     # to worry about it.
     # If optional keyword argument copykeys is set to True,
     # if a keyfigure is returned, a copy will be returned instead.
     # Also mainly for internal use.
-    def time(self, f, keyID=None, *, copykeys=False):
+    #
+    # `_skipTrivialTweens` is a hidden keyword-only argument mainly
+    # for internal use which tells time() to use the
+    # _static_acute attribute
+    # of a figure to decide whether tweening is necessary.
+    # By default, it's False so tweening behaves exactly as
+    # expected.
+    def time(self, f, keyID=None, *, copykeys=False, _skipTrivialTweens=False):
         # If f is a float, but it's really an int, make it an int.
         # This is so searching the timeline dict is done correctly
         # because all the keys in the dict are ints.
         # NOTE: Just learned that keys that are compared as equal are
         # treated as the same key in a dict! So maybe this line is
         # not necessary after all!
         if type(f) is float and f == int(f):
@@ -1904,15 +1911,15 @@
         # in the timeline. Return None unless actors persist.
         elif keyID == self.keyIDs[-1]:
             if Actor.persist:
                 return keyfig if not copykeys else keyfig.copy()
             else:
                 return None
         # If the latest keyframe is static, don't tween.
-        elif keyfig.static:
+        elif (_skipTrivialTweens and keyfig._static_acute) or keyfig.static:
             return keyfig if not copykeys else keyfig.copy()
             # return keyfig.copy()
         else:
             # keyfig2 = self.timeline[keyID+1]
             keyfig2 = self.key(k+1)
             T = morpho.numTween(0, 1, f,
                 start=keyID + keyfig.delay,
@@ -1940,14 +1947,29 @@
             raise TypeError("No global timeline to reference.")
 
         f = currentIndex - self.owner.timeOffset
         fig = self.time(f, copykeys=True)  # Make a copy in case it's a keyfigure
 
         return fig
 
+    # Optimizes the Actor for playback by setting keyfigures to be
+    # acutely static if it looks like there's no reason to tween
+    # them e.g. the starting and ending keyfigures appear equal, or
+    # the current keyfigure is invisible (whereby the tweened figure
+    # will inherit the invisibility).
+    def _optimize(self):
+        for n in range(len(self.timeline)-1):
+            keyfig = self.key[n]
+            keyfigNext = self.key[n+1]
+            if not keyfig.visible or keyfig._appearsEqual(keyfigNext):
+                keyfig._static_acute = True
+
+    def _deoptimize(self):
+        for keyfig in self.keys():
+            keyfig._static_acute = False
 
     # Should the final keyfigure persist after the final frame?
     # If set to True, to make an actor vanish, you will need to
     # make a new final keyframe with visibility attribute set to
     # False.
     persist = True
```

### Comparing `morpholib-0.7.0.dev1/src/morpholib/gadgets.py` & `morpholib-0.7.1.dev1/src/morpholib/gadgets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 import morpholib as morpho
 import morpholib.anim
 import morpholib.grid
 from morpholib.tools.basics import *
 
 import math, cmath
 
+# Decorator for gadget functions that operate on a box.
+# Allows such a gadget function to accept a Figure type input
+# whereby it will attempt to infer a box by calling the
+# figure's `box()` method, assuming it exists.
+# If given an Actor object, it will use the latest keyfigure.
+def handleBoxTypecasting(gadgetfunc):
+    def wrapper(box, *args, **kwargs):
+        if isinstance(box, morpho.Actor):
+            box = box.last()
+        if isinstance(box, morpho.Figure):
+            if not hasattr(box, "box"):
+                raise TypeError(f"`{type(box).__name__}` type figure does not support box() method.")
+            box = box.box()
+        return gadgetfunc(box, *args, **kwargs)
+    return wrapper
+
 # DEPRECATED! Use crossout() or crossoutPath() instead.
 # Returns a layer which when animated makes a colored X cross
 # out the box you specify.
 # box = a 4-item list/tuple in the same fashion as the view box
 # time = duration for the animation
 # width = thickness of the lines
 # color = color of the lines
@@ -46,14 +62,15 @@
 # color = color of the lines
 # transition = Transition function assigned to path.
 #              Default: morpho.transition.default
 # origin = origin point of path (complex number). Default: 0
 # relative = Boolean indicating whether the box values are relative to the origin
 #            point, or are in absolute physical coordinates of the layer.
 #            Default: False (absolute coordinates)
+@handleBoxTypecasting
 def crossoutPath(box, time=30, width=3, color=(1,0,0),
     transition=None, origin=0, relative=False,
     *, duration=None, pad=0, **kwargs):
 
     # "duration" is a dominant alias for the "time" parameter
     if duration is not None:
         time = duration
@@ -92,14 +109,15 @@
 # steps = Number of line segments in path. Default: 75
 # transition = Transition function assigned to path.
 #              Default: morpho.transition.default
 # origin = origin point of path (complex number). Default: 0
 # relative = Boolean indicating whether the box values are relative to the origin
 #            point, or are in absolute physical coordinates of the layer.
 #            Default: False (absolute coordinates)
+@handleBoxTypecasting
 def encircle(box, time=30, width=3, color=(1,0,0), phase=tau/4,
     CCW=True, steps=75, transition=None, origin=0, relative=False,
     *, duration=None, pad=0, **kwargs):
 
     # "duration" is a dominant alias for the "time" parameter
     if duration is not None:
         time = duration
@@ -142,16 +160,19 @@
 #          Values are given as diagonal compass directions:
 #          "NW", "SW", "SE", "NE". Default: "NW"
 # CCW = Boolean specifying draw direction being counter-clockwise or not.
 #       Default: True
 # transition = Transition function assigned to path.
 #              Default: morpho.transition.default
 # origin = origin point of path (complex number). Default: 0
+@handleBoxTypecasting
 def enboxPath(box, time=30, width=3, color=(1,0,0), corner="NW", CCW=True,
-    transition=None, origin=0, *, duration=None, pad=0, **kwargs):
+    transition=None, origin=0, *, duration=None, pad=0,
+    _debox=False, _pause=0,
+    **kwargs):
 
     # "duration" is a dominant alias for the "time" parameter
     if duration is not None:
         time = duration
 
     corner = corner.upper()
     dirs = ["NW", "SW", "SE", "NE"]
@@ -183,29 +204,53 @@
     path.close()
     path.width = width
     path.color = list(color)
     constTrans = path.constantSpeedTransition()
     path.origin = origin
     if transition is None:
         transition = morpho.transition.default
-    # if transition is None:
-    #     path.transition = lambda t: constTrans(morpho.transition.default(t))
-    path.transition = lambda t: constTrans(transition(t))
+
+    if _debox:
+        # Calculate in and out times
+        t1 = round(time/2)
+        t2 = time - t1
+        time = t1
+
+        # Split the transition between the in and out times
+        tran1, tran2 = morpho.transitions.split(transition, 0.5)
+        path.transition = lambda t: constTrans(tran1(t))
+    else:
+        path.transition = lambda t: constTrans(transition(t))
     path.end = 0
     path.set(**kwargs)  # Set any other attributes
 
     path = morpho.Actor(path)
     path.newkey(time)
     path.last().end = 1
+
+    if _debox:
+        if _pause > 0:
+            path.newendkey(_pause)
+        path.last().transition = lambda t: constTrans(tran2(t))
+        path.newendkey(t2).start = 1
+        path.last().visible = False
+
     path.last().transition = transition
 
     return path
 
 enbox = enboxPath  # Synonym for emboxPath()
 
+# Same as enbox(), but it deboxes immediately afterward.
+# Useful for briefly highlighting something with a box.
+# An additional keyword-only input `pause` can be specified
+# to provide a delay between enboxing and deboxing.
+def enboxHighlight(*args, pause=0, **kwargs):
+    return enbox(*args, _debox=True, _pause=pause, **kwargs)
+
 # Scales all the nodes of a path by the given factor about the given
 # centerpoint. If the center is unspecified, defaults to the center
 # of mass of all the path's nodes.
 def expandPath(path, factor, center=None):
     if center is None:
         center = sum(path.seq)/len(path.seq)
```

### Comparing `morpholib-0.7.0.dev1/src/morpholib/giffer.py` & `morpholib-0.7.1.dev1/src/morpholib/giffer.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.0.dev1/src/morpholib/graphics.py` & `morpholib-0.7.1.dev1/src/morpholib/graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 #            Default: True (physical units)
 class Image(BoundingBoxFigure):
     def __init__(self, source=None):
 
         # morpho.Figure.__init__(self)
         super().__init__()
 
+        self.NonTweenable("imageSurface", None)
+
         self.newSource(source)
 
         # Position in the complex plane
         pos = morpho.Tweenable("pos", complex(0), tags=["complex"])
         # align specifies where the centerpoint of the image is.
         # [0,0] means center, [-1,-1] is bottom-left, [1,1] is top-right.
         align = morpho.Tweenable(
@@ -95,17 +97,17 @@
 
         # Initialize tweenables
         self.update([pos, align, _width, _height, scale_x, scale_y,
             rotation, _transform, alpha, background, backAlpha, backPad])
 
         # If set to True, changing the width or height will
         # automatically change the other to maintain the proportion.
-        self.linked = True
-        self.aspectRatioWH = self.width/self.height
-        self.physical = True  # Are width and height in physical units, or pixel?
+        self.NonTweenable("linked", True)
+        self.NonTweenable("aspectRatioWH", self.width/self.height)
+        self.NonTweenable("physical", True)  # Are width and height in physical units, or pixel?
 
     # The "width" and "height" attrs are set up as properties,
     # because we may need to dynamically modify one in response
     # to a change in the other based on the "linked" attr.
     @property
     def width(self):
         return self._width
@@ -233,22 +235,19 @@
 
     @transform.setter
     def transform(self, value):
         self._transform = morpho.matrix.array(value)
 
 
     def copy(self):
-        # Do standard figure copy first.
-        # img = morpho.Figure.copy(self, self)
-        img = super().copy(self)
 
-        # Now copy the other parameters
-        img.linked = self.linked
-        img.aspectRatioWH = self.aspectRatioWH
-        img.physical = self.physical
+        # This is necessary because self needs to be passed
+        # into the constructor in order for the pixel dimensions
+        # to be correctly copied over!
+        img = super().copy(self)
 
         return img
 
     # Sets the "linked" attr to True and updates the aspect ratio.
     def link(self):
         # Do nothing if already linked.
         if self.linked:
@@ -538,14 +537,39 @@
         # # Set position in pixel space, adjusted by origin location.
         # self.sprite.position = \
         #     (x-self.origin[0]*self.sprite.scale_x,
         #         y-self.origin[1]*self.sprite.scale_y)
 
         # self.sprite.draw()
 
+@Image.action
+def growIn(img, duration=30, atFrame=None):
+    if atFrame is None:
+        atFrame = img.lastID()
+
+    img0 = img.last()
+    height = img0.height
+    linked = img0.linked
+    img0.visible = False
+    img1 = img.newkey(atFrame)
+    img1.link().set(height=0, visible=True)
+    img2 = img.newendkey(duration)
+    img2.set(height=height, linked=linked)
+
+@Image.action
+def shrinkOut(img, duration=30, atFrame=None):
+    if atFrame is None:
+        atFrame = img.lastID()
+
+    img.newkey(atFrame)
+    linked = img.last().linked
+    img.last().link()
+
+    img1 = img.newendkey(duration)
+    img1.set(height=0, visible=False, linked=linked)
 
 # Image class with winding number.
 # NOT IMPLEMENTED! I believe this class's purpose has been obsoleted by
 # the new "rotation" attribute of the Image class.
 # I should probably just delete this class...
 class ImagePolar(Image):
     def __init__(self, source):
@@ -569,15 +593,15 @@
 #              or just behave like a label always facing the camera. Default: False
 class SpaceImage(Image):
     def __init__(self, source=None):
         # Use superclass constructor
         super().__init__(source)
 
         # Redefine pos tweenable to be 3D.
-        _pos = morpho.Tweenable("_pos", np.zeros(3), tags=["nparray", "fimage"])
+        _pos = morpho.Tweenable("_pos", np.zeros(3), tags=["nparray", "fimage", "3d"])
         self._state.pop("pos")
         self._state["_pos"] = _pos
         _orient = morpho.Tweenable("_orient", np.identity(3), tags=["nparray", "orient"])
         self._state["_orient"] = _orient
 
         self.orientable = False
 
@@ -656,17 +680,18 @@
         orient = camera.orient
         focus = camera.focus
 
         if np.allclose(focus, 0):
             pos3d = orient @ self.pos
         else:
             pos3d = orient @ (self.pos - focus) + focus
+        pos3d = pos3d.tolist()
 
         img = Image(self)
-        img.pos = (pos3d[0] + 1j*pos3d[1]).tolist()
+        img.pos = pos3d[0] + 1j*pos3d[1]
         img.zdepth = pos3d[2]
         img.align = self.align[:]
         img._width = self._width
         img._height = self._height
         img.scale_x = self.scale_x
         img.scale_y = self.scale_y
         img.rotation = self.rotation
@@ -679,14 +704,16 @@
         img.backPad = self.backPad
 
         # img.rotateBeforeScale = self.rotateBeforeScale
         img.linked = self.linked
         img.aspectRatioWH = self.aspectRatioWH
         img.physical = self.physical
 
+        img._updateSettings(self)
+
         return [img]
 
 
     def draw(self, camera, ctx): #, orient=np.identity(3), focus=np.zeros(3)):
         primlist = self.primitives(camera)
         if len(primlist) == 0:
             return
```

### Comparing `morpholib-0.7.0.dev1/src/morpholib/grid.py` & `morpholib-0.7.1.dev1/src/morpholib/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import pyglet as pg
 pyglet = pg
 import cairo
 cr = cairo
 
 import math, cmath
 import numpy as np
+from collections.abc import Iterable
 
 
 def dummy():
     pass
 function = type(dummy)
 
 root3over2 = math.sqrt(3)/2
@@ -155,15 +156,15 @@
 class SpacePoint(Point):
     def __init__(self, pos=0, size=15, strokeWeight=1, color=None, fill=None,
         alpha=1):
         # Use superclass constructor
         super().__init__(0, size, strokeWeight, color, fill, alpha)
 
         # Redefine pos tweenable to be 3D.
-        _pos = morpho.Tweenable("_pos", morpho.matrix.array(pos), tags=["nparray", "fimage"])
+        _pos = morpho.Tweenable("_pos", morpho.matrix.array(pos), tags=["nparray", "fimage", "3d"])
         self._state.pop("pos")
         self._state["_pos"] = _pos
 
         self.pos = pos
 
         # # Change the "pos" tweenable's "complex" tag to "nparray"
         # tags = self._state["pos"].tags
@@ -196,14 +197,15 @@
         orient = camera.orient
         focus = camera.focus
 
         if np.allclose(focus, 0):
             pos3d = orient @ self.pos
         else:
             pos3d = orient @ (self.pos - focus) + focus
+        pos3d = pos3d.tolist()
 
         pt = Point()
         pt.pos = pos3d[0] + 1j*pos3d[1]
         pt.zdepth = pos3d[2]
         pt.strokeWeight = self.strokeWeight
         pt.color = self.color
         pt.fill = self.fill
@@ -217,15 +219,14 @@
     def draw(self, camera, ctx): #, orient=np.identity(3), focus=np.zeros(3)):
         primlist = self.primitives(camera)
         if len(primlist) == 0:
             return
         pt = primlist[0]
         pt.draw(camera, ctx)
 
-
 Spacepoint = SpacePoint
 
 
 # Wrapper around MultiFigure.Multi() which adds the effect
 # of segmenting the added subpaths so that tweening between
 # glyphs of different topological genus works better
 # (e.g. morphing "B" to "O" doesn't have a fill discontinuity).
@@ -534,14 +535,16 @@
             width, headSize, tailSize, dash, dashOffset,
             outlineWidth, outlineColor, outlineAlpha, origin, rotation, _transform]
             )
 
         self.Tweenable("background", (1,1,1), tags=["color"])
         self.Tweenable("backAlpha", 0, tags=["scalar"])
         self.Tweenable("backPad", 0, tags=["scalar"])
+        # Set of indices that represent where a path should terminate.
+        self.Tweenable("deadends", set(), tags=["notween"])
 
         # How to interpolate between the points given in the seq.
         # For now, the only interp method is "linear", which  means
         # connect successive points in the seq by straight lines.
         # self.interp = "linear"
         self.NonTweenable("interp", "linear")
 
@@ -550,18 +553,14 @@
         # ON and OFF dashes are, where the list is read cyclically.
         # Defaults to [] which means make the line solid.
         # Note that specifying only one value to the dash list is interpreted
         # as alternating that dash width ON and OFF.
         # Also note that dash pattern is ignored if gradient colors are used.
         # self.dash = []
 
-        # Set of indices that represent where a path should terminate.
-        # self.deadends = set()
-        self.NonTweenable("deadends", set())
-
         self.NonTweenable("headExternal", False)
         self.NonTweenable("tailExternal", False)
 
         # The technique that should be used to render outlines
         self.NonTweenable("outlineMethod", self.defaultOutlineMethod)
 
         # # Should strokes occur behind fills?
@@ -998,14 +997,17 @@
         if a is None:
             a = 0
         if b is None:
             b = 1
 
         return self.segment(a,b)
 
+    def __iter__(self):
+        raise TypeError("Paths are not iterable")
+
 
     # Returns the physical length of the path
     # NOTE: ignores deadends and pretends all nodes are connected!
     # Also ignores the transform attribute.
     def arclength(self):
         return sum(abs(self.seq[n+1]-self.seq[n]) for n in range(len(self.seq)-1))
 
@@ -1322,23 +1324,28 @@
 
         self._drawBackgroundBox(camera, ctx, self.origin, self.rotation, self._transform)
 
         # Don't bother drawing an invisible path.
         if self.alpha == 0:
             return
 
-        # Handle out-of-bounds start and end
-        if not(0 <= self.start <= 1 and 0 <= self.end <= 1):
-            drawOutOfBoundsStartEnd(self, camera, ctx)
-            return
+        tol = 1e-9  # Floating point error tolerance
 
         # Handle trivial length path and start >= end.
         len_seq = len(self.seq)
         maxIndex = len(self.seq) - 1
-        if maxIndex < 1 or self.start >= self.end:
+        if maxIndex < 1 or self.start + tol > self.end:
+            return
+
+        # Handle out-of-bounds start and end
+        if not(0 <= self.start <= 1 and 0 <= self.end <= 1):
+            backAlpha_orig = self.backAlpha
+            self.backAlpha = 0
+            drawOutOfBoundsStartEnd(self, camera, ctx)
+            self.backAlpha = backAlpha_orig
             return
 
         # Set initial transformation values to be identities
         origin = self.origin
         rot = mat = 1
         mat_inv = 1
 
@@ -1349,15 +1356,14 @@
             # If transform matrix is too distorted, don't draw.
             if morpho.matrix.thinness2x2(self.transform) < 1e-6:
                 return
             mat = morpho.matrix.Mat(*self.transform.flatten().tolist())
             mat_inv = mat.inv
 
         # Compute index bounds.
-        tol = 1e-9  # Snap to nearest integer if within this much of an integer.
         start = self.start*maxIndex
         if abs(start - round(start)) < tol:
             start = round(start)
         int_start = int(start)
 
         end = self.end*maxIndex
         if abs(end - round(end)) < tol:
@@ -2020,15 +2026,24 @@
     def squeeze(self):
         for path in self.figures[:]:
             if path.nodeCount() < 2:
                 self.figures.remove(path)
         return self
 
     def draw(self, camera, ctx):
-        self._drawBackgroundBox(camera, ctx, self.origin, self.rotation, self._transform)
+        # Don't draw empty MultiPath
+        if len(self.figures) == 0:
+            return
+
+        # Since there is no top-level alpha attribute for MultiPaths,
+        # it is inferred from the maximum alpha across all subpaths.
+        self._drawBackgroundBox(
+            camera, ctx, self.origin, self.rotation, self._transform,
+            _alpha=max(subpath.alpha for subpath in self.figures)
+            )
 
         # Temporarily apply additional transforms to subfigures if global
         # rotation/transform are non-identity
         if not(self.rotation == 0 and np.array_equal(self._transform, I2)):
             # Calculate as a single matrix the overall effect
             # of both the global rotation and transform.
             rotateAndTransform = self._transform @ morpho.matrix.rotation2d(self.rotation)
@@ -2073,14 +2088,178 @@
         return pivot
 
 Multipath = MultiPath  # Alias
 
 # Assign MultiPath as the Path class's dedicated multifigure version.
 Path._multitype = MultiPath
 
+# Like regular morphFrom(), except the source can optionally
+# be a list of actors/figures, in which case, the morph will
+# be performed from all of those figures.
+@MultiPath.action
+def morphFrom(actor, source, *args, **kwargs):
+    if isinstance(source, (list, tuple)):
+        if len(source) == 0:
+            raise TypeError("Source to morph from is empty.")
+        # Prepare the list of figures to morph from
+        mpaths = [mpath.last().copy() if isinstance(mpath, morpho.Actor) else mpath.copy() for mpath in source]
+        for mpath in mpaths:
+            mpath.commitTransforms()
+
+        # Combine into a single MultiPath figure
+        combined = mpaths[0]
+        for mpath in mpaths[1:]:
+            combined.merge(mpath)
+
+        return actor.morphFrom(combined, *args, **kwargs)
+    else:
+        return morpho.Figure.actions["morphFrom"](actor, source, *args, **kwargs)
+
+# Highlights the MultiPath actor
+@MultiPath.action
+def highlight(actor, duration=15, atFrame=None, *,
+    width=-3, fill=(1,1,0), color=(0,0,0), rescale=1, select=None):
+
+    if atFrame is None:
+        atFrame = actor.lastID()
+
+    if select is None:
+        select = sel[:]
+    elif isinstance(select, Iterable):
+        select = tuple(select)
+
+    path0 = actor.last()
+    path1 = actor.newkey(atFrame)
+    path2 = actor.newendkey(duration)
+
+    # Assignment to subframe needs to happen because
+    # if `select` is a choice function, modifying the
+    # width/fill/color of the subpaths can change what
+    # the choice function selects on the second call.
+    subframe = path2.select[select]
+    subframe.set(width=width, fill=fill, color=color)
+    if rescale != 1:
+        if select == sel[:]:
+            path2.rescale(rescale)
+        else:
+            subframe.rescale(rescale)
+
+# Highlights then immediately de-highlights the MultiPath actor.
+# Optional keyword input `pause` can be used to specify a number
+# of frames to pause after highlighting and before de-highlighting.
+@MultiPath.action
+def flourish(actor, duration=15, atFrame=None, *, pause=0, **kwargs):
+
+    if atFrame is None:
+        atFrame = actor.lastID()
+
+    path0 = actor.last()
+    path1 = actor.newkey(atFrame)
+
+    actor.highlight(duration, atFrame, **kwargs)
+    if pause > 0:
+        actor.newendkey(pause)
+    actor.newendkey(duration, path1.copy())
+
+
+# 3D version of MultiPath meant to enable 2D MultiPaths to be
+# positionable and orientable in 3D space. This is NOT a full
+# SpaceMultiPath class, which would be a MultiFigure of
+# SpaceSplines! Rather, this is just a regular 2D MultiPath
+# which can be rendered in a 3D space like SpaceImage can.
+#
+# The main differences from 2D MultiPaths is three new attributes:
+# pos = 3D position as an np.array. Default: [0,0,0] (the origin)
+# orient = Orientation in 3D space as a 3x3 rotation matrix.
+#       Default: np.eye(3) (oriented on the xy-plane facing the
+#       +z direction)
+# orientable = Boolean denoting whether the MultiPath should be
+#       treated as an orientable 3D object, or more like a
+#       2D "sticker" object. Default: False
+#
+# Note that `pos` is not merely an alias for `origin` like it is
+# for 2D MultiPaths. Here they are distinct: `pos` controls 3D
+# position, whereas `origin` controls 2D position within the
+# MultiPath's local plane.
+class MultiPath3D(MultiPath):
+    def __init__(self, seq=None, *args, **kwargs):
+        if isinstance(seq, MultiPath):
+            # Convert 2D MultiPath into 3D MultiPath
+            mpath = seq
+            super().__init__(None, *args, **kwargs)
+            self._updateFrom(mpath)
+        else:
+            super().__init__(seq, *args, **kwargs)
+
+        self.Tweenable("_pos", np.zeros(3), tags=["nparray", "nofimage", "3d"])
+        self.Tweenable("_orient", np.eye(3), tags=["nparray", "orient"])
+
+        self.NonTweenable("orientable", False)
+
+    @property
+    def pos(self):
+        return self._pos
+
+    @pos.setter
+    def pos(self, value):
+        self._pos = morpho.matrix.array(value)
+
+    @property
+    def orient(self):
+        return self._orient
+
+    @orient.setter
+    def orient(self, value):
+        self._orient = morpho.matrix.array(value)
+
+    def primitives(self, camera):
+        pos3d = camera.orient @ (self.pos - camera.focus) + camera.focus
+        pos3d = pos3d.tolist()
+
+        mpath = MultiPath()
+        mpath._updateFrom(self, common=True, copy=False)
+        if self.orientable:
+            totalOrientTransform = (camera.orient @ self.orient)[:2,:2]
+            mpath._transform = totalOrientTransform @ mpath._transform
+            mpath.origin = pos3d[0] + 1j*pos3d[1] + morpho.matrix.Mat(totalOrientTransform)*mpath.origin
+        else:
+            mpath.origin += pos3d[0] + 1j*pos3d[1]
+        mpath.zdepth = pos3d[2]
+
+        return [mpath]
+
+    draw = morpho.SpaceFigure.draw
+
+    ### TWEEN METHODS ###
+
+    @classmethod
+    def tweenPivot(cls, *args, **kwargs):
+        raise NotImplementedError
+
+MultiPath3d = MultiPath3D
+
+@MultiPath3D.action
+def fadeIn(mpath, duration=30, atFrame=None, jump=0, alpha=1):
+    morpho.Frame.actions["fadeIn"](mpath, duration, atFrame, 0, alpha)
+    jump = morpho.array(jump)
+    if duration > 0:
+        mpath.key[-2].pos = mpath.key[-2].pos - jump
+
+@MultiPath3D.action
+def fadeOut(mpath, duration=30, atFrame=None, jump=0):
+    morpho.Frame.actions["fadeOut"](mpath, duration, atFrame, 0)
+    jump = morpho.array(jump)
+    if duration > 0:
+        mpath.last().pos = mpath.last().pos + jump
+
+# Inherited morphFrom() from 2D MultiPath doesn't work for
+# 3D MultiPaths unfortunately, so default back to the original
+# morphFrom() for all figures.
+MultiPath3D.actions["morphFrom"] = morpho.Figure.actions["morphFrom"]
+
 class Track(Path):
     '''Path with tick marks - like a train track: --|--|--|--
 
     TWEENABLES (in addition to those inherited from Path)
     tickWidth = Width of tickmarks in pixels. Default: self.width/2
     tickLength = Length of tickmarks in pixels. Default: 15
     tickColor = Tickmark color (RGB vector-like).
@@ -2298,14 +2477,21 @@
         # Now draw self using the supermethod
         super().draw(camera, ctx)
 
 
 # Special modification of the list class so that whenever
 # an item is set, it converts it into a np.array of floats.
 class Arraylist(list):
+
+    # These lines have been commented out because I think
+    # the performance cost of looping over the array elements
+    # in python is too high. Also, this class is really only
+    # meant to be used internally, so it's fine if it doesn't
+    # behave ideally.
+
     # def __init__(self, *args, **kwargs):
     #     super().__init__(*args, **kwargs)
 
     #     # Reassign to convert to np.array() via modified __setitem__()
     #     for n in range(len(self)):
     #         self[n] = self[n]
 
@@ -2361,24 +2547,19 @@
         # Also note that dash pattern is ignored if gradient colors are used.
         # self.dash = []
 
         origin = morpho.matrix.array([0,0,0])
 
         # Update the seq attribute's value
         if seq is None:
-            seq = Arraylist([0,1])
+            seq = Arraylist([morpho.array(0), morpho.array(1)])
         elif type(seq) is Path:
-            # Copy over state and all other attributes except seq
-            for name in self._state:
-                if name != "seq":
-                    self._state[name] = seq._state[name].copy()
-            # Copy other attributes
-            self.interp = seq.interp
-            # self.dash = seq.dash[:]
-            self.deadends = seq.deadends.copy()
+            # Copy over state and all other attributes except `seq`
+            # and `origin`
+            self._updateFrom(seq, common=True, ignore={"seq", "origin"})
             origin = morpho.matrix.array(seq.origin)
 
             # FUTURE: Have SpacePath detect non-trivial rotation
             # and transform attributes and either modify the node
             # list, OR modify 3D rotation and transform if you ever
             # decide to implement those.
 
@@ -2645,16 +2826,61 @@
 
         # # Linearly tween the focus vector manually
         # if not np.array_equal(self.focus, other.focus):
         #     tw.focus = morpho.numTween1(self.focus, other.focus, t)
 
         return tw
 
-    # There is no spiral tween for spacepaths (yet, at least)
-    tweenSpiral = tweenLinear
+    # 3D spiral tween method
+    @morpho.TweenMethod
+    @handleDash
+    @morpho.color.handleGradients(["color"])
+    @morpho.color.handleGradientFills(["fill"])
+    @handlePathNodeInterp
+    def tweenSpiral(self, other, t):
+
+        # Tween everything except the node sequence.
+        tw = morpho.Figure.tweenSpiral(self, other, t, ignore="_seq")
+
+        pseq = np.array(self._seq, dtype=float)   # N x 3 array of nodes
+        qseq = np.array(other._seq, dtype=float)  # N x 3 array of nodes
+
+        result = morpho.spiralInterpArray3d(pseq, qseq, t, verbose=True)
+        tw._seq = list(result["twseq"])
+
+        # This clause disconnects two nodes if they are
+        # revolving in different directions too much.
+        # The value angle_tol represents how far two oppositely
+        # revolving nodes have to angularly differ before
+        # we disconnect them.
+        if 0.01 < t < 0.99:
+            crossProds = result["crossProds"]
+            good = result["good"]
+
+            crossProds1 = crossProds[:-1]
+            crossProds2 = crossProds[1:]
+
+            # Deadends should occur whenever the rotation axes of two
+            # neighboring nodes are anti-aligned OR whenever a good node
+            # is adjacent to a bad node. However, if either of the
+            # two neighboring nodes matches its respective destination
+            # node, then don't disconnect the node pair
+            # (this last condition is to allow cases like arrows
+            # where the tail sits at the origin (a "bad" node), but
+            # the head moves).
+            flagset = ((np.sum(crossProds1*crossProds2, axis=1) < -1e-10) | (good[:-1]^good[1:])) \
+                & ~np.all(np.isclose(pseq[:-1], qseq[:-1]), axis=1) \
+                & ~np.all(np.isclose(pseq[1:], qseq[1:]), axis=1)
+
+
+            tw.deadends.update(np.where(flagset)[0].tolist())
+
+        return tw
+
+
 
 Spacepath = SpacePath  # Synonym for SpacePath
 
 
 # 3D version of the Track class.
 # See `Track` and `SpacePath` for more info.
 class SpaceTrack(SpacePath, Track):
@@ -2677,15 +2903,17 @@
         self.tickAlpha = tickAlpha
         self.tickLength = tickLength
         self.tickGap = tickGap
 
 
     def primitives(self, camera):
         # Compute primitive 2D path
-        path = SpacePath.primitives(self, camera)[0]
+        primitives = SpacePath.primitives(self, camera)
+        if len(primitives) == 0: return []
+        path = primitives[0]
         # Turn it into a 2D Track figure
         track = Track()
         track.seq = path.seq  # No need to copy it.
         # Override its default values with those of self
         # (e.g. tickWidth, tickColor, etc.)
         track._updateFrom(self, copy=False, common=True)
         return [track]
@@ -2776,15 +3004,17 @@
         self.seq[1] = origEnd
 
 
 # Mainly for internal use.
 # 3D version of the Axis class. See `Axis` for more info.
 class SpaceAxis(SpaceTrack):
     def primitives(self, camera):
-        track = SpaceTrack.primitives(self, camera)[0]
+        primitives = SpaceTrack.primitives(self, camera)
+        if len(primitives) == 0: return []
+        track = primitives[0]
         axis = Axis()
         axis._updateFrom(track, copy=True, common=True)
 
         # Scale tick spacing based on how much the axis has
         # shrunk due to foreshortening.
         axis.tickGap *= abs(axis.seq[1]-axis.seq[0]) / np.linalg.norm(self.seq[1]-self.seq[0]).tolist()
 
@@ -3069,14 +3299,30 @@
         frm.figures.append(yaxis)
         frm.setName(yaxis=yaxis)
 
     frm.transition = transition
 
     return frm
 
+# 3D version of mathaxes(). Creates a pair of axes in the xy-plane.
+# See "mathaxes" for more info.
+def mathaxes3d(*args, **kwargs):
+    axes = mathaxes(*args, **kwargs)
+    axes3d = SpaceMathGrid()
+
+    # Convert subfigures to SpaceAxis type
+    for subfig in axes.figures:
+        newfig = SpaceAxis()
+        newfig._updateFrom(subfig, copy=False, common=True)
+        newfig.seq = subfig.seq  # This will convert 2D to 3D implicitly
+        axes3d.figures.append(newfig)
+
+    return axes3d
+
+
 
 # Construct a grid-like frame figure.
 #
 # INPUTS (keyword-only)
 # view = Bounding box of the grid ([xmin,xmax,ymin,ymax]). Default: [-5,5, -5,5]
 # dx,dy = Grid spacing in physical units. Default: 1
 #         You can also specify `spacing` to set both to the same value.
@@ -3198,15 +3444,15 @@
         )
 mathGrid = mathgrid  # Alternate camel-case name.
 
 # 3D version of mathgrid(). Creates a grid in the xy-plane.
 # See "mathgrid" for more info.
 def mathgrid3d(*,
     view=(-5,5, -5,5),
-    dx=1, dy=1,
+    dx=1, dy=1, spacing=None,
     hsteps=50, vsteps=50, steps=None,
     hnodes=None, vnodes=None, nodes=None,
     hcolor=(0,0,1), vcolor=(0,0,1), color=None, alpha=1,
     hmidColor=None, vmidColor=None, midColor=None,
     hwidth=3, vwidth=3, width=None,
     hmidlines=True, vmidlines=True, midlines=None,
     hmidWidth=1, vmidWidth=1, midWidth=None,
@@ -3214,54 +3460,55 @@
     xaxisWidth=5, yaxisWidth=5, axisWidth=None,
     tweenMethod=Spacepath.tweenLinear,
     transition=None,
     optimize=True):
 
     wire = mathgrid(
         view=view,
-        dx=dx, dy=dy,
+        dx=dx, dy=dy, spacing=spacing,
         hsteps=hsteps, vsteps=vsteps, steps=steps,
         hnodes=hnodes, vnodes=vnodes, nodes=nodes,
         hcolor=hcolor, vcolor=vcolor, color=color, alpha=alpha,
         hmidColor=hmidColor, vmidColor=vmidColor, midColor=midColor,
         hwidth=hwidth, vwidth=vwidth, width=width,
         hmidlines=hmidlines, vmidlines=vmidlines, midlines=midlines,
         hmidWidth=hmidWidth, vmidWidth=vmidWidth, midWidth=midWidth,
         BGgrid=False, axes=axes, axesColor=axesColor,
         xaxisWidth=xaxisWidth, yaxisWidth=yaxisWidth, axisWidth=axisWidth,
         axesStatic=False, polar=False,
-        tweenMethod=tweenMethod,
         transition=transition,
         optimize=optimize
         )
     wire = SpaceMathGrid(wire)
     for n in range(len(wire.figures)):
         # wire.figures[n] = Spacepath(wire.figures[n], orient.copy(), offset)
-        wire.figures[n] = SpacePath(wire.figures[n])
+        subfig = SpacePath(wire.figures[n])
+        subfig.set(tweenMethod=tweenMethod)
+        wire.figures[n] = subfig
 
     return wire
 
 # Equivalent to mathgrid(), but hsteps/vsteps default to 1,
 # and `BGgrid` and `axes` default to False.
 # See mathgrid() for more info.
-def basicgrid(
+def basicgrid(*,
     hsteps=1, vsteps=1,
     BGgrid=False, axes=False,
     **kwargs):
 
     return mathgrid(
         hsteps=hsteps, vsteps=vsteps,
         BGgrid=BGgrid, axes=axes,
         **kwargs
         )
 
 # Equivalent to mathgrid3d(), but hsteps/vsteps default to 1,
 # and `axes` defaults to False.
 # See mathgrid3d() for more info.
-def basicgrid3d(
+def basicgrid3d(*,
     hsteps=1, vsteps=1,
     axes=False,
     **kwargs):
 
     return mathgrid3d(
         hsteps=hsteps, vsteps=vsteps,
         axes=axes,
@@ -3329,14 +3576,19 @@
 
     # hnodes and vnodes determined by hsteps and vsteps if unspecified.
     if hnodes is None:
         hnodes = hsteps + 1
     if vnodes is None:
         vnodes = vsteps + 1
 
+    if isinstance(hcolor, morpho.color.Gradient):
+        raise TypeError("hcolor cannot be a gradient")
+    if isinstance(vcolor, morpho.color.Gradient):
+        raise TypeError("vcolor cannot be a gradient")
+
     hcolor = list(hcolor)
     vcolor = list(vcolor)
 
     if hmidColor is None:
         hmidColor = (1-0.5*(1-morpho.array(hcolor))).tolist()
     else:
         hmidColor = list(hmidColor)
@@ -3617,31 +3869,25 @@
             origin, rotation, _transform])
 
         # If set to True, then if fill is a GradientFill,
         # the border will be stroked using the GradientFill
         # instead of self.color.
         # Mainly for use by the Quadmesh class to remove
         # seams when width is zero and fill is a color function.
-        self._strokeGradient = False
+        self.NonTweenable("_strokeGradient", False)
+        # self._strokeGradient = False
 
     @property
     def transform(self):
         return self._transform
 
     @transform.setter
     def transform(self, value):
         self._transform = morpho.matrix.array(value)
 
-    def copy(self):
-        new = super().copy()
-
-        new._strokeGradient = self._strokeGradient
-
-        return new
-
     # Applies all of the transformation attributes
     # origin, rotation, transform
     # to the actual vertices list itself and then
     # resets the transformation attributes.
     def commitTransforms(self):
         rot = cmath.exp(self.rotation*1j)
         mat = morpho.matrix.Mat(*self.transform.flatten().tolist())
@@ -3685,14 +3931,23 @@
             path.rotation = self.rotation
         if "_transform" in self._state:
             path.transform = self.transform
 
 
         return path
 
+    # Converts the Polygon into an equivalent Path figure.
+    def toPath(self):
+        path = type(self)._edgeType(self.vertices[:])
+        path.close()
+
+        path._updateFrom(self, common=True)
+
+        return path
+
     def draw(self, camera, ctx):
 
         if len(self.vertices) < 2 or self.alpha == 0: return
 
         # # If determinant of the transform matrix is too small,
         # # don't attempt to draw.
         # if abs(np.linalg.det(self.transform)) < 1e-6:
@@ -3807,45 +4062,43 @@
 # The vertices in the list do not necessarily have to be coplanar, but
 # the polygon may look incorrect when viewed from certain angles if not.
 # This figure is primarily intended to draw planar polygons oriented in
 # 3D space.
 # Note that the transformation tweenables "rotation" and "transform"
 # are unsupported.
 class SpacePolygon(Polygon):
-    def __init__(self, vertices=None, width=3, color=(0,0,0), alphaEdge=1,
+    def __init__(self, vertices=None, width=3, color=(1,1,1), alphaEdge=1,
         fill=(1,0,0), alphaFill=1,
         alpha=1):
 
         super().__init__(None, width, color, alphaEdge,
             fill, alphaFill, alpha)
 
         origin = morpho.matrix.array([0,0,0])
 
         # Update the vertices attribute's value
         if vertices is None:
             vertices = Arraylist([])
         elif type(vertices) is Polygon:
-            # Copy over state and all other attributes except vertices
-            for name in self._state:
-                if name != "vertices":
-                    self._state[name] = vertices._state[name].copy()
-
+            # Copy over state and all other attributes except
+            # `vertices` and `origin`
+            self._updateFrom(vertices, common=True, ignore={"vertices", "origin"})
             origin = morpho.matrix.array(vertices.origin)
 
             # FUTURE: Have SpacePolygon detect non-trivial rotation
             # and transform attributes and either modify the vertex
             # list, OR modify 3D rotation and transform if you ever
             # decide to implement those.
 
             # Reassign vertices to the actual list of complex numbers
             vertices = vertices.vertices
 
         # Redefine vertices tweenable to be 3D.
         vertices = Arraylist(morpho.matrix.array(vertices[n]) for n in range(len(vertices)))
-        _vertices = morpho.Tweenable("_vertices", vertices, tags=["nparray", "list", "fimage", "nospiral"])
+        _vertices = morpho.Tweenable("_vertices", vertices, tags=["nparray", "list", "fimage", "3d"])
         self._state.pop("vertices")
         self._state["_vertices"] = _vertices
 
         # Re-implement "origin" as a property so it will auto-convert
         # into np.array.
         self._state.pop("origin")
         _origin = morpho.Tweenable("_origin", origin, tags=["nparray", "nofimage"])
@@ -4029,15 +4282,15 @@
             array[0,1,:] = [0,1,0]
             array[1,1,:] = [1,1,0]
 
         # Convert array to a float array if it's not already
         if array.dtype is not np.dtype(float):
             array = np.array(array, dtype=float)
 
-        _array = morpho.Tweenable(name="_array", value=morpho.matrix.array(array), tags=["nparray"])
+        _array = morpho.Tweenable(name="_array", value=morpho.matrix.array(array), tags=["nparray", "3d"])
         color = morpho.Tweenable(name="color", value=color, tags=["color"])
         alphaEdge = morpho.Tweenable(name="alphaEdge", value=alphaEdge, tags=["scalar"])
         fill = morpho.Tweenable(name="fill", value=fill, tags=["color", "nolinear"])
         fill2 = morpho.Tweenable(name="fill2", value=fill2, tags=["color", "nolinear"])
         alphaFill = morpho.Tweenable(name="alphaFill", value=alphaFill, tags=["scalar"])
         alpha = morpho.Tweenable(name="alpha", value=alpha, tags=["scalar"])
         width = morpho.Tweenable(name="width", value=width, tags=["size"])
@@ -4235,15 +4488,15 @@
 
         return newfig
 
     ### TWEEN METHODS ###
 
     def tweenLinear(self, other, t, *args, **kwargs):
         # Do standard tween first
-        tw = super().tweenLinear(other, t, *args, **kwargs)
+        tw = morpho.Figure.tweenLinear(self, other, t, *args, **kwargs)
 
         # Handle tween fill if it's a color function
         if callable(self.fill):
             if not callable(other.fill):
                 raise TypeError("Can't tween color function with non color function.")
             tw.fill = lambda v: (1-t)*morpho.matrix.array(self.fill(v)) + t*morpho.matrix.array(other.fill(v))
             return tw
@@ -4260,14 +4513,19 @@
         if (self.fill2 is None and other.fill2 is None):
             return tw
         self_fill2 = self.fill if self.fill2 is None else self.fill2
         other_fill2 = other.fill if other.fill2 is None else other.fill2
         tw.fill2 = [morpho.numTween(self_fill2[n], other_fill2[n], t) for n in range(3)]
         return tw
 
+    def tweenSpiral(self, other, t):
+        tw = self.tweenLinear(other, t, ignore="_array")
+        tw._array = morpho.spiralInterpArray3d(self._array.reshape(-1,3), other._array.reshape(-1,3), t).reshape(self._array.shape)
+        return tw
+
 QuadMesh = Quadmesh  # Synonym for Quadmesh class
 
 # Decorator modifies a color function (map from numpy 3-vectors to RGB)
 # to ensure the RGB vector-like thing it returns is a vanilla python
 # list of python floats. Helps to ensure consistency in the types.
 def handleColorTypeCasting(colorfunc):
     def wrapper(v):
@@ -4290,22 +4548,25 @@
 # alphaFill = Quadmesh interior opacity. Default: 1 (opaque)
 # alpha = Overall opacity. Multiplies alphaEdge and alphaFill. Default: 1 (opaque)
 # fill2 = Alternate fill used to create checkerboard pattern (RGB list).
 #         Ignored if primary fill is a color function.
 #         Default: None (match primary fill; i.e. no checkerboard pattern)
 # tweenMethod = Tween method to assign. Default: Quadmesh.tweenLinear
 # transition = Transition function to assign. Default: morpho.transition.default
+#
+# Any additional keyword inputs are set as attributes of the returned
+# Quadmesh.
 def quadgrid(*,
     view=(-5,5, -5,5),
     dx=1, dy=1,
     width=3,
     color=(0,0,0), alphaEdge=1,
     fill=(1,0,0), alphaFill=1, alpha=1, fill2=None,
     tweenMethod=Quadmesh.tweenLinear,
-    transition=None):
+    transition=None, **kwargs):
 
     xmin, xmax, ymin, ymax = view
     xmax += 1.0e-6  # +epsilon to deal with floating point error
     ymax += 1.0e-6
 
     Nx = 1 + int((xmax-xmin) // dx)
     Ny = 1 + int((ymax-ymin) // dy)
@@ -4314,19 +4575,22 @@
         for j in range(Ny):
             array[i,j,:] = [xmin+i*dx, ymin+j*dy, 0]
 
     quadmesh = Quadmesh(
         array, width, color, alphaEdge,
         fill, alphaFill, alpha, fill2
         )
+    quadmesh.tweenMethod = tweenMethod
 
     if transition is None:
         transition = morpho.transition.default
     quadmesh.transition = transition
 
+    quadmesh.set(**kwargs)
+
     return quadmesh
 
 
 # Pointy line segment. Kind of like path, but only supports two vertices
 # (tail and head). But contains a few helpful methods/properties that
 # calculate some useful vector properties (length, angle, etc.)
 #
```

### Comparing `morpholib-0.7.0.dev1/src/morpholib/matrix.py` & `morpholib-0.7.1.dev1/src/morpholib/matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,19 +45,20 @@
             array = np.array([[x1,x2],[y1,y2]], dtype=float)
         self.array = array
 
     def __mul__(self, other):
         # If given a scalar, treat it as a 2D vector and do
         # matrix multiplication
         if isinstance(other, complex) or isinstance(other, float) or \
-            isinstance(other, int) or isinstance(other, np.number):
+            isinstance(other, int) or isinstance(other, np.number) or \
+            (isinstance(other, np.ndarray) and other.size == 1):
 
             # Convert to 2D vector, compute matrix product, and
             # convert back to complex
-            Z = np.array([other.real, other.imag])
+            Z = np.array([other.real, other.imag]).squeeze()
             prod = (self.array @ Z).tolist()
             return prod[0] + 1j*prod[1]
 
         # If given another matrix, do matrix multiplication directly
         # on the underlying arrays.
         elif isinstance(other, type(self)):
             return type(self)(self.array @ other.array)
@@ -170,14 +171,26 @@
                 v = mat[:,j]
                 if not np.allclose(v, 0):
                     break
             return (v/np.linalg.norm(v), math.pi)
 
     return (rho/s, math.atan2(s,c))
 
+# Returns the wedge product as a skew-symmetric matrix.
+# That is, returns outer(u,v) - outer(v,u)
+def wedge(u, v):
+    outprod = np.outer(u,v)
+    return outprod - outprod.T
+
+# Returns the tilt product of u and v.
+# That is, returns outer(v,u) - outer(u,v)
+# or equivalently: wedge(v,u)
+def tilt(u, v):
+    return wedge(v,u)
+
 # Returns the 2D rotation matrix associated with the
 # input angle.
 def rotation2d(angle):
     c = math.cos(angle)
     s = math.sin(angle)
 
     return np.array([[c, -s], [s, c]], dtype=float)
```

### Comparing `morpholib-0.7.0.dev1/src/morpholib/sample.py` & `morpholib-0.7.1.dev1/src/morpholib/sample.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.0.dev1/src/morpholib/shapes.py` & `morpholib-0.7.1.dev1/src/morpholib/shapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,21 @@
 from morpholib.tools.dev import drawOutOfBoundsStartEnd, BoundingBoxFigure, \
     totalBox, shiftBox, translateArrayUnderTransforms
 from morpholib.matrix import mat
 from morpholib.anim import MultiFigure
 
 from morpholib import object_hasattr
 
-# Polygon and SpacePolygon can be accessed from the shapes
-# submodule as well as grid.
-from morpholib.grid import Polygon, SpacePolygon, Spacepolygon
+# Import these names from grid module so they can optionally
+# be accessed from the shapes module.
+from morpholib.grid import Polygon, SpacePolygon, Spacepolygon, \
+    Path, SpacePath, Spacepath, MultiPath, Multipath, MultiPath3D, \
+    MultiPath3d, Arrow, SpaceArrow, Point, SpacePoint, Spacepoint, \
+    Track, SpaceTrack, line, spaceLine, spaceline, rect
+from morpholib.grid import ellipse as ellipsePolygon
 
 import cairo
 cr = cairo
 
 import svgelements as se
 import io
 
@@ -171,28 +175,27 @@
         self.extendState([_data, start, end, color, alphaEdge, fill, alphaFill, alpha,
             width, dash, dashOffset, origin, rotation, _transform]
             )
 
         self.Tweenable("background", (1,1,1), tags=["color"])
         self.Tweenable("backAlpha", 0, tags=["scalar"])
         self.Tweenable("backPad", 0, tags=["scalar"])
+        # Set of indices that represent where a path should terminate.
+        self.Tweenable("deadends", set(), tags=["notween"])
 
 
         # The dash pattern for this line. The format is identical to how
         # pycairo handles dash patterns: each item in the list is how long
         # ON and OFF dashes are, where the list is read cyclically.
         # Defaults to [] which means make the line solid.
         # Note that specifying only one value to the dash list is interpreted
         # as alternating that dash width ON and OFF.
         # Also note that dash pattern is ignored if gradient colors are used.
         # self.dash = []
 
-        # Set of indices that represent where a path should terminate.
-        self.NonTweenable("deadends", set())
-
         # Boolean indicates whether the control point tangents
         # should be shown. This is mainly for debugging purposes.
         self.NonTweenable("showTangents", False)
 
         # # Should strokes occur behind fills?
         # self.NonTweenable("backstroke", False)
 
@@ -218,23 +221,14 @@
     def pos(self):
         return self.origin
 
     @pos.setter
     def pos(self, value):
         self.origin = value
 
-
-    def copy(self):
-        new = super().copy()
-        # new.dash = self.dash.copy() if "copy" in dir(self.dash) else self.dash
-        new.deadends = self.deadends.copy()
-        new.showTangents = self.showTangents
-
-        return new
-
     # Computes the loose bounding box of the spline.
     # That is, it returns the bounding box of all the
     # control points (positional and tangent) the spline contains.
     # This function may be improved in a future version to return
     # a tighter bounding box.
     #
     # If optional kwarg `raw` is set to True, the
@@ -284,15 +278,15 @@
         # for n in range(len(data)-1):
         #     p0 = data[n, 0].tolist()
         #     p1 = data[n, 2].tolist()
         #     p2 = data[n+1, 1].tolist()
         #     p3 = data[n+1, 0].tolist()
         #     subboxes.append(morpho.bezier.cubicbox(p0, p1, p2, p3))
 
-        # return totalBox(subboxes)
+        # return shiftBox(totalBox(subboxes), self.origin if not raw else 0)
 
     boxAlign = morpho.grid.Path.boxAlign
     rescale = morpho.grid.Path.rescale
     resize = morpho.grid.Path.resize
 
     # Transforms the spline so that the `origin` attribute
     # is in the physical position indicated by the alignment
@@ -521,14 +515,49 @@
         else:
             svgbbox = np.array(svgpath.bbox()).tolist()
         spline._transformForSVG(svgbbox, boxWidth, boxHeight, svgOrigin, align, flip)
 
         spline.set(**kwargs)  # Pass any additional kwargs to set()
         return spline
 
+    # Returns True if the compared spline has exactly the same size, shape,
+    # and position as self, ignoring transformation attributes.
+    def coincides(self, other):
+        self = self.copy()
+        other = other.copy()
+
+        self.commitHandles()
+        other.commitHandles()
+
+        with np.errstate(all="ignore"):  # Suppress numpy warnings
+            return self.deadends == other.deadends and \
+                self._data.shape == other._data.shape and \
+                np.allclose(self._data, other._data)
+
+    # Returns a "normalized" version of the spline where
+    # its box center is at the origin, all transformation attributes
+    # have been reset, and its boxHeight has been set to 1.
+    # Mainly for use by matchesShape() to compare different splines.
+    def _normalizedShape(self):
+        source = self.copy()
+        source.rotation = 0
+        source._transform = I2
+        source.resize(boxHeight=1)
+        source.origin -= source.center()
+        if source.origin != 0:
+            source.commitTransforms()
+        return source
+
+    # Checks if the given spline has the same shape as self,
+    # but only differs by size, position, or transformation
+    # attribute.
+    def matchesShape(self, other):
+        source = self._normalizedShape()
+        target = other._normalizedShape()
+        return source.coincides(target)
 
     # Returns the node count of the spline
     def length(self):
         return self.data.shape[0]
 
     # Returns the number of nodes
     def nodeCount(self):
@@ -1009,14 +1038,17 @@
 
         return subspline
 
     # Inherits the Path class's __getitem__()
     def __getitem__(self, t):
         return morpho.grid.Path.__getitem__(self, t)
 
+    def __iter__(self):
+        raise TypeError("Splines are not iterable")
+
 
     # Inserts the specified number of additional nodes to the
     # spline by interpolating along it. For large numNodes, the new
     # nodes will tend to bunch around the original nodes.
     def insertNodes(self, numNodes):
         segCount = self.length() - 1
         for n in range(numNodes):
@@ -1178,36 +1210,40 @@
 
         self._drawBackgroundBox(camera, ctx, self.origin, self.rotation, self._transform)
 
         # Need at least two nodes to draw
         if self.data.shape[0] < 2:
             return
 
+        tol = 1e-9  # Floating point error tolerance
+
         # Handle trivial length path and start >= end.
         len_seq = self.length()
         maxIndex = len_seq - 1
-        if maxIndex < 1 or self.start >= self.end or self.alpha == 0:
+        if maxIndex < 1 or self.start + tol > self.end or self.alpha == 0:
             return
 
         # # If determinant of the transform matrix is too small,
         # # don't attempt to draw.
         # if abs(np.linalg.det(self._transform)) < 1e-6:
         #     return
 
         # If transform matrix is too distorted, don't draw.
         if morpho.matrix.thinness2x2(self.transform) < 1e-6:
             return
 
         # Handle out-of-bounds start and end
         if not(0 <= self.start <= 1 and 0 <= self.end <= 1):
+            backAlpha_orig = self.backAlpha
+            self.backAlpha = 0
             drawOutOfBoundsStartEnd(self, camera, ctx)
+            self.backAlpha = backAlpha_orig
             return
 
         # Compute index bounds
-        tol = 1e-9  # Snap to nearest integer if within this much of an integer.
         start = self.start*maxIndex
         if abs(start - round(start)) < tol:
             start = round(start)
         int_start = int(start)
         end = self.end*maxIndex
         if abs(end - round(end)) < tol:
             end = round(end)
@@ -1659,15 +1695,15 @@
     #
     # By default it constructs a Spline from every SVG Path element
     # found within the source, but this can be changed by passing
     # in a tuple for the `index` input:
     #      index=(start, stop, step)
     # The tuple is interpreted identically to how range() works.
     # Any additional keyword arguments are set as attributes of
-    # the returned figure.
+    # the returned figure or its subfigures.
     @classmethod
     def fromsvg(cls, source, *,
         svgOrigin=None, align=(0,0), boxWidth=None, boxHeight=None,
         index=(None,), flip=True, arcError=0.1, tightbox=False,
         **kwargs):
 
         svg = parseSVG(source)
@@ -1731,16 +1767,34 @@
             boxHeight = box[-1] - box[-2]
         multispline = morpho.latex.parse(tex,
             align=align, boxWidth=boxWidth, boxHeight=boxHeight,
             **kwargs
             )
         self.figures = multispline.figures
         if pos is not None:
-            self.origin = pos
-        return self
+            # Using self.pos is intentional here! Don't replace with self.origin!
+            # This is because self.pos means something different for MultiSpline3D!
+            self.pos = pos
+        return self
+
+    # Checks if every corresponding subfigure between self and other
+    # coincides. See Spline.coincides() for more info.
+    def coincides(self, other):
+        return len(self.figures) == len(other.figures) and \
+            self.origin == other.origin and \
+            self.rotation == other.rotation and \
+            np.array_equal(self._transform, other._transform) and \
+            all(self_fig.coincides(other_fig) for self_fig, other_fig in zip(self.figures, other.figures))
+
+    # Checks if every corresponding subfigure between self and other
+    # have matching shapes. See Spline.matchesShape() for more info.
+    def matchesShape(self, other):
+        return len(self.figures) == len(other.figures) and \
+            all(self_fig.matchesShape(other_fig) for self_fig, other_fig in zip(self.figures, other.figures))
+
 
     ### TWEEN METHODS ###
 
     tweenLinear = MultiFigure.Multi(Spline.tweenLinear, MultiFigure.tweenLinear)
     tweenSpiral = MultiFigure.Multi(Spline.tweenSpiral, MultiFigure.tweenSpiral)
 
     @classmethod
@@ -1756,14 +1810,43 @@
 
 Multispline = MultiSpline  # Alias
 
 # Assign MultiSpline as the dedicated multifigure version of Spline.
 Spline._multitype = MultiSpline
 
 
+# 3D version of MultiSpline meant to enable 2D MultiSplines to be
+# positionable and orientable in 3D space. Its main use case is
+# for rendering 3D LaTeX expressions via morpho.latex.parse3d().
+#
+# Note that this is NOT a full SpaceMultiSpline class, which would
+# be a MultiFigure of SpaceSplines! Rather, this is just a regular
+# 2D MultiSpline which can be rendered in a 3D space like SpaceImage
+# can.
+#
+# The main differences from 2D MultiSplines is three new attributes:
+# pos = 3D position as an np.array. Default: [0,0,0] (the origin)
+# orient = Orientation in 3D space as a 3x3 rotation matrix.
+#       Default: np.eye(3) (oriented on the xy-plane facing the
+#       +z direction)
+# orientable = Boolean denoting whether the MultiSpline should be
+#       treated as an orientable 3D object, or more like a
+#       2D "sticker" object. Default: False
+#
+# Note that `pos` is not merely an alias for `origin` like it is
+# for 2D MultiSplines. Here they are distinct: `pos` controls 3D
+# position, whereas `origin` controls 2D position within the
+# MultiSpline's local plane.
+class MultiSpline3D(morpho.grid.MultiPath3D, MultiSpline):
+
+    ### TWEEN METHODS ###
+
+    tweenLinear = MultiSpline.tweenLinear
+
+
 # Space version of Spline figure. See "Spline" for more info.
 class SpaceSpline(Spline):
     def __init__(self, data=None, width=3, color=(1,1,1), alpha=1):
 
         # Use normal Spline constructor to start
         super().__init__(data=None, width=width, color=color, alpha=alpha)
 
@@ -2636,26 +2719,34 @@
         if self.strokeWeight < 0.5:  # Don't stroke if strokeWeight is too small
             ctx.new_path()
         else:
             ctx.set_source_rgba(*self.color, self.alphaEdge*self.alpha)
             ctx.set_line_width(self.strokeWeight)
             ctx.stroke()
 
+    # Converts the figure into an equivalent Path figure.
+    # Optionally specify the angular steps (in rads).
+    # Default: 2pi/72 (5 degrees)
+    # NOTE: Arc center will be assigned using the `origin`
+    # transformation attribute.
+    # You will need to call commitTransforms() on the resulting
+    # Path if you want the vertex list to perfectly reflect
+    # points on the arc in true space.
     def toPath(self, dTheta=tau/72):
-        raise NotImplementedError
+        return self.toPolygon(dTheta).toPath()
 
-    # Converts the figure into an equivalent polygon figure
+    # Converts the figure into an equivalent Polygon figure.
     # Optionally specify the angular steps (in rads).
     # Default: 2pi/72 (5 degrees)
-    # NOTE: Arc center will be assigned using Polygon.origin.
+    # NOTE: Arc center will be assigned using the `origin`
+    # transformation attribute.
     # You will need to call commitTransforms() on the resulting
-    # path figure if you want the vertex list to perfectly reflect
+    # Polygon if you want the vertex list to perfectly reflect
     # points on the arc in true space.
     def toPolygon(self, dTheta=tau/72):
-
         theta0, theta1 = self.theta0, self.theta1
         # If angular span is greater than tau,
         # just draw a circle
         if abs(theta1 - theta0) >= tau:
             theta1 = theta0 + tau
         # Ensure theta0 <= theta1
         elif theta1 < theta0:
```

### Comparing `morpholib-0.7.0.dev1/src/morpholib/text.py` & `morpholib-0.7.1.dev1/src/morpholib/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -948,17 +948,17 @@
     # The resulting MultiSpline will have its global origin set to the
     # position of the MultiPText's first component text figure's
     # position. All subsplines will have origin = 0.
     def toSpline(self):
         multisplines = [ptxt.toSpline().commitTransforms() for ptxt in self.figures]
         finalspline = morpho.shapes.MultiSpline(morpho.flattenList([multispline.figures for multispline in multisplines]))
         for spline in finalspline.figures:
-            spline.origin -= self.pos
+            spline.origin -= self.figures[0].pos
             spline.commitTransforms()
-        finalspline.origin = self.pos
+        finalspline.origin = self.figures[0].pos
         return finalspline
 
 MultiPtext = MultiPText
 
 
 # 3D version of the Text class.
 #
@@ -1005,15 +1005,15 @@
                 align=align
                 )
 
             if pos is None:
                 pos = np.zeros(3)
 
         # Redefine pos tweenable to be 3D.
-        _pos = morpho.Tweenable("_pos", morpho.matrix.array(pos), tags=["nparray", "fimage"])
+        _pos = morpho.Tweenable("_pos", morpho.matrix.array(pos), tags=["nparray", "fimage", "3d"])
         self._state.pop("pos")
         self._state["_pos"] = _pos
         _orient = morpho.Tweenable("_orient", np.identity(3), tags=["nparray", "orient"])
         self._state["_orient"] = _orient
 
         # self.orientable = False
         self.NonTweenable("orientable", False)
@@ -1075,18 +1075,19 @@
         orient = camera.orient
         focus = camera.focus
 
         if np.allclose(focus, 0):
             pos3d = orient @ self.pos
         else:
             pos3d = orient @ (self.pos - focus) + focus
+        pos3d = pos3d.tolist()
 
         txt = self._baseFigure()
         txt.text = self.text
-        txt.pos = (pos3d[0] + 1j*pos3d[1]).tolist()
+        txt.pos = pos3d[0] + 1j*pos3d[1]
         txt.zdepth = pos3d[2]
         txt.size = self.size
         txt.transform = self.transform
         if self.orientable:
             txt.transform = (orient @ self.orient)[:2,:2] @ txt.transform
         txt.color = self.color
         txt.alpha = self.alpha
@@ -1100,14 +1101,16 @@
         txt.prescale_x = self.prescale_x
         txt.prescale_y = self.prescale_y
 
         txt.font = self.font
         txt.bold = self.bold
         txt.italic = self.italic
 
+        txt._updateSettings(self)
+
         return [txt]
 
 
     def draw(self, camera, ctx): #, orient=np.identity(3), focus=np.zeros(3)):
         primlist = self.primitives(camera)
         if len(primlist) == 0:
             return
@@ -1680,15 +1683,15 @@
         if isinstance(text, FancyMultiText):
             super().__init__()
             self._updateFrom(text)
         else:
             super().__init__(text, *args, **kwargs)
 
         # Redefine pos tweenable to be 3D.
-        self.Tweenable("_pos", morpho.matrix.array(self.pos), tags=["nparray", "fimage"])
+        self.Tweenable("_pos", morpho.matrix.array(self.pos), tags=["nparray", "fimage", "3d"])
         self._state.pop("pos")
         self.Tweenable("_orient", np.identity(3), tags=["nparray", "orient"])
 
     @property
     def pos(self):
         return self._pos
 
@@ -1760,14 +1763,20 @@
 # Physical version of SpaceParagraph.
 # Mainly for internal use by paragraph3dPhys().
 # See SpaceParagraph and PText for more info.
 class SpaceParagraphPhys(SpaceParagraph):
     _baseMultiFigure = FancyMultiPText
 
 
+# Returns an invisible Text figure of a pair of periods.
+# A rough way to provide a one-off space between two clauses
+# in a paragraph figure.
+def space(**kwargs):
+    return Text("..", alpha=0).set(**kwargs)
+
 # Takes a collection of Text figures and returns a FancyMultiText
 # figure that concatenates all the individual Text figures.
 #
 # This function has been mostly obsoleted by the paragraph()
 # function. You should probably use that one instead.
 #
 # NOTE: This function makes copies of the individual Text figures
```

### Comparing `morpholib-0.7.0.dev1/src/morpholib/tools/basics.py` & `morpholib-0.7.1.dev1/src/morpholib/tools/basics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import morpholib as morpho
+
 import math, cmath
 import numpy as np
 from bisect import bisect_right, bisect_left
 
 ### CONSTANTS ###
 pi = math.pi
 tau = 2*pi
@@ -33,15 +35,18 @@
 # a numpy array.
 def isequal(a, b):
     if isinstance(a, np.ndarray) and isinstance(b, np.ndarray):
         return np.array_equal(a,b)
     elif isinstance(a, np.ndarray) != isinstance(b, np.ndarray):
         return False
     else:
-        return (a == b)
+        try:
+            return (a == b)
+        except ValueError:
+            return np.array_equal(a,b)
 
 # Conversion factors between degrees and radians.
 deg = tau/360
 rad = 1/deg
 
 # Real cotangent function
 PI_OVER_2 = pi/2
@@ -68,14 +73,21 @@
 
 # Computes the mean of a vector-like thing.
 def mean(a):
     if len(a) == 0:
         raise IndexError("Can't take mean of an empty list-like object!")
     return sum(a)/len(a)
 
+# Rounds a float x to an int if the float is sufficiently
+# close to an int. By default, it rounds if x is within
+# 1e-9 of an int.
+def snapround(x, tol=1e-9):
+    n = round(x)
+    return n if abs(n-x) < tol else x
+
 # Like round(), but truncates instead of rounding at the decimal digit you
 # specify
 def truncate(num, ndigits):
     decshift = 10**ndigits
     return int(num*decshift)/decshift
 
 def _rounder(x, roundfunc):
@@ -298,58 +310,80 @@
 # Usage: padbox(box, pad) -> paddedBox
 # where `box` is a 4-tuple defining the bounding box in the format
 #       [xmin, xmax, ymin, ymax]
 # Optionally, a ypad value can be specified, allowing the box to be
 # padded differently vertically vs horizontally:
 #       padbox(box, xpad, ypad) -> paddedBox
 def padbox(box, xpad, ypad=None, /):
+    # Typecast Actors/Figures to box
+    if isinstance(box, morpho.Actor):
+        box = box.last().box()
+    elif isinstance(box, morpho.Figure):
+        box = box.box()
+
     if ypad is None:
         ypad = xpad
 
     box = list(box)
     box[0] -= xpad
     box[1] += xpad
     box[2] -= ypad
     box[3] += ypad
 
     return box
+padBox = padbox  # Alias
 
 # Shifts a bounding box of the form [xmin,xmax,ymin,ymax]
 # by the given 2d vector `shift` expressed as a complex number.
 # Returns the modified box.
 def shiftBox(box, shift):
+    # Typecast Actors/Figures to box
+    if isinstance(box, morpho.Actor):
+        box = box.last().box()
+    elif isinstance(box, morpho.Figure):
+        box = box.box()
+
     left, right, bottom, top = box
     # Adjust by origin
     left += shift.real
     right += shift.real
     bottom += shift.imag
     top += shift.imag
     return [left, right, bottom, top]
 
 # Computes the total bounding box of a list of boxes.
-def totalBox(boxes):
+def totalBox(boxes, pad=0):
     XMIN, YMIN, XMAX, YMAX = oo, oo, -oo, -oo
     for box in boxes:
+        if isinstance(box, morpho.Actor):
+            box = box.last().box()
+        elif isinstance(box, morpho.Figure):
+            box = box.box()
         xmin, xmax, ymin, ymax = box
         XMIN = min(XMIN, xmin)
         YMIN = min(YMIN, ymin)
         XMAX = max(XMAX, xmax)
         YMAX = max(YMAX, ymax)
 
     bigbox = [XMIN, XMAX, YMIN, YMAX]
     if isbadarray(bigbox):
         raise ValueError("Total box is unbounded or undefined.")
 
-    return bigbox
+    return padbox(bigbox, pad)
 
 # Converts minutes with seconds into just seconds.
 # minsec(m,s) --> 60*m + s
 #
 # If given only a single decimal number as input, it treats
 # it as (minutes).(seconds) and converts it to seconds.
 # Example: minsec(2.05) --> 125 (within rounding error)
 def minsec(mins, secs=None, /):
     if secs is None:
         value = mins
         mins = int(value)
         secs = (value-mins)/0.6 * 60
     return 60*mins + secs
+
+# Allows one to easily define a Python slice object
+# using slice syntax.
+# Example: sel[1:3] --> slice(1,3)
+sel = np.s_
```

### Comparing `morpholib-0.7.0.dev1/src/morpholib/tools/dev.py` & `morpholib-0.7.1.dev1/src/morpholib/tools/dev.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import morpholib as morpho
 import morpholib.anim
 from morpholib.tools.basics import *
 
 import numpy as np
 import math, cmath
+from collections.abc import Iterable
 
 # Decorator allows a method to extract the needed
 # `view` and `ctx` parameters from Layer/Camera/Animation
 # inputs allowing for syntax like
 #   mytext.width(my_layer_or_camera, my_animation)
 # whereby `view` will be taken as the latest viewbox in the
 # layer and `windowShape` will be taken from the corresponding
@@ -152,35 +153,52 @@
     def anchorPoint(self, align, *args, **kwargs):
         anchor_x, anchor_y = align
         left, right, bottom, top = self.box(*args, **kwargs)
         x = morpho.lerp(left, right, anchor_x, start=-1, end=1)
         y = morpho.lerp(bottom, top, anchor_y, start=-1, end=1)
         return complex(x,y)
 
+    # Converts a complex number position into box coordinates
+    # where the bounds of the box are -1,1.
+    # Essentially the inverse of anchorPoint().
+    def boxCoords(self, pos, *args, **kwargs):
+        x,y = pos.real, pos.imag
+        left, right, bottom, top = self.box(*args, **kwargs)
+
+        anchor_x = morpho.lerp(-1, 1, x, start=left, end=right)
+        anchor_y = morpho.lerp(-1, 1, y, start=bottom, end=top)
+        return (anchor_x, anchor_y)
+
     def boxWidth(self, *args, **kwargs):
         box = self.box(*args, **kwargs)
         return box[1] - box[0]
 
     def boxHeight(self, *args, **kwargs):
         box = self.box(*args, **kwargs)
         return box[-1] - box[-2]
 
     # Only works for BoundingBoxFigures that have
     # background box tweenables `background`,
     # `backAlpha`, and `backPad` defined and the general
     # `alpha` tweenable, along with a box() method that
     # accepts the `raw` kwarg.
-    def _drawBackgroundBox(self, camera, ctx, origin=0, rotation=0, transform=np.eye(2)):
+    #
+    # Optionally, a kwarg `_alpha` can be passed in which
+    # will bypass accessing the top-level `alpha` attribute
+    # of self.
+    def _drawBackgroundBox(self, camera, ctx, origin=0, rotation=0, transform=np.eye(2), *,
+        _alpha=None):
         if self.backAlpha > 0:
+            alpha = self.alpha if _alpha is None else _alpha
             # Draw background box
             brect = morpho.grid.rect(padbox(self.box(raw=True), self.backPad))
             brect.set(
                 origin=origin, rotation=rotation,
                 _transform=transform,
-                width=0, fill=self.background, alpha=self.backAlpha*self.alpha
+                width=0, fill=self.background, alpha=self.backAlpha*alpha
                 )
             brect.draw(camera, ctx)
 
 # Draw a figure whose start or end attribute is outside the interval
 # [0,1] according to the cyclic rules.
 def drawOutOfBoundsStartEnd(fig, camera, ctx):
     diff = fig.end - fig.start
@@ -251,7 +269,60 @@
 
 def translateArrayUnderTransforms(array, shift, rotator, transformer):
     try:
         array += (transformer.inv*shift)/rotator
     except np.linalg.LinAlgError:
         raise ValueError("transform is singular.")
     return array
+
+# Duplicates specific items in a list as uniformly as possible.
+# Given a list, a sorted list (`slots`) of indices, and the number
+# of duplicates to create, the function inserts duplicates of the
+# items identified by `slots` in the same position in the list as
+# the original items. For example,
+#   makesubcopies([10,20,30,40,50], [0,2,3], 5)
+# produces [10,10,10, 20, 30,30,30, 40,40, 50]
+#
+# Optionally, an additional argument `itemfunc` can be supplied
+# which is applied to the original list item before it is
+# inserted as a duplicate back into the list. For example,
+# supplying `lambda item: item.copy()` will cause each item
+# to have its `copy()` method called before being inserted into
+# the list as a duplicate, in order to produce a deep copy
+# of the duplicated item.
+def makesubcopies(lst, slots, number, itemfunc=lambda item: item):
+    copiesPerSlot, remainder = divmod(number, len(slots))
+    for i, index in enumerate(reversed(slots)):
+        item = lst[index]
+        i = len(slots) - 1 - i
+        for n in range(copiesPerSlot+int(i < remainder)):
+            lst.insert(index, itemfunc(item))
+    return lst
+
+
+# Returns a dictionary mapping indices to items representing a
+# selection of items in a list. The `index` parameter can either
+# be an index, a slice, a choice function, or a combination of
+# these expressed as a tuple/iterable.
+#
+# One of the main features of this function is it won't return
+# duplicates when the indices in a multi-selection overlap.
+# And by using dicts, it is hopefully still a very speedy
+# function.
+def listselect(lst, index, /):
+    if callable(index):
+        condition = index
+        return dict((i,item) for i,item in enumerate(lst) if condition(item))
+    # Handle case of multiple index ranges provided
+    elif isinstance(index, Iterable):
+        pieces = index
+        selection = dict()
+        for piece in pieces:
+            selection.update(listselect(lst, piece))
+        return selection
+    else:
+        # Turn index into a slice if it's just a single int
+        if isinstance(index, int):
+            if index < 0:
+                index = index % len(lst)
+            index = sel[index:index+1]
+        return dict(zip(range(len(lst))[index], lst[index]))
```

### Comparing `morpholib-0.7.0.dev1/src/morpholib/tools/ktimer.py` & `morpholib-0.7.1.dev1/src/morpholib/tools/ktimer.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.0.dev1/src/morpholib/tools/latex2svg.py` & `morpholib-0.7.1.dev1/src/morpholib/tools/latex2svg.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.0.dev1/src/morpholib/tools/subimporter.py` & `morpholib-0.7.1.dev1/src/morpholib/tools/subimporter.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.0.dev1/src/morpholib/transitions.py` & `morpholib-0.7.1.dev1/src/morpholib/transitions.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,14 +85,24 @@
             return m*t**2/(2*a)
         elif t <= b:
             return m*(t-a/2)
         else:
             return 0.5*m*(b-a+1 - (t-1)**2/(1-b))
     return glideTransition
 
+# Equivalent to glide(), but the second inflection is specified
+# in terms of how far away it is from 1.
+# e.g. The following are equivalent:
+#   coast(a, b)
+#   glide(a, 1-b)
+def coast(a, b=None, /):
+    if b is not None:
+        b = 1-b
+    return glide(a,b)
+
 
 halfpi = math.pi/2
 # sinetoss = lambda t: math.sin(halfpi*t)
 # sinedrop = lambda t: 1 - math.cos(halfpi*t)
 # sineease = sinease = lambda t: (1-math.cos(math.pi*t))/2
 
 # Trig versions of toss/drop and ease.
```

### Comparing `morpholib-0.7.0.dev1/src/morpholib/video.py` & `morpholib-0.7.1.dev1/src/morpholib/video.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.0.dev1/src/morpholib.egg-info/PKG-INFO` & `morpholib-0.7.1.dev1/src/morpholib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morpholib
-Version: 0.7.0.dev1
+Version: 0.7.1.dev1
 Summary: A general-purpose programmatic animation tool
 Home-page: https://github.com/morpho-matters/morpholib
 Author: Kenneth Small
 Author-email: morpho.matters@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -51,14 +51,16 @@
 
 If you want to export animations as MP4s or small-sized GIFs, you will need to install [FFmpeg](https://ffmpeg.org/) for MP4 and/or [Gifsicle](https://www.lcdf.org/gifsicle/) for GIF. But if that doesn't matter to you (or if you just want to try out Morpho), you can still preview animations and export them as PNG sequences and large-sized GIFs just using the base installation of Morpho.
 
 Please note that FFmpeg and Gifsicle will need to be added to your PATH environment variable for Morpho to be able to access them by default.
 
 For Morpho to be able to parse LaTeX code, you must have a LaTeX distribution installed along with [dvisvgm](https://dvisvgm.de/). But if you're okay with not using Morpho's LaTeX features, this requirement is optional.
 
+SciPy is an optional, but recommended, dependency that is necessary currently for only few features (`flowStreamer` and `FlowField`). SciPy can be installed via pip with the command `pip install scipy`
+
 ### Testing the installation
 
 To see if it installed correctly, try running the following Python code:
 
 ```python
 import morpholib as morpho
 morpho.importAll()
```

### Comparing `morpholib-0.7.0.dev1/src/morpholib.egg-info/SOURCES.txt` & `morpholib-0.7.1.dev1/src/morpholib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

