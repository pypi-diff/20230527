# Comparing `tmp/datapipe_core-0.12.0.tar.gz` & `tmp/datapipe_core-0.12.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapipe_core-0.12.0.tar", max compression
+gzip compressed data, was "datapipe_core-0.12.0a1.tar", max compression
```

## Comparing `datapipe_core-0.12.0.tar` & `datapipe_core-0.12.0a1.tar`

### file list

```diff
@@ -1,22 +1,27 @@
--rw-r--r--   0        0        0     1514 2022-12-26 14:30:45.008686 datapipe_core-0.12.0/LICENSE
--rw-r--r--   0        0        0      555 2023-05-27 15:40:41.103405 datapipe_core-0.12.0/README.md
--rw-r--r--   0        0        0        0 2022-12-26 14:30:45.008686 datapipe_core-0.12.0/datapipe/__init__.py
--rw-r--r--   0        0        0    13078 2023-05-27 15:20:07.573406 datapipe_core-0.12.0/datapipe/cli.py
--rw-r--r--   0        0        0    13829 2023-05-27 15:20:07.573406 datapipe_core-0.12.0/datapipe/compute.py
--rw-r--r--   0        0        0    23696 2023-05-27 15:40:41.103405 datapipe_core-0.12.0/datapipe/core_steps.py
--rw-r--r--   0        0        0     8474 2023-05-27 15:20:07.573406 datapipe_core-0.12.0/datapipe/datatable.py
--rw-r--r--   0        0        0     4540 2023-05-27 15:20:07.573406 datapipe_core-0.12.0/datapipe/event_logger.py
--rw-r--r--   0        0        0     4168 2023-05-27 15:20:07.573406 datapipe_core-0.12.0/datapipe/lints.py
--rw-r--r--   0        0        0    19067 2023-05-27 15:20:07.573406 datapipe_core-0.12.0/datapipe/metastore.py
--rw-r--r--   0        0        0      969 2023-03-18 21:03:17.847655 datapipe_core-0.12.0/datapipe/run_config.py
--rw-r--r--   0        0        0        0 2022-12-26 14:30:45.008686 datapipe_core-0.12.0/datapipe/store/__init__.py
--rw-r--r--   0        0        0     8159 2023-05-27 15:20:07.573406 datapipe_core-0.12.0/datapipe/store/database.py
--rw-r--r--   0        0        0    16835 2023-05-27 15:20:07.573406 datapipe_core-0.12.0/datapipe/store/filedir.py
--rw-r--r--   0        0        0     3595 2023-03-18 21:02:49.286406 datapipe_core-0.12.0/datapipe/store/milvus.py
--rw-r--r--   0        0        0     1337 2023-03-18 21:02:52.117521 datapipe_core-0.12.0/datapipe/store/pandas.py
--rw-r--r--   0        0        0     8670 2023-05-27 15:20:07.573406 datapipe_core-0.12.0/datapipe/store/qdrant.py
--rw-r--r--   0        0        0     3210 2023-03-18 21:02:55.387534 datapipe_core-0.12.0/datapipe/store/redis.py
--rw-r--r--   0        0        0     3877 2023-03-18 21:02:58.537544 datapipe_core-0.12.0/datapipe/store/table_store.py
--rw-r--r--   0        0        0     3015 2023-05-27 15:20:07.573406 datapipe_core-0.12.0/datapipe/types.py
--rw-r--r--   0        0        0     2041 2023-05-27 15:40:41.103405 datapipe_core-0.12.0/pyproject.toml
--rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 datapipe_core-0.12.0/PKG-INFO
+-rw-r--r--   0        0        0     1514 2022-12-26 14:30:45.008686 datapipe_core-0.12.0a1/LICENSE
+-rw-r--r--   0        0        0        0 2022-12-26 14:30:45.008686 datapipe_core-0.12.0a1/datapipe/__init__.py
+-rw-r--r--   0        0        0    13078 2023-05-26 11:45:32.195995 datapipe_core-0.12.0a1/datapipe/cli.py
+-rw-r--r--   0        0        0    13829 2023-05-26 11:13:46.820252 datapipe_core-0.12.0a1/datapipe/compute.py
+-rw-r--r--   0        0        0    23567 2023-05-26 11:45:32.195995 datapipe_core-0.12.0a1/datapipe/core_steps.py
+-rw-r--r--   0        0        0     8474 2023-05-26 11:13:46.820252 datapipe_core-0.12.0a1/datapipe/datatable.py
+-rw-r--r--   0        0        0     4540 2023-05-08 09:40:20.336765 datapipe_core-0.12.0a1/datapipe/event_logger.py
+-rw-r--r--   0        0        0     4168 2023-05-26 11:48:22.667838 datapipe_core-0.12.0a1/datapipe/lints.py
+-rw-r--r--   0        0        0    19067 2023-05-26 11:45:32.195995 datapipe_core-0.12.0a1/datapipe/metastore.py
+-rw-r--r--   0        0        0      969 2023-03-18 21:03:17.847655 datapipe_core-0.12.0a1/datapipe/run_config.py
+-rw-r--r--   0        0        0        0 2022-12-26 14:30:45.008686 datapipe_core-0.12.0a1/datapipe/store/__init__.py
+-rw-r--r--   0        0        0      161 2022-12-26 15:39:05.557025 datapipe_core-0.12.0a1/datapipe/store/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     9522 2023-05-26 11:13:47.950258 datapipe_core-0.12.0a1/datapipe/store/__pycache__/database.cpython-310.pyc
+-rw-r--r--   0        0        0    16270 2023-05-08 09:40:22.086794 datapipe_core-0.12.0a1/datapipe/store/__pycache__/filedir.cpython-310.pyc
+-rw-r--r--   0        0        0     4269 2023-03-20 19:51:04.220261 datapipe_core-0.12.0a1/datapipe/store/__pycache__/milvus.cpython-310.pyc
+-rw-r--r--   0        0        0     1880 2023-03-18 21:02:53.257528 datapipe_core-0.12.0a1/datapipe/store/__pycache__/pandas.cpython-310.pyc
+-rw-r--r--   0        0        0     4518 2023-03-18 21:02:56.677538 datapipe_core-0.12.0a1/datapipe/store/__pycache__/redis.cpython-310.pyc
+-rw-r--r--   0        0        0     4923 2023-03-18 21:02:59.587547 datapipe_core-0.12.0a1/datapipe/store/__pycache__/table_store.cpython-310.pyc
+-rw-r--r--   0        0        0     8159 2023-05-26 11:13:46.820252 datapipe_core-0.12.0a1/datapipe/store/database.py
+-rw-r--r--   0        0        0    16835 2023-05-08 09:40:20.346765 datapipe_core-0.12.0a1/datapipe/store/filedir.py
+-rw-r--r--   0        0        0     3595 2023-03-18 21:02:49.286406 datapipe_core-0.12.0a1/datapipe/store/milvus.py
+-rw-r--r--   0        0        0     1337 2023-03-18 21:02:52.117521 datapipe_core-0.12.0a1/datapipe/store/pandas.py
+-rw-r--r--   0        0        0     3210 2023-03-18 21:02:55.387534 datapipe_core-0.12.0a1/datapipe/store/redis.py
+-rw-r--r--   0        0        0     3877 2023-03-18 21:02:58.537544 datapipe_core-0.12.0a1/datapipe/store/table_store.py
+-rw-r--r--   0        0        0     3015 2023-05-08 09:40:20.346765 datapipe_core-0.12.0a1/datapipe/types.py
+-rw-r--r--   0        0        0     1830 2023-05-26 11:46:17.730111 datapipe_core-0.12.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 datapipe_core-0.12.0a1/PKG-INFO
```

### Comparing `datapipe_core-0.12.0/LICENSE` & `datapipe_core-0.12.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.12.0/datapipe/cli.py` & `datapipe_core-0.12.0a1/datapipe/cli.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.12.0/datapipe/compute.py` & `datapipe_core-0.12.0a1/datapipe/compute.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.12.0/datapipe/core_steps.py` & `datapipe_core-0.12.0a1/datapipe/core_steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -713,21 +713,16 @@
             run_config=run_config,
         )
 
         table.meta_table.mark_rows_deleted(stale_idx, now=now)
 
 
 class UpdateExternalTable(PipelineStep):
