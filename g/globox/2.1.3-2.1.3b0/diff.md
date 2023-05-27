# Comparing `tmp/globox-2.1.3.tar.gz` & `tmp/globox-2.1.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globox-2.1.3.tar", max compression
+gzip compressed data, was "globox-2.1.3b0.tar", max compression
```

## Comparing `globox-2.1.3.tar` & `globox-2.1.3b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     9236 2023-05-27 13:03:53.301797 globox-2.1.3/README.md
--rw-r--r--   0        0        0     1085 2023-05-27 13:03:53.301797 globox-2.1.3/pyproject.toml
--rw-r--r--   0        0        0      273 2023-05-27 13:03:53.301797 globox-2.1.3/src/globox/__init__.py
--rw-r--r--   0        0        0       30 2023-05-27 13:03:53.301797 globox-2.1.3/src/globox/__main__.py
--rw-r--r--   0        0        0    18551 2023-05-27 13:03:53.301797 globox-2.1.3/src/globox/annotation.py
--rw-r--r--   0        0        0    33313 2023-05-27 13:03:53.301797 globox-2.1.3/src/globox/annotationset.py
--rw-r--r--   0        0        0     1015 2023-05-27 13:03:53.301797 globox-2.1.3/src/globox/atomic.py
--rw-r--r--   0        0        0    17250 2023-05-27 13:03:53.301797 globox-2.1.3/src/globox/boundingbox.py
--rw-r--r--   0        0        0    14247 2023-05-27 13:03:53.301797 globox-2.1.3/src/globox/cli.py
--rw-r--r--   0        0        0      539 2023-05-27 13:03:53.301797 globox-2.1.3/src/globox/errors.py
--rw-r--r--   0        0        0    21347 2023-05-27 13:03:53.305797 globox-2.1.3/src/globox/evaluation.py
--rw-r--r--   0        0        0      699 2023-05-27 13:03:53.305797 globox-2.1.3/src/globox/file_utils.py
--rw-r--r--   0        0        0     6983 2023-05-27 13:03:53.305797 globox-2.1.3/src/globox/image_utils.py
--rw-r--r--   0        0        0      880 2023-05-27 13:03:53.305797 globox-2.1.3/src/globox/thread_utils.py
--rw-r--r--   0        0        0      747 2023-05-27 13:03:53.305797 globox-2.1.3/src/globox/utils.py
--rw-r--r--   0        0        0    10287 1970-01-01 00:00:00.000000 globox-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     9236 2023-05-26 20:44:52.964782 globox-2.1.3b0/README.md
+-rw-r--r--   0        0        0     1042 2023-05-26 20:44:52.964782 globox-2.1.3b0/pyproject.toml
+-rw-r--r--   0        0        0      273 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/__init__.py
+-rw-r--r--   0        0        0       30 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/__main__.py
+-rw-r--r--   0        0        0    18551 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/annotation.py
+-rw-r--r--   0        0        0    33312 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/annotationset.py
+-rw-r--r--   0        0        0     1015 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/atomic.py
+-rw-r--r--   0        0        0    17250 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/boundingbox.py
+-rw-r--r--   0        0        0    14247 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/cli.py
+-rw-r--r--   0        0        0      539 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/errors.py
+-rw-r--r--   0        0        0    21347 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/evaluation.py
+-rw-r--r--   0        0        0      699 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/file_utils.py
+-rw-r--r--   0        0        0     6983 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/image_utils.py
+-rw-r--r--   0        0        0      880 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/thread_utils.py
+-rw-r--r--   0        0        0      747 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/utils.py
+-rw-r--r--   0        0        0    10289 1970-01-01 00:00:00.000000 globox-2.1.3b0/PKG-INFO
```

### Comparing `globox-2.1.3/README.md` & `globox-2.1.3b0/README.md`

 * *Files identical despite different names*

### Comparing `globox-2.1.3/pyproject.toml` & `globox-2.1.3b0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "globox"
-version = "2.1.3"
+version = "2.1.3-beta"
 authors = ["Louis Lac <lac.louis5@gmail.com>"]
 license = "MIT"
 packages = [{include = "globox", from = "src"}]
 readme = "README.md"
 description = "Globox is a package and command line interface to read and convert object detection databases (COCO, YOLO, PascalVOC, LabelMe, CVAT, OpenImage, ...) and evaluate them with COCO and PascalVOC."
 homepage = "https://github.com/laclouis5/globox"
 repository = "https://github.com/laclouis5/globox"
@@ -35,10 +35,7 @@
 
 [tool.poetry.scripts]
 globox = "globox.cli:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-
-[tool.pytest.ini_options]
-testpaths = ["tests"]
```

### Comparing `globox-2.1.3/src/globox/annotation.py` & `globox-2.1.3b0/src/globox/annotation.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.3/src/globox/annotationset.py` & `globox-2.1.3b0/src/globox/annotationset.py`

 * *Files 0% similar despite different names*

```diff
@@ -638,15 +638,15 @@
         verbose: bool = False,
     ):
         save_dir = Path(save_dir).expanduser().resolve()
         save_dir.mkdir(exist_ok=True)
 
         def _save(annotation: Annotation):
             path = save_dir / Path(annotation.image_id).with_suffix(".txt")
-            annotation._save_yolo(path, label_to_id=label_to_id, conf_last=conf_last)
+            annotation.save_yolo(path, label_to_id=label_to_id, conf_last=conf_last)
 
         self.save_from_it(_save, verbose=verbose)
 
     def save_yolo(
         self,
         save_dir: PathLike,
         *,
```

### Comparing `globox-2.1.3/src/globox/atomic.py` & `globox-2.1.3b0/src/globox/atomic.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.3/src/globox/boundingbox.py` & `globox-2.1.3b0/src/globox/boundingbox.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.3/src/globox/cli.py` & `globox-2.1.3b0/src/globox/cli.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.3/src/globox/errors.py` & `globox-2.1.3b0/src/globox/errors.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.3/src/globox/evaluation.py` & `globox-2.1.3b0/src/globox/evaluation.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.3/src/globox/file_utils.py` & `globox-2.1.3b0/src/globox/file_utils.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.3/src/globox/image_utils.py` & `globox-2.1.3b0/src/globox/image_utils.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.3/src/globox/thread_utils.py` & `globox-2.1.3b0/src/globox/thread_utils.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.3/src/globox/utils.py` & `globox-2.1.3b0/src/globox/utils.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.3/PKG-INFO` & `globox-2.1.3b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globox
-Version: 2.1.3
+Version: 2.1.3b0
 Summary: Globox is a package and command line interface to read and convert object detection databases (COCO, YOLO, PascalVOC, LabelMe, CVAT, OpenImage, ...) and evaluate them with COCO and PascalVOC.
 Home-page: https://github.com/laclouis5/globox
 License: MIT
 Keywords: annotation,metrics,object detection,bounding boxes,yolo,openimages,cvat,coco,pascal voc,average precision,mean average precision
 Author: Louis Lac
 Author-email: lac.louis5@gmail.com
 Requires-Python: >=3.8,<4.0
```

