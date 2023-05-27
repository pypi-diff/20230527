# Comparing `tmp/sect-7.0.0.tar.gz` & `tmp/sect-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sect-7.0.0.tar", last modified: Mon May 15 00:36:00 2023, max compression
+gzip compressed data, was "sect-7.1.0.tar", last modified: Sat May 27 04:22:29 2023, max compression
```

## Comparing `sect-7.0.0.tar` & `sect-7.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:36:00.302933 sect-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-15 00:35:47.000000 sect-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 00:35:47.000000 sect-7.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-15 00:36:00.298933 sect-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-05-15 00:35:47.000000 sect-7.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-15 00:35:47.000000 sect-7.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:36:00.298933 sect-7.0.0/sect/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-15 00:35:47.000000 sect-7.0.0/sect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:36:00.298933 sect-7.0.0/sect/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:36:00.298933 sect-7.0.0/sect/core/delaunay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/delaunay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/delaunay/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/delaunay/events_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/delaunay/hints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/delaunay/quad_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/delaunay/sweep_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    19304 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/delaunay/triangulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/delaunay/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/hints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:36:00.298933 sect-7.0.0/sect/core/trapezoidal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)    16525 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/hints.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/leaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/trapezoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/x_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/y_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-15 00:35:47.000000 sect-7.0.0/sect/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-15 00:35:47.000000 sect-7.0.0/sect/triangulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:36:00.298933 sect-7.0.0/sect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-15 00:36:00.000000 sect-7.0.0/sect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-15 00:36:00.000000 sect-7.0.0/sect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 00:36:00.000000 sect-7.0.0/sect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-15 00:36:00.000000 sect-7.0.0/sect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-15 00:36:00.000000 sect-7.0.0/sect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 00:36:00.302933 sect-7.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-15 00:35:47.000000 sect-7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:22:29.558150 sect-7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-27 04:22:19.000000 sect-7.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 04:22:19.000000 sect-7.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-27 04:22:29.558150 sect-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-05-27 04:22:19.000000 sect-7.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-27 04:22:19.000000 sect-7.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:22:29.554150 sect-7.1.0/sect/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-27 04:22:19.000000 sect-7.1.0/sect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:22:29.554150 sect-7.1.0/sect/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:22:29.554150 sect-7.1.0/sect/core/delaunay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/delaunay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/delaunay/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/delaunay/events_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/delaunay/hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/delaunay/quad_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/delaunay/sweep_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/delaunay/triangulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/delaunay/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/hints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:22:29.554150 sect-7.1.0/sect/core/trapezoidal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/trapezoidal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/trapezoidal/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16914 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/trapezoidal/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/trapezoidal/hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/trapezoidal/leaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/trapezoidal/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/trapezoidal/trapezoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/trapezoidal/x_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/trapezoidal/y_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-27 04:22:19.000000 sect-7.1.0/sect/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-27 04:22:19.000000 sect-7.1.0/sect/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-27 04:22:19.000000 sect-7.1.0/sect/triangulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:22:29.554150 sect-7.1.0/sect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-27 04:22:29.000000 sect-7.1.0/sect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-27 04:22:29.000000 sect-7.1.0/sect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 04:22:29.000000 sect-7.1.0/sect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-27 04:22:29.000000 sect-7.1.0/sect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-27 04:22:29.000000 sect-7.1.0/sect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 04:22:29.558150 sect-7.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-27 04:22:19.000000 sect-7.1.0/setup.py
```

### Comparing `sect-7.0.0/LICENSE` & `sect-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sect-7.0.0/PKG-INFO` & `sect-7.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sect
-Version: 7.0.0
+Version: 7.1.0
 Summary: Geometries partitioning.
 Home-page: https://github.com/lycantropos/sect/
 Download-URL: https://github.com/lycantropos/sect/archive/master.zip
 Author-email: Azat Ibrakov <azatibrakov@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Azat Ibrakov
```

### Comparing `sect-7.0.0/README.md` & `sect-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sect-7.0.0/pyproject.toml` & `sect-7.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,12 @@
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.coverage.run]
 source = ["sect"]
 
-[tool.mypy]
-strict = true
-
 [tool.pytest.ini_options]
 addopts = "--verbose -s --hypothesis-profile=default"
 
 [tool.setuptools.dynamic]
 version = { attr = "sect.__version__" }
```

### Comparing `sect-7.0.0/sect/core/delaunay/event.py` & `sect-7.1.0/sect/core/delaunay/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from abc import (ABC,
                  abstractmethod)
 from reprlib import recursive_repr
 from typing import Optional
 
 from ground.hints import Point
 from reprit.base import generate_repr
@@ -34,34 +36,35 @@
         """Checks if event is from left."""
 
 
 class LeftEvent(Event):
     is_left = True
 
     @classmethod
