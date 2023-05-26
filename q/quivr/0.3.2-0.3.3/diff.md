# Comparing `tmp/quivr-0.3.2.tar.gz` & `tmp/quivr-0.3.3.tar.gz`

## Comparing `quivr-0.3.2.tar` & `quivr-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 quivr-0.3.2/quivr/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.3.2/quivr/__version__.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 quivr-0.3.2/quivr/concat.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 quivr-0.3.2/quivr/defragment.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 quivr-0.3.2/quivr/errors.py
--rw-r--r--   0        0        0    25638 2020-02-02 00:00:00.000000 quivr-0.3.2/quivr/fields.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.3.2/quivr/indexing.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.3.2/quivr/matrix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.3.2/quivr/py.typed
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 quivr-0.3.2/quivr/schemagraph.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 quivr-0.3.2/quivr/streaming.py
--rw-r--r--   0        0        0    21677 2020-02-02 00:00:00.000000 quivr-0.3.2/quivr/tables.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 quivr-0.3.2/quivr/validators.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.3.2/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.3.2/LICENSE
--rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 quivr-0.3.2/README.md
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 quivr-0.3.2/pyproject.toml
--rw-r--r--   0        0        0    11097 2020-02-02 00:00:00.000000 quivr-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/__version__.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/attributes.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/concat.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/defragment.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/errors.py
+-rw-r--r--   0        0        0    25837 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/fields.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/indexing.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/py.typed
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/schemagraph.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/streaming.py
+-rw-r--r--   0        0        0    27450 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/tables.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 quivr-0.3.3/quivr/validators.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.3.3/LICENSE
+-rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 quivr-0.3.3/README.md
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 quivr-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0    11097 2020-02-02 00:00:00.000000 quivr-0.3.3/PKG-INFO
```

### Comparing `quivr-0.3.2/quivr/__init__.py` & `quivr-0.3.3/quivr/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from .__version__ import __version__
-
+from .attributes import FloatAttribute, IntAttribute, StringAttribute
 from .concat import concatenate
 from .errors import InvariantViolatedError, TableFragmentedError, ValidationError
 from .fields import (
     BinaryField,
     Date32Field,
     Date64Field,
     Decimal128Field,
     Decimal256Field,
     DictionaryField,
     DurationField,
     Field,
     Float16Field,
     Float32Field,
     Float64Field,
+    Int8Field,
     Int16Field,
     Int32Field,
     Int64Field,
     LargeBinaryField,
     LargeListField,
     LargeStringField,
     ListField,
     MapField,
     MonthDayNanoIntervalField,
     NullField,
     RunEndEncodedField,
     StringField,
     StructField,
+    SubTableField,
     Time32Field,
     Time64Field,
     TimestampField,
     UInt8Field,
     UInt16Field,
     UInt32Field,
     UInt64Field,
@@ -44,15 +46,16 @@
     "__version__",
     "Table",
     "MatrixArray",
     "MatrixExtensionType",
     "concatenate",
     "StringIndex",
     "Field",
-    "SubTableField" "Int8Field",
+    "SubTableField",
+    "Int8Field",
     "Int16Field",
     "Int32Field",
     "Int64Field",
     "UInt8Field",
     "UInt16Field",
     "UInt32Field",
     "UInt64Field",
@@ -85,8 +88,11 @@
     "lt",
     "le",
     "gt",
     "ge",
     "eq",
     "and_",
     "is_in",
+    "StringAttribute",
+    "IntAttribute",
+    "FloatAttribute",
 ]
```

### Comparing `quivr-0.3.2/quivr/concat.py` & `quivr-0.3.3/quivr/concat.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.2/quivr/fields.py` & `quivr-0.3.3/quivr/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,23 @@
         self.table_type = table_type
         self.schema = table_type.schema
         dtype = pa.struct(table_type.schema)
         super().__init__(dtype, nullable=nullable, metadata=metadata)
 
     def __get__(self, obj: "Table", objtype: type) -> T:
         array = obj.table.column(self.name)
