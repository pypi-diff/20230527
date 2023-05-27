# Comparing `tmp/rocksdict-0.3.8-cp39-none-win_amd64.whl.zip` & `tmp/rocksdict-0.3.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2696724 bytes, number of entries: 8
--rw-r--r--  4.6 unx     6702 b- defN 23-Mar-21 09:00 rocksdict-0.3.8.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 23-Mar-21 09:00 rocksdict-0.3.8.dist-info/WHEEL
--rw-r--r--  4.6 unx     1084 b- defN 23-Mar-21 09:00 rocksdict-0.3.8.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx        0 b- defN 23-Mar-21 09:00 rocksdict/py.typed
--rw-r--r--  4.6 unx    25182 b- defN 23-Mar-21 09:00 rocksdict/rocksdict.pyi
--rw-r--r--  4.6 unx     1078 b- defN 23-Mar-21 09:00 rocksdict/__init__.py
--rwxr-xr-x  4.6 unx  6572032 b- defN 23-Mar-21 09:00 rocksdict/rocksdict.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      645 b- defN 23-Mar-21 09:00 rocksdict-0.3.8.dist-info/RECORD
-8 files, 6606818 bytes uncompressed, 2695606 bytes compressed:  59.2%
+Zip file size: 2677848 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     6702 b- defN 23-Mar-22 12:31 rocksdict-0.3.9.dist-info/METADATA
+-rw-r--r--  4.6 unx       95 b- defN 23-Mar-22 12:31 rocksdict-0.3.9.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1084 b- defN 23-Mar-22 12:31 rocksdict-0.3.9.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx        0 b- defN 23-Mar-22 12:31 rocksdict/py.typed
+-rw-r--r--  4.6 unx    25711 b- defN 23-Mar-22 12:31 rocksdict/rocksdict.pyi
+-rw-r--r--  4.6 unx     1078 b- defN 23-Mar-22 12:31 rocksdict/__init__.py
+-rwxr-xr-x  4.6 unx  6503936 b- defN 23-Mar-22 12:31 rocksdict/rocksdict.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      645 b- defN 23-Mar-22 12:31 rocksdict-0.3.9.dist-info/RECORD
+8 files, 6539251 bytes uncompressed, 2676730 bytes compressed:  59.1%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: rocksdict-0.3.8.dist-info/METADATA
+Filename: rocksdict-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: rocksdict-0.3.8.dist-info/WHEEL
+Filename: rocksdict-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: rocksdict-0.3.8.dist-info/license_files/LICENSE
+Filename: rocksdict-0.3.9.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: rocksdict/py.typed
 Comment: 
 
 Filename: rocksdict/rocksdict.pyi
 Comment: 
 
 Filename: rocksdict/__init__.py
 Comment: 
 
 Filename: rocksdict/rocksdict.cp39-win_amd64.pyd
 Comment: 
 
-Filename: rocksdict-0.3.8.dist-info/RECORD
+Filename: rocksdict-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rocksdict/rocksdict.pyi

