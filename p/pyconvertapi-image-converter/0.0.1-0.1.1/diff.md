# Comparing `tmp/pyconvertapi_image_converter-0.0.1.tar.gz` & `tmp/pyconvertapi_image_converter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconvertapi_image_converter-0.0.1.tar", last modified: Sat May 27 14:26:26 2023, max compression
+gzip compressed data, was "pyconvertapi_image_converter-0.1.1.tar", last modified: Sat May 27 15:04:27 2023, max compression
```

## Comparing `pyconvertapi_image_converter-0.0.1.tar` & `pyconvertapi_image_converter-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 14:26:26.694486 pyconvertapi_image_converter-0.0.1/
--rw-rw-rw-   0        0        0     1104 2023-03-19 23:35:37.000000 pyconvertapi_image_converter-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0     4272 2023-05-27 14:26:26.686485 pyconvertapi_image_converter-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3398 2023-05-22 17:33:53.000000 pyconvertapi_image_converter-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 14:26:26.584501 pyconvertapi_image_converter-0.0.1/pyconvertapi_image_converter/
--rw-rw-rw-   0        0        0     1020 2023-05-22 17:34:34.000000 pyconvertapi_image_converter-0.0.1/pyconvertapi_image_converter/__init__.py
--rw-rw-rw-   0        0        0     5677 2023-05-22 17:44:35.000000 pyconvertapi_image_converter-0.0.1/pyconvertapi_image_converter/image_converter.py
-drwxrwxrwx   0        0        0        0 2023-05-27 14:26:26.679480 pyconvertapi_image_converter-0.0.1/pyconvertapi_image_converter.egg-info/
--rw-rw-rw-   0        0        0     4272 2023-05-27 14:26:26.000000 pyconvertapi_image_converter-0.0.1/pyconvertapi_image_converter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-05-27 14:26:26.000000 pyconvertapi_image_converter-0.0.1/pyconvertapi_image_converter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 14:26:26.000000 pyconvertapi_image_converter-0.0.1/pyconvertapi_image_converter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-27 14:26:26.000000 pyconvertapi_image_converter-0.0.1/pyconvertapi_image_converter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-05-27 14:26:26.000000 pyconvertapi_image_converter-0.0.1/pyconvertapi_image_converter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1013 2023-05-27 14:25:19.000000 pyconvertapi_image_converter-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 14:26:26.707484 pyconvertapi_image_converter-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 15:04:27.752842 pyconvertapi_image_converter-0.1.1/
+-rw-rw-rw-   0        0        0     1104 2023-03-19 23:35:37.000000 pyconvertapi_image_converter-0.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0     4272 2023-05-27 15:04:27.737814 pyconvertapi_image_converter-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3398 2023-05-22 17:33:53.000000 pyconvertapi_image_converter-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 15:04:27.602110 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter/
+-rw-rw-rw-   0        0        0     1020 2023-05-22 17:34:34.000000 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter/__init__.py
+-rw-rw-rw-   0        0        0     5818 2023-05-27 14:59:57.000000 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter/image_converter.py
+drwxrwxrwx   0        0        0        0 2023-05-27 15:04:27.736106 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter.egg-info/
+-rw-rw-rw-   0        0        0     4272 2023-05-27 15:04:27.000000 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-05-27 15:04:27.000000 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 15:04:27.000000 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-27 15:04:27.000000 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-05-27 15:04:27.000000 pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1013 2023-05-27 15:02:52.000000 pyconvertapi_image_converter-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 15:04:27.752842 pyconvertapi_image_converter-0.1.1/setup.cfg
```

### Comparing `pyconvertapi_image_converter-0.0.1/LICENSE.md` & `pyconvertapi_image_converter-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyconvertapi_image_converter-0.0.1/PKG-INFO` & `pyconvertapi_image_converter-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconvertapi_image_converter
-Version: 0.0.1
+Version: 0.1.1
 Summary: PyConvertAPI Image Converter is a Python library for converting images to different formats using ConvertAPI
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/pyconvertapi_image_converter
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/pyconvertapi_image_converter/issues
 Project-URL: Repository, https://github.com/ti-oluwa/pyconvertapi_image_converter
 Keywords: Image format conversion,ConvertAPI
```

### Comparing `pyconvertapi_image_converter-0.0.1/README.md` & `pyconvertapi_image_converter-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyconvertapi_image_converter-0.0.1/pyconvertapi_image_converter/__init__.py` & `pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `pyconvertapi_image_converter-0.0.1/pyconvertapi_image_converter/image_converter.py` & `pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter/image_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from_formats = ['jpg', 'png', 'svg', 'jpeg', 'webp', 'tiff', 'jpeg', 'heic', 'ico', 'gif']
 
 class ConvertAPIImageConverter:
     """
     Converts supported image type(s) to specified supported format.
 
     :param api_secret: convertapi secret key
-    :param save_to: path to save converted images to. Defaults to the directory containing the image(s) to convert
+    :param save_to: path to save converted images to.
 
     :attribute image_quality: image quality. Defaults to 90
     :attribute image_dpi: image resolution. Defaults to 326
     :attribute api_secret: convertapi secret key
     :attribute _store_files: whether to store converted files on convertapi servers. Defaults to True
     """
     image_quality: int = 90
@@ -97,15 +97,19 @@
             convertapi.api_secret = self.api_secret
             params = {
                 'ImageResolution': self.image_dpi,
                 'File': path,
                 'ImageQuality': self.image_quality,
                 'StoreFile': self._store_files
             }
-            convertapi.convert(to_format=to_fmt, params=params, from_format=from_fmt).save_files(self.save_to)
+            save_to = os.path.join(self.save_to, name.replace(from_fmt, to_fmt))
+            os.makedirs(os.path.dirname(save_to), exist_ok=True)
+            f = open(save_to, "w")
+            f.close()
+            convertapi.convert(to_format=to_fmt, params=params, from_format=from_fmt).save_files(save_to)
         return None
 
     
     def _convert_images_to(self, path: str, to_fmt: str):
         image_files = self._get_supported_images_in_dir(path)
         # slice image_files into parts of 10
         image_files_slice = [ image_files[i:i + 10] for i in range(0, len(image_files), 10) ]
```

### Comparing `pyconvertapi_image_converter-0.0.1/pyconvertapi_image_converter.egg-info/PKG-INFO` & `pyconvertapi_image_converter-0.1.1/pyconvertapi_image_converter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconvertapi-image-converter
-Version: 0.0.1
+Version: 0.1.1
 Summary: PyConvertAPI Image Converter is a Python library for converting images to different formats using ConvertAPI
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/pyconvertapi_image_converter
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/pyconvertapi_image_converter/issues
 Project-URL: Repository, https://github.com/ti-oluwa/pyconvertapi_image_converter
 Keywords: Image format conversion,ConvertAPI
```

### Comparing `pyconvertapi_image_converter-0.0.1/pyproject.toml` & `pyconvertapi_image_converter-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyconvertapi_image_converter"
-version = "0.0.1"
+version = "0.1.1"
 authors = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 maintainers = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 description = "PyConvertAPI Image Converter is a Python library for converting images to different formats using ConvertAPI"
```

