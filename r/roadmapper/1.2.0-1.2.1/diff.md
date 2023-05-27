# Comparing `tmp/roadmapper-1.2.0.tar.gz` & `tmp/roadmapper-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roadmapper-1.2.0.tar", last modified: Sun Apr 23 20:33:22 2023, max compression
+gzip compressed data, was "roadmapper-1.2.1.tar", last modified: Sat May 27 09:13:47 2023, max compression
```

## Comparing `roadmapper-1.2.0.tar` & `roadmapper-1.2.1.tar`

### file list

```diff
@@ -1,38 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:22.247319 roadmapper-1.2.0/
--rw-rw-rw-   0        0        0     1092 2023-01-07 22:57:29.000000 roadmapper-1.2.0/LICENSE.md
--rw-rw-rw-   0        0        0     4333 2023-04-23 20:33:22.247319 roadmapper-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3777 2023-04-23 20:25:06.000000 roadmapper-1.2.0/README.md
--rw-rw-rw-   0        0        0     1088 2023-01-31 06:22:36.000000 roadmapper-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 20:33:22.247319 roadmapper-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:22.215883 roadmapper-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:22.233887 roadmapper-1.2.0/src/roadmapper/
--rw-rw-rw-   0        0        0        0 2023-01-07 22:57:29.000000 roadmapper-1.2.0/src/roadmapper/__init__.py
--rw-rw-rw-   0        0        0    17086 2023-04-23 20:15:33.000000 roadmapper-1.2.0/src/roadmapper/colourtheme.py
--rw-rw-rw-   0        0        0     2888 2023-04-23 20:31:54.000000 roadmapper-1.2.0/src/roadmapper/footer.py
--rw-rw-rw-   0        0        0     6811 2023-04-23 20:32:10.000000 roadmapper-1.2.0/src/roadmapper/group.py
--rw-rw-rw-   0        0        0     4376 2023-04-23 20:32:17.000000 roadmapper-1.2.0/src/roadmapper/logo.py
--rw-rw-rw-   0        0        0     5253 2023-04-23 20:32:21.000000 roadmapper-1.2.0/src/roadmapper/marker.py
--rw-rw-rw-   0        0        0     3415 2023-04-23 20:32:23.000000 roadmapper-1.2.0/src/roadmapper/milestone.py
--rw-rw-rw-   0        0        0    19946 2023-04-23 20:32:26.000000 roadmapper-1.2.0/src/roadmapper/painter.py
--rw-rw-rw-   0        0        0    17902 2023-04-23 20:32:32.000000 roadmapper-1.2.0/src/roadmapper/roadmap.py
--rw-rw-rw-   0        0        0     2767 2023-04-23 20:32:35.000000 roadmapper-1.2.0/src/roadmapper/subtitle.py
--rw-rw-rw-   0        0        0    21541 2023-04-23 20:32:38.000000 roadmapper-1.2.0/src/roadmapper/task.py
--rw-rw-rw-   0        0        0    22043 2023-04-23 20:32:42.000000 roadmapper-1.2.0/src/roadmapper/timeline.py
--rw-rw-rw-   0        0        0    13397 2023-04-23 20:32:46.000000 roadmapper-1.2.0/src/roadmapper/timelineitem.py
--rw-rw-rw-   0        0        0     3846 2023-04-23 20:32:50.000000 roadmapper-1.2.0/src/roadmapper/timelineitemyear.py
--rw-rw-rw-   0        0        0     4655 2023-04-09 00:51:50.000000 roadmapper-1.2.0/src/roadmapper/timelinelocale.py
--rw-rw-rw-   0        0        0     1330 2023-04-09 00:51:50.000000 roadmapper-1.2.0/src/roadmapper/timelinemode.py
--rw-rw-rw-   0        0        0     2978 2023-04-23 20:33:00.000000 roadmapper-1.2.0/src/roadmapper/title.py
--rw-rw-rw-   0        0        0       24 2023-04-23 20:15:33.000000 roadmapper-1.2.0/src/roadmapper/version.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:22.241888 roadmapper-1.2.0/src/roadmapper.egg-info/
--rw-rw-rw-   0        0        0     4333 2023-04-23 20:33:22.000000 roadmapper-1.2.0/src/roadmapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-04-23 20:33:22.000000 roadmapper-1.2.0/src/roadmapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 20:33:22.000000 roadmapper-1.2.0/src/roadmapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-04-23 20:33:22.000000 roadmapper-1.2.0/src/roadmapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-04-23 20:33:22.000000 roadmapper-1.2.0/src/roadmapper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:22.245889 roadmapper-1.2.0/src/tests/
--rw-rw-rw-   0        0        0        0 2023-04-09 00:51:50.000000 roadmapper-1.2.0/src/tests/__init__.py
--rw-rw-rw-   0        0        0      925 2023-04-09 00:51:50.000000 roadmapper-1.2.0/src/tests/roadmap_draw_test.py
--rw-rw-rw-   0        0        0    42793 2023-04-23 20:15:33.000000 roadmapper-1.2.0/src/tests/test_cases.py
--rw-rw-rw-   0        0        0     3044 2023-04-23 20:15:33.000000 roadmapper-1.2.0/src/tests/test_painter.py
--rw-rw-rw-   0        0        0    13294 2023-04-23 20:15:33.000000 roadmapper-1.2.0/src/tests/test_roadmapper.py
+drwxrwxrwx   0        0        0        0 2023-05-27 09:13:47.670058 roadmapper-1.2.1/
+-rw-rw-rw-   0        0        0     1092 2023-01-07 22:57:29.000000 roadmapper-1.2.1/LICENSE.md
+-rw-rw-rw-   0        0        0     4337 2023-05-27 09:13:47.670058 roadmapper-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3781 2023-05-27 09:08:32.000000 roadmapper-1.2.1/README.md
+-rw-rw-rw-   0        0        0     1314 2023-05-27 09:13:34.000000 roadmapper-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 09:13:47.671059 roadmapper-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 09:13:47.624504 roadmapper-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 09:13:47.642562 roadmapper-1.2.1/src/roadmapper/
+-rw-rw-rw-   0        0        0        0 2023-01-07 22:57:29.000000 roadmapper-1.2.1/src/roadmapper/__init__.py
+-rw-rw-rw-   0        0        0    17086 2023-04-23 20:15:33.000000 roadmapper-1.2.1/src/roadmapper/colourtheme.py
+-rw-rw-rw-   0        0        0     2888 2023-04-23 20:31:54.000000 roadmapper-1.2.1/src/roadmapper/footer.py
+-rw-rw-rw-   0        0        0     6722 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/roadmapper/group.py
+-rw-rw-rw-   0        0        0     4376 2023-04-23 20:32:17.000000 roadmapper-1.2.1/src/roadmapper/logo.py
+-rw-rw-rw-   0        0        0     4833 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/roadmapper/marker.py
+-rw-rw-rw-   0        0        0     2732 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/roadmapper/milestone.py
+-rw-rw-rw-   0        0        0    20304 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/roadmapper/painter.py
+-rw-rw-rw-   0        0        0    17420 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/roadmapper/roadmap.py
+-rw-rw-rw-   0        0        0     2767 2023-04-23 20:32:35.000000 roadmapper-1.2.1/src/roadmapper/subtitle.py
+-rw-rw-rw-   0        0        0    20860 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/roadmapper/task.py
+-rw-rw-rw-   0        0        0    22043 2023-04-23 20:32:42.000000 roadmapper-1.2.1/src/roadmapper/timeline.py
+-rw-rw-rw-   0        0        0    13397 2023-04-23 20:32:46.000000 roadmapper-1.2.1/src/roadmapper/timelineitem.py
+-rw-rw-rw-   0        0        0     3846 2023-04-23 20:32:50.000000 roadmapper-1.2.1/src/roadmapper/timelineitemyear.py
+-rw-rw-rw-   0        0        0     4655 2023-04-09 00:51:50.000000 roadmapper-1.2.1/src/roadmapper/timelinelocale.py
+-rw-rw-rw-   0        0        0     1330 2023-04-09 00:51:50.000000 roadmapper-1.2.1/src/roadmapper/timelinemode.py
+-rw-rw-rw-   0        0        0     2978 2023-04-23 20:33:00.000000 roadmapper-1.2.1/src/roadmapper/title.py
+-rw-rw-rw-   0        0        0       24 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/roadmapper/version.py
+drwxrwxrwx   0        0        0        0 2023-05-27 09:13:47.658056 roadmapper-1.2.1/src/roadmapper.egg-info/
+-rw-rw-rw-   0        0        0     4337 2023-05-27 09:13:47.000000 roadmapper-1.2.1/src/roadmapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1139 2023-05-27 09:13:47.000000 roadmapper-1.2.1/src/roadmapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 09:13:47.000000 roadmapper-1.2.1/src/roadmapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-27 09:13:47.000000 roadmapper-1.2.1/src/roadmapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-05-27 09:13:47.000000 roadmapper-1.2.1/src/roadmapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 09:13:47.665057 roadmapper-1.2.1/src/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-09 00:51:50.000000 roadmapper-1.2.1/src/tests/__init__.py
+-rw-rw-rw-   0        0        0     2643 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/tests/compare_generated_roadmaps_test.py
+-rw-rw-rw-   0        0        0      141 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/tests/conftest.py
+-rw-rw-rw-   0        0        0     1056 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/tests/roadmap_draw_test.py
+drwxrwxrwx   0        0        0        0 2023-05-27 09:13:47.669058 roadmapper-1.2.1/src/tests/roadmap_generators/
+-rw-rw-rw-   0        0        0        0 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/tests/roadmap_generators/__init__.py
+-rw-rw-rw-   0        0        0     7122 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/tests/roadmap_generators/colour_theme_extensive.py
+-rw-rw-rw-   0        0        0      233 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/tests/roadmap_generators/roadmap_abc.py
+-rw-rw-rw-   0        0        0     1990 2023-05-27 08:40:54.000000 roadmapper-1.2.1/src/tests/roadmap_generators/roadmap_generator.py
+-rw-rw-rw-   0        0        0    43031 2023-05-27 08:49:41.000000 roadmapper-1.2.1/src/tests/test_cases.py
+-rw-rw-rw-   0        0        0      320 2023-05-26 11:31:22.000000 roadmapper-1.2.1/src/tests/test_generate_roadmap.py
+-rw-rw-rw-   0        0        0     3044 2023-04-23 20:15:33.000000 roadmapper-1.2.1/src/tests/test_painter.py
+-rw-rw-rw-   0        0        0    13290 2023-05-27 08:54:11.000000 roadmapper-1.2.1/src/tests/test_roadmapper.py
```

### Comparing `roadmapper-1.2.0/LICENSE.md` & `roadmapper-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.0/PKG-INFO` & `roadmapper-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadmapper
-Version: 1.2.0
+Version: 1.2.1
 Summary: Roadmapper. A Roadmap-as-Code (RaC) python library for generating a roadmap by using python code
 Author: CS Goh
 Project-URL: Homepage, https://github.com/csgoh/roadmapper
 Project-URL: Bug Tracker, https://github.com/csgoh/roadmapper/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,24 +32,24 @@
 With git repository like GitHub or Bitbucket, roadmaps created using RaC can be version controlled, track changes and can be easily shared with others.
 
 ### Latest version
 ![release](https://img.shields.io/pypi/v/roadmapper)
 
 :book: For usage documentation, how-to guide and code examples, refer to [Roadmapper Wiki](https://github.com/csgoh/roadmap-generator/wiki).
 
-View the [Change Logs](https://github.com/csgoh/processpiper/wiki/Change-Logs) to find out the latest updates and additions in the most recent version.
+View the [Change Logs](https://github.com/csgoh/roadmapper/wiki/Change-Logs) to find out the latest updates and additions in the most recent version.
 
 ![multilingual roadmappper](https://github.com/csgoh/roadmapper/blob/main/images/roadmapper-banner-multilingual.png?raw=true)
 
 ### Python version requirements:
 * Python 3.10+
   
 ### Library Dependencies
-* Pillow 9.4.0
-* python-dateutil
+* Pillow 9.5.0
+* python-dateutil 2.8.2
 
 Any feedback or suggestions are welcome. Please feel free to create an issue or pull request.
 <br/>
 <hr>
 
 
 ## Installation
```

### Comparing `roadmapper-1.2.0/README.md` & `roadmapper-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 With git repository like GitHub or Bitbucket, roadmaps created using RaC can be version controlled, track changes and can be easily shared with others.
 
 ### Latest version
 ![release](https://img.shields.io/pypi/v/roadmapper)
 
 :book: For usage documentation, how-to guide and code examples, refer to [Roadmapper Wiki](https://github.com/csgoh/roadmap-generator/wiki).
 
-View the [Change Logs](https://github.com/csgoh/processpiper/wiki/Change-Logs) to find out the latest updates and additions in the most recent version.
+View the [Change Logs](https://github.com/csgoh/roadmapper/wiki/Change-Logs) to find out the latest updates and additions in the most recent version.
 
 ![multilingual roadmappper](https://github.com/csgoh/roadmapper/blob/main/images/roadmapper-banner-multilingual.png?raw=true)
 
 ### Python version requirements:
 * Python 3.10+
   
 ### Library Dependencies
-* Pillow 9.4.0
-* python-dateutil
+* Pillow 9.5.0
+* python-dateutil 2.8.2
 
 Any feedback or suggestions are welcome. Please feel free to create an issue or pull request.
 <br/>
 <hr>
 
 
 ## Installation
```

### Comparing `roadmapper-1.2.0/pyproject.toml` & `roadmapper-1.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ['Pillow>=9.4.0', 'python-dateutil>=2.8.2']
+dependencies = ['Pillow>=9.5.0', 'python-dateutil>=2.8.2']
 
 [project.urls]
 "Homepage" = "https://github.com/csgoh/roadmapper"
 "Bug Tracker" = "https://github.com/csgoh/roadmapper/issues"
 
 [tool.setuptools.packages.find]
 where = ["src"] # list of folders that contain the packages (["."] by default)
@@ -28,7 +28,15 @@
     "test_cases",
     "tempCodeRunnerFile",
 ] # exclude packages matching these glob patterns (empty by default)
 
 [tool.setuptools.dynamic]
 version = { attr = "roadmapper.version.__version__" }
 readme = { file = ["README.md"] }
+
+[tool.pytest.ini_options]
+addopts = "-v"
+markers = [
+    "unit: Unit tests which are not dependent on environment",
+    "ubuntu: Test which only apply to Ubuntu environment",
+    "genimage: To generate test image",
+]
```

### Comparing `roadmapper-1.2.0/src/roadmapper/colourtheme.py` & `roadmapper-1.2.1/src/roadmapper/colourtheme.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.0/src/roadmapper/footer.py` & `roadmapper-1.2.1/src/roadmapper/footer.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.0/src/roadmapper/group.py` & `roadmapper-1.2.1/src/roadmapper/group.py`

 * *Files 16% similar despite different names*

```diff
@@ -76,26 +76,20 @@
             font_colour (str, optional): Task font colour. Defaults to "Black". HTML colour name or hex code. Eg. #FFFFFF or LightGreen
             fill_colour (str, optional): Task fill colour. Defaults to "LightGreen". HTML colour name or hex code
             text_alignment (str, optional): Task text alignment. Defaults to "centre". Options: "left", "centre", "right"
 
         Return:
             Task: Task instance to be used in with statement
         """
-
-        if font == "":
-            font = self.painter.task_font
-        if font_size == 0:
-            font_size = self.painter.task_font_size
-        if font_colour == "":
-            font_colour = self.painter.task_font_colour
-        if fill_colour == "":
-            fill_colour = self.painter.task_fill_colour
-
-        if style == "":
-            style = self.painter.task_style
+            
+        font = font or self.painter.task_font
+        font_size = font_size or self.painter.task_font_size
+        font_colour = font_colour or self.painter.task_font_colour
+        fill_colour = fill_colour or self.painter.task_fill_colour
+        style = style or self.painter.task_style
 
         task = Task(
             text=text,
             start=start,
             end=end,
             font=font,
             font_size=font_size,
```

### Comparing `roadmapper-1.2.0/src/roadmapper/logo.py` & `roadmapper-1.2.1/src/roadmapper/logo.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.0/src/roadmapper/marker.py` & `roadmapper-1.2.1/src/roadmapper/marker.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,27 +44,14 @@
     label_height: int = field(init=False, default=0)
     line_from_x: int = field(init=False, default=0)
     line_from_y: int = field(init=False, default=0)
     line_to_x: int = field(init=False, default=0)
     line_to_y: int = field(init=False, default=0)
     not_in_timeline_range: bool = field(init=False, default=False)
 
-    # def __post_init__(self):
-    #     """This method is called after __init__() is called"""
-    #     self.text = "▼"
-    #     self.label_x = 0
-    #     self.label_y = 0
-    #     self.label_width = 0
-    #     self.label_height = 0
-    #     self.line_from_x = 0
-    #     self.line_from_y = 0
-    #     self.line_to_x = 0
-    #     self.line_to_y = 0
-    #     self.not_in_timeline_range = False
-
     def set_label_draw_position(self, painter: Painter, timeline: Timeline) -> None:
         """Set marker label draw position
 
         Args:
             painter (Painter): Pillow wrapper class instance
             timeline (Timeline): Timeline instance
         """
```

### Comparing `roadmapper-1.2.0/src/roadmapper/milestone.py` & `roadmapper-1.2.1/src/roadmapper/milestone.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,38 +40,14 @@
     diamond_x: int = field(init=False, default=0)
     diamond_y: int = field(init=False, default=0)
     diamond_width: int = field(init=False, default=0)
     diamond_height: int = field(init=False, default=0)
     text_x: int = field(init=False, default=0)
     text_y: int = field(init=False, default=0)
 
-    # def __init__(
-    #     self,
-    #     text: str,
-    #     date: datetime,
-    #     font: str,
-    #     font_size: int,
-    #     font_colour: str,
-    #     fill_colour: str,
-    #     text_alignment: str,
-    # ) -> None:
-    #     self.text = text
-    #     self.date = date
-    #     self.font = font
-    #     self.font_size = font_size
-    #     self.font_colour = font_colour
-    #     self.fill_colour = fill_colour
-    #     self.text_alignment = text_alignment
-
-    #     self.diamond_x = 0
-    #     self.diamond_y = 0
-    #     self.diamond_width = 0
-    #     self.diamond_height = 0
-    #     self.text_x = 0
-    #     self.text_y = 0
 
     def draw(self, painter: Painter) -> None:
         """Draw milestone
 
         Args:
             painter (Painter): Pillow wrapper class instance
         """
```

### Comparing `roadmapper-1.2.0/src/roadmapper/painter.py` & `roadmapper-1.2.1/src/roadmapper/painter.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,34 +181,39 @@
             self.footer_font,
             self.footer_font_size,
             self.footer_font_colour,
         ) = self.colour_theme.get_colour_theme_settings("footer")
 
     def get_font_path(self, font_name: str) -> str:
         """Get the path to the font file"""
-        # Check if font_name contained ttf or otf extension
         if font_name.endswith(".ttf") or font_name.endswith(".otf"):
             return font_name
-        # Check if font_name contained ttf or otf extension
         if sys.platform.startswith("win"):  # Windows
             return os.path.join("C:\\", "Windows", "Fonts", f"{font_name}.ttf")
         elif sys.platform.startswith("darwin"):  # macOS
             return os.path.join(
                 "/", "System", "Library", "Fonts", "Supplemental", f"{font_name}.ttf"
             )
         elif sys.platform.startswith("linux"):  # Linux
-            return os.path.join(
-                "/",
-                "usr",
-                "share",
-                "fonts",
-                "truetype",
-                "msttcorefonts",
-                f"{font_name}.ttf",
-            )
+            font_dir = f"/usr/share/fonts/truetype/msttcorefonts"
+
+            if os.path.exists(os.path.join(font_dir, f"{font_name}.ttf")):
+                return os.path.join(font_dir, f"{font_name}.ttf")
+            else:
+                ### This is cater for cases where msttcorefonts is not installed
+                linux_font_name = "DejaVuSans"  # Default font for Linux
+                return os.path.join(
+                    "/",
+                    "usr",
+                    "share",
+                    "fonts",
+                    "truetype",
+                    "dejavu",  # Use the DejaVu font directory instead of msttcorefonts
+                    f"{linux_font_name}.ttf",
+                )
         else:
             raise Exception("Unsupported operating system")
 
     def draw_box(
         self, x: int, y: int, width: int, height: int, box_fill_colour: str
     ) -> None:
         """Draw a rectagle
```

### Comparing `roadmapper-1.2.0/src/roadmapper/roadmap.py` & `roadmapper-1.2.1/src/roadmapper/roadmap.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,22 +82,19 @@
             label_text_font (str, optional): Label text font. Defaults to "Arial".
             label_text_colour (str, optional): Label text colour. Defaults to "Black".
             label_text_size (int, optional): Label text size. Defaults to 10.
             line_colour (str, optional): Line colour. Defaults to "Black".
             line_width (int, optional): Line width. Defaults to 2.
             line_style (str, optional): Line style. Defaults to "solid". Options are "solid", "dashed"
         """
-        if label_text_font == "":
-            label_text_font = self._painter.marker_font
-        if label_text_size == 0:
-            label_text_size = self._painter.marker_font_size
-        if label_text_colour == "":
-            label_text_colour = self._painter.marker_font_colour
-        if line_colour == "":
-            line_colour = self._painter.marker_line_colour
+        label_text_font = label_text_font or self._painter.marker_font
+        label_text_size = label_text_size or self._painter.marker_font_size
+        label_text_colour = label_text_colour or self._painter.marker_font_colour
+        line_colour = line_colour or self._painter.marker_line_colour
+
 
         self._marker = Marker(
             font=label_text_font,
             font_size=label_text_size,
             font_colour=label_text_colour,
             line_colour=line_colour,
             line_width=line_width,
@@ -119,22 +116,19 @@
             label_text_font (str, optional): Label text font. Defaults to "Arial".
             label_text_colour (str, optional): Label text colour. Defaults to "Black".
             label_text_size (int, optional): Label text size. Defaults to 10.
             line_colour (str, optional): Line colour. Defaults to "Black".
             line_width (int, optional): Line width. Defaults to 2.
             line_style (str, optional): Line style. Defaults to "solid". Options are "solid", "dashed"
         """
-        if label_text_font == "":
-            label_text_font = self._painter.marker_font
-        if label_text_size == 0:
-            label_text_size = self._painter.marker_font_size
-        if label_text_colour == "":
-            label_text_colour = self._painter.marker_font_colour
-        if line_colour == "":
-            line_colour = self._painter.marker_line_colour
+            
+        label_text_font = label_text_font or self._painter.marker_font
+        label_text_size = label_text_size or self._painter.marker_font_size
+        label_text_colour = label_text_colour or self._painter.marker_font_colour
+        line_colour = line_colour or self._painter.marker_line_colour
 
         self._marker.font = label_text_font
         self._marker.font_size = label_text_size
         self.font_colour = label_text_colour
         self.line_colour = line_colour
         self.line_width = line_width
         self.line_style = line_style
@@ -150,20 +144,19 @@
 
         Args:
             text (str): Title text
             font (str, optional): Title font. Defaults to "Arial".
             font_size (int, optional): Title font size. Defaults to 18.
             font_colour (str, optional): Title font colour. Defaults to "Black".
         """
-        if font == "":
-            font = self._painter.title_font
-        if font_size == 0:
-            font_size = self._painter.title_font_size
-        if font_colour == "":
-            font_colour = self._painter.title_font_colour
+            
+        font = font or self._painter.title_font
+        font_size = font_size or self._painter.title_font_size
+        font_colour = font_colour or self._painter.title_font_colour
+        
 
         self._title = Title(
             text=text, font=font, font_size=font_size, font_colour=font_colour
         )
         self._title.text = text
 
         self._title.set_draw_position(self._painter)
@@ -179,20 +172,18 @@
 
         Args:
             text (str): Title text
             font (str, optional): Title font. Defaults to "Arial".
             font_size (int, optional): Title font size. Defaults to 18.
             font_colour (str, optional): Title font colour. Defaults to "Black".
         """
-        if font == "":
-            font = self._painter.subtitle_font
-        if font_size == 0:
-            font_size = self._painter.subtitle_font_size
-        if font_colour == "":
-            font_colour = self._painter.subtitle_font_colour
+            
+        font = font or self._painter.subtitle_font
+        font_size = font_size or self._painter.subtitle_font_size
+        font_colour = font_colour or self._painter.subtitle_font_colour
 
         self._subtitle = SubTitle(
             text=text, font=font, font_size=font_size, font_colour=font_colour
         )
         self._subtitle.text = text
 
         self._subtitle.set_draw_position(self._painter)
@@ -208,20 +199,18 @@
 
         Args:
             text (str): Footer text
             font (str, optional): Footer font. Defaults to "Arial".
             font_size (int, optional): Footer font size. Defaults to 18.
             font_colour (str, optional): Footer font colour. Defaults to "Black".
         """
-        if font == "":
-            font = self._painter.footer_font
-        if font_size == 0:
-            font_size = self._painter.footer_font_size
-        if font_colour == "":
-            font_colour = self._painter.footer_font_colour
+            
+        font = font or self._painter.footer_font
+        font_size = font_size or self._painter.footer_font_size
+        font_colour = font_colour or self._painter.footer_font_colour
 
         self._footer = Footer(
             text=text, font=font, font_size=font_size, font_colour=font_colour
         )
         self._footer.text = text
 
     def set_timeline(
@@ -261,31 +250,24 @@
             font_colour (str, optional): Timelinegroup font colour. Defaults to "DEFAULT" colour theme.
             fill_colour (str, optional): Timelinegroup fill colour. Defaults to "DEFAULT" colour theme.
             font (str, optional): Timeline font. Defaults to "DEFAULT" colour theme.
             font_size (int, optional): Timeline font size. Defaults to "DEFAULT" colour theme.
             font_colour (str, optional): Timeline font colour. Defaults to "DEFAULT" colour theme.
             fill_colour (str, optional): Timeline fill colour. Defaults to "DEFAULT" colour theme.
         """
-        if year_font == "":
-            year_font = self._painter.timeline_year_font
-        if year_font_size == 0:
-            year_font_size = self._painter.timeline_year_font_size
-        if year_font_colour == "":
-            year_font_colour = self._painter.timeline_year_font_colour
-        if year_fill_colour == "":
-            year_fill_colour = self._painter.timeline_year_fill_colour
-
-        if item_font == "":
-            item_font = self._painter.timeline_item_font
-        if item_font_size == 0:
-            item_font_size = self._painter.timeline_item_font_size
-        if item_font_colour == "":
-            item_font_colour = self._painter.timeline_item_font_colour
-        if item_fill_colour == "":
-            item_fill_colour = self._painter.timeline_item_fill_colour
+            
+        year_font = year_font or self._painter.timeline_year_font
+        year_font_size = year_font_size or self._painter.timeline_year_font_size
+        year_font_colour = year_font_colour or self._painter.timeline_year_font_colour
+        year_fill_colour = year_fill_colour or self._painter.timeline_year_fill_colour
+        
+        item_font = item_font or self._painter.timeline_item_font
+        item_font_size = item_font_size or self._painter.timeline_item_font_size
+        item_font_colour = item_font_colour or self._painter.timeline_item_font_colour
+        item_fill_colour = item_fill_colour or self._painter.timeline_item_fill_colour
 
         self._show_generic_dates = show_generic_dates
         start_date = datetime.strptime(start, "%Y-%m-%d")
         self._timeline = Timeline(
             mode=mode,
             start=start_date,
             locale_name=timeline_locale,
@@ -345,22 +327,18 @@
             font_colour (str, optional): Group text font colour. Defaults to "Black".
             fill_colour (str, optional): Group fill colour. Defaults to "lightgrey".
             text_alignment (str, optional): Group text alignment. Defaults to "centre". Options are "left", "centre", "right"
 
         Return:
             Group: A new group instance. Use this to add taks to the group
         """
-        if font == "":
-            font = self._painter.group_font
-        if font_size == 0:
-            font_size = self._painter.group_font_size
-        if font_colour == "":
-            font_colour = self._painter.group_font_colour
-        if fill_colour == "":
-            fill_colour = self._painter.group_fill_colour
+        font = font or self._painter.group_font
+        font_size = font_size or self._painter.group_font_size
+        font_colour = font_colour or self._painter.group_font_colour
+        fill_colour = fill_colour or self._painter.group_fill_colour
 
         group = Group(
             text=text,
             font=font,
             font_size=font_size,
             font_colour=font_colour,
             fill_colour=fill_colour,
```

### Comparing `roadmapper-1.2.0/src/roadmapper/subtitle.py` & `roadmapper-1.2.1/src/roadmapper/subtitle.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.0/src/roadmapper/task.py` & `roadmapper-1.2.1/src/roadmapper/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,26 +51,14 @@
     box_x: int = field(init=False, default=0)
     box_y: int = field(init=False, default=0)
     box_width: int = field(init=False, default=0)
     box_height: int = field(init=False, default=0)
     text_x: int = field(init=False, default=0)
     text_y: int = field(init=False, default=0)
 
-    # def __post_init__(self):
-    #     """This method is called after __init__() is called"""
-    #     self.milestones = []
-    #     self.tasks = []
-    #     self.boxes = []
-    #     self.box_x = 0
-    #     self.box_y = 0
-    #     self.box_width = 0
-    #     self.box_height = 0
-    #     self.text_x = 0
-    #     self.text_y = 0
-
     def add_parallel_task(
         self,
         text: str,
         start: datetime,
         end: datetime,
         font: str = "",
         font_size: int = 0,
@@ -89,25 +77,19 @@
             font_size (int, optional): Task text font size. Defaults to 12.
             font_colour (str, optional): Task text font colour. Defaults to "Black".
             fill_colour (str, optional): Task fill colour. Defaults to "LightGreen".
 
         Return:
             Task: A task object that can be used to add milestones
         """
-        if font == "":
-            font = self.painter.task_font
-        if font_size == 0:
-            font_size = self.painter.task_font_size
-        if font_colour == "":
-            font_colour = self.painter.task_font_colour
-        if fill_colour == "":
-            fill_colour = self.painter.task_fill_colour
-
-        if style == "":
-            style = self.painter.task_style
+        font = font or self.painter.task_font
+        font_size = font_size or self.painter.task_font_size
+        font_colour = font_colour or self.painter.task_font_colour
+        fill_colour = fill_colour or self.painter.task_fill_colour
+        style = style or self.painter.task_style
 
         task = Task(
             text=text,
             start=start,
             end=end,
             font=font,
             font_size=font_size,
@@ -141,22 +123,20 @@
             font_colour (str, optional): Milestone text font colour. Defaults to "Red". HTML colour name or hex code. Eg. #FFFFFF or LightGreen
             fill_colour (str, optional): Milestone fill colour. Defaults to "Red". HTML colour name or hex code. Eg. #FFFFFF or LightGreen
             text_alignment (str, optional): Milestone text alignment. Defaults to "centre". Options are "left", "centre", "right"
         """
 
         if self.painter is None:
             print("Painter is None")
-        if font == "":
-            font = self.painter.milestone_font
-        if font_size == 0:
-            font_size = self.painter.milestone_font_size
-        if font_colour == "":
-            font_colour = self.painter.milestone_font_colour
-        if fill_colour == "":
-            fill_colour = self.painter.milestone_fill_colour
+            
+        font = font or self.painter.milestone_font
+        font_size = font_size or self.painter.milestone_font_size
+        font_colour = font_colour or self.painter.milestone_font_colour
+        fill_colour = fill_colour or self.painter.milestone_fill_colour
+        
 
         self.milestones.append(
             Milestone(
                 text=text,
                 date=date,
                 font=font,
                 font_size=font_size,
@@ -554,16 +534,14 @@
         """
         box_x = 0
         box_y = 0
         width = 0
         height = 0
 
         for i, box in enumerate(self.boxes):
-            # painter.draw_box(box[0], box[1], box[2], box[3], self.fill_colour)
-            # painter.draw_rounded_box(box[0], box[1], box[2], box[3], self.fill_colour)
             if i == 0:
                 box_x = box[0]
                 box_y = box[1]
             width += int(box[2])
             height = box[3]
 
         box_width, box_height = (
```

### Comparing `roadmapper-1.2.0/src/roadmapper/timeline.py` & `roadmapper-1.2.1/src/roadmapper/timeline.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.0/src/roadmapper/timelineitem.py` & `roadmapper-1.2.1/src/roadmapper/timelineitem.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.0/src/roadmapper/timelineitemyear.py` & `roadmapper-1.2.1/src/roadmapper/timelineitemyear.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.0/src/roadmapper/timelinelocale.py` & `roadmapper-1.2.1/src/roadmapper/timelinelocale.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.0/src/roadmapper/timelinemode.py` & `roadmapper-1.2.1/src/roadmapper/timelinemode.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.0/src/roadmapper/title.py` & `roadmapper-1.2.1/src/roadmapper/title.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.0/src/roadmapper.egg-info/PKG-INFO` & `roadmapper-1.2.1/src/roadmapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadmapper
-Version: 1.2.0
+Version: 1.2.1
 Summary: Roadmapper. A Roadmap-as-Code (RaC) python library for generating a roadmap by using python code
 Author: CS Goh
 Project-URL: Homepage, https://github.com/csgoh/roadmapper
 Project-URL: Bug Tracker, https://github.com/csgoh/roadmapper/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,24 +32,24 @@
 With git repository like GitHub or Bitbucket, roadmaps created using RaC can be version controlled, track changes and can be easily shared with others.
 
 ### Latest version
 ![release](https://img.shields.io/pypi/v/roadmapper)
 
 :book: For usage documentation, how-to guide and code examples, refer to [Roadmapper Wiki](https://github.com/csgoh/roadmap-generator/wiki).
 
-View the [Change Logs](https://github.com/csgoh/processpiper/wiki/Change-Logs) to find out the latest updates and additions in the most recent version.
+View the [Change Logs](https://github.com/csgoh/roadmapper/wiki/Change-Logs) to find out the latest updates and additions in the most recent version.
 
 ![multilingual roadmappper](https://github.com/csgoh/roadmapper/blob/main/images/roadmapper-banner-multilingual.png?raw=true)
 
 ### Python version requirements:
 * Python 3.10+
   
 ### Library Dependencies
-* Pillow 9.4.0
-* python-dateutil
+* Pillow 9.5.0
+* python-dateutil 2.8.2
 
 Any feedback or suggestions are welcome. Please feel free to create an issue or pull request.
 <br/>
 <hr>
 
 
 ## Installation
```

### Comparing `roadmapper-1.2.0/src/tests/roadmap_draw_test.py` & `roadmapper-1.2.1/src/tests/roadmap_draw_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 import calendar
 
 import pytest
 
 from src.roadmapper.roadmap import Roadmap
 
 
-def test_draw_roadmap_with_minimal_required_features():
-    roadmap: Roadmap = Roadmap()
-    roadmap.set_timeline(start="2023-01-01")
-    roadmap.set_title("Test Title")
+@pytest.mark.unit
+class TestRoadmapDraw:
+    def test_draw_roadmap_with_minimal_required_features(self):
+        roadmap: Roadmap = Roadmap()
+        roadmap.set_timeline(start="2023-01-01")
+        roadmap.set_title("Test Title")
 
-    roadmap.draw()
-
-    filename_with_ts = str(calendar.timegm(time.gmtime())) + ".png"
-    roadmap.save(filename_with_ts)
+        roadmap.draw()
 
-    assert os.path.exists(filename_with_ts)
-    os.remove(filename_with_ts)
+        filename_with_ts = str(calendar.timegm(time.gmtime())) + ".png"
+        roadmap.save(filename_with_ts)
 
+        assert os.path.exists(filename_with_ts)
+        os.remove(filename_with_ts)
 
-def test_draw_roadmap_requires_timeline():
-    roadmap: Roadmap = Roadmap()
-    roadmap.set_title("Test Title")
+    def test_draw_roadmap_requires_timeline(self):
+        roadmap: Roadmap = Roadmap()
+        roadmap.set_title("Test Title")
 
-    with pytest.raises(ValueError) as e:
-        roadmap.draw()
+        with pytest.raises(ValueError) as e:
+            roadmap.draw()
 
-    assert "timeline" in str(e.value).lower()
+        assert "timeline" in str(e.value).lower()
 
+    def test_draw_roadmap_requires_title(self):
+        roadmap: Roadmap = Roadmap()
 
-def test_draw_roadmap_requires_title():
-    roadmap: Roadmap = Roadmap()
-
-    with pytest.raises(ValueError) as e:
-        roadmap.draw()
+        with pytest.raises(ValueError) as e:
+            roadmap.draw()
 
-    assert "title" in str(e.value).lower()
+        assert "title" in str(e.value).lower()
```

### Comparing `roadmapper-1.2.0/src/tests/test_cases.py` & `roadmapper-1.2.1/src/tests/test_cases.py`

 * *Files 5% similar despite different names*

```diff
@@ -671,50 +671,50 @@
     roadmap.draw()
     roadmap.save(output_file)
 
     assert os.path.exists(output_file)
 
 
 def banner_roadmap():
-    color_theme_roadmap("images/color-theme01.png", "DEFAULT")
-    color_theme_roadmap("images/color-theme02.png", "GREYWOOF")
-    color_theme_roadmap("images/color-theme03.png", "ORANGEPEEL")
-    color_theme_roadmap("images/color-theme04.png", "BLUEMOUNTAIN")
-    color_theme_roadmap("images/color-theme05.png", "GREENTURTLE")
+    color_theme_roadmap("../../images/color-theme01.png", "DEFAULT")
+    color_theme_roadmap("../../images/color-theme02.png", "GREYWOOF")
+    color_theme_roadmap("../../images/color-theme03.png", "ORANGEPEEL")
+    color_theme_roadmap("../../images/color-theme04.png", "BLUEMOUNTAIN")
+    color_theme_roadmap("../../images/color-theme05.png", "GREENTURTLE")
 
 
 def multilingual_roadmap():
-    en_NZ_roadmap("images/en_NZ-roadmap.png", "src/json/rainbow.json", "en_US")
+    en_NZ_roadmap("../../images/en_NZ-roadmap.png", "../json/rainbow.json", "en_US")
     zh_TW_with_locale_roadmap(
-        "images/zh_TW-roadmap.png",
-        "src/json/rainbow-unicode.json",
-        "src/json/zh_TW_timeline_settings.json",
+        "../../images/zh_TW-roadmap.png",
+        "../json/rainbow-unicode.json",
+        "../json/zh_TW_timeline_settings.json",
     )
     zh_TW_roadmap(
-        "images/zh_TW-timeline-roadmap.png",
-        "src/json/rainbow-unicode.json",
+        "../../images/zh_TW-timeline-roadmap.png",
+        "../json/rainbow-unicode.json",
     )
     ja_JP_roadmap(
-        "images/ja_JP-roadmap.png",
-        "src/json/rainbow-unicode.json",
-        "src/json/ja_JP_timeline_settings.json",
+        "../../images/ja_JP-roadmap.png",
+        "../json/rainbow-unicode.json",
+        "../json/ja_JP_timeline_settings.json",
     )
     ko_KR_roadmap(
-        "images/ko-KR-roadmap.png",
-        "src/json/rainbow-unicode.json",
-        "src/json/ko_KR_timeline_settings.json",
+        "../../images/ko-KR-roadmap.png",
+        "../json/rainbow-unicode.json",
+        "../json/ko_KR_timeline_settings.json",
     )
 
 
 ### Wiki Images
 def home_roadmap():
     if not os.path.exists("images"):
         os.mkdir("images")
 
-    output_file = "images/my_roadmap.png"
+    output_file = "../../images/my_roadmap.png"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     my_roadmap = Roadmap(width=500, height=400)
     my_roadmap.set_title("My Roadmap")
     my_roadmap.set_timeline(
@@ -732,25 +732,25 @@
     assert os.path.exists(output_file)
 
 
 def readme_roadmap():
     if not os.path.exists("images"):
         os.mkdir("images")
 
-    output_file = "images/demo01.png"
+    output_file = "../../images/demo01.png"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     roadmap = Roadmap(1200, 400, colour_theme="BLUEMOUNTAIN")
     roadmap.set_title("My Demo Roadmap")
     roadmap.set_subtitle("Matariki Technologies Ltd")
     roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01", number_of_items=12)
     roadmap.add_logo(
-        "images/logo/matariki-tech-logo.png", position="top-right", width=50, height=50
+        "../../images/logo/matariki-tech-logo.png", position="top-right", width=50, height=50
     )
 
     group = roadmap.add_group("Core Product Work Stream")
 
     task = group.add_task("Base Functionality", "2023-01-01", "2023-10-31")
     task.add_milestone("v.1.0", "2023-02-15")
     task.add_milestone("v.1.1", "2023-08-01")
@@ -991,68 +991,68 @@
     assert os.path.exists(output_file)
 
 
 ### Test case functions ###
 
 
 def test_sample_case1():
-    if not os.path.exists("images/test"):
-        os.mkdir("images/test")
+    if not os.path.exists("../../images/test"):
+        os.mkdir("../../images/test")
     colour_theme_demo(
         width=2500,
-        file_name="images/test/test-ORANGEPEEL-weekly.png",
+        file_name="../../images/test/test-ORANGEPEEL-weekly.png",
         colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.WEEKLY,
         number_of_items=52,
         start_date="2023-01-01",
     )
 
 
 def test_sample_case2():
-    if not os.path.exists("images/test"):
-        os.mkdir("images/test")
+    if not os.path.exists("../../images/test"):
+        os.mkdir("../../images/test")
     colour_theme_demo(
-        file_name="images/test/test-ORANGEPEEL-monthly.png",
+        file_name="../../images/test/test-ORANGEPEEL-monthly.png",
         colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
     )
 
 
 def test_sample_case3():
-    if not os.path.exists("images/test"):
-        os.mkdir("images/test")
+    if not os.path.exists("../../images/test"):
+        os.mkdir("../../images/test")
     colour_theme_demo(
-        file_name="images/test/test-ORANGEPEEL-quarter.png",
+        file_name="../../images/test/test-ORANGEPEEL-quarter.png",
         colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.QUARTERLY,
         number_of_items=4,
         start_date="2023-01-01",
     )
 
 
 def test_sample_unicase1():
-    if not os.path.exists("images/test"):
-        os.mkdir("images/test")
+    if not os.path.exists("../../images/test"):
+        os.mkdir("../../images/test")
     unicode_demo(
-        file_name="images/test/test-unicode-monthly.png",
+        file_name="../../images/test/test-unicode-monthly.png",
         # colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
     )
     assert True
 
 
 def test_draw_anatomy():
     if not os.path.exists("images"):
         os.mkdir("images")
 
-    output_file = "images/roadmapper-anatomy-base.png"
+    output_file = "../../images/roadmapper-anatomy-base.png"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     roadmap = Roadmap(1200, 380, colour_theme="BLUEMOUNTAIN", show_marker=True)
     roadmap.set_title("Product Roadmap")
     roadmap.set_subtitle("Matariki Tech Ltd")
@@ -1071,15 +1071,15 @@
     assert os.path.exists(output_file)
 
 
 def test_draw_banner_theme():
     if not os.path.exists("images"):
         os.mkdir("images")
 
-    output_file = "images/theme-demo01.png"
+    output_file = "../../images/theme-demo01.png"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     roadmap = Roadmap(600, 380, colour_theme="BLUEMOUNTAIN", show_marker=True)
     roadmap.set_title("My Demo Roadmap")
     roadmap.set_timeline(TimelineMode.QUARTERLY, start="2023-01-01", number_of_items=4)
@@ -1100,15 +1100,15 @@
     assert os.path.exists(output_file)
 
 
 def test_draw_banner():
     if not os.path.exists("images"):
         os.mkdir("images")
 
-    output_file = "images/demo01.png"
+    output_file = "../../images/demo01.png"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     roadmap = Roadmap(600, 500, show_marker=False, auto_height=True)
     roadmap.set_title("My Demo Roadmap")
     roadmap.set_timeline(
@@ -1176,121 +1176,121 @@
     assert os.path.exists(output_file)
 
 
 def test_gallery_images():
     ### Sample Roadmap ###
     sample_roadmap(
         width=1400,
-        file_name="images/gallery/gallery-sample-01.png",
+        file_name="../../images/gallery/gallery-sample-01.png",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
     )
 
     ### Colour Theme Roadmap ###
 
     colour_theme_roadmap(
-        file_name="images/gallery/gallery-DEFAULT-monthly.png",
+        file_name="../../images/gallery/gallery-DEFAULT-monthly.png",
         # colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
     )
 
     colour_theme_roadmap(
-        file_name="images/gallery/gallery-ORANGEPEEL-monthly.png",
+        file_name="../../images/gallery/gallery-ORANGEPEEL-monthly.png",
         colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
     )
 
     colour_theme_roadmap(
-        file_name="images/gallery/gallery-BLUEMOUNTAIN-monthly.png",
+        file_name="../../images/gallery/gallery-BLUEMOUNTAIN-monthly.png",
         colour_theme="BLUEMOUNTAIN",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
     )
 
     colour_theme_roadmap(
-        file_name="images/gallery/gallery-GREENTURTLE-monthly.png",
+        file_name="../../images/gallery/gallery-GREENTURTLE-monthly.png",
         colour_theme="GREENTURTLE",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
     )
 
     colour_theme_roadmap(
-        file_name="images/gallery/gallery-GREYWOOF-monthly.png",
+        file_name="../../images/gallery/gallery-GREYWOOF-monthly.png",
         colour_theme="GREYWOOF",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
     )
 
     ### Marker Roadmap ###
     custom_colour_roadmap(
         width=1200,
-        file_name="images/gallery/gallery-marker-monthly.png",
+        file_name="../../images/gallery/gallery-marker-monthly.png",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2022-11-01",
         show_marker=True,
         show_generic_dates=False,
     )
 
     ### WEEKLY Timeline Roadmap ###
     colour_theme_roadmap(
         width=2400,
-        file_name="images/gallery/gallery-DEFAULT-weekly.png",
+        file_name="../../images/gallery/gallery-DEFAULT-weekly.png",
         colour_theme="DEFAULT",
         timelinemode=TimelineMode.WEEKLY,
         number_of_items=52,
         start_date="2023-01-01",
         show_generic_dates=False,
     )
 
     ### QUARTERLY Timeline Roadmap ###
     colour_theme_roadmap(
         width=1400,
-        file_name="images/gallery/gallery-DEFAULT-quarterly.png",
+        file_name="../../images/gallery/gallery-DEFAULT-quarterly.png",
         colour_theme="DEFAULT",
         timelinemode=TimelineMode.QUARTERLY,
         number_of_items=6,
         start_date="2023-01-01",
         show_generic_dates=False,
     )
 
     ### HALF-YEARLY Timeline Roadmap ###
     colour_theme_roadmap(
         width=1400,
-        file_name="images/gallery/gallery-DEFAULT-halfyearly.png",
+        file_name="../../images/gallery/gallery-DEFAULT-halfyearly.png",
         colour_theme="DEFAULT",
         timelinemode=TimelineMode.HALF_YEARLY,
         number_of_items=4,
         start_date="2023-01-01",
         show_generic_dates=False,
     )
 
     ### YEARLY Timeline Roadmap ###
     colour_theme_roadmap(
         width=1400,
-        file_name="images/gallery/gallery-DEFAULT-yearly.png",
+        file_name="../../images/gallery/gallery-DEFAULT-yearly.png",
         colour_theme="DEFAULT",
         timelinemode=TimelineMode.YEARLY,
         number_of_items=2,
         start_date="2023-01-01",
         show_generic_dates=False,
     )
 
     ### Generic Dates Roadmap ###
     colour_theme_roadmap(
         width=1400,
-        file_name="images/gallery/gallery-DEFAULT-generic-monthly.png",
+        file_name="../../images/gallery/gallery-DEFAULT-generic-monthly.png",
         colour_theme="DEFAULT",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
         show_generic_dates=True,
     )
 
@@ -1321,8 +1321,8 @@
                 ) as parallel_task1:
                     parallel_task1.add_milestone("Milestone 2", "2023-08-10")
                 task1.add_milestone(
                     "Milestone 1",
                     "2023-04-01",
                 )
         my_roadmap.draw()
-        my_roadmap.save("images/with_context_manager.png")
+        my_roadmap.save("../../images/with_context_manager.png")
```

### Comparing `roadmapper-1.2.0/src/tests/test_painter.py` & `roadmapper-1.2.1/src/tests/test_painter.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.0/src/tests/test_roadmapper.py` & `roadmapper-1.2.1/src/tests/test_roadmapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,30 +346,30 @@
     )
 
     assert os.path.exists(output_file)
 
     output_file = "images/test/demo-my-colour-chinese.png"
     chinese_theme_demo(
         file_name=output_file,
-        colour_theme="src/json/chinese.json",
+        colour_theme="../json/chinese.json",
         timelinemode=TimelineMode.WEEKLY,
         start_date="2023-01-01",
         number_of_items=14,
-        locale_name="src/json/zh_TW_timeline_settings.json",
+        locale_name="../json/zh_TW_timeline_settings.json",
         show_generic_dates=False,
         show_first_day_of_week=True,
     )
     assert os.path.exists(output_file)
 
     output_file = "images/test/demo-my-colour-japanese.png"
     japanese_theme_demo(
         file_name=output_file,
-        colour_theme="src/json/chinese.json",
+        colour_theme="../json/chinese.json",
         timelinemode=TimelineMode.MONTHLY,
         start_date="2023-01-01",
         number_of_items=14,
-        locale_name="src/json/ja_JP_timeline_settings.json",
+        locale_name="../json/ja_JP_timeline_settings.json",
         show_generic_dates=False,
         show_first_day_of_week=True,
     )
 
     assert os.path.exists(output_file)
```

