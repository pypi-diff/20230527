# Comparing `tmp/redcat-0.0.3.tar.gz` & `tmp/redcat-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redcat-0.0.3.tar", max compression
+gzip compressed data, was "redcat-0.0.4.tar", max compression
```

## Comparing `redcat-0.0.3.tar` & `redcat-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1501 2023-05-21 04:17:02.338076 redcat-0.0.3/LICENSE
--rw-r--r--   0        0        0     2156 2023-05-21 04:17:02.338076 redcat-0.0.3/README.md
--rw-r--r--   0        0        0     4368 2023-05-21 04:17:02.338076 redcat-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      354 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/__init__.py
--rw-r--r--   0        0        0    17536 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/base.py
--rw-r--r--   0        0        0    16464 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/batchdict.py
--rw-r--r--   0        0        0     6626 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/batchlist.py
--rw-r--r--   0        0        0     2428 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/comparators.py
--rw-r--r--   0        0        0        0 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/datapipes/__init__.py
--rw-r--r--   0        0        0      315 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/datapipes/iter/__init__.py
--rw-r--r--   0        0        0     4087 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/datapipes/iter/batching.py
--rw-r--r--   0        0        0     3729 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/datapipes/iter/joining.py
--rw-r--r--   0        0        0     2123 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/datapipes/iter/shuffling.py
--rw-r--r--   0        0        0   140956 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/tensor.py
--rw-r--r--   0        0        0    52665 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/tensorseq.py
--rw-r--r--   0        0        0        0 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/utils/__init__.py
--rw-r--r--   0        0        0     1129 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/utils/format.py
--rw-r--r--   0        0        0     1446 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/utils/imports.py
--rw-r--r--   0        0        0    10154 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/utils/tensor.py
--rw-r--r--   0        0        0     3380 1970-01-01 00:00:00.000000 redcat-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-05-27 03:49:08.506193 redcat-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2156 2023-05-27 03:49:08.506193 redcat-0.0.4/README.md
+-rw-r--r--   0        0        0     4407 2023-05-27 03:49:08.506193 redcat-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      354 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/__init__.py
+-rw-r--r--   0        0        0    17482 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/base.py
+-rw-r--r--   0        0        0    17123 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/batchdict.py
+-rw-r--r--   0        0        0     6624 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/batchlist.py
+-rw-r--r--   0        0        0     2428 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/comparators.py
+-rw-r--r--   0        0        0        0 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/datapipes/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/datapipes/iter/__init__.py
+-rw-r--r--   0        0        0     4086 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/datapipes/iter/batching.py
+-rw-r--r--   0        0        0     3728 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/datapipes/iter/joining.py
+-rw-r--r--   0        0        0     2122 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/datapipes/iter/shuffling.py
+-rw-r--r--   0        0        0   140310 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/tensor.py
+-rw-r--r--   0        0        0    52673 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/tensorseq.py
+-rw-r--r--   0        0        0        0 2023-05-27 03:49:08.510193 redcat-0.0.4/src/redcat/utils/__init__.py
+-rw-r--r--   0        0        0     1128 2023-05-27 03:49:08.510193 redcat-0.0.4/src/redcat/utils/format.py
+-rw-r--r--   0        0        0     1446 2023-05-27 03:49:08.510193 redcat-0.0.4/src/redcat/utils/imports.py
+-rw-r--r--   0        0        0    10148 2023-05-27 03:49:08.510193 redcat-0.0.4/src/redcat/utils/tensor.py
+-rw-r--r--   0        0        0     3380 1970-01-01 00:00:00.000000 redcat-0.0.4/PKG-INFO
```

### Comparing `redcat-0.0.3/LICENSE` & `redcat-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `redcat-0.0.3/README.md` & `redcat-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `redcat-0.0.3/pyproject.toml` & `redcat-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redcat"
-version = "0.0.3"
+version = "0.0.4"
 description = "A library to manipulate batches of examples"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/redcat"
 repository = "https://github.com/durandtibo/redcat"
 keywords = ["batch"]
 license = "BSD-3-Clause"
@@ -39,21 +39,22 @@
 [tool.poetry.extras]
 all = [
     "polars",
 ]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3"
-coverage = { extras = ["toml"], version = ">=6.5,<8.0" }
-pre-commit = ">=2.21,<4.0"
+coverage = { extras = ["toml"], version = "^7.2" }
+docformatter = { extras = ["tomli"], version = "^1.7" }
+pre-commit = "^3.3"
 pylint = "^2.17"
 pytest = "^7.3"
-pytest-cov = "^4.0"
+pytest-cov = "^4.1"
 pytest-timeout = "^2.1"
-ruff = ">=0.0.262,<0.0.270"
+ruff = "^0.0,>=0.0.270"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
```

### Comparing `redcat-0.0.3/src/redcat/base.py` & `redcat-0.0.4/src/redcat/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         r"""Creates a copy of the current batch.
 
         Returns:
             ``BaseBatch``: A copy of the current batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch_copy = batch.clone()
             >>> batch_copy
             tensor([[1., 1., 1.],
@@ -73,15 +73,15 @@
 
         Returns:
             bool: ``True`` if the batches are equal within a tolerance,
                 ``False`` otherwise.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch1 = BatchedTensor(torch.ones(2, 3))
             >>> batch2 = BatchedTensor(torch.full((2, 3), 1.5))
             >>> batch1.allclose(batch2, atol=1, rtol=0)
             True
@@ -96,15 +96,15 @@
 
         Returns:
             bool: ``True`` if the batches have the same size,
                 elements and same batch dimension, ``False`` otherwise.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.ones(2, 3)).equal(BatchedTensor(torch.zeros(2, 3)))
             False
         """
 
@@ -123,15 +123,15 @@
                 input should be compatible with the shape of the data.
 
         Returns:
             ``BaseBatch``: A new batch with permuted data.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
             >>> batch.permute_along_batch([2, 1, 3, 0, 4])
             tensor([[4, 5],
                     [2, 3],
@@ -148,15 +148,15 @@
             permutation (sequence or ``torch.Tensor`` of type long
                 and shape ``(dimension,)``): Specifies the permutation
                 to use on the data. The dimension of the permutation
                 input should be compatible with the shape of the data.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
             >>> batch.permute_along_batch_([2, 1, 3, 0, 4])
             >>> batch
             tensor([[4, 5],
@@ -175,15 +175,15 @@
                 Default: ``None``
 
         Returns:
             ``BaseBatch``:  A new batch with shuffled data.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
             >>> batch.shuffle_along_batch()
             tensor([[4, 5],
                     [2, 3],
@@ -199,15 +199,15 @@
         Args:
             generator (``torch.Generator`` or ``None``, optional):
                 Specifies an optional random generator.
                 Default: ``None``
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
             >>> batch.shuffle_along_batch_()
             >>> batch
             tensor([[4, 5],
@@ -237,15 +237,15 @@
 
         Args:
             other (``TensorSeqBatch``): Specifies the batch to append
                 at the end of current batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.append(BatchedTensor(torch.zeros(1, 3)))
             >>> batch.append(BatchedTensor(torch.full((1, 3), 2.0)))
             >>> batch
@@ -267,15 +267,15 @@
                 dimension.
 
         Raises:
             RuntimeError if the number of chunks is incorrect
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2)).chunk_along_batch(chunks=3)
             (tensor([[0, 1], [2, 3]], batch_dim=0),
              tensor([[4, 5], [6, 7]], batch_dim=0),
              tensor([[8, 9]], batch_dim=0))
@@ -300,22 +300,20 @@
 
         Raises:
             TypeError: if there is no available implementation for the
                 input batch type.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
-            >>> batch.extend(
-            ...     [BatchedTensor(torch.zeros(1, 3)), BatchedTensor(torch.full((1, 3), 2.0))]
-            ... )
+            >>> batch.extend([BatchedTensor(torch.zeros(1, 3)), BatchedTensor(torch.full((1, 3), 2.0))])
             >>> batch.data
             tensor([[1., 1., 1.],
                     [1., 1., 1.],
                     [0., 0., 0.],
                     [2., 2., 2.]], batch_dim=0)
         """
 
@@ -330,15 +328,15 @@
         Returns:
             ``BaseBatch``: A new batch which indexes ``self``
                 along the batch dimension using the entries in
                 ``index``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
             >>> batch.index_select_along_batch([2, 4])
             tensor([[4, 5],
                     [8, 9]], batch_dim=0)
@@ -359,15 +357,15 @@
 
         Returns:
             ``BaseBatch``: The batch sliced along the batch
                 dimension at the given index.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2)).select_along_batch(2)
             tensor([4, 5])
         """
 
@@ -385,15 +383,15 @@
                 each index for slicing. Default: ``1``
 
         Returns:
             ``BaseBatch``: A slice of the current batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2)).slice_along_batch(start=2)
             tensor([[4, 5],
                     [6, 7],
                     [8, 9]], batch_dim=0)
@@ -417,15 +415,15 @@
 
         Returns:
             tuple: The batch split into chunks along the batch
                 dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2)).split_along_batch(2)
             (tensor([[0, 1], [2, 3]], batch_dim=0),
              tensor([[4, 5], [6, 7]], batch_dim=0),
              tensor([[8, 9]], batch_dim=0))
@@ -446,15 +444,15 @@
                 Default: ``False``
 
         Returns:
             int: The number of mini-batches.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10))
             >>> batch.get_num_minibatches(batch_size=4)
             3
             >>> batch.get_num_minibatches(batch_size=4, drop_last=True)
