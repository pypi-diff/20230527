# Comparing `tmp/pyconvertapi_image_converter-0.1.1.tar.gz` & `tmp/pyconvertapi_image_converter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconvertapi_image_converter-0.1.1.tar", last modified: Sat May 27 15:04:27 2023, max compression
+gzip compressed data, was "pyconvertapi_image_converter-0.1.2.tar", last modified: Sat May 27 15:38:10 2023, max compression
```

## Comparing `pyconvertapi_image_converter-0.1.1.tar` & `pyconvertapi_image_converter-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 15:04:27.752842 pyconvertapi_image_converter-0.1.1/
--rw-rw-rw-   0        0        0     1104 2023-03-19 23:35:37.000000 pyconvertapi_image_converter-0.1.1/LICENSE.md
--rw-rw-rw-   0        0        0     4272 2023-05-27 15:04:27.737814 pyconvertapi_image_converter-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3398 2023-05-22 17:33:53.000000 pyconvertapi_image_converter-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 15:04:27.602110 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter/
--rw-rw-rw-   0        0        0     1020 2023-05-22 17:34:34.000000 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter/__init__.py
--rw-rw-rw-   0        0        0     5818 2023-05-27 14:59:57.000000 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter/image_converter.py
-drwxrwxrwx   0        0        0        0 2023-05-27 15:04:27.736106 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter.egg-info/
--rw-rw-rw-   0        0        0     4272 2023-05-27 15:04:27.000000 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-05-27 15:04:27.000000 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 15:04:27.000000 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-27 15:04:27.000000 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-05-27 15:04:27.000000 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1013 2023-05-27 15:02:52.000000 pyconvertapi_image_converter-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 15:04:27.752842 pyconvertapi_image_converter-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 15:38:10.664688 pyconvertapi_image_converter-0.1.2/
+-rw-rw-rw-   0        0        0     1104 2023-03-19 23:35:37.000000 pyconvertapi_image_converter-0.1.2/LICENSE.md
+-rw-rw-rw-   0        0        0     4272 2023-05-27 15:38:10.661685 pyconvertapi_image_converter-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3398 2023-05-22 17:33:53.000000 pyconvertapi_image_converter-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 15:38:10.547687 pyconvertapi_image_converter-0.1.2/pyconvertapi_image_converter/
+-rw-rw-rw-   0        0        0     1020 2023-05-22 17:34:34.000000 pyconvertapi_image_converter-0.1.2/pyconvertapi_image_converter/__init__.py
+-rw-rw-rw-   0        0        0     5828 2023-05-27 15:16:03.000000 pyconvertapi_image_converter-0.1.2/pyconvertapi_image_converter/image_converter.py
+drwxrwxrwx   0        0        0        0 2023-05-27 15:38:10.653685 pyconvertapi_image_converter-0.1.2/pyconvertapi_image_converter.egg-info/
+-rw-rw-rw-   0        0        0     4272 2023-05-27 15:38:10.000000 pyconvertapi_image_converter-0.1.2/pyconvertapi_image_converter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-05-27 15:38:10.000000 pyconvertapi_image_converter-0.1.2/pyconvertapi_image_converter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 15:38:10.000000 pyconvertapi_image_converter-0.1.2/pyconvertapi_image_converter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-27 15:38:10.000000 pyconvertapi_image_converter-0.1.2/pyconvertapi_image_converter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-05-27 15:38:10.000000 pyconvertapi_image_converter-0.1.2/pyconvertapi_image_converter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1013 2023-05-27 15:37:03.000000 pyconvertapi_image_converter-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 15:38:10.665689 pyconvertapi_image_converter-0.1.2/setup.cfg
```

### Comparing `pyconvertapi_image_converter-0.1.1/LICENSE.md` & `pyconvertapi_image_converter-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyconvertapi_image_converter-0.1.1/PKG-INFO` & `pyconvertapi_image_converter-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconvertapi_image_converter
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyConvertAPI Image Converter is a Python library for converting images to different formats using ConvertAPI
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/pyconvertapi_image_converter
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/pyconvertapi_image_converter/issues
 Project-URL: Repository, https://github.com/ti-oluwa/pyconvertapi_image_converter
 Keywords: Image format conversion,ConvertAPI
```

### Comparing `pyconvertapi_image_converter-0.1.1/README.md` & `pyconvertapi_image_converter-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter/__init__.py` & `pyconvertapi_image_converter-0.1.2/pyconvertapi_image_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter/image_converter.py` & `pyconvertapi_image_converter-0.1.2/pyconvertapi_image_converter/image_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,11 +138,11 @@
     def _get_supported_images_in_dir(self, dir_path: str):
         dir_contents = os.listdir(dir_path)
         dir_files = filter(lambda content: os.path.isfile(f"{dir_path}/{content}"), dir_contents)
         dir_images = []
         for file in dir_files:
             file_path = os.path.join(dir_path, file)
             _, fmt = self._get_file_attr(file_path)
-            if fmt in py:
+            if fmt in from_formats:
                 dir_images.append(file_path)
         return dir_images
```

### Comparing `pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter.egg-info/PKG-INFO` & `pyconvertapi_image_converter-0.1.2/pyconvertapi_image_converter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconvertapi-image-converter
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyConvertAPI Image Converter is a Python library for converting images to different formats using ConvertAPI
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/pyconvertapi_image_converter
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/pyconvertapi_image_converter/issues
 Project-URL: Repository, https://github.com/ti-oluwa/pyconvertapi_image_converter
 Keywords: Image format conversion,ConvertAPI
```

### Comparing `pyconvertapi_image_converter-0.1.1/pyproject.toml` & `pyconvertapi_image_converter-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyconvertapi_image_converter"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 maintainers = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 description = "PyConvertAPI Image Converter is a Python library for converting images to different formats using ConvertAPI"
```

