# Comparing `tmp/redcat-0.0.4.tar.gz` & `tmp/redcat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redcat-0.0.4.tar", max compression
+gzip compressed data, was "redcat-0.0.5.tar", max compression
```

## Comparing `redcat-0.0.4.tar` & `redcat-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1501 2023-05-27 03:49:08.506193 redcat-0.0.4/LICENSE
--rw-r--r--   0        0        0     2156 2023-05-27 03:49:08.506193 redcat-0.0.4/README.md
--rw-r--r--   0        0        0     4407 2023-05-27 03:49:08.506193 redcat-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      354 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/__init__.py
--rw-r--r--   0        0        0    17482 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/base.py
--rw-r--r--   0        0        0    17123 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/batchdict.py
--rw-r--r--   0        0        0     6624 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/batchlist.py
--rw-r--r--   0        0        0     2428 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/comparators.py
--rw-r--r--   0        0        0        0 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/datapipes/__init__.py
--rw-r--r--   0        0        0      315 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/datapipes/iter/__init__.py
--rw-r--r--   0        0        0     4086 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/datapipes/iter/batching.py
--rw-r--r--   0        0        0     3728 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/datapipes/iter/joining.py
--rw-r--r--   0        0        0     2122 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/datapipes/iter/shuffling.py
--rw-r--r--   0        0        0   140310 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/tensor.py
--rw-r--r--   0        0        0    52673 2023-05-27 03:49:08.506193 redcat-0.0.4/src/redcat/tensorseq.py
--rw-r--r--   0        0        0        0 2023-05-27 03:49:08.510193 redcat-0.0.4/src/redcat/utils/__init__.py
--rw-r--r--   0        0        0     1128 2023-05-27 03:49:08.510193 redcat-0.0.4/src/redcat/utils/format.py
--rw-r--r--   0        0        0     1446 2023-05-27 03:49:08.510193 redcat-0.0.4/src/redcat/utils/imports.py
--rw-r--r--   0        0        0    10148 2023-05-27 03:49:08.510193 redcat-0.0.4/src/redcat/utils/tensor.py
--rw-r--r--   0        0        0     3380 1970-01-01 00:00:00.000000 redcat-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-05-27 20:07:39.776622 redcat-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2156 2023-05-27 20:07:39.776622 redcat-0.0.5/README.md
+-rw-r--r--   0        0        0     4407 2023-05-27 20:07:39.776622 redcat-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      354 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/__init__.py
+-rw-r--r--   0        0        0    18034 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/base.py
+-rw-r--r--   0        0        0    17391 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/batchdict.py
+-rw-r--r--   0        0        0     6733 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/batchlist.py
+-rw-r--r--   0        0        0     2428 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/comparators.py
+-rw-r--r--   0        0        0        0 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/datapipes/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/datapipes/iter/__init__.py
+-rw-r--r--   0        0        0     4086 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/datapipes/iter/batching.py
+-rw-r--r--   0        0        0     3728 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/datapipes/iter/joining.py
+-rw-r--r--   0        0        0     2122 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/datapipes/iter/shuffling.py
+-rw-r--r--   0        0        0   140507 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/tensor.py
+-rw-r--r--   0        0        0    52673 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/tensorseq.py
+-rw-r--r--   0        0        0        0 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/utils/__init__.py
+-rw-r--r--   0        0        0     1128 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/utils/format.py
+-rw-r--r--   0        0        0     1446 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/utils/imports.py
+-rw-r--r--   0        0        0    10148 2023-05-27 20:07:39.776622 redcat-0.0.5/src/redcat/utils/tensor.py
+-rw-r--r--   0        0        0     3380 1970-01-01 00:00:00.000000 redcat-0.0.5/PKG-INFO
```

### Comparing `redcat-0.0.4/LICENSE` & `redcat-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `redcat-0.0.4/README.md` & `redcat-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `redcat-0.0.4/pyproject.toml` & `redcat-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redcat"
-version = "0.0.4"
+version = "0.0.5"
 description = "A library to manipulate batches of examples"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/redcat"
 repository = "https://github.com/durandtibo/redcat"
 keywords = ["batch"]
 license = "BSD-3-Clause"
```

### Comparing `redcat-0.0.4/src/redcat/base.py` & `redcat-0.0.5/src/redcat/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -518,7 +518,28 @@
         if deepcopy:
             batch = batch.clone()
         if drop_last:
             batch = self.slice_along_batch(
                 stop=int(self.get_num_minibatches(batch_size, drop_last) * batch_size)
             )
         return batch.split_along_batch(batch_size)