```diff
@@ -283,15 +283,15 @@
     @property
     def user_key_length(self) -> int: ...
     @user_key_length.setter
     def user_key_length(self, v: int) -> None: ...
     def __init__(self) -> PlainTableFactoryOptions: ...
 
 class ReadOptions:
-    def __init__(self, raw_mode: bool = False) -> ReadOptions: ...
+    def __init__(self) -> ReadOptions: ...
     def fill_cache(self) -> None: ...
     def set_background_purge_on_iterator_cleanup(self, v: bool) -> None: ...
     def set_ignore_range_deletions(self, v: bool) -> None: ...
     def set_iterate_lower_bound(self, key: Union[str, int, float, bytes, bool]) -> None: ...
     def set_iterate_upper_bound(self, key: Union[str, int, float, bytes, bool]) -> None: ...
     def set_max_skippable_internal_keys(self, num: int) -> None: ...
     def set_pin_data(self, v: bool) -> None: ...
@@ -374,17 +374,27 @@
     def __enter__(self) -> Rdict: ...
     def set_read_options(self, read_opt: ReadOptions) -> None: ...
     def set_write_options(self, write_opt: WriteOptions) -> None: ...
     def __contains__(self, key: Union[str, int, float, bytes, bool]) -> bool: ...
     def __delitem__(self, key: Union[str, int, float, bytes, bool]) -> None: ...
     def __getitem__(self, key: Union[str, int, float, bytes, bool, List[str], List[int], List[float], List[bytes], List[bool]]) -> Any: ...
     def __setitem__(self, key: Union[str, int, float, bytes, bool], value: Any) -> None: ...
-    def delete(self, key: Union[str, int, float, bytes, bool]) -> None: ...
-    def get(self, key: Union[str, int, float, bytes, bool, List[str], List[int], List[float], List[bytes], List[bool]], default: Any = None) -> Any | None: ...
-    def put(self, key: Union[str, int, float, bytes, bool], value: Any) -> None: ...
+    def get(self,
+            key: Union[str, int, float, bytes, bool, List[str], List[int], List[float], List[bytes], List[bool]],
+            default: Any = None,
+            read_opt: Union[ReadOptions, None] = None) -> Any | None: ...
+    def put(self,
+            key: Union[str, int, float, bytes, bool],
+            value: Any,
+            write_opt: Union[WriteOptions, None] = None) -> None: ...
+    def delete(self, key: Union[str, int, float, bytes, bool], write_opt: Union[WriteOptions, None] = None) -> None: ...
+    def key_may_exist(self,
+                      key: Union[str, int, float, bytes, bool],
+                      fetch: bool = False,
+                      read_opt = None) -> Union[bool, Tuple[bool, Any]]: ...
     def iter(self, read_opt: Union[ReadOptions, None] = None) -> RdictIter: ...
     def items(self, backwards: bool = False,
               from_key: Union[str, int, float, bytes, bool, None] = None,
               read_opt: Union[ReadOptions, None] = None) -> RdictItems: ...
     def keys(self, backwards: bool = False,
              from_key: Union[str, int, float, bytes, bool, None] = None,
              read_opt: Union[ReadOptions, None] = None) -> RdictKeys: ...
@@ -392,25 +402,28 @@
                from_key: Union[str, int, float, bytes, bool, None] = None,
                read_opt: Union[ReadOptions, None] = None) -> RdictValues: ...
     def ingest_external_file(self, paths: List[str], opts: IngestExternalFileOptions = IngestExternalFileOptions()) -> None: ...
     def get_column_family(self, name: str) -> Rdict: ...
     def get_column_family_handle(self, name: str) -> ColumnFamily: ...
     def drop_column_family(self, name: str) -> None: ...
     def create_column_family(self, name: str, options: Options = Options()) -> Rdict: ...
-    def write(self, write_batch: WriteBatch, write_opt: WriteOptions = WriteOptions()) -> None: ...
-    def delete_range(self, begin: Union[str, int, float, bytes, bool], end: Union[str, int, float, bytes, bool]) -> None: ...
+    def write(self, write_batch: WriteBatch, write_opt: Union[WriteOptions, None] = None) -> None: ...
+    def delete_range(self,
+                     begin: Union[str, int, float, bytes, bool],
+                     end: Union[str, int, float, bytes, bool],
+                     write_opt: Union[WriteOptions, None] = None) -> None: ...
     def snapshot(self) -> Snapshot: ...
     def path(self) -> str: ...
     def set_options(self, options: Dict[str, str]) -> None: ...
     def property_value(self, name: str) -> Union[str, None]: ...
     def property_int_value(self, name: str) -> Union[int, None]: ...
     def latest_sequence_number(self) -> int: ...
     def live_files(self) -> List[Dict[str, Any]]: ...
-    def compact_range(self, begin: Union[str, int, float, bytes, bool],
-                      end: Union[str, int, float, bytes, bool],
+    def compact_range(self, begin: Union[str, int, float, bytes, bool, None],
+                      end: Union[str, int, float, bytes, bool, None],
                       compact_opt: CompactOptions = CompactOptions()) -> None: ...
     def close(self) -> None: ...
     def __exit__(self, exc_type, exc_val, exc_tb) -> None: ...
     def flush(self, wait: bool = True) -> None: ...
     def flush_wal(self, sync: bool = True) -> None: ...
     @staticmethod
     def destroy(path: str, options: Options = Options()) -> None: ...
```

## Comparing `rocksdict-0.3.8.dist-info/METADATA` & `rocksdict-0.3.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocksdict
-Version: 0.3.8
+Version: 0.3.9
 Classifier: Programming Language :: Rust
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Embedded Systems
```

## Comparing `rocksdict-0.3.8.dist-info/license_files/LICENSE` & `rocksdict-0.3.9.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `rocksdict-0.3.8.dist-info/RECORD` & `rocksdict-0.3.9.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-rocksdict-0.3.8.dist-info/METADATA,sha256=Q6TmvXyRY7UBIibiuksg1zrZBm2BLzsga-wSIzjU_zk,6702
-rocksdict-0.3.8.dist-info/WHEEL,sha256=ujIUOIChM84q2okk01hfCTGkfNmymRrIEhkXNzCT0tY,95
-rocksdict-0.3.8.dist-info/license_files/LICENSE,sha256=WZxZ0A9IQbUmTqI6H8Ki2EhpSzEcGLm2Ju4PGNg6d5w,1084
+rocksdict-0.3.9.dist-info/METADATA,sha256=udEsbYfWNRvUZ_A6IJXOOjz2no8WgLmXQy6ADQXPCoo,6702
+rocksdict-0.3.9.dist-info/WHEEL,sha256=ujIUOIChM84q2okk01hfCTGkfNmymRrIEhkXNzCT0tY,95
+rocksdict-0.3.9.dist-info/license_files/LICENSE,sha256=WZxZ0A9IQbUmTqI6H8Ki2EhpSzEcGLm2Ju4PGNg6d5w,1084
 rocksdict/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rocksdict/rocksdict.pyi,sha256=pDichfhTFL3AJN319ILAIHcJdvxTVmmcnIls9z0AWUQ,25182
+rocksdict/rocksdict.pyi,sha256=x2G-a-6lqOMNBp0AzoteEJxeE3OriaBU0tKcarrswTE,25711
 rocksdict/__init__.py,sha256=tV6Mxrvwn-Sa-bhRcbFBrt5Pmr18jXHHDEs-aMaRl74,1078
-rocksdict/rocksdict.cp39-win_amd64.pyd,sha256=OYT_KC-rfxvSyW8dgW87XWHZcA19gsJMkaF9RwshO1E,6572032
-rocksdict-0.3.8.dist-info/RECORD,,
+rocksdict/rocksdict.cp39-win_amd64.pyd,sha256=OJz-EYZoOjQ2HhugDi6Gq7pLsm94Byu_TWI0zxZiKgg,6503936
+rocksdict-0.3.9.dist-info/RECORD,,
```