-    def from_segment_endpoints(cls,
-                               endpoints: SegmentEndpoints,
-                               from_first: bool,
-                               is_counterclockwise_contour: bool
-                               ) -> 'LeftEvent':
+    def from_segment_endpoints(
+            cls,
+            endpoints: SegmentEndpoints,
+            from_first: bool,
+            is_counterclockwise_contour: bool
+    ) -> LeftEvent:
         start, end = endpoints
         interior_to_left = is_counterclockwise_contour
         if start > end:
             start, end = end, start
             interior_to_left = not interior_to_left
         result = cls(start, None, from_first, interior_to_left)
         result.right = RightEvent(end, result)
         return result
 
     __slots__ = ('edge', 'interior_to_left', 'is_overlap',
                  'other_interior_to_left', 'right', '_from_first', '_start')
 
     def __init__(self,
                  start: Point,
-                 right: Optional['RightEvent'],
+                 right: Optional[RightEvent],
                  from_first: bool,
                  interior_to_left: bool,
                  edge: Optional[QuadEdge] = None) -> None:
         self.right, self._from_first, self._start = right, from_first, start
         self.interior_to_left = interior_to_left
         self.edge = edge
         self.is_overlap = self.other_interior_to_left = False
@@ -84,15 +87,15 @@
         """
         return self.other_interior_to_left and not self.is_overlap
 
     @property
     def start(self) -> Point:
         return self._start
 
-    def divide(self, point: Point) -> 'LeftEvent':
+    def divide(self, point: Point) -> LeftEvent:
         tail = self.right.left = LeftEvent(point, self.right, True,
                                            self.interior_to_left, self.edge)
         self.right = RightEvent(point, self)
         return tail
 
 
 class RightEvent(Event):
```

### Comparing `sect-7.0.0/sect/core/delaunay/events_queue.py` & `sect-7.1.0/sect/core/delaunay/events_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from functools import partial
 from typing import (Iterable,
                     Optional)
 
 from ground.base import (Context,
                          Orientation,
                          Relation)
@@ -22,15 +24,15 @@
     __slots__ = 'event', 'orienteer'
 
     def __init__(self, orienteer: Orienteer, event: Event) -> None:
         self.orienteer, self.event = orienteer, event
 
     __repr__ = generate_repr(__init__)
 
-    def __lt__(self, other: 'EventsQueueKey') -> bool:
+    def __lt__(self, other: EventsQueueKey) -> bool:
         event, other_event = self.event, other.event
         start, other_start = event.start, other_event.start
         if start.x != other_start.x:
             # different x-coordinate,
             # the event with lower x-coordinate is processed first
             return start.x < other_start.x
         elif start.y != other_start.y:
```

### Comparing `sect-7.0.0/sect/core/delaunay/quad_edge.py` & `sect-7.1.0/sect/core/delaunay/quad_edge.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import (Iterable,
                     List,
                     Optional)
 
 from ground.base import (Context,
                          Orientation)
 from ground.hints import Point
@@ -15,17 +17,19 @@
 
     Reference:
         https://en.wikipedia.org/wiki/Quad-edge
         http://www.sccg.sk/~samuelcik/dgs/quad_edge.pdf
     """
 
     @classmethod
-    def from_endpoints(cls, start: Point, end: Point,
+    def from_endpoints(cls,
+                       start: Point,
+                       end: Point,
                        *,
-                       context: Context) -> 'QuadEdge':
+                       context: Context) -> QuadEdge:
         """Creates new edge from endpoints."""
         result, opposite = (cls(start,
                                 context=context),
                             cls(end,
                                 context=context))
         rotated, triple_rotated = (cls(context=context),
                                    cls(context=context))
@@ -47,50 +51,50 @@
     def end(self) -> Point:
         """
         aka "Dest" in L. Guibas and J. Stolfi notation.
         """
         return self.opposite.start
 
     @property
-    def left_from_end(self) -> 'QuadEdge':
+    def left_from_end(self) -> QuadEdge:
         """
         aka "Lnext" in L. Guibas and J. Stolfi notation.
         """
         return self.rotated.opposite.left_from_start.rotated
 
     @property
-    def left_from_start(self) -> 'QuadEdge':
+    def left_from_start(self) -> QuadEdge:
         """
         aka "Onext" in L. Guibas and J. Stolfi notation.
         """
         return self._left_from_start
 
     @property
-    def opposite(self) -> 'QuadEdge':
+    def opposite(self) -> QuadEdge:
         """
         aka "Sym" in L. Guibas and J. Stolfi notation.
         """
         return self.rotated.rotated
 
     @property
-    def right_from_end(self) -> 'QuadEdge':
+    def right_from_end(self) -> QuadEdge:
         """
         aka "Rprev" in L. Guibas and J. Stolfi notation.
         """
         return self.opposite.left_from_start
 
     @property
-    def right_from_start(self) -> 'QuadEdge':
+    def right_from_start(self) -> QuadEdge:
         """
         aka "Oprev" in L. Guibas and J. Stolfi notation.
         """
         return self.rotated.left_from_start.rotated
 
     @property
-    def rotated(self) -> 'QuadEdge':
+    def rotated(self) -> QuadEdge:
         """
         aka "Rot" in L. Guibas and J. Stolfi notation.
         """
         return self._rotated
 
     @property
     def start(self) -> Point:
@@ -99,24 +103,24 @@
         """
         return self._start
 
     __slots__ = '_context', '_left_from_start', '_rotated', '_start'
 
     def __init__(self,
                  start: Optional[Point] = None,
-                 left_from_start: Optional['QuadEdge'] = None,
-                 rotated: Optional['QuadEdge'] = None,
+                 left_from_start: Optional[QuadEdge] = None,
+                 rotated: Optional[QuadEdge] = None,
                  *,
                  context: Context) -> None:
         (self._context, self._left_from_start, self._rotated,
          self._start) = context, left_from_start, rotated, start
 
     __repr__ = generate_repr(from_endpoints)
 
-    def connect(self, other: 'QuadEdge') -> 'QuadEdge':
+    def connect(self, other: QuadEdge) -> QuadEdge:
         """Connects the edge with the other."""
         result = self.from_endpoints(self.end, other.start,
                                      context=self.context)
         result.splice(self.left_from_end)
         result.opposite.splice(other)
         return result
 
@@ -125,15 +129,15 @@
         self.splice(self.right_from_start)
         self.opposite.splice(self.opposite.right_from_start)
 
     def orientation_of(self, point: Point) -> Orientation:
         """Returns orientation of the point relative to the edge."""
         return self.context.angle_orientation(self.start, self.end, point)
 
-    def splice(self, other: 'QuadEdge') -> None:
+    def splice(self, other: QuadEdge) -> None:
         """Splices the edge with the other."""
         alpha = self.left_from_start.rotated
         beta = other.left_from_start.rotated
         self._left_from_start, other._left_from_start = (
             other.left_from_start, self.left_from_start
         )
         alpha._left_from_start, beta._left_from_start = (
```

### Comparing `sect-7.0.0/sect/core/delaunay/sweep_line.py` & `sect-7.1.0/sect/core/delaunay/sweep_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from functools import partial
 from typing import Optional
 
 from dendroid import red_black
 from ground.base import (Context,
                          Orientation)
 from reprit.base import generate_repr
@@ -45,15 +47,15 @@
     __slots__ = 'event', 'orienteer'
 
     def __init__(self, orienteer: Orienteer, event: LeftEvent) -> None:
         self.orienteer, self.event = orienteer, event
 
     __repr__ = generate_repr(__init__)
 
-    def __lt__(self, other: 'SweepLineKey') -> bool:
+    def __lt__(self, other: SweepLineKey) -> bool:
         """
         Checks if the segment (or at least the point) associated with event
         is lower than other's.
         """
         event, other_event = self.event, other.event
         if event is other_event:
             return False
```

### Comparing `sect-7.0.0/sect/core/delaunay/triangulation.py` & `sect-7.1.0/sect/core/delaunay/triangulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from collections import deque
 from functools import partial
 from itertools import (accumulate,
                        chain,
                        repeat)
 from typing import (Callable,
                     Dict,
@@ -44,15 +46,15 @@
 
     @classmethod
     def constrained_delaunay(cls,
                              polygon: Polygon,
                              *,
                              extra_constraints: Sequence[Segment] = (),
                              extra_points: Sequence[Point] = (),
-                             context: Context) -> 'Triangulation':
+                             context: Context) -> Triangulation:
         """
         Constructs constrained Delaunay triangulation of given polygon
         (with potentially extra points and constraints).
 
         Based on
 
         * divide-and-conquer algorithm by L. Guibas & J. Stolfi