-    def __init__(
-        self,
-        output: str,
-        labels: Optional[Labels] = None,
-    ) -> None:
+    def __init__(self, output: str) -> None:
         self.output_table_name = output
-        self.labels = labels
 
     def build_compute(self, ds: DataStore, catalog: Catalog) -> List[ComputeStep]:
         def transform_func(
             ds: DataStore,
             input_dts: List[DataTable],
             output_dts: List[DataTable],
             run_config: Optional[RunConfig],
@@ -737,10 +732,9 @@
 
         return [
             DatatableTransformStep(
                 name=f"update_{self.output_table_name}",
                 func=cast(DatatableTransformFunc, transform_func),
                 input_dts=[],
                 output_dts=[catalog.get_datatable(ds, self.output_table_name)],
-                labels=self.labels,
             )
         ]
```

### Comparing `datapipe_core-0.12.0/datapipe/datatable.py` & `datapipe_core-0.12.0a1/datapipe/datatable.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.12.0/datapipe/event_logger.py` & `datapipe_core-0.12.0a1/datapipe/event_logger.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.12.0/datapipe/lints.py` & `datapipe_core-0.12.0a1/datapipe/lints.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.12.0/datapipe/metastore.py` & `datapipe_core-0.12.0a1/datapipe/metastore.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.12.0/datapipe/run_config.py` & `datapipe_core-0.12.0a1/datapipe/run_config.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.12.0/datapipe/store/database.py` & `datapipe_core-0.12.0a1/datapipe/store/database.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.12.0/datapipe/store/filedir.py` & `datapipe_core-0.12.0a1/datapipe/store/filedir.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.12.0/datapipe/store/milvus.py` & `datapipe_core-0.12.0a1/datapipe/store/milvus.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.12.0/datapipe/store/pandas.py` & `datapipe_core-0.12.0a1/datapipe/store/pandas.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.12.0/datapipe/store/redis.py` & `datapipe_core-0.12.0a1/datapipe/store/redis.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.12.0/datapipe/store/table_store.py` & `datapipe_core-0.12.0a1/datapipe/store/table_store.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.12.0/datapipe/types.py` & `datapipe_core-0.12.0a1/datapipe/types.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.12.0/pyproject.toml` & `datapipe_core-0.12.0a1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 [tool.poetry]
 name = "datapipe-core"
-version = "0.12.0"
-description = "`datapipe` is a realtime incremental ETL library for Python application"
-readme = "README.md"
-repository = "https://github.com/epoch8/datapipe"
+version = "0.12.0-alpha.1"
+description = ""
 authors = ["Andrey Tatarinov <a@tatarinov.co>"]
 packages = [
     { include = "datapipe" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
@@ -36,15 +34,14 @@
 
 xlrd = {version=">=2.0.1", optional=true}
 openpyxl = {version=">=3.0.7", optional=true}
 redis = {version="^4.3.4", optional=true}
 
 pysqlite3-binary = {version="^0.5.0", optional=true}
 sqlalchemy-pysqlite3-binary = {version="^0.0.4", optional=true}
-qdrant-client = {version="^1.1.7", optional=true}
 
 click = ">=7.1.2"
 rich = "^13.3.2"
 
 # Copypaste without thinking from https://github.com/meltano/sdk/blob/main/pyproject.toml
 sphinx = {version = ">=4.5,<6.0", optional = true}
 myst-parser = {version = ">=0.17.2,<1.1.0", optional = true}
@@ -53,15 +50,14 @@
 
 sqlite = ["pysqlite3-binary", "sqlalchemy-pysqlite3-binary"]
 excel = ["xlrd", "openpyxl"]
 milvus = ["pymilvus"]
 gcsfs = ["gcsfs"]
 s3fs = ["s3fs"]
 redis = ["redis"]
-qdrant = ["qdrant-client"]
 
 docs = ["sphinx", "myst-parser"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 flake8 = "*"
 mypy = "*"
```

### Comparing `datapipe_core-0.12.0/PKG-INFO` & `datapipe_core-0.12.0a1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: datapipe-core
-Version: 0.12.0
-Summary: `datapipe` is a realtime incremental ETL library for Python application
-Home-page: https://github.com/epoch8/datapipe
+Version: 0.12.0a1
+Summary: 
 Author: Andrey Tatarinov
 Author-email: a@tatarinov.co
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: docs
 Provides-Extra: excel
 Provides-Extra: gcsfs
 Provides-Extra: milvus
-Provides-Extra: qdrant
 Provides-Extra: redis
 Provides-Extra: s3fs
 Provides-Extra: sqlite
 Requires-Dist: Pillow (>=9.0.0,<10.0.0)
 Requires-Dist: PyYAML (>=5.3.1)
 Requires-Dist: SQLAlchemy (>=1.4.25,<2.0.0)
 Requires-Dist: cityhash (>=0.4.2,<0.5.0)
@@ -33,35 +31,15 @@
 Requires-Dist: opentelemetry-api (>=1.8.0,<2.0.0)
 Requires-Dist: opentelemetry-instrumentation-sqlalchemy (==0.35b0)
 Requires-Dist: opentelemetry-sdk (>=1.8.0,<2.0.0)
 Requires-Dist: pandas (>=1.2.0,<2.0.0)
 Requires-Dist: psycopg2_binary (>=2.8.4)
 Requires-Dist: pymilvus (>=2.0.2,<3.0.0) ; extra == "milvus"
 Requires-Dist: pysqlite3-binary (>=0.5.0,<0.6.0) ; extra == "sqlite"
-Requires-Dist: qdrant-client (>=1.1.7,<2.0.0) ; extra == "qdrant"
 Requires-Dist: redis (>=4.3.4,<5.0.0) ; extra == "redis"
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: s3fs (>=2021.11.1) ; extra == "s3fs"
 Requires-Dist: sphinx (>=4.5,<6.0) ; extra == "docs"
 Requires-Dist: sqlalchemy-pysqlite3-binary (>=0.0.4,<0.0.5) ; extra == "sqlite"
 Requires-Dist: tqdm (>=4.60.0)
 Requires-Dist: traceback-with-variables (>=2.0.4,<3.0.0)
 Requires-Dist: xlrd (>=2.0.1) ; extra == "excel"
-Project-URL: Repository, https://github.com/epoch8/datapipe
-Description-Content-Type: text/markdown
-
-# Datapipe
-
-`datapipe` is a realtime incremental ETL library for Python application.
-
-# Version compatibility
-
-At the moment, the datapipe library is under active development. Versions:
-`v0.*.*`
-
-It should be expected that each minor version is not backward compatible with
-the previous one. That is, `v0.7.0` is not compatible with `v0.6.1`. Dependencies
-should be fixed to the exact minor version.
-
-After stabilization and transition to the major version `v1.*.*`, the common
-rules will apply: all versions with the same major component are compatible.
-
```