@@ -486,15 +484,15 @@
                 data. Default: ``False``
 
         Returns:
             iterable: The mini-batches.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> b = BatchedTensor(torch.arange(20).view(10, 2))
             >>> list(b.to_minibatches(batch_size=4))
             [tensor([[0, 1],
                      [2, 3],
```

### Comparing `redcat-0.0.3/src/redcat/batchdict.py` & `redcat-0.0.4/src/redcat/batchdict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 from __future__ import annotations
 
 __all__ = ["BatchDict", "check_same_batch_size", "check_same_keys", "get_seq_lens"]
 
 import copy
-from collections.abc import Hashable, Iterable, Sequence
+from collections.abc import (
+    Hashable,
+    ItemsView,
+    Iterable,
+    Iterator,
+    KeysView,
+    Sequence,
+    ValuesView,
+)
 from typing import Any, TypeVar
 
 import torch
 from coola import objects_are_allclose, objects_are_equal
 from coola.utils.format import str_indent
 from torch import Tensor
 
@@ -40,14 +48,49 @@
     def batch_size(self) -> int:
         return next(iter(self._data.values())).batch_size
 
     @property
     def data(self) -> dict[Hashable, BaseBatch]:
         return self._data
 
+    #################################
+    #     Dictionary operations     #
+    #################################
+
+    def __contains__(self, key: Hashable) -> bool:
+        return key in self._data
+
+    def __getitem__(self, key: Hashable) -> BaseBatch:
+        return self._data[key]
+
+    def __iter__(self) -> Iterator[Hashable]:
+        return iter(self._data)
+
+    def __len__(self) -> int:
+        return len(self._data)
+
+    def __setitem__(self, key: Hashable, value: BaseBatch) -> None:
+        if value.batch_size != self.batch_size:
+            raise RuntimeError(
+                f"Incorrect batch size. Expected {self.batch_size} but received {value.batch_size}"
+            )
+        self._data[key] = value
+
+    def get(self, key: Hashable, default: BaseBatch | None = None) -> BaseBatch | None:
+        return self._data.get(key, default)
+
+    def items(self) -> ItemsView:
+        return self._data.items()
+
+    def keys(self) -> KeysView:
+        return self._data.keys()
+
+    def values(self) -> ValuesView:
+        return self._data.values()
+
     ###############################
     #     Creation operations     #
     ###############################
 
     def clone(self) -> TBatchDict:
         return self.__class__(copy.deepcopy(self._data))
 
@@ -99,15 +142,15 @@
                 input should be compatible with the shape of the data.
 
         Returns:
             ``BatchDict``: A new batch with permuted data.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchDict, BatchList, BatchedTensorSeq
             >>> batch = BatchDict(
             ...     {
             ...         "key1": BatchedTensorSeq(torch.arange(10).view(2, 5)),
             ...         "key2": BatchList(["a", "b"]),
@@ -141,15 +184,15 @@
             permutation (sequence or ``torch.Tensor`` of type long
                 and shape ``(dimension,)``): Specifies the permutation
                 to use on the data. The dimension of the permutation
                 input should be compatible with the shape of the data.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchDict, BatchList, BatchedTensorSeq
             >>> batch = BatchDict(
             ...     {
             ...         "key1": BatchedTensorSeq(torch.arange(10).view(2, 5)),
             ...         "key2": BatchList(["a", "b"]),
@@ -182,15 +225,15 @@
             ``BatchDict``:  A new batch with shuffled data.
 
         Raises:
             RuntimeError if the batch has multiple sequence lengths.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchDict, BatchList, BatchedTensorSeq
             >>> batch = BatchDict(
             ...     {
             ...         "key1": BatchedTensorSeq(torch.arange(10).view(2, 5)),
             ...         "key2": BatchList(["a", "b"]),
@@ -224,15 +267,15 @@
                 Default: ``None``
 
         Raises:
             RuntimeError if the batch has multiple sequence lengths.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchDict, BatchList, BatchedTensorSeq
             >>> batch = BatchDict(
             ...     {
             ...         "key1": BatchedTensorSeq(torch.arange(10).view(2, 5)),
             ...         "key2": BatchList(["a", "b"]),
@@ -263,24 +306,14 @@
     #     Mathematical | trigo operations     #
     ###########################################
 
     ##########################################################
     #    Indexing, slicing, joining, mutating operations     #
     ##########################################################
 
-    def __getitem__(self, key: Hashable) -> BaseBatch:
-        return self._data[key]
-
-    def __setitem__(self, key: Hashable, value: BaseBatch) -> None:
-        if value.batch_size != self.batch_size:
-            raise RuntimeError(
-                f"Incorrect batch size. Expected {self.batch_size} but received {value.batch_size}"
-            )
-        self._data[key] = value
-
     def append(self, other: BatchDict) -> None:
         check_same_keys(self.data, other.data)
         for key, value in self._data.items():
             value.append(other[key])
 
     def cat_along_seq(self, batches: BatchDict | Sequence[BatchDict]) -> TBatchDict:
         r"""Concatenates the data of the batch(es) to the current batch
@@ -294,28 +327,26 @@
 
         Returns:
             ``BatchDict``: A batch with the concatenated data
                 along the sequence dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchDict, BatchList, BatchedTensorSeq
             >>> b = BatchDict(
             ...     {
             ...         "key1": BatchedTensorSeq(torch.arange(10).view(2, 5)),
             ...         "key2": BatchList(["a", "b"]),
             ...     }
             ... )
             >>> b.cat_along_seq(
-            ...     BatchDict(
-            ...         {"key1": BatchedTensorSeq(torch.tensor([[10, 11, 12], [20, 21, 22]]))}
-            ...     )
+            ...     BatchDict({"key1": BatchedTensorSeq(torch.tensor([[10, 11, 12], [20, 21, 22]]))})
             ... )
             BatchDict(
               (key1) tensor([[ 0,  1,  2,  3,  4, 10, 11, 12],
                              [ 5,  6,  7,  8,  9, 20, 21, 22]], batch_dim=0, seq_dim=1)
               (key2) BatchList(data=['a', 'b'])
             )
         """
@@ -336,28 +367,26 @@
 
         Args:
             batches (``BatchDict`` or  ``Sequence``): Specifies the
                 batch(es) to concatenate along the sequence dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchDict, BatchList, BatchedTensorSeq
             >>> b = BatchDict(
             ...     {
             ...         "key1": BatchedTensorSeq(torch.arange(10).view(2, 5)),
             ...         "key2": BatchList(["a", "b"]),
             ...     }
             ... )
             >>> b.cat_along_seq_(
-            ...     BatchDict(
-            ...         {"key1": BatchedTensorSeq(torch.tensor([[10, 11, 12], [20, 21, 22]]))}
-            ...     )
+            ...     BatchDict({"key1": BatchedTensorSeq(torch.tensor([[10, 11, 12], [20, 21, 22]]))})
             ... )
             >>> b
             BatchDict(
               (key1) tensor([[ 0,  1,  2,  3,  4, 10, 11, 12],
                              [ 5,  6,  7,  8,  9, 20, 21, 22]], batch_dim=0, seq_dim=1)
               (key2) BatchList(data=['a', 'b'])
             )
```

### Comparing `redcat-0.0.3/src/redcat/batchlist.py` & `redcat-0.0.4/src/redcat/batchlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
                 transformation of the data.
 
         Returns:
             ``BatchedTensor``: The transformed batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchList
             >>> BatchList([1, 2, 3]).apply(lambda val: val + 2)
             BatchList(data=[3, 4, 5])
         """
         return self._create_new_batch([fn(val) for val in self._data])
@@ -179,15 +179,15 @@
             fn (``Callable``): Specifies the function to be applied to
                 the element in the list. It is the responsibility of
                 the user to verify the function applies a valid
                 transformation of the data.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchList
             >>> batch = BatchList([1, 2, 3])
             >>> batch.apply_(lambda val: val + 2)
             >>> batch
             BatchList(data=[3, 4, 5])
```

### Comparing `redcat-0.0.3/src/redcat/comparators.py` & `redcat-0.0.4/src/redcat/comparators.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.3/src/redcat/datapipes/iter/batching.py` & `redcat-0.0.4/src/redcat/datapipes/iter/batching.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             shuffling is done per batch. Default: ``False``
         random_seed (int, optional): Specifies the random seed used to
             shuffle the batch before to split it.
             Default: ``5513175564631803238``
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> import torch
         >>> from torch.utils.data.datapipes.iter import IterableWrapper
         >>> from redcat import BatchedTensor
         >>> from redcat.datapipes.iter import MiniBatcher
         >>> datapipe = MiniBatcher(
         ...     IterableWrapper([BatchedTensor(torch.arange(4).add(i * 4)) for i in range(2)]),
```

### Comparing `redcat-0.0.3/src/redcat/datapipes/iter/joining.py` & `redcat-0.0.4/src/redcat/datapipes/iter/joining.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             batch. Default: ``10``
         drop_last (bool, optional): If ``True``, the last samples are
             dropped if the buffer is not full, otherwise it is
             returned. Default: ``False``
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> import torch
         >>> from torch.utils.data.datapipes.iter import IterableWrapper
         >>> from redcat import BatchedTensor
         >>> from redcat.datapipes.iter import BatchExtender
         >>> datapipe = BatchExtender(
         ...     IterableWrapper([BatchedTensor(torch.ones(2) * i) for i in range(10)]),
```

### Comparing `redcat-0.0.3/src/redcat/datapipes/iter/shuffling.py` & `redcat-0.0.4/src/redcat/datapipes/iter/shuffling.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         datapipe (``IterDataPipe``): Specifies the source DataPipe.
             The DataPipe has to return ``BaseBatch`` objects.
         random_seed (int, optional): Specifies the random seed used
             to shuffle the data. Default: ``3770589329299158004``
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> import torch
         >>> from torch.utils.data.datapipes.iter import IterableWrapper
         >>> from redcat import BatchedTensor
         >>> from redcat.datapipes.iter import BatchShuffler
         >>> datapipe = BatchShuffler(
         ...     IterableWrapper([BatchedTensor(torch.arange(4).add(i)) for i in range(2)])
```

### Comparing `redcat-0.0.3/src/redcat/tensor.py` & `redcat-0.0.4/src/redcat/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         r"""Gets the number of dimensions.
 
         Returns:
             int: The number of dimensions
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.ones(2, 3)).dim()
             2
         """
         return self._data.dim()
@@ -108,15 +108,15 @@
         r"""Gets the number of dimensions.
 
         Returns:
             int: The number of dimensions
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.ones(2, 3)).ndimension()
             2
         """
         return self.dim()
@@ -125,15 +125,15 @@
         r"""Gets the total number of elements in the tensor.
 
         Returns:
             int: The total number of elements
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.ones(2, 3)).numel()
             6
         """
         return self._data.numel()
@@ -154,15 +154,15 @@
 
         Returns:
             ``BatchedTensor``: A new batch with a contiguous
                 representation of the data.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3)).contiguous()
             >>> batch.is_contiguous()
             True
         """
@@ -179,15 +179,15 @@
 
         Returns:
             bool: ``True`` if the data are stored with a contiguous
                 tensor, otherwise ``False``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.ones(2, 3)).is_contiguous()
             True
         """
         return self._data.is_contiguous(memory_format=memory_format)
@@ -201,20 +201,20 @@
 
         Returns:
             ``BatchedTensor``: A new batch with the data after
                 dtype and/or device conversion.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
-            >>> batch_cuda = batch.to(device=torch.device('cuda:0'))
+            >>> batch_cuda = batch.to(device=torch.device("cuda:0"))
             >>> batch_bool = batch.to(dtype=torch.bool)
             >>> batch_bool
             tensor([[True, True, True],
                     [True, True, True]], batch_dim=0)
         """
         return self._create_new_batch(self._data.to(*args, **kwargs))
 
@@ -230,15 +230,15 @@
             **kwargs: See the documentation of ``torch.Tensor.clone``
 
         Returns:
             ``BatchedTensor``: A copy of the current batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch_copy = batch.clone()
             >>> batch_copy
             tensor([[1., 1., 1.],
@@ -257,15 +257,15 @@
 
         Returns:
             ``BatchedTensor``: A uninitialized batch with the same
                 shape as the current batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.empty_like(42)
             tensor([[0., 0., 0.],
                     [0., 0., 0.]], batch_dim=0)
@@ -283,15 +283,15 @@
 
         Returns:
             ``BatchedTensor``: A batch filled with the scalar
                 value, with the same shape as the current batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.full_like(42)
             tensor([[42., 42., 42.],
                     [42., 42., 42.]], batch_dim=0)
@@ -320,15 +320,15 @@
                 ``torch.Tensor.new_full``.
 
         Returns:
             ``BatchedTensor``: A batch filled with the scalar value.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.new_full(42)
             tensor([[42., 42., 42.],
                     [42., 42., 42.]], batch_dim=0)
@@ -366,15 +366,15 @@
 
         Returns:
             ``BatchedTensor``: A batch filled with the scalar
                 value ``1``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.zeros(2, 3))
             >>> batch.new_ones()
             tensor([[1., 1., 1.],
                     [1., 1., 1.]], batch_dim=0)
@@ -412,15 +412,15 @@
 
         Returns:
             ``BatchedTensor``: A batch filled with the scalar
                 value ``0``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.new_zeros()
             tensor([[0., 0., 0.],
                     [0., 0., 0.]], batch_dim=0)
@@ -450,15 +450,15 @@
         Returns:
             ``BatchedTensor``: A batch filled with the scalar
                 value ``1``, with the same shape as the current
                 batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.ones_like()
             tensor([[1., 1., 1.],
                     [1., 1., 1.]], batch_dim=0)
@@ -477,15 +477,15 @@
         Returns:
             ``BatchedTensor``: A batch filled with the scalar
                 value ``0``, with the same shape as the current
                 batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.zeros_like()
             tensor([[0., 0., 0.],
                     [0., 0., 0.]], batch_dim=0)
@@ -530,15 +530,15 @@
 
         Returns:
             ``BatchedTensor``: A batch containing the element-wise
                 equality.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch1 = BatchedTensor(torch.tensor([[1, 3, 4], [0, 2, 2]]))
             >>> batch2 = BatchedTensor(torch.tensor([[5, 3, 2], [0, 1, 2]]))
             >>> batch1.eq(batch2)
             tensor([[False,  True, False],
@@ -568,15 +568,15 @@
 
         Returns:
             ``BatchedTensor``: A batch containing the element-wise
                 comparison.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch1 = BatchedTensor(torch.tensor([[1, 3, 4], [0, 2, 2]]))
             >>> batch2 = BatchedTensor(torch.tensor([[5, 3, 2], [0, 1, 2]]))
             >>> batch1.ge(batch2)
             tensor([[False,  True,  True],
@@ -598,15 +598,15 @@
 
         Returns:
             ``BatchedTensor``: A batch containing the element-wise
                 comparison.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch1 = BatchedTensor(torch.tensor([[1, 3, 4], [0, 2, 2]]))
             >>> batch2 = BatchedTensor(torch.tensor([[5, 3, 2], [0, 1, 2]]))
             >>> batch1.gt(batch2)
             tensor([[False, False,  True],
@@ -627,20 +627,20 @@
         Returns:
             BatchedTensor:  A batch containing a boolean tensor
                 that is ``True`` where the current batch is infinite
                 and ``False`` elsewhere.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(
-            ...     torch.tensor([[1.0, 0.0, float('inf')], [-1.0, -2.0, float('-inf')]])
+            ...     torch.tensor([[1.0, 0.0, float("inf")], [-1.0, -2.0, float("-inf")]])
             ... )
             >>> batch.isinf()
             tensor([[False, False, True],
                     [False, False, True]], batch_dim=0)
         """
         return torch.isinf(self)
 
@@ -651,20 +651,20 @@
         Returns:
             BatchedTensor:  A batch containing a boolean tensor
                 that is ``True`` where the current batch is negative
                 infinity and ``False`` elsewhere.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(
-            ...     torch.tensor([[1.0, 0.0, float('inf')], [-1.0, -2.0, float('-inf')]])
+            ...     torch.tensor([[1.0, 0.0, float("inf")], [-1.0, -2.0, float("-inf")]])
             ... )
             >>> batch.isneginf()
             tensor([[False, False, False],
                     [False, False,  True]], batch_dim=0)
         """
         return torch.isneginf(self)
 
@@ -675,20 +675,20 @@
         Returns:
             BatchedTensor:  A batch containing a boolean tensor
                 that is ``True`` where the current batch is positive
                 infinity and ``False`` elsewhere.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(
-            ...     torch.tensor([[1.0, 0.0, float('inf')], [-1.0, -2.0, float('-inf')]])
+            ...     torch.tensor([[1.0, 0.0, float("inf")], [-1.0, -2.0, float("-inf")]])
             ... )
             >>> batch.isposinf()
             tensor([[False, False,   True],
                     [False, False,  False]], batch_dim=0)
         """
         return torch.isposinf(self)
 
@@ -698,20 +698,20 @@
         Returns:
             BatchedTensor:  A batch containing a boolean tensor
                 that is ``True`` where the current batch is infinite
                 and ``False`` elsewhere.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(
-            ...     torch.tensor([[1.0, 0.0, float('nan')], [float('nan'), -2.0, -1.0]])
+            ...     torch.tensor([[1.0, 0.0, float("nan")], [float("nan"), -2.0, -1.0]])
             ... )
             >>> batch.isnan()
             tensor([[False, False,  True],
                     [ True, False, False]], batch_dim=0)
         """
         return torch.isnan(self)
 
@@ -723,15 +723,15 @@
 
         Returns:
             ``BatchedTensor``: A batch containing the element-wise
                 comparison.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch1 = BatchedTensor(torch.tensor([[1, 3, 4], [0, 2, 2]]))
             >>> batch2 = BatchedTensor(torch.tensor([[5, 3, 2], [0, 1, 2]]))
             >>> batch1.le(batch2)
             tensor([[ True,  True, False],
@@ -753,15 +753,15 @@
 
         Returns:
             ``BatchedTensor``: A batch containing the element-wise
                 comparison.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch1 = BatchedTensor(torch.tensor([[1, 3, 4], [0, 2, 2]]))
             >>> batch2 = BatchedTensor(torch.tensor([[5, 3, 2], [0, 1, 2]]))
             >>> batch1.lt(batch2)
             tensor([[ True, False, False],
@@ -788,15 +788,15 @@
         r"""Converts the current batch to bool data type.
 
         Returns:
             ``BatchedTensor``: The current batch to bool data type.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.bool().dtype
             torch.bool
         """
@@ -806,15 +806,15 @@
         r"""Converts the current batch to double data type.
 
         Returns:
             ``BatchedTensor``: The current batch to double data type.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.double().dtype
             torch.float64
         """
@@ -824,15 +824,15 @@
         r"""Converts the current batch to float data type.
 
         Returns:
             ``BatchedTensor``: The current batch to float data type.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.float().dtype
             torch.float32
         """
@@ -842,15 +842,15 @@
         r"""Converts the current batch to int data type.
 
         Returns:
             ``BatchedTensor``: The current batch to int data type.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.int().dtype
             torch.int32
         """
@@ -860,15 +860,15 @@
         r"""Converts the current batch to long data type.
 
         Returns:
             ``BatchedTensor``: The current batch to long data type.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.long().dtype
             torch.int64
         """
@@ -928,15 +928,15 @@
 
         Returns:
             ``BatchedTensor``: A new batch containing the addition of
                 the two batches.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> out = batch.add(BatchedTensor(torch.full((2, 3), 2.0)))
             >>> batch
             tensor([[1., 1., 1.],
@@ -962,15 +962,15 @@
                 float): Specifies the other value to add to the
                 current batch.
             alpha (int or float, optional): Specifies the scale of the
                 batch to add. Default: ``1.0``
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.add_(BatchedTensor(torch.full((2, 3), 2.0)))
             >>> batch
             tensor([[3., 3., 3.],
@@ -1001,15 +1001,15 @@
 
         Returns:
             ``BatchedTensor``: A new batch containing the division
                 of the two batches.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> out = batch.div(BatchedTensor(torch.full((2, 3), 2.0)))
             >>> batch
             tensor([[1., 1., 1.],
@@ -1038,15 +1038,15 @@
                 - ``"trunc"``: rounds the results of the division
                     towards zero.
                 - ``"floor"``: floor division.
                 Default: ``None``
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.div_(BatchedTensor(torch.full((2, 3), 2.0)))
             >>> batch
             tensor([[0.5000, 0.5000, 0.5000],
@@ -1069,15 +1069,15 @@
 
         Returns:
             ``BatchedTensor``: A new batch containing the
                 element-wise remainder of division.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> out = batch.fmod(BatchedTensor(torch.full((2, 3), 2.0)))
             >>> batch
             tensor([[1., 1., 1.],
@@ -1095,15 +1095,15 @@
 
         Args:
             divisor (``BatchedTensor`` or ``torch.Tensor`` or int
                 or float): Specifies the divisor.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.fmod_(BatchedTensor(torch.full((2, 3), 2.0)))
             >>> batch
             tensor([[1., 1., 1.],
@@ -1123,15 +1123,15 @@
 
         Returns:
             ``BatchedTensor``: A new batch containing the
                 multiplication of the two batches.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> out = batch.mul(BatchedTensor(torch.full((2, 3), 2.0)))
             >>> batch
             tensor([[1., 1., 1.],
@@ -1153,15 +1153,15 @@
 
         Returns:
             ``BatchedTensor``: A new batch containing the
                 multiplication of the two batches.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.mul_(BatchedTensor(torch.full((2, 3), 2.0)))
             >>> batch
             tensor([[2., 2., 2.],
@@ -1175,15 +1175,15 @@
 
         Returns:
             ``BatchedTensor``: A new batch with the negative of
                 the elements.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> out = batch.neg()
             >>> batch
             tensor([[1., 1., 1.],
@@ -1212,15 +1212,15 @@
 
         Returns:
             ``BatchedTensor``: A new batch containing the diffence of
                 the two batches.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> out = batch.sub(BatchedTensor(torch.full((2, 3), 2.0)))
             >>> batch
             tensor([[1., 1., 1.],
@@ -1245,15 +1245,15 @@
             other (``BatchedTensor`` or ``torch.Tensor`` or int or
                 float): Specifies the value to subtract.
             alpha (int or float, optional): Specifies the scale of the
                 batch to substract. Default: ``1``
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.ones(2, 3))
             >>> batch.sub_(BatchedTensor(torch.full((2, 3), 2.0)))
             >>> batch
             tensor([[-1., -1., -1.],
@@ -1276,15 +1276,15 @@
 
         Returns:
             ``BatchedTensor``: A batch with the cumulative sum of
                 elements of the current batch in a given dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(2, 5)).cumsum(dim=1)
             tensor([[ 0,  1,  2,  3,  4],
                     [ 5,  7,  9, 11, 13]], batch_dim=0)
         """
@@ -1296,15 +1296,15 @@
 
         Args:
             dim (int): Specifies the dimension of the cumulative sum.
             **kwargs: see ``torch.cumsum_`` documentation
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
             >>> batch.cumsum_(dim=1)
             >>> batch
             tensor([[ 0,  1,  2,  3,  4],
@@ -1321,15 +1321,15 @@
 
         Returns:
             ``BatchedTensor``: A batch with the cumulative sum of
                 elements of the current batch in the batch dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(2, 5)).cumsum_along_batch()
             tensor([[ 0,  1,  2,  3,  4],
                     [ 5,  7,  9, 11, 13]], batch_dim=0)
         """
@@ -1337,15 +1337,15 @@
 
     def cumsum_along_batch_(self) -> None:
         r"""Computes the cumulative sum of elements of the current batch
         in the batch dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
             >>> batch.cumsum_along_batch_()
             >>> batch
             tensor([[ 0,  1,  2,  3,  4],
@@ -1364,15 +1364,15 @@
         Returns:
             ``BatchedTensor``: A batch with the cumulative
                 summation of the exponentiation of elements of the
                 current batch in a given dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(2, 5).float()).logcumsumexp(dim=1)
             tensor([[0.0000, 1.3133, 2.4076, 3.4402, 4.4519],
                     [5.0000, 6.3133, 7.4076, 8.4402, 9.4519]], batch_dim=0)
         """
@@ -1384,15 +1384,15 @@
         dimension.
 
         Args:
             dim (int): Specifies the dimension of the cumulative sum.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(2, 5).float())
             >>> batch.logcumsumexp_(dim=1)
             >>> batch
             tensor([[0.0000, 1.3133, 2.4076, 3.4402, 4.4519],
@@ -1408,15 +1408,15 @@
         Returns:
             ``BatchedTensor``: A batch with the cumulative
                 summation of the exponentiation of elements of the
                 current batch in the batch dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2).float()).logcumsumexp_along_batch()
             tensor([[0.0000, 1.0000],
                     [2.1269, 3.1269],
                     [4.1429, 5.1429],
@@ -1428,15 +1428,15 @@
     def logcumsumexp_along_batch_(self) -> None:
         r"""Computes the logarithm of the cumulative summation of the
         exponentiation of elements of the current batch in the batch
         dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(5, 2).float())
             >>> batch.logcumsumexp_along_batch_()
             >>> batch
             tensor([[0.0000, 1.0000],
@@ -1465,15 +1465,15 @@
                 is computed.
 
         Returns:
             ``BatchedTensor``: A new batch with permuted data.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2)).permute_along_dim([2, 1, 3, 0, 4], dim=0)
             tensor([[4, 5],
                     [2, 3],
                     [6, 7],
@@ -1495,15 +1495,15 @@
                 to use on the data. The dimension of the permutation
                 input should be compatible with the shape of the data.
             dim (int): Specifies the dimension where the permutation
                 is computed.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
             >>> batch.permute_along_dim_([2, 1, 3, 0, 4], dim=0)
             >>> batch
             tensor([[4, 5],
@@ -1528,15 +1528,15 @@
 
         Returns:
             ``BatchedTensor``:  A new batch with shuffled data
                 along a given dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2)).shuffle_along_dim(dim=0)
             tensor([[4, 5],
                     [2, 3],
                     [6, 7],
@@ -1557,15 +1557,15 @@
 
         Returns:
             ``BatchedTensor``:  A new batch with shuffled data
                 along a given dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
             >>> batch.shuffle_along_dim_(dim=0)
             >>> batch
             tensor([[4, 5],
@@ -1599,15 +1599,15 @@
                     - The first batch contains the batch values sorted
                         along the given dimension.
                     - The second batch contains the indices that sort
                         the batch along the given dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.rand(2, 5)).sort()
             torch.return_types.sort(
             values=tensor([[0.0239, 0.1395, 0.1742, 0.2742, 0.3203],
                     [0.1096, 0.1745, 0.5360, 0.8954, 0.9036]], batch_dim=0),
@@ -1638,15 +1638,15 @@
                     - The first batch contains the batch values sorted
                         along the given dimension.
                     - The second batch contains the indices that sort
                         the batch along the given dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.rand(2, 5)).sort_along_batch()
             torch.return_types.sort(
             values=tensor([[0.0091, 0.5615, 0.5453, 0.1468, 0.5192],
                     [0.4122, 0.8932, 0.8783, 0.6494, 0.7763]], batch_dim=0),
@@ -1664,15 +1664,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the absolute value of
                 each element.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[-2.0, 0.0, 2.0], [-1.0, 1.0, 3.0]]))
             >>> batch.abs()
             tensor([[2., 0., 2.],
                     [1., 1., 3.]], batch_dim=0)
@@ -1682,15 +1682,15 @@
     def abs_(self) -> None:
         r"""Computes the absolute value of each element.
 
         In-place version of ``abs()``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[-2.0, 0.0, 2.0], [-1.0, 1.0, 3.0]]))
             >>> batch.abs_()
             >>> batch
             tensor([[2., 0., 2.],
@@ -1716,15 +1716,15 @@
                 there is no upper bound. Default: ``None``
 
         Returns:
             ``BatchedTensor``: A batch with clamped values.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
             >>> batch.clamp(min=2, max=5)
             tensor([[2, 2, 2, 3, 4],
                     [5, 5, 5, 5, 5]], batch_dim=0)
@@ -1755,15 +1755,15 @@
                 there is no lower bound. Default: ``None``
             max (int, float or ``None``, optional): Specifies
                 the upper bound. If ``max`` is ``None``,
                 there is no upper bound. Default: ``None``
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
             >>> batch.clamp_(min=2, max=5)
             >>> batch
             tensor([[2, 2, 2, 3, 4],
@@ -1786,15 +1786,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the exponential of the
                 elements of the current batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[0.0, 1.0, 2.0], [3.0, 4.0, 5.0]]))
             >>> batch.exp()
             tensor([[  2.7183,   7.3891,  20.0855],
                     [ 54.5981, 148.4132, 403.4288]], batch_dim=0)
@@ -1804,15 +1804,15 @@
     def exp_(self) -> None:
         r"""Computes the exponential of the elements.
 
         In-place version of ``exp()``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[0.0, 1.0, 2.0], [3.0, 4.0, 5.0]]))
             >>> batch.exp_()
             >>> batch
             tensor([[  2.7183,   7.3891,  20.0855],
@@ -1825,15 +1825,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the natural
                 logarithm of the elements of the current batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(
             ...     torch.tensor([[0.0, 1.0, 2.0, 3.0, 4.0], [5.0, 6.0, 7.0, 8.0, 9.0]])
             ... )
             >>> batch.log()
@@ -1845,15 +1845,15 @@
     def log_(self) -> None:
         r"""Computes the natural logarithm of the elements.
 
         In-place version of ``log()``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(
             ...     torch.tensor([[0.0, 1.0, 2.0, 3.0, 4.0], [5.0, 6.0, 7.0, 8.0, 9.0]])
             ... )
             >>> batch.log_()
@@ -1868,33 +1868,35 @@
 
         Return:
             ``BatchedTensor``: A batch with the natural
                 logarithm of ``self + 1``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> batch = BatchedTensor(torch.tensor([[0.0, 1.0, 2.0, 3.0, 4.0], [5.0, 6.0, 7.0, 8.0, 9.0]]))
+            >>> batch = BatchedTensor(
+            ...     torch.tensor([[0.0, 1.0, 2.0, 3.0, 4.0], [5.0, 6.0, 7.0, 8.0, 9.0]])
+            ... )
             >>> batch.log1p()
             tensor([[0.0000, 0.6931, 1.0986, 1.3863, 1.6094],
                     [1.7918, 1.9459, 2.0794, 2.1972, 2.3026]], batch_dim=0)
         """
         return torch.log1p(self)
 
     def log1p_(self) -> None:
         r"""Computes the natural logarithm of ``self + 1``.
 
         In-place version of ``log1p()``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(
             ...     torch.tensor([[0.0, 1.0, 2.0, 3.0, 4.0], [5.0, 6.0, 7.0, 8.0, 9.0]])
             ... )
             >>> batch.log1p_()
@@ -1913,15 +1915,15 @@
 
         Returns:
             ``BatchedTensor``: The batch with the element-wise
                 maximum of ``self`` and ``other``
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(6).view(2, 3))
             >>> batch.maximum(BatchedTensor(torch.tensor([[1, 0, 2], [4, 5, 3]])))
             tensor([[1, 1, 2],
                     [4, 5, 5]], batch_dim=0)
@@ -1937,15 +1939,15 @@
 
         Returns:
             ``BatchedTensor``: The batch with the element-wise
                 minimum of ``self`` and ``other``
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(6).view(2, 3))
             >>> batch.minimum(BatchedTensor(torch.tensor([[1, 0, 2], [4, 5, 3]])))
             tensor([[0, 0, 2],
                     [3, 4, 3]], batch_dim=0)
@@ -1963,15 +1965,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the power of each
                 element with the given exponent.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[0.0, 1.0, 2.0], [3.0, 4.0, 5.0]]))
             >>> batch.pow(2)
             tensor([[ 0.,  1.,  4.],
                     [ 9., 16., 25.]], batch_dim=0)
@@ -1987,15 +1989,15 @@
             exponent (int or float or ``BatchedTensor``): Specifies
                 the exponent value. ``exponent`` can be either a
                 single numeric number or a ``BatchedTensor``
                 with the same number of elements.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[0.0, 1.0, 2.0], [3.0, 4.0, 5.0]]))
             >>> batch.pow_(2)
             >>> batch
             tensor([[ 0.,  1.,  4.],
@@ -2009,15 +2011,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the square-root of
                 each element.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.tensor([[1.0, 4.0], [16.0, 25.0]])).rsqrt()
             tensor([[1.0000, 0.5000],
                     [0.2500, 0.2000]], batch_dim=0)
         """
@@ -2026,15 +2028,15 @@
     def rsqrt_(self) -> None:
         r"""Computes the reciprocal of the square-root of each element.
 
         In-place version of ``rsqrt()``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[1.0, 4.0], [16.0, 25.0]]))
             >>> batch.rsqrt_()
             >>> batch
             tensor([[1.0000, 0.5000],
@@ -2047,15 +2049,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the square-root of
                 each element.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[0.0, 1.0, 4.0], [9.0, 16.0, 25.0]]))
             >>> batch.sqrt()
             tensor([[0., 1., 2.],
                     [3., 4., 5.]], batch_dim=0)
@@ -2065,15 +2067,15 @@
     def sqrt_(self) -> None:
         r"""Computes the square-root of each element.
 
         In-place version of ``sqrt()``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[0.0, 1.0, 4.0], [9.0, 16.0, 25.0]]))
             >>> batch.sqrt_()
             >>> batch
             tensor([[0., 1., 2.],
@@ -2094,15 +2096,15 @@
 
         Returns:
             ``torch.Tensor`` or ``torch.return_types.max``:
                 The maximum of all elements.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(2, 5)).max()
             tensor(9)
             >>> BatchedTensor(torch.arange(10).view(2, 5)).max(dim=1)
             torch.return_types.max(
@@ -2125,27 +2127,25 @@
 
         Returns:
             ``torch.return_types.max``: A batch with
                 the maximum values along the batch dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(
-            ...     torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])
-            ... ).max_along_batch()
+            >>> BatchedTensor(torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])).max_along_batch()
             torch.return_types.max(
             values=tensor([4, 9]),
             indices=tensor([4, 4]))
-            >>> BatchedTensor(
-            ...     torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])
-            ... ).max_along_batch(keepdim=True)
+            >>> BatchedTensor(torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])).max_along_batch(
+            ...     keepdim=True
+            ... )
             torch.return_types.max(
             values=tensor([[4], [9]]),
             indices=tensor([[4], [4]]))
         """
         return self.max(dim=self._batch_dim, keepdim=keepdim)
 
     def mean(self, *args, **kwargs) -> Tensor:
@@ -2156,15 +2156,15 @@
             **kwargs: See the documentation of ``torch.Tensor.mean``
 
         Returns:
             ``torch.Tensor``: The mean of all elements.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(2, 5).float()).mean()
             tensor(4.5)
             >>> BatchedTensor(torch.arange(10).view(2, 5).float()).mean(dim=1)
             tensor([2.0, 7.0])
@@ -2183,15 +2183,15 @@
 
         Returns:
             ``torch.Tensor``: A batch with
                 the mean values along the batch dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2).float()).mean_along_batch()
             tensor([4.0, 5.0])
             >>> BatchedTensor(torch.arange(10).view(5, 2).float()).mean_along_batch(keepdim=True)
             tensor([[4.0], [5.0]])
@@ -2210,15 +2210,15 @@
                 The median of all elements or per dimension.
                 The first tensor will be populated with the median
                 values and the second tensor, which must have dtype
                 long, with their indices in the dimension dim of input.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(2, 5)).median()
             tensor(4)
             >>> BatchedTensor(torch.arange(10).view(2, 5)).median(dim=1)
             torch.return_types.median(
@@ -2243,15 +2243,15 @@
             ``torch.return_types.median``:  The first tensor will
                 be populated with the median values and the second
                 tensor, which must have dtype long, with their indices
                 in the batch dimension of input.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(
             ...     torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])
             ... ).median_along_batch()
             torch.return_types.median(
@@ -2269,15 +2269,15 @@
 
         Returns:
             ``torch.Tensor`` or ``torch.return_types.min``:
                 The minimum of all elements.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(2, 5)).min()
             tensor(0)
             >>> BatchedTensor(torch.arange(10).view(2, 5)).min(dim=1)
             torch.return_types.min(
@@ -2300,27 +2300,25 @@
 
         Returns:
             ``torch.return_types.min``: A batch with
                 the minimum values along the batch dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(
-            ...     torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])
-            ... ).min_along_batch()
+            >>> BatchedTensor(torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])).min_along_batch()
             torch.return_types.min(
             values=tensor([0, 5]),
             indices=tensor([0, 0]))
-            >>> BatchedTensor(
-            ...     torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])
-            ... ).min_along_batch(keepdim=True)
+            >>> BatchedTensor(torch.tensor([[0, 5], [1, 6], [2, 7], [3, 8], [4, 9]])).min_along_batch(
+            ...     keepdim=True
+            ... )
             torch.return_types.min(
             values=tensor([[0], [5]]),
             indices=tensor([[0], [0]]))
         """
         return self.min(dim=self._batch_dim, keepdim=keepdim)
 
     def nanmean(self, *args, **kwargs) -> Tensor:
@@ -2331,29 +2329,27 @@
             **kwargs: See the documentation of ``torch.Tensor.nanmean``
 
         Returns:
             ``torch.Tensor``: The mean of all elements.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(
-            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
-            ... ).nanmean()
+            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nanmean()
             tensor(4.0)
-            >>> BatchedTensor(
-            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
-            ... ).nanmean(dim=1)
+            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nanmean(
+            ...     dim=1
+            ... )
             tensor([2.0, 6.5])
-            >>> BatchedTensor(
-            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
-            ... ).nanmean(dim=1, keepdim=True)
+            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nanmean(
+            ...     dim=1, keepdim=True
+            ... )
             tensor([[2.0], [6.5]])
         """
         return torch.nanmean(self, *args, **kwargs)
 
     def nanmean_along_batch(self, keepdim: bool = False) -> Tensor:
         r"""Computes the mean values along the batch dimension.
 
@@ -2364,24 +2360,24 @@
 
         Returns:
             ``torch.Tensor``: A batch with
                 the mean values along the batch dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(
-            ...     torch.tensor([[0., 5.], [1., 6.], [2., 7.], [3., 8.], [4., float("nan")]])
+            ...     torch.tensor([[0.0, 5.0], [1.0, 6.0], [2.0, 7.0], [3.0, 8.0], [4.0, float("nan")]])
             ... ).nanmean_along_batch()
             tensor([2.0, 6.5])
             >>> BatchedTensor(
-            ...     torch.tensor([[0., 5.], [1., 6.], [2., 7.], [3., 8.], [4., float("nan")]])
+            ...     torch.tensor([[0.0, 5.0], [1.0, 6.0], [2.0, 7.0], [3.0, 8.0], [4.0, float("nan")]])
             ... ).nanmean_along_batch(keepdim=True)
             tensor([[2.0, 6.5]])
         """
         return self.nanmean(dim=self._batch_dim, keepdim=keepdim)
 
     def nanmedian(self, *args, **kwargs) -> Tensor | torch.return_types.nanmedian:
         r"""Computes the median of all elements.
@@ -2395,31 +2391,29 @@
                 The median of all elements or per dimension.
                 The first tensor will be populated with the median
                 values and the second tensor, which must have dtype
                 long, with their indices in the dimension dim of input.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(
-            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
-            ... ).nanmedian()
+            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nanmedian()
             tensor(4.0)
-            >>> BatchedTensor(
-            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
-            ... ).nanmedian(dim=1)
+            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nanmedian(
+            ...     dim=1
+            ... )
             torch.return_types.nanmedian(
             values=tensor([2., 6.]),
             indices=tensor([2, 1]))
-            >>> BatchedTensor(
-            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
-            ... ).nanmedian(dim=1, keepdim=True)
+            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nanmedian(
+            ...     dim=1, keepdim=True
+            ... )
             torch.return_types.nanmedian(
             values=tensor([[2.], [6.]]),
             indices=tensor([[2], [1]]))
         """
         return torch.nanmedian(self, *args, **kwargs)
 
     def nanmedian_along_batch(self, keepdim: bool = False) -> torch.return_types.nanmedian:
@@ -2434,20 +2428,20 @@
             ``torch.return_types.nanmedian``:  The first tensor will
                 be populated with the median values and the second
                 tensor, which must have dtype long, with their indices
                 in the batch dimension of input.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(
-            ...     torch.tensor([[0., 5.], [1., 6.], [2., 7.], [3., 8.], [4., float("nan")]])
+            ...     torch.tensor([[0.0, 5.0], [1.0, 6.0], [2.0, 7.0], [3.0, 8.0], [4.0, float("nan")]])
             ... ).nanmedian_along_batch()
             torch.return_types.nanmedian(
             values=tensor([2., 6.]),
             indices=tensor([2, 1]))
         """
         return self.nanmedian(dim=self._batch_dim, keepdim=keepdim)
 
@@ -2459,29 +2453,25 @@
             **kwargs: See the documentation of ``torch.Tensor.nansum``
 
         Returns:
             ``torch.Tensor``: The sum of all elements.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(
-            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
-            ... ).nansum()
+            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nansum()
             tensor(36.)
-            >>> BatchedTensor(
-            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
-            ... ).nansum(dim=1)
+            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nansum(dim=1)
             tensor([10., 26.])
-            >>> BatchedTensor(
-            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
-            ... ).nansum(dim=1, keepdim=True)
+            >>> BatchedTensor(torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])).nansum(
+            ...     dim=1, keepdim=True
+            ... )
             tensor([[10.], [26.]])
         """
         return torch.nansum(self, *args, **kwargs)
 
     def nansum_along_batch(self, keepdim: bool = False) -> Tensor:
         r"""Computes the sum values along the batch dimension.
 
@@ -2492,20 +2482,20 @@
 
         Returns:
             ``torch.Tensor``: A tensor with the sum values along the
                 batch dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(
-            ...     torch.tensor([[0., 5.], [1., 6.], [2., 7.], [3., 8.], [4., float("nan")]])
+            ...     torch.tensor([[0.0, 5.0], [1.0, 6.0], [2.0, 7.0], [3.0, 8.0], [4.0, float("nan")]])
             ... ).nansum_along_batch()
             tensor([20., 26.])
         """
         return self.nansum(dim=self._batch_dim, keepdim=keepdim)
 
     def prod(self, *args, **kwargs) -> Tensor:
         r"""Computes the product of all elements.
@@ -2515,29 +2505,25 @@
             **kwargs: See the documentation of ``torch.Tensor.nansum``
 
         Returns:
             ``torch.Tensor``: The product of all elements.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(
-            ...     torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])
-            ... ).prod()
+            >>> BatchedTensor(torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])).prod()
             tensor(362880)
-            >>> BatchedTensor(
-            ...     torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])
-            ... ).prod(dim=1)
+            >>> BatchedTensor(torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])).prod(dim=1)
             tensor([ 120, 3024])
-            >>> BatchedTensor(
-            ...     torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])
-            ... ).prod(dim=1, keepdim=True)
+            >>> BatchedTensor(torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])).prod(
+            ...     dim=1, keepdim=True
+            ... )
             tensor([[ 120], [3024]])
         """
         return torch.prod(self, *args, **kwargs)
 
     def prod_along_batch(self, keepdim: bool = False) -> Tensor:
         r"""Computes the product values along the batch dimension.
 
@@ -2548,25 +2534,23 @@
 
         Returns:
             ``torch.Tensor``: A batch with
                 the product values along the batch dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
-            >>> BatchedTensor(
-            ...     torch.tensor([[1, 6], [2, 7], [3, 8], [4, 9], [5, 1]])
-            ... ).prod_along_batch()
+            >>> BatchedTensor(torch.tensor([[1, 6], [2, 7], [3, 8], [4, 9], [5, 1]])).prod_along_batch()
             tensor([ 120, 3024])
-            >>> BatchedTensor(
-            ...     torch.tensor([[1, 6], [2, 7], [3, 8], [4, 9], [5, 1]])
-            ... ).prod_along_batch(keepdim=True)
+            >>> BatchedTensor(torch.tensor([[1, 6], [2, 7], [3, 8], [4, 9], [5, 1]])).prod_along_batch(
+            ...     keepdim=True
+            ... )
             tensor([[ 120, 3024]])
         """
         return self.prod(dim=self._batch_dim, keepdim=keepdim)
 
     def sum(self, *args, **kwargs) -> Tensor:
         r"""Computes the sum of all elements.
 
@@ -2575,15 +2559,15 @@
             **kwargs: See the documentation of ``torch.Tensor.sum``
 
         Returns:
             ``torch.Tensor``: The sum of all elements.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(2, 5)).sum()
             tensor(45)
             >>> BatchedTensor(torch.arange(10).view(2, 5)).sum(dim=1)
             tensor([10, 35])
@@ -2602,15 +2586,15 @@
 
         Returns:
             ``torch.Tensor``: A tensor with the sum values along the
                 batch dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2)).sum_along_batch()
             tensor([20, 25])
         """
         return self.sum(dim=self._batch_dim, keepdim=keepdim)
@@ -2624,15 +2608,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the inverse cosine
                 (arccos) of each element.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[-1.0, 0.0, 1.0], [-0.5, 0.0, 0.5]]))
             >>> batch.acos()
             tensor([[3.1416, 1.5708, 0.0000],
                     [2.0944, 1.5708, 1.0472]], batch_dim=0)
@@ -2642,15 +2626,15 @@
     def acos_(self) -> None:
         r"""Computes the inverse cosine (arccos) of each element.
 
         In-place version of ``acos()``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[-1.0, 0.0, 1.0], [-0.5, 0.0, 0.5]]))
             >>> batch.acos_()
             >>> batch
             tensor([[-1.5708,  0.0000,  1.5708],
@@ -2664,15 +2648,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the inverse hyperbolic
                 cosine (arccosh) of each element.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[1.0, 2.0, 3.0], [4.0, 5.0, 6.0]]))
             >>> batch.acosh()
             tensor([[0.0000, 1.3170, 1.7627],
                     [2.0634, 2.2924, 2.4779]], batch_dim=0)
@@ -2685,15 +2669,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the inverse hyperbolic
                 cosine (arccosh) of each element.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[1.0, 2.0, 3.0], [4.0, 5.0, 6.0]]))
             >>> batch.acosh_()
             >>> batch
             tensor([[0.0000, 1.3170, 1.7627],
@@ -2706,15 +2690,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the inverse sine
                 (arcsin) of each element.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[-1.0, 0.0, 1.0], [-0.5, 0.0, 0.5]]))
             >>> batch.asin()
             tensor([[-1.5708,  0.0000,  1.5708],
                     [-0.5236,  0.0000,  0.5236]], batch_dim=0)
@@ -2724,15 +2708,15 @@
     def asin_(self) -> None:
         r"""Computes the inverse sine (arcsin) of each element.
 
         In-place version of ``asin()``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[-1.0, 0.0, 1.0], [-0.5, 0.0, 0.5]]))
             >>> batch.asin_()
             >>> batch
             tensor([[3.1416, 1.5708, 0.0000],
@@ -2746,15 +2730,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the inverse hyperbolic
                 sine (arcsinh) of each element.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[-1.0, 0.0, 1.0], [-0.5, 0.0, 0.5]]))
             >>> batch.asinh()
             tensor([[-0.8814,  0.0000,  0.8814],
                     [-0.4812,  0.0000,  0.4812]], batch_dim=0)
@@ -2765,15 +2749,15 @@
         r"""Computes the inverse hyperbolic sine (arcsinh) of each
         element.
 
         In-place version of ``asinh()``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[-1.0, 0.0, 1.0], [-0.5, 0.0, 0.5]]))
             >>> batch.asinh_()
             >>> batch
             tensor([[-0.8814,  0.0000,  0.8814],
@@ -2786,15 +2770,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the inverse tangent
                 of each element.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[0.0, 1.0, 2.0], [-2.0, -1.0, 0.0]]))
             >>> batch.atan()
             tensor([[ 0.0000,  0.7854,  1.1071],
                     [-1.1071, -0.7854,  0.0000]], batch_dim=0)
@@ -2804,15 +2788,15 @@
     def atan_(self) -> None:
         r"""Computes the inverse tangent of each element.
 
         In-place version of ``atan()``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[0.0, 1.0, 2.0], [-2.0, -1.0, 0.0]]))
             >>> batch.atan_()
             >>> batch
             tensor([[ 0.0000,  0.7854,  1.1071],
@@ -2825,15 +2809,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the inverse hyperbolic
                 tangent of each element.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[-0.5, 0.0, 0.5], [-0.1, 0.0, 0.1]]))
             >>> batch.atanh()
             tensor([[-0.5493,  0.0000,  0.5493],
                     [-0.1003,  0.0000,  0.1003]], batch_dim=0)
@@ -2843,15 +2827,15 @@
     def atanh_(self) -> None:
         r"""Computes the inverse hyperbolic tangent of each element.
 
         In-place version of ``atanh()``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[-0.5, 0.0, 0.5], [-0.1, 0.0, 0.1]]))
             >>> batch.atanh_()
             >>> batch
             tensor([[-0.5493,  0.0000,  0.5493],
@@ -2864,15 +2848,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the cosine of each
                 element.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> import math
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(
             ...     torch.tensor([[0.0, 0.5 * math.pi, math.pi], [2 * math.pi, 1.5 * math.pi, 0.0]])
             ... )
@@ -2885,15 +2869,15 @@
     def cos_(self) -> None:
         r"""Computes the cosine of each element.
 
         In-place version of ``cos()``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> import math
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(
             ...     torch.tensor([[0.0, 0.5 * math.pi, math.pi], [2 * math.pi, 1.5 * math.pi, 0.0]])
             ... )
@@ -2909,15 +2893,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the hyperbolic
                 cosine (arccosh) of each element.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[1.0, 2.0, 3.0], [4.0, 5.0, 6.0]]))
             >>> batch.cosh()
             tensor([[0.0000, 1.3170, 1.7627],
                     [2.0634, 2.2924, 2.4779]], batch_dim=0)
@@ -2927,15 +2911,15 @@
     def cosh_(self) -> None:
         r"""Computes the hyperbolic cosine (arccosh) of each element.
 
         In-place version of ``cosh()``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[1.0, 2.0, 3.0], [4.0, 5.0, 6.0]]))
             >>> batch.cosh_()
             >>> batch
             tensor([[0.0000, 1.3170, 1.7627],
@@ -2948,15 +2932,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the sine of each
                 element.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> import math
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(
             ...     torch.tensor([[0.0, 0.5 * math.pi, math.pi], [2 * math.pi, 1.5 * math.pi, 0.0]])
             ... )
@@ -2969,15 +2953,15 @@
     def sin_(self) -> None:
         r"""Computes the sine of each element.
 
         In-place version of ``sin()``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> import math
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(
             ...     torch.tensor([[0.0, 0.5 * math.pi, math.pi], [2 * math.pi, 1.5 * math.pi, 0.0]])
             ... )
@@ -2993,15 +2977,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the hyperbolic sine of
                 each element.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[-1.0, 0.0, 1.0], [-0.5, 0.0, 0.5]]))
             >>> batch.sinh()
             tensor([[-1.1752,  0.0000,  1.1752],
                     [-0.5211,  0.0000,  0.5211]], batch_dim=0)