-        subtable = pa.Table.from_arrays(array.flatten(), schema=self.schema)
+
+        metadata = self.metadata
+        if metadata is None:
+            metadata = {}
+        metadata.update(obj._metadata_for_field(self.name))
+
+        schema = self.schema.with_metadata(metadata)
+
+        subtable = pa.Table.from_arrays(array.flatten(), schema=schema)
         return self.table_type(subtable)
 
 
 class Int8Field(Field):
     """
     A field for storing 8-bit integers.
     """
```

### Comparing `quivr-0.3.2/quivr/indexing.py` & `quivr-0.3.3/quivr/indexing.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.2/quivr/matrix.py` & `quivr-0.3.3/quivr/matrix.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.2/quivr/schemagraph.py` & `quivr-0.3.3/quivr/schemagraph.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.2/quivr/tables.py` & `quivr-0.3.3/quivr/tables.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,75 @@
 import os
+import warnings
 from io import IOBase
 from typing import Any, ClassVar, Optional, Self, Union
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.csv
 import pyarrow.feather
 import pyarrow.parquet
 
+from .attributes import Attribute
 from .errors import TableFragmentedError, ValidationError
 from .fields import Field, MetadataDict, SubTableField
 from .schemagraph import _walk_schema
 
 
 class Table:
     schema: ClassVar[pa.Schema]
     table: pa.Table
 
     def __init_subclass__(cls, **kwargs):
         fields = []
         field_validators = {}
+        subtables = {}
+        attributes = {}
         for name, field in cls.__dict__.items():
             if isinstance(field, Field):
                 fields.append(field.pyarrow_field())
                 if field.validator is not None:
                     field_validators[name] = field.validator
+                if isinstance(field, SubTableField):
+                    subtables[name] = field
+            elif isinstance(field, Attribute):
+                attributes[name] = field
 
         # Generate a pyarrow schema
         schema = pa.schema(fields)
         cls.schema = schema
 
+        # Keep track of subtables
+        cls._quivr_subtables = subtables
+
+        # Add attributes
+        cls._quivr_attributes = attributes
+
         # Add validators
         cls._field_validators = field_validators
 
         # If the subclass has an __init__ override, it must have a
         # with_table override as well.
         if "__init__" in cls.__dict__ and "with_table" not in cls.__dict__:
             raise TypeError(
                 f"{cls.__name__} has an __init__ override, but does not have a with_table "
                 + "override. You must implement both or neither."
             )
 
         super().__init_subclass__(**kwargs)
 
-    def __init__(self, table: pa.Table):
+    def __init__(self, table: pa.Table, **kwargs):
         self.table = table
+        for name, value in kwargs.items():
+            if name in self._quivr_attributes:
+                setattr(self, name, value)
+            else:
+                raise AttributeError(f"{self.__class__.__name__} has no attribute {name}")
 
     @classmethod
     def from_data(cls, data: Optional[Any] = None, validate: bool = True, **kwargs) -> Self:
         """
         Create an instance of the Table and populate it with data.
 
         This is a convenience method which tries to infer the right
@@ -129,14 +148,15 @@
         # We don't know the size of the table until we've found a
         # field in the schema which corresponds to a kwarg with data.
         # Therefore, we need to keep track of which columns are empty
         # *before* we've discovered the size of the table so we can
         # populate them with nulls later.
         empty_columns = []
 
+        metadata = {}
         for i, field in enumerate(cls.schema):
             column_name = field.name
             value = kwargs.pop(column_name, None)
 
             if value is None:
                 if not field.nullable:
                     raise ValueError(f"Missing non-nullable column {column_name}")
@@ -153,14 +173,19 @@
                 size = len(value)
             elif len(value) != size:
                 raise ValueError(
                     f"Column {column_name} has wrong length {len(value)} (first column has length {size})"
                 )
 
             if isinstance(value, Table):
+                field_meta = value.table.schema.metadata
+                if field_meta is not None:
+                    for key, val in field_meta.items():
+                        key = (field.name + "." + key.decode("utf-8")).encode("utf-8")
+                        metadata[key] = val
                 arrays.append(value.to_structarray())
             elif isinstance(value, pa.Array):
                 arrays.append(value)
             elif isinstance(value, np.ndarray):
                 arrays.append(pa.array(value, type=field.type))
             elif isinstance(value, list):
                 arrays.append(pa.array(value, type=field.type))
@@ -168,29 +193,35 @@
                 raise TypeError(f"Unsupported type for {column_name}: {type(value)}")
 
         if size is None:
             raise ValueError("No data provided")
 
         for idx in empty_columns:
             arrays[idx] = pa.nulls(size, type=cls.schema[idx].type)
-        return cls.from_arrays(arrays, **kwargs)
+        return cls.from_arrays(arrays, metadata=metadata, **kwargs)
 
     @classmethod
-    def from_arrays(cls, arrays: list[pa.array], **kwargs) -> Self:
+    def from_arrays(
+        cls, arrays: list[pa.array], metadata: Optional[dict[bytes, bytes]] = None, **kwargs
+    ) -> Self:
         """Create a Table object from a list of arrays.
 
         Args:
             arrays: A list of pyarrow.Array objects.
