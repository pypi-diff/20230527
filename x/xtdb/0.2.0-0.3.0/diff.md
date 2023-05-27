# Comparing `tmp/xtdb-0.2.0.tar.gz` & `tmp/xtdb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtdb-0.2.0.tar", max compression
+gzip compressed data, was "xtdb-0.3.0.tar", max compression
```

## Comparing `xtdb-0.2.0.tar` & `xtdb-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    13827 2023-05-22 07:17:23.468748 xtdb-0.2.0/LICENSE
--rw-r--r--   0        0        0     2749 2023-05-22 07:17:23.468748 xtdb-0.2.0/README.md
--rw-r--r--   0        0        0     1581 2023-05-22 07:17:23.468748 xtdb-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-22 07:17:23.468748 xtdb-0.2.0/xtdb/__init__.py
--rw-r--r--   0        0        0      232 2023-05-22 07:17:23.468748 xtdb-0.2.0/xtdb/__main__.py
--rw-r--r--   0        0        0      165 2023-05-22 07:17:23.468748 xtdb-0.2.0/xtdb/exceptions.py
--rw-r--r--   0        0        0     1857 2023-05-22 07:17:23.468748 xtdb-0.2.0/xtdb/orm.py
--rw-r--r--   0        0        0     8079 2023-05-22 07:17:23.472748 xtdb-0.2.0/xtdb/query.py
--rw-r--r--   0        0        0    11754 2023-05-22 07:17:23.472748 xtdb-0.2.0/xtdb/session.py
--rw-r--r--   0        0        0     3443 1970-01-01 00:00:00.000000 xtdb-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    13827 2023-05-27 08:43:25.416783 xtdb-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3565 2023-05-27 08:43:25.416783 xtdb-0.3.0/README.md
+-rw-r--r--   0        0        0     1567 2023-05-27 08:43:25.416783 xtdb-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-27 08:43:25.416783 xtdb-0.3.0/xtdb/__init__.py
+-rw-r--r--   0        0        0      211 2023-05-27 08:43:25.416783 xtdb-0.3.0/xtdb/__main__.py
+-rw-r--r--   0        0        0    10485 2023-05-27 08:43:25.416783 xtdb-0.3.0/xtdb/datalog.py
+-rw-r--r--   0        0        0      120 2023-05-27 08:43:25.416783 xtdb-0.3.0/xtdb/exceptions.py
+-rw-r--r--   0        0        0     1769 2023-05-27 08:43:25.416783 xtdb-0.3.0/xtdb/orm.py
+-rw-r--r--   0        0        0     6303 2023-05-27 08:43:25.416783 xtdb-0.3.0/xtdb/query.py
+-rw-r--r--   0        0        0    11713 2023-05-27 08:43:25.420783 xtdb-0.3.0/xtdb/session.py
+-rw-r--r--   0        0        0     4245 1970-01-01 00:00:00.000000 xtdb-0.3.0/PKG-INFO
```

### Comparing `xtdb-0.2.0/LICENSE` & `xtdb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xtdb-0.2.0/README.md` & `xtdb-0.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,55 @@
-# XTDB Python
+![Logo](docs/logo.png)
 