@@ -3011,15 +2995,15 @@
     def sinh_(self) -> None:
         r"""Computes the hyperbolic sine of each element.
 
         In-place version of ``sinh()``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[-1.0, 0.0, 1.0], [-0.5, 0.0, 0.5]]))
             >>> batch.sinh_()
             >>> batch
             tensor([[-1.1752,  0.0000,  1.1752],
@@ -3032,25 +3016,22 @@
 
         Return:
             ``BatchedTensor``: A batch with the tangent of each
                 element.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> import math
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(
             ...     torch.tensor(
-            ...         [
-            ...             [0.0, 0.25 * math.pi, math.pi],
-            ...             [2 * math.pi, 1.75 * math.pi, -0.25 * math.pi]
-            ...         ]
+            ...         [[0.0, 0.25 * math.pi, math.pi], [2 * math.pi, 1.75 * math.pi, -0.25 * math.pi]]
             ...     )
             ... )
             >>> batch.tan()
             tensor([[ 0.0000e+00,  1.0000e+00,  8.7423e-08],
                     [ 1.7485e-07, -1.0000e+00, -1.0000e+00]], batch_dim=0)
         """
         return torch.tan(self)
@@ -3058,25 +3039,22 @@
     def tan_(self) -> None:
         r"""Computes the tangent of each element.
 
         In-place version of ``tan()``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> import math
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(
             ...     torch.tensor(
-            ...         [
-            ...             [0.0, 0.25 * math.pi, math.pi],
-            ...             [2 * math.pi, 1.75 * math.pi, -0.25 * math.pi]
-            ...         ]
+            ...         [[0.0, 0.25 * math.pi, math.pi], [2 * math.pi, 1.75 * math.pi, -0.25 * math.pi]]
             ...     )
             ... )
             >>> batch.tan_()
             >>> batch
             tensor([[ 0.0000e+00,  1.0000e+00,  8.7423e-08],
                     [ 1.7485e-07, -1.0000e+00, -1.0000e+00]], batch_dim=0)
         """