+            metadata: An optional dictionary of metadata to attach to the Table.
             **kwargs: Additional keyword arguments to pass to the Table's __init__ method.
 
         Returns:
             A Table object.
 
         """
-        table = pa.Table.from_arrays(arrays, schema=cls.schema)
+        if metadata is None:
+            metadata = {}
+        schema = cls.schema.with_metadata(metadata)
+        table = pa.Table.from_arrays(arrays, schema=schema)
         return cls(table=table, **kwargs)
 
     @classmethod
     def from_pydict(cls, d: dict[str, Union[pa.array, list, np.ndarray]], **kwargs) -> Self:
         table = pa.Table.from_pydict(d, schema=cls.schema)
         return cls(table=table, **kwargs)
 
@@ -546,29 +577,134 @@
         pyarrow.feather.write_feather(self.table, path, **kwargs)
 
     @classmethod
     def from_feather(cls, path: str, **kwargs):
         """Read a table from a Feather file."""
         return cls(table=pyarrow.feather.read_table(path), **kwargs)
 
-    def to_csv(self, path: str):
-        """Write the table to a CSV file. Any nested structure is flattened."""
-        pyarrow.csv.write_csv(self.flattened_table(), path)
+    def to_csv(self, path: str, attribute_columns: bool = True):
+        """Write the table to a CSV file. Any nested structure is flattened.
+
+        if attribute_columns is True (the default), then any Attributes defined
+        for the table (or its subtable fields) are stored in the CSV as columns;
+        they will have the same value repeated for every row. If it is False,
+        then Attribute data will  not be stored in the CSV, so it cannot be read back out.
+        """
+        table = self.flattened_table()
+        if attribute_columns:
+            for name, val in self._string_attributes().items():
+                table = table.append_column(
+                    name,
+                    pa.repeat(val, len(table)),
+                )
+        pyarrow.csv.write_csv(table, path)
 
     @classmethod
     def from_csv(cls, input_file: Union[str, os.PathLike, IOBase], **kwargs):
         """Read a table from a CSV file."""
         flat_table = pyarrow.csv.read_csv(input_file)
-        return cls(table=cls._unflatten_table(flat_table), **kwargs)
+
+        # Gather any attributes from the CSV. We do this by looking for specially named
+        # columns, and grabbing the value from their first row.
+        attributes = {}
+        attr_names = cls._attribute_metadata_keys()
+        if len(flat_table) > 0:
+            to_be_removed = []
+            for name in flat_table.column_names:
+                if name in attr_names:
+                    attributes[name] = str(flat_table.column(name)[0].as_py())
+                    to_be_removed.append(name)
+
+            if len(to_be_removed) > 0:
+                flat_table = flat_table.drop_columns(to_be_removed)
+
+        attribute_meta = cls._unpack_string_metadata(attributes)
+
+        table = cls._unflatten_table(flat_table)
+        metadata = table.schema.metadata or {}
+        metadata.update(attribute_meta)
+        table = table.replace_schema_metadata(metadata)
+        return cls(table, **kwargs)
 
     def is_valid(self) -> bool:
         """Validate the table against the schema."""
         for name, validator in self._field_validators.items():
             validator.valid(self.table.column(name))
 
     def validate(self):
         """Validate the table against the schema, raising an exception if invalid."""
         for name, validator in self._field_validators.items():
             try:
                 validator.validate(self.table.column(name))
             except ValidationError as e:
                 raise ValidationError(f"Column {name} failed validation: {str(e)}", e.failures) from e
+
+    @classmethod
+    def empty(cls, **kwargs) -> Self:
+        """Create an empty instance of the table."""
+        data = [[] for _ in range(len(cls.schema))]
+        empty_table = pa.table(data, schema=cls.schema)
+        return cls(table=empty_table, **kwargs)
+
+    def attributes(self) -> dict[str, Any]:
+        """Return a dictionary of the table's attributes."""
+        return {name: getattr(self, name) for name in self._quivr_attributes}
+
+    def _string_attributes(self) -> dict[str, str]:
+        """Return a dictionary of the table's attributes.
+
+        Attributes are presented in their string form.
+        """
+        d = {}
+        for name, descriptor in self._quivr_attributes.items():
+            value = getattr(self, name)
+            d[name] = descriptor.to_string(value)
+        for name in self._quivr_subtables.keys():
+            subattribs = getattr(self, name)._string_attributes()
+            for subname, subval in subattribs.items():
+                d[f"{name}.{subname}"] = subval
+        return d
+
+    @classmethod
+    def _unpack_string_metadata(cls, metadata: dict[str, str]) -> dict[bytes, bytes]:
+        result = {}
+
+        for k, v in metadata.items():
+            if "." in k:
+                # This is metadata for a subtable; we need to dig into it to find the
+                # descriptor for the attribute.
+                subtable_name, subtable_key = k.split(".", 1)
+                subtable_item = cls._quivr_subtables[subtable_name].table_type._unpack_string_metadata(
+                    {subtable_key: v}
+                )
+                result[k.encode("utf8")] = next(iter(subtable_item.values()))
+            else:
+                descriptor = cls._quivr_attributes.get(k)
+                if descriptor is None:
+                    warnings.warn(f"unexpected missing descriptor with name={k}")
+                result[k.encode("utf8")] = descriptor.to_bytes(descriptor.from_string(v))
+        return result
+
+    def _metadata_for_field(self, field_name: str) -> dict[bytes, bytes]:
+        """Return a dictionary of metadata associated with a subtable field."""
+        result = {}
+        if self.table.schema.metadata is None:
+            return result
+        field_name_bytes = (field_name + ".").encode("utf8")
+        for key, value in self.table.schema.metadata.items():
+            if key.startswith(field_name_bytes):
+                result[key[len(field_name_bytes) :]] = value
+        return result
+
+    @classmethod
+    def _attribute_metadata_keys(cls) -> set[str]:
+        """Return a set of all subtable attribute names."""
+        result = {attr.name for attr in cls._quivr_attributes.values()}
+        for field in cls._quivr_subtables.values():
+            attr_fields = field.table_type._quivr_attributes
+            for attr in attr_fields.values():
+                result.add(f"{field.name}.{attr.name}")
+
+            children = field.table_type._attribute_metadata_keys()
+            for key in children:
+                result.add(f"{field.name}.{key}")
+        return result
```

### Comparing `quivr-0.3.2/quivr/validators.py` & `quivr-0.3.3/quivr/validators.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.2/LICENSE` & `quivr-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.3.2/README.md` & `quivr-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `quivr-0.3.2/pyproject.toml` & `quivr-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quivr-0.3.2/PKG-INFO` & `quivr-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quivr
-Version: 0.3.2
+Version: 0.3.3
 Summary: Container library for working with tabular Arrow data
 Project-URL: Source, https://github.com/spenczar/quivr
 Author-email: Spencer Nelson <spencer@spencerwnelson.com>
 License-File: LICENSE
 Requires-Python: >=3.11
 Requires-Dist: mmh3
 Requires-Dist: numpy
```