@@ -119,15 +121,15 @@
         )
         return result
 
     @classmethod
     def delaunay(cls,
                  points: Sequence[Point],
                  *,
-                 context: Context) -> 'Triangulation':
+                 context: Context) -> Triangulation:
         """
         Constructs Delaunay triangulation of given points.
 
         Based on divide-and-conquer algorithm by L. Guibas & J. Stolfi.
 
         Time complexity:
             ``O(len(points) * log len(points))``
@@ -188,15 +190,15 @@
                                                        orienteer))
                 for vertices in vertices_sets
                 if vertices not in self._triangular_holes_vertices]
 
     @classmethod
     def _initialize_triangulation(cls,
                                   points: Sequence[Point],
-                                  context: Context) -> 'Triangulation':
+                                  context: Context) -> Triangulation:
         return base_cases[len(points)](cls, points, context)
 
 
 def bound(triangulation: Triangulation,
           border_edges: Sequence[Segment]) -> None:
     border_endpoints = {to_endpoints(edge) for edge in border_edges}
     non_boundary = {edge
@@ -441,16 +443,17 @@
 
 
 def to_unique_inner_edges(triangulation: Triangulation) -> Set[QuadEdge]:
     return (set(to_unique_edges(triangulation))
             .difference(to_boundary_edges(triangulation)))
 
 
-BaseCase = Callable[[Type[Triangulation], Sequence[Point], Context],
-                    Triangulation]
+BaseCase = Callable[
+    [Type[Triangulation], Sequence[Point], Context], Triangulation
+]
 base_cases = {}  # type: Dict[int, BaseCase]
 register_base_case = partial(partial, base_cases.setdefault)
 
 
 @register_base_case(2)
 def triangulate_two_points(cls: Type[Triangulation],
                            sorted_points: Sequence[Point],
```

### Comparing `sect-7.0.0/sect/core/delaunay/utils.py` & `sect-7.1.0/sect/core/delaunay/utils.py`

 * *Files identical despite different names*

### Comparing `sect-7.0.0/sect/core/trapezoidal/edge.py` & `sect-7.1.0/sect/core/trapezoidal/edge.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+from __future__ import annotations
+
 from ground.base import (Context,
                          Orientation)
 from ground.hints import Point
 from reprit.base import generate_repr
 
 
 class Edge:
     @classmethod
     def from_endpoints(cls,
                        left: Point,
                        right: Point,
                        interior_to_left: bool,
-                       context: Context) -> 'Edge':
+                       context: Context) -> Edge:
         """Constructs edge given its endpoints."""
         return cls(left, right, interior_to_left, context)
 
     __slots__ = 'context', 'interior_to_left', 'left', 'right'
 
     def __init__(self,
                  left: Point,
@@ -22,15 +24,15 @@
                  interior_to_left: bool,
                  context: Context) -> None:
         assert left < right, 'Incorrect endpoints order'
         self.context, self.interior_to_left, self.left, self.right = (
             context, interior_to_left, left, right
         )
 
-    def __lt__(self, other: 'Edge') -> bool:
+    def __lt__(self, other: Edge) -> bool:
         """Checks if the edge is lower than the other."""
         other_left_orientation = self.orientation_of(other.left)
         other_right_orientation = self.orientation_of(other.right)
         if other_left_orientation is other_right_orientation:
             return other_left_orientation is Orientation.COUNTERCLOCKWISE
         elif other_left_orientation is Orientation.COLLINEAR:
             return other_right_orientation is Orientation.COUNTERCLOCKWISE
```

### Comparing `sect-7.0.0/sect/core/trapezoidal/graph.py` & `sect-7.1.0/sect/core/trapezoidal/graph.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from __future__ import annotations
+
 import random
-from typing import List
+from typing import (List,
+                    Tuple)
 
 from ground.base import (Context,
                          Location,
                          Orientation)
 from ground.hints import (Box,
                           Multisegment,
                           Point,
@@ -25,15 +28,15 @@
     """Represents trapezoidal decomposition graph."""
 
     @classmethod
     def from_multisegment(cls,
                           multisegment: Multisegment,
                           *,
                           shuffler: Shuffler = random.shuffle,
-                          context: Context) -> 'Graph':
+                          context: Context) -> Graph:
         """
         Constructs trapezoidal decomposition graph of given multisegment.
 
         Based on incremental randomized algorithm by R. Seidel.
 
         Time complexity:
             ``O(segments_count * log segments_count)`` expected,
@@ -78,28 +81,29 @@
         True
         """
         edges = [
             Edge.from_endpoints(segment.start, segment.end, False, context)
             if segment.start < segment.end
             else Edge.from_endpoints(segment.end, segment.start, False,
                                      context)
-            for segment in multisegment.segments]
+            for segment in multisegment.segments
+        ]
         shuffler(edges)
         result = cls(box_to_node(context.segments_box(multisegment.segments),
                                  context))
         for edge in edges:
             add_edge(result, edge)
         return result
 
     @classmethod
     def from_polygon(cls,
                      polygon: Polygon,
                      *,
                      shuffler: Shuffler = random.shuffle,
-                     context: Context) -> 'Graph':
+                     context: Context) -> Graph:
         """
         Constructs trapezoidal decomposition graph of given polygon.
 
         Based on incremental randomized algorithm by R. Seidel.
 
         Time complexity:
             ``O(vertices_count * log vertices_count)`` expected,
@@ -159,24 +163,24 @@
         edges = [
             Edge.from_endpoints(start, end, is_border_positively_oriented,
                                 context)
             if start < end
             else Edge.from_endpoints(end, start,
                                      not is_border_positively_oriented,
                                      context)
-            for start, end in contour_to_edges_endpoints(border)]
+            for start, end in contour_to_edges_endpoints(border)
+        ]
         for hole in polygon.holes:
             is_hole_negatively_oriented = (
                     to_contour_orientation(hole, orienteer)
                     is Orientation.CLOCKWISE
             )
             edges.extend(
                     Edge.from_endpoints(start, end,
-                                        is_hole_negatively_oriented,
-                                        context)
+                                        is_hole_negatively_oriented, context)
                     if start < end
                     else
                     Edge.from_endpoints(end, start,
                                         not is_hole_negatively_oriented,
                                         context)
                     for start, end in contour_to_edges_endpoints(hole)
             )