@@ -3087,15 +3065,15 @@
 
         Return:
             ``BatchedTensor``: A batch with the tangent of each
                 element.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[0.0, 1.0, 2.0], [-2.0, -1.0, 0.0]]))
             >>> batch.tanh()
             tensor([[ 0.0000,  0.7616,  0.9640],
                     [-0.9640, -0.7616,  0.0000]], batch_dim=0)
@@ -3105,15 +3083,15 @@
     def tanh_(self) -> None:
         r"""Computes the tangent of each element.
 
         In-place version of ``tanh()``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[0.0, 1.0, 2.0], [-2.0, -1.0, 0.0]]))
             >>> batch.tanh_()
             >>> batch
             tensor([[ 0.0000,  0.7616,  0.9640],
@@ -3138,15 +3116,15 @@
 
         Returns:
             ``BatchedTensor``: A batch containing the element-wise
                 logical AND.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch1 = BatchedTensor(
             ...     torch.tensor([[True, True, False, False], [True, False, True, False]])
             ... )
             >>> batch2 = BatchedTensor(
@@ -3167,15 +3145,15 @@
         Args:
             other (``BatchedTensor`` or ``torch.Tensor``):
                 Specifies the batch or tensor to compute
                 logical AND with.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch1 = BatchedTensor(
             ...     torch.tensor([[True, True, False, False], [True, False, True, False]])
             ... )
             >>> batch2 = BatchedTensor(
@@ -3197,15 +3175,15 @@
 
         Returns:
             ``BatchedTensor``: A batch containing the element-wise
                 logical NOT of the current batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(
             ...     torch.tensor([[True, True, False, False], [True, False, True, False]])
             ... )
             >>> batch.logical_not()
@@ -3218,15 +3196,15 @@
         r"""Computes the element-wise logical NOT of the current batch.
 
         Zeros are treated as ``False`` and non-zeros are treated as
         ``True``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(
             ...     torch.tensor([[True, True, False, False], [True, False, True, False]])
             ... )
             >>> batch.logical_not_()
