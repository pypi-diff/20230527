# Comparing `tmp/grai_source_fivetran-0.0.7.tar.gz` & `tmp/grai_source_fivetran-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_fivetran-0.0.7.tar", max compression
+gzip compressed data, was "grai_source_fivetran-0.0.8.tar", max compression
```

## Comparing `grai_source_fivetran-0.0.7.tar` & `grai_source_fivetran-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      420 2023-05-25 16:20:32.597515 grai_source_fivetran-0.0.7/README.md
--rw-r--r--   0        0        0     1020 2023-05-26 19:11:57.309355 grai_source_fivetran-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      119 2023-02-14 16:39:18.542655 grai_source_fivetran-0.0.7/src/grai_source_fivetran/__init__.py
--rw-r--r--   0        0        0     6644 2023-05-19 11:07:12.931545 grai_source_fivetran-0.0.7/src/grai_source_fivetran/adapters.py
--rw-r--r--   0        0        0     2111 2023-05-26 18:51:17.053006 grai_source_fivetran-0.0.7/src/grai_source_fivetran/base.py
--rw-r--r--   0        0        0        0 2023-02-14 16:39:18.543040 grai_source_fivetran-0.0.7/src/grai_source_fivetran/fivetran_api/__init__.py
--rw-r--r--   0        0        0   436632 2023-02-14 16:39:18.545031 grai_source_fivetran-0.0.7/src/grai_source_fivetran/fivetran_api/api_models.py
--rw-r--r--   0        0        0    42232 2023-02-14 16:39:18.545359 grai_source_fivetran-0.0.7/src/grai_source_fivetran/fivetran_api/main.py
--rw-r--r--   0        0        0    13390 2023-05-26 18:52:58.771794 grai_source_fivetran-0.0.7/src/grai_source_fivetran/loader.py
--rw-r--r--   0        0        0     1668 2023-02-14 16:39:18.545711 grai_source_fivetran-0.0.7/src/grai_source_fivetran/mock_tools.py
--rw-r--r--   0        0        0     4751 2023-02-14 16:39:18.545877 grai_source_fivetran-0.0.7/src/grai_source_fivetran/models.py
--rw-r--r--   0        0        0      186 2023-02-14 16:39:18.546106 grai_source_fivetran-0.0.7/src/grai_source_fivetran/package_definitions.py
--rw-r--r--   0        0        0        0 2023-02-14 16:39:18.546143 grai_source_fivetran-0.0.7/src/grai_source_fivetran/py.typed
--rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      420 2023-05-25 16:20:32.597515 grai_source_fivetran-0.0.8/README.md
+-rw-r--r--   0        0        0     1020 2023-05-27 15:46:22.651284 grai_source_fivetran-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-02-14 16:39:18.542655 grai_source_fivetran-0.0.8/src/grai_source_fivetran/__init__.py
+-rw-r--r--   0        0        0     6644 2023-05-19 11:07:12.931545 grai_source_fivetran-0.0.8/src/grai_source_fivetran/adapters.py
+-rw-r--r--   0        0        0     2111 2023-05-26 22:51:50.125227 grai_source_fivetran-0.0.8/src/grai_source_fivetran/base.py
+-rw-r--r--   0        0        0        0 2023-02-14 16:39:18.543040 grai_source_fivetran-0.0.8/src/grai_source_fivetran/fivetran_api/__init__.py
+-rw-r--r--   0        0        0   436632 2023-02-14 16:39:18.545031 grai_source_fivetran-0.0.8/src/grai_source_fivetran/fivetran_api/api_models.py
+-rw-r--r--   0        0        0    42232 2023-02-14 16:39:18.545359 grai_source_fivetran-0.0.8/src/grai_source_fivetran/fivetran_api/main.py
+-rw-r--r--   0        0        0    13311 2023-05-27 15:45:55.987821 grai_source_fivetran-0.0.8/src/grai_source_fivetran/loader.py
+-rw-r--r--   0        0        0     1668 2023-02-14 16:39:18.545711 grai_source_fivetran-0.0.8/src/grai_source_fivetran/mock_tools.py
+-rw-r--r--   0        0        0     4751 2023-02-14 16:39:18.545877 grai_source_fivetran-0.0.8/src/grai_source_fivetran/models.py
+-rw-r--r--   0        0        0      186 2023-02-14 16:39:18.546106 grai_source_fivetran-0.0.8/src/grai_source_fivetran/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-02-14 16:39:18.546143 grai_source_fivetran-0.0.8/src/grai_source_fivetran/py.typed
+-rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.8/PKG-INFO
```

### Comparing `grai_source_fivetran-0.0.7/pyproject.toml` & `grai_source_fivetran-0.0.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_fivetran"
-version = "0.0.7"
+version = "0.0.8"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_fivetran", from = "src" },
 ]
 readme = "README.md"