-A Python connector and ORM for XTDB.
+# XTDB Python: A Python ORM for XTDB
 
 
-[![Code Integration](https://github.com/Donnype/xtdb-py/actions/workflows/tests.yml/badge.svg)](https://github.com/Donnype/xtdb-py/actions/workflows/tests.yml)
+[![Tests](https://github.com/Donnype/xtdb-py/actions/workflows/tests.yml/badge.svg)](https://github.com/Donnype/xtdb-py/actions/workflows/tests.yml)
 [![Stable Version](https://img.shields.io/pypi/v/xtdb?label=stable)](https://pypi.org/project/xtdb/#history)
 [![Python Versions](https://img.shields.io/pypi/pyversions/xtdb)](https://pypi.org/project/xtdb/)
 
 
 ## Installation
 
+You can install this project using pip:
+
 ```bash
 pip install xtdb
 ```
 
 ## Usage
 
 The following examples assume you have set the `XTDB_URI` variable in your environment.
 To start experimenting, you could use the following setup using Docker:
 ```bash
 $ docker run -p 3000:3000 -d juxt/xtdb-standalone-rocksdb:1.21.0
 $ export XTDB_URI=http://localhost:3000/_xtdb
 ```
 
+### Using the client
+
+The `XTDBClient` supports the full HTTP API spec.
+
+```python3
+import os
+
+from xtdb.session import XTDBClient, Operation
+
+client = XTDBClient(os.environ["XTDB_URI"])
+client.submit_transaction([Operation.put({"xt/id": "123", "name": "fred"})])
+
+client.query('{:query {:find [(pull ?e [*])] :where [[ ?e :name "fred" ]]}}')
+client.get_entity("123")
+```
+
+
 ### Using the ORM
 
+Below is an example of how to use the ORM functionality.
+
 ```python3
 import os
 from dataclasses import dataclass
 
 from xtdb.orm import Base
 from xtdb.query import Query
 from xtdb.session import XTDBSession
@@ -53,85 +74,87 @@
 
 query = Query(TestEntity).where(TestEntity, name="test")
 result = session.query(query)
 
 assert result[0].dict() == {"TestEntity/name": "test", "type": "TestEntity", "xt/id": entity.id}
 ```
 
-### Using only the client
-
-```python3
-import os
+To see more examples, check out the [examples directory](examples).
+Don't hesitate to add your own examples!
 
-from xtdb.session import XTDBClient, Operation
+### Using the CLI for querying
 
-client = XTDBClient(os.environ["XTDB_URI"])
-client.submit_transaction([Operation.put({"xt/id": "123", "name": "fred"})])
+This package also comes with an easy CLI tool to query XTDB.
+To query XTDB using a plain query you can run
 
-client.query('{:query {:find [(pull ?e [*])] :where [[ ?e :name "fred" ]]}}')
-client.get_entity("123")
-```
-
-### Using the CLI tool for querying
-
-Using a query string
 ```bash
 $ echo '{:query {:find [(pull ?e [*])] :where [[ ?e :name "fred" ]]}}' | python -m xtdb | jq
 [
   [
     {
-      "somenil": null,
+      "xt/id": "123"
       "name": "fred",
+      "somenil": null,
       "somedict": {
         "c": 3,
         "a": "b"
       },
-      "somelist": [
-        "jeez",
-        123
-      ],
-      "xt/id": "123"
     }
   ]
 ]
 ```
 
-or a query in a file:
+To use a query file the command can be modified to the following:
 
 ```bash
 $ cat query.txt
 {:query {:find [(pull ?e [*])] :where [[ ?e :name "fred" ]]}}
 $ python -m xtdb < query.txt | jq
 [
   [
     {
-      "somenil": null,
+      "xt/id": "123"
       "name": "fred",
+      "somenil": null,
       "somedict": {
         "c": 3,
         "a": "b"
       },
-      "somelist": [
-        "jeez",
-        123
-      ],
-      "xt/id": "123"
     }
   ]
 ]
 ```
 
-## Development
+## Contributing
 
-Using Poetry, simply run
 
+### Installation
+
+To get started, clone the repo and create an environment using Poetry
+```bash
+$ git clone https://github.com/Donnype/xtdb-py.git
+$ cd xtdb-py
+$ poetry install
+```
+
+Now set up XTDB, for instance using Docker
 ```bash
-poetry install
+$ docker run -p 3000:3000 -d juxt/xtdb-standalone-rocksdb:1.21.0
 ```
 
-to create your environment. The `Makefile` has several targets that should make development easier:
+Export the XTDB_URI environment variable to be able to use `os.environ["XTDB_URI"]` to fetch the endpoint
+```bash
+$ export XTDB_URI=http://localhost:3000/_xtdb
+```
+
+### Development
+
+The `Makefile` has several targets that should make development easier:
 ```bash
 $ make utest  # Run unit tests
 $ make itest  # Run integration tests
 $ make check  # Run all linters
 $ make done   # Run all of the above
 ```
+
+The CI runs these checks as well.
+Check out the [project page](https://github.com/users/Donnype/projects/1) for issues and features to work on.
```

### Comparing `xtdb-0.2.0/pyproject.toml` & `xtdb-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xtdb"
-version = "0.2.0"
+version = "0.3.0"
 packages = [{ include = "xtdb" }]
 include  = ["xtdb/**"]
 exclude = [
     "**/.idea",
     "**/.git*",
     "**/.*ignore",
     "**/.flake8",
@@ -13,15 +13,15 @@
     "**/Dockerfile*",
     "**/Makefile",
     "**/__pycache__",
 ]
 
 authors = ["Donny Peeters <donny.peeters@hotmail.com>"]
 maintainers = ["Donny Peeters <donny.peeters@hotmail.com>"]
-description = "A Python connector and ORM for XTDB."
+description = "A Python ORM for XTDB."
 readme = "README.md"
 homepage = "https://github.com/Donnype/xtdb-py"
 repository = "https://github.com/Donnype/xtdb-py"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.26.0"
```

### Comparing `xtdb-0.2.0/xtdb/orm.py` & `xtdb-0.3.0/xtdb/orm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import logging
 import uuid
 from dataclasses import asdict, dataclass
 from typing import Dict, List, Type
 
-logger = logging.getLogger(__name__)
-
 TYPE_FIELD = "type"
 
 
 @dataclass
 class Base:
     @property
     def id(self):
@@ -70,11 +67,8 @@
     identifier: str
 
     @property
     def id(self):
         return self.identifier
 
     def dict(self) -> Dict:
-        return {
-            "xt/id": self.identifier,
-            "xt/fn": self.function,
-        }
+        return {"xt/id": self.identifier, "xt/fn": self.function}
```

### Comparing `xtdb-0.2.0/xtdb/query.py` & `xtdb-0.3.0/xtdb/query.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,42 @@
-from dataclasses import dataclass, field
-from typing import List, Optional, Type, Union
+from dataclasses import dataclass
+from typing import Optional, Type, Union
 
+from xtdb.datalog import (
+    Avg,
+    Clause,
+    Count,
+    CountDistinct,
+    Distinct,
+    Find,
+    Limit,
+    Max,
+    Median,
+    Min,
+    Offset,
+    Or,
+    Rand,
+    Sample,
+    Stddev,
+    Sum,
+    Timeout,
+    Variance,
+    Where,
+)
 from xtdb.exceptions import InvalidField
-from xtdb.orm import TYPE_FIELD, Base
+from xtdb.orm import Base
 
 
 @dataclass
 class Var:
     val: str
 
+    def __str__(self):
+        return f"?{self.val}"
+
 
 @dataclass
 class Query:
     """Object representing an XTDB query.
 
         result_type: Object being queried: executing the query should yield only this Object.
 
@@ -27,18 +51,21 @@
         [ Object2 :Object2/object_one_reference Object1 ]
     ]}}
     '
     """
 
     result_type: Type[Base]
 
-    _where_clauses: List[str] = field(default_factory=list)
-    _find_clauses: List[str] = field(default_factory=list)
-    _limit: Optional[int] = None
-    _offset: Optional[int] = None
+    _find: Optional[Clause] = None
+    _where: Optional[Clause] = None
+
+    _limit: Optional[Limit] = None
+    _offset: Optional[Offset] = None
+    _timeout: Optional[Timeout] = None
+
     _preserved_return_type: bool = True
 
     def where(self, object_type: Type[Base], **kwargs) -> "Query":
         for field_name, value in kwargs.items():
             self._where_field_is(object_type, field_name, value)
 
         return self
@@ -46,127 +73,121 @@
     def format(self) -> str:
         return self._compile(separator="\n    ")
 
     def count(self, var: Union[Type[Base], Var]) -> "Query":
         self._preserved_return_type = False
 
         if isinstance(var, Var):
-            self._find_clauses.append(f"(count ?{var.val})")
+            self._find = self._find & Count(str(var))
             return self
 
-        self._find_clauses.append(f"(count {var.alias()})")
+        self._find = self._find & Count(var.alias())
         return self
 
     def avg(self, var: Var) -> "Query":
         self._preserved_return_type = False
-        self._find_clauses.append(f"(avg ?{var.val})")
+        self._find = self._find & Avg(str(var))
 
         return self
 
     def max(self, var: Var) -> "Query":
         self._preserved_return_type = False
-        self._find_clauses.append(f"(max ?{var.val})")
+        self._find = self._find & Max(str(var))
 
         return self
 
     def min(self, var: Var) -> "Query":
         self._preserved_return_type = False
-        self._find_clauses.append(f"(min ?{var.val})")
+        self._find = self._find & Min(str(var))
 
         return self
 
     def count_distinct(self, var: Var) -> "Query":
         self._preserved_return_type = False
-        self._find_clauses.append(f"(count-distinct ?{var.val})")
+        self._find = self._find & CountDistinct(str(var))
 
         return self
 
     def sum(self, var: Var) -> "Query":
         self._preserved_return_type = False
-        self._find_clauses.append(f"(sum ?{var.val})")
+        self._find = self._find & Sum(str(var))
 
         return self
 
     def median(self, var: Var) -> "Query":
         self._preserved_return_type = False
-        self._find_clauses.append(f"(median ?{var.val})")
+        self._find = self._find & Median(str(var))
 
         return self
 
     def variance(self, var: Var) -> "Query":
         self._preserved_return_type = False
-        self._find_clauses.append(f"(variance ?{var.val})")
+        self._find = self._find & Variance(str(var))
 
         return self
 
     def stddev(self, var: Var) -> "Query":
         self._preserved_return_type = False
-        self._find_clauses.append(f"(stddev ?{var.val})")
+        self._find = self._find & Stddev(str(var))
 
         return self
 
     def distinct(self, var: Var) -> "Query":
         self._preserved_return_type = False
-        self._find_clauses.append(f"(distinct ?{var.val})")
+        self._find = self._find & Distinct(str(var))
 
         return self
 
     def rand(self, var: Var, N: int) -> "Query":
         self._preserved_return_type = False
-        self._find_clauses.append(f"(rand {N} ?{var.val})")
+        self._find = self._find & Rand(str(var), N)
 
         return self
 
     def sample(self, var: Var, N: int) -> "Query":
         self._preserved_return_type = False
-        self._find_clauses.append(f"(sample {N} ?{var.val})")
+        self._find = self._find & Sample(str(var), N)
 
         return self
 
-    def group_by(self, object_type: Type[Base]) -> "Query":
-        self._preserved_return_type = False
-        self._find_clauses.append(f"{object_type.alias()}")
+    def limit(self, limit: int) -> "Query":
+        self._limit = Limit(limit)
 
         return self
 
-    def limit(self, limit: int) -> "Query":
-        self._limit = limit
+    def offset(self, offset: int) -> "Query":
+        self._offset = Offset(offset)
 
         return self
 
-    def offset(self, offset: int) -> "Query":
-        self._offset = offset
+    def timeout(self, timeout: int) -> "Query":
+        self._timeout = Timeout(timeout)
 
         return self
 
     def _where_field_is(
         self, object_type: Type[Base], field_name: str, value: Union[Type[Base], Var, str, None]
     ) -> None:
         if field_name not in object_type.fields():
             raise InvalidField(f'"{field_name}" is not a field of {object_type.alias()}')
 
-        if isinstance(value, Var):
-            self._add_where_statement(object_type, field_name, f"?{value.val}")
-            return
-
         if isinstance(value, str):
             value = value.replace('"', r"\"")
             self._add_where_statement(object_type, field_name, f'"{value}"')
             return
 
-        if type(value) in [int, float, bool]:
+        if type(value) in [int, float, bool, Var]:
             self._add_where_statement(object_type, field_name, f"{value}")
             return
 
         if value is None:
             self._add_where_statement(object_type, field_name, "nil")
             return
 
         # TODO: support for list and dict?
-
         if not isinstance(value, type):
             raise InvalidField(f"value '{value}' should be a string or a Base Type")
 
         if not issubclass(value, Base):
             raise InvalidField(f"{value} is not an Base Type")
 
         if field_name not in object_type._relations():
@@ -175,72 +196,28 @@
         if object_type._subclasses():
             self._add_or_statement(object_type, field_name, value.alias())
             return
 
         self._add_where_statement(object_type, field_name, value.alias())
 
     def _add_where_statement(self, object_type: Type[Base], field_name: str, to_alias: str) -> None:
-        self._where_clauses.append(self._relationship(object_type.alias(), object_type.alias(), field_name, to_alias))
+        self._where = self._where & Where(object_type.alias(), f"{object_type.alias()}/{field_name}", to_alias)
 
     def _add_or_statement(self, object_type: Type[Base], field_name: str, to_alias: str) -> None:
-        self._where_clauses.append(
-            self._or_statement(
-                object_type.alias(),
-                object_type.__subclasses__(),
-                field_name,
-                to_alias,
-            )
-        )
-
-    def _or_statement(self, from_alias: str, concrete_types: List[Type[Base]], field_name: str, to_alias: str) -> str:
-        relationships = [
-            self._relationship(from_alias, concrete_type.alias(), field_name, to_alias)
-            for concrete_type in concrete_types
+        clauses = [
+            Where(object_type.alias(), f"{sc.alias()}/{field_name}", to_alias) for sc in object_type._subclasses()
         ]
-
-        return f"(or {' '.join(relationships)} )"
-
-    def _relationship(self, from_alias: str, field_type: str, field_name: str, to_alias: str) -> str:
-        return f"[ {from_alias} :{field_type}/{field_name} {to_alias} ]"
-
-    def _assert_type(self, object_type: Type[Base]) -> str:
-        if not object_type._subclasses():
-            return self._to_type_statement(object_type, object_type)
-
-        return f"(or {' '.join([self._to_type_statement(object_type, x) for x in object_type.__subclasses__()])} )"
-
-    def _to_type_statement(self, object_type: Type[Base], other_type: Type[Base]) -> str:
-        return f'[ {object_type.alias()} :{TYPE_FIELD} "{other_type.alias()}" ]'
-
-    def _compile_where_clauses(self, where_clauses: List[str], *, separator=" ") -> str:
-        """Sorted and deduplicated where clauses, since they are both idempotent and commutative"""
-
-        return separator + separator.join(sorted(set(where_clauses)))
-
-    def _compile_find_clauses(self, find_clauses: List[str]) -> str:
-        return " ".join(find_clauses)
+        self._where = self._where & Or(clauses)  # type: ignore
 
     def _compile(self, *, separator=" ") -> str:
-        where_clauses = self._where_clauses
-        where_clauses.append(self._assert_type(self.result_type))
-
-        if not self._find_clauses:
-            find_clauses = self._compile_find_clauses([f"(pull {self.result_type.alias()} [*])"])
-        else:
-            find_clauses = self._compile_find_clauses(self._find_clauses)
-
-        compiled_where_clauses = self._compile_where_clauses(where_clauses, separator=separator)
-        compiled = f"{{:query {{:find [{find_clauses}] :where [{compiled_where_clauses}]"
-
-        if self._limit is not None:
-            compiled += f" :limit {self._limit}"
+        where = self._where & Where(self.result_type.alias(), "type", f'"{self.result_type.alias()}"')
+        find = Find(f"(pull {self.result_type.alias()} [*])") if self._find is None else self._find
 
-        if self._offset is not None:
-            compiled += f" :offset {self._offset}"
+        find_where = find & where & self._limit & self._offset & self._timeout
 
-        return compiled + "}}"
+        return find_where.compile(separator=separator)
 
     def __str__(self) -> str:
         return self._compile()
 
     def __eq__(self, other):
         return str(self) == str(other)
```

### Comparing `xtdb-0.2.0/xtdb/session.py` & `xtdb-0.3.0/xtdb/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,18 +205,15 @@
     def get_attribute_stats(self):
         res = self._session.get(f"{self.base_url}/attribute-stats")
         self._verify_response(res)
 
         return res.json()
 
     def sync(self, timeout: Optional[int] = None):
-        params = {}
-
-        if timeout is not None:
-            params["timeout"] = timeout
+        params = {} if timeout is None else {"timeout": timeout}
 
         res = self._session.get(f"{self.base_url}/sync", params=params)
         self._verify_response(res)
 
         return res.json()
 
     def query(
@@ -244,18 +241,15 @@
             data=str(query),
             headers={"Content-Type": "application/edn"},
         )
         self._verify_response(res)
         return res.json()
 
     def await_transaction(self, tx_id: int, timeout: Optional[int] = None) -> None:
-        params = {"txId": tx_id}
-
-        if timeout is not None:
-            params["timeout"] = timeout
+        params = {"txId": tx_id} if timeout is None else {"txId": tx_id, "timeout": timeout}
 
         self._session.get(f"{self.base_url}/await-tx", params=params)
 
     def await_transaction_time(self, tx_time: datetime, timeout: Optional[int] = None) -> None:
         params = {"tx-time": tx_time.isoformat()}
 
         if timeout is not None:
```

