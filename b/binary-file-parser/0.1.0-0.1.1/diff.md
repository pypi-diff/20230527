# Comparing `tmp/binary-file-parser-0.1.0.tar.gz` & `tmp/binary-file-parser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binary-file-parser-0.1.0.tar", last modified: Tue May  2 06:12:19 2023, max compression
+gzip compressed data, was "binary-file-parser-0.1.1.tar", last modified: Sat May 27 04:15:56 2023, max compression
```

## Comparing `binary-file-parser-0.1.0.tar` & `binary-file-parser-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 06:12:19.172717 binary-file-parser-0.1.0/
--rw-rw-rw-   0        0        0     1084 2022-12-14 12:48:09.000000 binary-file-parser-0.1.0/LICENSE
--rw-rw-rw-   0        0        0        0 2022-12-15 05:10:52.000000 binary-file-parser-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3411 2023-05-02 06:12:19.171717 binary-file-parser-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1482 2022-12-18 10:54:12.000000 binary-file-parser-0.1.0/README.md
--rw-rw-rw-   0        0        0      908 2023-03-21 02:27:40.000000 binary-file-parser-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 06:12:19.172717 binary-file-parser-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 06:12:18.929716 binary-file-parser-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 06:12:18.956715 binary-file-parser-0.1.0/src/binary_file_parser/
--rw-rw-rw-   0        0        0      290 2023-05-02 04:00:31.000000 binary-file-parser-0.1.0/src/binary_file_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 06:12:19.017718 binary-file-parser-0.1.0/src/binary_file_parser/errors/
--rw-rw-rw-   0        0        0      118 2022-12-15 18:24:53.000000 binary-file-parser-0.1.0/src/binary_file_parser/errors/CompressionError.py
--rw-rw-rw-   0        0        0       42 2022-12-15 07:13:59.000000 binary-file-parser-0.1.0/src/binary_file_parser/errors/ParsingError.py
--rw-rw-rw-   0        0        0      114 2022-12-15 18:24:20.000000 binary-file-parser-0.1.0/src/binary_file_parser/errors/VersionError.py
--rw-rw-rw-   0        0        0      128 2022-12-15 07:16:50.000000 binary-file-parser-0.1.0/src/binary_file_parser/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 06:12:19.081718 binary-file-parser-0.1.0/src/binary_file_parser/retrievers/
--rw-rw-rw-   0        0        0     2647 2023-02-18 09:06:26.000000 binary-file-parser-0.1.0/src/binary_file_parser/retrievers/MapValidate.py
--rw-rw-rw-   0        0        0     2272 2023-04-24 11:23:48.000000 binary-file-parser-0.1.0/src/binary_file_parser/retrievers/RetreiverCombiner.py
--rw-rw-rw-   0        0        0     1518 2023-04-24 11:16:38.000000 binary-file-parser-0.1.0/src/binary_file_parser/retrievers/RetreiverRef.py
--rw-rw-rw-   0        0        0    11222 2023-05-02 03:50:09.000000 binary-file-parser-0.1.0/src/binary_file_parser/retrievers/Retriever.py
--rw-rw-rw-   0        0        0      199 2023-04-21 01:37:15.000000 binary-file-parser-0.1.0/src/binary_file_parser/retrievers/__init__.py
--rw-rw-rw-   0        0        0    15418 2023-05-02 04:12:57.000000 binary-file-parser-0.1.0/src/binary_file_parser/retrievers/base_struct.py
-drwxrwxrwx   0        0        0        0 2023-05-02 06:12:19.169717 binary-file-parser-0.1.0/src/binary_file_parser/types/
--rw-rw-rw-   0        0        0     6438 2023-04-21 03:06:40.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/Array.py
--rw-rw-rw-   0        0        0      928 2023-04-18 12:21:20.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/Bool.py
--rw-rw-rw-   0        0        0     2796 2022-11-29 16:43:10.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/ByteStream.py
--rw-rw-rw-   0        0        0      855 2023-04-18 12:21:20.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/Bytes.py
--rw-rw-rw-   0        0        0      867 2023-04-18 12:21:20.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/Float.py
--rw-rw-rw-   0        0        0      987 2023-04-18 12:21:20.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/Int.py
--rw-rw-rw-   0        0        0     1345 2023-04-21 02:01:03.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/Parseable.py
--rw-rw-rw-   0        0        0     2584 2023-04-21 03:37:25.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/RefList.py
--rw-rw-rw-   0        0        0     3037 2023-04-18 12:21:20.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/Str.py
--rw-rw-rw-   0        0        0      545 2023-04-21 02:02:51.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/__init__.py
--rw-rw-rw-   0        0        0      596 2023-05-02 03:35:56.000000 binary-file-parser-0.1.0/src/binary_file_parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 06:12:18.976715 binary-file-parser-0.1.0/src/binary_file_parser.egg-info/
--rw-rw-rw-   0        0        0     3411 2023-05-02 06:12:18.000000 binary-file-parser-0.1.0/src/binary_file_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1209 2023-05-02 06:12:18.000000 binary-file-parser-0.1.0/src/binary_file_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 06:12:18.000000 binary-file-parser-0.1.0/src/binary_file_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-02 06:12:18.000000 binary-file-parser-0.1.0/src/binary_file_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-02 06:12:18.000000 binary-file-parser-0.1.0/src/binary_file_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 04:15:56.211383 binary-file-parser-0.1.1/
+-rw-rw-rw-   0        0        0     1084 2022-12-14 12:48:09.000000 binary-file-parser-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0        0 2022-12-15 05:10:52.000000 binary-file-parser-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5959 2023-05-27 04:15:56.210384 binary-file-parser-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4030 2023-05-27 04:13:45.000000 binary-file-parser-0.1.1/README.md
+-rw-rw-rw-   0        0        0      908 2023-05-27 04:15:27.000000 binary-file-parser-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 04:15:56.211383 binary-file-parser-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 04:15:56.056393 binary-file-parser-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 04:15:56.073417 binary-file-parser-0.1.1/src/binary_file_parser/
+-rw-rw-rw-   0        0        0      290 2023-05-02 04:00:31.000000 binary-file-parser-0.1.1/src/binary_file_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 04:15:56.120382 binary-file-parser-0.1.1/src/binary_file_parser/errors/
+-rw-rw-rw-   0        0        0      118 2022-12-15 18:24:53.000000 binary-file-parser-0.1.1/src/binary_file_parser/errors/CompressionError.py
+-rw-rw-rw-   0        0        0       42 2022-12-15 07:13:59.000000 binary-file-parser-0.1.1/src/binary_file_parser/errors/ParsingError.py
+-rw-rw-rw-   0        0        0      114 2022-12-15 18:24:20.000000 binary-file-parser-0.1.1/src/binary_file_parser/errors/VersionError.py
+-rw-rw-rw-   0        0        0      128 2022-12-15 07:16:50.000000 binary-file-parser-0.1.1/src/binary_file_parser/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 04:15:56.144435 binary-file-parser-0.1.1/src/binary_file_parser/retrievers/
+-rw-rw-rw-   0        0        0     2647 2023-02-18 09:06:26.000000 binary-file-parser-0.1.1/src/binary_file_parser/retrievers/MapValidate.py
+-rw-rw-rw-   0        0        0     2272 2023-04-24 11:23:48.000000 binary-file-parser-0.1.1/src/binary_file_parser/retrievers/RetreiverCombiner.py
+-rw-rw-rw-   0        0        0     1518 2023-04-24 11:16:38.000000 binary-file-parser-0.1.1/src/binary_file_parser/retrievers/RetreiverRef.py
+-rw-rw-rw-   0        0        0    11222 2023-05-02 03:50:09.000000 binary-file-parser-0.1.1/src/binary_file_parser/retrievers/Retriever.py
+-rw-rw-rw-   0        0        0      199 2023-04-21 01:37:15.000000 binary-file-parser-0.1.1/src/binary_file_parser/retrievers/__init__.py
+-rw-rw-rw-   0        0        0    15828 2023-05-27 04:13:34.000000 binary-file-parser-0.1.1/src/binary_file_parser/retrievers/base_struct.py
+drwxrwxrwx   0        0        0        0 2023-05-27 04:15:56.209426 binary-file-parser-0.1.1/src/binary_file_parser/types/
+-rw-rw-rw-   0        0        0     6438 2023-04-21 03:06:40.000000 binary-file-parser-0.1.1/src/binary_file_parser/types/Array.py
+-rw-rw-rw-   0        0        0      928 2023-04-18 12:21:20.000000 binary-file-parser-0.1.1/src/binary_file_parser/types/Bool.py
+-rw-rw-rw-   0        0        0     2796 2022-11-29 16:43:10.000000 binary-file-parser-0.1.1/src/binary_file_parser/types/ByteStream.py
+-rw-rw-rw-   0        0        0      855 2023-04-18 12:21:20.000000 binary-file-parser-0.1.1/src/binary_file_parser/types/Bytes.py
+-rw-rw-rw-   0        0        0      867 2023-04-18 12:21:20.000000 binary-file-parser-0.1.1/src/binary_file_parser/types/Float.py
+-rw-rw-rw-   0        0        0      987 2023-04-18 12:21:20.000000 binary-file-parser-0.1.1/src/binary_file_parser/types/Int.py
+-rw-rw-rw-   0        0        0     1345 2023-04-21 02:01:03.000000 binary-file-parser-0.1.1/src/binary_file_parser/types/Parseable.py
+-rw-rw-rw-   0        0        0     2584 2023-04-21 03:37:25.000000 binary-file-parser-0.1.1/src/binary_file_parser/types/RefList.py
+-rw-rw-rw-   0        0        0     3037 2023-04-18 12:21:20.000000 binary-file-parser-0.1.1/src/binary_file_parser/types/Str.py
+-rw-rw-rw-   0        0        0      545 2023-04-21 02:02:51.000000 binary-file-parser-0.1.1/src/binary_file_parser/types/__init__.py
+-rw-rw-rw-   0        0        0      596 2023-05-02 03:35:56.000000 binary-file-parser-0.1.1/src/binary_file_parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-27 04:15:56.098416 binary-file-parser-0.1.1/src/binary_file_parser.egg-info/
+-rw-rw-rw-   0        0        0     5959 2023-05-27 04:15:56.000000 binary-file-parser-0.1.1/src/binary_file_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1209 2023-05-27 04:15:56.000000 binary-file-parser-0.1.1/src/binary_file_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 04:15:56.000000 binary-file-parser-0.1.1/src/binary_file_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-27 04:15:56.000000 binary-file-parser-0.1.1/src/binary_file_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-27 04:15:56.000000 binary-file-parser-0.1.1/src/binary_file_parser.egg-info/top_level.txt
```

### Comparing `binary-file-parser-0.1.0/LICENSE` & `binary-file-parser-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.0/pyproject.toml` & `binary-file-parser-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=57.4.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "binary-file-parser"
-version = "0.1.0"
+version = "0.1.1"
 description = "Read/Write binary files after describing their specifications in code (similar to an ORM table schema)"
 readme = "README.md"
 authors = [{ name = "Divy1211", email = "divy1211.dc@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `binary-file-parser-0.1.0/src/binary_file_parser/retrievers/MapValidate.py` & `binary-file-parser-0.1.1/src/binary_file_parser/retrievers/MapValidate.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.0/src/binary_file_parser/retrievers/RetreiverCombiner.py` & `binary-file-parser-0.1.1/src/binary_file_parser/retrievers/RetreiverCombiner.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.0/src/binary_file_parser/retrievers/RetreiverRef.py` & `binary-file-parser-0.1.1/src/binary_file_parser/retrievers/RetreiverRef.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.0/src/binary_file_parser/retrievers/Retriever.py` & `binary-file-parser-0.1.1/src/binary_file_parser/retrievers/Retriever.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.0/src/binary_file_parser/retrievers/base_struct.py` & `binary-file-parser-0.1.1/src/binary_file_parser/retrievers/base_struct.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,17 @@
                     init = retriever.from_default(self)
                 setattr(self, retriever.p_name, init)
 
             size += retriever.default.size if retriever.dtype.is_struct else retriever.dtype.size
         super().__init__(size)
 
     def __init_subclass__(cls, **kwargs):
+        """
+        Note: subclasses of BaseStruct which intend to act as ABCs need to override this
+        """
         cls._retrievers, BaseStruct._retrievers = cls._retrievers.copy(), []
         cls._refs, BaseStruct._refs = cls._refs.copy(), []
         cls._combiners, BaseStruct._combiners = cls._combiners.copy(), []
 
     @property
     def is_struct(self) -> bool:
         return True
@@ -143,15 +146,16 @@
                 obj.parent = new_parent
         self._parent = new_parent
 
     @property
     def retriever_name_value_map(self) -> dict[str]:
         map_ = {}
         for retriever in self._retrievers:
-            map_[retriever.p_name] = getattr(self, retriever.p_name)
+            if retriever.supported(self.struct_ver):
+                map_[retriever.p_name] = getattr(self, retriever.p_name)
         return map_
 
     @classmethod
     def get_version(cls, stream: ByteStream, struct_ver: Version = Version((0,)), parent: BaseStruct = None) -> Version:
         """
         If defined, the struct will be versioned and values in the struct which are not supported in the version that is
         read will be skipped
@@ -190,14 +194,22 @@
         :raises CompressionError: - When unimplemented
         """
         raise CompressionError(
             "Unable to write object to file. "
             "A Structure with compressed section needs to implement 'compress' classmethod."
         )
 
+    def map(self) -> BaseStruct:
+        """
+        This method is called after a struct is read from bytes to allow any modifications post reading
+
+        :return: A BaseStruct instance
+        """
+        return self
+
     @classmethod
     def from_stream(
         cls, stream: ByteStream, *, struct_ver: Version = Version((0,)), strict: bool = False,
         show_progress: bool = False, parent: BaseStruct = None
     ) -> BaseStruct:
         """
         Create a struct object from a ByteStream
@@ -234,15 +246,15 @@
 
         if stream.progress != file_len and strict:
             raise ParsingError(
                 f"{file_len - stream.progress} bytes are left after parsing all retrievers successfully:\n"
                 f"{stream.remaining()}"
             )
 
-        return instance
+        return instance.map()
 
     @classmethod
     def from_bytes(cls, bytes_: bytes, *, struct_ver: Version = Version((0,)), strict = False) -> BaseStruct:
         """
         Create a struct object from bytes
 
         :param bytes_: The bytes to create the struct object from
```

### Comparing `binary-file-parser-0.1.0/src/binary_file_parser/types/Array.py` & `binary-file-parser-0.1.1/src/binary_file_parser/types/Array.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.0/src/binary_file_parser/types/Bool.py` & `binary-file-parser-0.1.1/src/binary_file_parser/types/Bool.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.0/src/binary_file_parser/types/ByteStream.py` & `binary-file-parser-0.1.1/src/binary_file_parser/types/ByteStream.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.0/src/binary_file_parser/types/Bytes.py` & `binary-file-parser-0.1.1/src/binary_file_parser/types/Bytes.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.0/src/binary_file_parser/types/Float.py` & `binary-file-parser-0.1.1/src/binary_file_parser/types/Float.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.0/src/binary_file_parser/types/Int.py` & `binary-file-parser-0.1.1/src/binary_file_parser/types/Int.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.0/src/binary_file_parser/types/Parseable.py` & `binary-file-parser-0.1.1/src/binary_file_parser/types/Parseable.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.0/src/binary_file_parser/types/RefList.py` & `binary-file-parser-0.1.1/src/binary_file_parser/types/RefList.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.0/src/binary_file_parser/types/Str.py` & `binary-file-parser-0.1.1/src/binary_file_parser/types/Str.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.0/src/binary_file_parser/types/__init__.py` & `binary-file-parser-0.1.1/src/binary_file_parser/types/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.0/src/binary_file_parser/utils.py` & `binary-file-parser-0.1.1/src/binary_file_parser/utils.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.0/src/binary_file_parser.egg-info/SOURCES.txt` & `binary-file-parser-0.1.1/src/binary_file_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