+
+    #################
+    #     Other     #
+    #################
+
+    @abstractmethod
+    def summary(self) -> str:
+        r"""Returns a summary of the current batch.
+
+        Returns:
+            str: The summary of the current batch
+
+        Example usage:
+
+        .. code-block:: pycon
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(torch.arange(20).view(10, 2)).summary()
+            'BatchedTensor(dtype=torch.int64, shape=torch.Size([2, 5]), device=cpu, batch_dim=0)'
+        """
```

### Comparing `redcat-0.0.4/src/redcat/batchdict.py` & `redcat-0.0.5/src/redcat/batchdict.py`

 * *Files 2% similar despite different names*

```diff
@@ -434,14 +434,22 @@
             batches.append(self.__class__({key: value for key, value in zip(keys, values)}))
         return tuple(batches)
 
     ########################
     #     mini-batches     #
     ########################
 
+    #################
+    #     Other     #
+    #################
+
+    def summary(self) -> str:
+        data_str = str_mapping({key: value.summary() for key, value in self._data.items()})
+        return f"{self.__class__.__qualname__}(\n  {str_indent(data_str)}\n)"
+
 
 def check_same_batch_size(data: dict[Hashable, BaseBatch]) -> None:
     r"""Checks if the all the batches in a group have the same batch
     size.
 
     Args:
         group (``BaseBatch`` or dict or sequence): Specifies the group
```

### Comparing `redcat-0.0.4/src/redcat/batchlist.py` & `redcat-0.0.5/src/redcat/batchlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,9 +190,12 @@
             >>> batch = BatchList([1, 2, 3])
             >>> batch.apply_(lambda val: val + 2)
             >>> batch
             BatchList(data=[3, 4, 5])
         """
         self._data = [fn(val) for val in self._data]
 
+    def summary(self) -> str:
+        return f"{self.__class__.__qualname__}(batch_size={self.batch_size})"
+
     def _create_new_batch(self, data: list[T]) -> TBatchList:
         return self.__class__(data)
```

### Comparing `redcat-0.0.4/src/redcat/comparators.py` & `redcat-0.0.5/src/redcat/comparators.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.4/src/redcat/datapipes/iter/batching.py` & `redcat-0.0.5/src/redcat/datapipes/iter/batching.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.4/src/redcat/datapipes/iter/joining.py` & `redcat-0.0.5/src/redcat/datapipes/iter/joining.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.4/src/redcat/datapipes/iter/shuffling.py` & `redcat-0.0.5/src/redcat/datapipes/iter/shuffling.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.4/src/redcat/tensor.py` & `redcat-0.0.5/src/redcat/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -3928,43 +3928,47 @@
             >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
             >>> batch.apply(lambda tensor: tensor + 2)
             tensor([[ 2,  3,  4,  5,  6],
                     [ 7,  8,  9, 10, 11]], batch_dim=0)
         """
         return self._create_new_batch(fn(self._data))
 
-    def apply_(self, fn: Callable[[Tensor], Tensor]) -> TBatchedTensor:
+    def apply_(self, fn: Callable[[Tensor], Tensor]) -> None:
         r"""Apply a function to transform the tensor of the current
         batch.
 
         In-place version of ``apply``.
 
         Args:
             fn (``Callable``): Specifies the function to be applied to
                 the tensor. It is the responsibility of the user to
                 verify the function applies a valid transformation of
                 the data.
 
-        Returns:
-            ``BatchedTensor``: The transformed batch.
-
         Example usage:
 
         .. code-block:: pycon
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(10).view(2, 5))
             >>> batch.apply_(lambda tensor: tensor + 2)
             >>> batch
             tensor([[ 2,  3,  4,  5,  6],
                     [ 7,  8,  9, 10, 11]], batch_dim=0)
         """
         self._data = fn(self._data)
 
+    def summary(self) -> str:
+        dims = ", ".join([f"{key}={value}" for key, value in self._get_kwargs().items()])
+        return (
+            f"{self.__class__.__qualname__}(dtype={self.dtype}, shape={self.shape}, "
+            f"device={self.device}, {dims})"
+        )
+
     def _create_new_batch(self, data: Tensor) -> TBatchedTensor:
         return self.__class__(data, **self._get_kwargs())
 
     def _get_kwargs(self) -> dict:
         return {"batch_dim": self._batch_dim}
```

### Comparing `redcat-0.0.4/src/redcat/tensorseq.py` & `redcat-0.0.5/src/redcat/tensorseq.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.4/src/redcat/utils/format.py` & `redcat-0.0.5/src/redcat/utils/format.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.4/src/redcat/utils/imports.py` & `redcat-0.0.5/src/redcat/utils/imports.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.4/src/redcat/utils/tensor.py` & `redcat-0.0.5/src/redcat/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.4/PKG-INFO` & `redcat-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redcat
-Version: 0.0.4
+Version: 0.0.5
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
-Metadata-Version: 2.1 Name: redcat Version: 0.0.4 Summary: A library to
+Metadata-Version: 2.1 Name: redcat Version: 0.0.5 Summary: A library to
 manipulate batches of examples Home-page: https://github.com/durandtibo/redcat
 License: BSD-3-Clause Keywords: batch Author: Thibaut Durand Author-email:
 durand.tibo+gh@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
```