```

### Comparing `grai_source_fivetran-0.0.7/src/grai_source_fivetran/adapters.py` & `grai_source_fivetran-0.0.8/src/grai_source_fivetran/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.7/src/grai_source_fivetran/base.py` & `grai_source_fivetran-0.0.8/src/grai_source_fivetran/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.7/src/grai_source_fivetran/fivetran_api/api_models.py` & `grai_source_fivetran-0.0.8/src/grai_source_fivetran/fivetran_api/api_models.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.7/src/grai_source_fivetran/fivetran_api/main.py` & `grai_source_fivetran-0.0.8/src/grai_source_fivetran/fivetran_api/main.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.7/src/grai_source_fivetran/loader.py` & `grai_source_fivetran-0.0.8/src/grai_source_fivetran/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,14 +212,53 @@
     source: str
     destination: str
 
 
 NamespaceTypes = Union[Dict[str, Union[str, SourceDestinationDict]], str]
 
 
+def build_namespace_map(
+    connectors: Dict, namespace_map: Union[str, Optional[NamespaceTypes]], default_namespace: Optional[str]
+) -> Dict[str, NamespaceIdentifier]:
+    if namespace_map is None and default_namespace is None:
+        message = (
+            f"The FivetranGraiMapper requires a not null value for `default_namespace` and/or `namespaces. "
+            f"These values are used to identify which Fivetran connection id's belong to which associated "
+            f"Grai namespace. `default_namespace` will map a single namespace to ALL connection id's."
+            "This behavior can be overridden by `namespaces` which maps {connection_id -> "
+            "namespace} or {connection_id -> {source: namespace, destination: namespace}}"
+        )
+        raise ValueError(message)
+    elif isinstance(namespace_map, str):
+        namespace_map = json.loads(namespace_map)
+
+    if namespace_map is None:
+        namespace_map = {}
+    else:
+        message = (
+            "The namespaces object should be a dictionary whose id's are Fivetran connector id's and whose values "
+            "identify the Grai namespace associated with either the source or destination of the connector. "
+            "The values can either be provided as a dictionary with the keys 'source' and 'destination' or ",
+            "as strings identifying the Grai namespace you'd like to associate with both the source "
+            "and destination.",
+        )
+        assert all(isinstance(v, (dict, str)) for v in namespace_map.values()), message
+        assert all("source" in v and "destination" in v for v in namespace_map.values() if isinstance(v, dict)), message
+
+    if default_namespace is not None:
+        namespace_map = namespace_map.copy()  # avoid modifying the users original argument
+        for k in connectors.keys():
+            namespace_map.setdefault(k, default_namespace)
+
+    return {
+        k: NamespaceIdentifier(source=v, destination=v) if isinstance(v, str) else NamespaceIdentifier(**v)
+        for k, v in namespace_map.items()
+    }
+
+
 class FivetranConnector(FivetranAPI):
     def __init__(
         self,
         namespaces: Optional[NamespaceTypes] = None,
         default_namespace: Optional[str] = None,
         parallelization: int = 10,
         *args,
@@ -228,15 +267,15 @@
         super().__init__(*args, **kwargs)
         self.parallelization = parallelization
         self.semaphore = asyncio.Semaphore(self.parallelization)
         self.http_runner = parallelize_http(self.semaphore)
         self.default_namespace = default_namespace
 
         self.connectors = {conn.id: conn for conn in self.get_connectors() if conn.id is not None}
-        self.namespace_map = self._build_namespace_map(namespaces)
+        self.namespace_map = build_namespace_map(self.connectors, namespaces, self.default_namespace)
         if self.default_namespace is None:
             self.connectors = {k: v for k, v in self.connectors.items() if k in self.namespace_map}
 
         self.table_to_conn_map: Dict[str, str] = {}
         self.column_to_conn_map: Dict[str, str] = {}
         self.schemas: Dict[str, SchemaMetadataResponse] = {}
         self.tables: Dict[str, TableMetadataResponse] = {}
@@ -254,52 +293,14 @@
             for column in c_res:
                 self.column_to_conn_map.setdefault(column.id, conn_id)
 
         self.schemas.update({item.id: item for seq in schemas for item in seq})
         self.tables.update({item.id: item for seq in tables for item in seq})
         self.columns.update({item.id: item for seq in columns for item in seq})
 
-    def _build_namespace_map(self, namespace_map: Optional[NamespaceTypes]) -> Dict[str, NamespaceIdentifier]:
-        if namespace_map is None and self.default_namespace is None:
-            message = (
-                f"The FivetranGraiMapper requires a not null value for `default_namespace` and/or `namespaces. "
-                f"These values are used to identify which Fivetran connection id's belong to which associated "
-                f"Grai namespace. `default_namespace` will map a single namespace to ALL connection id's."
-                "This behavior can be overridden by `namespaces` which maps {connection_id -> "
-                "namespace} or {connection_id -> {source: namespace, destination: namespace}}"
-            )
-            raise ValueError(message)
-        elif isinstance(namespace_map, str):
-            namespace_map = json.loads(namespace_map)
-
-        if namespace_map is None:
-            namespace_map = {}
-        else:
-            message = (
-                "The namespaces object should be a dictionary whose id's are Fivetran connector id's and whose values "
-                "identify the Grai namespace associated with either the source or destination of the connector. "
-                "The values can either be provided as a dictionary with the keys 'source' and 'destination' or ",
-                "as strings identifying the Grai namespace you'd like to associate with both the source "
-                "and destination.",
-            )
-            assert all(isinstance(v, (dict, str)) for v in namespace_map.values()), message
-            assert all(
-                isinstance(v, SourceDestinationDict) for v in namespace_map.values() if isinstance(v, dict)
-            ), message
-
-        if self.default_namespace is not None:
-            namespace_map = namespace_map.copy()  # avoid modifying the users original argument
-            for k in self.connectors.keys():
-                namespace_map.setdefault(k, self.default_namespace)
-
-        return {
-            k: NamespaceIdentifier(source=v, destination=v) if isinstance(v, str) else NamespaceIdentifier(**v)
-            for k, v in namespace_map.items()
-        }
-
     def get_nodes_and_edges(self) -> Tuple[List[NodeTypes], List[Edge]]:
         # table.parent_id -> schema.id
         # column.parent_id -> table.id
         self.build_lineage()
         tables = {
             table.id: Table.from_fivetran_models(
                 self.schemas[table.parent_id],
```

### Comparing `grai_source_fivetran-0.0.7/src/grai_source_fivetran/mock_tools.py` & `grai_source_fivetran-0.0.8/src/grai_source_fivetran/mock_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.7/src/grai_source_fivetran/models.py` & `grai_source_fivetran-0.0.8/src/grai_source_fivetran/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.7/PKG-INFO` & `grai_source_fivetran-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-fivetran
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.9.13,<4.0.0
 Classifier: License :: Other/Proprietary License
```