@@ -3248,15 +3226,15 @@
 
         Returns:
             ``BatchedTensor``: A batch containing the element-wise
                 logical OR.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch1 = BatchedTensor(
             ...     torch.tensor([[True, True, False, False], [True, False, True, False]])
             ... )
             >>> batch2 = BatchedTensor(
@@ -3276,15 +3254,15 @@
 
         Args:
             other (``BatchedTensor`` or ``torch.Tensor``):
                 Specifies the batch to compute logical OR with.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch1 = BatchedTensor(
             ...     torch.tensor([[True, True, False, False], [True, False, True, False]])
             ... )
             >>> batch2 = BatchedTensor(
@@ -3310,15 +3288,15 @@
 
         Returns:
             ``BatchedTensor``: A batch containing the element-wise
                 logical XOR.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch1 = BatchedTensor(
             ...     torch.tensor([[True, True, False, False], [True, False, True, False]])
             ... )
             >>> batch2 = BatchedTensor(
@@ -3338,15 +3316,15 @@
 
         Args:
             other (``BatchedTensor`` or ``torch.Tensor``):
                 Specifies the batch to compute logical XOR with.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch1 = BatchedTensor(
             ...     torch.tensor([[True, True, False, False], [True, False, True, False]])
             ... )
             >>> batch2 = BatchedTensor(
@@ -3395,15 +3373,15 @@
 
         Returns:
             ``BatchedTensor``: A batch with the concatenated data
                 in the batch dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.tensor([[0, 1, 2], [4, 5, 6]])).cat(
             ...     BatchedTensor(torch.tensor([[10, 11, 12], [13, 14, 15]]))
             ... )
             tensor([[ 0,  1,  2],
@@ -3425,22 +3403,20 @@
 
         Args:
             tensor (``BatchedTensor`` or ``torch.Tensor`` or
                 ``Iterable``): Specifies the batch(es) to concatenate.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[0, 1, 2], [4, 5, 6]]))
-            >>> batch.cat_(
-            ...     BatchedTensor(torch.tensor([[10, 11, 12], [13, 14, 15]]))
-            ... )
+            >>> batch.cat_(BatchedTensor(torch.tensor([[10, 11, 12], [13, 14, 15]])))
             >>> batch
             tensor([[ 0,  1,  2],
                     [ 4,  5,  6],
                     [10, 11, 12],
                     [13, 14, 15]], batch_dim=0)
         """
         self._data = self.cat(tensors, dim=dim).data
@@ -3457,15 +3433,15 @@
 
         Returns:
             ``BatchedTensor``: A batch with the concatenated data
                 in the batch dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.tensor([[0, 1, 2], [4, 5, 6]])).cat_along_batch(
             ...     BatchedTensor(torch.tensor([[10, 11, 12], [13, 14, 15]]))
             ... )
             tensor([[ 0,  1,  2],
@@ -3496,22 +3472,20 @@
 
         Args:
             tensors (``BatchedTensor`` or ``torch.Tensor`` or
                 ``Iterable``): Specifies the batch(es) to concatenate.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.tensor([[0, 1, 2], [4, 5, 6]]))
-            >>> batch.cat_along_batch_(
-            ...     BatchedTensor(torch.tensor([[10, 11, 12], [13, 14, 15]]))
-            ... )
+            >>> batch.cat_along_batch_(BatchedTensor(torch.tensor([[10, 11, 12], [13, 14, 15]])))
             >>> batch
             tensor([[ 0,  1,  2],
                     [ 4,  5,  6],
                     [10, 11, 12],
                     [13, 14, 15]], batch_dim=0)
             >>> BatchedTensor(torch.tensor([[0, 4], [1, 5], [2, 6]]))
             >>> batch.cat_along_batch_(
@@ -3541,15 +3515,15 @@
 
         Returns:
             tuple: The batch split into chunks along the given
                 dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2)).chunk(chunks=3)
             (tensor([[0, 1], [2, 3]], batch_dim=0),
              tensor([[4, 5], [6, 7]], batch_dim=0),
              tensor([[8, 9]], batch_dim=0))
@@ -3573,15 +3547,15 @@
         Returns:
             ``BatchedTensor``: A new batch which indexes ``self``
                 along the batch dimension using the entries in
                 ``index``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
             >>> batch.index_select(0, [2, 4])
             tensor([[4, 5],
                     [8, 9]], batch_dim=0)
@@ -3611,15 +3585,15 @@
             value (number): Specifies the value to fill in with.
 
         Returns:
             ``BatchedTensor``: A new batch with the updated values.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(5, 2))
             >>> mask = BatchedTensor(
             ...     torch.tensor(
             ...         [
@@ -3653,15 +3627,15 @@
 
         Returns:
             ``Tensor``: The batch sliced along the batch
                 dimension at the given index.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2)).select(dim=0, index=2)
             tensor([4, 5])
         """
         return torch.select(self._data, dim=dim, index=index)
@@ -3695,15 +3669,15 @@
                 each index for slicing. Default: ``1``
 
         Returns:
             ``BatchedTensor``: A slice of the current batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2)).slice_along_dim(start=2)
             tensor([[4, 5],
                     [6, 7],
                     [8, 9]], batch_dim=0)