@@ -229,163 +233,189 @@
             ``O(1)``
         """
         return self.root.locate(point)
 
 
 def add_edge(graph: Graph, edge: Edge) -> None:
     trapezoids = find_intersecting_trapezoids(graph, edge)
-    edge_left, edge_right = edge.left, edge.right
-    prev_trapezoid = prev_below = prev_above = None
-    for index, trapezoid in enumerate(trapezoids):
-        is_first, is_last = index == 0, index == len(trapezoids) - 1
-        have_left, have_right = (is_first and edge_left != trapezoid.left,
-                                 is_last and edge_right != trapezoid.right)
-        left = right = None
-        if is_first and is_last:
-            if have_left:
-                left = Trapezoid(trapezoid.left, edge_left, trapezoid.below,
-                                 trapezoid.above)
-            below = Trapezoid(edge_left, edge_right, trapezoid.below, edge)
-            above = Trapezoid(edge_left, edge_right, edge, trapezoid.above)
-            if have_right:
-                right = Trapezoid(edge_right, trapezoid.right, trapezoid.below,
-                                  trapezoid.above)
-            if have_left:
-                left.lower_left = trapezoid.lower_left
-                left.upper_left = trapezoid.upper_left
-                left.lower_right = below
-                left.upper_right = above
-            else:
-                below.lower_left = trapezoid.lower_left
-                above.upper_left = trapezoid.upper_left
-            if have_right:
-                right.lower_right = trapezoid.lower_right
-                right.upper_right = trapezoid.upper_right
-                below.lower_right = right
-                above.upper_right = right
-            else:
-                below.lower_right = trapezoid.lower_right
-                above.upper_right = trapezoid.upper_right
-        elif is_first:
-            # old trapezoid is the first of 2+ trapezoids
-            # that the segment intersects
-            if have_left:
-                left = Trapezoid(trapezoid.left, edge_left, trapezoid.below,
-                                 trapezoid.above)
-            below = Trapezoid(edge_left, trapezoid.right, trapezoid.below,
-                              edge)
-            above = Trapezoid(edge_left, trapezoid.right, edge,
-                              trapezoid.above)
-            # set pairs of trapezoid neighbours
-            if have_left:
-                left.lower_left = trapezoid.lower_left
-                left.upper_left = trapezoid.upper_left
-                left.lower_right = below
-                left.upper_right = above
-            else:
-                below.lower_left = trapezoid.lower_left
-                above.upper_left = trapezoid.upper_left
-            below.lower_right = trapezoid.lower_right
-            above.upper_right = trapezoid.upper_right
-        elif is_last:
-            # old trapezoid is the last of 2+ trapezoids
-            # that the segment intersects
-            if prev_below.below is trapezoid.below:
-                below = prev_below
-                below.right = edge_right
-            else:
-                below = Trapezoid(trapezoid.left, edge_right, trapezoid.below,
-                                  edge)
-            if prev_above.above is trapezoid.above:
-                above = prev_above
-                above.right = edge_right
-            else:
-                above = Trapezoid(trapezoid.left, edge_right, edge,
-                                  trapezoid.above)
-            if have_right:
-                right = Trapezoid(edge_right, trapezoid.right, trapezoid.below,
-                                  trapezoid.above)
-            # set pairs of trapezoid neighbours
-            if have_right:
-                right.lower_right = trapezoid.lower_right
-                right.upper_right = trapezoid.upper_right
-                below.lower_right = right
-                above.upper_right = right
-            else:
-                below.lower_right = trapezoid.lower_right
-                above.upper_right = trapezoid.upper_right
-            # connect to new trapezoids replacing old
-            if below is not prev_below:
-                below.upper_left = prev_below
-                below.lower_left = (
-                    prev_below
-                    if trapezoid.lower_left is prev_trapezoid
-                    else trapezoid.lower_left
-                )
-            if above is not prev_above:
-                above.lower_left = prev_above
-                above.upper_left = (
-                    prev_above
-                    if trapezoid.upper_left is prev_trapezoid
-                    else trapezoid.upper_left
-                )
-        else:
-            # middle trapezoid,
-            # old trapezoid is neither the first
-            # nor last of the 3+ trapezoids
-            # that the segment intersects
-            if prev_below.below is trapezoid.below:
-                below = prev_below
-                below.right = trapezoid.right
-            else:
-                below = Trapezoid(trapezoid.left, trapezoid.right,
-                                  trapezoid.below, edge)
-            if prev_above.above is trapezoid.above:
-                above = prev_above
-                above.right = trapezoid.right
-            else:
-                above = Trapezoid(trapezoid.left, trapezoid.right, edge,
-                                  trapezoid.above)
-            # connect to new trapezoids replacing prev_trapezoid
-            if below is not prev_below:
-                # below is new
-                below.upper_left = prev_below
-                below.lower_left = (
-                    prev_below
-                    if trapezoid.lower_left is prev_trapezoid
-                    else trapezoid.lower_left
-                )
-            if above is not prev_above:
-                # above is new
-                above.lower_left = prev_above
-                above.upper_left = (
-                    prev_above
-                    if trapezoid.upper_left is prev_trapezoid
-                    else trapezoid.upper_left
-                )
-            below.lower_right = trapezoid.lower_right
-            above.upper_right = trapezoid.upper_right
-        candidate = YNode(edge,
-                          below.node
-                          if below is prev_below
-                          else Leaf(below),
-                          above.node
-                          if above is prev_above
-                          else Leaf(above))
-        if have_right:
-            candidate = XNode(edge_right, candidate, Leaf(right))
-        if have_left:
-            candidate = XNode(edge_left, Leaf(left), candidate)
-        trapezoid_node = trapezoid.node
-        if trapezoid_node is graph.root:
-            graph.root = candidate
-        else:
-            trapezoid_node.replace_with(candidate)
-        # prepare for next loop
-        prev_trapezoid, prev_above, prev_below = trapezoid, above, below
+    first_trapezoid = trapezoids[0]
+    if len(trapezoids) == 1:
+        add_edge_to_single_trapezoid(graph, first_trapezoid, edge)
+    else:
+        assert graph.height > 0
+        prev_above, prev_below = add_edge_to_first_trapezoid(
+                graph, first_trapezoid, edge
+        )
+        # prepare for the loop
+        prev_trapezoid = first_trapezoid
+        for middle_trapezoid in trapezoids[1:-1]:
+            prev_above, prev_below = add_edge_to_middle_trapezoid(
+                    graph, middle_trapezoid, edge, prev_above, prev_below,
+                    prev_trapezoid
+            )
+            # prepare for next loop
+            prev_trapezoid = middle_trapezoid
+        add_edge_to_last_trapezoid(graph, trapezoids[-1], edge, prev_above,
+                                   prev_below, prev_trapezoid)
+
+
+def add_edge_to_first_trapezoid(graph: Graph,
+                                trapezoid: Trapezoid,
+                                edge: Edge) -> Tuple[Trapezoid, Trapezoid]:
+    above = Trapezoid(edge.left, trapezoid.right, edge, trapezoid.above)
+    below = Trapezoid(edge.left, trapezoid.right, trapezoid.below, edge)
+    replacement_node = YNode(edge, Leaf(below), Leaf(above))
+    # set pairs of trapezoid neighbours
+    if edge.left == trapezoid.left:
+        above.upper_left = trapezoid.upper_left
+        below.lower_left = trapezoid.lower_left
+    else:
+        left = Trapezoid(trapezoid.left, edge.left, trapezoid.below,
+                         trapezoid.above)
+        left.lower_left = trapezoid.lower_left
+        left.upper_left = trapezoid.upper_left
+        left.lower_right = below
+        left.upper_right = above
+
+        replacement_node = XNode(edge.left, Leaf(left), replacement_node)
+    above.upper_right = trapezoid.upper_right
+    below.lower_right = trapezoid.lower_right
+    assert trapezoid.node is not graph.root
+    trapezoid.node.replace_with(replacement_node)
+    return above, below
+
+
+def add_edge_to_last_trapezoid(
+        graph: Graph,
+        trapezoid: Trapezoid,
+        edge: Edge,
+        prev_above: Trapezoid,
+        prev_below: Trapezoid,
+        prev_trapezoid: Trapezoid
+) -> Tuple[Trapezoid, Trapezoid]:
+    if prev_above.above is trapezoid.above:
+        above = prev_above
+        above.right = edge.right
+    else:
+        above = Trapezoid(trapezoid.left, edge.right, edge, trapezoid.above)
+        above.lower_left = prev_above
+        above.upper_left = (prev_above
+                            if trapezoid.upper_left is prev_trapezoid
+                            else trapezoid.upper_left)
+    if prev_below.below is trapezoid.below:
+        below = prev_below
+        below.right = edge.right
+    else:
+        below = Trapezoid(trapezoid.left, edge.right, trapezoid.below, edge)
+        below.upper_left = prev_below
+        below.lower_left = (prev_below
+                            if trapezoid.lower_left is prev_trapezoid
+                            else trapezoid.lower_left)
+    replacement_node = YNode(edge,
+                             below.node
+                             if below is prev_below
+                             else Leaf(below),
+                             above.node
+                             if above is prev_above
+                             else Leaf(above))
+    # set pairs of trapezoid neighbours
+    if edge.right == trapezoid.right:
+        above.upper_right = trapezoid.upper_right
+        below.lower_right = trapezoid.lower_right
+    else:
+        right = Trapezoid(edge.right, trapezoid.right, trapezoid.below,
+                          trapezoid.above)
+        right.lower_right = trapezoid.lower_right
+        right.upper_right = trapezoid.upper_right
+        above.upper_right = below.lower_right = right
+
+        replacement_node = XNode(edge.right, replacement_node, Leaf(right))
+    assert trapezoid.node is not graph.root
+    trapezoid.node.replace_with(replacement_node)
+
+
+def add_edge_to_middle_trapezoid(
+        graph: Graph,
+        trapezoid: Trapezoid,
+        edge: Edge,
+        prev_above: Trapezoid,
+        prev_below: Trapezoid,
+        prev_trapezoid: Trapezoid
+) -> Tuple[Trapezoid, Trapezoid]:
+    if prev_above.above is trapezoid.above:
+        above = prev_above
+        above.right = trapezoid.right
+    else:
+        above = Trapezoid(trapezoid.left, trapezoid.right, edge,
+                          trapezoid.above)
+        above.lower_left = prev_above
+        above.upper_left = (prev_above
+                            if trapezoid.upper_left is prev_trapezoid
+                            else trapezoid.upper_left)
+    if prev_below.below is trapezoid.below:
+        below = prev_below
+        below.right = trapezoid.right
+    else:
+        below = Trapezoid(trapezoid.left, trapezoid.right, trapezoid.below,
+                          edge)
+        below.upper_left = prev_below
+        below.lower_left = (prev_below
+                            if trapezoid.lower_left is prev_trapezoid
+                            else trapezoid.lower_left)
+    above.upper_right = trapezoid.upper_right
+    below.lower_right = trapezoid.lower_right
+    replacement_node = YNode(edge,
+                             below.node
+                             if below is prev_below
+                             else Leaf(below),
+                             above.node
+                             if above is prev_above
+                             else Leaf(above))
+    assert trapezoid.node is not graph.root
+    trapezoid.node.replace_with(replacement_node)
+    return above, below
+
+
+def add_edge_to_single_trapezoid(graph: Graph,
+                                 trapezoid: Trapezoid,
+                                 edge: Edge) -> None:
+    above = Trapezoid(edge.left, edge.right, edge, trapezoid.above)
+    below = Trapezoid(edge.left, edge.right, trapezoid.below, edge)
+
+    replacement_node = YNode(edge, Leaf(below), Leaf(above))
+    if edge.right == trapezoid.right:
+        below.lower_right = trapezoid.lower_right
+        above.upper_right = trapezoid.upper_right
+    else:
+        right = Trapezoid(edge.right, trapezoid.right, trapezoid.below,
+                          trapezoid.above)
+        right.lower_right = trapezoid.lower_right
+        right.upper_right = trapezoid.upper_right
+        below.lower_right = right
+        above.upper_right = right
+
+        replacement_node = XNode(edge.right, replacement_node, Leaf(right))
+    if edge.left == trapezoid.left:
+        below.lower_left = trapezoid.lower_left
+        above.upper_left = trapezoid.upper_left
+    else:
+        left = Trapezoid(trapezoid.left, edge.left, trapezoid.below,
+                         trapezoid.above)
+        left.lower_left = trapezoid.lower_left
+        left.upper_left = trapezoid.upper_left
+        left.lower_right = below
+        left.upper_right = above
+
+        replacement_node = XNode(edge.left, Leaf(left), replacement_node)
+    if trapezoid.node is graph.root:
+        assert graph.height == 0
+        graph.root = replacement_node
+    else:
+        assert graph.height > 0
+        trapezoid.node.replace_with(replacement_node)
 
 
 def box_to_node(box: Box, context: Context) -> Leaf:
     min_x, min_y, max_x, max_y = box.min_x, box.min_y, box.max_x, box.max_y
     delta_x, delta_y = max_x - min_x, max_y - min_y
     # handle horizontal/vertical cases
     delta_x, delta_y = delta_x or 1, delta_y or 1
@@ -407,13 +437,12 @@
     trapezoid = graph.root.search_edge(edge)
     result = [trapezoid]
     right = edge.right
     while trapezoid.right < right:
         trapezoid = ((trapezoid.upper_right or trapezoid.lower_right)
                      if (edge.orientation_of(trapezoid.right)
                          is Orientation.CLOCKWISE)
-                     else (
-                trapezoid.lower_right or trapezoid.upper_right))
+                     else (trapezoid.lower_right or trapezoid.upper_right))
         assert trapezoid is not None, ('Expected neighbour trapezoid, '
                                        'but none found.')
         result.append(trapezoid)
     return result
```

### Comparing `sect-7.0.0/sect/core/trapezoidal/leaf.py` & `sect-7.1.0/sect/core/trapezoidal/leaf.py`

 * *Files identical despite different names*

### Comparing `sect-7.0.0/sect/core/trapezoidal/node.py` & `sect-7.1.0/sect/core/trapezoidal/node.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from abc import (ABC,
                  abstractmethod)
 from typing import List
 
 from ground.base import Location
 from ground.hints import Point
 
@@ -9,15 +11,15 @@
 from .trapezoid import Trapezoid
 
 
 class Node(ABC):
     __slots__ = '_parents',
 
     def __init__(self) -> None:
-        self._parents = []  # type: List['Node']
+        self._parents: List[Node] = []
 
     @property
     @abstractmethod
     def height(self) -> int:
         """
         Returns height of the node.
         """
@@ -31,24 +33,24 @@
     @abstractmethod
     def search_edge(self, edge: Edge) -> Trapezoid:
         """
         Recursive search for the trapezoid
         which contains the left endpoint of the given segment.
         """
 
-    def replace_with(self, other: 'Node') -> None:
+    def replace_with(self, other: Node) -> None:
         """
         Replaces the node with given one in all parents.
         """
         for parent in self._parents:
             parent._replace_child(self, other)
             other._add_parent(parent)
         self._parents.clear()
 
-    def _add_parent(self, parent: 'Node') -> None:
+    def _add_parent(self, parent: Node) -> None:
         self._parents.append(parent)
 
     @abstractmethod
-    def _replace_child(self, current: 'Node', replacement: 'Node') -> None:
+    def _replace_child(self, current: Node, replacement: Node) -> None:
         """
         Replaces child node with given one.
         """
```

### Comparing `sect-7.0.0/sect/core/trapezoidal/trapezoid.py` & `sect-7.1.0/sect/core/trapezoidal/trapezoid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,80 @@
-from typing import (Optional, TYPE_CHECKING)
+from __future__ import annotations
+
+from typing import (TYPE_CHECKING,
+                    Optional)
 
 from ground.hints import Point
 from reprit.base import generate_repr
 
 if TYPE_CHECKING:
-    from .node import Node
     from .edge import Edge
+    from .node import Node
 
 
 class Trapezoid:
     __slots__ = ('left', 'right', 'below', 'above', 'node', '_lower_left',
                  '_lower_right', '_upper_left', '_upper_right')
 
     def __init__(self,
                  left: Point,
                  right: Point,
-                 below: 'Edge',
-                 above: 'Edge') -> None:
+                 below: Edge,
+                 above: Edge) -> None:
         assert left < right, 'Incorrect endpoints order'
-        self.left = left
-        self.right = right
-        self.above = above
-        self.below = below
-        self.node = None  # type: Optional[Node]
-        self._lower_left = None  # type: Optional[Trapezoid]
-        self._lower_right = None  # type: Optional[Trapezoid]
-        self._upper_left = None  # type: Optional[Trapezoid]
-        self._upper_right = None  # type: Optional[Trapezoid]
+        self.above, self.below, self.left, self.right = (
+            above, below, left, right
+        )
+        self.node: Optional[Node] = None
+        self._lower_left: Optional[Trapezoid] = None
+        self._lower_right: Optional[Trapezoid] = None
+        self._upper_left: Optional[Trapezoid] = None
+        self._upper_right: Optional[Trapezoid] = None
 
     __repr__ = generate_repr(__init__)
 
     @property
     def component(self) -> bool:
         """
         Checks if the trapezoid is a component of decomposed geometry.
         """
         return self.below.interior_to_left and not self.above.interior_to_left
 
     @property
-    def lower_left(self) -> Optional['Trapezoid']:
+    def lower_left(self) -> Optional[Trapezoid]:
         return self._lower_left
 
     @property
-    def lower_right(self) -> Optional['Trapezoid']:
+    def lower_right(self) -> Optional[Trapezoid]:
         return self._lower_right
 
     @property
-    def upper_left(self) -> Optional['Trapezoid']:
+    def upper_left(self) -> Optional[Trapezoid]:
         return self._upper_left
 
     @property
-    def upper_right(self) -> Optional['Trapezoid']:
+    def upper_right(self) -> Optional[Trapezoid]:
         return self._upper_right
 
     @lower_left.setter
-    def lower_left(self, value: Optional['Trapezoid']) -> None:
+    def lower_left(self, value: Optional[Trapezoid]) -> None:
         self._lower_left = value
         if value is not None:
             value._lower_right = self
 
     @lower_right.setter
-    def lower_right(self, value: Optional['Trapezoid']) -> None:
+    def lower_right(self, value: Optional[Trapezoid]) -> None:
         self._lower_right = value
         if value is not None:
             value._lower_left = self
 
     @upper_left.setter
-    def upper_left(self, value: Optional['Trapezoid']) -> None:
+    def upper_left(self, value: Optional[Trapezoid]) -> None:
         self._upper_left = value
         if value is not None:
             value._upper_right = self
 
     @upper_right.setter
-    def upper_right(self, value: Optional['Trapezoid']) -> None:
+    def upper_right(self, value: Optional[Trapezoid]) -> None:
         self._upper_right = value
         if value is not None:
             value._upper_left = self
```

### Comparing `sect-7.0.0/sect/core/trapezoidal/x_node.py` & `sect-7.1.0/sect/core/trapezoidal/x_node.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 
 from .edge import Edge
 from .node import Node
 from .trapezoid import Trapezoid
 
 
 class XNode(Node):
-    __slots__ = 'point', 'left', 'right'
+    __slots__ = 'left', 'point', 'right'
 
     def __init__(self, point: Point, left: Node, right: Node) -> None:
         super().__init__()
-        self.point = point
-        self.left = left
-        self.right = right
+        self.left, self.point, self.right = left, point, right
         self.left._add_parent(self)
         self.right._add_parent(self)
 
     __repr__ = generate_repr(__init__)
 
     @property
     def height(self) -> int:
```

### Comparing `sect-7.0.0/sect/core/trapezoidal/y_node.py` & `sect-7.1.0/sect/core/trapezoidal/y_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,23 +5,21 @@
 
 from .edge import Edge
 from .node import Node
 from .trapezoid import Trapezoid
 
 
 class YNode(Node):
-    __slots__ = 'edge', 'above', 'below'
+    __slots__ = 'above', 'below', 'edge'
 
     def __init__(self, edge: Edge, below: Node, above: Node) -> None:
         super().__init__()
-        self.edge = edge
-        self.below = below
-        self.above = above
-        self.below._add_parent(self)
+        self.above, self.below, self.edge = above, below, edge
         self.above._add_parent(self)
+        self.below._add_parent(self)
 
     __repr__ = generate_repr(__init__)
 
     @property
     def height(self) -> int:
         return max(self.below.height, self.above.height) + 1
```

### Comparing `sect-7.0.0/sect/core/utils.py` & `sect-7.1.0/sect/core/utils.py`

 * *Files identical despite different names*

### Comparing `sect-7.0.0/sect.egg-info/PKG-INFO` & `sect-7.1.0/sect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sect
-Version: 7.0.0
+Version: 7.1.0
 Summary: Geometries partitioning.
 Home-page: https://github.com/lycantropos/sect/
 Download-URL: https://github.com/lycantropos/sect/archive/master.zip
 Author-email: Azat Ibrakov <azatibrakov@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Azat Ibrakov
```

### Comparing `sect-7.0.0/sect.egg-info/SOURCES.txt` & `sect-7.1.0/sect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