@@ -3737,15 +3711,15 @@
 
         Returns:
             tuple: The batch split into chunks along the given
                 dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2)).split(2, dim=0)
             (tensor([[0, 1], [2, 3]], batch_dim=0),
              tensor([[4, 5], [6, 7]], batch_dim=0),
              tensor([[8, 9]], batch_dim=0))
@@ -3768,15 +3742,15 @@
                 dimension.
 
         Returns:
             ``BaseBatch``: The batch with the selected data.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2)).take_along_batch(
             ...     BatchedTensor(torch.tensor([[3, 2], [0, 3], [1, 4]]))
             ... )
             tensor([[6, 5],
@@ -3798,15 +3772,15 @@
                 dimension.
 
         Returns:
             ``BaseBatch``: The batch with the selected data.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2)).take_along_dim(
             ...     BatchedTensor(torch.tensor([[3, 2], [0, 3], [1, 4]])), dim=0
             ... )
             tensor([[6, 5],
@@ -3830,15 +3804,15 @@
 
         Returns:
             ``BatchedTensor``: A new batch with an added singleton
                 dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.ones(2, 3)).unsqueeze(dim=0)
             tensor([[[1., 1., 1.],
                     [1., 1., 1.]]], batch_dim=1)
             >>> BatchedTensor(torch.ones(2, 3)).unsqueeze(dim=1)
@@ -3867,15 +3841,15 @@
             shape (tuple): Specifies the desired shape.
 
         Retunrs:
             ``torch.Tensor``: A new view of the tensor in the batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.ones(2, 6)).view(2, 3, 2)
             tensor([[[1., 1.],
                      [1., 1.],
                      [1., 1.]],
@@ -3899,15 +3873,15 @@
 
         Returns:
             ``BatchedTensor``: A new batch with the shape of
                 ``other``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch1 = BatchedTensor(torch.arange(10).view(2, 5))
             >>> batch2 = BatchedTensor(torch.zeros(2, 5, 1))
             >>> batch1.view_as(batch2)
             tensor([[[0],
@@ -3943,15 +3917,15 @@
                 the data.
 
         Returns:
             ``BatchedTensor``: The transformed batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
             >>> batch.apply(lambda tensor: tensor + 2)
             tensor([[ 2,  3,  4,  5,  6],
                     [ 7,  8,  9, 10, 11]], batch_dim=0)
@@ -3971,15 +3945,15 @@
                 the data.
 
         Returns:
             ``BatchedTensor``: The transformed batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
             >>> batch.apply_(lambda tensor: tensor + 2)
             >>> batch
             tensor([[ 2,  3,  4,  5,  6],
```

### Comparing `redcat-0.0.3/src/redcat/tensorseq.py` & `redcat-0.0.4/src/redcat/tensorseq.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
                 ``torch.Tensor.new_full``.
 
         Returns:
             ``BaseBatchedTensor``: A batch filled with the scalar value.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> batch = BatchedTensorSeq(torch.ones(2, 3))
             >>> batch.new_full(42)
             tensor([[42., 42., 42.],
                     [42., 42., 42.]], batch_dim=0, seq_dim=1)
@@ -175,15 +175,15 @@
 
         Returns:
             ``BaseBatchedTensor``: A batch filled with the scalar
                 value ``1``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> batch = BatchedTensorSeq(torch.zeros(2, 3))
             >>> batch.new_ones()
             tensor([[1., 1., 1.],
                     [1., 1., 1.]], batch_dim=0, seq_dim=1)
@@ -230,15 +230,15 @@
 
         Returns:
             ``BaseBatchedTensor``: A batch filled with the scalar
                 value ``0``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> batch = BatchedTensorSeq(torch.ones(2, 3))
             >>> batch.new_zeros()
             tensor([[0., 0., 0.],
                     [0., 0., 0.]], batch_dim=0, seq_dim=1)
@@ -271,15 +271,15 @@
                 be a torch.Tensor, list, tuple, NumPy ndarray, scalar,
                 and other types.
             kwargs: Keyword arguments that are passed to
                 ``torch.as_tensor``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq.from_seq_batch(torch.ones(2, 3))
             tensor([[1., 1., 1.],
                     [1., 1., 1.]], batch_dim=1, seq_dim=0)
         """
@@ -356,15 +356,15 @@
 
         Returns:
             ``BatchedTensorSeq``: A batch with the cumulative sum of
                 elements of the current batch in the sequence dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5)).cumsum_along_seq()
             >>> batch
             tensor([[ 0,  1,  3,  6, 10],
                     [ 5, 11, 18, 26, 35]], batch_dim=0, seq_dim=1)
@@ -373,15 +373,15 @@
 
     def cumsum_along_seq_(self) -> None:
         r"""Computes the cumulative sum of elements of the current batch
         in the sequence dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
             >>> batch.cumsum_along_seq_()
             >>> batch
             tensor([[ 0,  1,  3,  6, 10],
@@ -397,15 +397,15 @@
         Returns:
             ``BatchedTensorSeq``: A batch with the cumulative
                 summation of the exponentiation of elements of the
                 current batch in the sequence dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.arange(10).view(2, 5).float()).logcumsumexp_along_seq()
             tensor([[0.0000, 1.3133, 2.4076, 3.4402, 4.4519],
                     [5.0000, 6.3133, 7.4076, 8.4402, 9.4519]], batch_dim=0, seq_dim=1)
         """
@@ -414,15 +414,15 @@
     def logcumsumexp_along_seq_(self) -> None:
         r"""Computes the logarithm of the cumulative summation of the
         exponentiation of elements of the current batch in the sequence
         dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5).float())
             >>> batch.logcumsumexp_along_seq_()
             >>> batch
             tensor([[0.0000, 1.3133, 2.4076, 3.4402, 4.4519],
@@ -440,15 +440,15 @@
                 input should be compatible with the shape of the data.
 
         Returns:
             ``BatchedTensorSeq``: A new batch with permuted data.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
             >>> batch.permute_along_seq([2, 1, 3, 0, 4])
             tensor([[2, 1, 3, 0, 4],
                     [7, 6, 8, 5, 9]], batch_dim=0, seq_dim=1)
@@ -462,15 +462,15 @@
             permutation (sequence or ``torch.Tensor`` of type long
                 and shape ``(dimension,)``): Specifies the permutation
                 to use on the data. The dimension of the permutation
                 input should be compatible with the shape of the data.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
             >>> batch.permute_along_seq_([2, 1, 3, 0, 4])
             >>> batch
             tensor([[2, 1, 3, 0, 4],
@@ -487,15 +487,15 @@
                 Default: ``None``
 
         Returns:
             ``BatchedTensorSeq``:  A new batch with shuffled data.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).shuffle_along_seq()
             tensor([[2, 1, 4, 0, 3],
                     [7, 6, 9, 5, 8]], batch_dim=0, seq_dim=1)
         """
@@ -507,15 +507,15 @@
         Args:
             generator (``torch.Generator`` or ``None``, optional):
                 Specifies an optional random generator.
                 Default: ``None``
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
             >>> batch.shuffle_along_seq_()
             >>> batch
             tensor([[2, 1, 4, 0, 3],
@@ -543,15 +543,15 @@
                     - The first batch contains the batch values sorted
                         along the sequence dimension.
                     - The second batch contains the indices that sort
                         the batch along the sequence dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.rand(2, 5)).sort_along_seq()
             torch.return_types.sort(
             values=tensor([[0.2884, 0.4014, 0.5857, 0.6949, 0.8264],
                     [0.3811, 0.4431, 0.4857, 0.6009, 0.7207]], batch_dim=0, seq_dim=1),
@@ -598,15 +598,15 @@
 
         Returns:
             ``torch.return_types.max``: A batch with
                 the maximum values along the sequence dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).max_along_seq()
             torch.return_types.max(
             values=tensor([4, 9]),
             indices=tensor([4, 4]))
@@ -628,15 +628,15 @@
 
         Returns:
             ``BatchedTensor`` or ``BatchedTensorSeq``: A batch with
                 the mean values along the sequence dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.arange(10).view(2, 5).float()).mean_along_seq()
             tensor([2.0, 7.0])
             >>> BatchedTensorSeq(torch.arange(10).view(2, 5).float()).mean_along_seq(keepdim=True)
             tensor([[2.0], [7.0]])
@@ -655,15 +655,15 @@
             ``torch.return_types.median``:  The first tensor will
                 be populated with the median values and the second
                 tensor, which must have dtype long, with their indices
                 in the sequence dimension of input.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).median_along_seq()
             torch.return_types.median(
             values=tensor([2, 7]),
             indices=tensor([2, 2]))
@@ -680,15 +680,15 @@
 
         Returns:
             ``torch.return_types.min``: A batch with
                 the minimum values along the sequence dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).min_along_seq()
             torch.return_types.min(
             values=tensor([0, 5]),
             indices=tensor([0, 0]))
@@ -709,15 +709,15 @@
 
         Returns:
             ``torch.Tensor``: A batch with
                 the mean values along the sequence dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(
             ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
             ... ).nanmean_along_seq()
             tensor([2.0, 6.5])
@@ -740,15 +740,15 @@
             ``torch.return_types.nanmedian``:  The first tensor will
                 be populated with the median values and the second
                 tensor, which must have dtype long, with their indices
                 in the sequence dimension of input.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(
             ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
             ... ).nanmedian_along_seq()
             torch.return_types.nanmedian(
@@ -767,15 +767,15 @@
 
         Returns:
             ``torch.Tensor``: A tensor with the sum values along the
                 sequence dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(
             ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
             ... ).nansum_along_seq()
             tensor([20., 26.])
@@ -792,23 +792,23 @@
 
         Returns:
             ``torch.Tensor``: A batch with
                 the product values along the sequence dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])).prod_along_seq()
             tensor([ 120, 3024])
-            >>> BatchedTensorSeq(
-            ...     torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])
-            ... ).prod_along_seq(keepdim=True)
+            >>> BatchedTensorSeq(torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])).prod_along_seq(
+            ...     keepdim=True
+            ... )
             tensor([[ 120], [3024]])
         """
         return self.prod(dim=self._seq_dim, keepdim=keepdim)
 
     def sum_along_seq(self, keepdim: bool = False) -> Tensor:
         r"""Computes the sum values along the sequence dimension.
 
@@ -820,15 +820,15 @@
 
         Returns:
             ``torch.Tensor``: A tensor with the sum values along the
                 sequence dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).sum_along_seq()
             tensor([10, 35])
         """
         return self.sum(dim=self._seq_dim, keepdim=keepdim)
@@ -848,15 +848,15 @@
                 align the current batch.
 
         Returns:
             ``BatchedTensorSeq``: The aligned batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             # batch-sequence -> sequence-batch
             >>> seq_batch = BatchedTensorSeq(torch.ones(2, 3), batch_dim=1, seq_dim=0)
             >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).align_as(seq_batch)
             tensor([[0, 5],
@@ -896,15 +896,15 @@
 
         Returns:
             ``BatchedTensorSeq``: The batch in the batch-sequence
                 format.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> batch = BatchedTensorSeq(torch.arange(10).view(5, 2), batch_dim=1, seq_dim=0)
             >>> batch.align_to_batch_seq()
             tensor([[0, 2, 4, 6, 8],
                     [1, 3, 5, 7, 9]], batch_dim=0, seq_dim=1)
@@ -919,15 +919,15 @@
         r"""Aligns the current batch to the sequence-batch format.
 
         Returns:
             ``BatchedTensorSeq``: The batch in the sequence-batch format.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5), batch_dim=0, seq_dim=1)
             >>> batch.align_to_seq_batch()
             tensor([[0, 5],
                     [1, 6],
@@ -953,25 +953,27 @@
 
         Returns:
             ``BatchedTensorSeq``: A batch with the concatenated data
                 along the sequence dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.tensor([[0, 1, 2], [4, 5, 6]])).cat_along_seq(
             ...     BatchedTensorSeq(torch.tensor([[10, 11], [12, 13]]))
             ... )
             tensor([[ 0,  1,  2, 10, 11],
                     [ 4,  5,  6, 12, 13]], batch_dim=0, seq_dim=1)
             >>> BatchedTensorSeq(
-            ...     torch.tensor([[0, 4], [1, 5], [2, 6]]), batch_dim=1, seq_dim=0,
+            ...     torch.tensor([[0, 4], [1, 5], [2, 6]]),
+            ...     batch_dim=1,
+            ...     seq_dim=0,
             ... ).cat_along_seq(
             ...     [
             ...         BatchedTensorSeq(torch.tensor([[10, 12], [11, 13]]), batch_dim=1, seq_dim=0),
             ...         BatchedTensorSeq(torch.tensor([[20, 22], [21, 23]]), batch_dim=1, seq_dim=0),
             ...     ]
             ... )
             tensor([[ 0,  4],
@@ -994,27 +996,27 @@
 
         Args:
             tensors (``BatchedTensor`` or ``torch.Tensor`` or
                 ``Iterable``): Specifies the batch(es) to concatenate.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> batch = BatchedTensorSeq(torch.tensor([[0, 1, 2], [4, 5, 6]]))
-            >>> batch.cat_along_seq_(
-            ...     BatchedTensorSeq(torch.tensor([[10, 11], [12, 13]]))
-            ... )
+            >>> batch.cat_along_seq_(BatchedTensorSeq(torch.tensor([[10, 11], [12, 13]])))
             >>> batch
             tensor([[ 0,  1,  2, 10, 11],
                     [ 4,  5,  6, 12, 13]], batch_dim=0, seq_dim=1)
             >>> batch = BatchedTensorSeq(
-            ...     torch.tensor([[0, 4], [1, 5], [2, 6]]), batch_dim=1, seq_dim=0,
+            ...     torch.tensor([[0, 4], [1, 5], [2, 6]]),
+            ...     batch_dim=1,
+            ...     seq_dim=0,
             ... )
             >>> batch.cat_along_seq(
             ...     [
             ...         BatchedTensorSeq(torch.tensor([[10, 12], [11, 13]]), batch_dim=1, seq_dim=0),
             ...         BatchedTensorSeq(torch.tensor([[20, 22], [21, 23]]), batch_dim=1, seq_dim=0),
             ...     ]
             ... )
@@ -1037,15 +1039,15 @@
 
         Returns:
             tuple: The batch split into chunks along the sequence
                 dimension.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).chunk_along_seq(chunks=3)
             (tensor([[0, 1], [5, 6]], batch_dim=0, seq_dim=1),
              tensor([[2, 3], [7, 8]], batch_dim=0, seq_dim=1),
              tensor([[4], [9]], batch_dim=0, seq_dim=1))
@@ -1062,15 +1064,15 @@
 
         Returns:
             ``BatchedTensorSeq``: A new batch sliced along the sequence
                 dimension at the given indices.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> batch = BatchedTensorSeq(torch.arange(10).view(2, 5))
             >>> batch.index_select_along_seq([2, 4])
             tensor([[2, 4],
                     [7, 9]], batch_dim=0, seq_dim=1)
@@ -1097,15 +1099,15 @@
                 the batch along the sequence dimension.
 
         Returns:
             ``BatchedTensorSeq``: A repeated version of the input batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).repeat_along_seq(2)
             tensor([[0, 1, 2, 3, 4, 0, 1, 2, 3, 4],
                     [5, 6, 7, 8, 9, 5, 6, 7, 8, 9]], batch_dim=0, seq_dim=1)
         """
@@ -1122,15 +1124,15 @@
 
         Returns:
             ``BatchedTensorSeq``: The batch sliced along the sequence
                 dimension at the given index.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).select_along_seq(2)
             tensor([2, 7], batch_dim=0)
         """
         return BatchedTensor(
@@ -1153,15 +1155,15 @@
                 each index for slicing. Default: ``1``
 
         Returns:
             ``BatchedTensorSeq``: A slice of the current batch.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> batch = BatchedTensorSeq(torch.tensor([[0, 1, 2, 3, 4], [9, 8, 7, 6, 5]]))
             >>> batch.slice_along_seq(start=2)
             tensor([[2, 3, 4],
                     [7, 6, 5]], batch_dim=0, seq_dim=1)
@@ -1188,15 +1190,15 @@
                 dimension.
 
         Returns:
             ``BaseBatch``: The sequence with the selected data.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).take_along_seq(
             ...     BatchedTensorSeq(torch.tensor([[3, 0, 1], [2, 3, 4]]))
             ... )
             tensor([[3, 0, 1],
@@ -1433,15 +1435,15 @@
     Returns:
         ``BatchedTensorSeq``: A padded tensor. The underlying data is
             a ``torch.Tensor`` of shape
             ``(batch_size, sequence_length, *)``.
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> import torch
         >>> import redcat
         >>> redcat.tensorseq.from_sequences(
         ...     [torch.ones(3), torch.ones(5), torch.ones(1), torch.ones(0)]
         ... )
         tensor([[1., 1., 1., 0., 0.],
```

### Comparing `redcat-0.0.3/src/redcat/utils/format.py` & `redcat-0.0.4/src/redcat/utils/format.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
     Returns:
     -------
         str: The string representation of the mapping.
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from redcat.utils.format import str_mapping
-        >>> str_mapping({'key1': 'abc', 'key2': 'something\nelse'})
+        >>> str_mapping({"key1": "abc", "key2": "something\nelse"})
         (key1) abc
         (key2) something
           else
     """
     lines = []
     for key, value in sorted(mapping.items()) if sorted_keys else mapping.items():
         lines.append(f"({key}) {str_indent(value, num_spaces=num_spaces)}")
```

### Comparing `redcat-0.0.3/src/redcat/utils/imports.py` & `redcat-0.0.4/src/redcat/utils/imports.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.3/src/redcat/utils/tensor.py` & `redcat-0.0.4/src/redcat/utils/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     Returns:
         ``torch.Tensor``: A tensor of shape ``(batch_size, *)`` where
             `*` means any number of dimensions.
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> import torch
         >>> from redcat.utils.tensor import align_to_batch_first
         >>> align_to_batch_first(torch.arange(20).view(4, 5), batch_dim=1)
         tensor([[ 0,  5, 10, 15],
                 [ 1,  6, 11, 16],
                 [ 2,  7, 12, 17],
@@ -130,15 +130,15 @@
 
     Returns:
         list: The permutation to update the batch and sequence
             dimensions.
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from redcat.utils.tensor import compute_batch_seq_permutation
         >>> compute_batch_seq_permutation(5, 0, 1, 1, 0)
         [1, 0, 2, 3, 4]
         >>> compute_batch_seq_permutation(2, 0, 1, 1, 0)
         [1, 0]
         >>> compute_batch_seq_permutation(5, 0, 1, 2, 0)
@@ -172,15 +172,15 @@
 
     Returns
     -------
         tuple: The available devices.
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from redcat.utils.tensor import get_available_devices
         >>> get_available_devices()
         ('cpu', 'cuda:0')
     """
     if torch.cuda.is_available():
         return ("cpu", "cuda:0")
@@ -204,15 +204,15 @@
 
     Returns:
     -------
         ``torch.Generator``
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> import torch
         >>> from redcat.utils.tensor import get_torch_generator
         >>> generator = get_torch_generator(42)
         >>> torch.rand(2, 4, generator=generator)
         tensor([[0.8823, 0.9150, 0.3829, 0.9593],
                 [0.3904, 0.6009, 0.2566, 0.7936]])
@@ -241,15 +241,15 @@
 
     Returns:
     -------
         ``torch.Tensor``: The permuted tensor.
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from redcat.utils.tensor import permute_along_dim
         >>> permute_along_dim(tensor=torch.arange(4), permutation=torch.tensor([0, 2, 1, 3]))
         tensor([0, 2, 1, 3])
         >>> permute_along_dim(
         ...     tensor=torch.arange(20).view(4, 5),
         ...     permutation=torch.tensor([0, 2, 1, 3]),
@@ -305,15 +305,15 @@
 
     Returns:
         ``torch.Tensor`` or ``numpy.ndarray`` or ``MutableSequence``:
             The updated sequence.
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from redcat.utils.tensor import swap2
         >>> seq = [1, 2, 3, 4, 5]
         >>> swap2(seq, 2, 0)
         >>> seq
         [3, 2, 1, 4, 5]
     """
```

### Comparing `redcat-0.0.3/PKG-INFO` & `redcat-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redcat
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library to manipulate batches of examples
 Home-page: https://github.com/durandtibo/redcat
 License: BSD-3-Clause
 Keywords: batch
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: redcat Version: 0.0.3 Summary: A library to
+Metadata-Version: 2.1 Name: redcat Version: 0.0.4 Summary: A library to
 manipulate batches of examples Home-page: https://github.com/durandtibo/redcat
 License: BSD-3-Clause Keywords: batch Author: Thibaut Durand Author-email:
 durand.tibo+gh@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
```

